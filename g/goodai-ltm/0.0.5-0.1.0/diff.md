# Comparing `tmp/goodai-ltm-0.0.5.tar.gz` & `tmp/goodai-ltm-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "goodai-ltm-0.0.5.tar", last modified: Thu Apr 20 20:20:40 2023, max compression
+gzip compressed data, was "goodai-ltm-0.1.0.tar", last modified: Mon May 22 19:01:56 2023, max compression
```

## Comparing `goodai-ltm-0.0.5.tar` & `goodai-ltm-0.1.0.tar`

### file list

```diff
@@ -1,85 +1,98 @@
-drwxrwxrwx   0        0        0        0 2023-04-20 20:20:40.141632 goodai-ltm-0.0.5/
--rw-rw-rw-   0        0        0      184 2023-04-20 20:20:40.141632 goodai-ltm-0.0.5/PKG-INFO
--rw-rw-rw-   0        0        0     2087 2023-04-19 21:51:49.000000 goodai-ltm-0.0.5/README.md
-drwxrwxrwx   0        0        0        0 2023-04-20 20:20:40.037632 goodai-ltm-0.0.5/goodai/
-drwxrwxrwx   0        0        0        0 2023-04-20 20:20:40.055631 goodai-ltm-0.0.5/goodai/helpers/
--rw-rw-rw-   0        0        0        0 2023-04-19 16:47:00.000000 goodai-ltm-0.0.5/goodai/helpers/__init__.py
--rw-rw-rw-   0        0        0     1357 2023-04-18 18:54:58.000000 goodai-ltm-0.0.5/goodai/helpers/collections_helper.py
--rw-rw-rw-   0        0        0      717 2023-04-19 20:33:13.000000 goodai-ltm-0.0.5/goodai/helpers/file_helper.py
--rw-rw-rw-   0        0        0      214 2023-04-18 18:54:58.000000 goodai-ltm-0.0.5/goodai/helpers/html_helper.py
--rw-rw-rw-   0        0        0      165 2023-04-18 18:54:58.000000 goodai-ltm-0.0.5/goodai/helpers/json_helper.py
--rw-rw-rw-   0        0        0     3910 2023-04-18 18:54:58.000000 goodai-ltm-0.0.5/goodai/helpers/tokenizer_helper.py
--rw-rw-rw-   0        0        0      119 2023-04-18 18:54:58.000000 goodai-ltm-0.0.5/goodai/helpers/torch_helper.py
-drwxrwxrwx   0        0        0        0 2023-04-20 20:20:40.060632 goodai-ltm-0.0.5/goodai/ltm/
--rw-rw-rw-   0        0        0        0 2023-04-19 16:47:00.000000 goodai-ltm-0.0.5/goodai/ltm/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-20 20:20:40.063631 goodai-ltm-0.0.5/goodai/ltm/data/
--rw-rw-rw-   0        0        0        0 2023-04-19 16:47:00.000000 goodai-ltm-0.0.5/goodai/ltm/data/__init__.py
--rw-rw-rw-   0        0        0     1380 2023-04-18 18:54:58.000000 goodai-ltm-0.0.5/goodai/ltm/data/cloud.py
-drwxrwxrwx   0        0        0        0 2023-04-20 20:20:40.064632 goodai-ltm-0.0.5/goodai/ltm/data/names/
--rw-rw-rw-   0        0        0     1996 2023-04-19 22:25:12.000000 goodai-ltm-0.0.5/goodai/ltm/data/names/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-20 20:20:40.075632 goodai-ltm-0.0.5/goodai/ltm/data/query_passage/
--rw-rw-rw-   0        0        0        0 2023-04-19 16:47:00.000000 goodai-ltm-0.0.5/goodai/ltm/data/query_passage/__init__.py
--rw-rw-rw-   0        0        0     1626 2023-04-20 15:19:11.000000 goodai-ltm-0.0.5/goodai/ltm/data/query_passage/auto_data_source.py
--rw-rw-rw-   0        0        0      485 2023-04-20 19:49:15.000000 goodai-ltm-0.0.5/goodai/ltm/data/query_passage/data_source.py
--rw-rw-rw-   0        0        0     2422 2023-04-19 22:26:45.000000 goodai-ltm-0.0.5/goodai/ltm/data/query_passage/dataset.py
--rw-rw-rw-   0        0        0      331 2023-04-20 19:47:41.000000 goodai-ltm-0.0.5/goodai/ltm/data/query_passage/example.py
--rw-rw-rw-   0        0        0    11044 2023-04-20 19:51:43.000000 goodai-ltm-0.0.5/goodai/ltm/data/query_passage/qa.py
--rw-rw-rw-   0        0        0     1857 2023-04-19 22:30:12.000000 goodai-ltm-0.0.5/goodai/ltm/data/query_passage/qa_tok_entry.py
-drwxrwxrwx   0        0        0        0 2023-04-20 20:20:40.077631 goodai-ltm-0.0.5/goodai/ltm/data/query_passage/tests/
--rw-rw-rw-   0        0        0        0 2023-04-19 16:47:00.000000 goodai-ltm-0.0.5/goodai/ltm/data/query_passage/tests/__init__.py
--rw-rw-rw-   0        0        0     2527 2023-04-20 15:19:11.000000 goodai-ltm-0.0.5/goodai/ltm/data/query_passage/tests/test_query_passage_data_source.py
--rw-rw-rw-   0        0        0     6936 2023-04-20 19:54:07.000000 goodai-ltm-0.0.5/goodai/ltm/data/query_passage/wiki.py
-drwxrwxrwx   0        0        0        0 2023-04-20 20:20:40.090632 goodai-ltm-0.0.5/goodai/ltm/embedding_models/
--rw-rw-rw-   0        0        0        0 2023-04-19 16:47:01.000000 goodai-ltm-0.0.5/goodai/ltm/embedding_models/__init__.py
--rw-rw-rw-   0        0        0     1347 2023-04-20 15:19:11.000000 goodai-ltm-0.0.5/goodai/ltm/embedding_models/auto.py
--rw-rw-rw-   0        0        0     1554 2023-04-18 18:54:58.000000 goodai-ltm-0.0.5/goodai/ltm/embedding_models/contrast_classifier.py
--rw-rw-rw-   0        0        0     5366 2023-04-20 15:19:11.000000 goodai-ltm-0.0.5/goodai/ltm/embedding_models/default.py
--rw-rw-rw-   0        0        0     1533 2023-04-19 16:47:45.000000 goodai-ltm-0.0.5/goodai/ltm/embedding_models/emb_qp_prob_model.py
--rw-rw-rw-   0        0        0     2785 2023-04-20 15:19:11.000000 goodai-ltm-0.0.5/goodai/ltm/embedding_models/openai_emb.py
--rw-rw-rw-   0        0        0     2224 2023-04-20 15:19:11.000000 goodai-ltm-0.0.5/goodai/ltm/embedding_models/st_emb.py
--rw-rw-rw-   0        0        0     5440 2023-04-20 15:19:11.000000 goodai-ltm-0.0.5/goodai/ltm/embedding_models/trainable.py
--rw-rw-rw-   0        0        0     1584 2023-04-20 15:19:11.000000 goodai-ltm-0.0.5/goodai/ltm/embeddings.py
-drwxrwxrwx   0        0        0        0 2023-04-20 20:20:40.100632 goodai-ltm-0.0.5/goodai/ltm/eval/
--rw-rw-rw-   0        0        0        0 2023-04-19 16:47:00.000000 goodai-ltm-0.0.5/goodai/ltm/eval/__init__.py
--rw-rw-rw-   0        0        0      783 2023-04-20 15:19:11.000000 goodai-ltm-0.0.5/goodai/ltm/eval/auto.py
--rw-rw-rw-   0        0        0     4450 2023-04-20 19:42:22.000000 goodai-ltm-0.0.5/goodai/ltm/eval/mem.py
--rw-rw-rw-   0        0        0     2716 2023-04-19 23:22:15.000000 goodai-ltm-0.0.5/goodai/ltm/eval/metrics.py
--rw-rw-rw-   0        0        0     1901 2023-04-19 23:26:29.000000 goodai-ltm-0.0.5/goodai/ltm/eval/qrecc.py
--rw-rw-rw-   0        0        0     2072 2023-04-20 20:01:17.000000 goodai-ltm-0.0.5/goodai/ltm/eval/strategy_qa.py
-drwxrwxrwx   0        0        0        0 2023-04-20 20:20:40.102631 goodai-ltm-0.0.5/goodai/ltm/eval/tests/
--rw-rw-rw-   0        0        0     1420 2023-04-19 23:22:33.000000 goodai-ltm-0.0.5/goodai/ltm/eval/tests/test_metrics.py
--rw-rw-rw-   0        0        0     1188 2023-04-20 15:19:11.000000 goodai-ltm-0.0.5/goodai/ltm/matching.py
-drwxrwxrwx   0        0        0        0 2023-04-20 20:20:40.110633 goodai-ltm-0.0.5/goodai/ltm/matching_models/
--rw-rw-rw-   0        0        0        0 2023-04-19 16:47:01.000000 goodai-ltm-0.0.5/goodai/ltm/matching_models/__init__.py
--rw-rw-rw-   0        0        0      777 2023-04-20 15:19:11.000000 goodai-ltm-0.0.5/goodai/ltm/matching_models/auto.py
--rw-rw-rw-   0        0        0    10019 2023-04-19 22:29:29.000000 goodai-ltm-0.0.5/goodai/ltm/matching_models/default.py
--rw-rw-rw-   0        0        0      706 2023-04-20 15:19:11.000000 goodai-ltm-0.0.5/goodai/ltm/matching_models/prob_model.py
--rw-rw-rw-   0        0        0      658 2023-04-19 21:49:37.000000 goodai-ltm-0.0.5/goodai/ltm/matching_models/st_ce.py
--rw-rw-rw-   0        0        0     1208 2023-04-20 15:19:11.000000 goodai-ltm-0.0.5/goodai/ltm/memory.py
-drwxrwxrwx   0        0        0        0 2023-04-20 20:20:40.126632 goodai-ltm-0.0.5/goodai/ltm/memory_models/
--rw-rw-rw-   0        0        0        0 2023-04-19 16:47:00.000000 goodai-ltm-0.0.5/goodai/ltm/memory_models/__init__.py
--rw-rw-rw-   0        0        0     1376 2023-04-20 15:19:11.000000 goodai-ltm-0.0.5/goodai/ltm/memory_models/auto.py
--rw-rw-rw-   0        0        0     1238 2023-04-18 18:54:58.000000 goodai-ltm-0.0.5/goodai/ltm/memory_models/chunk.py
--rw-rw-rw-   0        0        0      679 2023-04-18 18:54:58.000000 goodai-ltm-0.0.5/goodai/ltm/memory_models/chunk_mixin.py
--rw-rw-rw-   0        0        0    10364 2023-04-20 15:19:11.000000 goodai-ltm-0.0.5/goodai/ltm/memory_models/chunk_queue.py
--rw-rw-rw-   0        0        0      181 2023-04-18 18:54:58.000000 goodai-ltm-0.0.5/goodai/ltm/memory_models/config.py
--rw-rw-rw-   0        0        0     5562 2023-04-19 22:25:35.000000 goodai-ltm-0.0.5/goodai/ltm/memory_models/default.py
--rw-rw-rw-   0        0        0     5784 2023-04-19 22:27:29.000000 goodai-ltm-0.0.5/goodai/ltm/memory_models/mem_foundation.py
--rw-rw-rw-   0        0        0     2960 2023-04-20 15:19:11.000000 goodai-ltm-0.0.5/goodai/ltm/memory_models/simple_vector_db.py
-drwxrwxrwx   0        0        0        0 2023-04-20 20:20:40.128631 goodai-ltm-0.0.5/goodai/ltm/memory_models/tests/
--rw-rw-rw-   0        0        0        0 2023-04-19 16:47:00.000000 goodai-ltm-0.0.5/goodai/ltm/memory_models/tests/__init__.py
--rw-rw-rw-   0        0        0     3101 2023-04-20 15:19:11.000000 goodai-ltm-0.0.5/goodai/ltm/memory_models/tests/test_chunk_queue.py
-drwxrwxrwx   0        0        0        0 2023-04-20 20:20:40.131636 goodai-ltm-0.0.5/goodai/ltm/training/
--rw-rw-rw-   0        0        0        0 2023-04-19 16:47:00.000000 goodai-ltm-0.0.5/goodai/ltm/training/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-20 20:20:40.134632 goodai-ltm-0.0.5/goodai/ltm/training/query_passage/
--rw-rw-rw-   0        0        0        0 2023-04-19 16:47:00.000000 goodai-ltm-0.0.5/goodai/ltm/training/query_passage/__init__.py
--rw-rw-rw-   0        0        0     7132 2023-04-19 16:47:45.000000 goodai-ltm-0.0.5/goodai/ltm/training/query_passage/trainer.py
--rw-rw-rw-   0        0        0     1473 2023-04-18 18:54:58.000000 goodai-ltm-0.0.5/goodai/ltm/training/sched_opt.py
-drwxrwxrwx   0        0        0        0 2023-04-20 20:20:40.140632 goodai-ltm-0.0.5/goodai_ltm.egg-info/
--rw-rw-rw-   0        0        0      184 2023-04-20 20:20:39.000000 goodai-ltm-0.0.5/goodai_ltm.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2357 2023-04-20 20:20:39.000000 goodai-ltm-0.0.5/goodai_ltm.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-20 20:20:39.000000 goodai-ltm-0.0.5/goodai_ltm.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      144 2023-04-20 20:20:39.000000 goodai-ltm-0.0.5/goodai_ltm.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-04-20 20:20:39.000000 goodai-ltm-0.0.5/goodai_ltm.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-20 20:20:40.141632 goodai-ltm-0.0.5/setup.cfg
--rw-rw-rw-   0        0        0      625 2023-04-20 19:37:55.000000 goodai-ltm-0.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-22 19:01:56.808776 goodai-ltm-0.1.0/
+-rw-rw-rw-   0        0        0     1084 2023-05-02 15:31:28.000000 goodai-ltm-0.1.0/LICENSE
+-rw-rw-rw-   0        0        0     2008 2023-05-22 19:01:56.807776 goodai-ltm-0.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0    15729 2023-05-22 19:01:10.000000 goodai-ltm-0.1.0/README.md
+drwxrwxrwx   0        0        0        0 2023-05-22 19:01:56.684777 goodai-ltm-0.1.0/goodai/
+drwxrwxrwx   0        0        0        0 2023-05-22 19:01:56.704779 goodai-ltm-0.1.0/goodai/helpers/
+-rw-rw-rw-   0        0        0        0 2023-05-02 15:31:28.000000 goodai-ltm-0.1.0/goodai/helpers/__init__.py
+-rw-rw-rw-   0        0        0     1357 2023-05-22 19:01:03.000000 goodai-ltm-0.1.0/goodai/helpers/collections_helper.py
+-rw-rw-rw-   0        0        0     3257 2023-05-11 14:39:36.000000 goodai-ltm-0.1.0/goodai/helpers/file_helper.py
+-rw-rw-rw-   0        0        0      214 2023-05-02 15:31:28.000000 goodai-ltm-0.1.0/goodai/helpers/html_helper.py
+-rw-rw-rw-   0        0        0      165 2023-05-02 15:31:28.000000 goodai-ltm-0.1.0/goodai/helpers/json_helper.py
+-rw-rw-rw-   0        0        0     1473 2023-05-03 13:13:46.000000 goodai-ltm-0.1.0/goodai/helpers/sched_opt.py
+-rw-rw-rw-   0        0        0     3911 2023-05-02 15:31:28.000000 goodai-ltm-0.1.0/goodai/helpers/tokenizer_helper.py
+-rw-rw-rw-   0        0        0      119 2023-05-02 15:31:28.000000 goodai-ltm-0.1.0/goodai/helpers/torch_helper.py
+drwxrwxrwx   0        0        0        0 2023-05-22 19:01:56.708777 goodai-ltm-0.1.0/goodai/ltm/
+-rw-rw-rw-   0        0        0       34 2023-05-02 15:31:28.000000 goodai-ltm-0.1.0/goodai/ltm/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-22 19:01:56.710777 goodai-ltm-0.1.0/goodai/ltm/data/
+-rw-rw-rw-   0        0        0        0 2023-05-02 15:31:28.000000 goodai-ltm-0.1.0/goodai/ltm/data/__init__.py
+-rw-rw-rw-   0        0        0     1380 2023-05-02 15:31:28.000000 goodai-ltm-0.1.0/goodai/ltm/data/cloud.py
+drwxrwxrwx   0        0        0        0 2023-05-22 19:01:56.714777 goodai-ltm-0.1.0/goodai/ltm/data/names/
+-rw-rw-rw-   0        0        0     1996 2023-05-02 15:31:28.000000 goodai-ltm-0.1.0/goodai/ltm/data/names/__init__.py
+-rw-rw-rw-   0        0        0   183119 2023-05-02 15:31:28.000000 goodai-ltm-0.1.0/goodai/ltm/data/names/wikidata-names.json
+drwxrwxrwx   0        0        0        0 2023-05-22 19:01:56.732776 goodai-ltm-0.1.0/goodai/ltm/data/query_passage/
+-rw-rw-rw-   0        0        0        0 2023-05-02 15:31:28.000000 goodai-ltm-0.1.0/goodai/ltm/data/query_passage/__init__.py
+-rw-rw-rw-   0        0        0     2281 2023-05-02 15:31:28.000000 goodai-ltm-0.1.0/goodai/ltm/data/query_passage/auto_data_source.py
+-rw-rw-rw-   0        0        0      485 2023-05-02 15:31:28.000000 goodai-ltm-0.1.0/goodai/ltm/data/query_passage/data_source.py
+-rw-rw-rw-   0        0        0     3036 2023-05-03 13:13:46.000000 goodai-ltm-0.1.0/goodai/ltm/data/query_passage/dataset.py
+-rw-rw-rw-   0        0        0      331 2023-05-02 15:31:28.000000 goodai-ltm-0.1.0/goodai/ltm/data/query_passage/example.py
+-rw-rw-rw-   0        0        0    11554 2023-05-03 13:13:46.000000 goodai-ltm-0.1.0/goodai/ltm/data/query_passage/qa.py
+-rw-rw-rw-   0        0        0     1857 2023-05-02 15:31:28.000000 goodai-ltm-0.1.0/goodai/ltm/data/query_passage/qa_tok_entry.py
+-rw-rw-rw-   0        0        0     8159 2023-05-03 13:13:46.000000 goodai-ltm-0.1.0/goodai/ltm/data/query_passage/sharc.py
+drwxrwxrwx   0        0        0        0 2023-05-22 19:01:56.734777 goodai-ltm-0.1.0/goodai/ltm/data/query_passage/tests/
+-rw-rw-rw-   0        0        0        0 2023-05-02 15:31:28.000000 goodai-ltm-0.1.0/goodai/ltm/data/query_passage/tests/__init__.py
+-rw-rw-rw-   0        0        0     2632 2023-05-08 20:37:32.000000 goodai-ltm-0.1.0/goodai/ltm/data/query_passage/tests/test_query_passage_data_source.py
+-rw-rw-rw-   0        0        0     7168 2023-05-03 13:13:46.000000 goodai-ltm-0.1.0/goodai/ltm/data/query_passage/wiki.py
+-rw-rw-rw-   0        0        0     7229 2023-05-03 13:13:46.000000 goodai-ltm-0.1.0/goodai/ltm/data/query_passage/wikianswers.py
+drwxrwxrwx   0        0        0        0 2023-05-22 19:01:56.749780 goodai-ltm-0.1.0/goodai/ltm/embeddings/
+-rw-rw-rw-   0        0        0        0 2023-05-02 15:31:28.000000 goodai-ltm-0.1.0/goodai/ltm/embeddings/__init__.py
+-rw-rw-rw-   0        0        0     2600 2023-05-11 14:39:36.000000 goodai-ltm-0.1.0/goodai/ltm/embeddings/auto.py
+-rw-rw-rw-   0        0        0     1726 2023-05-03 22:03:18.000000 goodai-ltm-0.1.0/goodai/ltm/embeddings/base.py
+-rw-rw-rw-   0        0        0     1554 2023-05-02 15:31:28.000000 goodai-ltm-0.1.0/goodai/ltm/embeddings/contrast_classifier.py
+-rw-rw-rw-   0        0        0     5994 2023-05-11 14:39:36.000000 goodai-ltm-0.1.0/goodai/ltm/embeddings/default.py
+-rw-rw-rw-   0        0        0     1515 2023-05-02 15:31:28.000000 goodai-ltm-0.1.0/goodai/ltm/embeddings/emb_qp_prob_model.py
+-rw-rw-rw-   0        0        0     3116 2023-05-11 14:39:36.000000 goodai-ltm-0.1.0/goodai/ltm/embeddings/openai_emb.py
+-rw-rw-rw-   0        0        0     2610 2023-05-03 22:03:18.000000 goodai-ltm-0.1.0/goodai/ltm/embeddings/st_emb.py
+-rw-rw-rw-   0        0        0     5962 2023-05-22 19:01:03.000000 goodai-ltm-0.1.0/goodai/ltm/embeddings/trainable.py
+drwxrwxrwx   0        0        0        0 2023-05-22 19:01:56.763775 goodai-ltm-0.1.0/goodai/ltm/eval/
+-rw-rw-rw-   0        0        0        0 2023-05-02 15:31:28.000000 goodai-ltm-0.1.0/goodai/ltm/eval/__init__.py
+-rw-rw-rw-   0        0        0     1589 2023-05-02 15:31:28.000000 goodai-ltm-0.1.0/goodai/ltm/eval/auto.py
+-rw-rw-rw-   0        0        0     4796 2023-05-18 14:51:26.000000 goodai-ltm-0.1.0/goodai/ltm/eval/mem.py
+-rw-rw-rw-   0        0        0     2716 2023-05-02 15:31:28.000000 goodai-ltm-0.1.0/goodai/ltm/eval/metrics.py
+-rw-rw-rw-   0        0        0     2158 2023-05-02 15:31:28.000000 goodai-ltm-0.1.0/goodai/ltm/eval/msmarco.py
+-rw-rw-rw-   0        0        0     1708 2023-05-02 15:31:28.000000 goodai-ltm-0.1.0/goodai/ltm/eval/qp_ds.py
+-rw-rw-rw-   0        0        0     1901 2023-05-02 15:31:28.000000 goodai-ltm-0.1.0/goodai/ltm/eval/qrecc.py
+-rw-rw-rw-   0        0        0     2072 2023-05-02 15:31:28.000000 goodai-ltm-0.1.0/goodai/ltm/eval/strategy_qa.py
+drwxrwxrwx   0        0        0        0 2023-05-22 19:01:56.765776 goodai-ltm-0.1.0/goodai/ltm/eval/tests/
+-rw-rw-rw-   0        0        0     1420 2023-05-02 15:31:28.000000 goodai-ltm-0.1.0/goodai/ltm/eval/tests/test_metrics.py
+drwxrwxrwx   0        0        0        0 2023-05-22 19:01:56.779776 goodai-ltm-0.1.0/goodai/ltm/mem/
+-rw-rw-rw-   0        0        0        0 2023-05-02 15:31:28.000000 goodai-ltm-0.1.0/goodai/ltm/mem/__init__.py
+-rw-rw-rw-   0        0        0     3550 2023-05-22 19:01:03.000000 goodai-ltm-0.1.0/goodai/ltm/mem/auto.py
+-rw-rw-rw-   0        0        0     2609 2023-05-22 19:01:03.000000 goodai-ltm-0.1.0/goodai/ltm/mem/base.py
+-rw-rw-rw-   0        0        0     1239 2023-05-22 19:01:03.000000 goodai-ltm-0.1.0/goodai/ltm/mem/chunk.py
+-rw-rw-rw-   0        0        0      679 2023-05-22 19:01:03.000000 goodai-ltm-0.1.0/goodai/ltm/mem/chunk_mixin.py
+-rw-rw-rw-   0        0        0    10596 2023-05-22 19:01:03.000000 goodai-ltm-0.1.0/goodai/ltm/mem/chunk_queue.py
+-rw-rw-rw-   0        0        0      995 2023-05-22 19:01:03.000000 goodai-ltm-0.1.0/goodai/ltm/mem/config.py
+-rw-rw-rw-   0        0        0     7939 2023-05-22 19:01:03.000000 goodai-ltm-0.1.0/goodai/ltm/mem/default.py
+-rw-rw-rw-   0        0        0    10980 2023-05-22 19:01:03.000000 goodai-ltm-0.1.0/goodai/ltm/mem/mem_foundation.py
+-rw-rw-rw-   0        0        0    13064 2023-05-11 14:39:36.000000 goodai-ltm-0.1.0/goodai/ltm/mem/rewrite_model.py
+-rw-rw-rw-   0        0        0     3454 2023-05-02 15:31:29.000000 goodai-ltm-0.1.0/goodai/ltm/mem/simple_vector_db.py
+drwxrwxrwx   0        0        0        0 2023-05-22 19:01:56.782777 goodai-ltm-0.1.0/goodai/ltm/mem/tests/
+-rw-rw-rw-   0        0        0        0 2023-05-02 15:31:29.000000 goodai-ltm-0.1.0/goodai/ltm/mem/tests/__init__.py
+-rw-rw-rw-   0        0        0     3091 2023-05-22 19:01:03.000000 goodai-ltm-0.1.0/goodai/ltm/mem/tests/test_chunk_queue.py
+-rw-rw-rw-   0        0        0     2747 2023-05-22 19:01:03.000000 goodai-ltm-0.1.0/goodai/ltm/mem/tests/test_mem.py
+drwxrwxrwx   0        0        0        0 2023-05-22 19:01:56.793775 goodai-ltm-0.1.0/goodai/ltm/reranking/
+-rw-rw-rw-   0        0        0        0 2023-05-02 15:31:29.000000 goodai-ltm-0.1.0/goodai/ltm/reranking/__init__.py
+-rw-rw-rw-   0        0        0     2003 2023-05-11 14:39:36.000000 goodai-ltm-0.1.0/goodai/ltm/reranking/auto.py
+-rw-rw-rw-   0        0        0     1248 2023-05-11 14:39:36.000000 goodai-ltm-0.1.0/goodai/ltm/reranking/base.py
+-rw-rw-rw-   0        0        0    10135 2023-05-11 14:39:36.000000 goodai-ltm-0.1.0/goodai/ltm/reranking/default.py
+-rw-rw-rw-   0        0        0     1857 2023-05-22 19:01:03.000000 goodai-ltm-0.1.0/goodai/ltm/reranking/emb.py
+-rw-rw-rw-   0        0        0      706 2023-05-02 15:31:29.000000 goodai-ltm-0.1.0/goodai/ltm/reranking/prob_model.py
+-rw-rw-rw-   0        0        0      672 2023-05-22 19:01:03.000000 goodai-ltm-0.1.0/goodai/ltm/reranking/st_ce.py
+drwxrwxrwx   0        0        0        0 2023-05-22 19:01:56.794776 goodai-ltm-0.1.0/goodai/ltm/training/
+-rw-rw-rw-   0        0        0        0 2023-05-02 15:31:29.000000 goodai-ltm-0.1.0/goodai/ltm/training/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-22 19:01:56.799776 goodai-ltm-0.1.0/goodai/ltm/training/query_passage/
+-rw-rw-rw-   0        0        0        0 2023-05-02 15:31:29.000000 goodai-ltm-0.1.0/goodai/ltm/training/query_passage/__init__.py
+-rw-rw-rw-   0        0        0     7420 2023-05-03 13:13:46.000000 goodai-ltm-0.1.0/goodai/ltm/training/query_passage/em_trainer.py
+-rw-rw-rw-   0        0        0     7635 2023-05-08 20:37:32.000000 goodai-ltm-0.1.0/goodai/ltm/training/query_passage/qppm_trainer.py
+-rw-rw-rw-   0        0        0       23 2023-05-18 14:51:26.000000 goodai-ltm-0.1.0/goodai/ltm/version.py
+drwxrwxrwx   0        0        0        0 2023-05-22 19:01:56.801778 goodai-ltm-0.1.0/goodai/modules/
+-rw-rw-rw-   0        0        0     1647 2023-05-11 14:39:36.000000 goodai-ltm-0.1.0/goodai/modules/loss.py
+drwxrwxrwx   0        0        0        0 2023-05-22 19:01:56.806776 goodai-ltm-0.1.0/goodai_ltm.egg-info/
+-rw-rw-rw-   0        0        0     2008 2023-05-22 19:01:56.000000 goodai-ltm-0.1.0/goodai_ltm.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2554 2023-05-22 19:01:56.000000 goodai-ltm-0.1.0/goodai_ltm.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-22 19:01:56.000000 goodai-ltm-0.1.0/goodai_ltm.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      144 2023-05-22 19:01:56.000000 goodai-ltm-0.1.0/goodai_ltm.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-05-22 19:01:56.000000 goodai-ltm-0.1.0/goodai_ltm.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-22 19:01:56.808776 goodai-ltm-0.1.0/setup.cfg
+-rw-rw-rw-   0        0        0     1043 2023-05-11 14:39:36.000000 goodai-ltm-0.1.0/setup.py
```

### Comparing `goodai-ltm-0.0.5/goodai/helpers/collections_helper.py` & `goodai-ltm-0.1.0/goodai/helpers/collections_helper.py`

 * *Files identical despite different names*

### Comparing `goodai-ltm-0.0.5/goodai/helpers/tokenizer_helper.py` & `goodai-ltm-0.1.0/goodai/helpers/tokenizer_helper.py`

 * *Files 2% similar despite different names*

```diff
@@ -53,21 +53,21 @@
             return i
     return -1
 
 
 def get_model_inputs(input_ids_list: List[List[int]], pad_id: int, device: torch.device,
                      min_seq_len: Optional[int] = None, prefix: str = '',
                      tokenizer: PreTrainedTokenizer = None, return_token_lengths: bool = False):
-    # Note: padding on the left
+    # Note: padding on the right
     max_seq_len = max(len(seq) for seq in input_ids_list)
     if min_seq_len is None:
         min_seq_len = max_seq_len
     else:
         min_seq_len = max(max_seq_len, min_seq_len)
-    input_ids_list = [[pad_id] * (min_seq_len - len(ids)) + ids for ids in input_ids_list]
+    input_ids_list = [ids + [pad_id] * (min_seq_len - len(ids)) for ids in input_ids_list]
     input_ids = torch.as_tensor(input_ids_list, dtype=torch.int64, device=device)
     attention_mask = (input_ids != pad_id).float()
     result = {
         prefix + 'input_ids': input_ids,
         prefix + 'attention_mask': attention_mask,
     }
     if return_token_lengths:
```

### Comparing `goodai-ltm-0.0.5/goodai/ltm/data/cloud.py` & `goodai-ltm-0.1.0/goodai/ltm/data/cloud.py`

 * *Files identical despite different names*

### Comparing `goodai-ltm-0.0.5/goodai/ltm/data/names/__init__.py` & `goodai-ltm-0.1.0/goodai/ltm/data/names/__init__.py`

 * *Files identical despite different names*

### Comparing `goodai-ltm-0.0.5/goodai/ltm/data/query_passage/dataset.py` & `goodai-ltm-0.1.0/goodai/ltm/data/query_passage/dataset.py`

 * *Files 16% similar despite different names*

```diff
@@ -9,40 +9,52 @@
 
 class QueryPassageDataset(Dataset):
     def __init__(
         self,
         data_sources: List[Tuple[BaseQueryPassageDataSource, float]],
         tokenizer: PreTrainedTokenizer,
         num_examples: int,
-        device: torch.device
+        device: torch.device,
+        add_special_tokens: bool = True,
+        approx_positive_fraction: float = 0.5,
     ):
         super().__init__()
         weight_sum = sum(w for _, w in data_sources)
 
         self.data_sources = data_sources
         self.tokenizer = tokenizer
         self.num_examples = num_examples
         self.device = device
         pad_id = tokenizer.pad_token_id
         if pad_id is None:
             raise SystemError('Tokenizer has no PAD token.')
+        bos_id = tokenizer.bos_token_id
+        eos_id = tokenizer.eos_token_id
 
         label_list = []
         query_list = []
         passage_list = []
 
         for i, (ds, weight) in enumerate(data_sources):
             w = weight / weight_sum
             n = round(num_examples * w)
-            items = ds.sample_items(n)
+            items = ds.sample_items(n, approx_positive_fraction=approx_positive_fraction)
             for item in items:
                 query_list.append(item.queryIds)
                 passage_list.append(item.passageIds)
                 label_list.append([1.0] if item.match else [0.0])
 
+        if add_special_tokens:
+            if bos_id is not None:
+                query_list = [[bos_id] + seq for seq in query_list]
+                passage_list = [[bos_id] + seq for seq in passage_list]
+            if eos_id is not None:
+                query_list = [seq + [eos_id] for seq in query_list]
+                passage_list = [seq + [eos_id] for seq in passage_list]
+
         query_inputs = get_model_inputs(query_list, pad_id, device, return_token_lengths=True, tokenizer=tokenizer)
         passage_inputs = get_model_inputs(passage_list, pad_id, device)
         self.query_input_ids = query_inputs['input_ids']
         self.query_att_mask = query_inputs['attention_mask']
         self.query_token_lengths = query_inputs['token_lengths']
         self.passage_input_ids = passage_inputs['input_ids']
         self.passage_att_mask = passage_inputs['attention_mask']
```

### Comparing `goodai-ltm-0.0.5/goodai/ltm/data/query_passage/qa.py` & `goodai-ltm-0.1.0/goodai/ltm/data/query_passage/qa.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import logging
-from typing import List, Dict, Tuple, Iterable
+from typing import List, Dict, Tuple, Iterable, Union
 
 import numpy as np
 from datasets import load_dataset, DatasetDict, Dataset
 
 from goodai.helpers.tokenizer_helper import get_sentence_punctuation_ids
 from goodai.ltm.data.query_passage.example import QueryPassageExample
 from transformers import PreTrainedTokenizer
@@ -120,21 +120,21 @@
         name2 = None
         if r.uniform() < use_names_p:
             name1, name2 = tuple(NameSource.get_instance().sample_first_names(r, 2))
         else:
             name1 = r.choice(['User', 'Player'])
         has_query_noise = self.random.uniform() < query_noise_p
         name_lead = ('\n' if has_query_noise else '') + name1 + ':'
-        name1_ids = self.tokenizer.encode(name_lead)
+        name1_ids = self.tokenizer.encode(name_lead, add_special_tokens=False)
         token_ids = name1_ids + tok_entry.question_token_ids
         ends_with_name = r.uniform() < ends_with_name_p
         if ends_with_name:
             if name2 is None:
                 name2 = r.choice(['AI', 'Assistant', 'Agent', 'NPC'])
-            name2_ids = self.tokenizer.encode('\n' + name2 + ':')
+            name2_ids = self.tokenizer.encode('\n' + name2 + ':', add_special_tokens=False)
             token_ids += name2_ids
         if has_query_noise:
             min_token_ids = min(self.max_query_tokens, max(self.min_query_tokens, len(token_ids)))
             num_tokens = r.randint(min_token_ids, self.max_query_tokens + 1)
             full_sequence = tok_entry.content_token_ids + token_ids
             num_noise_tokens = max(0, num_tokens - len(token_ids))
             return full_sequence[-num_tokens:], num_noise_tokens,
@@ -188,22 +188,22 @@
             passage_start = r.randint(0, p_to)
         passage_end = passage_start + num_tokens
         result = context_ids[passage_start:passage_end]
         if len(result) < self.min_passage_tokens:
             return None
         return result
 
-    def sample_item(self, is_match: bool, use_different_p=0.5) -> QueryPassageExample:
+    def sample_item(self, pos_index: int, is_match: bool, use_different_p=0.5) -> QueryPassageExample:
         r = self.random
         n = len(self.qa_examples)
         for attempt in range(100):
-            pos_index = r.randint(0, n)
             pos_tok_entry = self.get_tokenization(pos_index)
             if pos_tok_entry.answer_seq_index == -1:
                 logging.warning(f'Did not find location of answer excerpt in example with id {pos_tok_entry.e_id}')
+                pos_index = r.randint(0, n)
                 continue
             query_token_ids, nqn = self.get_query_token_ids(pos_tok_entry)
             if is_match:
                 passage_tok_entry = pos_tok_entry
                 non_answer = False
             else:
                 use_different = r.uniform() < use_different_p
@@ -213,16 +213,23 @@
                     non_answer = neg_index == pos_index
                     passage_tok_entry = neg_tok_entry
                 else:
                     non_answer = True
                     passage_tok_entry = pos_tok_entry
             passage_token_ids = self.get_passage_token_ids(passage_tok_entry, is_match, non_answer, nqn)
             if passage_token_ids is None:
+                if is_match or non_answer:
+                    pos_index = r.randint(0, n)
                 continue
             return QueryPassageExample(query_token_ids, passage_token_ids, is_match)
 
         raise SystemError('Unable to find suitable qa_example!')
 
+    def sample_item_indexes(self, total_items: int, sample_count: int) -> Union[List[int], np.ndarray]:
+        replace = sample_count > total_items
+        return self.random.choice(range(total_items), size=sample_count, replace=replace)
+
     def sample_items(self, count: int, approx_positive_fraction: float = 0.5) -> List[QueryPassageExample]:
         rnd_samples = self.random.uniform(size=count)
+        pos_indexes = self.sample_item_indexes(len(self.qa_examples), count)
         is_match = rnd_samples <= approx_positive_fraction
-        return [self.sample_item(is_match[i]) for i, _ in enumerate(range(count))]
+        return [self.sample_item(pos_indexes[i], is_match[i]) for i, _ in enumerate(range(count))]
```

### Comparing `goodai-ltm-0.0.5/goodai/ltm/data/query_passage/qa_tok_entry.py` & `goodai-ltm-0.1.0/goodai/ltm/data/query_passage/qa_tok_entry.py`

 * *Files identical despite different names*

### Comparing `goodai-ltm-0.0.5/goodai/ltm/data/query_passage/tests/test_query_passage_data_source.py` & `goodai-ltm-0.1.0/goodai/ltm/data/query_passage/tests/test_query_passage_data_source.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,27 +8,28 @@
 from goodai.helpers.html_helper import text_to_html
 
 
 class TestQueryPassageDataSource(unittest.TestCase):
     def test_show_examples(self):
         tokenizer: PreTrainedTokenizer = AutoTokenizer.from_pretrained('distilroberta-base')
         random = np.random.RandomState(1)
-        ds_names = ['adversarial_qa', 'coqa', 'squad_v2']
+        ds_names = ['wikianswers', 'sharc', 'adversarial_qa', 'coqa', 'squad_v2', 'wiki']
+        # ds_names = ['coqa', 'squad_v2']
         for ds_name in ds_names:
             print(f'Processing {ds_name}...')
             self._show_examples(random, ds_name, tokenizer)
 
     @staticmethod
     def _show_examples(random: np.random.RandomState, ds_name: str, tokenizer: PreTrainedTokenizer):
         train_ds, test_ds = AutoQueryPassageDataSource.create(ds_name, random, tokenizer,
                                                               max_query_tokens=40, min_passage_tokens=24,
                                                               max_passage_tokens=36)
 
         # Sample 100 examples from the training data source
-        examples = train_ds.sample_items(100)
+        examples = train_ds.sample_items(100, approx_positive_fraction=0.1)
 
         # Sort examples by match value
         examples.sort(key=lambda x: x.match, reverse=True)
 
         # Generate HTML table
         table_rows = ['<tr><th>Match</th><th>Query</th><th>Passage</th></tr>']
         for example in examples:
```

### Comparing `goodai-ltm-0.0.5/goodai/ltm/data/query_passage/wiki.py` & `goodai-ltm-0.1.0/goodai/ltm/data/query_passage/wiki.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import re
 from typing import List, Optional, Any, Dict, Tuple
 
 import numpy as np
+from datasets import load_dataset
 from transformers import PreTrainedTokenizer
 
 from goodai.ltm.data.query_passage.data_source import BaseQueryPassageDataSource
 from goodai.ltm.data.query_passage.example import QueryPassageExample
 
 
 class WikiQueryPassageDataSource(BaseQueryPassageDataSource):
@@ -28,19 +29,21 @@
         self.neg_article_token_ids: Optional[List[List[int]]] = None
         self.current_par_idx = -1
         self.tokenization_cache: Dict[int, List[List[int]]] = dict()
         self.par_pattern = re.compile(r'\r?\n\r?\n')
 
     @classmethod
     def create_data_sources(cls, train_fraction: float, random: np.random.RandomState, tokenizer: PreTrainedTokenizer,
-                            max_query_tokens: int, min_passage_tokens: int, max_passage_tokens: int,) ->\
+                            max_query_tokens: int, min_passage_tokens: int, max_passage_tokens: int,
+                            min_article_len: int = 512) ->\
             Tuple['WikiQueryPassageDataSource', 'WikiQueryPassageDataSource']:
-        # TODO access to sampled wikipedia data
-        wd = WikiData.get_instance()
-        articles = list(wd.get_articles())
+        ds = load_dataset('wikipedia', '20220301.simple')
+        ds_data = ds['train']
+        articles = list(ds_data)
+        articles = [a for a in articles if len(a['text']) >= min_article_len]
         random.shuffle(articles)
         train_len = round(len(articles) * train_fraction)
         train_articles = articles[:train_len]
         test_articles = articles[train_len:]
         train_ds = cls(random, tokenizer, train_articles, max_query_tokens, min_passage_tokens, max_passage_tokens)
         test_ds = cls(random, tokenizer, test_articles, max_query_tokens, min_passage_tokens, max_passage_tokens)
         return train_ds, test_ds,
@@ -62,15 +65,15 @@
 
     def is_new_article_needed(self):
         return self.pos_article_token_ids is None or self.current_par_idx >= len(self.pos_article_token_ids)
 
     def init_current_article(self):
         pos_art_token_ids: List[List[int]] = []
         neg_art_token_ids: List[List[int]] = []
-        for attempt in range(20):
+        for attempt in range(100):
             pos_index = self.random.randint(0, len(self.articles))
             pos_art_token_ids = self.get_tokenization(pos_index)
             if len(pos_art_token_ids) == 0:
                 continue
             neg_index = self.random.randint(0, len(self.articles))
             if neg_index == pos_index:
                 continue
@@ -80,15 +83,15 @@
             break
         if len(pos_art_token_ids) == 0 or len(neg_art_token_ids) == 0:
             raise SystemError('Unable to find article with suitable paragraph lengths.')
         self.neg_article_token_ids = neg_art_token_ids
         self.pos_article_token_ids = pos_art_token_ids
         self.current_par_idx = 0
 
-    def _get_neg_passage_ids(self, num_passage_tokens: int, p_use_different_art: float = 0.5):
+    def _get_neg_passage_ids(self, num_passage_tokens: int, p_use_different_art: float = 0.9):
         r = self.random
         use_different = r.uniform() < p_use_different_art
         if not use_different:
             from_par_idx = self.current_par_idx + 2
             to_par_idx = len(self.pos_article_token_ids)
             if from_par_idx < to_par_idx:
                 neg_par_idx = r.randint(from_par_idx, to_par_idx)
@@ -102,14 +105,15 @@
         flex = len(neg_par_token_ids) - num_passage_tokens
         passage_start = r.randint(0, flex + 1)
         passage_end = passage_start + num_passage_tokens
         passage_ids = neg_par_token_ids[passage_start:passage_end]
         return passage_ids
 
     def sample_items(self, count: int, approx_positive_fraction: float = 0.5) -> List[QueryPassageExample]:
+        # Note: sampling not suitable for embedding model training
         r = self.random
         result = []
         for i in range(count):
             if self.is_new_article_needed():
                 self.init_current_article()
             par_token_ids = self.pos_article_token_ids[self.current_par_idx]
             num_query_tokens = r.randint(self.min_query_tokens, self.max_query_tokens + 1)
```

### Comparing `goodai-ltm-0.0.5/goodai/ltm/embedding_models/contrast_classifier.py` & `goodai-ltm-0.1.0/goodai/ltm/embeddings/contrast_classifier.py`

 * *Files identical despite different names*

### Comparing `goodai-ltm-0.0.5/goodai/ltm/embedding_models/default.py` & `goodai-ltm-0.1.0/goodai/ltm/embeddings/default.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,52 +1,64 @@
 import itertools
+import logging
 from typing import Optional, Tuple
 
 import torch
 import torch.nn.functional as F
 from torch import nn
 from transformers import PreTrainedModel, PreTrainedTokenizer, PretrainedConfig
 from transformers.modeling_outputs import BaseModelOutput
 
 from goodai.helpers.tokenizer_helper import get_attention_after_token
-from goodai.ltm.embedding_models.trainable import TrainableEmbeddingModel
+from goodai.helpers.torch_helper import param_count
+from goodai.ltm.embeddings.trainable import TrainableEmbeddingModel
 
 
 class DefaultEmbeddingModel(TrainableEmbeddingModel):
     """
     Default implementation of trainable text embeddings.
     """
 
     def __init__(self, lang_model: PreTrainedModel, tokenizer: PreTrainedTokenizer,
                  num_retrieval_emb: int, num_storage_emb: int,
-                 num_end_chars_lb_ignore=18):
+                 num_end_chars_lb_ignore=18, inner_size=30, dropout=0.03):
         super(DefaultEmbeddingModel, self).__init__(tokenizer)
         lb_token_ids = tokenizer.encode('\n', add_special_tokens=False)
-        if len(lb_token_ids) != 1:
-            raise ValueError(f'Tokenizer {tokenizer.name_or_path} does not have a line break token!')
-        self.lb_token_id = lb_token_ids[0]
+        valid_lb_token_id = len(lb_token_ids) == 1
+        if not valid_lb_token_id:
+            logging.warning(f'Tokenizer "{tokenizer.name_or_path}" does not have a line-break token.')
+        self.lb_token_id = lb_token_ids[0] if valid_lb_token_id else -1
         self.num_end_chars_lb_ignore = num_end_chars_lb_ignore
         lm_config = lang_model.config
         self.lang_model = lang_model
         self.tokenizer = tokenizer
         self.num_storage_emb = num_storage_emb
         self.num_retrieval_emb = num_retrieval_emb
         self.emb_dim = self._get_embed_dim(lang_model, lang_model.config)
         hidden_size = lm_config.hidden_size
         out_size = num_retrieval_emb + num_storage_emb
         self.out_model = nn.Sequential(
-            nn.Dropout(p=0.03),
-            nn.Linear(hidden_size, out_size),
+            nn.Dropout(p=dropout),
+            nn.Linear(hidden_size, inner_size),
+            nn.ELU(),
+            nn.LayerNorm(inner_size),
+            nn.Dropout(p=dropout),
+            nn.Linear(inner_size, out_size),
         )
         self.dummy = nn.Parameter()
 
     @staticmethod
     def _get_embed_dim(model: PreTrainedModel, lm_config: PretrainedConfig):
         return lm_config.hidden_size
 
+    def get_info(self) -> str:
+        return f'GoodAI-finetuned model | Base: {self.lang_model.name_or_path} | ' \
+               f'Params: {param_count(self)/1e+6:.4g} million | Dimensions: {self.get_embedding_dim()} | ' \
+               f'{self.get_num_storage_embeddings()} storage embeddings'
+
     def get_device(self):
         return self.dummy.device
 
     def forward(self, is_retrieve: bool, token_lengths: Optional[torch.Tensor], **kwargs):
         input_ids = kwargs['input_ids']
         attention_mask = kwargs.get('attention_mask')
         if attention_mask is None:
@@ -68,41 +80,41 @@
         token_embeddings = lm_output.last_hidden_state
         # token_embeddings: (batch_size, seq_len, emb_size,)
         slf_att_logits_1 = self.out_model(token_embeddings)
         slf_att_logits = slf_att_logits_1 - 200 * (1.0 - out_att_mask[:, :, None])
         slf_att_logits = torch.clamp(slf_att_logits, min=-100, max=+80)
         slf_att_weights = torch.softmax(slf_att_logits, dim=1)
         # slf_att_weights: (batch_size, seq_len, total_keys,)
-        dot_product = token_embeddings[:, :, None, :] * slf_att_weights[:, :, :, None]
-        # dot_product: (batch_size, seq_len, total_keys, emb_size,)
+        emb_product = token_embeddings[:, :, None, :] * slf_att_weights[:, :, :, None]
+        # emb_product: (batch_size, seq_len, total_keys, emb_size,)
         if is_retrieve:
-            key_dot_product = dot_product[:, :, self.num_storage_emb:, :]
+            relevant_product = emb_product[:, :, self.num_storage_emb:, :]
         else:
-            key_dot_product = dot_product[:, :, :self.num_storage_emb, :]
-        raw_key_mean = torch.sum(key_dot_product, dim=1)
+            relevant_product = emb_product[:, :, :self.num_storage_emb, :]
+        raw_key_mean = torch.sum(relevant_product, dim=1)
         # raw_key_mean: (batch_size, num_keys, emb_size,)
         return F.normalize(raw_key_mean, dim=2)
 
     def get_lm_parameters(self):
         return self.lang_model.parameters()
 
     def get_added_parameters(self):
         return itertools.chain(self.out_model.parameters())
 
-    def get_storage_key(self, input_ids: torch.Tensor, attention_mask: torch.Tensor = None) -> torch.Tensor:
+    def get_storage_emb(self, input_ids: torch.Tensor, attention_mask: torch.Tensor = None) -> torch.Tensor:
         return self(input_ids=input_ids, token_lengths=None, attention_mask=attention_mask, is_retrieve=False)
 
-    def get_retrieval_key(self, input_ids: torch.Tensor, token_lengths: torch.Tensor,
+    def get_retrieval_emb(self, input_ids: torch.Tensor, token_lengths: torch.Tensor,
                           attention_mask: torch.Tensor = None) -> torch.Tensor:
         return self(input_ids=input_ids, token_lengths=token_lengths, attention_mask=attention_mask,
                     is_retrieve=True)
 
-    def get_keys(self, input_ids: torch.Tensor, attention_mask: torch.Tensor) -> Tuple[torch.Tensor, torch.Tensor]:
-        sk = self.get_storage_key(input_ids, attention_mask)
-        rk = self.get_retrieval_key(input_ids, attention_mask)
+    def get_emb(self, input_ids: torch.Tensor, attention_mask: torch.Tensor) -> Tuple[torch.Tensor, torch.Tensor]:
+        sk = self.get_storage_emb(input_ids, attention_mask)
+        rk = self.get_retrieval_emb(input_ids, attention_mask)
         return sk, rk,
 
     def get_embedding_dim(self) -> int:
         return self.emb_dim
 
     def get_num_retrieval_embeddings(self) -> int:
         return self.num_retrieval_emb
```

### Comparing `goodai-ltm-0.0.5/goodai/ltm/embedding_models/emb_qp_prob_model.py` & `goodai-ltm-0.1.0/goodai/ltm/embeddings/emb_qp_prob_model.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 import itertools
 import math
 
 import torch
 from torch import nn
 
-from goodai.ltm.embedding_models.contrast_classifier import ContrastClassifier
-from goodai.ltm.embedding_models.trainable import TrainableEmbeddingModel
-from goodai.ltm.matching_models.prob_model import BaseQueryPassageProbModel
+from goodai.ltm.embeddings.contrast_classifier import ContrastClassifier
+from goodai.ltm.embeddings.trainable import TrainableEmbeddingModel
+from goodai.ltm.reranking.prob_model import BaseQueryPassageProbModel
 
 
 class EmbeddingQueryPassageProbModel(nn.Module, BaseQueryPassageProbModel):
     def __init__(self, emb_model: TrainableEmbeddingModel):
         super(EmbeddingQueryPassageProbModel, self).__init__()
         self.emb_model = emb_model
         scale = math.sqrt(emb_model.get_embedding_dim())
         self.classifier = ContrastClassifier(scale)
 
     def forward(self, query_input_ids: torch.Tensor, query_attention_mask: torch.Tensor,
                 query_token_lengths: torch.Tensor,
                 passage_input_ids: torch.Tensor, passage_attention_mask: torch.Tensor) -> torch.Tensor:
-        rk = self.emb_model.get_retrieval_key(query_input_ids, token_lengths=query_token_lengths,
+        rk = self.emb_model.get_retrieval_emb(query_input_ids, token_lengths=query_token_lengths,
                                               attention_mask=query_attention_mask)
-        sk = self.emb_model.get_storage_key(passage_input_ids, passage_attention_mask)
+        sk = self.emb_model.get_storage_emb(passage_input_ids, passage_attention_mask)
         return self.classifier(rk, sk)
 
     def get_lm_parameters(self):
         return self.emb_model.get_lm_parameters()
 
     def get_added_parameters(self):
         km_added_parameters = self.emb_model.get_added_parameters()
```

### Comparing `goodai-ltm-0.0.5/goodai/ltm/embedding_models/openai_emb.py` & `goodai-ltm-0.1.0/goodai/ltm/embeddings/openai_emb.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,57 +3,65 @@
 import numpy as np
 import openai
 import torch
 from typing import List, Union
 
 from tqdm import tqdm
 
-from goodai.ltm.embeddings import BaseTextEmbeddingModel
+from goodai.ltm.embeddings.base import BaseTextEmbeddingModel
 
 _openai_lock = threading.Lock()
 
 
 class OpenAIEmbeddingModel(BaseTextEmbeddingModel):
     """
     Text embedding model based on OpenAI text embeddings.
 
     https://platform.openai.com/docs/guides/embeddings
     """
 
-    def __init__(self, api_key: str = None, model_name: str = 'text-embedding-ada-002', emb_dim: int = 1536):
+    def __init__(self, model_name: str = 'text-embedding-ada-002', emb_dim: int = 1536, api_key: str = None,
+                 device: Union[torch.Tensor, str] = None):
+        self.device = device
         self.api_key = api_key
         self.emb_dim = emb_dim
         self.model_name = model_name
 
     def get_embedding_dim(self) -> int:
         return self.emb_dim
 
     def get_num_retrieval_embeddings(self) -> int:
         return 1
 
     def get_num_storage_embeddings(self) -> int:
         return 1
 
+    def get_info(self) -> str:
+        return f'OpenAI embedding model "{self.model_name}" | Dimensions: {self.emb_dim}'
+
     def encode(self, sentences: List[str], batch_size: int = 64, show_progress_bar: bool = False,
                convert_to_tensor: bool = False,
                device: Union[str, torch.device] = None) -> Union[np.ndarray, torch.Tensor]:
+        if device is None:
+            device = self.device
         with _openai_lock:
-            openai.api_key = self.api_key
+            if self.api_key is not None:
+                openai.api_key = self.api_key
             rng = range(0, len(sentences), batch_size)
             if show_progress_bar:
                 rng = tqdm(rng, desc='Embeddings', unit='batch')
             all_emb_vectors = []
             for b0 in rng:
                 b_queries = sentences[b0:b0 + batch_size]
                 response = openai.Embedding.create(input=b_queries, model=self.model_name)
                 data_array = response['data']
                 emb_vectors = [entry['embedding'] for entry in data_array]
                 all_emb_vectors.extend(emb_vectors)
         if convert_to_tensor:
-            return torch.as_tensor(emb_vectors, dtype=torch.float, device=device).unsqueeze(1)
+            return torch.as_tensor(all_emb_vectors, dtype=torch.float, device=device).unsqueeze(1)
         else:
             return np.array(all_emb_vectors)[:, None, :]
 
     def encode_queries(self, queries: List[str], batch_size: int = 64, show_progress_bar: bool = False,
                        convert_to_tensor: bool = False,
                        device: Union[str, torch.device] = None) -> Union[np.ndarray, torch.Tensor]:
         return self.encode(queries, batch_size=batch_size, show_progress_bar=show_progress_bar,
```

### Comparing `goodai-ltm-0.0.5/goodai/ltm/embedding_models/trainable.py` & `goodai-ltm-0.1.0/goodai/ltm/embeddings/trainable.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import numpy as np
 import torch
 from torch import nn
 from tqdm import tqdm
 from transformers import PreTrainedTokenizer
 
 from goodai.helpers.tokenizer_helper import get_pad_token_id, get_model_inputs
-from goodai.ltm.embeddings import BaseTextEmbeddingModel
+from goodai.ltm.embeddings.base import BaseTextEmbeddingModel
 
 
 class TrainableEmbeddingModel(BaseTextEmbeddingModel, nn.Module):
     """
     Abstract base class for locally trainable text embeddings.
 
     Trainable embedding models support multiple retrieval and storage embeddings for a query or passage.
@@ -25,30 +25,30 @@
         self.tokenizer = tokenizer
         self.pad_token_id = get_pad_token_id(tokenizer)
 
     def get_device(self):
         return self.dummy.device
 
     @abstractmethod
-    def get_storage_key(self, input_ids: torch.Tensor, attention_mask: torch.Tensor = None) -> torch.Tensor:
+    def get_storage_emb(self, input_ids: torch.Tensor, attention_mask: torch.Tensor = None) -> torch.Tensor:
         """
         Returns an embedding of shape (batch_size, num_keys, emb_size,)
         """
         pass
 
     @abstractmethod
-    def get_retrieval_key(self, input_ids: torch.Tensor, token_lengths: torch.Tensor,
+    def get_retrieval_emb(self, input_ids: torch.Tensor, token_lengths: torch.Tensor,
                           attention_mask: torch.Tensor = None) -> torch.Tensor:
         """
         Returns an embedding of shape (batch_size, emb_size,)
         """
         pass
 
     @abstractmethod
-    def get_keys(self, input_ids: torch.Tensor, attention_mask: torch.Tensor) -> Tuple[torch.Tensor, torch.Tensor]:
+    def get_emb(self, input_ids: torch.Tensor, attention_mask: torch.Tensor) -> Tuple[torch.Tensor, torch.Tensor]:
         """
         Returns storage and retrieval embeddings.
         """
         pass
 
     @abstractmethod
     def get_lm_parameters(self):
@@ -60,66 +60,74 @@
     @abstractmethod
     def get_added_parameters(self):
         """
         :return: New parameters that don't belong to the pretrained language model.
         """
         pass
 
-    def get_storage_key_for_ids(self, input_ids: List[List[int]]):
+    def get_storage_emb_for_ids(self, input_ids: List[List[int]]):
         device = self.get_device()
         pad_token_id = self.pad_token_id
         m_inputs = get_model_inputs(input_ids, pad_id=pad_token_id, device=device)
-        return self.get_storage_key(**m_inputs)
+        return self.get_storage_emb(**m_inputs)
 
-    def get_retrieval_key_for_ids(self, input_ids: List[List[int]]):
+    def get_retrieval_emb_for_ids(self, input_ids: List[List[int]]):
         device = self.get_device()
         pad_token_id = self.pad_token_id
         m_inputs = get_model_inputs(input_ids, pad_id=pad_token_id, device=device, return_token_lengths=True,
                                     tokenizer=self.tokenizer)
-        return self.get_retrieval_key(**m_inputs)
+        return self.get_retrieval_emb(**m_inputs)
 
     def _get_token_ids(self, texts: List[str]) -> List[List[int]]:
         tok = self.tokenizer
         return [tok.encode(text, add_special_tokens=False) for text in texts]
 
-    def encode_in_batches(self, enc_fn: Callable, sentences: List[str], batch_size: int = 64,
+    def encode_in_batches(self, enc_fn: Callable, sentences: List[str],
+                          add_special_tokens: bool = True,
+                          batch_size: int = 50,
                           show_progress_bar: bool = False,
                           convert_to_tensor: bool = False,
                           return_token_lengths: bool = False,
+                          detach_tensors: bool = True,
                           device: Union[str, torch.device] = None):
         device = device if device else self.get_device()
         t = self.tokenizer
         rng = range(0, len(sentences), batch_size)
         if show_progress_bar:
             rng = tqdm(rng, desc='Embeddings', unit='batch')
         keys_list = []
         for b0 in rng:
             b_sentences = sentences[b0:b0 + batch_size]
-            input_ids_list = [t.encode(s, add_special_tokens=False) for s in b_sentences]
+            input_ids_list = [t.encode(s, add_special_tokens=add_special_tokens) for s in b_sentences]
             model_inputs = get_model_inputs(input_ids_list, self.pad_token_id,
                                             return_token_lengths=return_token_lengths,
+                                            tokenizer=self.tokenizer,
                                             device=device)
             keys = enc_fn(**model_inputs)
+            if detach_tensors or not convert_to_tensor:
+                keys = keys.detach()
             keys_list.append(keys)
         result = torch.cat(keys_list)
         if convert_to_tensor:
             return result
         else:
             return result.detach().cpu().numpy()
 
     def encode_queries(self, queries: List[str], batch_size: int = 64, show_progress_bar: bool = False,
-                       convert_to_tensor: bool = False,
+                       convert_to_tensor: bool = False, detach_tensors: bool = True,
                        device: Union[str, torch.device] = None) -> Union[np.ndarray, torch.Tensor]:
-        return self.encode_in_batches(self.get_retrieval_key, queries, batch_size=batch_size,
+        return self.encode_in_batches(self.get_retrieval_emb, queries, batch_size=batch_size,
                                       show_progress_bar=show_progress_bar,
                                       convert_to_tensor=convert_to_tensor,
+                                      detach_tensors=detach_tensors,
                                       return_token_lengths=True,
                                       device=device)
 
     def encode_corpus(self, passages: List[str], batch_size: int = 64, show_progress_bar: bool = False,
-                      convert_to_tensor: bool = False,
+                      convert_to_tensor: bool = False, detach_tensors: bool = True,
                       device: Union[str, torch.device] = None) -> Union[np.ndarray, torch.Tensor]:
-        return self.encode_in_batches(self.get_retrieval_key, passages, batch_size=batch_size,
+        return self.encode_in_batches(self.get_storage_emb, passages, batch_size=batch_size,
                                       show_progress_bar=show_progress_bar,
                                       convert_to_tensor=convert_to_tensor,
+                                      detach_tensors=detach_tensors,
                                       return_token_lengths=False,
                                       device=device)
```

### Comparing `goodai-ltm-0.0.5/goodai/ltm/embeddings.py` & `goodai-ltm-0.1.0/goodai/ltm/embeddings/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,14 +31,21 @@
     def get_num_storage_embeddings(self) -> int:
         """
         :return: The number of storage embeddings produced by the model, per passage.
         """
         pass
 
     @abstractmethod
+    def get_info(self) -> str:
+        """
+        :return: Information about the model.
+        """
+        pass
+
+    @abstractmethod
     def encode_queries(self, queries: List[str], batch_size: int = 64, show_progress_bar: bool = False,
                        convert_to_tensor: bool = False,
                        device: Union[str, torch.device] = None) -> Union[np.ndarray, torch.Tensor]:
         pass
 
     @abstractmethod
     def encode_corpus(self, passages: List[str], batch_size: int = 64, show_progress_bar: bool = False,
```

### Comparing `goodai-ltm-0.0.5/goodai/ltm/eval/mem.py` & `goodai-ltm-0.1.0/goodai/ltm/eval/mem.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 import abc
+import logging
 from abc import ABC
 from dataclasses import dataclass
 from typing import List, Dict, Tuple
 
 import numpy as np
 from tqdm import tqdm
 from transformers import PreTrainedTokenizer
 
 from goodai.ltm.data.names import NameSource
 from goodai.ltm.eval.metrics import get_correctness_score
-from goodai.ltm.memory import BaseTextMemory
+from goodai.ltm.mem.base import BaseTextMemory
 
 
 @dataclass
 class QAScenario:
     context: List[str]
     supportingFacts: List[str]
     question: str
@@ -43,21 +44,25 @@
         pass
 
     @abc.abstractmethod
     def get_scenarios(self) -> List[QAScenario]:
         pass
 
     def get_query(self, scenario: QAScenario) -> str:
-        name1, name2 = tuple(NameSource.get_instance().sample_first_names(self.rnd1, count=2))
-        names = [name1, name2]
-        names_context = [f'{names[i % 2]}: {ctx}' for i, ctx in enumerate(scenario.context)]
-        c_len = len(names_context)
-        q_name = names[c_len % 2]
-        a_name = names[(c_len + 1) % 2]
-        query = f'{q_name}: {scenario.question}\n{a_name}:'
+        if self.add_names_to_context:
+            name1, name2 = tuple(NameSource.get_instance().sample_first_names(self.rnd1, count=2))
+            names = [name1, name2]
+            names_context = [f'{names[i % 2]}: {ctx}' for i, ctx in enumerate(scenario.context)]
+            c_len = len(names_context)
+            q_name = names[c_len % 2]
+            a_name = names[(c_len + 1) % 2]
+            query = f'{q_name}: {scenario.question}\n{a_name}:'
+        else:
+            names_context = scenario.context
+            query = scenario.question
         truncate_q_ids_at = self.max_query_tokens
         if self.has_query_noise:
             no_noise_ids = self.tokenizer.encode(query, add_special_tokens=False)
             len_nni = len(no_noise_ids)
             if len_nni < self.max_query_tokens:
                 truncate_q_ids_at = self.rnd2.randint(max(1, len_nni), self.max_query_tokens + 1)
             context_as_text = '\n'.join(names_context[-3:])
@@ -81,23 +86,26 @@
         for rt in retrieved_texts:
             scores = [get_correctness_score(self.tokenizer, rt, f) for f in supporting_facts]
             result.append(max(scores))
         return result
 
     def evaluate(self, memory: BaseTextMemory) -> Dict[str, float]:
         facts = self.get_facts_to_be_stored()
-        for fact in tqdm(facts, desc='Storage', unit='fact'):
-            memory.add_text(fact + '\n')
+        facts_text = '\n'.join(facts)
+        memory.add_text(facts_text + '\n', show_progress_bar=True)
         scenarios = self.get_scenarios()
         queries, supports = self.get_queries_and_support(scenarios)
         k = max(self.top_ks)
         retrieved = memory.retrieve_multiple(queries, k=k, show_progress_bar=True)
         top_k_map: Dict[int, int] = dict()
-        for s_retrieved, s_supports in tqdm(zip(retrieved, supports), desc='Comparison', unit='scenario'):
+        for q, s_retrieved, s_supports in tqdm(zip(queries, retrieved, supports), desc='Comparison', unit='scenario'):
             s_retrieved_texts = [r.passage for r in s_retrieved]
+            if len(s_retrieved_texts) == 0:
+                logging.warning(f'No memories retrieved with query "{q}"')
+                continue
             correctness_values = self.cross_max_correctness(s_retrieved_texts, s_supports)
             for top_k in self.top_ks:
                 selected_cv = correctness_values[:top_k]
                 if max(selected_cv) >= self.correctness_threshold:
                     top_k_map[top_k] = top_k_map.get(top_k, 0) + 1
         item_count = len(retrieved)
         return {f'ACC@{top_k}': v / item_count for top_k, v in top_k_map.items()}
```

### Comparing `goodai-ltm-0.0.5/goodai/ltm/eval/metrics.py` & `goodai-ltm-0.1.0/goodai/ltm/eval/metrics.py`

 * *Files identical despite different names*

### Comparing `goodai-ltm-0.0.5/goodai/ltm/eval/qrecc.py` & `goodai-ltm-0.1.0/goodai/ltm/eval/qrecc.py`

 * *Files identical despite different names*

### Comparing `goodai-ltm-0.0.5/goodai/ltm/eval/strategy_qa.py` & `goodai-ltm-0.1.0/goodai/ltm/eval/strategy_qa.py`

 * *Files identical despite different names*

### Comparing `goodai-ltm-0.0.5/goodai/ltm/eval/tests/test_metrics.py` & `goodai-ltm-0.1.0/goodai/ltm/eval/tests/test_metrics.py`

 * *Files identical despite different names*

### Comparing `goodai-ltm-0.0.5/goodai/ltm/matching.py` & `goodai-ltm-0.1.0/goodai/ltm/reranking/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,7 +22,10 @@
         return self.predict(sentences, batch_size=batch_size, show_progress_bar=show_progress_bar)
 
     @abstractmethod
     def predict(self, sentences: List[Tuple[str, str]], batch_size: int = 32,
                 show_progress_bar: bool = False) -> List[float]:
         pass
 
+    @abstractmethod
+    def get_info(self):
+        pass
```

### Comparing `goodai-ltm-0.0.5/goodai/ltm/matching_models/default.py` & `goodai-ltm-0.1.0/goodai/ltm/reranking/default.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,82 +1,88 @@
 import itertools
+import logging
 import math
 import torch
 from torch import nn
 import torch.nn.functional as F
 from tqdm import tqdm
 from transformers import AutoModel, AutoTokenizer, PreTrainedTokenizer
 from typing import List, Optional, Tuple
 
 from goodai.helpers.tokenizer_helper import get_attention_after_token, get_model_inputs
-from goodai.ltm.embedding_models.contrast_classifier import ContrastClassifier
-from goodai.ltm.matching import BaseTextMatchingModel
-from goodai.ltm.matching_models.prob_model import BaseQueryPassageProbModel
+from goodai.helpers.torch_helper import param_count
+from goodai.ltm.embeddings.contrast_classifier import ContrastClassifier
+from goodai.ltm.reranking.base import BaseTextMatchingModel
+from goodai.ltm.reranking.prob_model import BaseQueryPassageProbModel
 
 
 class DefaultRerankingCrossEncoder(nn.Module, BaseQueryPassageProbModel, BaseTextMatchingModel):
     sep_id_tensor: torch.Tensor
 
     def __init__(self, model_name: str, default_query_seq_len: Optional[int] = None,
-                 default_passage_seq_len: Optional[int] = None, num_end_chars_lb_ignore=18):
+                 default_passage_seq_len: Optional[int] = None, num_end_chars_lb_ignore=18,
+                 dropout=0.01):
         super().__init__()
         self.num_end_chars_lb_ignore = num_end_chars_lb_ignore
         self.default_passage_seq_len = default_passage_seq_len
         self.default_query_seq_len = default_query_seq_len
         self.model = AutoModel.from_pretrained(model_name, output_hidden_states=True)
         self.tokenizer: PreTrainedTokenizer = AutoTokenizer.from_pretrained(model_name)
         hidden_size = self.model.config.hidden_size
         cls_emb_scale = math.sqrt(hidden_size)
         self.classifier = ContrastClassifier(cls_emb_scale)
         lb_token_ids = self.tokenizer.encode('\n', add_special_tokens=False)
         if len(lb_token_ids) != 1:
-            raise ValueError(f'Tokenizer {self.tokenizer.name_or_path} does not have a line break token!')
+            logging.warning(f'Tokenizer {self.tokenizer.name_or_path} does not have a line break token.')
+            self.lb_token_id = -1
+        else:
+            self.lb_token_id = lb_token_ids[0]
         if self.tokenizer.sep_token_id is None:
             self.tokenizer.sep_token_id = self.tokenizer.eos_token_id
         if self.tokenizer.sep_token_id is None:
             raise ValueError(f'Tokenizer {model_name} does not have SEP or EOS tokens!')
         if self.tokenizer.sep_token_id == self.tokenizer.pad_token_id:
             raise ValueError(f'Tokenizer {model_name} with SEP equal to PAD not supported!')
-        self.lb_token_id = lb_token_ids[0]
         sep_id_tensor = torch.as_tensor([[self.tokenizer.sep_token_id]], dtype=torch.long)
         self.register_buffer('sep_id_tensor', sep_id_tensor)
         self.dummy = nn.Parameter()
-        self.query_slfatt_model = nn.Sequential(
-            nn.Dropout(p=0.03),
-            nn.Linear(hidden_size, 1)
-        )
         self.passage_slfatt_model = nn.Sequential(
-            nn.Dropout(p=0.03),
-            nn.Linear(hidden_size, 4)
+            nn.Dropout(p=dropout),
+            nn.Linear(hidden_size, 5),
         )
 
+    def get_info(self):
+        return f'{self.__class__} | Params: {param_count(self) / 1e6:.4g} million'
+
     def get_device(self):
         return self.dummy.device
 
     def get_lm_parameters(self):
         return self.model.parameters()
 
     def get_added_parameters(self):
-        return itertools.chain(self.query_slfatt_model.parameters(),
-                               self.passage_slfatt_model.parameters(),
+        return itertools.chain(self.passage_slfatt_model.parameters(),
                                self.classifier.parameters())
 
     @staticmethod
     def get_embedding(hidden_states: torch.Tensor, attention_mask: torch.Tensor,
-                      att_model: nn.Module) -> torch.Tensor:
+                      att_model: Optional[nn.Module]) -> torch.Tensor:
         # hidden_states: (batch_size, seq_len, emb_size,)
         x_att_mask = attention_mask[:, :, None]
-        # x_att_mask: (batch_size, seq_len, 1,)
-        slf_att_logits = att_model(hidden_states)
-        # slf_att_logits: (batch_size, seq_len, total_keys,)
-        slf_att_logits = slf_att_logits - 200.0 * (1.0 - x_att_mask)
-        slf_att_logits = torch.clamp(slf_att_logits, min=-100, max=+80)
-        slf_att_weights = torch.softmax(slf_att_logits, dim=1)
-        # slf_att_weights: (batch_size, seq_len, total_keys,)
-        dot_product = hidden_states[:, :, None, :] * slf_att_weights[:, :, :, None]
+        if att_model:
+            # x_att_mask: (batch_size, seq_len, 1,)
+            slf_att_logits = att_model(hidden_states)
+            # slf_att_logits: (batch_size, seq_len, total_keys,)
+            slf_att_logits = slf_att_logits - 200.0 * (1.0 - x_att_mask)
+            slf_att_logits = torch.clamp(slf_att_logits, min=-100, max=+80)
+            slf_att_weights = torch.softmax(slf_att_logits, dim=1)
+            # slf_att_weights: (batch_size, seq_len, total_keys,)
+            dot_product = hidden_states[:, :, None, :] * slf_att_weights[:, :, :, None]
+        else:
+            dot_product = hidden_states[:, :, None, :] * x_att_mask[:, :, :, None]
         raw_w_mean = torch.sum(dot_product, dim=1)
         # raw_w_mean: (batch_size, total_keys, emb_size,)
         return F.normalize(raw_w_mean, dim=-1)
 
     def forward(self, query_input_ids: torch.Tensor, query_attention_mask: torch.Tensor,
                 query_token_lengths: torch.Tensor,
                 passage_input_ids: torch.Tensor, passage_attention_mask: torch.Tensor) -> torch.Tensor:
@@ -89,15 +95,15 @@
         last_hidden_states = outputs.last_hidden_state
         query_hidden_states = last_hidden_states[:, :query_len]
         passage_hidden_states = last_hidden_states[:, -passage_len:]
         lb_att_mask = get_attention_after_token(query_input_ids, query_attention_mask, query_token_lengths,
                                                 self.lb_token_id, exclude_last_n_chars=self.num_end_chars_lb_ignore,
                                                 device=self.get_device())
         emb_q_att_mask = query_attention_mask * lb_att_mask
-        query_embedding = self.get_embedding(query_hidden_states, emb_q_att_mask, self.query_slfatt_model)
+        query_embedding = self.get_embedding(query_hidden_states, emb_q_att_mask, None)
         passage_embedding = self.get_embedding(passage_hidden_states, passage_attention_mask, self.passage_slfatt_model)
         match_probabilities = self.classifier(query_embedding, passage_embedding)
         return match_probabilities
 
     def get_probabilities_in_batches(self, query_input_ids: torch.Tensor, query_attention_mask: torch.Tensor,
                                      query_token_lengths: torch.Tensor,
                                      passage_input_ids: torch.Tensor, passage_attention_mask: torch.Tensor,
@@ -143,18 +149,17 @@
         passage_ids_list = []
         for query, passage in sentences:
             query_ids = tokenizer.encode(query, add_special_tokens=False)
             if len(query_ids) > max_query_tokens:
                 query_ids = query_ids[-max_query_tokens:]
             passage_ids = tokenizer.encode(passage, add_special_tokens=False)
             if len(passage_ids) > max_passage_tokens:
-                passage_ids = query_ids[-max_passage_tokens:]
+                passage_ids = passage_ids[-max_passage_tokens:]
             passage_ids_list.append(passage_ids)
             query_ids_list.append(query_ids)
-        # Convert input_ids_list to tensor input_ids and attention_mask by adding padding
         device = self.get_device()
         query_seq_len = self.default_query_seq_len if use_preferred_seq_lengths else None
         passage_seq_len = self.default_passage_seq_len if use_preferred_seq_lengths else None
         query_inputs = get_model_inputs(query_ids_list, pad_id, device, prefix='query_',
                                         min_seq_len=query_seq_len, return_token_lengths=True,
                                         tokenizer=tokenizer)
         passage_inputs = get_model_inputs(passage_ids_list, pad_id, device, prefix='passage_',
```

### Comparing `goodai-ltm-0.0.5/goodai/ltm/matching_models/prob_model.py` & `goodai-ltm-0.1.0/goodai/ltm/reranking/prob_model.py`

 * *Files identical despite different names*

### Comparing `goodai-ltm-0.0.5/goodai/ltm/matching_models/st_ce.py` & `goodai-ltm-0.1.0/goodai/ltm/reranking/st_ce.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from typing import List, Tuple
 
 from sentence_transformers import CrossEncoder
 
-from goodai.ltm.matching import BaseTextMatchingModel
+from goodai.ltm.reranking.base import BaseTextMatchingModel
 
 
 class SentenceTransformerTextMatchingModel(BaseTextMatchingModel):
     def __init__(self, model_name: str):
         self.ce = CrossEncoder(model_name)
 
     def predict(self, sentences: List[Tuple[str, str]], batch_size: int = 32,
                 show_progress_bar: bool = False) -> List[float]:
         results = self.ce.predict(sentences, batch_size=batch_size, show_progress_bar=show_progress_bar,
-                                  convert_to_tensor=False, convert_to_numpy=False)
-        return results
+                                  convert_to_tensor=True, convert_to_numpy=False)
+        return results.tolist()
```

### Comparing `goodai-ltm-0.0.5/goodai/ltm/memory_models/chunk.py` & `goodai-ltm-0.1.0/goodai/ltm/mem/chunk.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from typing import Any, Optional
 
 
 class Chunk:
-    def __init__(self, index: int, capacity: int, from_token_seq_id: int, metadata: Optional[Any]):
+    def __init__(self, index: int, capacity: int, from_token_seq_id: int, metadata: Optional[dict]):
         self.metadata = metadata
         self.index = index
         self.capacity = capacity
         self.from_token_seq_id = from_token_seq_id
         self.to_token_seq_id = from_token_seq_id
         self.indexed: bool = False
```

### Comparing `goodai-ltm-0.0.5/goodai/ltm/memory_models/chunk_mixin.py` & `goodai-ltm-0.1.0/goodai/ltm/mem/chunk_mixin.py`

 * *Files identical despite different names*

### Comparing `goodai-ltm-0.0.5/goodai/ltm/memory_models/chunk_queue.py` & `goodai-ltm-0.1.0/goodai/ltm/mem/chunk_queue.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from abc import abstractmethod, ABC
 from typing import List, Tuple, Set, Dict, Optional, Any
 
-from goodai.ltm.memory_models.chunk import Chunk
-from goodai.ltm.memory_models.chunk_mixin import ChunkMixin
+from goodai.ltm.mem.chunk import Chunk
+from goodai.ltm.mem.chunk_mixin import ChunkMixin
 
 
 class BaseChunkQueue(ABC):
     """
     Abstract base class for text memory chunk queues.
     """
 
@@ -49,14 +49,22 @@
     def get_chunk_sequences(self) -> List[List[int]]:
         pass
 
     @abstractmethod
     def get_chunk(self, chunk_id: int) -> Chunk:
         pass
 
+    @abstractmethod
+    def get_all_chunks(self) -> List[Chunk]:
+        pass
+
+    @abstractmethod
+    def get_chunk_token_ids(self, chunk: Chunk):
+        pass
+
 
 class ChunkQueue(BaseChunkQueue, ChunkMixin):
     def __init__(self, queue_capacity: int, chunk_capacity: int, first_token_seq_id: int = 0):
         super().__init__()
         assert queue_capacity > 2, 'capacity cannot be 2 or less.'
         self.chunks: List[Chunk] = []
         self.capacity = queue_capacity
@@ -79,14 +87,17 @@
                 new_first_chunk = self.chunks[0]
                 new_first_token_seq_id = new_first_chunk.from_token_seq_id
                 num_removed = new_first_token_seq_id - self.first_token_seq_id
                 self.token_ids = self.token_ids[num_removed:]
                 self.first_token_seq_id = new_first_token_seq_id
         return chunk
 
+    def get_all_chunks(self) -> List[Chunk]:
+        return list(self.chunks)
+
     def check_overflow(self) -> List[Chunk]:
         removed_chunks = []
         while len(self.chunks) > self.capacity:
             removed_chunk = self._pop_chunk()
             if removed_chunk is not None:
                 removed_chunks.append(removed_chunk)
         return removed_chunks
```

### Comparing `goodai-ltm-0.0.5/goodai/ltm/memory_models/simple_vector_db.py` & `goodai-ltm-0.1.0/goodai/ltm/mem/simple_vector_db.py`

 * *Files 5% similar despite different names*

```diff
@@ -9,15 +9,25 @@
     """
 
     def __init__(self):
         super().__init__()
         self.all_vectors: Optional[np.ndarray] = None
         self.all_ids: Optional[np.ndarray] = None
 
-    def search(self, vectors: np.ndarray, k: int = 1) -> Tuple[np.ndarray, np.ndarray]:
+    def search(self, vectors: np.ndarray, k: int = 1, max_batch_size=256) -> Tuple[np.ndarray, np.ndarray]:
+        dist_list = []
+        idx_list = []
+        for b0 in range(0, vectors.shape[0], max_batch_size):
+            b_vectors = vectors[b0:b0 + max_batch_size]
+            b_dist, b_idx = self._search_direct(b_vectors, k=k)
+            dist_list.append(b_dist)
+            idx_list.append(b_idx)
+        return np.concatenate(dist_list), np.concatenate(idx_list),
+
+    def _search_direct(self, vectors: np.ndarray, k: int = 1) -> Tuple[np.ndarray, np.ndarray]:
         batch_size = vectors.shape[0]
         placeholder_dist = np.ones((batch_size, k)) * 1e+38
         placeholder_ids = -np.ones((batch_size, k), dtype=np.int64)
         if self.all_vectors is None:
             return placeholder_dist, placeholder_ids,
         # vectors: (n, emb_size,)
         # all_vectors: (m, emb_size,)
```

### Comparing `goodai-ltm-0.0.5/goodai/ltm/memory_models/tests/test_chunk_queue.py` & `goodai-ltm-0.1.0/goodai/ltm/mem/tests/test_chunk_queue.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import unittest
 
-from goodai.ltm.memory_models.chunk_queue import ChunkQueue
+from goodai.ltm.mem.chunk_queue import ChunkQueue
 
 
 class TestChunkQueue(unittest.TestCase):
     def test_insertion(self):
         seq_len = 8
         queue_capacity = 10
         num_seqs_in_chunk = 3
```

### Comparing `goodai-ltm-0.0.5/goodai/ltm/training/query_passage/trainer.py` & `goodai-ltm-0.1.0/goodai/ltm/training/query_passage/qppm_trainer.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,24 +10,28 @@
 
 from goodai.ltm.data.query_passage.auto_data_source import AutoQueryPassageDataSource
 from torch import nn
 from torch.utils.data import DataLoader, Dataset
 from transformers import PreTrainedTokenizer
 from timeit import default_timer as timer
 
-from goodai.ltm.matching_models.prob_model import BaseQueryPassageProbModel
-from goodai.ltm.training.sched_opt import ScheduledOptimizer
+from goodai.ltm.reranking.prob_model import BaseQueryPassageProbModel
+from goodai.helpers.sched_opt import ScheduledOptimizer
 
 
 class QPPMTrainer:
     def __init__(self, random: np.random.RandomState, tokenizer: PreTrainedTokenizer,
                  num_epochs: int, switch_ds_every: int, num_ds_examples: int, batch_size: int,
                  max_query_tokens: int, min_passage_tokens: int, max_passage_tokens: int,
-                 track_validation: bool, lm_lr: float, extras_lr: float, device: torch.device):
+                 track_validation: bool, lm_lr: float, extras_lr: float, device: torch.device,
+                 num_warmup_steps: int = 0, weight_decay: float = 1e-3, approx_positive_fraction: float = 0.5):
         super().__init__()
+        self.approx_positive_fraction = approx_positive_fraction
+        self.weight_decay = weight_decay
+        self.num_warmup_steps = num_warmup_steps
         self.extras_lr = extras_lr
         self.lm_lr = lm_lr
         self.max_passage_tokens = max_passage_tokens
         self.min_passage_tokens = min_passage_tokens
         self.max_query_tokens = max_query_tokens
         self.track_validation = track_validation
         self.batch_size = batch_size
@@ -106,15 +110,17 @@
             extra_parameters = model.get_added_parameters()
             num_training_steps = self.num_epochs * math.ceil(self.num_ds_examples / self.batch_size)
             parameters = [
                 {'params': lm_parameters, 'lr': self.lm_lr},
                 {'params': extra_parameters, 'lr': self.extras_lr},
             ]
             s_opt = ScheduledOptimizer(parameters, lr=self.lm_lr,
-                                       num_training_steps=num_training_steps)
+                                       num_training_steps=num_training_steps,
+                                       num_warmup_steps=self.num_warmup_steps,
+                                       weight_decay=self.weight_decay)
             sum_bp_time = 0
             time1 = timer()
             for epoch in range(0, self.num_epochs, self.switch_ds_every):
                 dataset = self.create_dataset(training=True)
                 train_loss, bp_time, _ = self.train_dataset(dataset, model, s_opt, validation=False)
                 sum_bp_time += bp_time
                 print(f'-- Epoch {epoch}: Train Loss={train_loss:.4g}')
@@ -134,8 +140,9 @@
             print(f'Training speed: {eph:.1f} epochs per hour.')
             torch.cuda.empty_cache()
             gc.collect()
 
     def create_dataset(self, training: bool):
         data_sources = self.train_data_sources if training else self.valid_data_sources
         return QueryPassageDataset(data_sources, self.tokenizer, self.num_ds_examples,
-                                   device=self.device)
+                                   device=self.device,
+                                   approx_positive_fraction=self.approx_positive_fraction)
```

### Comparing `goodai-ltm-0.0.5/goodai/ltm/training/sched_opt.py` & `goodai-ltm-0.1.0/goodai/helpers/sched_opt.py`

 * *Files identical despite different names*

### Comparing `goodai-ltm-0.0.5/goodai_ltm.egg-info/SOURCES.txt` & `goodai-ltm-0.1.0/goodai_ltm.egg-info/SOURCES.txt`

 * *Files 21% similar despite different names*

```diff
@@ -1,66 +1,78 @@
+LICENSE
 README.md
 setup.py
 goodai/helpers/__init__.py
 goodai/helpers/collections_helper.py
 goodai/helpers/file_helper.py
 goodai/helpers/html_helper.py
 goodai/helpers/json_helper.py
+goodai/helpers/sched_opt.py
 goodai/helpers/tokenizer_helper.py
 goodai/helpers/torch_helper.py
 goodai/ltm/__init__.py
-goodai/ltm/embeddings.py
-goodai/ltm/matching.py
-goodai/ltm/memory.py
+goodai/ltm/version.py
 goodai/ltm/data/__init__.py
 goodai/ltm/data/cloud.py
 goodai/ltm/data/names/__init__.py
+goodai/ltm/data/names/wikidata-names.json
 goodai/ltm/data/query_passage/__init__.py
 goodai/ltm/data/query_passage/auto_data_source.py
 goodai/ltm/data/query_passage/data_source.py
 goodai/ltm/data/query_passage/dataset.py
 goodai/ltm/data/query_passage/example.py
 goodai/ltm/data/query_passage/qa.py
 goodai/ltm/data/query_passage/qa_tok_entry.py
+goodai/ltm/data/query_passage/sharc.py
 goodai/ltm/data/query_passage/wiki.py
+goodai/ltm/data/query_passage/wikianswers.py
 goodai/ltm/data/query_passage/tests/__init__.py
 goodai/ltm/data/query_passage/tests/test_query_passage_data_source.py
-goodai/ltm/embedding_models/__init__.py
-goodai/ltm/embedding_models/auto.py
-goodai/ltm/embedding_models/contrast_classifier.py
-goodai/ltm/embedding_models/default.py
-goodai/ltm/embedding_models/emb_qp_prob_model.py
-goodai/ltm/embedding_models/openai_emb.py
-goodai/ltm/embedding_models/st_emb.py
-goodai/ltm/embedding_models/trainable.py
+goodai/ltm/embeddings/__init__.py
+goodai/ltm/embeddings/auto.py
+goodai/ltm/embeddings/base.py
+goodai/ltm/embeddings/contrast_classifier.py
+goodai/ltm/embeddings/default.py
+goodai/ltm/embeddings/emb_qp_prob_model.py
+goodai/ltm/embeddings/openai_emb.py
+goodai/ltm/embeddings/st_emb.py
+goodai/ltm/embeddings/trainable.py
 goodai/ltm/eval/__init__.py
 goodai/ltm/eval/auto.py
 goodai/ltm/eval/mem.py
 goodai/ltm/eval/metrics.py
+goodai/ltm/eval/msmarco.py
+goodai/ltm/eval/qp_ds.py
 goodai/ltm/eval/qrecc.py
 goodai/ltm/eval/strategy_qa.py
 goodai/ltm/eval/tests/test_metrics.py
-goodai/ltm/matching_models/__init__.py
-goodai/ltm/matching_models/auto.py
-goodai/ltm/matching_models/default.py
-goodai/ltm/matching_models/prob_model.py
-goodai/ltm/matching_models/st_ce.py
-goodai/ltm/memory_models/__init__.py
-goodai/ltm/memory_models/auto.py
-goodai/ltm/memory_models/chunk.py
-goodai/ltm/memory_models/chunk_mixin.py
-goodai/ltm/memory_models/chunk_queue.py
-goodai/ltm/memory_models/config.py
-goodai/ltm/memory_models/default.py
-goodai/ltm/memory_models/mem_foundation.py
-goodai/ltm/memory_models/simple_vector_db.py
-goodai/ltm/memory_models/tests/__init__.py
-goodai/ltm/memory_models/tests/test_chunk_queue.py
+goodai/ltm/mem/__init__.py
+goodai/ltm/mem/auto.py
+goodai/ltm/mem/base.py
+goodai/ltm/mem/chunk.py
+goodai/ltm/mem/chunk_mixin.py
+goodai/ltm/mem/chunk_queue.py
+goodai/ltm/mem/config.py
+goodai/ltm/mem/default.py
+goodai/ltm/mem/mem_foundation.py
+goodai/ltm/mem/rewrite_model.py
+goodai/ltm/mem/simple_vector_db.py
+goodai/ltm/mem/tests/__init__.py
+goodai/ltm/mem/tests/test_chunk_queue.py
+goodai/ltm/mem/tests/test_mem.py
+goodai/ltm/reranking/__init__.py
+goodai/ltm/reranking/auto.py
+goodai/ltm/reranking/base.py
+goodai/ltm/reranking/default.py
+goodai/ltm/reranking/emb.py
+goodai/ltm/reranking/prob_model.py
+goodai/ltm/reranking/st_ce.py
 goodai/ltm/training/__init__.py
-goodai/ltm/training/sched_opt.py
 goodai/ltm/training/query_passage/__init__.py
-goodai/ltm/training/query_passage/trainer.py
+goodai/ltm/training/query_passage/em_trainer.py
+goodai/ltm/training/query_passage/qppm_trainer.py
+goodai/modules/loss.py
 goodai_ltm.egg-info/PKG-INFO
 goodai_ltm.egg-info/SOURCES.txt
 goodai_ltm.egg-info/dependency_links.txt
 goodai_ltm.egg-info/requires.txt
 goodai_ltm.egg-info/top_level.txt
```

