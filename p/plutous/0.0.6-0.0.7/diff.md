# Comparing `tmp/plutous-0.0.6.tar.gz` & `tmp/plutous-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "plutous-0.0.6.tar", max compression
+gzip compressed data, was "plutous-0.0.7.tar", max compression
```

## Comparing `plutous-0.0.6.tar` & `plutous-0.0.7.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0     1064 2023-05-10 14:19:17.579815 plutous-0.0.6/LICENSE
--rw-r--r--   0        0        0       31 2023-05-16 15:20:39.229066 plutous-0.0.6/README.md
--rw-r--r--   0        0        0       87 2023-05-22 19:30:14.563811 plutous-0.0.6/plutous/__init__.py
--rw-r--r--   0        0        0        0 2023-05-16 13:50:41.766051 plutous-0.0.6/plutous/app/__init__.py
--rw-r--r--   0        0        0      486 2023-05-22 10:47:17.974453 plutous-0.0.6/plutous/app/main.py
--rw-r--r--   0        0        0        0 2023-05-16 16:16:48.809093 plutous-0.0.6/plutous/app/utils/__init__.py
--rw-r--r--   0        0        0      287 2023-05-16 16:17:49.462926 plutous-0.0.6/plutous/app/utils/session.py
--rw-r--r--   0        0        0        0 2023-05-10 14:48:51.206763 plutous-0.0.6/plutous/cli/__init__.py
--rw-r--r--   0        0        0      531 2023-05-22 13:46:32.044605 plutous-0.0.6/plutous/cli/main.py
--rw-r--r--   0        0        0      756 2023-05-22 11:46:04.769603 plutous-0.0.6/plutous/config.py
--rw-r--r--   0        0        0     2415 2023-05-22 19:03:40.598523 plutous-0.0.6/plutous/database.py
--rw-r--r--   0        0        0       30 2023-05-22 15:46:16.955532 plutous-0.0.6/plutous/enums/__init__.py
--rw-r--r--   0        0        0      335 2023-05-16 18:27:41.692272 plutous-0.0.6/plutous/enums/exchange.py
--rw-r--r--   0        0        0       27 2023-05-16 12:50:11.352964 plutous-0.0.6/plutous/models/__init__.py
--rw-r--r--   0        0        0     1285 2023-05-22 15:47:35.887122 plutous-0.0.6/plutous/models/base.py
--rw-r--r--   0        0        0      813 2023-05-22 19:30:19.196256 plutous-0.0.6/pyproject.toml
--rw-r--r--   0        0        0      767 1970-01-01 00:00:00.000000 plutous-0.0.6/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-05-10 14:19:17.579815 plutous-0.0.7/LICENSE
+-rw-r--r--   0        0        0       31 2023-05-16 15:20:39.229066 plutous-0.0.7/README.md
+-rw-r--r--   0        0        0       87 2023-05-22 19:43:48.418077 plutous-0.0.7/plutous/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-16 13:50:41.766051 plutous-0.0.7/plutous/app/__init__.py
+-rw-r--r--   0        0        0      486 2023-05-22 10:47:17.974453 plutous-0.0.7/plutous/app/main.py
+-rw-r--r--   0        0        0        0 2023-05-16 16:16:48.809093 plutous-0.0.7/plutous/app/utils/__init__.py
+-rw-r--r--   0        0        0      249 2023-05-22 19:43:04.997902 plutous-0.0.7/plutous/app/utils/session.py
+-rw-r--r--   0        0        0        0 2023-05-10 14:48:51.206763 plutous-0.0.7/plutous/cli/__init__.py
+-rw-r--r--   0        0        0      531 2023-05-22 13:46:32.044605 plutous-0.0.7/plutous/cli/main.py
+-rw-r--r--   0        0        0      756 2023-05-22 11:46:04.769603 plutous-0.0.7/plutous/config.py
+-rw-r--r--   0        0        0     2415 2023-05-22 19:03:40.598523 plutous-0.0.7/plutous/database.py
+-rw-r--r--   0        0        0       30 2023-05-22 15:46:16.955532 plutous-0.0.7/plutous/enums/__init__.py
+-rw-r--r--   0        0        0      335 2023-05-16 18:27:41.692272 plutous-0.0.7/plutous/enums/exchange.py
+-rw-r--r--   0        0        0       27 2023-05-16 12:50:11.352964 plutous-0.0.7/plutous/models/__init__.py
+-rw-r--r--   0        0        0     1285 2023-05-22 15:47:35.887122 plutous-0.0.7/plutous/models/base.py
+-rw-r--r--   0        0        0      813 2023-05-22 19:43:53.770592 plutous-0.0.7/pyproject.toml
+-rw-r--r--   0        0        0      767 1970-01-01 00:00:00.000000 plutous-0.0.7/PKG-INFO
```

### Comparing `plutous-0.0.6/LICENSE` & `plutous-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `plutous-0.0.6/plutous/cli/main.py` & `plutous-0.0.7/plutous/cli/main.py`

 * *Files identical despite different names*

### Comparing `plutous-0.0.6/plutous/config.py` & `plutous-0.0.7/plutous/config.py`

 * *Files identical despite different names*

### Comparing `plutous-0.0.6/plutous/database.py` & `plutous-0.0.7/plutous/database.py`

 * *Files identical despite different names*

### Comparing `plutous-0.0.6/plutous/models/base.py` & `plutous-0.0.7/plutous/models/base.py`

 * *Files identical despite different names*

### Comparing `plutous-0.0.6/pyproject.toml` & `plutous-0.0.7/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "plutous"
-version = "0.0.6"
+version = "0.0.7"
 description = "Plutous Library"
 packages = [{include = "plutous"}]
 authors = ["Cheun Hong <cheunhong@plutous.io>"]
 readme = "README.md"
 license="MIT"
 classifiers = [
     "Programming Language :: Python :: 3.10",
```

### Comparing `plutous-0.0.6/PKG-INFO` & `plutous-0.0.7/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plutous
-Version: 0.0.6
+Version: 0.0.7
 Summary: Plutous Library
 License: MIT
 Author: Cheun Hong
 Author-email: cheunhong@plutous.io
 Requires-Python: >=3.10,<3.11
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

