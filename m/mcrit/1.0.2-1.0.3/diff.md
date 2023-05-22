# Comparing `tmp/mcrit-1.0.2.tar.gz` & `tmp/mcrit-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mcrit-1.0.2.tar", last modified: Mon May 22 12:13:28 2023, max compression
+gzip compressed data, was "mcrit-1.0.3.tar", last modified: Mon May 22 12:32:44 2023, max compression
```

## Comparing `mcrit-1.0.2.tar` & `mcrit-1.0.3.tar`

### file list

```diff
@@ -1,84 +1,84 @@
-drwxrwxr-x   0 analyst   (1000) analyst   (1000)        0 2023-05-22 12:13:28.331190 mcrit-1.0.2/
--rw-rw-r--   0 analyst   (1000) analyst   (1000)    35149 2022-05-05 12:52:43.000000 mcrit-1.0.2/LICENSE
--rw-rw-r--   0 analyst   (1000) analyst   (1000)    11397 2023-05-22 12:13:28.331190 mcrit-1.0.2/PKG-INFO
--rw-rw-r--   0 analyst   (1000) analyst   (1000)    10645 2023-05-22 12:12:35.000000 mcrit-1.0.2/README.md
-drwxrwxr-x   0 analyst   (1000) analyst   (1000)        0 2023-05-22 12:13:28.327190 mcrit-1.0.2/mcrit/
--rw-rw-r--   0 analyst   (1000) analyst   (1000)    21415 2022-12-13 15:03:46.000000 mcrit-1.0.2/mcrit/Worker.py
--rw-rw-r--   0 analyst   (1000) analyst   (1000)        0 2022-02-03 10:05:12.000000 mcrit-1.0.2/mcrit/__init__.py
--rw-rw-r--   0 analyst   (1000) analyst   (1000)     1838 2023-03-16 12:54:37.000000 mcrit-1.0.2/mcrit/__main__.py
-drwxrwxr-x   0 analyst   (1000) analyst   (1000)        0 2023-05-22 12:13:28.327190 mcrit-1.0.2/mcrit/client/
--rw-rw-r--   0 analyst   (1000) analyst   (1000)    28489 2023-05-22 08:41:11.000000 mcrit-1.0.2/mcrit/client/McritClient.py
--rw-rw-r--   0 analyst   (1000) analyst   (1000)    18233 2023-05-22 12:10:34.000000 mcrit-1.0.2/mcrit/client/McritConsole.py
--rw-rw-r--   0 analyst   (1000) analyst   (1000)        0 2022-02-03 10:05:12.000000 mcrit-1.0.2/mcrit/client/__init__.py
-drwxrwxr-x   0 analyst   (1000) analyst   (1000)        0 2023-05-22 12:13:28.327190 mcrit-1.0.2/mcrit/config/
--rw-rw-r--   0 analyst   (1000) analyst   (1000)      855 2022-02-03 10:05:12.000000 mcrit-1.0.2/mcrit/config/ConfigInterface.py
--rw-rw-r--   0 analyst   (1000) analyst   (1000)      960 2023-05-22 12:12:44.000000 mcrit-1.0.2/mcrit/config/McritConfig.py
--rw-rw-r--   0 analyst   (1000) analyst   (1000)     2148 2023-05-22 08:41:11.000000 mcrit-1.0.2/mcrit/config/MinHashConfig.py
--rw-rw-r--   0 analyst   (1000) analyst   (1000)      821 2022-02-03 10:05:12.000000 mcrit-1.0.2/mcrit/config/QueueConfig.py
--rw-rw-r--   0 analyst   (1000) analyst   (1000)     1974 2022-02-08 09:50:02.000000 mcrit-1.0.2/mcrit/config/ShinglerConfig.py
--rw-rw-r--   0 analyst   (1000) analyst   (1000)     1775 2022-08-15 15:05:19.000000 mcrit-1.0.2/mcrit/config/StorageConfig.py
--rw-rw-r--   0 analyst   (1000) analyst   (1000)        0 2022-02-03 10:05:12.000000 mcrit-1.0.2/mcrit/config/__init__.py
-drwxrwxr-x   0 analyst   (1000) analyst   (1000)        0 2023-05-22 12:13:28.327190 mcrit-1.0.2/mcrit/index/
--rw-rw-r--   0 analyst   (1000) analyst   (1000)    29120 2023-05-22 08:41:11.000000 mcrit-1.0.2/mcrit/index/MinHashIndex.py
--rw-rw-r--   0 analyst   (1000) analyst   (1000)     3890 2022-08-16 08:15:37.000000 mcrit-1.0.2/mcrit/index/SearchCursor.py
--rw-rw-r--   0 analyst   (1000) analyst   (1000)     6210 2022-08-16 08:15:37.000000 mcrit-1.0.2/mcrit/index/SearchQueryParser.py
--rw-rw-r--   0 analyst   (1000) analyst   (1000)     6366 2022-08-16 08:15:37.000000 mcrit-1.0.2/mcrit/index/SearchQueryTree.py
--rw-rw-r--   0 analyst   (1000) analyst   (1000)        0 2022-02-03 10:05:12.000000 mcrit-1.0.2/mcrit/index/__init__.py
-drwxrwxr-x   0 analyst   (1000) analyst   (1000)        0 2023-05-22 12:13:28.327190 mcrit-1.0.2/mcrit/libs/
--rw-rw-r--   0 analyst   (1000) analyst   (1000)        0 2022-02-03 10:05:12.000000 mcrit-1.0.2/mcrit/libs/__init__.py
--rw-rw-r--   0 analyst   (1000) analyst   (1000)    16784 2022-09-01 07:23:47.000000 mcrit-1.0.2/mcrit/libs/mongoqueue.py
--rw-rw-r--   0 analyst   (1000) analyst   (1000)    14152 2022-02-03 10:05:12.000000 mcrit-1.0.2/mcrit/libs/pymmh3.py
--rw-rw-r--   0 analyst   (1000) analyst   (1000)     2028 2022-02-08 13:06:39.000000 mcrit-1.0.2/mcrit/libs/utility.py
-drwxrwxr-x   0 analyst   (1000) analyst   (1000)        0 2023-05-22 12:13:28.331190 mcrit-1.0.2/mcrit/matchers/
--rw-rw-r--   0 analyst   (1000) analyst   (1000)     6378 2022-09-01 07:23:47.000000 mcrit-1.0.2/mcrit/matchers/MatcherCross.py
--rw-rw-r--   0 analyst   (1000) analyst   (1000)    28260 2023-05-22 08:41:11.000000 mcrit-1.0.2/mcrit/matchers/MatcherInterface.py
--rw-rw-r--   0 analyst   (1000) analyst   (1000)     3014 2022-12-13 12:02:29.000000 mcrit-1.0.2/mcrit/matchers/MatcherQuery.py
--rw-rw-r--   0 analyst   (1000) analyst   (1000)     3097 2023-05-22 08:41:11.000000 mcrit-1.0.2/mcrit/matchers/MatcherQueryFunction.py
--rw-rw-r--   0 analyst   (1000) analyst   (1000)      751 2022-09-29 07:21:37.000000 mcrit-1.0.2/mcrit/matchers/MatcherSample.py
--rw-rw-r--   0 analyst   (1000) analyst   (1000)     2429 2022-12-13 15:01:23.000000 mcrit-1.0.2/mcrit/matchers/MatcherVs.py
--rw-rw-r--   0 analyst   (1000) analyst   (1000)        0 2022-09-01 07:23:47.000000 mcrit-1.0.2/mcrit/matchers/__init__.py
-drwxrwxr-x   0 analyst   (1000) analyst   (1000)        0 2023-05-22 12:13:28.331190 mcrit-1.0.2/mcrit/minhash/
--rw-rw-r--   0 analyst   (1000) analyst   (1000)     3662 2022-02-03 10:05:12.000000 mcrit-1.0.2/mcrit/minhash/MinHash.py
--rw-rw-r--   0 analyst   (1000) analyst   (1000)    10547 2022-11-15 08:15:21.000000 mcrit-1.0.2/mcrit/minhash/MinHasher.py
--rw-rw-r--   0 analyst   (1000) analyst   (1000)     3212 2022-02-03 10:05:12.000000 mcrit-1.0.2/mcrit/minhash/ShingleLoader.py
--rw-rw-r--   0 analyst   (1000) analyst   (1000)        0 2022-02-03 10:05:12.000000 mcrit-1.0.2/mcrit/minhash/__init__.py
-drwxrwxr-x   0 analyst   (1000) analyst   (1000)        0 2023-05-22 12:13:28.331190 mcrit-1.0.2/mcrit/queue/
--rw-rw-r--   0 analyst   (1000) analyst   (1000)    10980 2022-09-01 07:23:47.000000 mcrit-1.0.2/mcrit/queue/LocalQueue.py
--rw-rw-r--   0 analyst   (1000) analyst   (1000)     1308 2022-02-03 10:05:12.000000 mcrit-1.0.2/mcrit/queue/QueueFactory.py
--rw-rw-r--   0 analyst   (1000) analyst   (1000)    14987 2022-10-13 09:02:52.000000 mcrit-1.0.2/mcrit/queue/QueueRemoteCalls.py
--rw-rw-r--   0 analyst   (1000) analyst   (1000)        0 2022-09-01 07:23:47.000000 mcrit-1.0.2/mcrit/queue/__init__.py
-drwxrwxr-x   0 analyst   (1000) analyst   (1000)        0 2023-05-22 12:13:28.331190 mcrit-1.0.2/mcrit/server/
--rw-rw-r--   0 analyst   (1000) analyst   (1000)     1297 2023-03-29 07:45:34.000000 mcrit-1.0.2/mcrit/server/BlocksResource.py
--rw-rw-r--   0 analyst   (1000) analyst   (1000)     6004 2023-03-29 07:45:34.000000 mcrit-1.0.2/mcrit/server/FamilyResource.py
--rw-rw-r--   0 analyst   (1000) analyst   (1000)     3764 2023-05-22 08:41:11.000000 mcrit-1.0.2/mcrit/server/FunctionResource.py
--rw-rw-r--   0 analyst   (1000) analyst   (1000)     4609 2023-03-29 07:45:34.000000 mcrit-1.0.2/mcrit/server/JobResource.py
--rw-rw-r--   0 analyst   (1000) analyst   (1000)     3551 2023-03-29 07:45:34.000000 mcrit-1.0.2/mcrit/server/MatchResource.py
--rw-rw-r--   0 analyst   (1000) analyst   (1000)     7608 2023-03-29 07:45:34.000000 mcrit-1.0.2/mcrit/server/QueryResource.py
--rw-rw-r--   0 analyst   (1000) analyst   (1000)    11793 2023-03-29 07:45:34.000000 mcrit-1.0.2/mcrit/server/SampleResource.py
--rw-rw-r--   0 analyst   (1000) analyst   (1000)     5159 2023-03-29 07:45:34.000000 mcrit-1.0.2/mcrit/server/StatusResource.py
--rw-rw-r--   0 analyst   (1000) analyst   (1000)        0 2022-02-03 10:05:12.000000 mcrit-1.0.2/mcrit/server/__init__.py
--rw-rw-r--   0 analyst   (1000) analyst   (1000)     5887 2023-03-29 07:45:34.000000 mcrit-1.0.2/mcrit/server/application_routes.py
--rw-rw-r--   0 analyst   (1000) analyst   (1000)     1868 2023-03-29 07:45:34.000000 mcrit-1.0.2/mcrit/server/utils.py
--rw-rw-r--   0 analyst   (1000) analyst   (1000)       69 2022-02-03 10:05:12.000000 mcrit-1.0.2/mcrit/server/wsgi.py
-drwxrwxr-x   0 analyst   (1000) analyst   (1000)        0 2023-05-22 12:13:28.331190 mcrit-1.0.2/mcrit/storage/
--rw-rw-r--   0 analyst   (1000) analyst   (1000)     2077 2022-08-15 15:05:19.000000 mcrit-1.0.2/mcrit/storage/FamilyEntry.py
--rw-rw-r--   0 analyst   (1000) analyst   (1000)     6415 2023-03-29 07:45:34.000000 mcrit-1.0.2/mcrit/storage/FunctionEntry.py
--rw-rw-r--   0 analyst   (1000) analyst   (1000)     1661 2023-03-29 07:45:34.000000 mcrit-1.0.2/mcrit/storage/FunctionLabelEntry.py
--rw-rw-r--   0 analyst   (1000) analyst   (1000)     2764 2022-12-13 13:23:45.000000 mcrit-1.0.2/mcrit/storage/MatchedFunctionEntry.py
--rw-rw-r--   0 analyst   (1000) analyst   (1000)     6617 2023-03-16 12:54:37.000000 mcrit-1.0.2/mcrit/storage/MatchedSampleEntry.py
--rw-rw-r--   0 analyst   (1000) analyst   (1000)     1389 2023-05-22 08:41:11.000000 mcrit-1.0.2/mcrit/storage/MatchingCache.py
--rw-rw-r--   0 analyst   (1000) analyst   (1000)    21812 2023-03-16 12:54:37.000000 mcrit-1.0.2/mcrit/storage/MatchingResult.py
--rw-rw-r--   0 analyst   (1000) analyst   (1000)    44811 2023-05-22 08:41:03.000000 mcrit-1.0.2/mcrit/storage/MemoryStorage.py
--rw-rw-r--   0 analyst   (1000) analyst   (1000)    59597 2023-05-22 08:41:11.000000 mcrit-1.0.2/mcrit/storage/MongoDbStorage.py
--rw-rw-r--   0 analyst   (1000) analyst   (1000)     4932 2023-03-29 07:45:34.000000 mcrit-1.0.2/mcrit/storage/SampleEntry.py
--rw-rw-r--   0 analyst   (1000) analyst   (1000)      735 2022-11-15 08:15:21.000000 mcrit-1.0.2/mcrit/storage/StorageFactory.py
--rw-rw-r--   0 analyst   (1000) analyst   (1000)    25158 2023-03-29 07:45:34.000000 mcrit-1.0.2/mcrit/storage/StorageInterface.py
--rw-rw-r--   0 analyst   (1000) analyst   (1000)        0 2022-02-03 10:05:12.000000 mcrit-1.0.2/mcrit/storage/__init__.py
-drwxrwxr-x   0 analyst   (1000) analyst   (1000)        0 2023-05-22 12:13:28.327190 mcrit-1.0.2/mcrit.egg-info/
--rw-rw-r--   0 analyst   (1000) analyst   (1000)    11397 2023-05-22 12:13:28.000000 mcrit-1.0.2/mcrit.egg-info/PKG-INFO
--rw-rw-r--   0 analyst   (1000) analyst   (1000)     1950 2023-05-22 12:13:28.000000 mcrit-1.0.2/mcrit.egg-info/SOURCES.txt
--rw-rw-r--   0 analyst   (1000) analyst   (1000)        1 2023-05-22 12:13:28.000000 mcrit-1.0.2/mcrit.egg-info/dependency_links.txt
--rw-rw-r--   0 analyst   (1000) analyst   (1000)      135 2023-05-22 12:13:28.000000 mcrit-1.0.2/mcrit.egg-info/requires.txt
--rw-rw-r--   0 analyst   (1000) analyst   (1000)        6 2023-05-22 12:13:28.000000 mcrit-1.0.2/mcrit.egg-info/top_level.txt
--rw-rw-r--   0 analyst   (1000) analyst   (1000)       38 2023-05-22 12:13:28.331190 mcrit-1.0.2/setup.cfg
--rw-rw-r--   0 analyst   (1000) analyst   (1000)     1355 2023-05-22 12:12:01.000000 mcrit-1.0.2/setup.py
+drwxrwxr-x   0 analyst   (1000) analyst   (1000)        0 2023-05-22 12:32:44.779174 mcrit-1.0.3/
+-rw-rw-r--   0 analyst   (1000) analyst   (1000)    35149 2022-05-05 12:52:43.000000 mcrit-1.0.3/LICENSE
+-rw-rw-r--   0 analyst   (1000) analyst   (1000)    11397 2023-05-22 12:32:44.779174 mcrit-1.0.3/PKG-INFO
+-rw-rw-r--   0 analyst   (1000) analyst   (1000)    10645 2023-05-22 12:31:52.000000 mcrit-1.0.3/README.md
+drwxrwxr-x   0 analyst   (1000) analyst   (1000)        0 2023-05-22 12:32:44.771174 mcrit-1.0.3/mcrit/
+-rw-rw-r--   0 analyst   (1000) analyst   (1000)    21415 2022-12-13 15:03:46.000000 mcrit-1.0.3/mcrit/Worker.py
+-rw-rw-r--   0 analyst   (1000) analyst   (1000)        0 2022-02-03 10:05:12.000000 mcrit-1.0.3/mcrit/__init__.py
+-rw-rw-r--   0 analyst   (1000) analyst   (1000)     1838 2023-03-16 12:54:37.000000 mcrit-1.0.3/mcrit/__main__.py
+drwxrwxr-x   0 analyst   (1000) analyst   (1000)        0 2023-05-22 12:32:44.771174 mcrit-1.0.3/mcrit/client/
+-rw-rw-r--   0 analyst   (1000) analyst   (1000)    28489 2023-05-22 08:41:11.000000 mcrit-1.0.3/mcrit/client/McritClient.py
+-rw-rw-r--   0 analyst   (1000) analyst   (1000)    18792 2023-05-22 12:31:03.000000 mcrit-1.0.3/mcrit/client/McritConsole.py
+-rw-rw-r--   0 analyst   (1000) analyst   (1000)        0 2022-02-03 10:05:12.000000 mcrit-1.0.3/mcrit/client/__init__.py
+drwxrwxr-x   0 analyst   (1000) analyst   (1000)        0 2023-05-22 12:32:44.771174 mcrit-1.0.3/mcrit/config/
+-rw-rw-r--   0 analyst   (1000) analyst   (1000)      855 2022-02-03 10:05:12.000000 mcrit-1.0.3/mcrit/config/ConfigInterface.py
+-rw-rw-r--   0 analyst   (1000) analyst   (1000)      960 2023-05-22 12:31:58.000000 mcrit-1.0.3/mcrit/config/McritConfig.py
+-rw-rw-r--   0 analyst   (1000) analyst   (1000)     2148 2023-05-22 08:41:11.000000 mcrit-1.0.3/mcrit/config/MinHashConfig.py
+-rw-rw-r--   0 analyst   (1000) analyst   (1000)      821 2022-02-03 10:05:12.000000 mcrit-1.0.3/mcrit/config/QueueConfig.py
+-rw-rw-r--   0 analyst   (1000) analyst   (1000)     1974 2022-02-08 09:50:02.000000 mcrit-1.0.3/mcrit/config/ShinglerConfig.py
+-rw-rw-r--   0 analyst   (1000) analyst   (1000)     1775 2022-08-15 15:05:19.000000 mcrit-1.0.3/mcrit/config/StorageConfig.py
+-rw-rw-r--   0 analyst   (1000) analyst   (1000)        0 2022-02-03 10:05:12.000000 mcrit-1.0.3/mcrit/config/__init__.py
+drwxrwxr-x   0 analyst   (1000) analyst   (1000)        0 2023-05-22 12:32:44.775174 mcrit-1.0.3/mcrit/index/
+-rw-rw-r--   0 analyst   (1000) analyst   (1000)    29120 2023-05-22 08:41:11.000000 mcrit-1.0.3/mcrit/index/MinHashIndex.py
+-rw-rw-r--   0 analyst   (1000) analyst   (1000)     3890 2022-08-16 08:15:37.000000 mcrit-1.0.3/mcrit/index/SearchCursor.py
+-rw-rw-r--   0 analyst   (1000) analyst   (1000)     6210 2022-08-16 08:15:37.000000 mcrit-1.0.3/mcrit/index/SearchQueryParser.py
+-rw-rw-r--   0 analyst   (1000) analyst   (1000)     6366 2022-08-16 08:15:37.000000 mcrit-1.0.3/mcrit/index/SearchQueryTree.py
+-rw-rw-r--   0 analyst   (1000) analyst   (1000)        0 2022-02-03 10:05:12.000000 mcrit-1.0.3/mcrit/index/__init__.py
+drwxrwxr-x   0 analyst   (1000) analyst   (1000)        0 2023-05-22 12:32:44.775174 mcrit-1.0.3/mcrit/libs/
+-rw-rw-r--   0 analyst   (1000) analyst   (1000)        0 2022-02-03 10:05:12.000000 mcrit-1.0.3/mcrit/libs/__init__.py
+-rw-rw-r--   0 analyst   (1000) analyst   (1000)    16784 2022-09-01 07:23:47.000000 mcrit-1.0.3/mcrit/libs/mongoqueue.py
+-rw-rw-r--   0 analyst   (1000) analyst   (1000)    14152 2022-02-03 10:05:12.000000 mcrit-1.0.3/mcrit/libs/pymmh3.py
+-rw-rw-r--   0 analyst   (1000) analyst   (1000)     2028 2022-02-08 13:06:39.000000 mcrit-1.0.3/mcrit/libs/utility.py
+drwxrwxr-x   0 analyst   (1000) analyst   (1000)        0 2023-05-22 12:32:44.775174 mcrit-1.0.3/mcrit/matchers/
+-rw-rw-r--   0 analyst   (1000) analyst   (1000)     6378 2022-09-01 07:23:47.000000 mcrit-1.0.3/mcrit/matchers/MatcherCross.py
+-rw-rw-r--   0 analyst   (1000) analyst   (1000)    28260 2023-05-22 08:41:11.000000 mcrit-1.0.3/mcrit/matchers/MatcherInterface.py
+-rw-rw-r--   0 analyst   (1000) analyst   (1000)     3014 2022-12-13 12:02:29.000000 mcrit-1.0.3/mcrit/matchers/MatcherQuery.py
+-rw-rw-r--   0 analyst   (1000) analyst   (1000)     3097 2023-05-22 08:41:11.000000 mcrit-1.0.3/mcrit/matchers/MatcherQueryFunction.py
+-rw-rw-r--   0 analyst   (1000) analyst   (1000)      751 2022-09-29 07:21:37.000000 mcrit-1.0.3/mcrit/matchers/MatcherSample.py
+-rw-rw-r--   0 analyst   (1000) analyst   (1000)     2429 2022-12-13 15:01:23.000000 mcrit-1.0.3/mcrit/matchers/MatcherVs.py
+-rw-rw-r--   0 analyst   (1000) analyst   (1000)        0 2022-09-01 07:23:47.000000 mcrit-1.0.3/mcrit/matchers/__init__.py
+drwxrwxr-x   0 analyst   (1000) analyst   (1000)        0 2023-05-22 12:32:44.775174 mcrit-1.0.3/mcrit/minhash/
+-rw-rw-r--   0 analyst   (1000) analyst   (1000)     3662 2022-02-03 10:05:12.000000 mcrit-1.0.3/mcrit/minhash/MinHash.py
+-rw-rw-r--   0 analyst   (1000) analyst   (1000)    10547 2022-11-15 08:15:21.000000 mcrit-1.0.3/mcrit/minhash/MinHasher.py
+-rw-rw-r--   0 analyst   (1000) analyst   (1000)     3212 2022-02-03 10:05:12.000000 mcrit-1.0.3/mcrit/minhash/ShingleLoader.py
+-rw-rw-r--   0 analyst   (1000) analyst   (1000)        0 2022-02-03 10:05:12.000000 mcrit-1.0.3/mcrit/minhash/__init__.py
+drwxrwxr-x   0 analyst   (1000) analyst   (1000)        0 2023-05-22 12:32:44.775174 mcrit-1.0.3/mcrit/queue/
+-rw-rw-r--   0 analyst   (1000) analyst   (1000)    10980 2022-09-01 07:23:47.000000 mcrit-1.0.3/mcrit/queue/LocalQueue.py
+-rw-rw-r--   0 analyst   (1000) analyst   (1000)     1308 2022-02-03 10:05:12.000000 mcrit-1.0.3/mcrit/queue/QueueFactory.py
+-rw-rw-r--   0 analyst   (1000) analyst   (1000)    14987 2022-10-13 09:02:52.000000 mcrit-1.0.3/mcrit/queue/QueueRemoteCalls.py
+-rw-rw-r--   0 analyst   (1000) analyst   (1000)        0 2022-09-01 07:23:47.000000 mcrit-1.0.3/mcrit/queue/__init__.py
+drwxrwxr-x   0 analyst   (1000) analyst   (1000)        0 2023-05-22 12:32:44.775174 mcrit-1.0.3/mcrit/server/
+-rw-rw-r--   0 analyst   (1000) analyst   (1000)     1297 2023-03-29 07:45:34.000000 mcrit-1.0.3/mcrit/server/BlocksResource.py
+-rw-rw-r--   0 analyst   (1000) analyst   (1000)     6004 2023-03-29 07:45:34.000000 mcrit-1.0.3/mcrit/server/FamilyResource.py
+-rw-rw-r--   0 analyst   (1000) analyst   (1000)     3764 2023-05-22 08:41:11.000000 mcrit-1.0.3/mcrit/server/FunctionResource.py
+-rw-rw-r--   0 analyst   (1000) analyst   (1000)     4609 2023-03-29 07:45:34.000000 mcrit-1.0.3/mcrit/server/JobResource.py
+-rw-rw-r--   0 analyst   (1000) analyst   (1000)     3551 2023-03-29 07:45:34.000000 mcrit-1.0.3/mcrit/server/MatchResource.py
+-rw-rw-r--   0 analyst   (1000) analyst   (1000)     7608 2023-03-29 07:45:34.000000 mcrit-1.0.3/mcrit/server/QueryResource.py
+-rw-rw-r--   0 analyst   (1000) analyst   (1000)    11793 2023-03-29 07:45:34.000000 mcrit-1.0.3/mcrit/server/SampleResource.py
+-rw-rw-r--   0 analyst   (1000) analyst   (1000)     5159 2023-03-29 07:45:34.000000 mcrit-1.0.3/mcrit/server/StatusResource.py
+-rw-rw-r--   0 analyst   (1000) analyst   (1000)        0 2022-02-03 10:05:12.000000 mcrit-1.0.3/mcrit/server/__init__.py
+-rw-rw-r--   0 analyst   (1000) analyst   (1000)     5887 2023-03-29 07:45:34.000000 mcrit-1.0.3/mcrit/server/application_routes.py
+-rw-rw-r--   0 analyst   (1000) analyst   (1000)     1868 2023-03-29 07:45:34.000000 mcrit-1.0.3/mcrit/server/utils.py
+-rw-rw-r--   0 analyst   (1000) analyst   (1000)       69 2022-02-03 10:05:12.000000 mcrit-1.0.3/mcrit/server/wsgi.py
+drwxrwxr-x   0 analyst   (1000) analyst   (1000)        0 2023-05-22 12:32:44.775174 mcrit-1.0.3/mcrit/storage/
+-rw-rw-r--   0 analyst   (1000) analyst   (1000)     2077 2022-08-15 15:05:19.000000 mcrit-1.0.3/mcrit/storage/FamilyEntry.py
+-rw-rw-r--   0 analyst   (1000) analyst   (1000)     6415 2023-03-29 07:45:34.000000 mcrit-1.0.3/mcrit/storage/FunctionEntry.py
+-rw-rw-r--   0 analyst   (1000) analyst   (1000)     1661 2023-03-29 07:45:34.000000 mcrit-1.0.3/mcrit/storage/FunctionLabelEntry.py
+-rw-rw-r--   0 analyst   (1000) analyst   (1000)     2764 2022-12-13 13:23:45.000000 mcrit-1.0.3/mcrit/storage/MatchedFunctionEntry.py
+-rw-rw-r--   0 analyst   (1000) analyst   (1000)     6617 2023-03-16 12:54:37.000000 mcrit-1.0.3/mcrit/storage/MatchedSampleEntry.py
+-rw-rw-r--   0 analyst   (1000) analyst   (1000)     1389 2023-05-22 08:41:11.000000 mcrit-1.0.3/mcrit/storage/MatchingCache.py
+-rw-rw-r--   0 analyst   (1000) analyst   (1000)    21812 2023-03-16 12:54:37.000000 mcrit-1.0.3/mcrit/storage/MatchingResult.py
+-rw-rw-r--   0 analyst   (1000) analyst   (1000)    44811 2023-05-22 08:41:03.000000 mcrit-1.0.3/mcrit/storage/MemoryStorage.py
+-rw-rw-r--   0 analyst   (1000) analyst   (1000)    59597 2023-05-22 08:41:11.000000 mcrit-1.0.3/mcrit/storage/MongoDbStorage.py
+-rw-rw-r--   0 analyst   (1000) analyst   (1000)     4932 2023-03-29 07:45:34.000000 mcrit-1.0.3/mcrit/storage/SampleEntry.py
+-rw-rw-r--   0 analyst   (1000) analyst   (1000)      735 2022-11-15 08:15:21.000000 mcrit-1.0.3/mcrit/storage/StorageFactory.py
+-rw-rw-r--   0 analyst   (1000) analyst   (1000)    25158 2023-03-29 07:45:34.000000 mcrit-1.0.3/mcrit/storage/StorageInterface.py
+-rw-rw-r--   0 analyst   (1000) analyst   (1000)        0 2022-02-03 10:05:12.000000 mcrit-1.0.3/mcrit/storage/__init__.py
+drwxrwxr-x   0 analyst   (1000) analyst   (1000)        0 2023-05-22 12:32:44.771174 mcrit-1.0.3/mcrit.egg-info/
+-rw-rw-r--   0 analyst   (1000) analyst   (1000)    11397 2023-05-22 12:32:44.000000 mcrit-1.0.3/mcrit.egg-info/PKG-INFO
+-rw-rw-r--   0 analyst   (1000) analyst   (1000)     1950 2023-05-22 12:32:44.000000 mcrit-1.0.3/mcrit.egg-info/SOURCES.txt
+-rw-rw-r--   0 analyst   (1000) analyst   (1000)        1 2023-05-22 12:32:44.000000 mcrit-1.0.3/mcrit.egg-info/dependency_links.txt
+-rw-rw-r--   0 analyst   (1000) analyst   (1000)      135 2023-05-22 12:32:44.000000 mcrit-1.0.3/mcrit.egg-info/requires.txt
+-rw-rw-r--   0 analyst   (1000) analyst   (1000)        6 2023-05-22 12:32:44.000000 mcrit-1.0.3/mcrit.egg-info/top_level.txt
+-rw-rw-r--   0 analyst   (1000) analyst   (1000)       38 2023-05-22 12:32:44.779174 mcrit-1.0.3/setup.cfg
+-rw-rw-r--   0 analyst   (1000) analyst   (1000)     1355 2023-05-22 12:31:47.000000 mcrit-1.0.3/setup.py
```

### Comparing `mcrit-1.0.2/LICENSE` & `mcrit-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `mcrit-1.0.2/PKG-INFO` & `mcrit-1.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mcrit
-Version: 1.0.2
+Version: 1.0.3
 Summary: MCRIT is a framework created for simplified application of the MinHash algorithm to code similarity.
 Home-page: https://github.com/danielplohmann/mcrit
 Author: Daniel Plohmann, Manuel Blatt, Steffen Enders, Paul Hordiienko
 Author-email: daniel.plohmann@fkie.fraunhofer.de
 License: NU General Public License v3 (GPLv3)
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
@@ -130,15 +130,15 @@
 ./plugins/ida/ida_mcrit.py
 ```
 
 in IDA.
 
 
 ## Version History
- * 2023-05-22 v1.0.2: More robustness for path verification when using MCRIT CLI on Malpedia repo folder.
+ * 2023-05-22 v1.0.3: More robustness for path verification when using MCRIT CLI on Malpedia repo folder.
  * 2023-05-12 v1.0.1: Some progress on label import for the IDA plugin. Reflected API extension of MCRITweb in McritClient.
  * 2023-04-10 v1.0.0: Milestone release for Botconf 2023.
  * 2023-04-10 v0.25.0: IDA plugin can now do function queries for the currently viewed function.
  * 2023-03-24 v0.24.2: McritClient can forward username/apitoken, addJsonReport is now forwardable.
  * 2023-03-21 v0.24.0: FunctionEntries now can store additional FunctionLabelEntries, along submitting user/date.
  * 2023-03-17 v0.23.0: It is now possible to query matches for single SmdaFunctions (synchronously).
  * 2023-03-15 v0.22.0: McritClient now supports apitokens and raw responses for a subset of functionality.
```

### Comparing `mcrit-1.0.2/README.md` & `mcrit-1.0.3/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -113,15 +113,15 @@
 ./plugins/ida/ida_mcrit.py
 ```
 
 in IDA.
 
 
 ## Version History
- * 2023-05-22 v1.0.2: More robustness for path verification when using MCRIT CLI on Malpedia repo folder.
+ * 2023-05-22 v1.0.3: More robustness for path verification when using MCRIT CLI on Malpedia repo folder.
  * 2023-05-12 v1.0.1: Some progress on label import for the IDA plugin. Reflected API extension of MCRITweb in McritClient.
  * 2023-04-10 v1.0.0: Milestone release for Botconf 2023.
  * 2023-04-10 v0.25.0: IDA plugin can now do function queries for the currently viewed function.
  * 2023-03-24 v0.24.2: McritClient can forward username/apitoken, addJsonReport is now forwardable.
  * 2023-03-21 v0.24.0: FunctionEntries now can store additional FunctionLabelEntries, along submitting user/date.
  * 2023-03-17 v0.23.0: It is now possible to query matches for single SmdaFunctions (synchronously).
  * 2023-03-15 v0.22.0: McritClient now supports apitokens and raw responses for a subset of functionality.
```

### Comparing `mcrit-1.0.2/mcrit/Worker.py` & `mcrit-1.0.3/mcrit/Worker.py`

 * *Files identical despite different names*

### Comparing `mcrit-1.0.2/mcrit/__main__.py` & `mcrit-1.0.3/mcrit/__main__.py`

 * *Files identical despite different names*

### Comparing `mcrit-1.0.2/mcrit/client/McritClient.py` & `mcrit-1.0.3/mcrit/client/McritClient.py`

 * *Files identical despite different names*

### Comparing `mcrit-1.0.2/mcrit/client/McritConsole.py` & `mcrit-1.0.3/mcrit/client/McritConsole.py`

 * *Files 3% similar despite different names*

```diff
@@ -91,18 +91,30 @@
     else:
         if args.executables_only and not is_pe_or_elf(filepath):
             print(f"Skipping a file not recognized as executable: {filepath}")
         else:
             disassembler = Disassembler()
             if get_base_addr(filename) is not None:
                 base_addr = get_base_addr(filename)
-                smda_report = disassembler.disassembleBuffer(readFileContent(filepath), base_addr)
-                smda_report.filename = filename
+                try:
+                    smda_report = disassembler.disassembleBuffer(readFileContent(filepath), base_addr)
+                    smda_report.filename = filename
+                except Exception as exc:
+                    import traceback
+                    print(f"ERROR: SMDA caused an exception while processing this file: {filepath}")
+                    print(traceback.format_exc())
+                    return None
             else:
-                smda_report = disassembler.disassembleFile(filepath)
+                try:
+                    smda_report = disassembler.disassembleFile(filepath)
+                except:
+                    import traceback
+                    print(f"ERROR: SMDA caused an exception while processing this file: {filepath}")
+                    print(traceback.format_exc())
+                    return None
     # apply any of the forced flags: family, version, library
     if smda_report:
         if args.mode in ["file", "dir"]:
             if args.family is not None:
                 smda_report.family = args.family
             if args.version is not None:
                 smda_report.version = args.version
```

### Comparing `mcrit-1.0.2/mcrit/config/ConfigInterface.py` & `mcrit-1.0.3/mcrit/config/ConfigInterface.py`

 * *Files identical despite different names*

### Comparing `mcrit-1.0.2/mcrit/config/McritConfig.py` & `mcrit-1.0.3/mcrit/config/McritConfig.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from .ShinglerConfig import ShinglerConfig
 from .StorageConfig import StorageConfig
 
 
 class McritConfig(object):
 
     # NOTE to self: always change this in setup.py as well!
-    VERSION = "1.0.2"
+    VERSION = "1.0.3"
     CONFIG_FILE_PATH = str(os.path.abspath(__file__))
     PROJECT_ROOT = str(os.path.abspath(os.sep.join([CONFIG_FILE_PATH, "..", ".."])))
 
     ### global logging-config setup
     # Only do basicConfig if no handlers have been configured
     LOG_PATH = "./"
     LOG_LEVEL = logging.INFO
```

### Comparing `mcrit-1.0.2/mcrit/config/MinHashConfig.py` & `mcrit-1.0.3/mcrit/config/MinHashConfig.py`

 * *Files identical despite different names*

### Comparing `mcrit-1.0.2/mcrit/config/QueueConfig.py` & `mcrit-1.0.3/mcrit/config/QueueConfig.py`

 * *Files identical despite different names*

### Comparing `mcrit-1.0.2/mcrit/config/ShinglerConfig.py` & `mcrit-1.0.3/mcrit/config/ShinglerConfig.py`

 * *Files identical despite different names*

### Comparing `mcrit-1.0.2/mcrit/config/StorageConfig.py` & `mcrit-1.0.3/mcrit/config/StorageConfig.py`

 * *Files identical despite different names*

### Comparing `mcrit-1.0.2/mcrit/index/MinHashIndex.py` & `mcrit-1.0.3/mcrit/index/MinHashIndex.py`

 * *Files identical despite different names*

### Comparing `mcrit-1.0.2/mcrit/index/SearchCursor.py` & `mcrit-1.0.3/mcrit/index/SearchCursor.py`

 * *Files identical despite different names*

### Comparing `mcrit-1.0.2/mcrit/index/SearchQueryParser.py` & `mcrit-1.0.3/mcrit/index/SearchQueryParser.py`

 * *Files identical despite different names*

### Comparing `mcrit-1.0.2/mcrit/index/SearchQueryTree.py` & `mcrit-1.0.3/mcrit/index/SearchQueryTree.py`

 * *Files identical despite different names*

### Comparing `mcrit-1.0.2/mcrit/libs/mongoqueue.py` & `mcrit-1.0.3/mcrit/libs/mongoqueue.py`

 * *Files identical despite different names*

### Comparing `mcrit-1.0.2/mcrit/libs/pymmh3.py` & `mcrit-1.0.3/mcrit/libs/pymmh3.py`

 * *Files identical despite different names*

### Comparing `mcrit-1.0.2/mcrit/libs/utility.py` & `mcrit-1.0.3/mcrit/libs/utility.py`

 * *Files identical despite different names*

### Comparing `mcrit-1.0.2/mcrit/matchers/MatcherCross.py` & `mcrit-1.0.3/mcrit/matchers/MatcherCross.py`

 * *Files identical despite different names*

### Comparing `mcrit-1.0.2/mcrit/matchers/MatcherInterface.py` & `mcrit-1.0.3/mcrit/matchers/MatcherInterface.py`

 * *Files identical despite different names*

### Comparing `mcrit-1.0.2/mcrit/matchers/MatcherQuery.py` & `mcrit-1.0.3/mcrit/matchers/MatcherQuery.py`

 * *Files identical despite different names*

### Comparing `mcrit-1.0.2/mcrit/matchers/MatcherQueryFunction.py` & `mcrit-1.0.3/mcrit/matchers/MatcherQueryFunction.py`

 * *Files identical despite different names*

### Comparing `mcrit-1.0.2/mcrit/matchers/MatcherSample.py` & `mcrit-1.0.3/mcrit/matchers/MatcherSample.py`

 * *Files identical despite different names*

### Comparing `mcrit-1.0.2/mcrit/matchers/MatcherVs.py` & `mcrit-1.0.3/mcrit/matchers/MatcherVs.py`

 * *Files identical despite different names*

### Comparing `mcrit-1.0.2/mcrit/minhash/MinHash.py` & `mcrit-1.0.3/mcrit/minhash/MinHash.py`

 * *Files identical despite different names*

### Comparing `mcrit-1.0.2/mcrit/minhash/MinHasher.py` & `mcrit-1.0.3/mcrit/minhash/MinHasher.py`

 * *Files identical despite different names*

### Comparing `mcrit-1.0.2/mcrit/minhash/ShingleLoader.py` & `mcrit-1.0.3/mcrit/minhash/ShingleLoader.py`

 * *Files identical despite different names*

### Comparing `mcrit-1.0.2/mcrit/queue/LocalQueue.py` & `mcrit-1.0.3/mcrit/queue/LocalQueue.py`

 * *Files identical despite different names*

### Comparing `mcrit-1.0.2/mcrit/queue/QueueFactory.py` & `mcrit-1.0.3/mcrit/queue/QueueFactory.py`

 * *Files identical despite different names*

### Comparing `mcrit-1.0.2/mcrit/queue/QueueRemoteCalls.py` & `mcrit-1.0.3/mcrit/queue/QueueRemoteCalls.py`

 * *Files identical despite different names*

### Comparing `mcrit-1.0.2/mcrit/server/BlocksResource.py` & `mcrit-1.0.3/mcrit/server/BlocksResource.py`

 * *Files identical despite different names*

### Comparing `mcrit-1.0.2/mcrit/server/FamilyResource.py` & `mcrit-1.0.3/mcrit/server/FamilyResource.py`

 * *Files identical despite different names*

### Comparing `mcrit-1.0.2/mcrit/server/FunctionResource.py` & `mcrit-1.0.3/mcrit/server/FunctionResource.py`

 * *Files identical despite different names*

### Comparing `mcrit-1.0.2/mcrit/server/JobResource.py` & `mcrit-1.0.3/mcrit/server/JobResource.py`

 * *Files identical despite different names*

### Comparing `mcrit-1.0.2/mcrit/server/MatchResource.py` & `mcrit-1.0.3/mcrit/server/MatchResource.py`

 * *Files identical despite different names*

### Comparing `mcrit-1.0.2/mcrit/server/QueryResource.py` & `mcrit-1.0.3/mcrit/server/QueryResource.py`

 * *Files identical despite different names*

### Comparing `mcrit-1.0.2/mcrit/server/SampleResource.py` & `mcrit-1.0.3/mcrit/server/SampleResource.py`

 * *Files identical despite different names*

### Comparing `mcrit-1.0.2/mcrit/server/StatusResource.py` & `mcrit-1.0.3/mcrit/server/StatusResource.py`

 * *Files identical despite different names*

### Comparing `mcrit-1.0.2/mcrit/server/application_routes.py` & `mcrit-1.0.3/mcrit/server/application_routes.py`

 * *Files identical despite different names*

### Comparing `mcrit-1.0.2/mcrit/server/utils.py` & `mcrit-1.0.3/mcrit/server/utils.py`

 * *Files identical despite different names*

### Comparing `mcrit-1.0.2/mcrit/storage/FamilyEntry.py` & `mcrit-1.0.3/mcrit/storage/FamilyEntry.py`

 * *Files identical despite different names*

### Comparing `mcrit-1.0.2/mcrit/storage/FunctionEntry.py` & `mcrit-1.0.3/mcrit/storage/FunctionEntry.py`

 * *Files identical despite different names*

### Comparing `mcrit-1.0.2/mcrit/storage/FunctionLabelEntry.py` & `mcrit-1.0.3/mcrit/storage/FunctionLabelEntry.py`

 * *Files identical despite different names*

### Comparing `mcrit-1.0.2/mcrit/storage/MatchedFunctionEntry.py` & `mcrit-1.0.3/mcrit/storage/MatchedFunctionEntry.py`

 * *Files identical despite different names*

### Comparing `mcrit-1.0.2/mcrit/storage/MatchedSampleEntry.py` & `mcrit-1.0.3/mcrit/storage/MatchedSampleEntry.py`

 * *Files identical despite different names*

### Comparing `mcrit-1.0.2/mcrit/storage/MatchingCache.py` & `mcrit-1.0.3/mcrit/storage/MatchingCache.py`

 * *Files identical despite different names*

### Comparing `mcrit-1.0.2/mcrit/storage/MatchingResult.py` & `mcrit-1.0.3/mcrit/storage/MatchingResult.py`

 * *Files identical despite different names*

### Comparing `mcrit-1.0.2/mcrit/storage/MemoryStorage.py` & `mcrit-1.0.3/mcrit/storage/MemoryStorage.py`

 * *Files identical despite different names*

### Comparing `mcrit-1.0.2/mcrit/storage/MongoDbStorage.py` & `mcrit-1.0.3/mcrit/storage/MongoDbStorage.py`

 * *Files identical despite different names*

### Comparing `mcrit-1.0.2/mcrit/storage/SampleEntry.py` & `mcrit-1.0.3/mcrit/storage/SampleEntry.py`

 * *Files identical despite different names*

### Comparing `mcrit-1.0.2/mcrit/storage/StorageFactory.py` & `mcrit-1.0.3/mcrit/storage/StorageFactory.py`

 * *Files identical despite different names*

### Comparing `mcrit-1.0.2/mcrit/storage/StorageInterface.py` & `mcrit-1.0.3/mcrit/storage/StorageInterface.py`

 * *Files identical despite different names*

### Comparing `mcrit-1.0.2/mcrit.egg-info/PKG-INFO` & `mcrit-1.0.3/mcrit.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mcrit
-Version: 1.0.2
+Version: 1.0.3
 Summary: MCRIT is a framework created for simplified application of the MinHash algorithm to code similarity.
 Home-page: https://github.com/danielplohmann/mcrit
 Author: Daniel Plohmann, Manuel Blatt, Steffen Enders, Paul Hordiienko
 Author-email: daniel.plohmann@fkie.fraunhofer.de
 License: NU General Public License v3 (GPLv3)
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
@@ -130,15 +130,15 @@
 ./plugins/ida/ida_mcrit.py
 ```
 
 in IDA.
 
 
 ## Version History
- * 2023-05-22 v1.0.2: More robustness for path verification when using MCRIT CLI on Malpedia repo folder.
+ * 2023-05-22 v1.0.3: More robustness for path verification when using MCRIT CLI on Malpedia repo folder.
  * 2023-05-12 v1.0.1: Some progress on label import for the IDA plugin. Reflected API extension of MCRITweb in McritClient.
  * 2023-04-10 v1.0.0: Milestone release for Botconf 2023.
  * 2023-04-10 v0.25.0: IDA plugin can now do function queries for the currently viewed function.
  * 2023-03-24 v0.24.2: McritClient can forward username/apitoken, addJsonReport is now forwardable.
  * 2023-03-21 v0.24.0: FunctionEntries now can store additional FunctionLabelEntries, along submitting user/date.
  * 2023-03-17 v0.23.0: It is now possible to query matches for single SmdaFunctions (synchronously).
  * 2023-03-15 v0.22.0: McritClient now supports apitokens and raw responses for a subset of functionality.
```

### Comparing `mcrit-1.0.2/mcrit.egg-info/SOURCES.txt` & `mcrit-1.0.3/mcrit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mcrit-1.0.2/setup.py` & `mcrit-1.0.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,15 @@
     "smda>=1.3.0",
     "tqdm",
     "waitress",
 ]
 
 setup(
     name='mcrit',
-    version="1.0.2",
+    version="1.0.3",
     description='MCRIT is a framework created for simplified application of the MinHash algorithm to code similarity.',
     long_description_content_type="text/markdown",
     long_description=README,
     author='Daniel Plohmann, Manuel Blatt, Steffen Enders, Paul Hordiienko',
     author_email='daniel.plohmann@fkie.fraunhofer.de',
     url='https://github.com/danielplohmann/mcrit',
     license="NU General Public License v3 (GPLv3)",
```

