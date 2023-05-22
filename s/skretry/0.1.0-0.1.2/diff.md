# Comparing `tmp/skretry-0.1.0.tar.gz` & `tmp/skretry-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "skretry-0.1.0.tar", last modified: Mon May 22 08:26:01 2023, max compression
+gzip compressed data, was "skretry-0.1.2.tar", last modified: Mon May 22 08:32:47 2023, max compression
```

## Comparing `skretry-0.1.0.tar` & `skretry-0.1.2.tar`

### file list

```diff
@@ -1,19 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:26:01.173778 skretry-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)      566 2023-05-22 08:25:43.000000 skretry-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5464 2023-05-22 08:26:01.173778 skretry-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4560 2023-05-22 08:25:43.000000 skretry-0.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      878 2023-05-22 08:26:01.173778 skretry-0.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-05-22 08:25:43.000000 skretry-0.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:26:01.173778 skretry-0.1.0/skretry/
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-05-22 08:25:43.000000 skretry-0.1.0/skretry/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6715 2023-05-22 08:25:43.000000 skretry-0.1.0/skretry/api.py
--rw-r--r--   0 runner    (1001) docker     (123)      477 2023-05-22 08:25:43.000000 skretry-0.1.0/skretry/compat.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:26:01.173778 skretry-0.1.0/skretry.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5464 2023-05-22 08:26:01.000000 skretry-0.1.0/skretry.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      283 2023-05-22 08:26:01.000000 skretry-0.1.0/skretry.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 08:26:01.000000 skretry-0.1.0/skretry.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-22 08:26:01.000000 skretry-0.1.0/skretry.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-22 08:26:01.000000 skretry-0.1.0/skretry.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:26:01.173778 skretry-0.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1716 2023-05-22 08:25:43.000000 skretry-0.1.0/tests/test_async.py
--rw-r--r--   0 runner    (1001) docker     (123)     4058 2023-05-22 08:25:43.000000 skretry-0.1.0/tests/test_retry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:32:47.290211 skretry-0.1.2/
+-rw-r--r--   0 runner    (1001) docker     (123)      566 2023-05-22 08:32:35.000000 skretry-0.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      920 2023-05-22 08:32:47.290211 skretry-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-22 08:32:35.000000 skretry-0.1.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      878 2023-05-22 08:32:47.290211 skretry-0.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-05-22 08:32:35.000000 skretry-0.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:32:47.290211 skretry-0.1.2/skretry/
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-05-22 08:32:35.000000 skretry-0.1.2/skretry/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6715 2023-05-22 08:32:35.000000 skretry-0.1.2/skretry/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      477 2023-05-22 08:32:35.000000 skretry-0.1.2/skretry/compat.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:32:47.290211 skretry-0.1.2/skretry.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      920 2023-05-22 08:32:47.000000 skretry-0.1.2/skretry.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      243 2023-05-22 08:32:47.000000 skretry-0.1.2/skretry.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 08:32:47.000000 skretry-0.1.2/skretry.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-22 08:32:47.000000 skretry-0.1.2/skretry.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-22 08:32:47.000000 skretry-0.1.2/skretry.egg-info/top_level.txt
```

### Comparing `skretry-0.1.0/LICENSE` & `skretry-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `skretry-0.1.0/setup.cfg` & `skretry-0.1.2/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = skretry
-version = 0.1.0
+version = 0.1.2
 url = https://github.com/imsgj/skretry
 author = imsgj
 description = An easy to use, but functional decorator for retrying on exceptions.
 license = Apache License 2.0
 long_description = file: README.md
 long_description_content_type = text/markdown
 classifiers =
```

### Comparing `skretry-0.1.0/skretry/api.py` & `skretry-0.1.2/skretry/api.py`

 * *Files identical despite different names*

