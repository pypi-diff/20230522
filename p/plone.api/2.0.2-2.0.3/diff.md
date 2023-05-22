# Comparing `tmp/plone.api-2.0.2.tar.gz` & `tmp/plone.api-2.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "plone.api-2.0.2.tar", last modified: Thu Apr 13 22:55:19 2023, max compression
+gzip compressed data, was "plone.api-2.0.3.tar", last modified: Mon May 22 21:06:19 2023, max compression
```

## Comparing `plone.api-2.0.2.tar` & `plone.api-2.0.3.tar`

### file list

```diff
@@ -1,71 +1,71 @@
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-13 22:55:19.839508 plone.api-2.0.2/
--rw-r--r--   0 maurits    (501) staff       (20)    21316 2023-04-13 22:55:19.000000 plone.api-2.0.2/CHANGES.rst
--rw-r--r--   0 maurits    (501) staff       (20)       73 2023-04-13 22:55:19.000000 plone.api-2.0.2/CONTRIBUTING.rst
--rw-r--r--   0 maurits    (501) staff       (20)      679 2023-04-13 22:55:19.000000 plone.api-2.0.2/LICENSE
--rw-r--r--   0 maurits    (501) staff       (20)      357 2023-04-13 22:55:19.000000 plone.api-2.0.2/MANIFEST.in
--rw-r--r--   0 maurits    (501) staff       (20)    24878 2023-04-13 22:55:19.839653 plone.api-2.0.2/PKG-INFO
--rw-r--r--   0 maurits    (501) staff       (20)     1936 2023-04-13 22:55:19.000000 plone.api-2.0.2/README.md
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-13 22:55:19.825780 plone.api-2.0.2/docs/
--rw-r--r--   0 maurits    (501) staff       (20)     6015 2023-04-13 22:55:19.000000 plone.api-2.0.2/docs/about.md
--rw-r--r--   0 maurits    (501) staff       (20)    13950 2023-04-13 22:55:19.000000 plone.api-2.0.2/docs/content.md
--rw-r--r--   0 maurits    (501) staff       (20)     3311 2023-04-13 22:55:19.000000 plone.api-2.0.2/docs/env.md
--rw-r--r--   0 maurits    (501) staff       (20)     9491 2023-04-13 22:55:19.000000 plone.api-2.0.2/docs/group.md
--rw-r--r--   0 maurits    (501) staff       (20)     2295 2023-04-13 22:55:19.000000 plone.api-2.0.2/docs/index.md
--rw-r--r--   0 maurits    (501) staff       (20)    11162 2023-04-13 22:55:19.000000 plone.api-2.0.2/docs/portal.md
--rw-r--r--   0 maurits    (501) staff       (20)     3936 2023-04-13 22:55:19.000000 plone.api-2.0.2/docs/relation.md
--rw-r--r--   0 maurits    (501) staff       (20)    10599 2023-04-13 22:55:19.000000 plone.api-2.0.2/docs/user.md
--rw-r--r--   0 maurits    (501) staff       (20)      578 2023-04-13 22:55:19.000000 plone.api-2.0.2/pyproject.toml
--rw-r--r--   0 maurits    (501) staff       (20)      654 2023-04-13 22:55:19.840304 plone.api-2.0.2/setup.cfg
--rw-r--r--   0 maurits    (501) staff       (20)     2004 2023-04-13 22:55:19.000000 plone.api-2.0.2/setup.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-13 22:55:19.818556 plone.api-2.0.2/src/
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-13 22:55:19.826110 plone.api-2.0.2/src/plone/
--rw-r--r--   0 maurits    (501) staff       (20)       56 2023-04-13 22:55:19.000000 plone.api-2.0.2/src/plone/__init__.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-13 22:55:19.831939 plone.api-2.0.2/src/plone/api/
--rw-r--r--   0 maurits    (501) staff       (20)      193 2023-04-13 22:55:19.000000 plone.api-2.0.2/src/plone/api/__init__.py
--rw-r--r--   0 maurits    (501) staff       (20)       98 2023-04-13 22:55:19.000000 plone.api-2.0.2/src/plone/api/configure.zcml
--rw-r--r--   0 maurits    (501) staff       (20)    22260 2023-04-13 22:55:19.000000 plone.api-2.0.2/src/plone/api/content.py
--rw-r--r--   0 maurits    (501) staff       (20)     8042 2023-04-13 22:55:19.000000 plone.api-2.0.2/src/plone/api/env.py
--rw-r--r--   0 maurits    (501) staff       (20)     1051 2023-04-13 22:55:19.000000 plone.api-2.0.2/src/plone/api/exc.py
--rw-r--r--   0 maurits    (501) staff       (20)    11142 2023-04-13 22:55:19.000000 plone.api-2.0.2/src/plone/api/group.py
--rw-r--r--   0 maurits    (501) staff       (20)    13908 2023-04-13 22:55:19.000000 plone.api-2.0.2/src/plone/api/portal.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-13 22:55:19.818908 plone.api-2.0.2/src/plone/api/profiles/
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-13 22:55:19.832653 plone.api-2.0.2/src/plone/api/profiles/testfixture/
--rw-r--r--   0 maurits    (501) staff       (20)      229 2023-04-13 22:55:19.000000 plone.api-2.0.2/src/plone/api/profiles/testfixture/metadata.xml
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-13 22:55:19.833123 plone.api-2.0.2/src/plone/api/profiles/testfixture/types/
--rw-r--r--   0 maurits    (501) staff       (20)     1734 2023-04-13 22:55:19.000000 plone.api-2.0.2/src/plone/api/profiles/testfixture/types/Dexterity_Folder.xml
--rw-r--r--   0 maurits    (501) staff       (20)     1722 2023-04-13 22:55:19.000000 plone.api-2.0.2/src/plone/api/profiles/testfixture/types/Dexterity_Item.xml
--rw-r--r--   0 maurits    (501) staff       (20)      210 2023-04-13 22:55:19.000000 plone.api-2.0.2/src/plone/api/profiles/testfixture/types.xml
--rw-r--r--   0 maurits    (501) staff       (20)    11428 2023-04-13 22:55:19.000000 plone.api-2.0.2/src/plone/api/relation.py
--rw-r--r--   0 maurits    (501) staff       (20)      578 2023-04-13 22:55:19.000000 plone.api-2.0.2/src/plone/api/testing.zcml
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-13 22:55:19.836864 plone.api-2.0.2/src/plone/api/tests/
--rw-r--r--   0 maurits    (501) staff       (20)      106 2023-04-13 22:55:19.000000 plone.api-2.0.2/src/plone/api/tests/Dexterity_Folder.xml
--rw-r--r--   0 maurits    (501) staff       (20)      106 2023-04-13 22:55:19.000000 plone.api-2.0.2/src/plone/api/tests/Dexterity_Item.xml
--rw-r--r--   0 maurits    (501) staff       (20)        0 2023-04-13 22:55:19.000000 plone.api-2.0.2/src/plone/api/tests/__init__.py
--rw-r--r--   0 maurits    (501) staff       (20)     1658 2023-04-13 22:55:19.000000 plone.api-2.0.2/src/plone/api/tests/base.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-13 22:55:19.839284 plone.api-2.0.2/src/plone/api/tests/doctests/
--rw-r--r--   0 maurits    (501) staff       (20)     6015 2023-04-13 22:55:19.000000 plone.api-2.0.2/src/plone/api/tests/doctests/about.md
--rw-r--r--   0 maurits    (501) staff       (20)    13950 2023-04-13 22:55:19.000000 plone.api-2.0.2/src/plone/api/tests/doctests/content.md
--rw-r--r--   0 maurits    (501) staff       (20)     3311 2023-04-13 22:55:19.000000 plone.api-2.0.2/src/plone/api/tests/doctests/env.md
--rw-r--r--   0 maurits    (501) staff       (20)     9491 2023-04-13 22:55:19.000000 plone.api-2.0.2/src/plone/api/tests/doctests/group.md
--rw-r--r--   0 maurits    (501) staff       (20)    11162 2023-04-13 22:55:19.000000 plone.api-2.0.2/src/plone/api/tests/doctests/portal.md
--rw-r--r--   0 maurits    (501) staff       (20)     3936 2023-04-13 22:55:19.000000 plone.api-2.0.2/src/plone/api/tests/doctests/relation.md
--rw-r--r--   0 maurits    (501) staff       (20)    10599 2023-04-13 22:55:19.000000 plone.api-2.0.2/src/plone/api/tests/doctests/user.md
--rw-r--r--   0 maurits    (501) staff       (20)    48874 2023-04-13 22:55:19.000000 plone.api-2.0.2/src/plone/api/tests/test_content.py
--rw-r--r--   0 maurits    (501) staff       (20)     3318 2023-04-13 22:55:19.000000 plone.api-2.0.2/src/plone/api/tests/test_doctests.py
--rw-r--r--   0 maurits    (501) staff       (20)    17633 2023-04-13 22:55:19.000000 plone.api-2.0.2/src/plone/api/tests/test_env.py
--rw-r--r--   0 maurits    (501) staff       (20)    26958 2023-04-13 22:55:19.000000 plone.api-2.0.2/src/plone/api/tests/test_group.py
--rw-r--r--   0 maurits    (501) staff       (20)    30938 2023-04-13 22:55:19.000000 plone.api-2.0.2/src/plone/api/tests/test_portal.py
--rw-r--r--   0 maurits    (501) staff       (20)    18992 2023-04-13 22:55:19.000000 plone.api-2.0.2/src/plone/api/tests/test_relation.py
--rw-r--r--   0 maurits    (501) staff       (20)    35670 2023-04-13 22:55:19.000000 plone.api-2.0.2/src/plone/api/tests/test_user.py
--rw-r--r--   0 maurits    (501) staff       (20)     9812 2023-04-13 22:55:19.000000 plone.api-2.0.2/src/plone/api/tests/test_validation.py
--rw-r--r--   0 maurits    (501) staff       (20)    14825 2023-04-13 22:55:19.000000 plone.api-2.0.2/src/plone/api/user.py
--rw-r--r--   0 maurits    (501) staff       (20)     4862 2023-04-13 22:55:19.000000 plone.api-2.0.2/src/plone/api/validation.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-13 22:55:19.828464 plone.api-2.0.2/src/plone.api.egg-info/
--rw-r--r--   0 maurits    (501) staff       (20)    24878 2023-04-13 22:55:19.000000 plone.api-2.0.2/src/plone.api.egg-info/PKG-INFO
--rw-r--r--   0 maurits    (501) staff       (20)     1682 2023-04-13 22:55:19.000000 plone.api-2.0.2/src/plone.api.egg-info/SOURCES.txt
--rw-r--r--   0 maurits    (501) staff       (20)        1 2023-04-13 22:55:19.000000 plone.api-2.0.2/src/plone.api.egg-info/dependency_links.txt
--rw-r--r--   0 maurits    (501) staff       (20)        6 2023-04-13 22:55:19.000000 plone.api-2.0.2/src/plone.api.egg-info/namespace_packages.txt
--rw-r--r--   0 maurits    (501) staff       (20)        1 2023-04-13 22:55:19.000000 plone.api-2.0.2/src/plone.api.egg-info/not-zip-safe
--rw-r--r--   0 maurits    (501) staff       (20)      272 2023-04-13 22:55:19.000000 plone.api-2.0.2/src/plone.api.egg-info/requires.txt
--rw-r--r--   0 maurits    (501) staff       (20)        6 2023-04-13 22:55:19.000000 plone.api-2.0.2/src/plone.api.egg-info/top_level.txt
--rw-r--r--   0 maurits    (501) staff       (20)     3625 2023-04-13 22:55:19.000000 plone.api-2.0.2/tox.ini
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-05-22 21:06:19.108935 plone.api-2.0.3/
+-rw-r--r--   0 maurits    (501) staff       (20)    21507 2023-05-22 21:06:18.000000 plone.api-2.0.3/CHANGES.rst
+-rw-r--r--   0 maurits    (501) staff       (20)       73 2023-05-22 21:06:18.000000 plone.api-2.0.3/CONTRIBUTING.rst
+-rw-r--r--   0 maurits    (501) staff       (20)      679 2023-05-22 21:06:18.000000 plone.api-2.0.3/LICENSE
+-rw-r--r--   0 maurits    (501) staff       (20)      357 2023-05-22 21:06:18.000000 plone.api-2.0.3/MANIFEST.in
+-rw-r--r--   0 maurits    (501) staff       (20)    25069 2023-05-22 21:06:19.109106 plone.api-2.0.3/PKG-INFO
+-rw-r--r--   0 maurits    (501) staff       (20)     1936 2023-05-22 21:06:18.000000 plone.api-2.0.3/README.md
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-05-22 21:06:19.094941 plone.api-2.0.3/docs/
+-rw-r--r--   0 maurits    (501) staff       (20)     6015 2023-05-22 21:06:18.000000 plone.api-2.0.3/docs/about.md
+-rw-r--r--   0 maurits    (501) staff       (20)    13950 2023-05-22 21:06:18.000000 plone.api-2.0.3/docs/content.md
+-rw-r--r--   0 maurits    (501) staff       (20)     3311 2023-05-22 21:06:18.000000 plone.api-2.0.3/docs/env.md
+-rw-r--r--   0 maurits    (501) staff       (20)     9491 2023-05-22 21:06:18.000000 plone.api-2.0.3/docs/group.md
+-rw-r--r--   0 maurits    (501) staff       (20)     2295 2023-05-22 21:06:18.000000 plone.api-2.0.3/docs/index.md
+-rw-r--r--   0 maurits    (501) staff       (20)    11162 2023-05-22 21:06:18.000000 plone.api-2.0.3/docs/portal.md
+-rw-r--r--   0 maurits    (501) staff       (20)     3936 2023-05-22 21:06:18.000000 plone.api-2.0.3/docs/relation.md
+-rw-r--r--   0 maurits    (501) staff       (20)    10599 2023-05-22 21:06:18.000000 plone.api-2.0.3/docs/user.md
+-rw-r--r--   0 maurits    (501) staff       (20)      578 2023-05-22 21:06:18.000000 plone.api-2.0.3/pyproject.toml
+-rw-r--r--   0 maurits    (501) staff       (20)      654 2023-05-22 21:06:19.109688 plone.api-2.0.3/setup.cfg
+-rw-r--r--   0 maurits    (501) staff       (20)     2004 2023-05-22 21:06:18.000000 plone.api-2.0.3/setup.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-05-22 21:06:19.088947 plone.api-2.0.3/src/
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-05-22 21:06:19.095268 plone.api-2.0.3/src/plone/
+-rw-r--r--   0 maurits    (501) staff       (20)       56 2023-05-22 21:06:18.000000 plone.api-2.0.3/src/plone/__init__.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-05-22 21:06:19.101673 plone.api-2.0.3/src/plone/api/
+-rw-r--r--   0 maurits    (501) staff       (20)      193 2023-05-22 21:06:18.000000 plone.api-2.0.3/src/plone/api/__init__.py
+-rw-r--r--   0 maurits    (501) staff       (20)       98 2023-05-22 21:06:18.000000 plone.api-2.0.3/src/plone/api/configure.zcml
+-rw-r--r--   0 maurits    (501) staff       (20)    22260 2023-05-22 21:06:18.000000 plone.api-2.0.3/src/plone/api/content.py
+-rw-r--r--   0 maurits    (501) staff       (20)     8042 2023-05-22 21:06:18.000000 plone.api-2.0.3/src/plone/api/env.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1051 2023-05-22 21:06:18.000000 plone.api-2.0.3/src/plone/api/exc.py
+-rw-r--r--   0 maurits    (501) staff       (20)    11142 2023-05-22 21:06:18.000000 plone.api-2.0.3/src/plone/api/group.py
+-rw-r--r--   0 maurits    (501) staff       (20)    13908 2023-05-22 21:06:18.000000 plone.api-2.0.3/src/plone/api/portal.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-05-22 21:06:19.089301 plone.api-2.0.3/src/plone/api/profiles/
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-05-22 21:06:19.102528 plone.api-2.0.3/src/plone/api/profiles/testfixture/
+-rw-r--r--   0 maurits    (501) staff       (20)      229 2023-05-22 21:06:18.000000 plone.api-2.0.3/src/plone/api/profiles/testfixture/metadata.xml
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-05-22 21:06:19.103026 plone.api-2.0.3/src/plone/api/profiles/testfixture/types/
+-rw-r--r--   0 maurits    (501) staff       (20)     1734 2023-05-22 21:06:18.000000 plone.api-2.0.3/src/plone/api/profiles/testfixture/types/Dexterity_Folder.xml
+-rw-r--r--   0 maurits    (501) staff       (20)     1722 2023-05-22 21:06:18.000000 plone.api-2.0.3/src/plone/api/profiles/testfixture/types/Dexterity_Item.xml
+-rw-r--r--   0 maurits    (501) staff       (20)      210 2023-05-22 21:06:18.000000 plone.api-2.0.3/src/plone/api/profiles/testfixture/types.xml
+-rw-r--r--   0 maurits    (501) staff       (20)    11553 2023-05-22 21:06:18.000000 plone.api-2.0.3/src/plone/api/relation.py
+-rw-r--r--   0 maurits    (501) staff       (20)      578 2023-05-22 21:06:18.000000 plone.api-2.0.3/src/plone/api/testing.zcml
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-05-22 21:06:19.106701 plone.api-2.0.3/src/plone/api/tests/
+-rw-r--r--   0 maurits    (501) staff       (20)      106 2023-05-22 21:06:18.000000 plone.api-2.0.3/src/plone/api/tests/Dexterity_Folder.xml
+-rw-r--r--   0 maurits    (501) staff       (20)      106 2023-05-22 21:06:18.000000 plone.api-2.0.3/src/plone/api/tests/Dexterity_Item.xml
+-rw-r--r--   0 maurits    (501) staff       (20)        0 2023-05-22 21:06:18.000000 plone.api-2.0.3/src/plone/api/tests/__init__.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1658 2023-05-22 21:06:18.000000 plone.api-2.0.3/src/plone/api/tests/base.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-05-22 21:06:19.108596 plone.api-2.0.3/src/plone/api/tests/doctests/
+-rw-r--r--   0 maurits    (501) staff       (20)     6015 2023-05-22 21:06:18.000000 plone.api-2.0.3/src/plone/api/tests/doctests/about.md
+-rw-r--r--   0 maurits    (501) staff       (20)    13950 2023-05-22 21:06:18.000000 plone.api-2.0.3/src/plone/api/tests/doctests/content.md
+-rw-r--r--   0 maurits    (501) staff       (20)     3311 2023-05-22 21:06:18.000000 plone.api-2.0.3/src/plone/api/tests/doctests/env.md
+-rw-r--r--   0 maurits    (501) staff       (20)     9491 2023-05-22 21:06:18.000000 plone.api-2.0.3/src/plone/api/tests/doctests/group.md
+-rw-r--r--   0 maurits    (501) staff       (20)    11162 2023-05-22 21:06:18.000000 plone.api-2.0.3/src/plone/api/tests/doctests/portal.md
+-rw-r--r--   0 maurits    (501) staff       (20)     3936 2023-05-22 21:06:18.000000 plone.api-2.0.3/src/plone/api/tests/doctests/relation.md
+-rw-r--r--   0 maurits    (501) staff       (20)    10599 2023-05-22 21:06:18.000000 plone.api-2.0.3/src/plone/api/tests/doctests/user.md
+-rw-r--r--   0 maurits    (501) staff       (20)    48874 2023-05-22 21:06:18.000000 plone.api-2.0.3/src/plone/api/tests/test_content.py
+-rw-r--r--   0 maurits    (501) staff       (20)     3318 2023-05-22 21:06:18.000000 plone.api-2.0.3/src/plone/api/tests/test_doctests.py
+-rw-r--r--   0 maurits    (501) staff       (20)    17633 2023-05-22 21:06:18.000000 plone.api-2.0.3/src/plone/api/tests/test_env.py
+-rw-r--r--   0 maurits    (501) staff       (20)    26958 2023-05-22 21:06:18.000000 plone.api-2.0.3/src/plone/api/tests/test_group.py
+-rw-r--r--   0 maurits    (501) staff       (20)    30938 2023-05-22 21:06:18.000000 plone.api-2.0.3/src/plone/api/tests/test_portal.py
+-rw-r--r--   0 maurits    (501) staff       (20)    18992 2023-05-22 21:06:18.000000 plone.api-2.0.3/src/plone/api/tests/test_relation.py
+-rw-r--r--   0 maurits    (501) staff       (20)    35670 2023-05-22 21:06:18.000000 plone.api-2.0.3/src/plone/api/tests/test_user.py
+-rw-r--r--   0 maurits    (501) staff       (20)     9812 2023-05-22 21:06:18.000000 plone.api-2.0.3/src/plone/api/tests/test_validation.py
+-rw-r--r--   0 maurits    (501) staff       (20)    14825 2023-05-22 21:06:18.000000 plone.api-2.0.3/src/plone/api/user.py
+-rw-r--r--   0 maurits    (501) staff       (20)     4862 2023-05-22 21:06:18.000000 plone.api-2.0.3/src/plone/api/validation.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-05-22 21:06:19.097850 plone.api-2.0.3/src/plone.api.egg-info/
+-rw-r--r--   0 maurits    (501) staff       (20)    25069 2023-05-22 21:06:18.000000 plone.api-2.0.3/src/plone.api.egg-info/PKG-INFO
+-rw-r--r--   0 maurits    (501) staff       (20)     1682 2023-05-22 21:06:19.000000 plone.api-2.0.3/src/plone.api.egg-info/SOURCES.txt
+-rw-r--r--   0 maurits    (501) staff       (20)        1 2023-05-22 21:06:18.000000 plone.api-2.0.3/src/plone.api.egg-info/dependency_links.txt
+-rw-r--r--   0 maurits    (501) staff       (20)        6 2023-05-22 21:06:18.000000 plone.api-2.0.3/src/plone.api.egg-info/namespace_packages.txt
+-rw-r--r--   0 maurits    (501) staff       (20)        1 2023-05-22 21:06:18.000000 plone.api-2.0.3/src/plone.api.egg-info/not-zip-safe
+-rw-r--r--   0 maurits    (501) staff       (20)      272 2023-05-22 21:06:18.000000 plone.api-2.0.3/src/plone.api.egg-info/requires.txt
+-rw-r--r--   0 maurits    (501) staff       (20)        6 2023-05-22 21:06:18.000000 plone.api-2.0.3/src/plone.api.egg-info/top_level.txt
+-rw-r--r--   0 maurits    (501) staff       (20)     3625 2023-05-22 21:06:18.000000 plone.api-2.0.3/tox.ini
```

### Comparing `plone.api-2.0.2/CHANGES.rst` & `plone.api-2.0.3/CHANGES.rst`

 * *Files 0% similar despite different names*

```diff
@@ -4,14 +4,24 @@
 .. You should *NOT* be adding new change log entries to this file.
    You should create a file in the news directory instead.
    For helpful instructions, please see:
    https://github.com/plone/plone.releaser/blob/master/ADD-A-NEWS-ITEM.rst
 
 .. towncrier release notes start
 
+2.0.3 (2023-05-22)
+------------------
+
+Bug fixes:
+
+
+- Create relation only if there is no existing one with same source, target, relationname.
+  But mark source as modified. @ksuess (#507)
+
+
 2.0.2 (2023-04-14)
 ------------------
 
 Bug fixes:
 
 
 - Fix deletion of relations by relation name. @ksuess (#501)
```

### Comparing `plone.api-2.0.2/LICENSE` & `plone.api-2.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `plone.api-2.0.2/PKG-INFO` & `plone.api-2.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plone.api
-Version: 2.0.2
+Version: 2.0.3
 Summary: A Plone API.
 Home-page: https://github.com/plone/plone.api
 Author: Plone Foundation
 Author-email: plone-developers@lists.sourceforge.net
 License: GPL version 2
 Keywords: plone api
 Platform: Any
@@ -79,14 +79,24 @@
 .. You should *NOT* be adding new change log entries to this file.
    You should create a file in the news directory instead.
    For helpful instructions, please see:
    https://github.com/plone/plone.releaser/blob/master/ADD-A-NEWS-ITEM.rst
 
 .. towncrier release notes start
 
+2.0.3 (2023-05-22)
+------------------
+
+Bug fixes:
+
+
+- Create relation only if there is no existing one with same source, target, relationname.
+  But mark source as modified. @ksuess (#507)
+
+
 2.0.2 (2023-04-14)
 ------------------
 
 Bug fixes:
 
 
 - Fix deletion of relations by relation name. @ksuess (#501)
```

### Comparing `plone.api-2.0.2/README.md` & `plone.api-2.0.3/README.md`

 * *Files identical despite different names*

### Comparing `plone.api-2.0.2/docs/about.md` & `plone.api-2.0.3/docs/about.md`

 * *Files identical despite different names*

### Comparing `plone.api-2.0.2/docs/content.md` & `plone.api-2.0.3/docs/content.md`

 * *Files identical despite different names*

### Comparing `plone.api-2.0.2/docs/env.md` & `plone.api-2.0.3/docs/env.md`

 * *Files identical despite different names*

### Comparing `plone.api-2.0.2/docs/group.md` & `plone.api-2.0.3/docs/group.md`

 * *Files identical despite different names*

### Comparing `plone.api-2.0.2/docs/index.md` & `plone.api-2.0.3/docs/index.md`

 * *Files identical despite different names*

### Comparing `plone.api-2.0.2/docs/portal.md` & `plone.api-2.0.3/docs/portal.md`

 * *Files identical despite different names*

### Comparing `plone.api-2.0.2/docs/relation.md` & `plone.api-2.0.3/docs/relation.md`

 * *Files identical despite different names*

### Comparing `plone.api-2.0.2/docs/user.md` & `plone.api-2.0.3/docs/user.md`

 * *Files identical despite different names*

### Comparing `plone.api-2.0.2/pyproject.toml` & `plone.api-2.0.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `plone.api-2.0.2/setup.cfg` & `plone.api-2.0.3/setup.cfg`

 * *Files identical despite different names*

### Comparing `plone.api-2.0.2/setup.py` & `plone.api-2.0.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     return open(os.path.join(os.path.dirname(__file__), *rnames)).read()
 
 
 long_description = (
     read("README.md") + "\n\n" + read("CHANGES.rst") + "\n\n" + read("LICENSE")
 )
 
-version = "2.0.2"
+version = "2.0.3"
 
 setup(
     name="plone.api",
     version=version,
     description="A Plone API.",
     long_description=long_description,
     author="Plone Foundation",
```

### Comparing `plone.api-2.0.2/src/plone/api/content.py` & `plone.api-2.0.3/src/plone/api/content.py`

 * *Files identical despite different names*

### Comparing `plone.api-2.0.2/src/plone/api/env.py` & `plone.api-2.0.3/src/plone/api/env.py`

 * *Files identical despite different names*

### Comparing `plone.api-2.0.2/src/plone/api/exc.py` & `plone.api-2.0.3/src/plone/api/exc.py`

 * *Files identical despite different names*

### Comparing `plone.api-2.0.2/src/plone/api/group.py` & `plone.api-2.0.3/src/plone/api/group.py`

 * *Files identical despite different names*

### Comparing `plone.api-2.0.2/src/plone/api/portal.py` & `plone.api-2.0.3/src/plone/api/portal.py`

 * *Files identical despite different names*

### Comparing `plone.api-2.0.2/src/plone/api/profiles/testfixture/types/Dexterity_Folder.xml` & `plone.api-2.0.3/src/plone/api/profiles/testfixture/types/Dexterity_Folder.xml`

 * *Files identical despite different names*

### Comparing `plone.api-2.0.2/src/plone/api/profiles/testfixture/types/Dexterity_Item.xml` & `plone.api-2.0.3/src/plone/api/profiles/testfixture/types/Dexterity_Item.xml`

 * *Files identical despite different names*

### Comparing `plone.api-2.0.2/src/plone/api/relation.py` & `plone.api-2.0.3/src/plone/api/relation.py`

 * *Files 1% similar despite different names*

```diff
@@ -166,16 +166,19 @@
     # Check if there is exactly this relation.
     # If so remove it and create a fresh one.
     query = {
         "from_attribute": from_attribute,
         "from_id": from_id,
         "to_id": to_id,
     }
-    for rel in relation_catalog.findRelations(query):
-        relation_catalog.unindex(rel)
+    has_relation = (
+        False
+        if (len([el for el in relation_catalog.findRelations(query)]) == 0)
+        else True
+    )
 
     if from_attribute == referencedRelationship:
         # Don't mess with linkintegrity-relations!
         # Refresh them by triggering this subscriber.
         modifiedContent(source, None)
         return
 
@@ -208,29 +211,31 @@
     if isinstance(field, RelationList):
         logger.info(
             "Add relation to relationlist %s from %s to %s",
             from_attribute,
             source.absolute_url(),
             target.absolute_url(),
         )
-        existing_relations = getattr(source, from_attribute, [])
-        existing_relations.append(RelationValue(to_id))
-        setattr(source, from_attribute, existing_relations)
-        modified(source)
+        if not has_relation:
+            existing_relations = getattr(source, from_attribute, [])
+            existing_relations.append(RelationValue(to_id))
+            setattr(source, from_attribute, existing_relations)
+            modified(source)
         return
 
     elif isinstance(field, (Relation, RelationChoice)):
         logger.info(
             "Add relation %s from %s to %s",
             from_attribute,
             source.absolute_url(),
             target.absolute_url(),
         )
-        setattr(source, from_attribute, RelationValue(to_id))
-        modified(source)
+        if not has_relation:
+            setattr(source, from_attribute, RelationValue(to_id))
+            modified(source)
         return
 
     # If we end up here, someone is making a relationship that
     # has the same name as a non-relation field.
     # This can be harmless coincidence, and this could be an error,
     # indicating that the field is of the wrong type.
     # Let's create the relationship and log a warning.
```

### Comparing `plone.api-2.0.2/src/plone/api/testing.zcml` & `plone.api-2.0.3/src/plone/api/testing.zcml`

 * *Files identical despite different names*

### Comparing `plone.api-2.0.2/src/plone/api/tests/base.py` & `plone.api-2.0.3/src/plone/api/tests/base.py`

 * *Files identical despite different names*

### Comparing `plone.api-2.0.2/src/plone/api/tests/doctests/about.md` & `plone.api-2.0.3/src/plone/api/tests/doctests/about.md`

 * *Files identical despite different names*

### Comparing `plone.api-2.0.2/src/plone/api/tests/doctests/content.md` & `plone.api-2.0.3/src/plone/api/tests/doctests/content.md`

 * *Files identical despite different names*

### Comparing `plone.api-2.0.2/src/plone/api/tests/doctests/env.md` & `plone.api-2.0.3/src/plone/api/tests/doctests/env.md`

 * *Files identical despite different names*

### Comparing `plone.api-2.0.2/src/plone/api/tests/doctests/group.md` & `plone.api-2.0.3/src/plone/api/tests/doctests/group.md`

 * *Files identical despite different names*

### Comparing `plone.api-2.0.2/src/plone/api/tests/doctests/portal.md` & `plone.api-2.0.3/src/plone/api/tests/doctests/portal.md`

 * *Files identical despite different names*

### Comparing `plone.api-2.0.2/src/plone/api/tests/doctests/relation.md` & `plone.api-2.0.3/src/plone/api/tests/doctests/relation.md`

 * *Files identical despite different names*

### Comparing `plone.api-2.0.2/src/plone/api/tests/doctests/user.md` & `plone.api-2.0.3/src/plone/api/tests/doctests/user.md`

 * *Files identical despite different names*

### Comparing `plone.api-2.0.2/src/plone/api/tests/test_content.py` & `plone.api-2.0.3/src/plone/api/tests/test_content.py`

 * *Files identical despite different names*

### Comparing `plone.api-2.0.2/src/plone/api/tests/test_doctests.py` & `plone.api-2.0.3/src/plone/api/tests/test_doctests.py`

 * *Files identical despite different names*

### Comparing `plone.api-2.0.2/src/plone/api/tests/test_env.py` & `plone.api-2.0.3/src/plone/api/tests/test_env.py`

 * *Files identical despite different names*

### Comparing `plone.api-2.0.2/src/plone/api/tests/test_group.py` & `plone.api-2.0.3/src/plone/api/tests/test_group.py`

 * *Files identical despite different names*

### Comparing `plone.api-2.0.2/src/plone/api/tests/test_portal.py` & `plone.api-2.0.3/src/plone/api/tests/test_portal.py`

 * *Files identical despite different names*

### Comparing `plone.api-2.0.2/src/plone/api/tests/test_relation.py` & `plone.api-2.0.3/src/plone/api/tests/test_relation.py`

 * *Files identical despite different names*

### Comparing `plone.api-2.0.2/src/plone/api/tests/test_user.py` & `plone.api-2.0.3/src/plone/api/tests/test_user.py`

 * *Files identical despite different names*

### Comparing `plone.api-2.0.2/src/plone/api/tests/test_validation.py` & `plone.api-2.0.3/src/plone/api/tests/test_validation.py`

 * *Files identical despite different names*

### Comparing `plone.api-2.0.2/src/plone/api/user.py` & `plone.api-2.0.3/src/plone/api/user.py`

 * *Files identical despite different names*

### Comparing `plone.api-2.0.2/src/plone/api/validation.py` & `plone.api-2.0.3/src/plone/api/validation.py`

 * *Files identical despite different names*

### Comparing `plone.api-2.0.2/src/plone.api.egg-info/PKG-INFO` & `plone.api-2.0.3/src/plone.api.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plone.api
-Version: 2.0.2
+Version: 2.0.3
 Summary: A Plone API.
 Home-page: https://github.com/plone/plone.api
 Author: Plone Foundation
 Author-email: plone-developers@lists.sourceforge.net
 License: GPL version 2
 Keywords: plone api
 Platform: Any
@@ -79,14 +79,24 @@
 .. You should *NOT* be adding new change log entries to this file.
    You should create a file in the news directory instead.
    For helpful instructions, please see:
    https://github.com/plone/plone.releaser/blob/master/ADD-A-NEWS-ITEM.rst
 
 .. towncrier release notes start
 
+2.0.3 (2023-05-22)
+------------------
+
+Bug fixes:
+
+
+- Create relation only if there is no existing one with same source, target, relationname.
+  But mark source as modified. @ksuess (#507)
+
+
 2.0.2 (2023-04-14)
 ------------------
 
 Bug fixes:
 
 
 - Fix deletion of relations by relation name. @ksuess (#501)
```

### Comparing `plone.api-2.0.2/src/plone.api.egg-info/SOURCES.txt` & `plone.api-2.0.3/src/plone.api.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `plone.api-2.0.2/tox.ini` & `plone.api-2.0.3/tox.ini`

 * *Files identical despite different names*

