# Comparing `tmp/youte-2.2.1.tar.gz` & `tmp/youte-2.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "youte-2.2.1.tar", last modified: Tue May 16 23:16:00 2023, max compression
+gzip compressed data, was "youte-2.2.2.tar", last modified: Mon May 22 01:09:39 2023, max compression
```

## Comparing `youte-2.2.1.tar` & `youte-2.2.2.tar`

### file list

```diff
@@ -1,55 +1,55 @@
-drwxrwxr-x   0 boyd      (1000) boyd      (1000)        0 2023-05-16 23:16:00.632467 youte-2.2.1/
--rw-rw-r--   0 boyd      (1000) boyd      (1000)     1858 2023-02-16 01:17:30.000000 youte-2.2.1/.gitignore
--rw-rw-r--   0 boyd      (1000) boyd      (1000)      198 2023-03-20 05:21:27.000000 youte-2.2.1/.readthedocs.yaml
--rw-rw-r--   0 boyd      (1000) boyd      (1000)    23744 2023-05-16 23:12:52.000000 youte-2.2.1/CHANGELOG.md
--rw-rw-r--   0 boyd      (1000) boyd      (1000)     1081 2022-06-06 05:38:09.000000 youte-2.2.1/LICENCE
--rw-rw-r--   0 boyd      (1000) boyd      (1000)    16896 2023-05-16 23:16:00.632467 youte-2.2.1/PKG-INFO
--rw-rw-r--   0 boyd      (1000) boyd      (1000)    16257 2023-05-16 23:00:47.000000 youte-2.2.1/README.md
-drwxrwxr-x   0 boyd      (1000) boyd      (1000)        0 2023-05-16 23:16:00.628467 youte-2.2.1/docs/
--rw-rw-r--   0 boyd      (1000) boyd      (1000)    36412 2023-05-16 23:00:47.000000 youte-2.2.1/docs/documentation.md
-drwxrwxr-x   0 boyd      (1000) boyd      (1000)        0 2023-05-16 23:16:00.628467 youte-2.2.1/docs/images/
--rw-rw-r--   0 boyd      (1000) boyd      (1000)    23688 2023-02-16 01:17:30.000000 youte-2.2.1/docs/images/youte-logo-black-transparent.png
--rw-rw-r--   0 boyd      (1000) boyd      (1000)     7979 2023-02-16 01:17:30.000000 youte-2.2.1/docs/images/youte-logo-white-transparent-1x.png
--rw-rw-r--   0 boyd      (1000) boyd      (1000)    24570 2023-02-16 01:17:30.000000 youte-2.2.1/docs/images/youte-logo-white-transparent.png
--rw-rw-r--   0 boyd      (1000) boyd      (1000)    82963 2023-03-14 23:29:14.000000 youte-2.2.1/docs/images/youte_save_progress.png
--rw-rw-r--   0 boyd      (1000) boyd      (1000)   762396 2023-03-17 03:28:46.000000 youte-2.2.1/docs/images/youte_search_results.png
--rw-rw-r--   0 boyd      (1000) boyd      (1000)   183270 2023-03-17 03:37:54.000000 youte-2.2.1/docs/images/youte_search_results_pretty.png
--rw-rw-r--   0 boyd      (1000) boyd      (1000)    67111 2023-05-15 01:12:17.000000 youte-2.2.1/docs/images/youte_thumbnail.png
--rw-rw-r--   0 boyd      (1000) boyd      (1000)     4122 2023-05-16 23:00:47.000000 youte-2.2.1/docs/index.md
--rw-rw-r--   0 boyd      (1000) boyd      (1000)       56 2023-03-17 06:57:11.000000 youte-2.2.1/docs/reference.md
-drwxrwxr-x   0 boyd      (1000) boyd      (1000)        0 2023-05-16 23:16:00.628467 youte-2.2.1/docs/stylesheets/
--rw-rw-r--   0 boyd      (1000) boyd      (1000)      163 2023-02-16 01:17:30.000000 youte-2.2.1/docs/stylesheets/extra.css
--rw-rw-r--   0 boyd      (1000) boyd      (1000)    14669 2023-03-17 05:20:49.000000 youte-2.2.1/docs/tutorial.md
--rw-rw-r--   0 boyd      (1000) boyd      (1000)     1243 2023-05-15 01:12:12.000000 youte-2.2.1/mkdocs.yml
--rw-rw-r--   0 boyd      (1000) boyd      (1000)      430 2023-03-16 07:04:20.000000 youte-2.2.1/noxfile.py
--rw-rw-r--   0 boyd      (1000) boyd      (1000)      231 2023-04-14 05:35:56.000000 youte-2.2.1/pyproject.toml
--rw-rw-r--   0 boyd      (1000) boyd      (1000)      572 2023-03-20 05:22:46.000000 youte-2.2.1/requirements-mkdocs.txt
--rw-rw-r--   0 boyd      (1000) boyd      (1000)     1027 2023-05-16 23:16:00.632467 youte-2.2.1/setup.cfg
--rw-rw-r--   0 boyd      (1000) boyd      (1000)     1363 2023-05-16 23:15:21.000000 youte-2.2.1/setup.py
-drwxrwxr-x   0 boyd      (1000) boyd      (1000)        0 2023-05-16 23:16:00.624467 youte-2.2.1/src/
-drwxrwxr-x   0 boyd      (1000) boyd      (1000)        0 2023-05-16 23:16:00.628467 youte-2.2.1/src/youte/
--rw-rw-r--   0 boyd      (1000) boyd      (1000)        0 2023-04-27 05:21:18.000000 youte-2.2.1/src/youte/__init__.py
--rw-rw-r--   0 boyd      (1000) boyd      (1000)     1253 2023-04-14 05:35:56.000000 youte-2.2.1/src/youte/_logging.py
--rw-rw-r--   0 boyd      (1000) boyd      (1000)      967 2023-05-16 23:00:47.000000 youte-2.2.1/src/youte/_typing.py
--rw-rw-r--   0 boyd      (1000) boyd      (1000)    36959 2023-05-16 23:00:47.000000 youte-2.2.1/src/youte/cli.py
--rw-rw-r--   0 boyd      (1000) boyd      (1000)    28835 2023-05-16 23:00:47.000000 youte-2.2.1/src/youte/collector.py
--rw-rw-r--   0 boyd      (1000) boyd      (1000)     1566 2023-05-16 23:00:47.000000 youte-2.2.1/src/youte/common.py
--rw-rw-r--   0 boyd      (1000) boyd      (1000)     1269 2023-03-16 07:04:20.000000 youte-2.2.1/src/youte/config.py
--rw-rw-r--   0 boyd      (1000) boyd      (1000)    12937 2023-04-14 05:35:56.000000 youte-2.2.1/src/youte/database.py
--rw-rw-r--   0 boyd      (1000) boyd      (1000)      359 2023-05-16 23:00:47.000000 youte-2.2.1/src/youte/exceptions.py
--rw-rw-r--   0 boyd      (1000) boyd      (1000)    14908 2023-05-16 23:00:47.000000 youte-2.2.1/src/youte/parser.py
--rw-rw-r--   0 boyd      (1000) boyd      (1000)     3145 2023-05-16 23:04:31.000000 youte-2.2.1/src/youte/resources.py
--rw-rw-r--   0 boyd      (1000) boyd      (1000)     3747 2023-03-16 07:04:20.000000 youte-2.2.1/src/youte/utilities.py
--rw-rw-r--   0 boyd      (1000) boyd      (1000)      189 2023-05-16 23:10:25.000000 youte-2.2.1/src/youte/version.py
-drwxrwxr-x   0 boyd      (1000) boyd      (1000)        0 2023-05-16 23:16:00.628467 youte-2.2.1/src/youte.egg-info/
--rw-rw-r--   0 boyd      (1000) boyd      (1000)    16896 2023-05-16 23:16:00.000000 youte-2.2.1/src/youte.egg-info/PKG-INFO
--rw-rw-r--   0 boyd      (1000) boyd      (1000)     1087 2023-05-16 23:16:00.000000 youte-2.2.1/src/youte.egg-info/SOURCES.txt
--rw-rw-r--   0 boyd      (1000) boyd      (1000)        1 2023-05-16 23:16:00.000000 youte-2.2.1/src/youte.egg-info/dependency_links.txt
--rw-rw-r--   0 boyd      (1000) boyd      (1000)       42 2023-05-16 23:16:00.000000 youte-2.2.1/src/youte.egg-info/entry_points.txt
--rw-rw-r--   0 boyd      (1000) boyd      (1000)      147 2023-05-16 23:16:00.000000 youte-2.2.1/src/youte.egg-info/requires.txt
--rw-rw-r--   0 boyd      (1000) boyd      (1000)        6 2023-05-16 23:16:00.000000 youte-2.2.1/src/youte.egg-info/top_level.txt
-drwxrwxr-x   0 boyd      (1000) boyd      (1000)        0 2023-05-16 23:16:00.632467 youte-2.2.1/tests/
--rw-rw-r--   0 boyd      (1000) boyd      (1000)     2820 2023-04-14 05:35:56.000000 youte-2.2.1/tests/test_archive.py
--rw-rw-r--   0 boyd      (1000) boyd      (1000)     8449 2023-05-16 23:00:47.000000 youte-2.2.1/tests/test_cli.py
--rw-rw-r--   0 boyd      (1000) boyd      (1000)     3166 2023-05-16 23:00:47.000000 youte-2.2.1/tests/test_collector.py
--rw-rw-r--   0 boyd      (1000) boyd      (1000)     2555 2023-04-14 05:35:56.000000 youte-2.2.1/tests/test_parser.py
+drwxrwxr-x   0 boyd      (1000) boyd      (1000)        0 2023-05-22 01:09:39.908236 youte-2.2.2/
+-rw-rw-r--   0 boyd      (1000) boyd      (1000)     1858 2023-02-16 01:17:30.000000 youte-2.2.2/.gitignore
+-rw-rw-r--   0 boyd      (1000) boyd      (1000)      198 2023-03-20 05:21:27.000000 youte-2.2.2/.readthedocs.yaml
+-rw-rw-r--   0 boyd      (1000) boyd      (1000)     5832 2023-05-22 01:08:56.000000 youte-2.2.2/CHANGELOG.md
+-rw-rw-r--   0 boyd      (1000) boyd      (1000)     1081 2022-06-06 05:38:09.000000 youte-2.2.2/LICENCE
+-rw-rw-r--   0 boyd      (1000) boyd      (1000)    16896 2023-05-22 01:09:39.908236 youte-2.2.2/PKG-INFO
+-rw-rw-r--   0 boyd      (1000) boyd      (1000)    16257 2023-05-16 23:00:47.000000 youte-2.2.2/README.md
+drwxrwxr-x   0 boyd      (1000) boyd      (1000)        0 2023-05-22 01:09:39.900236 youte-2.2.2/docs/
+-rw-rw-r--   0 boyd      (1000) boyd      (1000)    36412 2023-05-16 23:00:47.000000 youte-2.2.2/docs/documentation.md
+drwxrwxr-x   0 boyd      (1000) boyd      (1000)        0 2023-05-22 01:09:39.908236 youte-2.2.2/docs/images/
+-rw-rw-r--   0 boyd      (1000) boyd      (1000)    23688 2023-02-16 01:17:30.000000 youte-2.2.2/docs/images/youte-logo-black-transparent.png
+-rw-rw-r--   0 boyd      (1000) boyd      (1000)     7979 2023-02-16 01:17:30.000000 youte-2.2.2/docs/images/youte-logo-white-transparent-1x.png
+-rw-rw-r--   0 boyd      (1000) boyd      (1000)    24570 2023-02-16 01:17:30.000000 youte-2.2.2/docs/images/youte-logo-white-transparent.png
+-rw-rw-r--   0 boyd      (1000) boyd      (1000)    82963 2023-03-14 23:29:14.000000 youte-2.2.2/docs/images/youte_save_progress.png
+-rw-rw-r--   0 boyd      (1000) boyd      (1000)   762396 2023-03-17 03:28:46.000000 youte-2.2.2/docs/images/youte_search_results.png
+-rw-rw-r--   0 boyd      (1000) boyd      (1000)   183270 2023-03-17 03:37:54.000000 youte-2.2.2/docs/images/youte_search_results_pretty.png
+-rw-rw-r--   0 boyd      (1000) boyd      (1000)    67111 2023-05-15 01:12:17.000000 youte-2.2.2/docs/images/youte_thumbnail.png
+-rw-rw-r--   0 boyd      (1000) boyd      (1000)     4122 2023-05-16 23:00:47.000000 youte-2.2.2/docs/index.md
+-rw-rw-r--   0 boyd      (1000) boyd      (1000)       56 2023-03-17 06:57:11.000000 youte-2.2.2/docs/reference.md
+drwxrwxr-x   0 boyd      (1000) boyd      (1000)        0 2023-05-22 01:09:39.908236 youte-2.2.2/docs/stylesheets/
+-rw-rw-r--   0 boyd      (1000) boyd      (1000)      163 2023-02-16 01:17:30.000000 youte-2.2.2/docs/stylesheets/extra.css
+-rw-rw-r--   0 boyd      (1000) boyd      (1000)    14669 2023-03-17 05:20:49.000000 youte-2.2.2/docs/tutorial.md
+-rw-rw-r--   0 boyd      (1000) boyd      (1000)     1243 2023-05-15 01:12:12.000000 youte-2.2.2/mkdocs.yml
+-rw-rw-r--   0 boyd      (1000) boyd      (1000)      430 2023-03-16 07:04:20.000000 youte-2.2.2/noxfile.py
+-rw-rw-r--   0 boyd      (1000) boyd      (1000)      231 2023-04-14 05:35:56.000000 youte-2.2.2/pyproject.toml
+-rw-rw-r--   0 boyd      (1000) boyd      (1000)      572 2023-03-20 05:22:46.000000 youte-2.2.2/requirements-mkdocs.txt
+-rw-rw-r--   0 boyd      (1000) boyd      (1000)     1027 2023-05-22 01:09:39.912236 youte-2.2.2/setup.cfg
+-rw-rw-r--   0 boyd      (1000) boyd      (1000)     1363 2023-05-22 01:08:56.000000 youte-2.2.2/setup.py
+drwxrwxr-x   0 boyd      (1000) boyd      (1000)        0 2023-05-22 01:09:39.900236 youte-2.2.2/src/
+drwxrwxr-x   0 boyd      (1000) boyd      (1000)        0 2023-05-22 01:09:39.908236 youte-2.2.2/src/youte/
+-rw-rw-r--   0 boyd      (1000) boyd      (1000)        0 2023-04-27 05:21:18.000000 youte-2.2.2/src/youte/__init__.py
+-rw-rw-r--   0 boyd      (1000) boyd      (1000)     1253 2023-04-14 05:35:56.000000 youte-2.2.2/src/youte/_logging.py
+-rw-rw-r--   0 boyd      (1000) boyd      (1000)      967 2023-05-16 23:00:47.000000 youte-2.2.2/src/youte/_typing.py
+-rw-rw-r--   0 boyd      (1000) boyd      (1000)    36959 2023-05-16 23:00:47.000000 youte-2.2.2/src/youte/cli.py
+-rw-rw-r--   0 boyd      (1000) boyd      (1000)    28835 2023-05-16 23:00:47.000000 youte-2.2.2/src/youte/collector.py
+-rw-rw-r--   0 boyd      (1000) boyd      (1000)     1428 2023-05-22 01:08:56.000000 youte-2.2.2/src/youte/common.py
+-rw-rw-r--   0 boyd      (1000) boyd      (1000)     1269 2023-03-16 07:04:20.000000 youte-2.2.2/src/youte/config.py
+-rw-rw-r--   0 boyd      (1000) boyd      (1000)    12937 2023-04-14 05:35:56.000000 youte-2.2.2/src/youte/database.py
+-rw-rw-r--   0 boyd      (1000) boyd      (1000)      359 2023-05-16 23:00:47.000000 youte-2.2.2/src/youte/exceptions.py
+-rw-rw-r--   0 boyd      (1000) boyd      (1000)    14908 2023-05-16 23:00:47.000000 youte-2.2.2/src/youte/parser.py
+-rw-rw-r--   0 boyd      (1000) boyd      (1000)     3145 2023-05-16 23:04:31.000000 youte-2.2.2/src/youte/resources.py
+-rw-rw-r--   0 boyd      (1000) boyd      (1000)     3747 2023-03-16 07:04:20.000000 youte-2.2.2/src/youte/utilities.py
+-rw-rw-r--   0 boyd      (1000) boyd      (1000)      189 2023-05-22 01:08:56.000000 youte-2.2.2/src/youte/version.py
+drwxrwxr-x   0 boyd      (1000) boyd      (1000)        0 2023-05-22 01:09:39.908236 youte-2.2.2/src/youte.egg-info/
+-rw-rw-r--   0 boyd      (1000) boyd      (1000)    16896 2023-05-22 01:09:39.000000 youte-2.2.2/src/youte.egg-info/PKG-INFO
+-rw-rw-r--   0 boyd      (1000) boyd      (1000)     1087 2023-05-22 01:09:39.000000 youte-2.2.2/src/youte.egg-info/SOURCES.txt
+-rw-rw-r--   0 boyd      (1000) boyd      (1000)        1 2023-05-22 01:09:39.000000 youte-2.2.2/src/youte.egg-info/dependency_links.txt
+-rw-rw-r--   0 boyd      (1000) boyd      (1000)       42 2023-05-22 01:09:39.000000 youte-2.2.2/src/youte.egg-info/entry_points.txt
+-rw-rw-r--   0 boyd      (1000) boyd      (1000)      147 2023-05-22 01:09:39.000000 youte-2.2.2/src/youte.egg-info/requires.txt
+-rw-rw-r--   0 boyd      (1000) boyd      (1000)        6 2023-05-22 01:09:39.000000 youte-2.2.2/src/youte.egg-info/top_level.txt
+drwxrwxr-x   0 boyd      (1000) boyd      (1000)        0 2023-05-22 01:09:39.908236 youte-2.2.2/tests/
+-rw-rw-r--   0 boyd      (1000) boyd      (1000)     2817 2023-05-22 01:08:56.000000 youte-2.2.2/tests/test_archive.py
+-rw-rw-r--   0 boyd      (1000) boyd      (1000)     8449 2023-05-16 23:00:47.000000 youte-2.2.2/tests/test_cli.py
+-rw-rw-r--   0 boyd      (1000) boyd      (1000)     3166 2023-05-16 23:00:47.000000 youte-2.2.2/tests/test_collector.py
+-rw-rw-r--   0 boyd      (1000) boyd      (1000)     2555 2023-04-14 05:35:56.000000 youte-2.2.2/tests/test_parser.py
```

### Comparing `youte-2.2.1/.gitignore` & `youte-2.2.2/.gitignore`

 * *Files identical despite different names*

### Comparing `youte-2.2.1/LICENCE` & `youte-2.2.2/LICENCE`

 * *Files identical despite different names*

### Comparing `youte-2.2.1/PKG-INFO` & `youte-2.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: youte
-Version: 2.2.1
+Version: 2.2.2
 Summary: Command-line tool to collect video metadata and comments from Youtube API
 Home-page: https://github.com/QUT-Digital-Observatory/youte
 Author: Digital Observatory
 Author-email: digitalobservatory@qut.edu.au
 Project-URL: Bug Tracker, https://github.com/QUT-Digital-Observatory/youte/issues
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `youte-2.2.1/README.md` & `youte-2.2.2/README.md`

 * *Files identical despite different names*

### Comparing `youte-2.2.1/docs/documentation.md` & `youte-2.2.2/docs/documentation.md`

 * *Files identical despite different names*

### Comparing `youte-2.2.1/docs/images/youte-logo-black-transparent.png` & `youte-2.2.2/docs/images/youte-logo-black-transparent.png`

 * *Files identical despite different names*

### Comparing `youte-2.2.1/docs/images/youte-logo-white-transparent-1x.png` & `youte-2.2.2/docs/images/youte-logo-white-transparent-1x.png`

 * *Files identical despite different names*

### Comparing `youte-2.2.1/docs/images/youte-logo-white-transparent.png` & `youte-2.2.2/docs/images/youte-logo-white-transparent.png`

 * *Files identical despite different names*

### Comparing `youte-2.2.1/docs/images/youte_save_progress.png` & `youte-2.2.2/docs/images/youte_save_progress.png`

 * *Files identical despite different names*

### Comparing `youte-2.2.1/docs/images/youte_search_results.png` & `youte-2.2.2/docs/images/youte_search_results.png`

 * *Files identical despite different names*

### Comparing `youte-2.2.1/docs/images/youte_search_results_pretty.png` & `youte-2.2.2/docs/images/youte_search_results_pretty.png`

 * *Files identical despite different names*

### Comparing `youte-2.2.1/docs/images/youte_thumbnail.png` & `youte-2.2.2/docs/images/youte_thumbnail.png`

 * *Files identical despite different names*

### Comparing `youte-2.2.1/docs/index.md` & `youte-2.2.2/docs/index.md`

 * *Files identical despite different names*

### Comparing `youte-2.2.1/docs/tutorial.md` & `youte-2.2.2/docs/tutorial.md`

 * *Files identical despite different names*

### Comparing `youte-2.2.1/mkdocs.yml` & `youte-2.2.2/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `youte-2.2.1/requirements-mkdocs.txt` & `youte-2.2.2/requirements-mkdocs.txt`

 * *Files identical despite different names*

### Comparing `youte-2.2.1/setup.cfg` & `youte-2.2.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `youte-2.2.1/setup.py` & `youte-2.2.2/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import pathlib
 
 from setuptools import find_packages, setup
 
 here = pathlib.Path(__file__).parent.resolve()
 
-__version__ = "2.2.1"
+__version__ = "2.2.2"
 
 # Get the long description from the README file
 long_description = (here / "README.md").read_text(encoding="utf-8")
 
 if __name__ == "__main__":
     setup(
         name="youte",
```

### Comparing `youte-2.2.1/src/youte/_logging.py` & `youte-2.2.2/src/youte/_logging.py`

 * *Files identical despite different names*

### Comparing `youte-2.2.1/src/youte/_typing.py` & `youte-2.2.2/src/youte/_typing.py`

 * *Files identical despite different names*

### Comparing `youte-2.2.1/src/youte/cli.py` & `youte-2.2.2/src/youte/cli.py`

 * *Files identical despite different names*

### Comparing `youte-2.2.1/src/youte/collector.py` & `youte-2.2.2/src/youte/collector.py`

 * *Files identical despite different names*

### Comparing `youte-2.2.1/src/youte/common.py` & `youte-2.2.2/src/youte/common.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from __future__ import annotations
 
 import csv
 import json
 from dataclasses import asdict, dataclass
 from pathlib import Path
-from typing import Optional
+from typing import Optional, Any
 
 
 @dataclass
 class Resources:
     items: list
 
     def to_json(self, filepath: Path | str, pretty: bool = False) -> None:
@@ -35,17 +35,12 @@
 def _flatten_json(obj: dict[str, Any]) -> dict[str, Any]:
     out = {}
 
     def flatten(x: str | dict | list, name: str = ""):
         if type(x) is dict:
             for a in x:
                 flatten(x[a], name + a + "_")
-        elif type(x) is list:
-            i = 0
-            for a in x:
-                flatten(a, name + str(i) + "_")
-                i += 1
         else:
             out[name[:-1]] = x
 
     flatten(obj)
     return out
```

### Comparing `youte-2.2.1/src/youte/config.py` & `youte-2.2.2/src/youte/config.py`

 * *Files identical despite different names*

### Comparing `youte-2.2.1/src/youte/database.py` & `youte-2.2.2/src/youte/database.py`

 * *Files identical despite different names*

### Comparing `youte-2.2.1/src/youte/parser.py` & `youte-2.2.2/src/youte/parser.py`

 * *Files identical despite different names*

### Comparing `youte-2.2.1/src/youte/resources.py` & `youte-2.2.2/src/youte/resources.py`

 * *Files identical despite different names*

### Comparing `youte-2.2.1/src/youte/utilities.py` & `youte-2.2.2/src/youte/utilities.py`

 * *Files identical despite different names*

### Comparing `youte-2.2.1/src/youte.egg-info/PKG-INFO` & `youte-2.2.2/src/youte.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: youte
-Version: 2.2.1
+Version: 2.2.2
 Summary: Command-line tool to collect video metadata and comments from Youtube API
 Home-page: https://github.com/QUT-Digital-Observatory/youte
 Author: Digital Observatory
 Author-email: digitalobservatory@qut.edu.au
 Project-URL: Bug Tracker, https://github.com/QUT-Digital-Observatory/youte/issues
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `youte-2.2.1/src/youte.egg-info/SOURCES.txt` & `youte-2.2.2/src/youte.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `youte-2.2.1/tests/test_archive.py` & `youte-2.2.2/tests/test_archive.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,42 +20,42 @@
 def test_full_archive():
     search_query = "stoicism"
     yob = Youte(api_key=API_KEY)
     engine = database.set_up_database("test.db")
 
     s_results = [
         result
-        for result in yob.search(search_query, max_result=50, max_pages_retrieved=2)
+        for result in yob.search(search_query, max_result=10, max_pages_retrieved=2)
     ]
     assert len(s_results) == 2
 
     searches = parser.parse_searches(s_results)
     assert isinstance(searches, Searches)
-    assert len(searches.items) > 50
+    assert len(searches.items) > 10
 
     video_ids = [s.id for s in searches.items]
     channel_ids = [c.channel_id for c in searches.items]
 
     v_results = [r for r in yob.get_video_metadata(video_ids)]
     assert len(v_results) > 0
 
     videos = parser.parse_videos(v_results)
     assert isinstance(videos, Videos)
-    assert len(videos.items) > 50
+    assert len(videos.items) > 10
 
     c_results = [r for r in yob.get_channel_metadata(channel_ids)]
     assert len(c_results) > 0
 
     channels = parser.parse_channels(c_results)
     assert isinstance(channels, Channels)
-    assert len(channels.items) > 10
+    assert len(channels.items) > 5
 
     ids_for_comments = [v.id for v in videos.items if v.comment_count < 200]
-    if len(ids_for_comments) > 10:
-        ids_for_comments = ids_for_comments[:10]
+    if len(ids_for_comments) > 5:
+        ids_for_comments = ids_for_comments[:5]
     cmt_results = [r for r in yob.get_comment_threads(video_ids=ids_for_comments)]
     assert len(cmt_results) > 0
 
     comments = parser.parse_comments(cmt_results)
     assert isinstance(comments, Comments)
     assert len(comments.items) > 5
 
@@ -70,17 +70,17 @@
     database.populate_searches(engine, [searches])
     database.populate_videos(engine, [videos])
     database.populate_channels(engine, [channels])
     database.populate_comments(engine, [comments, replies])
 
     with engine.connect() as conn:
         search_count = conn.execute(func.count(database.Search.id))
-        assert search_count.all()[0][0] > 20
+        assert search_count.all()[0][0] > 10
 
         video_count = conn.execute(func.count(database.Video.id))
-        assert video_count.all()[0][0] > 20
+        assert video_count.all()[0][0] > 10
 
         channel_count = conn.execute(func.count(database.Channel.id))
-        assert channel_count.all()[0][0] > 20
+        assert channel_count.all()[0][0] > 10
 
         cmt_count = conn.execute(func.count(database.Comment.id))
-        assert cmt_count.all()[0][0] > 20
+        assert cmt_count.all()[0][0] > 10
```

### Comparing `youte-2.2.1/tests/test_cli.py` & `youte-2.2.2/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `youte-2.2.1/tests/test_collector.py` & `youte-2.2.2/tests/test_collector.py`

 * *Files identical despite different names*

### Comparing `youte-2.2.1/tests/test_parser.py` & `youte-2.2.2/tests/test_parser.py`

 * *Files identical despite different names*

