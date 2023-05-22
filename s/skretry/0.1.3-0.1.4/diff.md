# Comparing `tmp/skretry-0.1.3.tar.gz` & `tmp/skretry-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "skretry-0.1.3.tar", last modified: Mon May 22 08:38:19 2023, max compression
+gzip compressed data, was "skretry-0.1.4.tar", last modified: Mon May 22 08:43:31 2023, max compression
```

## Comparing `skretry-0.1.3.tar` & `skretry-0.1.4.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:38:19.267486 skretry-0.1.3/
--rw-r--r--   0 runner    (1001) docker     (123)      566 2023-05-22 08:38:07.000000 skretry-0.1.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      920 2023-05-22 08:38:19.267486 skretry-0.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-22 08:38:07.000000 skretry-0.1.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      878 2023-05-22 08:38:19.267486 skretry-0.1.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-05-22 08:38:07.000000 skretry-0.1.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:38:19.263486 skretry-0.1.3/skretry/
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-05-22 08:38:07.000000 skretry-0.1.3/skretry/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6713 2023-05-22 08:38:07.000000 skretry-0.1.3/skretry/api.py
--rw-r--r--   0 runner    (1001) docker     (123)      477 2023-05-22 08:38:07.000000 skretry-0.1.3/skretry/compat.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:38:19.267486 skretry-0.1.3/skretry.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      920 2023-05-22 08:38:19.000000 skretry-0.1.3/skretry.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      243 2023-05-22 08:38:19.000000 skretry-0.1.3/skretry.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 08:38:19.000000 skretry-0.1.3/skretry.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-22 08:38:19.000000 skretry-0.1.3/skretry.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-22 08:38:19.000000 skretry-0.1.3/skretry.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:43:31.885608 skretry-0.1.4/
+-rw-r--r--   0 runner    (1001) docker     (123)      566 2023-05-22 08:43:18.000000 skretry-0.1.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      920 2023-05-22 08:43:31.885608 skretry-0.1.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-22 08:43:18.000000 skretry-0.1.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      878 2023-05-22 08:43:31.885608 skretry-0.1.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-05-22 08:43:18.000000 skretry-0.1.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:43:31.885608 skretry-0.1.4/skretry/
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-05-22 08:43:18.000000 skretry-0.1.4/skretry/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6709 2023-05-22 08:43:18.000000 skretry-0.1.4/skretry/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      477 2023-05-22 08:43:18.000000 skretry-0.1.4/skretry/compat.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:43:31.885608 skretry-0.1.4/skretry.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      920 2023-05-22 08:43:31.000000 skretry-0.1.4/skretry.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      243 2023-05-22 08:43:31.000000 skretry-0.1.4/skretry.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 08:43:31.000000 skretry-0.1.4/skretry.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-22 08:43:31.000000 skretry-0.1.4/skretry.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-22 08:43:31.000000 skretry-0.1.4/skretry.egg-info/top_level.txt
```

### Comparing `skretry-0.1.3/LICENSE` & `skretry-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `skretry-0.1.3/PKG-INFO` & `skretry-0.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: skretry
-Version: 0.1.3
+Version: 0.1.4
 Summary: An easy to use, but functional decorator for retrying on exceptions.
 Home-page: https://github.com/imsgj/skretry
 Author: imsgj
 License: Apache License 2.0
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Natural Language :: English
```

### Comparing `skretry-0.1.3/setup.cfg` & `skretry-0.1.4/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = skretry
-version = 0.1.3
+version = 0.1.4
 url = https://github.com/imsgj/skretry
 author = imsgj
 description = An easy to use, but functional decorator for retrying on exceptions.
 license = Apache License 2.0
 long_description = file: README.md
 long_description_content_type = text/markdown
 classifiers =
```

### Comparing `skretry-0.1.3/skretry/api.py` & `skretry-0.1.4/skretry/api.py`

 * *Files 0% similar despite different names*

```diff
@@ -92,15 +92,15 @@
             logger.error(tb_str)
 
         logger.error(
             f"{e}, attempt {tries - _tries}/{tries} failed - retrying in {_delay} seconds..."
         )
 
     elif tries > 1:
-        logger.exception(
+        logger.error(
             f"{e}, attempt {tries - _tries}/{tries} failed - giving up!"
         )
 
 
 def _new_delay(max_delay, backoff, jitter, _delay):
     _delay *= backoff
     _delay += random.uniform(*jitter) if isinstance(jitter, tuple) else jitter
```

### Comparing `skretry-0.1.3/skretry.egg-info/PKG-INFO` & `skretry-0.1.4/skretry.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: skretry
-Version: 0.1.3
+Version: 0.1.4
 Summary: An easy to use, but functional decorator for retrying on exceptions.
 Home-page: https://github.com/imsgj/skretry
 Author: imsgj
 License: Apache License 2.0
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Natural Language :: English
```

