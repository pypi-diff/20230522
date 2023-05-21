# Comparing `tmp/cyberdrop-dl-4.2.41.tar.gz` & `tmp/cyberdrop-dl-4.2.42.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cyberdrop-dl-4.2.41.tar", last modified: Sun May 21 17:04:00 2023, max compression
+gzip compressed data, was "cyberdrop-dl-4.2.42.tar", last modified: Sun May 21 23:43:59 2023, max compression
```

## Comparing `cyberdrop-dl-4.2.41.tar` & `cyberdrop-dl-4.2.42.tar`

### file list

```diff
@@ -1,62 +1,62 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 17:04:00.951463 cyberdrop-dl-4.2.41/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-21 17:03:46.000000 cyberdrop-dl-4.2.41/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    18155 2023-05-21 17:04:00.951463 cyberdrop-dl-4.2.41/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    17720 2023-05-21 17:03:46.000000 cyberdrop-dl-4.2.41/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 17:04:00.947463 cyberdrop-dl-4.2.41/cyberdrop_dl/
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-21 17:03:46.000000 cyberdrop-dl-4.2.41/cyberdrop_dl/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 17:04:00.947463 cyberdrop-dl-4.2.41/cyberdrop_dl/base_functions/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-21 17:03:46.000000 cyberdrop-dl-4.2.41/cyberdrop_dl/base_functions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6659 2023-05-21 17:03:46.000000 cyberdrop-dl-4.2.41/cyberdrop_dl/base_functions/base_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3033 2023-05-21 17:03:46.000000 cyberdrop-dl-4.2.41/cyberdrop_dl/base_functions/config_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     3471 2023-05-21 17:03:46.000000 cyberdrop-dl-4.2.41/cyberdrop_dl/base_functions/config_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     8468 2023-05-21 17:03:46.000000 cyberdrop-dl-4.2.41/cyberdrop_dl/base_functions/data_classes.py
--rw-r--r--   0 runner    (1001) docker     (123)     1184 2023-05-21 17:03:46.000000 cyberdrop-dl-4.2.41/cyberdrop_dl/base_functions/error_classes.py
--rw-r--r--   0 runner    (1001) docker     (123)     3450 2023-05-21 17:03:46.000000 cyberdrop-dl-4.2.41/cyberdrop_dl/base_functions/sorting_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)    12707 2023-05-21 17:03:46.000000 cyberdrop-dl-4.2.41/cyberdrop_dl/base_functions/sql_helper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 17:04:00.947463 cyberdrop-dl-4.2.41/cyberdrop_dl/client/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-21 17:03:46.000000 cyberdrop-dl-4.2.41/cyberdrop_dl/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10099 2023-05-21 17:03:46.000000 cyberdrop-dl-4.2.41/cyberdrop_dl/client/client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 17:04:00.951463 cyberdrop-dl-4.2.41/cyberdrop_dl/crawlers/
--rw-r--r--   0 runner    (1001) docker     (123)     2217 2023-05-21 17:03:46.000000 cyberdrop-dl-4.2.41/cyberdrop_dl/crawlers/Anonfiles_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     7802 2023-05-21 17:03:46.000000 cyberdrop-dl-4.2.41/cyberdrop_dl/crawlers/Bunkr_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     7922 2023-05-21 17:03:46.000000 cyberdrop-dl-4.2.41/cyberdrop_dl/crawlers/Coomeno_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)    12903 2023-05-21 17:03:46.000000 cyberdrop-dl-4.2.41/cyberdrop_dl/crawlers/CyberFile_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     3042 2023-05-21 17:03:46.000000 cyberdrop-dl-4.2.41/cyberdrop_dl/crawlers/Cyberdrop_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     3089 2023-05-21 17:03:46.000000 cyberdrop-dl-4.2.41/cyberdrop_dl/crawlers/EHentai_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     4239 2023-05-21 17:03:46.000000 cyberdrop-dl-4.2.41/cyberdrop_dl/crawlers/Erome_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     4206 2023-05-21 17:03:46.000000 cyberdrop-dl-4.2.41/cyberdrop_dl/crawlers/Fapello_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     1890 2023-05-21 17:03:46.000000 cyberdrop-dl-4.2.41/cyberdrop_dl/crawlers/Gfycat_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     5069 2023-05-21 17:03:46.000000 cyberdrop-dl-4.2.41/cyberdrop_dl/crawlers/GoFile_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     2884 2023-05-21 17:03:46.000000 cyberdrop-dl-4.2.41/cyberdrop_dl/crawlers/HGameCG_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     3140 2023-05-21 17:03:46.000000 cyberdrop-dl-4.2.41/cyberdrop_dl/crawlers/ImgBox_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     3676 2023-05-21 17:03:46.000000 cyberdrop-dl-4.2.41/cyberdrop_dl/crawlers/LoveFap_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     4389 2023-05-21 17:03:46.000000 cyberdrop-dl-4.2.41/cyberdrop_dl/crawlers/NSFWXXX_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     2918 2023-05-21 17:03:46.000000 cyberdrop-dl-4.2.41/cyberdrop_dl/crawlers/PimpAndHost_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     3362 2023-05-21 17:03:46.000000 cyberdrop-dl-4.2.41/cyberdrop_dl/crawlers/PixelDrain_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     3008 2023-05-21 17:03:46.000000 cyberdrop-dl-4.2.41/cyberdrop_dl/crawlers/PostImg_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     1499 2023-05-21 17:03:46.000000 cyberdrop-dl-4.2.41/cyberdrop_dl/crawlers/Saint_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     9157 2023-05-21 17:03:46.000000 cyberdrop-dl-4.2.41/cyberdrop_dl/crawlers/ShareX_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     2186 2023-05-21 17:03:46.000000 cyberdrop-dl-4.2.41/cyberdrop_dl/crawlers/XBunkr_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)    13919 2023-05-21 17:03:46.000000 cyberdrop-dl-4.2.41/cyberdrop_dl/crawlers/Xenforo_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-21 17:03:46.000000 cyberdrop-dl-4.2.41/cyberdrop_dl/crawlers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 17:04:00.951463 cyberdrop-dl-4.2.41/cyberdrop_dl/downloader/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-21 17:03:46.000000 cyberdrop-dl-4.2.41/cyberdrop_dl/downloader/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2924 2023-05-21 17:03:46.000000 cyberdrop-dl-4.2.41/cyberdrop_dl/downloader/downloader_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    18477 2023-05-21 17:03:46.000000 cyberdrop-dl-4.2.41/cyberdrop_dl/downloader/downloaders.py
--rw-r--r--   0 runner    (1001) docker     (123)    12870 2023-05-21 17:03:46.000000 cyberdrop-dl-4.2.41/cyberdrop_dl/downloader/old_downloaders.py
--rw-r--r--   0 runner    (1001) docker     (123)    17463 2023-05-21 17:03:46.000000 cyberdrop-dl-4.2.41/cyberdrop_dl/downloader/progress_definitions.py
--rw-r--r--   0 runner    (1001) docker     (123)    20536 2023-05-21 17:03:46.000000 cyberdrop-dl-4.2.41/cyberdrop_dl/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 17:04:00.951463 cyberdrop-dl-4.2.41/cyberdrop_dl/scraper/
--rw-r--r--   0 runner    (1001) docker     (123)     2531 2023-05-21 17:03:46.000000 cyberdrop-dl-4.2.41/cyberdrop_dl/scraper/JDownloader_Integration.py
--rw-r--r--   0 runner    (1001) docker     (123)    20427 2023-05-21 17:03:46.000000 cyberdrop-dl-4.2.41/cyberdrop_dl/scraper/Scraper.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-21 17:03:46.000000 cyberdrop-dl-4.2.41/cyberdrop_dl/scraper/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 17:04:00.947463 cyberdrop-dl-4.2.41/cyberdrop_dl.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    18155 2023-05-21 17:04:00.000000 cyberdrop-dl-4.2.41/cyberdrop_dl.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1933 2023-05-21 17:04:00.000000 cyberdrop-dl-4.2.41/cyberdrop_dl.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-21 17:04:00.000000 cyberdrop-dl-4.2.41/cyberdrop_dl.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-05-21 17:04:00.000000 cyberdrop-dl-4.2.41/cyberdrop_dl.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      176 2023-05-21 17:04:00.000000 cyberdrop-dl-4.2.41/cyberdrop_dl.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-21 17:04:00.000000 cyberdrop-dl-4.2.41/cyberdrop_dl.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-21 17:03:46.000000 cyberdrop-dl-4.2.41/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      860 2023-05-21 17:04:00.951463 cyberdrop-dl-4.2.41/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-21 17:03:46.000000 cyberdrop-dl-4.2.41/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 23:43:59.709133 cyberdrop-dl-4.2.42/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-21 23:43:50.000000 cyberdrop-dl-4.2.42/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    18155 2023-05-21 23:43:59.709133 cyberdrop-dl-4.2.42/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    17720 2023-05-21 23:43:50.000000 cyberdrop-dl-4.2.42/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 23:43:59.701133 cyberdrop-dl-4.2.42/cyberdrop_dl/
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-21 23:43:50.000000 cyberdrop-dl-4.2.42/cyberdrop_dl/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 23:43:59.701133 cyberdrop-dl-4.2.42/cyberdrop_dl/base_functions/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-21 23:43:50.000000 cyberdrop-dl-4.2.42/cyberdrop_dl/base_functions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6659 2023-05-21 23:43:50.000000 cyberdrop-dl-4.2.42/cyberdrop_dl/base_functions/base_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3033 2023-05-21 23:43:50.000000 cyberdrop-dl-4.2.42/cyberdrop_dl/base_functions/config_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3471 2023-05-21 23:43:50.000000 cyberdrop-dl-4.2.42/cyberdrop_dl/base_functions/config_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8468 2023-05-21 23:43:50.000000 cyberdrop-dl-4.2.42/cyberdrop_dl/base_functions/data_classes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1184 2023-05-21 23:43:50.000000 cyberdrop-dl-4.2.42/cyberdrop_dl/base_functions/error_classes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3450 2023-05-21 23:43:50.000000 cyberdrop-dl-4.2.42/cyberdrop_dl/base_functions/sorting_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12707 2023-05-21 23:43:50.000000 cyberdrop-dl-4.2.42/cyberdrop_dl/base_functions/sql_helper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 23:43:59.701133 cyberdrop-dl-4.2.42/cyberdrop_dl/client/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-21 23:43:50.000000 cyberdrop-dl-4.2.42/cyberdrop_dl/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10099 2023-05-21 23:43:50.000000 cyberdrop-dl-4.2.42/cyberdrop_dl/client/client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 23:43:59.705133 cyberdrop-dl-4.2.42/cyberdrop_dl/crawlers/
+-rw-r--r--   0 runner    (1001) docker     (123)     2217 2023-05-21 23:43:50.000000 cyberdrop-dl-4.2.42/cyberdrop_dl/crawlers/Anonfiles_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8196 2023-05-21 23:43:50.000000 cyberdrop-dl-4.2.42/cyberdrop_dl/crawlers/Bunkr_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7922 2023-05-21 23:43:50.000000 cyberdrop-dl-4.2.42/cyberdrop_dl/crawlers/Coomeno_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12903 2023-05-21 23:43:50.000000 cyberdrop-dl-4.2.42/cyberdrop_dl/crawlers/CyberFile_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3042 2023-05-21 23:43:50.000000 cyberdrop-dl-4.2.42/cyberdrop_dl/crawlers/Cyberdrop_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3089 2023-05-21 23:43:50.000000 cyberdrop-dl-4.2.42/cyberdrop_dl/crawlers/EHentai_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4239 2023-05-21 23:43:50.000000 cyberdrop-dl-4.2.42/cyberdrop_dl/crawlers/Erome_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4206 2023-05-21 23:43:50.000000 cyberdrop-dl-4.2.42/cyberdrop_dl/crawlers/Fapello_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1890 2023-05-21 23:43:50.000000 cyberdrop-dl-4.2.42/cyberdrop_dl/crawlers/Gfycat_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5069 2023-05-21 23:43:50.000000 cyberdrop-dl-4.2.42/cyberdrop_dl/crawlers/GoFile_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2884 2023-05-21 23:43:50.000000 cyberdrop-dl-4.2.42/cyberdrop_dl/crawlers/HGameCG_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3140 2023-05-21 23:43:50.000000 cyberdrop-dl-4.2.42/cyberdrop_dl/crawlers/ImgBox_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3676 2023-05-21 23:43:50.000000 cyberdrop-dl-4.2.42/cyberdrop_dl/crawlers/LoveFap_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4389 2023-05-21 23:43:50.000000 cyberdrop-dl-4.2.42/cyberdrop_dl/crawlers/NSFWXXX_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2918 2023-05-21 23:43:50.000000 cyberdrop-dl-4.2.42/cyberdrop_dl/crawlers/PimpAndHost_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3362 2023-05-21 23:43:50.000000 cyberdrop-dl-4.2.42/cyberdrop_dl/crawlers/PixelDrain_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3008 2023-05-21 23:43:50.000000 cyberdrop-dl-4.2.42/cyberdrop_dl/crawlers/PostImg_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1499 2023-05-21 23:43:50.000000 cyberdrop-dl-4.2.42/cyberdrop_dl/crawlers/Saint_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9157 2023-05-21 23:43:50.000000 cyberdrop-dl-4.2.42/cyberdrop_dl/crawlers/ShareX_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2186 2023-05-21 23:43:50.000000 cyberdrop-dl-4.2.42/cyberdrop_dl/crawlers/XBunkr_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13919 2023-05-21 23:43:50.000000 cyberdrop-dl-4.2.42/cyberdrop_dl/crawlers/Xenforo_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-21 23:43:50.000000 cyberdrop-dl-4.2.42/cyberdrop_dl/crawlers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 23:43:59.709133 cyberdrop-dl-4.2.42/cyberdrop_dl/downloader/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-21 23:43:50.000000 cyberdrop-dl-4.2.42/cyberdrop_dl/downloader/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2924 2023-05-21 23:43:50.000000 cyberdrop-dl-4.2.42/cyberdrop_dl/downloader/downloader_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18477 2023-05-21 23:43:50.000000 cyberdrop-dl-4.2.42/cyberdrop_dl/downloader/downloaders.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12870 2023-05-21 23:43:50.000000 cyberdrop-dl-4.2.42/cyberdrop_dl/downloader/old_downloaders.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17463 2023-05-21 23:43:50.000000 cyberdrop-dl-4.2.42/cyberdrop_dl/downloader/progress_definitions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20536 2023-05-21 23:43:50.000000 cyberdrop-dl-4.2.42/cyberdrop_dl/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 23:43:59.709133 cyberdrop-dl-4.2.42/cyberdrop_dl/scraper/
+-rw-r--r--   0 runner    (1001) docker     (123)     2531 2023-05-21 23:43:50.000000 cyberdrop-dl-4.2.42/cyberdrop_dl/scraper/JDownloader_Integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20427 2023-05-21 23:43:50.000000 cyberdrop-dl-4.2.42/cyberdrop_dl/scraper/Scraper.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-21 23:43:50.000000 cyberdrop-dl-4.2.42/cyberdrop_dl/scraper/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 23:43:59.701133 cyberdrop-dl-4.2.42/cyberdrop_dl.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    18155 2023-05-21 23:43:59.000000 cyberdrop-dl-4.2.42/cyberdrop_dl.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1933 2023-05-21 23:43:59.000000 cyberdrop-dl-4.2.42/cyberdrop_dl.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-21 23:43:59.000000 cyberdrop-dl-4.2.42/cyberdrop_dl.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-05-21 23:43:59.000000 cyberdrop-dl-4.2.42/cyberdrop_dl.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      176 2023-05-21 23:43:59.000000 cyberdrop-dl-4.2.42/cyberdrop_dl.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-21 23:43:59.000000 cyberdrop-dl-4.2.42/cyberdrop_dl.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-21 23:43:50.000000 cyberdrop-dl-4.2.42/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      860 2023-05-21 23:43:59.709133 cyberdrop-dl-4.2.42/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-21 23:43:50.000000 cyberdrop-dl-4.2.42/setup.py
```

### Comparing `cyberdrop-dl-4.2.41/LICENSE` & `cyberdrop-dl-4.2.42/LICENSE`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.41/PKG-INFO` & `cyberdrop-dl-4.2.42/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cyberdrop-dl
-Version: 4.2.41
+Version: 4.2.42
 Summary: Bulk downloader for multiple file hosts and forum sites
 Home-page: https://github.com/Jules-WinnfieldX/CyberDropDownloader
 Author: Jules-WinnfieldX
 Author-email: JulesWinnfieldII@protonmail.com
 Project-URL: Bug Tracker, https://github.com/Jules-WinnfieldX/CyberDropDownloader/issues
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: cyberdrop-dl Version: 4.2.41 Summary: Bulk
+Metadata-Version: 2.1 Name: cyberdrop-dl Version: 4.2.42 Summary: Bulk
 downloader for multiple file hosts and forum sites Home-page: https://
 github.com/Jules-WinnfieldX/CyberDropDownloader Author: Jules-WinnfieldX
 Author-email: JulesWinnfieldII@protonmail.com Project-URL: Bug Tracker, https:/
 /github.com/Jules-WinnfieldX/CyberDropDownloader/issues Requires-Python: >=3.7
 Description-Content-Type: text/markdown License-File: LICENSE # `cyberdrop-dl`
 **Bulk downloader for multiple file hosts** [![PyPI version](https://
 badge.fury.io/py/cyberdrop-dl.svg)](https://badge.fury.io/py/cyberdrop-dl) [!
```

### Comparing `cyberdrop-dl-4.2.41/README.md` & `cyberdrop-dl-4.2.42/README.md`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.41/cyberdrop_dl/base_functions/base_functions.py` & `cyberdrop-dl-4.2.42/cyberdrop_dl/base_functions/base_functions.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.41/cyberdrop_dl/base_functions/config_manager.py` & `cyberdrop-dl-4.2.42/cyberdrop_dl/base_functions/config_manager.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.41/cyberdrop_dl/base_functions/config_schema.py` & `cyberdrop-dl-4.2.42/cyberdrop_dl/base_functions/config_schema.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.41/cyberdrop_dl/base_functions/data_classes.py` & `cyberdrop-dl-4.2.42/cyberdrop_dl/base_functions/data_classes.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.41/cyberdrop_dl/base_functions/error_classes.py` & `cyberdrop-dl-4.2.42/cyberdrop_dl/base_functions/error_classes.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.41/cyberdrop_dl/base_functions/sorting_functions.py` & `cyberdrop-dl-4.2.42/cyberdrop_dl/base_functions/sorting_functions.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.41/cyberdrop_dl/base_functions/sql_helper.py` & `cyberdrop-dl-4.2.42/cyberdrop_dl/base_functions/sql_helper.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.41/cyberdrop_dl/client/client.py` & `cyberdrop-dl-4.2.42/cyberdrop_dl/client/client.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.41/cyberdrop_dl/crawlers/Anonfiles_Spider.py` & `cyberdrop-dl-4.2.42/cyberdrop_dl/crawlers/Anonfiles_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.41/cyberdrop_dl/crawlers/Bunkr_Spider.py` & `cyberdrop-dl-4.2.42/cyberdrop_dl/crawlers/Bunkr_Spider.py`

 * *Files 3% similar despite different names*

```diff
@@ -27,58 +27,71 @@
         self.quiet = quiet
         self.SQL_Helper = SQL_Helper
         self.remove_bunkr_id = remove_bunkr_id
         self.limiter = AsyncLimiter(20, 1)
 
         self.error_writer = error_writer
 
+    async def get_stream_link(self, url: URL):
+        cdn_possibilities = r"(?:cdn.bunkr...|cdn..bunkr...|cdn...bunkr...|media-files.bunkr...|media-files..bunkr...|media-files...bunkr...)"
+        ext = '.' + url.parts[-1].split('.')[-1]
+        if ext:
+            ext = ext.lower()
+        else:
+            return url
+
+        if ext in FILE_FORMATS['Images']:
+            url = URL(str(url).replace("https://cdn", "https://i"))
+        elif ext in FILE_FORMATS['Videos']:
+            url = URL(re.sub(cdn_possibilities, "bunkr.la/v", str(url)))
+        else:
+            url = URL(re.sub(cdn_possibilities, "bunkr.la/d", str(url)))
+        return url
+
     async def fetch(self, session: ScrapeSession, url: URL) -> AlbumItem:
         """Scraper for Bunkr"""
         album_obj = AlbumItem("Loose Bunkr Files", [])
         log(f"Starting: {url}", quiet=self.quiet, style="green")
 
+        url = await self.get_stream_link(url)
+
         if "v" in url.parts or "d" in url.parts:
             media = await self.get_file(session, url)
             if not media.filename:
                 return album_obj
             await album_obj.add_media(media)
             log(f"Finished: {url}", quiet=self.quiet, style="green")
             if not media.complete:
                 await self.SQL_Helper.insert_media("bunkr", "", media)
             return album_obj
 
-        if "a" in url.parts:
+        elif "a" in url.parts:
             album_obj = await self.get_album(session, url)
             await self.SQL_Helper.insert_album("bunkr", url, album_obj)
 
             if album_obj.media:
                 log(f"Finished: {url}", quiet=self.quiet, style="green")
             return album_obj
 
-        cdn_possibilities = r"(?:cdn.bunkr...|cdn..bunkr...|cdn...bunkr...|media-files.bunkr...|media-files..bunkr...|media-files...bunkr...)"
-        ext = '.' + url.parts[-1].split('.')[-1]
-        if ext:
-            ext = ext.lower()
-        if ext in FILE_FORMATS['Images']:
-            filename, ext = await get_filename_and_ext(url.name)
-            original_filename, filename = await self.remove_id(filename, ext)
+        else:
+            ext = '.' + url.parts[-1].split('.')[-1]
+            if ext:
+                ext = ext.lower()
+            if ext in FILE_FORMATS['Images']:
+                filename, ext = await get_filename_and_ext(url.name)
+                original_filename, filename = await self.remove_id(filename, ext)
 
-            await self.SQL_Helper.fix_bunkr_entries(url, original_filename)
-            check_complete = await self.SQL_Helper.check_complete_singular("bunkr", url)
+                await self.SQL_Helper.fix_bunkr_entries(url, original_filename)
+                check_complete = await self.SQL_Helper.check_complete_singular("bunkr", url)
 
-            url = URL(str(url).replace("https://cdn", "https://i"))
-            media_item = MediaItem(url, url, check_complete, filename, ext, original_filename)
-            await album_obj.add_media(media_item)
-        else:
-            if ext in FILE_FORMATS['Videos']:
-                referer = URL(re.sub(cdn_possibilities, "bunkr.la/v", str(url)))
+                media_item = MediaItem(url, url, check_complete, filename, ext, original_filename)
+                await album_obj.add_media(media_item)
             else:
-                referer = URL(re.sub(cdn_possibilities, "bunkr.la/d", str(url)))
-            media_item = await self.get_file(session, referer)
-            await album_obj.add_media(media_item)
+                media_item = await self.get_file(session, url)
+                await album_obj.add_media(media_item)
 
         await self.SQL_Helper.insert_album("bunkr", url, album_obj)
         log(f"Finished: {url}", quiet=self.quiet, style="green")
         return album_obj
 
     async def remove_id(self, filename: str, ext: str):
         """Removes the additional string bunkr adds to the end of every filename"""
@@ -154,14 +167,15 @@
                 link = file.get("href")
                 media_loc = file.select_one("img").get("src").split("//i")[-1].split(".bunkr.")[0]
 
                 assert url.host is not None
                 if link.startswith("/"):
                     link = URL("https://" + url.host + link)
                 link = URL(link)
+                referer = await self.get_stream_link(link)
 
                 try:
                     filename, ext = await get_filename_and_ext(link.name)
                 except NoExtensionFailure:
                     logger.debug("Couldn't get extension for %s", link)
                     continue
 
@@ -176,15 +190,15 @@
                 if ext not in FILE_FORMATS['Images']:
                     link = await self.check_for_la(link)
 
                 original_filename, filename = await self.remove_id(filename, ext)
 
                 await self.SQL_Helper.fix_bunkr_entries(link, original_filename)
                 complete = await self.SQL_Helper.check_complete_singular("bunkr", link)
-                media = MediaItem(link, url, complete, filename, ext, original_filename)
+                media = MediaItem(link, referer, complete, filename, ext, original_filename)
                 await album.add_media(media)
 
         except Exception as e:
             logger.debug("Error encountered while handling %s", url, exc_info=True)
             await self.error_writer.write_errored_scrape(url, e, self.quiet)
 
         return album
```

### Comparing `cyberdrop-dl-4.2.41/cyberdrop_dl/crawlers/Coomeno_Spider.py` & `cyberdrop-dl-4.2.42/cyberdrop_dl/crawlers/Coomeno_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.41/cyberdrop_dl/crawlers/CyberFile_Spider.py` & `cyberdrop-dl-4.2.42/cyberdrop_dl/crawlers/CyberFile_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.41/cyberdrop_dl/crawlers/Cyberdrop_Spider.py` & `cyberdrop-dl-4.2.42/cyberdrop_dl/crawlers/Cyberdrop_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.41/cyberdrop_dl/crawlers/EHentai_Spider.py` & `cyberdrop-dl-4.2.42/cyberdrop_dl/crawlers/EHentai_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.41/cyberdrop_dl/crawlers/Erome_Spider.py` & `cyberdrop-dl-4.2.42/cyberdrop_dl/crawlers/Erome_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.41/cyberdrop_dl/crawlers/Fapello_Spider.py` & `cyberdrop-dl-4.2.42/cyberdrop_dl/crawlers/Fapello_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.41/cyberdrop_dl/crawlers/Gfycat_Spider.py` & `cyberdrop-dl-4.2.42/cyberdrop_dl/crawlers/Gfycat_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.41/cyberdrop_dl/crawlers/GoFile_Spider.py` & `cyberdrop-dl-4.2.42/cyberdrop_dl/crawlers/GoFile_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.41/cyberdrop_dl/crawlers/HGameCG_Spider.py` & `cyberdrop-dl-4.2.42/cyberdrop_dl/crawlers/HGameCG_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.41/cyberdrop_dl/crawlers/ImgBox_Spider.py` & `cyberdrop-dl-4.2.42/cyberdrop_dl/crawlers/ImgBox_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.41/cyberdrop_dl/crawlers/LoveFap_Spider.py` & `cyberdrop-dl-4.2.42/cyberdrop_dl/crawlers/LoveFap_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.41/cyberdrop_dl/crawlers/NSFWXXX_Spider.py` & `cyberdrop-dl-4.2.42/cyberdrop_dl/crawlers/NSFWXXX_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.41/cyberdrop_dl/crawlers/PimpAndHost_Spider.py` & `cyberdrop-dl-4.2.42/cyberdrop_dl/crawlers/PimpAndHost_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.41/cyberdrop_dl/crawlers/PixelDrain_Spider.py` & `cyberdrop-dl-4.2.42/cyberdrop_dl/crawlers/PixelDrain_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.41/cyberdrop_dl/crawlers/PostImg_Spider.py` & `cyberdrop-dl-4.2.42/cyberdrop_dl/crawlers/PostImg_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.41/cyberdrop_dl/crawlers/Saint_Spider.py` & `cyberdrop-dl-4.2.42/cyberdrop_dl/crawlers/Saint_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.41/cyberdrop_dl/crawlers/ShareX_Spider.py` & `cyberdrop-dl-4.2.42/cyberdrop_dl/crawlers/ShareX_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.41/cyberdrop_dl/crawlers/XBunkr_Spider.py` & `cyberdrop-dl-4.2.42/cyberdrop_dl/crawlers/XBunkr_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.41/cyberdrop_dl/crawlers/Xenforo_Spider.py` & `cyberdrop-dl-4.2.42/cyberdrop_dl/crawlers/Xenforo_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.41/cyberdrop_dl/downloader/downloader_utils.py` & `cyberdrop-dl-4.2.42/cyberdrop_dl/downloader/downloader_utils.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.41/cyberdrop_dl/downloader/downloaders.py` & `cyberdrop-dl-4.2.42/cyberdrop_dl/downloader/downloaders.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.41/cyberdrop_dl/downloader/old_downloaders.py` & `cyberdrop-dl-4.2.42/cyberdrop_dl/downloader/old_downloaders.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.41/cyberdrop_dl/downloader/progress_definitions.py` & `cyberdrop-dl-4.2.42/cyberdrop_dl/downloader/progress_definitions.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.41/cyberdrop_dl/main.py` & `cyberdrop-dl-4.2.42/cyberdrop_dl/main.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.41/cyberdrop_dl/scraper/JDownloader_Integration.py` & `cyberdrop-dl-4.2.42/cyberdrop_dl/scraper/JDownloader_Integration.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.41/cyberdrop_dl/scraper/Scraper.py` & `cyberdrop-dl-4.2.42/cyberdrop_dl/scraper/Scraper.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.41/cyberdrop_dl.egg-info/PKG-INFO` & `cyberdrop-dl-4.2.42/cyberdrop_dl.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cyberdrop-dl
-Version: 4.2.41
+Version: 4.2.42
 Summary: Bulk downloader for multiple file hosts and forum sites
 Home-page: https://github.com/Jules-WinnfieldX/CyberDropDownloader
 Author: Jules-WinnfieldX
 Author-email: JulesWinnfieldII@protonmail.com
 Project-URL: Bug Tracker, https://github.com/Jules-WinnfieldX/CyberDropDownloader/issues
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: cyberdrop-dl Version: 4.2.41 Summary: Bulk
+Metadata-Version: 2.1 Name: cyberdrop-dl Version: 4.2.42 Summary: Bulk
 downloader for multiple file hosts and forum sites Home-page: https://
 github.com/Jules-WinnfieldX/CyberDropDownloader Author: Jules-WinnfieldX
 Author-email: JulesWinnfieldII@protonmail.com Project-URL: Bug Tracker, https:/
 /github.com/Jules-WinnfieldX/CyberDropDownloader/issues Requires-Python: >=3.7
 Description-Content-Type: text/markdown License-File: LICENSE # `cyberdrop-dl`
 **Bulk downloader for multiple file hosts** [![PyPI version](https://
 badge.fury.io/py/cyberdrop-dl.svg)](https://badge.fury.io/py/cyberdrop-dl) [!
```

### Comparing `cyberdrop-dl-4.2.41/cyberdrop_dl.egg-info/SOURCES.txt` & `cyberdrop-dl-4.2.42/cyberdrop_dl.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.41/setup.cfg` & `cyberdrop-dl-4.2.42/setup.cfg`

 * *Files identical despite different names*

