# Comparing `tmp/things-cli-0.1.4.tar.gz` & `tmp/things-cli-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "things-cli-0.1.4.tar", last modified: Mon Mar 21 06:34:53 2022, max compression
+gzip compressed data, was "things-cli-0.2.0.tar", last modified: Mon May 22 20:06:31 2023, max compression
```

## Comparing `things-cli-0.1.4.tar` & `things-cli-0.2.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 awi        (501) staff       (20)        0 2022-03-21 06:34:53.638519 things-cli-0.1.4/
--rw-r--r--   0 awi        (501) staff       (20)     5174 2022-03-21 06:34:53.638721 things-cli-0.1.4/PKG-INFO
--rw-r--r--   0 awi        (501) staff       (20)     4608 2021-11-16 09:31:03.000000 things-cli-0.1.4/README.md
--rw-r--r--   0 awi        (501) staff       (20)      358 2022-03-21 06:34:53.639644 things-cli-0.1.4/setup.cfg
--rw-r--r--   0 awi        (501) staff       (20)     1612 2021-04-21 06:51:42.000000 things-cli-0.1.4/setup.py
-drwxr-xr-x   0 awi        (501) staff       (20)        0 2022-03-21 06:34:53.633491 things-cli-0.1.4/tests/
--rw-r--r--   0 awi        (501) staff       (20)        0 2021-03-28 20:57:14.000000 things-cli-0.1.4/tests/__init__.py
--rw-r--r--   0 awi        (501) staff       (20)     3682 2022-01-23 12:41:29.000000 things-cli-0.1.4/tests/test_things_cli.py
-drwxr-xr-x   0 awi        (501) staff       (20)        0 2022-03-21 06:34:53.634556 things-cli-0.1.4/things_cli/
--rw-r--r--   0 awi        (501) staff       (20)      320 2022-03-21 06:31:12.000000 things-cli-0.1.4/things_cli/__init__.py
--rwxr-xr-x   0 awi        (501) staff       (20)    17247 2022-03-21 06:28:58.000000 things-cli-0.1.4/things_cli/cli.py
-drwxr-xr-x   0 awi        (501) staff       (20)        0 2022-03-21 06:34:53.637974 things-cli-0.1.4/things_cli.egg-info/
--rw-r--r--   0 awi        (501) staff       (20)     5174 2022-03-21 06:34:53.000000 things-cli-0.1.4/things_cli.egg-info/PKG-INFO
--rw-r--r--   0 awi        (501) staff       (20)      318 2022-03-21 06:34:53.000000 things-cli-0.1.4/things_cli.egg-info/SOURCES.txt
--rw-r--r--   0 awi        (501) staff       (20)        1 2022-03-21 06:34:53.000000 things-cli-0.1.4/things_cli.egg-info/dependency_links.txt
--rw-r--r--   0 awi        (501) staff       (20)       52 2022-03-21 06:34:53.000000 things-cli-0.1.4/things_cli.egg-info/entry_points.txt
--rw-r--r--   0 awi        (501) staff       (20)       22 2022-03-21 06:34:53.000000 things-cli-0.1.4/things_cli.egg-info/requires.txt
--rw-r--r--   0 awi        (501) staff       (20)       17 2022-03-21 06:34:53.000000 things-cli-0.1.4/things_cli.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 20:06:31.228853 things-cli-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     5174 2023-05-22 20:06:31.228853 things-cli-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4608 2023-05-22 20:06:11.000000 things-cli-0.2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      358 2023-05-22 20:06:31.228853 things-cli-0.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1612 2023-05-22 20:06:11.000000 things-cli-0.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 20:06:31.228853 things-cli-0.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 20:06:11.000000 things-cli-0.2.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3682 2023-05-22 20:06:11.000000 things-cli-0.2.0/tests/test_things_cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 20:06:31.228853 things-cli-0.2.0/things_cli/
+-rw-r--r--   0 runner    (1001) docker     (123)      320 2023-05-22 20:06:11.000000 things-cli-0.2.0/things_cli/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    17258 2023-05-22 20:06:11.000000 things-cli-0.2.0/things_cli/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 20:06:31.228853 things-cli-0.2.0/things_cli.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5174 2023-05-22 20:06:31.000000 things-cli-0.2.0/things_cli.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      318 2023-05-22 20:06:31.000000 things-cli-0.2.0/things_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 20:06:31.000000 things-cli-0.2.0/things_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-22 20:06:31.000000 things-cli-0.2.0/things_cli.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-22 20:06:31.000000 things-cli-0.2.0/things_cli.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-22 20:06:31.000000 things-cli-0.2.0/things_cli.egg-info/top_level.txt
```

### Comparing `things-cli-0.1.4/PKG-INFO` & `things-cli-0.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: things-cli
-Version: 0.1.4
+Version: 0.2.0
 Summary: A simple Python 3 CLI to read your Things app data.
 Home-page: https://github.com/thingsapi/things-cli
 Author: Alexander Willner
 Author-email: alex@willner.ws
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
```

### Comparing `things-cli-0.1.4/README.md` & `things-cli-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `things-cli-0.1.4/setup.py` & `things-cli-0.2.0/setup.py`

 * *Files identical despite different names*

### Comparing `things-cli-0.1.4/tests/test_things_cli.py` & `things-cli-0.2.0/tests/test_things_cli.py`

 * *Files identical despite different names*

### Comparing `things-cli-0.1.4/things_cli/cli.py` & `things-cli-0.2.0/things_cli/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -387,21 +387,21 @@
 
         argcomplete.autocomplete(parser)
 
         return parser
 
     def defaults(self):
         """Set default options for the new API."""
-        return dict(
-            project=self.filter_project,
-            area=self.filter_area,
-            tag=self.filter_tag,
-            include_items=self.recursive,
-            filepath=self.database,
-        )
+        return {
+            "project": self.filter_project,
+            "area": self.filter_area,
+            "tag": self.filter_tag,
+            "include_items": self.recursive,
+            "filepath": self.database,
+        }
 
     def main(self, args=None):
         """Start the main app."""
 
         if args is None:
             self.main(ThingsCLI.get_parser().parse_args())
         else:
```

### Comparing `things-cli-0.1.4/things_cli.egg-info/PKG-INFO` & `things-cli-0.2.0/things_cli.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: things-cli
-Version: 0.1.4
+Version: 0.2.0
 Summary: A simple Python 3 CLI to read your Things app data.
 Home-page: https://github.com/thingsapi/things-cli
 Author: Alexander Willner
 Author-email: alex@willner.ws
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
```

