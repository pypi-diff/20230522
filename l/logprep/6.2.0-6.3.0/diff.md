# Comparing `tmp/logprep-6.2.0.tar.gz` & `tmp/logprep-6.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "logprep-6.2.0.tar", last modified: Wed May 10 09:21:31 2023, max compression
+gzip compressed data, was "logprep-6.3.0.tar", last modified: Mon May 22 10:47:03 2023, max compression
```

## Comparing `logprep-6.2.0.tar` & `logprep-6.3.0.tar`

### file list

```diff
@@ -1,536 +1,536 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 09:21:31.976516 logprep-6.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)    26526 2023-05-10 09:21:25.000000 logprep-6.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-05-10 09:21:25.000000 logprep-6.2.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    17607 2023-05-10 09:21:31.976516 logprep-6.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    16888 2023-05-10 09:21:25.000000 logprep-6.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 09:21:31.976516 logprep-6.2.0/logprep/
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-05-10 09:21:25.000000 logprep-6.2.0/logprep/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-05-10 09:21:31.976516 logprep-6.2.0/logprep/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 09:21:31.928516 logprep-6.2.0/logprep/abc/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 09:21:25.000000 logprep-6.2.0/logprep/abc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2721 2023-05-10 09:21:25.000000 logprep-6.2.0/logprep/abc/component.py
--rw-r--r--   0 runner    (1001) docker     (123)     2097 2023-05-10 09:21:25.000000 logprep-6.2.0/logprep/abc/connector.py
--rw-r--r--   0 runner    (1001) docker     (123)     3741 2023-05-10 09:21:25.000000 logprep-6.2.0/logprep/abc/getter.py
--rw-r--r--   0 runner    (1001) docker     (123)    16580 2023-05-10 09:21:25.000000 logprep-6.2.0/logprep/abc/input.py
--rw-r--r--   0 runner    (1001) docker     (123)     2817 2023-05-10 09:21:25.000000 logprep-6.2.0/logprep/abc/output.py
--rw-r--r--   0 runner    (1001) docker     (123)    12024 2023-05-10 09:21:25.000000 logprep-6.2.0/logprep/abc/processor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1821 2023-05-10 09:21:25.000000 logprep-6.2.0/logprep/configuration.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 09:21:31.928516 logprep-6.2.0/logprep/connector/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 09:21:25.000000 logprep-6.2.0/logprep/connector/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 09:21:31.932516 logprep-6.2.0/logprep/connector/confluent_kafka/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 09:21:25.000000 logprep-6.2.0/logprep/connector/confluent_kafka/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12736 2023-05-10 09:21:25.000000 logprep-6.2.0/logprep/connector/confluent_kafka/input.py
--rw-r--r--   0 runner    (1001) docker     (123)     8002 2023-05-10 09:21:25.000000 logprep-6.2.0/logprep/connector/confluent_kafka/output.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 09:21:31.932516 logprep-6.2.0/logprep/connector/console/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 09:21:25.000000 logprep-6.2.0/logprep/connector/console/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      978 2023-05-10 09:21:25.000000 logprep-6.2.0/logprep/connector/console/output.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 09:21:31.932516 logprep-6.2.0/logprep/connector/dummy/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 09:21:25.000000 logprep-6.2.0/logprep/connector/dummy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1406 2023-05-10 09:21:25.000000 logprep-6.2.0/logprep/connector/dummy/input.py
--rw-r--r--   0 runner    (1001) docker     (123)     2722 2023-05-10 09:21:25.000000 logprep-6.2.0/logprep/connector/dummy/output.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 09:21:31.932516 logprep-6.2.0/logprep/connector/elasticsearch/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 09:21:25.000000 logprep-6.2.0/logprep/connector/elasticsearch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13487 2023-05-10 09:21:25.000000 logprep-6.2.0/logprep/connector/elasticsearch/output.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 09:21:31.932516 logprep-6.2.0/logprep/connector/file/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 09:21:25.000000 logprep-6.2.0/logprep/connector/file/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13765 2023-05-10 09:21:25.000000 logprep-6.2.0/logprep/connector/file/input.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 09:21:31.932516 logprep-6.2.0/logprep/connector/http/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 09:21:25.000000 logprep-6.2.0/logprep/connector/http/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5788 2023-05-10 09:21:25.000000 logprep-6.2.0/logprep/connector/http/input.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 09:21:31.932516 logprep-6.2.0/logprep/connector/json/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 09:21:25.000000 logprep-6.2.0/logprep/connector/json/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-05-10 09:21:25.000000 logprep-6.2.0/logprep/connector/json/input.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 09:21:31.932516 logprep-6.2.0/logprep/connector/jsonl/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 09:21:25.000000 logprep-6.2.0/logprep/connector/jsonl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      798 2023-05-10 09:21:25.000000 logprep-6.2.0/logprep/connector/jsonl/input.py
--rw-r--r--   0 runner    (1001) docker     (123)     3164 2023-05-10 09:21:25.000000 logprep-6.2.0/logprep/connector/jsonl/output.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 09:21:31.932516 logprep-6.2.0/logprep/connector/opensearch/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 09:21:25.000000 logprep-6.2.0/logprep/connector/opensearch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2372 2023-05-10 09:21:25.000000 logprep-6.2.0/logprep/connector/opensearch/output.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 09:21:31.932516 logprep-6.2.0/logprep/connector/s3/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 09:21:25.000000 logprep-6.2.0/logprep/connector/s3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11805 2023-05-10 09:21:25.000000 logprep-6.2.0/logprep/connector/s3/output.py
--rw-r--r--   0 runner    (1001) docker     (123)     2057 2023-05-10 09:21:25.000000 logprep-6.2.0/logprep/factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     1194 2023-05-10 09:21:25.000000 logprep-6.2.0/logprep/factory_error.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 09:21:31.932516 logprep-6.2.0/logprep/filter/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 09:21:25.000000 logprep-6.2.0/logprep/filter/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 09:21:31.932516 logprep-6.2.0/logprep/filter/expression/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 09:21:25.000000 logprep-6.2.0/logprep/filter/expression/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11681 2023-05-10 09:21:25.000000 logprep-6.2.0/logprep/filter/expression/filter_expression.py
--rw-r--r--   0 runner    (1001) docker     (123)    14986 2023-05-10 09:21:25.000000 logprep-6.2.0/logprep/filter/lucene_filter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 09:21:31.932516 logprep-6.2.0/logprep/framework/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 09:21:25.000000 logprep-6.2.0/logprep/framework/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19708 2023-05-10 09:21:25.000000 logprep-6.2.0/logprep/framework/pipeline.py
--rw-r--r--   0 runner    (1001) docker     (123)     4546 2023-05-10 09:21:25.000000 logprep-6.2.0/logprep/framework/pipeline_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 09:21:31.932516 logprep-6.2.0/logprep/framework/rule_tree/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 09:21:25.000000 logprep-6.2.0/logprep/framework/rule_tree/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3300 2023-05-10 09:21:25.000000 logprep-6.2.0/logprep/framework/rule_tree/node.py
--rw-r--r--   0 runner    (1001) docker     (123)    22708 2023-05-10 09:21:25.000000 logprep-6.2.0/logprep/framework/rule_tree/rule_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     9886 2023-05-10 09:21:25.000000 logprep-6.2.0/logprep/framework/rule_tree/rule_tree.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 09:21:31.932516 logprep-6.2.0/logprep/metrics/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 09:21:25.000000 logprep-6.2.0/logprep/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3450 2023-05-10 09:21:25.000000 logprep-6.2.0/logprep/metrics/metric.py
--rw-r--r--   0 runner    (1001) docker     (123)     4765 2023-05-10 09:21:25.000000 logprep-6.2.0/logprep/metrics/metric_exposer.py
--rw-r--r--   0 runner    (1001) docker     (123)     5930 2023-05-10 09:21:25.000000 logprep-6.2.0/logprep/metrics/metric_targets.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 09:21:31.932516 logprep-6.2.0/logprep/processor/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 09:21:25.000000 logprep-6.2.0/logprep/processor/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 09:21:31.936516 logprep-6.2.0/logprep/processor/amides/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 09:21:25.000000 logprep-6.2.0/logprep/processor/amides/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5193 2023-05-10 09:21:25.000000 logprep-6.2.0/logprep/processor/amides/detection.py
--rw-r--r--   0 runner    (1001) docker     (123)     4331 2023-05-10 09:21:25.000000 logprep-6.2.0/logprep/processor/amides/features.py
--rw-r--r--   0 runner    (1001) docker     (123)     2138 2023-05-10 09:21:25.000000 logprep-6.2.0/logprep/processor/amides/normalize.py
--rw-r--r--   0 runner    (1001) docker     (123)    11157 2023-05-10 09:21:25.000000 logprep-6.2.0/logprep/processor/amides/processor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1598 2023-05-10 09:21:25.000000 logprep-6.2.0/logprep/processor/amides/rule.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 09:21:31.936516 logprep-6.2.0/logprep/processor/base/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 09:21:25.000000 logprep-6.2.0/logprep/processor/base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2999 2023-05-10 09:21:25.000000 logprep-6.2.0/logprep/processor/base/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    12057 2023-05-10 09:21:25.000000 logprep-6.2.0/logprep/processor/base/rule.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 09:21:31.936516 logprep-6.2.0/logprep/processor/calculator/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 09:21:25.000000 logprep-6.2.0/logprep/processor/calculator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5442 2023-05-10 09:21:25.000000 logprep-6.2.0/logprep/processor/calculator/fourFn.py
--rw-r--r--   0 runner    (1001) docker     (123)     2770 2023-05-10 09:21:25.000000 logprep-6.2.0/logprep/processor/calculator/processor.py
--rw-r--r--   0 runner    (1001) docker     (123)     4159 2023-05-10 09:21:25.000000 logprep-6.2.0/logprep/processor/calculator/rule.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 09:21:31.936516 logprep-6.2.0/logprep/processor/clusterer/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 09:21:25.000000 logprep-6.2.0/logprep/processor/clusterer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      217 2023-05-10 09:21:25.000000 logprep-6.2.0/logprep/processor/clusterer/configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)     4995 2023-05-10 09:21:25.000000 logprep-6.2.0/logprep/processor/clusterer/processor.py
--rw-r--r--   0 runner    (1001) docker     (123)     4257 2023-05-10 09:21:25.000000 logprep-6.2.0/logprep/processor/clusterer/rule.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 09:21:31.936516 logprep-6.2.0/logprep/processor/clusterer/signature_calculation/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 09:21:25.000000 logprep-6.2.0/logprep/processor/clusterer/signature_calculation/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 09:21:31.936516 logprep-6.2.0/logprep/processor/clusterer/signature_calculation/rules/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 09:21:25.000000 logprep-6.2.0/logprep/processor/clusterer/signature_calculation/rules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      235 2023-05-10 09:21:25.000000 logprep-6.2.0/logprep/processor/clusterer/signature_calculation/rules/rule_template.py
--rw-r--r--   0 runner    (1001) docker     (123)     6672 2023-05-10 09:21:25.000000 logprep-6.2.0/logprep/processor/clusterer/signature_calculation/signature_phase.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 09:21:31.936516 logprep-6.2.0/logprep/processor/concatenator/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 09:21:25.000000 logprep-6.2.0/logprep/processor/concatenator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1924 2023-05-10 09:21:25.000000 logprep-6.2.0/logprep/processor/concatenator/processor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1766 2023-05-10 09:21:25.000000 logprep-6.2.0/logprep/processor/concatenator/rule.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 09:21:31.936516 logprep-6.2.0/logprep/processor/datetime_extractor/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 09:21:25.000000 logprep-6.2.0/logprep/processor/datetime_extractor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2743 2023-05-10 09:21:25.000000 logprep-6.2.0/logprep/processor/datetime_extractor/processor.py
--rw-r--r--   0 runner    (1001) docker     (123)      925 2023-05-10 09:21:25.000000 logprep-6.2.0/logprep/processor/datetime_extractor/rule.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 09:21:31.936516 logprep-6.2.0/logprep/processor/deleter/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 09:21:25.000000 logprep-6.2.0/logprep/processor/deleter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      690 2023-05-10 09:21:25.000000 logprep-6.2.0/logprep/processor/deleter/processor.py
--rw-r--r--   0 runner    (1001) docker     (123)      885 2023-05-10 09:21:25.000000 logprep-6.2.0/logprep/processor/deleter/rule.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 09:21:31.936516 logprep-6.2.0/logprep/processor/dissector/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 09:21:25.000000 logprep-6.2.0/logprep/processor/dissector/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3057 2023-05-10 09:21:25.000000 logprep-6.2.0/logprep/processor/dissector/processor.py
--rw-r--r--   0 runner    (1001) docker     (123)     8754 2023-05-10 09:21:25.000000 logprep-6.2.0/logprep/processor/dissector/rule.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 09:21:31.936516 logprep-6.2.0/logprep/processor/domain_label_extractor/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 09:21:25.000000 logprep-6.2.0/logprep/processor/domain_label_extractor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5921 2023-05-10 09:21:25.000000 logprep-6.2.0/logprep/processor/domain_label_extractor/processor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1667 2023-05-10 09:21:25.000000 logprep-6.2.0/logprep/processor/domain_label_extractor/rule.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 09:21:31.940516 logprep-6.2.0/logprep/processor/domain_resolver/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 09:21:25.000000 logprep-6.2.0/logprep/processor/domain_resolver/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8276 2023-05-10 09:21:25.000000 logprep-6.2.0/logprep/processor/domain_resolver/processor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1386 2023-05-10 09:21:25.000000 logprep-6.2.0/logprep/processor/domain_resolver/rule.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 09:21:31.940516 logprep-6.2.0/logprep/processor/dropper/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 09:21:25.000000 logprep-6.2.0/logprep/processor/dropper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1319 2023-05-10 09:21:25.000000 logprep-6.2.0/logprep/processor/dropper/processor.py
--rw-r--r--   0 runner    (1001) docker     (123)     2085 2023-05-10 09:21:25.000000 logprep-6.2.0/logprep/processor/dropper/rule.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 09:21:31.940516 logprep-6.2.0/logprep/processor/field_manager/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 09:21:25.000000 logprep-6.2.0/logprep/processor/field_manager/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4518 2023-05-10 09:21:25.000000 logprep-6.2.0/logprep/processor/field_manager/processor.py
--rw-r--r--   0 runner    (1001) docker     (123)     4832 2023-05-10 09:21:25.000000 logprep-6.2.0/logprep/processor/field_manager/rule.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 09:21:31.940516 logprep-6.2.0/logprep/processor/generic_adder/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 09:21:25.000000 logprep-6.2.0/logprep/processor/generic_adder/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5931 2023-05-10 09:21:25.000000 logprep-6.2.0/logprep/processor/generic_adder/mysql_connector.py
--rw-r--r--   0 runner    (1001) docker     (123)    10655 2023-05-10 09:21:25.000000 logprep-6.2.0/logprep/processor/generic_adder/processor.py
--rw-r--r--   0 runner    (1001) docker     (123)     9198 2023-05-10 09:21:25.000000 logprep-6.2.0/logprep/processor/generic_adder/rule.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 09:21:31.940516 logprep-6.2.0/logprep/processor/generic_resolver/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 09:21:25.000000 logprep-6.2.0/logprep/processor/generic_resolver/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5710 2023-05-10 09:21:25.000000 logprep-6.2.0/logprep/processor/generic_resolver/processor.py
--rw-r--r--   0 runner    (1001) docker     (123)     5490 2023-05-10 09:21:25.000000 logprep-6.2.0/logprep/processor/generic_resolver/rule.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 09:21:31.940516 logprep-6.2.0/logprep/processor/geoip_enricher/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 09:21:25.000000 logprep-6.2.0/logprep/processor/geoip_enricher/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4829 2023-05-10 09:21:25.000000 logprep-6.2.0/logprep/processor/geoip_enricher/processor.py
--rw-r--r--   0 runner    (1001) docker     (123)     3060 2023-05-10 09:21:25.000000 logprep-6.2.0/logprep/processor/geoip_enricher/rule.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 09:21:31.940516 logprep-6.2.0/logprep/processor/grokker/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 09:21:25.000000 logprep-6.2.0/logprep/processor/grokker/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3834 2023-05-10 09:21:25.000000 logprep-6.2.0/logprep/processor/grokker/processor.py
--rw-r--r--   0 runner    (1001) docker     (123)     5728 2023-05-10 09:21:25.000000 logprep-6.2.0/logprep/processor/grokker/rule.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 09:21:31.940516 logprep-6.2.0/logprep/processor/hyperscan_resolver/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 09:21:25.000000 logprep-6.2.0/logprep/processor/hyperscan_resolver/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8644 2023-05-10 09:21:25.000000 logprep-6.2.0/logprep/processor/hyperscan_resolver/processor.py
--rw-r--r--   0 runner    (1001) docker     (123)     7439 2023-05-10 09:21:25.000000 logprep-6.2.0/logprep/processor/hyperscan_resolver/rule.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 09:21:31.940516 logprep-6.2.0/logprep/processor/ip_informer/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 09:21:25.000000 logprep-6.2.0/logprep/processor/ip_informer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2682 2023-05-10 09:21:25.000000 logprep-6.2.0/logprep/processor/ip_informer/processor.py
--rw-r--r--   0 runner    (1001) docker     (123)     3451 2023-05-10 09:21:25.000000 logprep-6.2.0/logprep/processor/ip_informer/rule.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 09:21:31.940516 logprep-6.2.0/logprep/processor/key_checker/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 09:21:25.000000 logprep-6.2.0/logprep/processor/key_checker/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1388 2023-05-10 09:21:25.000000 logprep-6.2.0/logprep/processor/key_checker/processor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1452 2023-05-10 09:21:25.000000 logprep-6.2.0/logprep/processor/key_checker/rule.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 09:21:31.944516 logprep-6.2.0/logprep/processor/labeler/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 09:21:25.000000 logprep-6.2.0/logprep/processor/labeler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6943 2023-05-10 09:21:25.000000 logprep-6.2.0/logprep/processor/labeler/labeling_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     3621 2023-05-10 09:21:25.000000 logprep-6.2.0/logprep/processor/labeler/processor.py
--rw-r--r--   0 runner    (1001) docker     (123)     2143 2023-05-10 09:21:25.000000 logprep-6.2.0/logprep/processor/labeler/rule.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 09:21:31.944516 logprep-6.2.0/logprep/processor/list_comparison/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 09:21:25.000000 logprep-6.2.0/logprep/processor/list_comparison/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3832 2023-05-10 09:21:25.000000 logprep-6.2.0/logprep/processor/list_comparison/processor.py
--rw-r--r--   0 runner    (1001) docker     (123)     4836 2023-05-10 09:21:25.000000 logprep-6.2.0/logprep/processor/list_comparison/rule.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 09:21:31.944516 logprep-6.2.0/logprep/processor/normalizer/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 09:21:25.000000 logprep-6.2.0/logprep/processor/normalizer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16581 2023-05-10 09:21:25.000000 logprep-6.2.0/logprep/processor/normalizer/processor.py
--rw-r--r--   0 runner    (1001) docker     (123)    28741 2023-05-10 09:21:25.000000 logprep-6.2.0/logprep/processor/normalizer/rule.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 09:21:31.944516 logprep-6.2.0/logprep/processor/pre_detector/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 09:21:25.000000 logprep-6.2.0/logprep/processor/pre_detector/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3757 2023-05-10 09:21:25.000000 logprep-6.2.0/logprep/processor/pre_detector/ip_alerter.py
--rw-r--r--   0 runner    (1001) docker     (123)     4923 2023-05-10 09:21:25.000000 logprep-6.2.0/logprep/processor/pre_detector/processor.py
--rw-r--r--   0 runner    (1001) docker     (123)     3824 2023-05-10 09:21:25.000000 logprep-6.2.0/logprep/processor/pre_detector/rule.py
--rw-r--r--   0 runner    (1001) docker     (123)     3104 2023-05-10 09:21:25.000000 logprep-6.2.0/logprep/processor/processor_strategy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 09:21:31.944516 logprep-6.2.0/logprep/processor/pseudonymizer/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 09:21:25.000000 logprep-6.2.0/logprep/processor/pseudonymizer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2724 2023-05-10 09:21:25.000000 logprep-6.2.0/logprep/processor/pseudonymizer/encrypter.py
--rw-r--r--   0 runner    (1001) docker     (123)    16129 2023-05-10 09:21:25.000000 logprep-6.2.0/logprep/processor/pseudonymizer/processor.py
--rw-r--r--   0 runner    (1001) docker     (123)     2363 2023-05-10 09:21:25.000000 logprep-6.2.0/logprep/processor/pseudonymizer/rule.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 09:21:31.944516 logprep-6.2.0/logprep/processor/requester/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 09:21:25.000000 logprep-6.2.0/logprep/processor/requester/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3818 2023-05-10 09:21:25.000000 logprep-6.2.0/logprep/processor/requester/processor.py
--rw-r--r--   0 runner    (1001) docker     (123)     7079 2023-05-10 09:21:25.000000 logprep-6.2.0/logprep/processor/requester/rule.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 09:21:31.944516 logprep-6.2.0/logprep/processor/selective_extractor/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 09:21:25.000000 logprep-6.2.0/logprep/processor/selective_extractor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2819 2023-05-10 09:21:25.000000 logprep-6.2.0/logprep/processor/selective_extractor/processor.py
--rw-r--r--   0 runner    (1001) docker     (123)     5853 2023-05-10 09:21:25.000000 logprep-6.2.0/logprep/processor/selective_extractor/rule.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 09:21:31.944516 logprep-6.2.0/logprep/processor/string_splitter/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 09:21:25.000000 logprep-6.2.0/logprep/processor/string_splitter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1649 2023-05-10 09:21:25.000000 logprep-6.2.0/logprep/processor/string_splitter/processor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1583 2023-05-10 09:21:25.000000 logprep-6.2.0/logprep/processor/string_splitter/rule.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 09:21:31.944516 logprep-6.2.0/logprep/processor/template_replacer/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 09:21:25.000000 logprep-6.2.0/logprep/processor/template_replacer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5821 2023-05-10 09:21:25.000000 logprep-6.2.0/logprep/processor/template_replacer/processor.py
--rw-r--r--   0 runner    (1001) docker     (123)      772 2023-05-10 09:21:25.000000 logprep-6.2.0/logprep/processor/template_replacer/rule.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 09:21:31.944516 logprep-6.2.0/logprep/processor/timestamp_differ/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 09:21:25.000000 logprep-6.2.0/logprep/processor/timestamp_differ/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3239 2023-05-10 09:21:25.000000 logprep-6.2.0/logprep/processor/timestamp_differ/processor.py
--rw-r--r--   0 runner    (1001) docker     (123)     4114 2023-05-10 09:21:25.000000 logprep-6.2.0/logprep/processor/timestamp_differ/rule.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 09:21:31.948516 logprep-6.2.0/logprep/processor/timestamper/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 09:21:25.000000 logprep-6.2.0/logprep/processor/timestamper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2502 2023-05-10 09:21:25.000000 logprep-6.2.0/logprep/processor/timestamper/processor.py
--rw-r--r--   0 runner    (1001) docker     (123)     3971 2023-05-10 09:21:25.000000 logprep-6.2.0/logprep/processor/timestamper/rule.py
--rw-r--r--   0 runner    (1001) docker     (123)     4985 2023-05-10 09:21:25.000000 logprep-6.2.0/logprep/registry.py
--rw-r--r--   0 runner    (1001) docker     (123)     8561 2023-05-10 09:21:25.000000 logprep-6.2.0/logprep/run_logprep.py
--rw-r--r--   0 runner    (1001) docker     (123)    11023 2023-05-10 09:21:25.000000 logprep-6.2.0/logprep/runner.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 09:21:31.948516 logprep-6.2.0/logprep/util/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 09:21:25.000000 logprep-6.2.0/logprep/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2526 2023-05-10 09:21:25.000000 logprep-6.2.0/logprep/util/aggregating_logger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 09:21:31.948516 logprep-6.2.0/logprep/util/auto_rule_tester/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 09:21:25.000000 logprep-6.2.0/logprep/util/auto_rule_tester/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17268 2023-05-10 09:21:25.000000 logprep-6.2.0/logprep/util/auto_rule_tester/auto_rule_corpus_tester.py
--rw-r--r--   0 runner    (1001) docker     (123)    26980 2023-05-10 09:21:25.000000 logprep-6.2.0/logprep/util/auto_rule_tester/auto_rule_tester.py
--rw-r--r--   0 runner    (1001) docker     (123)     8157 2023-05-10 09:21:25.000000 logprep-6.2.0/logprep/util/auto_rule_tester/grok_pattern_replacer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-05-10 09:21:25.000000 logprep-6.2.0/logprep/util/cache.py
--rw-r--r--   0 runner    (1001) docker     (123)    19307 2023-05-10 09:21:25.000000 logprep-6.2.0/logprep/util/configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)      704 2023-05-10 09:21:25.000000 logprep-6.2.0/logprep/util/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)     4950 2023-05-10 09:21:25.000000 logprep-6.2.0/logprep/util/getter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 09:21:31.948516 logprep-6.2.0/logprep/util/grok/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 09:21:25.000000 logprep-6.2.0/logprep/util/grok/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7570 2023-05-10 09:21:25.000000 logprep-6.2.0/logprep/util/grok/grok.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 09:21:31.924516 logprep-6.2.0/logprep/util/grok/patterns/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 09:21:31.952516 logprep-6.2.0/logprep/util/grok/patterns/ecs-v1/
--rw-r--r--   0 runner    (1001) docker     (123)     4741 2023-05-10 09:21:25.000000 logprep-6.2.0/logprep/util/grok/patterns/ecs-v1/aws
--rw-r--r--   0 runner    (1001) docker     (123)     5852 2023-05-10 09:21:25.000000 logprep-6.2.0/logprep/util/grok/patterns/ecs-v1/bacula
--rw-r--r--   0 runner    (1001) docker     (123)      977 2023-05-10 09:21:25.000000 logprep-6.2.0/logprep/util/grok/patterns/ecs-v1/bind
--rw-r--r--   0 runner    (1001) docker     (123)     4612 2023-05-10 09:21:25.000000 logprep-6.2.0/logprep/util/grok/patterns/ecs-v1/bro
--rw-r--r--   0 runner    (1001) docker     (123)     1849 2023-05-10 09:21:25.000000 logprep-6.2.0/logprep/util/grok/patterns/ecs-v1/exim
--rw-r--r--   0 runner    (1001) docker     (123)    15471 2023-05-10 09:21:25.000000 logprep-6.2.0/logprep/util/grok/patterns/ecs-v1/firewalls
--rw-r--r--   0 runner    (1001) docker     (123)     5514 2023-05-10 09:21:25.000000 logprep-6.2.0/logprep/util/grok/patterns/ecs-v1/grok-patterns
--rw-r--r--   0 runner    (1001) docker     (123)     4015 2023-05-10 09:21:25.000000 logprep-6.2.0/logprep/util/grok/patterns/ecs-v1/haproxy
--rw-r--r--   0 runner    (1001) docker     (123)     1411 2023-05-10 09:21:25.000000 logprep-6.2.0/logprep/util/grok/patterns/ecs-v1/httpd
--rw-r--r--   0 runner    (1001) docker     (123)     2223 2023-05-10 09:21:25.000000 logprep-6.2.0/logprep/util/grok/patterns/ecs-v1/java
--rw-r--r--   0 runner    (1001) docker     (123)     1893 2023-05-10 09:21:25.000000 logprep-6.2.0/logprep/util/grok/patterns/ecs-v1/junos
--rw-r--r--   0 runner    (1001) docker     (123)     1143 2023-05-10 09:21:25.000000 logprep-6.2.0/logprep/util/grok/patterns/ecs-v1/linux-syslog
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-05-10 09:21:25.000000 logprep-6.2.0/logprep/util/grok/patterns/ecs-v1/maven
--rw-r--r--   0 runner    (1001) docker     (123)      206 2023-05-10 09:21:25.000000 logprep-6.2.0/logprep/util/grok/patterns/ecs-v1/mcollective
--rw-r--r--   0 runner    (1001) docker     (123)      842 2023-05-10 09:21:25.000000 logprep-6.2.0/logprep/util/grok/patterns/ecs-v1/mongodb
--rw-r--r--   0 runner    (1001) docker     (123)    10242 2023-05-10 09:21:25.000000 logprep-6.2.0/logprep/util/grok/patterns/ecs-v1/nagios
--rw-r--r--   0 runner    (1001) docker     (123)      198 2023-05-10 09:21:25.000000 logprep-6.2.0/logprep/util/grok/patterns/ecs-v1/postgresql
--rw-r--r--   0 runner    (1001) docker     (123)     1137 2023-05-10 09:21:25.000000 logprep-6.2.0/logprep/util/grok/patterns/ecs-v1/rails
--rw-r--r--   0 runner    (1001) docker     (123)      302 2023-05-10 09:21:25.000000 logprep-6.2.0/logprep/util/grok/patterns/ecs-v1/redis
--rw-r--r--   0 runner    (1001) docker     (123)      214 2023-05-10 09:21:25.000000 logprep-6.2.0/logprep/util/grok/patterns/ecs-v1/ruby
--rw-r--r--   0 runner    (1001) docker     (123)      637 2023-05-10 09:21:25.000000 logprep-6.2.0/logprep/util/grok/patterns/ecs-v1/squid
--rw-r--r--   0 runner    (1001) docker     (123)     5366 2023-05-10 09:21:25.000000 logprep-6.2.0/logprep/util/grok/patterns/ecs-v1/zeek
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 09:21:31.956516 logprep-6.2.0/logprep/util/grok/patterns/legacy/
--rw-r--r--   0 runner    (1001) docker     (123)     1839 2023-05-10 09:21:25.000000 logprep-6.2.0/logprep/util/grok/patterns/legacy/aws
--rw-r--r--   0 runner    (1001) docker     (123)     4833 2023-05-10 09:21:25.000000 logprep-6.2.0/logprep/util/grok/patterns/legacy/bacula
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-05-10 09:21:25.000000 logprep-6.2.0/logprep/util/grok/patterns/legacy/bind
--rw-r--r--   0 runner    (1001) docker     (123)     2154 2023-05-10 09:21:25.000000 logprep-6.2.0/logprep/util/grok/patterns/legacy/bro
--rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-05-10 09:21:25.000000 logprep-6.2.0/logprep/util/grok/patterns/legacy/exim
--rw-r--r--   0 runner    (1001) docker     (123)    10109 2023-05-10 09:21:25.000000 logprep-6.2.0/logprep/util/grok/patterns/legacy/firewalls
--rw-r--r--   0 runner    (1001) docker     (123)     5402 2023-05-10 09:21:25.000000 logprep-6.2.0/logprep/util/grok/patterns/legacy/grok-patterns
--rw-r--r--   0 runner    (1001) docker     (123)     3252 2023-05-10 09:21:25.000000 logprep-6.2.0/logprep/util/grok/patterns/legacy/haproxy
--rw-r--r--   0 runner    (1001) docker     (123)      998 2023-05-10 09:21:25.000000 logprep-6.2.0/logprep/util/grok/patterns/legacy/httpd
--rw-r--r--   0 runner    (1001) docker     (123)     1193 2023-05-10 09:21:25.000000 logprep-6.2.0/logprep/util/grok/patterns/legacy/java
--rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-05-10 09:21:25.000000 logprep-6.2.0/logprep/util/grok/patterns/legacy/junos
--rw-r--r--   0 runner    (1001) docker     (123)     1037 2023-05-10 09:21:25.000000 logprep-6.2.0/logprep/util/grok/patterns/legacy/linux-syslog
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-05-10 09:21:25.000000 logprep-6.2.0/logprep/util/grok/patterns/legacy/maven
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-10 09:21:25.000000 logprep-6.2.0/logprep/util/grok/patterns/legacy/mcollective
--rw-r--r--   0 runner    (1001) docker     (123)      190 2023-05-10 09:21:25.000000 logprep-6.2.0/logprep/util/grok/patterns/legacy/mcollective-patterns
--rw-r--r--   0 runner    (1001) docker     (123)      614 2023-05-10 09:21:25.000000 logprep-6.2.0/logprep/util/grok/patterns/legacy/mongodb
--rw-r--r--   0 runner    (1001) docker     (123)     9601 2023-05-10 09:21:25.000000 logprep-6.2.0/logprep/util/grok/patterns/legacy/nagios
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-05-10 09:21:25.000000 logprep-6.2.0/logprep/util/grok/patterns/legacy/postgresql
--rw-r--r--   0 runner    (1001) docker     (123)      845 2023-05-10 09:21:25.000000 logprep-6.2.0/logprep/util/grok/patterns/legacy/rails
--rw-r--r--   0 runner    (1001) docker     (123)      224 2023-05-10 09:21:25.000000 logprep-6.2.0/logprep/util/grok/patterns/legacy/redis
--rw-r--r--   0 runner    (1001) docker     (123)      188 2023-05-10 09:21:25.000000 logprep-6.2.0/logprep/util/grok/patterns/legacy/ruby
--rw-r--r--   0 runner    (1001) docker     (123)      411 2023-05-10 09:21:25.000000 logprep-6.2.0/logprep/util/grok/patterns/legacy/squid
--rw-r--r--   0 runner    (1001) docker     (123)     3015 2023-05-10 09:21:25.000000 logprep-6.2.0/logprep/util/grok_pattern_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)      666 2023-05-10 09:21:25.000000 logprep-6.2.0/logprep/util/hasher.py
--rw-r--r--   0 runner    (1001) docker     (123)     9641 2023-05-10 09:21:25.000000 logprep-6.2.0/logprep/util/helper.py
--rw-r--r--   0 runner    (1001) docker     (123)     2735 2023-05-10 09:21:25.000000 logprep-6.2.0/logprep/util/json_handling.py
--rw-r--r--   0 runner    (1001) docker     (123)     3411 2023-05-10 09:21:25.000000 logprep-6.2.0/logprep/util/log_aggregator.py
--rw-r--r--   0 runner    (1001) docker     (123)      814 2023-05-10 09:21:25.000000 logprep-6.2.0/logprep/util/multiprocessing_log_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-05-10 09:21:25.000000 logprep-6.2.0/logprep/util/pipeline_profiler.py
--rw-r--r--   0 runner    (1001) docker     (123)    12543 2023-05-10 09:21:25.000000 logprep-6.2.0/logprep/util/pre_detector_rule_matching_tester.py
--rw-r--r--   0 runner    (1001) docker     (123)     5150 2023-05-10 09:21:25.000000 logprep-6.2.0/logprep/util/processor_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3608 2023-05-10 09:21:25.000000 logprep-6.2.0/logprep/util/prometheus_exporter.py
--rw-r--r--   0 runner    (1001) docker     (123)     5644 2023-05-10 09:21:25.000000 logprep-6.2.0/logprep/util/rule_dry_runner.py
--rw-r--r--   0 runner    (1001) docker     (123)     7634 2023-05-10 09:21:25.000000 logprep-6.2.0/logprep/util/schema_and_rule_checker.py
--rw-r--r--   0 runner    (1001) docker     (123)     2665 2023-05-10 09:21:25.000000 logprep-6.2.0/logprep/util/time.py
--rw-r--r--   0 runner    (1001) docker     (123)     2228 2023-05-10 09:21:25.000000 logprep-6.2.0/logprep/util/time_measurement.py
--rw-r--r--   0 runner    (1001) docker     (123)     6602 2023-05-10 09:21:25.000000 logprep-6.2.0/logprep/util/validators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 09:21:31.928516 logprep-6.2.0/logprep.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    17607 2023-05-10 09:21:31.000000 logprep-6.2.0/logprep.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    17845 2023-05-10 09:21:31.000000 logprep-6.2.0/logprep.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-10 09:21:31.000000 logprep-6.2.0/logprep.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-05-10 09:21:31.000000 logprep-6.2.0/logprep.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      473 2023-05-10 09:21:31.000000 logprep-6.2.0/logprep.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-10 09:21:31.000000 logprep-6.2.0/logprep.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-05-10 09:21:25.000000 logprep-6.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      201 2023-05-10 09:21:31.976516 logprep-6.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1421 2023-05-10 09:21:25.000000 logprep-6.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 09:21:31.956516 logprep-6.2.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 09:21:25.000000 logprep-6.2.0/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 09:21:31.956516 logprep-6.2.0/tests/acceptance/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 09:21:25.000000 logprep-6.2.0/tests/acceptance/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1846 2023-05-10 09:21:25.000000 logprep-6.2.0/tests/acceptance/test_amides.py
--rw-r--r--   0 runner    (1001) docker     (123)     1718 2023-05-10 09:21:25.000000 logprep-6.2.0/tests/acceptance/test_config_refresh.py
--rw-r--r--   0 runner    (1001) docker     (123)     3390 2023-05-10 09:21:25.000000 logprep-6.2.0/tests/acceptance/test_file_input.py
--rw-r--r--   0 runner    (1001) docker     (123)     9180 2023-05-10 09:21:25.000000 logprep-6.2.0/tests/acceptance/test_full_configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)     4675 2023-05-10 09:21:25.000000 logprep-6.2.0/tests/acceptance/test_http_input.py
--rw-r--r--   0 runner    (1001) docker     (123)     5163 2023-05-10 09:21:25.000000 logprep-6.2.0/tests/acceptance/test_multiple_outputs.py
--rw-r--r--   0 runner    (1001) docker     (123)    19060 2023-05-10 09:21:25.000000 logprep-6.2.0/tests/acceptance/test_pre_detection.py
--rw-r--r--   0 runner    (1001) docker     (123)     1834 2023-05-10 09:21:25.000000 logprep-6.2.0/tests/acceptance/test_preprocessing.py
--rw-r--r--   0 runner    (1001) docker     (123)     2839 2023-05-10 09:21:25.000000 logprep-6.2.0/tests/acceptance/test_selective_extractor_full_pipeline_pass.py
--rw-r--r--   0 runner    (1001) docker     (123)     1973 2023-05-10 09:21:25.000000 logprep-6.2.0/tests/acceptance/test_wineventlog_normalization.py
--rw-r--r--   0 runner    (1001) docker     (123)     3192 2023-05-10 09:21:25.000000 logprep-6.2.0/tests/acceptance/test_wineventlog_processing.py
--rw-r--r--   0 runner    (1001) docker     (123)     2751 2023-05-10 09:21:25.000000 logprep-6.2.0/tests/acceptance/test_wineventlog_pseudonymization.py
--rw-r--r--   0 runner    (1001) docker     (123)    10368 2023-05-10 09:21:25.000000 logprep-6.2.0/tests/acceptance/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 09:21:31.956516 logprep-6.2.0/tests/ci/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 09:21:25.000000 logprep-6.2.0/tests/ci/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 09:21:31.956516 logprep-6.2.0/tests/ci/runner-image/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 09:21:25.000000 logprep-6.2.0/tests/ci/runner-image/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 09:21:31.956516 logprep-6.2.0/tests/ci/runner-image/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 09:21:25.000000 logprep-6.2.0/tests/ci/runner-image/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-05-10 09:21:25.000000 logprep-6.2.0/tests/ci/runner-image/scripts/compare_json.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 09:21:31.956516 logprep-6.2.0/tests/testdata/
--rw-r--r--   0 runner    (1001) docker     (123)     1534 2023-05-10 09:21:25.000000 logprep-6.2.0/tests/testdata/ConfigurationForTest.py
--rw-r--r--   0 runner    (1001) docker     (123)      655 2023-05-10 09:21:25.000000 logprep-6.2.0/tests/testdata/FilledTempFile.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 09:21:25.000000 logprep-6.2.0/tests/testdata/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      807 2023-05-10 09:21:25.000000 logprep-6.2.0/tests/testdata/metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-05-10 09:21:25.000000 logprep-6.2.0/tests/testdata/ruledata.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 09:21:31.956516 logprep-6.2.0/tests/testdata/unit/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 09:21:25.000000 logprep-6.2.0/tests/testdata/unit/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 09:21:31.956516 logprep-6.2.0/tests/testdata/unit/clusterer/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 09:21:25.000000 logprep-6.2.0/tests/testdata/unit/clusterer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12733 2023-05-10 09:21:25.000000 logprep-6.2.0/tests/testdata/unit/clusterer/test_data.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 09:21:31.956516 logprep-6.2.0/tests/unit/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 09:21:25.000000 logprep-6.2.0/tests/unit/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 09:21:31.956516 logprep-6.2.0/tests/unit/component/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 09:21:25.000000 logprep-6.2.0/tests/unit/component/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1693 2023-05-10 09:21:25.000000 logprep-6.2.0/tests/unit/component/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 09:21:31.960516 logprep-6.2.0/tests/unit/connector/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 09:21:25.000000 logprep-6.2.0/tests/unit/connector/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21616 2023-05-10 09:21:25.000000 logprep-6.2.0/tests/unit/connector/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2226 2023-05-10 09:21:25.000000 logprep-6.2.0/tests/unit/connector/test_confluent_kafka_common.py
--rw-r--r--   0 runner    (1001) docker     (123)     7303 2023-05-10 09:21:25.000000 logprep-6.2.0/tests/unit/connector/test_confluent_kafka_input.py
--rw-r--r--   0 runner    (1001) docker     (123)     7315 2023-05-10 09:21:25.000000 logprep-6.2.0/tests/unit/connector/test_confluent_kafka_output.py
--rw-r--r--   0 runner    (1001) docker     (123)     1761 2023-05-10 09:21:25.000000 logprep-6.2.0/tests/unit/connector/test_console_output.py
--rw-r--r--   0 runner    (1001) docker     (123)     1495 2023-05-10 09:21:25.000000 logprep-6.2.0/tests/unit/connector/test_dummy_input.py
--rw-r--r--   0 runner    (1001) docker     (123)     3545 2023-05-10 09:21:25.000000 logprep-6.2.0/tests/unit/connector/test_dummy_output.py
--rw-r--r--   0 runner    (1001) docker     (123)     9100 2023-05-10 09:21:25.000000 logprep-6.2.0/tests/unit/connector/test_elasticsearch_output.py
--rw-r--r--   0 runner    (1001) docker     (123)     9926 2023-05-10 09:21:25.000000 logprep-6.2.0/tests/unit/connector/test_file_input_default_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     3523 2023-05-10 09:21:25.000000 logprep-6.2.0/tests/unit/connector/test_file_input_not_tailing_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2532 2023-05-10 09:21:25.000000 logprep-6.2.0/tests/unit/connector/test_file_input_start_at_end_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     6314 2023-05-10 09:21:25.000000 logprep-6.2.0/tests/unit/connector/test_http_input.py
--rw-r--r--   0 runner    (1001) docker     (123)     2071 2023-05-10 09:21:25.000000 logprep-6.2.0/tests/unit/connector/test_json_input.py
--rw-r--r--   0 runner    (1001) docker     (123)     1985 2023-05-10 09:21:25.000000 logprep-6.2.0/tests/unit/connector/test_jsonl_input.py
--rw-r--r--   0 runner    (1001) docker     (123)     5034 2023-05-10 09:21:25.000000 logprep-6.2.0/tests/unit/connector/test_jsonl_output.py
--rw-r--r--   0 runner    (1001) docker     (123)     9276 2023-05-10 09:21:25.000000 logprep-6.2.0/tests/unit/connector/test_opensearch_output.py
--rw-r--r--   0 runner    (1001) docker     (123)    10265 2023-05-10 09:21:25.000000 logprep-6.2.0/tests/unit/connector/test_s3_output.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 09:21:31.960516 logprep-6.2.0/tests/unit/exceptions/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 09:21:25.000000 logprep-6.2.0/tests/unit/exceptions/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 09:21:31.960516 logprep-6.2.0/tests/unit/exceptions/processor/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 09:21:25.000000 logprep-6.2.0/tests/unit/exceptions/processor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2167 2023-05-10 09:21:25.000000 logprep-6.2.0/tests/unit/exceptions/processor/test_processing_warning.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 09:21:31.960516 logprep-6.2.0/tests/unit/filter/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 09:21:25.000000 logprep-6.2.0/tests/unit/filter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19683 2023-05-10 09:21:25.000000 logprep-6.2.0/tests/unit/filter/test_filter_expression.py
--rw-r--r--   0 runner    (1001) docker     (123)    20548 2023-05-10 09:21:25.000000 logprep-6.2.0/tests/unit/filter/test_lucene_filter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 09:21:31.960516 logprep-6.2.0/tests/unit/framework/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 09:21:25.000000 logprep-6.2.0/tests/unit/framework/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 09:21:31.960516 logprep-6.2.0/tests/unit/framework/rule_tree/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 09:21:25.000000 logprep-6.2.0/tests/unit/framework/rule_tree/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1894 2023-05-10 09:21:25.000000 logprep-6.2.0/tests/unit/framework/rule_tree/test_node.py
--rw-r--r--   0 runner    (1001) docker     (123)    27846 2023-05-10 09:21:25.000000 logprep-6.2.0/tests/unit/framework/rule_tree/test_rule_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)    19943 2023-05-10 09:21:25.000000 logprep-6.2.0/tests/unit/framework/rule_tree/test_rule_tree.py
--rw-r--r--   0 runner    (1001) docker     (123)    39696 2023-05-10 09:21:25.000000 logprep-6.2.0/tests/unit/framework/test_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (123)     9032 2023-05-10 09:21:25.000000 logprep-6.2.0/tests/unit/framework/test_pipeline_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 09:21:31.960516 logprep-6.2.0/tests/unit/metrics/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 09:21:25.000000 logprep-6.2.0/tests/unit/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8285 2023-05-10 09:21:25.000000 logprep-6.2.0/tests/unit/metrics/test_metric_exposer.py
--rw-r--r--   0 runner    (1001) docker     (123)    22193 2023-05-10 09:21:25.000000 logprep-6.2.0/tests/unit/metrics/test_metric_targets.py
--rw-r--r--   0 runner    (1001) docker     (123)     5612 2023-05-10 09:21:25.000000 logprep-6.2.0/tests/unit/metrics/test_metrics.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 09:21:31.964516 logprep-6.2.0/tests/unit/processor/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 09:21:25.000000 logprep-6.2.0/tests/unit/processor/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 09:21:31.964516 logprep-6.2.0/tests/unit/processor/amides/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 09:21:25.000000 logprep-6.2.0/tests/unit/processor/amides/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8119 2023-05-10 09:21:25.000000 logprep-6.2.0/tests/unit/processor/amides/test_amides.py
--rw-r--r--   0 runner    (1001) docker     (123)     2951 2023-05-10 09:21:25.000000 logprep-6.2.0/tests/unit/processor/amides/test_amides_rule.py
--rw-r--r--   0 runner    (1001) docker     (123)     4396 2023-05-10 09:21:25.000000 logprep-6.2.0/tests/unit/processor/amides/test_detection.py
--rw-r--r--   0 runner    (1001) docker     (123)     1760 2023-05-10 09:21:25.000000 logprep-6.2.0/tests/unit/processor/amides/test_normalize.py
--rw-r--r--   0 runner    (1001) docker     (123)     8041 2023-05-10 09:21:25.000000 logprep-6.2.0/tests/unit/processor/amides/test_tokenizer.py
--rw-r--r--   0 runner    (1001) docker     (123)    14110 2023-05-10 09:21:25.000000 logprep-6.2.0/tests/unit/processor/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 09:21:31.964516 logprep-6.2.0/tests/unit/processor/calculator/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 09:21:25.000000 logprep-6.2.0/tests/unit/processor/calculator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11779 2023-05-10 09:21:25.000000 logprep-6.2.0/tests/unit/processor/calculator/test_calculator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1884 2023-05-10 09:21:25.000000 logprep-6.2.0/tests/unit/processor/calculator/test_calculator_rule.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 09:21:31.964516 logprep-6.2.0/tests/unit/processor/clusterer/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 09:21:25.000000 logprep-6.2.0/tests/unit/processor/clusterer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7217 2023-05-10 09:21:25.000000 logprep-6.2.0/tests/unit/processor/clusterer/test_clusterer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3076 2023-05-10 09:21:25.000000 logprep-6.2.0/tests/unit/processor/clusterer/test_clusterer_rule.py
--rw-r--r--   0 runner    (1001) docker     (123)     4796 2023-05-10 09:21:25.000000 logprep-6.2.0/tests/unit/processor/clusterer/test_clusterer_signature_phase.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 09:21:31.964516 logprep-6.2.0/tests/unit/processor/concatenator/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 09:21:25.000000 logprep-6.2.0/tests/unit/processor/concatenator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6963 2023-05-10 09:21:25.000000 logprep-6.2.0/tests/unit/processor/concatenator/test_concatenator.py
--rw-r--r--   0 runner    (1001) docker     (123)    11216 2023-05-10 09:21:25.000000 logprep-6.2.0/tests/unit/processor/concatenator/test_concatenator_rule.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 09:21:31.964516 logprep-6.2.0/tests/unit/processor/datetime_extractor/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 09:21:25.000000 logprep-6.2.0/tests/unit/processor/datetime_extractor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8165 2023-05-10 09:21:25.000000 logprep-6.2.0/tests/unit/processor/datetime_extractor/test_datetime_extractor.py
--rw-r--r--   0 runner    (1001) docker     (123)     5869 2023-05-10 09:21:25.000000 logprep-6.2.0/tests/unit/processor/datetime_extractor/test_datetime_extractor_rule.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 09:21:31.964516 logprep-6.2.0/tests/unit/processor/deleter/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 09:21:25.000000 logprep-6.2.0/tests/unit/processor/deleter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      893 2023-05-10 09:21:25.000000 logprep-6.2.0/tests/unit/processor/deleter/test_deleter.py
--rw-r--r--   0 runner    (1001) docker     (123)     3527 2023-05-10 09:21:25.000000 logprep-6.2.0/tests/unit/processor/deleter/test_deleter_rule.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 09:21:31.964516 logprep-6.2.0/tests/unit/processor/dissector/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 09:21:25.000000 logprep-6.2.0/tests/unit/processor/dissector/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19625 2023-05-10 09:21:25.000000 logprep-6.2.0/tests/unit/processor/dissector/test_dissector.py
--rw-r--r--   0 runner    (1001) docker     (123)    17681 2023-05-10 09:21:25.000000 logprep-6.2.0/tests/unit/processor/dissector/test_dissector_rule.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 09:21:31.964516 logprep-6.2.0/tests/unit/processor/domain_label_extractor/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 09:21:25.000000 logprep-6.2.0/tests/unit/processor/domain_label_extractor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13265 2023-05-10 09:21:25.000000 logprep-6.2.0/tests/unit/processor/domain_label_extractor/test_domain_label_extractor.py
--rw-r--r--   0 runner    (1001) docker     (123)     5936 2023-05-10 09:21:25.000000 logprep-6.2.0/tests/unit/processor/domain_label_extractor/test_domain_label_extractor_rule.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 09:21:31.964516 logprep-6.2.0/tests/unit/processor/domain_resolver/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 09:21:25.000000 logprep-6.2.0/tests/unit/processor/domain_resolver/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11812 2023-05-10 09:21:25.000000 logprep-6.2.0/tests/unit/processor/domain_resolver/test_domain_resolver.py
--rw-r--r--   0 runner    (1001) docker     (123)     2487 2023-05-10 09:21:25.000000 logprep-6.2.0/tests/unit/processor/domain_resolver/test_domain_resolver_rule.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 09:21:31.968516 logprep-6.2.0/tests/unit/processor/dropper/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 09:21:25.000000 logprep-6.2.0/tests/unit/processor/dropper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6277 2023-05-10 09:21:25.000000 logprep-6.2.0/tests/unit/processor/dropper/test_dropper.py
--rw-r--r--   0 runner    (1001) docker     (123)     4523 2023-05-10 09:21:25.000000 logprep-6.2.0/tests/unit/processor/dropper/test_dropper_rule.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 09:21:31.968516 logprep-6.2.0/tests/unit/processor/field_manager/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 09:21:25.000000 logprep-6.2.0/tests/unit/processor/field_manager/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13374 2023-05-10 09:21:25.000000 logprep-6.2.0/tests/unit/processor/field_manager/test_field_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     3935 2023-05-10 09:21:25.000000 logprep-6.2.0/tests/unit/processor/field_manager/test_field_manager_rule.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 09:21:31.968516 logprep-6.2.0/tests/unit/processor/generic_adder/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 09:21:25.000000 logprep-6.2.0/tests/unit/processor/generic_adder/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    29997 2023-05-10 09:21:25.000000 logprep-6.2.0/tests/unit/processor/generic_adder/test_generic_adder.py
--rw-r--r--   0 runner    (1001) docker     (123)     3247 2023-05-10 09:21:25.000000 logprep-6.2.0/tests/unit/processor/generic_adder/test_generic_adder_rule.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 09:21:31.968516 logprep-6.2.0/tests/unit/processor/generic_resolver/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 09:21:25.000000 logprep-6.2.0/tests/unit/processor/generic_resolver/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14079 2023-05-10 09:21:25.000000 logprep-6.2.0/tests/unit/processor/generic_resolver/test_generic_resolver.py
--rw-r--r--   0 runner    (1001) docker     (123)     6408 2023-05-10 09:21:25.000000 logprep-6.2.0/tests/unit/processor/generic_resolver/test_generic_resolver_rule.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 09:21:31.968516 logprep-6.2.0/tests/unit/processor/geoip_enricher/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 09:21:25.000000 logprep-6.2.0/tests/unit/processor/geoip_enricher/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14996 2023-05-10 09:21:25.000000 logprep-6.2.0/tests/unit/processor/geoip_enricher/test_geoip_enricher.py
--rw-r--r--   0 runner    (1001) docker     (123)     2492 2023-05-10 09:21:25.000000 logprep-6.2.0/tests/unit/processor/geoip_enricher/test_geoip_enricher_rule.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 09:21:31.968516 logprep-6.2.0/tests/unit/processor/grokker/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 09:21:25.000000 logprep-6.2.0/tests/unit/processor/grokker/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7375 2023-05-10 09:21:25.000000 logprep-6.2.0/tests/unit/processor/grokker/test_grok.py
--rw-r--r--   0 runner    (1001) docker     (123)    12078 2023-05-10 09:21:25.000000 logprep-6.2.0/tests/unit/processor/grokker/test_grokker.py
--rw-r--r--   0 runner    (1001) docker     (123)    10893 2023-05-10 09:21:25.000000 logprep-6.2.0/tests/unit/processor/grokker/test_grokker_rule.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 09:21:31.968516 logprep-6.2.0/tests/unit/processor/hyperscan_resolver/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 09:21:25.000000 logprep-6.2.0/tests/unit/processor/hyperscan_resolver/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23145 2023-05-10 09:21:25.000000 logprep-6.2.0/tests/unit/processor/hyperscan_resolver/test_hyperscan_resolver.py
--rw-r--r--   0 runner    (1001) docker     (123)     6339 2023-05-10 09:21:25.000000 logprep-6.2.0/tests/unit/processor/hyperscan_resolver/test_hyperscan_resolver_rule.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 09:21:31.968516 logprep-6.2.0/tests/unit/processor/ip_informer/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 09:21:25.000000 logprep-6.2.0/tests/unit/processor/ip_informer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13607 2023-05-10 09:21:25.000000 logprep-6.2.0/tests/unit/processor/ip_informer/test_ip_informer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2110 2023-05-10 09:21:25.000000 logprep-6.2.0/tests/unit/processor/ip_informer/test_ip_informer_rule.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 09:21:31.968516 logprep-6.2.0/tests/unit/processor/labeler/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 09:21:25.000000 logprep-6.2.0/tests/unit/processor/labeler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9177 2023-05-10 09:21:25.000000 logprep-6.2.0/tests/unit/processor/labeler/test_labeler.py
--rw-r--r--   0 runner    (1001) docker     (123)     9016 2023-05-10 09:21:25.000000 logprep-6.2.0/tests/unit/processor/labeler/test_labeler_rule.py
--rw-r--r--   0 runner    (1001) docker     (123)    12544 2023-05-10 09:21:25.000000 logprep-6.2.0/tests/unit/processor/labeler/test_labeling_schema.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 09:21:31.968516 logprep-6.2.0/tests/unit/processor/list_comparison/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 09:21:25.000000 logprep-6.2.0/tests/unit/processor/list_comparison/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11202 2023-05-10 09:21:25.000000 logprep-6.2.0/tests/unit/processor/list_comparison/test_list_comparison.py
--rw-r--r--   0 runner    (1001) docker     (123)     3623 2023-05-10 09:21:25.000000 logprep-6.2.0/tests/unit/processor/list_comparison/test_list_comparison_rule.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 09:21:31.968516 logprep-6.2.0/tests/unit/processor/normalizer/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 09:21:25.000000 logprep-6.2.0/tests/unit/processor/normalizer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    38341 2023-05-10 09:21:25.000000 logprep-6.2.0/tests/unit/processor/normalizer/test_normalizer.py
--rw-r--r--   0 runner    (1001) docker     (123)    11123 2023-05-10 09:21:25.000000 logprep-6.2.0/tests/unit/processor/normalizer/test_normalizer_rule.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 09:21:31.972516 logprep-6.2.0/tests/unit/processor/pre_detector/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 09:21:25.000000 logprep-6.2.0/tests/unit/processor/pre_detector/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5419 2023-05-10 09:21:25.000000 logprep-6.2.0/tests/unit/processor/pre_detector/test_ip_alerter.py
--rw-r--r--   0 runner    (1001) docker     (123)    13961 2023-05-10 09:21:25.000000 logprep-6.2.0/tests/unit/processor/pre_detector/test_pre_detector.py
--rw-r--r--   0 runner    (1001) docker     (123)     6921 2023-05-10 09:21:25.000000 logprep-6.2.0/tests/unit/processor/pre_detector/test_pre_detector_rule.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 09:21:31.972516 logprep-6.2.0/tests/unit/processor/pseudonymizer/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 09:21:25.000000 logprep-6.2.0/tests/unit/processor/pseudonymizer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2974 2023-05-10 09:21:25.000000 logprep-6.2.0/tests/unit/processor/pseudonymizer/test_encrypter.py
--rw-r--r--   0 runner    (1001) docker     (123)    29770 2023-05-10 09:21:25.000000 logprep-6.2.0/tests/unit/processor/pseudonymizer/test_pseudonymizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2691 2023-05-10 09:21:25.000000 logprep-6.2.0/tests/unit/processor/pseudonymizer/test_pseudonymizer_rule.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 09:21:31.972516 logprep-6.2.0/tests/unit/processor/requester/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 09:21:25.000000 logprep-6.2.0/tests/unit/processor/requester/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12431 2023-05-10 09:21:25.000000 logprep-6.2.0/tests/unit/processor/requester/test_requester.py
--rw-r--r--   0 runner    (1001) docker     (123)     8142 2023-05-10 09:21:25.000000 logprep-6.2.0/tests/unit/processor/requester/test_requester_rule.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 09:21:31.972516 logprep-6.2.0/tests/unit/processor/selective_extractor/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 09:21:25.000000 logprep-6.2.0/tests/unit/processor/selective_extractor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5541 2023-05-10 09:21:25.000000 logprep-6.2.0/tests/unit/processor/selective_extractor/test_selective_extractor.py
--rw-r--r--   0 runner    (1001) docker     (123)    11040 2023-05-10 09:21:25.000000 logprep-6.2.0/tests/unit/processor/selective_extractor/test_selective_extractor_rule.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 09:21:31.972516 logprep-6.2.0/tests/unit/processor/string_splitter/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 09:21:25.000000 logprep-6.2.0/tests/unit/processor/string_splitter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2751 2023-05-10 09:21:25.000000 logprep-6.2.0/tests/unit/processor/string_splitter/test_string_splitter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2134 2023-05-10 09:21:25.000000 logprep-6.2.0/tests/unit/processor/string_splitter/test_string_splitter_rule.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 09:21:31.972516 logprep-6.2.0/tests/unit/processor/template_replacer/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 09:21:25.000000 logprep-6.2.0/tests/unit/processor/template_replacer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6683 2023-05-10 09:21:25.000000 logprep-6.2.0/tests/unit/processor/template_replacer/test_template_replacer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1613 2023-05-10 09:21:25.000000 logprep-6.2.0/tests/unit/processor/test_processor_rule.py
--rw-r--r--   0 runner    (1001) docker     (123)     8157 2023-05-10 09:21:25.000000 logprep-6.2.0/tests/unit/processor/test_processor_strategy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 09:21:31.972516 logprep-6.2.0/tests/unit/processor/timestamp_differ/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 09:21:25.000000 logprep-6.2.0/tests/unit/processor/timestamp_differ/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16573 2023-05-10 09:21:25.000000 logprep-6.2.0/tests/unit/processor/timestamp_differ/test_timestamp_differ.py
--rw-r--r--   0 runner    (1001) docker     (123)     4283 2023-05-10 09:21:25.000000 logprep-6.2.0/tests/unit/processor/timestamp_differ/test_timestamp_differ_rule.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 09:21:31.972516 logprep-6.2.0/tests/unit/processor/timestamper/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 09:21:25.000000 logprep-6.2.0/tests/unit/processor/timestamper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8570 2023-05-10 09:21:25.000000 logprep-6.2.0/tests/unit/processor/timestamper/test_timestamper.py
--rw-r--r--   0 runner    (1001) docker     (123)     1823 2023-05-10 09:21:25.000000 logprep-6.2.0/tests/unit/processor/timestamper/test_timestamper_rule.py
--rw-r--r--   0 runner    (1001) docker     (123)     6228 2023-05-10 09:21:25.000000 logprep-6.2.0/tests/unit/test_configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)     5507 2023-05-10 09:21:25.000000 logprep-6.2.0/tests/unit/test_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)    11779 2023-05-10 09:21:25.000000 logprep-6.2.0/tests/unit/test_run_logprep.py
--rw-r--r--   0 runner    (1001) docker     (123)    18858 2023-05-10 09:21:25.000000 logprep-6.2.0/tests/unit/test_runner.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 09:21:31.976516 logprep-6.2.0/tests/unit/util/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 09:21:25.000000 logprep-6.2.0/tests/unit/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19327 2023-05-10 09:21:25.000000 logprep-6.2.0/tests/unit/util/test_auto_rule_corpus_tester.py
--rw-r--r--   0 runner    (1001) docker     (123)    10250 2023-05-10 09:21:25.000000 logprep-6.2.0/tests/unit/util/test_auto_rule_tester.py
--rw-r--r--   0 runner    (1001) docker     (123)     1593 2023-05-10 09:21:25.000000 logprep-6.2.0/tests/unit/util/test_cache.py
--rw-r--r--   0 runner    (1001) docker     (123)    39375 2023-05-10 09:21:25.000000 logprep-6.2.0/tests/unit/util/test_configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)    16243 2023-05-10 09:21:25.000000 logprep-6.2.0/tests/unit/util/test_getter.py
--rw-r--r--   0 runner    (1001) docker     (123)     3097 2023-05-10 09:21:25.000000 logprep-6.2.0/tests/unit/util/test_grok_pattern_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)      469 2023-05-10 09:21:25.000000 logprep-6.2.0/tests/unit/util/test_hasher.py
--rw-r--r--   0 runner    (1001) docker     (123)     7897 2023-05-10 09:21:25.000000 logprep-6.2.0/tests/unit/util/test_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)     7246 2023-05-10 09:21:25.000000 logprep-6.2.0/tests/unit/util/test_helper_add_field.py
--rw-r--r--   0 runner    (1001) docker     (123)     6394 2023-05-10 09:21:25.000000 logprep-6.2.0/tests/unit/util/test_log_aggregator.py
--rw-r--r--   0 runner    (1001) docker     (123)     5521 2023-05-10 09:21:25.000000 logprep-6.2.0/tests/unit/util/test_processor_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     5762 2023-05-10 09:21:25.000000 logprep-6.2.0/tests/unit/util/test_prometheus_exporter.py
--rw-r--r--   0 runner    (1001) docker     (123)     6740 2023-05-10 09:21:25.000000 logprep-6.2.0/tests/unit/util/test_rule_dry_runner.py
--rw-r--r--   0 runner    (1001) docker     (123)      309 2023-05-10 09:21:25.000000 logprep-6.2.0/tests/unit/util/test_schema_and_rule_checker.py
--rw-r--r--   0 runner    (1001) docker     (123)     2368 2023-05-10 09:21:25.000000 logprep-6.2.0/tests/unit/util/test_time.py
--rw-r--r--   0 runner    (1001) docker     (123)     4103 2023-05-10 09:21:25.000000 logprep-6.2.0/tests/unit/util/test_time_measurement.py
--rw-r--r--   0 runner    (1001) docker     (123)    16746 2023-05-10 09:21:25.000000 logprep-6.2.0/tests/unit/util/test_validators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1540 2023-05-10 09:21:25.000000 logprep-6.2.0/tests/unit/util/tests_json_handling.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 09:21:31.976516 logprep-6.2.0/tests/util/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 09:21:25.000000 logprep-6.2.0/tests/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3893 2023-05-10 09:21:25.000000 logprep-6.2.0/tests/util/testhelpers.py
--rw-r--r--   0 runner    (1001) docker     (123)    81000 2023-05-10 09:21:25.000000 logprep-6.2.0/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 10:47:03.664559 logprep-6.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    26526 2023-05-22 10:46:57.000000 logprep-6.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-05-22 10:46:57.000000 logprep-6.3.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    17607 2023-05-22 10:47:03.664559 logprep-6.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    16888 2023-05-22 10:46:57.000000 logprep-6.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 10:47:03.664559 logprep-6.3.0/logprep/
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-05-22 10:46:57.000000 logprep-6.3.0/logprep/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-05-22 10:47:03.664559 logprep-6.3.0/logprep/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 10:47:03.624559 logprep-6.3.0/logprep/abc/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 10:46:57.000000 logprep-6.3.0/logprep/abc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2721 2023-05-22 10:46:57.000000 logprep-6.3.0/logprep/abc/component.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2097 2023-05-22 10:46:57.000000 logprep-6.3.0/logprep/abc/connector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3741 2023-05-22 10:46:57.000000 logprep-6.3.0/logprep/abc/getter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16580 2023-05-22 10:46:57.000000 logprep-6.3.0/logprep/abc/input.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2817 2023-05-22 10:46:57.000000 logprep-6.3.0/logprep/abc/output.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12111 2023-05-22 10:46:57.000000 logprep-6.3.0/logprep/abc/processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1821 2023-05-22 10:46:57.000000 logprep-6.3.0/logprep/configuration.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 10:47:03.624559 logprep-6.3.0/logprep/connector/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 10:46:57.000000 logprep-6.3.0/logprep/connector/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 10:47:03.624559 logprep-6.3.0/logprep/connector/confluent_kafka/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 10:46:57.000000 logprep-6.3.0/logprep/connector/confluent_kafka/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12736 2023-05-22 10:46:57.000000 logprep-6.3.0/logprep/connector/confluent_kafka/input.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8002 2023-05-22 10:46:57.000000 logprep-6.3.0/logprep/connector/confluent_kafka/output.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 10:47:03.624559 logprep-6.3.0/logprep/connector/console/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 10:46:57.000000 logprep-6.3.0/logprep/connector/console/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      978 2023-05-22 10:46:57.000000 logprep-6.3.0/logprep/connector/console/output.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 10:47:03.624559 logprep-6.3.0/logprep/connector/dummy/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 10:46:57.000000 logprep-6.3.0/logprep/connector/dummy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1406 2023-05-22 10:46:57.000000 logprep-6.3.0/logprep/connector/dummy/input.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2722 2023-05-22 10:46:57.000000 logprep-6.3.0/logprep/connector/dummy/output.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 10:47:03.624559 logprep-6.3.0/logprep/connector/elasticsearch/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 10:46:57.000000 logprep-6.3.0/logprep/connector/elasticsearch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13487 2023-05-22 10:46:57.000000 logprep-6.3.0/logprep/connector/elasticsearch/output.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 10:47:03.624559 logprep-6.3.0/logprep/connector/file/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 10:46:57.000000 logprep-6.3.0/logprep/connector/file/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13765 2023-05-22 10:46:57.000000 logprep-6.3.0/logprep/connector/file/input.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 10:47:03.624559 logprep-6.3.0/logprep/connector/http/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 10:46:57.000000 logprep-6.3.0/logprep/connector/http/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5788 2023-05-22 10:46:57.000000 logprep-6.3.0/logprep/connector/http/input.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 10:47:03.624559 logprep-6.3.0/logprep/connector/json/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 10:46:57.000000 logprep-6.3.0/logprep/connector/json/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-05-22 10:46:57.000000 logprep-6.3.0/logprep/connector/json/input.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 10:47:03.624559 logprep-6.3.0/logprep/connector/jsonl/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 10:46:57.000000 logprep-6.3.0/logprep/connector/jsonl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      798 2023-05-22 10:46:57.000000 logprep-6.3.0/logprep/connector/jsonl/input.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3164 2023-05-22 10:46:57.000000 logprep-6.3.0/logprep/connector/jsonl/output.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 10:47:03.624559 logprep-6.3.0/logprep/connector/opensearch/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 10:46:57.000000 logprep-6.3.0/logprep/connector/opensearch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2372 2023-05-22 10:46:57.000000 logprep-6.3.0/logprep/connector/opensearch/output.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 10:47:03.624559 logprep-6.3.0/logprep/connector/s3/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 10:46:57.000000 logprep-6.3.0/logprep/connector/s3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11805 2023-05-22 10:46:57.000000 logprep-6.3.0/logprep/connector/s3/output.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2057 2023-05-22 10:46:57.000000 logprep-6.3.0/logprep/factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1194 2023-05-22 10:46:57.000000 logprep-6.3.0/logprep/factory_error.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 10:47:03.624559 logprep-6.3.0/logprep/filter/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 10:46:57.000000 logprep-6.3.0/logprep/filter/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 10:47:03.624559 logprep-6.3.0/logprep/filter/expression/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 10:46:57.000000 logprep-6.3.0/logprep/filter/expression/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11681 2023-05-22 10:46:57.000000 logprep-6.3.0/logprep/filter/expression/filter_expression.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14986 2023-05-22 10:46:57.000000 logprep-6.3.0/logprep/filter/lucene_filter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 10:47:03.624559 logprep-6.3.0/logprep/framework/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 10:46:57.000000 logprep-6.3.0/logprep/framework/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19708 2023-05-22 10:46:57.000000 logprep-6.3.0/logprep/framework/pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4546 2023-05-22 10:46:57.000000 logprep-6.3.0/logprep/framework/pipeline_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 10:47:03.624559 logprep-6.3.0/logprep/framework/rule_tree/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 10:46:57.000000 logprep-6.3.0/logprep/framework/rule_tree/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3300 2023-05-22 10:46:57.000000 logprep-6.3.0/logprep/framework/rule_tree/node.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22708 2023-05-22 10:46:57.000000 logprep-6.3.0/logprep/framework/rule_tree/rule_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9886 2023-05-22 10:46:57.000000 logprep-6.3.0/logprep/framework/rule_tree/rule_tree.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 10:47:03.628558 logprep-6.3.0/logprep/metrics/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 10:46:57.000000 logprep-6.3.0/logprep/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3450 2023-05-22 10:46:57.000000 logprep-6.3.0/logprep/metrics/metric.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4765 2023-05-22 10:46:57.000000 logprep-6.3.0/logprep/metrics/metric_exposer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5930 2023-05-22 10:46:57.000000 logprep-6.3.0/logprep/metrics/metric_targets.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 10:47:03.628558 logprep-6.3.0/logprep/processor/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 10:46:57.000000 logprep-6.3.0/logprep/processor/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 10:47:03.628558 logprep-6.3.0/logprep/processor/amides/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 10:46:57.000000 logprep-6.3.0/logprep/processor/amides/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5193 2023-05-22 10:46:57.000000 logprep-6.3.0/logprep/processor/amides/detection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4331 2023-05-22 10:46:57.000000 logprep-6.3.0/logprep/processor/amides/features.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2138 2023-05-22 10:46:57.000000 logprep-6.3.0/logprep/processor/amides/normalize.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11343 2023-05-22 10:46:57.000000 logprep-6.3.0/logprep/processor/amides/processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1831 2023-05-22 10:46:57.000000 logprep-6.3.0/logprep/processor/amides/rule.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 10:47:03.628558 logprep-6.3.0/logprep/processor/base/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 10:46:57.000000 logprep-6.3.0/logprep/processor/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2999 2023-05-22 10:46:57.000000 logprep-6.3.0/logprep/processor/base/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12057 2023-05-22 10:46:57.000000 logprep-6.3.0/logprep/processor/base/rule.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 10:47:03.628558 logprep-6.3.0/logprep/processor/calculator/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 10:46:57.000000 logprep-6.3.0/logprep/processor/calculator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5442 2023-05-22 10:46:57.000000 logprep-6.3.0/logprep/processor/calculator/fourFn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2919 2023-05-22 10:46:57.000000 logprep-6.3.0/logprep/processor/calculator/processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4295 2023-05-22 10:46:57.000000 logprep-6.3.0/logprep/processor/calculator/rule.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 10:47:03.628558 logprep-6.3.0/logprep/processor/clusterer/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 10:46:57.000000 logprep-6.3.0/logprep/processor/clusterer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      217 2023-05-22 10:46:57.000000 logprep-6.3.0/logprep/processor/clusterer/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5215 2023-05-22 10:46:57.000000 logprep-6.3.0/logprep/processor/clusterer/processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4418 2023-05-22 10:46:57.000000 logprep-6.3.0/logprep/processor/clusterer/rule.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 10:47:03.628558 logprep-6.3.0/logprep/processor/clusterer/signature_calculation/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 10:46:57.000000 logprep-6.3.0/logprep/processor/clusterer/signature_calculation/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 10:47:03.628558 logprep-6.3.0/logprep/processor/clusterer/signature_calculation/rules/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 10:46:57.000000 logprep-6.3.0/logprep/processor/clusterer/signature_calculation/rules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-05-22 10:46:57.000000 logprep-6.3.0/logprep/processor/clusterer/signature_calculation/rules/rule_template.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6672 2023-05-22 10:46:57.000000 logprep-6.3.0/logprep/processor/clusterer/signature_calculation/signature_phase.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 10:47:03.628558 logprep-6.3.0/logprep/processor/concatenator/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 10:46:57.000000 logprep-6.3.0/logprep/processor/concatenator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2153 2023-05-22 10:46:57.000000 logprep-6.3.0/logprep/processor/concatenator/processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1733 2023-05-22 10:46:57.000000 logprep-6.3.0/logprep/processor/concatenator/rule.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 10:47:03.628558 logprep-6.3.0/logprep/processor/datetime_extractor/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 10:46:57.000000 logprep-6.3.0/logprep/processor/datetime_extractor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2989 2023-05-22 10:46:57.000000 logprep-6.3.0/logprep/processor/datetime_extractor/processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1757 2023-05-22 10:46:57.000000 logprep-6.3.0/logprep/processor/datetime_extractor/rule.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 10:47:03.628558 logprep-6.3.0/logprep/processor/deleter/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 10:46:57.000000 logprep-6.3.0/logprep/processor/deleter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      904 2023-05-22 10:46:57.000000 logprep-6.3.0/logprep/processor/deleter/processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      957 2023-05-22 10:46:57.000000 logprep-6.3.0/logprep/processor/deleter/rule.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 10:47:03.628558 logprep-6.3.0/logprep/processor/dissector/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 10:46:57.000000 logprep-6.3.0/logprep/processor/dissector/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3498 2023-05-22 10:46:57.000000 logprep-6.3.0/logprep/processor/dissector/processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9759 2023-05-22 10:46:57.000000 logprep-6.3.0/logprep/processor/dissector/rule.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 10:47:03.632558 logprep-6.3.0/logprep/processor/domain_label_extractor/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 10:46:57.000000 logprep-6.3.0/logprep/processor/domain_label_extractor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6178 2023-05-22 10:46:57.000000 logprep-6.3.0/logprep/processor/domain_label_extractor/processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2361 2023-05-22 10:46:57.000000 logprep-6.3.0/logprep/processor/domain_label_extractor/rule.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 10:47:03.632558 logprep-6.3.0/logprep/processor/domain_resolver/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 10:46:57.000000 logprep-6.3.0/logprep/processor/domain_resolver/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8513 2023-05-22 10:46:57.000000 logprep-6.3.0/logprep/processor/domain_resolver/processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1617 2023-05-22 10:46:57.000000 logprep-6.3.0/logprep/processor/domain_resolver/rule.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 10:47:03.632558 logprep-6.3.0/logprep/processor/dropper/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 10:46:57.000000 logprep-6.3.0/logprep/processor/dropper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1533 2023-05-22 10:46:57.000000 logprep-6.3.0/logprep/processor/dropper/processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2241 2023-05-22 10:46:57.000000 logprep-6.3.0/logprep/processor/dropper/rule.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 10:47:03.632558 logprep-6.3.0/logprep/processor/field_manager/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 10:46:57.000000 logprep-6.3.0/logprep/processor/field_manager/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7446 2023-05-22 10:46:57.000000 logprep-6.3.0/logprep/processor/field_manager/processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5495 2023-05-22 10:46:57.000000 logprep-6.3.0/logprep/processor/field_manager/rule.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 10:47:03.632558 logprep-6.3.0/logprep/processor/generic_adder/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 10:46:57.000000 logprep-6.3.0/logprep/processor/generic_adder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5931 2023-05-22 10:46:57.000000 logprep-6.3.0/logprep/processor/generic_adder/mysql_connector.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10887 2023-05-22 10:46:57.000000 logprep-6.3.0/logprep/processor/generic_adder/processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9353 2023-05-22 10:46:57.000000 logprep-6.3.0/logprep/processor/generic_adder/rule.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 10:47:03.632558 logprep-6.3.0/logprep/processor/generic_resolver/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 10:46:57.000000 logprep-6.3.0/logprep/processor/generic_resolver/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5951 2023-05-22 10:46:57.000000 logprep-6.3.0/logprep/processor/generic_resolver/processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5616 2023-05-22 10:46:57.000000 logprep-6.3.0/logprep/processor/generic_resolver/rule.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 10:47:03.632558 logprep-6.3.0/logprep/processor/geoip_enricher/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 10:46:57.000000 logprep-6.3.0/logprep/processor/geoip_enricher/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5065 2023-05-22 10:46:57.000000 logprep-6.3.0/logprep/processor/geoip_enricher/processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3291 2023-05-22 10:46:57.000000 logprep-6.3.0/logprep/processor/geoip_enricher/rule.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 10:47:03.632558 logprep-6.3.0/logprep/processor/grokker/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 10:46:57.000000 logprep-6.3.0/logprep/processor/grokker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4295 2023-05-22 10:46:57.000000 logprep-6.3.0/logprep/processor/grokker/processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5626 2023-05-22 10:46:57.000000 logprep-6.3.0/logprep/processor/grokker/rule.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 10:47:03.632558 logprep-6.3.0/logprep/processor/hyperscan_resolver/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 10:46:57.000000 logprep-6.3.0/logprep/processor/hyperscan_resolver/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9032 2023-05-22 10:46:57.000000 logprep-6.3.0/logprep/processor/hyperscan_resolver/processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7441 2023-05-22 10:46:57.000000 logprep-6.3.0/logprep/processor/hyperscan_resolver/rule.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 10:47:03.632558 logprep-6.3.0/logprep/processor/ip_informer/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 10:46:57.000000 logprep-6.3.0/logprep/processor/ip_informer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2905 2023-05-22 10:46:57.000000 logprep-6.3.0/logprep/processor/ip_informer/processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3600 2023-05-22 10:46:57.000000 logprep-6.3.0/logprep/processor/ip_informer/rule.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 10:47:03.632558 logprep-6.3.0/logprep/processor/key_checker/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 10:46:57.000000 logprep-6.3.0/logprep/processor/key_checker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1611 2023-05-22 10:46:57.000000 logprep-6.3.0/logprep/processor/key_checker/processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1820 2023-05-22 10:46:57.000000 logprep-6.3.0/logprep/processor/key_checker/rule.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 10:47:03.632558 logprep-6.3.0/logprep/processor/labeler/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 10:46:57.000000 logprep-6.3.0/logprep/processor/labeler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6943 2023-05-22 10:46:57.000000 logprep-6.3.0/logprep/processor/labeler/labeling_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3836 2023-05-22 10:46:57.000000 logprep-6.3.0/logprep/processor/labeler/processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2298 2023-05-22 10:46:57.000000 logprep-6.3.0/logprep/processor/labeler/rule.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 10:47:03.632558 logprep-6.3.0/logprep/processor/list_comparison/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 10:46:57.000000 logprep-6.3.0/logprep/processor/list_comparison/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4070 2023-05-22 10:46:57.000000 logprep-6.3.0/logprep/processor/list_comparison/processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5066 2023-05-22 10:46:57.000000 logprep-6.3.0/logprep/processor/list_comparison/rule.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 10:47:03.632558 logprep-6.3.0/logprep/processor/normalizer/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 10:46:57.000000 logprep-6.3.0/logprep/processor/normalizer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16806 2023-05-22 10:46:57.000000 logprep-6.3.0/logprep/processor/normalizer/processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28757 2023-05-22 10:46:57.000000 logprep-6.3.0/logprep/processor/normalizer/rule.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 10:47:03.636559 logprep-6.3.0/logprep/processor/pre_detector/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 10:46:57.000000 logprep-6.3.0/logprep/processor/pre_detector/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3757 2023-05-22 10:46:57.000000 logprep-6.3.0/logprep/processor/pre_detector/ip_alerter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5152 2023-05-22 10:46:57.000000 logprep-6.3.0/logprep/processor/pre_detector/processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3982 2023-05-22 10:46:57.000000 logprep-6.3.0/logprep/processor/pre_detector/rule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3104 2023-05-22 10:46:57.000000 logprep-6.3.0/logprep/processor/processor_strategy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 10:47:03.636559 logprep-6.3.0/logprep/processor/pseudonymizer/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 10:46:57.000000 logprep-6.3.0/logprep/processor/pseudonymizer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2724 2023-05-22 10:46:57.000000 logprep-6.3.0/logprep/processor/pseudonymizer/encrypter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16361 2023-05-22 10:46:57.000000 logprep-6.3.0/logprep/processor/pseudonymizer/processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2518 2023-05-22 10:46:57.000000 logprep-6.3.0/logprep/processor/pseudonymizer/rule.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 10:47:03.636559 logprep-6.3.0/logprep/processor/requester/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 10:46:57.000000 logprep-6.3.0/logprep/processor/requester/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3963 2023-05-22 10:46:57.000000 logprep-6.3.0/logprep/processor/requester/processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7290 2023-05-22 10:46:57.000000 logprep-6.3.0/logprep/processor/requester/rule.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 10:47:03.636559 logprep-6.3.0/logprep/processor/selective_extractor/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 10:46:57.000000 logprep-6.3.0/logprep/processor/selective_extractor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3067 2023-05-22 10:46:57.000000 logprep-6.3.0/logprep/processor/selective_extractor/processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6078 2023-05-22 10:46:57.000000 logprep-6.3.0/logprep/processor/selective_extractor/rule.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 10:47:03.636559 logprep-6.3.0/logprep/processor/string_splitter/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 10:46:57.000000 logprep-6.3.0/logprep/processor/string_splitter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1886 2023-05-22 10:46:57.000000 logprep-6.3.0/logprep/processor/string_splitter/processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1527 2023-05-22 10:46:57.000000 logprep-6.3.0/logprep/processor/string_splitter/rule.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 10:47:03.636559 logprep-6.3.0/logprep/processor/template_replacer/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 10:46:57.000000 logprep-6.3.0/logprep/processor/template_replacer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6064 2023-05-22 10:46:57.000000 logprep-6.3.0/logprep/processor/template_replacer/processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      924 2023-05-22 10:46:57.000000 logprep-6.3.0/logprep/processor/template_replacer/rule.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 10:47:03.636559 logprep-6.3.0/logprep/processor/timestamp_differ/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 10:46:57.000000 logprep-6.3.0/logprep/processor/timestamp_differ/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3399 2023-05-22 10:46:57.000000 logprep-6.3.0/logprep/processor/timestamp_differ/processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4037 2023-05-22 10:46:57.000000 logprep-6.3.0/logprep/processor/timestamp_differ/rule.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 10:47:03.636559 logprep-6.3.0/logprep/processor/timestamper/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 10:46:57.000000 logprep-6.3.0/logprep/processor/timestamper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2950 2023-05-22 10:46:57.000000 logprep-6.3.0/logprep/processor/timestamper/processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4242 2023-05-22 10:46:57.000000 logprep-6.3.0/logprep/processor/timestamper/rule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4985 2023-05-22 10:46:57.000000 logprep-6.3.0/logprep/registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8561 2023-05-22 10:46:57.000000 logprep-6.3.0/logprep/run_logprep.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11023 2023-05-22 10:46:57.000000 logprep-6.3.0/logprep/runner.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 10:47:03.640559 logprep-6.3.0/logprep/util/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 10:46:57.000000 logprep-6.3.0/logprep/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2526 2023-05-22 10:46:57.000000 logprep-6.3.0/logprep/util/aggregating_logger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 10:47:03.640559 logprep-6.3.0/logprep/util/auto_rule_tester/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 10:46:57.000000 logprep-6.3.0/logprep/util/auto_rule_tester/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17268 2023-05-22 10:46:57.000000 logprep-6.3.0/logprep/util/auto_rule_tester/auto_rule_corpus_tester.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26980 2023-05-22 10:46:57.000000 logprep-6.3.0/logprep/util/auto_rule_tester/auto_rule_tester.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8157 2023-05-22 10:46:57.000000 logprep-6.3.0/logprep/util/auto_rule_tester/grok_pattern_replacer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-05-22 10:46:57.000000 logprep-6.3.0/logprep/util/cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19307 2023-05-22 10:46:57.000000 logprep-6.3.0/logprep/util/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)      704 2023-05-22 10:46:57.000000 logprep-6.3.0/logprep/util/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4950 2023-05-22 10:46:57.000000 logprep-6.3.0/logprep/util/getter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 10:47:03.640559 logprep-6.3.0/logprep/util/grok/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 10:46:57.000000 logprep-6.3.0/logprep/util/grok/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8200 2023-05-22 10:46:57.000000 logprep-6.3.0/logprep/util/grok/grok.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 10:47:03.616558 logprep-6.3.0/logprep/util/grok/patterns/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 10:47:03.640559 logprep-6.3.0/logprep/util/grok/patterns/ecs-v1/
+-rw-r--r--   0 runner    (1001) docker     (123)     4741 2023-05-22 10:46:57.000000 logprep-6.3.0/logprep/util/grok/patterns/ecs-v1/aws
+-rw-r--r--   0 runner    (1001) docker     (123)     5852 2023-05-22 10:46:57.000000 logprep-6.3.0/logprep/util/grok/patterns/ecs-v1/bacula
+-rw-r--r--   0 runner    (1001) docker     (123)      977 2023-05-22 10:46:57.000000 logprep-6.3.0/logprep/util/grok/patterns/ecs-v1/bind
+-rw-r--r--   0 runner    (1001) docker     (123)     4612 2023-05-22 10:46:57.000000 logprep-6.3.0/logprep/util/grok/patterns/ecs-v1/bro
+-rw-r--r--   0 runner    (1001) docker     (123)     1849 2023-05-22 10:46:57.000000 logprep-6.3.0/logprep/util/grok/patterns/ecs-v1/exim
+-rw-r--r--   0 runner    (1001) docker     (123)    15471 2023-05-22 10:46:57.000000 logprep-6.3.0/logprep/util/grok/patterns/ecs-v1/firewalls
+-rw-r--r--   0 runner    (1001) docker     (123)     5514 2023-05-22 10:46:57.000000 logprep-6.3.0/logprep/util/grok/patterns/ecs-v1/grok-patterns
+-rw-r--r--   0 runner    (1001) docker     (123)     4015 2023-05-22 10:46:57.000000 logprep-6.3.0/logprep/util/grok/patterns/ecs-v1/haproxy
+-rw-r--r--   0 runner    (1001) docker     (123)     1411 2023-05-22 10:46:57.000000 logprep-6.3.0/logprep/util/grok/patterns/ecs-v1/httpd
+-rw-r--r--   0 runner    (1001) docker     (123)     2223 2023-05-22 10:46:57.000000 logprep-6.3.0/logprep/util/grok/patterns/ecs-v1/java
+-rw-r--r--   0 runner    (1001) docker     (123)     1893 2023-05-22 10:46:57.000000 logprep-6.3.0/logprep/util/grok/patterns/ecs-v1/junos
+-rw-r--r--   0 runner    (1001) docker     (123)     1143 2023-05-22 10:46:57.000000 logprep-6.3.0/logprep/util/grok/patterns/ecs-v1/linux-syslog
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-05-22 10:46:57.000000 logprep-6.3.0/logprep/util/grok/patterns/ecs-v1/maven
+-rw-r--r--   0 runner    (1001) docker     (123)      206 2023-05-22 10:46:57.000000 logprep-6.3.0/logprep/util/grok/patterns/ecs-v1/mcollective
+-rw-r--r--   0 runner    (1001) docker     (123)      842 2023-05-22 10:46:57.000000 logprep-6.3.0/logprep/util/grok/patterns/ecs-v1/mongodb
+-rw-r--r--   0 runner    (1001) docker     (123)    10242 2023-05-22 10:46:57.000000 logprep-6.3.0/logprep/util/grok/patterns/ecs-v1/nagios
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-05-22 10:46:57.000000 logprep-6.3.0/logprep/util/grok/patterns/ecs-v1/postgresql
+-rw-r--r--   0 runner    (1001) docker     (123)     1137 2023-05-22 10:46:57.000000 logprep-6.3.0/logprep/util/grok/patterns/ecs-v1/rails
+-rw-r--r--   0 runner    (1001) docker     (123)      302 2023-05-22 10:46:57.000000 logprep-6.3.0/logprep/util/grok/patterns/ecs-v1/redis
+-rw-r--r--   0 runner    (1001) docker     (123)      214 2023-05-22 10:46:57.000000 logprep-6.3.0/logprep/util/grok/patterns/ecs-v1/ruby
+-rw-r--r--   0 runner    (1001) docker     (123)      637 2023-05-22 10:46:57.000000 logprep-6.3.0/logprep/util/grok/patterns/ecs-v1/squid
+-rw-r--r--   0 runner    (1001) docker     (123)     5366 2023-05-22 10:46:57.000000 logprep-6.3.0/logprep/util/grok/patterns/ecs-v1/zeek
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 10:47:03.644559 logprep-6.3.0/logprep/util/grok/patterns/legacy/
+-rw-r--r--   0 runner    (1001) docker     (123)     1839 2023-05-22 10:46:57.000000 logprep-6.3.0/logprep/util/grok/patterns/legacy/aws
+-rw-r--r--   0 runner    (1001) docker     (123)     4833 2023-05-22 10:46:57.000000 logprep-6.3.0/logprep/util/grok/patterns/legacy/bacula
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-05-22 10:46:57.000000 logprep-6.3.0/logprep/util/grok/patterns/legacy/bind
+-rw-r--r--   0 runner    (1001) docker     (123)     2154 2023-05-22 10:46:57.000000 logprep-6.3.0/logprep/util/grok/patterns/legacy/bro
+-rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-05-22 10:46:57.000000 logprep-6.3.0/logprep/util/grok/patterns/legacy/exim
+-rw-r--r--   0 runner    (1001) docker     (123)    10109 2023-05-22 10:46:57.000000 logprep-6.3.0/logprep/util/grok/patterns/legacy/firewalls
+-rw-r--r--   0 runner    (1001) docker     (123)     5402 2023-05-22 10:46:57.000000 logprep-6.3.0/logprep/util/grok/patterns/legacy/grok-patterns
+-rw-r--r--   0 runner    (1001) docker     (123)     3252 2023-05-22 10:46:57.000000 logprep-6.3.0/logprep/util/grok/patterns/legacy/haproxy
+-rw-r--r--   0 runner    (1001) docker     (123)      998 2023-05-22 10:46:57.000000 logprep-6.3.0/logprep/util/grok/patterns/legacy/httpd
+-rw-r--r--   0 runner    (1001) docker     (123)     1193 2023-05-22 10:46:57.000000 logprep-6.3.0/logprep/util/grok/patterns/legacy/java
+-rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-05-22 10:46:57.000000 logprep-6.3.0/logprep/util/grok/patterns/legacy/junos
+-rw-r--r--   0 runner    (1001) docker     (123)     1037 2023-05-22 10:46:57.000000 logprep-6.3.0/logprep/util/grok/patterns/legacy/linux-syslog
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-05-22 10:46:57.000000 logprep-6.3.0/logprep/util/grok/patterns/legacy/maven
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-22 10:46:57.000000 logprep-6.3.0/logprep/util/grok/patterns/legacy/mcollective
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-05-22 10:46:57.000000 logprep-6.3.0/logprep/util/grok/patterns/legacy/mcollective-patterns
+-rw-r--r--   0 runner    (1001) docker     (123)      614 2023-05-22 10:46:57.000000 logprep-6.3.0/logprep/util/grok/patterns/legacy/mongodb
+-rw-r--r--   0 runner    (1001) docker     (123)     9601 2023-05-22 10:46:57.000000 logprep-6.3.0/logprep/util/grok/patterns/legacy/nagios
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-05-22 10:46:57.000000 logprep-6.3.0/logprep/util/grok/patterns/legacy/postgresql
+-rw-r--r--   0 runner    (1001) docker     (123)      845 2023-05-22 10:46:57.000000 logprep-6.3.0/logprep/util/grok/patterns/legacy/rails
+-rw-r--r--   0 runner    (1001) docker     (123)      224 2023-05-22 10:46:57.000000 logprep-6.3.0/logprep/util/grok/patterns/legacy/redis
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-05-22 10:46:57.000000 logprep-6.3.0/logprep/util/grok/patterns/legacy/ruby
+-rw-r--r--   0 runner    (1001) docker     (123)      411 2023-05-22 10:46:57.000000 logprep-6.3.0/logprep/util/grok/patterns/legacy/squid
+-rw-r--r--   0 runner    (1001) docker     (123)     3015 2023-05-22 10:46:57.000000 logprep-6.3.0/logprep/util/grok_pattern_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)      666 2023-05-22 10:46:57.000000 logprep-6.3.0/logprep/util/hasher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9641 2023-05-22 10:46:57.000000 logprep-6.3.0/logprep/util/helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2735 2023-05-22 10:46:57.000000 logprep-6.3.0/logprep/util/json_handling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3411 2023-05-22 10:46:57.000000 logprep-6.3.0/logprep/util/log_aggregator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      814 2023-05-22 10:46:57.000000 logprep-6.3.0/logprep/util/multiprocessing_log_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-05-22 10:46:57.000000 logprep-6.3.0/logprep/util/pipeline_profiler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12543 2023-05-22 10:46:57.000000 logprep-6.3.0/logprep/util/pre_detector_rule_matching_tester.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5150 2023-05-22 10:46:57.000000 logprep-6.3.0/logprep/util/processor_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3608 2023-05-22 10:46:57.000000 logprep-6.3.0/logprep/util/prometheus_exporter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5644 2023-05-22 10:46:57.000000 logprep-6.3.0/logprep/util/rule_dry_runner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7634 2023-05-22 10:46:57.000000 logprep-6.3.0/logprep/util/schema_and_rule_checker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2665 2023-05-22 10:46:57.000000 logprep-6.3.0/logprep/util/time.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2228 2023-05-22 10:46:57.000000 logprep-6.3.0/logprep/util/time_measurement.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6602 2023-05-22 10:46:57.000000 logprep-6.3.0/logprep/util/validators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 10:47:03.620558 logprep-6.3.0/logprep.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    17607 2023-05-22 10:47:03.000000 logprep-6.3.0/logprep.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    17845 2023-05-22 10:47:03.000000 logprep-6.3.0/logprep.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 10:47:03.000000 logprep-6.3.0/logprep.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-05-22 10:47:03.000000 logprep-6.3.0/logprep.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      473 2023-05-22 10:47:03.000000 logprep-6.3.0/logprep.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-22 10:47:03.000000 logprep-6.3.0/logprep.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-05-22 10:46:57.000000 logprep-6.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      201 2023-05-22 10:47:03.664559 logprep-6.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1421 2023-05-22 10:46:57.000000 logprep-6.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 10:47:03.644559 logprep-6.3.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 10:46:57.000000 logprep-6.3.0/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 10:47:03.644559 logprep-6.3.0/tests/acceptance/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 10:46:57.000000 logprep-6.3.0/tests/acceptance/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1846 2023-05-22 10:46:57.000000 logprep-6.3.0/tests/acceptance/test_amides.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1718 2023-05-22 10:46:57.000000 logprep-6.3.0/tests/acceptance/test_config_refresh.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3390 2023-05-22 10:46:57.000000 logprep-6.3.0/tests/acceptance/test_file_input.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9180 2023-05-22 10:46:57.000000 logprep-6.3.0/tests/acceptance/test_full_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4675 2023-05-22 10:46:57.000000 logprep-6.3.0/tests/acceptance/test_http_input.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5163 2023-05-22 10:46:57.000000 logprep-6.3.0/tests/acceptance/test_multiple_outputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19060 2023-05-22 10:46:57.000000 logprep-6.3.0/tests/acceptance/test_pre_detection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1834 2023-05-22 10:46:57.000000 logprep-6.3.0/tests/acceptance/test_preprocessing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2839 2023-05-22 10:46:57.000000 logprep-6.3.0/tests/acceptance/test_selective_extractor_full_pipeline_pass.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1973 2023-05-22 10:46:57.000000 logprep-6.3.0/tests/acceptance/test_wineventlog_normalization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3192 2023-05-22 10:46:57.000000 logprep-6.3.0/tests/acceptance/test_wineventlog_processing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2751 2023-05-22 10:46:57.000000 logprep-6.3.0/tests/acceptance/test_wineventlog_pseudonymization.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10368 2023-05-22 10:46:57.000000 logprep-6.3.0/tests/acceptance/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 10:47:03.644559 logprep-6.3.0/tests/ci/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 10:46:57.000000 logprep-6.3.0/tests/ci/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 10:47:03.644559 logprep-6.3.0/tests/ci/runner-image/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 10:46:57.000000 logprep-6.3.0/tests/ci/runner-image/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 10:47:03.644559 logprep-6.3.0/tests/ci/runner-image/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 10:46:57.000000 logprep-6.3.0/tests/ci/runner-image/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-05-22 10:46:57.000000 logprep-6.3.0/tests/ci/runner-image/scripts/compare_json.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 10:47:03.648559 logprep-6.3.0/tests/testdata/
+-rw-r--r--   0 runner    (1001) docker     (123)     1534 2023-05-22 10:46:57.000000 logprep-6.3.0/tests/testdata/ConfigurationForTest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      655 2023-05-22 10:46:57.000000 logprep-6.3.0/tests/testdata/FilledTempFile.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 10:46:57.000000 logprep-6.3.0/tests/testdata/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      807 2023-05-22 10:46:57.000000 logprep-6.3.0/tests/testdata/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-05-22 10:46:57.000000 logprep-6.3.0/tests/testdata/ruledata.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 10:47:03.648559 logprep-6.3.0/tests/testdata/unit/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 10:46:57.000000 logprep-6.3.0/tests/testdata/unit/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 10:47:03.648559 logprep-6.3.0/tests/testdata/unit/clusterer/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 10:46:57.000000 logprep-6.3.0/tests/testdata/unit/clusterer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12733 2023-05-22 10:46:57.000000 logprep-6.3.0/tests/testdata/unit/clusterer/test_data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 10:47:03.648559 logprep-6.3.0/tests/unit/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 10:46:57.000000 logprep-6.3.0/tests/unit/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 10:47:03.648559 logprep-6.3.0/tests/unit/component/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 10:46:57.000000 logprep-6.3.0/tests/unit/component/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1693 2023-05-22 10:46:57.000000 logprep-6.3.0/tests/unit/component/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 10:47:03.648559 logprep-6.3.0/tests/unit/connector/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 10:46:57.000000 logprep-6.3.0/tests/unit/connector/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21616 2023-05-22 10:46:57.000000 logprep-6.3.0/tests/unit/connector/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2226 2023-05-22 10:46:57.000000 logprep-6.3.0/tests/unit/connector/test_confluent_kafka_common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7303 2023-05-22 10:46:57.000000 logprep-6.3.0/tests/unit/connector/test_confluent_kafka_input.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7315 2023-05-22 10:46:57.000000 logprep-6.3.0/tests/unit/connector/test_confluent_kafka_output.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1761 2023-05-22 10:46:57.000000 logprep-6.3.0/tests/unit/connector/test_console_output.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1495 2023-05-22 10:46:57.000000 logprep-6.3.0/tests/unit/connector/test_dummy_input.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3545 2023-05-22 10:46:57.000000 logprep-6.3.0/tests/unit/connector/test_dummy_output.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9100 2023-05-22 10:46:57.000000 logprep-6.3.0/tests/unit/connector/test_elasticsearch_output.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9926 2023-05-22 10:46:57.000000 logprep-6.3.0/tests/unit/connector/test_file_input_default_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3523 2023-05-22 10:46:57.000000 logprep-6.3.0/tests/unit/connector/test_file_input_not_tailing_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2532 2023-05-22 10:46:57.000000 logprep-6.3.0/tests/unit/connector/test_file_input_start_at_end_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6314 2023-05-22 10:46:57.000000 logprep-6.3.0/tests/unit/connector/test_http_input.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2071 2023-05-22 10:46:57.000000 logprep-6.3.0/tests/unit/connector/test_json_input.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1985 2023-05-22 10:46:57.000000 logprep-6.3.0/tests/unit/connector/test_jsonl_input.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5034 2023-05-22 10:46:57.000000 logprep-6.3.0/tests/unit/connector/test_jsonl_output.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9276 2023-05-22 10:46:57.000000 logprep-6.3.0/tests/unit/connector/test_opensearch_output.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10265 2023-05-22 10:46:57.000000 logprep-6.3.0/tests/unit/connector/test_s3_output.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 10:47:03.648559 logprep-6.3.0/tests/unit/exceptions/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 10:46:57.000000 logprep-6.3.0/tests/unit/exceptions/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 10:47:03.648559 logprep-6.3.0/tests/unit/exceptions/processor/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 10:46:57.000000 logprep-6.3.0/tests/unit/exceptions/processor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2167 2023-05-22 10:46:57.000000 logprep-6.3.0/tests/unit/exceptions/processor/test_processing_warning.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 10:47:03.648559 logprep-6.3.0/tests/unit/filter/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 10:46:57.000000 logprep-6.3.0/tests/unit/filter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19683 2023-05-22 10:46:57.000000 logprep-6.3.0/tests/unit/filter/test_filter_expression.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20548 2023-05-22 10:46:57.000000 logprep-6.3.0/tests/unit/filter/test_lucene_filter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 10:47:03.652559 logprep-6.3.0/tests/unit/framework/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 10:46:57.000000 logprep-6.3.0/tests/unit/framework/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 10:47:03.652559 logprep-6.3.0/tests/unit/framework/rule_tree/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 10:46:57.000000 logprep-6.3.0/tests/unit/framework/rule_tree/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1894 2023-05-22 10:46:57.000000 logprep-6.3.0/tests/unit/framework/rule_tree/test_node.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27846 2023-05-22 10:46:57.000000 logprep-6.3.0/tests/unit/framework/rule_tree/test_rule_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19943 2023-05-22 10:46:57.000000 logprep-6.3.0/tests/unit/framework/rule_tree/test_rule_tree.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39696 2023-05-22 10:46:57.000000 logprep-6.3.0/tests/unit/framework/test_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9032 2023-05-22 10:46:57.000000 logprep-6.3.0/tests/unit/framework/test_pipeline_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 10:47:03.652559 logprep-6.3.0/tests/unit/metrics/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 10:46:57.000000 logprep-6.3.0/tests/unit/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8285 2023-05-22 10:46:57.000000 logprep-6.3.0/tests/unit/metrics/test_metric_exposer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22193 2023-05-22 10:46:57.000000 logprep-6.3.0/tests/unit/metrics/test_metric_targets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5612 2023-05-22 10:46:57.000000 logprep-6.3.0/tests/unit/metrics/test_metrics.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 10:47:03.652559 logprep-6.3.0/tests/unit/processor/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 10:46:57.000000 logprep-6.3.0/tests/unit/processor/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 10:47:03.652559 logprep-6.3.0/tests/unit/processor/amides/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 10:46:57.000000 logprep-6.3.0/tests/unit/processor/amides/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8119 2023-05-22 10:46:57.000000 logprep-6.3.0/tests/unit/processor/amides/test_amides.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2951 2023-05-22 10:46:57.000000 logprep-6.3.0/tests/unit/processor/amides/test_amides_rule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4396 2023-05-22 10:46:57.000000 logprep-6.3.0/tests/unit/processor/amides/test_detection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1760 2023-05-22 10:46:57.000000 logprep-6.3.0/tests/unit/processor/amides/test_normalize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8041 2023-05-22 10:46:57.000000 logprep-6.3.0/tests/unit/processor/amides/test_tokenizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14110 2023-05-22 10:46:57.000000 logprep-6.3.0/tests/unit/processor/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 10:47:03.652559 logprep-6.3.0/tests/unit/processor/calculator/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 10:46:57.000000 logprep-6.3.0/tests/unit/processor/calculator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11779 2023-05-22 10:46:57.000000 logprep-6.3.0/tests/unit/processor/calculator/test_calculator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1884 2023-05-22 10:46:57.000000 logprep-6.3.0/tests/unit/processor/calculator/test_calculator_rule.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 10:47:03.652559 logprep-6.3.0/tests/unit/processor/clusterer/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 10:46:57.000000 logprep-6.3.0/tests/unit/processor/clusterer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7217 2023-05-22 10:46:57.000000 logprep-6.3.0/tests/unit/processor/clusterer/test_clusterer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3076 2023-05-22 10:46:57.000000 logprep-6.3.0/tests/unit/processor/clusterer/test_clusterer_rule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4796 2023-05-22 10:46:57.000000 logprep-6.3.0/tests/unit/processor/clusterer/test_clusterer_signature_phase.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 10:47:03.652559 logprep-6.3.0/tests/unit/processor/concatenator/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 10:46:57.000000 logprep-6.3.0/tests/unit/processor/concatenator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6963 2023-05-22 10:46:57.000000 logprep-6.3.0/tests/unit/processor/concatenator/test_concatenator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11216 2023-05-22 10:46:57.000000 logprep-6.3.0/tests/unit/processor/concatenator/test_concatenator_rule.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 10:47:03.652559 logprep-6.3.0/tests/unit/processor/datetime_extractor/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 10:46:57.000000 logprep-6.3.0/tests/unit/processor/datetime_extractor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8165 2023-05-22 10:46:57.000000 logprep-6.3.0/tests/unit/processor/datetime_extractor/test_datetime_extractor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5869 2023-05-22 10:46:57.000000 logprep-6.3.0/tests/unit/processor/datetime_extractor/test_datetime_extractor_rule.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 10:47:03.652559 logprep-6.3.0/tests/unit/processor/deleter/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 10:46:57.000000 logprep-6.3.0/tests/unit/processor/deleter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      893 2023-05-22 10:46:57.000000 logprep-6.3.0/tests/unit/processor/deleter/test_deleter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3527 2023-05-22 10:46:57.000000 logprep-6.3.0/tests/unit/processor/deleter/test_deleter_rule.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 10:47:03.652559 logprep-6.3.0/tests/unit/processor/dissector/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 10:46:57.000000 logprep-6.3.0/tests/unit/processor/dissector/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23002 2023-05-22 10:46:57.000000 logprep-6.3.0/tests/unit/processor/dissector/test_dissector.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17960 2023-05-22 10:46:57.000000 logprep-6.3.0/tests/unit/processor/dissector/test_dissector_rule.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 10:47:03.656559 logprep-6.3.0/tests/unit/processor/domain_label_extractor/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 10:46:57.000000 logprep-6.3.0/tests/unit/processor/domain_label_extractor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13265 2023-05-22 10:46:57.000000 logprep-6.3.0/tests/unit/processor/domain_label_extractor/test_domain_label_extractor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5936 2023-05-22 10:46:57.000000 logprep-6.3.0/tests/unit/processor/domain_label_extractor/test_domain_label_extractor_rule.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 10:47:03.656559 logprep-6.3.0/tests/unit/processor/domain_resolver/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 10:46:57.000000 logprep-6.3.0/tests/unit/processor/domain_resolver/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11812 2023-05-22 10:46:57.000000 logprep-6.3.0/tests/unit/processor/domain_resolver/test_domain_resolver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2487 2023-05-22 10:46:57.000000 logprep-6.3.0/tests/unit/processor/domain_resolver/test_domain_resolver_rule.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 10:47:03.656559 logprep-6.3.0/tests/unit/processor/dropper/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 10:46:57.000000 logprep-6.3.0/tests/unit/processor/dropper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6277 2023-05-22 10:46:57.000000 logprep-6.3.0/tests/unit/processor/dropper/test_dropper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4523 2023-05-22 10:46:57.000000 logprep-6.3.0/tests/unit/processor/dropper/test_dropper_rule.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 10:47:03.656559 logprep-6.3.0/tests/unit/processor/field_manager/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 10:46:57.000000 logprep-6.3.0/tests/unit/processor/field_manager/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18589 2023-05-22 10:46:57.000000 logprep-6.3.0/tests/unit/processor/field_manager/test_field_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4214 2023-05-22 10:46:57.000000 logprep-6.3.0/tests/unit/processor/field_manager/test_field_manager_rule.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 10:47:03.656559 logprep-6.3.0/tests/unit/processor/generic_adder/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 10:46:57.000000 logprep-6.3.0/tests/unit/processor/generic_adder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29997 2023-05-22 10:46:57.000000 logprep-6.3.0/tests/unit/processor/generic_adder/test_generic_adder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3247 2023-05-22 10:46:57.000000 logprep-6.3.0/tests/unit/processor/generic_adder/test_generic_adder_rule.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 10:47:03.656559 logprep-6.3.0/tests/unit/processor/generic_resolver/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 10:46:57.000000 logprep-6.3.0/tests/unit/processor/generic_resolver/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14079 2023-05-22 10:46:57.000000 logprep-6.3.0/tests/unit/processor/generic_resolver/test_generic_resolver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6408 2023-05-22 10:46:57.000000 logprep-6.3.0/tests/unit/processor/generic_resolver/test_generic_resolver_rule.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 10:47:03.656559 logprep-6.3.0/tests/unit/processor/geoip_enricher/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 10:46:57.000000 logprep-6.3.0/tests/unit/processor/geoip_enricher/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14996 2023-05-22 10:46:57.000000 logprep-6.3.0/tests/unit/processor/geoip_enricher/test_geoip_enricher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2492 2023-05-22 10:46:57.000000 logprep-6.3.0/tests/unit/processor/geoip_enricher/test_geoip_enricher_rule.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 10:47:03.656559 logprep-6.3.0/tests/unit/processor/grokker/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 10:46:57.000000 logprep-6.3.0/tests/unit/processor/grokker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7375 2023-05-22 10:46:57.000000 logprep-6.3.0/tests/unit/processor/grokker/test_grok.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13924 2023-05-22 10:46:57.000000 logprep-6.3.0/tests/unit/processor/grokker/test_grokker.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10901 2023-05-22 10:46:57.000000 logprep-6.3.0/tests/unit/processor/grokker/test_grokker_rule.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 10:47:03.656559 logprep-6.3.0/tests/unit/processor/hyperscan_resolver/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 10:46:57.000000 logprep-6.3.0/tests/unit/processor/hyperscan_resolver/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23145 2023-05-22 10:46:57.000000 logprep-6.3.0/tests/unit/processor/hyperscan_resolver/test_hyperscan_resolver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6339 2023-05-22 10:46:57.000000 logprep-6.3.0/tests/unit/processor/hyperscan_resolver/test_hyperscan_resolver_rule.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 10:47:03.656559 logprep-6.3.0/tests/unit/processor/ip_informer/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 10:46:57.000000 logprep-6.3.0/tests/unit/processor/ip_informer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13607 2023-05-22 10:46:57.000000 logprep-6.3.0/tests/unit/processor/ip_informer/test_ip_informer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2110 2023-05-22 10:46:57.000000 logprep-6.3.0/tests/unit/processor/ip_informer/test_ip_informer_rule.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 10:47:03.656559 logprep-6.3.0/tests/unit/processor/labeler/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 10:46:57.000000 logprep-6.3.0/tests/unit/processor/labeler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9177 2023-05-22 10:46:57.000000 logprep-6.3.0/tests/unit/processor/labeler/test_labeler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9016 2023-05-22 10:46:57.000000 logprep-6.3.0/tests/unit/processor/labeler/test_labeler_rule.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12544 2023-05-22 10:46:57.000000 logprep-6.3.0/tests/unit/processor/labeler/test_labeling_schema.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 10:47:03.656559 logprep-6.3.0/tests/unit/processor/list_comparison/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 10:46:57.000000 logprep-6.3.0/tests/unit/processor/list_comparison/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11202 2023-05-22 10:46:57.000000 logprep-6.3.0/tests/unit/processor/list_comparison/test_list_comparison.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3623 2023-05-22 10:46:57.000000 logprep-6.3.0/tests/unit/processor/list_comparison/test_list_comparison_rule.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 10:47:03.660559 logprep-6.3.0/tests/unit/processor/normalizer/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 10:46:57.000000 logprep-6.3.0/tests/unit/processor/normalizer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38341 2023-05-22 10:46:57.000000 logprep-6.3.0/tests/unit/processor/normalizer/test_normalizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11123 2023-05-22 10:46:57.000000 logprep-6.3.0/tests/unit/processor/normalizer/test_normalizer_rule.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 10:47:03.660559 logprep-6.3.0/tests/unit/processor/pre_detector/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 10:46:57.000000 logprep-6.3.0/tests/unit/processor/pre_detector/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5419 2023-05-22 10:46:57.000000 logprep-6.3.0/tests/unit/processor/pre_detector/test_ip_alerter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13961 2023-05-22 10:46:57.000000 logprep-6.3.0/tests/unit/processor/pre_detector/test_pre_detector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6921 2023-05-22 10:46:57.000000 logprep-6.3.0/tests/unit/processor/pre_detector/test_pre_detector_rule.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 10:47:03.660559 logprep-6.3.0/tests/unit/processor/pseudonymizer/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 10:46:57.000000 logprep-6.3.0/tests/unit/processor/pseudonymizer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2974 2023-05-22 10:46:57.000000 logprep-6.3.0/tests/unit/processor/pseudonymizer/test_encrypter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29770 2023-05-22 10:46:57.000000 logprep-6.3.0/tests/unit/processor/pseudonymizer/test_pseudonymizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2691 2023-05-22 10:46:57.000000 logprep-6.3.0/tests/unit/processor/pseudonymizer/test_pseudonymizer_rule.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 10:47:03.660559 logprep-6.3.0/tests/unit/processor/requester/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 10:46:57.000000 logprep-6.3.0/tests/unit/processor/requester/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12431 2023-05-22 10:46:57.000000 logprep-6.3.0/tests/unit/processor/requester/test_requester.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8142 2023-05-22 10:46:57.000000 logprep-6.3.0/tests/unit/processor/requester/test_requester_rule.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 10:47:03.660559 logprep-6.3.0/tests/unit/processor/selective_extractor/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 10:46:57.000000 logprep-6.3.0/tests/unit/processor/selective_extractor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5541 2023-05-22 10:46:57.000000 logprep-6.3.0/tests/unit/processor/selective_extractor/test_selective_extractor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11040 2023-05-22 10:46:57.000000 logprep-6.3.0/tests/unit/processor/selective_extractor/test_selective_extractor_rule.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 10:47:03.660559 logprep-6.3.0/tests/unit/processor/string_splitter/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 10:46:57.000000 logprep-6.3.0/tests/unit/processor/string_splitter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2751 2023-05-22 10:46:57.000000 logprep-6.3.0/tests/unit/processor/string_splitter/test_string_splitter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2134 2023-05-22 10:46:57.000000 logprep-6.3.0/tests/unit/processor/string_splitter/test_string_splitter_rule.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 10:47:03.660559 logprep-6.3.0/tests/unit/processor/template_replacer/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 10:46:57.000000 logprep-6.3.0/tests/unit/processor/template_replacer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6683 2023-05-22 10:46:57.000000 logprep-6.3.0/tests/unit/processor/template_replacer/test_template_replacer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1613 2023-05-22 10:46:57.000000 logprep-6.3.0/tests/unit/processor/test_processor_rule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8157 2023-05-22 10:46:57.000000 logprep-6.3.0/tests/unit/processor/test_processor_strategy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 10:47:03.660559 logprep-6.3.0/tests/unit/processor/timestamp_differ/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 10:46:57.000000 logprep-6.3.0/tests/unit/processor/timestamp_differ/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16573 2023-05-22 10:46:57.000000 logprep-6.3.0/tests/unit/processor/timestamp_differ/test_timestamp_differ.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4283 2023-05-22 10:46:57.000000 logprep-6.3.0/tests/unit/processor/timestamp_differ/test_timestamp_differ_rule.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 10:47:03.660559 logprep-6.3.0/tests/unit/processor/timestamper/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 10:46:57.000000 logprep-6.3.0/tests/unit/processor/timestamper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10055 2023-05-22 10:46:57.000000 logprep-6.3.0/tests/unit/processor/timestamper/test_timestamper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2120 2023-05-22 10:46:57.000000 logprep-6.3.0/tests/unit/processor/timestamper/test_timestamper_rule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6228 2023-05-22 10:46:57.000000 logprep-6.3.0/tests/unit/test_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5507 2023-05-22 10:46:57.000000 logprep-6.3.0/tests/unit/test_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11779 2023-05-22 10:46:57.000000 logprep-6.3.0/tests/unit/test_run_logprep.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18858 2023-05-22 10:46:57.000000 logprep-6.3.0/tests/unit/test_runner.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 10:47:03.664559 logprep-6.3.0/tests/unit/util/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 10:46:57.000000 logprep-6.3.0/tests/unit/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19327 2023-05-22 10:46:57.000000 logprep-6.3.0/tests/unit/util/test_auto_rule_corpus_tester.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10250 2023-05-22 10:46:57.000000 logprep-6.3.0/tests/unit/util/test_auto_rule_tester.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1593 2023-05-22 10:46:57.000000 logprep-6.3.0/tests/unit/util/test_cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39375 2023-05-22 10:46:57.000000 logprep-6.3.0/tests/unit/util/test_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16243 2023-05-22 10:46:57.000000 logprep-6.3.0/tests/unit/util/test_getter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3097 2023-05-22 10:46:57.000000 logprep-6.3.0/tests/unit/util/test_grok_pattern_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)      469 2023-05-22 10:46:57.000000 logprep-6.3.0/tests/unit/util/test_hasher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7897 2023-05-22 10:46:57.000000 logprep-6.3.0/tests/unit/util/test_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7246 2023-05-22 10:46:57.000000 logprep-6.3.0/tests/unit/util/test_helper_add_field.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6394 2023-05-22 10:46:57.000000 logprep-6.3.0/tests/unit/util/test_log_aggregator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5521 2023-05-22 10:46:57.000000 logprep-6.3.0/tests/unit/util/test_processor_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5762 2023-05-22 10:46:57.000000 logprep-6.3.0/tests/unit/util/test_prometheus_exporter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6740 2023-05-22 10:46:57.000000 logprep-6.3.0/tests/unit/util/test_rule_dry_runner.py
+-rw-r--r--   0 runner    (1001) docker     (123)      309 2023-05-22 10:46:57.000000 logprep-6.3.0/tests/unit/util/test_schema_and_rule_checker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2368 2023-05-22 10:46:57.000000 logprep-6.3.0/tests/unit/util/test_time.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4103 2023-05-22 10:46:57.000000 logprep-6.3.0/tests/unit/util/test_time_measurement.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16746 2023-05-22 10:46:57.000000 logprep-6.3.0/tests/unit/util/test_validators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1540 2023-05-22 10:46:57.000000 logprep-6.3.0/tests/unit/util/tests_json_handling.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 10:47:03.664559 logprep-6.3.0/tests/util/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 10:46:57.000000 logprep-6.3.0/tests/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3893 2023-05-22 10:46:57.000000 logprep-6.3.0/tests/util/testhelpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    81000 2023-05-22 10:46:57.000000 logprep-6.3.0/versioneer.py
```

### Comparing `logprep-6.2.0/LICENSE` & `logprep-6.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `logprep-6.2.0/PKG-INFO` & `logprep-6.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: logprep
-Version: 6.2.0
+Version: 6.3.0
 Summary: Logprep allows to collect, process and forward log messages from various data sources.
 Home-page: https://github.com/fkie-cad/Logprep
 Author: Logprep Team
 License: LGPL-2.1 license
 Project-URL: Homepage, https://github.com/fkie-cad/Logprep
 Project-URL: Documentation, https://logprep.readthedocs.io/en/latest/
 Platform: UNKNOWN
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: logprep Version: 6.2.0 Summary: Logprep allows to
+Metadata-Version: 2.1 Name: logprep Version: 6.3.0 Summary: Logprep allows to
 collect, process and forward log messages from various data sources. Home-page:
 https://github.com/fkie-cad/Logprep Author: Logprep Team License: LGPL-2.1
 license Project-URL: Homepage, https://github.com/fkie-cad/Logprep Project-URL:
 Documentation, https://logprep.readthedocs.io/en/latest/ Platform: UNKNOWN
 Classifier: Programming Language :: Python Classifier: Programming Language ::
 Python :: 3 Classifier: Programming Language :: Python :: 3.9 Classifier:
 Programming Language :: Python :: 3.10 Classifier: Programming Language ::
```

### Comparing `logprep-6.2.0/README.md` & `logprep-6.3.0/README.md`

 * *Files identical despite different names*

### Comparing `logprep-6.2.0/logprep/abc/component.py` & `logprep-6.3.0/logprep/abc/component.py`

 * *Files identical despite different names*

### Comparing `logprep-6.2.0/logprep/abc/connector.py` & `logprep-6.3.0/logprep/abc/connector.py`

 * *Files identical despite different names*

### Comparing `logprep-6.2.0/logprep/abc/getter.py` & `logprep-6.3.0/logprep/abc/getter.py`

 * *Files identical despite different names*

### Comparing `logprep-6.2.0/logprep/abc/input.py` & `logprep-6.3.0/logprep/abc/input.py`

 * *Files identical despite different names*

### Comparing `logprep-6.2.0/logprep/abc/output.py` & `logprep-6.3.0/logprep/abc/output.py`

 * *Files identical despite different names*

### Comparing `logprep-6.2.0/logprep/abc/processor.py` & `logprep-6.3.0/logprep/abc/processor.py`

 * *Files 2% similar despite different names*

```diff
@@ -273,20 +273,22 @@
         for field_ in fields:
             if field_ in dict_ and isinstance(dict_, dict):
                 dict_ = dict_[field_]
             else:
                 return False
         return True
 
-    def _handle_warning_error(self, event, rule, error):
+    def _handle_warning_error(self, event, rule, error, failure_tags=None):
         tags = get_dotted_field_value(event, "tags")
+        if failure_tags is None:
+            failure_tags = rule.failure_tags
         if tags is None:
-            add_and_overwrite(event, "tags", sorted(list({*rule.failure_tags})))
+            add_and_overwrite(event, "tags", sorted(list({*failure_tags})))
         else:
-            add_and_overwrite(event, "tags", sorted(list({*tags, *rule.failure_tags})))
+            add_and_overwrite(event, "tags", sorted(list({*tags, *failure_tags})))
         if isinstance(error, ProcessingWarning):
             self._logger.warning(str(error))
         else:
             self._logger.warning(str(ProcessingWarning(self, str(error), rule, event)))
 
     def _has_missing_values(self, event, rule, source_field_dict):
         missing_fields = list(
```

### Comparing `logprep-6.2.0/logprep/configuration.py` & `logprep-6.3.0/logprep/configuration.py`

 * *Files identical despite different names*

### Comparing `logprep-6.2.0/logprep/connector/confluent_kafka/input.py` & `logprep-6.3.0/logprep/connector/confluent_kafka/input.py`

 * *Files identical despite different names*

### Comparing `logprep-6.2.0/logprep/connector/confluent_kafka/output.py` & `logprep-6.3.0/logprep/connector/confluent_kafka/output.py`

 * *Files identical despite different names*

### Comparing `logprep-6.2.0/logprep/connector/console/output.py` & `logprep-6.3.0/logprep/connector/console/output.py`

 * *Files identical despite different names*

### Comparing `logprep-6.2.0/logprep/connector/dummy/input.py` & `logprep-6.3.0/logprep/connector/dummy/input.py`

 * *Files identical despite different names*

### Comparing `logprep-6.2.0/logprep/connector/dummy/output.py` & `logprep-6.3.0/logprep/connector/dummy/output.py`

 * *Files identical despite different names*

### Comparing `logprep-6.2.0/logprep/connector/elasticsearch/output.py` & `logprep-6.3.0/logprep/connector/elasticsearch/output.py`

 * *Files identical despite different names*

### Comparing `logprep-6.2.0/logprep/connector/file/input.py` & `logprep-6.3.0/logprep/connector/file/input.py`

 * *Files identical despite different names*

### Comparing `logprep-6.2.0/logprep/connector/http/input.py` & `logprep-6.3.0/logprep/connector/http/input.py`

 * *Files identical despite different names*

### Comparing `logprep-6.2.0/logprep/connector/json/input.py` & `logprep-6.3.0/logprep/connector/json/input.py`

 * *Files identical despite different names*

### Comparing `logprep-6.2.0/logprep/connector/jsonl/input.py` & `logprep-6.3.0/logprep/connector/jsonl/input.py`

 * *Files identical despite different names*

### Comparing `logprep-6.2.0/logprep/connector/jsonl/output.py` & `logprep-6.3.0/logprep/connector/jsonl/output.py`

 * *Files identical despite different names*

### Comparing `logprep-6.2.0/logprep/connector/opensearch/output.py` & `logprep-6.3.0/logprep/connector/opensearch/output.py`

 * *Files identical despite different names*

### Comparing `logprep-6.2.0/logprep/connector/s3/output.py` & `logprep-6.3.0/logprep/connector/s3/output.py`

 * *Files identical despite different names*

### Comparing `logprep-6.2.0/logprep/factory.py` & `logprep-6.3.0/logprep/factory.py`

 * *Files identical despite different names*

### Comparing `logprep-6.2.0/logprep/factory_error.py` & `logprep-6.3.0/logprep/factory_error.py`

 * *Files identical despite different names*

### Comparing `logprep-6.2.0/logprep/filter/expression/filter_expression.py` & `logprep-6.3.0/logprep/filter/expression/filter_expression.py`

 * *Files identical despite different names*

### Comparing `logprep-6.2.0/logprep/filter/lucene_filter.py` & `logprep-6.3.0/logprep/filter/lucene_filter.py`

 * *Files identical despite different names*

### Comparing `logprep-6.2.0/logprep/framework/pipeline.py` & `logprep-6.3.0/logprep/framework/pipeline.py`

 * *Files identical despite different names*

### Comparing `logprep-6.2.0/logprep/framework/pipeline_manager.py` & `logprep-6.3.0/logprep/framework/pipeline_manager.py`

 * *Files identical despite different names*

### Comparing `logprep-6.2.0/logprep/framework/rule_tree/node.py` & `logprep-6.3.0/logprep/framework/rule_tree/node.py`

 * *Files identical despite different names*

### Comparing `logprep-6.2.0/logprep/framework/rule_tree/rule_parser.py` & `logprep-6.3.0/logprep/framework/rule_tree/rule_parser.py`

 * *Files identical despite different names*

### Comparing `logprep-6.2.0/logprep/framework/rule_tree/rule_tree.py` & `logprep-6.3.0/logprep/framework/rule_tree/rule_tree.py`

 * *Files identical despite different names*

### Comparing `logprep-6.2.0/logprep/metrics/metric.py` & `logprep-6.3.0/logprep/metrics/metric.py`

 * *Files identical despite different names*

### Comparing `logprep-6.2.0/logprep/metrics/metric_exposer.py` & `logprep-6.3.0/logprep/metrics/metric_exposer.py`

 * *Files identical despite different names*

### Comparing `logprep-6.2.0/logprep/metrics/metric_targets.py` & `logprep-6.3.0/logprep/metrics/metric_targets.py`

 * *Files identical despite different names*

### Comparing `logprep-6.2.0/logprep/processor/amides/detection.py` & `logprep-6.3.0/logprep/processor/amides/detection.py`

 * *Files identical despite different names*

### Comparing `logprep-6.2.0/logprep/processor/amides/features.py` & `logprep-6.3.0/logprep/processor/amides/features.py`

 * *Files identical despite different names*

### Comparing `logprep-6.2.0/logprep/processor/amides/normalize.py` & `logprep-6.3.0/logprep/processor/amides/normalize.py`

 * *Files identical despite different names*

### Comparing `logprep-6.2.0/logprep/processor/amides/processor.py` & `logprep-6.3.0/logprep/processor/amides/processor.py`

 * *Files 2% similar despite different names*

```diff
@@ -51,52 +51,58 @@
 
 Models used by the `MisuseDetector` and `RuleAttributor` are currently generated by `scikit-learn`.
 Each trained model needs to be packed into a dictionary together with its corresponding feature extractor
 and scaler. Dictionaries are then pickled and compressed (.zip). The URI or path of the compressed models 
 file is given by the :code:`models_path` configuration parameter. An example of a configuration of the 
 :code:`Amides` processor is given below:
 
-Example
-^^^^^^^
+Processor Configuration
+^^^^^^^^^^^^^^^^^^^^^^^
 ..  code-block:: yaml
     :linenos:
 
     - amides:
         type: amides
         specific_rules:
             - tests/testdata/rules/specific/
         generic_rules:
             - tests/testdata/rules/generic/
         max_cache_entries: 10000
         decision_threshold: 0.0
         num_rule_attributions: 10
-        
-        
-        
+
 To keep track of the components performance, the :code:`Amides` processor tracks several processor metrics.
 This includes the mean misuse detection time, the mean rule attribution time, and several cache-related
 metrics like the number of hits and misses and the current cache load.
+
+.. autoclass:: logprep.processor.amides.processor.Amides.Config
+   :members:
+   :undoc-members:
+   :inherited-members:
+   :noindex:
+
+.. automodule:: logprep.processor.amides.rule
 """
-from time import time
+from functools import lru_cache, cached_property
 from multiprocessing import current_process
+from pathlib import Path
+from time import time
 from typing import List, Tuple
 from zipfile import ZipFile
-from pathlib import Path
-from functools import lru_cache, cached_property
-import joblib
 
+import joblib
 from attr import define, field, validators
 
 from logprep.abc.processor import Processor
 from logprep.metrics.metric import calculate_new_average
-from logprep.processor.amides.rule import AmidesRule
 from logprep.processor.amides.detection import MisuseDetector, RuleAttributor
 from logprep.processor.amides.normalize import CommandLineNormalizer
-from logprep.util.helper import get_dotted_field_value
+from logprep.processor.amides.rule import AmidesRule
 from logprep.util.getter import GetterFactory
+from logprep.util.helper import get_dotted_field_value
 
 
 class Amides(Processor):
     """Proof-of-concept implemenation of the Adaptive Misuse Detection System (AMIDES)."""
 
     @define(kw_only=True)
     class Config(Processor.Config):
```

### Comparing `logprep-6.2.0/logprep/processor/amides/rule.py` & `logprep-6.3.0/logprep/processor/amides/rule.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,34 +1,38 @@
 """
-Amides
-======
+Rule Configuration
+^^^^^^^^^^^^^^^^^^
 
 This rule enables to check if incoming documents are of a specific type
 suitable for classification by the :code:`Amides` processor. The specified
 :code:`source_field` should contain command line strings. In case of an
 positive detection result, rule attributions are written into
 the :code:`target_field`.
 
-
 The following example shows a complete rule:
 
 ..  code-block:: yaml
     :linenos:
     :caption: Example
 
     filter: 'some_field: "sample_cmdline"'
     amides:
         source_fields: ["process.command_line"]
         target_field: "rule_attributions"
     description: Sample rule for AMIDES processor.
 
+.. autoclass:: logprep.processor.amides.rule.AmidesRule.Config
+   :noindex:
+   :members:
+   :inherited-members:
+   :no-undoc-members:
 """
+from attrs import define, field, validators
 from ruamel.yaml import YAML
 
-from attrs import define, field, validators
 from logprep.processor.field_manager.rule import FieldManagerRule
 
 yaml = YAML(typ="safe", pure=True)
 
 
 class AmidesRule(FieldManagerRule):
     """AmidesRule checks if incoming documents contain fields suitable
@@ -47,7 +51,8 @@
                 validators.min_len(1),
                 validators.max_len(1),
             ]
         )
         target_field: str = field(
             validator=validators.instance_of(str), default="rule_attributions"
         )
+        mapping: dict = field(default="", init=False, repr=False, eq=False)
```

### Comparing `logprep-6.2.0/logprep/processor/base/exceptions.py` & `logprep-6.3.0/logprep/processor/base/exceptions.py`

 * *Files identical despite different names*

### Comparing `logprep-6.2.0/logprep/processor/base/rule.py` & `logprep-6.3.0/logprep/processor/base/rule.py`

 * *Files identical despite different names*

### Comparing `logprep-6.2.0/logprep/processor/calculator/fourFn.py` & `logprep-6.3.0/logprep/processor/calculator/fourFn.py`

 * *Files identical despite different names*

### Comparing `logprep-6.2.0/logprep/processor/calculator/processor.py` & `logprep-6.3.0/logprep/processor/calculator/processor.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,26 +1,32 @@
 """
 Calculator
 ==========
 
 The Calculator can be used to calculate with or without field values.
-For further information for the rule language see: :ref:`calculator_rule`
 
-Example
-^^^^^^^
+Processor Configuration
+^^^^^^^^^^^^^^^^^^^^^^^
 ..  code-block:: yaml
     :linenos:
 
     - calculatorname:
         type: calculator
         specific_rules:
             - tests/testdata/rules/specific/
         generic_rules:
             - tests/testdata/rules/generic/
 
+.. autoclass:: logprep.processor.calculator.processor.Calculator.Config
+   :members:
+   :undoc-members:
+   :inherited-members:
+   :noindex:
+
+.. automodule:: logprep.processor.calculator.rule
 """
 import re
 from functools import cached_property
 
 from pyparsing import ParseException
 
 from logprep.abc.processor import Processor
```

### Comparing `logprep-6.2.0/logprep/processor/calculator/rule.py` & `logprep-6.3.0/logprep/processor/calculator/rule.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,10 @@
 """
-.. _calculator_rule:
-
-Calculator
-==========
-
-The Calculator processor allows to calculate with and without field values.
+Rule Configuration
+^^^^^^^^^^^^^^^^^^
 
 A speaking example:
 
 ..  code-block:: yaml
     :linenos:
     :caption: Given calculator rule
 
@@ -27,14 +23,20 @@
 
 ..  code-block:: json
     :linenos:
     :caption: Processed event
 
     {"duration": 10000.0}
 
+.. autoclass:: logprep.processor.calculator.rule.CalculatorRule.Config
+   :noindex:
+   :members:
+   :inherited-members:
+   :no-undoc-members:
+
 Following a list with example calculation expressions, where all factors and the operators can be
 retrieved from a field with the schema :code:`${your.dotted.field}`:
 
 * :code:`9` => :code:`9`
 * :code:`-9` => :code:`-9`
 * :code:`--9` => :code:`9`
 * :code:`-E` => :code:`-math.e`
@@ -106,14 +108,15 @@
         source_fields: list = field(factory=list, init=False, repr=False, eq=False)
         extend_target_list: bool = field(validator=validators.instance_of(bool), default=False)
         """If the target field exists and is a list, the list will be extended with the values
         of the source fields.
         """
         timeout: int = field(validator=validators.instance_of(int), converter=int, default=1)
         """The maximum time in seconds for the calculation. Defaults to :code:`1`"""
+        mapping: dict = field(default="", init=False, repr=False, eq=False)
 
         def __attrs_post_init__(self):
             self.source_fields = re.findall(FIELD_PATTERN, self.calc)
             super().__attrs_post_init__()
 
     @property
     def calc(self):
```

### Comparing `logprep-6.2.0/logprep/processor/clusterer/processor.py` & `logprep-6.3.0/logprep/processor/clusterer/processor.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """
 Clusterer
----------
+=========
 
 The log clustering is mainly developed for Syslogs, unstructured and semi-structured logs.
 The clusterer calculates a log signature based on the message field.
 The log signature is calculated with heuristic and deterministic rules.
 The idea of a log signature is to extract a subset of the constant parts of a log and
 to delete the dynamic parts.
 If the fields syslog.facility and event.severity are in the log, then they are prefixed
@@ -14,27 +14,34 @@
 
 ..  code-block:: yaml
 
     Criteria 1: { "message": "A sample message", "tags": ["clusterable", ...], ... }
     Criteria 2: { "message": "A sample message", "clusterable": true, ... }
     Criteria 3: { "message": "A sample message", "syslog": { "facility": <number> }, "event": { "severity": <string> }, ... }
 
-
-Example
-^^^^^^^
+Processor Configuration
+^^^^^^^^^^^^^^^^^^^^^^^
 ..  code-block:: yaml
     :linenos:
 
     - clusterername:
         type: clusterer
         specific_rules:
             - tests/testdata/rules/specific/
         generic_rules:
             - tests/testdata/rules/generic/
         output_field_name: target_field
+
+.. autoclass:: logprep.processor.clusterer.processor.Clusterer.Config
+   :members:
+   :undoc-members:
+   :inherited-members:
+   :noindex:
+
+.. automodule:: logprep.processor.clusterer.rule
 """
 
 from logging import Logger
 from typing import List
 
 from attr import define, field, validators
 from logprep.abc.processor import Processor
```

### Comparing `logprep-6.2.0/logprep/processor/clusterer/rule.py` & `logprep-6.3.0/logprep/processor/clusterer/rule.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """
-Clusterer
-=========
+Rule Configuration
+^^^^^^^^^^^^^^^^^^
 
 Rules of the clusterer are evaluated in alphanumerical order.
 Some rules do only make sense if they are performed in a sequence with other rules.
 The clusterer matches multiple rules at once and applies them all before creating a
 clustering signature.
 Therefore, it is recommended to prefix rules with numbers, i.e. `00_01_*`.
 Here the first two digits represent a type of rules that make sense together and the second digits
@@ -87,18 +87,26 @@
     clusterer:
       target: message
       pattern: 'foo (bar) baz'
       repl: '<+>\1</+>'
     description: '...'
     tests:
       raw:    'foo bar baz'
-      result: 'foo <+>bar</+> baz'"""
+      result: 'foo <+>bar</+> baz'
+
+.. autoclass:: logprep.processor.clusterer.rule.ClustererRule.Config
+   :noindex:
+   :members:
+   :inherited-members:
+   :no-undoc-members:
+"""
 
 import re
 from typing import Pattern
+
 from attrs import define, field, validators
 
 from logprep.processor.base.rule import Rule
 
 
 class ClustererRule(Rule):
     """Check if documents match a filter."""
```

### Comparing `logprep-6.2.0/logprep/processor/clusterer/signature_calculation/signature_phase.py` & `logprep-6.3.0/logprep/processor/clusterer/signature_calculation/signature_phase.py`

 * *Files identical despite different names*

### Comparing `logprep-6.2.0/logprep/processor/concatenator/processor.py` & `logprep-6.3.0/logprep/processor/concatenator/processor.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,27 +1,34 @@
 """
 Concatenator
-------------
+============
 
 The `concatenator` processor allows to concat a list of source fields into one new target field. The
 concat separator and the target field can be specified. Furthermore, it is possible to directly
 delete all given source fields, or to overwrite the specified target field.
 
-
-Example
-^^^^^^^
+Processor Configuration
+^^^^^^^^^^^^^^^^^^^^^^^
 ..  code-block:: yaml
     :linenos:
 
     - Concatenatorname:
         type: concatenator
         specific_rules:
             - tests/testdata/rules/specific/
         generic_rules:
             - tests/testdata/rules/generic/
+
+.. autoclass:: logprep.processor.concatenator.processor.Concatenator.Config
+   :members:
+   :undoc-members:
+   :inherited-members:
+   :noindex:
+
+.. automodule:: logprep.processor.concatenator.rule
 """
 from logprep.abc.processor import Processor
 from logprep.processor.concatenator.rule import ConcatenatorRule
 from logprep.util.helper import get_dotted_field_value
 
 
 class ConcatenatorError(BaseException):
```

### Comparing `logprep-6.2.0/logprep/processor/concatenator/rule.py` & `logprep-6.3.0/logprep/processor/concatenator/rule.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,14 +1,10 @@
 """
-Concatenator
-============
-
-The concatenator processor allows to concat a list of source fields into one new target field. The
-separator and the target field can be specified. Furthermore, it is possible to directly delete
-all given source fields, or to overwrite the specified target field.
+Rule Configuration
+^^^^^^^^^^^^^^^^^^
 
 A speaking example:
 
 ..  code-block:: yaml
     :linenos:
     :caption: Given concatenator rule
 
@@ -33,14 +29,20 @@
 ..  code-block:: json
     :linenos:
     :caption: Processed event
 
     {
         "timetsamp": "01.01.1007 13:07"
     }
+
+.. autoclass:: logprep.processor.concatenator.rule.ConcatenatorRule.Config
+   :members:
+   :undoc-members:
+   :inherited-members:
+   :noindex:
 """
 
 from attrs import define, field, fields, validators
 
 from logprep.processor.field_manager.rule import FieldManagerRule
 
 
@@ -56,11 +58,12 @@
                 fields(FieldManagerRule.Config).source_fields.validator,
                 validators.min_len(2),
             ]
         )
         """The source fields that should be concatenated, can contain dotted field paths."""
         separator: str = field(validator=validators.instance_of(str))
         """The character(s) that should be used between the combined source field values."""
+        mapping: dict = field(default="", init=False, repr=False, eq=False)
 
     @property
     def separator(self) -> str:  # pylint: disable=missing-docstring
         return self._config.separator
```

### Comparing `logprep-6.2.0/logprep/processor/datetime_extractor/processor.py` & `logprep-6.3.0/logprep/processor/datetime_extractor/processor.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,26 +1,33 @@
 """
 DatetimeExtractor
------------------
+=================
 
 The `datetime_extractor` is a processor that can extract timestamps from a field and
 split it into its parts.
 
-
-Example
-^^^^^^^
+Processor Configuration
+^^^^^^^^^^^^^^^^^^^^^^^
 ..  code-block:: yaml
     :linenos:
 
     - datetimeextractorname:
         type: datetime_extractor
         specific_rules:
             - tests/testdata/rules/specific/
         generic_rules:
             - tests/testdata/rules/generic/
+
+.. autoclass:: logprep.processor.datetime_extractor.processor.DatetimeExtractor.Config
+   :members:
+   :undoc-members:
+   :inherited-members:
+   :noindex:
+
+.. automodule:: logprep.processor.datetime_extractor.rule
 """
 
 from datetime import datetime
 from logging import Logger
 
 from dateutil.parser import parse
 from dateutil.tz import tzlocal
```

### Comparing `logprep-6.2.0/logprep/processor/deleter/processor.py` & `logprep-6.3.0/logprep/processor/deleter/processor.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,25 +1,32 @@
 """
 Deleter
--------
+=======
 
 The `deleter` is a processor that removes an entire event from further pipeline processing.
 
-
-Example
-^^^^^^^
+Processor Configuration
+^^^^^^^^^^^^^^^^^^^^^^^
 ..  code-block:: yaml
     :linenos:
 
     - deletename:
         type: deleter
         specific_rules:
             - tests/testdata/rules/specific/
         generic_rules:
             - tests/testdata/rules/generic/
+
+.. autoclass:: logprep.processor.deleter.processor.Deleter.Config
+   :members:
+   :undoc-members:
+   :inherited-members:
+   :noindex:
+
+.. automodule:: logprep.processor.deleter.rule
 """
 
 from logprep.abc.processor import Processor
 from logprep.processor.deleter.rule import DeleterRule
 
 
 class Deleter(Processor):
```

### Comparing `logprep-6.2.0/logprep/processor/deleter/rule.py` & `logprep-6.3.0/logprep/processor/deleter/rule.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,21 +1,27 @@
 """
-Deleter
-=======
-The deleter processor deletes the entire log message if the filter produces a match.
+Rule Configuration
+^^^^^^^^^^^^^^^^^^
+
 The example below deletes the log message if the message field equals "foo".
 
 ..  code-block:: yaml
     :linenos:
     :caption: Example delete rule
 
     filter: 'message: "foo"'
     deleter:
         delete: true
     description: '...'
+
+.. autoclass:: logprep.processor.deleter.rule.DeleterRule.Config
+   :members:
+   :undoc-members:
+   :inherited-members:
+   :noindex:
 """
 
 from attrs import define, field, validators
 
 from logprep.processor.base.rule import Rule
```

### Comparing `logprep-6.2.0/logprep/processor/dissector/processor.py` & `logprep-6.3.0/logprep/processor/dissector/processor.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,28 +1,35 @@
 """
 Dissector
 =========
 
 The `dissector` is a processor that tokenizes incoming strings using defined patterns.
 The behavior is based of the logstash dissect filter plugin and has the same advantage that
 for the event processing no regular expressions are used.
-Additionally it can be used to convert datatypes of given fields.
+Additionally, it can be used to convert datatypes of given fields.
 
-
-Example
-^^^^^^^
+Processor Configuration
+^^^^^^^^^^^^^^^^^^^^^^^
 ..  code-block:: yaml
     :linenos:
 
     - dissectorname:
         type: dissector
         specific_rules:
             - tests/testdata/rules/specific/
         generic_rules:
             - tests/testdata/rules/generic/
+
+.. autoclass:: logprep.processor.dissector.processor.Dissector.Config
+   :members:
+   :undoc-members:
+   :inherited-members:
+   :noindex:
+
+.. automodule:: logprep.processor.dissector.rule
 """
 from typing import Callable, List, Tuple
 
 from logprep.abc.processor import Processor
 from logprep.processor.dissector.rule import DissectorRule
 from logprep.util.helper import get_dotted_field_value, add_field_to
 
@@ -43,33 +50,43 @@
         for action, *args, _ in action_mappings_sorted_by_position:
             action(*args)
 
     def _get_mappings(self, event, rule) -> List[Tuple[Callable, dict, str, str, str, int]]:
         current_field = None
         target_field_mapping = {}
         for rule_action in rule.actions:
-            source_field, delimeter, target_field, rule_action, separator, position = rule_action
+            (
+                source_field,
+                delimiter,
+                target_field,
+                rule_action,
+                separator,
+                strip_char,
+                position,
+            ) = rule_action
             if current_field != source_field:
                 current_field = source_field
                 loop_content = get_dotted_field_value(event, current_field)
                 if loop_content is None:
                     error = BaseException(
                         f"dissector: mapping field '{source_field}' does not exist"
                     )
                     self._handle_warning_error(event, rule, error)
-            if delimeter is not None and loop_content is not None:
-                content, _, loop_content = loop_content.partition(delimeter)
+            if delimiter is not None and loop_content is not None:
+                content, _, loop_content = loop_content.partition(delimiter)
             else:
                 content = loop_content
             if target_field.startswith("?"):
                 target_field_mapping[target_field.lstrip("?")] = content
                 target_field = content
                 content = ""
             if target_field.startswith("&"):
                 target_field = target_field_mapping.get(target_field.lstrip("&"))
+            if strip_char:
+                content = content.strip(strip_char)
             yield rule_action, event, target_field, content, separator, position
 
     def _apply_convert_datatype(self, event, rule):
         for target_field, converter in rule.convert_actions:
             try:
                 target_value = converter(get_dotted_field_value(event, target_field))
                 add_field_to(event, target_field, target_value, overwrite_output_field=True)
```

### Comparing `logprep-6.2.0/logprep/processor/dissector/rule.py` & `logprep-6.3.0/logprep/processor/dissector/rule.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,10 @@
 """
-Dissector
-=========
-
-The dissector processor tokenizes values from fields into new fields or appends the value to
-existing fields. Additionally it can be used to convert datatypes of field values.
+Rule Configuration
+^^^^^^^^^^^^^^^^^^
 
 A speaking example:
 
 ..  code-block:: yaml
     :linenos:
     :caption: Given dissector rule
 
@@ -40,34 +37,47 @@
 
 The dissect pattern describes the textual format of the source field.
 
 Given a dissect pattern of :code:`%{field1} %{field2}` the source field value will be dissected into
 everything before the first whitespace which would be written into the field `field1` and everything
 after the first whitespace which would be written into the field `field2`.
 
-The string surrounded by :code:`%{` and :code:`}` is the desired target field. This can be declared
+The string between :code:`%{` and :code:`}` is the desired target field. This can be declared
 in dotted field notation (e.g. :code:`%{target.subfield1.subfield2}`). Every subfield between the
 first and the last subfield will be created if necessary.
 
-By default the target field will always be overwritten with the captured value. If you want to
+By default, the target field will always be overwritten with the captured value. If you want to
 append to a preexisting target field value, as string or list, you have to use
 the :code:`+` operator. If you want to use a prefix before the appended string use this notation
 :code:`+( )`. In this example a whitespace would be added before the extracted string is added.
 If you want to use the symbols :code:`(` or :code:`)` as your separator, you have to escape with
-:code:`\` (e.g. :code:`+(\()`)
+:code:`\\\` (e.g. :code:`+(\\\()`).
+
+If you want to remove unwanted padding characters around a dissected pattern you have to use the
+:code:`-(<char>)` notation, while :code:`<char>` can be any character similar to the :code:`+( )`
+notation. If for example you have a field like
+:code:`"[2022-11-04 10:00:00 AM     ] - 127.0.0.1"` and you want to extract the timestamp and the
+ip, you can use the dissect-pattern :code:`[%{time-( )}] - %{ip}` to remove the unwanted spaces
+after the 'AM'. This works independent of the number of spaces.
 
-It is possible to capture the target field name from the source field value with the notation
+It is also possible to capture the target field name from the source field value with the notation
 :code:`%{?<your name for the reference>}` (e.g. :code:`%{?key1}`). In the same dissection pattern
 this can be referred to with the notation :code:`%{&<the reference>}` (e.g. :code:`%{&key1}`).
-References can be combined with the append operator.
+References can be combined with the append operator. For examples see below.
 
-Optional convert datatype can be provided after the key using :code:`|` as separator
+Additionally an optional convert datatype can be provided after the key using :code:`|` as separator
 to convert the value from string to :code:`int`, :code:`float` or :code:`bool`.
 The conversion to :code:`bool` is interpreted by meaning.
-(e.g. :code:`yes` is translated to :code:`True`)
+(e.g. :code:`yes` is translated to :code:`True`). When removing padding characters at the same time
+then the conversion has to come after the padding character (e.g. :code:`%{field2-(#)|bool}`).
+
+If you want to reorder parts of a dissection you can give the order by adding :code:`/<position>` to
+the dissect pattern. A valid example would be: :code:`%{time/1} %{+time/3} %{+time/2}`. When
+removing padding characters at the same time then the position has to come after the padding
+character (e.g. :code:`%{time-(*)/2}`).
 
 .. autoclass:: logprep.processor.dissector.rule.DissectorRule.Config
    :members:
    :undoc-members:
    :inherited-members:
    :noindex:
 
@@ -94,25 +104,24 @@
 APPEND_WITHOUT_SEPERATOR = r"(\+(?!\([^%]))"
 INDIRECT_FIELD_NOTATION = r"([&\?]))"
 VALID_ACTION = rf"({APPEND_WITH_SEPERATOR}|{APPEND_WITHOUT_SEPERATOR}|{INDIRECT_FIELD_NOTATION}"
 VALID_POSITION = r"(\/\d*)"
 VALID_DATATYPE = r"(\|(int|float|str|bool))"
 POSITION_OR_DATATYPE = rf"({VALID_POSITION}|{VALID_DATATYPE})"
 DISSECT = rf"{START}{VALID_ACTION}?{VALID_TARGET_FIELD}{POSITION_OR_DATATYPE}?{END}"
-DELIMETER = r"([^%]+)"
+DELIMITER = r"([^%]+)"
 ACTION = r"(?P<action>[+])?"
-SEPERATOR = r"(\((?P<separator>.+)\))?"
-TARGET_FIELD = r"(?P<target_field>[^\/\|]*)"
+STRIP_CHAR = r"(-\((?P<strip>.)\))?"
+SEPERATOR = r"(\((?P<separator>\\\)|[^)]+)\))?"
+TARGET_FIELD = r"(?P<target_field>[^\/\|-]*)"
 POSITION = r"(\/(?P<position>\d*))?"
 DATATYPE = r"(\|(?P<datatype>int|float|bool))?"
-SECTION_MATCH = (
-    rf"{START}{ACTION}{SEPERATOR}{TARGET_FIELD}{POSITION}{DATATYPE}{END}(?P<delimeter>.*)"
-)
+SECTION_MATCH = rf"{START}{ACTION}{SEPERATOR}{TARGET_FIELD}{STRIP_CHAR}{POSITION}{DATATYPE}{END}(?P<delimiter>.*)"
 
-MAPPING_VALIDATION_REGEX = re.compile(rf"^({DELIMETER})?({DISSECT}{DELIMETER})+({DISSECT})?$")
+MAPPING_VALIDATION_REGEX = re.compile(rf"^({DELIMITER})?({DISSECT}{DELIMITER})+({DISSECT})?$")
 
 
 def _do_nothing(*_):
     return
 
 
 def str_to_bool(input_str: str) -> bool:
@@ -172,16 +181,17 @@
         "+": append,
     }
 
     _converter_mapping: dict = {"int": int, "float": float, "string": str, "bool": str_to_bool}
 
     _config: "DissectorRule.Config"
 
-    actions: List[Tuple[str, str, str, Callable, int]]
-    """list tuple format (<source_field>, <separator>, <target_field>, <function>), <position> """
+    actions: List[Tuple[str, str, str, Callable, str, str, int]]
+    """list tuple format (source_field, delimiter, target_field, action, separator, strip_char,
+    position)"""
 
     convert_actions: List[Tuple[str, Callable]]
     """list tuple format <target_field>, <converter callable>"""
 
     @property
     def failure_tags(self):
         """Returns the failure tags"""
@@ -202,24 +212,25 @@
                 section_match = re.match(SECTION_MATCH, section)
                 separator = section_match.group("separator")
                 separator = "" if separator is None else separator
                 separator = separator.replace("\\(", "(")
                 separator = separator.replace("\\)", ")")
                 action_key = section_match.group("action")
                 target_field = section_match.group("target_field")
+                strip_char = section_match.group("strip")
                 datatype = section_match.group("datatype")
                 position = section_match.group("position")
                 if datatype is not None:
                     self._config.convert_datatype.update({target_field: datatype})
-                delimeter = section_match.group("delimeter")
-                delimeter = None if delimeter == "" else delimeter
+                delimiter = section_match.group("delimiter")
+                delimiter = None if delimiter == "" else delimiter
                 position = int(position) if position is not None else 0
                 action = self._actions_mapping.get(action_key) if target_field else _do_nothing
                 self.actions.append(
-                    (source_field, delimeter, target_field, action, separator, position)
+                    (source_field, delimiter, target_field, action, separator, strip_char, position)
                 )
 
     def _set_convert_actions(self):
         self.convert_actions = []
         for target_field, converter_string in self._config.convert_datatype.items():
             self.convert_actions.append(
                 (target_field, self._converter_mapping.get(converter_string))
```

### Comparing `logprep-6.2.0/logprep/processor/domain_label_extractor/processor.py` & `logprep-6.3.0/logprep/processor/domain_label_extractor/processor.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,34 +1,41 @@
 """
 DomainLabelExtractor
---------------------
+====================
 
 The `domain_label_extractor` is a processor that splits a domain into it's corresponding labels
 like :code:`registered_domain`, :code:`top_level_domain` and :code:`subdomain`. If instead an IP
 is given in the target field an informational tag is added to the configured tags field. If
 neither a domain nor an ip address can be recognized an invalid error tag will be be added to the
 tag field in the event. The added tags contain each the target field name that was checked by the
 configured rule, such that it is possible to distinguish between different domain fields in one
 event. For example for the target field :code:`url.domain` following tags could be added:
 :code:`invalid_domain_in_url_domain` and :code:`ip_in_url_domain`
 
-
-Example
-^^^^^^^
+Processor Configuration
+^^^^^^^^^^^^^^^^^^^^^^^
 ..  code-block:: yaml
     :linenos:
 
     - domainlabelextractorname:
         type: domain_label_extractor
         specific_rules:
             - tests/testdata/rules/specific/
         generic_rules:
             - tests/testdata/rules/generic/
         tld_lists: /path/to/list/file
         tagging_field_name: resolved
+
+.. autoclass:: logprep.processor.domain_label_extractor.processor.DomainLabelExtractor.Config
+   :members:
+   :undoc-members:
+   :inherited-members:
+   :noindex:
+
+.. automodule:: logprep.processor.domain_label_extractor.rule
 """
 import ipaddress
 from functools import cached_property
 from multiprocessing import current_process
 from pathlib import Path
 from typing import Optional
```

### Comparing `logprep-6.2.0/logprep/processor/domain_label_extractor/rule.py` & `logprep-6.3.0/logprep/processor/domain_label_extractor/rule.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """
-Domain Label Extractor
-======================
+Rule Configuration
+^^^^^^^^^^^^^^^^^^
 
 The domain label extractor requires the additional field :code:`domain_label_extractor`.
 The mandatory keys under :code:`domain_label_extractor` are :code:`source_fields`
 and :code:`target_field`. Former is used to identify the field
 (declared as list with one element) which contains the domain.
 And the latter is used to define the parent field where theresults should be written to.
 Both fields can be dotted subfields. The sub fields of the parent output field of the
@@ -45,14 +45,33 @@
             "domain": "www.sub.domain.de",
             "registered_domain": "domain.de",
             "top_level_domain": "de",
             "subdomain": "www.sub"
         }
     }
 
+.. autoclass:: logprep.processor.domain_label_extractor.rule.DomainLabelExtractorRule.Config
+   :members:
+   :undoc-members:
+   :inherited-members:
+   :noindex:
 """
+from attr import field, validators, define
 
 from logprep.processor.field_manager.rule import FieldManagerRule
 
 
 class DomainLabelExtractorRule(FieldManagerRule):
     """Check if documents match a filter."""
+
+    @define(kw_only=True)
+    class Config(FieldManagerRule.Config):
+        """Config for DomainLabelExtractorRule"""
+
+        source_fields: list = field(
+            validator=[
+                validators.instance_of(list),
+                validators.deep_iterable(member_validator=validators.instance_of(str)),
+            ],
+        )
+        """The fields from where to get the values which should be processed."""
+        mapping: dict = field(default="", init=False, repr=False, eq=False)
```

### Comparing `logprep-6.2.0/logprep/processor/domain_resolver/processor.py` & `logprep-6.3.0/logprep/processor/domain_resolver/processor.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 """
 DomainResolver
---------------
+==============
 
 The `domain_resolver` is a processor that can resolve domains inside a defined field.
 
-
-Example
-^^^^^^^
+Processor Configuration
+^^^^^^^^^^^^^^^^^^^^^^^
 ..  code-block:: yaml
     :linenos:
 
     - domainresolvername:
         type: domain_resolver
         specific_rules:
             - tests/testdata/rules/specific/
@@ -20,14 +19,22 @@
         tld_list: tmp/path/tld.dat
         timeout: 0.5
         max_cached_domains: 20000
         max_caching_days: 1
         hash_salt: secure_salt
         cache_enabled: true
         debug_cache: false
+
+.. autoclass:: logprep.processor.domain_resolver.processor.DomainResolver.Config
+   :members:
+   :undoc-members:
+   :inherited-members:
+   :noindex:
+
+.. automodule:: logprep.processor.domain_resolver.rule
 """
 import datetime
 import socket
 from functools import cached_property
 from logging import Logger
 from multiprocessing import context, current_process
 from multiprocessing.pool import ThreadPool
```

### Comparing `logprep-6.2.0/logprep/processor/domain_resolver/rule.py` & `logprep-6.3.0/logprep/processor/domain_resolver/rule.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """
-Domain Resolver
-===============
+Rule Configuration
+^^^^^^^^^^^^^^^^^^
 
 The domain resolver requires the additional field :code:`domain_resolver`.
 The additional field :code:`domain_resolver.source_fields` must be defined as list with one element.
 It contains the field from which an URL should be parsed and then written to :code:`resolved_ip`.
 The URL can be located in continuous text insofar the URL is valid.
 
 Optionally, the output field can be configured (overriding the default :code:`resolved_ip`) using the parameter :code:`target_field`.
@@ -16,14 +16,20 @@
     :linenos:
     :caption: Example
 
       filter: url
       domain_resolver:
         source_fields: [url]
       description: '...'
+
+.. autoclass:: logprep.processor.domain_resolver.rule.DomainResolverRule.Config
+   :members:
+   :undoc-members:
+   :inherited-members:
+   :noindex:
 """
 from attrs import define, field, fields
 
 from logprep.processor.field_manager.rule import FieldManagerRule
 
 
 class DomainResolverRule(FieldManagerRule):
@@ -34,7 +40,8 @@
         """RuleConfig for DomainResolver"""
 
         target_field: str = field(
             validator=fields(FieldManagerRule.Config).target_field.validator,
             default="resolved_ip",
         )
         """The field where to write the processor output to. Defaults to :code:`resovled_ip`"""
+        mapping: dict = field(default="", init=False, repr=False, eq=False)
```

### Comparing `logprep-6.2.0/logprep/processor/dropper/processor.py` & `logprep-6.3.0/logprep/processor/dropper/processor.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,26 +1,33 @@
 """
 Dropper
--------
+=======
 
 The `dropper` is a processor that removes fields from log messages. Which fields are deleted is
 determined within each rule.
 
-
-Example
-^^^^^^^
+Processor Configuration
+^^^^^^^^^^^^^^^^^^^^^^^
 ..  code-block:: yaml
     :linenos:
 
     - droppername:
         type: dropper
         specific_rules:
             - tests/testdata/rules/specific/
         generic_rules:
             - tests/testdata/rules/generic/
+
+.. autoclass:: logprep.processor.dropper.processor.Dropper.Config
+   :members:
+   :undoc-members:
+   :inherited-members:
+   :noindex:
+
+.. automodule:: logprep.processor.dropper.rule
 """
 
 from functools import partial
 from logprep.abc.processor import Processor
 
 from logprep.processor.dropper.rule import DropperRule
 from logprep.util.helper import pop_dotted_field_value, get_dotted_field_value
```

### Comparing `logprep-6.2.0/logprep/processor/dropper/rule.py` & `logprep-6.3.0/logprep/processor/dropper/rule.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """
-Dropper
-=======
+Rule Configuration
+^^^^^^^^^^^^^^^^^^
 
 Which fields are removed is defined in the additional field :code:`drop`.
 It contains a list of fields in dot notation.
 For nested fields all subfields are also removed if they are empty.
 If only the specified subfield should be removed, then this can be achieved by setting
 the option :code:`drop_full: false`.
 
@@ -36,14 +36,20 @@
     :caption: Example - Expected output after application of the rule
 
     [{
         "keep_me": {
             "keep_me_too": "something"
         }
     }]
+
+.. autoclass:: logprep.processor.dropper.rule.DropperRule.Config
+   :members:
+   :undoc-members:
+   :inherited-members:
+   :noindex:
 """
 
 from typing import List
 
 from attrs import define, field, validators
 
 from logprep.processor.base.rule import Rule
```

### Comparing `logprep-6.2.0/logprep/processor/field_manager/rule.py` & `logprep-6.3.0/logprep/processor/field_manager/rule.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,10 @@
 """
-FieldManager
-============
-
-The `field_manager` processor copies or moves field from multiple source fields to one target field.
-Additionaly it can be used to merge lists or simple values from source fields to
-one target field list.
+Rule Configuration
+^^^^^^^^^^^^^^^^^^
 
 A speaking example:
 
 ..  code-block:: yaml
     :linenos:
     :caption: Given field_manager rule
 
@@ -94,20 +90,35 @@
     class Config(Rule.Config):
         """Config for FieldManagerRule"""
 
         source_fields: list = field(
             validator=[
                 validators.instance_of(list),
                 validators.deep_iterable(member_validator=validators.instance_of(str)),
-                validators.min_len(1),
-            ]
+            ],
+            default=[],
+        )
+        """The fields from where to get the values which should be processed, requires
+        :code:`target_field`."""
+        target_field: str = field(validator=validators.instance_of(str), default="")
+        """The field where to write the processed values to. Can be used to move/copy single values,
+        merge multiple values to one list or extend a list. Requires :code:`source_field`."""
+        mapping: dict = field(
+            validator=[
+                validators.instance_of(dict),
+                validators.deep_mapping(
+                    key_validator=validators.instance_of(str),
+                    value_validator=validators.instance_of(str),
+                ),
+            ],
+            default={},
         )
-        """The fields from where to get the values which should be processed"""
-        target_field: str = field(validator=validators.instance_of(str))
-        """The field where to write the processed values to"""
+        """A key-value mapping from source fields to target fields. Can be used to copy/move
+        multiple fields at once. If you want to move fields set :code:`delete_source_fields` to
+        true. Works independent of :code:`source_fields` and :code:`target_field`."""
         delete_source_fields: bool = field(validator=validators.instance_of(bool), default=False)
         """Whether to delete all the source fields or not. Defaults to :code:`False`"""
         overwrite_target: bool = field(validator=validators.instance_of(bool), default=False)
         """Overwrite the target field value if exists. Defaults to :code:`False`"""
         extend_target_list: bool = field(validator=validators.instance_of(bool), default=False)
         """If the target field exists and is a list, the list will be extended with the values
         of the source fields. If the source field is a list, the lists will be merged.
@@ -135,14 +146,18 @@
         return []
 
     @property
     def target_field(self):
         return self._config.target_field
 
     @property
+    def mapping(self):
+        return self._config.mapping
+
+    @property
     def overwrite_target(self):
         return self._config.overwrite_target
 
     @property
     def extend_target_list(self):
         return self._config.extend_target_list
```

### Comparing `logprep-6.2.0/logprep/processor/generic_adder/mysql_connector.py` & `logprep-6.3.0/logprep/processor/generic_adder/mysql_connector.py`

 * *Files identical despite different names*

### Comparing `logprep-6.2.0/logprep/processor/generic_adder/processor.py` & `logprep-6.3.0/logprep/processor/generic_adder/processor.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 """
 GenericAdder
-------------
+============
 The `generic_adder` is a processor that adds new fields and values to documents based on a list.
 The list can reside inside a rule, inside a file or retrieved from an sql database.
 
 
-Example
-^^^^^^^
+Processor Configuration
+^^^^^^^^^^^^^^^^^^^^^^^
 ..  code-block:: yaml
     :linenos:
 
     - genericaddername:
         type: generic_adder
         specific_rules:
             - tests/testdata/rules/specific/
@@ -21,14 +21,22 @@
             password: example_password
             host: "127.0.0.1
             database: example_db
             table: example_table
             target_column: example_column
             add_target_column: True
             timer: 0.1
+
+.. autoclass:: logprep.processor.generic_adder.processor.GenericAdder.Config
+   :members:
+   :undoc-members:
+   :inherited-members:
+   :noindex:
+
+.. automodule:: logprep.processor.generic_adder.rule
 """
 import json
 import os
 import re
 import time
 from logging import Logger
 from typing import Optional
```

### Comparing `logprep-6.2.0/logprep/processor/generic_adder/rule.py` & `logprep-6.3.0/logprep/processor/generic_adder/rule.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # pylint: disable=anomalous-backslash-in-string
 """
-Generic Adder
-=============
+Rule Configuration
+^^^^^^^^^^^^^^^^^^
 
 The generic adder requires the additional field :code:`generic_adder`.
 The field :code:`generic_adder.add` can be defined.
 It contains a dictionary of field names and values that should be added.
 If dot notation is being used, then all fields on the path are being automatically created.
 
 In the following example, the field :code:`some.added.field` with the
@@ -80,14 +80,20 @@
     filter: '*'
     generic_adder:
       sql_table:
         event_source_field: source
         pattern: '([a-zA-Z0-9]+)_\S+'
         destination_field_prefix: nested.dict
     description: '...'
+
+.. autoclass:: logprep.processor.generic_adder.rule.GenericAdderRule.Config
+   :members:
+   :undoc-members:
+   :inherited-members:
+   :noindex:
 """
 # pylint: enable=anomalous-backslash-in-string
 
 import re
 from typing import Any
 
 from attrs import define, field, validators
```

### Comparing `logprep-6.2.0/logprep/processor/generic_resolver/processor.py` & `logprep-6.3.0/logprep/processor/generic_resolver/processor.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,24 +1,32 @@
 """
 GenericResolver
----------------
+===============
 
 The `generic_resolver` resolves log event values using regex lists.
 
-Example
-^^^^^^^
+Processor Configuration
+^^^^^^^^^^^^^^^^^^^^^^^
 ..  code-block:: yaml
     :linenos:
 
     - genericresolvername:
         type: generic_resolver
         specific_rules:
             - tests/testdata/rules/specific/
         generic_rules:
             - tests/testdata/rules/generic/
+
+.. autoclass:: logprep.processor.generic_resolver.processor.GenericResolver.Config
+   :members:
+   :undoc-members:
+   :inherited-members:
+   :noindex:
+
+.. automodule:: logprep.processor.generic_resolver.rule
 """
 import re
 from logging import Logger
 
 from logprep.abc.processor import Processor
 from logprep.processor.base.exceptions import FieldExistsWarning
 from logprep.processor.generic_resolver.rule import GenericResolverRule
```

### Comparing `logprep-6.2.0/logprep/processor/generic_resolver/rule.py` & `logprep-6.3.0/logprep/processor/generic_resolver/rule.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,10 @@
 """
-.. _generic-resolver-rule:
-
-Generic Resolver
-================
+Rule Configuration
+^^^^^^^^^^^^^^^^^^
 
 The generic resolver requires the additional field :code:`generic_resolver`.
 It works similarly to the hyperscan resolver, which utilizes hyperscan to process resolve lists.
 Configurable fields are being checked by regex patterns and a configurable value will be added
 if a pattern matches.
 The parameters within :code:`generic_resolver` must be of the form
 :code:`field_mapping: {SOURCE_FIELD: DESTINATION_FIELD},
@@ -63,14 +61,19 @@
 ..  code-block:: yaml
     :linenos:
     :caption: Example file with resolve list
 
     foo: resolved foo
     bar: resolved bar
 
+.. autoclass:: logprep.processor.generic_resolver.rule.GenericResolverRule.Config
+   :members:
+   :undoc-members:
+   :inherited-members:
+   :noindex:
 """
 from attrs import define, field, validators
 
 from logprep.processor.base.rule import Rule
 
 
 class GenericResolverRule(Rule):
```

### Comparing `logprep-6.2.0/logprep/processor/geoip_enricher/processor.py` & `logprep-6.3.0/logprep/processor/geoip_enricher/processor.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,24 +1,33 @@
 """
 GeoipEnricher
--------------
+=============
+
 Processor to enrich log messages with geolocalization information
 
-Example
-^^^^^^^
+Processor Configuration
+^^^^^^^^^^^^^^^^^^^^^^^
 ..  code-block:: yaml
     :linenos:
 
     - geoipenrichername:
         type: geoip_enricher
         specific_rules:
             - tests/testdata/geoip_enricher/rules/
         generic_rules:
             - tests/testdata/geoip_enricher/rules/
         db_path: /path/to/GeoLite2-City.mmdb
+
+.. autoclass:: logprep.processor.geoip_enricher.processor.GeoipEnricher.Config
+   :members:
+   :undoc-members:
+   :inherited-members:
+   :noindex:
+
+.. automodule:: logprep.processor.geoip_enricher.rule
 """
 from functools import cached_property
 from ipaddress import ip_address
 from multiprocessing import current_process
 from pathlib import Path
 
 from attr import define, field, validators
```

### Comparing `logprep-6.2.0/logprep/processor/geoip_enricher/rule.py` & `logprep-6.3.0/logprep/processor/geoip_enricher/rule.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """
-Geoip Enricher
-==============
+Rule Configuration
+^^^^^^^^^^^^^^^^^^
 
 The geoip enricher requires the additional field :code:`geoip`.
 The default output_field can be overridden using the optional parameter
 :code:`target_field`. This can be a dotted subfield.
 The additional field :code:`geoip.source_fields` must be given as list with one element.
 It contains the IP for which the geoip data should be added.
 
@@ -14,14 +14,20 @@
     :linenos:
     :caption: Example
 
     filter: client.ip
     geoip:
       source_fields: [client.ip]
     description: '...'
+
+.. autoclass:: logprep.processor.geoip_enricher.rule.GeoipEnricherRule.Config
+   :members:
+   :undoc-members:
+   :inherited-members:
+   :noindex:
 """
 from attr import Factory
 from attrs import define, field, validators
 
 from logprep.processor.field_manager.rule import FieldManagerRule
 
 GEOIP_DATA_STUBS = {
@@ -81,11 +87,12 @@
             geoip:
               source_fields: [client.ip]
               customize_target_subfields:
                 geometry.type: client.geo.type
                 geometry.coordinates: client.geo.coordinates
             description: '...'
         """
+        mapping: dict = field(default="", init=False, repr=False, eq=False)
 
     @property
     def customize_target_subfields(self) -> dict:  # pylint: disable=missing-function-docstring
         return self._config.customize_target_subfields
```

### Comparing `logprep-6.2.0/logprep/processor/grokker/processor.py` & `logprep-6.3.0/logprep/processor/grokker/processor.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,30 +1,38 @@
 """
 Grokker
-============
+=======
 
 The `grokker` processor dissects a message on a basis of grok patterns. This processor is based
 of the ideas of the logstash grok filter plugin.
 (see: https://www.elastic.co/guide/en/logstash/current/plugins-filters-grok.html)
 
 The default builtin grok patterns shipped with logprep are the same than in logstash.
 
 
-Example
-^^^^^^^
+Processor Configuration
+^^^^^^^^^^^^^^^^^^^^^^^
 ..  code-block:: yaml
     :linenos:
 
     - my_grokker:
         type: grokker
         specific_rules:
             - tests/testdata/rules/specific/
         generic_rules:
             - tests/testdata/rules/generic/
         custom_patterns_dir: "http://the.patterns.us/patterns.zip"
+
+.. autoclass:: logprep.processor.grokker.processor.Grokker.Config
+   :members:
+   :undoc-members:
+   :inherited-members:
+   :noindex:
+
+.. automodule:: logprep.processor.grokker.rule
 """
 import re
 from pathlib import Path
 from zipfile import ZipFile
 
 from attrs import define, field, validators
 
@@ -53,16 +61,20 @@
         """
 
     def _apply_rules(self, event: dict, rule: GrokkerRule):
         conflicting_fields = []
         matches = []
         for dotted_field, grok in rule.actions.items():
             field_value = get_dotted_field_value(event, dotted_field)
+            if field_value is None:
+                error = BaseException(f"{self.name}: missing source_field: '{dotted_field}'")
+                self._handle_warning_error(event=event, rule=rule, error=error)
+                continue
             result = grok.match(field_value)
-            if result is None:
+            if result is None or result == {}:
                 continue
             matches.append(True)
             for dotted_field, value in result.items():
                 if value is None:
                     continue
                 success = add_field_to(
                     event, dotted_field, value, rule.extend_target_list, rule.overwrite_target
```

### Comparing `logprep-6.2.0/logprep/processor/grokker/rule.py` & `logprep-6.3.0/logprep/processor/grokker/rule.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,10 @@
 """
-Grokker
-=======
-
-The `grokker` processor dissects a message on a basis of grok patterns. This processor is based
-of the ideas of the logstash grok filter plugin.
-(see: https://www.elastic.co/guide/en/logstash/current/plugins-filters-grok.html)
+Rule Configuration
+^^^^^^^^^^^^^^^^^^
 
 A speaking example:
 
 ..  code-block:: yaml
     :linenos:
     :caption: Given grokker rule
 
@@ -65,25 +61,30 @@
 FIELD_PATTERN = re.compile(r"%\{[A-Z0-9_]*?:([^\[\]]*?)(:.*)?\}")
 
 
 def _dotted_field_to_logstash_converter(mapping: dict) -> dict:
     if not mapping:
         return mapping
 
-    def _replace_pattern(pattern):
-        if isinstance(pattern, list):
-            pattern = "|".join(pattern)
+    def _transform(pattern):  # nosemgrep
         fields = re.findall(FIELD_PATTERN, pattern)
         for dotted_field, _ in fields:
             splitted_field = dotted_field.split(".")
             if len(splitted_field) > 1:
                 replacement = "".join(f"[{element}]" for element in splitted_field)
                 pattern = re.sub(re.escape(dotted_field), replacement, pattern)
         return pattern
 
+    def _replace_pattern(pattern):
+        if isinstance(pattern, list):
+            pattern = list(map(_transform, pattern))
+        else:
+            pattern = [_transform(pattern)]
+        return pattern
+
     return {dotted_field: _replace_pattern(pattern) for dotted_field, pattern in mapping.items()}
 
 
 class GrokkerRule(DissectorRule):
     """grokker rule"""
 
     @define(kw_only=True)
@@ -91,48 +92,47 @@
         """Config for GrokkerRule"""
 
         mapping: dict = field(
             validator=[
                 validators.instance_of(dict),
                 validators.deep_mapping(
                     key_validator=validators.instance_of(str),
-                    value_validator=validators.instance_of(str),
-                ),
-                validators.deep_mapping(
-                    key_validator=validators.instance_of(str),
-                    value_validator=validators.matches_re(MAPPING_VALIDATION_REGEX),
+                    value_validator=validators.deep_iterable(
+                        member_validator=validators.matches_re(MAPPING_VALIDATION_REGEX),
+                        iterable_validator=validators.instance_of(list),
+                    ),
                 ),
                 validators.deep_iterable(
                     member_validator=validators.instance_of(str),
                     iterable_validator=validators.min_len(1),
                 ),
             ],
             converter=_dotted_field_to_logstash_converter,
         )
         """A mapping from source fields to a grok pattern.
         Dotted field notation is possible in key and in the grok pattern.
         Additionally logstash field notation is possible in grok pattern.
         The value can be a list of search patterns or a single search pattern.
-        Lists of search pattern will be joined by :code:`|` and only the first matching pattern
-        will return values.
+        Lists of search pattern will be checked in the order of the list until the first matching
+        pattern.
         It is possible to use `oniguruma` regex pattern with or without grok patterns in the
         patterns part.
         Logstashs ecs conform grok patterns are used to resolve the here used grok patterns.
         """
         patterns: dict = field(
             validator=[
                 validators.instance_of(dict),
                 validators.deep_mapping(
                     key_validator=validators.instance_of(str),
                     value_validator=validators.instance_of(str),
                 ),
             ],
             factory=dict,
         )
-        """(Optional) additional grok patterns as mapping. E.g. :code:`CUSTOM_PATTERN: [^\s]*`
+        r"""(Optional) additional grok patterns as mapping. E.g. :code:`CUSTOM_PATTERN: [^\s]*`
         if you want to use special target fields, you are able to use them an usual in the
         mapping sections. Here you only have to declare the matching regex without named groups.
         """
 
     actions: dict[str, Grok]
 
     def _set_mapping_actions(self):
```

### Comparing `logprep-6.2.0/logprep/processor/hyperscan_resolver/processor.py` & `logprep-6.3.0/logprep/processor/hyperscan_resolver/processor.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,28 +1,38 @@
 """
 HyperscanResolver
------------------
+=================
 
 The `hyperscan_resolver` is a processor that can resolve fields by using a map of resolve patterns
-and resolve values. The map can be defined within rules or within a file. It uses pythion hyperscan
+and resolve values. The map can be defined within rules or within a file. It uses python hyperscan
 to speedup the pattern matching.
+It works similarly to the generic resolver, but utilized hyperscan to process resolve lists.
 
+For further information see: `GenericResolver`_.
 
-Example
-^^^^^^^
+Processor Configuration
+^^^^^^^^^^^^^^^^^^^^^^^
 ..  code-block:: yaml
     :linenos:
 
     - hyperscanresolvername:
         type: hyperscan_resolver
         specific_rules:
             - tests/testdata/rules/specific/
         generic_rules:
             - tests/testdata/rules/generic/
         hyperscan_db_path: tmp/path/scan.db
+
+.. autoclass:: logprep.processor.hyperscan_resolver.processor.HyperscanResolver.Config
+   :members:
+   :undoc-members:
+   :inherited-members:
+   :noindex:
+
+.. automodule:: logprep.processor.hyperscan_resolver.rule
 """
 
 import errno
 from logging import Logger
 from os import makedirs, path
 from typing import Any, Dict, Tuple
```

### Comparing `logprep-6.2.0/logprep/processor/hyperscan_resolver/rule.py` & `logprep-6.3.0/logprep/processor/hyperscan_resolver/rule.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 """
-Hyperscan Resolver
-==================
+Rule Configuration
+^^^^^^^^^^^^^^^^^^
 
 The hyperscan resolver requires the additional field :code:`hyperscan_resolver`.
-It works similarly to the generic resolver, but utilized hyperscan to process resolve lists.
-
-For further information see: :ref:`generic-resolver-rule`
 
 The hyperscan resolver uses the
 `Python Hyperscan library <https://python-hyperscan.readthedocs.io/en/latest/>`_
 to check regex patterns.
 By default, the compiled Hyperscan databases will be stored persistently in the directory
 specified in the :code:`pipeline.yml`.
 The field :code:`store_db_persistent` can be used to configure
 if a database compiled from a rule's :code:`resolve_list` should be stored persistently.
 
+.. autoclass:: logprep.processor.hyperscan_resolver.rule.HyperscanResolverRule.Config
+   :members:
+   :undoc-members:
+   :inherited-members:
+   :noindex:
 """
 import re
 from typing import Tuple
 
 from attrs import define, field, validators
 
 from logprep.processor.base.rule import Rule, InvalidRuleDefinitionError
```

### Comparing `logprep-6.2.0/logprep/processor/ip_informer/processor.py` & `logprep-6.3.0/logprep/processor/ip_informer/processor.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,25 +1,32 @@
 """
 IpInformer
-============
+==========
 
 The `ip_informer` processor enriches an event with ip information.
 
-
-Example
-^^^^^^^
+Processor Configuration
+^^^^^^^^^^^^^^^^^^^^^^^
 ..  code-block:: yaml
     :linenos:
 
     - myipinformer:
         type: ip_informer
         specific_rules:
             - tests/testdata/rules/specific/
         generic_rules:
             - tests/testdata/rules/generic/
+
+.. autoclass:: logprep.processor.ip_informer.processor.IpInformer.Config
+   :members:
+   :undoc-members:
+   :inherited-members:
+   :noindex:
+
+.. automodule:: logprep.processor.ip_informer.rule
 """
 import ipaddress
 from functools import partial
 from itertools import chain
 from typing import Iterable
 
 from logprep.processor.base.exceptions import ProcessingWarning
```

### Comparing `logprep-6.2.0/logprep/processor/ip_informer/rule.py` & `logprep-6.3.0/logprep/processor/ip_informer/rule.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,10 @@
 """
-IpInformer
-============
-
-The `ip_informer` processor is a processor to enrich events with ip information.
+Rule Configuration
+^^^^^^^^^^^^^^^^^^
 
 A speaking example:
 
 ..  code-block:: yaml
     :linenos:
     :caption: Given ip_informer rule
 
@@ -42,25 +40,31 @@
                 "max_prefixlen": 32,
                 "reverse_pointer": "1.5.168.192.in-addr.arpa",
                 "version": 4
             }
         }
     }
 
+.. autoclass:: logprep.processor.ip_informer.rule.IpInformerRule.Config
+   :members:
+   :undoc-members:
+   :inherited-members:
+   :noindex:
 
 Examples for ip_informer:
 ------------------------------------------------
 
 .. datatemplate:import-module:: tests.unit.processor.ip_informer.test_ip_informer
    :template: testcase-renderer.tmpl
 
 """
 from ipaddress import IPv4Address, IPv6Address
 
 from attrs import define, field, validators
+
 from logprep.processor.field_manager.rule import FieldManagerRule
 
 
 def get_ip_property_names(cls):
     """Returns all property names"""
     return [
         prop_name
@@ -99,12 +103,13 @@
         'sixtofour', 'teredo', 'version']`.
 
         Default is to extract all available properties. If you explicitly want to extract
         a property, which does not exist for an IPAddress
         (e.g. toredo which is only given for IPv4Addresses),
         the property will be extracted with the value :code:`False`.
         """
+        mapping: dict = field(default="", init=False, repr=False, eq=False)
 
     @property
     def properties(self):
         """return the configured properties"""
         return self._config.properties
```

### Comparing `logprep-6.2.0/logprep/processor/key_checker/processor.py` & `logprep-6.3.0/logprep/processor/key_checker/processor.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,26 +1,33 @@
 """
 KeyChecker
-------------
+==========
 
 The `key_checker` processor checks if all field names in a provided list are
 given in the processed event.
 
-Example
-^^^^^^^
+Processor Configuration
+^^^^^^^^^^^^^^^^^^^^^^^
 ..  code-block:: yaml
     :linenos:
 
     - keycheckername:
         type: key_checker
         specific_rules:
             - tests/testdata/rules/specific/
         generic_rules:
             - tests/testdata/rules/generic/
 
+.. autoclass:: logprep.processor.key_checker.processor.KeyChecker.Config
+   :members:
+   :undoc-members:
+   :inherited-members:
+   :noindex:
+
+.. automodule:: logprep.processor.key_checker.rule
 """
 
 from typing import Iterable
 
 from logprep.abc.processor import Processor
 from logprep.processor.base.rule import Rule
 from logprep.processor.key_checker.rule import KeyCheckerRule
```

### Comparing `logprep-6.2.0/logprep/processor/key_checker/rule.py` & `logprep-6.3.0/logprep/processor/key_checker/rule.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """
-Key Checker
-===========
+Rule Configuration
+^^^^^^^^^^^^^^^^^^
 
 The `key_checker` processor needs a list with at least one element in it.
 The Rule contains this list and it also contains a custom field where the processor
 can store all missing keys.
 
 ..  code-block:: yaml
     :linenos:
@@ -33,14 +33,19 @@
 
     {
         "testkey": "key1_value",
         "_index": "value",
         "missing_fields": "key1","key2"
     }
 
+.. autoclass:: logprep.processor.key_checker.rule.KeyCheckerRule.Config
+   :members:
+   :undoc-members:
+   :inherited-members:
+   :noindex:
 """
 
 from attrs import define, field, validators
 
 from logprep.processor.field_manager.rule import FieldManagerRule
 
 
@@ -58,7 +63,10 @@
                     iterable_validator=validators.instance_of(set),
                 ),
                 validators.min_len(1),
             ],
             converter=set,
         )
         """List of fields to check for."""
+        target_field: str = field(validator=validators.instance_of(str))
+        """The field where to write the processed values to. """
+        mapping: dict = field(default="", init=False, repr=False, eq=False)
```

### Comparing `logprep-6.2.0/logprep/processor/labeler/labeling_schema.py` & `logprep-6.3.0/logprep/processor/labeler/labeling_schema.py`

 * *Files identical despite different names*

### Comparing `logprep-6.2.0/logprep/processor/labeler/processor.py` & `logprep-6.3.0/logprep/processor/labeler/processor.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,37 +1,45 @@
 """
 Labeler
--------
+=======
+
 Labeling-Schema and validating Rules
 ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
 
 The validation of schemata and rules can be started separately by executing:
 
 ..  code-block:: bash
 
     PYTHONPATH="." python3 logprep/util/schema_and_rule_checker.py $LABELING_SCHEMA $RULES
 
 Where :code:`$LABELING_SCHEMA` is the path to a labeling schema file and :code:`$RULES` is the path
 to a directory with rule files.
 
-Example
-^^^^^^^
+Processor Configuration
+^^^^^^^^^^^^^^^^^^^^^^^
 
 ..  code-block:: yaml
     :linenos:
 
     - labelername:
         type: labeler
         schema: tests/testdata/labeler_rules/labeling/schema.json
         include_parent_labels: true
         generic_rules:
             - tests/testdata/labeler_rules/rules/
         specific_rules:
             - tests/testdata/labeler_rules/rules/
 
+.. autoclass:: logprep.processor.labeler.processor.Labeler.Config
+   :members:
+   :undoc-members:
+   :inherited-members:
+   :noindex:
+
+.. automodule:: logprep.processor.labeler.rule
 """
 
 from logging import Logger
 from typing import Optional
 
 from attr import define, field, validators
```

### Comparing `logprep-6.2.0/logprep/processor/labeler/rule.py` & `logprep-6.3.0/logprep/processor/labeler/rule.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """
-Labeler
-=======
+Rule Configuration
+^^^^^^^^^^^^^^^^^^
 
 The labeler requires the additional field :code:`label`.
 The keys under :code:`label` define the categories under which a label should be added.
 The values are a list of labels that should be added under a category.
 
 In the following example, the label :code:`execute` will be added
 to the labels of the category :code:`action`:
@@ -16,14 +16,19 @@
     filter: 'command: "executing something"'
     labeler:
         label:
             action:
             - execute
     description: '...'
 
+.. autoclass:: logprep.processor.labeler.rule.LabelerRule.Config
+   :members:
+   :undoc-members:
+   :inherited-members:
+   :noindex:
 """
 from attrs import define, field, validators
 
 from logprep.processor.base.rule import Rule
 from logprep.processor.labeler.labeling_schema import LabelingSchema
```

### Comparing `logprep-6.2.0/logprep/processor/list_comparison/processor.py` & `logprep-6.3.0/logprep/processor/list_comparison/processor.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,27 +1,35 @@
 """
 ListComparison
---------------
+==============
 
 The `list_comparison` processor allows to compare values of source fields against lists provided
 as files.
 
 
-Example
-^^^^^^^
+Processor Configuration
+^^^^^^^^^^^^^^^^^^^^^^^
 ..  code-block:: yaml
     :linenos:
 
     - listcomparisonname:
         type: list_comparison
         specific_rules:
             - tests/testdata/rules/specific/
         generic_rules:
             - tests/testdata/rules/generic/
         list_search_base_path: /path/to/list/dir
+
+.. autoclass:: logprep.processor.list_comparison.processor.ListComparison.Config
+   :members:
+   :undoc-members:
+   :inherited-members:
+   :noindex:
+
+.. automodule:: logprep.processor.list_comparison.rule
 """
 from logging import Logger
 
 from attr import define, field, validators
 
 from logprep.abc.processor import Processor
 from logprep.processor.base.exceptions import FieldExistsWarning
```

### Comparing `logprep-6.2.0/logprep/processor/list_comparison/rule.py` & `logprep-6.3.0/logprep/processor/list_comparison/rule.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """
-List Comparison
-===============
+Rule Configuration
+^^^^^^^^^^^^^^^^^^
 
 The list comparison enricher requires the additional field :code:`list_comparison`.
 The mandatory keys under :code:`list_comparison` are :code:`source_fields`
 (as list with one element) and :code:`target_field`. Former
 is used to identify the field which is to be checked against the provided lists.
 And the latter is used to define the parent field where the results should
 be written to. Both fields can be dotted subfields.
@@ -30,14 +30,19 @@
             - lists/privileged_users.txt
     description: '...'
 
 .. note::
 
     Currently it is not possible to check in more than one source_field per rule
 
+.. autoclass:: logprep.processor.list_comparison.rule.ListComparisonRule.Config
+   :members:
+   :undoc-members:
+   :inherited-members:
+   :noindex:
 """
 import os.path
 from string import Template
 from typing import List, Optional
 
 from attrs import define, field, validators
 
@@ -60,14 +65,15 @@
         )
         """List of files. For string format see :ref:`getters`."""
         list_search_base_path: str = field(validator=validators.instance_of(str), factory=str)
         """Base Path from where to find relative files from :code:`list_file_paths`.
         You can also pass a template with keys from environment,
         e.g.,  :code:`${<your environment variable>}`. The special key :code:`${LOGPREP_LIST}`
         will be filled by this processor. """
+        mapping: dict = field(default="", init=False, repr=False, eq=False)
 
     def __init__(self, filter_rule: FilterExpression, config: dict):
         super().__init__(filter_rule, config)
         self._compare_sets = {}
 
     def _get_list_search_base_path(self, list_search_base_path):
         if list_search_base_path is None:
```

### Comparing `logprep-6.2.0/logprep/processor/normalizer/processor.py` & `logprep-6.3.0/logprep/processor/normalizer/processor.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """
 Normalizer
-----------
+==========
+
 The Normalizer copies specific values to configurable fields.
 
-Example
-^^^^^^^
+Processor Configuration
+^^^^^^^^^^^^^^^^^^^^^^^
 
 ..  code-block:: yaml
     :linenos:
 
     - normalizername:
         type: normalizer
         generic_rules:
@@ -18,14 +19,22 @@
         regex_mapping: tests/testdata/unit/normalizer/normalizer_regex_mapping.yml
         html_replace_fields: tests/testdata/unit/normalizer/html_replace_fields.yml
         count_grok_pattern_matches:
             count_directory_path: "path/to/directory"
             write_period: 0.1
             lock_file_path: "path/to/lock/file"
 
+.. autoclass:: logprep.processor.normalizer.processor.Normalizer.Config
+   :members:
+   :undoc-members:
+   :inherited-members:
+   :noindex:
+
+.. automodule:: logprep.processor.normalizer.rule
+
 """
 import calendar
 import html
 import json
 import os
 import re
 from datetime import datetime
```

### Comparing `logprep-6.2.0/logprep/processor/normalizer/rule.py` & `logprep-6.3.0/logprep/processor/normalizer/rule.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # pylint: disable=anomalous-backslash-in-string
 """
-Normalizer
-==========
+Rule Configuration
+^^^^^^^^^^^^^^^^^^
 
 The normalizer requires the additional field :code:`normalize`.
 It contains key-value pairs that define if and how fields gets normalized.
 The keys describe fields that are going to be normalized and the values describe the new
 normalized fields. Through normalizing, old fields are being copied to new fields, but the old
 fields are not deleted.
```

### Comparing `logprep-6.2.0/logprep/processor/pre_detector/ip_alerter.py` & `logprep-6.3.0/logprep/processor/pre_detector/ip_alerter.py`

 * *Files identical despite different names*

### Comparing `logprep-6.2.0/logprep/processor/pre_detector/processor.py` & `logprep-6.3.0/logprep/processor/pre_detector/processor.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,29 +1,37 @@
 """
 PreDetector
------------
+===========
 
 The `pre_detector` is a processor that creates alerts for matching events. It adds MITRE ATT&CK
 data to the alerts.
 
 
-Example
-^^^^^^^
+Processor Configuration
+^^^^^^^^^^^^^^^^^^^^^^^
 ..  code-block:: yaml
     :linenos:
 
     - predetectorname:
         type: pre_detector
         specific_rules:
             - tests/testdata/rules/specific/
         generic_rules:
             - tests/testdata/rules/generic/
         outputs:
             - kafka: sre_topic
         alert_ip_list_path: /tmp/ip_list.yml
+
+.. autoclass:: logprep.processor.pre_detector.processor.PreDetector.Config
+   :members:
+   :undoc-members:
+   :inherited-members:
+   :noindex:
+
+.. automodule:: logprep.processor.pre_detector.rule
 """
 from functools import cached_property
 from logging import DEBUG, Logger
 from uuid import uuid4
 
 from attr import define, field, validators
```

### Comparing `logprep-6.2.0/logprep/processor/pre_detector/rule.py` & `logprep-6.3.0/logprep/processor/pre_detector/rule.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """
-PreDetector
-===========
+Rule Configuration
+^^^^^^^^^^^^^^^^^^
 
 The predetector requires the additional field :code:`pre_detector`.
 
 The rule fields and a `pre_detector_id` are written into a custom output
 of the current output connector.
 The `pre_detector_id` will be furthermore added to the triggering event
 so that an event can be linked with its detection.
@@ -43,17 +43,24 @@
       severity: critical
       mitre:
       - some_tag
       case_condition: directly
     description: Some malicous event.
     ip_fields:
     - some_ip_field
+
+.. autoclass:: logprep.processor.pre_detector.rule.PreDetectorRule.Config
+   :members:
+   :undoc-members:
+   :inherited-members:
+   :noindex:
 """
 from functools import cached_property
 from typing import Union, Optional
+
 from attrs import define, field, validators, asdict
 
 from logprep.processor.base.rule import Rule
 
 
 class PreDetectorRule(Rule):
     """Check if documents match a filter."""
```

### Comparing `logprep-6.2.0/logprep/processor/processor_strategy.py` & `logprep-6.3.0/logprep/processor/processor_strategy.py`

 * *Files identical despite different names*

### Comparing `logprep-6.2.0/logprep/processor/pseudonymizer/encrypter.py` & `logprep-6.3.0/logprep/processor/pseudonymizer/encrypter.py`

 * *Files identical despite different names*

### Comparing `logprep-6.2.0/logprep/processor/pseudonymizer/processor.py` & `logprep-6.3.0/logprep/processor/pseudonymizer/processor.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 """
 Pseudonymizer
--------------
+=============
 
 The `pseudonymizer` is a processor that pseudonymizes certain fields of log messages to ensure
 privacy regulations can be adhered to.
 
-
-Example
-^^^^^^^
+Processor Configuration
+^^^^^^^^^^^^^^^^^^^^^^^
 ..  code-block:: yaml
     :linenos:
 
     - pseudonymizername:
         type: pseudonymizer
         specific_rules:
             - tests/testdata/rules/specific/
@@ -23,14 +22,22 @@
         pubkey_depseudo: /path/to/depseudo_pubkey.pem
         hash_salt: secret_salt
         regex_mapping: /path/to/regex_mapping.json
         max_cached_pseudonyms: 1000000
         max_caching_days: 1
         tld_lists:
             -/path/to/tld_list.dat
+
+.. autoclass:: logprep.processor.pseudonymizer.processor.Pseudonymizer.Config
+   :members:
+   :undoc-members:
+   :inherited-members:
+   :noindex:
+
+.. automodule:: logprep.processor.pseudonymizer.rule
 """
 import datetime
 import re
 from functools import cached_property
 from logging import Logger
 from typing import Any, List, Optional, Tuple, Union, Pattern
 from urllib.parse import parse_qs
```

### Comparing `logprep-6.2.0/logprep/processor/pseudonymizer/rule.py` & `logprep-6.3.0/logprep/processor/pseudonymizer/rule.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """
-Pseudonymizer
-=============
+Rule Configuration
+^^^^^^^^^^^^^^^^^^
 
 The pseudonymizer requires the additional field :code:`pseudonymizer.pseudonyms`.
 It contains key value pairs that define what will be pseudonymized.
 
 They key represents the field that will be pseudonymized and the value contains a regex keyword.
 The regex keyword defines which parts of the value are being pseudonymized.
 Only the regex matches are being pseudonymized that are also in a capture group.
@@ -33,14 +33,19 @@
 
     {
       "RE_WHOLE_FIELD": "(.*)",
       "RE_DOMAIN_BACKSLASH_USERNAME": "\\w+\\\\(.*)",
       "RE_IP4_COLON_PORT": "([\\d.]+):\\d+"
     }
 
+.. autoclass:: logprep.processor.pseudonymizer.rule.PseudonymizerRule.Config
+   :members:
+   :undoc-members:
+   :inherited-members:
+   :noindex:
 """
 
 from typing import List
 
 from attrs import define, field, validators
 
 from logprep.processor.base.rule import Rule
```

### Comparing `logprep-6.2.0/logprep/processor/requester/processor.py` & `logprep-6.3.0/logprep/processor/requester/processor.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,28 +1,33 @@
 """
 Requester
 =========
 
 A processor to invoke http requests. Can be used to enrich events from an external api or
 to trigger external systems by and with event field values.
 
-For further information for the rule language see: :ref:`requester_rule`.
-
-Example
-^^^^^^^
+Processor Configuration
+^^^^^^^^^^^^^^^^^^^^^^^
 ..  code-block:: yaml
     :linenos:
 
     - requestername:
         type: requester
         specific_rules:
             - tests/testdata/rules/specific/
         generic_rules:
             - tests/testdata/rules/generic/
 
+.. autoclass:: logprep.processor.requester.processor.Requester.Config
+   :members:
+   :undoc-members:
+   :inherited-members:
+   :noindex:
+
+.. automodule:: logprep.processor.requester.rule
 """
 import json
 import re
 
 import requests
 
 from logprep.abc.processor import Processor
```

### Comparing `logprep-6.2.0/logprep/processor/requester/rule.py` & `logprep-6.3.0/logprep/processor/requester/rule.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,10 @@
 """
-.. _requester_rule:
-
-Requester
-=========
+Rule Configuration
+^^^^^^^^^^^^^^^^^^
 
 The Requester is configured by the keyword :code:`requester`.
 It can be used to trigger external systems via web request or enrich eventdata by external
 apis.
 
 A speaking example for event enrichment via external api:
 
@@ -53,14 +51,20 @@
              "city": "Montreal",
              "Building": "L76",
              "Floor": 3,
              "Room": 34
              }
         }
     }
+
+.. autoclass:: logprep.processor.requester.rule.RequesterRule.Config
+   :members:
+   :undoc-members:
+   :inherited-members:
+   :noindex:
 """
 import inspect
 import json
 import re
 
 import requests
 from attrs import define, field, validators
@@ -166,14 +170,15 @@
             factory=dict,
         )
         """(Optional) Dictionary mapping protocol or protocol and host to the
         URL of the proxy (e.g. :code:`{"http": "foo.bar:3128", "http://host.name": "foo.bar:4012"}`)
         to be used on the request"""
         cert: str = field(validator=validators.instance_of(str), default="")
         """(Optional) SSL client certificate as path to ssl client cert file (.pem)."""
+        mapping: dict = field(default="", init=False, repr=False, eq=False)
 
         def __attrs_post_init__(self):
             url_fields = re.findall(FIELD_PATTERN, self.url)
             json_fields = re.findall(FIELD_PATTERN, json.dumps(self.json))
             data_fields = re.findall(FIELD_PATTERN, self.data)
             params_fields = re.findall(FIELD_PATTERN, json.dumps(self.params))
             self.source_fields = list({*url_fields, *json_fields, *data_fields, *params_fields})
```

### Comparing `logprep-6.2.0/logprep/processor/selective_extractor/processor.py` & `logprep-6.3.0/logprep/processor/selective_extractor/processor.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,36 +1,42 @@
 """
 SelectiveExtractor
-------------------
+==================
 
 The `selective_extractor` is a processor that allows to write field values of a given log message to
 a different Kafka topic. The output topic is configured via the pipeline yml, while the fields to
 be extracted are specified by means of a list which is also specified in the pipeline configuration
 as a file path. This processor is applied to all messages, because of that it does not need further
 rules to specify it's behavior.
 
-
-Example
-^^^^^^^
+Processor Configuration
+^^^^^^^^^^^^^^^^^^^^^^^
 ..  code-block:: yaml
     :linenos:
 
     - selectiveextractorname:
         type: selective_extractor
         specific_rules:
             - tests/testdata/rules/specific/
         generic_rules:
             - tests/testdata/rules/generic/
+
+.. autoclass:: logprep.processor.selective_extractor.processor.SelectiveExtractor.Config
+   :members:
+   :undoc-members:
+   :inherited-members:
+   :noindex:
+
+.. automodule:: logprep.processor.selective_extractor.rule
 """
 
 from logging import Logger
 from typing import List, Tuple
 
 from logprep.processor.field_manager.processor import FieldManager
-
 from logprep.processor.selective_extractor.rule import SelectiveExtractorRule
 from logprep.util.helper import add_field_to, get_source_fields_dict
 
 
 class SelectiveExtractor(FieldManager):
     """Processor used to selectively extract fields from log events."""
```

### Comparing `logprep-6.2.0/logprep/processor/selective_extractor/rule.py` & `logprep-6.3.0/logprep/processor/selective_extractor/rule.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """
-Selective Extractor
-===================
+Rule Configuration
+^^^^^^^^^^^^^^^^^^
 
 The selective extractor requires the additional field :code:`selective_extractor`.
 It contains a list of field names that should be extracted (:code:`source_fields`)
 and list of output mappings to which they should be send to (:code:`outputs`).
 If dotted notation is being used, then all fields on the path are being automatically
 created.
 
@@ -88,14 +88,19 @@
 ..  code-block:: text
     :caption: Example of file with field list
 
     field1
     field2
     field3
 
+.. autoclass:: logprep.processor.selective_extractor.rule.SelectiveExtractorRule.Config
+   :members:
+   :undoc-members:
+   :inherited-members:
+   :noindex:
 """
 
 from typing import List
 
 from attrs import define, field, validators
 
 from logprep.processor.base.rule import InvalidRuleDefinitionError
@@ -124,15 +129,14 @@
                     iterable_validator=validators.instance_of(list),
                 )
             ],
             factory=list,
             converter=sorted,
         )
         """List of fields in dotted field notation"""
-
         outputs: tuple[dict[str, str]] = field(
             validator=[
                 validators.deep_iterable(
                     member_validator=[
                         validators.instance_of(dict),
                         validators.deep_mapping(
                             key_validator=validators.instance_of(str),
@@ -144,24 +148,21 @@
                 ),
                 validators.min_len(1),
             ],
             converter=tuple,
         )
         """list of output mappings in form of :code:`output_name:topic`.
         Only one mapping is allowed per list element"""
-
         extract_from_file: str = field(validator=validators.instance_of(str), default="", eq=False)
         """The path or url to a file with a flat list of fields to extract.
         For string format see :ref:`getters`."""
-
         target_field: str = field(default="", init=False, repr=False, eq=False)
-
         overwrite_target: bool = field(default=False, init=False, repr=False, eq=False)
-
         extend_target_list: bool = field(default=False, init=False, repr=False, eq=False)
+        mapping: dict = field(default="", init=False, repr=False, eq=False)
 
         def __attrs_post_init__(self):
             super().__attrs_post_init__()
             if not self.extract_from_file:
                 return
             try:
                 content = GetterFactory.from_string(self.extract_from_file).get()
```

### Comparing `logprep-6.2.0/logprep/processor/string_splitter/processor.py` & `logprep-6.3.0/logprep/processor/string_splitter/processor.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,26 +1,33 @@
 """
 StringSplitter
 ==============
 
-The `string_splitter` processor splits string by whitespace (default) or a given delimeter and
+The `string_splitter` processor splits string by whitespace (default) or a given delimiter and
 writes the resulting list to a target field.
 
-
-Example
-^^^^^^^
+Processor Configuration
+^^^^^^^^^^^^^^^^^^^^^^^
 ..  code-block:: yaml
     :linenos:
 
     - samplename:
         type: string_splitter
         specific_rules:
             - tests/testdata/rules/specific/
         generic_rules:
             - tests/testdata/rules/generic/
+
+.. autoclass:: logprep.processor.string_splitter.processor.StringSplitter.Config
+   :members:
+   :undoc-members:
+   :inherited-members:
+   :noindex:
+
+.. automodule:: logprep.processor.string_splitter.rule
 """
 
 from logprep.processor.base.exceptions import FieldExistsWarning, ProcessingWarning
 from logprep.processor.field_manager.processor import FieldManager
 from logprep.processor.string_splitter.rule import StringSplitterRule
 from logprep.util.helper import add_field_to, get_dotted_field_value
```

### Comparing `logprep-6.2.0/logprep/processor/string_splitter/rule.py` & `logprep-6.3.0/logprep/processor/string_splitter/rule.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,13 +1,10 @@
 """
-StringSplitter
-==============
-
-The `string_splitter` processor splits string by whitespace (default) or a given delimeter and
-writes the resulting list to a target field.
+Rule Configuration
+^^^^^^^^^^^^^^^^^^
 
 A speaking example:
 
 ..  code-block:: yaml
     :linenos:
     :caption: Given string_splitter rule
 
@@ -41,24 +38,26 @@
 
 .. datatemplate:import-module:: tests.unit.processor.string_splitter.test_string_splitter
    :template: testcase-renderer.tmpl
 
 """
 
 from attrs import define, field, validators
+
 from logprep.processor.field_manager.rule import FieldManagerRule
 
 
 class StringSplitterRule(FieldManagerRule):
     """..."""
 
     @define(kw_only=True)
     class Config(FieldManagerRule.Config):
         """Config for StringSplitterRule"""
 
         delimeter: str = field(validator=validators.instance_of(str), default=" ")
         """The delimeter for splitting. Defaults to whitespace"""
+        mapping: dict = field(default="", init=False, repr=False, eq=False)
 
     @property
     def delimeter(self):
         """returns the configured delimeter"""
         return self._config.delimeter
```

### Comparing `logprep-6.2.0/logprep/processor/template_replacer/processor.py` & `logprep-6.3.0/logprep/processor/template_replacer/processor.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 """
 TemplateReplacer
-----------------
+================
 
 The `template_replacer` is a processor that can replace parts of a text field to anonymize those
 parts. The replacement is based on a template file.
 
-
-Example
-^^^^^^^
+Processor Configuration
+^^^^^^^^^^^^^^^^^^^^^^^
 ..  code-block:: yaml
     :linenos:
 
     - templatereplacername:
         type: template_replacer
         specific_rules:
             - tests/testdata/rules/specific/
@@ -21,14 +20,22 @@
         pattern:
             delimiter: ","
             fields:
                 - field.name.a
                 - field.name.b
             allowed_delimiter_field: field.name.b
             target_field: target.field
+
+.. autoclass:: logprep.processor.template_replacer.processor.TemplateReplacer.Config
+   :members:
+   :undoc-members:
+   :inherited-members:
+   :noindex:
+
+.. automodule:: logprep.processor.template_replacer.rule
 """
 from logging import Logger
 from typing import Optional
 
 from attr import define, field, validators
 
 from logprep.abc.processor import Processor
```

### Comparing `logprep-6.2.0/logprep/processor/template_replacer/rule.py` & `logprep-6.3.0/logprep/processor/template_replacer/rule.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,9 +1,10 @@
-"""Template Replacer
-====================
+"""
+Rule Configuration
+^^^^^^^^^^^^^^^^^^
 
 The template replacer requires the additional field :code:`template_replacer`.
 No additional configuration parameters are required for the rules.
 The module is completely configured over the pipeline configuration.
 
 In the following example the target field specified in the processor configuration
 is replaced for all log messages that have :code:`winlog.provider_name` and
@@ -13,14 +14,19 @@
     :linenos:
     :caption: Example
 
     filter: winlog.provider_name AND winlog.event_id
     template_replacer: {}
     description: ''
 
+.. autoclass:: logprep.processor.template_replacer.rule.TemplateReplacerRule.Config
+   :members:
+   :undoc-members:
+   :inherited-members:
+   :noindex:
 """
 
 from logprep.processor.base.rule import Rule
 
 
 class TemplateReplacerRule(Rule):
     """Check if documents match a filter."""
```

### Comparing `logprep-6.2.0/logprep/processor/timestamp_differ/processor.py` & `logprep-6.3.0/logprep/processor/timestamp_differ/processor.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,25 +1,32 @@
 """
 TimestampDiffer
 ===============
 
 The `timestamp_differ` can calculate the time difference between two timestamps.
-For further information for the rule language see: :ref:`timestamp_differ_rule`.
 
-Example
-^^^^^^^
+Processor Configuration
+^^^^^^^^^^^^^^^^^^^^^^^
 ..  code-block:: yaml
     :linenos:
 
     - timestampdiffer_name:
         type: timestamp_differ
         specific_rules:
             - tests/testdata/rules/specific/
         generic_rules:
             - tests/testdata/rules/generic/
+
+.. autoclass:: logprep.processor.timestamp_differ.processor.TimestampDiffer.Config
+   :members:
+   :undoc-members:
+   :inherited-members:
+   :noindex:
+
+.. automodule:: logprep.processor.timestamp_differ.rule
 """
 from datetime import datetime
 from functools import reduce
 from typing import Union
 
 from logprep.abc.processor import Processor
 from logprep.processor.base.exceptions import FieldExistsWarning
```

### Comparing `logprep-6.2.0/logprep/processor/timestamp_differ/rule.py` & `logprep-6.3.0/logprep/processor/timestamp_differ/rule.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,11 @@
 """
-.. _timestamp_differ_rule:
+Rule Configuration
+^^^^^^^^^^^^^^^^^^
 
-TimestampDiffer
-===============
-
-The `timestamp_differ` processor allows to calculate the time difference between two timestamps.
 The timestamp format can be specified per timestamp. Following patterns can be used to define the
 timestamp format:
 `Timestamp tokens <https://docs.python.org/3/library/datetime.html#strftime-and-strptime-format-codes>`_.
 
 A speaking example:
 
 ..  code-block:: yaml
@@ -30,14 +27,20 @@
 
 ..  code-block:: json
     :linenos:
     :caption: Processed event
 
     {"ingest": "2022-12-06 10:00:00", "processed": "2022-12-06 10:00:05", "processing_time": "5.0"}
 
+.. autoclass:: logprep.processor.timestamper.rule.TimestamperRule.Config
+   :members:
+   :undoc-members:
+   :inherited-members:
+   :noindex:
+
 Examples for timestamp_differ:
 ------------------------------
 
 .. datatemplate:import-module:: tests.unit.processor.timestamp_differ.test_timestamp_differ
    :template: testcase-renderer.tmpl
 """
 import re
@@ -51,17 +54,14 @@
 class TimestampDifferRule(FieldManagerRule):
     """TimestampDifferRule"""
 
     @define(kw_only=True)
     class Config(FieldManagerRule.Config):
         """Config for TimestampDiffer"""
 
-        source_fields: list = field(factory=list, init=False, repr=False, eq=False)
-        source_field_formats: list = field(factory=list, init=False, repr=False, eq=False)
-
         diff: str = field(
             validator=[
                 validators.instance_of(str),
                 validators.matches_re(rf"({FIELD_PATTERN} - {FIELD_PATTERN})"),
             ]
         )
         """Specifies the timestamp subtraction and their respective timestamp formats. The fields
@@ -81,14 +81,15 @@
         )
         """(Optional) Specifies the desired output format of the timestamp difference, allowed
         values are: :code:`seconds`, :code:`milliseconds`, :code:`nanoseconds`, defaults to:
         :code:`seconds`."""
         show_unit: bool = field(default=False)
         """(Optional) Specifies whether the unit (s, ms, ns) should be part of the output.
         Defaults to :code:`False`."""
+        mapping: dict = field(default="", init=False, repr=False, eq=False)
 
         def __attrs_post_init__(self):
             field_format_str = re.findall(FIELD_PATTERN, self.diff)
             field_format_tuple = map(lambda s: s.split(":", maxsplit=1), field_format_str)
             field_format_tuple = map(lambda x: x + [None] if len(x) == 1 else x, field_format_tuple)
             source_fields, source_field_formats = list(map(list, zip(*field_format_tuple)))
             self.source_fields = source_fields
```

### Comparing `logprep-6.2.0/logprep/processor/timestamper/processor.py` & `logprep-6.3.0/logprep/processor/timestamper/processor.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,25 +1,33 @@
 """
 Timestamper
-============
+===========
 
 The `timestamper` processor normalizes timestamps to *iso8601* compliant output format.
 
-
-Example
-^^^^^^^
+Processor Configuration
+^^^^^^^^^^^^^^^^^^^^^^^
 ..  code-block:: yaml
     :linenos:
 
     - myteimestamper:
         type: timestamper
         specific_rules:
             - tests/testdata/rules/specific/
         generic_rules:
             - tests/testdata/rules/generic/
+
+
+.. autoclass:: logprep.processor.timestamper.processor.Timestamper.Config
+   :members:
+   :undoc-members:
+   :inherited-members:
+   :noindex:
+
+.. automodule:: logprep.processor.timestamper.rule
 """
 
 from logprep.processor.base.exceptions import ProcessingWarning
 from logprep.processor.field_manager.processor import FieldManager
 from logprep.processor.timestamper.rule import TimestamperRule
 from logprep.util.helper import get_dotted_field_value
 from logprep.util.time import TimeParser, TimeParserException
@@ -28,25 +36,31 @@
 class Timestamper(FieldManager):
     """A processor that extracts and parses timestamps"""
 
     rule_class = TimestamperRule
 
     def _apply_rules(self, event, rule):
         source_field = self._get_source_field(event, rule)
-        source_timezone, target_timezone, source_format = (
+        source_timezone, target_timezone, source_formats = (
             rule.source_timezone,
             rule.target_timezone,
             rule.source_format,
         )
-        try:
-            parsed_datetime = self._parse_datetime(source_field, source_format, source_timezone)
-        except TimeParserException as error:
-            raise ProcessingWarning(self, str(error), rule, event) from error
-        result = parsed_datetime.astimezone(target_timezone).isoformat().replace("+00:00", "Z")
-        self._write_target_field(event, rule, result)
+        parsed_successfully = False
+        for source_format in source_formats:
+            try:
+                parsed_datetime = self._parse_datetime(source_field, source_format, source_timezone)
+            except TimeParserException:
+                continue
+            result = parsed_datetime.astimezone(target_timezone).isoformat().replace("+00:00", "Z")
+            self._write_target_field(event, rule, result)
+            parsed_successfully = True
+            break
+        if not parsed_successfully:
+            raise ProcessingWarning(self, str("Could not parse timestamp"), rule, event)
 
     def _get_source_field(self, event, rule):
         source_field = rule.source_fields[0]
         source_field_value = get_dotted_field_value(event, source_field)
         if not source_field_value:
             raise ProcessingWarning(
                 self, f"'{source_field}' does not exist or is falsy value", rule, event
```

### Comparing `logprep-6.2.0/logprep/processor/timestamper/rule.py` & `logprep-6.3.0/logprep/processor/timestamper/rule.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,12 +1,10 @@
 """
-Timestamper
-============
-
-The `timestamper` processor normalizes timestamps to *iso8601* compliant output format.
+Rule Configuration
+^^^^^^^^^^^^^^^^^^
 
 A speaking example:
 
 ..  code-block:: yaml
     :linenos:
     :caption: Given timestamper rule
 
@@ -79,32 +77,40 @@
                 validators.max_len(1),
                 validators.deep_iterable(member_validator=validators.instance_of(str)),
             ]
         )
         """The field from where to get the time from as list with one element"""
         target_field: str = field(validator=validators.instance_of(str), default="@timestamp")
         """The field where to write the processed values to, defaults to :code:`@timestamp`"""
-        source_format: str = field(validator=validators.instance_of(str), default="ISO8601")
-        """The source format if source_fields is not an iso8601 compliant time format string
+        source_format: list = field(
+            validator=validators.deep_iterable(
+                member_validator=validators.instance_of(str),
+                iterable_validator=validators.instance_of(list),
+            ),
+            default=["ISO8601"],
+            converter=lambda x: x if isinstance(x, list) else [x],
+        )
+        """A list of possible source formats if source_fields is not an iso8601 compliant time format string
         the format must be given in the syntax of the python builtin :code:`datetime.strptime`
         (see: https://docs.python.org/3/library/datetime.html#strftime-and-strptime-format-codes).
-        Additionally, the value :code:`ISO8601` (default)  and :code:`UNIX` can be used for
-        the source_formats field. The former can be used if the timestamp already exists
+        Additionally, the value :code:`ISO8601` (default)  and :code:`UNIX` can be used in the list
+        of the source_formats field. The former can be used if the timestamp already exists
         in the ISO8601 format, such that only a timezone conversion should be applied.
         And the latter can be used if the timestamp is given in the UNIX Epoch Time.
         This supports the Unix timestamps in seconds and milliseconds.
         """
         source_timezone: ZoneInfo = field(
             validator=[validators.instance_of(ZoneInfo)], converter=ZoneInfo, default="UTC"
         )
         """ timezone of source_fields. defaults to :code:`UTC`"""
         target_timezone: ZoneInfo = field(
             validator=[validators.instance_of(ZoneInfo)], converter=ZoneInfo, default="UTC"
         )
         """ timezone for target_field. defaults to :code:`UTC`"""
+        mapping: dict = field(default="", init=False, repr=False, eq=False)
 
     @property
     def source_format(self):
         """returns the source format"""
         return self._config.source_format
 
     @property
```

### Comparing `logprep-6.2.0/logprep/registry.py` & `logprep-6.3.0/logprep/registry.py`

 * *Files identical despite different names*

### Comparing `logprep-6.2.0/logprep/run_logprep.py` & `logprep-6.3.0/logprep/run_logprep.py`

 * *Files identical despite different names*

### Comparing `logprep-6.2.0/logprep/runner.py` & `logprep-6.3.0/logprep/runner.py`

 * *Files identical despite different names*

### Comparing `logprep-6.2.0/logprep/util/aggregating_logger.py` & `logprep-6.3.0/logprep/util/aggregating_logger.py`

 * *Files identical despite different names*

### Comparing `logprep-6.2.0/logprep/util/auto_rule_tester/auto_rule_corpus_tester.py` & `logprep-6.3.0/logprep/util/auto_rule_tester/auto_rule_corpus_tester.py`

 * *Files identical despite different names*

### Comparing `logprep-6.2.0/logprep/util/auto_rule_tester/auto_rule_tester.py` & `logprep-6.3.0/logprep/util/auto_rule_tester/auto_rule_tester.py`

 * *Files identical despite different names*

### Comparing `logprep-6.2.0/logprep/util/auto_rule_tester/grok_pattern_replacer.py` & `logprep-6.3.0/logprep/util/auto_rule_tester/grok_pattern_replacer.py`

 * *Files identical despite different names*

### Comparing `logprep-6.2.0/logprep/util/cache.py` & `logprep-6.3.0/logprep/util/cache.py`

 * *Files identical despite different names*

### Comparing `logprep-6.2.0/logprep/util/configuration.py` & `logprep-6.3.0/logprep/util/configuration.py`

 * *Files identical despite different names*

### Comparing `logprep-6.2.0/logprep/util/decorators.py` & `logprep-6.3.0/logprep/util/decorators.py`

 * *Files identical despite different names*

### Comparing `logprep-6.2.0/logprep/util/getter.py` & `logprep-6.3.0/logprep/util/getter.py`

 * *Files identical despite different names*

### Comparing `logprep-6.2.0/logprep/util/grok/grok.py` & `logprep-6.3.0/logprep/util/grok/grok.py`

 * *Files 7% similar despite different names*

```diff
@@ -48,15 +48,15 @@
 class Grok:
     """Grok object"""
 
     field_pattern = re.compile(r"\[(.*?)\]")
     grok_pattern = re.compile(GROK)
     oniguruma = re.compile(ONIGURUMA)
 
-    pattern: str = field(validator=validators.instance_of(str))
+    pattern: str = field(validator=validators.instance_of((str, list)))
     custom_patterns_dir: str = field(default="")
     custom_patterns: dict = field(factory=dict)
     fullmatch: bool = field(default=True)
     predefined_patterns: dict = field(init=False, factory=dict, repr=False)
     type_mapper: dict = field(init=False, factory=dict)
     field_mapper: dict = field(init=False, factory=dict)
     regex_obj = field(init=False, default=None)
@@ -75,35 +75,43 @@
             self.predefined_patterns.update(custom_pats)
 
         self._load_search_pattern()
 
     def match(self, text):
         """If text is matched with pattern, return variable names
         specified(%{pattern:variable name}) in pattern and their
-        corresponding values.If not matched, return None.
+        corresponding values. If not matched, return None.
         custom patterns can be passed in by
         custom_patterns(pattern name, pattern regular expression pair)
         or custom_patterns_dir.
         """
 
-        match_obj = None
         if self.fullmatch:
-            match_obj = self.regex_obj.fullmatch(text)
+            match_obj = [regex_pattern.fullmatch(text) for regex_pattern in self.regex_obj]
         else:
-            match_obj = self.regex_obj.search(text)
+            match_obj = [regex_pattern.search(text) for regex_pattern in self.regex_obj]
 
-        if match_obj is None:
-            return None
-        matches = match_obj.groupdict()
+        match_obj = [match for match in match_obj if match is not None]
+        matches = [match.groupdict() for match in match_obj]
         if self.type_mapper:
-            for key, match in matches.items():
-                type_ = INT_FLOAT.get(self.type_mapper.get(key))
-                if type_ is not None and match is not None:
-                    matches[key] = type_(match)
-        return {self.field_mapper[field_hash]: value for field_hash, value in matches.items()}
+            matches = list(map(self._map_types, matches))
+        # deduplicate matches
+        matches = [dict(tup) for tup in {tuple(match.items()) for match in matches}]
+        return {
+            self.field_mapper[field_hash]: value
+            for match in matches
+            for field_hash, value in match.items()
+        }
+
+    def _map_types(self, matches):
+        for key, match in matches.items():
+            type_ = INT_FLOAT.get(self.type_mapper.get(key))
+            if type_ is not None and match is not None:
+                matches[key] = type_(match)
+        return matches
 
     def set_search_pattern(self, pattern=None):
         """sets the search pattern"""
         if not isinstance(pattern, str):
             raise ValueError("Please supply a valid pattern")
         self.pattern = pattern
         self._load_search_pattern()
@@ -144,30 +152,35 @@
         dotted_fields = self._to_dotted_field(dundered_fields)
         fields_hash = f"md5{md5(fields.encode()).hexdigest()}"  # nosemgrep
         self.field_mapper |= {fields_hash: dotted_fields}
         return rf"(?P<{fields_hash}>" rf"{pattern})"
 
     def _load_search_pattern(self):
         py_regex_pattern = self.pattern
+        if isinstance(py_regex_pattern, list):
+            self.regex_obj = list(map(self._compile_pattern, py_regex_pattern))
+        else:
+            self.regex_obj = [self._compile_pattern(py_regex_pattern)]
+
+    def _compile_pattern(self, py_regex_pattern):
         while re.search(Grok.oniguruma, py_regex_pattern):
             py_regex_pattern = re.sub(
                 Grok.oniguruma,
                 self._resolve_oniguruma,
                 py_regex_pattern,
                 count=1,
             )
         while re.search(Grok.grok_pattern, py_regex_pattern):
             py_regex_pattern = re.sub(
                 Grok.grok_pattern,
                 self._resolve_grok,
                 py_regex_pattern,
                 count=1,
             )
-
-        self.regex_obj = re.compile(py_regex_pattern)
+        return re.compile(py_regex_pattern)
 
 
 def _reload_patterns(patterns_dirs):
     """ """
     patterns_dirs = [Path(directory) for directory in patterns_dirs]
     patterns_dirs += chain(*[list(directory.rglob("**/*")) for directory in patterns_dirs])
     patterns_dirs = [directory for directory in patterns_dirs if directory.is_dir()]
```

### Comparing `logprep-6.2.0/logprep/util/grok/patterns/ecs-v1/aws` & `logprep-6.3.0/logprep/util/grok/patterns/ecs-v1/aws`

 * *Files identical despite different names*

### Comparing `logprep-6.2.0/logprep/util/grok/patterns/ecs-v1/bacula` & `logprep-6.3.0/logprep/util/grok/patterns/ecs-v1/bacula`

 * *Files identical despite different names*

### Comparing `logprep-6.2.0/logprep/util/grok/patterns/ecs-v1/bind` & `logprep-6.3.0/logprep/util/grok/patterns/ecs-v1/bind`

 * *Files identical despite different names*

### Comparing `logprep-6.2.0/logprep/util/grok/patterns/ecs-v1/bro` & `logprep-6.3.0/logprep/util/grok/patterns/ecs-v1/bro`

 * *Files identical despite different names*

### Comparing `logprep-6.2.0/logprep/util/grok/patterns/ecs-v1/exim` & `logprep-6.3.0/logprep/util/grok/patterns/ecs-v1/exim`

 * *Files identical despite different names*

### Comparing `logprep-6.2.0/logprep/util/grok/patterns/ecs-v1/firewalls` & `logprep-6.3.0/logprep/util/grok/patterns/ecs-v1/firewalls`

 * *Files identical despite different names*

### Comparing `logprep-6.2.0/logprep/util/grok/patterns/ecs-v1/grok-patterns` & `logprep-6.3.0/logprep/util/grok/patterns/ecs-v1/grok-patterns`

 * *Files identical despite different names*

### Comparing `logprep-6.2.0/logprep/util/grok/patterns/ecs-v1/haproxy` & `logprep-6.3.0/logprep/util/grok/patterns/ecs-v1/haproxy`

 * *Files identical despite different names*

### Comparing `logprep-6.2.0/logprep/util/grok/patterns/ecs-v1/httpd` & `logprep-6.3.0/logprep/util/grok/patterns/ecs-v1/httpd`

 * *Files identical despite different names*

### Comparing `logprep-6.2.0/logprep/util/grok/patterns/ecs-v1/java` & `logprep-6.3.0/logprep/util/grok/patterns/ecs-v1/java`

 * *Files identical despite different names*

### Comparing `logprep-6.2.0/logprep/util/grok/patterns/ecs-v1/junos` & `logprep-6.3.0/logprep/util/grok/patterns/ecs-v1/junos`

 * *Files identical despite different names*

### Comparing `logprep-6.2.0/logprep/util/grok/patterns/ecs-v1/linux-syslog` & `logprep-6.3.0/logprep/util/grok/patterns/ecs-v1/linux-syslog`

 * *Files identical despite different names*

### Comparing `logprep-6.2.0/logprep/util/grok/patterns/ecs-v1/mongodb` & `logprep-6.3.0/logprep/util/grok/patterns/ecs-v1/mongodb`

 * *Files identical despite different names*

### Comparing `logprep-6.2.0/logprep/util/grok/patterns/ecs-v1/nagios` & `logprep-6.3.0/logprep/util/grok/patterns/ecs-v1/nagios`

 * *Files identical despite different names*

### Comparing `logprep-6.2.0/logprep/util/grok/patterns/ecs-v1/rails` & `logprep-6.3.0/logprep/util/grok/patterns/ecs-v1/rails`

 * *Files identical despite different names*

### Comparing `logprep-6.2.0/logprep/util/grok/patterns/ecs-v1/squid` & `logprep-6.3.0/logprep/util/grok/patterns/ecs-v1/squid`

 * *Files identical despite different names*

### Comparing `logprep-6.2.0/logprep/util/grok/patterns/ecs-v1/zeek` & `logprep-6.3.0/logprep/util/grok/patterns/ecs-v1/zeek`

 * *Files identical despite different names*

### Comparing `logprep-6.2.0/logprep/util/grok/patterns/legacy/aws` & `logprep-6.3.0/logprep/util/grok/patterns/legacy/aws`

 * *Files identical despite different names*

### Comparing `logprep-6.2.0/logprep/util/grok/patterns/legacy/bacula` & `logprep-6.3.0/logprep/util/grok/patterns/legacy/bacula`

 * *Files identical despite different names*

### Comparing `logprep-6.2.0/logprep/util/grok/patterns/legacy/bro` & `logprep-6.3.0/logprep/util/grok/patterns/legacy/bro`

 * *Files identical despite different names*

### Comparing `logprep-6.2.0/logprep/util/grok/patterns/legacy/exim` & `logprep-6.3.0/logprep/util/grok/patterns/legacy/exim`

 * *Files identical despite different names*

### Comparing `logprep-6.2.0/logprep/util/grok/patterns/legacy/firewalls` & `logprep-6.3.0/logprep/util/grok/patterns/legacy/firewalls`

 * *Files identical despite different names*

### Comparing `logprep-6.2.0/logprep/util/grok/patterns/legacy/grok-patterns` & `logprep-6.3.0/logprep/util/grok/patterns/legacy/grok-patterns`

 * *Files identical despite different names*

### Comparing `logprep-6.2.0/logprep/util/grok/patterns/legacy/haproxy` & `logprep-6.3.0/logprep/util/grok/patterns/legacy/haproxy`

 * *Files identical despite different names*

### Comparing `logprep-6.2.0/logprep/util/grok/patterns/legacy/httpd` & `logprep-6.3.0/logprep/util/grok/patterns/legacy/httpd`

 * *Files identical despite different names*

### Comparing `logprep-6.2.0/logprep/util/grok/patterns/legacy/java` & `logprep-6.3.0/logprep/util/grok/patterns/legacy/java`

 * *Files identical despite different names*

### Comparing `logprep-6.2.0/logprep/util/grok/patterns/legacy/junos` & `logprep-6.3.0/logprep/util/grok/patterns/legacy/junos`

 * *Files identical despite different names*

### Comparing `logprep-6.2.0/logprep/util/grok/patterns/legacy/linux-syslog` & `logprep-6.3.0/logprep/util/grok/patterns/legacy/linux-syslog`

 * *Files identical despite different names*

### Comparing `logprep-6.2.0/logprep/util/grok/patterns/legacy/mongodb` & `logprep-6.3.0/logprep/util/grok/patterns/legacy/mongodb`

 * *Files identical despite different names*

### Comparing `logprep-6.2.0/logprep/util/grok/patterns/legacy/nagios` & `logprep-6.3.0/logprep/util/grok/patterns/legacy/nagios`

 * *Files identical despite different names*

### Comparing `logprep-6.2.0/logprep/util/grok/patterns/legacy/rails` & `logprep-6.3.0/logprep/util/grok/patterns/legacy/rails`

 * *Files identical despite different names*

### Comparing `logprep-6.2.0/logprep/util/grok_pattern_loader.py` & `logprep-6.3.0/logprep/util/grok_pattern_loader.py`

 * *Files identical despite different names*

### Comparing `logprep-6.2.0/logprep/util/hasher.py` & `logprep-6.3.0/logprep/util/hasher.py`

 * *Files identical despite different names*

### Comparing `logprep-6.2.0/logprep/util/helper.py` & `logprep-6.3.0/logprep/util/helper.py`

 * *Files identical despite different names*

### Comparing `logprep-6.2.0/logprep/util/json_handling.py` & `logprep-6.3.0/logprep/util/json_handling.py`

 * *Files identical despite different names*

### Comparing `logprep-6.2.0/logprep/util/log_aggregator.py` & `logprep-6.3.0/logprep/util/log_aggregator.py`

 * *Files identical despite different names*

### Comparing `logprep-6.2.0/logprep/util/multiprocessing_log_handler.py` & `logprep-6.3.0/logprep/util/multiprocessing_log_handler.py`

 * *Files identical despite different names*

### Comparing `logprep-6.2.0/logprep/util/pipeline_profiler.py` & `logprep-6.3.0/logprep/util/pipeline_profiler.py`

 * *Files identical despite different names*

### Comparing `logprep-6.2.0/logprep/util/pre_detector_rule_matching_tester.py` & `logprep-6.3.0/logprep/util/pre_detector_rule_matching_tester.py`

 * *Files identical despite different names*

### Comparing `logprep-6.2.0/logprep/util/processor_generator.py` & `logprep-6.3.0/logprep/util/processor_generator.py`

 * *Files identical despite different names*

### Comparing `logprep-6.2.0/logprep/util/prometheus_exporter.py` & `logprep-6.3.0/logprep/util/prometheus_exporter.py`

 * *Files identical despite different names*

### Comparing `logprep-6.2.0/logprep/util/rule_dry_runner.py` & `logprep-6.3.0/logprep/util/rule_dry_runner.py`

 * *Files identical despite different names*

### Comparing `logprep-6.2.0/logprep/util/schema_and_rule_checker.py` & `logprep-6.3.0/logprep/util/schema_and_rule_checker.py`

 * *Files identical despite different names*

### Comparing `logprep-6.2.0/logprep/util/time.py` & `logprep-6.3.0/logprep/util/time.py`

 * *Files identical despite different names*

### Comparing `logprep-6.2.0/logprep/util/time_measurement.py` & `logprep-6.3.0/logprep/util/time_measurement.py`

 * *Files identical despite different names*

### Comparing `logprep-6.2.0/logprep/util/validators.py` & `logprep-6.3.0/logprep/util/validators.py`

 * *Files identical despite different names*

### Comparing `logprep-6.2.0/logprep.egg-info/PKG-INFO` & `logprep-6.3.0/logprep.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: logprep
-Version: 6.2.0
+Version: 6.3.0
 Summary: Logprep allows to collect, process and forward log messages from various data sources.
 Home-page: https://github.com/fkie-cad/Logprep
 Author: Logprep Team
 License: LGPL-2.1 license
 Project-URL: Homepage, https://github.com/fkie-cad/Logprep
 Project-URL: Documentation, https://logprep.readthedocs.io/en/latest/
 Platform: UNKNOWN
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: logprep Version: 6.2.0 Summary: Logprep allows to
+Metadata-Version: 2.1 Name: logprep Version: 6.3.0 Summary: Logprep allows to
 collect, process and forward log messages from various data sources. Home-page:
 https://github.com/fkie-cad/Logprep Author: Logprep Team License: LGPL-2.1
 license Project-URL: Homepage, https://github.com/fkie-cad/Logprep Project-URL:
 Documentation, https://logprep.readthedocs.io/en/latest/ Platform: UNKNOWN
 Classifier: Programming Language :: Python Classifier: Programming Language ::
 Python :: 3 Classifier: Programming Language :: Python :: 3.9 Classifier:
 Programming Language :: Python :: 3.10 Classifier: Programming Language ::
```

### Comparing `logprep-6.2.0/logprep.egg-info/SOURCES.txt` & `logprep-6.3.0/logprep.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `logprep-6.2.0/setup.py` & `logprep-6.3.0/setup.py`

 * *Files identical despite different names*

### Comparing `logprep-6.2.0/tests/acceptance/test_amides.py` & `logprep-6.3.0/tests/acceptance/test_amides.py`

 * *Files identical despite different names*

### Comparing `logprep-6.2.0/tests/acceptance/test_config_refresh.py` & `logprep-6.3.0/tests/acceptance/test_config_refresh.py`

 * *Files identical despite different names*

### Comparing `logprep-6.2.0/tests/acceptance/test_file_input.py` & `logprep-6.3.0/tests/acceptance/test_file_input.py`

 * *Files identical despite different names*

### Comparing `logprep-6.2.0/tests/acceptance/test_full_configuration.py` & `logprep-6.3.0/tests/acceptance/test_full_configuration.py`

 * *Files identical despite different names*

### Comparing `logprep-6.2.0/tests/acceptance/test_http_input.py` & `logprep-6.3.0/tests/acceptance/test_http_input.py`

 * *Files identical despite different names*

### Comparing `logprep-6.2.0/tests/acceptance/test_multiple_outputs.py` & `logprep-6.3.0/tests/acceptance/test_multiple_outputs.py`

 * *Files identical despite different names*

### Comparing `logprep-6.2.0/tests/acceptance/test_pre_detection.py` & `logprep-6.3.0/tests/acceptance/test_pre_detection.py`

 * *Files identical despite different names*

### Comparing `logprep-6.2.0/tests/acceptance/test_preprocessing.py` & `logprep-6.3.0/tests/acceptance/test_preprocessing.py`

 * *Files identical despite different names*

### Comparing `logprep-6.2.0/tests/acceptance/test_selective_extractor_full_pipeline_pass.py` & `logprep-6.3.0/tests/acceptance/test_selective_extractor_full_pipeline_pass.py`

 * *Files identical despite different names*

### Comparing `logprep-6.2.0/tests/acceptance/test_wineventlog_normalization.py` & `logprep-6.3.0/tests/acceptance/test_wineventlog_normalization.py`

 * *Files identical despite different names*

### Comparing `logprep-6.2.0/tests/acceptance/test_wineventlog_processing.py` & `logprep-6.3.0/tests/acceptance/test_wineventlog_processing.py`

 * *Files identical despite different names*

### Comparing `logprep-6.2.0/tests/acceptance/test_wineventlog_pseudonymization.py` & `logprep-6.3.0/tests/acceptance/test_wineventlog_pseudonymization.py`

 * *Files identical despite different names*

### Comparing `logprep-6.2.0/tests/acceptance/util.py` & `logprep-6.3.0/tests/acceptance/util.py`

 * *Files identical despite different names*

### Comparing `logprep-6.2.0/tests/ci/runner-image/scripts/compare_json.py` & `logprep-6.3.0/tests/ci/runner-image/scripts/compare_json.py`

 * *Files identical despite different names*

### Comparing `logprep-6.2.0/tests/testdata/ConfigurationForTest.py` & `logprep-6.3.0/tests/testdata/ConfigurationForTest.py`

 * *Files identical despite different names*

### Comparing `logprep-6.2.0/tests/testdata/FilledTempFile.py` & `logprep-6.3.0/tests/testdata/FilledTempFile.py`

 * *Files identical despite different names*

### Comparing `logprep-6.2.0/tests/testdata/metadata.py` & `logprep-6.3.0/tests/testdata/metadata.py`

 * *Files identical despite different names*

### Comparing `logprep-6.2.0/tests/testdata/ruledata.py` & `logprep-6.3.0/tests/testdata/ruledata.py`

 * *Files identical despite different names*

### Comparing `logprep-6.2.0/tests/testdata/unit/clusterer/test_data.py` & `logprep-6.3.0/tests/testdata/unit/clusterer/test_data.py`

 * *Files identical despite different names*

### Comparing `logprep-6.2.0/tests/unit/component/base.py` & `logprep-6.3.0/tests/unit/component/base.py`

 * *Files identical despite different names*

### Comparing `logprep-6.2.0/tests/unit/connector/base.py` & `logprep-6.3.0/tests/unit/connector/base.py`

 * *Files identical despite different names*

### Comparing `logprep-6.2.0/tests/unit/connector/test_confluent_kafka_common.py` & `logprep-6.3.0/tests/unit/connector/test_confluent_kafka_common.py`

 * *Files identical despite different names*

### Comparing `logprep-6.2.0/tests/unit/connector/test_confluent_kafka_input.py` & `logprep-6.3.0/tests/unit/connector/test_confluent_kafka_input.py`

 * *Files identical despite different names*

### Comparing `logprep-6.2.0/tests/unit/connector/test_confluent_kafka_output.py` & `logprep-6.3.0/tests/unit/connector/test_confluent_kafka_output.py`

 * *Files identical despite different names*

### Comparing `logprep-6.2.0/tests/unit/connector/test_console_output.py` & `logprep-6.3.0/tests/unit/connector/test_console_output.py`

 * *Files identical despite different names*

### Comparing `logprep-6.2.0/tests/unit/connector/test_dummy_input.py` & `logprep-6.3.0/tests/unit/connector/test_dummy_input.py`

 * *Files identical despite different names*

### Comparing `logprep-6.2.0/tests/unit/connector/test_dummy_output.py` & `logprep-6.3.0/tests/unit/connector/test_dummy_output.py`

 * *Files identical despite different names*

### Comparing `logprep-6.2.0/tests/unit/connector/test_elasticsearch_output.py` & `logprep-6.3.0/tests/unit/connector/test_elasticsearch_output.py`

 * *Files identical despite different names*

### Comparing `logprep-6.2.0/tests/unit/connector/test_file_input_default_config.py` & `logprep-6.3.0/tests/unit/connector/test_file_input_default_config.py`

 * *Files identical despite different names*

### Comparing `logprep-6.2.0/tests/unit/connector/test_file_input_not_tailing_config.py` & `logprep-6.3.0/tests/unit/connector/test_file_input_not_tailing_config.py`

 * *Files identical despite different names*

### Comparing `logprep-6.2.0/tests/unit/connector/test_file_input_start_at_end_config.py` & `logprep-6.3.0/tests/unit/connector/test_file_input_start_at_end_config.py`

 * *Files identical despite different names*

### Comparing `logprep-6.2.0/tests/unit/connector/test_http_input.py` & `logprep-6.3.0/tests/unit/connector/test_http_input.py`

 * *Files identical despite different names*

### Comparing `logprep-6.2.0/tests/unit/connector/test_json_input.py` & `logprep-6.3.0/tests/unit/connector/test_json_input.py`

 * *Files identical despite different names*

### Comparing `logprep-6.2.0/tests/unit/connector/test_jsonl_input.py` & `logprep-6.3.0/tests/unit/connector/test_jsonl_input.py`

 * *Files identical despite different names*

### Comparing `logprep-6.2.0/tests/unit/connector/test_jsonl_output.py` & `logprep-6.3.0/tests/unit/connector/test_jsonl_output.py`

 * *Files identical despite different names*

### Comparing `logprep-6.2.0/tests/unit/connector/test_opensearch_output.py` & `logprep-6.3.0/tests/unit/connector/test_opensearch_output.py`

 * *Files identical despite different names*

### Comparing `logprep-6.2.0/tests/unit/connector/test_s3_output.py` & `logprep-6.3.0/tests/unit/connector/test_s3_output.py`

 * *Files identical despite different names*

### Comparing `logprep-6.2.0/tests/unit/exceptions/processor/test_processing_warning.py` & `logprep-6.3.0/tests/unit/exceptions/processor/test_processing_warning.py`

 * *Files identical despite different names*

### Comparing `logprep-6.2.0/tests/unit/filter/test_filter_expression.py` & `logprep-6.3.0/tests/unit/filter/test_filter_expression.py`

 * *Files identical despite different names*

### Comparing `logprep-6.2.0/tests/unit/filter/test_lucene_filter.py` & `logprep-6.3.0/tests/unit/filter/test_lucene_filter.py`

 * *Files identical despite different names*

### Comparing `logprep-6.2.0/tests/unit/framework/rule_tree/test_node.py` & `logprep-6.3.0/tests/unit/framework/rule_tree/test_node.py`

 * *Files identical despite different names*

### Comparing `logprep-6.2.0/tests/unit/framework/rule_tree/test_rule_parser.py` & `logprep-6.3.0/tests/unit/framework/rule_tree/test_rule_parser.py`

 * *Files identical despite different names*

### Comparing `logprep-6.2.0/tests/unit/framework/rule_tree/test_rule_tree.py` & `logprep-6.3.0/tests/unit/framework/rule_tree/test_rule_tree.py`

 * *Files identical despite different names*

### Comparing `logprep-6.2.0/tests/unit/framework/test_pipeline.py` & `logprep-6.3.0/tests/unit/framework/test_pipeline.py`

 * *Files identical despite different names*

### Comparing `logprep-6.2.0/tests/unit/framework/test_pipeline_manager.py` & `logprep-6.3.0/tests/unit/framework/test_pipeline_manager.py`

 * *Files identical despite different names*

### Comparing `logprep-6.2.0/tests/unit/metrics/test_metric_exposer.py` & `logprep-6.3.0/tests/unit/metrics/test_metric_exposer.py`

 * *Files identical despite different names*

### Comparing `logprep-6.2.0/tests/unit/metrics/test_metric_targets.py` & `logprep-6.3.0/tests/unit/metrics/test_metric_targets.py`

 * *Files identical despite different names*

### Comparing `logprep-6.2.0/tests/unit/metrics/test_metrics.py` & `logprep-6.3.0/tests/unit/metrics/test_metrics.py`

 * *Files identical despite different names*

### Comparing `logprep-6.2.0/tests/unit/processor/amides/test_amides.py` & `logprep-6.3.0/tests/unit/processor/amides/test_amides.py`

 * *Files identical despite different names*

### Comparing `logprep-6.2.0/tests/unit/processor/amides/test_amides_rule.py` & `logprep-6.3.0/tests/unit/processor/amides/test_amides_rule.py`

 * *Files identical despite different names*

### Comparing `logprep-6.2.0/tests/unit/processor/amides/test_detection.py` & `logprep-6.3.0/tests/unit/processor/amides/test_detection.py`

 * *Files identical despite different names*

### Comparing `logprep-6.2.0/tests/unit/processor/amides/test_normalize.py` & `logprep-6.3.0/tests/unit/processor/amides/test_normalize.py`

 * *Files identical despite different names*

### Comparing `logprep-6.2.0/tests/unit/processor/amides/test_tokenizer.py` & `logprep-6.3.0/tests/unit/processor/amides/test_tokenizer.py`

 * *Files identical despite different names*

### Comparing `logprep-6.2.0/tests/unit/processor/base.py` & `logprep-6.3.0/tests/unit/processor/base.py`

 * *Files identical despite different names*

### Comparing `logprep-6.2.0/tests/unit/processor/calculator/test_calculator.py` & `logprep-6.3.0/tests/unit/processor/calculator/test_calculator.py`

 * *Files identical despite different names*

### Comparing `logprep-6.2.0/tests/unit/processor/calculator/test_calculator_rule.py` & `logprep-6.3.0/tests/unit/processor/calculator/test_calculator_rule.py`

 * *Files identical despite different names*

### Comparing `logprep-6.2.0/tests/unit/processor/clusterer/test_clusterer.py` & `logprep-6.3.0/tests/unit/processor/clusterer/test_clusterer.py`

 * *Files identical despite different names*

### Comparing `logprep-6.2.0/tests/unit/processor/clusterer/test_clusterer_rule.py` & `logprep-6.3.0/tests/unit/processor/clusterer/test_clusterer_rule.py`

 * *Files identical despite different names*

### Comparing `logprep-6.2.0/tests/unit/processor/clusterer/test_clusterer_signature_phase.py` & `logprep-6.3.0/tests/unit/processor/clusterer/test_clusterer_signature_phase.py`

 * *Files identical despite different names*

### Comparing `logprep-6.2.0/tests/unit/processor/concatenator/test_concatenator.py` & `logprep-6.3.0/tests/unit/processor/concatenator/test_concatenator.py`

 * *Files identical despite different names*

### Comparing `logprep-6.2.0/tests/unit/processor/concatenator/test_concatenator_rule.py` & `logprep-6.3.0/tests/unit/processor/concatenator/test_concatenator_rule.py`

 * *Files identical despite different names*

### Comparing `logprep-6.2.0/tests/unit/processor/datetime_extractor/test_datetime_extractor.py` & `logprep-6.3.0/tests/unit/processor/datetime_extractor/test_datetime_extractor.py`

 * *Files identical despite different names*

### Comparing `logprep-6.2.0/tests/unit/processor/datetime_extractor/test_datetime_extractor_rule.py` & `logprep-6.3.0/tests/unit/processor/datetime_extractor/test_datetime_extractor_rule.py`

 * *Files identical despite different names*

### Comparing `logprep-6.2.0/tests/unit/processor/deleter/test_deleter.py` & `logprep-6.3.0/tests/unit/processor/deleter/test_deleter.py`

 * *Files identical despite different names*

### Comparing `logprep-6.2.0/tests/unit/processor/deleter/test_deleter_rule.py` & `logprep-6.3.0/tests/unit/processor/deleter/test_deleter_rule.py`

 * *Files identical despite different names*

### Comparing `logprep-6.2.0/tests/unit/processor/dissector/test_dissector.py` & `logprep-6.3.0/tests/unit/processor/dissector/test_dissector.py`

 * *Files 9% similar despite different names*

```diff
@@ -391,22 +391,22 @@
             "field4": "+ message",
         },
     ),
     (
         "handles special chars in captured content and target field names",
         {
             "filter": "message",
-            "dissector": {"mapping": {"message": "%{~field1} %{fie ld2} %{-fie}ld3} %{+field4}"}},
+            "dissector": {"mapping": {"message": "%{~field1} %{fie ld2} %{$fie}ld3} %{+field4}"}},
         },
         {"message": "&This is\2 a mess}age /1"},
         {
             "message": "&This is\2 a mess}age /1",
             "~field1": "&This",
             "fie ld2": "is\2",
-            "-fie}ld3": "a",
+            "$fie}ld3": "a",
             "field4": "mess}age /1",
         },
     ),
     (
         "deletes source fields",
         {
             "filter": "message",
@@ -474,15 +474,15 @@
         },
         {
             "message": "INFO#2022 12 06 15:12:30:534#+0100#MOREINFO",
             "date": "(2022 12 06 15:12:30:534)+0100",
         },
     ),
     (
-        "Dissection with delimeter ending",
+        "Dissection with delimiter ending",
         {"filter": "message", "dissector": {"mapping": {"message": "this is %{target}."}}},
         {"message": "this is the message."},
         {"message": "this is the message.", "target": "the message"},
     ),
     (
         "Convert datatype via dissect pattern",
         {
@@ -490,14 +490,116 @@
             "dissector": {
                 "mapping": {"message": "this is %{field1|int} message and this is %{field2|bool}"}
             },
         },
         {"message": "this is 42 message and this is 0"},
         {"message": "this is 42 message and this is 0", "field1": 42, "field2": False},
     ),
+    (
+        "Strip char after dissecting",
+        {
+            "filter": "message",
+            "dissector": {"mapping": {"message": "[%{time-( )}] - %{ip}"}},
+        },
+        {"message": "[2022-11-04 10:00:00 AM     ] - 127.0.0.1"},
+        {
+            "message": "[2022-11-04 10:00:00 AM     ] - 127.0.0.1",
+            "time": "2022-11-04 10:00:00 AM",
+            "ip": "127.0.0.1",
+        },
+    ),
+    (
+        "Strip special char after dissecting",
+        {
+            "filter": "message",
+            "dissector": {"mapping": {"message": "[%{time-(#)}] - %{ip}"}},
+        },
+        {"message": "[2022-11-04 10:00:00 AM####] - 127.0.0.1"},
+        {
+            "message": "[2022-11-04 10:00:00 AM####] - 127.0.0.1",
+            "time": "2022-11-04 10:00:00 AM",
+            "ip": "127.0.0.1",
+        },
+    ),
+    (
+        "Strip another special char after dissecting",
+        {
+            "filter": "message",
+            "dissector": {"mapping": {"message": "[%{time-(?)}] - %{ip}"}},
+        },
+        {"message": "[2022-11-04 10:00:00 AM?????] - 127.0.0.1"},
+        {
+            "message": "[2022-11-04 10:00:00 AM?????] - 127.0.0.1",
+            "time": "2022-11-04 10:00:00 AM",
+            "ip": "127.0.0.1",
+        },
+    ),
+    (
+        "Strip char on both sides",
+        {
+            "filter": "message",
+            "dissector": {"mapping": {"message": "[%{time-(*)}] - %{ip}"}},
+        },
+        {"message": "[***2022-11-04 10:00:00 AM***] - 127.0.0.1"},
+        {
+            "message": "[***2022-11-04 10:00:00 AM***] - 127.0.0.1",
+            "time": "2022-11-04 10:00:00 AM",
+            "ip": "127.0.0.1",
+        },
+    ),
+    (
+        "Strip char while appending",
+        {
+            "filter": "message",
+            "dissector": {"mapping": {"message": "[%{time} %{+( )time} %{+( )time-(*)}] - %{ip}"}},
+        },
+        {"message": "[2022-11-04 10:00:00 AM***] - 127.0.0.1"},
+        {
+            "message": "[2022-11-04 10:00:00 AM***] - 127.0.0.1",
+            "time": "2022-11-04 10:00:00 AM",
+            "ip": "127.0.0.1",
+        },
+    ),
+    (
+        "Strip char while changing position",
+        {
+            "filter": "message",
+            "dissector": {
+                "mapping": {"message": "[%{time/1} %{+( )time/3} %{+( )time-(*)/2}] - %{ip}"}
+            },
+        },
+        {"message": "[2022-11-04 10:00:00 AM***] - 127.0.0.1"},
+        {
+            "message": "[2022-11-04 10:00:00 AM***] - 127.0.0.1",
+            "time": "2022-11-04 AM 10:00:00",
+            "ip": "127.0.0.1",
+        },
+    ),
+    (
+        "Strip char in indirect field notation",
+        {
+            "filter": "message",
+            "dissector": {"mapping": {"message": "%{?key} %{&key-(#)} %{} %{+( )&key-(#)}"}},
+        },
+        {"message": "This is## the message####"},
+        {"message": "This is## the message####", "This": "is message"},
+    ),
+    (
+        "Strip char while inferring datatype",
+        {
+            "filter": "message",
+            "dissector": {
+                "mapping": {
+                    "message": "this is %{field1-(#)|int} message and this is %{field2-(#)|bool}"
+                }
+            },
+        },
+        {"message": "this is 42#### message and this is 0##"},
+        {"message": "this is 42#### message and this is 0##", "field1": 42, "field2": False},
+    ),
 ]
 failure_test_cases = [  # testcase, rule, event, expected
     (
         "Tags failure if convert is not possible",
         {
             "filter": "message",
             "dissector": {
```

### Comparing `logprep-6.2.0/tests/unit/processor/dissector/test_dissector_rule.py` & `logprep-6.3.0/tests/unit/processor/dissector/test_dissector_rule.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 # pylint: disable=missing-docstring
 # pylint: disable=protected-access
 # pylint: disable=anomalous-backslash-in-string
+# pylint: disable=line-too-long
 import pytest
 
 from logprep.processor.base.exceptions import InvalidRuleDefinitionError
 from logprep.processor.dissector.rule import DissectorRule, add_and_overwrite, append, str_to_bool
 
 
 class TestDissectorRule:
@@ -326,141 +327,155 @@
         rule = {
             "filter": "message",
             "dissector": {
                 "mapping": {"field1": "%{field2}:%{field3} %{field4}"},
                 "tag_on_failure": ["_failed"],
             },
         }
-        dissector_rule = DissectorRule._create_from_dict(rule)
-        assert dissector_rule.actions
-        assert dissector_rule.actions[0] == ("field1", ":", "field2", add_and_overwrite, "", 0)
-        assert dissector_rule.actions[1] == ("field1", " ", "field3", add_and_overwrite, "", 0)
-        assert dissector_rule.actions[2] == ("field1", None, "field4", add_and_overwrite, "", 0)
+        rule = DissectorRule._create_from_dict(rule)
+        assert rule.actions
+        assert rule.actions[0] == ("field1", ":", "field2", add_and_overwrite, "", None, 0)
+        assert rule.actions[1] == ("field1", " ", "field3", add_and_overwrite, "", None, 0)
+        assert rule.actions[2] == ("field1", None, "field4", add_and_overwrite, "", None, 0)
 
     def test_converts_mappings_with_append_operator_to_append_field_to_action(self):
         rule = {
             "filter": "message",
             "dissector": {
                 "mapping": {"field1": "%{field2}:%{+field3} %{field4}"},
                 "tag_on_failure": ["_failed"],
             },
         }
-        dissector_rule = DissectorRule._create_from_dict(rule)
-        assert dissector_rule.actions
-        assert dissector_rule.actions[0] == ("field1", ":", "field2", add_and_overwrite, "", 0)
-        assert dissector_rule.actions[1] == ("field1", " ", "field3", append, "", 0)
-        assert dissector_rule.actions[2] == ("field1", None, "field4", add_and_overwrite, "", 0)
+        rule = DissectorRule._create_from_dict(rule)
+        assert rule.actions
+        assert rule.actions[0] == ("field1", ":", "field2", add_and_overwrite, "", None, 0)
+        assert rule.actions[1] == ("field1", " ", "field3", append, "", None, 0)
+        assert rule.actions[2] == ("field1", None, "field4", add_and_overwrite, "", None, 0)
 
     def test_converts_mappings_with_append_operator_and_order_modifier(self):
         rule = {
             "filter": "message",
             "dissector": {
                 "mapping": {"field1": "%{field2}:%{+field3/1} %{+field4/3}"},
                 "tag_on_failure": ["_failed"],
             },
         }
-        dissector_rule = DissectorRule._create_from_dict(rule)
-        assert dissector_rule.actions
-        assert dissector_rule.actions[0] == ("field1", ":", "field2", add_and_overwrite, "", 0)
-        assert dissector_rule.actions[1] == ("field1", " ", "field3", append, "", 1)
-        assert dissector_rule.actions[2] == ("field1", None, "field4", append, "", 3)
+        rule = DissectorRule._create_from_dict(rule)
+        assert rule.actions
+        assert rule.actions[0] == ("field1", ":", "field2", add_and_overwrite, "", None, 0)
+        assert rule.actions[1] == ("field1", " ", "field3", append, "", None, 1)
+        assert rule.actions[2] == ("field1", None, "field4", append, "", None, 3)
 
     def test_adds_convert_actions(self):
         rule = {"filter": "message", "dissector": {"convert_datatype": {"field1": "int"}}}
-        dissector_rule = DissectorRule._create_from_dict(rule)
-        assert dissector_rule.convert_actions
-        assert dissector_rule.convert_actions[0][0] == "field1"
-        assert dissector_rule.convert_actions[0][1] == int
+        rule = DissectorRule._create_from_dict(rule)
+        assert rule.convert_actions
+        assert rule.convert_actions[0][0] == "field1"
+        assert rule.convert_actions[0][1] == int
 
     def test_adds_multiple_convert_actions(self):
         rule = {
             "filter": "message",
             "dissector": {
                 "convert_datatype": {
                     "field1": "int",
                     "other_field": "string",
                     "yet another field": "float",
                 }
             },
         }
-        dissector_rule = DissectorRule._create_from_dict(rule)
-        assert dissector_rule.convert_actions
-        assert dissector_rule.convert_actions[0][0] == "field1"
-        assert dissector_rule.convert_actions[0][1] == int
-        assert dissector_rule.convert_actions[1][0] == "other_field"
-        assert dissector_rule.convert_actions[1][1] == str
-        assert dissector_rule.convert_actions[2][0] == "yet another field"
-        assert dissector_rule.convert_actions[2][1] == float
+        rule = DissectorRule._create_from_dict(rule)
+        assert rule.convert_actions
+        assert rule.convert_actions[0][0] == "field1"
+        assert rule.convert_actions[0][1] == int
+        assert rule.convert_actions[1][0] == "other_field"
+        assert rule.convert_actions[1][1] == str
+        assert rule.convert_actions[2][0] == "yet another field"
+        assert rule.convert_actions[2][1] == float
 
     def test_parses_defined_separator(self):
         rule = {
             "filter": "message",
             "dissector": {
                 "mapping": {"field1": "%{field2}:%{+( )field3/1} %{+(,)field4/3}"},
                 "tag_on_failure": ["_failed"],
             },
         }
-        dissector_rule = DissectorRule._create_from_dict(rule)
-        assert dissector_rule.actions
-        assert dissector_rule.actions[0] == ("field1", ":", "field2", add_and_overwrite, "", 0)
-        assert dissector_rule.actions[1] == ("field1", " ", "field3", append, " ", 1)
-        assert dissector_rule.actions[2] == ("field1", None, "field4", append, ",", 3)
+        rule = DissectorRule._create_from_dict(rule)
+        assert rule.actions
+        assert rule.actions[0] == ("field1", ":", "field2", add_and_overwrite, "", None, 0)
+        assert rule.actions[1] == ("field1", " ", "field3", append, " ", None, 1)
+        assert rule.actions[2] == ("field1", None, "field4", append, ",", None, 3)
 
     def test_parses_defined_multichar_separator(self):
         rule = {
             "filter": "message",
             "dissector": {
                 "mapping": {"field1": "%{field2}:%{+(separator)field3/1} %{+(,)field4/3}"},
                 "tag_on_failure": ["_failed"],
             },
         }
-        dissector_rule = DissectorRule._create_from_dict(rule)
-        assert dissector_rule.actions
-        assert dissector_rule.actions[0] == ("field1", ":", "field2", add_and_overwrite, "", 0)
-        assert dissector_rule.actions[1] == ("field1", " ", "field3", append, "separator", 1)
-        assert dissector_rule.actions[2] == ("field1", None, "field4", append, ",", 3)
+        rule = DissectorRule._create_from_dict(rule)
+        assert rule.actions
+        assert rule.actions[0] == ("field1", ":", "field2", add_and_overwrite, "", None, 0)
+        assert rule.actions[1] == ("field1", " ", "field3", append, "separator", None, 1)
+        assert rule.actions[2] == ("field1", None, "field4", append, ",", None, 3)
 
     def test_parses_defined_special_chars_separator(self):
         rule = {
             "filter": "message",
             "dissector": {
                 "mapping": {"field1": "%{field2}:%{+(\()field3/1} %{+(\))field4/3}"},
                 "tag_on_failure": ["_failed"],
             },
         }
-        dissector_rule = DissectorRule._create_from_dict(rule)
-        assert dissector_rule.actions
-        assert dissector_rule.actions[0] == ("field1", ":", "field2", add_and_overwrite, "", 0)
-        assert dissector_rule.actions[1] == ("field1", " ", "field3", append, "(", 1)
-        assert dissector_rule.actions[2] == ("field1", None, "field4", append, ")", 3)
+        rule = DissectorRule._create_from_dict(rule)
+        assert rule.actions
+        assert rule.actions[0] == ("field1", ":", "field2", add_and_overwrite, "", None, 0)
+        assert rule.actions[1] == ("field1", " ", "field3", append, "(", None, 1)
+        assert rule.actions[2] == ("field1", None, "field4", append, ")", None, 3)
 
     def test_parses_defined_very_special_chars_separator(self):
         rule = {
             "filter": "message",
             "dissector": {
                 "mapping": {"field1": "%{field2}:%{+(#)field3/1} %{+(})field4/3}"},
                 "tag_on_failure": ["_failed"],
             },
         }
-        dissector_rule = DissectorRule._create_from_dict(rule)
-        assert dissector_rule.actions
-        assert dissector_rule.actions[0] == ("field1", ":", "field2", add_and_overwrite, "", 0)
-        assert dissector_rule.actions[1] == ("field1", " ", "field3", append, "#", 1)
-        assert dissector_rule.actions[2] == ("field1", None, "field4", append, "}", 3)
+        rule = DissectorRule._create_from_dict(rule)
+        assert rule.actions
+        assert rule.actions[0] == ("field1", ":", "field2", add_and_overwrite, "", None, 0)
+        assert rule.actions[1] == ("field1", " ", "field3", append, "#", None, 1)
+        assert rule.actions[2] == ("field1", None, "field4", append, "}", None, 3)
+
+    def test_parses_strip_char(self):
+        rule = {
+            "filter": "message",
+            "dissector": {
+                "mapping": {"field1": "%{field2}:%{field3} %{field4-( )}"},
+                "tag_on_failure": ["_failed"],
+            },
+        }
+        rule = DissectorRule._create_from_dict(rule)
+        assert rule.actions
+        assert rule.actions[0] == ("field1", ":", "field2", add_and_overwrite, "", None, 0)
+        assert rule.actions[1] == ("field1", " ", "field3", add_and_overwrite, "", None, 0)
+        assert rule.actions[2] == ("field1", None, "field4", add_and_overwrite, "", " ", 0)
 
     def test_parses_datatype_conversion_from_dissect_pattern(self):
         rule = {
             "filter": "message",
             "dissector": {
                 "mapping": {"field1": "%{field2}:%{field3|int} %{field4}"},
             },
         }
-        dissector_rule = DissectorRule._create_from_dict(rule)
-        assert dissector_rule._config.convert_datatype.get("field3") == "int"
-        assert len(dissector_rule._config.convert_datatype.keys()) == 1
+        rule = DissectorRule._create_from_dict(rule)
+        assert rule._config.convert_datatype.get("field3") == "int"
+        assert len(rule._config.convert_datatype.keys()) == 1
 
     @pytest.mark.parametrize(
         "input_str, expected",
         [("yes", True), ("no", False), (None, False), ("42", True), ("on", True), ("off", False)],
     )
     def test_str_to_bool_returns(self, input_str, expected):
         assert str_to_bool(input_str) == expected
```

### Comparing `logprep-6.2.0/tests/unit/processor/domain_label_extractor/test_domain_label_extractor.py` & `logprep-6.3.0/tests/unit/processor/domain_label_extractor/test_domain_label_extractor.py`

 * *Files identical despite different names*

### Comparing `logprep-6.2.0/tests/unit/processor/domain_label_extractor/test_domain_label_extractor_rule.py` & `logprep-6.3.0/tests/unit/processor/domain_label_extractor/test_domain_label_extractor_rule.py`

 * *Files identical despite different names*

### Comparing `logprep-6.2.0/tests/unit/processor/domain_resolver/test_domain_resolver.py` & `logprep-6.3.0/tests/unit/processor/domain_resolver/test_domain_resolver.py`

 * *Files identical despite different names*

### Comparing `logprep-6.2.0/tests/unit/processor/domain_resolver/test_domain_resolver_rule.py` & `logprep-6.3.0/tests/unit/processor/domain_resolver/test_domain_resolver_rule.py`

 * *Files identical despite different names*

### Comparing `logprep-6.2.0/tests/unit/processor/dropper/test_dropper.py` & `logprep-6.3.0/tests/unit/processor/dropper/test_dropper.py`

 * *Files identical despite different names*

### Comparing `logprep-6.2.0/tests/unit/processor/dropper/test_dropper_rule.py` & `logprep-6.3.0/tests/unit/processor/dropper/test_dropper_rule.py`

 * *Files identical despite different names*

### Comparing `logprep-6.2.0/tests/unit/processor/field_manager/test_field_manager.py` & `logprep-6.3.0/tests/unit/processor/field_manager/test_field_manager.py`

 * *Files 26% similar despite different names*

```diff
@@ -278,54 +278,204 @@
                     "223.2.3.2",
                     "8.8.8.8",
                     "fe89::",
                 ]
             },
         },
     ),
+    (
+        "copies multiple fields to multiple target fields",
+        {
+            "filter": "field",
+            "field_manager": {
+                "mapping": {"field.one": "one", "field.two": "two", "field.three": "three"},
+            },
+        },
+        {"field": {"one": 1, "two": 2, "three": 3}},
+        {"field": {"one": 1, "two": 2, "three": 3}, "one": 1, "two": 2, "three": 3},
+    ),
+    (
+        "copies multiple fields to multiple target fields, while overwriting existing fields",
+        {
+            "filter": "field",
+            "field_manager": {
+                "mapping": {"field.one": "one", "field.two": "two", "field.three": "three"},
+                "overwrite_target": True,
+            },
+        },
+        {"field": {"one": 1, "two": 2, "three": 3}, "three": "exists already"},
+        {"field": {"one": 1, "two": 2, "three": 3}, "one": 1, "two": 2, "three": 3},
+    ),
+    (
+        "copies multiple fields to multiple target fields, while one list will be extended",
+        {
+            "filter": "field",
+            "field_manager": {
+                "mapping": {"field.one": "one", "field.two": "two", "field.three": "three"},
+                "extend_target_list": True,
+            },
+        },
+        {"field": {"one": 1, "two": 2, "three": 3}, "three": ["exists already"]},
+        {
+            "field": {"one": 1, "two": 2, "three": 3},
+            "one": 1,
+            "two": 2,
+            "three": ["exists already", 3],
+        },
+    ),
+    (
+        "copies multiple fields to multiple target fields, while one list will be extended with existing list",
+        {
+            "filter": "field",
+            "field_manager": {
+                "mapping": {"field.one": "one", "field.two": "two", "field.three": "three"},
+                "extend_target_list": True,
+            },
+        },
+        {"field": {"one": 1, "two": 2, "three": [3, 3]}, "three": ["exists already"]},
+        {
+            "field": {"one": 1, "two": 2, "three": [3, 3]},
+            "one": 1,
+            "two": 2,
+            "three": ["exists already", 3, 3],
+        },
+    ),
+    (
+        "copies multiple fields to multiple target fields, while one target list will be overwritten with existing list",
+        {
+            "filter": "field",
+            "field_manager": {
+                "mapping": {"field.one": "one", "field.two": "two", "field.three": "three"},
+                "overwrite_target": True,
+            },
+        },
+        {"field": {"one": 1, "two": 2, "three": [3, 3]}, "three": ["exists already"]},
+        {"field": {"one": 1, "two": 2, "three": [3, 3]}, "one": 1, "two": 2, "three": [3, 3]},
+    ),
+    (
+        "copies multiple fields to multiple target fields, while one source field is missing",
+        {
+            "filter": "field",
+            "field_manager": {
+                "mapping": {"field.one": "one", "field.two": "two", "field.three": "three"},
+            },
+        },
+        {
+            "field": {"one": 1, "three": 3},
+        },
+        {
+            "field": {"one": 1, "three": 3},
+            "one": 1,
+            "three": 3,
+            "tags": ["_field_manager_missing_field_warning"],
+        },
+    ),
+    (
+        "moves multiple fields to multiple target fields",
+        {
+            "filter": "field",
+            "field_manager": {
+                "mapping": {"field.one": "one", "field.two": "two", "field.three": "three"},
+                "delete_source_fields": True,
+            },
+        },
+        {"field": {"one": 1, "two": 2, "three": 3}},
+        {"one": 1, "two": 2, "three": 3},
+    ),
+    (
+        "Combine fields to list and copy fields at the same time",
+        {
+            "filter": "field",
+            "field_manager": {
+                "source_fields": ["source.one", "source.two"],
+                "target_field": "merged",
+                "mapping": {"field.one": "one", "field.two": "two", "field.three": "three"},
+                "extend_target_list": True,
+            },
+        },
+        {"field": {"one": 1, "two": 2, "three": 3}, "source": {"one": ["a"], "two": ["b"]}},
+        {
+            "field": {"one": 1, "two": 2, "three": 3},
+            "source": {"one": ["a"], "two": ["b"]},
+            "one": 1,
+            "two": 2,
+            "three": 3,
+            "merged": ["a", "b"],
+        },
+    ),
 ]
 
 failure_test_cases = [
     (
         "single source field not found",
         {
             "filter": "message",
             "field_manager": {
                 "source_fields": ["do.not.exits"],
                 "target_field": "new_field",
             },
         },
         {"message": "This is a message"},
-        {"message": "This is a message", "tags": ["_field_manager_failure"]},
+        {"message": "This is a message", "tags": ["_field_manager_missing_field_warning"]},
+        ".*ProcessingWarning.*",
     ),
     (
         "single source field not found and preexisting tags",
         {
             "filter": "message",
             "field_manager": {
                 "source_fields": ["do.not.exits"],
                 "target_field": "new_field",
             },
         },
         {"message": "This is a message", "tags": ["preexisting"]},
-        {"message": "This is a message", "tags": ["_field_manager_failure", "preexisting"]},
+        {
+            "message": "This is a message",
+            "tags": ["_field_manager_missing_field_warning", "preexisting"],
+        },
+        ".*ProcessingWarning.*",
     ),
     (
         "single source field not found and preexisting tags with deduplication",
         {
             "filter": "message",
             "field_manager": {
                 "source_fields": ["do.not.exits"],
                 "target_field": "new_field",
             },
         },
-        {"message": "This is a message", "tags": ["_field_manager_failure", "preexisting"]},
-        {"message": "This is a message", "tags": ["_field_manager_failure", "preexisting"]},
+        {
+            "message": "This is a message",
+            "tags": ["_field_manager_missing_field_warning", "preexisting"],
+        },
+        {
+            "message": "This is a message",
+            "tags": ["_field_manager_missing_field_warning", "preexisting"],
+        },
+        ".*ProcessingWarning.*",
+    ),
+    (
+        "copies multiple fields to multiple target fields, while one target exists already",
+        {
+            "filter": "field",
+            "field_manager": {
+                "mapping": {"field.one": "one", "field.two": "two", "field.three": "three"},
+            },
+        },
+        {"field": {"one": 1, "two": 2, "three": 3}, "three": "exists"},
+        {
+            "field": {"one": 1, "two": 2, "three": 3},
+            "one": 1,
+            "two": 2,
+            "three": "exists",
+            "tags": ["_field_manager_failure"],
+        },
+        ".*FieldExistsWarning.*",
     ),
-]  # testcase, rule, event, expected
+]  # testcase, rule, event, expected, error
 
 
 class TestFieldManager(BaseProcessorTestCase):
     CONFIG: dict = {
         "type": "field_manager",
         "specific_rules": ["tests/testdata/unit/field_manager/specific_rules"],
         "generic_rules": ["tests/testdata/unit/field_manager/generic_rules"],
@@ -333,20 +483,20 @@
 
     @pytest.mark.parametrize("testcase, rule, event, expected", test_cases)
     def test_testcases(self, testcase, rule, event, expected):  # pylint: disable=unused-argument
         self._load_specific_rule(rule)
         self.object.process(event)
         assert event == expected
 
-    @pytest.mark.parametrize("testcase, rule, event, expected", failure_test_cases)
-    def test_testcases_failure_handling(self, testcase, rule, event, expected, caplog):
+    @pytest.mark.parametrize("testcase, rule, event, expected, error", failure_test_cases)
+    def test_testcases_failure_handling(self, testcase, rule, event, expected, error, caplog):
         self._load_specific_rule(rule)
         with caplog.at_level(logging.WARNING):
             self.object.process(event)
-        assert re.match(".*ProcessingWarning.*", caplog.text)
+        assert re.match(error, caplog.text)
         assert event == expected, testcase
 
     def test_process_raises_duplication_error_if_target_field_exists_and_should_not_be_overwritten(
         self, caplog
     ):
         rule = {
             "filter": "field.a",
```

### Comparing `logprep-6.2.0/tests/unit/processor/field_manager/test_field_manager_rule.py` & `logprep-6.3.0/tests/unit/processor/field_manager/test_field_manager_rule.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 # pylint: disable=protected-access
 # pylint: disable=missing-docstring
 import pytest
+
 from logprep.processor.base.exceptions import InvalidRuleDefinitionError
 from logprep.processor.field_manager.rule import FieldManagerRule
 
 
 class TestFieldManagerRule:
     def test_create_from_dict_returns_field_manager_rule(self):
         rule = {
@@ -40,18 +41,18 @@
                 },
                 TypeError,
                 "unexpected keyword argument 'source_field'",
             ),
             (
                 {
                     "filter": "message",
-                    "field_manager": {"source_fields": ["message"], "target_fields": ["new_field"]},
+                    "field_manager": {"source_fields": ["message"], "unknown": ["new_field"]},
                 },
                 TypeError,
-                "unexpected keyword argument 'target_fields'",
+                "unexpected keyword argument 'unknown'",
             ),
             (
                 {
                     "filter": "message",
                     "field_manager": {
                         "source_fields": ["message"],
                         "target_field": "new_field",
@@ -69,14 +70,24 @@
                         "target_field": "new_field",
                         "delte_source_field": True,
                     },
                 },
                 TypeError,
                 "got an unexpected keyword argument 'delte_source_field'",
             ),
+            (
+                {
+                    "filter": "message",
+                    "field_manager": {
+                        "mapping": {"field.one": "one", "field.two": "two"},
+                    },
+                },
+                None,
+                None,
+            ),
         ],
     )
     def test_create_from_dict_validates_config(self, rule, error, message):
         if error:
             with pytest.raises(error, match=message):
                 FieldManagerRule._create_from_dict(rule)
         else:
```

### Comparing `logprep-6.2.0/tests/unit/processor/generic_adder/test_generic_adder.py` & `logprep-6.3.0/tests/unit/processor/generic_adder/test_generic_adder.py`

 * *Files identical despite different names*

### Comparing `logprep-6.2.0/tests/unit/processor/generic_adder/test_generic_adder_rule.py` & `logprep-6.3.0/tests/unit/processor/generic_adder/test_generic_adder_rule.py`

 * *Files identical despite different names*

### Comparing `logprep-6.2.0/tests/unit/processor/generic_resolver/test_generic_resolver.py` & `logprep-6.3.0/tests/unit/processor/generic_resolver/test_generic_resolver.py`

 * *Files identical despite different names*

### Comparing `logprep-6.2.0/tests/unit/processor/generic_resolver/test_generic_resolver_rule.py` & `logprep-6.3.0/tests/unit/processor/generic_resolver/test_generic_resolver_rule.py`

 * *Files identical despite different names*

### Comparing `logprep-6.2.0/tests/unit/processor/geoip_enricher/test_geoip_enricher.py` & `logprep-6.3.0/tests/unit/processor/geoip_enricher/test_geoip_enricher.py`

 * *Files identical despite different names*

### Comparing `logprep-6.2.0/tests/unit/processor/geoip_enricher/test_geoip_enricher_rule.py` & `logprep-6.3.0/tests/unit/processor/geoip_enricher/test_geoip_enricher_rule.py`

 * *Files identical despite different names*

### Comparing `logprep-6.2.0/tests/unit/processor/grokker/test_grok.py` & `logprep-6.3.0/tests/unit/processor/grokker/test_grok.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,41 +35,41 @@
 
 
 def test_one_pat_4():
     text = "github.com"
     pat = "%{HOSTNAME:website}"
     grok = Grok(pat)
     match = grok.match(text)
-    assert match["website"] == text.strip(), f"grok match failed:{text}, {pat}"
+    assert match["website"] == text.strip(), f"grok match failed: {text}, {pat}"
 
 
 def test_one_pat_5():
     text = "1989-11-04 05:33:02+0800"
     pat = "%{TIMESTAMP_ISO8601:ts}"
     grok = Grok(pat)
     match = grok.match(text)
-    assert match["ts"] == text.strip(), f"grok match failed:{text}, {pat}"
+    assert match["ts"] == text.strip(), f"grok match failed: {text}, {pat}"
 
 
 def test_one_pat_6():
     text = "github"
     pat = "%{WORD}"
     grok = Grok(pat)
     match = grok.match(text)
-    assert match == {}, f"grok match failed:{text}, {pat}"
+    assert match == {}, f"grok match failed: {text}, {pat}"
     # you get nothing because variable name is not set,
     # compare "%{WORD}" and "%{WORD:variable_name}"
 
 
 def test_one_pat_7():
     text = "github"
     pat = "%{NUMBER:test_num}"
     grok = Grok(pat)
     match = grok.match(text)
-    assert match is None, f"grok match failed:{text}, {pat}"
+    assert match == {}, f"grok match failed: {text}, {pat}"
     # not match
 
 
 def test_one_pat_8():
     text = "1989"
     pat = "%{NUMBER:birthyear:int}"
     grok = Grok(pat)
@@ -94,15 +94,15 @@
     assert match == {}, f"grok match failed:{text}, {pat}"
 
     # "male" is not INT
     text = 'gary male "never quit"'
     pat = "%{WORD:name} %{INT:age} %{QUOTEDSTRING:motto}"
     grok = Grok(pat)
     match = grok.match(text)
-    assert match is None, f"grok match failed:{text}, {pat}"
+    assert match == {}, f"grok match failed:{text}, {pat}"
 
     # nginx log
     text = (
         "edge.v.iask.com.edge.sinastorage.com 14.18.243.65 6.032s - [21/Jul/2014:16:00:02 +0800]"
         + ' "GET /edge.v.iask.com/125880034.hlv HTTP/1.0" 200 70528990 "-"'
         + ' "Mozilla/5.0 (Windows NT 6.1; WOW64) AppleWebKit/537.36 (KHTML, like Gecko)'
         + ' Chrome/36.0.1985.125 Safari/537.36"'
```

### Comparing `logprep-6.2.0/tests/unit/processor/grokker/test_grokker.py` & `logprep-6.3.0/tests/unit/processor/grokker/test_grokker.py`

 * *Files 6% similar despite different names*

```diff
@@ -108,15 +108,15 @@
         {
             "filter": "winlog.event_id: 123456789",
             "grokker": {
                 "mapping": {
                     "winlog.event_data.normalize me!": [
                         "%{IP:some_ip_1} %{NUMBER:port_1:int} foo",
                         "%{IP:some_ip_2} %{NUMBER:port_2:int} bar",
-                        "%{IP:some_ip_3} %{NUMBER:port_3:int} bar",
+                        "%{IP:some_ip_2} %{NUMBER:port_2:int} bar",
                     ]
                 }
             },
         },
         {
             "winlog": {
                 "api": "wineventlog",
@@ -131,14 +131,44 @@
                 "event_data": {"normalize me!": "123.123.123.123 1234 bar"},
             },
             "some_ip_2": "123.123.123.123",
             "port_2": 1234,
         },
     ),
     (
+        "grok list match first matching after skipping non matching with same target fields",
+        {
+            "filter": "winlog.event_id: 123456789",
+            "grokker": {
+                "mapping": {
+                    "winlog.event_data.normalize me!": [
+                        "%{IP:some_ip} %{NUMBER:port:int} foo",
+                        "%{IP:some_ip} %{NUMBER:port:int} bar",
+                    ]
+                }
+            },
+        },
+        {
+            "winlog": {
+                "api": "wineventlog",
+                "event_id": 123456789,
+                "event_data": {"normalize me!": "123.123.123.123 1234 bar"},
+            }
+        },
+        {
+            "winlog": {
+                "api": "wineventlog",
+                "event_id": 123456789,
+                "event_data": {"normalize me!": "123.123.123.123 1234 bar"},
+            },
+            "some_ip": "123.123.123.123",
+            "port": 1234,
+        },
+    ),
+    (
         "normalization from nested grok",
         {
             "filter": "winlog.event_id: 123456789",
             "grokker": {
                 "mapping": {
                     "winlog.event_data.normalize me!": r"%{IP:[parent][some_ip]} \w+ %{NUMBER:[parent][port]:int} %[ts]+ %{NUMBER:test:int}"
                 },
@@ -212,14 +242,40 @@
         {"message": "this is the MyUser586"},
         {"message": "this is the MyUser586", "userfield": "MyUser586"},
     ),
 ]
 
 failure_test_cases = [
     (
+        "only field does not exist",
+        {"filter": "message", "grokker": {"mapping": {"unknown": "this is the %{USER:userfield}"}}},
+        {"message": "this is the MyUser586"},
+        {"message": "this is the MyUser586", "tags": ["_grokker_failure"]},
+        "missing source_field: 'unknown'",
+    ),
+    (
+        "only one field does not exist",
+        {
+            "filter": "message",
+            "grokker": {
+                "mapping": {
+                    "message": "this is the %{USER:userfield}",
+                    "unknown": "this is the %{USER:userfield}",
+                }
+            },
+        },
+        {"message": "this is the MyUser586"},
+        {
+            "message": "this is the MyUser586",
+            "userfield": "MyUser586",
+            "tags": ["_grokker_failure"],
+        },
+        "missing source_field: 'unknown'",
+    ),
+    (
         "writes failure tag if no grok patterns matches",
         {
             "filter": "grok_me",
             "grokker": {
                 "mapping": {
                     "grok_me": [
                         "%{IP:some_ip_1} %{NUMBER:port_1:int} foo",
```

### Comparing `logprep-6.2.0/tests/unit/processor/grokker/test_grokker_rule.py` & `logprep-6.3.0/tests/unit/processor/grokker/test_grokker_rule.py`

 * *Files 2% similar despite different names*

```diff
@@ -292,41 +292,41 @@
             (
                 {
                     "filter": "message",
                     "grokker": {
                         "mapping": {"message": "this is a %{USER:[user][username]}"},
                     },
                 },
-                {"message": "this is a %{USER:[user][username]}"},
+                {"message": ["this is a %{USER:[user][username]}"]},
             ),
             (
                 {
                     "filter": "message",
                     "grokker": {
                         "mapping": {"message": "this is a %{USER:user.username}"},
                     },
                 },
-                {"message": "this is a %{USER:[user][username]}"},
+                {"message": ["this is a %{USER:[user][username]}"]},
             ),
             (
                 {
                     "filter": "message",
                     "grokker": {
                         "mapping": {"message": "this is a %{USER:user.username.firstname}"},
                     },
                 },
-                {"message": "this is a %{USER:[user][username][firstname]}"},
+                {"message": ["this is a %{USER:[user][username][firstname]}"]},
             ),
             (
                 {
                     "filter": "message",
                     "grokker": {
                         "mapping": {"message": "this is a %{USER:user}"},
                     },
                 },
-                {"message": "this is a %{USER:user}"},
+                {"message": ["this is a %{USER:user}"]},
             ),
         ],
     )
     def test_ensure_dotted_field_notation_in_mapping(self, rule, expected_mapping):
         rule = GrokkerRule._create_from_dict(rule)
         assert rule._config.mapping == expected_mapping
```

### Comparing `logprep-6.2.0/tests/unit/processor/hyperscan_resolver/test_hyperscan_resolver.py` & `logprep-6.3.0/tests/unit/processor/hyperscan_resolver/test_hyperscan_resolver.py`

 * *Files identical despite different names*

### Comparing `logprep-6.2.0/tests/unit/processor/hyperscan_resolver/test_hyperscan_resolver_rule.py` & `logprep-6.3.0/tests/unit/processor/hyperscan_resolver/test_hyperscan_resolver_rule.py`

 * *Files identical despite different names*

### Comparing `logprep-6.2.0/tests/unit/processor/ip_informer/test_ip_informer.py` & `logprep-6.3.0/tests/unit/processor/ip_informer/test_ip_informer.py`

 * *Files identical despite different names*

### Comparing `logprep-6.2.0/tests/unit/processor/ip_informer/test_ip_informer_rule.py` & `logprep-6.3.0/tests/unit/processor/ip_informer/test_ip_informer_rule.py`

 * *Files identical despite different names*

### Comparing `logprep-6.2.0/tests/unit/processor/labeler/test_labeler.py` & `logprep-6.3.0/tests/unit/processor/labeler/test_labeler.py`

 * *Files identical despite different names*

### Comparing `logprep-6.2.0/tests/unit/processor/labeler/test_labeler_rule.py` & `logprep-6.3.0/tests/unit/processor/labeler/test_labeler_rule.py`

 * *Files identical despite different names*

### Comparing `logprep-6.2.0/tests/unit/processor/labeler/test_labeling_schema.py` & `logprep-6.3.0/tests/unit/processor/labeler/test_labeling_schema.py`

 * *Files identical despite different names*

### Comparing `logprep-6.2.0/tests/unit/processor/list_comparison/test_list_comparison.py` & `logprep-6.3.0/tests/unit/processor/list_comparison/test_list_comparison.py`

 * *Files identical despite different names*

### Comparing `logprep-6.2.0/tests/unit/processor/list_comparison/test_list_comparison_rule.py` & `logprep-6.3.0/tests/unit/processor/list_comparison/test_list_comparison_rule.py`

 * *Files identical despite different names*

### Comparing `logprep-6.2.0/tests/unit/processor/normalizer/test_normalizer.py` & `logprep-6.3.0/tests/unit/processor/normalizer/test_normalizer.py`

 * *Files identical despite different names*

### Comparing `logprep-6.2.0/tests/unit/processor/normalizer/test_normalizer_rule.py` & `logprep-6.3.0/tests/unit/processor/normalizer/test_normalizer_rule.py`

 * *Files identical despite different names*

### Comparing `logprep-6.2.0/tests/unit/processor/pre_detector/test_ip_alerter.py` & `logprep-6.3.0/tests/unit/processor/pre_detector/test_ip_alerter.py`

 * *Files identical despite different names*

### Comparing `logprep-6.2.0/tests/unit/processor/pre_detector/test_pre_detector.py` & `logprep-6.3.0/tests/unit/processor/pre_detector/test_pre_detector.py`

 * *Files identical despite different names*

### Comparing `logprep-6.2.0/tests/unit/processor/pre_detector/test_pre_detector_rule.py` & `logprep-6.3.0/tests/unit/processor/pre_detector/test_pre_detector_rule.py`

 * *Files identical despite different names*

### Comparing `logprep-6.2.0/tests/unit/processor/pseudonymizer/test_encrypter.py` & `logprep-6.3.0/tests/unit/processor/pseudonymizer/test_encrypter.py`

 * *Files identical despite different names*

### Comparing `logprep-6.2.0/tests/unit/processor/pseudonymizer/test_pseudonymizer.py` & `logprep-6.3.0/tests/unit/processor/pseudonymizer/test_pseudonymizer.py`

 * *Files identical despite different names*

### Comparing `logprep-6.2.0/tests/unit/processor/pseudonymizer/test_pseudonymizer_rule.py` & `logprep-6.3.0/tests/unit/processor/pseudonymizer/test_pseudonymizer_rule.py`

 * *Files identical despite different names*

### Comparing `logprep-6.2.0/tests/unit/processor/requester/test_requester.py` & `logprep-6.3.0/tests/unit/processor/requester/test_requester.py`

 * *Files identical despite different names*

### Comparing `logprep-6.2.0/tests/unit/processor/requester/test_requester_rule.py` & `logprep-6.3.0/tests/unit/processor/requester/test_requester_rule.py`

 * *Files identical despite different names*

### Comparing `logprep-6.2.0/tests/unit/processor/selective_extractor/test_selective_extractor.py` & `logprep-6.3.0/tests/unit/processor/selective_extractor/test_selective_extractor.py`

 * *Files identical despite different names*

### Comparing `logprep-6.2.0/tests/unit/processor/selective_extractor/test_selective_extractor_rule.py` & `logprep-6.3.0/tests/unit/processor/selective_extractor/test_selective_extractor_rule.py`

 * *Files identical despite different names*

### Comparing `logprep-6.2.0/tests/unit/processor/string_splitter/test_string_splitter.py` & `logprep-6.3.0/tests/unit/processor/string_splitter/test_string_splitter.py`

 * *Files identical despite different names*

### Comparing `logprep-6.2.0/tests/unit/processor/string_splitter/test_string_splitter_rule.py` & `logprep-6.3.0/tests/unit/processor/string_splitter/test_string_splitter_rule.py`

 * *Files identical despite different names*

### Comparing `logprep-6.2.0/tests/unit/processor/template_replacer/test_template_replacer.py` & `logprep-6.3.0/tests/unit/processor/template_replacer/test_template_replacer.py`

 * *Files identical despite different names*

### Comparing `logprep-6.2.0/tests/unit/processor/test_processor_rule.py` & `logprep-6.3.0/tests/unit/processor/test_processor_rule.py`

 * *Files identical despite different names*

### Comparing `logprep-6.2.0/tests/unit/processor/test_processor_strategy.py` & `logprep-6.3.0/tests/unit/processor/test_processor_strategy.py`

 * *Files identical despite different names*

### Comparing `logprep-6.2.0/tests/unit/processor/timestamp_differ/test_timestamp_differ.py` & `logprep-6.3.0/tests/unit/processor/timestamp_differ/test_timestamp_differ.py`

 * *Files identical despite different names*

### Comparing `logprep-6.2.0/tests/unit/processor/timestamp_differ/test_timestamp_differ_rule.py` & `logprep-6.3.0/tests/unit/processor/timestamp_differ/test_timestamp_differ_rule.py`

 * *Files identical despite different names*

### Comparing `logprep-6.2.0/tests/unit/processor/timestamper/test_timestamper.py` & `logprep-6.3.0/tests/unit/processor/timestamper/test_timestamper.py`

 * *Files 11% similar despite different names*

```diff
@@ -190,25 +190,59 @@
             "winlog": {
                 "api": "wineventlog",
                 "event_id": 123456789,
                 "event_data": {"some_timestamp_utc": "1642160449"},
             },
         },
     ),
+    (
+        "attempt parsing with multiple patterns, second one successful",
+        {
+            "filter": "message",
+            "timestamper": {
+                "source_fields": ["message"],
+                "source_format": ["%Y %m %d", "%Y %m %d - %H:%M:%S"],
+            },
+        },
+        {
+            "message": "2000 12 31 - 22:59:59",
+        },
+        {
+            "message": "2000 12 31 - 22:59:59",
+            "@timestamp": "2000-12-31T22:59:59Z",
+        },
+    ),
+    (
+        "attempt parsing with multiple patterns, both successful but stopping after first",
+        {
+            "filter": "message",
+            "timestamper": {
+                "source_fields": ["message"],
+                "source_format": ["%Y %m %d - %H:%M:%S", "%Y %m %d - %H:%M:%S"],
+            },
+        },
+        {
+            "message": "2000 12 31 - 22:59:59",
+        },
+        {
+            "message": "2000 12 31 - 22:59:59",
+            "@timestamp": "2000-12-31T22:59:59Z",
+        },
+    ),
 ]
 
 failure_test_cases = [
     (
         "normalization from timestamp with non matching patterns",
         {
             "filter": "winlog.event_id: 123456789",
             "timestamper": {
                 "source_fields": ["winlog.event_data.some_timestamp_utc"],
                 "target_field": "@timestamp",
-                "source_format": "a%Y %m",
+                "source_format": ["a%Y %m"],
                 "source_timezone": "UTC",
                 "target_timezone": "Europe/Berlin",
             },
         },
         {
             "winlog": {
                 "api": "wineventlog",
@@ -220,15 +254,30 @@
             "winlog": {
                 "api": "wineventlog",
                 "event_id": 123456789,
                 "event_data": {"some_timestamp_utc": "1999 12 12 - 12:12:22 UTC"},
             },
             "tags": ["_timestamper_failure"],
         },
-        r"does not match format",
+        r"Could not parse timestamp",
+    ),
+    (
+        "attempt parsing with multiple patterns, none is successful",
+        {
+            "filter": "message",
+            "timestamper": {
+                "source_fields": ["message"],
+                "source_format": ["%Y %m %d", "%H:%M:%S"],
+            },
+        },
+        {
+            "message": "2000 12 31 - 22:59:59",
+        },
+        {"message": "2000 12 31 - 22:59:59", "tags": ["_timestamper_failure"]},
+        r"Could not parse timestamp",
     ),
     (
         "raises if source field is none",
         {"filter": "message", "timestamper": {"source_fields": ["@timestamp"]}},
         {"message": "this does not matter"},
         {"message": "this does not matter", "tags": ["_timestamper_failure"]},
         "'@timestamp' does not exist or is falsy value",
```

### Comparing `logprep-6.2.0/tests/unit/test_configuration.py` & `logprep-6.3.0/tests/unit/test_configuration.py`

 * *Files identical despite different names*

### Comparing `logprep-6.2.0/tests/unit/test_factory.py` & `logprep-6.3.0/tests/unit/test_factory.py`

 * *Files identical despite different names*

### Comparing `logprep-6.2.0/tests/unit/test_run_logprep.py` & `logprep-6.3.0/tests/unit/test_run_logprep.py`

 * *Files identical despite different names*

### Comparing `logprep-6.2.0/tests/unit/test_runner.py` & `logprep-6.3.0/tests/unit/test_runner.py`

 * *Files identical despite different names*

### Comparing `logprep-6.2.0/tests/unit/util/test_auto_rule_corpus_tester.py` & `logprep-6.3.0/tests/unit/util/test_auto_rule_corpus_tester.py`

 * *Files identical despite different names*

### Comparing `logprep-6.2.0/tests/unit/util/test_auto_rule_tester.py` & `logprep-6.3.0/tests/unit/util/test_auto_rule_tester.py`

 * *Files identical despite different names*

### Comparing `logprep-6.2.0/tests/unit/util/test_cache.py` & `logprep-6.3.0/tests/unit/util/test_cache.py`

 * *Files identical despite different names*

### Comparing `logprep-6.2.0/tests/unit/util/test_configuration.py` & `logprep-6.3.0/tests/unit/util/test_configuration.py`

 * *Files identical despite different names*

### Comparing `logprep-6.2.0/tests/unit/util/test_getter.py` & `logprep-6.3.0/tests/unit/util/test_getter.py`

 * *Files identical despite different names*

### Comparing `logprep-6.2.0/tests/unit/util/test_grok_pattern_loader.py` & `logprep-6.3.0/tests/unit/util/test_grok_pattern_loader.py`

 * *Files identical despite different names*

### Comparing `logprep-6.2.0/tests/unit/util/test_helper.py` & `logprep-6.3.0/tests/unit/util/test_helper.py`

 * *Files identical despite different names*

### Comparing `logprep-6.2.0/tests/unit/util/test_helper_add_field.py` & `logprep-6.3.0/tests/unit/util/test_helper_add_field.py`

 * *Files identical despite different names*

### Comparing `logprep-6.2.0/tests/unit/util/test_log_aggregator.py` & `logprep-6.3.0/tests/unit/util/test_log_aggregator.py`

 * *Files identical despite different names*

### Comparing `logprep-6.2.0/tests/unit/util/test_processor_generator.py` & `logprep-6.3.0/tests/unit/util/test_processor_generator.py`

 * *Files identical despite different names*

### Comparing `logprep-6.2.0/tests/unit/util/test_prometheus_exporter.py` & `logprep-6.3.0/tests/unit/util/test_prometheus_exporter.py`

 * *Files identical despite different names*

### Comparing `logprep-6.2.0/tests/unit/util/test_rule_dry_runner.py` & `logprep-6.3.0/tests/unit/util/test_rule_dry_runner.py`

 * *Files identical despite different names*

### Comparing `logprep-6.2.0/tests/unit/util/test_time.py` & `logprep-6.3.0/tests/unit/util/test_time.py`

 * *Files identical despite different names*

### Comparing `logprep-6.2.0/tests/unit/util/test_time_measurement.py` & `logprep-6.3.0/tests/unit/util/test_time_measurement.py`

 * *Files identical despite different names*

### Comparing `logprep-6.2.0/tests/unit/util/test_validators.py` & `logprep-6.3.0/tests/unit/util/test_validators.py`

 * *Files identical despite different names*

### Comparing `logprep-6.2.0/tests/unit/util/tests_json_handling.py` & `logprep-6.3.0/tests/unit/util/tests_json_handling.py`

 * *Files identical despite different names*

### Comparing `logprep-6.2.0/tests/util/testhelpers.py` & `logprep-6.3.0/tests/util/testhelpers.py`

 * *Files identical despite different names*

### Comparing `logprep-6.2.0/versioneer.py` & `logprep-6.3.0/versioneer.py`

 * *Files identical despite different names*

