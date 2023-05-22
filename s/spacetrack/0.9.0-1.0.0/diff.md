# Comparing `tmp/spacetrack-0.9.0.tar.gz` & `tmp/spacetrack-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/spacetrack-0.9.0.tar", last modified: Thu Jan 28 20:48:37 2016, max compression
+gzip compressed data, was "spacetrack-1.0.0.tar", last modified: Mon May 22 16:46:43 2023, max compression
```

## Comparing `spacetrack-0.9.0.tar` & `spacetrack-1.0.0.tar`

### file list

```diff
@@ -1,16 +1,41 @@
-drwxr-xr-x   0 frazer     (501) staff       (20)        0 2016-01-28 20:48:37.000000 spacetrack-0.9.0/
--rw-r--r--   0 frazer     (501) staff       (20)     2353 2016-01-28 20:48:37.000000 spacetrack-0.9.0/PKG-INFO
--rw-r--r--   0 frazer     (501) staff       (20)     1567 2015-12-29 03:01:05.000000 spacetrack-0.9.0/README.rst
--rw-r--r--   0 frazer     (501) staff       (20)       88 2016-01-28 20:48:37.000000 spacetrack-0.9.0/setup.cfg
--rw-r--r--   0 frazer     (501) staff       (20)     3033 2016-01-28 20:38:38.000000 spacetrack-0.9.0/setup.py
-drwxr-xr-x   0 frazer     (501) staff       (20)        0 2016-01-28 20:48:37.000000 spacetrack-0.9.0/spacetrack/
--rw-r--r--   0 frazer     (501) staff       (20)      760 2016-01-28 20:42:42.000000 spacetrack-0.9.0/spacetrack/__init__.py
--rw-r--r--   0 frazer     (501) staff       (20)    11027 2016-01-06 22:29:41.000000 spacetrack-0.9.0/spacetrack/aio.py
--rw-r--r--   0 frazer     (501) staff       (20)    14881 2016-01-28 19:11:21.000000 spacetrack-0.9.0/spacetrack/base.py
--rw-r--r--   0 frazer     (501) staff       (20)     1586 2016-01-27 21:45:42.000000 spacetrack-0.9.0/spacetrack/operators.py
-drwxr-xr-x   0 frazer     (501) staff       (20)        0 2016-01-28 20:48:37.000000 spacetrack-0.9.0/spacetrack.egg-info/
--rw-r--r--   0 frazer     (501) staff       (20)        1 2016-01-28 20:48:37.000000 spacetrack-0.9.0/spacetrack.egg-info/dependency_links.txt
--rw-r--r--   0 frazer     (501) staff       (20)     2353 2016-01-28 20:48:37.000000 spacetrack-0.9.0/spacetrack.egg-info/PKG-INFO
--rw-r--r--   0 frazer     (501) staff       (20)      657 2016-01-28 20:48:37.000000 spacetrack-0.9.0/spacetrack.egg-info/requires.txt
--rw-r--r--   0 frazer     (501) staff       (20)      282 2016-01-28 20:48:37.000000 spacetrack-0.9.0/spacetrack.egg-info/SOURCES.txt
--rw-r--r--   0 frazer     (501) staff       (20)       11 2016-01-28 20:48:37.000000 spacetrack-0.9.0/spacetrack.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 16:46:43.165195 spacetrack-1.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      985 2023-05-22 16:46:23.000000 spacetrack-1.0.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      145 2023-05-22 16:46:23.000000 spacetrack-1.0.0/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      211 2023-05-22 16:46:23.000000 spacetrack-1.0.0/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-05-22 16:46:23.000000 spacetrack-1.0.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      216 2023-05-22 16:46:23.000000 spacetrack-1.0.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4022 2023-05-22 16:46:43.165195 spacetrack-1.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3158 2023-05-22 16:46:23.000000 spacetrack-1.0.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-05-22 16:46:23.000000 spacetrack-1.0.0/dev-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 16:46:43.157195 spacetrack-1.0.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     8652 2023-05-22 16:46:23.000000 spacetrack-1.0.0/docs/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2286 2023-05-22 16:46:23.000000 spacetrack-1.0.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      463 2023-05-22 16:46:23.000000 spacetrack-1.0.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      458 2023-05-22 16:46:23.000000 spacetrack-1.0.0/docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-05-22 16:46:23.000000 spacetrack-1.0.0/docs/module.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 16:46:43.161195 spacetrack-1.0.0/docs/modules/
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-05-22 16:46:23.000000 spacetrack-1.0.0/docs/modules/aio.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-05-22 16:46:23.000000 spacetrack-1.0.0/docs/modules/base.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      299 2023-05-22 16:46:23.000000 spacetrack-1.0.0/docs/modules/operators.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     6898 2023-05-22 16:46:23.000000 spacetrack-1.0.0/docs/usage.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1542 2023-05-22 16:46:23.000000 spacetrack-1.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-05-22 16:46:43.165195 spacetrack-1.0.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 16:46:43.153195 spacetrack-1.0.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 16:46:43.161195 spacetrack-1.0.0/src/spacetrack/
+-rw-r--r--   0 runner    (1001) docker     (123)      489 2023-05-22 16:46:23.000000 spacetrack-1.0.0/src/spacetrack/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7992 2023-05-22 16:46:23.000000 spacetrack-1.0.0/src/spacetrack/aio.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28440 2023-05-22 16:46:23.000000 spacetrack-1.0.0/src/spacetrack/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1469 2023-05-22 16:46:23.000000 spacetrack-1.0.0/src/spacetrack/operators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 16:46:43.161195 spacetrack-1.0.0/src/spacetrack.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4022 2023-05-22 16:46:43.000000 spacetrack-1.0.0/src/spacetrack.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      705 2023-05-22 16:46:43.000000 spacetrack-1.0.0/src/spacetrack.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 16:46:43.000000 spacetrack-1.0.0/src/spacetrack.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-05-22 16:46:43.000000 spacetrack-1.0.0/src/spacetrack.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-22 16:46:43.000000 spacetrack-1.0.0/src/spacetrack.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 16:46:43.165195 spacetrack-1.0.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 16:46:23.000000 spacetrack-1.0.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2551 2023-05-22 16:46:23.000000 spacetrack-1.0.0/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4558 2023-05-22 16:46:23.000000 spacetrack-1.0.0/tests/test_aio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-05-22 16:46:23.000000 spacetrack-1.0.0/tests/test_operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16870 2023-05-22 16:46:23.000000 spacetrack-1.0.0/tests/test_spacetrack.py
+-rw-r--r--   0 runner    (1001) docker     (123)      944 2023-05-22 16:46:23.000000 spacetrack-1.0.0/tox.ini
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `spacetrack-0.9.0/spacetrack/operators.py` & `spacetrack-1.0.0/src/spacetrack/operators.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,60 +1,54 @@
-# coding: utf-8
-from __future__ import absolute_import, division, print_function
-
 import datetime
-from collections import Sequence
-
-import six
+from collections.abc import Sequence
 
 
 def greater_than(value):
     """``'>value'``."""
-    return '>' + _stringify_predicate_value(value)
+    return ">" + _stringify_predicate_value(value)
 
 
 def less_than(value):
     """``'<value'``."""
-    return '<' + _stringify_predicate_value(value)
+    return "<" + _stringify_predicate_value(value)
 
 
 def not_equal(value):
     """``'<>value'``."""
-    return '<>' + _stringify_predicate_value(value)
+    return "<>" + _stringify_predicate_value(value)
 
 
 def inclusive_range(left, right):
     """``'left--right'``."""
-    return (_stringify_predicate_value(left) + '--' +
-            _stringify_predicate_value(right))
+    return _stringify_predicate_value(left) + "--" + _stringify_predicate_value(right)
 
 
 def like(value):
     """``'~~value'``."""
-    return '~~' + _stringify_predicate_value(value)
+    return "~~" + _stringify_predicate_value(value)
 
 
 def startswith(value):
     """``'^value'``."""
-    return '^' + _stringify_predicate_value(value)
+    return "^" + _stringify_predicate_value(value)
 
 
 def _stringify_predicate_value(value):
     """Convert Python objects to Space-Track compatible strings
 
     - Booleans (``True`` -> ``'true'``)
     - Sequences (``[25544, 34602]`` -> ``'25544,34602'``)
     - dates/datetimes (``date(2015, 12, 23)`` -> ``'2015-12-23'``)
     - ``None`` -> ``'null-val'``
     """
     if isinstance(value, bool):
         return str(value).lower()
-    elif isinstance(value, Sequence) and not isinstance(value, six.string_types):
-        return ','.join(_stringify_predicate_value(x) for x in value)
+    elif isinstance(value, Sequence) and not isinstance(value, str):
+        return ",".join(_stringify_predicate_value(x) for x in value)
     elif isinstance(value, datetime.datetime):
-        return value.isoformat(sep=' ')
+        return value.isoformat(sep=" ")
     elif isinstance(value, datetime.date):
         return value.isoformat()
     elif value is None:
-        return 'null-val'
+        return "null-val"
     else:
         return str(value)
```

