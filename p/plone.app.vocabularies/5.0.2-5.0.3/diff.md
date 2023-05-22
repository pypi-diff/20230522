# Comparing `tmp/plone.app.vocabularies-5.0.2.tar.gz` & `tmp/plone.app.vocabularies-5.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "plone.app.vocabularies-5.0.2.tar", last modified: Thu Apr  6 10:33:04 2023, max compression
+gzip compressed data, was "plone.app.vocabularies-5.0.3.tar", last modified: Mon May 22 18:02:13 2023, max compression
```

## Comparing `plone.app.vocabularies-5.0.2.tar` & `plone.app.vocabularies-5.0.3.tar`

### file list

```diff
@@ -1,55 +1,55 @@
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-06 10:33:04.251399 plone.app.vocabularies-5.0.2/
--rw-r--r--   0 maurits    (501) staff       (20)    15924 2023-04-06 10:33:03.000000 plone.app.vocabularies-5.0.2/CHANGES.rst
--rw-r--r--   0 maurits    (501) staff       (20)       70 2023-04-06 10:33:03.000000 plone.app.vocabularies-5.0.2/CONTRIBUTING.rst
--rw-r--r--   0 maurits    (501) staff       (20)    15220 2023-04-06 10:33:03.000000 plone.app.vocabularies-5.0.2/LICENSE.GPL
--rw-r--r--   0 maurits    (501) staff       (20)      684 2023-04-06 10:33:03.000000 plone.app.vocabularies-5.0.2/LICENSE.txt
--rw-r--r--   0 maurits    (501) staff       (20)      152 2023-04-06 10:33:03.000000 plone.app.vocabularies-5.0.2/MANIFEST.in
--rw-r--r--   0 maurits    (501) staff       (20)    23785 2023-04-06 10:33:04.251522 plone.app.vocabularies-5.0.2/PKG-INFO
--rw-r--r--   0 maurits    (501) staff       (20)     6839 2023-04-06 10:33:03.000000 plone.app.vocabularies-5.0.2/README.rst
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-06 10:33:04.239185 plone.app.vocabularies-5.0.2/plone/
--rw-r--r--   0 maurits    (501) staff       (20)       56 2023-04-06 10:33:03.000000 plone.app.vocabularies-5.0.2/plone/__init__.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-06 10:33:04.241459 plone.app.vocabularies-5.0.2/plone/app/
--rw-r--r--   0 maurits    (501) staff       (20)       56 2023-04-06 10:33:03.000000 plone.app.vocabularies-5.0.2/plone/app/__init__.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-06 10:33:04.248471 plone.app.vocabularies-5.0.2/plone/app/vocabularies/
--rw-r--r--   0 maurits    (501) staff       (20)     1992 2023-04-06 10:33:03.000000 plone.app.vocabularies-5.0.2/plone/app/vocabularies/__init__.py
--rw-r--r--   0 maurits    (501) staff       (20)     1724 2023-04-06 10:33:03.000000 plone.app.vocabularies-5.0.2/plone/app/vocabularies/actions.py
--rw-r--r--   0 maurits    (501) staff       (20)    30846 2023-04-06 10:33:03.000000 plone.app.vocabularies-5.0.2/plone/app/vocabularies/catalog.py
--rw-r--r--   0 maurits    (501) staff       (20)     5907 2023-04-06 10:33:03.000000 plone.app.vocabularies-5.0.2/plone/app/vocabularies/configure.zcml
--rw-r--r--   0 maurits    (501) staff       (20)     7842 2023-04-06 10:33:03.000000 plone.app.vocabularies-5.0.2/plone/app/vocabularies/datetimerelated.py
--rw-r--r--   0 maurits    (501) staff       (20)      890 2023-04-06 10:33:03.000000 plone.app.vocabularies-5.0.2/plone/app/vocabularies/editors.py
--rw-r--r--   0 maurits    (501) staff       (20)     5449 2023-04-06 10:33:03.000000 plone.app.vocabularies-5.0.2/plone/app/vocabularies/groups.py
--rw-r--r--   0 maurits    (501) staff       (20)      951 2023-04-06 10:33:03.000000 plone.app.vocabularies-5.0.2/plone/app/vocabularies/images.py
--rw-r--r--   0 maurits    (501) staff       (20)     1735 2023-04-06 10:33:03.000000 plone.app.vocabularies-5.0.2/plone/app/vocabularies/interfaces.py
--rw-r--r--   0 maurits    (501) staff       (20)     4032 2023-04-06 10:33:03.000000 plone.app.vocabularies-5.0.2/plone/app/vocabularies/language.py
--rw-r--r--   0 maurits    (501) staff       (20)     2450 2023-04-06 10:33:03.000000 plone.app.vocabularies-5.0.2/plone/app/vocabularies/metadatafields.py
--rw-r--r--   0 maurits    (501) staff       (20)     9462 2023-04-06 10:33:03.000000 plone.app.vocabularies-5.0.2/plone/app/vocabularies/principals.py
--rw-r--r--   0 maurits    (501) staff       (20)      534 2023-04-06 10:33:03.000000 plone.app.vocabularies-5.0.2/plone/app/vocabularies/searchabletextsource.pt
--rw-r--r--   0 maurits    (501) staff       (20)     2926 2023-04-06 10:33:03.000000 plone.app.vocabularies-5.0.2/plone/app/vocabularies/security.py
--rw-r--r--   0 maurits    (501) staff       (20)     2097 2023-04-06 10:33:03.000000 plone.app.vocabularies-5.0.2/plone/app/vocabularies/skins.py
--rw-r--r--   0 maurits    (501) staff       (20)     1928 2023-04-06 10:33:03.000000 plone.app.vocabularies-5.0.2/plone/app/vocabularies/syndication.py
--rw-r--r--   0 maurits    (501) staff       (20)     3287 2023-04-06 10:33:03.000000 plone.app.vocabularies-5.0.2/plone/app/vocabularies/terms.py
--rw-r--r--   0 maurits    (501) staff       (20)      605 2023-04-06 10:33:03.000000 plone.app.vocabularies-5.0.2/plone/app/vocabularies/testing.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-06 10:33:04.251102 plone.app.vocabularies-5.0.2/plone/app/vocabularies/tests/
--rw-r--r--   0 maurits    (501) staff       (20)        0 2023-04-06 10:33:03.000000 plone.app.vocabularies-5.0.2/plone/app/vocabularies/tests/__init__.py
--rw-r--r--   0 maurits    (501) staff       (20)     3859 2023-04-06 10:33:03.000000 plone.app.vocabularies-5.0.2/plone/app/vocabularies/tests/base.py
--rw-r--r--   0 maurits    (501) staff       (20)      972 2023-04-06 10:33:03.000000 plone.app.vocabularies-5.0.2/plone/app/vocabularies/tests/test_editors.py
--rw-r--r--   0 maurits    (501) staff       (20)      728 2023-04-06 10:33:03.000000 plone.app.vocabularies-5.0.2/plone/app/vocabularies/tests/test_imagesvocabularies.py
--rw-r--r--   0 maurits    (501) staff       (20)    19195 2023-04-06 10:33:03.000000 plone.app.vocabularies-5.0.2/plone/app/vocabularies/tests/test_principals.py
--rw-r--r--   0 maurits    (501) staff       (20)     3356 2023-04-06 10:33:03.000000 plone.app.vocabularies-5.0.2/plone/app/vocabularies/tests/test_subjects_under_context.py
--rw-r--r--   0 maurits    (501) staff       (20)     2775 2023-04-06 10:33:03.000000 plone.app.vocabularies-5.0.2/plone/app/vocabularies/tests/test_timezonevocabularies.py
--rw-r--r--   0 maurits    (501) staff       (20)     3515 2023-04-06 10:33:03.000000 plone.app.vocabularies-5.0.2/plone/app/vocabularies/tests/test_vocabularies.py
--rw-r--r--   0 maurits    (501) staff       (20)    10406 2023-04-06 10:33:03.000000 plone.app.vocabularies-5.0.2/plone/app/vocabularies/types.py
--rw-r--r--   0 maurits    (501) staff       (20)     5586 2023-04-06 10:33:03.000000 plone.app.vocabularies-5.0.2/plone/app/vocabularies/users.py
--rw-r--r--   0 maurits    (501) staff       (20)      741 2023-04-06 10:33:03.000000 plone.app.vocabularies-5.0.2/plone/app/vocabularies/utils.py
--rw-r--r--   0 maurits    (501) staff       (20)     8080 2023-04-06 10:33:03.000000 plone.app.vocabularies-5.0.2/plone/app/vocabularies/workflow.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-06 10:33:04.241231 plone.app.vocabularies-5.0.2/plone.app.vocabularies.egg-info/
--rw-r--r--   0 maurits    (501) staff       (20)    23785 2023-04-06 10:33:04.000000 plone.app.vocabularies-5.0.2/plone.app.vocabularies.egg-info/PKG-INFO
--rw-r--r--   0 maurits    (501) staff       (20)     1655 2023-04-06 10:33:04.000000 plone.app.vocabularies-5.0.2/plone.app.vocabularies.egg-info/SOURCES.txt
--rw-r--r--   0 maurits    (501) staff       (20)        1 2023-04-06 10:33:04.000000 plone.app.vocabularies-5.0.2/plone.app.vocabularies.egg-info/dependency_links.txt
--rw-r--r--   0 maurits    (501) staff       (20)       16 2023-04-06 10:33:04.000000 plone.app.vocabularies-5.0.2/plone.app.vocabularies.egg-info/namespace_packages.txt
--rw-r--r--   0 maurits    (501) staff       (20)        1 2023-04-06 10:33:04.000000 plone.app.vocabularies-5.0.2/plone.app.vocabularies.egg-info/not-zip-safe
--rw-r--r--   0 maurits    (501) staff       (20)      255 2023-04-06 10:33:04.000000 plone.app.vocabularies-5.0.2/plone.app.vocabularies.egg-info/requires.txt
--rw-r--r--   0 maurits    (501) staff       (20)        6 2023-04-06 10:33:04.000000 plone.app.vocabularies-5.0.2/plone.app.vocabularies.egg-info/top_level.txt
--rw-r--r--   0 maurits    (501) staff       (20)     1797 2023-04-06 10:33:03.000000 plone.app.vocabularies-5.0.2/pyproject.toml
--rw-r--r--   0 maurits    (501) staff       (20)      217 2023-04-06 10:33:04.251963 plone.app.vocabularies-5.0.2/setup.cfg
--rw-r--r--   0 maurits    (501) staff       (20)     1842 2023-04-06 10:33:03.000000 plone.app.vocabularies-5.0.2/setup.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-05-22 18:02:13.403282 plone.app.vocabularies-5.0.3/
+-rw-r--r--   0 maurits    (501) staff       (20)    16435 2023-05-22 18:02:12.000000 plone.app.vocabularies-5.0.3/CHANGES.rst
+-rw-r--r--   0 maurits    (501) staff       (20)       70 2023-05-22 18:02:12.000000 plone.app.vocabularies-5.0.3/CONTRIBUTING.rst
+-rw-r--r--   0 maurits    (501) staff       (20)    15220 2023-05-22 18:02:12.000000 plone.app.vocabularies-5.0.3/LICENSE.GPL
+-rw-r--r--   0 maurits    (501) staff       (20)      684 2023-05-22 18:02:12.000000 plone.app.vocabularies-5.0.3/LICENSE.txt
+-rw-r--r--   0 maurits    (501) staff       (20)      152 2023-05-22 18:02:12.000000 plone.app.vocabularies-5.0.3/MANIFEST.in
+-rw-r--r--   0 maurits    (501) staff       (20)    24296 2023-05-22 18:02:13.403415 plone.app.vocabularies-5.0.3/PKG-INFO
+-rw-r--r--   0 maurits    (501) staff       (20)     6839 2023-05-22 18:02:12.000000 plone.app.vocabularies-5.0.3/README.rst
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-05-22 18:02:13.392319 plone.app.vocabularies-5.0.3/plone/
+-rw-r--r--   0 maurits    (501) staff       (20)       56 2023-05-22 18:02:12.000000 plone.app.vocabularies-5.0.3/plone/__init__.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-05-22 18:02:13.394858 plone.app.vocabularies-5.0.3/plone/app/
+-rw-r--r--   0 maurits    (501) staff       (20)       56 2023-05-22 18:02:12.000000 plone.app.vocabularies-5.0.3/plone/app/__init__.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-05-22 18:02:13.400894 plone.app.vocabularies-5.0.3/plone/app/vocabularies/
+-rw-r--r--   0 maurits    (501) staff       (20)     1992 2023-05-22 18:02:12.000000 plone.app.vocabularies-5.0.3/plone/app/vocabularies/__init__.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1724 2023-05-22 18:02:12.000000 plone.app.vocabularies-5.0.3/plone/app/vocabularies/actions.py
+-rw-r--r--   0 maurits    (501) staff       (20)    28641 2023-05-22 18:02:12.000000 plone.app.vocabularies-5.0.3/plone/app/vocabularies/catalog.py
+-rw-r--r--   0 maurits    (501) staff       (20)     5792 2023-05-22 18:02:12.000000 plone.app.vocabularies-5.0.3/plone/app/vocabularies/configure.zcml
+-rw-r--r--   0 maurits    (501) staff       (20)     7842 2023-05-22 18:02:12.000000 plone.app.vocabularies-5.0.3/plone/app/vocabularies/datetimerelated.py
+-rw-r--r--   0 maurits    (501) staff       (20)      890 2023-05-22 18:02:12.000000 plone.app.vocabularies-5.0.3/plone/app/vocabularies/editors.py
+-rw-r--r--   0 maurits    (501) staff       (20)     5449 2023-05-22 18:02:12.000000 plone.app.vocabularies-5.0.3/plone/app/vocabularies/groups.py
+-rw-r--r--   0 maurits    (501) staff       (20)      951 2023-05-22 18:02:12.000000 plone.app.vocabularies-5.0.3/plone/app/vocabularies/images.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1735 2023-05-22 18:02:12.000000 plone.app.vocabularies-5.0.3/plone/app/vocabularies/interfaces.py
+-rw-r--r--   0 maurits    (501) staff       (20)     4032 2023-05-22 18:02:12.000000 plone.app.vocabularies-5.0.3/plone/app/vocabularies/language.py
+-rw-r--r--   0 maurits    (501) staff       (20)     2450 2023-05-22 18:02:12.000000 plone.app.vocabularies-5.0.3/plone/app/vocabularies/metadatafields.py
+-rw-r--r--   0 maurits    (501) staff       (20)     9462 2023-05-22 18:02:12.000000 plone.app.vocabularies-5.0.3/plone/app/vocabularies/principals.py
+-rw-r--r--   0 maurits    (501) staff       (20)      534 2023-05-22 18:02:12.000000 plone.app.vocabularies-5.0.3/plone/app/vocabularies/searchabletextsource.pt
+-rw-r--r--   0 maurits    (501) staff       (20)     2926 2023-05-22 18:02:12.000000 plone.app.vocabularies-5.0.3/plone/app/vocabularies/security.py
+-rw-r--r--   0 maurits    (501) staff       (20)     2097 2023-05-22 18:02:12.000000 plone.app.vocabularies-5.0.3/plone/app/vocabularies/skins.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1928 2023-05-22 18:02:12.000000 plone.app.vocabularies-5.0.3/plone/app/vocabularies/syndication.py
+-rw-r--r--   0 maurits    (501) staff       (20)     3287 2023-05-22 18:02:12.000000 plone.app.vocabularies-5.0.3/plone/app/vocabularies/terms.py
+-rw-r--r--   0 maurits    (501) staff       (20)      605 2023-05-22 18:02:12.000000 plone.app.vocabularies-5.0.3/plone/app/vocabularies/testing.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-05-22 18:02:13.403079 plone.app.vocabularies-5.0.3/plone/app/vocabularies/tests/
+-rw-r--r--   0 maurits    (501) staff       (20)        0 2023-05-22 18:02:12.000000 plone.app.vocabularies-5.0.3/plone/app/vocabularies/tests/__init__.py
+-rw-r--r--   0 maurits    (501) staff       (20)     3859 2023-05-22 18:02:12.000000 plone.app.vocabularies-5.0.3/plone/app/vocabularies/tests/base.py
+-rw-r--r--   0 maurits    (501) staff       (20)      972 2023-05-22 18:02:12.000000 plone.app.vocabularies-5.0.3/plone/app/vocabularies/tests/test_editors.py
+-rw-r--r--   0 maurits    (501) staff       (20)      728 2023-05-22 18:02:12.000000 plone.app.vocabularies-5.0.3/plone/app/vocabularies/tests/test_imagesvocabularies.py
+-rw-r--r--   0 maurits    (501) staff       (20)    19195 2023-05-22 18:02:12.000000 plone.app.vocabularies-5.0.3/plone/app/vocabularies/tests/test_principals.py
+-rw-r--r--   0 maurits    (501) staff       (20)     3356 2023-05-22 18:02:12.000000 plone.app.vocabularies-5.0.3/plone/app/vocabularies/tests/test_subjects_under_context.py
+-rw-r--r--   0 maurits    (501) staff       (20)     2775 2023-05-22 18:02:12.000000 plone.app.vocabularies-5.0.3/plone/app/vocabularies/tests/test_timezonevocabularies.py
+-rw-r--r--   0 maurits    (501) staff       (20)     3515 2023-05-22 18:02:12.000000 plone.app.vocabularies-5.0.3/plone/app/vocabularies/tests/test_vocabularies.py
+-rw-r--r--   0 maurits    (501) staff       (20)    10406 2023-05-22 18:02:12.000000 plone.app.vocabularies-5.0.3/plone/app/vocabularies/types.py
+-rw-r--r--   0 maurits    (501) staff       (20)     5586 2023-05-22 18:02:12.000000 plone.app.vocabularies-5.0.3/plone/app/vocabularies/users.py
+-rw-r--r--   0 maurits    (501) staff       (20)      275 2023-05-22 18:02:12.000000 plone.app.vocabularies-5.0.3/plone/app/vocabularies/utils.py
+-rw-r--r--   0 maurits    (501) staff       (20)     8080 2023-05-22 18:02:12.000000 plone.app.vocabularies-5.0.3/plone/app/vocabularies/workflow.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-05-22 18:02:13.394539 plone.app.vocabularies-5.0.3/plone.app.vocabularies.egg-info/
+-rw-r--r--   0 maurits    (501) staff       (20)    24296 2023-05-22 18:02:13.000000 plone.app.vocabularies-5.0.3/plone.app.vocabularies.egg-info/PKG-INFO
+-rw-r--r--   0 maurits    (501) staff       (20)     1655 2023-05-22 18:02:13.000000 plone.app.vocabularies-5.0.3/plone.app.vocabularies.egg-info/SOURCES.txt
+-rw-r--r--   0 maurits    (501) staff       (20)        1 2023-05-22 18:02:13.000000 plone.app.vocabularies-5.0.3/plone.app.vocabularies.egg-info/dependency_links.txt
+-rw-r--r--   0 maurits    (501) staff       (20)       16 2023-05-22 18:02:13.000000 plone.app.vocabularies-5.0.3/plone.app.vocabularies.egg-info/namespace_packages.txt
+-rw-r--r--   0 maurits    (501) staff       (20)        1 2023-05-22 18:02:13.000000 plone.app.vocabularies-5.0.3/plone.app.vocabularies.egg-info/not-zip-safe
+-rw-r--r--   0 maurits    (501) staff       (20)      233 2023-05-22 18:02:13.000000 plone.app.vocabularies-5.0.3/plone.app.vocabularies.egg-info/requires.txt
+-rw-r--r--   0 maurits    (501) staff       (20)        6 2023-05-22 18:02:13.000000 plone.app.vocabularies-5.0.3/plone.app.vocabularies.egg-info/top_level.txt
+-rw-r--r--   0 maurits    (501) staff       (20)     1797 2023-05-22 18:02:12.000000 plone.app.vocabularies-5.0.3/pyproject.toml
+-rw-r--r--   0 maurits    (501) staff       (20)      217 2023-05-22 18:02:13.403855 plone.app.vocabularies-5.0.3/setup.cfg
+-rw-r--r--   0 maurits    (501) staff       (20)     2014 2023-05-22 18:02:12.000000 plone.app.vocabularies-5.0.3/setup.py
```

### Comparing `plone.app.vocabularies-5.0.2/CHANGES.rst` & `plone.app.vocabularies-5.0.3/CHANGES.rst`

 * *Files 2% similar despite different names*

```diff
@@ -4,14 +4,26 @@
 .. You should *NOT* be adding new change log entries to this file.
    You should create a file in the news directory instead.
    For helpful instructions, please see:
    https://github.com/plone/plone.releaser/blob/master/ADD-A-NEWS-ITEM.rst
 
 .. towncrier release notes start
 
+5.0.3 (2023-05-22)
+------------------
+
+Bug fixes:
+
+
+- Fix a circular dependency to `plone.app.querystring`.
+  Move `.catalog.CatalogVocabularyFactory` to `plone.app.querystring.vocabularies`, move the ZCML to register the factory, move the the test and put BBB code with deprecation wanring into place.
+  Move `.utils.parse_query` with new name `parseAndModifyFormquery` to `plone.app.querystring.queryparser` and put BBB code with deprecation wanring into place.
+  [@jensens] (fix-circular-dep-paquerstring)
+
+
 5.0.2 (2023-04-06)
 ------------------
 
 Bug fixes:
 
 
 - Import navigation root specific from plone.base.
```

### Comparing `plone.app.vocabularies-5.0.2/LICENSE.GPL` & `plone.app.vocabularies-5.0.3/LICENSE.GPL`

 * *Files identical despite different names*

### Comparing `plone.app.vocabularies-5.0.2/LICENSE.txt` & `plone.app.vocabularies-5.0.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `plone.app.vocabularies-5.0.2/PKG-INFO` & `plone.app.vocabularies-5.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plone.app.vocabularies
-Version: 5.0.2
+Version: 5.0.3
 Summary: Collection of generally useful vocabularies for Plone.
 Home-page: https://github.com/plone/plone.app.vocabularies
 Author: Plone Foundation
 Author-email: plone-developers@lists.sourceforge.net
 License: GPL version 2
 Keywords: Plone Zope vocabularies
 Classifier: Development Status :: 6 - Mature
@@ -234,14 +234,26 @@
 .. You should *NOT* be adding new change log entries to this file.
    You should create a file in the news directory instead.
    For helpful instructions, please see:
    https://github.com/plone/plone.releaser/blob/master/ADD-A-NEWS-ITEM.rst
 
 .. towncrier release notes start
 
+5.0.3 (2023-05-22)
+------------------
+
+Bug fixes:
+
+
+- Fix a circular dependency to `plone.app.querystring`.
+  Move `.catalog.CatalogVocabularyFactory` to `plone.app.querystring.vocabularies`, move the ZCML to register the factory, move the the test and put BBB code with deprecation wanring into place.
+  Move `.utils.parse_query` with new name `parseAndModifyFormquery` to `plone.app.querystring.queryparser` and put BBB code with deprecation wanring into place.
+  [@jensens] (fix-circular-dep-paquerstring)
+
+
 5.0.2 (2023-04-06)
 ------------------
 
 Bug fixes:
 
 
 - Import navigation root specific from plone.base.
```

### Comparing `plone.app.vocabularies-5.0.2/README.rst` & `plone.app.vocabularies-5.0.3/README.rst`

 * *Files identical despite different names*

### Comparing `plone.app.vocabularies-5.0.2/plone/app/vocabularies/__init__.py` & `plone.app.vocabularies-5.0.3/plone/app/vocabularies/__init__.py`

 * *Files identical despite different names*

### Comparing `plone.app.vocabularies-5.0.2/plone/app/vocabularies/actions.py` & `plone.app.vocabularies-5.0.3/plone/app/vocabularies/actions.py`

 * *Files identical despite different names*

### Comparing `plone.app.vocabularies-5.0.2/plone/app/vocabularies/catalog.py` & `plone.app.vocabularies-5.0.3/plone/app/vocabularies/catalog.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 from BTrees.IIBTree import intersection
 from plone.app.vocabularies import SlicableVocabulary
 from plone.app.vocabularies.terms import BrowsableTerm
 from plone.app.vocabularies.terms import safe_simplevocabulary_from_values
-from plone.app.vocabularies.utils import parseQueryString
 from plone.base.navigationroot import get_navigation_root_object
 from plone.base.utils import safe_text
 from plone.memoize import request
 from plone.memoize.instance import memoize
 from plone.registry.interfaces import IRegistry
 from plone.uuid.interfaces import IUUID
 from Products.CMFCore.utils import getToolByName
 from Products.Five.browser.pagetemplatefile import ViewPageTemplateFile
 from Products.ZCTextIndex.ParseTree import ParseError
 from z3c.formwidget.query.interfaces import IQuerySource
 from zope.browser.interfaces import ITerms
 from zope.component import queryUtility
 from zope.component.hooks import getSite
+from zope.deferredimport import deprecated
 from zope.globalrequest import getRequest
 from zope.interface import implementer
 from zope.interface import provider
 from zope.schema.interfaces import IContextSourceBinder
 from zope.schema.interfaces import ISource
 from zope.schema.interfaces import IVocabularyFactory
 from zope.schema.vocabulary import SimpleTerm
@@ -36,14 +36,20 @@
 except ImportError:
     from zope.interface import Interface
 
     class ISourceQueryView(Interface):
         pass
 
 
+deprecated(
+    "Import CatalogVocabularyFactory from plone.app.querystring.vocabularies instead (will be removed in Plone 7)",
+    CatalogVocabularyFactory="plone.app.querystring.vocabularies:CatalogVocabularyFactory",
+)
+
+
 def parse_query(query, path_prefix=""):
     """Parse the query string and turn it into a dictionary for querying the
     catalog.
 
     We want to find anything which starts with the given string, so we add
     a * at the end of words.
 
@@ -321,15 +327,15 @@
     ...                         't.browse.foo' : '/foo'})
     >>> view = QuerySearchableTextSourceView(source, request)
     >>> sorted(view.results('t'))
     ['', '', '/1234', 'foo']
 
     Titles need to be unicode:
     >>> view.getTerm(list(view.results('t'))[0]).title
-    u'/foo'
+    '/foo'
     """
 
     template = ViewPageTemplateFile("searchabletextsource.pt")
 
     def __init__(self, context, request):
         msg = (
             "QuerySearchableTextSourceView is deprecated and will be "
@@ -595,72 +601,14 @@
         brains = self.catalog(**query)
         for b in brains:
             return self.createTerm(b, None)
 
     getTermByToken = getTerm
 
 
-@implementer(IVocabularyFactory)
-class CatalogVocabularyFactory:
-    """
-    Test application of Navigation Root:
-
-      >>> from plone.app.vocabularies.tests.base import create_context
-      >>> from plone.app.vocabularies.tests.base import DummyUrlTool
-      >>> from plone.app.vocabularies.tests.base import DummyCatalog
-      >>> class DummyPathCatalog(DummyCatalog):
-      ...     def __call__(self, **query):
-      ...         if 'path' in query and 'query' in query['path']:
-      ...             return [v for v in self.values() if
-      ...                     v.getPath().startswith(query['path']['query'])]
-      ...         return self.values()
-      >>> catalog = DummyPathCatalog(['/abcd', '/defg', '/dummy/sub-site',
-      ...                             '/dummy/sub-site/ghij'])
-      >>> context = create_context()
-      >>> context.portal_catalog = catalog
-      >>> context.portal_url = DummyUrlTool(context)
-      >>> factory = CatalogVocabularyFactory()
-
-      >>> sorted(t.token for t in factory(context))
-      ['/abcd', '/defg', '/dummy/sub-site', '/dummy/sub-site/ghij']
-
-      >>> from plone.app.vocabularies.tests.base import DummyNavRoot
-      >>> nav_root = DummyNavRoot('sub-site', parent=context)
-      >>> [t.token for t in factory(nav_root)]
-      ['/dummy/sub-site', '/dummy/sub-site/ghij']
-
-    """
-
-    # We want to get rid of this and use CatalogSource instead,
-    # but we can't in Plone versions that support
-    # plone.app.widgets < 1.6.0
-
-    def __call__(self, context, query=None):
-        parsed = {}
-        if query:
-            parsed = parseQueryString(context, query["criteria"])
-            if "sort_on" in query:
-                parsed["sort_on"] = query["sort_on"]
-            if "sort_order" in query:
-                parsed["sort_order"] = str(query["sort_order"])
-
-        # If no path is specified check if we are in a sub-site and use that
-        # as the path root for catalog searches
-        if "path" not in parsed:
-            site = getSite()
-            nav_root = get_navigation_root_object(context, site)
-            site_path = site.getPhysicalPath()
-            if nav_root and nav_root.getPhysicalPath() != site_path:
-                parsed["path"] = {
-                    "query": "/".join(nav_root.getPhysicalPath()),
-                    "depth": -1,
-                }
-        return CatalogVocabulary.fromItems(parsed, context)
-
-
 def request_query_cache_key(func, vocab):
     return json.dumps([vocab.query, vocab.text_search_index, vocab.title_template])
 
 
 @implementer(IQuerySource, IVocabularyFactory)
 class StaticCatalogVocabulary(CatalogVocabulary):
     """Catalog Vocabulary for static queries of content based on a fixed query.
@@ -751,37 +699,37 @@
       >>> list(vocab.search(''))
       []
 
       >>> vocab.search('foo')
       <zope.schema.vocabulary.SimpleVocabulary object at ...>
 
       >>> [(t.title, t.value) for t in vocab.search('foo')]
-      [(u'BrainTitle (/1234)', '/1234'), (u'BrainTitle (/2345)', '/2345')]
+      [('BrainTitle (/1234)', '/1234'), ('BrainTitle (/2345)', '/2345')]
 
     We strip out the site path from the rendered path in the title template:
 
       >>> catalog = DummyCatalog(('/site/1234', '/site/2345'))
       >>> context.portal_catalog = catalog
       >>> vocab = StaticCatalogVocabulary({'portal_type': ['Document']})
       >>> [(t.title, t.value) for t in vocab.search('bar')]
-      [(u'BrainTitle (/site/1234)', '/site/1234'),
-       (u'BrainTitle (/site/2345)', '/site/2345')]
+      [('BrainTitle (/site/1234)', '/site/1234'),
+       ('BrainTitle (/site/2345)', '/site/2345')]
 
       >>> context.__name__ = 'site'
       >>> vocab = StaticCatalogVocabulary({'portal_type': ['Document']})
       >>> [(t.title, t.value) for t in vocab.search('bar')]
-      [(u'BrainTitle (/1234)', '/site/1234'),
-       (u'BrainTitle (/2345)', '/site/2345')]
+      [('BrainTitle (/1234)', '/site/1234'),
+       ('BrainTitle (/2345)', '/site/2345')]
 
     The title template can be customized:
 
       >>> vocab.title_template = "{url} {brain.UID} - {brain.Title} {path}"
       >>> [(t.title, t.value) for t in vocab.search('bar')]
-      [(u'proto:/site/1234 /site/1234 - BrainTitle /1234', '/site/1234'),
-       (u'proto:/site/2345 /site/2345 - BrainTitle /2345', '/site/2345')]
+      [('proto:/site/1234 /site/1234 - BrainTitle /1234', '/site/1234'),
+       ('proto:/site/2345 /site/2345 - BrainTitle /2345', '/site/2345')]
 
     """
 
     title_template = "{brain.Title} ({path})"
     text_search_index = "SearchableText"
 
     def __init__(self, query, text_search_index=None, title_template=None):
```

### Comparing `plone.app.vocabularies-5.0.2/plone/app/vocabularies/configure.zcml` & `plone.app.vocabularies-5.0.3/plone/app/vocabularies/configure.zcml`

 * *Files 2% similar despite different names*

```diff
@@ -98,19 +98,14 @@
       />
   <utility
       factory=".principals.PrincipalsFactory"
       name="plone.app.vocabularies.Principals"
       />
 
   <utility
-      factory=".catalog.CatalogVocabularyFactory"
-      name="plone.app.vocabularies.Catalog"
-      />
-
-  <utility
       name="plone.app.vocabularies.Actions"
       component=".actions.ActionCategoriesVocabularyFactory"
       />
 
   <utility
       name="plone.app.vocabularies.PortalActionCategories"
       component=".actions.PortalActionCategoriesVocabularyFactory"
```

### Comparing `plone.app.vocabularies-5.0.2/plone/app/vocabularies/datetimerelated.py` & `plone.app.vocabularies-5.0.3/plone/app/vocabularies/datetimerelated.py`

 * *Files identical despite different names*

### Comparing `plone.app.vocabularies-5.0.2/plone/app/vocabularies/editors.py` & `plone.app.vocabularies-5.0.3/plone/app/vocabularies/editors.py`

 * *Files identical despite different names*

### Comparing `plone.app.vocabularies-5.0.2/plone/app/vocabularies/groups.py` & `plone.app.vocabularies-5.0.3/plone/app/vocabularies/groups.py`

 * *Files identical despite different names*

### Comparing `plone.app.vocabularies-5.0.2/plone/app/vocabularies/images.py` & `plone.app.vocabularies-5.0.3/plone/app/vocabularies/images.py`

 * *Files identical despite different names*

### Comparing `plone.app.vocabularies-5.0.2/plone/app/vocabularies/interfaces.py` & `plone.app.vocabularies-5.0.3/plone/app/vocabularies/interfaces.py`

 * *Files identical despite different names*

### Comparing `plone.app.vocabularies-5.0.2/plone/app/vocabularies/language.py` & `plone.app.vocabularies-5.0.3/plone/app/vocabularies/language.py`

 * *Files identical despite different names*

### Comparing `plone.app.vocabularies-5.0.2/plone/app/vocabularies/metadatafields.py` & `plone.app.vocabularies-5.0.3/plone/app/vocabularies/metadatafields.py`

 * *Files identical despite different names*

### Comparing `plone.app.vocabularies-5.0.2/plone/app/vocabularies/principals.py` & `plone.app.vocabularies-5.0.3/plone/app/vocabularies/principals.py`

 * *Files identical despite different names*

### Comparing `plone.app.vocabularies-5.0.2/plone/app/vocabularies/searchabletextsource.pt` & `plone.app.vocabularies-5.0.3/plone/app/vocabularies/searchabletextsource.pt`

 * *Files identical despite different names*

### Comparing `plone.app.vocabularies-5.0.2/plone/app/vocabularies/security.py` & `plone.app.vocabularies-5.0.3/plone/app/vocabularies/security.py`

 * *Files identical despite different names*

### Comparing `plone.app.vocabularies-5.0.2/plone/app/vocabularies/skins.py` & `plone.app.vocabularies-5.0.3/plone/app/vocabularies/skins.py`

 * *Files identical despite different names*

### Comparing `plone.app.vocabularies-5.0.2/plone/app/vocabularies/syndication.py` & `plone.app.vocabularies-5.0.3/plone/app/vocabularies/syndication.py`

 * *Files identical despite different names*

### Comparing `plone.app.vocabularies-5.0.2/plone/app/vocabularies/terms.py` & `plone.app.vocabularies-5.0.3/plone/app/vocabularies/terms.py`

 * *Files identical despite different names*

### Comparing `plone.app.vocabularies-5.0.2/plone/app/vocabularies/testing.py` & `plone.app.vocabularies-5.0.3/plone/app/vocabularies/testing.py`

 * *Files identical despite different names*

### Comparing `plone.app.vocabularies-5.0.2/plone/app/vocabularies/tests/base.py` & `plone.app.vocabularies-5.0.3/plone/app/vocabularies/tests/base.py`

 * *Files identical despite different names*

### Comparing `plone.app.vocabularies-5.0.2/plone/app/vocabularies/tests/test_editors.py` & `plone.app.vocabularies-5.0.3/plone/app/vocabularies/tests/test_editors.py`

 * *Files identical despite different names*

### Comparing `plone.app.vocabularies-5.0.2/plone/app/vocabularies/tests/test_imagesvocabularies.py` & `plone.app.vocabularies-5.0.3/plone/app/vocabularies/tests/test_imagesvocabularies.py`

 * *Files identical despite different names*

### Comparing `plone.app.vocabularies-5.0.2/plone/app/vocabularies/tests/test_principals.py` & `plone.app.vocabularies-5.0.3/plone/app/vocabularies/tests/test_principals.py`

 * *Files identical despite different names*

### Comparing `plone.app.vocabularies-5.0.2/plone/app/vocabularies/tests/test_subjects_under_context.py` & `plone.app.vocabularies-5.0.3/plone/app/vocabularies/tests/test_subjects_under_context.py`

 * *Files identical despite different names*

### Comparing `plone.app.vocabularies-5.0.2/plone/app/vocabularies/tests/test_timezonevocabularies.py` & `plone.app.vocabularies-5.0.3/plone/app/vocabularies/tests/test_timezonevocabularies.py`

 * *Files identical despite different names*

### Comparing `plone.app.vocabularies-5.0.2/plone/app/vocabularies/tests/test_vocabularies.py` & `plone.app.vocabularies-5.0.3/plone/app/vocabularies/tests/test_vocabularies.py`

 * *Files identical despite different names*

### Comparing `plone.app.vocabularies-5.0.2/plone/app/vocabularies/types.py` & `plone.app.vocabularies-5.0.3/plone/app/vocabularies/types.py`

 * *Files identical despite different names*

### Comparing `plone.app.vocabularies-5.0.2/plone/app/vocabularies/users.py` & `plone.app.vocabularies-5.0.3/plone/app/vocabularies/users.py`

 * *Files identical despite different names*

### Comparing `plone.app.vocabularies-5.0.2/plone/app/vocabularies/workflow.py` & `plone.app.vocabularies-5.0.3/plone/app/vocabularies/workflow.py`

 * *Files identical despite different names*

### Comparing `plone.app.vocabularies-5.0.2/plone.app.vocabularies.egg-info/PKG-INFO` & `plone.app.vocabularies-5.0.3/plone.app.vocabularies.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plone.app.vocabularies
-Version: 5.0.2
+Version: 5.0.3
 Summary: Collection of generally useful vocabularies for Plone.
 Home-page: https://github.com/plone/plone.app.vocabularies
 Author: Plone Foundation
 Author-email: plone-developers@lists.sourceforge.net
 License: GPL version 2
 Keywords: Plone Zope vocabularies
 Classifier: Development Status :: 6 - Mature
@@ -234,14 +234,26 @@
 .. You should *NOT* be adding new change log entries to this file.
    You should create a file in the news directory instead.
    For helpful instructions, please see:
    https://github.com/plone/plone.releaser/blob/master/ADD-A-NEWS-ITEM.rst
 
 .. towncrier release notes start
 
+5.0.3 (2023-05-22)
+------------------
+
+Bug fixes:
+
+
+- Fix a circular dependency to `plone.app.querystring`.
+  Move `.catalog.CatalogVocabularyFactory` to `plone.app.querystring.vocabularies`, move the ZCML to register the factory, move the the test and put BBB code with deprecation wanring into place.
+  Move `.utils.parse_query` with new name `parseAndModifyFormquery` to `plone.app.querystring.queryparser` and put BBB code with deprecation wanring into place.
+  [@jensens] (fix-circular-dep-paquerstring)
+
+
 5.0.2 (2023-04-06)
 ------------------
 
 Bug fixes:
 
 
 - Import navigation root specific from plone.base.
```

### Comparing `plone.app.vocabularies-5.0.2/plone.app.vocabularies.egg-info/SOURCES.txt` & `plone.app.vocabularies-5.0.3/plone.app.vocabularies.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `plone.app.vocabularies-5.0.2/pyproject.toml` & `plone.app.vocabularies-5.0.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `plone.app.vocabularies-5.0.2/setup.py` & `plone.app.vocabularies-5.0.3/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import find_packages
 from setuptools import setup
 
 
-version = "5.0.2"
+version = "5.0.3"
 
 setup(
     name="plone.app.vocabularies",
     version=version,
     description="Collection of generally useful vocabularies for Plone.",
     long_description="{}\n{}".format(
         open("README.rst").read(), open("CHANGES.rst").read()
@@ -33,17 +33,19 @@
     license="GPL version 2",
     packages=find_packages(),
     namespace_packages=["plone", "plone.app"],
     include_package_data=True,
     zip_safe=False,
     python_requires=">=3.8",
     install_requires=[
+        # be very careful adding dependencies here, as this package is used
+        # by many many other packages in plone.app.* namespace
+        # it is very easy to add transitive circular dependencies
         "BTrees",
         "Products.ZCatalog",
-        "plone.app.querystring",
         "plone.base",
         "plone.memoize",
         "plone.namedfile",
         "plone.registry",
         "plone.uuid",
         "pytz",
         "setuptools",
```

