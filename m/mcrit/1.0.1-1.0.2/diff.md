# Comparing `tmp/mcrit-1.0.1.tar.gz` & `tmp/mcrit-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mcrit-1.0.1.tar", last modified: Fri May 12 14:54:29 2023, max compression
+gzip compressed data, was "mcrit-1.0.2.tar", last modified: Mon May 22 12:13:28 2023, max compression
```

## Comparing `mcrit-1.0.1.tar` & `mcrit-1.0.2.tar`

### file list

```diff
@@ -1,84 +1,84 @@
-drwxrwxr-x   0 pnx       (1000) pnx       (1000)        0 2023-05-12 14:54:29.865078 mcrit-1.0.1/
--rw-rw-r--   0 pnx       (1000) pnx       (1000)    35149 2022-05-13 09:44:28.000000 mcrit-1.0.1/LICENSE
--rw-rw-r--   0 pnx       (1000) pnx       (1000)    12788 2023-05-12 14:54:29.865078 mcrit-1.0.1/PKG-INFO
--rw-rw-r--   0 pnx       (1000) pnx       (1000)    10451 2023-05-12 14:53:49.000000 mcrit-1.0.1/README.md
-drwxrwxr-x   0 pnx       (1000) pnx       (1000)        0 2023-05-12 14:54:29.857078 mcrit-1.0.1/mcrit/
--rw-rw-r--   0 pnx       (1000) pnx       (1000)    21415 2022-12-14 11:14:13.000000 mcrit-1.0.1/mcrit/Worker.py
--rw-rw-r--   0 pnx       (1000) pnx       (1000)        0 2022-05-13 09:44:28.000000 mcrit-1.0.1/mcrit/__init__.py
--rw-rw-r--   0 pnx       (1000) pnx       (1000)     1838 2023-03-21 09:06:40.000000 mcrit-1.0.1/mcrit/__main__.py
-drwxrwxr-x   0 pnx       (1000) pnx       (1000)        0 2023-05-12 14:54:29.857078 mcrit-1.0.1/mcrit/client/
--rw-rw-r--   0 pnx       (1000) pnx       (1000)    28489 2023-05-12 13:29:52.000000 mcrit-1.0.1/mcrit/client/McritClient.py
--rw-rw-r--   0 pnx       (1000) pnx       (1000)    17638 2023-04-10 16:19:48.000000 mcrit-1.0.1/mcrit/client/McritConsole.py
--rw-rw-r--   0 pnx       (1000) pnx       (1000)        0 2022-05-13 09:44:28.000000 mcrit-1.0.1/mcrit/client/__init__.py
-drwxrwxr-x   0 pnx       (1000) pnx       (1000)        0 2023-05-12 14:54:29.861078 mcrit-1.0.1/mcrit/config/
--rw-rw-r--   0 pnx       (1000) pnx       (1000)      855 2022-05-13 09:44:28.000000 mcrit-1.0.1/mcrit/config/ConfigInterface.py
--rw-rw-r--   0 pnx       (1000) pnx       (1000)      960 2023-05-12 14:54:03.000000 mcrit-1.0.1/mcrit/config/McritConfig.py
--rw-rw-r--   0 pnx       (1000) pnx       (1000)     2148 2023-04-10 15:53:10.000000 mcrit-1.0.1/mcrit/config/MinHashConfig.py
--rw-rw-r--   0 pnx       (1000) pnx       (1000)      821 2022-05-13 09:44:28.000000 mcrit-1.0.1/mcrit/config/QueueConfig.py
--rw-rw-r--   0 pnx       (1000) pnx       (1000)     1974 2022-05-13 09:44:28.000000 mcrit-1.0.1/mcrit/config/ShinglerConfig.py
--rw-rw-r--   0 pnx       (1000) pnx       (1000)     1775 2022-07-29 10:29:16.000000 mcrit-1.0.1/mcrit/config/StorageConfig.py
--rw-rw-r--   0 pnx       (1000) pnx       (1000)        0 2022-05-13 09:44:28.000000 mcrit-1.0.1/mcrit/config/__init__.py
-drwxrwxr-x   0 pnx       (1000) pnx       (1000)        0 2023-05-12 14:54:29.861078 mcrit-1.0.1/mcrit/index/
--rw-rw-r--   0 pnx       (1000) pnx       (1000)    29120 2023-04-26 15:34:26.000000 mcrit-1.0.1/mcrit/index/MinHashIndex.py
--rw-rw-r--   0 pnx       (1000) pnx       (1000)     3890 2022-08-08 11:41:38.000000 mcrit-1.0.1/mcrit/index/SearchCursor.py
--rw-rw-r--   0 pnx       (1000) pnx       (1000)     6210 2022-08-08 11:41:38.000000 mcrit-1.0.1/mcrit/index/SearchQueryParser.py
--rw-rw-r--   0 pnx       (1000) pnx       (1000)     6366 2022-08-08 11:41:38.000000 mcrit-1.0.1/mcrit/index/SearchQueryTree.py
--rw-rw-r--   0 pnx       (1000) pnx       (1000)        0 2022-05-13 09:44:28.000000 mcrit-1.0.1/mcrit/index/__init__.py
-drwxrwxr-x   0 pnx       (1000) pnx       (1000)        0 2023-05-12 14:54:29.861078 mcrit-1.0.1/mcrit/libs/
--rw-rw-r--   0 pnx       (1000) pnx       (1000)        0 2022-05-13 09:44:28.000000 mcrit-1.0.1/mcrit/libs/__init__.py
--rw-rw-r--   0 pnx       (1000) pnx       (1000)    16784 2022-08-23 11:53:24.000000 mcrit-1.0.1/mcrit/libs/mongoqueue.py
--rw-rw-r--   0 pnx       (1000) pnx       (1000)    14152 2022-05-13 09:44:28.000000 mcrit-1.0.1/mcrit/libs/pymmh3.py
--rw-rw-r--   0 pnx       (1000) pnx       (1000)     2028 2022-05-13 09:44:28.000000 mcrit-1.0.1/mcrit/libs/utility.py
-drwxrwxr-x   0 pnx       (1000) pnx       (1000)        0 2023-05-12 14:54:29.861078 mcrit-1.0.1/mcrit/matchers/
--rw-rw-r--   0 pnx       (1000) pnx       (1000)     6378 2022-08-31 07:13:17.000000 mcrit-1.0.1/mcrit/matchers/MatcherCross.py
--rw-rw-r--   0 pnx       (1000) pnx       (1000)    28260 2023-04-10 15:53:10.000000 mcrit-1.0.1/mcrit/matchers/MatcherInterface.py
--rw-rw-r--   0 pnx       (1000) pnx       (1000)     3014 2022-11-25 14:50:57.000000 mcrit-1.0.1/mcrit/matchers/MatcherQuery.py
--rw-rw-r--   0 pnx       (1000) pnx       (1000)     3097 2023-04-10 15:53:10.000000 mcrit-1.0.1/mcrit/matchers/MatcherQueryFunction.py
--rw-rw-r--   0 pnx       (1000) pnx       (1000)      751 2022-09-28 13:53:00.000000 mcrit-1.0.1/mcrit/matchers/MatcherSample.py
--rw-rw-r--   0 pnx       (1000) pnx       (1000)     2429 2022-12-14 11:14:13.000000 mcrit-1.0.1/mcrit/matchers/MatcherVs.py
--rw-rw-r--   0 pnx       (1000) pnx       (1000)        0 2022-08-29 06:59:30.000000 mcrit-1.0.1/mcrit/matchers/__init__.py
-drwxrwxr-x   0 pnx       (1000) pnx       (1000)        0 2023-05-12 14:54:29.865078 mcrit-1.0.1/mcrit/minhash/
--rw-rw-r--   0 pnx       (1000) pnx       (1000)     3662 2022-05-13 09:44:28.000000 mcrit-1.0.1/mcrit/minhash/MinHash.py
--rw-rw-r--   0 pnx       (1000) pnx       (1000)    10547 2022-11-11 10:02:06.000000 mcrit-1.0.1/mcrit/minhash/MinHasher.py
--rw-rw-r--   0 pnx       (1000) pnx       (1000)     3212 2022-05-13 09:44:28.000000 mcrit-1.0.1/mcrit/minhash/ShingleLoader.py
--rw-rw-r--   0 pnx       (1000) pnx       (1000)        0 2022-05-13 09:44:28.000000 mcrit-1.0.1/mcrit/minhash/__init__.py
-drwxrwxr-x   0 pnx       (1000) pnx       (1000)        0 2023-05-12 14:54:29.865078 mcrit-1.0.1/mcrit/queue/
--rw-rw-r--   0 pnx       (1000) pnx       (1000)    10980 2022-08-31 07:13:17.000000 mcrit-1.0.1/mcrit/queue/LocalQueue.py
--rw-rw-r--   0 pnx       (1000) pnx       (1000)     1308 2022-05-13 09:44:28.000000 mcrit-1.0.1/mcrit/queue/QueueFactory.py
--rw-rw-r--   0 pnx       (1000) pnx       (1000)    14987 2022-10-12 12:19:42.000000 mcrit-1.0.1/mcrit/queue/QueueRemoteCalls.py
--rw-rw-r--   0 pnx       (1000) pnx       (1000)        0 2022-08-29 06:36:44.000000 mcrit-1.0.1/mcrit/queue/__init__.py
-drwxrwxr-x   0 pnx       (1000) pnx       (1000)        0 2023-05-12 14:54:29.865078 mcrit-1.0.1/mcrit/server/
--rw-rw-r--   0 pnx       (1000) pnx       (1000)     1297 2023-03-21 14:19:34.000000 mcrit-1.0.1/mcrit/server/BlocksResource.py
--rw-rw-r--   0 pnx       (1000) pnx       (1000)     6004 2023-03-21 14:19:34.000000 mcrit-1.0.1/mcrit/server/FamilyResource.py
--rw-rw-r--   0 pnx       (1000) pnx       (1000)     3764 2023-05-12 13:35:06.000000 mcrit-1.0.1/mcrit/server/FunctionResource.py
--rw-rw-r--   0 pnx       (1000) pnx       (1000)     4609 2023-03-21 14:19:34.000000 mcrit-1.0.1/mcrit/server/JobResource.py
--rw-rw-r--   0 pnx       (1000) pnx       (1000)     3551 2023-03-21 14:19:34.000000 mcrit-1.0.1/mcrit/server/MatchResource.py
--rw-rw-r--   0 pnx       (1000) pnx       (1000)     7608 2023-03-22 15:50:20.000000 mcrit-1.0.1/mcrit/server/QueryResource.py
--rw-rw-r--   0 pnx       (1000) pnx       (1000)    11793 2023-03-21 14:19:34.000000 mcrit-1.0.1/mcrit/server/SampleResource.py
--rw-rw-r--   0 pnx       (1000) pnx       (1000)     5159 2023-03-21 14:19:34.000000 mcrit-1.0.1/mcrit/server/StatusResource.py
--rw-rw-r--   0 pnx       (1000) pnx       (1000)        0 2022-05-13 09:44:28.000000 mcrit-1.0.1/mcrit/server/__init__.py
--rw-rw-r--   0 pnx       (1000) pnx       (1000)     5887 2023-03-17 17:07:42.000000 mcrit-1.0.1/mcrit/server/application_routes.py
--rw-rw-r--   0 pnx       (1000) pnx       (1000)     1868 2023-03-21 14:19:34.000000 mcrit-1.0.1/mcrit/server/utils.py
--rw-rw-r--   0 pnx       (1000) pnx       (1000)       69 2022-05-13 09:44:28.000000 mcrit-1.0.1/mcrit/server/wsgi.py
-drwxrwxr-x   0 pnx       (1000) pnx       (1000)        0 2023-05-12 14:54:29.865078 mcrit-1.0.1/mcrit/storage/
--rw-rw-r--   0 pnx       (1000) pnx       (1000)     2077 2022-08-03 10:24:19.000000 mcrit-1.0.1/mcrit/storage/FamilyEntry.py
--rw-rw-r--   0 pnx       (1000) pnx       (1000)     6415 2023-03-21 14:19:34.000000 mcrit-1.0.1/mcrit/storage/FunctionEntry.py
--rw-rw-r--   0 pnx       (1000) pnx       (1000)     1661 2023-03-21 14:19:34.000000 mcrit-1.0.1/mcrit/storage/FunctionLabelEntry.py
--rw-rw-r--   0 pnx       (1000) pnx       (1000)     2764 2023-02-27 12:31:29.000000 mcrit-1.0.1/mcrit/storage/MatchedFunctionEntry.py
--rw-rw-r--   0 pnx       (1000) pnx       (1000)     6617 2023-02-14 15:17:18.000000 mcrit-1.0.1/mcrit/storage/MatchedSampleEntry.py
--rw-rw-r--   0 pnx       (1000) pnx       (1000)     1389 2023-04-10 15:53:10.000000 mcrit-1.0.1/mcrit/storage/MatchingCache.py
--rw-rw-r--   0 pnx       (1000) pnx       (1000)    21812 2023-05-08 07:42:59.000000 mcrit-1.0.1/mcrit/storage/MatchingResult.py
--rw-rw-r--   0 pnx       (1000) pnx       (1000)    44811 2023-03-24 15:01:21.000000 mcrit-1.0.1/mcrit/storage/MemoryStorage.py
--rw-rw-r--   0 pnx       (1000) pnx       (1000)    59597 2023-04-26 15:32:48.000000 mcrit-1.0.1/mcrit/storage/MongoDbStorage.py
--rw-rw-r--   0 pnx       (1000) pnx       (1000)     4932 2023-03-17 17:07:42.000000 mcrit-1.0.1/mcrit/storage/SampleEntry.py
--rw-rw-r--   0 pnx       (1000) pnx       (1000)      735 2022-11-13 10:29:45.000000 mcrit-1.0.1/mcrit/storage/StorageFactory.py
--rw-rw-r--   0 pnx       (1000) pnx       (1000)    25158 2023-03-21 14:19:34.000000 mcrit-1.0.1/mcrit/storage/StorageInterface.py
--rw-rw-r--   0 pnx       (1000) pnx       (1000)        0 2022-05-13 09:44:28.000000 mcrit-1.0.1/mcrit/storage/__init__.py
-drwxrwxr-x   0 pnx       (1000) pnx       (1000)        0 2023-05-12 14:54:29.857078 mcrit-1.0.1/mcrit.egg-info/
--rw-rw-r--   0 pnx       (1000) pnx       (1000)    12788 2023-05-12 14:54:29.000000 mcrit-1.0.1/mcrit.egg-info/PKG-INFO
--rw-rw-r--   0 pnx       (1000) pnx       (1000)     1950 2023-05-12 14:54:29.000000 mcrit-1.0.1/mcrit.egg-info/SOURCES.txt
--rw-rw-r--   0 pnx       (1000) pnx       (1000)        1 2023-05-12 14:54:29.000000 mcrit-1.0.1/mcrit.egg-info/dependency_links.txt
--rw-rw-r--   0 pnx       (1000) pnx       (1000)      135 2023-05-12 14:54:29.000000 mcrit-1.0.1/mcrit.egg-info/requires.txt
--rw-rw-r--   0 pnx       (1000) pnx       (1000)        6 2023-05-12 14:54:29.000000 mcrit-1.0.1/mcrit.egg-info/top_level.txt
--rw-rw-r--   0 pnx       (1000) pnx       (1000)       38 2023-05-12 14:54:29.865078 mcrit-1.0.1/setup.cfg
--rw-rw-r--   0 pnx       (1000) pnx       (1000)     1355 2023-05-12 14:53:08.000000 mcrit-1.0.1/setup.py
+drwxrwxr-x   0 analyst   (1000) analyst   (1000)        0 2023-05-22 12:13:28.331190 mcrit-1.0.2/
+-rw-rw-r--   0 analyst   (1000) analyst   (1000)    35149 2022-05-05 12:52:43.000000 mcrit-1.0.2/LICENSE
+-rw-rw-r--   0 analyst   (1000) analyst   (1000)    11397 2023-05-22 12:13:28.331190 mcrit-1.0.2/PKG-INFO
+-rw-rw-r--   0 analyst   (1000) analyst   (1000)    10645 2023-05-22 12:12:35.000000 mcrit-1.0.2/README.md
+drwxrwxr-x   0 analyst   (1000) analyst   (1000)        0 2023-05-22 12:13:28.327190 mcrit-1.0.2/mcrit/
+-rw-rw-r--   0 analyst   (1000) analyst   (1000)    21415 2022-12-13 15:03:46.000000 mcrit-1.0.2/mcrit/Worker.py
+-rw-rw-r--   0 analyst   (1000) analyst   (1000)        0 2022-02-03 10:05:12.000000 mcrit-1.0.2/mcrit/__init__.py
+-rw-rw-r--   0 analyst   (1000) analyst   (1000)     1838 2023-03-16 12:54:37.000000 mcrit-1.0.2/mcrit/__main__.py
+drwxrwxr-x   0 analyst   (1000) analyst   (1000)        0 2023-05-22 12:13:28.327190 mcrit-1.0.2/mcrit/client/
+-rw-rw-r--   0 analyst   (1000) analyst   (1000)    28489 2023-05-22 08:41:11.000000 mcrit-1.0.2/mcrit/client/McritClient.py
+-rw-rw-r--   0 analyst   (1000) analyst   (1000)    18233 2023-05-22 12:10:34.000000 mcrit-1.0.2/mcrit/client/McritConsole.py
+-rw-rw-r--   0 analyst   (1000) analyst   (1000)        0 2022-02-03 10:05:12.000000 mcrit-1.0.2/mcrit/client/__init__.py
+drwxrwxr-x   0 analyst   (1000) analyst   (1000)        0 2023-05-22 12:13:28.327190 mcrit-1.0.2/mcrit/config/
+-rw-rw-r--   0 analyst   (1000) analyst   (1000)      855 2022-02-03 10:05:12.000000 mcrit-1.0.2/mcrit/config/ConfigInterface.py
+-rw-rw-r--   0 analyst   (1000) analyst   (1000)      960 2023-05-22 12:12:44.000000 mcrit-1.0.2/mcrit/config/McritConfig.py
+-rw-rw-r--   0 analyst   (1000) analyst   (1000)     2148 2023-05-22 08:41:11.000000 mcrit-1.0.2/mcrit/config/MinHashConfig.py
+-rw-rw-r--   0 analyst   (1000) analyst   (1000)      821 2022-02-03 10:05:12.000000 mcrit-1.0.2/mcrit/config/QueueConfig.py
+-rw-rw-r--   0 analyst   (1000) analyst   (1000)     1974 2022-02-08 09:50:02.000000 mcrit-1.0.2/mcrit/config/ShinglerConfig.py
+-rw-rw-r--   0 analyst   (1000) analyst   (1000)     1775 2022-08-15 15:05:19.000000 mcrit-1.0.2/mcrit/config/StorageConfig.py
+-rw-rw-r--   0 analyst   (1000) analyst   (1000)        0 2022-02-03 10:05:12.000000 mcrit-1.0.2/mcrit/config/__init__.py
+drwxrwxr-x   0 analyst   (1000) analyst   (1000)        0 2023-05-22 12:13:28.327190 mcrit-1.0.2/mcrit/index/
+-rw-rw-r--   0 analyst   (1000) analyst   (1000)    29120 2023-05-22 08:41:11.000000 mcrit-1.0.2/mcrit/index/MinHashIndex.py
+-rw-rw-r--   0 analyst   (1000) analyst   (1000)     3890 2022-08-16 08:15:37.000000 mcrit-1.0.2/mcrit/index/SearchCursor.py
+-rw-rw-r--   0 analyst   (1000) analyst   (1000)     6210 2022-08-16 08:15:37.000000 mcrit-1.0.2/mcrit/index/SearchQueryParser.py
+-rw-rw-r--   0 analyst   (1000) analyst   (1000)     6366 2022-08-16 08:15:37.000000 mcrit-1.0.2/mcrit/index/SearchQueryTree.py
+-rw-rw-r--   0 analyst   (1000) analyst   (1000)        0 2022-02-03 10:05:12.000000 mcrit-1.0.2/mcrit/index/__init__.py
+drwxrwxr-x   0 analyst   (1000) analyst   (1000)        0 2023-05-22 12:13:28.327190 mcrit-1.0.2/mcrit/libs/
+-rw-rw-r--   0 analyst   (1000) analyst   (1000)        0 2022-02-03 10:05:12.000000 mcrit-1.0.2/mcrit/libs/__init__.py
+-rw-rw-r--   0 analyst   (1000) analyst   (1000)    16784 2022-09-01 07:23:47.000000 mcrit-1.0.2/mcrit/libs/mongoqueue.py
+-rw-rw-r--   0 analyst   (1000) analyst   (1000)    14152 2022-02-03 10:05:12.000000 mcrit-1.0.2/mcrit/libs/pymmh3.py
+-rw-rw-r--   0 analyst   (1000) analyst   (1000)     2028 2022-02-08 13:06:39.000000 mcrit-1.0.2/mcrit/libs/utility.py
+drwxrwxr-x   0 analyst   (1000) analyst   (1000)        0 2023-05-22 12:13:28.331190 mcrit-1.0.2/mcrit/matchers/
+-rw-rw-r--   0 analyst   (1000) analyst   (1000)     6378 2022-09-01 07:23:47.000000 mcrit-1.0.2/mcrit/matchers/MatcherCross.py
+-rw-rw-r--   0 analyst   (1000) analyst   (1000)    28260 2023-05-22 08:41:11.000000 mcrit-1.0.2/mcrit/matchers/MatcherInterface.py
+-rw-rw-r--   0 analyst   (1000) analyst   (1000)     3014 2022-12-13 12:02:29.000000 mcrit-1.0.2/mcrit/matchers/MatcherQuery.py
+-rw-rw-r--   0 analyst   (1000) analyst   (1000)     3097 2023-05-22 08:41:11.000000 mcrit-1.0.2/mcrit/matchers/MatcherQueryFunction.py
+-rw-rw-r--   0 analyst   (1000) analyst   (1000)      751 2022-09-29 07:21:37.000000 mcrit-1.0.2/mcrit/matchers/MatcherSample.py
+-rw-rw-r--   0 analyst   (1000) analyst   (1000)     2429 2022-12-13 15:01:23.000000 mcrit-1.0.2/mcrit/matchers/MatcherVs.py
+-rw-rw-r--   0 analyst   (1000) analyst   (1000)        0 2022-09-01 07:23:47.000000 mcrit-1.0.2/mcrit/matchers/__init__.py
+drwxrwxr-x   0 analyst   (1000) analyst   (1000)        0 2023-05-22 12:13:28.331190 mcrit-1.0.2/mcrit/minhash/
+-rw-rw-r--   0 analyst   (1000) analyst   (1000)     3662 2022-02-03 10:05:12.000000 mcrit-1.0.2/mcrit/minhash/MinHash.py
+-rw-rw-r--   0 analyst   (1000) analyst   (1000)    10547 2022-11-15 08:15:21.000000 mcrit-1.0.2/mcrit/minhash/MinHasher.py
+-rw-rw-r--   0 analyst   (1000) analyst   (1000)     3212 2022-02-03 10:05:12.000000 mcrit-1.0.2/mcrit/minhash/ShingleLoader.py
+-rw-rw-r--   0 analyst   (1000) analyst   (1000)        0 2022-02-03 10:05:12.000000 mcrit-1.0.2/mcrit/minhash/__init__.py
+drwxrwxr-x   0 analyst   (1000) analyst   (1000)        0 2023-05-22 12:13:28.331190 mcrit-1.0.2/mcrit/queue/
+-rw-rw-r--   0 analyst   (1000) analyst   (1000)    10980 2022-09-01 07:23:47.000000 mcrit-1.0.2/mcrit/queue/LocalQueue.py
+-rw-rw-r--   0 analyst   (1000) analyst   (1000)     1308 2022-02-03 10:05:12.000000 mcrit-1.0.2/mcrit/queue/QueueFactory.py
+-rw-rw-r--   0 analyst   (1000) analyst   (1000)    14987 2022-10-13 09:02:52.000000 mcrit-1.0.2/mcrit/queue/QueueRemoteCalls.py
+-rw-rw-r--   0 analyst   (1000) analyst   (1000)        0 2022-09-01 07:23:47.000000 mcrit-1.0.2/mcrit/queue/__init__.py
+drwxrwxr-x   0 analyst   (1000) analyst   (1000)        0 2023-05-22 12:13:28.331190 mcrit-1.0.2/mcrit/server/
+-rw-rw-r--   0 analyst   (1000) analyst   (1000)     1297 2023-03-29 07:45:34.000000 mcrit-1.0.2/mcrit/server/BlocksResource.py
+-rw-rw-r--   0 analyst   (1000) analyst   (1000)     6004 2023-03-29 07:45:34.000000 mcrit-1.0.2/mcrit/server/FamilyResource.py
+-rw-rw-r--   0 analyst   (1000) analyst   (1000)     3764 2023-05-22 08:41:11.000000 mcrit-1.0.2/mcrit/server/FunctionResource.py
+-rw-rw-r--   0 analyst   (1000) analyst   (1000)     4609 2023-03-29 07:45:34.000000 mcrit-1.0.2/mcrit/server/JobResource.py
+-rw-rw-r--   0 analyst   (1000) analyst   (1000)     3551 2023-03-29 07:45:34.000000 mcrit-1.0.2/mcrit/server/MatchResource.py
+-rw-rw-r--   0 analyst   (1000) analyst   (1000)     7608 2023-03-29 07:45:34.000000 mcrit-1.0.2/mcrit/server/QueryResource.py
+-rw-rw-r--   0 analyst   (1000) analyst   (1000)    11793 2023-03-29 07:45:34.000000 mcrit-1.0.2/mcrit/server/SampleResource.py
+-rw-rw-r--   0 analyst   (1000) analyst   (1000)     5159 2023-03-29 07:45:34.000000 mcrit-1.0.2/mcrit/server/StatusResource.py
+-rw-rw-r--   0 analyst   (1000) analyst   (1000)        0 2022-02-03 10:05:12.000000 mcrit-1.0.2/mcrit/server/__init__.py
+-rw-rw-r--   0 analyst   (1000) analyst   (1000)     5887 2023-03-29 07:45:34.000000 mcrit-1.0.2/mcrit/server/application_routes.py
+-rw-rw-r--   0 analyst   (1000) analyst   (1000)     1868 2023-03-29 07:45:34.000000 mcrit-1.0.2/mcrit/server/utils.py
+-rw-rw-r--   0 analyst   (1000) analyst   (1000)       69 2022-02-03 10:05:12.000000 mcrit-1.0.2/mcrit/server/wsgi.py
+drwxrwxr-x   0 analyst   (1000) analyst   (1000)        0 2023-05-22 12:13:28.331190 mcrit-1.0.2/mcrit/storage/
+-rw-rw-r--   0 analyst   (1000) analyst   (1000)     2077 2022-08-15 15:05:19.000000 mcrit-1.0.2/mcrit/storage/FamilyEntry.py
+-rw-rw-r--   0 analyst   (1000) analyst   (1000)     6415 2023-03-29 07:45:34.000000 mcrit-1.0.2/mcrit/storage/FunctionEntry.py
+-rw-rw-r--   0 analyst   (1000) analyst   (1000)     1661 2023-03-29 07:45:34.000000 mcrit-1.0.2/mcrit/storage/FunctionLabelEntry.py
+-rw-rw-r--   0 analyst   (1000) analyst   (1000)     2764 2022-12-13 13:23:45.000000 mcrit-1.0.2/mcrit/storage/MatchedFunctionEntry.py
+-rw-rw-r--   0 analyst   (1000) analyst   (1000)     6617 2023-03-16 12:54:37.000000 mcrit-1.0.2/mcrit/storage/MatchedSampleEntry.py
+-rw-rw-r--   0 analyst   (1000) analyst   (1000)     1389 2023-05-22 08:41:11.000000 mcrit-1.0.2/mcrit/storage/MatchingCache.py
+-rw-rw-r--   0 analyst   (1000) analyst   (1000)    21812 2023-03-16 12:54:37.000000 mcrit-1.0.2/mcrit/storage/MatchingResult.py
+-rw-rw-r--   0 analyst   (1000) analyst   (1000)    44811 2023-05-22 08:41:03.000000 mcrit-1.0.2/mcrit/storage/MemoryStorage.py
+-rw-rw-r--   0 analyst   (1000) analyst   (1000)    59597 2023-05-22 08:41:11.000000 mcrit-1.0.2/mcrit/storage/MongoDbStorage.py
+-rw-rw-r--   0 analyst   (1000) analyst   (1000)     4932 2023-03-29 07:45:34.000000 mcrit-1.0.2/mcrit/storage/SampleEntry.py
+-rw-rw-r--   0 analyst   (1000) analyst   (1000)      735 2022-11-15 08:15:21.000000 mcrit-1.0.2/mcrit/storage/StorageFactory.py
+-rw-rw-r--   0 analyst   (1000) analyst   (1000)    25158 2023-03-29 07:45:34.000000 mcrit-1.0.2/mcrit/storage/StorageInterface.py
+-rw-rw-r--   0 analyst   (1000) analyst   (1000)        0 2022-02-03 10:05:12.000000 mcrit-1.0.2/mcrit/storage/__init__.py
+drwxrwxr-x   0 analyst   (1000) analyst   (1000)        0 2023-05-22 12:13:28.327190 mcrit-1.0.2/mcrit.egg-info/
+-rw-rw-r--   0 analyst   (1000) analyst   (1000)    11397 2023-05-22 12:13:28.000000 mcrit-1.0.2/mcrit.egg-info/PKG-INFO
+-rw-rw-r--   0 analyst   (1000) analyst   (1000)     1950 2023-05-22 12:13:28.000000 mcrit-1.0.2/mcrit.egg-info/SOURCES.txt
+-rw-rw-r--   0 analyst   (1000) analyst   (1000)        1 2023-05-22 12:13:28.000000 mcrit-1.0.2/mcrit.egg-info/dependency_links.txt
+-rw-rw-r--   0 analyst   (1000) analyst   (1000)      135 2023-05-22 12:13:28.000000 mcrit-1.0.2/mcrit.egg-info/requires.txt
+-rw-rw-r--   0 analyst   (1000) analyst   (1000)        6 2023-05-22 12:13:28.000000 mcrit-1.0.2/mcrit.egg-info/top_level.txt
+-rw-rw-r--   0 analyst   (1000) analyst   (1000)       38 2023-05-22 12:13:28.331190 mcrit-1.0.2/setup.cfg
+-rw-rw-r--   0 analyst   (1000) analyst   (1000)     1355 2023-05-22 12:12:01.000000 mcrit-1.0.2/setup.py
```

### Comparing `mcrit-1.0.1/LICENSE` & `mcrit-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `mcrit-1.0.1/PKG-INFO` & `mcrit-1.0.2/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,214 +1,217 @@
 Metadata-Version: 2.1
 Name: mcrit
-Version: 1.0.1
+Version: 1.0.2
 Summary: MCRIT is a framework created for simplified application of the MinHash algorithm to code similarity.
 Home-page: https://github.com/danielplohmann/mcrit
 Author: Daniel Plohmann, Manuel Blatt, Steffen Enders, Paul Hordiienko
 Author-email: daniel.plohmann@fkie.fraunhofer.de
 License: NU General Public License v3 (GPLv3)
-Description: # MinHash-based Code Relationship & Investigation Toolkit (MCRIT)
-        [![Test](https://github.com/danielplohmann/mcrit/actions/workflows/test.yml/badge.svg)](https://github.com/danielplohmann/mcrit/actions/workflows/test.yml)
-        
-        MCRIT is a framework created to simplify the application of the MinHash algorithm in the context of code similarity.
-        It can be used to rapidly implement "shinglers", i.e. methods which encode properties of disassembled functions, to then be used for similarity estimation via the MinHash algorithm.
-        It is tailored to work with disassembly reports emitted by [SMDA](https://github.com/danielplohmann/smda).
-        
-        ## Usage
-        
-        ### Dockerized Usage
-        
-        We highly recommend to use the fully packaged [docker-mcrit](https://github.com/danielplohmann/docker-mcrit) for trivial deployment and usage.  
-        First and foremost, this will ensure that you have fully compatible versions across all components, including a database for persistence and a web frontend for convenient interaction.
-        
-        ### Standalone Usage
-        
-        Installing MCRIT on its own will require some more steps.  
-        For the following, we assume Ubuntu as host operating system.
-        
-        The Python installation requirements are listed in `requirements.txt` and can be installed using:
-        
-        ```bash
-        # install python and MCRIT dependencies
-        $ sudo apt install python3 python3-pip
-        $ pip install -r requirements.txt 
-        ```
-        
-        By default, MongoDB 5.0 is used as backend, which is also the recommended mode of operation as it provides a persistent data storage.
-        The following commands outline an example installation on Ubuntu:
-        ```bash
-        # fetch mongodb signing key
-        $ sudo apt-get install gnupg
-        $ wget -qO - https://www.mongodb.org/static/pgp/server-5.0.asc | sudo apt-key add -
-        # add package repository (Ubuntu 22.04)
-        $ echo "deb [ arch=amd64,arm64 ] https://repo.mongodb.org/apt/ubuntu jammy/mongodb-org/5.0 multiverse" | sudo tee /etc/apt/sources.list.d/mongodb-org-5.0.list
-        # OR add package repository (Ubuntu 20.04)
-        $ echo "deb [ arch=amd64,arm64 ] https://repo.mongodb.org/apt/ubuntu focal/mongodb-org/5.0 multiverse" | sudo tee /etc/apt/sources.list.d/mongodb-org-5.0.list
-        # OR add package repository (Ubuntu 18.04)
-        $ echo "deb [ arch=amd64,arm64 ] https://repo.mongodb.org/apt/ubuntu bionic/mongodb-org/5.0 multiverse" | sudo tee /etc/apt/sources.list.d/mongodb-org-5.0.list
-        # install mongodb
-        $ sudo apt-get update
-        $ sudo apt-get install -y mongodb-org
-        # start mongodb as a service
-        $ sudo systemctl start mongod
-        # optionally configure to start the service with system startup
-        $ sudo systemctl enable mongod
-        ```
-        
-        When doing the standalone installation, you possibly want to install the MCRIT module based on the cloned repository, like so:
-        
-        ```bash
-        $ pip install -e .
-        ```
-        
-        After this initial installation and if desired, MCRIT can be used without an internet connection.
-        
-        
-        #### Operation
-        
-        The MCRIT backend is generally divided into two components, a server providing an API interface to work with and one or more workers processing queued jobs.
-        They can be started in seperate shells using:
-        
-        ```bash
-        $ python -m mcrit server
-        ```
-        
-        and
-        
-        ```bash
-        $ python -m mcrit worker
-        ```
-        
-        By default, the REST API server will be listening on [http://127.0.0.1:8000/](http://127.0.0.1:8000/).
-        
-        
-        ## Interaction
-        
-        Regardless of your choice for installation, once running you can interact with the MCRIT backend.
-        
-        
-        ### MCRIT Client
-        
-        We have created a Python client module that is capable of working with all available endpoints of the server.  
-        Documentation for this client module is currently in development.
-        
-        ### MCRIT CLI
-        
-        There is also a CLI which is based on this client package, examples:
-        
-        ```bash
-        # query some stats of the data stored in the backend 
-        $ python -m mcrit client status
-        {'status': {'db_state': 187, 'storage_type': 'mongodb', 'num_bands': 20, 'num_samples': 137, 'num_families': 14, 'num_functions': 129110, 'num_pichashes': 25385}}
-        # submit a malware sample with filename sample_unpacked, using family name "some_family"
-        $ python -m mcrit client submit sample_unpacked -f some_family
-         1.039s -> (architecture: intel.32bit, base_addr: 0x10000000): 634 functions
-        ```
-        
-        ### MCRIT IDA Plugin
-        
-        An IDA plugin is also currently under development.
-        To use it, first create your own config.py and make required changes depending on the deployment of your MCRIT instance:
-        ```
-        cp ./plugins/ida/template.config.py ./plugins/ida/config.py
-        nano ./plugins/ida/config.py
-        ```
-        
-        Then simply run the script found at
-        
-        ```
-        ./plugins/ida/ida_mcrit.py
-        ```
-        
-        in IDA.
-        
-        
-        ## Version History
-         * 2023-05-12 v1.0.1: Some progress on label import for the IDA plugin. Reflected API extension of MCRITweb in McritClient.
-         * 2023-04-10 v1.0.0: Milestone release for Botconf 2023.
-         * 2023-04-10 v0.25.0: IDA plugin can now do function queries for the currently viewed function.
-         * 2023-03-24 v0.24.2: McritClient can forward username/apitoken, addJsonReport is now forwardable.
-         * 2023-03-21 v0.24.0: FunctionEntries now can store additional FunctionLabelEntries, along submitting user/date.
-         * 2023-03-17 v0.23.0: It is now possible to query matches for single SmdaFunctions (synchronously).
-         * 2023-03-15 v0.22.0: McritClient now supports apitokens and raw responses for a subset of functionality.
-         * 2023-03-14 v0.21.0: Backend support for more fine grained filtering.
-         * 2023-03-13 v0.20.6: Backend support for filtering family/sample by score in MatchResult.
-         * 2023-02-22 v0.20.4: Bugfix for calculating unique scores and accessing these results.
-         * 2023-02-21 v0.20.3: Supporting frontend capabilities with result presentation.
-         * 2023-02-17 v0.20.2: Extended match report object to support frontend improvements.
-         * 2023-02-14 v0.20.0: Overhauled console client to simplify shell-based interactions with the backend.
-         * 2023-01-12 v0.19.4: Additional filtering capabilities for MatchingResults.
-         * 2022-12-13 v0.19.1: It is now possible to require specific (higher) amounts of band matches for candidates (i.e. reduce fuzziness of matching).
-         * 2022-12-13 v0.18.x: Enable matching of arbitrary function IDs.
-         * 2022-11-25 v0.18.9: Accelerated Query matching.
-         * 2022-11-18 v0.18.8: Harmonized handling of deletion and modifications, minor fixes.
-         * 2022-11-13 v0.18.7: Drastically accelerated sample deletion.
-         * 2022-11-13 v0.18.6: Added functionality to modify existing sample and family information.
-         * 2022-11-11 v0.18.2: Upgrading matching procedure, should now be able to handle larger binaries more robustly and efficiently.
-         * 2022-11-03 v0.18.1: Minor fixes.
-         * 2022-11-03 v0.18.0: Unique block isolation now also generates a proposal for a YARA rule, restructured result output.
-         * 2022-10-24 v0.17.4: Harmonized setup.py with requirements, improved memory efficiency for processing cross jobs.
-         * 2022-10-18 v0.17.3: Added a convenience script to recursively produce SMDA reports from a semi-structured folder.
-         * 2022-10-13 v0.17.2: Fixed potential OOM issues during MinHash calculation by processing functions to be hashed in smaller batches.
-         * 2022-10-12 v0.17.1: Added a function to schedule a job that will ensure minhashes have been calculated for all samples/functions.
-         * 2022-10-11 v0.17.0: Search for unique blocks is now an asychronous job through the Worker.
-         * 2022-10-11 v0.16.0: Samples from MatchQuery jobs will now be stored with their Sample/FunctionEntries to allow better post processing.
-         * 2022-10-04 v0.15.4: Server can now display its version.
-         * 2022-09-28 v0.15.3: Addressing performance issues for bigger instances, generating escaped instruction sequence for unique blocks.
-         * 2022-09-26 v0.15.0: CrossJobs now in backend, started to provide functionality to identify unique basic blocks in samples.
-         * 2022-08-29 v0.14.2: Minor fixes for deployment.
-         * 2022-08-22 v0.14.0: Jobs can now depend on other jobs (preparation for moving crossjobs to backend), QoL improvements to job handling.
-         * 2022-08-17 v0.13.1: Added commandline option for profiling (requires cProfile).
-         * 2022-08-09 v0.13.0: Can now do efficient direct queries for PicHash and PicBlockHash matches.
-         * 2022-08-09 v0.12.3: Bugfix for FamilyEntry
-         * 2022-08-08 v0.12.2: Bugfix for delivery of XCFG data, added missing dependency.
-         * 2022-08-08 v0.12.0: Integrated Advanced Search syntax.
-         * 2022-08-03 v0.11.0: (BREAKING) Families are now represented with a FamilyEntry.
-         * 2022-08-03 v0.10.3: Now leaving function xcfg data by default in DB, exposed access to it via REST API and McritClient.
-         * 2022-07-29 v0.10.2: Added ability to delete families - now also keeping XCFG info for all functions by default.
-         * 2022-07-12 v0.10.1: Improved performance.
-         * 2022-07-12 v0.10.0: (BREAKING) Job handling simplified.
-         * 2022-05-13  v0.9.4: Bug fix for receiving submitted files.
-         * 2022-05-13  v0.9.3: Further updates to MatchingResults.
-         * 2022-05-13  v0.9.2: Added another field and more convenience functions in MatchingResult for better access - those are breaking changes for previously created MatchingResults.
-         * 2022-05-05  v0.9.1: Processing of binary submissions, minor fixes for minhash queuing - INITIAL RELEASE.
-         * 2022-02-09  v0.9.0: Added PicBlocks to MCRIT.
-         * 2022-01-19  v0.8.0: Migrated the client and the examples into the primary MCRIT repository.
-         * 2021-12-16  v0.7.0: Initial private release.
-        
-        ## Credits & Notes
-        
-        Thanks to Steffen Enders and Paul Hordiienko for their contributions to the internal research prototype of this project!
-        Thanks to Manuel Blatt for his extensive contributions to and refactorings of this project as well as for the client module!
-        
-        Pull requests welcome! :)
-        
-        ## License
-        ```
-            MinHash-based Code Relationship & Investigation Toolkit (MCRIT)
-            Copyright (C) 2022  Daniel Plohmann, Manuel Blatt
-        
-            This program is free software: you can redistribute it and/or modify
-            it under the terms of the GNU General Public License as published by
-            the Free Software Foundation, either version 3 of the License, or
-            (at your option) any later version.
-        
-            This program is distributed in the hope that it will be useful,
-            but WITHOUT ANY WARRANTY; without even the implied warranty of
-            MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-            GNU General Public License for more details.
-        
-            You should have received a copy of the GNU General Public License
-            along with this program.  If not, see <http://www.gnu.org/licenses/>.
-            
-            Some plug-ins and libraries may have different licenses. 
-            If so, a license file is provided in the plug-in's folder.
-        ```
-        
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Security
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# MinHash-based Code Relationship & Investigation Toolkit (MCRIT)
+[![Test](https://github.com/danielplohmann/mcrit/actions/workflows/test.yml/badge.svg)](https://github.com/danielplohmann/mcrit/actions/workflows/test.yml)
+
+MCRIT is a framework created to simplify the application of the MinHash algorithm in the context of code similarity.
+It can be used to rapidly implement "shinglers", i.e. methods which encode properties of disassembled functions, to then be used for similarity estimation via the MinHash algorithm.
+It is tailored to work with disassembly reports emitted by [SMDA](https://github.com/danielplohmann/smda).
+
+## Usage
+
+### Dockerized Usage
+
+We highly recommend to use the fully packaged [docker-mcrit](https://github.com/danielplohmann/docker-mcrit) for trivial deployment and usage.  
+First and foremost, this will ensure that you have fully compatible versions across all components, including a database for persistence and a web frontend for convenient interaction.
+
+### Standalone Usage
+
+Installing MCRIT on its own will require some more steps.  
+For the following, we assume Ubuntu as host operating system.
+
+The Python installation requirements are listed in `requirements.txt` and can be installed using:
+
+```bash
+# install python and MCRIT dependencies
+$ sudo apt install python3 python3-pip
+$ pip install -r requirements.txt 
+```
+
+By default, MongoDB 5.0 is used as backend, which is also the recommended mode of operation as it provides a persistent data storage.
+The following commands outline an example installation on Ubuntu:
+```bash
+# fetch mongodb signing key
+$ sudo apt-get install gnupg
+$ wget -qO - https://www.mongodb.org/static/pgp/server-5.0.asc | sudo apt-key add -
+# add package repository (Ubuntu 22.04)
+$ echo "deb [ arch=amd64,arm64 ] https://repo.mongodb.org/apt/ubuntu jammy/mongodb-org/5.0 multiverse" | sudo tee /etc/apt/sources.list.d/mongodb-org-5.0.list
+# OR add package repository (Ubuntu 20.04)
+$ echo "deb [ arch=amd64,arm64 ] https://repo.mongodb.org/apt/ubuntu focal/mongodb-org/5.0 multiverse" | sudo tee /etc/apt/sources.list.d/mongodb-org-5.0.list
+# OR add package repository (Ubuntu 18.04)
+$ echo "deb [ arch=amd64,arm64 ] https://repo.mongodb.org/apt/ubuntu bionic/mongodb-org/5.0 multiverse" | sudo tee /etc/apt/sources.list.d/mongodb-org-5.0.list
+# install mongodb
+$ sudo apt-get update
+$ sudo apt-get install -y mongodb-org
+# start mongodb as a service
+$ sudo systemctl start mongod
+# optionally configure to start the service with system startup
+$ sudo systemctl enable mongod
+```
+
+When doing the standalone installation, you possibly want to install the MCRIT module based on the cloned repository, like so:
+
+```bash
+$ pip install -e .
+```
+
+After this initial installation and if desired, MCRIT can be used without an internet connection.
+
+
+#### Operation
+
+The MCRIT backend is generally divided into two components, a server providing an API interface to work with and one or more workers processing queued jobs.
+They can be started in seperate shells using:
+
+```bash
+$ python -m mcrit server
+```
+
+and
+
+```bash
+$ python -m mcrit worker
+```
+
+By default, the REST API server will be listening on [http://127.0.0.1:8000/](http://127.0.0.1:8000/).
+
+
+## Interaction
+
+Regardless of your choice for installation, once running you can interact with the MCRIT backend.
+
+
+### MCRIT Client
+
+We have created a Python client module that is capable of working with all available endpoints of the server.  
+Documentation for this client module is currently in development.
+
+### MCRIT CLI
+
+There is also a CLI which is based on this client package, examples:
+
+```bash
+# query some stats of the data stored in the backend 
+$ python -m mcrit client status
+{'status': {'db_state': 187, 'storage_type': 'mongodb', 'num_bands': 20, 'num_samples': 137, 'num_families': 14, 'num_functions': 129110, 'num_pichashes': 25385}}
+# submit a malware sample with filename sample_unpacked, using family name "some_family"
+$ python -m mcrit client submit sample_unpacked -f some_family
+ 1.039s -> (architecture: intel.32bit, base_addr: 0x10000000): 634 functions
+```
+
+A more extensive documentation of the MCRIT CLI is available [here](docs/mcrit-cli.md)
+
+### MCRIT IDA Plugin
+
+An IDA plugin is also currently under development.
+To use it, first create your own config.py and make required changes depending on the deployment of your MCRIT instance:
+```
+cp ./plugins/ida/template.config.py ./plugins/ida/config.py
+nano ./plugins/ida/config.py
+```
+
+Then simply run the script found at
+
+```
+./plugins/ida/ida_mcrit.py
+```
+
+in IDA.
+
+
+## Version History
+ * 2023-05-22 v1.0.2: More robustness for path verification when using MCRIT CLI on Malpedia repo folder.
+ * 2023-05-12 v1.0.1: Some progress on label import for the IDA plugin. Reflected API extension of MCRITweb in McritClient.
+ * 2023-04-10 v1.0.0: Milestone release for Botconf 2023.
+ * 2023-04-10 v0.25.0: IDA plugin can now do function queries for the currently viewed function.
+ * 2023-03-24 v0.24.2: McritClient can forward username/apitoken, addJsonReport is now forwardable.
+ * 2023-03-21 v0.24.0: FunctionEntries now can store additional FunctionLabelEntries, along submitting user/date.
+ * 2023-03-17 v0.23.0: It is now possible to query matches for single SmdaFunctions (synchronously).
+ * 2023-03-15 v0.22.0: McritClient now supports apitokens and raw responses for a subset of functionality.
+ * 2023-03-14 v0.21.0: Backend support for more fine grained filtering.
+ * 2023-03-13 v0.20.6: Backend support for filtering family/sample by score in MatchResult.
+ * 2023-02-22 v0.20.4: Bugfix for calculating unique scores and accessing these results.
+ * 2023-02-21 v0.20.3: Supporting frontend capabilities with result presentation.
+ * 2023-02-17 v0.20.2: Extended match report object to support frontend improvements.
+ * 2023-02-14 v0.20.0: Overhauled console client to simplify shell-based interactions with the backend.
+ * 2023-01-12 v0.19.4: Additional filtering capabilities for MatchingResults.
+ * 2022-12-13 v0.19.1: It is now possible to require specific (higher) amounts of band matches for candidates (i.e. reduce fuzziness of matching).
+ * 2022-12-13 v0.18.x: Enable matching of arbitrary function IDs.
+ * 2022-11-25 v0.18.9: Accelerated Query matching.
+ * 2022-11-18 v0.18.8: Harmonized handling of deletion and modifications, minor fixes.
+ * 2022-11-13 v0.18.7: Drastically accelerated sample deletion.
+ * 2022-11-13 v0.18.6: Added functionality to modify existing sample and family information.
+ * 2022-11-11 v0.18.2: Upgrading matching procedure, should now be able to handle larger binaries more robustly and efficiently.
+ * 2022-11-03 v0.18.1: Minor fixes.
+ * 2022-11-03 v0.18.0: Unique block isolation now also generates a proposal for a YARA rule, restructured result output.
+ * 2022-10-24 v0.17.4: Harmonized setup.py with requirements, improved memory efficiency for processing cross jobs.
+ * 2022-10-18 v0.17.3: Added a convenience script to recursively produce SMDA reports from a semi-structured folder.
+ * 2022-10-13 v0.17.2: Fixed potential OOM issues during MinHash calculation by processing functions to be hashed in smaller batches.
+ * 2022-10-12 v0.17.1: Added a function to schedule a job that will ensure minhashes have been calculated for all samples/functions.
+ * 2022-10-11 v0.17.0: Search for unique blocks is now an asychronous job through the Worker.
+ * 2022-10-11 v0.16.0: Samples from MatchQuery jobs will now be stored with their Sample/FunctionEntries to allow better post processing.
+ * 2022-10-04 v0.15.4: Server can now display its version.
+ * 2022-09-28 v0.15.3: Addressing performance issues for bigger instances, generating escaped instruction sequence for unique blocks.
+ * 2022-09-26 v0.15.0: CrossJobs now in backend, started to provide functionality to identify unique basic blocks in samples.
+ * 2022-08-29 v0.14.2: Minor fixes for deployment.
+ * 2022-08-22 v0.14.0: Jobs can now depend on other jobs (preparation for moving crossjobs to backend), QoL improvements to job handling.
+ * 2022-08-17 v0.13.1: Added commandline option for profiling (requires cProfile).
+ * 2022-08-09 v0.13.0: Can now do efficient direct queries for PicHash and PicBlockHash matches.
+ * 2022-08-09 v0.12.3: Bugfix for FamilyEntry
+ * 2022-08-08 v0.12.2: Bugfix for delivery of XCFG data, added missing dependency.
+ * 2022-08-08 v0.12.0: Integrated Advanced Search syntax.
+ * 2022-08-03 v0.11.0: (BREAKING) Families are now represented with a FamilyEntry.
+ * 2022-08-03 v0.10.3: Now leaving function xcfg data by default in DB, exposed access to it via REST API and McritClient.
+ * 2022-07-29 v0.10.2: Added ability to delete families - now also keeping XCFG info for all functions by default.
+ * 2022-07-12 v0.10.1: Improved performance.
+ * 2022-07-12 v0.10.0: (BREAKING) Job handling simplified.
+ * 2022-05-13  v0.9.4: Bug fix for receiving submitted files.
+ * 2022-05-13  v0.9.3: Further updates to MatchingResults.
+ * 2022-05-13  v0.9.2: Added another field and more convenience functions in MatchingResult for better access - those are breaking changes for previously created MatchingResults.
+ * 2022-05-05  v0.9.1: Processing of binary submissions, minor fixes for minhash queuing - INITIAL RELEASE.
+ * 2022-02-09  v0.9.0: Added PicBlocks to MCRIT.
+ * 2022-01-19  v0.8.0: Migrated the client and the examples into the primary MCRIT repository.
+ * 2021-12-16  v0.7.0: Initial private release.
+
+## Credits & Notes
+
+Thanks to Steffen Enders and Paul Hordiienko for their contributions to the internal research prototype of this project!
+Thanks to Manuel Blatt for his extensive contributions to and refactorings of this project as well as for the client module!
+
+Pull requests welcome! :)
+
+## License
+```
+    MinHash-based Code Relationship & Investigation Toolkit (MCRIT)
+    Copyright (C) 2022  Daniel Plohmann, Manuel Blatt
+
+    This program is free software: you can redistribute it and/or modify
+    it under the terms of the GNU General Public License as published by
+    the Free Software Foundation, either version 3 of the License, or
+    (at your option) any later version.
+
+    This program is distributed in the hope that it will be useful,
+    but WITHOUT ANY WARRANTY; without even the implied warranty of
+    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+    GNU General Public License for more details.
+
+    You should have received a copy of the GNU General Public License
+    along with this program.  If not, see <http://www.gnu.org/licenses/>.
+    
+    Some plug-ins and libraries may have different licenses. 
+    If so, a license file is provided in the plug-in's folder.
+```
```

### Comparing `mcrit-1.0.1/README.md` & `mcrit-1.0.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -92,14 +92,16 @@
 $ python -m mcrit client status
 {'status': {'db_state': 187, 'storage_type': 'mongodb', 'num_bands': 20, 'num_samples': 137, 'num_families': 14, 'num_functions': 129110, 'num_pichashes': 25385}}
 # submit a malware sample with filename sample_unpacked, using family name "some_family"
 $ python -m mcrit client submit sample_unpacked -f some_family
  1.039s -> (architecture: intel.32bit, base_addr: 0x10000000): 634 functions
 ```
 
+A more extensive documentation of the MCRIT CLI is available [here](docs/mcrit-cli.md)
+
 ### MCRIT IDA Plugin
 
 An IDA plugin is also currently under development.
 To use it, first create your own config.py and make required changes depending on the deployment of your MCRIT instance:
 ```
 cp ./plugins/ida/template.config.py ./plugins/ida/config.py
 nano ./plugins/ida/config.py
@@ -111,14 +113,15 @@
 ./plugins/ida/ida_mcrit.py
 ```
 
 in IDA.
 
 
 ## Version History
+ * 2023-05-22 v1.0.2: More robustness for path verification when using MCRIT CLI on Malpedia repo folder.
  * 2023-05-12 v1.0.1: Some progress on label import for the IDA plugin. Reflected API extension of MCRITweb in McritClient.
  * 2023-04-10 v1.0.0: Milestone release for Botconf 2023.
  * 2023-04-10 v0.25.0: IDA plugin can now do function queries for the currently viewed function.
  * 2023-03-24 v0.24.2: McritClient can forward username/apitoken, addJsonReport is now forwardable.
  * 2023-03-21 v0.24.0: FunctionEntries now can store additional FunctionLabelEntries, along submitting user/date.
  * 2023-03-17 v0.23.0: It is now possible to query matches for single SmdaFunctions (synchronously).
  * 2023-03-15 v0.22.0: McritClient now supports apitokens and raw responses for a subset of functionality.
```

### Comparing `mcrit-1.0.1/mcrit/Worker.py` & `mcrit-1.0.2/mcrit/Worker.py`

 * *Files identical despite different names*

### Comparing `mcrit-1.0.1/mcrit/__main__.py` & `mcrit-1.0.2/mcrit/__main__.py`

 * *Files identical despite different names*

### Comparing `mcrit-1.0.1/mcrit/client/McritClient.py` & `mcrit-1.0.2/mcrit/client/McritClient.py`

 * *Files identical despite different names*

### Comparing `mcrit-1.0.1/mcrit/client/McritConsole.py` & `mcrit-1.0.2/mcrit/client/McritConsole.py`

 * *Files 6% similar despite different names*

```diff
@@ -300,25 +300,34 @@
                         smda_report.family = getFamilyName(folder_relative_path)
                         smda_report.version = getSampleVersion(folder_relative_path, smda_report.family)
                         print(filepath)
                         print(smda_report)
                         client.addReport(smda_report)
 
     def _handle_submit_malpedia(self, args):
+        # verify that we have a malpedia root
+        malpedia_root = os.path.abspath(args.filepath)
+        malpedia_root = malpedia_root.rstrip("/")
+        if not malpedia_root.endswith("malpedia"):
+            print(f"Error: You pointing to a folder named differently than 'malpedia'.")
+            return
+        if not "malpedia.bib" in os.listdir(malpedia_root):
+            print(f"Error: 'malpedia.bib' is missing in that folder, are you sure you are poniting to a Malpedia repository?")
+            return
         client = McritClient()
         # get current status of all samples in MCRIT
         mcrit_samples = client.getSamples()
         mcrit_samples_by_filename = {}
         for sample_id, sample in mcrit_samples.items():
             # verify that filename has malpedia format (starts with sha256 and _unpacked/_dump)
             if sample.filename in mcrit_samples_by_filename:
                 print(f"WARNING: filename {sample.filename} appears to exist more than once in your MCRIT instance, now using SHA256 {sample.sha256[:8]}.")
             mcrit_samples_by_filename[sample.filename] = sample
         # get all unpacked/dumped files and their family/version by crawling given Malpedia location
-        malpedia_samples_by_filename = self._getMalpediaSamplesByFilename(args.filepath)
+        malpedia_samples_by_filename = self._getMalpediaSamplesByFilename(malpedia_root)
         # use submission filenames within MCRIT to check for presence of files and verify their family/version identity
         for filename, malpedia_info in malpedia_samples_by_filename.items():
             malpedia_family = malpedia_info["family"]
             malpedia_version = malpedia_info["version"]
             malpedia_filepath = malpedia_info["filepath"]
             if filename in mcrit_samples_by_filename:
                 mcrit_family = mcrit_samples_by_filename[filename].family
@@ -334,22 +343,24 @@
                 smda_report = getSmdaReportFromFilepath(args, malpedia_filepath)
                 if smda_report:
                     smda_report.family = malpedia_family
                     smda_report.version = malpedia_version
                     print(malpedia_filepath)
                     print(smda_report)
                     client.addReport(smda_report)
-        # warn about files that appear deleted because not present in Malpedia but in MCRIT (based on name schea)
+        # warn about files that appear deleted because not present in Malpedia but in MCRIT (based on name schema)
         for filename, mcrit_sample in mcrit_samples_by_filename.items():
             if self._isMalpediaFilename(filename) and filename not in malpedia_samples_by_filename:
                 print(f"WARNING: Sample {mcrit_sample.sample_id} with filename {filename} ({mcrit_sample.family}|{mcrit_sample.version}) present in MCRIT but not in Malpedia?")
 
     def _getMalpediaSamplesByFilename(self, malpedia_root):
         malpedia_samples_by_filename = {}
         for root, subdir, files in sorted(os.walk(malpedia_root)):
+            if not "win." in root or "elf." in root:
+                continue
             folder_relative_path = getFolderFilePath(malpedia_root, root)
             for filename in sorted(files):
                 if self._isMalpediaFilename(filename):
                     filepath = root + os.sep + filename
                     sample_family = getFamilyName(folder_relative_path)
                     malpedia_samples_by_filename[filename] = {
                         "filename": filename,
```

### Comparing `mcrit-1.0.1/mcrit/config/ConfigInterface.py` & `mcrit-1.0.2/mcrit/config/ConfigInterface.py`

 * *Files identical despite different names*

### Comparing `mcrit-1.0.1/mcrit/config/McritConfig.py` & `mcrit-1.0.2/mcrit/config/McritConfig.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from .ShinglerConfig import ShinglerConfig
 from .StorageConfig import StorageConfig
 
 
 class McritConfig(object):
 
     # NOTE to self: always change this in setup.py as well!
-    VERSION = "1.0.1"
+    VERSION = "1.0.2"
     CONFIG_FILE_PATH = str(os.path.abspath(__file__))
     PROJECT_ROOT = str(os.path.abspath(os.sep.join([CONFIG_FILE_PATH, "..", ".."])))
 
     ### global logging-config setup
     # Only do basicConfig if no handlers have been configured
     LOG_PATH = "./"
     LOG_LEVEL = logging.INFO
```

### Comparing `mcrit-1.0.1/mcrit/config/MinHashConfig.py` & `mcrit-1.0.2/mcrit/config/MinHashConfig.py`

 * *Files identical despite different names*

### Comparing `mcrit-1.0.1/mcrit/config/QueueConfig.py` & `mcrit-1.0.2/mcrit/config/QueueConfig.py`

 * *Files identical despite different names*

### Comparing `mcrit-1.0.1/mcrit/config/ShinglerConfig.py` & `mcrit-1.0.2/mcrit/config/ShinglerConfig.py`

 * *Files identical despite different names*

### Comparing `mcrit-1.0.1/mcrit/config/StorageConfig.py` & `mcrit-1.0.2/mcrit/config/StorageConfig.py`

 * *Files identical despite different names*

### Comparing `mcrit-1.0.1/mcrit/index/MinHashIndex.py` & `mcrit-1.0.2/mcrit/index/MinHashIndex.py`

 * *Files identical despite different names*

### Comparing `mcrit-1.0.1/mcrit/index/SearchCursor.py` & `mcrit-1.0.2/mcrit/index/SearchCursor.py`

 * *Files identical despite different names*

### Comparing `mcrit-1.0.1/mcrit/index/SearchQueryParser.py` & `mcrit-1.0.2/mcrit/index/SearchQueryParser.py`

 * *Files identical despite different names*

### Comparing `mcrit-1.0.1/mcrit/index/SearchQueryTree.py` & `mcrit-1.0.2/mcrit/index/SearchQueryTree.py`

 * *Files identical despite different names*

### Comparing `mcrit-1.0.1/mcrit/libs/mongoqueue.py` & `mcrit-1.0.2/mcrit/libs/mongoqueue.py`

 * *Files identical despite different names*

### Comparing `mcrit-1.0.1/mcrit/libs/pymmh3.py` & `mcrit-1.0.2/mcrit/libs/pymmh3.py`

 * *Files identical despite different names*

### Comparing `mcrit-1.0.1/mcrit/libs/utility.py` & `mcrit-1.0.2/mcrit/libs/utility.py`

 * *Files identical despite different names*

### Comparing `mcrit-1.0.1/mcrit/matchers/MatcherCross.py` & `mcrit-1.0.2/mcrit/matchers/MatcherCross.py`

 * *Files identical despite different names*

### Comparing `mcrit-1.0.1/mcrit/matchers/MatcherInterface.py` & `mcrit-1.0.2/mcrit/matchers/MatcherInterface.py`

 * *Files identical despite different names*

### Comparing `mcrit-1.0.1/mcrit/matchers/MatcherQuery.py` & `mcrit-1.0.2/mcrit/matchers/MatcherQuery.py`

 * *Files identical despite different names*

### Comparing `mcrit-1.0.1/mcrit/matchers/MatcherQueryFunction.py` & `mcrit-1.0.2/mcrit/matchers/MatcherQueryFunction.py`

 * *Files identical despite different names*

### Comparing `mcrit-1.0.1/mcrit/matchers/MatcherSample.py` & `mcrit-1.0.2/mcrit/matchers/MatcherSample.py`

 * *Files identical despite different names*

### Comparing `mcrit-1.0.1/mcrit/matchers/MatcherVs.py` & `mcrit-1.0.2/mcrit/matchers/MatcherVs.py`

 * *Files identical despite different names*

### Comparing `mcrit-1.0.1/mcrit/minhash/MinHash.py` & `mcrit-1.0.2/mcrit/minhash/MinHash.py`

 * *Files identical despite different names*

### Comparing `mcrit-1.0.1/mcrit/minhash/MinHasher.py` & `mcrit-1.0.2/mcrit/minhash/MinHasher.py`

 * *Files identical despite different names*

### Comparing `mcrit-1.0.1/mcrit/minhash/ShingleLoader.py` & `mcrit-1.0.2/mcrit/minhash/ShingleLoader.py`

 * *Files identical despite different names*

### Comparing `mcrit-1.0.1/mcrit/queue/LocalQueue.py` & `mcrit-1.0.2/mcrit/queue/LocalQueue.py`

 * *Files identical despite different names*

### Comparing `mcrit-1.0.1/mcrit/queue/QueueFactory.py` & `mcrit-1.0.2/mcrit/queue/QueueFactory.py`

 * *Files identical despite different names*

### Comparing `mcrit-1.0.1/mcrit/queue/QueueRemoteCalls.py` & `mcrit-1.0.2/mcrit/queue/QueueRemoteCalls.py`

 * *Files identical despite different names*

### Comparing `mcrit-1.0.1/mcrit/server/BlocksResource.py` & `mcrit-1.0.2/mcrit/server/BlocksResource.py`

 * *Files identical despite different names*

### Comparing `mcrit-1.0.1/mcrit/server/FamilyResource.py` & `mcrit-1.0.2/mcrit/server/FamilyResource.py`

 * *Files identical despite different names*

### Comparing `mcrit-1.0.1/mcrit/server/FunctionResource.py` & `mcrit-1.0.2/mcrit/server/FunctionResource.py`

 * *Files identical despite different names*

### Comparing `mcrit-1.0.1/mcrit/server/JobResource.py` & `mcrit-1.0.2/mcrit/server/JobResource.py`

 * *Files identical despite different names*

### Comparing `mcrit-1.0.1/mcrit/server/MatchResource.py` & `mcrit-1.0.2/mcrit/server/MatchResource.py`

 * *Files identical despite different names*

### Comparing `mcrit-1.0.1/mcrit/server/QueryResource.py` & `mcrit-1.0.2/mcrit/server/QueryResource.py`

 * *Files identical despite different names*

### Comparing `mcrit-1.0.1/mcrit/server/SampleResource.py` & `mcrit-1.0.2/mcrit/server/SampleResource.py`

 * *Files identical despite different names*

### Comparing `mcrit-1.0.1/mcrit/server/StatusResource.py` & `mcrit-1.0.2/mcrit/server/StatusResource.py`

 * *Files identical despite different names*

### Comparing `mcrit-1.0.1/mcrit/server/application_routes.py` & `mcrit-1.0.2/mcrit/server/application_routes.py`

 * *Files identical despite different names*

### Comparing `mcrit-1.0.1/mcrit/server/utils.py` & `mcrit-1.0.2/mcrit/server/utils.py`

 * *Files identical despite different names*

### Comparing `mcrit-1.0.1/mcrit/storage/FamilyEntry.py` & `mcrit-1.0.2/mcrit/storage/FamilyEntry.py`

 * *Files identical despite different names*

### Comparing `mcrit-1.0.1/mcrit/storage/FunctionEntry.py` & `mcrit-1.0.2/mcrit/storage/FunctionEntry.py`

 * *Files identical despite different names*

### Comparing `mcrit-1.0.1/mcrit/storage/FunctionLabelEntry.py` & `mcrit-1.0.2/mcrit/storage/FunctionLabelEntry.py`

 * *Files identical despite different names*

### Comparing `mcrit-1.0.1/mcrit/storage/MatchedFunctionEntry.py` & `mcrit-1.0.2/mcrit/storage/MatchedFunctionEntry.py`

 * *Files identical despite different names*

### Comparing `mcrit-1.0.1/mcrit/storage/MatchedSampleEntry.py` & `mcrit-1.0.2/mcrit/storage/MatchedSampleEntry.py`

 * *Files identical despite different names*

### Comparing `mcrit-1.0.1/mcrit/storage/MatchingCache.py` & `mcrit-1.0.2/mcrit/storage/MatchingCache.py`

 * *Files identical despite different names*

### Comparing `mcrit-1.0.1/mcrit/storage/MatchingResult.py` & `mcrit-1.0.2/mcrit/storage/MatchingResult.py`

 * *Files identical despite different names*

### Comparing `mcrit-1.0.1/mcrit/storage/MemoryStorage.py` & `mcrit-1.0.2/mcrit/storage/MemoryStorage.py`

 * *Files identical despite different names*

### Comparing `mcrit-1.0.1/mcrit/storage/MongoDbStorage.py` & `mcrit-1.0.2/mcrit/storage/MongoDbStorage.py`

 * *Files identical despite different names*

### Comparing `mcrit-1.0.1/mcrit/storage/SampleEntry.py` & `mcrit-1.0.2/mcrit/storage/SampleEntry.py`

 * *Files identical despite different names*

### Comparing `mcrit-1.0.1/mcrit/storage/StorageFactory.py` & `mcrit-1.0.2/mcrit/storage/StorageFactory.py`

 * *Files identical despite different names*

### Comparing `mcrit-1.0.1/mcrit/storage/StorageInterface.py` & `mcrit-1.0.2/mcrit/storage/StorageInterface.py`

 * *Files identical despite different names*

### Comparing `mcrit-1.0.1/mcrit.egg-info/PKG-INFO` & `mcrit-1.0.2/mcrit.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,214 +1,217 @@
 Metadata-Version: 2.1
 Name: mcrit
-Version: 1.0.1
+Version: 1.0.2
 Summary: MCRIT is a framework created for simplified application of the MinHash algorithm to code similarity.
 Home-page: https://github.com/danielplohmann/mcrit
 Author: Daniel Plohmann, Manuel Blatt, Steffen Enders, Paul Hordiienko
 Author-email: daniel.plohmann@fkie.fraunhofer.de
 License: NU General Public License v3 (GPLv3)
-Description: # MinHash-based Code Relationship & Investigation Toolkit (MCRIT)
-        [![Test](https://github.com/danielplohmann/mcrit/actions/workflows/test.yml/badge.svg)](https://github.com/danielplohmann/mcrit/actions/workflows/test.yml)
-        
-        MCRIT is a framework created to simplify the application of the MinHash algorithm in the context of code similarity.
-        It can be used to rapidly implement "shinglers", i.e. methods which encode properties of disassembled functions, to then be used for similarity estimation via the MinHash algorithm.
-        It is tailored to work with disassembly reports emitted by [SMDA](https://github.com/danielplohmann/smda).
-        
-        ## Usage
-        
-        ### Dockerized Usage
-        
-        We highly recommend to use the fully packaged [docker-mcrit](https://github.com/danielplohmann/docker-mcrit) for trivial deployment and usage.  
-        First and foremost, this will ensure that you have fully compatible versions across all components, including a database for persistence and a web frontend for convenient interaction.
-        
-        ### Standalone Usage
-        
-        Installing MCRIT on its own will require some more steps.  
-        For the following, we assume Ubuntu as host operating system.
-        
-        The Python installation requirements are listed in `requirements.txt` and can be installed using:
-        
-        ```bash
-        # install python and MCRIT dependencies
-        $ sudo apt install python3 python3-pip
-        $ pip install -r requirements.txt 
-        ```
-        
-        By default, MongoDB 5.0 is used as backend, which is also the recommended mode of operation as it provides a persistent data storage.
-        The following commands outline an example installation on Ubuntu:
-        ```bash
-        # fetch mongodb signing key
-        $ sudo apt-get install gnupg
-        $ wget -qO - https://www.mongodb.org/static/pgp/server-5.0.asc | sudo apt-key add -
-        # add package repository (Ubuntu 22.04)
-        $ echo "deb [ arch=amd64,arm64 ] https://repo.mongodb.org/apt/ubuntu jammy/mongodb-org/5.0 multiverse" | sudo tee /etc/apt/sources.list.d/mongodb-org-5.0.list
-        # OR add package repository (Ubuntu 20.04)
-        $ echo "deb [ arch=amd64,arm64 ] https://repo.mongodb.org/apt/ubuntu focal/mongodb-org/5.0 multiverse" | sudo tee /etc/apt/sources.list.d/mongodb-org-5.0.list
-        # OR add package repository (Ubuntu 18.04)
-        $ echo "deb [ arch=amd64,arm64 ] https://repo.mongodb.org/apt/ubuntu bionic/mongodb-org/5.0 multiverse" | sudo tee /etc/apt/sources.list.d/mongodb-org-5.0.list
-        # install mongodb
-        $ sudo apt-get update
-        $ sudo apt-get install -y mongodb-org
-        # start mongodb as a service
-        $ sudo systemctl start mongod
-        # optionally configure to start the service with system startup
-        $ sudo systemctl enable mongod
-        ```
-        
-        When doing the standalone installation, you possibly want to install the MCRIT module based on the cloned repository, like so:
-        
-        ```bash
-        $ pip install -e .
-        ```
-        
-        After this initial installation and if desired, MCRIT can be used without an internet connection.
-        
-        
-        #### Operation
-        
-        The MCRIT backend is generally divided into two components, a server providing an API interface to work with and one or more workers processing queued jobs.
-        They can be started in seperate shells using:
-        
-        ```bash
-        $ python -m mcrit server
-        ```
-        
-        and
-        
-        ```bash
-        $ python -m mcrit worker
-        ```
-        
-        By default, the REST API server will be listening on [http://127.0.0.1:8000/](http://127.0.0.1:8000/).
-        
-        
-        ## Interaction
-        
-        Regardless of your choice for installation, once running you can interact with the MCRIT backend.
-        
-        
-        ### MCRIT Client
-        
-        We have created a Python client module that is capable of working with all available endpoints of the server.  
-        Documentation for this client module is currently in development.
-        
-        ### MCRIT CLI
-        
-        There is also a CLI which is based on this client package, examples:
-        
-        ```bash
-        # query some stats of the data stored in the backend 
-        $ python -m mcrit client status
-        {'status': {'db_state': 187, 'storage_type': 'mongodb', 'num_bands': 20, 'num_samples': 137, 'num_families': 14, 'num_functions': 129110, 'num_pichashes': 25385}}
-        # submit a malware sample with filename sample_unpacked, using family name "some_family"
-        $ python -m mcrit client submit sample_unpacked -f some_family
-         1.039s -> (architecture: intel.32bit, base_addr: 0x10000000): 634 functions
-        ```
-        
-        ### MCRIT IDA Plugin
-        
-        An IDA plugin is also currently under development.
-        To use it, first create your own config.py and make required changes depending on the deployment of your MCRIT instance:
-        ```
-        cp ./plugins/ida/template.config.py ./plugins/ida/config.py
-        nano ./plugins/ida/config.py
-        ```
-        
-        Then simply run the script found at
-        
-        ```
-        ./plugins/ida/ida_mcrit.py
-        ```
-        
-        in IDA.
-        
-        
-        ## Version History
-         * 2023-05-12 v1.0.1: Some progress on label import for the IDA plugin. Reflected API extension of MCRITweb in McritClient.
-         * 2023-04-10 v1.0.0: Milestone release for Botconf 2023.
-         * 2023-04-10 v0.25.0: IDA plugin can now do function queries for the currently viewed function.
-         * 2023-03-24 v0.24.2: McritClient can forward username/apitoken, addJsonReport is now forwardable.
-         * 2023-03-21 v0.24.0: FunctionEntries now can store additional FunctionLabelEntries, along submitting user/date.
-         * 2023-03-17 v0.23.0: It is now possible to query matches for single SmdaFunctions (synchronously).
-         * 2023-03-15 v0.22.0: McritClient now supports apitokens and raw responses for a subset of functionality.
-         * 2023-03-14 v0.21.0: Backend support for more fine grained filtering.
-         * 2023-03-13 v0.20.6: Backend support for filtering family/sample by score in MatchResult.
-         * 2023-02-22 v0.20.4: Bugfix for calculating unique scores and accessing these results.
-         * 2023-02-21 v0.20.3: Supporting frontend capabilities with result presentation.
-         * 2023-02-17 v0.20.2: Extended match report object to support frontend improvements.
-         * 2023-02-14 v0.20.0: Overhauled console client to simplify shell-based interactions with the backend.
-         * 2023-01-12 v0.19.4: Additional filtering capabilities for MatchingResults.
-         * 2022-12-13 v0.19.1: It is now possible to require specific (higher) amounts of band matches for candidates (i.e. reduce fuzziness of matching).
-         * 2022-12-13 v0.18.x: Enable matching of arbitrary function IDs.
-         * 2022-11-25 v0.18.9: Accelerated Query matching.
-         * 2022-11-18 v0.18.8: Harmonized handling of deletion and modifications, minor fixes.
-         * 2022-11-13 v0.18.7: Drastically accelerated sample deletion.
-         * 2022-11-13 v0.18.6: Added functionality to modify existing sample and family information.
-         * 2022-11-11 v0.18.2: Upgrading matching procedure, should now be able to handle larger binaries more robustly and efficiently.
-         * 2022-11-03 v0.18.1: Minor fixes.
-         * 2022-11-03 v0.18.0: Unique block isolation now also generates a proposal for a YARA rule, restructured result output.
-         * 2022-10-24 v0.17.4: Harmonized setup.py with requirements, improved memory efficiency for processing cross jobs.
-         * 2022-10-18 v0.17.3: Added a convenience script to recursively produce SMDA reports from a semi-structured folder.
-         * 2022-10-13 v0.17.2: Fixed potential OOM issues during MinHash calculation by processing functions to be hashed in smaller batches.
-         * 2022-10-12 v0.17.1: Added a function to schedule a job that will ensure minhashes have been calculated for all samples/functions.
-         * 2022-10-11 v0.17.0: Search for unique blocks is now an asychronous job through the Worker.
-         * 2022-10-11 v0.16.0: Samples from MatchQuery jobs will now be stored with their Sample/FunctionEntries to allow better post processing.
-         * 2022-10-04 v0.15.4: Server can now display its version.
-         * 2022-09-28 v0.15.3: Addressing performance issues for bigger instances, generating escaped instruction sequence for unique blocks.
-         * 2022-09-26 v0.15.0: CrossJobs now in backend, started to provide functionality to identify unique basic blocks in samples.
-         * 2022-08-29 v0.14.2: Minor fixes for deployment.
-         * 2022-08-22 v0.14.0: Jobs can now depend on other jobs (preparation for moving crossjobs to backend), QoL improvements to job handling.
-         * 2022-08-17 v0.13.1: Added commandline option for profiling (requires cProfile).
-         * 2022-08-09 v0.13.0: Can now do efficient direct queries for PicHash and PicBlockHash matches.
-         * 2022-08-09 v0.12.3: Bugfix for FamilyEntry
-         * 2022-08-08 v0.12.2: Bugfix for delivery of XCFG data, added missing dependency.
-         * 2022-08-08 v0.12.0: Integrated Advanced Search syntax.
-         * 2022-08-03 v0.11.0: (BREAKING) Families are now represented with a FamilyEntry.
-         * 2022-08-03 v0.10.3: Now leaving function xcfg data by default in DB, exposed access to it via REST API and McritClient.
-         * 2022-07-29 v0.10.2: Added ability to delete families - now also keeping XCFG info for all functions by default.
-         * 2022-07-12 v0.10.1: Improved performance.
-         * 2022-07-12 v0.10.0: (BREAKING) Job handling simplified.
-         * 2022-05-13  v0.9.4: Bug fix for receiving submitted files.
-         * 2022-05-13  v0.9.3: Further updates to MatchingResults.
-         * 2022-05-13  v0.9.2: Added another field and more convenience functions in MatchingResult for better access - those are breaking changes for previously created MatchingResults.
-         * 2022-05-05  v0.9.1: Processing of binary submissions, minor fixes for minhash queuing - INITIAL RELEASE.
-         * 2022-02-09  v0.9.0: Added PicBlocks to MCRIT.
-         * 2022-01-19  v0.8.0: Migrated the client and the examples into the primary MCRIT repository.
-         * 2021-12-16  v0.7.0: Initial private release.
-        
-        ## Credits & Notes
-        
-        Thanks to Steffen Enders and Paul Hordiienko for their contributions to the internal research prototype of this project!
-        Thanks to Manuel Blatt for his extensive contributions to and refactorings of this project as well as for the client module!
-        
-        Pull requests welcome! :)
-        
-        ## License
-        ```
-            MinHash-based Code Relationship & Investigation Toolkit (MCRIT)
-            Copyright (C) 2022  Daniel Plohmann, Manuel Blatt
-        
-            This program is free software: you can redistribute it and/or modify
-            it under the terms of the GNU General Public License as published by
-            the Free Software Foundation, either version 3 of the License, or
-            (at your option) any later version.
-        
-            This program is distributed in the hope that it will be useful,
-            but WITHOUT ANY WARRANTY; without even the implied warranty of
-            MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-            GNU General Public License for more details.
-        
-            You should have received a copy of the GNU General Public License
-            along with this program.  If not, see <http://www.gnu.org/licenses/>.
-            
-            Some plug-ins and libraries may have different licenses. 
-            If so, a license file is provided in the plug-in's folder.
-        ```
-        
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Security
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# MinHash-based Code Relationship & Investigation Toolkit (MCRIT)
+[![Test](https://github.com/danielplohmann/mcrit/actions/workflows/test.yml/badge.svg)](https://github.com/danielplohmann/mcrit/actions/workflows/test.yml)
+
+MCRIT is a framework created to simplify the application of the MinHash algorithm in the context of code similarity.
+It can be used to rapidly implement "shinglers", i.e. methods which encode properties of disassembled functions, to then be used for similarity estimation via the MinHash algorithm.
+It is tailored to work with disassembly reports emitted by [SMDA](https://github.com/danielplohmann/smda).
+
+## Usage
+
+### Dockerized Usage
+
+We highly recommend to use the fully packaged [docker-mcrit](https://github.com/danielplohmann/docker-mcrit) for trivial deployment and usage.  
+First and foremost, this will ensure that you have fully compatible versions across all components, including a database for persistence and a web frontend for convenient interaction.
+
+### Standalone Usage
+
+Installing MCRIT on its own will require some more steps.  
+For the following, we assume Ubuntu as host operating system.
+
+The Python installation requirements are listed in `requirements.txt` and can be installed using:
+
+```bash
+# install python and MCRIT dependencies
+$ sudo apt install python3 python3-pip
+$ pip install -r requirements.txt 
+```
+
+By default, MongoDB 5.0 is used as backend, which is also the recommended mode of operation as it provides a persistent data storage.
+The following commands outline an example installation on Ubuntu:
+```bash
+# fetch mongodb signing key
+$ sudo apt-get install gnupg
+$ wget -qO - https://www.mongodb.org/static/pgp/server-5.0.asc | sudo apt-key add -
+# add package repository (Ubuntu 22.04)
+$ echo "deb [ arch=amd64,arm64 ] https://repo.mongodb.org/apt/ubuntu jammy/mongodb-org/5.0 multiverse" | sudo tee /etc/apt/sources.list.d/mongodb-org-5.0.list
+# OR add package repository (Ubuntu 20.04)
+$ echo "deb [ arch=amd64,arm64 ] https://repo.mongodb.org/apt/ubuntu focal/mongodb-org/5.0 multiverse" | sudo tee /etc/apt/sources.list.d/mongodb-org-5.0.list
+# OR add package repository (Ubuntu 18.04)
+$ echo "deb [ arch=amd64,arm64 ] https://repo.mongodb.org/apt/ubuntu bionic/mongodb-org/5.0 multiverse" | sudo tee /etc/apt/sources.list.d/mongodb-org-5.0.list
+# install mongodb
+$ sudo apt-get update
+$ sudo apt-get install -y mongodb-org
+# start mongodb as a service
+$ sudo systemctl start mongod
+# optionally configure to start the service with system startup
+$ sudo systemctl enable mongod
+```
+
+When doing the standalone installation, you possibly want to install the MCRIT module based on the cloned repository, like so:
+
+```bash
+$ pip install -e .
+```
+
+After this initial installation and if desired, MCRIT can be used without an internet connection.
+
+
+#### Operation
+
+The MCRIT backend is generally divided into two components, a server providing an API interface to work with and one or more workers processing queued jobs.
+They can be started in seperate shells using:
+
+```bash
+$ python -m mcrit server
+```
+
+and
+
+```bash
+$ python -m mcrit worker
+```
+
+By default, the REST API server will be listening on [http://127.0.0.1:8000/](http://127.0.0.1:8000/).
+
+
+## Interaction
+
+Regardless of your choice for installation, once running you can interact with the MCRIT backend.
+
+
+### MCRIT Client
+
+We have created a Python client module that is capable of working with all available endpoints of the server.  
+Documentation for this client module is currently in development.
+
+### MCRIT CLI
+
+There is also a CLI which is based on this client package, examples:
+
+```bash
+# query some stats of the data stored in the backend 
+$ python -m mcrit client status
+{'status': {'db_state': 187, 'storage_type': 'mongodb', 'num_bands': 20, 'num_samples': 137, 'num_families': 14, 'num_functions': 129110, 'num_pichashes': 25385}}
+# submit a malware sample with filename sample_unpacked, using family name "some_family"
+$ python -m mcrit client submit sample_unpacked -f some_family
+ 1.039s -> (architecture: intel.32bit, base_addr: 0x10000000): 634 functions
+```
+
+A more extensive documentation of the MCRIT CLI is available [here](docs/mcrit-cli.md)
+
+### MCRIT IDA Plugin
+
+An IDA plugin is also currently under development.
+To use it, first create your own config.py and make required changes depending on the deployment of your MCRIT instance:
+```
+cp ./plugins/ida/template.config.py ./plugins/ida/config.py
+nano ./plugins/ida/config.py
+```
+
+Then simply run the script found at
+
+```
+./plugins/ida/ida_mcrit.py
+```
+
+in IDA.
+
+
+## Version History
+ * 2023-05-22 v1.0.2: More robustness for path verification when using MCRIT CLI on Malpedia repo folder.
+ * 2023-05-12 v1.0.1: Some progress on label import for the IDA plugin. Reflected API extension of MCRITweb in McritClient.
+ * 2023-04-10 v1.0.0: Milestone release for Botconf 2023.
+ * 2023-04-10 v0.25.0: IDA plugin can now do function queries for the currently viewed function.
+ * 2023-03-24 v0.24.2: McritClient can forward username/apitoken, addJsonReport is now forwardable.
+ * 2023-03-21 v0.24.0: FunctionEntries now can store additional FunctionLabelEntries, along submitting user/date.
+ * 2023-03-17 v0.23.0: It is now possible to query matches for single SmdaFunctions (synchronously).
+ * 2023-03-15 v0.22.0: McritClient now supports apitokens and raw responses for a subset of functionality.
+ * 2023-03-14 v0.21.0: Backend support for more fine grained filtering.
+ * 2023-03-13 v0.20.6: Backend support for filtering family/sample by score in MatchResult.
+ * 2023-02-22 v0.20.4: Bugfix for calculating unique scores and accessing these results.
+ * 2023-02-21 v0.20.3: Supporting frontend capabilities with result presentation.
+ * 2023-02-17 v0.20.2: Extended match report object to support frontend improvements.
+ * 2023-02-14 v0.20.0: Overhauled console client to simplify shell-based interactions with the backend.
+ * 2023-01-12 v0.19.4: Additional filtering capabilities for MatchingResults.
+ * 2022-12-13 v0.19.1: It is now possible to require specific (higher) amounts of band matches for candidates (i.e. reduce fuzziness of matching).
+ * 2022-12-13 v0.18.x: Enable matching of arbitrary function IDs.
+ * 2022-11-25 v0.18.9: Accelerated Query matching.
+ * 2022-11-18 v0.18.8: Harmonized handling of deletion and modifications, minor fixes.
+ * 2022-11-13 v0.18.7: Drastically accelerated sample deletion.
+ * 2022-11-13 v0.18.6: Added functionality to modify existing sample and family information.
+ * 2022-11-11 v0.18.2: Upgrading matching procedure, should now be able to handle larger binaries more robustly and efficiently.
+ * 2022-11-03 v0.18.1: Minor fixes.
+ * 2022-11-03 v0.18.0: Unique block isolation now also generates a proposal for a YARA rule, restructured result output.
+ * 2022-10-24 v0.17.4: Harmonized setup.py with requirements, improved memory efficiency for processing cross jobs.
+ * 2022-10-18 v0.17.3: Added a convenience script to recursively produce SMDA reports from a semi-structured folder.
+ * 2022-10-13 v0.17.2: Fixed potential OOM issues during MinHash calculation by processing functions to be hashed in smaller batches.
+ * 2022-10-12 v0.17.1: Added a function to schedule a job that will ensure minhashes have been calculated for all samples/functions.
+ * 2022-10-11 v0.17.0: Search for unique blocks is now an asychronous job through the Worker.
+ * 2022-10-11 v0.16.0: Samples from MatchQuery jobs will now be stored with their Sample/FunctionEntries to allow better post processing.
+ * 2022-10-04 v0.15.4: Server can now display its version.
+ * 2022-09-28 v0.15.3: Addressing performance issues for bigger instances, generating escaped instruction sequence for unique blocks.
+ * 2022-09-26 v0.15.0: CrossJobs now in backend, started to provide functionality to identify unique basic blocks in samples.
+ * 2022-08-29 v0.14.2: Minor fixes for deployment.
+ * 2022-08-22 v0.14.0: Jobs can now depend on other jobs (preparation for moving crossjobs to backend), QoL improvements to job handling.
+ * 2022-08-17 v0.13.1: Added commandline option for profiling (requires cProfile).
+ * 2022-08-09 v0.13.0: Can now do efficient direct queries for PicHash and PicBlockHash matches.
+ * 2022-08-09 v0.12.3: Bugfix for FamilyEntry
+ * 2022-08-08 v0.12.2: Bugfix for delivery of XCFG data, added missing dependency.
+ * 2022-08-08 v0.12.0: Integrated Advanced Search syntax.
+ * 2022-08-03 v0.11.0: (BREAKING) Families are now represented with a FamilyEntry.
+ * 2022-08-03 v0.10.3: Now leaving function xcfg data by default in DB, exposed access to it via REST API and McritClient.
+ * 2022-07-29 v0.10.2: Added ability to delete families - now also keeping XCFG info for all functions by default.
+ * 2022-07-12 v0.10.1: Improved performance.
+ * 2022-07-12 v0.10.0: (BREAKING) Job handling simplified.
+ * 2022-05-13  v0.9.4: Bug fix for receiving submitted files.
+ * 2022-05-13  v0.9.3: Further updates to MatchingResults.
+ * 2022-05-13  v0.9.2: Added another field and more convenience functions in MatchingResult for better access - those are breaking changes for previously created MatchingResults.
+ * 2022-05-05  v0.9.1: Processing of binary submissions, minor fixes for minhash queuing - INITIAL RELEASE.
+ * 2022-02-09  v0.9.0: Added PicBlocks to MCRIT.
+ * 2022-01-19  v0.8.0: Migrated the client and the examples into the primary MCRIT repository.
+ * 2021-12-16  v0.7.0: Initial private release.
+
+## Credits & Notes
+
+Thanks to Steffen Enders and Paul Hordiienko for their contributions to the internal research prototype of this project!
+Thanks to Manuel Blatt for his extensive contributions to and refactorings of this project as well as for the client module!
+
+Pull requests welcome! :)
+
+## License
+```
+    MinHash-based Code Relationship & Investigation Toolkit (MCRIT)
+    Copyright (C) 2022  Daniel Plohmann, Manuel Blatt
+
+    This program is free software: you can redistribute it and/or modify
+    it under the terms of the GNU General Public License as published by
+    the Free Software Foundation, either version 3 of the License, or
+    (at your option) any later version.
+
+    This program is distributed in the hope that it will be useful,
+    but WITHOUT ANY WARRANTY; without even the implied warranty of
+    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+    GNU General Public License for more details.
+
+    You should have received a copy of the GNU General Public License
+    along with this program.  If not, see <http://www.gnu.org/licenses/>.
+    
+    Some plug-ins and libraries may have different licenses. 
+    If so, a license file is provided in the plug-in's folder.
+```
```

### Comparing `mcrit-1.0.1/mcrit.egg-info/SOURCES.txt` & `mcrit-1.0.2/mcrit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mcrit-1.0.1/setup.py` & `mcrit-1.0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
     "smda>=1.3.0",
     "tqdm",
     "waitress",
 ]
 
 setup(
     name='mcrit',
-    version="1.0.1",
+    version="1.0.2",
     description='MCRIT is a framework created for simplified application of the MinHash algorithm to code similarity.',
     long_description_content_type="text/markdown",
     long_description=README,
     author='Daniel Plohmann, Manuel Blatt, Steffen Enders, Paul Hordiienko',
     author_email='daniel.plohmann@fkie.fraunhofer.de',
     url='https://github.com/danielplohmann/mcrit',
     license="NU General Public License v3 (GPLv3)",
```

