# Comparing `tmp/CmonCrawl-1.0.1.tar.gz` & `tmp/CmonCrawl-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "CmonCrawl-1.0.1.tar", last modified: Fri May 12 23:28:24 2023, max compression
+gzip compressed data, was "CmonCrawl-1.0.2.tar", last modified: Mon May 22 20:28:44 2023, max compression
```

## Comparing `CmonCrawl-1.0.1.tar` & `CmonCrawl-1.0.2.tar`

### file list

```diff
@@ -1,958 +1,959 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 23:28:24.145061 CmonCrawl-1.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 23:28:24.033059 CmonCrawl-1.0.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 23:28:24.045059 CmonCrawl-1.0.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      632 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/.github/workflows/test_and_push.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3078 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      377 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/.pre-commit-config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 23:28:24.045059 CmonCrawl-1.0.1/.vscode/
--rw-r--r--   0 runner    (1001) docker     (123)     1367 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/.vscode/launch.json
--rw-r--r--   0 runner    (1001) docker     (123)      459 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/.vscode/settings.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 23:28:24.045059 CmonCrawl-1.0.1/CmonCrawl.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5835 2023-05-12 23:28:23.000000 CmonCrawl-1.0.1/CmonCrawl.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    61003 2023-05-12 23:28:24.000000 CmonCrawl-1.0.1/CmonCrawl.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-12 23:28:23.000000 CmonCrawl-1.0.1/CmonCrawl.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-05-12 23:28:23.000000 CmonCrawl-1.0.1/CmonCrawl.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      446 2023-05-12 23:28:23.000000 CmonCrawl-1.0.1/CmonCrawl.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-12 23:28:23.000000 CmonCrawl-1.0.1/CmonCrawl.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5835 2023-05-12 23:28:24.145061 CmonCrawl-1.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4102 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 23:28:24.045059 CmonCrawl-1.0.1/cmoncrawl/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/cmoncrawl/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 23:28:24.045059 CmonCrawl-1.0.1/cmoncrawl/aggregator/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 23:28:24.045059 CmonCrawl-1.0.1/cmoncrawl/aggregator/.vscode/
--rw-r--r--   0 runner    (1001) docker     (123)      215 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/cmoncrawl/aggregator/.vscode/settings.json
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/cmoncrawl/aggregator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16838 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/cmoncrawl/aggregator/index_query.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 23:28:24.045059 CmonCrawl-1.0.1/cmoncrawl/aggregator/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/cmoncrawl/aggregator/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      865 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/cmoncrawl/aggregator/utils/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)      209 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/cmoncrawl/aggregator/utils/ndjson_decoder.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 23:28:24.045059 CmonCrawl-1.0.1/cmoncrawl/common/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/cmoncrawl/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      996 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/cmoncrawl/common/loggers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2305 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/cmoncrawl/common/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 23:28:24.045059 CmonCrawl-1.0.1/cmoncrawl/integrations/
--rw-r--r--   0 runner    (1001) docker     (123)     1439 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/cmoncrawl/integrations/commands.py
--rw-r--r--   0 runner    (1001) docker     (123)     6048 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/cmoncrawl/integrations/download.py
--rw-r--r--   0 runner    (1001) docker     (123)     6675 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/cmoncrawl/integrations/extract.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 23:28:24.045059 CmonCrawl-1.0.1/cmoncrawl/middleware/
--rw-r--r--   0 runner    (1001) docker     (123)    12061 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/cmoncrawl/middleware/stompware.py
--rw-r--r--   0 runner    (1001) docker     (123)     4703 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/cmoncrawl/middleware/synchronized.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 23:28:24.049059 CmonCrawl-1.0.1/cmoncrawl/processor/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/cmoncrawl/processor/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 23:28:24.049059 CmonCrawl-1.0.1/cmoncrawl/processor/extraction/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/cmoncrawl/processor/extraction/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1123 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/cmoncrawl/processor/extraction/filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     8378 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/cmoncrawl/processor/extraction/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 23:28:24.049059 CmonCrawl-1.0.1/cmoncrawl/processor/pipeline/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/cmoncrawl/processor/pipeline/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8156 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/cmoncrawl/processor/pipeline/downloader.py
--rw-r--r--   0 runner    (1001) docker     (123)     5611 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/cmoncrawl/processor/pipeline/extractor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1835 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/cmoncrawl/processor/pipeline/pipeline.py
--rw-r--r--   0 runner    (1001) docker     (123)     5698 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/cmoncrawl/processor/pipeline/router.py
--rw-r--r--   0 runner    (1001) docker     (123)     6929 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/cmoncrawl/processor/pipeline/streamer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 23:28:24.049059 CmonCrawl-1.0.1/docs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/.nojekyll
--rw-r--r--   0 runner    (1001) docker     (123)      638 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 23:28:24.033059 CmonCrawl-1.0.1/docs/build/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 23:28:24.049059 CmonCrawl-1.0.1/docs/build/doctrees/
--rw-r--r--   0 runner    (1001) docker     (123)     4150 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/doctrees/api.doctree
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 23:28:24.049059 CmonCrawl-1.0.1/docs/build/doctrees/cli/
--rw-r--r--   0 runner    (1001) docker     (123)     7226 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/doctrees/cli/cli.doctree
--rw-r--r--   0 runner    (1001) docker     (123)    16083 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/doctrees/cli/download.doctree
--rw-r--r--   0 runner    (1001) docker     (123)    17674 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/doctrees/cli/extract.doctree
--rw-r--r--   0 runner    (1001) docker     (123)     2845 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/doctrees/cli/index.doctree
--rw-r--r--   0 runner    (1001) docker     (123)   447558 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/doctrees/environment.pickle
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 23:28:24.049059 CmonCrawl-1.0.1/docs/build/doctrees/extraction/
--rw-r--r--   0 runner    (1001) docker     (123)    18267 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/doctrees/extraction/config_file.doctree
--rw-r--r--   0 runner    (1001) docker     (123)    15604 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/doctrees/extraction/creating_extractor.doctree
--rw-r--r--   0 runner    (1001) docker     (123)     2848 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/doctrees/extraction/index.doctree
--rw-r--r--   0 runner    (1001) docker     (123)     8169 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/doctrees/extraction/utils.doctree
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 23:28:24.069059 CmonCrawl-1.0.1/docs/build/doctrees/generated/
--rw-r--r--   0 runner    (1001) docker     (123)     5976 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/doctrees/generated/cmoncrawl.aggregator.doctree
--rw-r--r--   0 runner    (1001) docker     (123)    16051 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/doctrees/generated/cmoncrawl.aggregator.index_query.IndexAggregator.__init__.doctree
--rw-r--r--   0 runner    (1001) docker     (123)     9377 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/doctrees/generated/cmoncrawl.aggregator.index_query.IndexAggregator.aclose.doctree
--rw-r--r--   0 runner    (1001) docker     (123)     4857 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/doctrees/generated/cmoncrawl.aggregator.index_query.IndexAggregator.aopen.doctree
--rw-r--r--   0 runner    (1001) docker     (123)    37518 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/doctrees/generated/cmoncrawl.aggregator.index_query.IndexAggregator.doctree
--rw-r--r--   0 runner    (1001) docker     (123)     6990 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/doctrees/generated/cmoncrawl.aggregator.index_query.IndexAggregator.get_all_CC_indexes.doctree
--rw-r--r--   0 runner    (1001) docker     (123)    11632 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/doctrees/generated/cmoncrawl.aggregator.index_query.IndexAggregator.get_captured_responses.doctree
--rw-r--r--   0 runner    (1001) docker     (123)     9861 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/doctrees/generated/cmoncrawl.aggregator.index_query.IndexAggregator.get_number_of_pages.doctree
--rw-r--r--   0 runner    (1001) docker     (123)     8979 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/doctrees/generated/cmoncrawl.aggregator.index_query.doctree
--rw-r--r--   0 runner    (1001) docker     (123)     6196 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/doctrees/generated/cmoncrawl.aggregator.utils.doctree
--rw-r--r--   0 runner    (1001) docker     (123)     4914 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/doctrees/generated/cmoncrawl.aggregator.utils.helpers.doctree
--rw-r--r--   0 runner    (1001) docker     (123)    13989 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/doctrees/generated/cmoncrawl.aggregator.utils.ndjson_decoder.Decoder.__init__.doctree
--rw-r--r--   0 runner    (1001) docker     (123)     6254 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/doctrees/generated/cmoncrawl.aggregator.utils.ndjson_decoder.Decoder.decode.doctree
--rw-r--r--   0 runner    (1001) docker     (123)    25998 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/doctrees/generated/cmoncrawl.aggregator.utils.ndjson_decoder.Decoder.doctree
--rw-r--r--   0 runner    (1001) docker     (123)     6093 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/doctrees/generated/cmoncrawl.aggregator.utils.ndjson_decoder.Decoder.raw_decode.doctree
--rw-r--r--   0 runner    (1001) docker     (123)     5490 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/doctrees/generated/cmoncrawl.aggregator.utils.ndjson_decoder.doctree
--rw-r--r--   0 runner    (1001) docker     (123)     5824 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/doctrees/generated/cmoncrawl.common.doctree
--rw-r--r--   0 runner    (1001) docker     (123)     2859 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/doctrees/generated/cmoncrawl.common.loggers.doctree
--rw-r--r--   0 runner    (1001) docker     (123)     7639 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/doctrees/generated/cmoncrawl.common.types.DomainCrawl.__init__.doctree
--rw-r--r--   0 runner    (1001) docker     (123)    17989 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/doctrees/generated/cmoncrawl.common.types.DomainCrawl.doctree
--rw-r--r--   0 runner    (1001) docker     (123)    12190 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/doctrees/generated/cmoncrawl.common.types.DomainRecord.__init__.doctree
--rw-r--r--   0 runner    (1001) docker     (123)    36970 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/doctrees/generated/cmoncrawl.common.types.DomainRecord.doctree
--rw-r--r--   0 runner    (1001) docker     (123)     8890 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/doctrees/generated/cmoncrawl.common.types.DomainRecord.from_dict.doctree
--rw-r--r--   0 runner    (1001) docker     (123)     8994 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/doctrees/generated/cmoncrawl.common.types.DomainRecord.from_json.doctree
--rw-r--r--   0 runner    (1001) docker     (123)    11251 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/doctrees/generated/cmoncrawl.common.types.DomainRecord.schema.doctree
--rw-r--r--   0 runner    (1001) docker     (123)     8412 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/doctrees/generated/cmoncrawl.common.types.DomainRecord.to_dict.doctree
--rw-r--r--   0 runner    (1001) docker     (123)    16752 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/doctrees/generated/cmoncrawl.common.types.DomainRecord.to_json.doctree
--rw-r--r--   0 runner    (1001) docker     (123)     6301 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/doctrees/generated/cmoncrawl.common.types.ExtractConfig.__init__.doctree
--rw-r--r--   0 runner    (1001) docker     (123)    20553 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/doctrees/generated/cmoncrawl.common.types.ExtractConfig.doctree
--rw-r--r--   0 runner    (1001) docker     (123)     8905 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/doctrees/generated/cmoncrawl.common.types.ExtractConfig.from_dict.doctree
--rw-r--r--   0 runner    (1001) docker     (123)     9009 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/doctrees/generated/cmoncrawl.common.types.ExtractConfig.from_json.doctree
--rw-r--r--   0 runner    (1001) docker     (123)    11265 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/doctrees/generated/cmoncrawl.common.types.ExtractConfig.schema.doctree
--rw-r--r--   0 runner    (1001) docker     (123)     8427 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/doctrees/generated/cmoncrawl.common.types.ExtractConfig.to_dict.doctree
--rw-r--r--   0 runner    (1001) docker     (123)    16767 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/doctrees/generated/cmoncrawl.common.types.ExtractConfig.to_json.doctree
--rw-r--r--   0 runner    (1001) docker     (123)     8264 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/doctrees/generated/cmoncrawl.common.types.ExtractorConfig.__init__.doctree
--rw-r--r--   0 runner    (1001) docker     (123)    25358 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/doctrees/generated/cmoncrawl.common.types.ExtractorConfig.doctree
--rw-r--r--   0 runner    (1001) docker     (123)     8935 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/doctrees/generated/cmoncrawl.common.types.ExtractorConfig.from_dict.doctree
--rw-r--r--   0 runner    (1001) docker     (123)     9039 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/doctrees/generated/cmoncrawl.common.types.ExtractorConfig.from_json.doctree
--rw-r--r--   0 runner    (1001) docker     (123)    11293 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/doctrees/generated/cmoncrawl.common.types.ExtractorConfig.schema.doctree
--rw-r--r--   0 runner    (1001) docker     (123)     8457 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/doctrees/generated/cmoncrawl.common.types.ExtractorConfig.to_dict.doctree
--rw-r--r--   0 runner    (1001) docker     (123)    16797 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/doctrees/generated/cmoncrawl.common.types.ExtractorConfig.to_json.doctree
--rw-r--r--   0 runner    (1001) docker     (123)     7157 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/doctrees/generated/cmoncrawl.common.types.PipeMetadata.__init__.doctree
--rw-r--r--   0 runner    (1001) docker     (123)    20439 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/doctrees/generated/cmoncrawl.common.types.PipeMetadata.doctree
--rw-r--r--   0 runner    (1001) docker     (123)     6895 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/doctrees/generated/cmoncrawl.common.types.RetrieveResponse.__init__.doctree
--rw-r--r--   0 runner    (1001) docker     (123)    16512 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/doctrees/generated/cmoncrawl.common.types.RetrieveResponse.doctree
--rw-r--r--   0 runner    (1001) docker     (123)     5149 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/doctrees/generated/cmoncrawl.common.types.RoutesConfig.__init__.doctree
--rw-r--r--   0 runner    (1001) docker     (123)    18100 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/doctrees/generated/cmoncrawl.common.types.RoutesConfig.doctree
--rw-r--r--   0 runner    (1001) docker     (123)     8890 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/doctrees/generated/cmoncrawl.common.types.RoutesConfig.from_dict.doctree
--rw-r--r--   0 runner    (1001) docker     (123)     8994 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/doctrees/generated/cmoncrawl.common.types.RoutesConfig.from_json.doctree
--rw-r--r--   0 runner    (1001) docker     (123)    11251 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/doctrees/generated/cmoncrawl.common.types.RoutesConfig.schema.doctree
--rw-r--r--   0 runner    (1001) docker     (123)     8412 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/doctrees/generated/cmoncrawl.common.types.RoutesConfig.to_dict.doctree
--rw-r--r--   0 runner    (1001) docker     (123)    16752 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/doctrees/generated/cmoncrawl.common.types.RoutesConfig.to_json.doctree
--rw-r--r--   0 runner    (1001) docker     (123)    12267 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/doctrees/generated/cmoncrawl.common.types.doctree
--rw-r--r--   0 runner    (1001) docker     (123)     6530 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/doctrees/generated/cmoncrawl.doctree
--rw-r--r--   0 runner    (1001) docker     (123)     5962 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/doctrees/generated/cmoncrawl.processor.doctree
--rw-r--r--   0 runner    (1001) docker     (123)     6244 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/doctrees/generated/cmoncrawl.processor.extraction.doctree
--rw-r--r--   0 runner    (1001) docker     (123)     6802 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/doctrees/generated/cmoncrawl.processor.extraction.filters.doctree
--rw-r--r--   0 runner    (1001) docker     (123)    15336 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/doctrees/generated/cmoncrawl.processor.extraction.utils.doctree
--rw-r--r--   0 runner    (1001) docker     (123)     9365 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/doctrees/generated/cmoncrawl.processor.pipeline.doctree
--rw-r--r--   0 runner    (1001) docker     (123)    10078 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/doctrees/generated/cmoncrawl.processor.pipeline.downloader.AsyncDownloader.__init__.doctree
--rw-r--r--   0 runner    (1001) docker     (123)     9400 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/doctrees/generated/cmoncrawl.processor.pipeline.downloader.AsyncDownloader.aclose.doctree
--rw-r--r--   0 runner    (1001) docker     (123)     4897 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/doctrees/generated/cmoncrawl.processor.pipeline.downloader.AsyncDownloader.aopen.doctree
--rw-r--r--   0 runner    (1001) docker     (123)    24370 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/doctrees/generated/cmoncrawl.processor.pipeline.downloader.AsyncDownloader.doctree
--rw-r--r--   0 runner    (1001) docker     (123)     5359 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/doctrees/generated/cmoncrawl.processor.pipeline.downloader.AsyncDownloader.download.doctree
--rw-r--r--   0 runner    (1001) docker     (123)     7304 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/doctrees/generated/cmoncrawl.processor.pipeline.downloader.AsyncDownloader.unwrap.doctree
--rw-r--r--   0 runner    (1001) docker     (123)     8595 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/doctrees/generated/cmoncrawl.processor.pipeline.downloader.DownloaderDummy.__init__.doctree
--rw-r--r--   0 runner    (1001) docker     (123)    21942 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/doctrees/generated/cmoncrawl.processor.pipeline.downloader.DownloaderDummy.doctree
--rw-r--r--   0 runner    (1001) docker     (123)     5359 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/doctrees/generated/cmoncrawl.processor.pipeline.downloader.DownloaderDummy.download.doctree
--rw-r--r--   0 runner    (1001) docker     (123)     5116 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/doctrees/generated/cmoncrawl.processor.pipeline.downloader.DownloaderDummy.extract_url.doctree
--rw-r--r--   0 runner    (1001) docker     (123)     5099 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/doctrees/generated/cmoncrawl.processor.pipeline.downloader.DownloaderDummy.extract_year.doctree
--rw-r--r--   0 runner    (1001) docker     (123)     5744 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/doctrees/generated/cmoncrawl.processor.pipeline.downloader.DownloaderDummy.mine_metadata.doctree
--rw-r--r--   0 runner    (1001) docker     (123)     4155 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/doctrees/generated/cmoncrawl.processor.pipeline.downloader.IDownloader.__init__.doctree
--rw-r--r--   0 runner    (1001) docker     (123)     8781 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/doctrees/generated/cmoncrawl.processor.pipeline.downloader.IDownloader.doctree
--rw-r--r--   0 runner    (1001) docker     (123)     6867 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/doctrees/generated/cmoncrawl.processor.pipeline.downloader.IDownloader.download.doctree
--rw-r--r--   0 runner    (1001) docker     (123)     8113 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/doctrees/generated/cmoncrawl.processor.pipeline.downloader.doctree
--rw-r--r--   0 runner    (1001) docker     (123)     5883 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/doctrees/generated/cmoncrawl.processor.pipeline.extractor.BaseExtractor.__init__.doctree
--rw-r--r--   0 runner    (1001) docker     (123)    17113 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/doctrees/generated/cmoncrawl.processor.pipeline.extractor.BaseExtractor.doctree
--rw-r--r--   0 runner    (1001) docker     (123)     7171 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/doctrees/generated/cmoncrawl.processor.pipeline.extractor.BaseExtractor.extract.doctree
--rw-r--r--   0 runner    (1001) docker     (123)     7645 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/doctrees/generated/cmoncrawl.processor.pipeline.extractor.BaseExtractor.extract_soup.doctree
--rw-r--r--   0 runner    (1001) docker     (123)     6031 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/doctrees/generated/cmoncrawl.processor.pipeline.extractor.BaseExtractor.filter_raw.doctree
--rw-r--r--   0 runner    (1001) docker     (123)     6100 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/doctrees/generated/cmoncrawl.processor.pipeline.extractor.BaseExtractor.filter_soup.doctree
--rw-r--r--   0 runner    (1001) docker     (123)     5960 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/doctrees/generated/cmoncrawl.processor.pipeline.extractor.BaseExtractor.preprocess.doctree
--rw-r--r--   0 runner    (1001) docker     (123)     5597 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/doctrees/generated/cmoncrawl.processor.pipeline.extractor.DomainRecordExtractor.__init__.doctree
--rw-r--r--   0 runner    (1001) docker     (123)    17063 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/doctrees/generated/cmoncrawl.processor.pipeline.extractor.DomainRecordExtractor.doctree
--rw-r--r--   0 runner    (1001) docker     (123)     7283 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/doctrees/generated/cmoncrawl.processor.pipeline.extractor.DomainRecordExtractor.extract.doctree
--rw-r--r--   0 runner    (1001) docker     (123)     5960 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/doctrees/generated/cmoncrawl.processor.pipeline.extractor.DomainRecordExtractor.extract_soup.doctree
--rw-r--r--   0 runner    (1001) docker     (123)     5876 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/doctrees/generated/cmoncrawl.processor.pipeline.extractor.DomainRecordExtractor.filter_raw.doctree
--rw-r--r--   0 runner    (1001) docker     (123)     6220 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/doctrees/generated/cmoncrawl.processor.pipeline.extractor.DomainRecordExtractor.filter_soup.doctree
--rw-r--r--   0 runner    (1001) docker     (123)     6072 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/doctrees/generated/cmoncrawl.processor.pipeline.extractor.DomainRecordExtractor.preprocess.doctree
--rw-r--r--   0 runner    (1001) docker     (123)     5469 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/doctrees/generated/cmoncrawl.processor.pipeline.extractor.HTMLExtractor.__init__.doctree
--rw-r--r--   0 runner    (1001) docker     (123)    16655 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/doctrees/generated/cmoncrawl.processor.pipeline.extractor.HTMLExtractor.doctree
--rw-r--r--   0 runner    (1001) docker     (123)     7171 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/doctrees/generated/cmoncrawl.processor.pipeline.extractor.HTMLExtractor.extract.doctree
--rw-r--r--   0 runner    (1001) docker     (123)     5832 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/doctrees/generated/cmoncrawl.processor.pipeline.extractor.HTMLExtractor.extract_soup.doctree
--rw-r--r--   0 runner    (1001) docker     (123)     5748 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/doctrees/generated/cmoncrawl.processor.pipeline.extractor.HTMLExtractor.filter_raw.doctree
--rw-r--r--   0 runner    (1001) docker     (123)     6100 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/doctrees/generated/cmoncrawl.processor.pipeline.extractor.HTMLExtractor.filter_soup.doctree
--rw-r--r--   0 runner    (1001) docker     (123)     5960 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/doctrees/generated/cmoncrawl.processor.pipeline.extractor.HTMLExtractor.preprocess.doctree
--rw-r--r--   0 runner    (1001) docker     (123)     4128 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/doctrees/generated/cmoncrawl.processor.pipeline.extractor.IExtractor.__init__.doctree
--rw-r--r--   0 runner    (1001) docker     (123)     8734 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/doctrees/generated/cmoncrawl.processor.pipeline.extractor.IExtractor.doctree
--rw-r--r--   0 runner    (1001) docker     (123)     7407 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/doctrees/generated/cmoncrawl.processor.pipeline.extractor.IExtractor.extract.doctree
--rw-r--r--   0 runner    (1001) docker     (123)     9217 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/doctrees/generated/cmoncrawl.processor.pipeline.extractor.doctree
--rw-r--r--   0 runner    (1001) docker     (123)     6770 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/doctrees/generated/cmoncrawl.processor.pipeline.pipeline.ProcessorPipeline.__init__.doctree
--rw-r--r--   0 runner    (1001) docker     (123)    14259 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/doctrees/generated/cmoncrawl.processor.pipeline.pipeline.ProcessorPipeline.doctree
--rw-r--r--   0 runner    (1001) docker     (123)     7149 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/doctrees/generated/cmoncrawl.processor.pipeline.pipeline.ProcessorPipeline.process_domain_record.doctree
--rw-r--r--   0 runner    (1001) docker     (123)     5401 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/doctrees/generated/cmoncrawl.processor.pipeline.pipeline.doctree
--rw-r--r--   0 runner    (1001) docker     (123)     4047 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/doctrees/generated/cmoncrawl.processor.pipeline.router.IRouter.__init__.doctree
--rw-r--r--   0 runner    (1001) docker     (123)     8547 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/doctrees/generated/cmoncrawl.processor.pipeline.router.IRouter.doctree
--rw-r--r--   0 runner    (1001) docker     (123)     7889 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/doctrees/generated/cmoncrawl.processor.pipeline.router.IRouter.route.doctree
--rw-r--r--   0 runner    (1001) docker     (123)     7921 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/doctrees/generated/cmoncrawl.processor.pipeline.router.Route.__init__.doctree
--rw-r--r--   0 runner    (1001) docker     (123)    19674 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/doctrees/generated/cmoncrawl.processor.pipeline.router.Route.doctree
--rw-r--r--   0 runner    (1001) docker     (123)     4031 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/doctrees/generated/cmoncrawl.processor.pipeline.router.Router.__init__.doctree
--rw-r--r--   0 runner    (1001) docker     (123)    15623 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/doctrees/generated/cmoncrawl.processor.pipeline.router.Router.doctree
--rw-r--r--   0 runner    (1001) docker     (123)     5681 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/doctrees/generated/cmoncrawl.processor.pipeline.router.Router.load_extractor.doctree
--rw-r--r--   0 runner    (1001) docker     (123)     4902 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/doctrees/generated/cmoncrawl.processor.pipeline.router.Router.load_module.doctree
--rw-r--r--   0 runner    (1001) docker     (123)     5103 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/doctrees/generated/cmoncrawl.processor.pipeline.router.Router.load_module_as_extractor.doctree
--rw-r--r--   0 runner    (1001) docker     (123)     4892 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/doctrees/generated/cmoncrawl.processor.pipeline.router.Router.load_modules.doctree
--rw-r--r--   0 runner    (1001) docker     (123)     9971 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/doctrees/generated/cmoncrawl.processor.pipeline.router.Router.register_route.doctree
--rw-r--r--   0 runner    (1001) docker     (123)     5445 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/doctrees/generated/cmoncrawl.processor.pipeline.router.Router.register_routes.doctree
--rw-r--r--   0 runner    (1001) docker     (123)     7593 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/doctrees/generated/cmoncrawl.processor.pipeline.router.Router.route.doctree
--rw-r--r--   0 runner    (1001) docker     (123)     7194 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/doctrees/generated/cmoncrawl.processor.pipeline.router.doctree
--rw-r--r--   0 runner    (1001) docker     (123)     9351 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/doctrees/generated/cmoncrawl.processor.pipeline.streamer.BaseStreamerFile.__init__.doctree
--rw-r--r--   0 runner    (1001) docker     (123)     4837 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/doctrees/generated/cmoncrawl.processor.pipeline.streamer.BaseStreamerFile.clean_up.doctree
--rw-r--r--   0 runner    (1001) docker     (123)    23368 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/doctrees/generated/cmoncrawl.processor.pipeline.streamer.BaseStreamerFile.doctree
--rw-r--r--   0 runner    (1001) docker     (123)     5197 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/doctrees/generated/cmoncrawl.processor.pipeline.streamer.BaseStreamerFile.get_file_name.doctree
--rw-r--r--   0 runner    (1001) docker     (123)     6582 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/doctrees/generated/cmoncrawl.processor.pipeline.streamer.BaseStreamerFile.metadata_to_string.doctree
--rw-r--r--   0 runner    (1001) docker     (123)     7136 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/doctrees/generated/cmoncrawl.processor.pipeline.streamer.BaseStreamerFile.stream.doctree
--rw-r--r--   0 runner    (1001) docker     (123)     4101 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/doctrees/generated/cmoncrawl.processor.pipeline.streamer.IStreamer.__init__.doctree
--rw-r--r--   0 runner    (1001) docker     (123)     4921 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/doctrees/generated/cmoncrawl.processor.pipeline.streamer.IStreamer.clean_up.doctree
--rw-r--r--   0 runner    (1001) docker     (123)    10102 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/doctrees/generated/cmoncrawl.processor.pipeline.streamer.IStreamer.doctree
--rw-r--r--   0 runner    (1001) docker     (123)     7218 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/doctrees/generated/cmoncrawl.processor.pipeline.streamer.IStreamer.stream.doctree
--rw-r--r--   0 runner    (1001) docker     (123)     4165 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/doctrees/generated/cmoncrawl.processor.pipeline.streamer.StreamerDummy.__init__.doctree
--rw-r--r--   0 runner    (1001) docker     (123)     4450 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/doctrees/generated/cmoncrawl.processor.pipeline.streamer.StreamerDummy.clean_up.doctree
--rw-r--r--   0 runner    (1001) docker     (123)    10278 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/doctrees/generated/cmoncrawl.processor.pipeline.streamer.StreamerDummy.doctree
--rw-r--r--   0 runner    (1001) docker     (123)     6779 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/doctrees/generated/cmoncrawl.processor.pipeline.streamer.StreamerDummy.stream.doctree
--rw-r--r--   0 runner    (1001) docker     (123)     5696 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/doctrees/generated/cmoncrawl.processor.pipeline.streamer.StreamerFileHTML.__init__.doctree
--rw-r--r--   0 runner    (1001) docker     (123)     4837 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/doctrees/generated/cmoncrawl.processor.pipeline.streamer.StreamerFileHTML.clean_up.doctree
--rw-r--r--   0 runner    (1001) docker     (123)    15596 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/doctrees/generated/cmoncrawl.processor.pipeline.streamer.StreamerFileHTML.doctree
--rw-r--r--   0 runner    (1001) docker     (123)     5197 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/doctrees/generated/cmoncrawl.processor.pipeline.streamer.StreamerFileHTML.get_file_name.doctree
--rw-r--r--   0 runner    (1001) docker     (123)     6301 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/doctrees/generated/cmoncrawl.processor.pipeline.streamer.StreamerFileHTML.metadata_to_string.doctree
--rw-r--r--   0 runner    (1001) docker     (123)     7136 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/doctrees/generated/cmoncrawl.processor.pipeline.streamer.StreamerFileHTML.stream.doctree
--rw-r--r--   0 runner    (1001) docker     (123)     7513 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/doctrees/generated/cmoncrawl.processor.pipeline.streamer.StreamerFileJSON.__init__.doctree
--rw-r--r--   0 runner    (1001) docker     (123)     4837 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/doctrees/generated/cmoncrawl.processor.pipeline.streamer.StreamerFileJSON.clean_up.doctree
--rw-r--r--   0 runner    (1001) docker     (123)    19273 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/doctrees/generated/cmoncrawl.processor.pipeline.streamer.StreamerFileJSON.doctree
--rw-r--r--   0 runner    (1001) docker     (123)     5197 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/doctrees/generated/cmoncrawl.processor.pipeline.streamer.StreamerFileJSON.get_file_name.doctree
--rw-r--r--   0 runner    (1001) docker     (123)     6301 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/doctrees/generated/cmoncrawl.processor.pipeline.streamer.StreamerFileJSON.metadata_to_string.doctree
--rw-r--r--   0 runner    (1001) docker     (123)     7136 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/doctrees/generated/cmoncrawl.processor.pipeline.streamer.StreamerFileJSON.stream.doctree
--rw-r--r--   0 runner    (1001) docker     (123)    10726 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/doctrees/generated/cmoncrawl.processor.pipeline.streamer.doctree
--rw-r--r--   0 runner    (1001) docker     (123)     5198 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/doctrees/index.doctree
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 23:28:24.069059 CmonCrawl-1.0.1/docs/build/doctrees/misc/
--rw-r--r--   0 runner    (1001) docker     (123)    10600 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/doctrees/misc/domain_record.doctree
--rw-r--r--   0 runner    (1001) docker     (123)     2781 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/doctrees/misc/index.doctree
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 23:28:24.069059 CmonCrawl-1.0.1/docs/build/doctrees/prog_guide/
--rw-r--r--   0 runner    (1001) docker     (123)     2834 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/doctrees/prog_guide/index.doctree
--rw-r--r--   0 runner    (1001) docker     (123)    24337 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/doctrees/prog_guide/overview.doctree
--rw-r--r--   0 runner    (1001) docker     (123)     8880 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/doctrees/prog_guide/pip.doctree
--rw-r--r--   0 runner    (1001) docker     (123)     9009 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/doctrees/usage.doctree
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 23:28:24.069059 CmonCrawl-1.0.1/docs/build/html/
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/html/.buildinfo
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 23:28:24.069059 CmonCrawl-1.0.1/docs/build/html/_sources/
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/html/_sources/api.rst.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 23:28:24.073059 CmonCrawl-1.0.1/docs/build/html/_sources/cli/
--rw-r--r--   0 runner    (1001) docker     (123)     1175 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/html/_sources/cli/cli.rst.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1987 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/html/_sources/cli/download.rst.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2753 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/html/_sources/cli/extract.rst.txt
--rw-r--r--   0 runner    (1001) docker     (123)      137 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/html/_sources/cli/index.rst.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 23:28:24.073059 CmonCrawl-1.0.1/docs/build/html/_sources/extraction/
--rw-r--r--   0 runner    (1001) docker     (123)     3910 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/html/_sources/extraction/config_file.rst.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2392 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/html/_sources/extraction/creating_extractor.rst.txt
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/html/_sources/extraction/index.rst.txt
--rw-r--r--   0 runner    (1001) docker     (123)      861 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/html/_sources/extraction/utils.rst.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 23:28:24.089060 CmonCrawl-1.0.1/docs/build/html/_sources/generated/
--rw-r--r--   0 runner    (1001) docker     (123)      220 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/html/_sources/generated/cmoncrawl.aggregator.index_query.IndexAggregator.__init__.rst.txt
--rw-r--r--   0 runner    (1001) docker     (123)      206 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/html/_sources/generated/cmoncrawl.aggregator.index_query.IndexAggregator.aclose.rst.txt
--rw-r--r--   0 runner    (1001) docker     (123)      203 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/html/_sources/generated/cmoncrawl.aggregator.index_query.IndexAggregator.aopen.rst.txt
--rw-r--r--   0 runner    (1001) docker     (123)      248 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/html/_sources/generated/cmoncrawl.aggregator.index_query.IndexAggregator.get_all_CC_indexes.rst.txt
--rw-r--r--   0 runner    (1001) docker     (123)      258 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/html/_sources/generated/cmoncrawl.aggregator.index_query.IndexAggregator.get_captured_responses.rst.txt
--rw-r--r--   0 runner    (1001) docker     (123)      251 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/html/_sources/generated/cmoncrawl.aggregator.index_query.IndexAggregator.get_number_of_pages.rst.txt
--rw-r--r--   0 runner    (1001) docker     (123)      530 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/html/_sources/generated/cmoncrawl.aggregator.index_query.IndexAggregator.rst.txt
--rw-r--r--   0 runner    (1001) docker     (123)      391 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/html/_sources/generated/cmoncrawl.aggregator.index_query.rst.txt
--rw-r--r--   0 runner    (1001) docker     (123)      269 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/html/_sources/generated/cmoncrawl.aggregator.rst.txt
--rw-r--r--   0 runner    (1001) docker     (123)      250 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/html/_sources/generated/cmoncrawl.aggregator.utils.helpers.rst.txt
--rw-r--r--   0 runner    (1001) docker     (123)      223 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/html/_sources/generated/cmoncrawl.aggregator.utils.ndjson_decoder.Decoder.__init__.rst.txt
--rw-r--r--   0 runner    (1001) docker     (123)      209 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/html/_sources/generated/cmoncrawl.aggregator.utils.ndjson_decoder.Decoder.decode.rst.txt
--rw-r--r--   0 runner    (1001) docker     (123)      223 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/html/_sources/generated/cmoncrawl.aggregator.utils.ndjson_decoder.Decoder.raw_decode.rst.txt
--rw-r--r--   0 runner    (1001) docker     (123)      383 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/html/_sources/generated/cmoncrawl.aggregator.utils.ndjson_decoder.Decoder.rst.txt
--rw-r--r--   0 runner    (1001) docker     (123)      282 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/html/_sources/generated/cmoncrawl.aggregator.utils.ndjson_decoder.rst.txt
--rw-r--r--   0 runner    (1001) docker     (123)      304 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/html/_sources/generated/cmoncrawl.aggregator.utils.rst.txt
--rw-r--r--   0 runner    (1001) docker     (123)      147 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/html/_sources/generated/cmoncrawl.common.loggers.rst.txt
--rw-r--r--   0 runner    (1001) docker     (123)      245 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/html/_sources/generated/cmoncrawl.common.rst.txt
--rw-r--r--   0 runner    (1001) docker     (123)      176 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/html/_sources/generated/cmoncrawl.common.types.DomainCrawl.__init__.rst.txt
--rw-r--r--   0 runner    (1001) docker     (123)      427 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/html/_sources/generated/cmoncrawl.common.types.DomainCrawl.rst.txt
--rw-r--r--   0 runner    (1001) docker     (123)      179 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/html/_sources/generated/cmoncrawl.common.types.DomainRecord.__init__.rst.txt
--rw-r--r--   0 runner    (1001) docker     (123)      176 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/html/_sources/generated/cmoncrawl.common.types.DomainRecord.from_dict.rst.txt
--rw-r--r--   0 runner    (1001) docker     (123)      176 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/html/_sources/generated/cmoncrawl.common.types.DomainRecord.from_json.rst.txt
--rw-r--r--   0 runner    (1001) docker     (123)      687 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/html/_sources/generated/cmoncrawl.common.types.DomainRecord.rst.txt
--rw-r--r--   0 runner    (1001) docker     (123)      165 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/html/_sources/generated/cmoncrawl.common.types.DomainRecord.schema.rst.txt
--rw-r--r--   0 runner    (1001) docker     (123)      170 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/html/_sources/generated/cmoncrawl.common.types.DomainRecord.to_dict.rst.txt
--rw-r--r--   0 runner    (1001) docker     (123)      170 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/html/_sources/generated/cmoncrawl.common.types.DomainRecord.to_json.rst.txt
--rw-r--r--   0 runner    (1001) docker     (123)      182 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/html/_sources/generated/cmoncrawl.common.types.ExtractConfig.__init__.rst.txt
--rw-r--r--   0 runner    (1001) docker     (123)      179 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/html/_sources/generated/cmoncrawl.common.types.ExtractConfig.from_dict.rst.txt
--rw-r--r--   0 runner    (1001) docker     (123)      179 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/html/_sources/generated/cmoncrawl.common.types.ExtractConfig.from_json.rst.txt
--rw-r--r--   0 runner    (1001) docker     (123)      568 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/html/_sources/generated/cmoncrawl.common.types.ExtractConfig.rst.txt
--rw-r--r--   0 runner    (1001) docker     (123)      168 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/html/_sources/generated/cmoncrawl.common.types.ExtractConfig.schema.rst.txt
--rw-r--r--   0 runner    (1001) docker     (123)      173 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/html/_sources/generated/cmoncrawl.common.types.ExtractConfig.to_dict.rst.txt
--rw-r--r--   0 runner    (1001) docker     (123)      173 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/html/_sources/generated/cmoncrawl.common.types.ExtractConfig.to_json.rst.txt
--rw-r--r--   0 runner    (1001) docker     (123)      188 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/html/_sources/generated/cmoncrawl.common.types.ExtractorConfig.__init__.rst.txt
--rw-r--r--   0 runner    (1001) docker     (123)      185 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/html/_sources/generated/cmoncrawl.common.types.ExtractorConfig.from_dict.rst.txt
--rw-r--r--   0 runner    (1001) docker     (123)      185 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/html/_sources/generated/cmoncrawl.common.types.ExtractorConfig.from_json.rst.txt
--rw-r--r--   0 runner    (1001) docker     (123)      604 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/html/_sources/generated/cmoncrawl.common.types.ExtractorConfig.rst.txt
--rw-r--r--   0 runner    (1001) docker     (123)      174 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/html/_sources/generated/cmoncrawl.common.types.ExtractorConfig.schema.rst.txt
--rw-r--r--   0 runner    (1001) docker     (123)      179 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/html/_sources/generated/cmoncrawl.common.types.ExtractorConfig.to_dict.rst.txt
--rw-r--r--   0 runner    (1001) docker     (123)      179 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/html/_sources/generated/cmoncrawl.common.types.ExtractorConfig.to_json.rst.txt
--rw-r--r--   0 runner    (1001) docker     (123)      179 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/html/_sources/generated/cmoncrawl.common.types.PipeMetadata.__init__.rst.txt
--rw-r--r--   0 runner    (1001) docker     (123)      536 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/html/_sources/generated/cmoncrawl.common.types.PipeMetadata.rst.txt
--rw-r--r--   0 runner    (1001) docker     (123)      191 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/html/_sources/generated/cmoncrawl.common.types.RetrieveResponse.__init__.rst.txt
--rw-r--r--   0 runner    (1001) docker     (123)      461 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/html/_sources/generated/cmoncrawl.common.types.RetrieveResponse.rst.txt
--rw-r--r--   0 runner    (1001) docker     (123)      179 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/html/_sources/generated/cmoncrawl.common.types.RoutesConfig.__init__.rst.txt
--rw-r--r--   0 runner    (1001) docker     (123)      176 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/html/_sources/generated/cmoncrawl.common.types.RoutesConfig.from_dict.rst.txt
--rw-r--r--   0 runner    (1001) docker     (123)      176 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/html/_sources/generated/cmoncrawl.common.types.RoutesConfig.from_json.rst.txt
--rw-r--r--   0 runner    (1001) docker     (123)      553 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/html/_sources/generated/cmoncrawl.common.types.RoutesConfig.rst.txt
--rw-r--r--   0 runner    (1001) docker     (123)      165 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/html/_sources/generated/cmoncrawl.common.types.RoutesConfig.schema.rst.txt
--rw-r--r--   0 runner    (1001) docker     (123)      170 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/html/_sources/generated/cmoncrawl.common.types.RoutesConfig.to_dict.rst.txt
--rw-r--r--   0 runner    (1001) docker     (123)      170 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/html/_sources/generated/cmoncrawl.common.types.RoutesConfig.to_json.rst.txt
--rw-r--r--   0 runner    (1001) docker     (123)      349 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/html/_sources/generated/cmoncrawl.common.types.rst.txt
--rw-r--r--   0 runner    (1001) docker     (123)      295 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/html/_sources/generated/cmoncrawl.processor.extraction.filters.rst.txt
--rw-r--r--   0 runner    (1001) docker     (123)      315 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/html/_sources/generated/cmoncrawl.processor.extraction.rst.txt
--rw-r--r--   0 runner    (1001) docker     (123)      500 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/html/_sources/generated/cmoncrawl.processor.extraction.utils.rst.txt
--rw-r--r--   0 runner    (1001) docker     (123)      239 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/html/_sources/generated/cmoncrawl.processor.pipeline.downloader.AsyncDownloader.__init__.rst.txt
--rw-r--r--   0 runner    (1001) docker     (123)      225 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/html/_sources/generated/cmoncrawl.processor.pipeline.downloader.AsyncDownloader.aclose.rst.txt
--rw-r--r--   0 runner    (1001) docker     (123)      222 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/html/_sources/generated/cmoncrawl.processor.pipeline.downloader.AsyncDownloader.aopen.rst.txt
--rw-r--r--   0 runner    (1001) docker     (123)      231 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/html/_sources/generated/cmoncrawl.processor.pipeline.downloader.AsyncDownloader.download.rst.txt
--rw-r--r--   0 runner    (1001) docker     (123)      480 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/html/_sources/generated/cmoncrawl.processor.pipeline.downloader.AsyncDownloader.rst.txt
--rw-r--r--   0 runner    (1001) docker     (123)      225 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/html/_sources/generated/cmoncrawl.processor.pipeline.downloader.AsyncDownloader.unwrap.rst.txt
--rw-r--r--   0 runner    (1001) docker     (123)      239 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/html/_sources/generated/cmoncrawl.processor.pipeline.downloader.DownloaderDummy.__init__.rst.txt
--rw-r--r--   0 runner    (1001) docker     (123)      231 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/html/_sources/generated/cmoncrawl.processor.pipeline.downloader.DownloaderDummy.download.rst.txt
--rw-r--r--   0 runner    (1001) docker     (123)      242 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/html/_sources/generated/cmoncrawl.processor.pipeline.downloader.DownloaderDummy.extract_url.rst.txt
--rw-r--r--   0 runner    (1001) docker     (123)      245 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/html/_sources/generated/cmoncrawl.processor.pipeline.downloader.DownloaderDummy.extract_year.rst.txt
--rw-r--r--   0 runner    (1001) docker     (123)      248 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/html/_sources/generated/cmoncrawl.processor.pipeline.downloader.DownloaderDummy.mine_metadata.rst.txt
--rw-r--r--   0 runner    (1001) docker     (123)      499 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/html/_sources/generated/cmoncrawl.processor.pipeline.downloader.DownloaderDummy.rst.txt
--rw-r--r--   0 runner    (1001) docker     (123)      227 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/html/_sources/generated/cmoncrawl.processor.pipeline.downloader.IDownloader.__init__.rst.txt
--rw-r--r--   0 runner    (1001) docker     (123)      219 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/html/_sources/generated/cmoncrawl.processor.pipeline.downloader.IDownloader.download.rst.txt
--rw-r--r--   0 runner    (1001) docker     (123)      371 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/html/_sources/generated/cmoncrawl.processor.pipeline.downloader.IDownloader.rst.txt
--rw-r--r--   0 runner    (1001) docker     (123)      322 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/html/_sources/generated/cmoncrawl.processor.pipeline.downloader.rst.txt
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/html/_sources/generated/cmoncrawl.processor.pipeline.extractor.BaseExtractor.__init__.rst.txt
--rw-r--r--   0 runner    (1001) docker     (123)      219 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/html/_sources/generated/cmoncrawl.processor.pipeline.extractor.BaseExtractor.extract.rst.txt
--rw-r--r--   0 runner    (1001) docker     (123)      236 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/html/_sources/generated/cmoncrawl.processor.pipeline.extractor.BaseExtractor.extract_soup.rst.txt
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/html/_sources/generated/cmoncrawl.processor.pipeline.extractor.BaseExtractor.filter_raw.rst.txt
--rw-r--r--   0 runner    (1001) docker     (123)      233 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/html/_sources/generated/cmoncrawl.processor.pipeline.extractor.BaseExtractor.filter_soup.rst.txt
--rw-r--r--   0 runner    (1001) docker     (123)      228 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/html/_sources/generated/cmoncrawl.processor.pipeline.extractor.BaseExtractor.preprocess.rst.txt
--rw-r--r--   0 runner    (1001) docker     (123)      508 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/html/_sources/generated/cmoncrawl.processor.pipeline.extractor.BaseExtractor.rst.txt
--rw-r--r--   0 runner    (1001) docker     (123)      254 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/html/_sources/generated/cmoncrawl.processor.pipeline.extractor.DomainRecordExtractor.__init__.rst.txt
--rw-r--r--   0 runner    (1001) docker     (123)      243 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/html/_sources/generated/cmoncrawl.processor.pipeline.extractor.DomainRecordExtractor.extract.rst.txt
--rw-r--r--   0 runner    (1001) docker     (123)      260 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/html/_sources/generated/cmoncrawl.processor.pipeline.extractor.DomainRecordExtractor.extract_soup.rst.txt
--rw-r--r--   0 runner    (1001) docker     (123)      254 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/html/_sources/generated/cmoncrawl.processor.pipeline.extractor.DomainRecordExtractor.filter_raw.rst.txt
--rw-r--r--   0 runner    (1001) docker     (123)      257 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/html/_sources/generated/cmoncrawl.processor.pipeline.extractor.DomainRecordExtractor.filter_soup.rst.txt
--rw-r--r--   0 runner    (1001) docker     (123)      252 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/html/_sources/generated/cmoncrawl.processor.pipeline.extractor.DomainRecordExtractor.preprocess.rst.txt
--rw-r--r--   0 runner    (1001) docker     (123)      580 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/html/_sources/generated/cmoncrawl.processor.pipeline.extractor.DomainRecordExtractor.rst.txt
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/html/_sources/generated/cmoncrawl.processor.pipeline.extractor.HTMLExtractor.__init__.rst.txt
--rw-r--r--   0 runner    (1001) docker     (123)      219 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/html/_sources/generated/cmoncrawl.processor.pipeline.extractor.HTMLExtractor.extract.rst.txt
--rw-r--r--   0 runner    (1001) docker     (123)      236 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/html/_sources/generated/cmoncrawl.processor.pipeline.extractor.HTMLExtractor.extract_soup.rst.txt
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/html/_sources/generated/cmoncrawl.processor.pipeline.extractor.HTMLExtractor.filter_raw.rst.txt
--rw-r--r--   0 runner    (1001) docker     (123)      233 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/html/_sources/generated/cmoncrawl.processor.pipeline.extractor.HTMLExtractor.filter_soup.rst.txt
--rw-r--r--   0 runner    (1001) docker     (123)      228 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/html/_sources/generated/cmoncrawl.processor.pipeline.extractor.HTMLExtractor.preprocess.rst.txt
--rw-r--r--   0 runner    (1001) docker     (123)      508 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/html/_sources/generated/cmoncrawl.processor.pipeline.extractor.HTMLExtractor.rst.txt
--rw-r--r--   0 runner    (1001) docker     (123)      221 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/html/_sources/generated/cmoncrawl.processor.pipeline.extractor.IExtractor.__init__.rst.txt
--rw-r--r--   0 runner    (1001) docker     (123)      210 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/html/_sources/generated/cmoncrawl.processor.pipeline.extractor.IExtractor.extract.rst.txt
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/html/_sources/generated/cmoncrawl.processor.pipeline.extractor.IExtractor.rst.txt
--rw-r--r--   0 runner    (1001) docker     (123)      342 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/html/_sources/generated/cmoncrawl.processor.pipeline.extractor.rst.txt
--rw-r--r--   0 runner    (1001) docker     (123)      239 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/html/_sources/generated/cmoncrawl.processor.pipeline.pipeline.ProcessorPipeline.__init__.rst.txt
--rw-r--r--   0 runner    (1001) docker     (123)      274 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/html/_sources/generated/cmoncrawl.processor.pipeline.pipeline.ProcessorPipeline.process_domain_record.rst.txt
--rw-r--r--   0 runner    (1001) docker     (123)      408 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/html/_sources/generated/cmoncrawl.processor.pipeline.pipeline.ProcessorPipeline.rst.txt
--rw-r--r--   0 runner    (1001) docker     (123)      278 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/html/_sources/generated/cmoncrawl.processor.pipeline.pipeline.rst.txt
--rw-r--r--   0 runner    (1001) docker     (123)      203 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/html/_sources/generated/cmoncrawl.processor.pipeline.router.IRouter.__init__.rst.txt
--rw-r--r--   0 runner    (1001) docker     (123)      186 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/html/_sources/generated/cmoncrawl.processor.pipeline.router.IRouter.route.rst.txt
--rw-r--r--   0 runner    (1001) docker     (123)      336 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/html/_sources/generated/cmoncrawl.processor.pipeline.router.IRouter.rst.txt
--rw-r--r--   0 runner    (1001) docker     (123)      197 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/html/_sources/generated/cmoncrawl.processor.pipeline.router.Route.__init__.rst.txt
--rw-r--r--   0 runner    (1001) docker     (123)      436 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/html/_sources/generated/cmoncrawl.processor.pipeline.router.Route.rst.txt
--rw-r--r--   0 runner    (1001) docker     (123)      200 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/html/_sources/generated/cmoncrawl.processor.pipeline.router.Router.__init__.rst.txt
--rw-r--r--   0 runner    (1001) docker     (123)      212 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/html/_sources/generated/cmoncrawl.processor.pipeline.router.Router.load_extractor.rst.txt
--rw-r--r--   0 runner    (1001) docker     (123)      203 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/html/_sources/generated/cmoncrawl.processor.pipeline.router.Router.load_module.rst.txt
--rw-r--r--   0 runner    (1001) docker     (123)      246 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/html/_sources/generated/cmoncrawl.processor.pipeline.router.Router.load_module_as_extractor.rst.txt
--rw-r--r--   0 runner    (1001) docker     (123)      206 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/html/_sources/generated/cmoncrawl.processor.pipeline.router.Router.load_modules.rst.txt
--rw-r--r--   0 runner    (1001) docker     (123)      212 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/html/_sources/generated/cmoncrawl.processor.pipeline.router.Router.register_route.rst.txt
--rw-r--r--   0 runner    (1001) docker     (123)      215 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/html/_sources/generated/cmoncrawl.processor.pipeline.router.Router.register_routes.rst.txt
--rw-r--r--   0 runner    (1001) docker     (123)      183 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/html/_sources/generated/cmoncrawl.processor.pipeline.router.Router.route.rst.txt
--rw-r--r--   0 runner    (1001) docker     (123)      511 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/html/_sources/generated/cmoncrawl.processor.pipeline.router.Router.rst.txt
--rw-r--r--   0 runner    (1001) docker     (123)      287 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/html/_sources/generated/cmoncrawl.processor.pipeline.router.rst.txt
--rw-r--r--   0 runner    (1001) docker     (123)      433 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/html/_sources/generated/cmoncrawl.processor.pipeline.rst.txt
--rw-r--r--   0 runner    (1001) docker     (123)      236 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/html/_sources/generated/cmoncrawl.processor.pipeline.streamer.BaseStreamerFile.__init__.rst.txt
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/html/_sources/generated/cmoncrawl.processor.pipeline.streamer.BaseStreamerFile.clean_up.rst.txt
--rw-r--r--   0 runner    (1001) docker     (123)      247 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/html/_sources/generated/cmoncrawl.processor.pipeline.streamer.BaseStreamerFile.get_file_name.rst.txt
--rw-r--r--   0 runner    (1001) docker     (123)      262 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/html/_sources/generated/cmoncrawl.processor.pipeline.streamer.BaseStreamerFile.metadata_to_string.rst.txt
--rw-r--r--   0 runner    (1001) docker     (123)      502 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/html/_sources/generated/cmoncrawl.processor.pipeline.streamer.BaseStreamerFile.rst.txt
--rw-r--r--   0 runner    (1001) docker     (123)      222 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/html/_sources/generated/cmoncrawl.processor.pipeline.streamer.BaseStreamerFile.stream.rst.txt
--rw-r--r--   0 runner    (1001) docker     (123)      215 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/html/_sources/generated/cmoncrawl.processor.pipeline.streamer.IStreamer.__init__.rst.txt
--rw-r--r--   0 runner    (1001) docker     (123)      209 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/html/_sources/generated/cmoncrawl.processor.pipeline.streamer.IStreamer.clean_up.rst.txt
--rw-r--r--   0 runner    (1001) docker     (123)      379 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/html/_sources/generated/cmoncrawl.processor.pipeline.streamer.IStreamer.rst.txt
--rw-r--r--   0 runner    (1001) docker     (123)      201 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/html/_sources/generated/cmoncrawl.processor.pipeline.streamer.IStreamer.stream.rst.txt
--rw-r--r--   0 runner    (1001) docker     (123)      227 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/html/_sources/generated/cmoncrawl.processor.pipeline.streamer.StreamerDummy.__init__.rst.txt
--rw-r--r--   0 runner    (1001) docker     (123)      221 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/html/_sources/generated/cmoncrawl.processor.pipeline.streamer.StreamerDummy.clean_up.rst.txt
--rw-r--r--   0 runner    (1001) docker     (123)      403 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/html/_sources/generated/cmoncrawl.processor.pipeline.streamer.StreamerDummy.rst.txt
--rw-r--r--   0 runner    (1001) docker     (123)      213 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/html/_sources/generated/cmoncrawl.processor.pipeline.streamer.StreamerDummy.stream.rst.txt
--rw-r--r--   0 runner    (1001) docker     (123)      236 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/html/_sources/generated/cmoncrawl.processor.pipeline.streamer.StreamerFileHTML.__init__.rst.txt
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/html/_sources/generated/cmoncrawl.processor.pipeline.streamer.StreamerFileHTML.clean_up.rst.txt
--rw-r--r--   0 runner    (1001) docker     (123)      247 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/html/_sources/generated/cmoncrawl.processor.pipeline.streamer.StreamerFileHTML.get_file_name.rst.txt
--rw-r--r--   0 runner    (1001) docker     (123)      262 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/html/_sources/generated/cmoncrawl.processor.pipeline.streamer.StreamerFileHTML.metadata_to_string.rst.txt
--rw-r--r--   0 runner    (1001) docker     (123)      502 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/html/_sources/generated/cmoncrawl.processor.pipeline.streamer.StreamerFileHTML.rst.txt
--rw-r--r--   0 runner    (1001) docker     (123)      222 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/html/_sources/generated/cmoncrawl.processor.pipeline.streamer.StreamerFileHTML.stream.rst.txt
--rw-r--r--   0 runner    (1001) docker     (123)      236 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/html/_sources/generated/cmoncrawl.processor.pipeline.streamer.StreamerFileJSON.__init__.rst.txt
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/html/_sources/generated/cmoncrawl.processor.pipeline.streamer.StreamerFileJSON.clean_up.rst.txt
--rw-r--r--   0 runner    (1001) docker     (123)      247 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/html/_sources/generated/cmoncrawl.processor.pipeline.streamer.StreamerFileJSON.get_file_name.rst.txt
--rw-r--r--   0 runner    (1001) docker     (123)      262 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/html/_sources/generated/cmoncrawl.processor.pipeline.streamer.StreamerFileJSON.metadata_to_string.rst.txt
--rw-r--r--   0 runner    (1001) docker     (123)      502 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/html/_sources/generated/cmoncrawl.processor.pipeline.streamer.StreamerFileJSON.rst.txt
--rw-r--r--   0 runner    (1001) docker     (123)      222 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/html/_sources/generated/cmoncrawl.processor.pipeline.streamer.StreamerFileJSON.stream.rst.txt
--rw-r--r--   0 runner    (1001) docker     (123)      359 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/html/_sources/generated/cmoncrawl.processor.pipeline.streamer.rst.txt
--rw-r--r--   0 runner    (1001) docker     (123)      266 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/html/_sources/generated/cmoncrawl.processor.rst.txt
--rw-r--r--   0 runner    (1001) docker     (123)      240 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/html/_sources/generated/cmoncrawl.rst.txt
--rw-r--r--   0 runner    (1001) docker     (123)      563 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/html/_sources/index.rst.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 23:28:24.089060 CmonCrawl-1.0.1/docs/build/html/_sources/misc/
--rw-r--r--   0 runner    (1001) docker     (123)     1669 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/html/_sources/misc/domain_record.rst.txt
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/html/_sources/misc/index.rst.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 23:28:24.089060 CmonCrawl-1.0.1/docs/build/html/_sources/prog_guide/
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/html/_sources/prog_guide/index.rst.txt
--rw-r--r--   0 runner    (1001) docker     (123)     4685 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/html/_sources/prog_guide/overview.rst.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1974 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/html/_sources/prog_guide/pip.rst.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1235 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/html/_sources/usage.rst.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 23:28:24.093060 CmonCrawl-1.0.1/docs/build/html/_static/
--rw-r--r--   0 runner    (1001) docker     (123)     4418 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/html/_static/_sphinx_javascript_frameworks_compat.js
--rw-r--r--   0 runner    (1001) docker     (123)    14621 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/html/_static/basic.css
--rw-r--r--   0 runner    (1001) docker     (123)      313 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/html/_static/check-solid.svg
--rw-r--r--   0 runner    (1001) docker     (123)     9031 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/html/_static/clipboard.min.js
--rw-r--r--   0 runner    (1001) docker     (123)      411 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/html/_static/copy-button.svg
--rw-r--r--   0 runner    (1001) docker     (123)     2010 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/html/_static/copybutton.css
--rw-r--r--   0 runner    (1001) docker     (123)     7479 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/html/_static/copybutton.js
--rw-r--r--   0 runner    (1001) docker     (123)     2198 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/html/_static/copybutton_funcs.js
--rw-r--r--   0 runner    (1001) docker     (123)     4472 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/html/_static/doctools.js
--rw-r--r--   0 runner    (1001) docker     (123)      419 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/html/_static/documentation_options.js
--rw-r--r--   0 runner    (1001) docker     (123)      286 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/html/_static/file.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 23:28:24.093060 CmonCrawl-1.0.1/docs/build/html/_static/images/
--rw-r--r--   0 runner    (1001) docker     (123)     1186 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/html/_static/images/logo_binder.svg
--rw-r--r--   0 runner    (1001) docker     (123)     7601 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/html/_static/images/logo_colab.png
--rw-r--r--   0 runner    (1001) docker     (123)      681 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/html/_static/images/logo_deepnote.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1758 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/html/_static/images/logo_jupyterhub.svg
--rw-r--r--   0 runner    (1001) docker     (123)   288580 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/html/_static/jquery-3.6.0.js
--rw-r--r--   0 runner    (1001) docker     (123)    89501 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/html/_static/jquery.js
--rw-r--r--   0 runner    (1001) docker     (123)     4758 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/html/_static/language_data.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 23:28:24.041059 CmonCrawl-1.0.1/docs/build/html/_static/locales/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 23:28:24.037059 CmonCrawl-1.0.1/docs/build/html/_static/locales/ar/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 23:28:24.093060 CmonCrawl-1.0.1/docs/build/html/_static/locales/ar/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     1608 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/html/_static/locales/ar/LC_MESSAGES/booktheme.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 23:28:24.037059 CmonCrawl-1.0.1/docs/build/html/_static/locales/bg/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 23:28:24.093060 CmonCrawl-1.0.1/docs/build/html/_static/locales/bg/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     1789 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/html/_static/locales/bg/LC_MESSAGES/booktheme.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 23:28:24.037059 CmonCrawl-1.0.1/docs/build/html/_static/locales/bn/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 23:28:24.093060 CmonCrawl-1.0.1/docs/build/html/_static/locales/bn/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     1667 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/html/_static/locales/bn/LC_MESSAGES/booktheme.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 23:28:24.037059 CmonCrawl-1.0.1/docs/build/html/_static/locales/ca/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 23:28:24.093060 CmonCrawl-1.0.1/docs/build/html/_static/locales/ca/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     1231 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/html/_static/locales/ca/LC_MESSAGES/booktheme.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 23:28:24.037059 CmonCrawl-1.0.1/docs/build/html/_static/locales/cs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 23:28:24.093060 CmonCrawl-1.0.1/docs/build/html/_static/locales/cs/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     1449 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/html/_static/locales/cs/LC_MESSAGES/booktheme.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 23:28:24.037059 CmonCrawl-1.0.1/docs/build/html/_static/locales/da/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 23:28:24.093060 CmonCrawl-1.0.1/docs/build/html/_static/locales/da/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     1343 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/html/_static/locales/da/LC_MESSAGES/booktheme.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 23:28:24.037059 CmonCrawl-1.0.1/docs/build/html/_static/locales/de/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 23:28:24.093060 CmonCrawl-1.0.1/docs/build/html/_static/locales/de/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     1444 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/html/_static/locales/de/LC_MESSAGES/booktheme.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 23:28:24.037059 CmonCrawl-1.0.1/docs/build/html/_static/locales/el/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 23:28:24.093060 CmonCrawl-1.0.1/docs/build/html/_static/locales/el/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     1816 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/html/_static/locales/el/LC_MESSAGES/booktheme.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 23:28:24.037059 CmonCrawl-1.0.1/docs/build/html/_static/locales/eo/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 23:28:24.093060 CmonCrawl-1.0.1/docs/build/html/_static/locales/eo/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     1384 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/html/_static/locales/eo/LC_MESSAGES/booktheme.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 23:28:24.037059 CmonCrawl-1.0.1/docs/build/html/_static/locales/es/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 23:28:24.093060 CmonCrawl-1.0.1/docs/build/html/_static/locales/es/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     1438 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/html/_static/locales/es/LC_MESSAGES/booktheme.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 23:28:24.037059 CmonCrawl-1.0.1/docs/build/html/_static/locales/et/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 23:28:24.093060 CmonCrawl-1.0.1/docs/build/html/_static/locales/et/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     1391 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/html/_static/locales/et/LC_MESSAGES/booktheme.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 23:28:24.037059 CmonCrawl-1.0.1/docs/build/html/_static/locales/fi/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 23:28:24.093060 CmonCrawl-1.0.1/docs/build/html/_static/locales/fi/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     1409 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/html/_static/locales/fi/LC_MESSAGES/booktheme.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 23:28:24.037059 CmonCrawl-1.0.1/docs/build/html/_static/locales/fr/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 23:28:24.093060 CmonCrawl-1.0.1/docs/build/html/_static/locales/fr/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     1469 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/html/_static/locales/fr/LC_MESSAGES/booktheme.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 23:28:24.037059 CmonCrawl-1.0.1/docs/build/html/_static/locales/hr/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 23:28:24.093060 CmonCrawl-1.0.1/docs/build/html/_static/locales/hr/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     1449 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/html/_static/locales/hr/LC_MESSAGES/booktheme.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 23:28:24.037059 CmonCrawl-1.0.1/docs/build/html/_static/locales/id/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 23:28:24.093060 CmonCrawl-1.0.1/docs/build/html/_static/locales/id/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     1360 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/html/_static/locales/id/LC_MESSAGES/booktheme.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 23:28:24.037059 CmonCrawl-1.0.1/docs/build/html/_static/locales/it/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 23:28:24.093060 CmonCrawl-1.0.1/docs/build/html/_static/locales/it/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     1447 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/html/_static/locales/it/LC_MESSAGES/booktheme.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 23:28:24.037059 CmonCrawl-1.0.1/docs/build/html/_static/locales/iw/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 23:28:24.093060 CmonCrawl-1.0.1/docs/build/html/_static/locales/iw/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     1490 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/html/_static/locales/iw/LC_MESSAGES/booktheme.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 23:28:24.037059 CmonCrawl-1.0.1/docs/build/html/_static/locales/ja/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 23:28:24.093060 CmonCrawl-1.0.1/docs/build/html/_static/locales/ja/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/html/_static/locales/ja/LC_MESSAGES/booktheme.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 23:28:24.037059 CmonCrawl-1.0.1/docs/build/html/_static/locales/ko/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 23:28:24.093060 CmonCrawl-1.0.1/docs/build/html/_static/locales/ko/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     1406 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/html/_static/locales/ko/LC_MESSAGES/booktheme.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 23:28:24.037059 CmonCrawl-1.0.1/docs/build/html/_static/locales/lt/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 23:28:24.093060 CmonCrawl-1.0.1/docs/build/html/_static/locales/lt/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     1461 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/html/_static/locales/lt/LC_MESSAGES/booktheme.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 23:28:24.037059 CmonCrawl-1.0.1/docs/build/html/_static/locales/lv/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 23:28:24.093060 CmonCrawl-1.0.1/docs/build/html/_static/locales/lv/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     1450 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/html/_static/locales/lv/LC_MESSAGES/booktheme.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 23:28:24.037059 CmonCrawl-1.0.1/docs/build/html/_static/locales/ml/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 23:28:24.093060 CmonCrawl-1.0.1/docs/build/html/_static/locales/ml/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     1890 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/html/_static/locales/ml/LC_MESSAGES/booktheme.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 23:28:24.037059 CmonCrawl-1.0.1/docs/build/html/_static/locales/mr/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 23:28:24.097060 CmonCrawl-1.0.1/docs/build/html/_static/locales/mr/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     1675 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/html/_static/locales/mr/LC_MESSAGES/booktheme.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 23:28:24.037059 CmonCrawl-1.0.1/docs/build/html/_static/locales/ms/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 23:28:24.097060 CmonCrawl-1.0.1/docs/build/html/_static/locales/ms/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     1189 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/html/_static/locales/ms/LC_MESSAGES/booktheme.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 23:28:24.037059 CmonCrawl-1.0.1/docs/build/html/_static/locales/nl/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 23:28:24.097060 CmonCrawl-1.0.1/docs/build/html/_static/locales/nl/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     1398 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/html/_static/locales/nl/LC_MESSAGES/booktheme.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 23:28:24.037059 CmonCrawl-1.0.1/docs/build/html/_static/locales/no/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 23:28:24.097060 CmonCrawl-1.0.1/docs/build/html/_static/locales/no/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     1357 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/html/_static/locales/no/LC_MESSAGES/booktheme.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 23:28:24.037059 CmonCrawl-1.0.1/docs/build/html/_static/locales/pl/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 23:28:24.097060 CmonCrawl-1.0.1/docs/build/html/_static/locales/pl/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     1420 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/html/_static/locales/pl/LC_MESSAGES/booktheme.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 23:28:24.037059 CmonCrawl-1.0.1/docs/build/html/_static/locales/pt/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 23:28:24.097060 CmonCrawl-1.0.1/docs/build/html/_static/locales/pt/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     1409 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/html/_static/locales/pt/LC_MESSAGES/booktheme.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 23:28:24.041059 CmonCrawl-1.0.1/docs/build/html/_static/locales/ro/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 23:28:24.097060 CmonCrawl-1.0.1/docs/build/html/_static/locales/ro/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     1441 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/html/_static/locales/ro/LC_MESSAGES/booktheme.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 23:28:24.041059 CmonCrawl-1.0.1/docs/build/html/_static/locales/ru/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 23:28:24.097060 CmonCrawl-1.0.1/docs/build/html/_static/locales/ru/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     1797 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/html/_static/locales/ru/LC_MESSAGES/booktheme.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 23:28:24.041059 CmonCrawl-1.0.1/docs/build/html/_static/locales/sk/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 23:28:24.097060 CmonCrawl-1.0.1/docs/build/html/_static/locales/sk/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     1441 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/html/_static/locales/sk/LC_MESSAGES/booktheme.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 23:28:24.041059 CmonCrawl-1.0.1/docs/build/html/_static/locales/sl/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 23:28:24.097060 CmonCrawl-1.0.1/docs/build/html/_static/locales/sl/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     1418 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/html/_static/locales/sl/LC_MESSAGES/booktheme.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 23:28:24.041059 CmonCrawl-1.0.1/docs/build/html/_static/locales/sr/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 23:28:24.097060 CmonCrawl-1.0.1/docs/build/html/_static/locales/sr/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     1760 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/html/_static/locales/sr/LC_MESSAGES/booktheme.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 23:28:24.041059 CmonCrawl-1.0.1/docs/build/html/_static/locales/sv/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 23:28:24.097060 CmonCrawl-1.0.1/docs/build/html/_static/locales/sv/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     1391 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/html/_static/locales/sv/LC_MESSAGES/booktheme.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 23:28:24.041059 CmonCrawl-1.0.1/docs/build/html/_static/locales/ta/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 23:28:24.097060 CmonCrawl-1.0.1/docs/build/html/_static/locales/ta/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     1968 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/html/_static/locales/ta/LC_MESSAGES/booktheme.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 23:28:24.041059 CmonCrawl-1.0.1/docs/build/html/_static/locales/te/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 23:28:24.097060 CmonCrawl-1.0.1/docs/build/html/_static/locales/te/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     1834 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/html/_static/locales/te/LC_MESSAGES/booktheme.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 23:28:24.041059 CmonCrawl-1.0.1/docs/build/html/_static/locales/tg/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 23:28:24.097060 CmonCrawl-1.0.1/docs/build/html/_static/locales/tg/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     1710 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/html/_static/locales/tg/LC_MESSAGES/booktheme.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 23:28:24.041059 CmonCrawl-1.0.1/docs/build/html/_static/locales/th/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 23:28:24.097060 CmonCrawl-1.0.1/docs/build/html/_static/locales/th/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     1860 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/html/_static/locales/th/LC_MESSAGES/booktheme.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 23:28:24.041059 CmonCrawl-1.0.1/docs/build/html/_static/locales/tl/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 23:28:24.097060 CmonCrawl-1.0.1/docs/build/html/_static/locales/tl/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     1259 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/html/_static/locales/tl/LC_MESSAGES/booktheme.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 23:28:24.041059 CmonCrawl-1.0.1/docs/build/html/_static/locales/tr/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 23:28:24.097060 CmonCrawl-1.0.1/docs/build/html/_static/locales/tr/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     1405 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/html/_static/locales/tr/LC_MESSAGES/booktheme.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 23:28:24.041059 CmonCrawl-1.0.1/docs/build/html/_static/locales/uk/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 23:28:24.097060 CmonCrawl-1.0.1/docs/build/html/_static/locales/uk/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     1756 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/html/_static/locales/uk/LC_MESSAGES/booktheme.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 23:28:24.041059 CmonCrawl-1.0.1/docs/build/html/_static/locales/ur/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 23:28:24.097060 CmonCrawl-1.0.1/docs/build/html/_static/locales/ur/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     1460 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/html/_static/locales/ur/LC_MESSAGES/booktheme.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 23:28:24.041059 CmonCrawl-1.0.1/docs/build/html/_static/locales/vi/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 23:28:24.097060 CmonCrawl-1.0.1/docs/build/html/_static/locales/vi/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     1487 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/html/_static/locales/vi/LC_MESSAGES/booktheme.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 23:28:24.041059 CmonCrawl-1.0.1/docs/build/html/_static/locales/zh_CN/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 23:28:24.097060 CmonCrawl-1.0.1/docs/build/html/_static/locales/zh_CN/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     1279 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/html/_static/locales/zh_CN/LC_MESSAGES/booktheme.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 23:28:24.041059 CmonCrawl-1.0.1/docs/build/html/_static/locales/zh_TW/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 23:28:24.097060 CmonCrawl-1.0.1/docs/build/html/_static/locales/zh_TW/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     1323 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/html/_static/locales/zh_TW/LC_MESSAGES/booktheme.po
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/html/_static/minus.png
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/html/_static/plus.png
--rw-r--r--   0 runner    (1001) docker     (123)     5510 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/html/_static/pygments.css
--rw-r--r--   0 runner    (1001) docker     (123)      419 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/html/_static/sbt-webpack-macros.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 23:28:24.097060 CmonCrawl-1.0.1/docs/build/html/_static/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)    87299 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/html/_static/scripts/pydata-sphinx-theme.js
--rw-r--r--   0 runner    (1001) docker     (123)     3388 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/html/_static/scripts/sphinx-book-theme.js
--rw-r--r--   0 runner    (1001) docker     (123)    15106 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/html/_static/scripts/sphinx-book-theme.js.map
--rw-r--r--   0 runner    (1001) docker     (123)    18215 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/html/_static/searchtools.js
--rw-r--r--   0 runner    (1001) docker     (123)     4712 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/html/_static/sphinx_highlight.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 23:28:24.097060 CmonCrawl-1.0.1/docs/build/html/_static/styles/
--rw-r--r--   0 runner    (1001) docker     (123)   162094 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/html/_static/styles/pydata-sphinx-theme.css
--rw-r--r--   0 runner    (1001) docker     (123)    20970 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/html/_static/styles/sphinx-book-theme.css
--rw-r--r--   0 runner    (1001) docker     (123)     5488 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/html/_static/styles/theme.css
--rw-r--r--   0 runner    (1001) docker     (123)    68420 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/html/_static/underscore-1.13.1.js
--rw-r--r--   0 runner    (1001) docker     (123)    19530 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/html/_static/underscore.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 23:28:24.041059 CmonCrawl-1.0.1/docs/build/html/_static/vendor/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 23:28:24.041059 CmonCrawl-1.0.1/docs/build/html/_static/vendor/fontawesome/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 23:28:24.097060 CmonCrawl-1.0.1/docs/build/html/_static/vendor/fontawesome/5.13.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1548 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/html/_static/vendor/fontawesome/5.13.0/LICENSE.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 23:28:24.097060 CmonCrawl-1.0.1/docs/build/html/_static/vendor/fontawesome/5.13.0/css/
--rw-r--r--   0 runner    (1001) docker     (123)    58578 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/html/_static/vendor/fontawesome/5.13.0/css/all.min.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 23:28:24.105060 CmonCrawl-1.0.1/docs/build/html/_static/vendor/fontawesome/5.13.0/webfonts/
--rw-r--r--   0 runner    (1001) docker     (123)   133034 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/html/_static/vendor/fontawesome/5.13.0/webfonts/fa-brands-400.eot
--rw-r--r--   0 runner    (1001) docker     (123)   715890 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/html/_static/vendor/fontawesome/5.13.0/webfonts/fa-brands-400.svg
--rw-r--r--   0 runner    (1001) docker     (123)   132728 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/html/_static/vendor/fontawesome/5.13.0/webfonts/fa-brands-400.ttf
--rw-r--r--   0 runner    (1001) docker     (123)    89824 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/html/_static/vendor/fontawesome/5.13.0/webfonts/fa-brands-400.woff
--rw-r--r--   0 runner    (1001) docker     (123)    76612 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/html/_static/vendor/fontawesome/5.13.0/webfonts/fa-brands-400.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    34390 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/html/_static/vendor/fontawesome/5.13.0/webfonts/fa-regular-400.eot
--rw-r--r--   0 runner    (1001) docker     (123)   144322 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/html/_static/vendor/fontawesome/5.13.0/webfonts/fa-regular-400.svg
--rw-r--r--   0 runner    (1001) docker     (123)    34092 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/html/_static/vendor/fontawesome/5.13.0/webfonts/fa-regular-400.ttf
--rw-r--r--   0 runner    (1001) docker     (123)    16800 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/html/_static/vendor/fontawesome/5.13.0/webfonts/fa-regular-400.woff
--rw-r--r--   0 runner    (1001) docker     (123)    13584 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/html/_static/vendor/fontawesome/5.13.0/webfonts/fa-regular-400.woff2
--rw-r--r--   0 runner    (1001) docker     (123)   202902 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/html/_static/vendor/fontawesome/5.13.0/webfonts/fa-solid-900.eot
--rw-r--r--   0 runner    (1001) docker     (123)   897426 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/html/_static/vendor/fontawesome/5.13.0/webfonts/fa-solid-900.svg
--rw-r--r--   0 runner    (1001) docker     (123)   202616 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/html/_static/vendor/fontawesome/5.13.0/webfonts/fa-solid-900.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   103300 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/html/_static/vendor/fontawesome/5.13.0/webfonts/fa-solid-900.woff
--rw-r--r--   0 runner    (1001) docker     (123)    79444 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/html/_static/vendor/fontawesome/5.13.0/webfonts/fa-solid-900.woff2
--rw-r--r--   0 runner    (1001) docker     (123)     1361 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/html/_static/webpack-macros.html
--rw-r--r--   0 runner    (1001) docker     (123)    14718 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/html/api.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 23:28:24.105060 CmonCrawl-1.0.1/docs/build/html/cli/
--rw-r--r--   0 runner    (1001) docker     (123)    17247 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/html/cli/cli.html
--rw-r--r--   0 runner    (1001) docker     (123)    20066 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/html/cli/download.html
--rw-r--r--   0 runner    (1001) docker     (123)    21279 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/html/cli/extract.html
--rw-r--r--   0 runner    (1001) docker     (123)    16088 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/html/cli/index.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 23:28:24.105060 CmonCrawl-1.0.1/docs/build/html/extraction/
--rw-r--r--   0 runner    (1001) docker     (123)    25464 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/html/extraction/config_file.html
--rw-r--r--   0 runner    (1001) docker     (123)    22074 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/html/extraction/creating_extractor.html
--rw-r--r--   0 runner    (1001) docker     (123)    16080 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/html/extraction/index.html
--rw-r--r--   0 runner    (1001) docker     (123)    17188 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/html/extraction/utils.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 23:28:24.125060 CmonCrawl-1.0.1/docs/build/html/generated/
--rw-r--r--   0 runner    (1001) docker     (123)    15445 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/html/generated/cmoncrawl.aggregator.html
--rw-r--r--   0 runner    (1001) docker     (123)    20850 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/html/generated/cmoncrawl.aggregator.index_query.IndexAggregator.__init__.html
--rw-r--r--   0 runner    (1001) docker     (123)    18561 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/html/generated/cmoncrawl.aggregator.index_query.IndexAggregator.aclose.html
--rw-r--r--   0 runner    (1001) docker     (123)    17264 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/html/generated/cmoncrawl.aggregator.index_query.IndexAggregator.aopen.html
--rw-r--r--   0 runner    (1001) docker     (123)    17840 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/html/generated/cmoncrawl.aggregator.index_query.IndexAggregator.get_all_CC_indexes.html
--rw-r--r--   0 runner    (1001) docker     (123)    19556 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/html/generated/cmoncrawl.aggregator.index_query.IndexAggregator.get_captured_responses.html
--rw-r--r--   0 runner    (1001) docker     (123)    18596 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/html/generated/cmoncrawl.aggregator.index_query.IndexAggregator.get_number_of_pages.html
--rw-r--r--   0 runner    (1001) docker     (123)    28606 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/html/generated/cmoncrawl.aggregator.index_query.IndexAggregator.html
--rw-r--r--   0 runner    (1001) docker     (123)    16097 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/html/generated/cmoncrawl.aggregator.index_query.html
--rw-r--r--   0 runner    (1001) docker     (123)    15202 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/html/generated/cmoncrawl.aggregator.utils.helpers.html
--rw-r--r--   0 runner    (1001) docker     (123)    15824 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/html/generated/cmoncrawl.aggregator.utils.html
--rw-r--r--   0 runner    (1001) docker     (123)    20653 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/html/generated/cmoncrawl.aggregator.utils.ndjson_decoder.Decoder.__init__.html
--rw-r--r--   0 runner    (1001) docker     (123)    17509 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/html/generated/cmoncrawl.aggregator.utils.ndjson_decoder.Decoder.decode.html
--rw-r--r--   0 runner    (1001) docker     (123)    25373 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/html/generated/cmoncrawl.aggregator.utils.ndjson_decoder.Decoder.html
--rw-r--r--   0 runner    (1001) docker     (123)    17442 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/html/generated/cmoncrawl.aggregator.utils.ndjson_decoder.Decoder.raw_decode.html
--rw-r--r--   0 runner    (1001) docker     (123)    15546 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/html/generated/cmoncrawl.aggregator.utils.ndjson_decoder.html
--rw-r--r--   0 runner    (1001) docker     (123)    15545 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/html/generated/cmoncrawl.common.html
--rw-r--r--   0 runner    (1001) docker     (123)    14638 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/html/generated/cmoncrawl.common.loggers.html
--rw-r--r--   0 runner    (1001) docker     (123)    17736 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/html/generated/cmoncrawl.common.types.DomainCrawl.__init__.html
--rw-r--r--   0 runner    (1001) docker     (123)    21085 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/html/generated/cmoncrawl.common.types.DomainCrawl.html
--rw-r--r--   0 runner    (1001) docker     (123)    19154 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/html/generated/cmoncrawl.common.types.DomainRecord.__init__.html
--rw-r--r--   0 runner    (1001) docker     (123)    18089 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/html/generated/cmoncrawl.common.types.DomainRecord.from_dict.html
--rw-r--r--   0 runner    (1001) docker     (123)    18381 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/html/generated/cmoncrawl.common.types.DomainRecord.from_json.html
--rw-r--r--   0 runner    (1001) docker     (123)    26445 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/html/generated/cmoncrawl.common.types.DomainRecord.html
--rw-r--r--   0 runner    (1001) docker     (123)    19292 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/html/generated/cmoncrawl.common.types.DomainRecord.schema.html
--rw-r--r--   0 runner    (1001) docker     (123)    17907 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/html/generated/cmoncrawl.common.types.DomainRecord.to_dict.html
--rw-r--r--   0 runner    (1001) docker     (123)    20725 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/html/generated/cmoncrawl.common.types.DomainRecord.to_json.html
--rw-r--r--   0 runner    (1001) docker     (123)    17437 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/html/generated/cmoncrawl.common.types.ExtractConfig.__init__.html
--rw-r--r--   0 runner    (1001) docker     (123)    18110 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/html/generated/cmoncrawl.common.types.ExtractConfig.from_dict.html
--rw-r--r--   0 runner    (1001) docker     (123)    18402 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/html/generated/cmoncrawl.common.types.ExtractConfig.from_json.html
--rw-r--r--   0 runner    (1001) docker     (123)    22253 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/html/generated/cmoncrawl.common.types.ExtractConfig.html
--rw-r--r--   0 runner    (1001) docker     (123)    19313 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/html/generated/cmoncrawl.common.types.ExtractConfig.schema.html
--rw-r--r--   0 runner    (1001) docker     (123)    17928 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/html/generated/cmoncrawl.common.types.ExtractConfig.to_dict.html
--rw-r--r--   0 runner    (1001) docker     (123)    20750 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/html/generated/cmoncrawl.common.types.ExtractConfig.to_json.html
--rw-r--r--   0 runner    (1001) docker     (123)    17965 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/html/generated/cmoncrawl.common.types.ExtractorConfig.__init__.html
--rw-r--r--   0 runner    (1001) docker     (123)    18152 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/html/generated/cmoncrawl.common.types.ExtractorConfig.from_dict.html
--rw-r--r--   0 runner    (1001) docker     (123)    18444 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/html/generated/cmoncrawl.common.types.ExtractorConfig.from_json.html
--rw-r--r--   0 runner    (1001) docker     (123)    23452 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/html/generated/cmoncrawl.common.types.ExtractorConfig.html
--rw-r--r--   0 runner    (1001) docker     (123)    19355 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/html/generated/cmoncrawl.common.types.ExtractorConfig.schema.html
--rw-r--r--   0 runner    (1001) docker     (123)    17970 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/html/generated/cmoncrawl.common.types.ExtractorConfig.to_dict.html
--rw-r--r--   0 runner    (1001) docker     (123)    20772 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/html/generated/cmoncrawl.common.types.ExtractorConfig.to_json.html
--rw-r--r--   0 runner    (1001) docker     (123)    18059 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/html/generated/cmoncrawl.common.types.PipeMetadata.__init__.html
--rw-r--r--   0 runner    (1001) docker     (123)    22314 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/html/generated/cmoncrawl.common.types.PipeMetadata.html
--rw-r--r--   0 runner    (1001) docker     (123)    17470 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/html/generated/cmoncrawl.common.types.RetrieveResponse.__init__.html
--rw-r--r--   0 runner    (1001) docker     (123)    20597 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/html/generated/cmoncrawl.common.types.RetrieveResponse.html
--rw-r--r--   0 runner    (1001) docker     (123)    17108 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/html/generated/cmoncrawl.common.types.RoutesConfig.__init__.html
--rw-r--r--   0 runner    (1001) docker     (123)    18089 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/html/generated/cmoncrawl.common.types.RoutesConfig.from_dict.html
--rw-r--r--   0 runner    (1001) docker     (123)    18381 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/html/generated/cmoncrawl.common.types.RoutesConfig.from_json.html
--rw-r--r--   0 runner    (1001) docker     (123)    21617 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/html/generated/cmoncrawl.common.types.RoutesConfig.html
--rw-r--r--   0 runner    (1001) docker     (123)    19292 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/html/generated/cmoncrawl.common.types.RoutesConfig.schema.html
--rw-r--r--   0 runner    (1001) docker     (123)    17907 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/html/generated/cmoncrawl.common.types.RoutesConfig.to_dict.html
--rw-r--r--   0 runner    (1001) docker     (123)    20657 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/html/generated/cmoncrawl.common.types.RoutesConfig.to_json.html
--rw-r--r--   0 runner    (1001) docker     (123)    17489 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/html/generated/cmoncrawl.common.types.html
--rw-r--r--   0 runner    (1001) docker     (123)    15473 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/html/generated/cmoncrawl.html
--rw-r--r--   0 runner    (1001) docker     (123)    15586 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/html/generated/cmoncrawl.processor.extraction.filters.html
--rw-r--r--   0 runner    (1001) docker     (123)    15664 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/html/generated/cmoncrawl.processor.extraction.html
--rw-r--r--   0 runner    (1001) docker     (123)    17047 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/html/generated/cmoncrawl.processor.extraction.utils.html
--rw-r--r--   0 runner    (1001) docker     (123)    15567 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/html/generated/cmoncrawl.processor.html
--rw-r--r--   0 runner    (1001) docker     (123)    18794 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/html/generated/cmoncrawl.processor.pipeline.downloader.AsyncDownloader.__init__.html
--rw-r--r--   0 runner    (1001) docker     (123)    18692 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/html/generated/cmoncrawl.processor.pipeline.downloader.AsyncDownloader.aclose.html
--rw-r--r--   0 runner    (1001) docker     (123)    17371 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/html/generated/cmoncrawl.processor.pipeline.downloader.AsyncDownloader.aopen.html
--rw-r--r--   0 runner    (1001) docker     (123)    17399 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/html/generated/cmoncrawl.processor.pipeline.downloader.AsyncDownloader.download.html
--rw-r--r--   0 runner    (1001) docker     (123)    24091 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/html/generated/cmoncrawl.processor.pipeline.downloader.AsyncDownloader.html
--rw-r--r--   0 runner    (1001) docker     (123)    18163 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/html/generated/cmoncrawl.processor.pipeline.downloader.AsyncDownloader.unwrap.html
--rw-r--r--   0 runner    (1001) docker     (123)    18242 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/html/generated/cmoncrawl.processor.pipeline.downloader.DownloaderDummy.__init__.html
--rw-r--r--   0 runner    (1001) docker     (123)    17431 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/html/generated/cmoncrawl.processor.pipeline.downloader.DownloaderDummy.download.html
--rw-r--r--   0 runner    (1001) docker     (123)    17227 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/html/generated/cmoncrawl.processor.pipeline.downloader.DownloaderDummy.extract_url.html
--rw-r--r--   0 runner    (1001) docker     (123)    17249 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/html/generated/cmoncrawl.processor.pipeline.downloader.DownloaderDummy.extract_year.html
--rw-r--r--   0 runner    (1001) docker     (123)    23249 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/html/generated/cmoncrawl.processor.pipeline.downloader.DownloaderDummy.html
--rw-r--r--   0 runner    (1001) docker     (123)    17402 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/html/generated/cmoncrawl.processor.pipeline.downloader.DownloaderDummy.mine_metadata.html
--rw-r--r--   0 runner    (1001) docker     (123)    16828 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/html/generated/cmoncrawl.processor.pipeline.downloader.IDownloader.__init__.html
--rw-r--r--   0 runner    (1001) docker     (123)    17922 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/html/generated/cmoncrawl.processor.pipeline.downloader.IDownloader.download.html
--rw-r--r--   0 runner    (1001) docker     (123)    18960 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/html/generated/cmoncrawl.processor.pipeline.downloader.IDownloader.html
--rw-r--r--   0 runner    (1001) docker     (123)    16456 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/html/generated/cmoncrawl.processor.pipeline.downloader.html
--rw-r--r--   0 runner    (1001) docker     (123)    17347 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/html/generated/cmoncrawl.processor.pipeline.extractor.BaseExtractor.__init__.html
--rw-r--r--   0 runner    (1001) docker     (123)    17993 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/html/generated/cmoncrawl.processor.pipeline.extractor.BaseExtractor.extract.html
--rw-r--r--   0 runner    (1001) docker     (123)    18135 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/html/generated/cmoncrawl.processor.pipeline.extractor.BaseExtractor.extract_soup.html
--rw-r--r--   0 runner    (1001) docker     (123)    17686 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/html/generated/cmoncrawl.processor.pipeline.extractor.BaseExtractor.filter_raw.html
--rw-r--r--   0 runner    (1001) docker     (123)    17693 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/html/generated/cmoncrawl.processor.pipeline.extractor.BaseExtractor.filter_soup.html
--rw-r--r--   0 runner    (1001) docker     (123)    21657 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/html/generated/cmoncrawl.processor.pipeline.extractor.BaseExtractor.html
--rw-r--r--   0 runner    (1001) docker     (123)    17665 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/html/generated/cmoncrawl.processor.pipeline.extractor.BaseExtractor.preprocess.html
--rw-r--r--   0 runner    (1001) docker     (123)    17390 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/html/generated/cmoncrawl.processor.pipeline.extractor.DomainRecordExtractor.__init__.html
--rw-r--r--   0 runner    (1001) docker     (123)    18161 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/html/generated/cmoncrawl.processor.pipeline.extractor.DomainRecordExtractor.extract.html
--rw-r--r--   0 runner    (1001) docker     (123)    17713 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/html/generated/cmoncrawl.processor.pipeline.extractor.DomainRecordExtractor.extract_soup.html
--rw-r--r--   0 runner    (1001) docker     (123)    17705 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/html/generated/cmoncrawl.processor.pipeline.extractor.DomainRecordExtractor.filter_raw.html
--rw-r--r--   0 runner    (1001) docker     (123)    17861 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/html/generated/cmoncrawl.processor.pipeline.extractor.DomainRecordExtractor.filter_soup.html
--rw-r--r--   0 runner    (1001) docker     (123)    21894 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/html/generated/cmoncrawl.processor.pipeline.extractor.DomainRecordExtractor.html
--rw-r--r--   0 runner    (1001) docker     (123)    17769 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/html/generated/cmoncrawl.processor.pipeline.extractor.DomainRecordExtractor.preprocess.html
--rw-r--r--   0 runner    (1001) docker     (123)    17222 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/html/generated/cmoncrawl.processor.pipeline.extractor.HTMLExtractor.__init__.html
--rw-r--r--   0 runner    (1001) docker     (123)    17993 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/html/generated/cmoncrawl.processor.pipeline.extractor.HTMLExtractor.extract.html
--rw-r--r--   0 runner    (1001) docker     (123)    17545 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/html/generated/cmoncrawl.processor.pipeline.extractor.HTMLExtractor.extract_soup.html
--rw-r--r--   0 runner    (1001) docker     (123)    17537 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/html/generated/cmoncrawl.processor.pipeline.extractor.HTMLExtractor.filter_raw.html
--rw-r--r--   0 runner    (1001) docker     (123)    17693 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/html/generated/cmoncrawl.processor.pipeline.extractor.HTMLExtractor.filter_soup.html
--rw-r--r--   0 runner    (1001) docker     (123)    21598 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/html/generated/cmoncrawl.processor.pipeline.extractor.HTMLExtractor.html
--rw-r--r--   0 runner    (1001) docker     (123)    17621 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/html/generated/cmoncrawl.processor.pipeline.extractor.HTMLExtractor.preprocess.html
--rw-r--r--   0 runner    (1001) docker     (123)    16785 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/html/generated/cmoncrawl.processor.pipeline.extractor.IExtractor.__init__.html
--rw-r--r--   0 runner    (1001) docker     (123)    17913 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/html/generated/cmoncrawl.processor.pipeline.extractor.IExtractor.extract.html
--rw-r--r--   0 runner    (1001) docker     (123)    18884 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/html/generated/cmoncrawl.processor.pipeline.extractor.IExtractor.html
--rw-r--r--   0 runner    (1001) docker     (123)    16907 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/html/generated/cmoncrawl.processor.pipeline.extractor.html
--rw-r--r--   0 runner    (1001) docker     (123)    16815 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/html/generated/cmoncrawl.processor.pipeline.html
--rw-r--r--   0 runner    (1001) docker     (123)    18210 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/html/generated/cmoncrawl.processor.pipeline.pipeline.ProcessorPipeline.__init__.html
--rw-r--r--   0 runner    (1001) docker     (123)    21591 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/html/generated/cmoncrawl.processor.pipeline.pipeline.ProcessorPipeline.html
--rw-r--r--   0 runner    (1001) docker     (123)    17922 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/html/generated/cmoncrawl.processor.pipeline.pipeline.ProcessorPipeline.process_domain_record.html
--rw-r--r--   0 runner    (1001) docker     (123)    15650 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/html/generated/cmoncrawl.processor.pipeline.pipeline.html
--rw-r--r--   0 runner    (1001) docker     (123)    16660 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/html/generated/cmoncrawl.processor.pipeline.router.IRouter.__init__.html
--rw-r--r--   0 runner    (1001) docker     (123)    18604 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/html/generated/cmoncrawl.processor.pipeline.router.IRouter.html
--rw-r--r--   0 runner    (1001) docker     (123)    18128 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/html/generated/cmoncrawl.processor.pipeline.router.IRouter.route.html
--rw-r--r--   0 runner    (1001) docker     (123)    17834 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/html/generated/cmoncrawl.processor.pipeline.router.Route.__init__.html
--rw-r--r--   0 runner    (1001) docker     (123)    21472 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/html/generated/cmoncrawl.processor.pipeline.router.Route.html
--rw-r--r--   0 runner    (1001) docker     (123)    16675 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/html/generated/cmoncrawl.processor.pipeline.router.Router.__init__.html
--rw-r--r--   0 runner    (1001) docker     (123)    21103 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/html/generated/cmoncrawl.processor.pipeline.router.Router.html
--rw-r--r--   0 runner    (1001) docker     (123)    17409 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/html/generated/cmoncrawl.processor.pipeline.router.Router.load_extractor.html
--rw-r--r--   0 runner    (1001) docker     (123)    17033 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/html/generated/cmoncrawl.processor.pipeline.router.Router.load_module.html
--rw-r--r--   0 runner    (1001) docker     (123)    17142 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/html/generated/cmoncrawl.processor.pipeline.router.Router.load_module_as_extractor.html
--rw-r--r--   0 runner    (1001) docker     (123)    17041 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/html/generated/cmoncrawl.processor.pipeline.router.Router.load_modules.html
--rw-r--r--   0 runner    (1001) docker     (123)    18585 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/html/generated/cmoncrawl.processor.pipeline.router.Router.register_route.html
--rw-r--r--   0 runner    (1001) docker     (123)    17301 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/html/generated/cmoncrawl.processor.pipeline.router.Router.register_routes.html
--rw-r--r--   0 runner    (1001) docker     (123)    18040 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/html/generated/cmoncrawl.processor.pipeline.router.Router.route.html
--rw-r--r--   0 runner    (1001) docker     (123)    16303 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/html/generated/cmoncrawl.processor.pipeline.router.html
--rw-r--r--   0 runner    (1001) docker     (123)    18500 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/html/generated/cmoncrawl.processor.pipeline.streamer.BaseStreamerFile.__init__.html
--rw-r--r--   0 runner    (1001) docker     (123)    17190 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/html/generated/cmoncrawl.processor.pipeline.streamer.BaseStreamerFile.clean_up.html
--rw-r--r--   0 runner    (1001) docker     (123)    17424 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/html/generated/cmoncrawl.processor.pipeline.streamer.BaseStreamerFile.get_file_name.html
--rw-r--r--   0 runner    (1001) docker     (123)    23620 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/html/generated/cmoncrawl.processor.pipeline.streamer.BaseStreamerFile.html
--rw-r--r--   0 runner    (1001) docker     (123)    17755 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/html/generated/cmoncrawl.processor.pipeline.streamer.BaseStreamerFile.metadata_to_string.html
--rw-r--r--   0 runner    (1001) docker     (123)    17941 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/html/generated/cmoncrawl.processor.pipeline.streamer.BaseStreamerFile.stream.html
--rw-r--r--   0 runner    (1001) docker     (123)    16750 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/html/generated/cmoncrawl.processor.pipeline.streamer.IStreamer.__init__.html
--rw-r--r--   0 runner    (1001) docker     (123)    17072 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/html/generated/cmoncrawl.processor.pipeline.streamer.IStreamer.clean_up.html
--rw-r--r--   0 runner    (1001) docker     (123)    19248 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/html/generated/cmoncrawl.processor.pipeline.streamer.IStreamer.html
--rw-r--r--   0 runner    (1001) docker     (123)    17855 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/html/generated/cmoncrawl.processor.pipeline.streamer.IStreamer.stream.html
--rw-r--r--   0 runner    (1001) docker     (123)    16834 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/html/generated/cmoncrawl.processor.pipeline.streamer.StreamerDummy.__init__.html
--rw-r--r--   0 runner    (1001) docker     (123)    16950 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/html/generated/cmoncrawl.processor.pipeline.streamer.StreamerDummy.clean_up.html
--rw-r--r--   0 runner    (1001) docker     (123)    19364 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/html/generated/cmoncrawl.processor.pipeline.streamer.StreamerDummy.html
--rw-r--r--   0 runner    (1001) docker     (123)    17729 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/html/generated/cmoncrawl.processor.pipeline.streamer.StreamerDummy.stream.html
--rw-r--r--   0 runner    (1001) docker     (123)    17320 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/html/generated/cmoncrawl.processor.pipeline.streamer.StreamerFileHTML.__init__.html
--rw-r--r--   0 runner    (1001) docker     (123)    17190 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/html/generated/cmoncrawl.processor.pipeline.streamer.StreamerFileHTML.clean_up.html
--rw-r--r--   0 runner    (1001) docker     (123)    17424 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/html/generated/cmoncrawl.processor.pipeline.streamer.StreamerFileHTML.get_file_name.html
--rw-r--r--   0 runner    (1001) docker     (123)    21251 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/html/generated/cmoncrawl.processor.pipeline.streamer.StreamerFileHTML.html
--rw-r--r--   0 runner    (1001) docker     (123)    17672 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/html/generated/cmoncrawl.processor.pipeline.streamer.StreamerFileHTML.metadata_to_string.html
--rw-r--r--   0 runner    (1001) docker     (123)    17969 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/html/generated/cmoncrawl.processor.pipeline.streamer.StreamerFileHTML.stream.html
--rw-r--r--   0 runner    (1001) docker     (123)    17904 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/html/generated/cmoncrawl.processor.pipeline.streamer.StreamerFileJSON.__init__.html
--rw-r--r--   0 runner    (1001) docker     (123)    17190 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/html/generated/cmoncrawl.processor.pipeline.streamer.StreamerFileJSON.clean_up.html
--rw-r--r--   0 runner    (1001) docker     (123)    17424 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/html/generated/cmoncrawl.processor.pipeline.streamer.StreamerFileJSON.get_file_name.html
--rw-r--r--   0 runner    (1001) docker     (123)    22447 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/html/generated/cmoncrawl.processor.pipeline.streamer.StreamerFileJSON.html
--rw-r--r--   0 runner    (1001) docker     (123)    17672 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/html/generated/cmoncrawl.processor.pipeline.streamer.StreamerFileJSON.metadata_to_string.html
--rw-r--r--   0 runner    (1001) docker     (123)    17455 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/html/generated/cmoncrawl.processor.pipeline.streamer.StreamerFileJSON.stream.html
--rw-r--r--   0 runner    (1001) docker     (123)    17327 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/html/generated/cmoncrawl.processor.pipeline.streamer.html
--rw-r--r--   0 runner    (1001) docker     (123)    55272 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/html/genindex.html
--rw-r--r--   0 runner    (1001) docker     (123)    22125 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/html/index.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 23:28:24.125060 CmonCrawl-1.0.1/docs/build/html/misc/
--rw-r--r--   0 runner    (1001) docker     (123)    18439 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/html/misc/domain_record.html
--rw-r--r--   0 runner    (1001) docker     (123)    14882 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/html/misc/index.html
--rw-r--r--   0 runner    (1001) docker     (123)    13098 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/html/objects.inv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 23:28:24.125060 CmonCrawl-1.0.1/docs/build/html/prog_guide/
--rw-r--r--   0 runner    (1001) docker     (123)    16012 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/html/prog_guide/index.html
--rw-r--r--   0 runner    (1001) docker     (123)    26474 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/html/prog_guide/overview.html
--rw-r--r--   0 runner    (1001) docker     (123)    21406 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/html/prog_guide/pip.html
--rw-r--r--   0 runner    (1001) docker     (123)    17907 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/html/py-modindex.html
--rw-r--r--   0 runner    (1001) docker     (123)    13230 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/html/search.html
--rw-r--r--   0 runner    (1001) docker     (123)    99618 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/html/searchindex.js
--rw-r--r--   0 runner    (1001) docker     (123)    17202 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/build/html/usage.html
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/index.html
--rw-r--r--   0 runner    (1001) docker     (123)      769 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 23:28:24.125060 CmonCrawl-1.0.1/docs/source/
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/source/api.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 23:28:24.125060 CmonCrawl-1.0.1/docs/source/cli/
--rw-r--r--   0 runner    (1001) docker     (123)     1175 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/source/cli/cli.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1987 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/source/cli/download.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2753 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/source/cli/extract.rst
--rw-r--r--   0 runner    (1001) docker     (123)      137 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/source/cli/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2484 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/source/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 23:28:24.125060 CmonCrawl-1.0.1/docs/source/extraction/
--rw-r--r--   0 runner    (1001) docker     (123)     3910 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/source/extraction/config_file.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2392 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/source/extraction/creating_extractor.rst
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/source/extraction/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      861 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/source/extraction/utils.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 23:28:24.141061 CmonCrawl-1.0.1/docs/source/generated/
--rw-r--r--   0 runner    (1001) docker     (123)      220 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/source/generated/cmoncrawl.aggregator.index_query.IndexAggregator.__init__.rst
--rw-r--r--   0 runner    (1001) docker     (123)      206 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/source/generated/cmoncrawl.aggregator.index_query.IndexAggregator.aclose.rst
--rw-r--r--   0 runner    (1001) docker     (123)      203 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/source/generated/cmoncrawl.aggregator.index_query.IndexAggregator.aopen.rst
--rw-r--r--   0 runner    (1001) docker     (123)      248 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/source/generated/cmoncrawl.aggregator.index_query.IndexAggregator.get_all_CC_indexes.rst
--rw-r--r--   0 runner    (1001) docker     (123)      258 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/source/generated/cmoncrawl.aggregator.index_query.IndexAggregator.get_captured_responses.rst
--rw-r--r--   0 runner    (1001) docker     (123)      251 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/source/generated/cmoncrawl.aggregator.index_query.IndexAggregator.get_number_of_pages.rst
--rw-r--r--   0 runner    (1001) docker     (123)      530 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/source/generated/cmoncrawl.aggregator.index_query.IndexAggregator.rst
--rw-r--r--   0 runner    (1001) docker     (123)      391 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/source/generated/cmoncrawl.aggregator.index_query.rst
--rw-r--r--   0 runner    (1001) docker     (123)      269 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/source/generated/cmoncrawl.aggregator.rst
--rw-r--r--   0 runner    (1001) docker     (123)      250 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/source/generated/cmoncrawl.aggregator.utils.helpers.rst
--rw-r--r--   0 runner    (1001) docker     (123)      223 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/source/generated/cmoncrawl.aggregator.utils.ndjson_decoder.Decoder.__init__.rst
--rw-r--r--   0 runner    (1001) docker     (123)      209 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/source/generated/cmoncrawl.aggregator.utils.ndjson_decoder.Decoder.decode.rst
--rw-r--r--   0 runner    (1001) docker     (123)      223 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/source/generated/cmoncrawl.aggregator.utils.ndjson_decoder.Decoder.raw_decode.rst
--rw-r--r--   0 runner    (1001) docker     (123)      383 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/source/generated/cmoncrawl.aggregator.utils.ndjson_decoder.Decoder.rst
--rw-r--r--   0 runner    (1001) docker     (123)      282 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/source/generated/cmoncrawl.aggregator.utils.ndjson_decoder.rst
--rw-r--r--   0 runner    (1001) docker     (123)      304 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/source/generated/cmoncrawl.aggregator.utils.rst
--rw-r--r--   0 runner    (1001) docker     (123)      147 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/source/generated/cmoncrawl.common.loggers.rst
--rw-r--r--   0 runner    (1001) docker     (123)      245 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/source/generated/cmoncrawl.common.rst
--rw-r--r--   0 runner    (1001) docker     (123)      176 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/source/generated/cmoncrawl.common.types.DomainCrawl.__init__.rst
--rw-r--r--   0 runner    (1001) docker     (123)      427 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/source/generated/cmoncrawl.common.types.DomainCrawl.rst
--rw-r--r--   0 runner    (1001) docker     (123)      179 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/source/generated/cmoncrawl.common.types.DomainRecord.__init__.rst
--rw-r--r--   0 runner    (1001) docker     (123)      176 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/source/generated/cmoncrawl.common.types.DomainRecord.from_dict.rst
--rw-r--r--   0 runner    (1001) docker     (123)      176 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/source/generated/cmoncrawl.common.types.DomainRecord.from_json.rst
--rw-r--r--   0 runner    (1001) docker     (123)      687 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/source/generated/cmoncrawl.common.types.DomainRecord.rst
--rw-r--r--   0 runner    (1001) docker     (123)      165 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/source/generated/cmoncrawl.common.types.DomainRecord.schema.rst
--rw-r--r--   0 runner    (1001) docker     (123)      170 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/source/generated/cmoncrawl.common.types.DomainRecord.to_dict.rst
--rw-r--r--   0 runner    (1001) docker     (123)      170 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/source/generated/cmoncrawl.common.types.DomainRecord.to_json.rst
--rw-r--r--   0 runner    (1001) docker     (123)      182 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/source/generated/cmoncrawl.common.types.ExtractConfig.__init__.rst
--rw-r--r--   0 runner    (1001) docker     (123)      179 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/source/generated/cmoncrawl.common.types.ExtractConfig.from_dict.rst
--rw-r--r--   0 runner    (1001) docker     (123)      179 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/source/generated/cmoncrawl.common.types.ExtractConfig.from_json.rst
--rw-r--r--   0 runner    (1001) docker     (123)      568 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/source/generated/cmoncrawl.common.types.ExtractConfig.rst
--rw-r--r--   0 runner    (1001) docker     (123)      168 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/source/generated/cmoncrawl.common.types.ExtractConfig.schema.rst
--rw-r--r--   0 runner    (1001) docker     (123)      173 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/source/generated/cmoncrawl.common.types.ExtractConfig.to_dict.rst
--rw-r--r--   0 runner    (1001) docker     (123)      173 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/source/generated/cmoncrawl.common.types.ExtractConfig.to_json.rst
--rw-r--r--   0 runner    (1001) docker     (123)      188 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/source/generated/cmoncrawl.common.types.ExtractorConfig.__init__.rst
--rw-r--r--   0 runner    (1001) docker     (123)      185 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/source/generated/cmoncrawl.common.types.ExtractorConfig.from_dict.rst
--rw-r--r--   0 runner    (1001) docker     (123)      185 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/source/generated/cmoncrawl.common.types.ExtractorConfig.from_json.rst
--rw-r--r--   0 runner    (1001) docker     (123)      604 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/source/generated/cmoncrawl.common.types.ExtractorConfig.rst
--rw-r--r--   0 runner    (1001) docker     (123)      174 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/source/generated/cmoncrawl.common.types.ExtractorConfig.schema.rst
--rw-r--r--   0 runner    (1001) docker     (123)      179 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/source/generated/cmoncrawl.common.types.ExtractorConfig.to_dict.rst
--rw-r--r--   0 runner    (1001) docker     (123)      179 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/source/generated/cmoncrawl.common.types.ExtractorConfig.to_json.rst
--rw-r--r--   0 runner    (1001) docker     (123)      179 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/source/generated/cmoncrawl.common.types.PipeMetadata.__init__.rst
--rw-r--r--   0 runner    (1001) docker     (123)      536 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/source/generated/cmoncrawl.common.types.PipeMetadata.rst
--rw-r--r--   0 runner    (1001) docker     (123)      191 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/source/generated/cmoncrawl.common.types.RetrieveResponse.__init__.rst
--rw-r--r--   0 runner    (1001) docker     (123)      461 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/source/generated/cmoncrawl.common.types.RetrieveResponse.rst
--rw-r--r--   0 runner    (1001) docker     (123)      179 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/source/generated/cmoncrawl.common.types.RoutesConfig.__init__.rst
--rw-r--r--   0 runner    (1001) docker     (123)      176 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/source/generated/cmoncrawl.common.types.RoutesConfig.from_dict.rst
--rw-r--r--   0 runner    (1001) docker     (123)      176 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/source/generated/cmoncrawl.common.types.RoutesConfig.from_json.rst
--rw-r--r--   0 runner    (1001) docker     (123)      553 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/source/generated/cmoncrawl.common.types.RoutesConfig.rst
--rw-r--r--   0 runner    (1001) docker     (123)      165 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/source/generated/cmoncrawl.common.types.RoutesConfig.schema.rst
--rw-r--r--   0 runner    (1001) docker     (123)      170 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/source/generated/cmoncrawl.common.types.RoutesConfig.to_dict.rst
--rw-r--r--   0 runner    (1001) docker     (123)      170 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/source/generated/cmoncrawl.common.types.RoutesConfig.to_json.rst
--rw-r--r--   0 runner    (1001) docker     (123)      349 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/source/generated/cmoncrawl.common.types.rst
--rw-r--r--   0 runner    (1001) docker     (123)      295 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/source/generated/cmoncrawl.processor.extraction.filters.rst
--rw-r--r--   0 runner    (1001) docker     (123)      315 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/source/generated/cmoncrawl.processor.extraction.rst
--rw-r--r--   0 runner    (1001) docker     (123)      500 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/source/generated/cmoncrawl.processor.extraction.utils.rst
--rw-r--r--   0 runner    (1001) docker     (123)      239 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/source/generated/cmoncrawl.processor.pipeline.downloader.AsyncDownloader.__init__.rst
--rw-r--r--   0 runner    (1001) docker     (123)      225 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/source/generated/cmoncrawl.processor.pipeline.downloader.AsyncDownloader.aclose.rst
--rw-r--r--   0 runner    (1001) docker     (123)      222 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/source/generated/cmoncrawl.processor.pipeline.downloader.AsyncDownloader.aopen.rst
--rw-r--r--   0 runner    (1001) docker     (123)      231 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/source/generated/cmoncrawl.processor.pipeline.downloader.AsyncDownloader.download.rst
--rw-r--r--   0 runner    (1001) docker     (123)      480 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/source/generated/cmoncrawl.processor.pipeline.downloader.AsyncDownloader.rst
--rw-r--r--   0 runner    (1001) docker     (123)      225 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/source/generated/cmoncrawl.processor.pipeline.downloader.AsyncDownloader.unwrap.rst
--rw-r--r--   0 runner    (1001) docker     (123)      239 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/source/generated/cmoncrawl.processor.pipeline.downloader.DownloaderDummy.__init__.rst
--rw-r--r--   0 runner    (1001) docker     (123)      231 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/source/generated/cmoncrawl.processor.pipeline.downloader.DownloaderDummy.download.rst
--rw-r--r--   0 runner    (1001) docker     (123)      242 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/source/generated/cmoncrawl.processor.pipeline.downloader.DownloaderDummy.extract_url.rst
--rw-r--r--   0 runner    (1001) docker     (123)      245 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/source/generated/cmoncrawl.processor.pipeline.downloader.DownloaderDummy.extract_year.rst
--rw-r--r--   0 runner    (1001) docker     (123)      248 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/source/generated/cmoncrawl.processor.pipeline.downloader.DownloaderDummy.mine_metadata.rst
--rw-r--r--   0 runner    (1001) docker     (123)      499 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/source/generated/cmoncrawl.processor.pipeline.downloader.DownloaderDummy.rst
--rw-r--r--   0 runner    (1001) docker     (123)      227 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/source/generated/cmoncrawl.processor.pipeline.downloader.IDownloader.__init__.rst
--rw-r--r--   0 runner    (1001) docker     (123)      219 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/source/generated/cmoncrawl.processor.pipeline.downloader.IDownloader.download.rst
--rw-r--r--   0 runner    (1001) docker     (123)      371 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/source/generated/cmoncrawl.processor.pipeline.downloader.IDownloader.rst
--rw-r--r--   0 runner    (1001) docker     (123)      322 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/source/generated/cmoncrawl.processor.pipeline.downloader.rst
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/source/generated/cmoncrawl.processor.pipeline.extractor.BaseExtractor.__init__.rst
--rw-r--r--   0 runner    (1001) docker     (123)      219 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/source/generated/cmoncrawl.processor.pipeline.extractor.BaseExtractor.extract.rst
--rw-r--r--   0 runner    (1001) docker     (123)      236 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/source/generated/cmoncrawl.processor.pipeline.extractor.BaseExtractor.extract_soup.rst
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/source/generated/cmoncrawl.processor.pipeline.extractor.BaseExtractor.filter_raw.rst
--rw-r--r--   0 runner    (1001) docker     (123)      233 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/source/generated/cmoncrawl.processor.pipeline.extractor.BaseExtractor.filter_soup.rst
--rw-r--r--   0 runner    (1001) docker     (123)      228 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/source/generated/cmoncrawl.processor.pipeline.extractor.BaseExtractor.preprocess.rst
--rw-r--r--   0 runner    (1001) docker     (123)      508 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/source/generated/cmoncrawl.processor.pipeline.extractor.BaseExtractor.rst
--rw-r--r--   0 runner    (1001) docker     (123)      254 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/source/generated/cmoncrawl.processor.pipeline.extractor.DomainRecordExtractor.__init__.rst
--rw-r--r--   0 runner    (1001) docker     (123)      243 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/source/generated/cmoncrawl.processor.pipeline.extractor.DomainRecordExtractor.extract.rst
--rw-r--r--   0 runner    (1001) docker     (123)      260 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/source/generated/cmoncrawl.processor.pipeline.extractor.DomainRecordExtractor.extract_soup.rst
--rw-r--r--   0 runner    (1001) docker     (123)      254 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/source/generated/cmoncrawl.processor.pipeline.extractor.DomainRecordExtractor.filter_raw.rst
--rw-r--r--   0 runner    (1001) docker     (123)      257 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/source/generated/cmoncrawl.processor.pipeline.extractor.DomainRecordExtractor.filter_soup.rst
--rw-r--r--   0 runner    (1001) docker     (123)      252 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/source/generated/cmoncrawl.processor.pipeline.extractor.DomainRecordExtractor.preprocess.rst
--rw-r--r--   0 runner    (1001) docker     (123)      580 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/source/generated/cmoncrawl.processor.pipeline.extractor.DomainRecordExtractor.rst
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/source/generated/cmoncrawl.processor.pipeline.extractor.HTMLExtractor.__init__.rst
--rw-r--r--   0 runner    (1001) docker     (123)      219 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/source/generated/cmoncrawl.processor.pipeline.extractor.HTMLExtractor.extract.rst
--rw-r--r--   0 runner    (1001) docker     (123)      236 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/source/generated/cmoncrawl.processor.pipeline.extractor.HTMLExtractor.extract_soup.rst
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/source/generated/cmoncrawl.processor.pipeline.extractor.HTMLExtractor.filter_raw.rst
--rw-r--r--   0 runner    (1001) docker     (123)      233 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/source/generated/cmoncrawl.processor.pipeline.extractor.HTMLExtractor.filter_soup.rst
--rw-r--r--   0 runner    (1001) docker     (123)      228 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/source/generated/cmoncrawl.processor.pipeline.extractor.HTMLExtractor.preprocess.rst
--rw-r--r--   0 runner    (1001) docker     (123)      508 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/source/generated/cmoncrawl.processor.pipeline.extractor.HTMLExtractor.rst
--rw-r--r--   0 runner    (1001) docker     (123)      221 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/source/generated/cmoncrawl.processor.pipeline.extractor.IExtractor.__init__.rst
--rw-r--r--   0 runner    (1001) docker     (123)      210 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/source/generated/cmoncrawl.processor.pipeline.extractor.IExtractor.extract.rst
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/source/generated/cmoncrawl.processor.pipeline.extractor.IExtractor.rst
--rw-r--r--   0 runner    (1001) docker     (123)      342 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/source/generated/cmoncrawl.processor.pipeline.extractor.rst
--rw-r--r--   0 runner    (1001) docker     (123)      239 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/source/generated/cmoncrawl.processor.pipeline.pipeline.ProcessorPipeline.__init__.rst
--rw-r--r--   0 runner    (1001) docker     (123)      274 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/source/generated/cmoncrawl.processor.pipeline.pipeline.ProcessorPipeline.process_domain_record.rst
--rw-r--r--   0 runner    (1001) docker     (123)      408 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/source/generated/cmoncrawl.processor.pipeline.pipeline.ProcessorPipeline.rst
--rw-r--r--   0 runner    (1001) docker     (123)      278 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/source/generated/cmoncrawl.processor.pipeline.pipeline.rst
--rw-r--r--   0 runner    (1001) docker     (123)      203 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/source/generated/cmoncrawl.processor.pipeline.router.IRouter.__init__.rst
--rw-r--r--   0 runner    (1001) docker     (123)      186 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/source/generated/cmoncrawl.processor.pipeline.router.IRouter.route.rst
--rw-r--r--   0 runner    (1001) docker     (123)      336 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/source/generated/cmoncrawl.processor.pipeline.router.IRouter.rst
--rw-r--r--   0 runner    (1001) docker     (123)      197 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/source/generated/cmoncrawl.processor.pipeline.router.Route.__init__.rst
--rw-r--r--   0 runner    (1001) docker     (123)      436 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/source/generated/cmoncrawl.processor.pipeline.router.Route.rst
--rw-r--r--   0 runner    (1001) docker     (123)      200 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/source/generated/cmoncrawl.processor.pipeline.router.Router.__init__.rst
--rw-r--r--   0 runner    (1001) docker     (123)      212 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/source/generated/cmoncrawl.processor.pipeline.router.Router.load_extractor.rst
--rw-r--r--   0 runner    (1001) docker     (123)      203 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/source/generated/cmoncrawl.processor.pipeline.router.Router.load_module.rst
--rw-r--r--   0 runner    (1001) docker     (123)      246 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/source/generated/cmoncrawl.processor.pipeline.router.Router.load_module_as_extractor.rst
--rw-r--r--   0 runner    (1001) docker     (123)      206 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/source/generated/cmoncrawl.processor.pipeline.router.Router.load_modules.rst
--rw-r--r--   0 runner    (1001) docker     (123)      212 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/source/generated/cmoncrawl.processor.pipeline.router.Router.register_route.rst
--rw-r--r--   0 runner    (1001) docker     (123)      215 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/source/generated/cmoncrawl.processor.pipeline.router.Router.register_routes.rst
--rw-r--r--   0 runner    (1001) docker     (123)      183 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/source/generated/cmoncrawl.processor.pipeline.router.Router.route.rst
--rw-r--r--   0 runner    (1001) docker     (123)      511 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/source/generated/cmoncrawl.processor.pipeline.router.Router.rst
--rw-r--r--   0 runner    (1001) docker     (123)      287 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/source/generated/cmoncrawl.processor.pipeline.router.rst
--rw-r--r--   0 runner    (1001) docker     (123)      433 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/source/generated/cmoncrawl.processor.pipeline.rst
--rw-r--r--   0 runner    (1001) docker     (123)      236 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/source/generated/cmoncrawl.processor.pipeline.streamer.BaseStreamerFile.__init__.rst
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/source/generated/cmoncrawl.processor.pipeline.streamer.BaseStreamerFile.clean_up.rst
--rw-r--r--   0 runner    (1001) docker     (123)      247 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/source/generated/cmoncrawl.processor.pipeline.streamer.BaseStreamerFile.get_file_name.rst
--rw-r--r--   0 runner    (1001) docker     (123)      262 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/source/generated/cmoncrawl.processor.pipeline.streamer.BaseStreamerFile.metadata_to_string.rst
--rw-r--r--   0 runner    (1001) docker     (123)      502 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/source/generated/cmoncrawl.processor.pipeline.streamer.BaseStreamerFile.rst
--rw-r--r--   0 runner    (1001) docker     (123)      222 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/source/generated/cmoncrawl.processor.pipeline.streamer.BaseStreamerFile.stream.rst
--rw-r--r--   0 runner    (1001) docker     (123)      215 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/source/generated/cmoncrawl.processor.pipeline.streamer.IStreamer.__init__.rst
--rw-r--r--   0 runner    (1001) docker     (123)      209 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/source/generated/cmoncrawl.processor.pipeline.streamer.IStreamer.clean_up.rst
--rw-r--r--   0 runner    (1001) docker     (123)      379 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/source/generated/cmoncrawl.processor.pipeline.streamer.IStreamer.rst
--rw-r--r--   0 runner    (1001) docker     (123)      201 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/source/generated/cmoncrawl.processor.pipeline.streamer.IStreamer.stream.rst
--rw-r--r--   0 runner    (1001) docker     (123)      227 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/source/generated/cmoncrawl.processor.pipeline.streamer.StreamerDummy.__init__.rst
--rw-r--r--   0 runner    (1001) docker     (123)      221 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/source/generated/cmoncrawl.processor.pipeline.streamer.StreamerDummy.clean_up.rst
--rw-r--r--   0 runner    (1001) docker     (123)      403 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/source/generated/cmoncrawl.processor.pipeline.streamer.StreamerDummy.rst
--rw-r--r--   0 runner    (1001) docker     (123)      213 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/source/generated/cmoncrawl.processor.pipeline.streamer.StreamerDummy.stream.rst
--rw-r--r--   0 runner    (1001) docker     (123)      236 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/source/generated/cmoncrawl.processor.pipeline.streamer.StreamerFileHTML.__init__.rst
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/source/generated/cmoncrawl.processor.pipeline.streamer.StreamerFileHTML.clean_up.rst
--rw-r--r--   0 runner    (1001) docker     (123)      247 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/source/generated/cmoncrawl.processor.pipeline.streamer.StreamerFileHTML.get_file_name.rst
--rw-r--r--   0 runner    (1001) docker     (123)      262 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/source/generated/cmoncrawl.processor.pipeline.streamer.StreamerFileHTML.metadata_to_string.rst
--rw-r--r--   0 runner    (1001) docker     (123)      502 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/source/generated/cmoncrawl.processor.pipeline.streamer.StreamerFileHTML.rst
--rw-r--r--   0 runner    (1001) docker     (123)      222 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/source/generated/cmoncrawl.processor.pipeline.streamer.StreamerFileHTML.stream.rst
--rw-r--r--   0 runner    (1001) docker     (123)      236 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/source/generated/cmoncrawl.processor.pipeline.streamer.StreamerFileJSON.__init__.rst
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/source/generated/cmoncrawl.processor.pipeline.streamer.StreamerFileJSON.clean_up.rst
--rw-r--r--   0 runner    (1001) docker     (123)      247 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/source/generated/cmoncrawl.processor.pipeline.streamer.StreamerFileJSON.get_file_name.rst
--rw-r--r--   0 runner    (1001) docker     (123)      262 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/source/generated/cmoncrawl.processor.pipeline.streamer.StreamerFileJSON.metadata_to_string.rst
--rw-r--r--   0 runner    (1001) docker     (123)      502 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/source/generated/cmoncrawl.processor.pipeline.streamer.StreamerFileJSON.rst
--rw-r--r--   0 runner    (1001) docker     (123)      222 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/source/generated/cmoncrawl.processor.pipeline.streamer.StreamerFileJSON.stream.rst
--rw-r--r--   0 runner    (1001) docker     (123)      359 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/source/generated/cmoncrawl.processor.pipeline.streamer.rst
--rw-r--r--   0 runner    (1001) docker     (123)      266 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/source/generated/cmoncrawl.processor.rst
--rw-r--r--   0 runner    (1001) docker     (123)      240 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/source/generated/cmoncrawl.rst
--rw-r--r--   0 runner    (1001) docker     (123)      563 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/source/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 23:28:24.141061 CmonCrawl-1.0.1/docs/source/misc/
--rw-r--r--   0 runner    (1001) docker     (123)     1669 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/source/misc/domain_record.rst
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/source/misc/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 23:28:24.141061 CmonCrawl-1.0.1/docs/source/prog_guide/
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/source/prog_guide/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4685 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/source/prog_guide/overview.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1974 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/source/prog_guide/pip.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1235 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/docs/source/usage.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 23:28:24.041059 CmonCrawl-1.0.1/examples/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 23:28:24.141061 CmonCrawl-1.0.1/examples/extractor_tutorial/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 23:28:24.141061 CmonCrawl-1.0.1/examples/extractor_tutorial/Extractors/
--rw-r--r--   0 runner    (1001) docker     (123)     1357 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/examples/extractor_tutorial/Extractors/bbc_extractor.py
--rw-r--r--   0 runner    (1001) docker     (123)      181 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/examples/extractor_tutorial/config.json
--rw-r--r--   0 runner    (1001) docker     (123)      887 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      446 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-12 23:28:24.145061 CmonCrawl-1.0.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 23:28:24.141061 CmonCrawl-1.0.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     7349 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/tests/aggregator_tests.py
--rw-r--r--   0 runner    (1001) docker     (123)     3003 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/tests/end_to_end_tests.py
--rw-r--r--   0 runner    (1001) docker     (123)     4642 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/tests/processor_tests.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 23:28:24.141061 CmonCrawl-1.0.1/tests/test_extract/
--rw-r--r--   0 runner    (1001) docker     (123)      272 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/tests/test_extract/cfg.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 23:28:24.141061 CmonCrawl-1.0.1/tests/test_extract/extractors/
--rw-r--r--   0 runner    (1001) docker     (123)      495 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/tests/test_extract/extractors/test_extract.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 23:28:24.145061 CmonCrawl-1.0.1/tests/test_extract/files/
--rw-r--r--   0 runner    (1001) docker     (123)   828135 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/tests/test_extract/files/file.html
--rw-r--r--   0 runner    (1001) docker     (123)  1743032 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/tests/test_extract/files/file.jsonl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 23:28:24.145061 CmonCrawl-1.0.1/tests/test_routes/
--rw-r--r--   0 runner    (1001) docker     (123)      401 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/tests/test_routes/a.py
--rw-r--r--   0 runner    (1001) docker     (123)      400 2023-05-12 23:28:09.000000 CmonCrawl-1.0.1/tests/test_routes/b.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 20:28:44.433698 CmonCrawl-1.0.2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 20:28:44.201687 CmonCrawl-1.0.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 20:28:44.233688 CmonCrawl-1.0.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1021 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1194 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/.github/workflows/test_and_types.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3078 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      377 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/.pre-commit-config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 20:28:44.233688 CmonCrawl-1.0.2/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (123)     1367 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/.vscode/launch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      459 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/.vscode/settings.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 20:28:44.237689 CmonCrawl-1.0.2/CmonCrawl.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5835 2023-05-22 20:28:44.000000 CmonCrawl-1.0.2/CmonCrawl.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    61037 2023-05-22 20:28:44.000000 CmonCrawl-1.0.2/CmonCrawl.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 20:28:44.000000 CmonCrawl-1.0.2/CmonCrawl.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-05-22 20:28:44.000000 CmonCrawl-1.0.2/CmonCrawl.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      446 2023-05-22 20:28:44.000000 CmonCrawl-1.0.2/CmonCrawl.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-22 20:28:44.000000 CmonCrawl-1.0.2/CmonCrawl.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5835 2023-05-22 20:28:44.433698 CmonCrawl-1.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4102 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 20:28:44.237689 CmonCrawl-1.0.2/cmoncrawl/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/cmoncrawl/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 20:28:44.237689 CmonCrawl-1.0.2/cmoncrawl/aggregator/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 20:28:44.237689 CmonCrawl-1.0.2/cmoncrawl/aggregator/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (123)      215 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/cmoncrawl/aggregator/.vscode/settings.json
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/cmoncrawl/aggregator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16530 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/cmoncrawl/aggregator/index_query.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 20:28:44.237689 CmonCrawl-1.0.2/cmoncrawl/aggregator/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/cmoncrawl/aggregator/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      865 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/cmoncrawl/aggregator/utils/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/cmoncrawl/aggregator/utils/ndjson.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 20:28:44.241689 CmonCrawl-1.0.2/cmoncrawl/common/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/cmoncrawl/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      996 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/cmoncrawl/common/loggers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2305 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/cmoncrawl/common/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 20:28:44.241689 CmonCrawl-1.0.2/cmoncrawl/integrations/
+-rw-r--r--   0 runner    (1001) docker     (123)     1439 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/cmoncrawl/integrations/commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6558 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/cmoncrawl/integrations/download.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6723 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/cmoncrawl/integrations/extract.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 20:28:44.241689 CmonCrawl-1.0.2/cmoncrawl/middleware/
+-rw-r--r--   0 runner    (1001) docker     (123)    12291 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/cmoncrawl/middleware/stompware.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4767 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/cmoncrawl/middleware/synchronized.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 20:28:44.241689 CmonCrawl-1.0.2/cmoncrawl/processor/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/cmoncrawl/processor/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 20:28:44.241689 CmonCrawl-1.0.2/cmoncrawl/processor/extraction/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/cmoncrawl/processor/extraction/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1123 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/cmoncrawl/processor/extraction/filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8378 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/cmoncrawl/processor/extraction/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 20:28:44.245689 CmonCrawl-1.0.2/cmoncrawl/processor/pipeline/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/cmoncrawl/processor/pipeline/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8196 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/cmoncrawl/processor/pipeline/downloader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6512 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/cmoncrawl/processor/pipeline/extractor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1835 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/cmoncrawl/processor/pipeline/pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5698 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/cmoncrawl/processor/pipeline/router.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6929 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/cmoncrawl/processor/pipeline/streamer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 20:28:44.245689 CmonCrawl-1.0.2/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/.nojekyll
+-rw-r--r--   0 runner    (1001) docker     (123)      638 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 20:28:44.205687 CmonCrawl-1.0.2/docs/build/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 20:28:44.245689 CmonCrawl-1.0.2/docs/build/doctrees/
+-rw-r--r--   0 runner    (1001) docker     (123)     4150 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/doctrees/api.doctree
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 20:28:44.245689 CmonCrawl-1.0.2/docs/build/doctrees/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)     7226 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/doctrees/cli/cli.doctree
+-rw-r--r--   0 runner    (1001) docker     (123)    16083 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/doctrees/cli/download.doctree
+-rw-r--r--   0 runner    (1001) docker     (123)    17674 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/doctrees/cli/extract.doctree
+-rw-r--r--   0 runner    (1001) docker     (123)     2845 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/doctrees/cli/index.doctree
+-rw-r--r--   0 runner    (1001) docker     (123)   447558 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/doctrees/environment.pickle
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 20:28:44.249689 CmonCrawl-1.0.2/docs/build/doctrees/extraction/
+-rw-r--r--   0 runner    (1001) docker     (123)    18267 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/doctrees/extraction/config_file.doctree
+-rw-r--r--   0 runner    (1001) docker     (123)    15604 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/doctrees/extraction/creating_extractor.doctree
+-rw-r--r--   0 runner    (1001) docker     (123)     2848 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/doctrees/extraction/index.doctree
+-rw-r--r--   0 runner    (1001) docker     (123)     8169 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/doctrees/extraction/utils.doctree
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 20:28:44.297691 CmonCrawl-1.0.2/docs/build/doctrees/generated/
+-rw-r--r--   0 runner    (1001) docker     (123)     5976 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/doctrees/generated/cmoncrawl.aggregator.doctree
+-rw-r--r--   0 runner    (1001) docker     (123)    16051 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/doctrees/generated/cmoncrawl.aggregator.index_query.IndexAggregator.__init__.doctree
+-rw-r--r--   0 runner    (1001) docker     (123)     9377 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/doctrees/generated/cmoncrawl.aggregator.index_query.IndexAggregator.aclose.doctree
+-rw-r--r--   0 runner    (1001) docker     (123)     4857 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/doctrees/generated/cmoncrawl.aggregator.index_query.IndexAggregator.aopen.doctree
+-rw-r--r--   0 runner    (1001) docker     (123)    37518 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/doctrees/generated/cmoncrawl.aggregator.index_query.IndexAggregator.doctree
+-rw-r--r--   0 runner    (1001) docker     (123)     6990 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/doctrees/generated/cmoncrawl.aggregator.index_query.IndexAggregator.get_all_CC_indexes.doctree
+-rw-r--r--   0 runner    (1001) docker     (123)    11632 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/doctrees/generated/cmoncrawl.aggregator.index_query.IndexAggregator.get_captured_responses.doctree
+-rw-r--r--   0 runner    (1001) docker     (123)     9861 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/doctrees/generated/cmoncrawl.aggregator.index_query.IndexAggregator.get_number_of_pages.doctree
+-rw-r--r--   0 runner    (1001) docker     (123)     8979 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/doctrees/generated/cmoncrawl.aggregator.index_query.doctree
+-rw-r--r--   0 runner    (1001) docker     (123)     6196 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/doctrees/generated/cmoncrawl.aggregator.utils.doctree
+-rw-r--r--   0 runner    (1001) docker     (123)     4914 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/doctrees/generated/cmoncrawl.aggregator.utils.helpers.doctree
+-rw-r--r--   0 runner    (1001) docker     (123)    13989 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/doctrees/generated/cmoncrawl.aggregator.utils.ndjson_decoder.Decoder.__init__.doctree
+-rw-r--r--   0 runner    (1001) docker     (123)     6254 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/doctrees/generated/cmoncrawl.aggregator.utils.ndjson_decoder.Decoder.decode.doctree
+-rw-r--r--   0 runner    (1001) docker     (123)    25998 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/doctrees/generated/cmoncrawl.aggregator.utils.ndjson_decoder.Decoder.doctree
+-rw-r--r--   0 runner    (1001) docker     (123)     6093 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/doctrees/generated/cmoncrawl.aggregator.utils.ndjson_decoder.Decoder.raw_decode.doctree
+-rw-r--r--   0 runner    (1001) docker     (123)     5490 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/doctrees/generated/cmoncrawl.aggregator.utils.ndjson_decoder.doctree
+-rw-r--r--   0 runner    (1001) docker     (123)     5824 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/doctrees/generated/cmoncrawl.common.doctree
+-rw-r--r--   0 runner    (1001) docker     (123)     2859 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/doctrees/generated/cmoncrawl.common.loggers.doctree
+-rw-r--r--   0 runner    (1001) docker     (123)     7639 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/doctrees/generated/cmoncrawl.common.types.DomainCrawl.__init__.doctree
+-rw-r--r--   0 runner    (1001) docker     (123)    17989 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/doctrees/generated/cmoncrawl.common.types.DomainCrawl.doctree
+-rw-r--r--   0 runner    (1001) docker     (123)    12190 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/doctrees/generated/cmoncrawl.common.types.DomainRecord.__init__.doctree
+-rw-r--r--   0 runner    (1001) docker     (123)    36970 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/doctrees/generated/cmoncrawl.common.types.DomainRecord.doctree
+-rw-r--r--   0 runner    (1001) docker     (123)     8890 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/doctrees/generated/cmoncrawl.common.types.DomainRecord.from_dict.doctree
+-rw-r--r--   0 runner    (1001) docker     (123)     8994 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/doctrees/generated/cmoncrawl.common.types.DomainRecord.from_json.doctree
+-rw-r--r--   0 runner    (1001) docker     (123)    11251 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/doctrees/generated/cmoncrawl.common.types.DomainRecord.schema.doctree
+-rw-r--r--   0 runner    (1001) docker     (123)     8412 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/doctrees/generated/cmoncrawl.common.types.DomainRecord.to_dict.doctree
+-rw-r--r--   0 runner    (1001) docker     (123)    16752 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/doctrees/generated/cmoncrawl.common.types.DomainRecord.to_json.doctree
+-rw-r--r--   0 runner    (1001) docker     (123)     6301 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/doctrees/generated/cmoncrawl.common.types.ExtractConfig.__init__.doctree
+-rw-r--r--   0 runner    (1001) docker     (123)    20553 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/doctrees/generated/cmoncrawl.common.types.ExtractConfig.doctree
+-rw-r--r--   0 runner    (1001) docker     (123)     8905 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/doctrees/generated/cmoncrawl.common.types.ExtractConfig.from_dict.doctree
+-rw-r--r--   0 runner    (1001) docker     (123)     9009 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/doctrees/generated/cmoncrawl.common.types.ExtractConfig.from_json.doctree
+-rw-r--r--   0 runner    (1001) docker     (123)    11265 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/doctrees/generated/cmoncrawl.common.types.ExtractConfig.schema.doctree
+-rw-r--r--   0 runner    (1001) docker     (123)     8427 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/doctrees/generated/cmoncrawl.common.types.ExtractConfig.to_dict.doctree
+-rw-r--r--   0 runner    (1001) docker     (123)    16767 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/doctrees/generated/cmoncrawl.common.types.ExtractConfig.to_json.doctree
+-rw-r--r--   0 runner    (1001) docker     (123)     8264 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/doctrees/generated/cmoncrawl.common.types.ExtractorConfig.__init__.doctree
+-rw-r--r--   0 runner    (1001) docker     (123)    25358 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/doctrees/generated/cmoncrawl.common.types.ExtractorConfig.doctree
+-rw-r--r--   0 runner    (1001) docker     (123)     8935 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/doctrees/generated/cmoncrawl.common.types.ExtractorConfig.from_dict.doctree
+-rw-r--r--   0 runner    (1001) docker     (123)     9039 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/doctrees/generated/cmoncrawl.common.types.ExtractorConfig.from_json.doctree
+-rw-r--r--   0 runner    (1001) docker     (123)    11293 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/doctrees/generated/cmoncrawl.common.types.ExtractorConfig.schema.doctree
+-rw-r--r--   0 runner    (1001) docker     (123)     8457 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/doctrees/generated/cmoncrawl.common.types.ExtractorConfig.to_dict.doctree
+-rw-r--r--   0 runner    (1001) docker     (123)    16797 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/doctrees/generated/cmoncrawl.common.types.ExtractorConfig.to_json.doctree
+-rw-r--r--   0 runner    (1001) docker     (123)     7157 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/doctrees/generated/cmoncrawl.common.types.PipeMetadata.__init__.doctree
+-rw-r--r--   0 runner    (1001) docker     (123)    20439 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/doctrees/generated/cmoncrawl.common.types.PipeMetadata.doctree
+-rw-r--r--   0 runner    (1001) docker     (123)     6895 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/doctrees/generated/cmoncrawl.common.types.RetrieveResponse.__init__.doctree
+-rw-r--r--   0 runner    (1001) docker     (123)    16512 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/doctrees/generated/cmoncrawl.common.types.RetrieveResponse.doctree
+-rw-r--r--   0 runner    (1001) docker     (123)     5149 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/doctrees/generated/cmoncrawl.common.types.RoutesConfig.__init__.doctree
+-rw-r--r--   0 runner    (1001) docker     (123)    18100 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/doctrees/generated/cmoncrawl.common.types.RoutesConfig.doctree
+-rw-r--r--   0 runner    (1001) docker     (123)     8890 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/doctrees/generated/cmoncrawl.common.types.RoutesConfig.from_dict.doctree
+-rw-r--r--   0 runner    (1001) docker     (123)     8994 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/doctrees/generated/cmoncrawl.common.types.RoutesConfig.from_json.doctree
+-rw-r--r--   0 runner    (1001) docker     (123)    11251 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/doctrees/generated/cmoncrawl.common.types.RoutesConfig.schema.doctree
+-rw-r--r--   0 runner    (1001) docker     (123)     8412 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/doctrees/generated/cmoncrawl.common.types.RoutesConfig.to_dict.doctree
+-rw-r--r--   0 runner    (1001) docker     (123)    16752 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/doctrees/generated/cmoncrawl.common.types.RoutesConfig.to_json.doctree
+-rw-r--r--   0 runner    (1001) docker     (123)    12267 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/doctrees/generated/cmoncrawl.common.types.doctree
+-rw-r--r--   0 runner    (1001) docker     (123)     6530 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/doctrees/generated/cmoncrawl.doctree
+-rw-r--r--   0 runner    (1001) docker     (123)     5962 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/doctrees/generated/cmoncrawl.processor.doctree
+-rw-r--r--   0 runner    (1001) docker     (123)     6244 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/doctrees/generated/cmoncrawl.processor.extraction.doctree
+-rw-r--r--   0 runner    (1001) docker     (123)     6802 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/doctrees/generated/cmoncrawl.processor.extraction.filters.doctree
+-rw-r--r--   0 runner    (1001) docker     (123)    15336 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/doctrees/generated/cmoncrawl.processor.extraction.utils.doctree
+-rw-r--r--   0 runner    (1001) docker     (123)     9365 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/doctrees/generated/cmoncrawl.processor.pipeline.doctree
+-rw-r--r--   0 runner    (1001) docker     (123)    10078 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/doctrees/generated/cmoncrawl.processor.pipeline.downloader.AsyncDownloader.__init__.doctree
+-rw-r--r--   0 runner    (1001) docker     (123)     9400 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/doctrees/generated/cmoncrawl.processor.pipeline.downloader.AsyncDownloader.aclose.doctree
+-rw-r--r--   0 runner    (1001) docker     (123)     4897 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/doctrees/generated/cmoncrawl.processor.pipeline.downloader.AsyncDownloader.aopen.doctree
+-rw-r--r--   0 runner    (1001) docker     (123)    24370 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/doctrees/generated/cmoncrawl.processor.pipeline.downloader.AsyncDownloader.doctree
+-rw-r--r--   0 runner    (1001) docker     (123)     5359 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/doctrees/generated/cmoncrawl.processor.pipeline.downloader.AsyncDownloader.download.doctree
+-rw-r--r--   0 runner    (1001) docker     (123)     7304 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/doctrees/generated/cmoncrawl.processor.pipeline.downloader.AsyncDownloader.unwrap.doctree
+-rw-r--r--   0 runner    (1001) docker     (123)     8595 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/doctrees/generated/cmoncrawl.processor.pipeline.downloader.DownloaderDummy.__init__.doctree
+-rw-r--r--   0 runner    (1001) docker     (123)    21942 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/doctrees/generated/cmoncrawl.processor.pipeline.downloader.DownloaderDummy.doctree
+-rw-r--r--   0 runner    (1001) docker     (123)     5359 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/doctrees/generated/cmoncrawl.processor.pipeline.downloader.DownloaderDummy.download.doctree
+-rw-r--r--   0 runner    (1001) docker     (123)     5116 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/doctrees/generated/cmoncrawl.processor.pipeline.downloader.DownloaderDummy.extract_url.doctree
+-rw-r--r--   0 runner    (1001) docker     (123)     5099 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/doctrees/generated/cmoncrawl.processor.pipeline.downloader.DownloaderDummy.extract_year.doctree
+-rw-r--r--   0 runner    (1001) docker     (123)     5744 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/doctrees/generated/cmoncrawl.processor.pipeline.downloader.DownloaderDummy.mine_metadata.doctree
+-rw-r--r--   0 runner    (1001) docker     (123)     4155 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/doctrees/generated/cmoncrawl.processor.pipeline.downloader.IDownloader.__init__.doctree
+-rw-r--r--   0 runner    (1001) docker     (123)     8781 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/doctrees/generated/cmoncrawl.processor.pipeline.downloader.IDownloader.doctree
+-rw-r--r--   0 runner    (1001) docker     (123)     6867 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/doctrees/generated/cmoncrawl.processor.pipeline.downloader.IDownloader.download.doctree
+-rw-r--r--   0 runner    (1001) docker     (123)     8113 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/doctrees/generated/cmoncrawl.processor.pipeline.downloader.doctree
+-rw-r--r--   0 runner    (1001) docker     (123)     5883 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/doctrees/generated/cmoncrawl.processor.pipeline.extractor.BaseExtractor.__init__.doctree
+-rw-r--r--   0 runner    (1001) docker     (123)    17113 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/doctrees/generated/cmoncrawl.processor.pipeline.extractor.BaseExtractor.doctree
+-rw-r--r--   0 runner    (1001) docker     (123)     7171 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/doctrees/generated/cmoncrawl.processor.pipeline.extractor.BaseExtractor.extract.doctree
+-rw-r--r--   0 runner    (1001) docker     (123)     7645 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/doctrees/generated/cmoncrawl.processor.pipeline.extractor.BaseExtractor.extract_soup.doctree
+-rw-r--r--   0 runner    (1001) docker     (123)     6031 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/doctrees/generated/cmoncrawl.processor.pipeline.extractor.BaseExtractor.filter_raw.doctree
+-rw-r--r--   0 runner    (1001) docker     (123)     6100 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/doctrees/generated/cmoncrawl.processor.pipeline.extractor.BaseExtractor.filter_soup.doctree
+-rw-r--r--   0 runner    (1001) docker     (123)     5960 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/doctrees/generated/cmoncrawl.processor.pipeline.extractor.BaseExtractor.preprocess.doctree
+-rw-r--r--   0 runner    (1001) docker     (123)     5597 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/doctrees/generated/cmoncrawl.processor.pipeline.extractor.DomainRecordExtractor.__init__.doctree
+-rw-r--r--   0 runner    (1001) docker     (123)    17063 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/doctrees/generated/cmoncrawl.processor.pipeline.extractor.DomainRecordExtractor.doctree
+-rw-r--r--   0 runner    (1001) docker     (123)     7283 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/doctrees/generated/cmoncrawl.processor.pipeline.extractor.DomainRecordExtractor.extract.doctree
+-rw-r--r--   0 runner    (1001) docker     (123)     5960 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/doctrees/generated/cmoncrawl.processor.pipeline.extractor.DomainRecordExtractor.extract_soup.doctree
+-rw-r--r--   0 runner    (1001) docker     (123)     5876 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/doctrees/generated/cmoncrawl.processor.pipeline.extractor.DomainRecordExtractor.filter_raw.doctree
+-rw-r--r--   0 runner    (1001) docker     (123)     6220 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/doctrees/generated/cmoncrawl.processor.pipeline.extractor.DomainRecordExtractor.filter_soup.doctree
+-rw-r--r--   0 runner    (1001) docker     (123)     6072 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/doctrees/generated/cmoncrawl.processor.pipeline.extractor.DomainRecordExtractor.preprocess.doctree
+-rw-r--r--   0 runner    (1001) docker     (123)     5469 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/doctrees/generated/cmoncrawl.processor.pipeline.extractor.HTMLExtractor.__init__.doctree
+-rw-r--r--   0 runner    (1001) docker     (123)    16655 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/doctrees/generated/cmoncrawl.processor.pipeline.extractor.HTMLExtractor.doctree
+-rw-r--r--   0 runner    (1001) docker     (123)     7171 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/doctrees/generated/cmoncrawl.processor.pipeline.extractor.HTMLExtractor.extract.doctree
+-rw-r--r--   0 runner    (1001) docker     (123)     5832 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/doctrees/generated/cmoncrawl.processor.pipeline.extractor.HTMLExtractor.extract_soup.doctree
+-rw-r--r--   0 runner    (1001) docker     (123)     5748 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/doctrees/generated/cmoncrawl.processor.pipeline.extractor.HTMLExtractor.filter_raw.doctree
+-rw-r--r--   0 runner    (1001) docker     (123)     6100 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/doctrees/generated/cmoncrawl.processor.pipeline.extractor.HTMLExtractor.filter_soup.doctree
+-rw-r--r--   0 runner    (1001) docker     (123)     5960 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/doctrees/generated/cmoncrawl.processor.pipeline.extractor.HTMLExtractor.preprocess.doctree
+-rw-r--r--   0 runner    (1001) docker     (123)     4128 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/doctrees/generated/cmoncrawl.processor.pipeline.extractor.IExtractor.__init__.doctree
+-rw-r--r--   0 runner    (1001) docker     (123)     8734 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/doctrees/generated/cmoncrawl.processor.pipeline.extractor.IExtractor.doctree
+-rw-r--r--   0 runner    (1001) docker     (123)     7407 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/doctrees/generated/cmoncrawl.processor.pipeline.extractor.IExtractor.extract.doctree
+-rw-r--r--   0 runner    (1001) docker     (123)     9217 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/doctrees/generated/cmoncrawl.processor.pipeline.extractor.doctree
+-rw-r--r--   0 runner    (1001) docker     (123)     6770 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/doctrees/generated/cmoncrawl.processor.pipeline.pipeline.ProcessorPipeline.__init__.doctree
+-rw-r--r--   0 runner    (1001) docker     (123)    14259 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/doctrees/generated/cmoncrawl.processor.pipeline.pipeline.ProcessorPipeline.doctree
+-rw-r--r--   0 runner    (1001) docker     (123)     7149 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/doctrees/generated/cmoncrawl.processor.pipeline.pipeline.ProcessorPipeline.process_domain_record.doctree
+-rw-r--r--   0 runner    (1001) docker     (123)     5401 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/doctrees/generated/cmoncrawl.processor.pipeline.pipeline.doctree
+-rw-r--r--   0 runner    (1001) docker     (123)     4047 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/doctrees/generated/cmoncrawl.processor.pipeline.router.IRouter.__init__.doctree
+-rw-r--r--   0 runner    (1001) docker     (123)     8547 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/doctrees/generated/cmoncrawl.processor.pipeline.router.IRouter.doctree
+-rw-r--r--   0 runner    (1001) docker     (123)     7889 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/doctrees/generated/cmoncrawl.processor.pipeline.router.IRouter.route.doctree
+-rw-r--r--   0 runner    (1001) docker     (123)     7921 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/doctrees/generated/cmoncrawl.processor.pipeline.router.Route.__init__.doctree
+-rw-r--r--   0 runner    (1001) docker     (123)    19674 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/doctrees/generated/cmoncrawl.processor.pipeline.router.Route.doctree
+-rw-r--r--   0 runner    (1001) docker     (123)     4031 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/doctrees/generated/cmoncrawl.processor.pipeline.router.Router.__init__.doctree
+-rw-r--r--   0 runner    (1001) docker     (123)    15623 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/doctrees/generated/cmoncrawl.processor.pipeline.router.Router.doctree
+-rw-r--r--   0 runner    (1001) docker     (123)     5681 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/doctrees/generated/cmoncrawl.processor.pipeline.router.Router.load_extractor.doctree
+-rw-r--r--   0 runner    (1001) docker     (123)     4902 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/doctrees/generated/cmoncrawl.processor.pipeline.router.Router.load_module.doctree
+-rw-r--r--   0 runner    (1001) docker     (123)     5103 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/doctrees/generated/cmoncrawl.processor.pipeline.router.Router.load_module_as_extractor.doctree
+-rw-r--r--   0 runner    (1001) docker     (123)     4892 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/doctrees/generated/cmoncrawl.processor.pipeline.router.Router.load_modules.doctree
+-rw-r--r--   0 runner    (1001) docker     (123)     9971 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/doctrees/generated/cmoncrawl.processor.pipeline.router.Router.register_route.doctree
+-rw-r--r--   0 runner    (1001) docker     (123)     5445 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/doctrees/generated/cmoncrawl.processor.pipeline.router.Router.register_routes.doctree
+-rw-r--r--   0 runner    (1001) docker     (123)     7593 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/doctrees/generated/cmoncrawl.processor.pipeline.router.Router.route.doctree
+-rw-r--r--   0 runner    (1001) docker     (123)     7194 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/doctrees/generated/cmoncrawl.processor.pipeline.router.doctree
+-rw-r--r--   0 runner    (1001) docker     (123)     9351 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/doctrees/generated/cmoncrawl.processor.pipeline.streamer.BaseStreamerFile.__init__.doctree
+-rw-r--r--   0 runner    (1001) docker     (123)     4837 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/doctrees/generated/cmoncrawl.processor.pipeline.streamer.BaseStreamerFile.clean_up.doctree
+-rw-r--r--   0 runner    (1001) docker     (123)    23368 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/doctrees/generated/cmoncrawl.processor.pipeline.streamer.BaseStreamerFile.doctree
+-rw-r--r--   0 runner    (1001) docker     (123)     5197 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/doctrees/generated/cmoncrawl.processor.pipeline.streamer.BaseStreamerFile.get_file_name.doctree
+-rw-r--r--   0 runner    (1001) docker     (123)     6582 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/doctrees/generated/cmoncrawl.processor.pipeline.streamer.BaseStreamerFile.metadata_to_string.doctree
+-rw-r--r--   0 runner    (1001) docker     (123)     7136 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/doctrees/generated/cmoncrawl.processor.pipeline.streamer.BaseStreamerFile.stream.doctree
+-rw-r--r--   0 runner    (1001) docker     (123)     4101 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/doctrees/generated/cmoncrawl.processor.pipeline.streamer.IStreamer.__init__.doctree
+-rw-r--r--   0 runner    (1001) docker     (123)     4921 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/doctrees/generated/cmoncrawl.processor.pipeline.streamer.IStreamer.clean_up.doctree
+-rw-r--r--   0 runner    (1001) docker     (123)    10102 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/doctrees/generated/cmoncrawl.processor.pipeline.streamer.IStreamer.doctree
+-rw-r--r--   0 runner    (1001) docker     (123)     7218 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/doctrees/generated/cmoncrawl.processor.pipeline.streamer.IStreamer.stream.doctree
+-rw-r--r--   0 runner    (1001) docker     (123)     4165 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/doctrees/generated/cmoncrawl.processor.pipeline.streamer.StreamerDummy.__init__.doctree
+-rw-r--r--   0 runner    (1001) docker     (123)     4450 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/doctrees/generated/cmoncrawl.processor.pipeline.streamer.StreamerDummy.clean_up.doctree
+-rw-r--r--   0 runner    (1001) docker     (123)    10278 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/doctrees/generated/cmoncrawl.processor.pipeline.streamer.StreamerDummy.doctree
+-rw-r--r--   0 runner    (1001) docker     (123)     6779 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/doctrees/generated/cmoncrawl.processor.pipeline.streamer.StreamerDummy.stream.doctree
+-rw-r--r--   0 runner    (1001) docker     (123)     5696 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/doctrees/generated/cmoncrawl.processor.pipeline.streamer.StreamerFileHTML.__init__.doctree
+-rw-r--r--   0 runner    (1001) docker     (123)     4837 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/doctrees/generated/cmoncrawl.processor.pipeline.streamer.StreamerFileHTML.clean_up.doctree
+-rw-r--r--   0 runner    (1001) docker     (123)    15596 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/doctrees/generated/cmoncrawl.processor.pipeline.streamer.StreamerFileHTML.doctree
+-rw-r--r--   0 runner    (1001) docker     (123)     5197 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/doctrees/generated/cmoncrawl.processor.pipeline.streamer.StreamerFileHTML.get_file_name.doctree
+-rw-r--r--   0 runner    (1001) docker     (123)     6301 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/doctrees/generated/cmoncrawl.processor.pipeline.streamer.StreamerFileHTML.metadata_to_string.doctree
+-rw-r--r--   0 runner    (1001) docker     (123)     7136 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/doctrees/generated/cmoncrawl.processor.pipeline.streamer.StreamerFileHTML.stream.doctree
+-rw-r--r--   0 runner    (1001) docker     (123)     7513 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/doctrees/generated/cmoncrawl.processor.pipeline.streamer.StreamerFileJSON.__init__.doctree
+-rw-r--r--   0 runner    (1001) docker     (123)     4837 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/doctrees/generated/cmoncrawl.processor.pipeline.streamer.StreamerFileJSON.clean_up.doctree
+-rw-r--r--   0 runner    (1001) docker     (123)    19273 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/doctrees/generated/cmoncrawl.processor.pipeline.streamer.StreamerFileJSON.doctree
+-rw-r--r--   0 runner    (1001) docker     (123)     5197 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/doctrees/generated/cmoncrawl.processor.pipeline.streamer.StreamerFileJSON.get_file_name.doctree
+-rw-r--r--   0 runner    (1001) docker     (123)     6301 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/doctrees/generated/cmoncrawl.processor.pipeline.streamer.StreamerFileJSON.metadata_to_string.doctree
+-rw-r--r--   0 runner    (1001) docker     (123)     7136 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/doctrees/generated/cmoncrawl.processor.pipeline.streamer.StreamerFileJSON.stream.doctree
+-rw-r--r--   0 runner    (1001) docker     (123)    10726 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/doctrees/generated/cmoncrawl.processor.pipeline.streamer.doctree
+-rw-r--r--   0 runner    (1001) docker     (123)     5198 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/doctrees/index.doctree
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 20:28:44.297691 CmonCrawl-1.0.2/docs/build/doctrees/misc/
+-rw-r--r--   0 runner    (1001) docker     (123)    10600 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/doctrees/misc/domain_record.doctree
+-rw-r--r--   0 runner    (1001) docker     (123)     2781 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/doctrees/misc/index.doctree
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 20:28:44.297691 CmonCrawl-1.0.2/docs/build/doctrees/prog_guide/
+-rw-r--r--   0 runner    (1001) docker     (123)     2834 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/doctrees/prog_guide/index.doctree
+-rw-r--r--   0 runner    (1001) docker     (123)    24337 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/doctrees/prog_guide/overview.doctree
+-rw-r--r--   0 runner    (1001) docker     (123)     8880 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/doctrees/prog_guide/pip.doctree
+-rw-r--r--   0 runner    (1001) docker     (123)     9009 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/doctrees/usage.doctree
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 20:28:44.301692 CmonCrawl-1.0.2/docs/build/html/
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/html/.buildinfo
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 20:28:44.301692 CmonCrawl-1.0.2/docs/build/html/_sources/
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/html/_sources/api.rst.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 20:28:44.301692 CmonCrawl-1.0.2/docs/build/html/_sources/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)     1175 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/html/_sources/cli/cli.rst.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1987 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/html/_sources/cli/download.rst.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2753 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/html/_sources/cli/extract.rst.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/html/_sources/cli/index.rst.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 20:28:44.301692 CmonCrawl-1.0.2/docs/build/html/_sources/extraction/
+-rw-r--r--   0 runner    (1001) docker     (123)     3910 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/html/_sources/extraction/config_file.rst.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2392 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/html/_sources/extraction/creating_extractor.rst.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/html/_sources/extraction/index.rst.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      861 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/html/_sources/extraction/utils.rst.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 20:28:44.349694 CmonCrawl-1.0.2/docs/build/html/_sources/generated/
+-rw-r--r--   0 runner    (1001) docker     (123)      220 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/html/_sources/generated/cmoncrawl.aggregator.index_query.IndexAggregator.__init__.rst.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      206 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/html/_sources/generated/cmoncrawl.aggregator.index_query.IndexAggregator.aclose.rst.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      203 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/html/_sources/generated/cmoncrawl.aggregator.index_query.IndexAggregator.aopen.rst.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/html/_sources/generated/cmoncrawl.aggregator.index_query.IndexAggregator.get_all_CC_indexes.rst.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      258 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/html/_sources/generated/cmoncrawl.aggregator.index_query.IndexAggregator.get_captured_responses.rst.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      251 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/html/_sources/generated/cmoncrawl.aggregator.index_query.IndexAggregator.get_number_of_pages.rst.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      530 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/html/_sources/generated/cmoncrawl.aggregator.index_query.IndexAggregator.rst.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      391 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/html/_sources/generated/cmoncrawl.aggregator.index_query.rst.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      269 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/html/_sources/generated/cmoncrawl.aggregator.rst.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      250 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/html/_sources/generated/cmoncrawl.aggregator.utils.helpers.rst.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      223 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/html/_sources/generated/cmoncrawl.aggregator.utils.ndjson_decoder.Decoder.__init__.rst.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/html/_sources/generated/cmoncrawl.aggregator.utils.ndjson_decoder.Decoder.decode.rst.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      223 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/html/_sources/generated/cmoncrawl.aggregator.utils.ndjson_decoder.Decoder.raw_decode.rst.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      383 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/html/_sources/generated/cmoncrawl.aggregator.utils.ndjson_decoder.Decoder.rst.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      282 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/html/_sources/generated/cmoncrawl.aggregator.utils.ndjson_decoder.rst.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      304 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/html/_sources/generated/cmoncrawl.aggregator.utils.rst.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/html/_sources/generated/cmoncrawl.common.loggers.rst.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      245 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/html/_sources/generated/cmoncrawl.common.rst.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      176 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/html/_sources/generated/cmoncrawl.common.types.DomainCrawl.__init__.rst.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      427 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/html/_sources/generated/cmoncrawl.common.types.DomainCrawl.rst.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      179 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/html/_sources/generated/cmoncrawl.common.types.DomainRecord.__init__.rst.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      176 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/html/_sources/generated/cmoncrawl.common.types.DomainRecord.from_dict.rst.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      176 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/html/_sources/generated/cmoncrawl.common.types.DomainRecord.from_json.rst.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      687 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/html/_sources/generated/cmoncrawl.common.types.DomainRecord.rst.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/html/_sources/generated/cmoncrawl.common.types.DomainRecord.schema.rst.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      170 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/html/_sources/generated/cmoncrawl.common.types.DomainRecord.to_dict.rst.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      170 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/html/_sources/generated/cmoncrawl.common.types.DomainRecord.to_json.rst.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      182 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/html/_sources/generated/cmoncrawl.common.types.ExtractConfig.__init__.rst.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      179 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/html/_sources/generated/cmoncrawl.common.types.ExtractConfig.from_dict.rst.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      179 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/html/_sources/generated/cmoncrawl.common.types.ExtractConfig.from_json.rst.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      568 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/html/_sources/generated/cmoncrawl.common.types.ExtractConfig.rst.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/html/_sources/generated/cmoncrawl.common.types.ExtractConfig.schema.rst.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/html/_sources/generated/cmoncrawl.common.types.ExtractConfig.to_dict.rst.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/html/_sources/generated/cmoncrawl.common.types.ExtractConfig.to_json.rst.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/html/_sources/generated/cmoncrawl.common.types.ExtractorConfig.__init__.rst.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      185 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/html/_sources/generated/cmoncrawl.common.types.ExtractorConfig.from_dict.rst.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      185 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/html/_sources/generated/cmoncrawl.common.types.ExtractorConfig.from_json.rst.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      604 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/html/_sources/generated/cmoncrawl.common.types.ExtractorConfig.rst.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      174 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/html/_sources/generated/cmoncrawl.common.types.ExtractorConfig.schema.rst.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      179 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/html/_sources/generated/cmoncrawl.common.types.ExtractorConfig.to_dict.rst.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      179 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/html/_sources/generated/cmoncrawl.common.types.ExtractorConfig.to_json.rst.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      179 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/html/_sources/generated/cmoncrawl.common.types.PipeMetadata.__init__.rst.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      536 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/html/_sources/generated/cmoncrawl.common.types.PipeMetadata.rst.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      191 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/html/_sources/generated/cmoncrawl.common.types.RetrieveResponse.__init__.rst.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      461 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/html/_sources/generated/cmoncrawl.common.types.RetrieveResponse.rst.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      179 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/html/_sources/generated/cmoncrawl.common.types.RoutesConfig.__init__.rst.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      176 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/html/_sources/generated/cmoncrawl.common.types.RoutesConfig.from_dict.rst.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      176 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/html/_sources/generated/cmoncrawl.common.types.RoutesConfig.from_json.rst.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      553 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/html/_sources/generated/cmoncrawl.common.types.RoutesConfig.rst.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/html/_sources/generated/cmoncrawl.common.types.RoutesConfig.schema.rst.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      170 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/html/_sources/generated/cmoncrawl.common.types.RoutesConfig.to_dict.rst.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      170 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/html/_sources/generated/cmoncrawl.common.types.RoutesConfig.to_json.rst.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      349 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/html/_sources/generated/cmoncrawl.common.types.rst.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      295 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/html/_sources/generated/cmoncrawl.processor.extraction.filters.rst.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      315 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/html/_sources/generated/cmoncrawl.processor.extraction.rst.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      500 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/html/_sources/generated/cmoncrawl.processor.extraction.utils.rst.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      239 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/html/_sources/generated/cmoncrawl.processor.pipeline.downloader.AsyncDownloader.__init__.rst.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      225 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/html/_sources/generated/cmoncrawl.processor.pipeline.downloader.AsyncDownloader.aclose.rst.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      222 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/html/_sources/generated/cmoncrawl.processor.pipeline.downloader.AsyncDownloader.aopen.rst.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      231 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/html/_sources/generated/cmoncrawl.processor.pipeline.downloader.AsyncDownloader.download.rst.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      480 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/html/_sources/generated/cmoncrawl.processor.pipeline.downloader.AsyncDownloader.rst.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      225 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/html/_sources/generated/cmoncrawl.processor.pipeline.downloader.AsyncDownloader.unwrap.rst.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      239 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/html/_sources/generated/cmoncrawl.processor.pipeline.downloader.DownloaderDummy.__init__.rst.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      231 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/html/_sources/generated/cmoncrawl.processor.pipeline.downloader.DownloaderDummy.download.rst.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      242 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/html/_sources/generated/cmoncrawl.processor.pipeline.downloader.DownloaderDummy.extract_url.rst.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      245 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/html/_sources/generated/cmoncrawl.processor.pipeline.downloader.DownloaderDummy.extract_year.rst.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/html/_sources/generated/cmoncrawl.processor.pipeline.downloader.DownloaderDummy.mine_metadata.rst.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      499 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/html/_sources/generated/cmoncrawl.processor.pipeline.downloader.DownloaderDummy.rst.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      227 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/html/_sources/generated/cmoncrawl.processor.pipeline.downloader.IDownloader.__init__.rst.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      219 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/html/_sources/generated/cmoncrawl.processor.pipeline.downloader.IDownloader.download.rst.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      371 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/html/_sources/generated/cmoncrawl.processor.pipeline.downloader.IDownloader.rst.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      322 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/html/_sources/generated/cmoncrawl.processor.pipeline.downloader.rst.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/html/_sources/generated/cmoncrawl.processor.pipeline.extractor.BaseExtractor.__init__.rst.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      219 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/html/_sources/generated/cmoncrawl.processor.pipeline.extractor.BaseExtractor.extract.rst.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      236 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/html/_sources/generated/cmoncrawl.processor.pipeline.extractor.BaseExtractor.extract_soup.rst.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/html/_sources/generated/cmoncrawl.processor.pipeline.extractor.BaseExtractor.filter_raw.rst.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      233 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/html/_sources/generated/cmoncrawl.processor.pipeline.extractor.BaseExtractor.filter_soup.rst.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/html/_sources/generated/cmoncrawl.processor.pipeline.extractor.BaseExtractor.preprocess.rst.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      508 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/html/_sources/generated/cmoncrawl.processor.pipeline.extractor.BaseExtractor.rst.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      254 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/html/_sources/generated/cmoncrawl.processor.pipeline.extractor.DomainRecordExtractor.__init__.rst.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      243 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/html/_sources/generated/cmoncrawl.processor.pipeline.extractor.DomainRecordExtractor.extract.rst.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      260 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/html/_sources/generated/cmoncrawl.processor.pipeline.extractor.DomainRecordExtractor.extract_soup.rst.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      254 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/html/_sources/generated/cmoncrawl.processor.pipeline.extractor.DomainRecordExtractor.filter_raw.rst.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      257 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/html/_sources/generated/cmoncrawl.processor.pipeline.extractor.DomainRecordExtractor.filter_soup.rst.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      252 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/html/_sources/generated/cmoncrawl.processor.pipeline.extractor.DomainRecordExtractor.preprocess.rst.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      580 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/html/_sources/generated/cmoncrawl.processor.pipeline.extractor.DomainRecordExtractor.rst.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/html/_sources/generated/cmoncrawl.processor.pipeline.extractor.HTMLExtractor.__init__.rst.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      219 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/html/_sources/generated/cmoncrawl.processor.pipeline.extractor.HTMLExtractor.extract.rst.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      236 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/html/_sources/generated/cmoncrawl.processor.pipeline.extractor.HTMLExtractor.extract_soup.rst.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/html/_sources/generated/cmoncrawl.processor.pipeline.extractor.HTMLExtractor.filter_raw.rst.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      233 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/html/_sources/generated/cmoncrawl.processor.pipeline.extractor.HTMLExtractor.filter_soup.rst.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/html/_sources/generated/cmoncrawl.processor.pipeline.extractor.HTMLExtractor.preprocess.rst.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      508 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/html/_sources/generated/cmoncrawl.processor.pipeline.extractor.HTMLExtractor.rst.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      221 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/html/_sources/generated/cmoncrawl.processor.pipeline.extractor.IExtractor.__init__.rst.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/html/_sources/generated/cmoncrawl.processor.pipeline.extractor.IExtractor.extract.rst.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/html/_sources/generated/cmoncrawl.processor.pipeline.extractor.IExtractor.rst.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      342 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/html/_sources/generated/cmoncrawl.processor.pipeline.extractor.rst.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      239 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/html/_sources/generated/cmoncrawl.processor.pipeline.pipeline.ProcessorPipeline.__init__.rst.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      274 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/html/_sources/generated/cmoncrawl.processor.pipeline.pipeline.ProcessorPipeline.process_domain_record.rst.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      408 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/html/_sources/generated/cmoncrawl.processor.pipeline.pipeline.ProcessorPipeline.rst.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      278 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/html/_sources/generated/cmoncrawl.processor.pipeline.pipeline.rst.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      203 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/html/_sources/generated/cmoncrawl.processor.pipeline.router.IRouter.__init__.rst.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/html/_sources/generated/cmoncrawl.processor.pipeline.router.IRouter.route.rst.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      336 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/html/_sources/generated/cmoncrawl.processor.pipeline.router.IRouter.rst.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      197 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/html/_sources/generated/cmoncrawl.processor.pipeline.router.Route.__init__.rst.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      436 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/html/_sources/generated/cmoncrawl.processor.pipeline.router.Route.rst.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      200 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/html/_sources/generated/cmoncrawl.processor.pipeline.router.Router.__init__.rst.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      212 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/html/_sources/generated/cmoncrawl.processor.pipeline.router.Router.load_extractor.rst.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      203 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/html/_sources/generated/cmoncrawl.processor.pipeline.router.Router.load_module.rst.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/html/_sources/generated/cmoncrawl.processor.pipeline.router.Router.load_module_as_extractor.rst.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      206 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/html/_sources/generated/cmoncrawl.processor.pipeline.router.Router.load_modules.rst.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      212 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/html/_sources/generated/cmoncrawl.processor.pipeline.router.Router.register_route.rst.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      215 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/html/_sources/generated/cmoncrawl.processor.pipeline.router.Router.register_routes.rst.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      183 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/html/_sources/generated/cmoncrawl.processor.pipeline.router.Router.route.rst.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      511 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/html/_sources/generated/cmoncrawl.processor.pipeline.router.Router.rst.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      287 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/html/_sources/generated/cmoncrawl.processor.pipeline.router.rst.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      433 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/html/_sources/generated/cmoncrawl.processor.pipeline.rst.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      236 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/html/_sources/generated/cmoncrawl.processor.pipeline.streamer.BaseStreamerFile.__init__.rst.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/html/_sources/generated/cmoncrawl.processor.pipeline.streamer.BaseStreamerFile.clean_up.rst.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      247 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/html/_sources/generated/cmoncrawl.processor.pipeline.streamer.BaseStreamerFile.get_file_name.rst.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      262 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/html/_sources/generated/cmoncrawl.processor.pipeline.streamer.BaseStreamerFile.metadata_to_string.rst.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      502 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/html/_sources/generated/cmoncrawl.processor.pipeline.streamer.BaseStreamerFile.rst.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      222 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/html/_sources/generated/cmoncrawl.processor.pipeline.streamer.BaseStreamerFile.stream.rst.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      215 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/html/_sources/generated/cmoncrawl.processor.pipeline.streamer.IStreamer.__init__.rst.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/html/_sources/generated/cmoncrawl.processor.pipeline.streamer.IStreamer.clean_up.rst.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      379 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/html/_sources/generated/cmoncrawl.processor.pipeline.streamer.IStreamer.rst.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      201 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/html/_sources/generated/cmoncrawl.processor.pipeline.streamer.IStreamer.stream.rst.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      227 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/html/_sources/generated/cmoncrawl.processor.pipeline.streamer.StreamerDummy.__init__.rst.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      221 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/html/_sources/generated/cmoncrawl.processor.pipeline.streamer.StreamerDummy.clean_up.rst.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      403 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/html/_sources/generated/cmoncrawl.processor.pipeline.streamer.StreamerDummy.rst.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      213 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/html/_sources/generated/cmoncrawl.processor.pipeline.streamer.StreamerDummy.stream.rst.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      236 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/html/_sources/generated/cmoncrawl.processor.pipeline.streamer.StreamerFileHTML.__init__.rst.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/html/_sources/generated/cmoncrawl.processor.pipeline.streamer.StreamerFileHTML.clean_up.rst.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      247 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/html/_sources/generated/cmoncrawl.processor.pipeline.streamer.StreamerFileHTML.get_file_name.rst.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      262 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/html/_sources/generated/cmoncrawl.processor.pipeline.streamer.StreamerFileHTML.metadata_to_string.rst.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      502 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/html/_sources/generated/cmoncrawl.processor.pipeline.streamer.StreamerFileHTML.rst.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      222 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/html/_sources/generated/cmoncrawl.processor.pipeline.streamer.StreamerFileHTML.stream.rst.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      236 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/html/_sources/generated/cmoncrawl.processor.pipeline.streamer.StreamerFileJSON.__init__.rst.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/html/_sources/generated/cmoncrawl.processor.pipeline.streamer.StreamerFileJSON.clean_up.rst.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      247 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/html/_sources/generated/cmoncrawl.processor.pipeline.streamer.StreamerFileJSON.get_file_name.rst.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      262 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/html/_sources/generated/cmoncrawl.processor.pipeline.streamer.StreamerFileJSON.metadata_to_string.rst.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      502 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/html/_sources/generated/cmoncrawl.processor.pipeline.streamer.StreamerFileJSON.rst.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      222 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/html/_sources/generated/cmoncrawl.processor.pipeline.streamer.StreamerFileJSON.stream.rst.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      359 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/html/_sources/generated/cmoncrawl.processor.pipeline.streamer.rst.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      266 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/html/_sources/generated/cmoncrawl.processor.rst.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      240 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/html/_sources/generated/cmoncrawl.rst.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      563 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/html/_sources/index.rst.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 20:28:44.349694 CmonCrawl-1.0.2/docs/build/html/_sources/misc/
+-rw-r--r--   0 runner    (1001) docker     (123)     1669 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/html/_sources/misc/domain_record.rst.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/html/_sources/misc/index.rst.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 20:28:44.349694 CmonCrawl-1.0.2/docs/build/html/_sources/prog_guide/
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/html/_sources/prog_guide/index.rst.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     4685 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/html/_sources/prog_guide/overview.rst.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1974 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/html/_sources/prog_guide/pip.rst.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1235 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/html/_sources/usage.rst.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 20:28:44.357694 CmonCrawl-1.0.2/docs/build/html/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)     4418 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/html/_static/_sphinx_javascript_frameworks_compat.js
+-rw-r--r--   0 runner    (1001) docker     (123)    14621 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/html/_static/basic.css
+-rw-r--r--   0 runner    (1001) docker     (123)      313 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/html/_static/check-solid.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     9031 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/html/_static/clipboard.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)      411 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/html/_static/copy-button.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     2010 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/html/_static/copybutton.css
+-rw-r--r--   0 runner    (1001) docker     (123)     7479 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/html/_static/copybutton.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2198 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/html/_static/copybutton_funcs.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4472 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/html/_static/doctools.js
+-rw-r--r--   0 runner    (1001) docker     (123)      419 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/html/_static/documentation_options.js
+-rw-r--r--   0 runner    (1001) docker     (123)      286 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/html/_static/file.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 20:28:44.357694 CmonCrawl-1.0.2/docs/build/html/_static/images/
+-rw-r--r--   0 runner    (1001) docker     (123)     1186 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/html/_static/images/logo_binder.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     7601 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/html/_static/images/logo_colab.png
+-rw-r--r--   0 runner    (1001) docker     (123)      681 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/html/_static/images/logo_deepnote.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1758 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/html/_static/images/logo_jupyterhub.svg
+-rw-r--r--   0 runner    (1001) docker     (123)   288580 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/html/_static/jquery-3.6.0.js
+-rw-r--r--   0 runner    (1001) docker     (123)    89501 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/html/_static/jquery.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4758 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/html/_static/language_data.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 20:28:44.225688 CmonCrawl-1.0.2/docs/build/html/_static/locales/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 20:28:44.209687 CmonCrawl-1.0.2/docs/build/html/_static/locales/ar/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 20:28:44.357694 CmonCrawl-1.0.2/docs/build/html/_static/locales/ar/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     1608 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/html/_static/locales/ar/LC_MESSAGES/booktheme.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 20:28:44.209687 CmonCrawl-1.0.2/docs/build/html/_static/locales/bg/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 20:28:44.357694 CmonCrawl-1.0.2/docs/build/html/_static/locales/bg/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     1789 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/html/_static/locales/bg/LC_MESSAGES/booktheme.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 20:28:44.209687 CmonCrawl-1.0.2/docs/build/html/_static/locales/bn/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 20:28:44.357694 CmonCrawl-1.0.2/docs/build/html/_static/locales/bn/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     1667 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/html/_static/locales/bn/LC_MESSAGES/booktheme.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 20:28:44.209687 CmonCrawl-1.0.2/docs/build/html/_static/locales/ca/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 20:28:44.357694 CmonCrawl-1.0.2/docs/build/html/_static/locales/ca/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     1231 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/html/_static/locales/ca/LC_MESSAGES/booktheme.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 20:28:44.213688 CmonCrawl-1.0.2/docs/build/html/_static/locales/cs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 20:28:44.357694 CmonCrawl-1.0.2/docs/build/html/_static/locales/cs/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     1449 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/html/_static/locales/cs/LC_MESSAGES/booktheme.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 20:28:44.213688 CmonCrawl-1.0.2/docs/build/html/_static/locales/da/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 20:28:44.357694 CmonCrawl-1.0.2/docs/build/html/_static/locales/da/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     1343 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/html/_static/locales/da/LC_MESSAGES/booktheme.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 20:28:44.213688 CmonCrawl-1.0.2/docs/build/html/_static/locales/de/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 20:28:44.357694 CmonCrawl-1.0.2/docs/build/html/_static/locales/de/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     1444 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/html/_static/locales/de/LC_MESSAGES/booktheme.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 20:28:44.213688 CmonCrawl-1.0.2/docs/build/html/_static/locales/el/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 20:28:44.361694 CmonCrawl-1.0.2/docs/build/html/_static/locales/el/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     1816 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/html/_static/locales/el/LC_MESSAGES/booktheme.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 20:28:44.213688 CmonCrawl-1.0.2/docs/build/html/_static/locales/eo/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 20:28:44.361694 CmonCrawl-1.0.2/docs/build/html/_static/locales/eo/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     1384 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/html/_static/locales/eo/LC_MESSAGES/booktheme.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 20:28:44.213688 CmonCrawl-1.0.2/docs/build/html/_static/locales/es/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 20:28:44.361694 CmonCrawl-1.0.2/docs/build/html/_static/locales/es/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     1438 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/html/_static/locales/es/LC_MESSAGES/booktheme.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 20:28:44.213688 CmonCrawl-1.0.2/docs/build/html/_static/locales/et/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 20:28:44.361694 CmonCrawl-1.0.2/docs/build/html/_static/locales/et/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     1391 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/html/_static/locales/et/LC_MESSAGES/booktheme.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 20:28:44.213688 CmonCrawl-1.0.2/docs/build/html/_static/locales/fi/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 20:28:44.361694 CmonCrawl-1.0.2/docs/build/html/_static/locales/fi/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     1409 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/html/_static/locales/fi/LC_MESSAGES/booktheme.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 20:28:44.213688 CmonCrawl-1.0.2/docs/build/html/_static/locales/fr/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 20:28:44.361694 CmonCrawl-1.0.2/docs/build/html/_static/locales/fr/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     1469 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/html/_static/locales/fr/LC_MESSAGES/booktheme.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 20:28:44.213688 CmonCrawl-1.0.2/docs/build/html/_static/locales/hr/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 20:28:44.361694 CmonCrawl-1.0.2/docs/build/html/_static/locales/hr/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     1449 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/html/_static/locales/hr/LC_MESSAGES/booktheme.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 20:28:44.213688 CmonCrawl-1.0.2/docs/build/html/_static/locales/id/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 20:28:44.361694 CmonCrawl-1.0.2/docs/build/html/_static/locales/id/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     1360 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/html/_static/locales/id/LC_MESSAGES/booktheme.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 20:28:44.217688 CmonCrawl-1.0.2/docs/build/html/_static/locales/it/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 20:28:44.361694 CmonCrawl-1.0.2/docs/build/html/_static/locales/it/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     1447 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/html/_static/locales/it/LC_MESSAGES/booktheme.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 20:28:44.217688 CmonCrawl-1.0.2/docs/build/html/_static/locales/iw/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 20:28:44.361694 CmonCrawl-1.0.2/docs/build/html/_static/locales/iw/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     1490 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/html/_static/locales/iw/LC_MESSAGES/booktheme.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 20:28:44.217688 CmonCrawl-1.0.2/docs/build/html/_static/locales/ja/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 20:28:44.361694 CmonCrawl-1.0.2/docs/build/html/_static/locales/ja/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/html/_static/locales/ja/LC_MESSAGES/booktheme.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 20:28:44.217688 CmonCrawl-1.0.2/docs/build/html/_static/locales/ko/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 20:28:44.361694 CmonCrawl-1.0.2/docs/build/html/_static/locales/ko/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     1406 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/html/_static/locales/ko/LC_MESSAGES/booktheme.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 20:28:44.217688 CmonCrawl-1.0.2/docs/build/html/_static/locales/lt/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 20:28:44.361694 CmonCrawl-1.0.2/docs/build/html/_static/locales/lt/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     1461 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/html/_static/locales/lt/LC_MESSAGES/booktheme.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 20:28:44.217688 CmonCrawl-1.0.2/docs/build/html/_static/locales/lv/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 20:28:44.361694 CmonCrawl-1.0.2/docs/build/html/_static/locales/lv/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     1450 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/html/_static/locales/lv/LC_MESSAGES/booktheme.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 20:28:44.217688 CmonCrawl-1.0.2/docs/build/html/_static/locales/ml/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 20:28:44.361694 CmonCrawl-1.0.2/docs/build/html/_static/locales/ml/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     1890 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/html/_static/locales/ml/LC_MESSAGES/booktheme.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 20:28:44.217688 CmonCrawl-1.0.2/docs/build/html/_static/locales/mr/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 20:28:44.361694 CmonCrawl-1.0.2/docs/build/html/_static/locales/mr/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     1675 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/html/_static/locales/mr/LC_MESSAGES/booktheme.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 20:28:44.217688 CmonCrawl-1.0.2/docs/build/html/_static/locales/ms/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 20:28:44.361694 CmonCrawl-1.0.2/docs/build/html/_static/locales/ms/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     1189 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/html/_static/locales/ms/LC_MESSAGES/booktheme.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 20:28:44.217688 CmonCrawl-1.0.2/docs/build/html/_static/locales/nl/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 20:28:44.361694 CmonCrawl-1.0.2/docs/build/html/_static/locales/nl/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     1398 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/html/_static/locales/nl/LC_MESSAGES/booktheme.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 20:28:44.221688 CmonCrawl-1.0.2/docs/build/html/_static/locales/no/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 20:28:44.361694 CmonCrawl-1.0.2/docs/build/html/_static/locales/no/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     1357 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/html/_static/locales/no/LC_MESSAGES/booktheme.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 20:28:44.221688 CmonCrawl-1.0.2/docs/build/html/_static/locales/pl/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 20:28:44.361694 CmonCrawl-1.0.2/docs/build/html/_static/locales/pl/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     1420 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/html/_static/locales/pl/LC_MESSAGES/booktheme.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 20:28:44.221688 CmonCrawl-1.0.2/docs/build/html/_static/locales/pt/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 20:28:44.361694 CmonCrawl-1.0.2/docs/build/html/_static/locales/pt/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     1409 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/html/_static/locales/pt/LC_MESSAGES/booktheme.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 20:28:44.221688 CmonCrawl-1.0.2/docs/build/html/_static/locales/ro/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 20:28:44.361694 CmonCrawl-1.0.2/docs/build/html/_static/locales/ro/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     1441 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/html/_static/locales/ro/LC_MESSAGES/booktheme.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 20:28:44.221688 CmonCrawl-1.0.2/docs/build/html/_static/locales/ru/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 20:28:44.361694 CmonCrawl-1.0.2/docs/build/html/_static/locales/ru/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     1797 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/html/_static/locales/ru/LC_MESSAGES/booktheme.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 20:28:44.221688 CmonCrawl-1.0.2/docs/build/html/_static/locales/sk/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 20:28:44.361694 CmonCrawl-1.0.2/docs/build/html/_static/locales/sk/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     1441 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/html/_static/locales/sk/LC_MESSAGES/booktheme.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 20:28:44.221688 CmonCrawl-1.0.2/docs/build/html/_static/locales/sl/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 20:28:44.365694 CmonCrawl-1.0.2/docs/build/html/_static/locales/sl/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     1418 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/html/_static/locales/sl/LC_MESSAGES/booktheme.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 20:28:44.221688 CmonCrawl-1.0.2/docs/build/html/_static/locales/sr/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 20:28:44.365694 CmonCrawl-1.0.2/docs/build/html/_static/locales/sr/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     1760 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/html/_static/locales/sr/LC_MESSAGES/booktheme.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 20:28:44.221688 CmonCrawl-1.0.2/docs/build/html/_static/locales/sv/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 20:28:44.365694 CmonCrawl-1.0.2/docs/build/html/_static/locales/sv/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     1391 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/html/_static/locales/sv/LC_MESSAGES/booktheme.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 20:28:44.221688 CmonCrawl-1.0.2/docs/build/html/_static/locales/ta/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 20:28:44.365694 CmonCrawl-1.0.2/docs/build/html/_static/locales/ta/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     1968 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/html/_static/locales/ta/LC_MESSAGES/booktheme.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 20:28:44.225688 CmonCrawl-1.0.2/docs/build/html/_static/locales/te/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 20:28:44.365694 CmonCrawl-1.0.2/docs/build/html/_static/locales/te/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     1834 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/html/_static/locales/te/LC_MESSAGES/booktheme.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 20:28:44.225688 CmonCrawl-1.0.2/docs/build/html/_static/locales/tg/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 20:28:44.365694 CmonCrawl-1.0.2/docs/build/html/_static/locales/tg/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     1710 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/html/_static/locales/tg/LC_MESSAGES/booktheme.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 20:28:44.225688 CmonCrawl-1.0.2/docs/build/html/_static/locales/th/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 20:28:44.365694 CmonCrawl-1.0.2/docs/build/html/_static/locales/th/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     1860 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/html/_static/locales/th/LC_MESSAGES/booktheme.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 20:28:44.225688 CmonCrawl-1.0.2/docs/build/html/_static/locales/tl/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 20:28:44.365694 CmonCrawl-1.0.2/docs/build/html/_static/locales/tl/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     1259 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/html/_static/locales/tl/LC_MESSAGES/booktheme.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 20:28:44.225688 CmonCrawl-1.0.2/docs/build/html/_static/locales/tr/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 20:28:44.365694 CmonCrawl-1.0.2/docs/build/html/_static/locales/tr/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     1405 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/html/_static/locales/tr/LC_MESSAGES/booktheme.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 20:28:44.225688 CmonCrawl-1.0.2/docs/build/html/_static/locales/uk/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 20:28:44.365694 CmonCrawl-1.0.2/docs/build/html/_static/locales/uk/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     1756 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/html/_static/locales/uk/LC_MESSAGES/booktheme.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 20:28:44.225688 CmonCrawl-1.0.2/docs/build/html/_static/locales/ur/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 20:28:44.365694 CmonCrawl-1.0.2/docs/build/html/_static/locales/ur/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     1460 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/html/_static/locales/ur/LC_MESSAGES/booktheme.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 20:28:44.225688 CmonCrawl-1.0.2/docs/build/html/_static/locales/vi/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 20:28:44.365694 CmonCrawl-1.0.2/docs/build/html/_static/locales/vi/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     1487 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/html/_static/locales/vi/LC_MESSAGES/booktheme.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 20:28:44.225688 CmonCrawl-1.0.2/docs/build/html/_static/locales/zh_CN/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 20:28:44.365694 CmonCrawl-1.0.2/docs/build/html/_static/locales/zh_CN/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     1279 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/html/_static/locales/zh_CN/LC_MESSAGES/booktheme.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 20:28:44.225688 CmonCrawl-1.0.2/docs/build/html/_static/locales/zh_TW/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 20:28:44.365694 CmonCrawl-1.0.2/docs/build/html/_static/locales/zh_TW/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     1323 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/html/_static/locales/zh_TW/LC_MESSAGES/booktheme.po
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/html/_static/minus.png
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/html/_static/plus.png
+-rw-r--r--   0 runner    (1001) docker     (123)     5510 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/html/_static/pygments.css
+-rw-r--r--   0 runner    (1001) docker     (123)      419 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/html/_static/sbt-webpack-macros.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 20:28:44.365694 CmonCrawl-1.0.2/docs/build/html/_static/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)    87299 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/html/_static/scripts/pydata-sphinx-theme.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3388 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/html/_static/scripts/sphinx-book-theme.js
+-rw-r--r--   0 runner    (1001) docker     (123)    15106 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/html/_static/scripts/sphinx-book-theme.js.map
+-rw-r--r--   0 runner    (1001) docker     (123)    18215 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/html/_static/searchtools.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4712 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/html/_static/sphinx_highlight.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 20:28:44.365694 CmonCrawl-1.0.2/docs/build/html/_static/styles/
+-rw-r--r--   0 runner    (1001) docker     (123)   162094 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/html/_static/styles/pydata-sphinx-theme.css
+-rw-r--r--   0 runner    (1001) docker     (123)    20970 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/html/_static/styles/sphinx-book-theme.css
+-rw-r--r--   0 runner    (1001) docker     (123)     5488 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/html/_static/styles/theme.css
+-rw-r--r--   0 runner    (1001) docker     (123)    68420 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/html/_static/underscore-1.13.1.js
+-rw-r--r--   0 runner    (1001) docker     (123)    19530 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/html/_static/underscore.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 20:28:44.229688 CmonCrawl-1.0.2/docs/build/html/_static/vendor/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 20:28:44.229688 CmonCrawl-1.0.2/docs/build/html/_static/vendor/fontawesome/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 20:28:44.365694 CmonCrawl-1.0.2/docs/build/html/_static/vendor/fontawesome/5.13.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1548 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/html/_static/vendor/fontawesome/5.13.0/LICENSE.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 20:28:44.365694 CmonCrawl-1.0.2/docs/build/html/_static/vendor/fontawesome/5.13.0/css/
+-rw-r--r--   0 runner    (1001) docker     (123)    58578 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/html/_static/vendor/fontawesome/5.13.0/css/all.min.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 20:28:44.373695 CmonCrawl-1.0.2/docs/build/html/_static/vendor/fontawesome/5.13.0/webfonts/
+-rw-r--r--   0 runner    (1001) docker     (123)   133034 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/html/_static/vendor/fontawesome/5.13.0/webfonts/fa-brands-400.eot
+-rw-r--r--   0 runner    (1001) docker     (123)   715890 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/html/_static/vendor/fontawesome/5.13.0/webfonts/fa-brands-400.svg
+-rw-r--r--   0 runner    (1001) docker     (123)   132728 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/html/_static/vendor/fontawesome/5.13.0/webfonts/fa-brands-400.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)    89824 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/html/_static/vendor/fontawesome/5.13.0/webfonts/fa-brands-400.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    76612 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/html/_static/vendor/fontawesome/5.13.0/webfonts/fa-brands-400.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    34390 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/html/_static/vendor/fontawesome/5.13.0/webfonts/fa-regular-400.eot
+-rw-r--r--   0 runner    (1001) docker     (123)   144322 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/html/_static/vendor/fontawesome/5.13.0/webfonts/fa-regular-400.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    34092 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/html/_static/vendor/fontawesome/5.13.0/webfonts/fa-regular-400.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)    16800 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/html/_static/vendor/fontawesome/5.13.0/webfonts/fa-regular-400.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    13584 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/html/_static/vendor/fontawesome/5.13.0/webfonts/fa-regular-400.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)   202902 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/html/_static/vendor/fontawesome/5.13.0/webfonts/fa-solid-900.eot
+-rw-r--r--   0 runner    (1001) docker     (123)   897426 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/html/_static/vendor/fontawesome/5.13.0/webfonts/fa-solid-900.svg
+-rw-r--r--   0 runner    (1001) docker     (123)   202616 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/html/_static/vendor/fontawesome/5.13.0/webfonts/fa-solid-900.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   103300 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/html/_static/vendor/fontawesome/5.13.0/webfonts/fa-solid-900.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    79444 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/html/_static/vendor/fontawesome/5.13.0/webfonts/fa-solid-900.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)     1361 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/html/_static/webpack-macros.html
+-rw-r--r--   0 runner    (1001) docker     (123)    14718 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/html/api.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 20:28:44.373695 CmonCrawl-1.0.2/docs/build/html/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)    17247 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/html/cli/cli.html
+-rw-r--r--   0 runner    (1001) docker     (123)    20066 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/html/cli/download.html
+-rw-r--r--   0 runner    (1001) docker     (123)    21279 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/html/cli/extract.html
+-rw-r--r--   0 runner    (1001) docker     (123)    16088 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/html/cli/index.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 20:28:44.373695 CmonCrawl-1.0.2/docs/build/html/extraction/
+-rw-r--r--   0 runner    (1001) docker     (123)    25464 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/html/extraction/config_file.html
+-rw-r--r--   0 runner    (1001) docker     (123)    22074 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/html/extraction/creating_extractor.html
+-rw-r--r--   0 runner    (1001) docker     (123)    16080 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/html/extraction/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)    17188 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/html/extraction/utils.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 20:28:44.397696 CmonCrawl-1.0.2/docs/build/html/generated/
+-rw-r--r--   0 runner    (1001) docker     (123)    15445 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/html/generated/cmoncrawl.aggregator.html
+-rw-r--r--   0 runner    (1001) docker     (123)    20850 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/html/generated/cmoncrawl.aggregator.index_query.IndexAggregator.__init__.html
+-rw-r--r--   0 runner    (1001) docker     (123)    18561 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/html/generated/cmoncrawl.aggregator.index_query.IndexAggregator.aclose.html
+-rw-r--r--   0 runner    (1001) docker     (123)    17264 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/html/generated/cmoncrawl.aggregator.index_query.IndexAggregator.aopen.html
+-rw-r--r--   0 runner    (1001) docker     (123)    17840 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/html/generated/cmoncrawl.aggregator.index_query.IndexAggregator.get_all_CC_indexes.html
+-rw-r--r--   0 runner    (1001) docker     (123)    19556 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/html/generated/cmoncrawl.aggregator.index_query.IndexAggregator.get_captured_responses.html
+-rw-r--r--   0 runner    (1001) docker     (123)    18596 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/html/generated/cmoncrawl.aggregator.index_query.IndexAggregator.get_number_of_pages.html
+-rw-r--r--   0 runner    (1001) docker     (123)    28606 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/html/generated/cmoncrawl.aggregator.index_query.IndexAggregator.html
+-rw-r--r--   0 runner    (1001) docker     (123)    16097 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/html/generated/cmoncrawl.aggregator.index_query.html
+-rw-r--r--   0 runner    (1001) docker     (123)    15202 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/html/generated/cmoncrawl.aggregator.utils.helpers.html
+-rw-r--r--   0 runner    (1001) docker     (123)    15824 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/html/generated/cmoncrawl.aggregator.utils.html
+-rw-r--r--   0 runner    (1001) docker     (123)    20653 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/html/generated/cmoncrawl.aggregator.utils.ndjson_decoder.Decoder.__init__.html
+-rw-r--r--   0 runner    (1001) docker     (123)    17509 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/html/generated/cmoncrawl.aggregator.utils.ndjson_decoder.Decoder.decode.html
+-rw-r--r--   0 runner    (1001) docker     (123)    25373 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/html/generated/cmoncrawl.aggregator.utils.ndjson_decoder.Decoder.html
+-rw-r--r--   0 runner    (1001) docker     (123)    17442 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/html/generated/cmoncrawl.aggregator.utils.ndjson_decoder.Decoder.raw_decode.html
+-rw-r--r--   0 runner    (1001) docker     (123)    15546 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/html/generated/cmoncrawl.aggregator.utils.ndjson_decoder.html
+-rw-r--r--   0 runner    (1001) docker     (123)    15545 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/html/generated/cmoncrawl.common.html
+-rw-r--r--   0 runner    (1001) docker     (123)    14638 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/html/generated/cmoncrawl.common.loggers.html
+-rw-r--r--   0 runner    (1001) docker     (123)    17736 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/html/generated/cmoncrawl.common.types.DomainCrawl.__init__.html
+-rw-r--r--   0 runner    (1001) docker     (123)    21085 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/html/generated/cmoncrawl.common.types.DomainCrawl.html
+-rw-r--r--   0 runner    (1001) docker     (123)    19154 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/html/generated/cmoncrawl.common.types.DomainRecord.__init__.html
+-rw-r--r--   0 runner    (1001) docker     (123)    18089 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/html/generated/cmoncrawl.common.types.DomainRecord.from_dict.html
+-rw-r--r--   0 runner    (1001) docker     (123)    18381 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/html/generated/cmoncrawl.common.types.DomainRecord.from_json.html
+-rw-r--r--   0 runner    (1001) docker     (123)    26445 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/html/generated/cmoncrawl.common.types.DomainRecord.html
+-rw-r--r--   0 runner    (1001) docker     (123)    19292 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/html/generated/cmoncrawl.common.types.DomainRecord.schema.html
+-rw-r--r--   0 runner    (1001) docker     (123)    17907 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/html/generated/cmoncrawl.common.types.DomainRecord.to_dict.html
+-rw-r--r--   0 runner    (1001) docker     (123)    20725 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/html/generated/cmoncrawl.common.types.DomainRecord.to_json.html
+-rw-r--r--   0 runner    (1001) docker     (123)    17437 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/html/generated/cmoncrawl.common.types.ExtractConfig.__init__.html
+-rw-r--r--   0 runner    (1001) docker     (123)    18110 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/html/generated/cmoncrawl.common.types.ExtractConfig.from_dict.html
+-rw-r--r--   0 runner    (1001) docker     (123)    18402 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/html/generated/cmoncrawl.common.types.ExtractConfig.from_json.html
+-rw-r--r--   0 runner    (1001) docker     (123)    22253 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/html/generated/cmoncrawl.common.types.ExtractConfig.html
+-rw-r--r--   0 runner    (1001) docker     (123)    19313 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/html/generated/cmoncrawl.common.types.ExtractConfig.schema.html
+-rw-r--r--   0 runner    (1001) docker     (123)    17928 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/html/generated/cmoncrawl.common.types.ExtractConfig.to_dict.html
+-rw-r--r--   0 runner    (1001) docker     (123)    20750 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/html/generated/cmoncrawl.common.types.ExtractConfig.to_json.html
+-rw-r--r--   0 runner    (1001) docker     (123)    17965 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/html/generated/cmoncrawl.common.types.ExtractorConfig.__init__.html
+-rw-r--r--   0 runner    (1001) docker     (123)    18152 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/html/generated/cmoncrawl.common.types.ExtractorConfig.from_dict.html
+-rw-r--r--   0 runner    (1001) docker     (123)    18444 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/html/generated/cmoncrawl.common.types.ExtractorConfig.from_json.html
+-rw-r--r--   0 runner    (1001) docker     (123)    23452 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/html/generated/cmoncrawl.common.types.ExtractorConfig.html
+-rw-r--r--   0 runner    (1001) docker     (123)    19355 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/html/generated/cmoncrawl.common.types.ExtractorConfig.schema.html
+-rw-r--r--   0 runner    (1001) docker     (123)    17970 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/html/generated/cmoncrawl.common.types.ExtractorConfig.to_dict.html
+-rw-r--r--   0 runner    (1001) docker     (123)    20772 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/html/generated/cmoncrawl.common.types.ExtractorConfig.to_json.html
+-rw-r--r--   0 runner    (1001) docker     (123)    18059 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/html/generated/cmoncrawl.common.types.PipeMetadata.__init__.html
+-rw-r--r--   0 runner    (1001) docker     (123)    22314 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/html/generated/cmoncrawl.common.types.PipeMetadata.html
+-rw-r--r--   0 runner    (1001) docker     (123)    17470 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/html/generated/cmoncrawl.common.types.RetrieveResponse.__init__.html
+-rw-r--r--   0 runner    (1001) docker     (123)    20597 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/html/generated/cmoncrawl.common.types.RetrieveResponse.html
+-rw-r--r--   0 runner    (1001) docker     (123)    17108 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/html/generated/cmoncrawl.common.types.RoutesConfig.__init__.html
+-rw-r--r--   0 runner    (1001) docker     (123)    18089 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/html/generated/cmoncrawl.common.types.RoutesConfig.from_dict.html
+-rw-r--r--   0 runner    (1001) docker     (123)    18381 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/html/generated/cmoncrawl.common.types.RoutesConfig.from_json.html
+-rw-r--r--   0 runner    (1001) docker     (123)    21617 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/html/generated/cmoncrawl.common.types.RoutesConfig.html
+-rw-r--r--   0 runner    (1001) docker     (123)    19292 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/html/generated/cmoncrawl.common.types.RoutesConfig.schema.html
+-rw-r--r--   0 runner    (1001) docker     (123)    17907 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/html/generated/cmoncrawl.common.types.RoutesConfig.to_dict.html
+-rw-r--r--   0 runner    (1001) docker     (123)    20657 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/html/generated/cmoncrawl.common.types.RoutesConfig.to_json.html
+-rw-r--r--   0 runner    (1001) docker     (123)    17489 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/html/generated/cmoncrawl.common.types.html
+-rw-r--r--   0 runner    (1001) docker     (123)    15473 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/html/generated/cmoncrawl.html
+-rw-r--r--   0 runner    (1001) docker     (123)    15586 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/html/generated/cmoncrawl.processor.extraction.filters.html
+-rw-r--r--   0 runner    (1001) docker     (123)    15664 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/html/generated/cmoncrawl.processor.extraction.html
+-rw-r--r--   0 runner    (1001) docker     (123)    17047 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/html/generated/cmoncrawl.processor.extraction.utils.html
+-rw-r--r--   0 runner    (1001) docker     (123)    15567 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/html/generated/cmoncrawl.processor.html
+-rw-r--r--   0 runner    (1001) docker     (123)    18794 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/html/generated/cmoncrawl.processor.pipeline.downloader.AsyncDownloader.__init__.html
+-rw-r--r--   0 runner    (1001) docker     (123)    18692 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/html/generated/cmoncrawl.processor.pipeline.downloader.AsyncDownloader.aclose.html
+-rw-r--r--   0 runner    (1001) docker     (123)    17371 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/html/generated/cmoncrawl.processor.pipeline.downloader.AsyncDownloader.aopen.html
+-rw-r--r--   0 runner    (1001) docker     (123)    17399 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/html/generated/cmoncrawl.processor.pipeline.downloader.AsyncDownloader.download.html
+-rw-r--r--   0 runner    (1001) docker     (123)    24091 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/html/generated/cmoncrawl.processor.pipeline.downloader.AsyncDownloader.html
+-rw-r--r--   0 runner    (1001) docker     (123)    18163 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/html/generated/cmoncrawl.processor.pipeline.downloader.AsyncDownloader.unwrap.html
+-rw-r--r--   0 runner    (1001) docker     (123)    18242 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/html/generated/cmoncrawl.processor.pipeline.downloader.DownloaderDummy.__init__.html
+-rw-r--r--   0 runner    (1001) docker     (123)    17431 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/html/generated/cmoncrawl.processor.pipeline.downloader.DownloaderDummy.download.html
+-rw-r--r--   0 runner    (1001) docker     (123)    17227 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/html/generated/cmoncrawl.processor.pipeline.downloader.DownloaderDummy.extract_url.html
+-rw-r--r--   0 runner    (1001) docker     (123)    17249 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/html/generated/cmoncrawl.processor.pipeline.downloader.DownloaderDummy.extract_year.html
+-rw-r--r--   0 runner    (1001) docker     (123)    23249 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/html/generated/cmoncrawl.processor.pipeline.downloader.DownloaderDummy.html
+-rw-r--r--   0 runner    (1001) docker     (123)    17402 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/html/generated/cmoncrawl.processor.pipeline.downloader.DownloaderDummy.mine_metadata.html
+-rw-r--r--   0 runner    (1001) docker     (123)    16828 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/html/generated/cmoncrawl.processor.pipeline.downloader.IDownloader.__init__.html
+-rw-r--r--   0 runner    (1001) docker     (123)    17922 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/html/generated/cmoncrawl.processor.pipeline.downloader.IDownloader.download.html
+-rw-r--r--   0 runner    (1001) docker     (123)    18960 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/html/generated/cmoncrawl.processor.pipeline.downloader.IDownloader.html
+-rw-r--r--   0 runner    (1001) docker     (123)    16456 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/html/generated/cmoncrawl.processor.pipeline.downloader.html
+-rw-r--r--   0 runner    (1001) docker     (123)    17347 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/html/generated/cmoncrawl.processor.pipeline.extractor.BaseExtractor.__init__.html
+-rw-r--r--   0 runner    (1001) docker     (123)    17993 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/html/generated/cmoncrawl.processor.pipeline.extractor.BaseExtractor.extract.html
+-rw-r--r--   0 runner    (1001) docker     (123)    18135 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/html/generated/cmoncrawl.processor.pipeline.extractor.BaseExtractor.extract_soup.html
+-rw-r--r--   0 runner    (1001) docker     (123)    17686 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/html/generated/cmoncrawl.processor.pipeline.extractor.BaseExtractor.filter_raw.html
+-rw-r--r--   0 runner    (1001) docker     (123)    17693 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/html/generated/cmoncrawl.processor.pipeline.extractor.BaseExtractor.filter_soup.html
+-rw-r--r--   0 runner    (1001) docker     (123)    21657 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/html/generated/cmoncrawl.processor.pipeline.extractor.BaseExtractor.html
+-rw-r--r--   0 runner    (1001) docker     (123)    17665 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/html/generated/cmoncrawl.processor.pipeline.extractor.BaseExtractor.preprocess.html
+-rw-r--r--   0 runner    (1001) docker     (123)    17390 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/html/generated/cmoncrawl.processor.pipeline.extractor.DomainRecordExtractor.__init__.html
+-rw-r--r--   0 runner    (1001) docker     (123)    18161 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/html/generated/cmoncrawl.processor.pipeline.extractor.DomainRecordExtractor.extract.html
+-rw-r--r--   0 runner    (1001) docker     (123)    17713 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/html/generated/cmoncrawl.processor.pipeline.extractor.DomainRecordExtractor.extract_soup.html
+-rw-r--r--   0 runner    (1001) docker     (123)    17705 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/html/generated/cmoncrawl.processor.pipeline.extractor.DomainRecordExtractor.filter_raw.html
+-rw-r--r--   0 runner    (1001) docker     (123)    17861 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/html/generated/cmoncrawl.processor.pipeline.extractor.DomainRecordExtractor.filter_soup.html
+-rw-r--r--   0 runner    (1001) docker     (123)    21894 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/html/generated/cmoncrawl.processor.pipeline.extractor.DomainRecordExtractor.html
+-rw-r--r--   0 runner    (1001) docker     (123)    17769 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/html/generated/cmoncrawl.processor.pipeline.extractor.DomainRecordExtractor.preprocess.html
+-rw-r--r--   0 runner    (1001) docker     (123)    17222 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/html/generated/cmoncrawl.processor.pipeline.extractor.HTMLExtractor.__init__.html
+-rw-r--r--   0 runner    (1001) docker     (123)    17993 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/html/generated/cmoncrawl.processor.pipeline.extractor.HTMLExtractor.extract.html
+-rw-r--r--   0 runner    (1001) docker     (123)    17545 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/html/generated/cmoncrawl.processor.pipeline.extractor.HTMLExtractor.extract_soup.html
+-rw-r--r--   0 runner    (1001) docker     (123)    17537 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/html/generated/cmoncrawl.processor.pipeline.extractor.HTMLExtractor.filter_raw.html
+-rw-r--r--   0 runner    (1001) docker     (123)    17693 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/html/generated/cmoncrawl.processor.pipeline.extractor.HTMLExtractor.filter_soup.html
+-rw-r--r--   0 runner    (1001) docker     (123)    21598 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/html/generated/cmoncrawl.processor.pipeline.extractor.HTMLExtractor.html
+-rw-r--r--   0 runner    (1001) docker     (123)    17621 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/html/generated/cmoncrawl.processor.pipeline.extractor.HTMLExtractor.preprocess.html
+-rw-r--r--   0 runner    (1001) docker     (123)    16785 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/html/generated/cmoncrawl.processor.pipeline.extractor.IExtractor.__init__.html
+-rw-r--r--   0 runner    (1001) docker     (123)    17913 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/html/generated/cmoncrawl.processor.pipeline.extractor.IExtractor.extract.html
+-rw-r--r--   0 runner    (1001) docker     (123)    18884 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/html/generated/cmoncrawl.processor.pipeline.extractor.IExtractor.html
+-rw-r--r--   0 runner    (1001) docker     (123)    16907 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/html/generated/cmoncrawl.processor.pipeline.extractor.html
+-rw-r--r--   0 runner    (1001) docker     (123)    16815 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/html/generated/cmoncrawl.processor.pipeline.html
+-rw-r--r--   0 runner    (1001) docker     (123)    18210 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/html/generated/cmoncrawl.processor.pipeline.pipeline.ProcessorPipeline.__init__.html
+-rw-r--r--   0 runner    (1001) docker     (123)    21591 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/html/generated/cmoncrawl.processor.pipeline.pipeline.ProcessorPipeline.html
+-rw-r--r--   0 runner    (1001) docker     (123)    17922 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/html/generated/cmoncrawl.processor.pipeline.pipeline.ProcessorPipeline.process_domain_record.html
+-rw-r--r--   0 runner    (1001) docker     (123)    15650 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/html/generated/cmoncrawl.processor.pipeline.pipeline.html
+-rw-r--r--   0 runner    (1001) docker     (123)    16660 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/html/generated/cmoncrawl.processor.pipeline.router.IRouter.__init__.html
+-rw-r--r--   0 runner    (1001) docker     (123)    18604 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/html/generated/cmoncrawl.processor.pipeline.router.IRouter.html
+-rw-r--r--   0 runner    (1001) docker     (123)    18128 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/html/generated/cmoncrawl.processor.pipeline.router.IRouter.route.html
+-rw-r--r--   0 runner    (1001) docker     (123)    17834 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/html/generated/cmoncrawl.processor.pipeline.router.Route.__init__.html
+-rw-r--r--   0 runner    (1001) docker     (123)    21472 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/html/generated/cmoncrawl.processor.pipeline.router.Route.html
+-rw-r--r--   0 runner    (1001) docker     (123)    16675 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/html/generated/cmoncrawl.processor.pipeline.router.Router.__init__.html
+-rw-r--r--   0 runner    (1001) docker     (123)    21103 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/html/generated/cmoncrawl.processor.pipeline.router.Router.html
+-rw-r--r--   0 runner    (1001) docker     (123)    17409 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/html/generated/cmoncrawl.processor.pipeline.router.Router.load_extractor.html
+-rw-r--r--   0 runner    (1001) docker     (123)    17033 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/html/generated/cmoncrawl.processor.pipeline.router.Router.load_module.html
+-rw-r--r--   0 runner    (1001) docker     (123)    17142 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/html/generated/cmoncrawl.processor.pipeline.router.Router.load_module_as_extractor.html
+-rw-r--r--   0 runner    (1001) docker     (123)    17041 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/html/generated/cmoncrawl.processor.pipeline.router.Router.load_modules.html
+-rw-r--r--   0 runner    (1001) docker     (123)    18585 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/html/generated/cmoncrawl.processor.pipeline.router.Router.register_route.html
+-rw-r--r--   0 runner    (1001) docker     (123)    17301 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/html/generated/cmoncrawl.processor.pipeline.router.Router.register_routes.html
+-rw-r--r--   0 runner    (1001) docker     (123)    18040 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/html/generated/cmoncrawl.processor.pipeline.router.Router.route.html
+-rw-r--r--   0 runner    (1001) docker     (123)    16303 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/html/generated/cmoncrawl.processor.pipeline.router.html
+-rw-r--r--   0 runner    (1001) docker     (123)    18500 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/html/generated/cmoncrawl.processor.pipeline.streamer.BaseStreamerFile.__init__.html
+-rw-r--r--   0 runner    (1001) docker     (123)    17190 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/html/generated/cmoncrawl.processor.pipeline.streamer.BaseStreamerFile.clean_up.html
+-rw-r--r--   0 runner    (1001) docker     (123)    17424 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/html/generated/cmoncrawl.processor.pipeline.streamer.BaseStreamerFile.get_file_name.html
+-rw-r--r--   0 runner    (1001) docker     (123)    23620 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/html/generated/cmoncrawl.processor.pipeline.streamer.BaseStreamerFile.html
+-rw-r--r--   0 runner    (1001) docker     (123)    17755 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/html/generated/cmoncrawl.processor.pipeline.streamer.BaseStreamerFile.metadata_to_string.html
+-rw-r--r--   0 runner    (1001) docker     (123)    17941 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/html/generated/cmoncrawl.processor.pipeline.streamer.BaseStreamerFile.stream.html
+-rw-r--r--   0 runner    (1001) docker     (123)    16750 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/html/generated/cmoncrawl.processor.pipeline.streamer.IStreamer.__init__.html
+-rw-r--r--   0 runner    (1001) docker     (123)    17072 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/html/generated/cmoncrawl.processor.pipeline.streamer.IStreamer.clean_up.html
+-rw-r--r--   0 runner    (1001) docker     (123)    19248 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/html/generated/cmoncrawl.processor.pipeline.streamer.IStreamer.html
+-rw-r--r--   0 runner    (1001) docker     (123)    17855 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/html/generated/cmoncrawl.processor.pipeline.streamer.IStreamer.stream.html
+-rw-r--r--   0 runner    (1001) docker     (123)    16834 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/html/generated/cmoncrawl.processor.pipeline.streamer.StreamerDummy.__init__.html
+-rw-r--r--   0 runner    (1001) docker     (123)    16950 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/html/generated/cmoncrawl.processor.pipeline.streamer.StreamerDummy.clean_up.html
+-rw-r--r--   0 runner    (1001) docker     (123)    19364 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/html/generated/cmoncrawl.processor.pipeline.streamer.StreamerDummy.html
+-rw-r--r--   0 runner    (1001) docker     (123)    17729 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/html/generated/cmoncrawl.processor.pipeline.streamer.StreamerDummy.stream.html
+-rw-r--r--   0 runner    (1001) docker     (123)    17320 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/html/generated/cmoncrawl.processor.pipeline.streamer.StreamerFileHTML.__init__.html
+-rw-r--r--   0 runner    (1001) docker     (123)    17190 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/html/generated/cmoncrawl.processor.pipeline.streamer.StreamerFileHTML.clean_up.html
+-rw-r--r--   0 runner    (1001) docker     (123)    17424 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/html/generated/cmoncrawl.processor.pipeline.streamer.StreamerFileHTML.get_file_name.html
+-rw-r--r--   0 runner    (1001) docker     (123)    21251 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/html/generated/cmoncrawl.processor.pipeline.streamer.StreamerFileHTML.html
+-rw-r--r--   0 runner    (1001) docker     (123)    17672 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/html/generated/cmoncrawl.processor.pipeline.streamer.StreamerFileHTML.metadata_to_string.html
+-rw-r--r--   0 runner    (1001) docker     (123)    17969 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/html/generated/cmoncrawl.processor.pipeline.streamer.StreamerFileHTML.stream.html
+-rw-r--r--   0 runner    (1001) docker     (123)    17904 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/html/generated/cmoncrawl.processor.pipeline.streamer.StreamerFileJSON.__init__.html
+-rw-r--r--   0 runner    (1001) docker     (123)    17190 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/html/generated/cmoncrawl.processor.pipeline.streamer.StreamerFileJSON.clean_up.html
+-rw-r--r--   0 runner    (1001) docker     (123)    17424 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/html/generated/cmoncrawl.processor.pipeline.streamer.StreamerFileJSON.get_file_name.html
+-rw-r--r--   0 runner    (1001) docker     (123)    22447 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/html/generated/cmoncrawl.processor.pipeline.streamer.StreamerFileJSON.html
+-rw-r--r--   0 runner    (1001) docker     (123)    17672 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/html/generated/cmoncrawl.processor.pipeline.streamer.StreamerFileJSON.metadata_to_string.html
+-rw-r--r--   0 runner    (1001) docker     (123)    17455 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/html/generated/cmoncrawl.processor.pipeline.streamer.StreamerFileJSON.stream.html
+-rw-r--r--   0 runner    (1001) docker     (123)    17327 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/html/generated/cmoncrawl.processor.pipeline.streamer.html
+-rw-r--r--   0 runner    (1001) docker     (123)    55272 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/html/genindex.html
+-rw-r--r--   0 runner    (1001) docker     (123)    22125 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/html/index.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 20:28:44.397696 CmonCrawl-1.0.2/docs/build/html/misc/
+-rw-r--r--   0 runner    (1001) docker     (123)    18439 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/html/misc/domain_record.html
+-rw-r--r--   0 runner    (1001) docker     (123)    14882 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/html/misc/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)    13098 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/html/objects.inv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 20:28:44.397696 CmonCrawl-1.0.2/docs/build/html/prog_guide/
+-rw-r--r--   0 runner    (1001) docker     (123)    16012 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/html/prog_guide/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)    26474 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/html/prog_guide/overview.html
+-rw-r--r--   0 runner    (1001) docker     (123)    21406 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/html/prog_guide/pip.html
+-rw-r--r--   0 runner    (1001) docker     (123)    17907 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/html/py-modindex.html
+-rw-r--r--   0 runner    (1001) docker     (123)    13230 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/html/search.html
+-rw-r--r--   0 runner    (1001) docker     (123)    99618 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/html/searchindex.js
+-rw-r--r--   0 runner    (1001) docker     (123)    17202 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/build/html/usage.html
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)      769 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 20:28:44.397696 CmonCrawl-1.0.2/docs/source/
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/source/api.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 20:28:44.397696 CmonCrawl-1.0.2/docs/source/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)     1175 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/source/cli/cli.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1987 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/source/cli/download.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2753 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/source/cli/extract.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/source/cli/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2482 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/source/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 20:28:44.401696 CmonCrawl-1.0.2/docs/source/extraction/
+-rw-r--r--   0 runner    (1001) docker     (123)     3910 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/source/extraction/config_file.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2392 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/source/extraction/creating_extractor.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/source/extraction/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      861 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/source/extraction/utils.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 20:28:44.425697 CmonCrawl-1.0.2/docs/source/generated/
+-rw-r--r--   0 runner    (1001) docker     (123)      220 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/source/generated/cmoncrawl.aggregator.index_query.IndexAggregator.__init__.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      206 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/source/generated/cmoncrawl.aggregator.index_query.IndexAggregator.aclose.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      203 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/source/generated/cmoncrawl.aggregator.index_query.IndexAggregator.aopen.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/source/generated/cmoncrawl.aggregator.index_query.IndexAggregator.get_all_CC_indexes.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      258 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/source/generated/cmoncrawl.aggregator.index_query.IndexAggregator.get_captured_responses.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      251 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/source/generated/cmoncrawl.aggregator.index_query.IndexAggregator.get_number_of_pages.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      530 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/source/generated/cmoncrawl.aggregator.index_query.IndexAggregator.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      391 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/source/generated/cmoncrawl.aggregator.index_query.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      269 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/source/generated/cmoncrawl.aggregator.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      250 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/source/generated/cmoncrawl.aggregator.utils.helpers.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      223 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/source/generated/cmoncrawl.aggregator.utils.ndjson_decoder.Decoder.__init__.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/source/generated/cmoncrawl.aggregator.utils.ndjson_decoder.Decoder.decode.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      223 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/source/generated/cmoncrawl.aggregator.utils.ndjson_decoder.Decoder.raw_decode.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      383 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/source/generated/cmoncrawl.aggregator.utils.ndjson_decoder.Decoder.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      282 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/source/generated/cmoncrawl.aggregator.utils.ndjson_decoder.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      304 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/source/generated/cmoncrawl.aggregator.utils.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/source/generated/cmoncrawl.common.loggers.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      245 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/source/generated/cmoncrawl.common.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      176 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/source/generated/cmoncrawl.common.types.DomainCrawl.__init__.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      427 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/source/generated/cmoncrawl.common.types.DomainCrawl.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      179 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/source/generated/cmoncrawl.common.types.DomainRecord.__init__.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      176 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/source/generated/cmoncrawl.common.types.DomainRecord.from_dict.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      176 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/source/generated/cmoncrawl.common.types.DomainRecord.from_json.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      687 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/source/generated/cmoncrawl.common.types.DomainRecord.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/source/generated/cmoncrawl.common.types.DomainRecord.schema.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      170 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/source/generated/cmoncrawl.common.types.DomainRecord.to_dict.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      170 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/source/generated/cmoncrawl.common.types.DomainRecord.to_json.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      182 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/source/generated/cmoncrawl.common.types.ExtractConfig.__init__.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      179 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/source/generated/cmoncrawl.common.types.ExtractConfig.from_dict.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      179 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/source/generated/cmoncrawl.common.types.ExtractConfig.from_json.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      568 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/source/generated/cmoncrawl.common.types.ExtractConfig.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/source/generated/cmoncrawl.common.types.ExtractConfig.schema.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/source/generated/cmoncrawl.common.types.ExtractConfig.to_dict.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/source/generated/cmoncrawl.common.types.ExtractConfig.to_json.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/source/generated/cmoncrawl.common.types.ExtractorConfig.__init__.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      185 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/source/generated/cmoncrawl.common.types.ExtractorConfig.from_dict.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      185 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/source/generated/cmoncrawl.common.types.ExtractorConfig.from_json.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      604 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/source/generated/cmoncrawl.common.types.ExtractorConfig.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      174 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/source/generated/cmoncrawl.common.types.ExtractorConfig.schema.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      179 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/source/generated/cmoncrawl.common.types.ExtractorConfig.to_dict.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      179 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/source/generated/cmoncrawl.common.types.ExtractorConfig.to_json.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      179 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/source/generated/cmoncrawl.common.types.PipeMetadata.__init__.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      536 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/source/generated/cmoncrawl.common.types.PipeMetadata.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      191 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/source/generated/cmoncrawl.common.types.RetrieveResponse.__init__.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      461 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/source/generated/cmoncrawl.common.types.RetrieveResponse.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      179 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/source/generated/cmoncrawl.common.types.RoutesConfig.__init__.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      176 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/source/generated/cmoncrawl.common.types.RoutesConfig.from_dict.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      176 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/source/generated/cmoncrawl.common.types.RoutesConfig.from_json.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      553 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/source/generated/cmoncrawl.common.types.RoutesConfig.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/source/generated/cmoncrawl.common.types.RoutesConfig.schema.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      170 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/source/generated/cmoncrawl.common.types.RoutesConfig.to_dict.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      170 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/source/generated/cmoncrawl.common.types.RoutesConfig.to_json.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      349 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/source/generated/cmoncrawl.common.types.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      295 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/source/generated/cmoncrawl.processor.extraction.filters.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      315 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/source/generated/cmoncrawl.processor.extraction.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      500 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/source/generated/cmoncrawl.processor.extraction.utils.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      239 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/source/generated/cmoncrawl.processor.pipeline.downloader.AsyncDownloader.__init__.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      225 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/source/generated/cmoncrawl.processor.pipeline.downloader.AsyncDownloader.aclose.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      222 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/source/generated/cmoncrawl.processor.pipeline.downloader.AsyncDownloader.aopen.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      231 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/source/generated/cmoncrawl.processor.pipeline.downloader.AsyncDownloader.download.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      480 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/source/generated/cmoncrawl.processor.pipeline.downloader.AsyncDownloader.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      225 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/source/generated/cmoncrawl.processor.pipeline.downloader.AsyncDownloader.unwrap.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      239 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/source/generated/cmoncrawl.processor.pipeline.downloader.DownloaderDummy.__init__.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      231 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/source/generated/cmoncrawl.processor.pipeline.downloader.DownloaderDummy.download.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      242 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/source/generated/cmoncrawl.processor.pipeline.downloader.DownloaderDummy.extract_url.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      245 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/source/generated/cmoncrawl.processor.pipeline.downloader.DownloaderDummy.extract_year.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/source/generated/cmoncrawl.processor.pipeline.downloader.DownloaderDummy.mine_metadata.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      499 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/source/generated/cmoncrawl.processor.pipeline.downloader.DownloaderDummy.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      227 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/source/generated/cmoncrawl.processor.pipeline.downloader.IDownloader.__init__.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      219 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/source/generated/cmoncrawl.processor.pipeline.downloader.IDownloader.download.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      371 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/source/generated/cmoncrawl.processor.pipeline.downloader.IDownloader.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      322 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/source/generated/cmoncrawl.processor.pipeline.downloader.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/source/generated/cmoncrawl.processor.pipeline.extractor.BaseExtractor.__init__.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      219 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/source/generated/cmoncrawl.processor.pipeline.extractor.BaseExtractor.extract.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      236 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/source/generated/cmoncrawl.processor.pipeline.extractor.BaseExtractor.extract_soup.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/source/generated/cmoncrawl.processor.pipeline.extractor.BaseExtractor.filter_raw.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      233 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/source/generated/cmoncrawl.processor.pipeline.extractor.BaseExtractor.filter_soup.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/source/generated/cmoncrawl.processor.pipeline.extractor.BaseExtractor.preprocess.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      508 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/source/generated/cmoncrawl.processor.pipeline.extractor.BaseExtractor.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      254 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/source/generated/cmoncrawl.processor.pipeline.extractor.DomainRecordExtractor.__init__.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      243 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/source/generated/cmoncrawl.processor.pipeline.extractor.DomainRecordExtractor.extract.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      260 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/source/generated/cmoncrawl.processor.pipeline.extractor.DomainRecordExtractor.extract_soup.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      254 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/source/generated/cmoncrawl.processor.pipeline.extractor.DomainRecordExtractor.filter_raw.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      257 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/source/generated/cmoncrawl.processor.pipeline.extractor.DomainRecordExtractor.filter_soup.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      252 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/source/generated/cmoncrawl.processor.pipeline.extractor.DomainRecordExtractor.preprocess.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      580 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/source/generated/cmoncrawl.processor.pipeline.extractor.DomainRecordExtractor.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/source/generated/cmoncrawl.processor.pipeline.extractor.HTMLExtractor.__init__.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      219 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/source/generated/cmoncrawl.processor.pipeline.extractor.HTMLExtractor.extract.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      236 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/source/generated/cmoncrawl.processor.pipeline.extractor.HTMLExtractor.extract_soup.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/source/generated/cmoncrawl.processor.pipeline.extractor.HTMLExtractor.filter_raw.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      233 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/source/generated/cmoncrawl.processor.pipeline.extractor.HTMLExtractor.filter_soup.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/source/generated/cmoncrawl.processor.pipeline.extractor.HTMLExtractor.preprocess.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      508 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/source/generated/cmoncrawl.processor.pipeline.extractor.HTMLExtractor.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      221 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/source/generated/cmoncrawl.processor.pipeline.extractor.IExtractor.__init__.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/source/generated/cmoncrawl.processor.pipeline.extractor.IExtractor.extract.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/source/generated/cmoncrawl.processor.pipeline.extractor.IExtractor.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      342 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/source/generated/cmoncrawl.processor.pipeline.extractor.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      239 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/source/generated/cmoncrawl.processor.pipeline.pipeline.ProcessorPipeline.__init__.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      274 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/source/generated/cmoncrawl.processor.pipeline.pipeline.ProcessorPipeline.process_domain_record.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      408 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/source/generated/cmoncrawl.processor.pipeline.pipeline.ProcessorPipeline.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      278 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/source/generated/cmoncrawl.processor.pipeline.pipeline.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      203 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/source/generated/cmoncrawl.processor.pipeline.router.IRouter.__init__.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/source/generated/cmoncrawl.processor.pipeline.router.IRouter.route.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      336 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/source/generated/cmoncrawl.processor.pipeline.router.IRouter.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      197 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/source/generated/cmoncrawl.processor.pipeline.router.Route.__init__.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      436 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/source/generated/cmoncrawl.processor.pipeline.router.Route.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      200 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/source/generated/cmoncrawl.processor.pipeline.router.Router.__init__.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      212 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/source/generated/cmoncrawl.processor.pipeline.router.Router.load_extractor.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      203 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/source/generated/cmoncrawl.processor.pipeline.router.Router.load_module.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/source/generated/cmoncrawl.processor.pipeline.router.Router.load_module_as_extractor.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      206 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/source/generated/cmoncrawl.processor.pipeline.router.Router.load_modules.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      212 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/source/generated/cmoncrawl.processor.pipeline.router.Router.register_route.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      215 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/source/generated/cmoncrawl.processor.pipeline.router.Router.register_routes.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      183 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/source/generated/cmoncrawl.processor.pipeline.router.Router.route.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      511 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/source/generated/cmoncrawl.processor.pipeline.router.Router.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      287 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/source/generated/cmoncrawl.processor.pipeline.router.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      433 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/source/generated/cmoncrawl.processor.pipeline.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      236 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/source/generated/cmoncrawl.processor.pipeline.streamer.BaseStreamerFile.__init__.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/source/generated/cmoncrawl.processor.pipeline.streamer.BaseStreamerFile.clean_up.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      247 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/source/generated/cmoncrawl.processor.pipeline.streamer.BaseStreamerFile.get_file_name.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      262 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/source/generated/cmoncrawl.processor.pipeline.streamer.BaseStreamerFile.metadata_to_string.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      502 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/source/generated/cmoncrawl.processor.pipeline.streamer.BaseStreamerFile.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      222 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/source/generated/cmoncrawl.processor.pipeline.streamer.BaseStreamerFile.stream.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      215 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/source/generated/cmoncrawl.processor.pipeline.streamer.IStreamer.__init__.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/source/generated/cmoncrawl.processor.pipeline.streamer.IStreamer.clean_up.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      379 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/source/generated/cmoncrawl.processor.pipeline.streamer.IStreamer.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      201 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/source/generated/cmoncrawl.processor.pipeline.streamer.IStreamer.stream.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      227 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/source/generated/cmoncrawl.processor.pipeline.streamer.StreamerDummy.__init__.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      221 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/source/generated/cmoncrawl.processor.pipeline.streamer.StreamerDummy.clean_up.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      403 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/source/generated/cmoncrawl.processor.pipeline.streamer.StreamerDummy.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      213 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/source/generated/cmoncrawl.processor.pipeline.streamer.StreamerDummy.stream.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      236 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/source/generated/cmoncrawl.processor.pipeline.streamer.StreamerFileHTML.__init__.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/source/generated/cmoncrawl.processor.pipeline.streamer.StreamerFileHTML.clean_up.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      247 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/source/generated/cmoncrawl.processor.pipeline.streamer.StreamerFileHTML.get_file_name.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      262 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/source/generated/cmoncrawl.processor.pipeline.streamer.StreamerFileHTML.metadata_to_string.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      502 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/source/generated/cmoncrawl.processor.pipeline.streamer.StreamerFileHTML.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      222 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/source/generated/cmoncrawl.processor.pipeline.streamer.StreamerFileHTML.stream.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      236 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/source/generated/cmoncrawl.processor.pipeline.streamer.StreamerFileJSON.__init__.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/source/generated/cmoncrawl.processor.pipeline.streamer.StreamerFileJSON.clean_up.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      247 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/source/generated/cmoncrawl.processor.pipeline.streamer.StreamerFileJSON.get_file_name.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      262 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/source/generated/cmoncrawl.processor.pipeline.streamer.StreamerFileJSON.metadata_to_string.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      502 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/source/generated/cmoncrawl.processor.pipeline.streamer.StreamerFileJSON.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      222 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/source/generated/cmoncrawl.processor.pipeline.streamer.StreamerFileJSON.stream.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      359 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/source/generated/cmoncrawl.processor.pipeline.streamer.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      266 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/source/generated/cmoncrawl.processor.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      240 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/source/generated/cmoncrawl.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      563 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/source/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 20:28:44.425697 CmonCrawl-1.0.2/docs/source/misc/
+-rw-r--r--   0 runner    (1001) docker     (123)     1668 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/source/misc/domain_record.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/source/misc/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 20:28:44.425697 CmonCrawl-1.0.2/docs/source/prog_guide/
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/source/prog_guide/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4685 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/source/prog_guide/overview.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1974 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/source/prog_guide/pip.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1235 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/docs/source/usage.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 20:28:44.229688 CmonCrawl-1.0.2/examples/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 20:28:44.425697 CmonCrawl-1.0.2/examples/extractor_tutorial/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 20:28:44.425697 CmonCrawl-1.0.2/examples/extractor_tutorial/Extractors/
+-rw-r--r--   0 runner    (1001) docker     (123)     1437 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/examples/extractor_tutorial/Extractors/bbc_extractor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      181 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/examples/extractor_tutorial/config.json
+-rw-r--r--   0 runner    (1001) docker     (123)      887 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/pyrightconfig.json
+-rw-r--r--   0 runner    (1001) docker     (123)      446 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-22 20:28:44.433698 CmonCrawl-1.0.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 20:28:44.429697 CmonCrawl-1.0.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     7170 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/tests/aggregator_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3003 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/tests/end_to_end_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6378 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/tests/processor_tests.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 20:28:44.429697 CmonCrawl-1.0.2/tests/test_extract/
+-rw-r--r--   0 runner    (1001) docker     (123)      272 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/tests/test_extract/cfg.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 20:28:44.429697 CmonCrawl-1.0.2/tests/test_extract/extractors/
+-rw-r--r--   0 runner    (1001) docker     (123)      495 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/tests/test_extract/extractors/test_extract.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 20:28:44.429697 CmonCrawl-1.0.2/tests/test_extract/files/
+-rw-r--r--   0 runner    (1001) docker     (123)   828135 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/tests/test_extract/files/file.html
+-rw-r--r--   0 runner    (1001) docker     (123)  1743032 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/tests/test_extract/files/file.jsonl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 20:28:44.433698 CmonCrawl-1.0.2/tests/test_routes/
+-rw-r--r--   0 runner    (1001) docker     (123)      401 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/tests/test_routes/a.py
+-rw-r--r--   0 runner    (1001) docker     (123)      400 2023-05-22 20:28:29.000000 CmonCrawl-1.0.2/tests/test_routes/b.py
```

### Comparing `CmonCrawl-1.0.1/.gitignore` & `CmonCrawl-1.0.2/.gitignore`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.0.1/.vscode/launch.json` & `CmonCrawl-1.0.2/.vscode/launch.json`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.0.1/CmonCrawl.egg-info/PKG-INFO` & `CmonCrawl-1.0.2/CmonCrawl.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CmonCrawl
-Version: 1.0.1
+Version: 1.0.2
 License: MIT License
         
         Copyright (c) [2023] [Hynek Kydlíček]
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
@@ -132,10 +132,10 @@
 ```
 
 Note that you can use the --n_proc option to specify the number of processes to use for the extraction. Multiprocessing is done on file level, so if you have just one file it will not be used.
 
 
 ### Advanced usage
 The whole project was written with modularity in mind. That means that you
-can adjust the framework to your needs. To know more check  see [https://hynky1999.github.io/CmonCrawl/build/html/index.html](documentation)
+can adjust the framework to your needs. To know more check  see [https://hynky1999.github.io/CmonCrawl/build/html/usage.html](documentation)
 
 Instead of first getting the records and then extracting them, you can do both in a distributed setting. For more info look at [CZE-NEC](https://github.com/hynky1999/Czech-News-Classification-dataset) project.
```

### Comparing `CmonCrawl-1.0.1/CmonCrawl.egg-info/SOURCES.txt` & `CmonCrawl-1.0.2/CmonCrawl.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -1,30 +1,31 @@
-.flake8
 .gitignore
 .pre-commit-config.yaml
 LICENSE
 README.md
 pyproject.toml
+pyrightconfig.json
 requirements.txt
-.github/workflows/test_and_push.yml
+.github/workflows/release.yml
+.github/workflows/test_and_types.yml
 .vscode/launch.json
 .vscode/settings.json
 CmonCrawl.egg-info/PKG-INFO
 CmonCrawl.egg-info/SOURCES.txt
 CmonCrawl.egg-info/dependency_links.txt
 CmonCrawl.egg-info/entry_points.txt
 CmonCrawl.egg-info/requires.txt
 CmonCrawl.egg-info/top_level.txt
 cmoncrawl/__init__.py
 cmoncrawl/aggregator/__init__.py
 cmoncrawl/aggregator/index_query.py
 cmoncrawl/aggregator/.vscode/settings.json
 cmoncrawl/aggregator/utils/__init__.py
 cmoncrawl/aggregator/utils/helpers.py
-cmoncrawl/aggregator/utils/ndjson_decoder.py
+cmoncrawl/aggregator/utils/ndjson.py
 cmoncrawl/common/__init__.py
 cmoncrawl/common/loggers.py
 cmoncrawl/common/types.py
 cmoncrawl/integrations/commands.py
 cmoncrawl/integrations/download.py
 cmoncrawl/integrations/extract.py
 cmoncrawl/middleware/stompware.py
```

### Comparing `CmonCrawl-1.0.1/LICENSE` & `CmonCrawl-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.0.1/PKG-INFO` & `CmonCrawl-1.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CmonCrawl
-Version: 1.0.1
+Version: 1.0.2
 License: MIT License
         
         Copyright (c) [2023] [Hynek Kydlíček]
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
@@ -132,10 +132,10 @@
 ```
 
 Note that you can use the --n_proc option to specify the number of processes to use for the extraction. Multiprocessing is done on file level, so if you have just one file it will not be used.
 
 
 ### Advanced usage
 The whole project was written with modularity in mind. That means that you
-can adjust the framework to your needs. To know more check  see [https://hynky1999.github.io/CmonCrawl/build/html/index.html](documentation)
+can adjust the framework to your needs. To know more check  see [https://hynky1999.github.io/CmonCrawl/build/html/usage.html](documentation)
 
 Instead of first getting the records and then extracting them, you can do both in a distributed setting. For more info look at [CZE-NEC](https://github.com/hynky1999/Czech-News-Classification-dataset) project.
```

### Comparing `CmonCrawl-1.0.1/README.md` & `CmonCrawl-1.0.2/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -98,10 +98,10 @@
 ```
 
 Note that you can use the --n_proc option to specify the number of processes to use for the extraction. Multiprocessing is done on file level, so if you have just one file it will not be used.
 
 
 ### Advanced usage
 The whole project was written with modularity in mind. That means that you
-can adjust the framework to your needs. To know more check  see [https://hynky1999.github.io/CmonCrawl/build/html/index.html](documentation)
+can adjust the framework to your needs. To know more check  see [https://hynky1999.github.io/CmonCrawl/build/html/usage.html](documentation)
 
 Instead of first getting the records and then extracting them, you can do both in a distributed setting. For more info look at [CZE-NEC](https://github.com/hynky1999/Czech-News-Classification-dataset) project.
```

### Comparing `CmonCrawl-1.0.1/cmoncrawl/aggregator/index_query.py` & `CmonCrawl-1.0.2/cmoncrawl/aggregator/index_query.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,18 +1,21 @@
 from __future__ import annotations
 from collections import deque
 from datetime import datetime
 import re
 
-from cmoncrawl.aggregator.utils.ndjson_decoder import Decoder
+from cmoncrawl.aggregator.utils import ndjson
+import json
 from types import TracebackType
 from typing import (
     Any,
     AsyncIterable,
     AsyncIterator,
+    Awaitable,
+    Callable,
     Deque,
     List,
     Dict,
     Set,
     Tuple,
     Type,
 )
@@ -20,15 +23,21 @@
 from cmoncrawl.common.types import (
     DomainRecord,
     RetrieveResponse,
     DomainCrawl,
     MatchType,
 )
 
-from aiohttp import ClientError, ClientSession, ContentTypeError, ServerConnectionError
+from aiohttp import (
+    ClientError,
+    ClientResponse,
+    ClientSession,
+    ContentTypeError,
+    ServerConnectionError,
+)
 import asyncio
 import random
 
 ALLOWED_ERR_FOR_RETRIES = [500, 502, 503, 504]
 
 
 class IndexAggregator(AsyncIterable[DomainRecord]):
@@ -152,43 +161,52 @@
                 return False
 
             return True
 
         status = 0
         content = None
         reason: str | None = None
+        decode: Callable[[ClientResponse], Awaitable[Any]]
+
+        if content_type == "text/x-ndjson":
+            decode = lambda response: response.json(
+                content_type=content_type, loads=ndjson.Decoder().decode
+            )
+        elif content_type == "application/json":
+            decode = lambda response: response.json(content_type=content_type)
+        else:
+            raise ValueError(f"Unknown content type: {content_type}")
 
         for retry in range(max_retry):
             try:
                 all_purpose_logger.debug(
                     f"Sending request to {cdx_server} with params: {params}, retry: {retry + 1}/{max_retry}"
                 )
                 async with client.get(cdx_server, params=params) as response:
                     status = response.status
                     if not response.ok:
-                        reason = response.reason if response.reason else "Unknown"
+                        reason = str(response.reason) if response.reason else "Unknown"  # type: ignore
                         if not should_retry(retry, reason, status, **args):
                             break
                     else:
-                        content = await response.json(
-                            content_type=content_type, loads=Decoder().decode
-                        )
+                        content = await decode(response)
                         all_purpose_logger.info(
                             f"Successfully retrieved page of {domain} from {cdx_server} add_info: {args}"
                         )
                         break
 
             except (
                 ClientError,
                 TimeoutError,
                 ServerConnectionError,
                 ContentTypeError,
             ) as e:
                 reason = f"{type(e)} {str(e)}"
-                if not should_retry(retry, reason, 500, **args):
+                status = 500
+                if not should_retry(retry, reason, status, **args):
                     break
 
             await asyncio.sleep(random.randint(0, (retry + 1) * sleep_step))
         return RetrieveResponse(status, content, reason)
 
     @staticmethod
     async def get_number_of_pages(
@@ -276,23 +294,30 @@
         return reponse
 
     @staticmethod
     async def get_all_CC_indexes(client: ClientSession, cdx_server: str) -> List[str]:
         """
         Get all CC index servers from a given CDX server
         """
-        for _ in range(3):
-            async with client.get(cdx_server) as response:
-                r_json = await response.json(content_type="application/json")
-                CC_servers = [js["cdx-api"] for js in r_json]
-                return CC_servers
-        all_purpose_logger.error(
-            f"Failed to get CC servers from {cdx_server} after 3 attempts"
+        response = await IndexAggregator.__retrieve(
+            client=client,
+            cdx_server=cdx_server,
+            domain=cdx_server,
+            params={},
+            content_type="application/json",
+            max_retry=10,
+            sleep_step=1,
         )
-        return []
+        if response.content is None:
+            all_purpose_logger.error(
+                f"Failed to get CC servers from {cdx_server} after 3 attempts"
+            )
+            return []
+        CC_servers = [js["cdx-api"] for js in response.content]
+        return CC_servers
 
     class IndexAggregatorIterator(AsyncIterator[DomainRecord]):
         def __init__(
             self,
             client: ClientSession,
             domains: List[str],
             CC_files: List[str],
@@ -305,15 +330,15 @@
             # time sleeping lineary increases with failed attempts
             sleep_step: int,
         ):
             self.__client = client
             self.__opt_prefetch_size = prefetch_size
             self.__domain_records: Deque[DomainRecord] = deque()
             self.prefetch_queue: Set[
-                asyncio.Task[Tuple[RetrieveResponse, DomainCrawl, int]]
+                asyncio.Task[Tuple[RetrieveResponse, DomainCrawl]]
             ] = set()
             self.__since = since
             self.__to = to
             self.__limit = limit
             self.__max_retry = max_retry
             self.__total = 0
             self.__sleep_step = sleep_step
@@ -355,15 +380,15 @@
                     # Failed to retrieve it
                     return await self.__prefetch_next_crawl()
                 pages = retr.content[0]
 
                 for i in range(pages):
                     dc = DomainCrawl(next_crawl.domain, next_crawl.cdx_server, i)
                     self.prefetch_queue.add(
-                        asyncio.create_task(self.__fetch_next_dc(dc, 0))
+                        asyncio.create_task(self.__fetch_next_dc(dc))
                     )
                 return pages
             return 0
 
         async def __await_next_prefetch(self):
             """
             Gets the next index retry
@@ -380,38 +405,21 @@
                 await self.__prefetch_next_crawl()
 
             while len(self.prefetch_queue) > 0 and len(self.__domain_records) == 0:
                 done, self.prefetch_queue = await asyncio.wait(
                     self.prefetch_queue, return_when="FIRST_COMPLETED"
                 )
                 for task in done:
-                    response, dc, retry = task.result()
+                    response, dc = task.result()
 
                     if response.content is not None:
                         self.__domain_records.extend(response.content)
                         all_purpose_logger.info(
                             f"Found {len(response.content)} records for {dc.domain} of {dc.cdx_server}"
                         )
-                    else:
-                        _max_retry = (
-                            self.__max_retry
-                            if response.status in ALLOWED_ERR_FOR_RETRIES
-                            else retry
-                        )
-                        if (
-                            retry < _max_retry
-                            and response.status in ALLOWED_ERR_FOR_RETRIES
-                        ):
-                            self.prefetch_queue.add(
-                                asyncio.create_task(self.__fetch_next_dc(dc, retry + 1))
-                            )
-                        else:
-                            all_purpose_logger.error(
-                                f"Failed to fetch {dc.domain} of {dc.cdx_server} with status {response.status}"
-                            )
 
             # Nothing more to prefetch
 
         async def __anext__(self) -> DomainRecord:
             # Stop if we fetched everything or reached limit
             if self.__limit is not None and self.__total >= self.__limit:
                 self.clean()
@@ -434,30 +442,28 @@
             return result
 
         # Helper functions
         def clean(self):
             for task in self.prefetch_queue:
                 task.cancel()
 
-        async def __fetch_next_dc(self, dc: DomainCrawl, retry: int):
-            await asyncio.sleep(random.randint(0, self.__sleep_step * (retry)))
+        async def __fetch_next_dc(self, dc: DomainCrawl):
             return (
                 await IndexAggregator.get_captured_responses(
                     self.__client,
                     dc.cdx_server,
                     dc.domain,
                     match_type=self.__match_type,
                     page=dc.page,
                     since=self.__since,
                     to=self.__to,
-                    max_retry=1,
+                    max_retry=self.__max_retry,
                     sleep_step=self.__sleep_step,
                 ),
                 dc,
-                retry,
             )
 
 
 def to_timestamp_format(date: datetime):
     return date.strftime("%Y%m%d%H%M%S")
```

### Comparing `CmonCrawl-1.0.1/cmoncrawl/aggregator/utils/helpers.py` & `CmonCrawl-1.0.2/cmoncrawl/aggregator/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.0.1/cmoncrawl/common/loggers.py` & `CmonCrawl-1.0.2/cmoncrawl/common/loggers.py`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.0.1/cmoncrawl/common/types.py` & `CmonCrawl-1.0.2/cmoncrawl/common/types.py`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.0.1/cmoncrawl/integrations/commands.py` & `CmonCrawl-1.0.2/cmoncrawl/integrations/commands.py`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.0.1/cmoncrawl/integrations/download.py` & `CmonCrawl-1.0.2/cmoncrawl/integrations/download.py`

 * *Files 10% similar despite different names*

```diff
@@ -30,17 +30,25 @@
     )
     record_parser.add_argument(
         "--max_crawls_per_file",
         type=int,
         default=500_000,
         help="Max number of domain records per file output",
     )
-    subparser.add_parser(
+    html_parser = subparser.add_parser(
         DownloadOutputFormat.HTML.value, help="Download HTML files from Common Crawl"
     )
+
+    html_parser.add_argument(
+        "--encoding",
+        type=str,
+        default=None,
+        help="Force usage of specified encoding is possible",
+    )
+
     return subparser
 
 
 def add_args(subparser: Any):
     parser = subparser.add_parser("download", help="Download data from Common Crawl")
     parser.add_argument("url", type=str, help="URL to query")
     parser.add_argument("output", type=Path, help="Path to output directory")
@@ -101,25 +109,26 @@
         default=True,
         help="Filter out non 200 status code",
     )
     parser.set_defaults(func=run_download)
 
 
 def url_download_prepare_router(
-    output_format: DownloadOutputFormat, filter_non_200: bool
+    output_format: DownloadOutputFormat, filter_non_200: bool, encoding: str | None
 ):
     router = Router()
     match output_format:
         case DownloadOutputFormat.RECORD:
             router.load_extractor(
                 "dummy_extractor", DomainRecordExtractor(filter_non_ok=filter_non_200)
             )
         case DownloadOutputFormat.HTML:
             router.load_extractor(
-                "dummy_extractor", HTMLExtractor(filter_non_ok=filter_non_200)
+                "dummy_extractor",
+                HTMLExtractor(filter_non_ok=filter_non_200, encoding=encoding),
             )
     router.register_route("dummy_extractor", [r".*"])
     return router
 
 
 def url_download_prepare_streamer(
     output_format: DownloadOutputFormat,
@@ -136,31 +145,32 @@
             )
         case DownloadOutputFormat.HTML:
             return StreamerFileHTML(root=output, max_directory_size=max_direrctory_size)
 
 
 async def url_download(
     url: str,
-    match_type: str | None,
+    match_type: MatchType | None,
     output: Path,
     cc_server: List[str] | None,
     since: datetime,
     to: datetime,
     limit: int,
     max_retry: int,
     sleep_step: int,
     mode: DownloadOutputFormat,
     max_crawls_per_file: int,
     max_directory_size: int,
     filter_non_200: bool,
+    encoding: str | None,
 ):
     outstreamer = url_download_prepare_streamer(
         mode, output, max_directory_size, max_crawls_per_file
     )
-    router = url_download_prepare_router(mode, filter_non_200)
+    router = url_download_prepare_router(mode, filter_non_200, encoding)
     pipeline = ProcessorPipeline(
         router, AsyncDownloader(max_retry=max_retry), outstreamer
     )
 
     index_agg = IndexAggregator(
         cc_servers=cc_server or [],
         domains=[url],
@@ -174,22 +184,25 @@
     await query_and_extract(index_agg, pipeline)
 
 
 def run_download(args: argparse.Namespace):
     mode = DownloadOutputFormat(args.mode)
     return asyncio.run(
         url_download(
-            args.url,
-            args.match_type,
-            args.output,
-            args.cc_server,
-            args.since,
-            args.to,
-            args.limit,
-            args.max_retry,
-            args.sleep_step,
-            mode,
-            args.max_crawls_per_file if mode == DownloadOutputFormat.RECORD else 1,
-            args.max_directory_size,
-            args.filter_non_200,
+            url=args.url,
+            match_type=args.match_type,
+            output=args.output,
+            cc_server=args.cc_server,
+            since=args.since,
+            to=args.to,
+            limit=args.limit,
+            max_retry=args.max_retry,
+            sleep_step=args.sleep_step,
+            mode=mode,
+            max_crawls_per_file=args.max_crawls_per_file
+            if mode == DownloadOutputFormat.RECORD
+            else 1,
+            max_directory_size=args.max_directory_size,
+            filter_non_200=args.filter_non_200,
+            encoding=args.encoding if mode == DownloadOutputFormat.HTML else None,
         )
     )
```

### Comparing `CmonCrawl-1.0.1/cmoncrawl/integrations/extract.py` & `CmonCrawl-1.0.2/cmoncrawl/integrations/extract.py`

 * *Files 3% similar despite different names*

```diff
@@ -115,35 +115,35 @@
 def get_domain_records_json(
     file_path: Path,
 ) -> List[Tuple[DomainRecord, Dict[str, Any]]]:
     records: List[Tuple[DomainRecord, Dict[str, Any]]] = []
     with open(file_path, "r") as f:
         for line in tqdm(f):
             js = json.loads(line)
-            domain_record: DomainRecord = DomainRecord.schema().load(
+            domain_record: DomainRecord = DomainRecord.schema().load(  # type: ignore
                 js["domain_record"]
             )
             additional_info = js.get("additional_info", {})
             if not isinstance(additional_info, dict):
                 additional_info = {}
-            records.append((domain_record, additional_info))
+            records.append((domain_record, additional_info))  # type: ignore
     return records
 
 
 def get_domain_records_html(
     url: str | None, date: datetime | None
 ) -> List[Tuple[DomainRecord, Dict[str, Any]]]:
     # Just return dummy as correct crawl will be loaded from dummy downloader
     return [(DomainRecord("", url=url, offset=0, length=0, timestamp=date), {})]
 
 
 def load_config(config_path: Path) -> ExtractConfig:
     with open(config_path, "r") as f:
         config = json.load(f)
-    return ExtractConfig.schema().load(config)
+    return ExtractConfig.schema().load(config)  # type: ignore
 
 
 def create_router(config: ExtractConfig) -> Router:
     router = Router()
     router.load_modules(config.extractors_path)
     router.register_routes(config.routes)
     return router
```

### Comparing `CmonCrawl-1.0.1/cmoncrawl/middleware/stompware.py` & `CmonCrawl-1.0.2/cmoncrawl/middleware/stompware.py`

 * *Files 6% similar despite different names*

```diff
@@ -67,15 +67,15 @@
         self.heartbeat = heartbeat
 
     def _init_connection(self):
         conn = Connection(
             [(self.queue_host, self.queue_port)],
             heartbeats=(self.heartbeat, self.heartbeat),
         )
-        conn.connect(login="producer", passcode="producer", wait=True)
+        conn.connect(login="producer", passcode="producer", wait=True)  # type: ignore
         all_purpose_logger.info(f"Connected to queue")
         return conn
 
     async def aggregate(self, filter_duplicates: bool = True):
         """
         Aggregates the results of the index aggregator and sends them to the queue.
         If `filter_duplicates` is True, it will use the `DUPL_ID_HEADER` header,
@@ -94,18 +94,18 @@
             async for domain_record in aggregator:
                 try:
                     while not conn.is_connected():
                         conn = self._init_connection()
 
                     json_str = json.dumps(domain_record.__dict__, default=str)
                     headers = {}
-                    id = unify_url_id(domain_record.url)
+                    id = unify_url_id(domain_record.url or "")
                     if filter_duplicates:
                         headers[DUPL_ID_HEADER] = id
-                    conn.send(
+                    conn.send(  # type: ignore
                         f"queue.{self.url}",
                         json_str,
                         headers=headers,
                     )
                     all_purpose_logger.debug(
                         f"Sent url: {domain_record.url} with id: {id}"
                     )
@@ -115,18 +115,18 @@
                     continue
 
                 except Exception as e:
                     all_purpose_logger.error(e, exc_info=True)
                     break
 
         all_purpose_logger.info(f"Sent {i} messages")
-        conn.send(
+        conn.send(  # type: ignore
             f"topic.poisson_pill.{self.url}", "", headers={"type": "poisson_pill"}
         )
-        conn.disconnect()
+        conn.disconnect()  # type: ignore
 
 
 class ArtemisProcessor:
     """
     Processor that listens to a queues and processes the messages using a pipeline.
     When it receives a message with type enough `poisson_pill` messages, it will
     stop listening if it doesn't receive any messages for `timeout` minutes.
@@ -171,42 +171,42 @@
             listener_stats: ListnerStats,
         ):
             self.messages = messages
             self.pills = 0
             self.listener_stats = listener_stats
 
         def on_message(self, frame: Frame):
-            if frame.headers.get("type") == "poisson_pill":
+            if frame.headers.get("type") == "poisson_pill":  # type: ignore
                 self.pills += 1
             else:
-                msg_json = json.loads(frame.body)
+                msg_json = json.loads(frame.body)  # type: ignore
                 try:
                     msg_json["timestamp"] = datetime.fromisoformat(
                         msg_json.get("timestamp")
                     )
                     domain_record = DomainRecord(**msg_json)
-                    self.messages.put_nowait(Message(domain_record, frame.headers))
+                    self.messages.put_nowait(Message(domain_record, frame.headers))  # type: ignore
                     self.listener_stats.messages += 1
                     self.listener_stats.last_message_time = datetime.now()
                 except ValueError:
                     pass
 
     def _init_connection(self, addresses: List[str]):
         conn = Connection(
             [(self.queue_host, self.queue_port)],
             reconnect_attempts_max=-1,
             heartbeats=(self.heartbeat, self.heartbeat),
         )
-        conn.connect(login="consumer", passcode="consumer", wait=True)
+        conn.connect(login="consumer", passcode="consumer", wait=True)  # type: ignore
         for address in addresses:
-            conn.subscribe(address, id=address, ack="client-individual")
-        conn.subscribe("topic.poisson_pill.#", id="poisson_pill", ack="auto")
+            conn.subscribe(address, id=address, ack="client-individual")  # type: ignore
+        conn.subscribe("topic.poisson_pill.#", id="poisson_pill", ack="auto")  # type: ignore
         listener_stats = ListnerStats()
         listener = self.Listener(asyncio.Queue(0), listener_stats)
-        conn.set_listener("", listener)
+        conn.set_listener("", listener)  # type: ignore
         all_purpose_logger.info("Connected to queue")
         return conn, listener
 
     async def _call_pipeline_with_ack(
         self,
         pipeline: ProcessorPipeline,
         msg: Message,
@@ -240,15 +240,15 @@
                 all_purpose_logger.error(e, exc_info=True)
                 await asyncio.sleep(5)
                 continue
         all_purpose_logger.debug("Connecting to queue")
         extracted_num = 0
         try:
             if hasattr(self.pipeline.downloader, "__aenter__"):
-                await self.pipeline.downloader.__aenter__()
+                await self.pipeline.downloader.__aenter__()  # type: ignore
 
             while True:
                 if (
                     listener.messages.empty()
                     and (
                         self.pills_to_die is None or listener.pills >= self.pills_to_die
                     )
@@ -314,13 +314,13 @@
                 else:
                     all_purpose_logger.info(f"Failed to extract {message.dr.url}")
         except Exception as e:
             pass
 
         finally:
             if hasattr(self.pipeline.downloader, "__aexit__"):
-                await self.pipeline.downloader.__aexit__(None, None, None)
+                await self.pipeline.downloader.__aexit__(None, None, None)  # type: ignore
 
         all_purpose_logger.info(
             f"Extracted {extracted_num}/{listener.listener_stats.messages} articles"
         )
-        conn.disconnect()
+        conn.disconnect()  # type: ignore
```

### Comparing `CmonCrawl-1.0.1/cmoncrawl/middleware/synchronized.py` & `CmonCrawl-1.0.2/cmoncrawl/middleware/synchronized.py`

 * *Files 6% similar despite different names*

```diff
@@ -25,15 +25,15 @@
             the rest will be skipped. Defaults to False.
 
     """
     processed_urls: Set[str] = set()
     total_extracted: int = 0
 
     if hasattr(pipeline.downloader, "__aenter__"):
-        await pipeline.downloader.__aenter__()
+        await pipeline.downloader.__aenter__()  # type: ignore
     try:
         async with index_agg:
             async for domain_record in index_agg:
                 url = domain_record.url or ""
                 if filter_non_unique_url and unify_url_id(url) in processed_urls:
                     continue
                 try:
@@ -46,15 +46,15 @@
                 except Exception as e:
                     all_purpose_logger.error(
                         f"Failed to process {domain_record.url} with {e}"
                     )
 
     finally:
         if hasattr(pipeline.downloader, "__aexit__"):
-            await pipeline.downloader.__aexit__(None, None, None)
+            await pipeline.downloader.__aexit__(None, None, None)  # type: ignore
     all_purpose_logger.info(f"Extracted {total_extracted} urls")
     return processed_urls
 
 
 async def _extract_task(
     domain_record: DomainRecord,
     additional_info: Dict[str, Any],
@@ -89,15 +89,15 @@
             Defaults to 20.
 
     """
     domain_records_iterator = iter(tqdm(records))
     domains_exausted = False
     total_extracted: int = 0
     if hasattr(pipeline.downloader, "__aenter__"):
-        await pipeline.downloader.__aenter__()
+        await pipeline.downloader.__aenter__()  # type: ignore
     try:
         queue: Set[asyncio.Task[List[Path]]] = set()
         while not domains_exausted or len(queue) > 0:
             # Put into queue till possible
             while len(queue) < concurrent_length and not domains_exausted:
                 next_record = next(domain_records_iterator, None)
                 if next_record is None:
@@ -123,9 +123,9 @@
                     all_purpose_logger.error(f"Failed to process {task}")
                     pass
     except Exception as e:
         all_purpose_logger.error(e, exc_info=True)
 
     finally:
         if hasattr(pipeline.downloader, "__aexit__"):
-            await pipeline.downloader.__aexit__(None, None, None)
+            await pipeline.downloader.__aexit__(None, None, None)  # type: ignore
     all_purpose_logger.info(f"Extracted {total_extracted} urls")
```

### Comparing `CmonCrawl-1.0.1/cmoncrawl/processor/extraction/filters.py` & `CmonCrawl-1.0.2/cmoncrawl/processor/extraction/filters.py`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.0.1/cmoncrawl/processor/extraction/utils.py` & `CmonCrawl-1.0.2/cmoncrawl/processor/extraction/utils.py`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.0.1/cmoncrawl/processor/pipeline/downloader.py` & `CmonCrawl-1.0.2/cmoncrawl/processor/pipeline/downloader.py`

 * *Files 1% similar despite different names*

```diff
@@ -112,15 +112,15 @@
         ret: List[Tuple[str, PipeMetadata]] = []
         return ret
 
     def unwrap(
         self, response: bytes, domain_record: DomainRecord
     ) -> List[Tuple[str, PipeMetadata]]:
         ariter = ArchiveIterator(
-            io.BytesIO(response), check_digests="raise", arc2warc=True
+            io.BytesIO(response), check_digests="raise", arc2warc=True  # type: ignore wrong typing in package
         )
         encoding = self.encoding
         warcs: List[Tuple[str, PipeMetadata]] = [
             (
                 warc.content_stream().read().decode(encoding),
                 PipeMetadata(
                     domain_record,
```

### Comparing `CmonCrawl-1.0.1/cmoncrawl/processor/pipeline/extractor.py` & `CmonCrawl-1.0.2/cmoncrawl/processor/pipeline/extractor.py`

 * *Files 17% similar despite different names*

```diff
@@ -27,19 +27,20 @@
 
 class BaseExtractor(IExtractor, ABC):
     """
     Base class for all soup extractors
 
     Args:
         encoding (str, optional): Default encoding to be used. Defaults to None.
-
+        raise_on_encoding (bool, optional): If True, the extractor will raise ValueException if it fails to decode the response. Defaults to False.
     """
 
-    def __init__(self, encoding: str | None = None):
+    def __init__(self, encoding: str | None = None, raise_on_encoding: bool = False):
         self.encoding = encoding
+        self.raise_on_encoding = raise_on_encoding
 
     def filter_raw(self, response: str, metadata: PipeMetadata) -> bool:
         # If raw fails bs4 will not be used -> speed
         return True
 
     def filter_soup(self, soup: BeautifulSoup, metadata: PipeMetadata) -> bool:
         # slow but has more info
@@ -66,56 +67,66 @@
 
     @abstractmethod
     def extract_soup(
         self, soup: BeautifulSoup, metadata: PipeMetadata
     ) -> Dict[str, Any] | None:
         raise NotImplementedError()
 
-    def preprocess(self, response: str, metadata: PipeMetadata) -> str:
-        linux = response.replace("\r\n", "\n")
-        # Sorted set pythonic way
+    def encode(self, response: str, metadata: PipeMetadata):
+        # Sorted set pythonic way, we assume that dict is sortd
         encodings: Dict[str, int] = {}
         if self.encoding is not None:
             encodings[self.encoding] = 1
         if metadata.domain_record.encoding is not None:
             encodings[metadata.domain_record.encoding] = 1
+        # GET from http header
         http_split = metadata.http_header.get("Content-Type", "").split("charset=")
         if len(http_split) > 1 and http_split[1] != "":
             encodings[http_split[-1]] = 1
 
         # Fallbacks
         encodings["utf-8"] = 1
-
-        encoded = linux.encode(metadata.encoding)
+        encoded = response.encode(metadata.encoding)
+        decoded = None
         for encoding in encodings:
             try:
                 decoded = encoded.decode(encoding)
                 metadata.encoding = encoding
                 break
             except ValueError:
                 metadata_logger.warn(
                     f"Failed to decode with {encoding}",
                     extra={"domain_record": metadata.domain_record},
                 )
-        else:
-            raise ValueError("Failed to decode")
+
+        if decoded is None:
+            if self.raise_on_encoding:
+                raise ValueError("Failed to decode")
+            else:
+                decoded = response
 
         return decoded
 
+    def preprocess(self, response: str, metadata: PipeMetadata) -> str:
+        response = response.replace("\r\n", "\n")
+        response = self.encode(response, metadata)
+        return response
+
 
 class HTMLExtractor(BaseExtractor):
     """
     Dummy Extractor which simply extracts the html
 
     Args:
         filter_non_ok (bool, optional): If True, only 200 status codes will be extracted. Defaults to True.
+        encoding (str, optional): Default encoding to be used. Defaults to None. If set, the extractor will raise ValueException if it fails to decode the response.
     """
 
-    def __init__(self, filter_non_ok: bool = True):
-        super().__init__()
+    def __init__(self, filter_non_ok: bool = True, encoding: str | None = None):
+        super().__init__(encoding=encoding, raise_on_encoding=encoding is not None)
         self.filter_non_ok = filter_non_ok
 
     def extract_soup(self, soup: BeautifulSoup, metadata: PipeMetadata):
         metadata.name = (
             metadata.domain_record.url.replace("/", "_")[:100]
             if metadata.domain_record.url is not None
             else "unknown"
@@ -142,25 +153,26 @@
     Dummy Extractor which simply extracts the domain record
 
     Args:
         filter_non_ok (bool, optional): If True, only 200 status codes will be extracted. Defaults to True.
     """
 
     def __init__(self, filter_non_ok: bool = True):
+        # We only extract records, don't try to encode
         super().__init__()
         self.filter_non_ok = filter_non_ok
 
     def extract_soup(self, soup: BeautifulSoup, metadata: PipeMetadata):
         metadata.name = (
             metadata.domain_record.url.replace("/", "_")[:100]
             if metadata.domain_record.url is not None
             else "unknown"
         )
         result_dict: Dict[str, Any] = {
-            "domain_record": metadata.domain_record.to_dict()
+            "domain_record": metadata.domain_record.to_dict()  # type: ignore Wrong type
         }
 
         return result_dict
 
     def filter_raw(self, response: str, metadata: PipeMetadata):
         if (
             self.filter_non_ok
```

### Comparing `CmonCrawl-1.0.1/cmoncrawl/processor/pipeline/pipeline.py` & `CmonCrawl-1.0.2/cmoncrawl/processor/pipeline/pipeline.py`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.0.1/cmoncrawl/processor/pipeline/router.py` & `CmonCrawl-1.0.2/cmoncrawl/processor/pipeline/router.py`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.0.1/cmoncrawl/processor/pipeline/streamer.py` & `CmonCrawl-1.0.2/cmoncrawl/processor/pipeline/streamer.py`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.0.1/docs/Makefile` & `CmonCrawl-1.0.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.0.1/docs/build/doctrees/api.doctree` & `CmonCrawl-1.0.2/docs/build/doctrees/api.doctree`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.0.1/docs/build/doctrees/cli/cli.doctree` & `CmonCrawl-1.0.2/docs/build/doctrees/cli/cli.doctree`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.0.1/docs/build/doctrees/cli/download.doctree` & `CmonCrawl-1.0.2/docs/build/doctrees/cli/download.doctree`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.0.1/docs/build/doctrees/cli/extract.doctree` & `CmonCrawl-1.0.2/docs/build/doctrees/cli/extract.doctree`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.0.1/docs/build/doctrees/cli/index.doctree` & `CmonCrawl-1.0.2/docs/build/doctrees/cli/index.doctree`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.0.1/docs/build/doctrees/environment.pickle` & `CmonCrawl-1.0.2/docs/build/doctrees/environment.pickle`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.0.1/docs/build/doctrees/extraction/config_file.doctree` & `CmonCrawl-1.0.2/docs/build/doctrees/extraction/config_file.doctree`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.0.1/docs/build/doctrees/extraction/creating_extractor.doctree` & `CmonCrawl-1.0.2/docs/build/doctrees/extraction/creating_extractor.doctree`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.0.1/docs/build/doctrees/extraction/index.doctree` & `CmonCrawl-1.0.2/docs/build/doctrees/extraction/index.doctree`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.0.1/docs/build/doctrees/extraction/utils.doctree` & `CmonCrawl-1.0.2/docs/build/doctrees/extraction/utils.doctree`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.0.1/docs/build/doctrees/generated/cmoncrawl.aggregator.doctree` & `CmonCrawl-1.0.2/docs/build/doctrees/generated/cmoncrawl.aggregator.doctree`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.0.1/docs/build/doctrees/generated/cmoncrawl.aggregator.index_query.IndexAggregator.__init__.doctree` & `CmonCrawl-1.0.2/docs/build/doctrees/generated/cmoncrawl.aggregator.index_query.IndexAggregator.__init__.doctree`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.0.1/docs/build/doctrees/generated/cmoncrawl.aggregator.index_query.IndexAggregator.aclose.doctree` & `CmonCrawl-1.0.2/docs/build/doctrees/generated/cmoncrawl.aggregator.index_query.IndexAggregator.aclose.doctree`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.0.1/docs/build/doctrees/generated/cmoncrawl.aggregator.index_query.IndexAggregator.aopen.doctree` & `CmonCrawl-1.0.2/docs/build/doctrees/generated/cmoncrawl.aggregator.index_query.IndexAggregator.aopen.doctree`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.0.1/docs/build/doctrees/generated/cmoncrawl.aggregator.index_query.IndexAggregator.doctree` & `CmonCrawl-1.0.2/docs/build/doctrees/generated/cmoncrawl.aggregator.index_query.IndexAggregator.doctree`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.0.1/docs/build/doctrees/generated/cmoncrawl.aggregator.index_query.IndexAggregator.get_all_CC_indexes.doctree` & `CmonCrawl-1.0.2/docs/build/doctrees/generated/cmoncrawl.aggregator.index_query.IndexAggregator.get_all_CC_indexes.doctree`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.0.1/docs/build/doctrees/generated/cmoncrawl.aggregator.index_query.IndexAggregator.get_captured_responses.doctree` & `CmonCrawl-1.0.2/docs/build/doctrees/generated/cmoncrawl.aggregator.index_query.IndexAggregator.get_captured_responses.doctree`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.0.1/docs/build/doctrees/generated/cmoncrawl.aggregator.index_query.IndexAggregator.get_number_of_pages.doctree` & `CmonCrawl-1.0.2/docs/build/doctrees/generated/cmoncrawl.aggregator.index_query.IndexAggregator.get_number_of_pages.doctree`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.0.1/docs/build/doctrees/generated/cmoncrawl.aggregator.index_query.doctree` & `CmonCrawl-1.0.2/docs/build/doctrees/generated/cmoncrawl.aggregator.index_query.doctree`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.0.1/docs/build/doctrees/generated/cmoncrawl.aggregator.utils.doctree` & `CmonCrawl-1.0.2/docs/build/doctrees/generated/cmoncrawl.aggregator.utils.doctree`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.0.1/docs/build/doctrees/generated/cmoncrawl.aggregator.utils.helpers.doctree` & `CmonCrawl-1.0.2/docs/build/doctrees/generated/cmoncrawl.aggregator.utils.helpers.doctree`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.0.1/docs/build/doctrees/generated/cmoncrawl.aggregator.utils.ndjson_decoder.Decoder.__init__.doctree` & `CmonCrawl-1.0.2/docs/build/doctrees/generated/cmoncrawl.aggregator.utils.ndjson_decoder.Decoder.__init__.doctree`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.0.1/docs/build/doctrees/generated/cmoncrawl.aggregator.utils.ndjson_decoder.Decoder.decode.doctree` & `CmonCrawl-1.0.2/docs/build/doctrees/generated/cmoncrawl.aggregator.utils.ndjson_decoder.Decoder.decode.doctree`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.0.1/docs/build/doctrees/generated/cmoncrawl.aggregator.utils.ndjson_decoder.Decoder.doctree` & `CmonCrawl-1.0.2/docs/build/doctrees/generated/cmoncrawl.aggregator.utils.ndjson_decoder.Decoder.doctree`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.0.1/docs/build/doctrees/generated/cmoncrawl.aggregator.utils.ndjson_decoder.Decoder.raw_decode.doctree` & `CmonCrawl-1.0.2/docs/build/doctrees/generated/cmoncrawl.aggregator.utils.ndjson_decoder.Decoder.raw_decode.doctree`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.0.1/docs/build/doctrees/generated/cmoncrawl.aggregator.utils.ndjson_decoder.doctree` & `CmonCrawl-1.0.2/docs/build/doctrees/generated/cmoncrawl.aggregator.utils.ndjson_decoder.doctree`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.0.1/docs/build/doctrees/generated/cmoncrawl.common.doctree` & `CmonCrawl-1.0.2/docs/build/doctrees/generated/cmoncrawl.common.doctree`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.0.1/docs/build/doctrees/generated/cmoncrawl.common.loggers.doctree` & `CmonCrawl-1.0.2/docs/build/doctrees/generated/cmoncrawl.common.loggers.doctree`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.0.1/docs/build/doctrees/generated/cmoncrawl.common.types.DomainCrawl.__init__.doctree` & `CmonCrawl-1.0.2/docs/build/doctrees/generated/cmoncrawl.common.types.DomainCrawl.__init__.doctree`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.0.1/docs/build/doctrees/generated/cmoncrawl.common.types.DomainCrawl.doctree` & `CmonCrawl-1.0.2/docs/build/doctrees/generated/cmoncrawl.common.types.DomainCrawl.doctree`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.0.1/docs/build/doctrees/generated/cmoncrawl.common.types.DomainRecord.__init__.doctree` & `CmonCrawl-1.0.2/docs/build/doctrees/generated/cmoncrawl.common.types.DomainRecord.__init__.doctree`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.0.1/docs/build/doctrees/generated/cmoncrawl.common.types.DomainRecord.doctree` & `CmonCrawl-1.0.2/docs/build/doctrees/generated/cmoncrawl.common.types.DomainRecord.doctree`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.0.1/docs/build/doctrees/generated/cmoncrawl.common.types.DomainRecord.from_dict.doctree` & `CmonCrawl-1.0.2/docs/build/doctrees/generated/cmoncrawl.common.types.DomainRecord.from_dict.doctree`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.0.1/docs/build/doctrees/generated/cmoncrawl.common.types.DomainRecord.from_json.doctree` & `CmonCrawl-1.0.2/docs/build/doctrees/generated/cmoncrawl.common.types.DomainRecord.from_json.doctree`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.0.1/docs/build/doctrees/generated/cmoncrawl.common.types.DomainRecord.schema.doctree` & `CmonCrawl-1.0.2/docs/build/doctrees/generated/cmoncrawl.common.types.DomainRecord.schema.doctree`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.0.1/docs/build/doctrees/generated/cmoncrawl.common.types.DomainRecord.to_dict.doctree` & `CmonCrawl-1.0.2/docs/build/doctrees/generated/cmoncrawl.common.types.DomainRecord.to_dict.doctree`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.0.1/docs/build/doctrees/generated/cmoncrawl.common.types.DomainRecord.to_json.doctree` & `CmonCrawl-1.0.2/docs/build/doctrees/generated/cmoncrawl.common.types.DomainRecord.to_json.doctree`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.0.1/docs/build/doctrees/generated/cmoncrawl.common.types.ExtractConfig.__init__.doctree` & `CmonCrawl-1.0.2/docs/build/doctrees/generated/cmoncrawl.common.types.ExtractConfig.__init__.doctree`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.0.1/docs/build/doctrees/generated/cmoncrawl.common.types.ExtractConfig.doctree` & `CmonCrawl-1.0.2/docs/build/doctrees/generated/cmoncrawl.common.types.ExtractConfig.doctree`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.0.1/docs/build/doctrees/generated/cmoncrawl.common.types.ExtractConfig.from_dict.doctree` & `CmonCrawl-1.0.2/docs/build/doctrees/generated/cmoncrawl.common.types.ExtractConfig.from_dict.doctree`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.0.1/docs/build/doctrees/generated/cmoncrawl.common.types.ExtractConfig.from_json.doctree` & `CmonCrawl-1.0.2/docs/build/doctrees/generated/cmoncrawl.common.types.ExtractConfig.from_json.doctree`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.0.1/docs/build/doctrees/generated/cmoncrawl.common.types.ExtractConfig.schema.doctree` & `CmonCrawl-1.0.2/docs/build/doctrees/generated/cmoncrawl.common.types.ExtractConfig.schema.doctree`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.0.1/docs/build/doctrees/generated/cmoncrawl.common.types.ExtractConfig.to_dict.doctree` & `CmonCrawl-1.0.2/docs/build/doctrees/generated/cmoncrawl.common.types.ExtractConfig.to_dict.doctree`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.0.1/docs/build/doctrees/generated/cmoncrawl.common.types.ExtractConfig.to_json.doctree` & `CmonCrawl-1.0.2/docs/build/doctrees/generated/cmoncrawl.common.types.ExtractConfig.to_json.doctree`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.0.1/docs/build/doctrees/generated/cmoncrawl.common.types.ExtractorConfig.__init__.doctree` & `CmonCrawl-1.0.2/docs/build/doctrees/generated/cmoncrawl.common.types.ExtractorConfig.__init__.doctree`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.0.1/docs/build/doctrees/generated/cmoncrawl.common.types.ExtractorConfig.doctree` & `CmonCrawl-1.0.2/docs/build/doctrees/generated/cmoncrawl.common.types.ExtractorConfig.doctree`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.0.1/docs/build/doctrees/generated/cmoncrawl.common.types.ExtractorConfig.from_dict.doctree` & `CmonCrawl-1.0.2/docs/build/doctrees/generated/cmoncrawl.common.types.ExtractorConfig.from_dict.doctree`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.0.1/docs/build/doctrees/generated/cmoncrawl.common.types.ExtractorConfig.from_json.doctree` & `CmonCrawl-1.0.2/docs/build/doctrees/generated/cmoncrawl.common.types.ExtractorConfig.from_json.doctree`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.0.1/docs/build/doctrees/generated/cmoncrawl.common.types.ExtractorConfig.schema.doctree` & `CmonCrawl-1.0.2/docs/build/doctrees/generated/cmoncrawl.common.types.ExtractorConfig.schema.doctree`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.0.1/docs/build/doctrees/generated/cmoncrawl.common.types.ExtractorConfig.to_dict.doctree` & `CmonCrawl-1.0.2/docs/build/doctrees/generated/cmoncrawl.common.types.ExtractorConfig.to_dict.doctree`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.0.1/docs/build/doctrees/generated/cmoncrawl.common.types.ExtractorConfig.to_json.doctree` & `CmonCrawl-1.0.2/docs/build/doctrees/generated/cmoncrawl.common.types.ExtractorConfig.to_json.doctree`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.0.1/docs/build/doctrees/generated/cmoncrawl.common.types.PipeMetadata.__init__.doctree` & `CmonCrawl-1.0.2/docs/build/doctrees/generated/cmoncrawl.common.types.PipeMetadata.__init__.doctree`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.0.1/docs/build/doctrees/generated/cmoncrawl.common.types.PipeMetadata.doctree` & `CmonCrawl-1.0.2/docs/build/doctrees/generated/cmoncrawl.common.types.PipeMetadata.doctree`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.0.1/docs/build/doctrees/generated/cmoncrawl.common.types.RetrieveResponse.__init__.doctree` & `CmonCrawl-1.0.2/docs/build/doctrees/generated/cmoncrawl.common.types.RetrieveResponse.__init__.doctree`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.0.1/docs/build/doctrees/generated/cmoncrawl.common.types.RetrieveResponse.doctree` & `CmonCrawl-1.0.2/docs/build/doctrees/generated/cmoncrawl.common.types.RetrieveResponse.doctree`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.0.1/docs/build/doctrees/generated/cmoncrawl.common.types.RoutesConfig.__init__.doctree` & `CmonCrawl-1.0.2/docs/build/doctrees/generated/cmoncrawl.common.types.RoutesConfig.__init__.doctree`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.0.1/docs/build/doctrees/generated/cmoncrawl.common.types.RoutesConfig.doctree` & `CmonCrawl-1.0.2/docs/build/doctrees/generated/cmoncrawl.common.types.RoutesConfig.doctree`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.0.1/docs/build/doctrees/generated/cmoncrawl.common.types.RoutesConfig.from_dict.doctree` & `CmonCrawl-1.0.2/docs/build/doctrees/generated/cmoncrawl.common.types.RoutesConfig.from_dict.doctree`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.0.1/docs/build/doctrees/generated/cmoncrawl.common.types.RoutesConfig.from_json.doctree` & `CmonCrawl-1.0.2/docs/build/doctrees/generated/cmoncrawl.common.types.RoutesConfig.from_json.doctree`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.0.1/docs/build/doctrees/generated/cmoncrawl.common.types.RoutesConfig.schema.doctree` & `CmonCrawl-1.0.2/docs/build/doctrees/generated/cmoncrawl.common.types.RoutesConfig.schema.doctree`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.0.1/docs/build/doctrees/generated/cmoncrawl.common.types.RoutesConfig.to_dict.doctree` & `CmonCrawl-1.0.2/docs/build/doctrees/generated/cmoncrawl.common.types.RoutesConfig.to_dict.doctree`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.0.1/docs/build/doctrees/generated/cmoncrawl.common.types.RoutesConfig.to_json.doctree` & `CmonCrawl-1.0.2/docs/build/doctrees/generated/cmoncrawl.common.types.RoutesConfig.to_json.doctree`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.0.1/docs/build/doctrees/generated/cmoncrawl.common.types.doctree` & `CmonCrawl-1.0.2/docs/build/doctrees/generated/cmoncrawl.common.types.doctree`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.0.1/docs/build/doctrees/generated/cmoncrawl.doctree` & `CmonCrawl-1.0.2/docs/build/doctrees/generated/cmoncrawl.doctree`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.0.1/docs/build/doctrees/generated/cmoncrawl.processor.doctree` & `CmonCrawl-1.0.2/docs/build/doctrees/generated/cmoncrawl.processor.doctree`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.0.1/docs/build/doctrees/generated/cmoncrawl.processor.extraction.doctree` & `CmonCrawl-1.0.2/docs/build/doctrees/generated/cmoncrawl.processor.extraction.doctree`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.0.1/docs/build/doctrees/generated/cmoncrawl.processor.extraction.filters.doctree` & `CmonCrawl-1.0.2/docs/build/doctrees/generated/cmoncrawl.processor.extraction.filters.doctree`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.0.1/docs/build/doctrees/generated/cmoncrawl.processor.extraction.utils.doctree` & `CmonCrawl-1.0.2/docs/build/doctrees/generated/cmoncrawl.processor.extraction.utils.doctree`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.0.1/docs/build/doctrees/generated/cmoncrawl.processor.pipeline.doctree` & `CmonCrawl-1.0.2/docs/build/doctrees/generated/cmoncrawl.processor.pipeline.doctree`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.0.1/docs/build/doctrees/generated/cmoncrawl.processor.pipeline.downloader.AsyncDownloader.__init__.doctree` & `CmonCrawl-1.0.2/docs/build/doctrees/generated/cmoncrawl.processor.pipeline.downloader.AsyncDownloader.__init__.doctree`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.0.1/docs/build/doctrees/generated/cmoncrawl.processor.pipeline.downloader.AsyncDownloader.aclose.doctree` & `CmonCrawl-1.0.2/docs/build/doctrees/generated/cmoncrawl.processor.pipeline.downloader.AsyncDownloader.aclose.doctree`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.0.1/docs/build/doctrees/generated/cmoncrawl.processor.pipeline.downloader.AsyncDownloader.aopen.doctree` & `CmonCrawl-1.0.2/docs/build/doctrees/generated/cmoncrawl.processor.pipeline.downloader.AsyncDownloader.aopen.doctree`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.0.1/docs/build/doctrees/generated/cmoncrawl.processor.pipeline.downloader.AsyncDownloader.doctree` & `CmonCrawl-1.0.2/docs/build/doctrees/generated/cmoncrawl.processor.pipeline.downloader.AsyncDownloader.doctree`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.0.1/docs/build/doctrees/generated/cmoncrawl.processor.pipeline.downloader.AsyncDownloader.download.doctree` & `CmonCrawl-1.0.2/docs/build/doctrees/generated/cmoncrawl.processor.pipeline.downloader.AsyncDownloader.download.doctree`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.0.1/docs/build/doctrees/generated/cmoncrawl.processor.pipeline.downloader.AsyncDownloader.unwrap.doctree` & `CmonCrawl-1.0.2/docs/build/doctrees/generated/cmoncrawl.processor.pipeline.downloader.AsyncDownloader.unwrap.doctree`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.0.1/docs/build/doctrees/generated/cmoncrawl.processor.pipeline.downloader.DownloaderDummy.__init__.doctree` & `CmonCrawl-1.0.2/docs/build/doctrees/generated/cmoncrawl.processor.pipeline.downloader.DownloaderDummy.__init__.doctree`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.0.1/docs/build/doctrees/generated/cmoncrawl.processor.pipeline.downloader.DownloaderDummy.doctree` & `CmonCrawl-1.0.2/docs/build/doctrees/generated/cmoncrawl.processor.pipeline.downloader.DownloaderDummy.doctree`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.0.1/docs/build/doctrees/generated/cmoncrawl.processor.pipeline.downloader.DownloaderDummy.download.doctree` & `CmonCrawl-1.0.2/docs/build/doctrees/generated/cmoncrawl.processor.pipeline.downloader.DownloaderDummy.download.doctree`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.0.1/docs/build/doctrees/generated/cmoncrawl.processor.pipeline.downloader.DownloaderDummy.extract_url.doctree` & `CmonCrawl-1.0.2/docs/build/doctrees/generated/cmoncrawl.processor.pipeline.downloader.DownloaderDummy.extract_url.doctree`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.0.1/docs/build/doctrees/generated/cmoncrawl.processor.pipeline.downloader.DownloaderDummy.extract_year.doctree` & `CmonCrawl-1.0.2/docs/build/doctrees/generated/cmoncrawl.processor.pipeline.downloader.DownloaderDummy.extract_year.doctree`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.0.1/docs/build/doctrees/generated/cmoncrawl.processor.pipeline.downloader.DownloaderDummy.mine_metadata.doctree` & `CmonCrawl-1.0.2/docs/build/doctrees/generated/cmoncrawl.processor.pipeline.downloader.DownloaderDummy.mine_metadata.doctree`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.0.1/docs/build/doctrees/generated/cmoncrawl.processor.pipeline.downloader.IDownloader.__init__.doctree` & `CmonCrawl-1.0.2/docs/build/doctrees/generated/cmoncrawl.processor.pipeline.downloader.IDownloader.__init__.doctree`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.0.1/docs/build/doctrees/generated/cmoncrawl.processor.pipeline.downloader.IDownloader.doctree` & `CmonCrawl-1.0.2/docs/build/doctrees/generated/cmoncrawl.processor.pipeline.downloader.IDownloader.doctree`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.0.1/docs/build/doctrees/generated/cmoncrawl.processor.pipeline.downloader.IDownloader.download.doctree` & `CmonCrawl-1.0.2/docs/build/doctrees/generated/cmoncrawl.processor.pipeline.downloader.IDownloader.download.doctree`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.0.1/docs/build/doctrees/generated/cmoncrawl.processor.pipeline.downloader.doctree` & `CmonCrawl-1.0.2/docs/build/doctrees/generated/cmoncrawl.processor.pipeline.downloader.doctree`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.0.1/docs/build/doctrees/generated/cmoncrawl.processor.pipeline.extractor.BaseExtractor.__init__.doctree` & `CmonCrawl-1.0.2/docs/build/doctrees/generated/cmoncrawl.processor.pipeline.extractor.BaseExtractor.__init__.doctree`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.0.1/docs/build/doctrees/generated/cmoncrawl.processor.pipeline.extractor.BaseExtractor.doctree` & `CmonCrawl-1.0.2/docs/build/doctrees/generated/cmoncrawl.processor.pipeline.extractor.BaseExtractor.doctree`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.0.1/docs/build/doctrees/generated/cmoncrawl.processor.pipeline.extractor.BaseExtractor.extract.doctree` & `CmonCrawl-1.0.2/docs/build/doctrees/generated/cmoncrawl.processor.pipeline.extractor.BaseExtractor.extract.doctree`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.0.1/docs/build/doctrees/generated/cmoncrawl.processor.pipeline.extractor.BaseExtractor.extract_soup.doctree` & `CmonCrawl-1.0.2/docs/build/doctrees/generated/cmoncrawl.processor.pipeline.extractor.BaseExtractor.extract_soup.doctree`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.0.1/docs/build/doctrees/generated/cmoncrawl.processor.pipeline.extractor.BaseExtractor.filter_raw.doctree` & `CmonCrawl-1.0.2/docs/build/doctrees/generated/cmoncrawl.processor.pipeline.extractor.BaseExtractor.filter_raw.doctree`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.0.1/docs/build/doctrees/generated/cmoncrawl.processor.pipeline.extractor.BaseExtractor.filter_soup.doctree` & `CmonCrawl-1.0.2/docs/build/doctrees/generated/cmoncrawl.processor.pipeline.extractor.BaseExtractor.filter_soup.doctree`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.0.1/docs/build/doctrees/generated/cmoncrawl.processor.pipeline.extractor.BaseExtractor.preprocess.doctree` & `CmonCrawl-1.0.2/docs/build/doctrees/generated/cmoncrawl.processor.pipeline.extractor.BaseExtractor.preprocess.doctree`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.0.1/docs/build/doctrees/generated/cmoncrawl.processor.pipeline.extractor.DomainRecordExtractor.__init__.doctree` & `CmonCrawl-1.0.2/docs/build/doctrees/generated/cmoncrawl.processor.pipeline.extractor.DomainRecordExtractor.__init__.doctree`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.0.1/docs/build/doctrees/generated/cmoncrawl.processor.pipeline.extractor.DomainRecordExtractor.doctree` & `CmonCrawl-1.0.2/docs/build/doctrees/generated/cmoncrawl.processor.pipeline.extractor.DomainRecordExtractor.doctree`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.0.1/docs/build/doctrees/generated/cmoncrawl.processor.pipeline.extractor.DomainRecordExtractor.extract.doctree` & `CmonCrawl-1.0.2/docs/build/doctrees/generated/cmoncrawl.processor.pipeline.extractor.DomainRecordExtractor.extract.doctree`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.0.1/docs/build/doctrees/generated/cmoncrawl.processor.pipeline.extractor.DomainRecordExtractor.extract_soup.doctree` & `CmonCrawl-1.0.2/docs/build/doctrees/generated/cmoncrawl.processor.pipeline.extractor.DomainRecordExtractor.extract_soup.doctree`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.0.1/docs/build/doctrees/generated/cmoncrawl.processor.pipeline.extractor.DomainRecordExtractor.filter_raw.doctree` & `CmonCrawl-1.0.2/docs/build/doctrees/generated/cmoncrawl.processor.pipeline.extractor.DomainRecordExtractor.filter_raw.doctree`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.0.1/docs/build/doctrees/generated/cmoncrawl.processor.pipeline.extractor.DomainRecordExtractor.filter_soup.doctree` & `CmonCrawl-1.0.2/docs/build/doctrees/generated/cmoncrawl.processor.pipeline.extractor.DomainRecordExtractor.filter_soup.doctree`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.0.1/docs/build/doctrees/generated/cmoncrawl.processor.pipeline.extractor.DomainRecordExtractor.preprocess.doctree` & `CmonCrawl-1.0.2/docs/build/doctrees/generated/cmoncrawl.processor.pipeline.extractor.DomainRecordExtractor.preprocess.doctree`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.0.1/docs/build/doctrees/generated/cmoncrawl.processor.pipeline.extractor.HTMLExtractor.__init__.doctree` & `CmonCrawl-1.0.2/docs/build/doctrees/generated/cmoncrawl.processor.pipeline.extractor.HTMLExtractor.__init__.doctree`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.0.1/docs/build/doctrees/generated/cmoncrawl.processor.pipeline.extractor.HTMLExtractor.doctree` & `CmonCrawl-1.0.2/docs/build/doctrees/generated/cmoncrawl.processor.pipeline.extractor.HTMLExtractor.doctree`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.0.1/docs/build/doctrees/generated/cmoncrawl.processor.pipeline.extractor.HTMLExtractor.extract.doctree` & `CmonCrawl-1.0.2/docs/build/doctrees/generated/cmoncrawl.processor.pipeline.extractor.HTMLExtractor.extract.doctree`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.0.1/docs/build/doctrees/generated/cmoncrawl.processor.pipeline.extractor.HTMLExtractor.extract_soup.doctree` & `CmonCrawl-1.0.2/docs/build/doctrees/generated/cmoncrawl.processor.pipeline.extractor.HTMLExtractor.extract_soup.doctree`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.0.1/docs/build/doctrees/generated/cmoncrawl.processor.pipeline.extractor.HTMLExtractor.filter_raw.doctree` & `CmonCrawl-1.0.2/docs/build/doctrees/generated/cmoncrawl.processor.pipeline.extractor.HTMLExtractor.filter_raw.doctree`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.0.1/docs/build/doctrees/generated/cmoncrawl.processor.pipeline.extractor.HTMLExtractor.filter_soup.doctree` & `CmonCrawl-1.0.2/docs/build/doctrees/generated/cmoncrawl.processor.pipeline.extractor.HTMLExtractor.filter_soup.doctree`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.0.1/docs/build/doctrees/generated/cmoncrawl.processor.pipeline.extractor.HTMLExtractor.preprocess.doctree` & `CmonCrawl-1.0.2/docs/build/doctrees/generated/cmoncrawl.processor.pipeline.extractor.HTMLExtractor.preprocess.doctree`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.0.1/docs/build/doctrees/generated/cmoncrawl.processor.pipeline.extractor.IExtractor.__init__.doctree` & `CmonCrawl-1.0.2/docs/build/doctrees/generated/cmoncrawl.processor.pipeline.extractor.IExtractor.__init__.doctree`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.0.1/docs/build/doctrees/generated/cmoncrawl.processor.pipeline.extractor.IExtractor.doctree` & `CmonCrawl-1.0.2/docs/build/doctrees/generated/cmoncrawl.processor.pipeline.extractor.IExtractor.doctree`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.0.1/docs/build/doctrees/generated/cmoncrawl.processor.pipeline.extractor.IExtractor.extract.doctree` & `CmonCrawl-1.0.2/docs/build/doctrees/generated/cmoncrawl.processor.pipeline.extractor.IExtractor.extract.doctree`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.0.1/docs/build/doctrees/generated/cmoncrawl.processor.pipeline.extractor.doctree` & `CmonCrawl-1.0.2/docs/build/doctrees/generated/cmoncrawl.processor.pipeline.extractor.doctree`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.0.1/docs/build/doctrees/generated/cmoncrawl.processor.pipeline.pipeline.ProcessorPipeline.__init__.doctree` & `CmonCrawl-1.0.2/docs/build/doctrees/generated/cmoncrawl.processor.pipeline.pipeline.ProcessorPipeline.__init__.doctree`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.0.1/docs/build/doctrees/generated/cmoncrawl.processor.pipeline.pipeline.ProcessorPipeline.doctree` & `CmonCrawl-1.0.2/docs/build/doctrees/generated/cmoncrawl.processor.pipeline.pipeline.ProcessorPipeline.doctree`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.0.1/docs/build/doctrees/generated/cmoncrawl.processor.pipeline.pipeline.ProcessorPipeline.process_domain_record.doctree` & `CmonCrawl-1.0.2/docs/build/doctrees/generated/cmoncrawl.processor.pipeline.pipeline.ProcessorPipeline.process_domain_record.doctree`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.0.1/docs/build/doctrees/generated/cmoncrawl.processor.pipeline.pipeline.doctree` & `CmonCrawl-1.0.2/docs/build/doctrees/generated/cmoncrawl.processor.pipeline.pipeline.doctree`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.0.1/docs/build/doctrees/generated/cmoncrawl.processor.pipeline.router.IRouter.__init__.doctree` & `CmonCrawl-1.0.2/docs/build/doctrees/generated/cmoncrawl.processor.pipeline.router.IRouter.__init__.doctree`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.0.1/docs/build/doctrees/generated/cmoncrawl.processor.pipeline.router.IRouter.doctree` & `CmonCrawl-1.0.2/docs/build/doctrees/generated/cmoncrawl.processor.pipeline.router.IRouter.doctree`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.0.1/docs/build/doctrees/generated/cmoncrawl.processor.pipeline.router.IRouter.route.doctree` & `CmonCrawl-1.0.2/docs/build/doctrees/generated/cmoncrawl.processor.pipeline.router.IRouter.route.doctree`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.0.1/docs/build/doctrees/generated/cmoncrawl.processor.pipeline.router.Route.__init__.doctree` & `CmonCrawl-1.0.2/docs/build/doctrees/generated/cmoncrawl.processor.pipeline.router.Route.__init__.doctree`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.0.1/docs/build/doctrees/generated/cmoncrawl.processor.pipeline.router.Route.doctree` & `CmonCrawl-1.0.2/docs/build/doctrees/generated/cmoncrawl.processor.pipeline.router.Route.doctree`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.0.1/docs/build/doctrees/generated/cmoncrawl.processor.pipeline.router.Router.__init__.doctree` & `CmonCrawl-1.0.2/docs/build/doctrees/generated/cmoncrawl.processor.pipeline.router.Router.__init__.doctree`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.0.1/docs/build/doctrees/generated/cmoncrawl.processor.pipeline.router.Router.doctree` & `CmonCrawl-1.0.2/docs/build/doctrees/generated/cmoncrawl.processor.pipeline.router.Router.doctree`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.0.1/docs/build/doctrees/generated/cmoncrawl.processor.pipeline.router.Router.load_extractor.doctree` & `CmonCrawl-1.0.2/docs/build/doctrees/generated/cmoncrawl.processor.pipeline.router.Router.load_extractor.doctree`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.0.1/docs/build/doctrees/generated/cmoncrawl.processor.pipeline.router.Router.load_module.doctree` & `CmonCrawl-1.0.2/docs/build/doctrees/generated/cmoncrawl.processor.pipeline.router.Router.load_module.doctree`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.0.1/docs/build/doctrees/generated/cmoncrawl.processor.pipeline.router.Router.load_module_as_extractor.doctree` & `CmonCrawl-1.0.2/docs/build/doctrees/generated/cmoncrawl.processor.pipeline.router.Router.load_module_as_extractor.doctree`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.0.1/docs/build/doctrees/generated/cmoncrawl.processor.pipeline.router.Router.load_modules.doctree` & `CmonCrawl-1.0.2/docs/build/doctrees/generated/cmoncrawl.processor.pipeline.router.Router.load_modules.doctree`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.0.1/docs/build/doctrees/generated/cmoncrawl.processor.pipeline.router.Router.register_route.doctree` & `CmonCrawl-1.0.2/docs/build/doctrees/generated/cmoncrawl.processor.pipeline.router.Router.register_route.doctree`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.0.1/docs/build/doctrees/generated/cmoncrawl.processor.pipeline.router.Router.register_routes.doctree` & `CmonCrawl-1.0.2/docs/build/doctrees/generated/cmoncrawl.processor.pipeline.router.Router.register_routes.doctree`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.0.1/docs/build/doctrees/generated/cmoncrawl.processor.pipeline.router.Router.route.doctree` & `CmonCrawl-1.0.2/docs/build/doctrees/generated/cmoncrawl.processor.pipeline.router.Router.route.doctree`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.0.1/docs/build/doctrees/generated/cmoncrawl.processor.pipeline.router.doctree` & `CmonCrawl-1.0.2/docs/build/doctrees/generated/cmoncrawl.processor.pipeline.router.doctree`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.0.1/docs/build/doctrees/generated/cmoncrawl.processor.pipeline.streamer.BaseStreamerFile.__init__.doctree` & `CmonCrawl-1.0.2/docs/build/doctrees/generated/cmoncrawl.processor.pipeline.streamer.BaseStreamerFile.__init__.doctree`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.0.1/docs/build/doctrees/generated/cmoncrawl.processor.pipeline.streamer.BaseStreamerFile.clean_up.doctree` & `CmonCrawl-1.0.2/docs/build/doctrees/generated/cmoncrawl.processor.pipeline.streamer.BaseStreamerFile.clean_up.doctree`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.0.1/docs/build/doctrees/generated/cmoncrawl.processor.pipeline.streamer.BaseStreamerFile.doctree` & `CmonCrawl-1.0.2/docs/build/doctrees/generated/cmoncrawl.processor.pipeline.streamer.BaseStreamerFile.doctree`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.0.1/docs/build/doctrees/generated/cmoncrawl.processor.pipeline.streamer.BaseStreamerFile.get_file_name.doctree` & `CmonCrawl-1.0.2/docs/build/doctrees/generated/cmoncrawl.processor.pipeline.streamer.BaseStreamerFile.get_file_name.doctree`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.0.1/docs/build/doctrees/generated/cmoncrawl.processor.pipeline.streamer.BaseStreamerFile.metadata_to_string.doctree` & `CmonCrawl-1.0.2/docs/build/doctrees/generated/cmoncrawl.processor.pipeline.streamer.BaseStreamerFile.metadata_to_string.doctree`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.0.1/docs/build/doctrees/generated/cmoncrawl.processor.pipeline.streamer.BaseStreamerFile.stream.doctree` & `CmonCrawl-1.0.2/docs/build/doctrees/generated/cmoncrawl.processor.pipeline.streamer.BaseStreamerFile.stream.doctree`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.0.1/docs/build/doctrees/generated/cmoncrawl.processor.pipeline.streamer.IStreamer.__init__.doctree` & `CmonCrawl-1.0.2/docs/build/doctrees/generated/cmoncrawl.processor.pipeline.streamer.IStreamer.__init__.doctree`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.0.1/docs/build/doctrees/generated/cmoncrawl.processor.pipeline.streamer.IStreamer.clean_up.doctree` & `CmonCrawl-1.0.2/docs/build/doctrees/generated/cmoncrawl.processor.pipeline.streamer.IStreamer.clean_up.doctree`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.0.1/docs/build/doctrees/generated/cmoncrawl.processor.pipeline.streamer.IStreamer.doctree` & `CmonCrawl-1.0.2/docs/build/doctrees/generated/cmoncrawl.processor.pipeline.streamer.IStreamer.doctree`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.0.1/docs/build/doctrees/generated/cmoncrawl.processor.pipeline.streamer.IStreamer.stream.doctree` & `CmonCrawl-1.0.2/docs/build/doctrees/generated/cmoncrawl.processor.pipeline.streamer.IStreamer.stream.doctree`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.0.1/docs/build/doctrees/generated/cmoncrawl.processor.pipeline.streamer.StreamerDummy.__init__.doctree` & `CmonCrawl-1.0.2/docs/build/doctrees/generated/cmoncrawl.processor.pipeline.streamer.StreamerDummy.__init__.doctree`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.0.1/docs/build/doctrees/generated/cmoncrawl.processor.pipeline.streamer.StreamerDummy.clean_up.doctree` & `CmonCrawl-1.0.2/docs/build/doctrees/generated/cmoncrawl.processor.pipeline.streamer.StreamerDummy.clean_up.doctree`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.0.1/docs/build/doctrees/generated/cmoncrawl.processor.pipeline.streamer.StreamerDummy.doctree` & `CmonCrawl-1.0.2/docs/build/doctrees/generated/cmoncrawl.processor.pipeline.streamer.StreamerDummy.doctree`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.0.1/docs/build/doctrees/generated/cmoncrawl.processor.pipeline.streamer.StreamerDummy.stream.doctree` & `CmonCrawl-1.0.2/docs/build/doctrees/generated/cmoncrawl.processor.pipeline.streamer.StreamerDummy.stream.doctree`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.0.1/docs/build/doctrees/generated/cmoncrawl.processor.pipeline.streamer.StreamerFileHTML.__init__.doctree` & `CmonCrawl-1.0.2/docs/build/doctrees/generated/cmoncrawl.processor.pipeline.streamer.StreamerFileHTML.__init__.doctree`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.0.1/docs/build/doctrees/generated/cmoncrawl.processor.pipeline.streamer.StreamerFileHTML.clean_up.doctree` & `CmonCrawl-1.0.2/docs/build/doctrees/generated/cmoncrawl.processor.pipeline.streamer.StreamerFileHTML.clean_up.doctree`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.0.1/docs/build/doctrees/generated/cmoncrawl.processor.pipeline.streamer.StreamerFileHTML.doctree` & `CmonCrawl-1.0.2/docs/build/doctrees/generated/cmoncrawl.processor.pipeline.streamer.StreamerFileHTML.doctree`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.0.1/docs/build/doctrees/generated/cmoncrawl.processor.pipeline.streamer.StreamerFileHTML.get_file_name.doctree` & `CmonCrawl-1.0.2/docs/build/doctrees/generated/cmoncrawl.processor.pipeline.streamer.StreamerFileHTML.get_file_name.doctree`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.0.1/docs/build/doctrees/generated/cmoncrawl.processor.pipeline.streamer.StreamerFileHTML.metadata_to_string.doctree` & `CmonCrawl-1.0.2/docs/build/doctrees/generated/cmoncrawl.processor.pipeline.streamer.StreamerFileHTML.metadata_to_string.doctree`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.0.1/docs/build/doctrees/generated/cmoncrawl.processor.pipeline.streamer.StreamerFileHTML.stream.doctree` & `CmonCrawl-1.0.2/docs/build/doctrees/generated/cmoncrawl.processor.pipeline.streamer.StreamerFileHTML.stream.doctree`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.0.1/docs/build/doctrees/generated/cmoncrawl.processor.pipeline.streamer.StreamerFileJSON.__init__.doctree` & `CmonCrawl-1.0.2/docs/build/doctrees/generated/cmoncrawl.processor.pipeline.streamer.StreamerFileJSON.__init__.doctree`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.0.1/docs/build/doctrees/generated/cmoncrawl.processor.pipeline.streamer.StreamerFileJSON.clean_up.doctree` & `CmonCrawl-1.0.2/docs/build/doctrees/generated/cmoncrawl.processor.pipeline.streamer.StreamerFileJSON.clean_up.doctree`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.0.1/docs/build/doctrees/generated/cmoncrawl.processor.pipeline.streamer.StreamerFileJSON.doctree` & `CmonCrawl-1.0.2/docs/build/doctrees/generated/cmoncrawl.processor.pipeline.streamer.StreamerFileJSON.doctree`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.0.1/docs/build/doctrees/generated/cmoncrawl.processor.pipeline.streamer.StreamerFileJSON.get_file_name.doctree` & `CmonCrawl-1.0.2/docs/build/doctrees/generated/cmoncrawl.processor.pipeline.streamer.StreamerFileJSON.get_file_name.doctree`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.0.1/docs/build/doctrees/generated/cmoncrawl.processor.pipeline.streamer.StreamerFileJSON.metadata_to_string.doctree` & `CmonCrawl-1.0.2/docs/build/doctrees/generated/cmoncrawl.processor.pipeline.streamer.StreamerFileJSON.metadata_to_string.doctree`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.0.1/docs/build/doctrees/generated/cmoncrawl.processor.pipeline.streamer.StreamerFileJSON.stream.doctree` & `CmonCrawl-1.0.2/docs/build/doctrees/generated/cmoncrawl.processor.pipeline.streamer.StreamerFileJSON.stream.doctree`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.0.1/docs/build/doctrees/generated/cmoncrawl.processor.pipeline.streamer.doctree` & `CmonCrawl-1.0.2/docs/build/doctrees/generated/cmoncrawl.processor.pipeline.streamer.doctree`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.0.1/docs/build/doctrees/index.doctree` & `CmonCrawl-1.0.2/docs/build/doctrees/index.doctree`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.0.1/docs/build/doctrees/misc/domain_record.doctree` & `CmonCrawl-1.0.2/docs/build/doctrees/misc/domain_record.doctree`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.0.1/docs/build/doctrees/misc/index.doctree` & `CmonCrawl-1.0.2/docs/build/doctrees/misc/index.doctree`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.0.1/docs/build/doctrees/prog_guide/index.doctree` & `CmonCrawl-1.0.2/docs/build/doctrees/prog_guide/index.doctree`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.0.1/docs/build/doctrees/prog_guide/overview.doctree` & `CmonCrawl-1.0.2/docs/build/doctrees/prog_guide/overview.doctree`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.0.1/docs/build/doctrees/prog_guide/pip.doctree` & `CmonCrawl-1.0.2/docs/build/doctrees/prog_guide/pip.doctree`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.0.1/docs/build/doctrees/usage.doctree` & `CmonCrawl-1.0.2/docs/build/doctrees/usage.doctree`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.0.1/docs/build/html/_sources/cli/cli.rst.txt` & `CmonCrawl-1.0.2/docs/build/html/_sources/cli/cli.rst.txt`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.0.1/docs/build/html/_sources/cli/download.rst.txt` & `CmonCrawl-1.0.2/docs/build/html/_sources/cli/download.rst.txt`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.0.1/docs/build/html/_sources/cli/extract.rst.txt` & `CmonCrawl-1.0.2/docs/build/html/_sources/cli/extract.rst.txt`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.0.1/docs/build/html/_sources/extraction/config_file.rst.txt` & `CmonCrawl-1.0.2/docs/build/html/_sources/extraction/config_file.rst.txt`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.0.1/docs/build/html/_sources/extraction/creating_extractor.rst.txt` & `CmonCrawl-1.0.2/docs/build/html/_sources/extraction/creating_extractor.rst.txt`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.0.1/docs/build/html/_sources/extraction/utils.rst.txt` & `CmonCrawl-1.0.2/docs/build/html/_sources/extraction/utils.rst.txt`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.0.1/docs/build/html/_sources/generated/cmoncrawl.aggregator.index_query.IndexAggregator.rst.txt` & `CmonCrawl-1.0.2/docs/build/html/_sources/generated/cmoncrawl.aggregator.index_query.IndexAggregator.rst.txt`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.0.1/docs/build/html/_sources/generated/cmoncrawl.common.types.DomainRecord.rst.txt` & `CmonCrawl-1.0.2/docs/build/html/_sources/generated/cmoncrawl.common.types.DomainRecord.rst.txt`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.0.1/docs/build/html/_sources/generated/cmoncrawl.common.types.ExtractConfig.rst.txt` & `CmonCrawl-1.0.2/docs/build/html/_sources/generated/cmoncrawl.common.types.ExtractConfig.rst.txt`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.0.1/docs/build/html/_sources/generated/cmoncrawl.common.types.ExtractorConfig.rst.txt` & `CmonCrawl-1.0.2/docs/build/html/_sources/generated/cmoncrawl.common.types.ExtractorConfig.rst.txt`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.0.1/docs/build/html/_sources/generated/cmoncrawl.common.types.PipeMetadata.rst.txt` & `CmonCrawl-1.0.2/docs/build/html/_sources/generated/cmoncrawl.common.types.PipeMetadata.rst.txt`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.0.1/docs/build/html/_sources/generated/cmoncrawl.common.types.RoutesConfig.rst.txt` & `CmonCrawl-1.0.2/docs/build/html/_sources/generated/cmoncrawl.common.types.RoutesConfig.rst.txt`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.0.1/docs/build/html/_sources/generated/cmoncrawl.processor.pipeline.extractor.DomainRecordExtractor.rst.txt` & `CmonCrawl-1.0.2/docs/build/html/_sources/generated/cmoncrawl.processor.pipeline.extractor.DomainRecordExtractor.rst.txt`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.0.1/docs/build/html/_sources/index.rst.txt` & `CmonCrawl-1.0.2/docs/build/html/_sources/index.rst.txt`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.0.1/docs/build/html/_sources/misc/domain_record.rst.txt` & `CmonCrawl-1.0.2/docs/build/html/_sources/misc/domain_record.rst.txt`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.0.1/docs/build/html/_sources/prog_guide/overview.rst.txt` & `CmonCrawl-1.0.2/docs/build/html/_sources/prog_guide/overview.rst.txt`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.0.1/docs/build/html/_sources/prog_guide/pip.rst.txt` & `CmonCrawl-1.0.2/docs/build/html/_sources/prog_guide/pip.rst.txt`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.0.1/docs/build/html/_sources/usage.rst.txt` & `CmonCrawl-1.0.2/docs/build/html/_sources/usage.rst.txt`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.0.1/docs/build/html/_static/_sphinx_javascript_frameworks_compat.js` & `CmonCrawl-1.0.2/docs/build/html/_static/_sphinx_javascript_frameworks_compat.js`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.0.1/docs/build/html/_static/basic.css` & `CmonCrawl-1.0.2/docs/build/html/_static/basic.css`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.0.1/docs/build/html/_static/clipboard.min.js` & `CmonCrawl-1.0.2/docs/build/html/_static/clipboard.min.js`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.0.1/docs/build/html/_static/copybutton.css` & `CmonCrawl-1.0.2/docs/build/html/_static/copybutton.css`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.0.1/docs/build/html/_static/copybutton.js` & `CmonCrawl-1.0.2/docs/build/html/_static/copybutton.js`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.0.1/docs/build/html/_static/copybutton_funcs.js` & `CmonCrawl-1.0.2/docs/build/html/_static/copybutton_funcs.js`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.0.1/docs/build/html/_static/doctools.js` & `CmonCrawl-1.0.2/docs/build/html/_static/doctools.js`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.0.1/docs/build/html/_static/images/logo_binder.svg` & `CmonCrawl-1.0.2/docs/build/html/_static/images/logo_binder.svg`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.0.1/docs/build/html/_static/images/logo_colab.png` & `CmonCrawl-1.0.2/docs/build/html/_static/images/logo_colab.png`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.0.1/docs/build/html/_static/images/logo_deepnote.svg` & `CmonCrawl-1.0.2/docs/build/html/_static/images/logo_deepnote.svg`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.0.1/docs/build/html/_static/images/logo_jupyterhub.svg` & `CmonCrawl-1.0.2/docs/build/html/_static/images/logo_jupyterhub.svg`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.0.1/docs/build/html/_static/jquery-3.6.0.js` & `CmonCrawl-1.0.2/docs/build/html/_static/jquery-3.6.0.js`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.0.1/docs/build/html/_static/jquery.js` & `CmonCrawl-1.0.2/docs/build/html/_static/jquery.js`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.0.1/docs/build/html/_static/language_data.js` & `CmonCrawl-1.0.2/docs/build/html/_static/language_data.js`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.0.1/docs/build/html/_static/locales/ar/LC_MESSAGES/booktheme.po` & `CmonCrawl-1.0.2/docs/build/html/_static/locales/ar/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.0.1/docs/build/html/_static/locales/bg/LC_MESSAGES/booktheme.po` & `CmonCrawl-1.0.2/docs/build/html/_static/locales/bg/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.0.1/docs/build/html/_static/locales/bn/LC_MESSAGES/booktheme.po` & `CmonCrawl-1.0.2/docs/build/html/_static/locales/bn/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.0.1/docs/build/html/_static/locales/ca/LC_MESSAGES/booktheme.po` & `CmonCrawl-1.0.2/docs/build/html/_static/locales/ca/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.0.1/docs/build/html/_static/locales/cs/LC_MESSAGES/booktheme.po` & `CmonCrawl-1.0.2/docs/build/html/_static/locales/cs/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.0.1/docs/build/html/_static/locales/da/LC_MESSAGES/booktheme.po` & `CmonCrawl-1.0.2/docs/build/html/_static/locales/da/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.0.1/docs/build/html/_static/locales/de/LC_MESSAGES/booktheme.po` & `CmonCrawl-1.0.2/docs/build/html/_static/locales/de/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.0.1/docs/build/html/_static/locales/el/LC_MESSAGES/booktheme.po` & `CmonCrawl-1.0.2/docs/build/html/_static/locales/el/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.0.1/docs/build/html/_static/locales/eo/LC_MESSAGES/booktheme.po` & `CmonCrawl-1.0.2/docs/build/html/_static/locales/eo/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.0.1/docs/build/html/_static/locales/es/LC_MESSAGES/booktheme.po` & `CmonCrawl-1.0.2/docs/build/html/_static/locales/es/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.0.1/docs/build/html/_static/locales/et/LC_MESSAGES/booktheme.po` & `CmonCrawl-1.0.2/docs/build/html/_static/locales/et/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.0.1/docs/build/html/_static/locales/fi/LC_MESSAGES/booktheme.po` & `CmonCrawl-1.0.2/docs/build/html/_static/locales/fi/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.0.1/docs/build/html/_static/locales/fr/LC_MESSAGES/booktheme.po` & `CmonCrawl-1.0.2/docs/build/html/_static/locales/fr/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.0.1/docs/build/html/_static/locales/hr/LC_MESSAGES/booktheme.po` & `CmonCrawl-1.0.2/docs/build/html/_static/locales/hr/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.0.1/docs/build/html/_static/locales/id/LC_MESSAGES/booktheme.po` & `CmonCrawl-1.0.2/docs/build/html/_static/locales/id/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.0.1/docs/build/html/_static/locales/it/LC_MESSAGES/booktheme.po` & `CmonCrawl-1.0.2/docs/build/html/_static/locales/it/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.0.1/docs/build/html/_static/locales/iw/LC_MESSAGES/booktheme.po` & `CmonCrawl-1.0.2/docs/build/html/_static/locales/iw/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.0.1/docs/build/html/_static/locales/ja/LC_MESSAGES/booktheme.po` & `CmonCrawl-1.0.2/docs/build/html/_static/locales/ja/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.0.1/docs/build/html/_static/locales/ko/LC_MESSAGES/booktheme.po` & `CmonCrawl-1.0.2/docs/build/html/_static/locales/ko/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.0.1/docs/build/html/_static/locales/lt/LC_MESSAGES/booktheme.po` & `CmonCrawl-1.0.2/docs/build/html/_static/locales/lt/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.0.1/docs/build/html/_static/locales/lv/LC_MESSAGES/booktheme.po` & `CmonCrawl-1.0.2/docs/build/html/_static/locales/lv/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.0.1/docs/build/html/_static/locales/ml/LC_MESSAGES/booktheme.po` & `CmonCrawl-1.0.2/docs/build/html/_static/locales/ml/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.0.1/docs/build/html/_static/locales/mr/LC_MESSAGES/booktheme.po` & `CmonCrawl-1.0.2/docs/build/html/_static/locales/mr/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.0.1/docs/build/html/_static/locales/ms/LC_MESSAGES/booktheme.po` & `CmonCrawl-1.0.2/docs/build/html/_static/locales/ms/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.0.1/docs/build/html/_static/locales/nl/LC_MESSAGES/booktheme.po` & `CmonCrawl-1.0.2/docs/build/html/_static/locales/nl/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.0.1/docs/build/html/_static/locales/no/LC_MESSAGES/booktheme.po` & `CmonCrawl-1.0.2/docs/build/html/_static/locales/no/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.0.1/docs/build/html/_static/locales/pl/LC_MESSAGES/booktheme.po` & `CmonCrawl-1.0.2/docs/build/html/_static/locales/pl/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.0.1/docs/build/html/_static/locales/pt/LC_MESSAGES/booktheme.po` & `CmonCrawl-1.0.2/docs/build/html/_static/locales/pt/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.0.1/docs/build/html/_static/locales/ro/LC_MESSAGES/booktheme.po` & `CmonCrawl-1.0.2/docs/build/html/_static/locales/ro/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.0.1/docs/build/html/_static/locales/ru/LC_MESSAGES/booktheme.po` & `CmonCrawl-1.0.2/docs/build/html/_static/locales/ru/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.0.1/docs/build/html/_static/locales/sk/LC_MESSAGES/booktheme.po` & `CmonCrawl-1.0.2/docs/build/html/_static/locales/sk/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.0.1/docs/build/html/_static/locales/sl/LC_MESSAGES/booktheme.po` & `CmonCrawl-1.0.2/docs/build/html/_static/locales/sl/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.0.1/docs/build/html/_static/locales/sr/LC_MESSAGES/booktheme.po` & `CmonCrawl-1.0.2/docs/build/html/_static/locales/sr/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.0.1/docs/build/html/_static/locales/sv/LC_MESSAGES/booktheme.po` & `CmonCrawl-1.0.2/docs/build/html/_static/locales/sv/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.0.1/docs/build/html/_static/locales/ta/LC_MESSAGES/booktheme.po` & `CmonCrawl-1.0.2/docs/build/html/_static/locales/ta/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.0.1/docs/build/html/_static/locales/te/LC_MESSAGES/booktheme.po` & `CmonCrawl-1.0.2/docs/build/html/_static/locales/te/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.0.1/docs/build/html/_static/locales/tg/LC_MESSAGES/booktheme.po` & `CmonCrawl-1.0.2/docs/build/html/_static/locales/tg/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.0.1/docs/build/html/_static/locales/th/LC_MESSAGES/booktheme.po` & `CmonCrawl-1.0.2/docs/build/html/_static/locales/th/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.0.1/docs/build/html/_static/locales/tl/LC_MESSAGES/booktheme.po` & `CmonCrawl-1.0.2/docs/build/html/_static/locales/tl/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.0.1/docs/build/html/_static/locales/tr/LC_MESSAGES/booktheme.po` & `CmonCrawl-1.0.2/docs/build/html/_static/locales/tr/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.0.1/docs/build/html/_static/locales/uk/LC_MESSAGES/booktheme.po` & `CmonCrawl-1.0.2/docs/build/html/_static/locales/uk/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.0.1/docs/build/html/_static/locales/ur/LC_MESSAGES/booktheme.po` & `CmonCrawl-1.0.2/docs/build/html/_static/locales/ur/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.0.1/docs/build/html/_static/locales/vi/LC_MESSAGES/booktheme.po` & `CmonCrawl-1.0.2/docs/build/html/_static/locales/vi/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.0.1/docs/build/html/_static/locales/zh_CN/LC_MESSAGES/booktheme.po` & `CmonCrawl-1.0.2/docs/build/html/_static/locales/zh_CN/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.0.1/docs/build/html/_static/locales/zh_TW/LC_MESSAGES/booktheme.po` & `CmonCrawl-1.0.2/docs/build/html/_static/locales/zh_TW/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.0.1/docs/build/html/_static/pygments.css` & `CmonCrawl-1.0.2/docs/build/html/_static/pygments.css`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.0.1/docs/build/html/_static/scripts/pydata-sphinx-theme.js` & `CmonCrawl-1.0.2/docs/build/html/_static/scripts/pydata-sphinx-theme.js`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.0.1/docs/build/html/_static/scripts/sphinx-book-theme.js` & `CmonCrawl-1.0.2/docs/build/html/_static/scripts/sphinx-book-theme.js`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.0.1/docs/build/html/_static/scripts/sphinx-book-theme.js.map` & `CmonCrawl-1.0.2/docs/build/html/_static/scripts/sphinx-book-theme.js.map`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.0.1/docs/build/html/_static/searchtools.js` & `CmonCrawl-1.0.2/docs/build/html/_static/searchtools.js`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.0.1/docs/build/html/_static/sphinx_highlight.js` & `CmonCrawl-1.0.2/docs/build/html/_static/sphinx_highlight.js`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.0.1/docs/build/html/_static/styles/pydata-sphinx-theme.css` & `CmonCrawl-1.0.2/docs/build/html/_static/styles/pydata-sphinx-theme.css`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.0.1/docs/build/html/_static/styles/sphinx-book-theme.css` & `CmonCrawl-1.0.2/docs/build/html/_static/styles/sphinx-book-theme.css`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.0.1/docs/build/html/_static/styles/theme.css` & `CmonCrawl-1.0.2/docs/build/html/_static/styles/theme.css`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.0.1/docs/build/html/_static/underscore-1.13.1.js` & `CmonCrawl-1.0.2/docs/build/html/_static/underscore-1.13.1.js`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.0.1/docs/build/html/_static/underscore.js` & `CmonCrawl-1.0.2/docs/build/html/_static/underscore.js`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.0.1/docs/build/html/_static/vendor/fontawesome/5.13.0/LICENSE.txt` & `CmonCrawl-1.0.2/docs/build/html/_static/vendor/fontawesome/5.13.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.0.1/docs/build/html/_static/vendor/fontawesome/5.13.0/css/all.min.css` & `CmonCrawl-1.0.2/docs/build/html/_static/vendor/fontawesome/5.13.0/css/all.min.css`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.0.1/docs/build/html/_static/vendor/fontawesome/5.13.0/webfonts/fa-brands-400.eot` & `CmonCrawl-1.0.2/docs/build/html/_static/vendor/fontawesome/5.13.0/webfonts/fa-brands-400.eot`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.0.1/docs/build/html/_static/vendor/fontawesome/5.13.0/webfonts/fa-brands-400.svg` & `CmonCrawl-1.0.2/docs/build/html/_static/vendor/fontawesome/5.13.0/webfonts/fa-brands-400.svg`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.0.1/docs/build/html/_static/vendor/fontawesome/5.13.0/webfonts/fa-brands-400.ttf` & `CmonCrawl-1.0.2/docs/build/html/_static/vendor/fontawesome/5.13.0/webfonts/fa-brands-400.ttf`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.0.1/docs/build/html/_static/vendor/fontawesome/5.13.0/webfonts/fa-brands-400.woff` & `CmonCrawl-1.0.2/docs/build/html/_static/vendor/fontawesome/5.13.0/webfonts/fa-brands-400.woff`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.0.1/docs/build/html/_static/vendor/fontawesome/5.13.0/webfonts/fa-brands-400.woff2` & `CmonCrawl-1.0.2/docs/build/html/_static/vendor/fontawesome/5.13.0/webfonts/fa-brands-400.woff2`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.0.1/docs/build/html/_static/vendor/fontawesome/5.13.0/webfonts/fa-regular-400.eot` & `CmonCrawl-1.0.2/docs/build/html/_static/vendor/fontawesome/5.13.0/webfonts/fa-regular-400.eot`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.0.1/docs/build/html/_static/vendor/fontawesome/5.13.0/webfonts/fa-regular-400.svg` & `CmonCrawl-1.0.2/docs/build/html/_static/vendor/fontawesome/5.13.0/webfonts/fa-regular-400.svg`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.0.1/docs/build/html/_static/vendor/fontawesome/5.13.0/webfonts/fa-regular-400.ttf` & `CmonCrawl-1.0.2/docs/build/html/_static/vendor/fontawesome/5.13.0/webfonts/fa-regular-400.ttf`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.0.1/docs/build/html/_static/vendor/fontawesome/5.13.0/webfonts/fa-regular-400.woff` & `CmonCrawl-1.0.2/docs/build/html/_static/vendor/fontawesome/5.13.0/webfonts/fa-regular-400.woff`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.0.1/docs/build/html/_static/vendor/fontawesome/5.13.0/webfonts/fa-regular-400.woff2` & `CmonCrawl-1.0.2/docs/build/html/_static/vendor/fontawesome/5.13.0/webfonts/fa-regular-400.woff2`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.0.1/docs/build/html/_static/vendor/fontawesome/5.13.0/webfonts/fa-solid-900.eot` & `CmonCrawl-1.0.2/docs/build/html/_static/vendor/fontawesome/5.13.0/webfonts/fa-solid-900.eot`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.0.1/docs/build/html/_static/vendor/fontawesome/5.13.0/webfonts/fa-solid-900.svg` & `CmonCrawl-1.0.2/docs/build/html/_static/vendor/fontawesome/5.13.0/webfonts/fa-solid-900.svg`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.0.1/docs/build/html/_static/vendor/fontawesome/5.13.0/webfonts/fa-solid-900.ttf` & `CmonCrawl-1.0.2/docs/build/html/_static/vendor/fontawesome/5.13.0/webfonts/fa-solid-900.ttf`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.0.1/docs/build/html/_static/vendor/fontawesome/5.13.0/webfonts/fa-solid-900.woff` & `CmonCrawl-1.0.2/docs/build/html/_static/vendor/fontawesome/5.13.0/webfonts/fa-solid-900.woff`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.0.1/docs/build/html/_static/vendor/fontawesome/5.13.0/webfonts/fa-solid-900.woff2` & `CmonCrawl-1.0.2/docs/build/html/_static/vendor/fontawesome/5.13.0/webfonts/fa-solid-900.woff2`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.0.1/docs/build/html/_static/webpack-macros.html` & `CmonCrawl-1.0.2/docs/build/html/_static/webpack-macros.html`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.0.1/docs/build/html/api.html` & `CmonCrawl-1.0.2/docs/build/html/api.html`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.0.1/docs/build/html/cli/cli.html` & `CmonCrawl-1.0.2/docs/build/html/cli/cli.html`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.0.1/docs/build/html/cli/download.html` & `CmonCrawl-1.0.2/docs/build/html/cli/download.html`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.0.1/docs/build/html/cli/extract.html` & `CmonCrawl-1.0.2/docs/build/html/cli/extract.html`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.0.1/docs/build/html/cli/index.html` & `CmonCrawl-1.0.2/docs/build/html/cli/index.html`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.0.1/docs/build/html/extraction/config_file.html` & `CmonCrawl-1.0.2/docs/build/html/extraction/config_file.html`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.0.1/docs/build/html/extraction/creating_extractor.html` & `CmonCrawl-1.0.2/docs/build/html/extraction/creating_extractor.html`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.0.1/docs/build/html/extraction/index.html` & `CmonCrawl-1.0.2/docs/build/html/extraction/index.html`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.0.1/docs/build/html/extraction/utils.html` & `CmonCrawl-1.0.2/docs/build/html/extraction/utils.html`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.0.1/docs/build/html/generated/cmoncrawl.aggregator.html` & `CmonCrawl-1.0.2/docs/build/html/generated/cmoncrawl.aggregator.html`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.0.1/docs/build/html/generated/cmoncrawl.aggregator.index_query.IndexAggregator.__init__.html` & `CmonCrawl-1.0.2/docs/build/html/generated/cmoncrawl.aggregator.index_query.IndexAggregator.__init__.html`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.0.1/docs/build/html/generated/cmoncrawl.aggregator.index_query.IndexAggregator.aclose.html` & `CmonCrawl-1.0.2/docs/build/html/generated/cmoncrawl.aggregator.index_query.IndexAggregator.aclose.html`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.0.1/docs/build/html/generated/cmoncrawl.aggregator.index_query.IndexAggregator.aopen.html` & `CmonCrawl-1.0.2/docs/build/html/generated/cmoncrawl.aggregator.index_query.IndexAggregator.aopen.html`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.0.1/docs/build/html/generated/cmoncrawl.aggregator.index_query.IndexAggregator.get_all_CC_indexes.html` & `CmonCrawl-1.0.2/docs/build/html/generated/cmoncrawl.aggregator.index_query.IndexAggregator.get_all_CC_indexes.html`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.0.1/docs/build/html/generated/cmoncrawl.aggregator.index_query.IndexAggregator.get_captured_responses.html` & `CmonCrawl-1.0.2/docs/build/html/generated/cmoncrawl.aggregator.index_query.IndexAggregator.get_captured_responses.html`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.0.1/docs/build/html/generated/cmoncrawl.aggregator.index_query.IndexAggregator.get_number_of_pages.html` & `CmonCrawl-1.0.2/docs/build/html/generated/cmoncrawl.aggregator.index_query.IndexAggregator.get_number_of_pages.html`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.0.1/docs/build/html/generated/cmoncrawl.aggregator.index_query.IndexAggregator.html` & `CmonCrawl-1.0.2/docs/build/html/generated/cmoncrawl.aggregator.index_query.IndexAggregator.html`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.0.1/docs/build/html/generated/cmoncrawl.aggregator.index_query.html` & `CmonCrawl-1.0.2/docs/build/html/generated/cmoncrawl.aggregator.index_query.html`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.0.1/docs/build/html/generated/cmoncrawl.aggregator.utils.helpers.html` & `CmonCrawl-1.0.2/docs/build/html/generated/cmoncrawl.aggregator.utils.helpers.html`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.0.1/docs/build/html/generated/cmoncrawl.aggregator.utils.html` & `CmonCrawl-1.0.2/docs/build/html/generated/cmoncrawl.aggregator.utils.html`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.0.1/docs/build/html/generated/cmoncrawl.aggregator.utils.ndjson_decoder.Decoder.__init__.html` & `CmonCrawl-1.0.2/docs/build/html/generated/cmoncrawl.aggregator.utils.ndjson_decoder.Decoder.__init__.html`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.0.1/docs/build/html/generated/cmoncrawl.aggregator.utils.ndjson_decoder.Decoder.decode.html` & `CmonCrawl-1.0.2/docs/build/html/generated/cmoncrawl.aggregator.utils.ndjson_decoder.Decoder.decode.html`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.0.1/docs/build/html/generated/cmoncrawl.aggregator.utils.ndjson_decoder.Decoder.html` & `CmonCrawl-1.0.2/docs/build/html/generated/cmoncrawl.aggregator.utils.ndjson_decoder.Decoder.html`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.0.1/docs/build/html/generated/cmoncrawl.aggregator.utils.ndjson_decoder.Decoder.raw_decode.html` & `CmonCrawl-1.0.2/docs/build/html/generated/cmoncrawl.aggregator.utils.ndjson_decoder.Decoder.raw_decode.html`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.0.1/docs/build/html/generated/cmoncrawl.aggregator.utils.ndjson_decoder.html` & `CmonCrawl-1.0.2/docs/build/html/generated/cmoncrawl.aggregator.utils.ndjson_decoder.html`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.0.1/docs/build/html/generated/cmoncrawl.common.html` & `CmonCrawl-1.0.2/docs/build/html/generated/cmoncrawl.common.html`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.0.1/docs/build/html/generated/cmoncrawl.common.loggers.html` & `CmonCrawl-1.0.2/docs/build/html/generated/cmoncrawl.common.loggers.html`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.0.1/docs/build/html/generated/cmoncrawl.common.types.DomainCrawl.__init__.html` & `CmonCrawl-1.0.2/docs/build/html/generated/cmoncrawl.common.types.DomainCrawl.__init__.html`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.0.1/docs/build/html/generated/cmoncrawl.common.types.DomainCrawl.html` & `CmonCrawl-1.0.2/docs/build/html/generated/cmoncrawl.common.types.DomainCrawl.html`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.0.1/docs/build/html/generated/cmoncrawl.common.types.DomainRecord.__init__.html` & `CmonCrawl-1.0.2/docs/build/html/generated/cmoncrawl.common.types.DomainRecord.__init__.html`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.0.1/docs/build/html/generated/cmoncrawl.common.types.DomainRecord.from_dict.html` & `CmonCrawl-1.0.2/docs/build/html/generated/cmoncrawl.common.types.DomainRecord.from_dict.html`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.0.1/docs/build/html/generated/cmoncrawl.common.types.DomainRecord.from_json.html` & `CmonCrawl-1.0.2/docs/build/html/generated/cmoncrawl.common.types.DomainRecord.from_json.html`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.0.1/docs/build/html/generated/cmoncrawl.common.types.DomainRecord.html` & `CmonCrawl-1.0.2/docs/build/html/generated/cmoncrawl.common.types.DomainRecord.html`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.0.1/docs/build/html/generated/cmoncrawl.common.types.DomainRecord.schema.html` & `CmonCrawl-1.0.2/docs/build/html/generated/cmoncrawl.common.types.DomainRecord.schema.html`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.0.1/docs/build/html/generated/cmoncrawl.common.types.DomainRecord.to_dict.html` & `CmonCrawl-1.0.2/docs/build/html/generated/cmoncrawl.common.types.DomainRecord.to_dict.html`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.0.1/docs/build/html/generated/cmoncrawl.common.types.DomainRecord.to_json.html` & `CmonCrawl-1.0.2/docs/build/html/generated/cmoncrawl.common.types.DomainRecord.to_json.html`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.0.1/docs/build/html/generated/cmoncrawl.common.types.ExtractConfig.__init__.html` & `CmonCrawl-1.0.2/docs/build/html/generated/cmoncrawl.common.types.ExtractConfig.__init__.html`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.0.1/docs/build/html/generated/cmoncrawl.common.types.ExtractConfig.from_dict.html` & `CmonCrawl-1.0.2/docs/build/html/generated/cmoncrawl.common.types.ExtractConfig.from_dict.html`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.0.1/docs/build/html/generated/cmoncrawl.common.types.ExtractConfig.from_json.html` & `CmonCrawl-1.0.2/docs/build/html/generated/cmoncrawl.common.types.ExtractConfig.from_json.html`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.0.1/docs/build/html/generated/cmoncrawl.common.types.ExtractConfig.html` & `CmonCrawl-1.0.2/docs/build/html/generated/cmoncrawl.common.types.ExtractConfig.html`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.0.1/docs/build/html/generated/cmoncrawl.common.types.ExtractConfig.schema.html` & `CmonCrawl-1.0.2/docs/build/html/generated/cmoncrawl.common.types.ExtractConfig.schema.html`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.0.1/docs/build/html/generated/cmoncrawl.common.types.ExtractConfig.to_dict.html` & `CmonCrawl-1.0.2/docs/build/html/generated/cmoncrawl.common.types.ExtractConfig.to_dict.html`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.0.1/docs/build/html/generated/cmoncrawl.common.types.ExtractConfig.to_json.html` & `CmonCrawl-1.0.2/docs/build/html/generated/cmoncrawl.common.types.ExtractConfig.to_json.html`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.0.1/docs/build/html/generated/cmoncrawl.common.types.ExtractorConfig.__init__.html` & `CmonCrawl-1.0.2/docs/build/html/generated/cmoncrawl.common.types.ExtractorConfig.__init__.html`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.0.1/docs/build/html/generated/cmoncrawl.common.types.ExtractorConfig.from_dict.html` & `CmonCrawl-1.0.2/docs/build/html/generated/cmoncrawl.common.types.ExtractorConfig.from_dict.html`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.0.1/docs/build/html/generated/cmoncrawl.common.types.ExtractorConfig.from_json.html` & `CmonCrawl-1.0.2/docs/build/html/generated/cmoncrawl.common.types.ExtractorConfig.from_json.html`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.0.1/docs/build/html/generated/cmoncrawl.common.types.ExtractorConfig.html` & `CmonCrawl-1.0.2/docs/build/html/generated/cmoncrawl.common.types.ExtractorConfig.html`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.0.1/docs/build/html/generated/cmoncrawl.common.types.ExtractorConfig.schema.html` & `CmonCrawl-1.0.2/docs/build/html/generated/cmoncrawl.common.types.ExtractorConfig.schema.html`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.0.1/docs/build/html/generated/cmoncrawl.common.types.ExtractorConfig.to_dict.html` & `CmonCrawl-1.0.2/docs/build/html/generated/cmoncrawl.common.types.ExtractorConfig.to_dict.html`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.0.1/docs/build/html/generated/cmoncrawl.common.types.ExtractorConfig.to_json.html` & `CmonCrawl-1.0.2/docs/build/html/generated/cmoncrawl.common.types.ExtractorConfig.to_json.html`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.0.1/docs/build/html/generated/cmoncrawl.common.types.PipeMetadata.__init__.html` & `CmonCrawl-1.0.2/docs/build/html/generated/cmoncrawl.common.types.PipeMetadata.__init__.html`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.0.1/docs/build/html/generated/cmoncrawl.common.types.PipeMetadata.html` & `CmonCrawl-1.0.2/docs/build/html/generated/cmoncrawl.common.types.PipeMetadata.html`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.0.1/docs/build/html/generated/cmoncrawl.common.types.RetrieveResponse.__init__.html` & `CmonCrawl-1.0.2/docs/build/html/generated/cmoncrawl.common.types.RetrieveResponse.__init__.html`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.0.1/docs/build/html/generated/cmoncrawl.common.types.RetrieveResponse.html` & `CmonCrawl-1.0.2/docs/build/html/generated/cmoncrawl.common.types.RetrieveResponse.html`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.0.1/docs/build/html/generated/cmoncrawl.common.types.RoutesConfig.__init__.html` & `CmonCrawl-1.0.2/docs/build/html/generated/cmoncrawl.common.types.RoutesConfig.__init__.html`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.0.1/docs/build/html/generated/cmoncrawl.common.types.RoutesConfig.from_dict.html` & `CmonCrawl-1.0.2/docs/build/html/generated/cmoncrawl.common.types.RoutesConfig.from_dict.html`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.0.1/docs/build/html/generated/cmoncrawl.common.types.RoutesConfig.from_json.html` & `CmonCrawl-1.0.2/docs/build/html/generated/cmoncrawl.common.types.RoutesConfig.from_json.html`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.0.1/docs/build/html/generated/cmoncrawl.common.types.RoutesConfig.html` & `CmonCrawl-1.0.2/docs/build/html/generated/cmoncrawl.common.types.RoutesConfig.html`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.0.1/docs/build/html/generated/cmoncrawl.common.types.RoutesConfig.schema.html` & `CmonCrawl-1.0.2/docs/build/html/generated/cmoncrawl.common.types.RoutesConfig.schema.html`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.0.1/docs/build/html/generated/cmoncrawl.common.types.RoutesConfig.to_dict.html` & `CmonCrawl-1.0.2/docs/build/html/generated/cmoncrawl.common.types.RoutesConfig.to_dict.html`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.0.1/docs/build/html/generated/cmoncrawl.common.types.RoutesConfig.to_json.html` & `CmonCrawl-1.0.2/docs/build/html/generated/cmoncrawl.common.types.RoutesConfig.to_json.html`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.0.1/docs/build/html/generated/cmoncrawl.common.types.html` & `CmonCrawl-1.0.2/docs/build/html/generated/cmoncrawl.common.types.html`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.0.1/docs/build/html/generated/cmoncrawl.html` & `CmonCrawl-1.0.2/docs/build/html/generated/cmoncrawl.html`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.0.1/docs/build/html/generated/cmoncrawl.processor.extraction.filters.html` & `CmonCrawl-1.0.2/docs/build/html/generated/cmoncrawl.processor.extraction.filters.html`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.0.1/docs/build/html/generated/cmoncrawl.processor.extraction.html` & `CmonCrawl-1.0.2/docs/build/html/generated/cmoncrawl.processor.extraction.html`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.0.1/docs/build/html/generated/cmoncrawl.processor.extraction.utils.html` & `CmonCrawl-1.0.2/docs/build/html/generated/cmoncrawl.processor.extraction.utils.html`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.0.1/docs/build/html/generated/cmoncrawl.processor.html` & `CmonCrawl-1.0.2/docs/build/html/generated/cmoncrawl.processor.html`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.0.1/docs/build/html/generated/cmoncrawl.processor.pipeline.downloader.AsyncDownloader.__init__.html` & `CmonCrawl-1.0.2/docs/build/html/generated/cmoncrawl.processor.pipeline.downloader.AsyncDownloader.__init__.html`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.0.1/docs/build/html/generated/cmoncrawl.processor.pipeline.downloader.AsyncDownloader.aclose.html` & `CmonCrawl-1.0.2/docs/build/html/generated/cmoncrawl.processor.pipeline.downloader.AsyncDownloader.aclose.html`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.0.1/docs/build/html/generated/cmoncrawl.processor.pipeline.downloader.AsyncDownloader.aopen.html` & `CmonCrawl-1.0.2/docs/build/html/generated/cmoncrawl.processor.pipeline.downloader.AsyncDownloader.aopen.html`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.0.1/docs/build/html/generated/cmoncrawl.processor.pipeline.downloader.AsyncDownloader.download.html` & `CmonCrawl-1.0.2/docs/build/html/generated/cmoncrawl.processor.pipeline.downloader.AsyncDownloader.download.html`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.0.1/docs/build/html/generated/cmoncrawl.processor.pipeline.downloader.AsyncDownloader.html` & `CmonCrawl-1.0.2/docs/build/html/generated/cmoncrawl.processor.pipeline.downloader.AsyncDownloader.html`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.0.1/docs/build/html/generated/cmoncrawl.processor.pipeline.downloader.AsyncDownloader.unwrap.html` & `CmonCrawl-1.0.2/docs/build/html/generated/cmoncrawl.processor.pipeline.downloader.AsyncDownloader.unwrap.html`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.0.1/docs/build/html/generated/cmoncrawl.processor.pipeline.downloader.DownloaderDummy.__init__.html` & `CmonCrawl-1.0.2/docs/build/html/generated/cmoncrawl.processor.pipeline.downloader.DownloaderDummy.__init__.html`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.0.1/docs/build/html/generated/cmoncrawl.processor.pipeline.downloader.DownloaderDummy.download.html` & `CmonCrawl-1.0.2/docs/build/html/generated/cmoncrawl.processor.pipeline.downloader.DownloaderDummy.download.html`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.0.1/docs/build/html/generated/cmoncrawl.processor.pipeline.downloader.DownloaderDummy.extract_url.html` & `CmonCrawl-1.0.2/docs/build/html/generated/cmoncrawl.processor.pipeline.downloader.DownloaderDummy.extract_url.html`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.0.1/docs/build/html/generated/cmoncrawl.processor.pipeline.downloader.DownloaderDummy.extract_year.html` & `CmonCrawl-1.0.2/docs/build/html/generated/cmoncrawl.processor.pipeline.downloader.DownloaderDummy.extract_year.html`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.0.1/docs/build/html/generated/cmoncrawl.processor.pipeline.downloader.DownloaderDummy.html` & `CmonCrawl-1.0.2/docs/build/html/generated/cmoncrawl.processor.pipeline.downloader.DownloaderDummy.html`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.0.1/docs/build/html/generated/cmoncrawl.processor.pipeline.downloader.DownloaderDummy.mine_metadata.html` & `CmonCrawl-1.0.2/docs/build/html/generated/cmoncrawl.processor.pipeline.downloader.DownloaderDummy.mine_metadata.html`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.0.1/docs/build/html/generated/cmoncrawl.processor.pipeline.downloader.IDownloader.__init__.html` & `CmonCrawl-1.0.2/docs/build/html/generated/cmoncrawl.processor.pipeline.downloader.IDownloader.__init__.html`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.0.1/docs/build/html/generated/cmoncrawl.processor.pipeline.downloader.IDownloader.download.html` & `CmonCrawl-1.0.2/docs/build/html/generated/cmoncrawl.processor.pipeline.downloader.IDownloader.download.html`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.0.1/docs/build/html/generated/cmoncrawl.processor.pipeline.downloader.IDownloader.html` & `CmonCrawl-1.0.2/docs/build/html/generated/cmoncrawl.processor.pipeline.downloader.IDownloader.html`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.0.1/docs/build/html/generated/cmoncrawl.processor.pipeline.downloader.html` & `CmonCrawl-1.0.2/docs/build/html/generated/cmoncrawl.processor.pipeline.downloader.html`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.0.1/docs/build/html/generated/cmoncrawl.processor.pipeline.extractor.BaseExtractor.__init__.html` & `CmonCrawl-1.0.2/docs/build/html/generated/cmoncrawl.processor.pipeline.extractor.BaseExtractor.__init__.html`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.0.1/docs/build/html/generated/cmoncrawl.processor.pipeline.extractor.BaseExtractor.extract.html` & `CmonCrawl-1.0.2/docs/build/html/generated/cmoncrawl.processor.pipeline.extractor.BaseExtractor.extract.html`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.0.1/docs/build/html/generated/cmoncrawl.processor.pipeline.extractor.BaseExtractor.extract_soup.html` & `CmonCrawl-1.0.2/docs/build/html/generated/cmoncrawl.processor.pipeline.extractor.BaseExtractor.extract_soup.html`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.0.1/docs/build/html/generated/cmoncrawl.processor.pipeline.extractor.BaseExtractor.filter_raw.html` & `CmonCrawl-1.0.2/docs/build/html/generated/cmoncrawl.processor.pipeline.extractor.BaseExtractor.filter_raw.html`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.0.1/docs/build/html/generated/cmoncrawl.processor.pipeline.extractor.BaseExtractor.filter_soup.html` & `CmonCrawl-1.0.2/docs/build/html/generated/cmoncrawl.processor.pipeline.extractor.BaseExtractor.filter_soup.html`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.0.1/docs/build/html/generated/cmoncrawl.processor.pipeline.extractor.BaseExtractor.html` & `CmonCrawl-1.0.2/docs/build/html/generated/cmoncrawl.processor.pipeline.extractor.BaseExtractor.html`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.0.1/docs/build/html/generated/cmoncrawl.processor.pipeline.extractor.BaseExtractor.preprocess.html` & `CmonCrawl-1.0.2/docs/build/html/generated/cmoncrawl.processor.pipeline.extractor.BaseExtractor.preprocess.html`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.0.1/docs/build/html/generated/cmoncrawl.processor.pipeline.extractor.DomainRecordExtractor.__init__.html` & `CmonCrawl-1.0.2/docs/build/html/generated/cmoncrawl.processor.pipeline.extractor.DomainRecordExtractor.__init__.html`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.0.1/docs/build/html/generated/cmoncrawl.processor.pipeline.extractor.DomainRecordExtractor.extract.html` & `CmonCrawl-1.0.2/docs/build/html/generated/cmoncrawl.processor.pipeline.extractor.DomainRecordExtractor.extract.html`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.0.1/docs/build/html/generated/cmoncrawl.processor.pipeline.extractor.DomainRecordExtractor.extract_soup.html` & `CmonCrawl-1.0.2/docs/build/html/generated/cmoncrawl.processor.pipeline.extractor.DomainRecordExtractor.extract_soup.html`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.0.1/docs/build/html/generated/cmoncrawl.processor.pipeline.extractor.DomainRecordExtractor.filter_raw.html` & `CmonCrawl-1.0.2/docs/build/html/generated/cmoncrawl.processor.pipeline.extractor.DomainRecordExtractor.filter_raw.html`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.0.1/docs/build/html/generated/cmoncrawl.processor.pipeline.extractor.DomainRecordExtractor.filter_soup.html` & `CmonCrawl-1.0.2/docs/build/html/generated/cmoncrawl.processor.pipeline.extractor.DomainRecordExtractor.filter_soup.html`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.0.1/docs/build/html/generated/cmoncrawl.processor.pipeline.extractor.DomainRecordExtractor.html` & `CmonCrawl-1.0.2/docs/build/html/generated/cmoncrawl.processor.pipeline.extractor.DomainRecordExtractor.html`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.0.1/docs/build/html/generated/cmoncrawl.processor.pipeline.extractor.DomainRecordExtractor.preprocess.html` & `CmonCrawl-1.0.2/docs/build/html/generated/cmoncrawl.processor.pipeline.extractor.DomainRecordExtractor.preprocess.html`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.0.1/docs/build/html/generated/cmoncrawl.processor.pipeline.extractor.HTMLExtractor.__init__.html` & `CmonCrawl-1.0.2/docs/build/html/generated/cmoncrawl.processor.pipeline.extractor.HTMLExtractor.__init__.html`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.0.1/docs/build/html/generated/cmoncrawl.processor.pipeline.extractor.HTMLExtractor.extract.html` & `CmonCrawl-1.0.2/docs/build/html/generated/cmoncrawl.processor.pipeline.extractor.HTMLExtractor.extract.html`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.0.1/docs/build/html/generated/cmoncrawl.processor.pipeline.extractor.HTMLExtractor.extract_soup.html` & `CmonCrawl-1.0.2/docs/build/html/generated/cmoncrawl.processor.pipeline.extractor.HTMLExtractor.extract_soup.html`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.0.1/docs/build/html/generated/cmoncrawl.processor.pipeline.extractor.HTMLExtractor.filter_raw.html` & `CmonCrawl-1.0.2/docs/build/html/generated/cmoncrawl.processor.pipeline.extractor.HTMLExtractor.filter_raw.html`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.0.1/docs/build/html/generated/cmoncrawl.processor.pipeline.extractor.HTMLExtractor.filter_soup.html` & `CmonCrawl-1.0.2/docs/build/html/generated/cmoncrawl.processor.pipeline.extractor.HTMLExtractor.filter_soup.html`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.0.1/docs/build/html/generated/cmoncrawl.processor.pipeline.extractor.HTMLExtractor.html` & `CmonCrawl-1.0.2/docs/build/html/generated/cmoncrawl.processor.pipeline.extractor.HTMLExtractor.html`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.0.1/docs/build/html/generated/cmoncrawl.processor.pipeline.extractor.HTMLExtractor.preprocess.html` & `CmonCrawl-1.0.2/docs/build/html/generated/cmoncrawl.processor.pipeline.extractor.HTMLExtractor.preprocess.html`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.0.1/docs/build/html/generated/cmoncrawl.processor.pipeline.extractor.IExtractor.__init__.html` & `CmonCrawl-1.0.2/docs/build/html/generated/cmoncrawl.processor.pipeline.extractor.IExtractor.__init__.html`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.0.1/docs/build/html/generated/cmoncrawl.processor.pipeline.extractor.IExtractor.extract.html` & `CmonCrawl-1.0.2/docs/build/html/generated/cmoncrawl.processor.pipeline.extractor.IExtractor.extract.html`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.0.1/docs/build/html/generated/cmoncrawl.processor.pipeline.extractor.IExtractor.html` & `CmonCrawl-1.0.2/docs/build/html/generated/cmoncrawl.processor.pipeline.extractor.IExtractor.html`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.0.1/docs/build/html/generated/cmoncrawl.processor.pipeline.extractor.html` & `CmonCrawl-1.0.2/docs/build/html/generated/cmoncrawl.processor.pipeline.extractor.html`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.0.1/docs/build/html/generated/cmoncrawl.processor.pipeline.html` & `CmonCrawl-1.0.2/docs/build/html/generated/cmoncrawl.processor.pipeline.html`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.0.1/docs/build/html/generated/cmoncrawl.processor.pipeline.pipeline.ProcessorPipeline.__init__.html` & `CmonCrawl-1.0.2/docs/build/html/generated/cmoncrawl.processor.pipeline.pipeline.ProcessorPipeline.__init__.html`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.0.1/docs/build/html/generated/cmoncrawl.processor.pipeline.pipeline.ProcessorPipeline.html` & `CmonCrawl-1.0.2/docs/build/html/generated/cmoncrawl.processor.pipeline.pipeline.ProcessorPipeline.html`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.0.1/docs/build/html/generated/cmoncrawl.processor.pipeline.pipeline.ProcessorPipeline.process_domain_record.html` & `CmonCrawl-1.0.2/docs/build/html/generated/cmoncrawl.processor.pipeline.pipeline.ProcessorPipeline.process_domain_record.html`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.0.1/docs/build/html/generated/cmoncrawl.processor.pipeline.pipeline.html` & `CmonCrawl-1.0.2/docs/build/html/generated/cmoncrawl.processor.pipeline.pipeline.html`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.0.1/docs/build/html/generated/cmoncrawl.processor.pipeline.router.IRouter.__init__.html` & `CmonCrawl-1.0.2/docs/build/html/generated/cmoncrawl.processor.pipeline.router.IRouter.__init__.html`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.0.1/docs/build/html/generated/cmoncrawl.processor.pipeline.router.IRouter.html` & `CmonCrawl-1.0.2/docs/build/html/generated/cmoncrawl.processor.pipeline.router.IRouter.html`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.0.1/docs/build/html/generated/cmoncrawl.processor.pipeline.router.IRouter.route.html` & `CmonCrawl-1.0.2/docs/build/html/generated/cmoncrawl.processor.pipeline.router.IRouter.route.html`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.0.1/docs/build/html/generated/cmoncrawl.processor.pipeline.router.Route.__init__.html` & `CmonCrawl-1.0.2/docs/build/html/generated/cmoncrawl.processor.pipeline.router.Route.__init__.html`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.0.1/docs/build/html/generated/cmoncrawl.processor.pipeline.router.Route.html` & `CmonCrawl-1.0.2/docs/build/html/generated/cmoncrawl.processor.pipeline.router.Route.html`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.0.1/docs/build/html/generated/cmoncrawl.processor.pipeline.router.Router.__init__.html` & `CmonCrawl-1.0.2/docs/build/html/generated/cmoncrawl.processor.pipeline.router.Router.__init__.html`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.0.1/docs/build/html/generated/cmoncrawl.processor.pipeline.router.Router.html` & `CmonCrawl-1.0.2/docs/build/html/generated/cmoncrawl.processor.pipeline.router.Router.html`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.0.1/docs/build/html/generated/cmoncrawl.processor.pipeline.router.Router.load_extractor.html` & `CmonCrawl-1.0.2/docs/build/html/generated/cmoncrawl.processor.pipeline.router.Router.load_extractor.html`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.0.1/docs/build/html/generated/cmoncrawl.processor.pipeline.router.Router.load_module.html` & `CmonCrawl-1.0.2/docs/build/html/generated/cmoncrawl.processor.pipeline.router.Router.load_module.html`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.0.1/docs/build/html/generated/cmoncrawl.processor.pipeline.router.Router.load_module_as_extractor.html` & `CmonCrawl-1.0.2/docs/build/html/generated/cmoncrawl.processor.pipeline.router.Router.load_module_as_extractor.html`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.0.1/docs/build/html/generated/cmoncrawl.processor.pipeline.router.Router.load_modules.html` & `CmonCrawl-1.0.2/docs/build/html/generated/cmoncrawl.processor.pipeline.router.Router.load_modules.html`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.0.1/docs/build/html/generated/cmoncrawl.processor.pipeline.router.Router.register_route.html` & `CmonCrawl-1.0.2/docs/build/html/generated/cmoncrawl.processor.pipeline.router.Router.register_route.html`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.0.1/docs/build/html/generated/cmoncrawl.processor.pipeline.router.Router.register_routes.html` & `CmonCrawl-1.0.2/docs/build/html/generated/cmoncrawl.processor.pipeline.router.Router.register_routes.html`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.0.1/docs/build/html/generated/cmoncrawl.processor.pipeline.router.Router.route.html` & `CmonCrawl-1.0.2/docs/build/html/generated/cmoncrawl.processor.pipeline.router.Router.route.html`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.0.1/docs/build/html/generated/cmoncrawl.processor.pipeline.router.html` & `CmonCrawl-1.0.2/docs/build/html/generated/cmoncrawl.processor.pipeline.router.html`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.0.1/docs/build/html/generated/cmoncrawl.processor.pipeline.streamer.BaseStreamerFile.__init__.html` & `CmonCrawl-1.0.2/docs/build/html/generated/cmoncrawl.processor.pipeline.streamer.BaseStreamerFile.__init__.html`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.0.1/docs/build/html/generated/cmoncrawl.processor.pipeline.streamer.BaseStreamerFile.clean_up.html` & `CmonCrawl-1.0.2/docs/build/html/generated/cmoncrawl.processor.pipeline.streamer.BaseStreamerFile.clean_up.html`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.0.1/docs/build/html/generated/cmoncrawl.processor.pipeline.streamer.BaseStreamerFile.get_file_name.html` & `CmonCrawl-1.0.2/docs/build/html/generated/cmoncrawl.processor.pipeline.streamer.BaseStreamerFile.get_file_name.html`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.0.1/docs/build/html/generated/cmoncrawl.processor.pipeline.streamer.BaseStreamerFile.html` & `CmonCrawl-1.0.2/docs/build/html/generated/cmoncrawl.processor.pipeline.streamer.BaseStreamerFile.html`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.0.1/docs/build/html/generated/cmoncrawl.processor.pipeline.streamer.BaseStreamerFile.metadata_to_string.html` & `CmonCrawl-1.0.2/docs/build/html/generated/cmoncrawl.processor.pipeline.streamer.BaseStreamerFile.metadata_to_string.html`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.0.1/docs/build/html/generated/cmoncrawl.processor.pipeline.streamer.BaseStreamerFile.stream.html` & `CmonCrawl-1.0.2/docs/build/html/generated/cmoncrawl.processor.pipeline.streamer.BaseStreamerFile.stream.html`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.0.1/docs/build/html/generated/cmoncrawl.processor.pipeline.streamer.IStreamer.__init__.html` & `CmonCrawl-1.0.2/docs/build/html/generated/cmoncrawl.processor.pipeline.streamer.IStreamer.__init__.html`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.0.1/docs/build/html/generated/cmoncrawl.processor.pipeline.streamer.IStreamer.clean_up.html` & `CmonCrawl-1.0.2/docs/build/html/generated/cmoncrawl.processor.pipeline.streamer.IStreamer.clean_up.html`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.0.1/docs/build/html/generated/cmoncrawl.processor.pipeline.streamer.IStreamer.html` & `CmonCrawl-1.0.2/docs/build/html/generated/cmoncrawl.processor.pipeline.streamer.IStreamer.html`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.0.1/docs/build/html/generated/cmoncrawl.processor.pipeline.streamer.IStreamer.stream.html` & `CmonCrawl-1.0.2/docs/build/html/generated/cmoncrawl.processor.pipeline.streamer.IStreamer.stream.html`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.0.1/docs/build/html/generated/cmoncrawl.processor.pipeline.streamer.StreamerDummy.__init__.html` & `CmonCrawl-1.0.2/docs/build/html/generated/cmoncrawl.processor.pipeline.streamer.StreamerDummy.__init__.html`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.0.1/docs/build/html/generated/cmoncrawl.processor.pipeline.streamer.StreamerDummy.clean_up.html` & `CmonCrawl-1.0.2/docs/build/html/generated/cmoncrawl.processor.pipeline.streamer.StreamerDummy.clean_up.html`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.0.1/docs/build/html/generated/cmoncrawl.processor.pipeline.streamer.StreamerDummy.html` & `CmonCrawl-1.0.2/docs/build/html/generated/cmoncrawl.processor.pipeline.streamer.StreamerDummy.html`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.0.1/docs/build/html/generated/cmoncrawl.processor.pipeline.streamer.StreamerDummy.stream.html` & `CmonCrawl-1.0.2/docs/build/html/generated/cmoncrawl.processor.pipeline.streamer.StreamerDummy.stream.html`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.0.1/docs/build/html/generated/cmoncrawl.processor.pipeline.streamer.StreamerFileHTML.__init__.html` & `CmonCrawl-1.0.2/docs/build/html/generated/cmoncrawl.processor.pipeline.streamer.StreamerFileHTML.__init__.html`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.0.1/docs/build/html/generated/cmoncrawl.processor.pipeline.streamer.StreamerFileHTML.clean_up.html` & `CmonCrawl-1.0.2/docs/build/html/generated/cmoncrawl.processor.pipeline.streamer.StreamerFileHTML.clean_up.html`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.0.1/docs/build/html/generated/cmoncrawl.processor.pipeline.streamer.StreamerFileHTML.get_file_name.html` & `CmonCrawl-1.0.2/docs/build/html/generated/cmoncrawl.processor.pipeline.streamer.StreamerFileHTML.get_file_name.html`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.0.1/docs/build/html/generated/cmoncrawl.processor.pipeline.streamer.StreamerFileHTML.html` & `CmonCrawl-1.0.2/docs/build/html/generated/cmoncrawl.processor.pipeline.streamer.StreamerFileHTML.html`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.0.1/docs/build/html/generated/cmoncrawl.processor.pipeline.streamer.StreamerFileHTML.metadata_to_string.html` & `CmonCrawl-1.0.2/docs/build/html/generated/cmoncrawl.processor.pipeline.streamer.StreamerFileHTML.metadata_to_string.html`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.0.1/docs/build/html/generated/cmoncrawl.processor.pipeline.streamer.StreamerFileHTML.stream.html` & `CmonCrawl-1.0.2/docs/build/html/generated/cmoncrawl.processor.pipeline.streamer.StreamerFileHTML.stream.html`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.0.1/docs/build/html/generated/cmoncrawl.processor.pipeline.streamer.StreamerFileJSON.__init__.html` & `CmonCrawl-1.0.2/docs/build/html/generated/cmoncrawl.processor.pipeline.streamer.StreamerFileJSON.__init__.html`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.0.1/docs/build/html/generated/cmoncrawl.processor.pipeline.streamer.StreamerFileJSON.clean_up.html` & `CmonCrawl-1.0.2/docs/build/html/generated/cmoncrawl.processor.pipeline.streamer.StreamerFileJSON.clean_up.html`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.0.1/docs/build/html/generated/cmoncrawl.processor.pipeline.streamer.StreamerFileJSON.get_file_name.html` & `CmonCrawl-1.0.2/docs/build/html/generated/cmoncrawl.processor.pipeline.streamer.StreamerFileJSON.get_file_name.html`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.0.1/docs/build/html/generated/cmoncrawl.processor.pipeline.streamer.StreamerFileJSON.html` & `CmonCrawl-1.0.2/docs/build/html/generated/cmoncrawl.processor.pipeline.streamer.StreamerFileJSON.html`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.0.1/docs/build/html/generated/cmoncrawl.processor.pipeline.streamer.StreamerFileJSON.metadata_to_string.html` & `CmonCrawl-1.0.2/docs/build/html/generated/cmoncrawl.processor.pipeline.streamer.StreamerFileJSON.metadata_to_string.html`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.0.1/docs/build/html/generated/cmoncrawl.processor.pipeline.streamer.StreamerFileJSON.stream.html` & `CmonCrawl-1.0.2/docs/build/html/generated/cmoncrawl.processor.pipeline.streamer.StreamerFileJSON.stream.html`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.0.1/docs/build/html/generated/cmoncrawl.processor.pipeline.streamer.html` & `CmonCrawl-1.0.2/docs/build/html/generated/cmoncrawl.processor.pipeline.streamer.html`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.0.1/docs/build/html/genindex.html` & `CmonCrawl-1.0.2/docs/build/html/genindex.html`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.0.1/docs/build/html/index.html` & `CmonCrawl-1.0.2/docs/build/html/index.html`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.0.1/docs/build/html/misc/domain_record.html` & `CmonCrawl-1.0.2/docs/build/html/misc/domain_record.html`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.0.1/docs/build/html/misc/index.html` & `CmonCrawl-1.0.2/docs/build/html/misc/index.html`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.0.1/docs/build/html/objects.inv` & `CmonCrawl-1.0.2/docs/build/html/objects.inv`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.0.1/docs/build/html/prog_guide/index.html` & `CmonCrawl-1.0.2/docs/build/html/prog_guide/index.html`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.0.1/docs/build/html/prog_guide/overview.html` & `CmonCrawl-1.0.2/docs/build/html/prog_guide/overview.html`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.0.1/docs/build/html/prog_guide/pip.html` & `CmonCrawl-1.0.2/docs/build/html/prog_guide/pip.html`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.0.1/docs/build/html/py-modindex.html` & `CmonCrawl-1.0.2/docs/build/html/py-modindex.html`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.0.1/docs/build/html/search.html` & `CmonCrawl-1.0.2/docs/build/html/search.html`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.0.1/docs/build/html/searchindex.js` & `CmonCrawl-1.0.2/docs/build/html/searchindex.js`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.0.1/docs/build/html/usage.html` & `CmonCrawl-1.0.2/docs/build/html/usage.html`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.0.1/docs/make.bat` & `CmonCrawl-1.0.2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.0.1/docs/source/cli/cli.rst` & `CmonCrawl-1.0.2/docs/source/cli/cli.rst`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.0.1/docs/source/cli/download.rst` & `CmonCrawl-1.0.2/docs/source/cli/download.rst`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.0.1/docs/source/cli/extract.rst` & `CmonCrawl-1.0.2/docs/source/cli/extract.rst`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.0.1/docs/source/conf.py` & `CmonCrawl-1.0.2/docs/source/conf.py`

 * *Files 0% similar despite different names*

```diff
@@ -66,9 +66,7 @@
 # -- Options for HTML output -------------------------------------------------
 
 # The theme to use for HTML and HTML Help pages.  See the documentation for
 # a list of builtin themes.
 #
 html_theme = "sphinx_book_theme"
 autosummary_generate_overwrite = False
-
-
```

### Comparing `CmonCrawl-1.0.1/docs/source/extraction/config_file.rst` & `CmonCrawl-1.0.2/docs/source/extraction/config_file.rst`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.0.1/docs/source/extraction/creating_extractor.rst` & `CmonCrawl-1.0.2/docs/source/extraction/creating_extractor.rst`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.0.1/docs/source/extraction/utils.rst` & `CmonCrawl-1.0.2/docs/source/extraction/utils.rst`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.0.1/docs/source/generated/cmoncrawl.aggregator.index_query.IndexAggregator.rst` & `CmonCrawl-1.0.2/docs/source/generated/cmoncrawl.aggregator.index_query.IndexAggregator.rst`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.0.1/docs/source/generated/cmoncrawl.common.types.DomainRecord.rst` & `CmonCrawl-1.0.2/docs/source/generated/cmoncrawl.common.types.DomainRecord.rst`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.0.1/docs/source/generated/cmoncrawl.common.types.ExtractConfig.rst` & `CmonCrawl-1.0.2/docs/source/generated/cmoncrawl.common.types.ExtractConfig.rst`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.0.1/docs/source/generated/cmoncrawl.common.types.ExtractorConfig.rst` & `CmonCrawl-1.0.2/docs/source/generated/cmoncrawl.common.types.ExtractorConfig.rst`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.0.1/docs/source/generated/cmoncrawl.common.types.PipeMetadata.rst` & `CmonCrawl-1.0.2/docs/source/generated/cmoncrawl.common.types.PipeMetadata.rst`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.0.1/docs/source/generated/cmoncrawl.common.types.RoutesConfig.rst` & `CmonCrawl-1.0.2/docs/source/generated/cmoncrawl.common.types.RoutesConfig.rst`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.0.1/docs/source/generated/cmoncrawl.processor.pipeline.extractor.DomainRecordExtractor.rst` & `CmonCrawl-1.0.2/docs/source/generated/cmoncrawl.processor.pipeline.extractor.DomainRecordExtractor.rst`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.0.1/docs/source/index.rst` & `CmonCrawl-1.0.2/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.0.1/docs/source/misc/domain_record.rst` & `CmonCrawl-1.0.2/docs/source/misc/domain_record.rst`

 * *Files 0% similar despite different names*

```diff
@@ -46,11 +46,10 @@
 Each such json must be on a separate line in a file.
 You don't have to provide all the fields, only ```url``, ```filename```,
 ```offset``` and ```length``` are required.
 The Athena SQL keys are:
 ```u.url, cc.warc_filename, cc.warc_record_offset, cc.warc_record_length, cc.content_digest, cc.fetch_time```
 
 
-
 The ```additional_info``` field is optional and can contain any additional
 information. It will be added to extracted fields as is. It's usefull
 when you for example want to add to which set the url belongs to.
```

### Comparing `CmonCrawl-1.0.1/docs/source/prog_guide/overview.rst` & `CmonCrawl-1.0.2/docs/source/prog_guide/overview.rst`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.0.1/docs/source/prog_guide/pip.rst` & `CmonCrawl-1.0.2/docs/source/prog_guide/pip.rst`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.0.1/docs/source/usage.rst` & `CmonCrawl-1.0.2/docs/source/usage.rst`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.0.1/examples/extractor_tutorial/Extractors/bbc_extractor.py` & `CmonCrawl-1.0.2/examples/extractor_tutorial/Extractors/bbc_extractor.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,40 +1,45 @@
 from datetime import datetime
 from Processor.App.ArticleUtils.article_extractor import ArticleExtractor
-from Processor.App.ArticleUtils.article_utils import headline_transform, get_text_transform, text_unifications_transform
-    
-REQUIRED_FIELDS = {
-    "title": False,
-    "content": True
-}
+from Processor.App.ArticleUtils.article_utils import (
+    headline_transform,
+    get_text_transform,
+    text_unifications_transform,
+)
+
+REQUIRED_FIELDS = {"title": False, "content": True}
+
 
 def content_transform(soup):
     return [p.text for p in soup.find_all("p", recursive=True)]
 
 
 class BBCExtractor(ArticleExtractor):
-    SINCE = datetime(2021, 1 , 20)
+    SINCE = datetime(2021, 1, 20)
     TO = datetime(2021, 3, 20)
 
     def __init__(self):
         super().__init__(
             header_css_dict={},
             header_extract_dict={},
             article_css_dict={
                 "title": "h1#content",
                 "content": "main[role=main]",
             },
             # Here we define how to transform the content of the tag into a string.
-            article_extract_dict= {
+            article_extract_dict={
                 "title": [get_text_transform, headline_transform],
-                "content": [content_transform, text_unifications_transform, lambda lines : "\n".join(lines)]
+                "content": [
+                    content_transform,
+                    text_unifications_transform,
+                    lambda lines: "\n".join(lines),
+                ],
             },
-
-
             # Here we define how to bind a tag that containt all fields we will use in article_css_dict
             # If you don't know just use body
             article_css_selector="body",
             required_fields=REQUIRED_FIELDS,
-            non_empty = True
+            non_empty=True,
         )
 
-extractor = BBCExtractor()
+
+extractor = BBCExtractor()
```

### Comparing `CmonCrawl-1.0.1/pyproject.toml` & `CmonCrawl-1.0.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.0.1/tests/aggregator_tests.py` & `CmonCrawl-1.0.2/tests/aggregator_tests.py`

 * *Files 5% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 class TestIndexerAsync(unittest.IsolatedAsyncioTestCase):
     async def asyncSetUp(self) -> None:
         self.CC_SERVERS = ["https://index.commoncrawl.org/CC-MAIN-2022-05-index"]
         self.di = await IndexAggregator(
             ["idnes.cz"],
             cc_servers=self.CC_SERVERS,
-            max_retry=50,
+            max_retry=100,
             sleep_step=10,
             prefetch_size=1,
             match_type=MatchType.DOMAIN,
         ).aopen()
         self.client = self.di.client
 
     async def asyncTearDown(self) -> None:
@@ -55,33 +55,26 @@
         indexes = indexes[
             : indexes.index("https://index.commoncrawl.org/CC-MAIN-2022-27-index") + 1
         ]
         self.assertEqual(len(indexes), 89)
 
     async def test_since(self):
         # That is crawl date not published date
-        records: List[DomainRecord] = []
         self.di.since = datetime(2022, 1, 21)
+        self.di.limit = 5
 
         async for record in self.di:
             self.assertGreaterEqual(record.timestamp, self.di.since)
-            records.append(record)
-
-        self.assertEqual(len(records), 131149)
 
     async def test_to(self):
         # That is crawl date not published date
-        records: List[DomainRecord] = []
         self.di.to = datetime(2022, 1, 21)
 
         async for record in self.di:
             self.assertLessEqual(record.timestamp, self.di.to)
-            records.append(record)
-
-        self.assertEqual(len(records), 63244)
 
     async def test_limit(self):
         records: List[DomainRecord] = []
         self.di.limit = 10
         async for record in self.di:
             records.append(record)
 
@@ -94,14 +87,15 @@
             [],
             since=datetime(2022, 5, 1),
             to=datetime(2022, 1, 10),
             limit=None,
             max_retry=10,
             sleep_step=4,
             prefetch_size=2,
+            match_type=MatchType.DOMAIN,
         )
         # Generates only for 2020
         q = iterator.init_crawls_queue(
             self.di.domains,
             self.di.cc_servers
             + [
                 "https://index.commoncrawl.org/CC-MAIN-2021-43-index",
```

### Comparing `CmonCrawl-1.0.1/tests/end_to_end_tests.py` & `CmonCrawl-1.0.2/tests/end_to_end_tests.py`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.0.1/tests/processor_tests.py` & `CmonCrawl-1.0.2/tests/processor_tests.py`

 * *Files 24% similar despite different names*

```diff
@@ -3,17 +3,19 @@
 
 import asyncio
 import unittest
 import os
 import re
 from datetime import datetime
 from cmoncrawl.processor.pipeline.downloader import AsyncDownloader
+from cmoncrawl.processor.pipeline.extractor import BaseExtractor, HTMLExtractor
 from cmoncrawl.processor.pipeline.streamer import StreamerFileJSON, StreamerFileHTML
 from cmoncrawl.processor.pipeline.router import Router
 from cmoncrawl.common.types import DomainRecord, PipeMetadata
+from bs4 import BeautifulSoup
 
 
 class DownloaderTests(unittest.IsolatedAsyncioTestCase):
     async def asyncSetUp(self) -> None:
         self.downloader: AsyncDownloader = await AsyncDownloader(
             digest_verification=True
         ).aopen()
@@ -61,14 +63,61 @@
             pass
 
         c3 = self.router.route("seznam.cz", datetime.today(), metadata)
         self.assertEqual(c1, self.router.modules["AAA"])
         self.assertEqual(c3, self.router.modules["BBB"])
 
 
+class ExtradctorTests(unittest.TestCase):
+    def test_encoding(self):
+        def create_html():
+            return "<html><body><p>test</p></body></html>".encode("latin-1").decode(
+                "latin-1"
+            )
+
+        def create_non_utf8():
+            return bytes([0x81, 0x81, 0x82, 0x83]).decode("latin-1")
+
+        def create_metadata():
+            return PipeMetadata(
+                domain_record=DomainRecord(
+                    filename="",
+                    offset=0,
+                    length=0,
+                    url="",
+                ),
+            )
+
+        extractor = HTMLExtractor()  # type: ignore
+        metadata = create_metadata()
+        extractor.encode(create_html(), metadata)
+        # By default utf-8 is tried
+        self.assertEqual(metadata.encoding, "utf-8")
+
+        # Can be overwriten by setting encoding
+        # Revert back to default
+        metadata = create_metadata()
+        # Set expected encoding
+        metadata.domain_record.encoding = "latin-1"
+        extractor.encode(create_html(), metadata)
+        self.assertEqual(metadata.encoding, "latin-1")
+
+        # By default if everything fails, the default(latin-1) is used
+        metadata = create_metadata()
+        extractor.encode(create_non_utf8(), metadata)
+        self.assertEqual(metadata.encoding, "latin-1")
+
+        # But we can overwrite it by setting raise_on_error
+        metadata = create_metadata()
+        extractor.raise_on_encoding = True
+        metadata.encoding = "latin-1"
+        with self.assertRaises(ValueError):
+            extractor.encode(create_non_utf8(), metadata)
+
+
 class OutStremaerTests(unittest.IsolatedAsyncioTestCase):
     def setUp(self) -> None:
         self.html_folder = Path(__file__).parent / "test_html"
         self.json_folder = Path(__file__).parent / "test_json"
         self.outstreamer_json = StreamerFileJSON(self.json_folder, 100, 100)
         self.outstreamer_html = StreamerFileHTML(self.html_folder, 5)
         self.metadata = PipeMetadata(DomainRecord("", "", 0, 0))
@@ -101,15 +150,15 @@
             asyncio.create_task(self.outstreamer_json.stream(dict(), self.metadata))
             for _ in range(5)
         ]
         await asyncio.gather(*writes)
         size = len(os.listdir(self.json_folder))
         self.assertEqual(size, 1)
         num_lines = sum(
-            1 for _ in open(self.json_folder / "directory_0" / "0_file.json", "r")
+            1 for _ in open(self.json_folder / "directory_0" / "0_file.jsonl", "r")
         )
         self.assertEqual(num_lines, 5)
 
     async def test_check_content_json(self):
         writes = [
             asyncio.create_task(self.outstreamer_json.stream({"num": n}, self.metadata))
             for n in range(2)
```

### Comparing `CmonCrawl-1.0.1/tests/test_extract/files/file.html` & `CmonCrawl-1.0.2/tests/test_extract/files/file.html`

 * *Files identical despite different names*

### Comparing `CmonCrawl-1.0.1/tests/test_extract/files/file.jsonl` & `CmonCrawl-1.0.2/tests/test_extract/files/file.jsonl`

 * *Files identical despite different names*

