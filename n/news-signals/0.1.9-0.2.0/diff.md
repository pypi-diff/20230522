# Comparing `tmp/news-signals-0.1.9.tar.gz` & `tmp/news-signals-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "news-signals-0.1.9.tar", last modified: Wed Mar 15 22:09:25 2023, max compression
+gzip compressed data, was "news-signals-0.2.0.tar", last modified: Sun May 21 22:29:08 2023, max compression
```

## Comparing `news-signals-0.1.9.tar` & `news-signals-0.2.0.tar`

### file list

```diff
@@ -1,78 +1,80 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 22:09:25.170960 news-signals-0.1.9/
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-03-15 22:09:15.000000 news-signals-0.1.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-03-15 22:09:15.000000 news-signals-0.1.9/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2134 2023-03-15 22:09:25.170960 news-signals-0.1.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1953 2023-03-15 22:09:15.000000 news-signals-0.1.9/README.md
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-03-15 22:09:15.000000 news-signals-0.1.9/VERSION
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 22:09:25.162960 news-signals-0.1.9/news_signals/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-15 22:09:15.000000 news-signals-0.1.9/news_signals/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2032 2023-03-15 22:09:15.000000 news-signals-0.1.9/news_signals/anomaly_detection.py
--rw-r--r--   0 runner    (1001) docker     (123)     6472 2023-03-15 22:09:15.000000 news-signals-0.1.9/news_signals/aql_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     1761 2023-03-15 22:09:15.000000 news-signals-0.1.9/news_signals/data.py
--rw-r--r--   0 runner    (1001) docker     (123)     1615 2023-03-15 22:09:15.000000 news-signals-0.1.9/news_signals/dataset_transformations.py
--rw-r--r--   0 runner    (1001) docker     (123)     4130 2023-03-15 22:09:15.000000 news-signals-0.1.9/news_signals/exogenous_signals.py
--rw-r--r--   0 runner    (1001) docker     (123)      434 2023-03-15 22:09:15.000000 news-signals-0.1.9/news_signals/log.py
--rw-r--r--   0 runner    (1001) docker     (123)     6084 2023-03-15 22:09:15.000000 news-signals-0.1.9/news_signals/newsapi.py
--rw-r--r--   0 runner    (1001) docker     (123)     2501 2023-03-15 22:09:15.000000 news-signals-0.1.9/news_signals/plotting.py
--rw-r--r--   0 runner    (1001) docker     (123)     3782 2023-03-15 22:09:15.000000 news-signals-0.1.9/news_signals/representative_story.py
--rw-r--r--   0 runner    (1001) docker     (123)    36759 2023-03-15 22:09:15.000000 news-signals-0.1.9/news_signals/signals.py
--rw-r--r--   0 runner    (1001) docker     (123)    15981 2023-03-15 22:09:15.000000 news-signals-0.1.9/news_signals/signals_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)    13060 2023-03-15 22:09:15.000000 news-signals-0.1.9/news_signals/summarization.py
--rw-r--r--   0 runner    (1001) docker     (123)     2119 2023-03-15 22:09:15.000000 news-signals-0.1.9/news_signals/test_anomaly_detection.py
--rw-r--r--   0 runner    (1001) docker     (123)     2543 2023-03-15 22:09:15.000000 news-signals-0.1.9/news_signals/test_aql_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)      677 2023-03-15 22:09:15.000000 news-signals-0.1.9/news_signals/test_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     3260 2023-03-15 22:09:15.000000 news-signals-0.1.9/news_signals/test_dataset_transformations.py
--rw-r--r--   0 runner    (1001) docker     (123)     2737 2023-03-15 22:09:15.000000 news-signals-0.1.9/news_signals/test_exogenous_signals.py
--rw-r--r--   0 runner    (1001) docker     (123)     3189 2023-03-15 22:09:15.000000 news-signals-0.1.9/news_signals/test_newsapi.py
--rw-r--r--   0 runner    (1001) docker     (123)     1826 2023-03-15 22:09:15.000000 news-signals-0.1.9/news_signals/test_representative_story.py
--rw-r--r--   0 runner    (1001) docker     (123)    22399 2023-03-15 22:09:15.000000 news-signals-0.1.9/news_signals/test_signals.py
--rw-r--r--   0 runner    (1001) docker     (123)     7575 2023-03-15 22:09:15.000000 news-signals-0.1.9/news_signals/test_signals_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     5543 2023-03-15 22:09:15.000000 news-signals-0.1.9/news_signals/test_summarization.py
--rw-r--r--   0 runner    (1001) docker     (123)     1687 2023-03-15 22:09:15.000000 news-signals-0.1.9/news_signals/yfinance_timeseries.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 22:09:25.162960 news-signals-0.1.9/news_signals.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2134 2023-03-15 22:09:25.000000 news-signals-0.1.9/news_signals.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4424 2023-03-15 22:09:25.000000 news-signals-0.1.9/news_signals.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-15 22:09:25.000000 news-signals-0.1.9/news_signals.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      235 2023-03-15 22:09:25.000000 news-signals-0.1.9/news_signals.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-03-15 22:09:25.000000 news-signals-0.1.9/news_signals.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 22:09:25.158960 news-signals-0.1.9/resources/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 22:09:25.166960 news-signals-0.1.9/resources/test/
--rw-r--r--   0 runner    (1001) docker     (123)    28512 2023-03-15 22:09:15.000000 news-signals-0.1.9/resources/test/elon_musk_timeseries.json
--rw-r--r--   0 runner    (1001) docker     (123)      205 2023-03-15 22:09:15.000000 news-signals-0.1.9/resources/test/nasdaq100.small.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 22:09:25.170960 news-signals-0.1.9/resources/test/nasdaq100_sample_dataset/
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-03-15 22:09:15.000000 news-signals-0.1.9/resources/test/nasdaq100_sample_dataset/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     3508 2023-03-15 22:09:15.000000 news-signals-0.1.9/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExMDI0NDU0IiwgIm1ldGFkYXRhIjoge319.df.parquet
--rw-r--r--   0 runner    (1001) docker     (123)      278 2023-03-15 22:09:15.000000 news-signals-0.1.9/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExMDI0NDU0IiwgIm1ldGFkYXRhIjoge319.static_fields.json
--rw-r--r--   0 runner    (1001) docker     (123)   110293 2023-03-15 22:09:15.000000 news-signals-0.1.9/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExMDI0NDU0IiwgIm1ldGFkYXRhIjoge319.stories_df.parquet
--rw-r--r--   0 runner    (1001) docker     (123)     3500 2023-03-15 22:09:15.000000 news-signals-0.1.9/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExMDU1MzkwIiwgIm1ldGFkYXRhIjoge319.df.parquet
--rw-r--r--   0 runner    (1001) docker     (123)      278 2023-03-15 22:09:15.000000 news-signals-0.1.9/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExMDU1MzkwIiwgIm1ldGFkYXRhIjoge319.static_fields.json
--rw-r--r--   0 runner    (1001) docker     (123)   113236 2023-03-15 22:09:15.000000 news-signals-0.1.9/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExMDU1MzkwIiwgIm1ldGFkYXRhIjoge319.stories_df.parquet
--rw-r--r--   0 runner    (1001) docker     (123)     3484 2023-03-15 22:09:15.000000 news-signals-0.1.9/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExMDkyNTcxIiwgIm1ldGFkYXRhIjoge319.df.parquet
--rw-r--r--   0 runner    (1001) docker     (123)      278 2023-03-15 22:09:15.000000 news-signals-0.1.9/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExMDkyNTcxIiwgIm1ldGFkYXRhIjoge319.static_fields.json
--rw-r--r--   0 runner    (1001) docker     (123)    90390 2023-03-15 22:09:15.000000 news-signals-0.1.9/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExMDkyNTcxIiwgIm1ldGFkYXRhIjoge319.stories_df.parquet
--rw-r--r--   0 runner    (1001) docker     (123)     3526 2023-03-15 22:09:15.000000 news-signals-0.1.9/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExMTQ2MyIsICJtZXRhZGF0YSI6IHt9fQ==.df.parquet
--rw-r--r--   0 runner    (1001) docker     (123)      272 2023-03-15 22:09:15.000000 news-signals-0.1.9/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExMTQ2MyIsICJtZXRhZGF0YSI6IHt9fQ==.static_fields.json
--rw-r--r--   0 runner    (1001) docker     (123)   131955 2023-03-15 22:09:15.000000 news-signals-0.1.9/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExMTQ2MyIsICJtZXRhZGF0YSI6IHt9fQ==.stories_df.parquet
--rw-r--r--   0 runner    (1001) docker     (123)     3494 2023-03-15 22:09:15.000000 news-signals-0.1.9/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExMTU1NjY4IiwgIm1ldGFkYXRhIjoge319.df.parquet
--rw-r--r--   0 runner    (1001) docker     (123)      278 2023-03-15 22:09:15.000000 news-signals-0.1.9/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExMTU1NjY4IiwgIm1ldGFkYXRhIjoge319.static_fields.json
--rw-r--r--   0 runner    (1001) docker     (123)   123388 2023-03-15 22:09:15.000000 news-signals-0.1.9/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExMTU1NjY4IiwgIm1ldGFkYXRhIjoge319.stories_df.parquet
--rw-r--r--   0 runner    (1001) docker     (123)     3494 2023-03-15 22:09:15.000000 news-signals-0.1.9/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExMzgzNjY5IiwgIm1ldGFkYXRhIjoge319.df.parquet
--rw-r--r--   0 runner    (1001) docker     (123)      278 2023-03-15 22:09:15.000000 news-signals-0.1.9/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExMzgzNjY5IiwgIm1ldGFkYXRhIjoge319.static_fields.json
--rw-r--r--   0 runner    (1001) docker     (123)   109117 2023-03-15 22:09:15.000000 news-signals-0.1.9/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExMzgzNjY5IiwgIm1ldGFkYXRhIjoge319.stories_df.parquet
--rw-r--r--   0 runner    (1001) docker     (123)     3496 2023-03-15 22:09:15.000000 news-signals-0.1.9/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExNDc3MiIsICJtZXRhZGF0YSI6IHt9fQ==.df.parquet
--rw-r--r--   0 runner    (1001) docker     (123)      272 2023-03-15 22:09:15.000000 news-signals-0.1.9/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExNDc3MiIsICJtZXRhZGF0YSI6IHt9fQ==.static_fields.json
--rw-r--r--   0 runner    (1001) docker     (123)    91683 2023-03-15 22:09:15.000000 news-signals-0.1.9/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExNDc3MiIsICJtZXRhZGF0YSI6IHt9fQ==.stories_df.parquet
--rw-r--r--   0 runner    (1001) docker     (123)     3494 2023-03-15 22:09:15.000000 news-signals-0.1.9/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExNTEwOTg2NSIsICJtZXRhZGF0YSI6IHt9fQ==.df.parquet
--rw-r--r--   0 runner    (1001) docker     (123)      281 2023-03-15 22:09:15.000000 news-signals-0.1.9/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExNTEwOTg2NSIsICJtZXRhZGF0YSI6IHt9fQ==.static_fields.json
--rw-r--r--   0 runner    (1001) docker     (123)    94002 2023-03-15 22:09:15.000000 news-signals-0.1.9/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExNTEwOTg2NSIsICJtZXRhZGF0YSI6IHt9fQ==.stories_df.parquet
--rw-r--r--   0 runner    (1001) docker     (123)     3465 2023-03-15 22:09:15.000000 news-signals-0.1.9/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExNTQ1MDc2IiwgIm1ldGFkYXRhIjoge319.df.parquet
--rw-r--r--   0 runner    (1001) docker     (123)      278 2023-03-15 22:09:15.000000 news-signals-0.1.9/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExNTQ1MDc2IiwgIm1ldGFkYXRhIjoge319.static_fields.json
--rw-r--r--   0 runner    (1001) docker     (123)   100871 2023-03-15 22:09:15.000000 news-signals-0.1.9/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExNTQ1MDc2IiwgIm1ldGFkYXRhIjoge319.stories_df.parquet
--rw-r--r--   0 runner    (1001) docker     (123)     3530 2023-03-15 22:09:15.000000 news-signals-0.1.9/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExNzA4MTYxMiIsICJtZXRhZGF0YSI6IHt9fQ==.df.parquet
--rw-r--r--   0 runner    (1001) docker     (123)      281 2023-03-15 22:09:15.000000 news-signals-0.1.9/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExNzA4MTYxMiIsICJtZXRhZGF0YSI6IHt9fQ==.static_fields.json
--rw-r--r--   0 runner    (1001) docker     (123)   135305 2023-03-15 22:09:15.000000 news-signals-0.1.9/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExNzA4MTYxMiIsICJtZXRhZGF0YSI6IHt9fQ==.stories_df.parquet
--rw-r--r--   0 runner    (1001) docker     (123)    28298 2023-03-15 22:09:15.000000 news-signals-0.1.9/resources/test/politics_china_australia_timeseries.json
--rw-r--r--   0 runner    (1001) docker     (123)   235658 2023-03-15 22:09:15.000000 news-signals-0.1.9/resources/test/sample_stories.json
--rw-r--r--   0 runner    (1001) docker     (123)   218541 2023-03-15 22:09:15.000000 news-signals-0.1.9/resources/test/tesla_stories.json
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-15 22:09:25.170960 news-signals-0.1.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1140 2023-03-15 22:09:15.000000 news-signals-0.1.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 22:29:08.288320 news-signals-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-05-21 22:28:54.000000 news-signals-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-05-21 22:28:54.000000 news-signals-0.2.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2691 2023-05-21 22:29:08.288320 news-signals-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2510 2023-05-21 22:28:54.000000 news-signals-0.2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-21 22:28:54.000000 news-signals-0.2.0/VERSION
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 22:29:08.280320 news-signals-0.2.0/news_signals/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-21 22:28:54.000000 news-signals-0.2.0/news_signals/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2032 2023-05-21 22:28:54.000000 news-signals-0.2.0/news_signals/anomaly_detection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6472 2023-05-21 22:28:54.000000 news-signals-0.2.0/news_signals/aql_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1761 2023-05-21 22:28:54.000000 news-signals-0.2.0/news_signals/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1773 2023-05-21 22:28:54.000000 news-signals-0.2.0/news_signals/dataset_transformations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4251 2023-05-21 22:28:54.000000 news-signals-0.2.0/news_signals/exogenous_signals.py
+-rw-r--r--   0 runner    (1001) docker     (123)      434 2023-05-21 22:28:54.000000 news-signals-0.2.0/news_signals/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6333 2023-05-21 22:28:54.000000 news-signals-0.2.0/news_signals/newsapi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2501 2023-05-21 22:28:54.000000 news-signals-0.2.0/news_signals/plotting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3782 2023-05-21 22:28:54.000000 news-signals-0.2.0/news_signals/representative_story.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38558 2023-05-21 22:28:54.000000 news-signals-0.2.0/news_signals/signals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16364 2023-05-21 22:28:54.000000 news-signals-0.2.0/news_signals/signals_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13060 2023-05-21 22:28:54.000000 news-signals-0.2.0/news_signals/summarization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2119 2023-05-21 22:28:54.000000 news-signals-0.2.0/news_signals/test_anomaly_detection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2543 2023-05-21 22:28:54.000000 news-signals-0.2.0/news_signals/test_aql_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)      677 2023-05-21 22:28:54.000000 news-signals-0.2.0/news_signals/test_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3260 2023-05-21 22:28:54.000000 news-signals-0.2.0/news_signals/test_dataset_transformations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2737 2023-05-21 22:28:54.000000 news-signals-0.2.0/news_signals/test_exogenous_signals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3189 2023-05-21 22:28:54.000000 news-signals-0.2.0/news_signals/test_newsapi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1826 2023-05-21 22:28:54.000000 news-signals-0.2.0/news_signals/test_representative_story.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23975 2023-05-21 22:28:54.000000 news-signals-0.2.0/news_signals/test_signals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7590 2023-05-21 22:28:54.000000 news-signals-0.2.0/news_signals/test_signals_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5543 2023-05-21 22:28:54.000000 news-signals-0.2.0/news_signals/test_summarization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6624 2023-05-21 22:28:54.000000 news-signals-0.2.0/news_signals/users.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1163 2023-05-21 22:28:54.000000 news-signals-0.2.0/news_signals/wikidata_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1687 2023-05-21 22:28:54.000000 news-signals-0.2.0/news_signals/yfinance_timeseries.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 22:29:08.280320 news-signals-0.2.0/news_signals.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2691 2023-05-21 22:29:08.000000 news-signals-0.2.0/news_signals.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4477 2023-05-21 22:29:08.000000 news-signals-0.2.0/news_signals.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-21 22:29:08.000000 news-signals-0.2.0/news_signals.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-05-21 22:29:08.000000 news-signals-0.2.0/news_signals.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-21 22:29:08.000000 news-signals-0.2.0/news_signals.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 22:29:08.276320 news-signals-0.2.0/resources/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 22:29:08.284320 news-signals-0.2.0/resources/test/
+-rw-r--r--   0 runner    (1001) docker     (123)    28512 2023-05-21 22:28:54.000000 news-signals-0.2.0/resources/test/elon_musk_timeseries.json
+-rw-r--r--   0 runner    (1001) docker     (123)      205 2023-05-21 22:28:54.000000 news-signals-0.2.0/resources/test/nasdaq100.small.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 22:29:08.288320 news-signals-0.2.0/resources/test/nasdaq100_sample_dataset/
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-05-21 22:28:54.000000 news-signals-0.2.0/resources/test/nasdaq100_sample_dataset/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3508 2023-05-21 22:28:54.000000 news-signals-0.2.0/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExMDI0NDU0IiwgIm1ldGFkYXRhIjoge319.df.parquet
+-rw-r--r--   0 runner    (1001) docker     (123)      278 2023-05-21 22:28:54.000000 news-signals-0.2.0/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExMDI0NDU0IiwgIm1ldGFkYXRhIjoge319.static_fields.json
+-rw-r--r--   0 runner    (1001) docker     (123)   110293 2023-05-21 22:28:54.000000 news-signals-0.2.0/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExMDI0NDU0IiwgIm1ldGFkYXRhIjoge319.stories_df.parquet
+-rw-r--r--   0 runner    (1001) docker     (123)     3500 2023-05-21 22:28:54.000000 news-signals-0.2.0/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExMDU1MzkwIiwgIm1ldGFkYXRhIjoge319.df.parquet
+-rw-r--r--   0 runner    (1001) docker     (123)      278 2023-05-21 22:28:54.000000 news-signals-0.2.0/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExMDU1MzkwIiwgIm1ldGFkYXRhIjoge319.static_fields.json
+-rw-r--r--   0 runner    (1001) docker     (123)   113236 2023-05-21 22:28:54.000000 news-signals-0.2.0/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExMDU1MzkwIiwgIm1ldGFkYXRhIjoge319.stories_df.parquet
+-rw-r--r--   0 runner    (1001) docker     (123)     3484 2023-05-21 22:28:54.000000 news-signals-0.2.0/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExMDkyNTcxIiwgIm1ldGFkYXRhIjoge319.df.parquet
+-rw-r--r--   0 runner    (1001) docker     (123)      278 2023-05-21 22:28:54.000000 news-signals-0.2.0/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExMDkyNTcxIiwgIm1ldGFkYXRhIjoge319.static_fields.json
+-rw-r--r--   0 runner    (1001) docker     (123)    90390 2023-05-21 22:28:54.000000 news-signals-0.2.0/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExMDkyNTcxIiwgIm1ldGFkYXRhIjoge319.stories_df.parquet
+-rw-r--r--   0 runner    (1001) docker     (123)     3526 2023-05-21 22:28:54.000000 news-signals-0.2.0/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExMTQ2MyIsICJtZXRhZGF0YSI6IHt9fQ==.df.parquet
+-rw-r--r--   0 runner    (1001) docker     (123)      272 2023-05-21 22:28:54.000000 news-signals-0.2.0/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExMTQ2MyIsICJtZXRhZGF0YSI6IHt9fQ==.static_fields.json
+-rw-r--r--   0 runner    (1001) docker     (123)   131955 2023-05-21 22:28:54.000000 news-signals-0.2.0/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExMTQ2MyIsICJtZXRhZGF0YSI6IHt9fQ==.stories_df.parquet
+-rw-r--r--   0 runner    (1001) docker     (123)     3494 2023-05-21 22:28:54.000000 news-signals-0.2.0/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExMTU1NjY4IiwgIm1ldGFkYXRhIjoge319.df.parquet
+-rw-r--r--   0 runner    (1001) docker     (123)      278 2023-05-21 22:28:54.000000 news-signals-0.2.0/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExMTU1NjY4IiwgIm1ldGFkYXRhIjoge319.static_fields.json
+-rw-r--r--   0 runner    (1001) docker     (123)   123388 2023-05-21 22:28:54.000000 news-signals-0.2.0/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExMTU1NjY4IiwgIm1ldGFkYXRhIjoge319.stories_df.parquet
+-rw-r--r--   0 runner    (1001) docker     (123)     3494 2023-05-21 22:28:54.000000 news-signals-0.2.0/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExMzgzNjY5IiwgIm1ldGFkYXRhIjoge319.df.parquet
+-rw-r--r--   0 runner    (1001) docker     (123)      278 2023-05-21 22:28:54.000000 news-signals-0.2.0/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExMzgzNjY5IiwgIm1ldGFkYXRhIjoge319.static_fields.json
+-rw-r--r--   0 runner    (1001) docker     (123)   109117 2023-05-21 22:28:54.000000 news-signals-0.2.0/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExMzgzNjY5IiwgIm1ldGFkYXRhIjoge319.stories_df.parquet
+-rw-r--r--   0 runner    (1001) docker     (123)     3496 2023-05-21 22:28:54.000000 news-signals-0.2.0/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExNDc3MiIsICJtZXRhZGF0YSI6IHt9fQ==.df.parquet
+-rw-r--r--   0 runner    (1001) docker     (123)      272 2023-05-21 22:28:54.000000 news-signals-0.2.0/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExNDc3MiIsICJtZXRhZGF0YSI6IHt9fQ==.static_fields.json
+-rw-r--r--   0 runner    (1001) docker     (123)    91683 2023-05-21 22:28:54.000000 news-signals-0.2.0/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExNDc3MiIsICJtZXRhZGF0YSI6IHt9fQ==.stories_df.parquet
+-rw-r--r--   0 runner    (1001) docker     (123)     3494 2023-05-21 22:28:54.000000 news-signals-0.2.0/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExNTEwOTg2NSIsICJtZXRhZGF0YSI6IHt9fQ==.df.parquet
+-rw-r--r--   0 runner    (1001) docker     (123)      281 2023-05-21 22:28:54.000000 news-signals-0.2.0/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExNTEwOTg2NSIsICJtZXRhZGF0YSI6IHt9fQ==.static_fields.json
+-rw-r--r--   0 runner    (1001) docker     (123)    94002 2023-05-21 22:28:54.000000 news-signals-0.2.0/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExNTEwOTg2NSIsICJtZXRhZGF0YSI6IHt9fQ==.stories_df.parquet
+-rw-r--r--   0 runner    (1001) docker     (123)     3465 2023-05-21 22:28:54.000000 news-signals-0.2.0/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExNTQ1MDc2IiwgIm1ldGFkYXRhIjoge319.df.parquet
+-rw-r--r--   0 runner    (1001) docker     (123)      278 2023-05-21 22:28:54.000000 news-signals-0.2.0/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExNTQ1MDc2IiwgIm1ldGFkYXRhIjoge319.static_fields.json
+-rw-r--r--   0 runner    (1001) docker     (123)   100871 2023-05-21 22:28:54.000000 news-signals-0.2.0/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExNTQ1MDc2IiwgIm1ldGFkYXRhIjoge319.stories_df.parquet
+-rw-r--r--   0 runner    (1001) docker     (123)     3530 2023-05-21 22:28:54.000000 news-signals-0.2.0/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExNzA4MTYxMiIsICJtZXRhZGF0YSI6IHt9fQ==.df.parquet
+-rw-r--r--   0 runner    (1001) docker     (123)      281 2023-05-21 22:28:54.000000 news-signals-0.2.0/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExNzA4MTYxMiIsICJtZXRhZGF0YSI6IHt9fQ==.static_fields.json
+-rw-r--r--   0 runner    (1001) docker     (123)   135305 2023-05-21 22:28:54.000000 news-signals-0.2.0/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExNzA4MTYxMiIsICJtZXRhZGF0YSI6IHt9fQ==.stories_df.parquet
+-rw-r--r--   0 runner    (1001) docker     (123)    28298 2023-05-21 22:28:54.000000 news-signals-0.2.0/resources/test/politics_china_australia_timeseries.json
+-rw-r--r--   0 runner    (1001) docker     (123)   235658 2023-05-21 22:28:54.000000 news-signals-0.2.0/resources/test/sample_stories.json
+-rw-r--r--   0 runner    (1001) docker     (123)   218541 2023-05-21 22:28:54.000000 news-signals-0.2.0/resources/test/tesla_stories.json
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-21 22:29:08.288320 news-signals-0.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1140 2023-05-21 22:28:54.000000 news-signals-0.2.0/setup.py
```

### Comparing `news-signals-0.1.9/LICENSE` & `news-signals-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `news-signals-0.1.9/news_signals/anomaly_detection.py` & `news-signals-0.2.0/news_signals/anomaly_detection.py`

 * *Files identical despite different names*

### Comparing `news-signals-0.1.9/news_signals/aql_builder.py` & `news-signals-0.2.0/news_signals/aql_builder.py`

 * *Files identical despite different names*

### Comparing `news-signals-0.1.9/news_signals/data.py` & `news-signals-0.2.0/news_signals/data.py`

 * *Files identical despite different names*

### Comparing `news-signals-0.1.9/news_signals/dataset_transformations.py` & `news-signals-0.2.0/news_signals/dataset_transformations.py`

 * *Files 13% similar despite different names*

```diff
@@ -50,13 +50,20 @@
             wikimedia_endpoint=wikimedia_endpoint,
             overwrite_existing=overwrite_existing
         )
     dataset.map(transform)
     return dataset
 
 
+REGISTRY = {
+    "add_anomalies": add_anomalies,
+    "add_summaries": add_summaries,
+    "add_wikimedia_pageviews": add_wikimedia_pageviews
+}
+
+
 def get_dataset_transform(func_name):
     try:
-        func = globals()[func_name]
-    except:
+        func = REGISTRY[func_name]
+    except KeyError as _:
         raise NotImplementedError(f'Unknown transformation function: {func_name}')
-    return func
+    return func
```

### Comparing `news-signals-0.1.9/news_signals/exogenous_signals.py` & `news-signals-0.2.0/news_signals/exogenous_signals.py`

 * *Files 4% similar despite different names*

```diff
@@ -96,15 +96,15 @@
     if client is None:
         client = WikidataClient()
     url = None
     try:
         entity_data = client(wikidata_id)
         url = entity_data['sitelinks']['enwiki']['url']
     except KeyError:
-        logger.error(f'Error: no wikipedia url found for entity data: {entity.data}')
+        logger.error(f'Error: no wikipedia url found for entity data: {entity_data}')
     except urllib.error.HTTPError as e:
         logger.error(f'Error retrieving wikidata entity: {wikidata_id}')    
     return url
 
 
 def wikimedia_pageviews_timeseries_from_wikipedia_link(
     wikipedia_link: str,
@@ -119,25 +119,27 @@
     Requests pageviews timeseries of a Wikipedia page for a given time range from Wikimedia API.
     """
     if endpoint is None:
         endpoint = RequestsEndpoint()
 
     url_date_format = "%Y%m%d00"
     assert granularity in ["daily", "monthly"]
-    start = start.strftime(url_date_format)
-    end = end.strftime(url_date_format)
+    start_ = start.strftime(url_date_format)
+    end_ = end.strftime(url_date_format)
     page_name = wikipedia_link.split("/")[-1]
-    url = f"https://wikimedia.org/api/rest_v1/metrics/pageviews/per-article/{language}.wikipedia/all-access/all-agents/{page_name}/{granularity}/{start}/{end}"
+    url = f"https://wikimedia.org/api/rest_v1/metrics/pageviews/per-article/{language}.wikipedia/all-access/all-agents/{page_name}/{granularity}/{start_}/{end_}"
     df = None
     try:
         response = endpoint(url, headers=wikimedia_headers)        
         records = [
             {
                 "wikimedia_pageviews": item["views"],
                 "timestamp": datetime.datetime.strptime(item["timestamp"], url_date_format)
             }
             for item in response["items"]
         ]
         df = ts_records_to_ts_df(records)
+        date_range = pd.date_range(start=start, end=end, freq="D")
+        df = df.reindex(date_range, fill_value=0)
     except KeyError:
         logger.error(response)
     return df
```

### Comparing `news-signals-0.1.9/news_signals/newsapi.py` & `news-signals-0.2.0/news_signals/newsapi.py`

 * *Files 2% similar despite different names*

```diff
@@ -82,16 +82,20 @@
             time.sleep(wait_seconds)
         except CONNECTION_ERRORS as e:
             logger.info(
                 f"Connection error: {e}. "
                 f" Waiting {wait_seconds} seconds. Trial: {i}/{trials}"
             )
             time.sleep(wait_seconds)
+        except json.decoder.JSONDecodeError as e:
+            logger.error(f"exception from decoding this json: {response.text}")            
+            logger.error(f"status code: {response.status_code}, retrying")
+            time.sleep(wait_seconds)
         except Exception as e:
-            logger.error("uncaught exception validating request: {e}")
+            logger.error("uncaught exception validating request")
             raise e
 
 
 def validate_newsapi_response(endpoint, data):
     if "errors" in data and len(data["errors"]) > 0:
         if data["errors"][0]["status"] == 429:
             raise TooManyRequestsError
```

### Comparing `news-signals-0.1.9/news_signals/plotting.py` & `news-signals-0.2.0/news_signals/plotting.py`

 * *Files identical despite different names*

### Comparing `news-signals-0.1.9/news_signals/representative_story.py` & `news-signals-0.2.0/news_signals/representative_story.py`

 * *Files identical despite different names*

### Comparing `news-signals-0.1.9/news_signals/signals.py` & `news-signals-0.2.0/news_signals/signals.py`

 * *Files 2% similar despite different names*

```diff
@@ -128,14 +128,22 @@
                 how='left'
             )
 
         # static metadata about the signal
         df['signal_name'] = self.name
         df['freq'] = self.infer_freq()
         return df
+    
+    @property
+    def start(self):
+        return self.df.index.min()
+
+    @property
+    def end(self):
+        return self.df.index.max()
 
     @abstractmethod
     def inputs(self):
         """
         return the inputs to this signal
         this let us easily traverse the signal graph
         to give insight into the path that a signal takes
@@ -186,22 +194,29 @@
             return self.timeseries_df[self.ts_column]
         else:
             raise NotImplementedError(
                 'to_series() is not implemented for this signal type'
             )
 
     def infer_freq(self):
-        if getattr(self, 'timeseries_df', None) is not None:
-            return pd.infer_freq(self.timeseries_df.index)
-        elif getattr(self, 'feeds_df', None) is not None:
-            return pd.infer_freq(self.feeds_df.index)
-        else:
-            raise NotImplementedError(
-                'infer_freq() is not implemented for this signal type'
+        try:
+            if getattr(self, 'timeseries_df', None) is not None:
+                return pd.infer_freq(self.timeseries_df.index)
+            elif getattr(self, 'feeds_df', None) is not None:
+                return pd.infer_freq(self.feeds_df.index)
+            else:
+                raise NotImplementedError(
+                    'infer_freq() is not implemented for this signal type'
+                )
+        except ValueError as e:
+            logger.warning(
+                f'Could not infer frequency for signal {self.name}, '
+                'this may be because the signal has no data, returning default freq = \'D\''
             )
+            return 'D'
 
     def significant_windows(
             self, min_value=1., min_delta=3, window_range=1,
             format='datetime', normalize_weights=True
     ):
         freq = self.infer_freq()
         freq_attr = 'days'
@@ -277,24 +292,21 @@
         """
         Anomaly detection methods expect a minimum amount of history,
         or function is not idempotent wrt dates (same date will have different scores
         over time)
 
         Anomaly detection methods have a threshold
         For aggregate signals, we may sometimes want to set _different_ thresholds
-        for each anomaly signal
 
-        :param: history_length: history length
-        :param: history_interval: history interval (months, days, hours, ...)
         """
 
         # if user didn't supply start and end, we want signal to have enough data that 
         # we can take the first part and use it to compute necessary stats to do the 
         # anomaly transformation on the rest of the signal
-        if not overwrite_existing and 'anomalies' in self.timeseries_df.columns:
+        if not overwrite_existing and self.timeseries_df is not None and 'anomalies' in self.timeseries_df.columns:
             return self
             
         if start is None:
             ts_begin = self.timeseries_df.index.min()
             ts_end = self.timeseries_df.index.max()
             dates = self.date_range(ts_begin, ts_end)
             if freq == 'D' and len(dates) > 2:
@@ -409,45 +421,58 @@
         static_fields = {
             k: v
             for k, v in signal_dict.items()
             if type(v) is not pd.DataFrame
         }
         # make type json serializable
         static_fields['type'] = type(self).__name__
-        with open(datadir / f'{signal_id}.static_fields.json', 'w') as out:
+        signal_config_file = datadir / f'{signal_id}.static_fields.json'
+        with open(signal_config_file, 'w') as out:
             out.write(json.dumps(static_fields, indent=2))
 
         # "time indexed columns" are ones that are in dfs in the original signal
         for k, v in signal_dict.items():
             if type(v) is pd.DataFrame:
                 v.to_parquet(datadir / f'{signal_id}.{k}.parquet', index=True)
-
+        return signal_config_file
+    
     @staticmethod
-    def load(signals_path):
+    def load_from_signal_config(signal_config_path):
+        signal_config_path = Path(signal_config_path)
+        assert signal_config_path.is_file(), f'signal config {signal_config_path} not found'
+        with open(signal_config_path) as f:
+            signal_config = json.load(f)
+        signal_id = str(signal_config_path.name).split('.')[0]
+        # load signal dataframes from parquet files
+        parent_dir = signal_config_path.parent
+        df_paths = [p.name for p in parent_dir.glob(f'{signal_id}.*.parquet')]
+        for df_path in df_paths:
+            df_key = str(df_path).split('.')[1]
+            df = pd.read_parquet(parent_dir / df_path)
+            # if the df index is not already datetime64, cast it
+            if not df.index.inferred_type == "datetime64":
+                df.index = pd.to_datetime(df.index)
+            signal_config[df_key] = df
+        return Signal.from_dict(signal_config)
 
-        signals_dir = Path(signals_path)
-        assert os.path.isdir(signals_dir), 'Signals load paths must be directories'
-
-        static_config_paths = signals_dir.glob('*.static_fields.json')
-        signals = []
-        for signal_config_path in static_config_paths:
-            with open(signal_config_path) as f:
-                signal_config = json.load(f)
-            signal_id = str(signal_config_path.name).split('.')[0]
-            # load signal dataframes from parquet files
-            df_paths = [p.name for p in signals_dir.glob(f'{signal_id}.*.parquet')]
-            for df_path in df_paths:
-                df_key = str(df_path).split('.')[1]
-                df = pd.read_parquet(signals_dir / df_path)
-                # if the df index is not already datetime64, cast it
-                if not df.index.inferred_type == "datetime64":
-                    df.index = pd.to_datetime(df.index)
-                signal_config[df_key] = df
-            signals.append(Signal.from_dict(signal_config))            
-        return signals
+    @staticmethod
+    def load(signals_path):        
+        signals_path = Path(signals_path)
+        if os.path.isdir(signals_path):
+            signals_dir = Path(signals_path)
+
+            static_config_paths = signals_dir.glob('*.static_fields.json')
+            signals = []
+            for signal_config_path in static_config_paths:
+                signals.append(Signal.load_from_signal_config(signal_config_path))            
+            return signals
+        else:
+            assert str(signals_path).endswith('.static_fields.json'), f'expected a static_fields.json file, got {signals_path}'
+            assert signals_path.is_file(), f'signal config {signals_path} not found'
+            return Signal.load_from_signal_config(signals_path)
 
     @property
     def id(self):
         """
         Generate a unique id for this signal
         by leveraging the `name` and `metadata` fields, the user
         can control how the id is generated, and thus control the equality
@@ -470,14 +495,21 @@
     
     @property
     def end(self):
         """
         Return the start timestamp of the signal
         """
         return self.timeseries_df.index.max()
+    
+    @property
+    def freq(self):
+        """
+        Return the frequency of the signal
+        """
+        return pd.infer_freq(self.timeseries_df.index)
 
 
 class DataframeSignal(Signal):
     """
     Holds static data in a dataframe with a datetime index
     """
     def __init__(
@@ -620,15 +652,14 @@
             # on Aylien timeseries
             raise UnknownFrequencyArgument
 
         self.update(start=start, end=end, freq=freq)
 
         return self
 
-
     @staticmethod
     def pd_freq_to_aylien_period(freq):
         if freq == 'D':
             return '+1DAY'
         elif freq == 'H':
             return '+1HOUR'
         else:
@@ -719,24 +750,36 @@
 
     def create_aylien_dataset(self, start, end):
         _ = self.__call__(start, end)
         _ = self.sample_stories_in_window(
             start, end, sample_per_tick=True
         )
         return self.to_dict()
+    
+    def sample_stories(self, num_stories=10, **kwargs):
+        """
+        sample stories for every tick of this signal
+        """
+        self.sample_stories_in_window(
+            self.start, self.end,
+            sample_per_tick=True, freq=self.freq, num_stories=num_stories,
+            **kwargs
+        )
+        return self
 
     @staticmethod
     def normalize_aylien_story(story):
         """
         stories is a list of dicts, each dict is a story
         """
         # this is needed because arrow cannot serialize empty dicts
-        for e in story['entities']:
-            if 'external_ids' in e and len(e['external_ids']) == 0:
-                del e['external_ids']
+        if 'entities' in story:
+            for e in story['entities']:
+                if 'external_ids' in e and len(e['external_ids']) == 0:
+                    del e['external_ids']
         return story
 
     def sample_stories_in_window(self, start, end,
                                  num_stories=20,
                                  sample_per_tick=True,
                                  overwrite_existing=False,
                                  stories_column='stories',
@@ -758,24 +801,30 @@
                 index=pd.DatetimeIndex(date_range[:-1], tz='UTC')
             )
         
         if sample_per_tick:
             date_range = self.date_range(start, end)
             start_end_tups = [(s, e) for s, e in zip(list(date_range), list(date_range)[1:])]
             for start, end in tqdm.tqdm(start_end_tups):
-                # note we check if the type is a list instead of pd.isna because
-                # the polymorphic .isna check in pandas is weird
-                if type(self.feeds_df.loc[start][stories_column]) is list and not overwrite_existing:
-                    logger.info(f'Already have stories for {start} to {end}')
-                    continue
-                else:
-                    logger.info(f'Getting stories for {start} to {end}')
-                    params = self.make_query(start, end)
-                    stories = [self.normalize_aylien_story(s) for s in self.stories_endpoint(params)]
-                    story_bucket_records.append({'timestamp': start, stories_column: stories})
+                # Note the polymorphic .isnull check from pandas won't work with arrays, thus try/except
+                if not overwrite_existing:
+                    try:
+                        current_value = self.feeds_df.loc[start][stories_column]
+                        # nans will be floats
+                        if not type(current_value) is float:
+                            if len(current_value) > 0:
+                                raise ValueError
+                    except ValueError:
+                        logger.info(f'Already have stories for {start} to {end}')
+                        continue
+                
+                logger.info(f'Getting stories for {start} to {end}')
+                params = self.make_query(start, end)
+                stories = [self.normalize_aylien_story(s) for s in self.stories_endpoint(params)]
+                story_bucket_records.append({'timestamp': start, stories_column: stories})
         else:
             params = self.make_query(start, end)
             stories = [self.normalize_aylien_story(s) for s in self.stories_endpoint(params)]
             records = defaultdict(list)
             for story in stories:
                 ts = self.normalize_timestamp(story['published_at'], freq)
                 records[ts].append(story)
```

### Comparing `news-signals-0.1.9/news_signals/signals_dataset.py` & `news-signals-0.2.0/news_signals/signals_dataset.py`

 * *Files 1% similar despite different names*

```diff
@@ -118,15 +118,15 @@
         return cls(
             signals=dataset_signals,
             metadata=metadata
         )
 
     def save(self, dataset_path, compress=True, overwrite=False):
         dataset_path = Path(dataset_path)
-        if overwrite and not dataset_path.is_dir():
+        if (overwrite and dataset_path.exists()) and not dataset_path.is_dir():
             dataset_path.unlink()
         dataset_path.mkdir(parents=True, exist_ok=overwrite)
         for signal in self.signals.values():
             signal.save(dataset_path)
         write_json(
             self.metadata,
             dataset_path / 'metadata.json'
@@ -134,15 +134,16 @@
         if compress:
             shutil.make_archive(
                 base_name=dataset_path,
                 format='gztar',
                 root_dir=dataset_path.parent,
                 base_dir=dataset_path.name
             )
-            shutil.rmtree(dataset_path)
+            if dataset_path.exists():
+                shutil.rmtree(dataset_path)
             logger.info(f'Saved compressed dataset to {dataset_path}.tar.gz')
             return f'{dataset_path}.tar.gz'
         else:
             logger.info(
                 f'Saved {len(self.signals)} signals in dataset to {dataset_path}.'
             )
             return dataset_path
@@ -414,20 +415,20 @@
     name_field: str = "",
     stories_per_day: int = 20,
     overwrite: bool = False,
     delete_tmp_files: bool = False,
     stories_endpoint=newsapi.retrieve_stories,
     ts_endpoint=newsapi.retrieve_timeseries,
     post_process_story=None,
+    compress=True,
 ):
 
     """
     Turn list of signals into a dataset by populating each signal with time
     series and stories using Aylien Newsapi endpoints.
-    The dataset is stored in an SqliteDict database.
     """
 
     if isinstance(input, Path):
         # this CSV should have a Wikidata ID and name for each entity
         df = pd.read_csv(input)
         signals_ = []
         for x in df.to_dict(orient="records"):
@@ -471,34 +472,43 @@
 
         # TODO: pick a surface form vs. ID, or both
         params = signal.params
 
         # we save TS and stories to make continuation of the 
         # dataset generation process easier if it gets interrupted
         # by an error.
+        logger.info("retrieving time series")
         ts = retrieve_and_write_timeseries(
             params, start, end, ts_path,
             ts_endpoint=ts_endpoint
         )
+        logger.info("retrieving stories")
         retrieve_and_write_stories(
             params,
             start, end,
             ts,
             stories_path,
             num_stories=stories_per_day,
             stories_endpoint=stories_endpoint,
             post_process_story=post_process_story
         )
 
         # now this signal is completely realized
         stories_df = df_from_jsonl_buckets(stories_path)
-        ts_df = aylien_ts_to_df({"time_series": ts}, dt_index=True)        
+        ts_df = aylien_ts_to_df({"time_series": ts}, dt_index=True)
         signal.timeseries_df = ts_df
         signal.feeds_df = stories_df
+        logger.info(f"saving signal: {signal.name}")
         signal.save(output_dataset_dir)
+        # clear memory
+        del signal.feeds_df, signal.timeseries_df
 
         # delete temporary files
         if delete_tmp_files:
             ts_path.unlink()
             stories_path.unlink()
 
-    return SignalsDataset.load(output_dataset_dir)
+    dataset = SignalsDataset.load(output_dataset_dir)
+    if compress:
+        shutil.rmtree(output_dataset_dir)
+        dataset.save(output_dataset_dir, compress=compress)
+    return dataset
```

### Comparing `news-signals-0.1.9/news_signals/summarization.py` & `news-signals-0.2.0/news_signals/summarization.py`

 * *Files identical despite different names*

### Comparing `news-signals-0.1.9/news_signals/test_anomaly_detection.py` & `news-signals-0.2.0/news_signals/test_anomaly_detection.py`

 * *Files identical despite different names*

### Comparing `news-signals-0.1.9/news_signals/test_aql_builder.py` & `news-signals-0.2.0/news_signals/test_aql_builder.py`

 * *Files identical despite different names*

### Comparing `news-signals-0.1.9/news_signals/test_data.py` & `news-signals-0.2.0/news_signals/test_data.py`

 * *Files identical despite different names*

### Comparing `news-signals-0.1.9/news_signals/test_dataset_transformations.py` & `news-signals-0.2.0/news_signals/test_dataset_transformations.py`

 * *Files identical despite different names*

### Comparing `news-signals-0.1.9/news_signals/test_exogenous_signals.py` & `news-signals-0.2.0/news_signals/test_exogenous_signals.py`

 * *Files identical despite different names*

### Comparing `news-signals-0.1.9/news_signals/test_newsapi.py` & `news-signals-0.2.0/news_signals/test_newsapi.py`

 * *Files identical despite different names*

### Comparing `news-signals-0.1.9/news_signals/test_representative_story.py` & `news-signals-0.2.0/news_signals/test_representative_story.py`

 * *Files identical despite different names*

### Comparing `news-signals-0.1.9/news_signals/test_signals.py` & `news-signals-0.2.0/news_signals/test_signals.py`

 * *Files 5% similar despite different names*

```diff
@@ -99,14 +99,28 @@
         """
         signal = self.aylien_signals()[0]
         start = '1971-01-01'
         end = '1971-01-31'
         # these dates aren't cached on the signal
         df = signal[start:end]
         assert len(df) == 0
+
+    def test_signal_start_end_properties(self):
+        """
+        Test that we can get the start and end dates of a signal
+        """
+        signal = self.aylien_signals()[0]
+        assert len(signal.date_range(signal.start, signal.end)) == len(signal) == len(signal.df)
+
+    def test_freq_property(self):
+        """
+        Test that we can access the frequency of a signal
+        """
+        signal = self.aylien_signals()[0]
+        assert signal.freq == 'D'
     
 
 class TestDataframeSignal(SignalTest):
 
     def test_datetime_index(self):
         """
         Test DataframeSignals index type
@@ -390,14 +404,41 @@
             start, end,
             sample_per_tick=True
         )
         date_range = signals.Signal.date_range(start, end)
         assert all(len(s) == stories_per_tick for s in signal_with_stories.feeds_df['stories'] if type(s) is list)
         assert len(signal_with_stories) == len(date_range) - 1
 
+    def test_sampling_stories_for_all_ticks(self):
+        signal = self.aylien_signals()[0]
+        # dynamically set mock endpoint payload
+        stories_per_tick = 3
+        payload = {
+            'stories': [
+                {'title': 'title', 'body': 'body', 'published_at': '2021-08-02T01:05:00Z'}
+                for _ in range(stories_per_tick)
+            ]
+        }
+        signal.params = payload
+
+        # we should already have stories for most ticks
+        # so the endpoint should not be called for most ticks
+        num_ticks_without_stories = len([s for s in signal.df['stories'] if len(s) == 0])
+        stories_endpoint_mock = MockEndpoint()
+        signal.stories_endpoint = stories_endpoint_mock
+        _ = signal.sample_stories()
+        assert stories_endpoint_mock.num_calls == num_ticks_without_stories
+
+        # reset mock endpoint
+        stories_endpoint_mock.num_calls = 0
+
+        _ = signal.sample_stories(overwrite_existing=True)
+        assert stories_endpoint_mock.num_calls == \
+            len(signal.date_range(signal.start, signal.end, freq=signal.freq)) - 1
+
     def test_summarize(self):
         signal, _, _, stories = self.setup_summarization_tests()
         summarizer = summarization.CentralTitleSummarizer()
         raw_summary = summarizer(stories)
         # note cache flag is set to True
         signal_summaries = signal.summarize(
             summarizer, cache_summaries=True
```

### Comparing `news-signals-0.1.9/news_signals/test_signals_dataset.py` & `news-signals-0.2.0/news_signals/test_signals_dataset.py`

 * *Files 1% similar despite different names*

```diff
@@ -102,15 +102,16 @@
             output_dataset_dir=Path(self.output_dataset_dir),
             start=datetime.datetime(2023, 1, 1),
             end=datetime.datetime(2023, 1, 4),
             id_field="Wikidata ID",
             name_field="Wikidata Label",
             delete_tmp_files=True,
             stories_endpoint=self.stories_endpoint,
-            ts_endpoint=self.ts_endpoint,            
+            ts_endpoint=self.ts_endpoint,
+            compress=False
         )
 
     def test_generate_dataset(self):
         self.generate_sample_dataset()
 
         signals_ = signals_dataset.SignalsDataset.load(
             self.output_dataset_dir
```

### Comparing `news-signals-0.1.9/news_signals/test_summarization.py` & `news-signals-0.2.0/news_signals/test_summarization.py`

 * *Files identical despite different names*

### Comparing `news-signals-0.1.9/news_signals/yfinance_timeseries.py` & `news-signals-0.2.0/news_signals/yfinance_timeseries.py`

 * *Files identical despite different names*

### Comparing `news-signals-0.1.9/news_signals.egg-info/SOURCES.txt` & `news-signals-0.2.0/news_signals.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -22,14 +22,16 @@
 news_signals/test_dataset_transformations.py
 news_signals/test_exogenous_signals.py
 news_signals/test_newsapi.py
 news_signals/test_representative_story.py
 news_signals/test_signals.py
 news_signals/test_signals_dataset.py
 news_signals/test_summarization.py
+news_signals/users.py
+news_signals/wikidata_utils.py
 news_signals/yfinance_timeseries.py
 news_signals.egg-info/PKG-INFO
 news_signals.egg-info/SOURCES.txt
 news_signals.egg-info/dependency_links.txt
 news_signals.egg-info/requires.txt
 news_signals.egg-info/top_level.txt
 resources/test/elon_musk_timeseries.json
```

### Comparing `news-signals-0.1.9/resources/test/elon_musk_timeseries.json` & `news-signals-0.2.0/resources/test/elon_musk_timeseries.json`

 * *Files identical despite different names*

### Comparing `news-signals-0.1.9/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExMDI0NDU0IiwgIm1ldGFkYXRhIjoge319.df.parquet` & `news-signals-0.2.0/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExMDI0NDU0IiwgIm1ldGFkYXRhIjoge319.df.parquet`

 * *Files identical despite different names*

### Comparing `news-signals-0.1.9/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExMDI0NDU0IiwgIm1ldGFkYXRhIjoge319.stories_df.parquet` & `news-signals-0.2.0/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExMDI0NDU0IiwgIm1ldGFkYXRhIjoge319.stories_df.parquet`

 * *Files identical despite different names*

### Comparing `news-signals-0.1.9/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExMDU1MzkwIiwgIm1ldGFkYXRhIjoge319.df.parquet` & `news-signals-0.2.0/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExMDU1MzkwIiwgIm1ldGFkYXRhIjoge319.df.parquet`

 * *Files identical despite different names*

### Comparing `news-signals-0.1.9/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExMDU1MzkwIiwgIm1ldGFkYXRhIjoge319.stories_df.parquet` & `news-signals-0.2.0/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExMDU1MzkwIiwgIm1ldGFkYXRhIjoge319.stories_df.parquet`

 * *Files identical despite different names*

### Comparing `news-signals-0.1.9/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExMDkyNTcxIiwgIm1ldGFkYXRhIjoge319.df.parquet` & `news-signals-0.2.0/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExMDkyNTcxIiwgIm1ldGFkYXRhIjoge319.df.parquet`

 * *Files identical despite different names*

### Comparing `news-signals-0.1.9/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExMDkyNTcxIiwgIm1ldGFkYXRhIjoge319.stories_df.parquet` & `news-signals-0.2.0/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExMDkyNTcxIiwgIm1ldGFkYXRhIjoge319.stories_df.parquet`

 * *Files identical despite different names*

### Comparing `news-signals-0.1.9/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExMTQ2MyIsICJtZXRhZGF0YSI6IHt9fQ==.df.parquet` & `news-signals-0.2.0/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExMTQ2MyIsICJtZXRhZGF0YSI6IHt9fQ==.df.parquet`

 * *Files identical despite different names*

### Comparing `news-signals-0.1.9/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExMTQ2MyIsICJtZXRhZGF0YSI6IHt9fQ==.stories_df.parquet` & `news-signals-0.2.0/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExMTQ2MyIsICJtZXRhZGF0YSI6IHt9fQ==.stories_df.parquet`

 * *Files identical despite different names*

### Comparing `news-signals-0.1.9/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExMTU1NjY4IiwgIm1ldGFkYXRhIjoge319.df.parquet` & `news-signals-0.2.0/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExMTU1NjY4IiwgIm1ldGFkYXRhIjoge319.df.parquet`

 * *Files identical despite different names*

### Comparing `news-signals-0.1.9/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExMTU1NjY4IiwgIm1ldGFkYXRhIjoge319.stories_df.parquet` & `news-signals-0.2.0/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExMTU1NjY4IiwgIm1ldGFkYXRhIjoge319.stories_df.parquet`

 * *Files identical despite different names*

### Comparing `news-signals-0.1.9/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExMzgzNjY5IiwgIm1ldGFkYXRhIjoge319.df.parquet` & `news-signals-0.2.0/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExMzgzNjY5IiwgIm1ldGFkYXRhIjoge319.df.parquet`

 * *Files identical despite different names*

### Comparing `news-signals-0.1.9/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExMzgzNjY5IiwgIm1ldGFkYXRhIjoge319.stories_df.parquet` & `news-signals-0.2.0/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExMzgzNjY5IiwgIm1ldGFkYXRhIjoge319.stories_df.parquet`

 * *Files identical despite different names*

### Comparing `news-signals-0.1.9/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExNDc3MiIsICJtZXRhZGF0YSI6IHt9fQ==.df.parquet` & `news-signals-0.2.0/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExNDc3MiIsICJtZXRhZGF0YSI6IHt9fQ==.df.parquet`

 * *Files identical despite different names*

### Comparing `news-signals-0.1.9/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExNDc3MiIsICJtZXRhZGF0YSI6IHt9fQ==.stories_df.parquet` & `news-signals-0.2.0/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExNDc3MiIsICJtZXRhZGF0YSI6IHt9fQ==.stories_df.parquet`

 * *Files identical despite different names*

### Comparing `news-signals-0.1.9/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExNTEwOTg2NSIsICJtZXRhZGF0YSI6IHt9fQ==.df.parquet` & `news-signals-0.2.0/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExNTEwOTg2NSIsICJtZXRhZGF0YSI6IHt9fQ==.df.parquet`

 * *Files identical despite different names*

### Comparing `news-signals-0.1.9/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExNTEwOTg2NSIsICJtZXRhZGF0YSI6IHt9fQ==.stories_df.parquet` & `news-signals-0.2.0/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExNTEwOTg2NSIsICJtZXRhZGF0YSI6IHt9fQ==.stories_df.parquet`

 * *Files identical despite different names*

### Comparing `news-signals-0.1.9/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExNTQ1MDc2IiwgIm1ldGFkYXRhIjoge319.df.parquet` & `news-signals-0.2.0/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExNTQ1MDc2IiwgIm1ldGFkYXRhIjoge319.df.parquet`

 * *Files identical despite different names*

### Comparing `news-signals-0.1.9/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExNTQ1MDc2IiwgIm1ldGFkYXRhIjoge319.stories_df.parquet` & `news-signals-0.2.0/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExNTQ1MDc2IiwgIm1ldGFkYXRhIjoge319.stories_df.parquet`

 * *Files identical despite different names*

### Comparing `news-signals-0.1.9/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExNzA4MTYxMiIsICJtZXRhZGF0YSI6IHt9fQ==.df.parquet` & `news-signals-0.2.0/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExNzA4MTYxMiIsICJtZXRhZGF0YSI6IHt9fQ==.df.parquet`

 * *Files identical despite different names*

### Comparing `news-signals-0.1.9/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExNzA4MTYxMiIsICJtZXRhZGF0YSI6IHt9fQ==.stories_df.parquet` & `news-signals-0.2.0/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExNzA4MTYxMiIsICJtZXRhZGF0YSI6IHt9fQ==.stories_df.parquet`

 * *Files identical despite different names*

### Comparing `news-signals-0.1.9/resources/test/politics_china_australia_timeseries.json` & `news-signals-0.2.0/resources/test/politics_china_australia_timeseries.json`

 * *Files identical despite different names*

### Comparing `news-signals-0.1.9/resources/test/sample_stories.json` & `news-signals-0.2.0/resources/test/sample_stories.json`

 * *Files identical despite different names*

### Comparing `news-signals-0.1.9/resources/test/tesla_stories.json` & `news-signals-0.2.0/resources/test/tesla_stories.json`

 * *Files identical despite different names*

### Comparing `news-signals-0.1.9/setup.py` & `news-signals-0.2.0/setup.py`

 * *Files identical despite different names*

