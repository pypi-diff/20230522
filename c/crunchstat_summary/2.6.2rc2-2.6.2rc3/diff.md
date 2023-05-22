# Comparing `tmp/crunchstat_summary-2.6.2rc2.tar.gz` & `tmp/crunchstat_summary-2.6.2rc3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was ".upload_dist/crunchstat_summary-2.6.2rc2.tar", last modified: Fri Apr 21 19:29:48 2023, max compression
+gzip compressed data, was ".upload_dist/crunchstat_summary-2.6.2rc3.tar", last modified: Mon May  1 21:20:16 2023, max compression
```

## Comparing `crunchstat_summary-2.6.2rc2.tar` & `crunchstat_summary-2.6.2rc3.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 jenkins   (1001) jenkins   (1002)        0 2023-04-21 19:29:48.000000 crunchstat_summary-2.6.2rc2/
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)      226 2023-04-21 19:29:21.000000 crunchstat_summary-2.6.2rc2/MANIFEST.in
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)      380 2023-04-21 19:29:48.000000 crunchstat_summary-2.6.2rc2/PKG-INFO
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)      130 2023-04-21 19:29:21.000000 crunchstat_summary-2.6.2rc2/README.rst
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)    34520 2023-04-21 19:29:21.000000 crunchstat_summary-2.6.2rc2/agpl-3.0.txt
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)     2028 2023-04-21 19:29:21.000000 crunchstat_summary-2.6.2rc2/arvados_version.py
-drwxr-xr-x   0 jenkins   (1001) jenkins   (1002)        0 2023-04-21 19:29:48.000000 crunchstat_summary-2.6.2rc2/bin/
--rwxr-xr-x   0 jenkins   (1001) jenkins   (1002)      475 2023-04-21 19:29:21.000000 crunchstat_summary-2.6.2rc2/bin/crunchstat-summary
-drwxr-xr-x   0 jenkins   (1001) jenkins   (1002)        0 2023-04-21 19:29:48.000000 crunchstat_summary-2.6.2rc2/crunchstat_summary/
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)      191 2023-04-21 19:29:21.000000 crunchstat_summary-2.6.2rc2/crunchstat_summary/__init__.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)       25 2023-04-21 19:29:47.000000 crunchstat_summary-2.6.2rc2/crunchstat_summary/_version.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)     3720 2023-04-21 19:29:21.000000 crunchstat_summary-2.6.2rc2/crunchstat_summary/command.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)     3017 2023-04-21 19:29:21.000000 crunchstat_summary-2.6.2rc2/crunchstat_summary/dygraphs.js
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)     1754 2023-04-21 19:29:21.000000 crunchstat_summary-2.6.2rc2/crunchstat_summary/dygraphs.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)     3380 2023-04-21 19:29:21.000000 crunchstat_summary-2.6.2rc2/crunchstat_summary/reader.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)    30650 2023-04-21 19:29:21.000000 crunchstat_summary-2.6.2rc2/crunchstat_summary/summarizer.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)     8454 2023-04-21 19:29:21.000000 crunchstat_summary-2.6.2rc2/crunchstat_summary/synchronizer.js
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)     2131 2023-04-21 19:29:21.000000 crunchstat_summary-2.6.2rc2/crunchstat_summary/webchart.py
-drwxr-xr-x   0 jenkins   (1001) jenkins   (1002)        0 2023-04-21 19:29:48.000000 crunchstat_summary-2.6.2rc2/crunchstat_summary.egg-info/
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)      380 2023-04-21 19:29:48.000000 crunchstat_summary-2.6.2rc2/crunchstat_summary.egg-info/PKG-INFO
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)      618 2023-04-21 19:29:48.000000 crunchstat_summary-2.6.2rc2/crunchstat_summary.egg-info/SOURCES.txt
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)        1 2023-04-21 19:29:48.000000 crunchstat_summary-2.6.2rc2/crunchstat_summary.egg-info/dependency_links.txt
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)        1 2021-06-03 18:28:10.000000 crunchstat_summary-2.6.2rc2/crunchstat_summary.egg-info/not-zip-safe
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)       32 2023-04-21 19:29:48.000000 crunchstat_summary-2.6.2rc2/crunchstat_summary.egg-info/requires.txt
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)       19 2023-04-21 19:29:48.000000 crunchstat_summary-2.6.2rc2/crunchstat_summary.egg-info/top_level.txt
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)       38 2023-04-21 19:29:48.000000 crunchstat_summary-2.6.2rc2/setup.cfg
--rwxr-xr-x   0 jenkins   (1001) jenkins   (1002)     1558 2023-04-21 19:29:21.000000 crunchstat_summary-2.6.2rc2/setup.py
+drwxr-xr-x   0 jenkins   (1001) jenkins   (1002)        0 2023-05-01 21:20:16.000000 crunchstat_summary-2.6.2rc3/
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)      226 2023-04-21 19:29:21.000000 crunchstat_summary-2.6.2rc3/MANIFEST.in
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)      380 2023-05-01 21:20:16.000000 crunchstat_summary-2.6.2rc3/PKG-INFO
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)      130 2023-04-21 19:29:21.000000 crunchstat_summary-2.6.2rc3/README.rst
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)    34520 2023-04-21 19:29:21.000000 crunchstat_summary-2.6.2rc3/agpl-3.0.txt
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)     2028 2023-04-21 19:29:21.000000 crunchstat_summary-2.6.2rc3/arvados_version.py
+drwxr-xr-x   0 jenkins   (1001) jenkins   (1002)        0 2023-05-01 21:20:16.000000 crunchstat_summary-2.6.2rc3/bin/
+-rwxr-xr-x   0 jenkins   (1001) jenkins   (1002)      475 2023-04-21 19:29:21.000000 crunchstat_summary-2.6.2rc3/bin/crunchstat-summary
+drwxr-xr-x   0 jenkins   (1001) jenkins   (1002)        0 2023-05-01 21:20:16.000000 crunchstat_summary-2.6.2rc3/crunchstat_summary/
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)      191 2023-04-21 19:29:21.000000 crunchstat_summary-2.6.2rc3/crunchstat_summary/__init__.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)       25 2023-05-01 21:20:16.000000 crunchstat_summary-2.6.2rc3/crunchstat_summary/_version.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)     3720 2023-04-21 19:29:21.000000 crunchstat_summary-2.6.2rc3/crunchstat_summary/command.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)     3017 2023-04-21 19:29:21.000000 crunchstat_summary-2.6.2rc3/crunchstat_summary/dygraphs.js
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)     1754 2023-04-21 19:29:21.000000 crunchstat_summary-2.6.2rc3/crunchstat_summary/dygraphs.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)     3380 2023-04-21 19:29:21.000000 crunchstat_summary-2.6.2rc3/crunchstat_summary/reader.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)    30650 2023-04-21 19:29:21.000000 crunchstat_summary-2.6.2rc3/crunchstat_summary/summarizer.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)     8454 2023-04-21 19:29:21.000000 crunchstat_summary-2.6.2rc3/crunchstat_summary/synchronizer.js
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)     2131 2023-04-21 19:29:21.000000 crunchstat_summary-2.6.2rc3/crunchstat_summary/webchart.py
+drwxr-xr-x   0 jenkins   (1001) jenkins   (1002)        0 2023-05-01 21:20:16.000000 crunchstat_summary-2.6.2rc3/crunchstat_summary.egg-info/
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)      380 2023-05-01 21:20:16.000000 crunchstat_summary-2.6.2rc3/crunchstat_summary.egg-info/PKG-INFO
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)      618 2023-05-01 21:20:16.000000 crunchstat_summary-2.6.2rc3/crunchstat_summary.egg-info/SOURCES.txt
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)        1 2023-05-01 21:20:16.000000 crunchstat_summary-2.6.2rc3/crunchstat_summary.egg-info/dependency_links.txt
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)        1 2021-06-03 18:28:10.000000 crunchstat_summary-2.6.2rc3/crunchstat_summary.egg-info/not-zip-safe
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)       32 2023-05-01 21:20:16.000000 crunchstat_summary-2.6.2rc3/crunchstat_summary.egg-info/requires.txt
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)       19 2023-05-01 21:20:16.000000 crunchstat_summary-2.6.2rc3/crunchstat_summary.egg-info/top_level.txt
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)       38 2023-05-01 21:20:16.000000 crunchstat_summary-2.6.2rc3/setup.cfg
+-rwxr-xr-x   0 jenkins   (1001) jenkins   (1002)     1558 2023-04-21 19:29:21.000000 crunchstat_summary-2.6.2rc3/setup.py
```

### Comparing `crunchstat_summary-2.6.2rc2/agpl-3.0.txt` & `crunchstat_summary-2.6.2rc3/agpl-3.0.txt`

 * *Files identical despite different names*

### Comparing `crunchstat_summary-2.6.2rc2/arvados_version.py` & `crunchstat_summary-2.6.2rc3/arvados_version.py`

 * *Files identical despite different names*

### Comparing `crunchstat_summary-2.6.2rc2/crunchstat_summary/command.py` & `crunchstat_summary-2.6.2rc3/crunchstat_summary/command.py`

 * *Files identical despite different names*

### Comparing `crunchstat_summary-2.6.2rc2/crunchstat_summary/dygraphs.js` & `crunchstat_summary-2.6.2rc3/crunchstat_summary/dygraphs.js`

 * *Files identical despite different names*

### Comparing `crunchstat_summary-2.6.2rc2/crunchstat_summary/dygraphs.py` & `crunchstat_summary-2.6.2rc3/crunchstat_summary/dygraphs.py`

 * *Files identical despite different names*

### Comparing `crunchstat_summary-2.6.2rc2/crunchstat_summary/reader.py` & `crunchstat_summary-2.6.2rc3/crunchstat_summary/reader.py`

 * *Files identical despite different names*

### Comparing `crunchstat_summary-2.6.2rc2/crunchstat_summary/summarizer.py` & `crunchstat_summary-2.6.2rc3/crunchstat_summary/summarizer.py`

 * *Files identical despite different names*

### Comparing `crunchstat_summary-2.6.2rc2/crunchstat_summary/synchronizer.js` & `crunchstat_summary-2.6.2rc3/crunchstat_summary/synchronizer.js`

 * *Files identical despite different names*

### Comparing `crunchstat_summary-2.6.2rc2/crunchstat_summary/webchart.py` & `crunchstat_summary-2.6.2rc3/crunchstat_summary/webchart.py`

 * *Files identical despite different names*

### Comparing `crunchstat_summary-2.6.2rc2/crunchstat_summary.egg-info/SOURCES.txt` & `crunchstat_summary-2.6.2rc3/crunchstat_summary.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `crunchstat_summary-2.6.2rc2/setup.py` & `crunchstat_summary-2.6.2rc3/setup.py`

 * *Files identical despite different names*

