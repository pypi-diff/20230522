# Comparing `tmp/hftbacktest-1.6.0.tar.gz` & `tmp/hftbacktest-1.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hftbacktest-1.6.0.tar", last modified: Thu May 18 14:43:53 2023, max compression
+gzip compressed data, was "hftbacktest-1.6.1.tar", last modified: Mon May 22 14:36:49 2023, max compression
```

## Comparing `hftbacktest-1.6.0.tar` & `hftbacktest-1.6.1.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxr-xr-x   0 nkaz001   (1000) nkaz001   (1000)        0 2023-05-18 14:43:53.086622 hftbacktest-1.6.0/
--rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)     1079 2023-04-27 05:42:48.000000 hftbacktest-1.6.0/LICENSE
--rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)     6805 2023-05-18 14:43:53.086622 hftbacktest-1.6.0/PKG-INFO
--rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)     5696 2023-05-10 14:57:57.000000 hftbacktest-1.6.0/README.rst
-drwxr-xr-x   0 nkaz001   (1000) nkaz001   (1000)        0 2023-05-18 14:43:53.085622 hftbacktest-1.6.0/hftbacktest/
--rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)    11523 2023-05-18 13:06:32.000000 hftbacktest-1.6.0/hftbacktest/__init__.py
--rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)     1011 2023-04-27 05:42:48.000000 hftbacktest-1.6.0/hftbacktest/assettype.py
--rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)    15671 2023-05-17 15:15:26.000000 hftbacktest-1.6.0/hftbacktest/backtest.py
-drwxr-xr-x   0 nkaz001   (1000) nkaz001   (1000)        0 2023-05-18 14:43:53.085622 hftbacktest-1.6.0/hftbacktest/data/
--rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)     1592 2023-04-27 05:42:48.000000 hftbacktest-1.6.0/hftbacktest/data/__init__.py
-drwxr-xr-x   0 nkaz001   (1000) nkaz001   (1000)        0 2023-05-18 14:43:53.086622 hftbacktest-1.6.0/hftbacktest/data/utils/
--rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)       44 2023-04-27 05:42:48.000000 hftbacktest-1.6.0/hftbacktest/data/utils/__init__.py
--rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)    11484 2023-04-28 13:21:33.000000 hftbacktest-1.6.0/hftbacktest/data/utils/binancefutures.py
--rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)     2160 2023-04-30 14:00:09.000000 hftbacktest-1.6.0/hftbacktest/data/utils/snapshot.py
--rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)     6901 2023-04-28 13:18:47.000000 hftbacktest-1.6.0/hftbacktest/data/utils/tardis.py
--rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)    11553 2023-04-28 12:19:24.000000 hftbacktest-1.6.0/hftbacktest/data/validation.py
-drwxr-xr-x   0 nkaz001   (1000) nkaz001   (1000)        0 2023-05-18 14:43:53.086622 hftbacktest-1.6.0/hftbacktest/experimental/
--rwxr-xr-x   0 nkaz001   (1000) nkaz001   (1000)        0 2023-04-29 10:30:43.000000 hftbacktest-1.6.0/hftbacktest/experimental/__init__.py
--rwxr-xr-x   0 nkaz001   (1000) nkaz001   (1000)    14543 2023-05-11 12:00:41.000000 hftbacktest-1.6.0/hftbacktest/experimental/backtest.py
-drwxr-xr-x   0 nkaz001   (1000) nkaz001   (1000)        0 2023-05-18 14:43:53.086622 hftbacktest-1.6.0/hftbacktest/experimental/live/
--rwxr-xr-x   0 nkaz001   (1000) nkaz001   (1000)        0 2023-04-29 10:30:43.000000 hftbacktest-1.6.0/hftbacktest/experimental/live/__init__.py
--rwxr-xr-x   0 nkaz001   (1000) nkaz001   (1000)    19630 2023-04-29 10:30:43.000000 hftbacktest-1.6.0/hftbacktest/experimental/live/binancefutures.py
--rwxr-xr-x   0 nkaz001   (1000) nkaz001   (1000)      333 2023-04-29 10:30:43.000000 hftbacktest-1.6.0/hftbacktest/experimental/live/custom_strategy.py
--rwxr-xr-x   0 nkaz001   (1000) nkaz001   (1000)     7792 2023-04-29 10:30:43.000000 hftbacktest-1.6.0/hftbacktest/experimental/live/ordermanager.py
--rwxr-xr-x   0 nkaz001   (1000) nkaz001   (1000)     3578 2023-04-29 10:30:43.000000 hftbacktest-1.6.0/hftbacktest/experimental/live/settings.py
--rwxr-xr-x   0 nkaz001   (1000) nkaz001   (1000)     6817 2023-05-11 11:48:17.000000 hftbacktest-1.6.0/hftbacktest/experimental/multiasset.py
--rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)     6194 2023-04-27 05:42:48.000000 hftbacktest-1.6.0/hftbacktest/marketdepth.py
-drwxr-xr-x   0 nkaz001   (1000) nkaz001   (1000)        0 2023-05-18 14:43:53.086622 hftbacktest-1.6.0/hftbacktest/models/
--rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)        0 2023-04-27 05:42:48.000000 hftbacktest-1.6.0/hftbacktest/models/__init__.py
--rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)    10010 2023-04-29 14:47:02.000000 hftbacktest-1.6.0/hftbacktest/models/latencies.py
--rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)     3305 2023-04-27 05:42:48.000000 hftbacktest-1.6.0/hftbacktest/models/queue.py
--rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)     4150 2023-05-17 14:22:00.000000 hftbacktest-1.6.0/hftbacktest/order.py
-drwxr-xr-x   0 nkaz001   (1000) nkaz001   (1000)        0 2023-05-18 14:43:53.086622 hftbacktest-1.6.0/hftbacktest/proc/
--rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)        0 2023-04-27 05:42:48.000000 hftbacktest-1.6.0/hftbacktest/proc/__init__.py
--rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)     6538 2023-05-18 14:26:22.000000 hftbacktest-1.6.0/hftbacktest/proc/local.py
--rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)    19211 2023-05-18 13:30:05.000000 hftbacktest-1.6.0/hftbacktest/proc/nopartialfillexchange.py
--rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)    29420 2023-05-18 13:41:42.000000 hftbacktest-1.6.0/hftbacktest/proc/partialfillexchange.py
--rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)     5899 2023-05-10 12:56:12.000000 hftbacktest-1.6.0/hftbacktest/proc/proc.py
--rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)     3252 2023-04-27 05:42:48.000000 hftbacktest-1.6.0/hftbacktest/reader.py
--rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)    13687 2023-05-10 13:22:50.000000 hftbacktest-1.6.0/hftbacktest/stat.py
--rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)     2149 2023-05-11 12:00:32.000000 hftbacktest-1.6.0/hftbacktest/state.py
--rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)      876 2023-05-11 11:04:39.000000 hftbacktest-1.6.0/hftbacktest/typing.py
-drwxr-xr-x   0 nkaz001   (1000) nkaz001   (1000)        0 2023-05-18 14:43:53.085622 hftbacktest-1.6.0/hftbacktest.egg-info/
--rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)     6805 2023-05-18 14:43:53.000000 hftbacktest-1.6.0/hftbacktest.egg-info/PKG-INFO
--rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)     1248 2023-05-18 14:43:53.000000 hftbacktest-1.6.0/hftbacktest.egg-info/SOURCES.txt
--rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)        1 2023-05-18 14:43:53.000000 hftbacktest-1.6.0/hftbacktest.egg-info/dependency_links.txt
--rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)        1 2023-04-28 14:15:39.000000 hftbacktest-1.6.0/hftbacktest.egg-info/not-zip-safe
--rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)       48 2023-05-18 14:43:53.000000 hftbacktest-1.6.0/hftbacktest.egg-info/requires.txt
--rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)       12 2023-05-18 14:43:53.000000 hftbacktest-1.6.0/hftbacktest.egg-info/top_level.txt
--rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)     1249 2023-05-18 14:43:53.086622 hftbacktest-1.6.0/setup.cfg
--rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)       61 2023-04-27 05:42:48.000000 hftbacktest-1.6.0/setup.py
+drwxr-xr-x   0 nkaz001   (1000) nkaz001   (1000)        0 2023-05-22 14:36:49.875651 hftbacktest-1.6.1/
+-rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)     1079 2023-04-27 05:42:48.000000 hftbacktest-1.6.1/LICENSE
+-rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)     6805 2023-05-22 14:36:49.875651 hftbacktest-1.6.1/PKG-INFO
+-rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)     5696 2023-05-10 14:57:57.000000 hftbacktest-1.6.1/README.rst
+drwxr-xr-x   0 nkaz001   (1000) nkaz001   (1000)        0 2023-05-22 14:36:49.872651 hftbacktest-1.6.1/hftbacktest/
+-rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)    11523 2023-05-22 14:19:54.000000 hftbacktest-1.6.1/hftbacktest/__init__.py
+-rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)     1011 2023-04-27 05:42:48.000000 hftbacktest-1.6.1/hftbacktest/assettype.py
+-rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)    15671 2023-05-17 15:15:26.000000 hftbacktest-1.6.1/hftbacktest/backtest.py
+drwxr-xr-x   0 nkaz001   (1000) nkaz001   (1000)        0 2023-05-22 14:36:49.873651 hftbacktest-1.6.1/hftbacktest/data/
+-rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)     1592 2023-04-27 05:42:48.000000 hftbacktest-1.6.1/hftbacktest/data/__init__.py
+drwxr-xr-x   0 nkaz001   (1000) nkaz001   (1000)        0 2023-05-22 14:36:49.873651 hftbacktest-1.6.1/hftbacktest/data/utils/
+-rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)       44 2023-04-27 05:42:48.000000 hftbacktest-1.6.1/hftbacktest/data/utils/__init__.py
+-rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)    11565 2023-05-22 14:23:10.000000 hftbacktest-1.6.1/hftbacktest/data/utils/binancefutures.py
+-rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)     2160 2023-04-30 14:00:09.000000 hftbacktest-1.6.1/hftbacktest/data/utils/snapshot.py
+-rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)     6901 2023-04-28 13:18:47.000000 hftbacktest-1.6.1/hftbacktest/data/utils/tardis.py
+-rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)    11553 2023-04-28 12:19:24.000000 hftbacktest-1.6.1/hftbacktest/data/validation.py
+drwxr-xr-x   0 nkaz001   (1000) nkaz001   (1000)        0 2023-05-22 14:36:49.873651 hftbacktest-1.6.1/hftbacktest/experimental/
+-rwxr-xr-x   0 nkaz001   (1000) nkaz001   (1000)        0 2023-04-29 10:30:43.000000 hftbacktest-1.6.1/hftbacktest/experimental/__init__.py
+-rwxr-xr-x   0 nkaz001   (1000) nkaz001   (1000)    14543 2023-05-11 12:00:41.000000 hftbacktest-1.6.1/hftbacktest/experimental/backtest.py
+drwxr-xr-x   0 nkaz001   (1000) nkaz001   (1000)        0 2023-05-22 14:36:49.874652 hftbacktest-1.6.1/hftbacktest/experimental/live/
+-rwxr-xr-x   0 nkaz001   (1000) nkaz001   (1000)        0 2023-04-29 10:30:43.000000 hftbacktest-1.6.1/hftbacktest/experimental/live/__init__.py
+-rwxr-xr-x   0 nkaz001   (1000) nkaz001   (1000)    19630 2023-04-29 10:30:43.000000 hftbacktest-1.6.1/hftbacktest/experimental/live/binancefutures.py
+-rwxr-xr-x   0 nkaz001   (1000) nkaz001   (1000)      333 2023-04-29 10:30:43.000000 hftbacktest-1.6.1/hftbacktest/experimental/live/custom_strategy.py
+-rwxr-xr-x   0 nkaz001   (1000) nkaz001   (1000)     7792 2023-04-29 10:30:43.000000 hftbacktest-1.6.1/hftbacktest/experimental/live/ordermanager.py
+-rwxr-xr-x   0 nkaz001   (1000) nkaz001   (1000)     3578 2023-04-29 10:30:43.000000 hftbacktest-1.6.1/hftbacktest/experimental/live/settings.py
+-rwxr-xr-x   0 nkaz001   (1000) nkaz001   (1000)     6817 2023-05-11 11:48:17.000000 hftbacktest-1.6.1/hftbacktest/experimental/multiasset.py
+-rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)     6194 2023-04-27 05:42:48.000000 hftbacktest-1.6.1/hftbacktest/marketdepth.py
+drwxr-xr-x   0 nkaz001   (1000) nkaz001   (1000)        0 2023-05-22 14:36:49.874652 hftbacktest-1.6.1/hftbacktest/models/
+-rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)        0 2023-04-27 05:42:48.000000 hftbacktest-1.6.1/hftbacktest/models/__init__.py
+-rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)    10010 2023-04-29 14:47:02.000000 hftbacktest-1.6.1/hftbacktest/models/latencies.py
+-rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)     3305 2023-04-27 05:42:48.000000 hftbacktest-1.6.1/hftbacktest/models/queue.py
+-rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)     4150 2023-05-17 14:22:00.000000 hftbacktest-1.6.1/hftbacktest/order.py
+drwxr-xr-x   0 nkaz001   (1000) nkaz001   (1000)        0 2023-05-22 14:36:49.874652 hftbacktest-1.6.1/hftbacktest/proc/
+-rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)        0 2023-04-27 05:42:48.000000 hftbacktest-1.6.1/hftbacktest/proc/__init__.py
+-rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)     6538 2023-05-18 14:26:22.000000 hftbacktest-1.6.1/hftbacktest/proc/local.py
+-rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)    19211 2023-05-18 13:30:05.000000 hftbacktest-1.6.1/hftbacktest/proc/nopartialfillexchange.py
+-rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)    29420 2023-05-18 13:41:42.000000 hftbacktest-1.6.1/hftbacktest/proc/partialfillexchange.py
+-rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)     5899 2023-05-10 12:56:12.000000 hftbacktest-1.6.1/hftbacktest/proc/proc.py
+-rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)     3252 2023-04-27 05:42:48.000000 hftbacktest-1.6.1/hftbacktest/reader.py
+-rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)    13687 2023-05-10 13:22:50.000000 hftbacktest-1.6.1/hftbacktest/stat.py
+-rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)     2149 2023-05-11 12:00:32.000000 hftbacktest-1.6.1/hftbacktest/state.py
+-rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)      876 2023-05-11 11:04:39.000000 hftbacktest-1.6.1/hftbacktest/typing.py
+drwxr-xr-x   0 nkaz001   (1000) nkaz001   (1000)        0 2023-05-22 14:36:49.873651 hftbacktest-1.6.1/hftbacktest.egg-info/
+-rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)     6805 2023-05-22 14:36:49.000000 hftbacktest-1.6.1/hftbacktest.egg-info/PKG-INFO
+-rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)     1248 2023-05-22 14:36:49.000000 hftbacktest-1.6.1/hftbacktest.egg-info/SOURCES.txt
+-rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)        1 2023-05-22 14:36:49.000000 hftbacktest-1.6.1/hftbacktest.egg-info/dependency_links.txt
+-rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)        1 2023-04-28 14:15:39.000000 hftbacktest-1.6.1/hftbacktest.egg-info/not-zip-safe
+-rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)       48 2023-05-22 14:36:49.000000 hftbacktest-1.6.1/hftbacktest.egg-info/requires.txt
+-rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)       12 2023-05-22 14:36:49.000000 hftbacktest-1.6.1/hftbacktest.egg-info/top_level.txt
+-rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)     1249 2023-05-22 14:36:49.875651 hftbacktest-1.6.1/setup.cfg
+-rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)       61 2023-04-27 05:42:48.000000 hftbacktest-1.6.1/setup.py
```

### Comparing `hftbacktest-1.6.0/LICENSE` & `hftbacktest-1.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `hftbacktest-1.6.0/PKG-INFO` & `hftbacktest-1.6.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hftbacktest
-Version: 1.6.0
+Version: 1.6.1
 Summary: High-frequency trading and market making backtesting tool
 Home-page: https://github.com/nkaz001/hftbacktest
 Author: nkaz001
 Author-email: nkaz001@protonmail.com
 License: MIT
 Project-URL: Docs, https://hftbacktest.readthedocs.io/en/latest/
 Project-URL: GitHub: issues, https://github.com/nkaz001/hftbacktest/issues
```

### Comparing `hftbacktest-1.6.0/README.rst` & `hftbacktest-1.6.1/README.rst`

 * *Files identical despite different names*

### Comparing `hftbacktest-1.6.0/hftbacktest/__init__.py` & `hftbacktest-1.6.1/hftbacktest/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -124,15 +124,15 @@
     'validate_data',
     'correct_local_timestamp',
     'correct_exch_timestamp',
     'correct_exch_timestamp_adjust',
     'correct'
 )
 
-__version__ = '1.6.0'
+__version__ = '1.6.1'
 
 
 # JIT'ed latency models
 ConstantLatency = jitclass()(ConstantLatency_)
 FeedLatency = jitclass()(FeedLatency_)
 ForwardFeedLatency = jitclass()(ForwardFeedLatency_)
 BackwardFeedLatency = jitclass()(BackwardFeedLatency_)
```

### Comparing `hftbacktest-1.6.0/hftbacktest/assettype.py` & `hftbacktest-1.6.1/hftbacktest/assettype.py`

 * *Files identical despite different names*

### Comparing `hftbacktest-1.6.0/hftbacktest/backtest.py` & `hftbacktest-1.6.1/hftbacktest/backtest.py`

 * *Files identical despite different names*

### Comparing `hftbacktest-1.6.0/hftbacktest/data/__init__.py` & `hftbacktest-1.6.1/hftbacktest/data/__init__.py`

 * *Files identical despite different names*

### Comparing `hftbacktest-1.6.0/hftbacktest/data/utils/binancefutures.py` & `hftbacktest-1.6.1/hftbacktest/data/utils/binancefutures.py`

 * *Files 1% similar despite different names*

```diff
@@ -64,14 +64,16 @@
                 break
             local_timestamp = int(line[:16])
             message = json.loads(line[17:])
             data = message.get('data')
             if data is not None:
                 evt = data['e']
                 if evt == 'trade':
+                    if data['X'] != 'MARKET':
+                        continue
                     # event_time = data['E']
                     transaction_time = data['T']
                     price = data['p']
                     qty = data['q']
                     side = -1 if data['m'] else 1  # trade initiator's side
                     exch_timestamp = int(transaction_time) * 1000
                     rows.append([2, exch_timestamp, local_timestamp, side, float(price), float(qty)])
```

### Comparing `hftbacktest-1.6.0/hftbacktest/data/utils/snapshot.py` & `hftbacktest-1.6.1/hftbacktest/data/utils/snapshot.py`

 * *Files identical despite different names*

### Comparing `hftbacktest-1.6.0/hftbacktest/data/utils/tardis.py` & `hftbacktest-1.6.1/hftbacktest/data/utils/tardis.py`

 * *Files identical despite different names*

### Comparing `hftbacktest-1.6.0/hftbacktest/data/validation.py` & `hftbacktest-1.6.1/hftbacktest/data/validation.py`

 * *Files identical despite different names*

### Comparing `hftbacktest-1.6.0/hftbacktest/experimental/backtest.py` & `hftbacktest-1.6.1/hftbacktest/experimental/backtest.py`

 * *Files identical despite different names*

### Comparing `hftbacktest-1.6.0/hftbacktest/experimental/live/binancefutures.py` & `hftbacktest-1.6.1/hftbacktest/experimental/live/binancefutures.py`

 * *Files identical despite different names*

### Comparing `hftbacktest-1.6.0/hftbacktest/experimental/live/ordermanager.py` & `hftbacktest-1.6.1/hftbacktest/experimental/live/ordermanager.py`

 * *Files identical despite different names*

### Comparing `hftbacktest-1.6.0/hftbacktest/experimental/live/settings.py` & `hftbacktest-1.6.1/hftbacktest/experimental/live/settings.py`

 * *Files identical despite different names*

### Comparing `hftbacktest-1.6.0/hftbacktest/experimental/multiasset.py` & `hftbacktest-1.6.1/hftbacktest/experimental/multiasset.py`

 * *Files identical despite different names*

### Comparing `hftbacktest-1.6.0/hftbacktest/marketdepth.py` & `hftbacktest-1.6.1/hftbacktest/marketdepth.py`

 * *Files identical despite different names*

### Comparing `hftbacktest-1.6.0/hftbacktest/models/latencies.py` & `hftbacktest-1.6.1/hftbacktest/models/latencies.py`

 * *Files identical despite different names*

### Comparing `hftbacktest-1.6.0/hftbacktest/models/queue.py` & `hftbacktest-1.6.1/hftbacktest/models/queue.py`

 * *Files identical despite different names*

### Comparing `hftbacktest-1.6.0/hftbacktest/order.py` & `hftbacktest-1.6.1/hftbacktest/order.py`

 * *Files identical despite different names*

### Comparing `hftbacktest-1.6.0/hftbacktest/proc/local.py` & `hftbacktest-1.6.1/hftbacktest/proc/local.py`

 * *Files identical despite different names*

### Comparing `hftbacktest-1.6.0/hftbacktest/proc/nopartialfillexchange.py` & `hftbacktest-1.6.1/hftbacktest/proc/nopartialfillexchange.py`

 * *Files identical despite different names*

### Comparing `hftbacktest-1.6.0/hftbacktest/proc/partialfillexchange.py` & `hftbacktest-1.6.1/hftbacktest/proc/partialfillexchange.py`

 * *Files identical despite different names*

### Comparing `hftbacktest-1.6.0/hftbacktest/proc/proc.py` & `hftbacktest-1.6.1/hftbacktest/proc/proc.py`

 * *Files identical despite different names*

### Comparing `hftbacktest-1.6.0/hftbacktest/reader.py` & `hftbacktest-1.6.1/hftbacktest/reader.py`

 * *Files identical despite different names*

### Comparing `hftbacktest-1.6.0/hftbacktest/stat.py` & `hftbacktest-1.6.1/hftbacktest/stat.py`

 * *Files identical despite different names*

### Comparing `hftbacktest-1.6.0/hftbacktest/state.py` & `hftbacktest-1.6.1/hftbacktest/state.py`

 * *Files identical despite different names*

### Comparing `hftbacktest-1.6.0/hftbacktest/typing.py` & `hftbacktest-1.6.1/hftbacktest/typing.py`

 * *Files identical despite different names*

### Comparing `hftbacktest-1.6.0/hftbacktest.egg-info/PKG-INFO` & `hftbacktest-1.6.1/hftbacktest.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hftbacktest
-Version: 1.6.0
+Version: 1.6.1
 Summary: High-frequency trading and market making backtesting tool
 Home-page: https://github.com/nkaz001/hftbacktest
 Author: nkaz001
 Author-email: nkaz001@protonmail.com
 License: MIT
 Project-URL: Docs, https://hftbacktest.readthedocs.io/en/latest/
 Project-URL: GitHub: issues, https://github.com/nkaz001/hftbacktest/issues
```

### Comparing `hftbacktest-1.6.0/hftbacktest.egg-info/SOURCES.txt` & `hftbacktest-1.6.1/hftbacktest.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hftbacktest-1.6.0/setup.cfg` & `hftbacktest-1.6.1/setup.cfg`

 * *Files identical despite different names*

