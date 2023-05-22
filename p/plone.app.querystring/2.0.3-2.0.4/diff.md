# Comparing `tmp/plone.app.querystring-2.0.3.tar.gz` & `tmp/plone.app.querystring-2.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "plone.app.querystring-2.0.3.tar", last modified: Wed Apr 26 21:58:25 2023, max compression
+gzip compressed data, was "plone.app.querystring-2.0.4.tar", last modified: Mon May 22 18:01:36 2023, max compression
```

## Comparing `plone.app.querystring-2.0.3.tar` & `plone.app.querystring-2.0.4.tar`

### file list

```diff
@@ -1,84 +1,86 @@
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-26 21:58:25.265349 plone.app.querystring-2.0.3/
--rw-r--r--   0 maurits    (501) staff       (20)    12307 2023-04-26 21:58:24.000000 plone.app.querystring-2.0.3/CHANGES.rst
--rw-r--r--   0 maurits    (501) staff       (20)       70 2023-04-26 21:58:24.000000 plone.app.querystring-2.0.3/CONTRIBUTING.rst
--rw-r--r--   0 maurits    (501) staff       (20)      149 2023-04-26 21:58:24.000000 plone.app.querystring-2.0.3/MANIFEST.in
--rw-r--r--   0 maurits    (501) staff       (20)    14198 2023-04-26 21:58:25.265502 plone.app.querystring-2.0.3/PKG-INFO
--rw-r--r--   0 maurits    (501) staff       (20)      966 2023-04-26 21:58:24.000000 plone.app.querystring-2.0.3/README.rst
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-26 21:58:25.243237 plone.app.querystring-2.0.3/docs/
--rw-r--r--   0 maurits    (501) staff       (20)    15220 2023-04-26 21:58:24.000000 plone.app.querystring-2.0.3/docs/LICENSE.GPL
--rw-r--r--   0 maurits    (501) staff       (20)      683 2023-04-26 21:58:24.000000 plone.app.querystring-2.0.3/docs/LICENSE.txt
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-26 21:58:25.243541 plone.app.querystring-2.0.3/plone/
--rw-r--r--   0 maurits    (501) staff       (20)       56 2023-04-26 21:58:24.000000 plone.app.querystring-2.0.3/plone/__init__.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-26 21:58:25.247624 plone.app.querystring-2.0.3/plone/app/
--rw-r--r--   0 maurits    (501) staff       (20)       56 2023-04-26 21:58:24.000000 plone.app.querystring-2.0.3/plone/app/__init__.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-26 21:58:25.254094 plone.app.querystring-2.0.3/plone/app/querystring/
--rw-r--r--   0 maurits    (501) staff       (20)        2 2023-04-26 21:58:24.000000 plone.app.querystring-2.0.3/plone/app/querystring/__init__.py
--rw-r--r--   0 maurits    (501) staff       (20)     1692 2023-04-26 21:58:24.000000 plone.app.querystring-2.0.3/plone/app/querystring/configure.zcml
--rw-r--r--   0 maurits    (501) staff       (20)     1020 2023-04-26 21:58:24.000000 plone.app.querystring-2.0.3/plone/app/querystring/hiddenprofiles.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-26 21:58:25.255499 plone.app.querystring-2.0.3/plone/app/querystring/indexmodifiers/
--rw-r--r--   0 maurits    (501) staff       (20)        0 2023-04-26 21:58:24.000000 plone.app.querystring-2.0.3/plone/app/querystring/indexmodifiers/__init__.py
--rw-r--r--   0 maurits    (501) staff       (20)     1240 2023-04-26 21:58:24.000000 plone.app.querystring-2.0.3/plone/app/querystring/indexmodifiers/configure.zcml
--rw-r--r--   0 maurits    (501) staff       (20)     2644 2023-04-26 21:58:24.000000 plone.app.querystring-2.0.3/plone/app/querystring/indexmodifiers/query_index_modifiers.py
--rw-r--r--   0 maurits    (501) staff       (20)     1562 2023-04-26 21:58:24.000000 plone.app.querystring-2.0.3/plone/app/querystring/interfaces.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-26 21:58:25.238587 plone.app.querystring-2.0.3/plone/app/querystring/profiles/
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-26 21:58:25.256503 plone.app.querystring-2.0.3/plone/app/querystring/profiles/default/
--rw-r--r--   0 maurits    (501) staff       (20)      185 2023-04-26 21:58:24.000000 plone.app.querystring-2.0.3/plone/app/querystring/profiles/default/metadata.xml
--rw-r--r--   0 maurits    (501) staff       (20)    32950 2023-04-26 21:58:24.000000 plone.app.querystring-2.0.3/plone/app/querystring/profiles/default/registry.xml
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-26 21:58:25.240017 plone.app.querystring-2.0.3/plone/app/querystring/profiles/upgrades/
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-26 21:58:25.257157 plone.app.querystring-2.0.3/plone/app/querystring/profiles/upgrades/to_10/
--rw-r--r--   0 maurits    (501) staff       (20)      539 2023-04-26 21:58:24.000000 plone.app.querystring-2.0.3/plone/app/querystring/profiles/upgrades/to_10/registry.xml
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-26 21:58:25.257680 plone.app.querystring-2.0.3/plone/app/querystring/profiles/upgrades/to_11/
--rw-r--r--   0 maurits    (501) staff       (20)     3366 2023-04-26 21:58:24.000000 plone.app.querystring-2.0.3/plone/app/querystring/profiles/upgrades/to_11/registry.xml
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-26 21:58:25.258242 plone.app.querystring-2.0.3/plone/app/querystring/profiles/upgrades/to_14/
--rw-r--r--   0 maurits    (501) staff       (20)     2961 2023-04-26 21:58:24.000000 plone.app.querystring-2.0.3/plone/app/querystring/profiles/upgrades/to_14/registry.xml
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-26 21:58:25.258736 plone.app.querystring-2.0.3/plone/app/querystring/profiles/upgrades/to_3/
--rw-r--r--   0 maurits    (501) staff       (20)     1411 2023-04-26 21:58:24.000000 plone.app.querystring-2.0.3/plone/app/querystring/profiles/upgrades/to_3/registry.xml
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-26 21:58:25.259098 plone.app.querystring-2.0.3/plone/app/querystring/profiles/upgrades/to_5/
--rw-r--r--   0 maurits    (501) staff       (20)     1819 2023-04-26 21:58:24.000000 plone.app.querystring-2.0.3/plone/app/querystring/profiles/upgrades/to_5/registry.xml
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-26 21:58:25.259434 plone.app.querystring-2.0.3/plone/app/querystring/profiles/upgrades/to_6/
--rw-r--r--   0 maurits    (501) staff       (20)     1772 2023-04-26 21:58:24.000000 plone.app.querystring-2.0.3/plone/app/querystring/profiles/upgrades/to_6/registry.xml
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-26 21:58:25.259775 plone.app.querystring-2.0.3/plone/app/querystring/profiles/upgrades/to_7/
--rw-r--r--   0 maurits    (501) staff       (20)      339 2023-04-26 21:58:24.000000 plone.app.querystring-2.0.3/plone/app/querystring/profiles/upgrades/to_7/registry.xml
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-26 21:58:25.260093 plone.app.querystring-2.0.3/plone/app/querystring/profiles/upgrades/to_8/
--rw-r--r--   0 maurits    (501) staff       (20)     1818 2023-04-26 21:58:24.000000 plone.app.querystring-2.0.3/plone/app/querystring/profiles/upgrades/to_8/registry.xml
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-26 21:58:25.260413 plone.app.querystring-2.0.3/plone/app/querystring/profiles/upgrades/to_9/
--rw-r--r--   0 maurits    (501) staff       (20)     1060 2023-04-26 21:58:24.000000 plone.app.querystring-2.0.3/plone/app/querystring/profiles/upgrades/to_9/registry.xml
--rw-r--r--   0 maurits    (501) staff       (20)     2785 2023-04-26 21:58:24.000000 plone.app.querystring-2.0.3/plone/app/querystring/profiles.zcml
--rw-r--r--   0 maurits    (501) staff       (20)     9157 2023-04-26 21:58:24.000000 plone.app.querystring-2.0.3/plone/app/querystring/querybuilder.py
--rw-r--r--   0 maurits    (501) staff       (20)      715 2023-04-26 21:58:24.000000 plone.app.querystring-2.0.3/plone/app/querystring/querymodifiers.py
--rw-r--r--   0 maurits    (501) staff       (20)    10543 2023-04-26 21:58:24.000000 plone.app.querystring-2.0.3/plone/app/querystring/queryparser.py
--rw-r--r--   0 maurits    (501) staff       (20)     5128 2023-04-26 21:58:24.000000 plone.app.querystring-2.0.3/plone/app/querystring/registryreader.py
--rw-r--r--   0 maurits    (501) staff       (20)     4662 2023-04-26 21:58:24.000000 plone.app.querystring-2.0.3/plone/app/querystring/results.pt
--rw-r--r--   0 maurits    (501) staff       (20)     2205 2023-04-26 21:58:24.000000 plone.app.querystring-2.0.3/plone/app/querystring/testing.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-26 21:58:25.264479 plone.app.querystring-2.0.3/plone/app/querystring/tests/
--rw-r--r--   0 maurits    (501) staff       (20)        0 2023-04-26 21:58:24.000000 plone.app.querystring-2.0.3/plone/app/querystring/tests/__init__.py
--rw-r--r--   0 maurits    (501) staff       (20)      481 2023-04-26 21:58:24.000000 plone.app.querystring-2.0.3/plone/app/querystring/tests/configure.zcml
--rw-r--r--   0 maurits    (501) staff       (20)      863 2023-04-26 21:58:24.000000 plone.app.querystring-2.0.3/plone/app/querystring/tests/index_testmodifier.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-26 21:58:25.240488 plone.app.querystring-2.0.3/plone/app/querystring/tests/profiles/
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-26 21:58:25.265090 plone.app.querystring-2.0.3/plone/app/querystring/tests/profiles/registry/
--rw-r--r--   0 maurits    (501) staff       (20)      184 2023-04-26 21:58:24.000000 plone.app.querystring-2.0.3/plone/app/querystring/tests/profiles/registry/metadata.xml
--rw-r--r--   0 maurits    (501) staff       (20)     1283 2023-04-26 21:58:24.000000 plone.app.querystring-2.0.3/plone/app/querystring/tests/profiles/registry/registry.xml
--rw-r--r--   0 maurits    (501) staff       (20)     2202 2023-04-26 21:58:24.000000 plone.app.querystring-2.0.3/plone/app/querystring/tests/registry_minimal_correct.xml
--rw-r--r--   0 maurits    (501) staff       (20)      984 2023-04-26 21:58:24.000000 plone.app.querystring-2.0.3/plone/app/querystring/tests/registry_test_missing_operator.xml
--rw-r--r--   0 maurits    (501) staff       (20)     1000 2023-04-26 21:58:24.000000 plone.app.querystring-2.0.3/plone/app/querystring/tests/registry_test_vocabulary.xml
--rw-r--r--   0 maurits    (501) staff       (20)     2806 2023-04-26 21:58:24.000000 plone.app.querystring-2.0.3/plone/app/querystring/tests/registry_testdata.py
--rw-r--r--   0 maurits    (501) staff       (20)     2405 2023-04-26 21:58:24.000000 plone.app.querystring-2.0.3/plone/app/querystring/tests/testIndexmodifiers.py
--rw-r--r--   0 maurits    (501) staff       (20)    15001 2023-04-26 21:58:24.000000 plone.app.querystring-2.0.3/plone/app/querystring/tests/testQueryBuilder.py
--rw-r--r--   0 maurits    (501) staff       (20)     3515 2023-04-26 21:58:24.000000 plone.app.querystring-2.0.3/plone/app/querystring/tests/testQueryBuilderModifiers.py
--rw-r--r--   0 maurits    (501) staff       (20)    21787 2023-04-26 21:58:24.000000 plone.app.querystring-2.0.3/plone/app/querystring/tests/testQueryParser.py
--rw-r--r--   0 maurits    (501) staff       (20)     2941 2023-04-26 21:58:24.000000 plone.app.querystring-2.0.3/plone/app/querystring/tests/testRegistryIntegration.py
--rw-r--r--   0 maurits    (501) staff       (20)     5653 2023-04-26 21:58:24.000000 plone.app.querystring-2.0.3/plone/app/querystring/tests/testRegistryReader.py
--rw-r--r--   0 maurits    (501) staff       (20)     2178 2023-04-26 21:58:24.000000 plone.app.querystring-2.0.3/plone/app/querystring/upgrades.py
--rw-r--r--   0 maurits    (501) staff       (20)     5147 2023-04-26 21:58:24.000000 plone.app.querystring-2.0.3/plone/app/querystring/upgrades.zcml
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-26 21:58:25.247137 plone.app.querystring-2.0.3/plone.app.querystring.egg-info/
--rw-r--r--   0 maurits    (501) staff       (20)    14198 2023-04-26 21:58:25.000000 plone.app.querystring-2.0.3/plone.app.querystring.egg-info/PKG-INFO
--rw-r--r--   0 maurits    (501) staff       (20)     2579 2023-04-26 21:58:25.000000 plone.app.querystring-2.0.3/plone.app.querystring.egg-info/SOURCES.txt
--rw-r--r--   0 maurits    (501) staff       (20)        1 2023-04-26 21:58:25.000000 plone.app.querystring-2.0.3/plone.app.querystring.egg-info/dependency_links.txt
--rw-r--r--   0 maurits    (501) staff       (20)       40 2023-04-26 21:58:25.000000 plone.app.querystring-2.0.3/plone.app.querystring.egg-info/entry_points.txt
--rw-r--r--   0 maurits    (501) staff       (20)       16 2023-04-26 21:58:25.000000 plone.app.querystring-2.0.3/plone.app.querystring.egg-info/namespace_packages.txt
--rw-r--r--   0 maurits    (501) staff       (20)        1 2023-04-26 21:58:25.000000 plone.app.querystring-2.0.3/plone.app.querystring.egg-info/not-zip-safe
--rw-r--r--   0 maurits    (501) staff       (20)      274 2023-04-26 21:58:25.000000 plone.app.querystring-2.0.3/plone.app.querystring.egg-info/requires.txt
--rw-r--r--   0 maurits    (501) staff       (20)        6 2023-04-26 21:58:25.000000 plone.app.querystring-2.0.3/plone.app.querystring.egg-info/top_level.txt
--rw-r--r--   0 maurits    (501) staff       (20)     1690 2023-04-26 21:58:24.000000 plone.app.querystring-2.0.3/pyproject.toml
--rw-r--r--   0 maurits    (501) staff       (20)      217 2023-04-26 21:58:25.266117 plone.app.querystring-2.0.3/setup.cfg
--rw-r--r--   0 maurits    (501) staff       (20)     1962 2023-04-26 21:58:24.000000 plone.app.querystring-2.0.3/setup.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-05-22 18:01:36.269214 plone.app.querystring-2.0.4/
+-rw-r--r--   0 maurits    (501) staff       (20)    12787 2023-05-22 18:01:35.000000 plone.app.querystring-2.0.4/CHANGES.rst
+-rw-r--r--   0 maurits    (501) staff       (20)       70 2023-05-22 18:01:35.000000 plone.app.querystring-2.0.4/CONTRIBUTING.rst
+-rw-r--r--   0 maurits    (501) staff       (20)      149 2023-05-22 18:01:35.000000 plone.app.querystring-2.0.4/MANIFEST.in
+-rw-r--r--   0 maurits    (501) staff       (20)    14678 2023-05-22 18:01:36.269335 plone.app.querystring-2.0.4/PKG-INFO
+-rw-r--r--   0 maurits    (501) staff       (20)      966 2023-05-22 18:01:35.000000 plone.app.querystring-2.0.4/README.rst
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-05-22 18:01:36.253178 plone.app.querystring-2.0.4/docs/
+-rw-r--r--   0 maurits    (501) staff       (20)    15220 2023-05-22 18:01:35.000000 plone.app.querystring-2.0.4/docs/LICENSE.GPL
+-rw-r--r--   0 maurits    (501) staff       (20)      683 2023-05-22 18:01:35.000000 plone.app.querystring-2.0.4/docs/LICENSE.txt
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-05-22 18:01:36.253423 plone.app.querystring-2.0.4/plone/
+-rw-r--r--   0 maurits    (501) staff       (20)       56 2023-05-22 18:01:35.000000 plone.app.querystring-2.0.4/plone/__init__.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-05-22 18:01:36.255989 plone.app.querystring-2.0.4/plone/app/
+-rw-r--r--   0 maurits    (501) staff       (20)       56 2023-05-22 18:01:35.000000 plone.app.querystring-2.0.4/plone/app/__init__.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-05-22 18:01:36.260054 plone.app.querystring-2.0.4/plone/app/querystring/
+-rw-r--r--   0 maurits    (501) staff       (20)        2 2023-05-22 18:01:35.000000 plone.app.querystring-2.0.4/plone/app/querystring/__init__.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1811 2023-05-22 18:01:35.000000 plone.app.querystring-2.0.4/plone/app/querystring/configure.zcml
+-rw-r--r--   0 maurits    (501) staff       (20)     1020 2023-05-22 18:01:35.000000 plone.app.querystring-2.0.4/plone/app/querystring/hiddenprofiles.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-05-22 18:01:36.260908 plone.app.querystring-2.0.4/plone/app/querystring/indexmodifiers/
+-rw-r--r--   0 maurits    (501) staff       (20)        0 2023-05-22 18:01:35.000000 plone.app.querystring-2.0.4/plone/app/querystring/indexmodifiers/__init__.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1240 2023-05-22 18:01:35.000000 plone.app.querystring-2.0.4/plone/app/querystring/indexmodifiers/configure.zcml
+-rw-r--r--   0 maurits    (501) staff       (20)     2644 2023-05-22 18:01:35.000000 plone.app.querystring-2.0.4/plone/app/querystring/indexmodifiers/query_index_modifiers.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1562 2023-05-22 18:01:35.000000 plone.app.querystring-2.0.4/plone/app/querystring/interfaces.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-05-22 18:01:36.248683 plone.app.querystring-2.0.4/plone/app/querystring/profiles/
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-05-22 18:01:36.261393 plone.app.querystring-2.0.4/plone/app/querystring/profiles/default/
+-rw-r--r--   0 maurits    (501) staff       (20)      185 2023-05-22 18:01:35.000000 plone.app.querystring-2.0.4/plone/app/querystring/profiles/default/metadata.xml
+-rw-r--r--   0 maurits    (501) staff       (20)    32950 2023-05-22 18:01:35.000000 plone.app.querystring-2.0.4/plone/app/querystring/profiles/default/registry.xml
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-05-22 18:01:36.250192 plone.app.querystring-2.0.4/plone/app/querystring/profiles/upgrades/
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-05-22 18:01:36.261735 plone.app.querystring-2.0.4/plone/app/querystring/profiles/upgrades/to_10/
+-rw-r--r--   0 maurits    (501) staff       (20)      539 2023-05-22 18:01:35.000000 plone.app.querystring-2.0.4/plone/app/querystring/profiles/upgrades/to_10/registry.xml
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-05-22 18:01:36.262108 plone.app.querystring-2.0.4/plone/app/querystring/profiles/upgrades/to_11/
+-rw-r--r--   0 maurits    (501) staff       (20)     3366 2023-05-22 18:01:35.000000 plone.app.querystring-2.0.4/plone/app/querystring/profiles/upgrades/to_11/registry.xml
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-05-22 18:01:36.262466 plone.app.querystring-2.0.4/plone/app/querystring/profiles/upgrades/to_14/
+-rw-r--r--   0 maurits    (501) staff       (20)     2961 2023-05-22 18:01:35.000000 plone.app.querystring-2.0.4/plone/app/querystring/profiles/upgrades/to_14/registry.xml
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-05-22 18:01:36.262738 plone.app.querystring-2.0.4/plone/app/querystring/profiles/upgrades/to_3/
+-rw-r--r--   0 maurits    (501) staff       (20)     1411 2023-05-22 18:01:35.000000 plone.app.querystring-2.0.4/plone/app/querystring/profiles/upgrades/to_3/registry.xml
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-05-22 18:01:36.263016 plone.app.querystring-2.0.4/plone/app/querystring/profiles/upgrades/to_5/
+-rw-r--r--   0 maurits    (501) staff       (20)     1819 2023-05-22 18:01:35.000000 plone.app.querystring-2.0.4/plone/app/querystring/profiles/upgrades/to_5/registry.xml
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-05-22 18:01:36.263506 plone.app.querystring-2.0.4/plone/app/querystring/profiles/upgrades/to_6/
+-rw-r--r--   0 maurits    (501) staff       (20)     1772 2023-05-22 18:01:35.000000 plone.app.querystring-2.0.4/plone/app/querystring/profiles/upgrades/to_6/registry.xml
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-05-22 18:01:36.263775 plone.app.querystring-2.0.4/plone/app/querystring/profiles/upgrades/to_7/
+-rw-r--r--   0 maurits    (501) staff       (20)      339 2023-05-22 18:01:35.000000 plone.app.querystring-2.0.4/plone/app/querystring/profiles/upgrades/to_7/registry.xml
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-05-22 18:01:36.264032 plone.app.querystring-2.0.4/plone/app/querystring/profiles/upgrades/to_8/
+-rw-r--r--   0 maurits    (501) staff       (20)     1818 2023-05-22 18:01:35.000000 plone.app.querystring-2.0.4/plone/app/querystring/profiles/upgrades/to_8/registry.xml
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-05-22 18:01:36.264308 plone.app.querystring-2.0.4/plone/app/querystring/profiles/upgrades/to_9/
+-rw-r--r--   0 maurits    (501) staff       (20)     1060 2023-05-22 18:01:35.000000 plone.app.querystring-2.0.4/plone/app/querystring/profiles/upgrades/to_9/registry.xml
+-rw-r--r--   0 maurits    (501) staff       (20)     2785 2023-05-22 18:01:35.000000 plone.app.querystring-2.0.4/plone/app/querystring/profiles.zcml
+-rw-r--r--   0 maurits    (501) staff       (20)     9157 2023-05-22 18:01:35.000000 plone.app.querystring-2.0.4/plone/app/querystring/querybuilder.py
+-rw-r--r--   0 maurits    (501) staff       (20)      715 2023-05-22 18:01:35.000000 plone.app.querystring-2.0.4/plone/app/querystring/querymodifiers.py
+-rw-r--r--   0 maurits    (501) staff       (20)    11264 2023-05-22 18:01:35.000000 plone.app.querystring-2.0.4/plone/app/querystring/queryparser.py
+-rw-r--r--   0 maurits    (501) staff       (20)     5128 2023-05-22 18:01:35.000000 plone.app.querystring-2.0.4/plone/app/querystring/registryreader.py
+-rw-r--r--   0 maurits    (501) staff       (20)     4662 2023-05-22 18:01:35.000000 plone.app.querystring-2.0.4/plone/app/querystring/results.pt
+-rw-r--r--   0 maurits    (501) staff       (20)     2205 2023-05-22 18:01:35.000000 plone.app.querystring-2.0.4/plone/app/querystring/testing.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-05-22 18:01:36.268469 plone.app.querystring-2.0.4/plone/app/querystring/tests/
+-rw-r--r--   0 maurits    (501) staff       (20)        0 2023-05-22 18:01:35.000000 plone.app.querystring-2.0.4/plone/app/querystring/tests/__init__.py
+-rw-r--r--   0 maurits    (501) staff       (20)      481 2023-05-22 18:01:35.000000 plone.app.querystring-2.0.4/plone/app/querystring/tests/configure.zcml
+-rw-r--r--   0 maurits    (501) staff       (20)      863 2023-05-22 18:01:35.000000 plone.app.querystring-2.0.4/plone/app/querystring/tests/index_testmodifier.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-05-22 18:01:36.250566 plone.app.querystring-2.0.4/plone/app/querystring/tests/profiles/
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-05-22 18:01:36.269016 plone.app.querystring-2.0.4/plone/app/querystring/tests/profiles/registry/
+-rw-r--r--   0 maurits    (501) staff       (20)      184 2023-05-22 18:01:35.000000 plone.app.querystring-2.0.4/plone/app/querystring/tests/profiles/registry/metadata.xml
+-rw-r--r--   0 maurits    (501) staff       (20)     1283 2023-05-22 18:01:35.000000 plone.app.querystring-2.0.4/plone/app/querystring/tests/profiles/registry/registry.xml
+-rw-r--r--   0 maurits    (501) staff       (20)     2202 2023-05-22 18:01:35.000000 plone.app.querystring-2.0.4/plone/app/querystring/tests/registry_minimal_correct.xml
+-rw-r--r--   0 maurits    (501) staff       (20)      984 2023-05-22 18:01:35.000000 plone.app.querystring-2.0.4/plone/app/querystring/tests/registry_test_missing_operator.xml
+-rw-r--r--   0 maurits    (501) staff       (20)     1000 2023-05-22 18:01:35.000000 plone.app.querystring-2.0.4/plone/app/querystring/tests/registry_test_vocabulary.xml
+-rw-r--r--   0 maurits    (501) staff       (20)     2806 2023-05-22 18:01:35.000000 plone.app.querystring-2.0.4/plone/app/querystring/tests/registry_testdata.py
+-rw-r--r--   0 maurits    (501) staff       (20)     2405 2023-05-22 18:01:35.000000 plone.app.querystring-2.0.4/plone/app/querystring/tests/testIndexmodifiers.py
+-rw-r--r--   0 maurits    (501) staff       (20)    15001 2023-05-22 18:01:35.000000 plone.app.querystring-2.0.4/plone/app/querystring/tests/testQueryBuilder.py
+-rw-r--r--   0 maurits    (501) staff       (20)     3515 2023-05-22 18:01:35.000000 plone.app.querystring-2.0.4/plone/app/querystring/tests/testQueryBuilderModifiers.py
+-rw-r--r--   0 maurits    (501) staff       (20)    21787 2023-05-22 18:01:35.000000 plone.app.querystring-2.0.4/plone/app/querystring/tests/testQueryParser.py
+-rw-r--r--   0 maurits    (501) staff       (20)     2941 2023-05-22 18:01:35.000000 plone.app.querystring-2.0.4/plone/app/querystring/tests/testRegistryIntegration.py
+-rw-r--r--   0 maurits    (501) staff       (20)     5653 2023-05-22 18:01:35.000000 plone.app.querystring-2.0.4/plone/app/querystring/tests/testRegistryReader.py
+-rw-r--r--   0 maurits    (501) staff       (20)      532 2023-05-22 18:01:35.000000 plone.app.querystring-2.0.4/plone/app/querystring/tests/testVocabularies.py
+-rw-r--r--   0 maurits    (501) staff       (20)     2178 2023-05-22 18:01:35.000000 plone.app.querystring-2.0.4/plone/app/querystring/upgrades.py
+-rw-r--r--   0 maurits    (501) staff       (20)     5147 2023-05-22 18:01:35.000000 plone.app.querystring-2.0.4/plone/app/querystring/upgrades.zcml
+-rw-r--r--   0 maurits    (501) staff       (20)     2634 2023-05-22 18:01:35.000000 plone.app.querystring-2.0.4/plone/app/querystring/vocabularies.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-05-22 18:01:36.255751 plone.app.querystring-2.0.4/plone.app.querystring.egg-info/
+-rw-r--r--   0 maurits    (501) staff       (20)    14678 2023-05-22 18:01:36.000000 plone.app.querystring-2.0.4/plone.app.querystring.egg-info/PKG-INFO
+-rw-r--r--   0 maurits    (501) staff       (20)     2665 2023-05-22 18:01:36.000000 plone.app.querystring-2.0.4/plone.app.querystring.egg-info/SOURCES.txt
+-rw-r--r--   0 maurits    (501) staff       (20)        1 2023-05-22 18:01:36.000000 plone.app.querystring-2.0.4/plone.app.querystring.egg-info/dependency_links.txt
+-rw-r--r--   0 maurits    (501) staff       (20)       40 2023-05-22 18:01:36.000000 plone.app.querystring-2.0.4/plone.app.querystring.egg-info/entry_points.txt
+-rw-r--r--   0 maurits    (501) staff       (20)       16 2023-05-22 18:01:36.000000 plone.app.querystring-2.0.4/plone.app.querystring.egg-info/namespace_packages.txt
+-rw-r--r--   0 maurits    (501) staff       (20)        1 2023-05-22 18:01:36.000000 plone.app.querystring-2.0.4/plone.app.querystring.egg-info/not-zip-safe
+-rw-r--r--   0 maurits    (501) staff       (20)      297 2023-05-22 18:01:36.000000 plone.app.querystring-2.0.4/plone.app.querystring.egg-info/requires.txt
+-rw-r--r--   0 maurits    (501) staff       (20)        6 2023-05-22 18:01:36.000000 plone.app.querystring-2.0.4/plone.app.querystring.egg-info/top_level.txt
+-rw-r--r--   0 maurits    (501) staff       (20)     1690 2023-05-22 18:01:35.000000 plone.app.querystring-2.0.4/pyproject.toml
+-rw-r--r--   0 maurits    (501) staff       (20)      217 2023-05-22 18:01:36.269782 plone.app.querystring-2.0.4/setup.cfg
+-rw-r--r--   0 maurits    (501) staff       (20)     1996 2023-05-22 18:01:35.000000 plone.app.querystring-2.0.4/setup.py
```

### Comparing `plone.app.querystring-2.0.3/CHANGES.rst` & `plone.app.querystring-2.0.4/CHANGES.rst`

 * *Files 3% similar despite different names*

```diff
@@ -4,14 +4,27 @@
 .. You should *NOT* be adding new change log entries to this file.
    You should create a file in the news directory instead.
    For helpful instructions, please see:
    https://github.com/plone/plone.releaser/blob/master/ADD-A-NEWS-ITEM.rst
 
 .. towncrier release notes start
 
+2.0.4 (2023-05-22)
+------------------
+
+Bug fixes:
+
+
+- Fix a circular transitive dependency to `plone.app.querystring`.
+  New direct dependency explicit on `plone.app.vocabularies`.
+  Move `plone.app.querystring.catalog.CatalogVocabularyFactory` to `.vocabularies`, move the ZCML to register the factory, move the the test.
+  Move `plone.app.querystring.utils.parse_query` with new name `parseAndModifyFormquery` to `.queryparser`.
+  [@jensens] (fix-circular-dep-pavocabularies)
+
+
 2.0.3 (2023-04-26)
 ------------------
 
 Bug fixes:
 
 
 - Fix cyclic dependency, do not depend on `plone.app.layout`.
```

### Comparing `plone.app.querystring-2.0.3/PKG-INFO` & `plone.app.querystring-2.0.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plone.app.querystring
-Version: 2.0.3
+Version: 2.0.4
 Summary: A queryparser, querybuilder and extra helper tools, to parse stored queries to actual results, used in new style Plone collections
 Home-page: https://github.com/plone/plone.app.querystring
 Author: Plone Foundation
 Author-email: plone-developers@lists.sourceforge.net
 License: GPL version 2
 Keywords: collection queries
 Classifier: Development Status :: 5 - Production/Stable
@@ -59,14 +59,27 @@
 .. You should *NOT* be adding new change log entries to this file.
    You should create a file in the news directory instead.
    For helpful instructions, please see:
    https://github.com/plone/plone.releaser/blob/master/ADD-A-NEWS-ITEM.rst
 
 .. towncrier release notes start
 
+2.0.4 (2023-05-22)
+------------------
+
+Bug fixes:
+
+
+- Fix a circular transitive dependency to `plone.app.querystring`.
+  New direct dependency explicit on `plone.app.vocabularies`.
+  Move `plone.app.querystring.catalog.CatalogVocabularyFactory` to `.vocabularies`, move the ZCML to register the factory, move the the test.
+  Move `plone.app.querystring.utils.parse_query` with new name `parseAndModifyFormquery` to `.queryparser`.
+  [@jensens] (fix-circular-dep-pavocabularies)
+
+
 2.0.3 (2023-04-26)
 ------------------
 
 Bug fixes:
 
 
 - Fix cyclic dependency, do not depend on `plone.app.layout`.
```

### Comparing `plone.app.querystring-2.0.3/README.rst` & `plone.app.querystring-2.0.4/README.rst`

 * *Files identical despite different names*

### Comparing `plone.app.querystring-2.0.3/docs/LICENSE.GPL` & `plone.app.querystring-2.0.4/docs/LICENSE.GPL`

 * *Files identical despite different names*

### Comparing `plone.app.querystring-2.0.3/docs/LICENSE.txt` & `plone.app.querystring-2.0.4/docs/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `plone.app.querystring-2.0.3/plone/app/querystring/configure.zcml` & `plone.app.querystring-2.0.4/plone/app/querystring/configure.zcml`

 * *Files 24% similar despite different names*

```diff
@@ -60,8 +60,12 @@
       class=".querybuilder.RegistryConfiguration"
       permission="zope2.View"
       />
   <utility
       name="1000"
       component=".querymodifiers.modify_query_to_enforce_navigation_root"
       />
+  <utility
+      factory=".vocabularies.CatalogVocabularyFactory"
+      name="plone.app.vocabularies.Catalog"
+      />
 </configure>
```

### Comparing `plone.app.querystring-2.0.3/plone/app/querystring/hiddenprofiles.py` & `plone.app.querystring-2.0.4/plone/app/querystring/hiddenprofiles.py`

 * *Files identical despite different names*

### Comparing `plone.app.querystring-2.0.3/plone/app/querystring/indexmodifiers/configure.zcml` & `plone.app.querystring-2.0.4/plone/app/querystring/indexmodifiers/configure.zcml`

 * *Files identical despite different names*

### Comparing `plone.app.querystring-2.0.3/plone/app/querystring/indexmodifiers/query_index_modifiers.py` & `plone.app.querystring-2.0.4/plone/app/querystring/indexmodifiers/query_index_modifiers.py`

 * *Files identical despite different names*

### Comparing `plone.app.querystring-2.0.3/plone/app/querystring/interfaces.py` & `plone.app.querystring-2.0.4/plone/app/querystring/interfaces.py`

 * *Files identical despite different names*

### Comparing `plone.app.querystring-2.0.3/plone/app/querystring/profiles/default/registry.xml` & `plone.app.querystring-2.0.4/plone/app/querystring/profiles/default/registry.xml`

 * *Files identical despite different names*

### Comparing `plone.app.querystring-2.0.3/plone/app/querystring/profiles/upgrades/to_10/registry.xml` & `plone.app.querystring-2.0.4/plone/app/querystring/profiles/upgrades/to_10/registry.xml`

 * *Files identical despite different names*

### Comparing `plone.app.querystring-2.0.3/plone/app/querystring/profiles/upgrades/to_11/registry.xml` & `plone.app.querystring-2.0.4/plone/app/querystring/profiles/upgrades/to_11/registry.xml`

 * *Files identical despite different names*

### Comparing `plone.app.querystring-2.0.3/plone/app/querystring/profiles/upgrades/to_14/registry.xml` & `plone.app.querystring-2.0.4/plone/app/querystring/profiles/upgrades/to_14/registry.xml`

 * *Files identical despite different names*

### Comparing `plone.app.querystring-2.0.3/plone/app/querystring/profiles/upgrades/to_3/registry.xml` & `plone.app.querystring-2.0.4/plone/app/querystring/profiles/upgrades/to_3/registry.xml`

 * *Files identical despite different names*

### Comparing `plone.app.querystring-2.0.3/plone/app/querystring/profiles/upgrades/to_5/registry.xml` & `plone.app.querystring-2.0.4/plone/app/querystring/profiles/upgrades/to_5/registry.xml`

 * *Files identical despite different names*

### Comparing `plone.app.querystring-2.0.3/plone/app/querystring/profiles/upgrades/to_6/registry.xml` & `plone.app.querystring-2.0.4/plone/app/querystring/profiles/upgrades/to_6/registry.xml`

 * *Files identical despite different names*

### Comparing `plone.app.querystring-2.0.3/plone/app/querystring/profiles/upgrades/to_8/registry.xml` & `plone.app.querystring-2.0.4/plone/app/querystring/profiles/upgrades/to_8/registry.xml`

 * *Files identical despite different names*

### Comparing `plone.app.querystring-2.0.3/plone/app/querystring/profiles/upgrades/to_9/registry.xml` & `plone.app.querystring-2.0.4/plone/app/querystring/profiles/upgrades/to_9/registry.xml`

 * *Files identical despite different names*

### Comparing `plone.app.querystring-2.0.3/plone/app/querystring/profiles.zcml` & `plone.app.querystring-2.0.4/plone/app/querystring/profiles.zcml`

 * *Files identical despite different names*

### Comparing `plone.app.querystring-2.0.3/plone/app/querystring/querybuilder.py` & `plone.app.querystring-2.0.4/plone/app/querystring/querybuilder.py`

 * *Files identical despite different names*

### Comparing `plone.app.querystring-2.0.3/plone/app/querystring/querymodifiers.py` & `plone.app.querystring-2.0.4/plone/app/querystring/querymodifiers.py`

 * *Files identical despite different names*

### Comparing `plone.app.querystring-2.0.3/plone/app/querystring/queryparser.py` & `plone.app.querystring-2.0.4/plone/app/querystring/queryparser.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,17 +1,19 @@
+from .interfaces import IParsedQueryIndexModifier
 from Acquisition import aq_parent
 from collections import namedtuple
 from DateTime import DateTime
 from DateTime.interfaces import DateTimeError
 from plone.base.interfaces import IPloneSiteRoot
 from plone.base.navigationroot import get_navigation_root
 from plone.base.utils import base_hasattr
 from plone.registry.interfaces import IRegistry
 from plone.uuid.interfaces import IUUID
 from Products.CMFCore.utils import getToolByName
+from zope.component import getUtilitiesFor
 from zope.component import getUtility
 from zope.dottedname.resolve import resolve
 
 
 Row = namedtuple("Row", ["index", "operator", "values"])
 PATH_INDICES = {"path"}
 
@@ -63,14 +65,31 @@
         if sort_on in catalog.indexes():
             query["sort_on"] = sort_on
             if sort_order:
                 query["sort_order"] = sort_order
     return query
 
 
+def parseAndModifyFormquery(context, query, sort_on=None, sort_order=None):
+    parsedquery = parseFormquery(context, query, sort_on, sort_order)
+
+    index_modifiers = getUtilitiesFor(IParsedQueryIndexModifier)
+    for name, modifier in index_modifiers:
+        if name in parsedquery:
+            new_name, query = modifier(parsedquery[name])
+            parsedquery[name] = query
+            # if a new index name has been returned, we need to replace
+            # the native ones
+            if name != new_name:
+                del parsedquery[name]
+                parsedquery[new_name] = query
+
+    return parsedquery
+
+
 # Query operators
 
 
 def _contains(context, row):
     return _equal(context, row)
```

### Comparing `plone.app.querystring-2.0.3/plone/app/querystring/registryreader.py` & `plone.app.querystring-2.0.4/plone/app/querystring/registryreader.py`

 * *Files identical despite different names*

### Comparing `plone.app.querystring-2.0.3/plone/app/querystring/results.pt` & `plone.app.querystring-2.0.4/plone/app/querystring/results.pt`

 * *Files identical despite different names*

### Comparing `plone.app.querystring-2.0.3/plone/app/querystring/testing.py` & `plone.app.querystring-2.0.4/plone/app/querystring/testing.py`

 * *Files identical despite different names*

### Comparing `plone.app.querystring-2.0.3/plone/app/querystring/tests/index_testmodifier.py` & `plone.app.querystring-2.0.4/plone/app/querystring/tests/index_testmodifier.py`

 * *Files identical despite different names*

### Comparing `plone.app.querystring-2.0.3/plone/app/querystring/tests/profiles/registry/registry.xml` & `plone.app.querystring-2.0.4/plone/app/querystring/tests/profiles/registry/registry.xml`

 * *Files identical despite different names*

### Comparing `plone.app.querystring-2.0.3/plone/app/querystring/tests/registry_minimal_correct.xml` & `plone.app.querystring-2.0.4/plone/app/querystring/tests/registry_minimal_correct.xml`

 * *Files identical despite different names*

### Comparing `plone.app.querystring-2.0.3/plone/app/querystring/tests/registry_test_missing_operator.xml` & `plone.app.querystring-2.0.4/plone/app/querystring/tests/registry_test_missing_operator.xml`

 * *Files identical despite different names*

### Comparing `plone.app.querystring-2.0.3/plone/app/querystring/tests/registry_test_vocabulary.xml` & `plone.app.querystring-2.0.4/plone/app/querystring/tests/registry_test_vocabulary.xml`

 * *Files identical despite different names*

### Comparing `plone.app.querystring-2.0.3/plone/app/querystring/tests/registry_testdata.py` & `plone.app.querystring-2.0.4/plone/app/querystring/tests/registry_testdata.py`

 * *Files identical despite different names*

### Comparing `plone.app.querystring-2.0.3/plone/app/querystring/tests/testIndexmodifiers.py` & `plone.app.querystring-2.0.4/plone/app/querystring/tests/testIndexmodifiers.py`

 * *Files identical despite different names*

### Comparing `plone.app.querystring-2.0.3/plone/app/querystring/tests/testQueryBuilder.py` & `plone.app.querystring-2.0.4/plone/app/querystring/tests/testQueryBuilder.py`

 * *Files identical despite different names*

### Comparing `plone.app.querystring-2.0.3/plone/app/querystring/tests/testQueryBuilderModifiers.py` & `plone.app.querystring-2.0.4/plone/app/querystring/tests/testQueryBuilderModifiers.py`

 * *Files identical despite different names*

### Comparing `plone.app.querystring-2.0.3/plone/app/querystring/tests/testQueryParser.py` & `plone.app.querystring-2.0.4/plone/app/querystring/tests/testQueryParser.py`

 * *Files identical despite different names*

### Comparing `plone.app.querystring-2.0.3/plone/app/querystring/tests/testRegistryIntegration.py` & `plone.app.querystring-2.0.4/plone/app/querystring/tests/testRegistryIntegration.py`

 * *Files identical despite different names*

### Comparing `plone.app.querystring-2.0.3/plone/app/querystring/tests/testRegistryReader.py` & `plone.app.querystring-2.0.4/plone/app/querystring/tests/testRegistryReader.py`

 * *Files identical despite different names*

### Comparing `plone.app.querystring-2.0.3/plone/app/querystring/upgrades.py` & `plone.app.querystring-2.0.4/plone/app/querystring/upgrades.py`

 * *Files identical despite different names*

### Comparing `plone.app.querystring-2.0.3/plone/app/querystring/upgrades.zcml` & `plone.app.querystring-2.0.4/plone/app/querystring/upgrades.zcml`

 * *Files identical despite different names*

### Comparing `plone.app.querystring-2.0.3/plone.app.querystring.egg-info/PKG-INFO` & `plone.app.querystring-2.0.4/plone.app.querystring.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plone.app.querystring
-Version: 2.0.3
+Version: 2.0.4
 Summary: A queryparser, querybuilder and extra helper tools, to parse stored queries to actual results, used in new style Plone collections
 Home-page: https://github.com/plone/plone.app.querystring
 Author: Plone Foundation
 Author-email: plone-developers@lists.sourceforge.net
 License: GPL version 2
 Keywords: collection queries
 Classifier: Development Status :: 5 - Production/Stable
@@ -59,14 +59,27 @@
 .. You should *NOT* be adding new change log entries to this file.
    You should create a file in the news directory instead.
    For helpful instructions, please see:
    https://github.com/plone/plone.releaser/blob/master/ADD-A-NEWS-ITEM.rst
 
 .. towncrier release notes start
 
+2.0.4 (2023-05-22)
+------------------
+
+Bug fixes:
+
+
+- Fix a circular transitive dependency to `plone.app.querystring`.
+  New direct dependency explicit on `plone.app.vocabularies`.
+  Move `plone.app.querystring.catalog.CatalogVocabularyFactory` to `.vocabularies`, move the ZCML to register the factory, move the the test.
+  Move `plone.app.querystring.utils.parse_query` with new name `parseAndModifyFormquery` to `.queryparser`.
+  [@jensens] (fix-circular-dep-pavocabularies)
+
+
 2.0.3 (2023-04-26)
 ------------------
 
 Bug fixes:
 
 
 - Fix cyclic dependency, do not depend on `plone.app.layout`.
```

### Comparing `plone.app.querystring-2.0.3/plone.app.querystring.egg-info/SOURCES.txt` & `plone.app.querystring-2.0.4/plone.app.querystring.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -26,14 +26,15 @@
 plone/app/querystring/querymodifiers.py
 plone/app/querystring/queryparser.py
 plone/app/querystring/registryreader.py
 plone/app/querystring/results.pt
 plone/app/querystring/testing.py
 plone/app/querystring/upgrades.py
 plone/app/querystring/upgrades.zcml
+plone/app/querystring/vocabularies.py
 plone/app/querystring/indexmodifiers/__init__.py
 plone/app/querystring/indexmodifiers/configure.zcml
 plone/app/querystring/indexmodifiers/query_index_modifiers.py
 plone/app/querystring/profiles/default/metadata.xml
 plone/app/querystring/profiles/default/registry.xml
 plone/app/querystring/profiles/upgrades/to_10/registry.xml
 plone/app/querystring/profiles/upgrades/to_11/registry.xml
@@ -53,9 +54,10 @@
 plone/app/querystring/tests/registry_testdata.py
 plone/app/querystring/tests/testIndexmodifiers.py
 plone/app/querystring/tests/testQueryBuilder.py
 plone/app/querystring/tests/testQueryBuilderModifiers.py
 plone/app/querystring/tests/testQueryParser.py
 plone/app/querystring/tests/testRegistryIntegration.py
 plone/app/querystring/tests/testRegistryReader.py
+plone/app/querystring/tests/testVocabularies.py
 plone/app/querystring/tests/profiles/registry/metadata.xml
 plone/app/querystring/tests/profiles/registry/registry.xml
```

### Comparing `plone.app.querystring-2.0.3/pyproject.toml` & `plone.app.querystring-2.0.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `plone.app.querystring-2.0.3/setup.py` & `plone.app.querystring-2.0.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import find_packages
 from setuptools import setup
 
 
-version = "2.0.3"
+version = "2.0.4"
 
 long_description = open("README.rst").read() + "\n"
 long_description += open("CHANGES.rst").read()
 
 setup(
     name="plone.app.querystring",
     version=version,
@@ -38,14 +38,15 @@
     include_package_data=True,
     zip_safe=False,
     python_requires=">=3.8",
     install_requires=[
         "setuptools",
         "plone.app.contentlisting",
         "plone.app.registry>=1.1",
+        "plone.app.vocabularies",
         "plone.base",
         "plone.batching",
         "plone.i18n",
         "plone.registry",
         "plone.uuid",
         "Products.GenericSetup",
         "Products.ZCatalog",
```

