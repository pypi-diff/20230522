# Comparing `tmp/hollihop_api_client-0.0.7.tar.gz` & `tmp/hollihop_api_client-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hollihop_api_client-0.0.7.tar", last modified: Fri May 19 13:03:53 2023, max compression
+gzip compressed data, was "hollihop_api_client-0.0.8.tar", last modified: Mon May 22 12:15:17 2023, max compression
```

## Comparing `hollihop_api_client-0.0.7.tar` & `hollihop_api_client-0.0.8.tar`

### file list

```diff
@@ -1,56 +1,61 @@
-drwxr-xr-x   0 malts.tech   (501) staff       (20)        0 2023-05-19 13:03:53.556903 hollihop_api_client-0.0.7/
--rw-r--r--   0 malts.tech   (501) staff       (20)     1073 2023-05-18 10:42:19.000000 hollihop_api_client-0.0.7/LICENSE
--rw-r--r--   0 malts.tech   (501) staff       (20)     2401 2023-05-19 13:03:53.556743 hollihop_api_client-0.0.7/PKG-INFO
--rw-r--r--   0 malts.tech   (501) staff       (20)     1753 2023-05-18 10:42:19.000000 hollihop_api_client-0.0.7/README.md
--rw-r--r--   0 malts.tech   (501) staff       (20)      791 2023-05-19 13:03:38.000000 hollihop_api_client-0.0.7/pyproject.toml
--rw-r--r--   0 malts.tech   (501) staff       (20)       38 2023-05-19 13:03:53.556949 hollihop_api_client-0.0.7/setup.cfg
-drwxr-xr-x   0 malts.tech   (501) staff       (20)        0 2023-05-19 13:03:53.551448 hollihop_api_client-0.0.7/src/
-drwxr-xr-x   0 malts.tech   (501) staff       (20)        0 2023-05-19 13:03:53.552456 hollihop_api_client-0.0.7/src/hollihop_api_client/
--rw-r--r--   0 malts.tech   (501) staff       (20)       94 2023-05-18 11:24:48.000000 hollihop_api_client-0.0.7/src/hollihop_api_client/__init__.py
-drwxr-xr-x   0 malts.tech   (501) staff       (20)        0 2023-05-19 13:03:53.553364 hollihop_api_client-0.0.7/src/hollihop_api_client/api/
--rw-r--r--   0 malts.tech   (501) staff       (20)      138 2023-05-18 10:42:19.000000 hollihop_api_client-0.0.7/src/hollihop_api_client/api/__init__.py
--rw-r--r--   0 malts.tech   (501) staff       (20)      598 2023-05-19 07:20:27.000000 hollihop_api_client-0.0.7/src/hollihop_api_client/api/abc.py
--rw-r--r--   0 malts.tech   (501) staff       (20)     2542 2023-05-19 07:22:09.000000 hollihop_api_client-0.0.7/src/hollihop_api_client/api/api.py
-drwxr-xr-x   0 malts.tech   (501) staff       (20)        0 2023-05-19 13:03:53.553569 hollihop_api_client-0.0.7/src/hollihop_api_client/base/
--rw-r--r--   0 malts.tech   (501) staff       (20)       63 2023-05-19 06:42:36.000000 hollihop_api_client-0.0.7/src/hollihop_api_client/base/__init__.py
--rw-r--r--   0 malts.tech   (501) staff       (20)      540 2023-05-19 06:42:33.000000 hollihop_api_client-0.0.7/src/hollihop_api_client/base/category.py
--rw-r--r--   0 malts.tech   (501) staff       (20)      936 2023-05-19 07:22:58.000000 hollihop_api_client-0.0.7/src/hollihop_api_client/categories.py
-drwxr-xr-x   0 malts.tech   (501) staff       (20)        0 2023-05-19 13:03:53.554227 hollihop_api_client-0.0.7/src/hollihop_api_client/methods/
--rw-r--r--   0 malts.tech   (501) staff       (20)      315 2023-05-18 12:16:07.000000 hollihop_api_client-0.0.7/src/hollihop_api_client/methods/__init__.py
--rw-r--r--   0 malts.tech   (501) staff       (20)     6845 2023-05-19 07:20:27.000000 hollihop_api_client-0.0.7/src/hollihop_api_client/methods/ed_unit_students.py
--rw-r--r--   0 malts.tech   (501) staff       (20)     6500 2023-05-19 07:20:27.000000 hollihop_api_client-0.0.7/src/hollihop_api_client/methods/ed_units.py
--rw-r--r--   0 malts.tech   (501) staff       (20)     3170 2023-05-19 13:02:35.000000 hollihop_api_client-0.0.7/src/hollihop_api_client/methods/leads.py
--rw-r--r--   0 malts.tech   (501) staff       (20)     1320 2023-05-19 07:20:27.000000 hollihop_api_client-0.0.7/src/hollihop_api_client/methods/locations.py
--rw-r--r--   0 malts.tech   (501) staff       (20)     1628 2023-05-19 07:20:27.000000 hollihop_api_client-0.0.7/src/hollihop_api_client/methods/offices.py
-drwxr-xr-x   0 malts.tech   (501) staff       (20)        0 2023-05-19 13:03:53.554963 hollihop_api_client-0.0.7/src/hollihop_api_client/tests/
--rw-r--r--   0 malts.tech   (501) staff       (20)        0 2023-03-11 10:01:33.000000 hollihop_api_client-0.0.7/src/hollihop_api_client/tests/__init__.py
--rw-r--r--   0 malts.tech   (501) staff       (20)     1527 2023-05-19 07:20:27.000000 hollihop_api_client-0.0.7/src/hollihop_api_client/tests/conftest.py
--rw-r--r--   0 malts.tech   (501) staff       (20)      474 2023-03-12 18:14:57.000000 hollihop_api_client-0.0.7/src/hollihop_api_client/tests/test_ed_unit_students.py
--rw-r--r--   0 malts.tech   (501) staff       (20)      995 2023-03-12 11:19:09.000000 hollihop_api_client-0.0.7/src/hollihop_api_client/tests/test_ed_units.py
--rw-r--r--   0 malts.tech   (501) staff       (20)      165 2023-03-12 11:17:10.000000 hollihop_api_client-0.0.7/src/hollihop_api_client/tests/test_lead.py
--rw-r--r--   0 malts.tech   (501) staff       (20)      374 2023-03-12 11:16:33.000000 hollihop_api_client-0.0.7/src/hollihop_api_client/tests/test_locations.py
--rw-r--r--   0 malts.tech   (501) staff       (20)      636 2023-03-12 11:15:54.000000 hollihop_api_client-0.0.7/src/hollihop_api_client/tests/test_offices.py
-drwxr-xr-x   0 malts.tech   (501) staff       (20)        0 2023-05-19 13:03:53.555072 hollihop_api_client-0.0.7/src/hollihop_api_client/tools/
--rw-r--r--   0 malts.tech   (501) staff       (20)     3142 2023-05-19 07:20:27.000000 hollihop_api_client-0.0.7/src/hollihop_api_client/tools/__init__.py
-drwxr-xr-x   0 malts.tech   (501) staff       (20)        0 2023-05-19 13:03:53.551866 hollihop_api_client-0.0.7/src/hollihop_api_client/venv/
-drwxr-xr-x   0 malts.tech   (501) staff       (20)        0 2023-05-19 13:03:53.556450 hollihop_api_client-0.0.7/src/hollihop_api_client/venv/bin/
--rwxr-xr-x   0 malts.tech   (501) staff       (20)      673 2023-05-18 11:11:38.000000 hollihop_api_client-0.0.7/src/hollihop_api_client/venv/bin/rst2html.py
--rwxr-xr-x   0 malts.tech   (501) staff       (20)      795 2023-05-18 11:11:38.000000 hollihop_api_client-0.0.7/src/hollihop_api_client/venv/bin/rst2html4.py
--rwxr-xr-x   0 malts.tech   (501) staff       (20)     1130 2023-05-18 11:11:38.000000 hollihop_api_client-0.0.7/src/hollihop_api_client/venv/bin/rst2html5.py
--rwxr-xr-x   0 malts.tech   (501) staff       (20)      872 2023-05-18 11:11:38.000000 hollihop_api_client-0.0.7/src/hollihop_api_client/venv/bin/rst2latex.py
--rwxr-xr-x   0 malts.tech   (501) staff       (20)      695 2023-05-18 11:11:38.000000 hollihop_api_client-0.0.7/src/hollihop_api_client/venv/bin/rst2man.py
--rwxr-xr-x   0 malts.tech   (501) staff       (20)      861 2023-05-18 11:11:38.000000 hollihop_api_client-0.0.7/src/hollihop_api_client/venv/bin/rst2odt.py
--rwxr-xr-x   0 malts.tech   (501) staff       (20)      667 2023-05-18 11:11:38.000000 hollihop_api_client-0.0.7/src/hollihop_api_client/venv/bin/rst2odt_prepstyles.py
--rwxr-xr-x   0 malts.tech   (501) staff       (20)      680 2023-05-18 11:11:38.000000 hollihop_api_client-0.0.7/src/hollihop_api_client/venv/bin/rst2pseudoxml.py
--rwxr-xr-x   0 malts.tech   (501) staff       (20)      716 2023-05-18 11:11:38.000000 hollihop_api_client-0.0.7/src/hollihop_api_client/venv/bin/rst2s5.py
--rwxr-xr-x   0 malts.tech   (501) staff       (20)      952 2023-05-18 11:11:38.000000 hollihop_api_client-0.0.7/src/hollihop_api_client/venv/bin/rst2xetex.py
--rwxr-xr-x   0 malts.tech   (501) staff       (20)      681 2023-05-18 11:11:38.000000 hollihop_api_client-0.0.7/src/hollihop_api_client/venv/bin/rst2xml.py
--rwxr-xr-x   0 malts.tech   (501) staff       (20)      749 2023-05-18 11:11:38.000000 hollihop_api_client-0.0.7/src/hollihop_api_client/venv/bin/rstpep2html.py
-drwxr-xr-x   0 malts.tech   (501) staff       (20)        0 2023-05-19 13:03:53.553018 hollihop_api_client-0.0.7/src/hollihop_api_client.egg-info/
--rw-r--r--   0 malts.tech   (501) staff       (20)     2401 2023-05-19 13:03:53.000000 hollihop_api_client-0.0.7/src/hollihop_api_client.egg-info/PKG-INFO
--rw-r--r--   0 malts.tech   (501) staff       (20)     1737 2023-05-19 13:03:53.000000 hollihop_api_client-0.0.7/src/hollihop_api_client.egg-info/SOURCES.txt
--rw-r--r--   0 malts.tech   (501) staff       (20)        1 2023-05-19 13:03:53.000000 hollihop_api_client-0.0.7/src/hollihop_api_client.egg-info/dependency_links.txt
--rw-r--r--   0 malts.tech   (501) staff       (20)       38 2023-05-19 13:03:53.000000 hollihop_api_client-0.0.7/src/hollihop_api_client.egg-info/requires.txt
--rw-r--r--   0 malts.tech   (501) staff       (20)       20 2023-05-19 13:03:53.000000 hollihop_api_client-0.0.7/src/hollihop_api_client.egg-info/top_level.txt
-drwxr-xr-x   0 malts.tech   (501) staff       (20)        0 2023-05-19 13:03:53.556565 hollihop_api_client-0.0.7/tests/
--rw-r--r--   0 malts.tech   (501) staff       (20)      211 2023-05-19 12:52:03.000000 hollihop_api_client-0.0.7/tests/test.py
+drwxr-xr-x   0 malts.tech   (501) staff       (20)        0 2023-05-22 12:15:17.290403 hollihop_api_client-0.0.8/
+-rw-r--r--   0 malts.tech   (501) staff       (20)     1073 2023-05-18 10:42:19.000000 hollihop_api_client-0.0.8/LICENSE
+-rw-r--r--   0 malts.tech   (501) staff       (20)     2401 2023-05-22 12:15:17.290262 hollihop_api_client-0.0.8/PKG-INFO
+-rw-r--r--   0 malts.tech   (501) staff       (20)     1753 2023-05-18 10:42:19.000000 hollihop_api_client-0.0.8/README.md
+-rw-r--r--   0 malts.tech   (501) staff       (20)      791 2023-05-22 12:15:04.000000 hollihop_api_client-0.0.8/pyproject.toml
+-rw-r--r--   0 malts.tech   (501) staff       (20)       38 2023-05-22 12:15:17.290438 hollihop_api_client-0.0.8/setup.cfg
+drwxr-xr-x   0 malts.tech   (501) staff       (20)        0 2023-05-22 12:15:17.284232 hollihop_api_client-0.0.8/src/
+drwxr-xr-x   0 malts.tech   (501) staff       (20)        0 2023-05-22 12:15:17.285412 hollihop_api_client-0.0.8/src/hollihop_api_client/
+-rw-r--r--   0 malts.tech   (501) staff       (20)       94 2023-05-18 11:24:48.000000 hollihop_api_client-0.0.8/src/hollihop_api_client/__init__.py
+drwxr-xr-x   0 malts.tech   (501) staff       (20)        0 2023-05-22 12:15:17.286374 hollihop_api_client-0.0.8/src/hollihop_api_client/api/
+-rw-r--r--   0 malts.tech   (501) staff       (20)      138 2023-05-18 10:42:19.000000 hollihop_api_client-0.0.8/src/hollihop_api_client/api/__init__.py
+-rw-r--r--   0 malts.tech   (501) staff       (20)      598 2023-05-19 07:20:27.000000 hollihop_api_client-0.0.8/src/hollihop_api_client/api/abc.py
+-rw-r--r--   0 malts.tech   (501) staff       (20)     2542 2023-05-19 07:22:09.000000 hollihop_api_client-0.0.8/src/hollihop_api_client/api/api.py
+drwxr-xr-x   0 malts.tech   (501) staff       (20)        0 2023-05-22 12:15:17.286594 hollihop_api_client-0.0.8/src/hollihop_api_client/base/
+-rw-r--r--   0 malts.tech   (501) staff       (20)       63 2023-05-19 06:42:36.000000 hollihop_api_client-0.0.8/src/hollihop_api_client/base/__init__.py
+-rw-r--r--   0 malts.tech   (501) staff       (20)      540 2023-05-19 06:42:33.000000 hollihop_api_client-0.0.8/src/hollihop_api_client/base/category.py
+-rw-r--r--   0 malts.tech   (501) staff       (20)      936 2023-05-19 07:22:58.000000 hollihop_api_client-0.0.8/src/hollihop_api_client/categories.py
+drwxr-xr-x   0 malts.tech   (501) staff       (20)        0 2023-05-22 12:15:17.287314 hollihop_api_client-0.0.8/src/hollihop_api_client/methods/
+-rw-r--r--   0 malts.tech   (501) staff       (20)      315 2023-05-18 12:16:07.000000 hollihop_api_client-0.0.8/src/hollihop_api_client/methods/__init__.py
+-rw-r--r--   0 malts.tech   (501) staff       (20)     6845 2023-05-19 07:20:27.000000 hollihop_api_client-0.0.8/src/hollihop_api_client/methods/ed_unit_students.py
+-rw-r--r--   0 malts.tech   (501) staff       (20)     6757 2023-05-22 10:17:26.000000 hollihop_api_client-0.0.8/src/hollihop_api_client/methods/ed_units.py
+-rw-r--r--   0 malts.tech   (501) staff       (20)     3524 2023-05-22 12:08:18.000000 hollihop_api_client-0.0.8/src/hollihop_api_client/methods/leads.py
+-rw-r--r--   0 malts.tech   (501) staff       (20)     1320 2023-05-19 07:20:27.000000 hollihop_api_client-0.0.8/src/hollihop_api_client/methods/locations.py
+-rw-r--r--   0 malts.tech   (501) staff       (20)     1628 2023-05-19 07:20:27.000000 hollihop_api_client-0.0.8/src/hollihop_api_client/methods/offices.py
+drwxr-xr-x   0 malts.tech   (501) staff       (20)        0 2023-05-22 12:15:17.288059 hollihop_api_client-0.0.8/src/hollihop_api_client/tests/
+-rw-r--r--   0 malts.tech   (501) staff       (20)        0 2023-03-11 10:01:33.000000 hollihop_api_client-0.0.8/src/hollihop_api_client/tests/__init__.py
+-rw-r--r--   0 malts.tech   (501) staff       (20)     1527 2023-05-19 07:20:27.000000 hollihop_api_client-0.0.8/src/hollihop_api_client/tests/conftest.py
+-rw-r--r--   0 malts.tech   (501) staff       (20)      474 2023-03-12 18:14:57.000000 hollihop_api_client-0.0.8/src/hollihop_api_client/tests/test_ed_unit_students.py
+-rw-r--r--   0 malts.tech   (501) staff       (20)      995 2023-03-12 11:19:09.000000 hollihop_api_client-0.0.8/src/hollihop_api_client/tests/test_ed_units.py
+-rw-r--r--   0 malts.tech   (501) staff       (20)      165 2023-03-12 11:17:10.000000 hollihop_api_client-0.0.8/src/hollihop_api_client/tests/test_lead.py
+-rw-r--r--   0 malts.tech   (501) staff       (20)      374 2023-03-12 11:16:33.000000 hollihop_api_client-0.0.8/src/hollihop_api_client/tests/test_locations.py
+-rw-r--r--   0 malts.tech   (501) staff       (20)      636 2023-03-12 11:15:54.000000 hollihop_api_client-0.0.8/src/hollihop_api_client/tests/test_offices.py
+drwxr-xr-x   0 malts.tech   (501) staff       (20)        0 2023-05-22 12:15:17.288170 hollihop_api_client-0.0.8/src/hollihop_api_client/tools/
+-rw-r--r--   0 malts.tech   (501) staff       (20)     3448 2023-05-22 10:02:10.000000 hollihop_api_client-0.0.8/src/hollihop_api_client/tools/__init__.py
+drwxr-xr-x   0 malts.tech   (501) staff       (20)        0 2023-05-22 12:15:17.284641 hollihop_api_client-0.0.8/src/hollihop_api_client/venv/
+drwxr-xr-x   0 malts.tech   (501) staff       (20)        0 2023-05-22 12:15:17.289480 hollihop_api_client-0.0.8/src/hollihop_api_client/venv/bin/
+-rwxr-xr-x   0 malts.tech   (501) staff       (20)      673 2023-05-18 11:11:38.000000 hollihop_api_client-0.0.8/src/hollihop_api_client/venv/bin/rst2html.py
+-rwxr-xr-x   0 malts.tech   (501) staff       (20)      795 2023-05-18 11:11:38.000000 hollihop_api_client-0.0.8/src/hollihop_api_client/venv/bin/rst2html4.py
+-rwxr-xr-x   0 malts.tech   (501) staff       (20)     1130 2023-05-18 11:11:38.000000 hollihop_api_client-0.0.8/src/hollihop_api_client/venv/bin/rst2html5.py
+-rwxr-xr-x   0 malts.tech   (501) staff       (20)      872 2023-05-18 11:11:38.000000 hollihop_api_client-0.0.8/src/hollihop_api_client/venv/bin/rst2latex.py
+-rwxr-xr-x   0 malts.tech   (501) staff       (20)      695 2023-05-18 11:11:38.000000 hollihop_api_client-0.0.8/src/hollihop_api_client/venv/bin/rst2man.py
+-rwxr-xr-x   0 malts.tech   (501) staff       (20)      861 2023-05-18 11:11:38.000000 hollihop_api_client-0.0.8/src/hollihop_api_client/venv/bin/rst2odt.py
+-rwxr-xr-x   0 malts.tech   (501) staff       (20)      667 2023-05-18 11:11:38.000000 hollihop_api_client-0.0.8/src/hollihop_api_client/venv/bin/rst2odt_prepstyles.py
+-rwxr-xr-x   0 malts.tech   (501) staff       (20)      680 2023-05-18 11:11:38.000000 hollihop_api_client-0.0.8/src/hollihop_api_client/venv/bin/rst2pseudoxml.py
+-rwxr-xr-x   0 malts.tech   (501) staff       (20)      716 2023-05-18 11:11:38.000000 hollihop_api_client-0.0.8/src/hollihop_api_client/venv/bin/rst2s5.py
+-rwxr-xr-x   0 malts.tech   (501) staff       (20)      952 2023-05-18 11:11:38.000000 hollihop_api_client-0.0.8/src/hollihop_api_client/venv/bin/rst2xetex.py
+-rwxr-xr-x   0 malts.tech   (501) staff       (20)      681 2023-05-18 11:11:38.000000 hollihop_api_client-0.0.8/src/hollihop_api_client/venv/bin/rst2xml.py
+-rwxr-xr-x   0 malts.tech   (501) staff       (20)      749 2023-05-18 11:11:38.000000 hollihop_api_client-0.0.8/src/hollihop_api_client/venv/bin/rstpep2html.py
+drwxr-xr-x   0 malts.tech   (501) staff       (20)        0 2023-05-22 12:15:17.286035 hollihop_api_client-0.0.8/src/hollihop_api_client.egg-info/
+-rw-r--r--   0 malts.tech   (501) staff       (20)     2401 2023-05-22 12:15:17.000000 hollihop_api_client-0.0.8/src/hollihop_api_client.egg-info/PKG-INFO
+-rw-r--r--   0 malts.tech   (501) staff       (20)     1874 2023-05-22 12:15:17.000000 hollihop_api_client-0.0.8/src/hollihop_api_client.egg-info/SOURCES.txt
+-rw-r--r--   0 malts.tech   (501) staff       (20)        1 2023-05-22 12:15:17.000000 hollihop_api_client-0.0.8/src/hollihop_api_client.egg-info/dependency_links.txt
+-rw-r--r--   0 malts.tech   (501) staff       (20)       38 2023-05-22 12:15:17.000000 hollihop_api_client-0.0.8/src/hollihop_api_client.egg-info/requires.txt
+-rw-r--r--   0 malts.tech   (501) staff       (20)       20 2023-05-22 12:15:17.000000 hollihop_api_client-0.0.8/src/hollihop_api_client.egg-info/top_level.txt
+drwxr-xr-x   0 malts.tech   (501) staff       (20)        0 2023-05-22 12:15:17.290103 hollihop_api_client-0.0.8/tests/
+-rw-r--r--   0 malts.tech   (501) staff       (20)      474 2023-03-12 18:14:57.000000 hollihop_api_client-0.0.8/tests/test_ed_unit_students.py
+-rw-r--r--   0 malts.tech   (501) staff       (20)      995 2023-03-12 11:19:09.000000 hollihop_api_client-0.0.8/tests/test_ed_units.py
+-rw-r--r--   0 malts.tech   (501) staff       (20)      209 2023-05-22 10:24:06.000000 hollihop_api_client-0.0.8/tests/test_ed_units_students.py
+-rw-r--r--   0 malts.tech   (501) staff       (20)      197 2023-05-22 09:43:54.000000 hollihop_api_client-0.0.8/tests/test_lead.py
+-rw-r--r--   0 malts.tech   (501) staff       (20)      374 2023-03-12 11:16:33.000000 hollihop_api_client-0.0.8/tests/test_locations.py
+-rw-r--r--   0 malts.tech   (501) staff       (20)      636 2023-03-12 11:15:54.000000 hollihop_api_client-0.0.8/tests/test_offices.py
```

### Comparing `hollihop_api_client-0.0.7/LICENSE` & `hollihop_api_client-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `hollihop_api_client-0.0.7/PKG-INFO` & `hollihop_api_client-0.0.8/src/hollihop_api_client.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: hollihop_api_client
-Version: 0.0.7
+Name: hollihop-api-client
+Version: 0.0.8
 Summary: This library helps you easily create a python application with Hollihop API
 Author-email: Nicholas Maltseb <nmmaltsev@outlook.com>
 Project-URL: Homepage, https://github.com/nicholasChieftain/hollihop_api_client/
 Project-URL: Bug Tracker, https://github.com/nicholasChieftain/hollihop_api_client/issues
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: MacOS
```

### Comparing `hollihop_api_client-0.0.7/README.md` & `hollihop_api_client-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `hollihop_api_client-0.0.7/pyproject.toml` & `hollihop_api_client-0.0.8/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "hollihop_api_client"
-version = "0.0.7"
+version = "0.0.8"
 authors = [
   { name="Nicholas Maltseb", email="nmmaltsev@outlook.com" },
 ]
 description = "This library helps you easily create a python application with Hollihop API"
 readme = "README.md"
 requires-python = ">=3.10"
 dependencies = [
```

### Comparing `hollihop_api_client-0.0.7/src/hollihop_api_client/api/abc.py` & `hollihop_api_client-0.0.8/src/hollihop_api_client/api/abc.py`

 * *Files identical despite different names*

### Comparing `hollihop_api_client-0.0.7/src/hollihop_api_client/api/api.py` & `hollihop_api_client-0.0.8/src/hollihop_api_client/api/api.py`

 * *Files identical despite different names*

### Comparing `hollihop_api_client-0.0.7/src/hollihop_api_client/base/category.py` & `hollihop_api_client-0.0.8/src/hollihop_api_client/base/category.py`

 * *Files identical despite different names*

### Comparing `hollihop_api_client-0.0.7/src/hollihop_api_client/categories.py` & `hollihop_api_client-0.0.8/src/hollihop_api_client/categories.py`

 * *Files identical despite different names*

### Comparing `hollihop_api_client-0.0.7/src/hollihop_api_client/methods/ed_unit_students.py` & `hollihop_api_client-0.0.8/src/hollihop_api_client/methods/ed_unit_students.py`

 * *Files identical despite different names*

### Comparing `hollihop_api_client-0.0.7/src/hollihop_api_client/methods/ed_units.py` & `hollihop_api_client-0.0.8/src/hollihop_api_client/methods/ed_units.py`

 * *Files 2% similar despite different names*

```diff
@@ -191,14 +191,22 @@
             data=data
         )
 
         response = dict_to_snake(response)
 
         return [EdUnit(**_) for _ in EdUnits(**response).ed_units]
 
+    def get_ed_unit_students(self, student_client_id: int):
+        data = dict_to_camel(self.handle_parameters(locals()))
+
+        response = self.api.request(
+            method='GetEdUnitStudents', http_method='GET', data=data)
+
+        return response
+
     def get_all_ed_units_name(self, **kwargs) -> list[str]:
         ed_units = self.get_ed_units(**kwargs)
         return [ed_unit.name for ed_unit in ed_units]
 
     def get_all_ed_units_id(self, **kwargs) -> list[int]:
         ed_units = self.get_ed_units(**kwargs)
         return [ed_unit.id for ed_unit in ed_units]
```

### Comparing `hollihop_api_client-0.0.7/src/hollihop_api_client/methods/leads.py` & `hollihop_api_client-0.0.8/src/hollihop_api_client/methods/leads.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from dataclasses import dataclass, field
 from datetime import datetime
 from typing import TYPE_CHECKING, Any
 
 from hollihop_api_client.base import BaseCategory
-from hollihop_api_client.tools import dict_to_camel, dict_to_snake
+from hollihop_api_client.tools import dict_to_camel, dict_to_snake, format_phone
+
 
 if TYPE_CHECKING:
     from hollihop_api_client.api import AbstractAPI
 
 
 @dataclass
 class Agent:
@@ -22,14 +23,18 @@
     mobile: str | None = None
     use_mobile_by_system: bool | None = None
     job_or_study_place: str | None = None
     position: str | None = None
     birthday: datetime | None = None
     skype: str | None = None
 
+    def __post_init__(self):
+        if not self.phone is None:
+            self.phone = format_phone(self.phone.replace('+', ''))
+
 
 @dataclass
 class ExtraField:
     name: str | None = None
     value: str | None = None
 
 
@@ -65,14 +70,18 @@
     def __post_init__(self):
         self.name = ' '.join(filter(lambda str_obj: str_obj, [
                              self.last_name, self.first_name, self.middle_name]))
         if self.agents:
             self.agents = [Agent(**_) for _ in self.agents]
         if self.extra_fields:
             self.extra_fields = [ExtraField(**_) for _ in self.extra_fields]
+        if not self.mobile is None:
+            self.mobile = format_phone(self.mobile.replace('+'. ''))
+        if not self.phone is None:
+            self.phone = format_phone(self.phone.replace('+', ''))
 
 
 @dataclass
 class Leads:
     leads: None | list[Lead] = field(default_factory=list)
     now: None | datetime = None
```

### Comparing `hollihop_api_client-0.0.7/src/hollihop_api_client/methods/locations.py` & `hollihop_api_client-0.0.8/src/hollihop_api_client/methods/locations.py`

 * *Files identical despite different names*

### Comparing `hollihop_api_client-0.0.7/src/hollihop_api_client/methods/offices.py` & `hollihop_api_client-0.0.8/src/hollihop_api_client/methods/offices.py`

 * *Files identical despite different names*

### Comparing `hollihop_api_client-0.0.7/src/hollihop_api_client/tests/conftest.py` & `hollihop_api_client-0.0.8/src/hollihop_api_client/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `hollihop_api_client-0.0.7/src/hollihop_api_client/tests/test_ed_units.py` & `hollihop_api_client-0.0.8/src/hollihop_api_client/tests/test_ed_units.py`

 * *Files identical despite different names*

### Comparing `hollihop_api_client-0.0.7/src/hollihop_api_client/tests/test_offices.py` & `hollihop_api_client-0.0.8/src/hollihop_api_client/tests/test_offices.py`

 * *Files identical despite different names*

### Comparing `hollihop_api_client-0.0.7/src/hollihop_api_client/tools/__init__.py` & `hollihop_api_client-0.0.8/src/hollihop_api_client/tools/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,11 @@
+import phonenumbers
 from functools import lru_cache
 from typing import Any
+import logging
 
 keyword_tuple = ('False', 'await', 'else', 'import', 'pass',
                  'None', 'break', 'except', 'in', 'raise',
                  'True', 'class', 'finally', 'is', 'return',
                  'and', 'continue', 'for', 'lambda', 'try',
                  'as', 'def', 'from', 'nonlocal', 'while',
                  'assert', 'del', 'global', 'not', 'with',
@@ -18,17 +20,19 @@
             key = to_camel(k)
         else:
             key = k
 
         if isinstance(v, dict):
             converted[key] = dict_to_camel(v)
         elif isinstance(v, list):
-            converted[key] = [dict_to_camel(x) if isinstance(x, dict) else x for x in v]
+            converted[key] = [dict_to_camel(
+                x) if isinstance(x, dict) else x for x in v]
         elif isinstance(v, tuple):
-            converted[key] = tuple(dict_to_camel(x) if isinstance(x, dict) else x for x in v)
+            converted[key] = tuple(dict_to_camel(
+                x) if isinstance(x, dict) else x for x in v)
         else:
             converted[key] = data[k]
 
     return converted
 
 
 def dict_to_snake(data: dict[Any, Any]) -> dict[Any, Any]:
@@ -43,17 +47,19 @@
                 key = to_snake(k)
         else:
             key = k
 
         if isinstance(v, dict):
             converted[key] = dict_to_snake(v)
         elif isinstance(v, list):
-            converted[key] = [dict_to_snake(x) if isinstance(x, dict) else x for x in v]
+            converted[key] = [dict_to_snake(
+                x) if isinstance(x, dict) else x for x in v]
         elif isinstance(v, tuple):
-            converted[key] = tuple(dict_to_snake(x) if isinstance(x, dict) else x for x in v)
+            converted[key] = tuple(dict_to_snake(
+                x) if isinstance(x, dict) else x for x in v)
         else:
             converted[key] = data[k]
 
     return converted
 
 
 def dict_to_pascal(data: dict[Any, Any]) -> dict[Any, Any]:
@@ -63,17 +69,19 @@
             key = to_pascal(k)
         else:
             key = k
 
         if isinstance(v, dict):
             converted[key] = dict_to_pascal(v)
         elif isinstance(v, list):
-            converted[key] = [dict_to_pascal(x) if isinstance(x, dict) else x for x in v]
+            converted[key] = [dict_to_pascal(
+                x) if isinstance(x, dict) else x for x in v]
         elif isinstance(v, tuple):
-            converted[key] = tuple(dict_to_pascal(x) if isinstance(x, dict) else x for x in v)
+            converted[key] = tuple(dict_to_pascal(
+                x) if isinstance(x, dict) else x for x in v)
         else:
             converted[key] = data[k]
 
     return converted
 
 
 @lru_cache(maxsize=4096)
@@ -93,7 +101,14 @@
     words = _split_snake(snake_string)
 
     return "".join(word.title() for word in words)
 
 
 def _split_snake(snake_string: str) -> list[str]:
     return snake_string.split("_")
+
+
+def format_phone(phone: str) -> str:
+    return phonenumbers.format_number(
+        phonenumbers.parse(phone, 'RU'),
+        phonenumbers.PhoneNumberFormat.E164
+    )
```

### Comparing `hollihop_api_client-0.0.7/src/hollihop_api_client/venv/bin/rst2html.py` & `hollihop_api_client-0.0.8/src/hollihop_api_client/venv/bin/rst2html.py`

 * *Files identical despite different names*

### Comparing `hollihop_api_client-0.0.7/src/hollihop_api_client/venv/bin/rst2html4.py` & `hollihop_api_client-0.0.8/src/hollihop_api_client/venv/bin/rst2html4.py`

 * *Files identical despite different names*

### Comparing `hollihop_api_client-0.0.7/src/hollihop_api_client/venv/bin/rst2html5.py` & `hollihop_api_client-0.0.8/src/hollihop_api_client/venv/bin/rst2html5.py`

 * *Files identical despite different names*

### Comparing `hollihop_api_client-0.0.7/src/hollihop_api_client/venv/bin/rst2latex.py` & `hollihop_api_client-0.0.8/src/hollihop_api_client/venv/bin/rst2latex.py`

 * *Files identical despite different names*

### Comparing `hollihop_api_client-0.0.7/src/hollihop_api_client/venv/bin/rst2man.py` & `hollihop_api_client-0.0.8/src/hollihop_api_client/venv/bin/rst2man.py`

 * *Files identical despite different names*

### Comparing `hollihop_api_client-0.0.7/src/hollihop_api_client/venv/bin/rst2odt.py` & `hollihop_api_client-0.0.8/src/hollihop_api_client/venv/bin/rst2odt.py`

 * *Files identical despite different names*

### Comparing `hollihop_api_client-0.0.7/src/hollihop_api_client/venv/bin/rst2odt_prepstyles.py` & `hollihop_api_client-0.0.8/src/hollihop_api_client/venv/bin/rst2odt_prepstyles.py`

 * *Files identical despite different names*

### Comparing `hollihop_api_client-0.0.7/src/hollihop_api_client/venv/bin/rst2pseudoxml.py` & `hollihop_api_client-0.0.8/src/hollihop_api_client/venv/bin/rst2pseudoxml.py`

 * *Files identical despite different names*

### Comparing `hollihop_api_client-0.0.7/src/hollihop_api_client/venv/bin/rst2s5.py` & `hollihop_api_client-0.0.8/src/hollihop_api_client/venv/bin/rst2s5.py`

 * *Files identical despite different names*

### Comparing `hollihop_api_client-0.0.7/src/hollihop_api_client/venv/bin/rst2xetex.py` & `hollihop_api_client-0.0.8/src/hollihop_api_client/venv/bin/rst2xetex.py`

 * *Files identical despite different names*

### Comparing `hollihop_api_client-0.0.7/src/hollihop_api_client/venv/bin/rst2xml.py` & `hollihop_api_client-0.0.8/src/hollihop_api_client/venv/bin/rst2xml.py`

 * *Files identical despite different names*

### Comparing `hollihop_api_client-0.0.7/src/hollihop_api_client/venv/bin/rstpep2html.py` & `hollihop_api_client-0.0.8/src/hollihop_api_client/venv/bin/rstpep2html.py`

 * *Files identical despite different names*

### Comparing `hollihop_api_client-0.0.7/src/hollihop_api_client.egg-info/PKG-INFO` & `hollihop_api_client-0.0.8/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: hollihop-api-client
-Version: 0.0.7
+Name: hollihop_api_client
+Version: 0.0.8
 Summary: This library helps you easily create a python application with Hollihop API
 Author-email: Nicholas Maltseb <nmmaltsev@outlook.com>
 Project-URL: Homepage, https://github.com/nicholasChieftain/hollihop_api_client/
 Project-URL: Bug Tracker, https://github.com/nicholasChieftain/hollihop_api_client/issues
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: MacOS
```

### Comparing `hollihop_api_client-0.0.7/src/hollihop_api_client.egg-info/SOURCES.txt` & `hollihop_api_client-0.0.8/src/hollihop_api_client.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -35,8 +35,13 @@
 src/hollihop_api_client/venv/bin/rst2odt.py
 src/hollihop_api_client/venv/bin/rst2odt_prepstyles.py
 src/hollihop_api_client/venv/bin/rst2pseudoxml.py
 src/hollihop_api_client/venv/bin/rst2s5.py
 src/hollihop_api_client/venv/bin/rst2xetex.py
 src/hollihop_api_client/venv/bin/rst2xml.py
 src/hollihop_api_client/venv/bin/rstpep2html.py
-tests/test.py
+tests/test_ed_unit_students.py
+tests/test_ed_units.py
+tests/test_ed_units_students.py
+tests/test_lead.py
+tests/test_locations.py
+tests/test_offices.py
```

