# Comparing `tmp/astro_ghost-0.2.7.tar.gz` & `tmp/astro_ghost-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "astro_ghost-0.2.7.tar", last modified: Thu May 11 05:43:33 2023, max compression
+gzip compressed data, was "astro_ghost-1.0.0.tar", last modified: Mon May 22 05:31:42 2023, max compression
```

## Comparing `astro_ghost-0.2.7.tar` & `astro_ghost-1.0.0.tar`

### file list

```diff
@@ -1,60 +1,61 @@
-drwxr-xr-x   0 alexgagliano   (501) staff       (20)        0 2023-05-11 05:43:33.928088 astro_ghost-0.2.7/
-drwxr-xr-x   0 alexgagliano   (501) staff       (20)        0 2023-05-11 05:43:33.862445 astro_ghost-0.2.7/.github/
-drwxr-xr-x   0 alexgagliano   (501) staff       (20)        0 2023-05-11 05:43:33.869078 astro_ghost-0.2.7/.github/workflows/
--rw-r--r--   0 alexgagliano   (501) staff       (20)      377 2022-08-10 18:18:27.000000 astro_ghost-0.2.7/.github/workflows/docs.yml
--rw-r--r--   0 alexgagliano   (501) staff       (20)      626 2023-05-09 16:17:11.000000 astro_ghost-0.2.7/.github/workflows/tests.yml
--rw-r--r--   0 alexgagliano   (501) staff       (20)      769 2022-08-10 18:18:27.000000 astro_ghost-0.2.7/.gitignore
--rw-r--r--   0 alexgagliano   (501) staff       (20)      170 2022-08-10 18:18:27.000000 astro_ghost-0.2.7/.readthedocs.yml
--rw-r--r--   0 alexgagliano   (501) staff       (20)      341 2022-08-10 18:18:27.000000 astro_ghost-0.2.7/MANIFEST.in
--rw-r--r--   0 alexgagliano   (501) staff       (20)     4089 2023-05-11 05:43:33.928364 astro_ghost-0.2.7/PKG-INFO
--rw-r--r--   0 alexgagliano   (501) staff       (20)     3488 2023-05-10 20:43:06.000000 astro_ghost-0.2.7/README.rst
-drwxr-xr-x   0 alexgagliano   (501) staff       (20)        0 2023-05-11 05:43:33.903931 astro_ghost-0.2.7/astro_ghost/
--rw-r--r--   0 alexgagliano   (501) staff       (20)    15169 2023-05-11 04:59:00.000000 astro_ghost-0.2.7/astro_ghost/DLR.py
--rw-r--r--   0 alexgagliano   (501) staff       (20)     4668 2023-05-10 23:12:18.000000 astro_ghost-0.2.7/astro_ghost/NEDQueryFunctions.py
--rw-r--r--   0 alexgagliano   (501) staff       (20)    38356 2023-05-11 04:54:25.000000 astro_ghost-0.2.7/astro_ghost/PS1QueryFunctions.py
--rw-r--r--   0 alexgagliano   (501) staff       (20)     1296 2023-05-10 22:09:14.000000 astro_ghost-0.2.7/astro_ghost/SimbadQueryFunctions.py
--rw-r--r--   0 alexgagliano   (501) staff       (20) 13643353 2023-05-08 18:43:43.000000 astro_ghost-0.2.7/astro_ghost/Star_Galaxy_RealisticModel_GHOST_PS1ClassLabels.sav
--rw-r--r--   0 alexgagliano   (501) staff       (20)     1475 2023-05-11 05:34:31.000000 astro_ghost-0.2.7/astro_ghost/TNSQueryFunctions.py
--rw-r--r--   0 alexgagliano   (501) staff       (20)      112 2023-02-17 00:45:54.000000 astro_ghost-0.2.7/astro_ghost/__init__.py
--rw-r--r--   0 alexgagliano   (501) staff       (20)       22 2023-05-11 05:43:06.000000 astro_ghost-0.2.7/astro_ghost/_version.py
--rw-r--r--   0 alexgagliano   (501) staff       (20)     1957 2023-02-17 00:45:54.000000 astro_ghost-0.2.7/astro_ghost/conftest.py
--rw-r--r--   0 alexgagliano   (501) staff       (20)    37898 2023-05-11 05:12:32.000000 astro_ghost-0.2.7/astro_ghost/ghostHelperFunctions.py
--rw-r--r--   0 alexgagliano   (501) staff       (20)    32745 2023-05-10 22:07:36.000000 astro_ghost-0.2.7/astro_ghost/gradientAscent.py
--rw-r--r--   0 alexgagliano   (501) staff       (20)     2838 2023-05-09 20:46:38.000000 astro_ghost-0.2.7/astro_ghost/hostMatching.py
--rw-r--r--   0 alexgagliano   (501) staff       (20)    15960 2023-05-10 22:18:36.000000 astro_ghost-0.2.7/astro_ghost/photoz_helper.py
--rw-r--r--   0 alexgagliano   (501) staff       (20)    10333 2023-05-09 19:38:06.000000 astro_ghost-0.2.7/astro_ghost/sourceCleaning.py
--rw-r--r--   0 alexgagliano   (501) staff       (20)     6519 2023-05-11 05:26:18.000000 astro_ghost-0.2.7/astro_ghost/starSeparation.py
--rw-r--r--   0 alexgagliano   (501) staff       (20)     4611 2023-05-11 04:35:06.000000 astro_ghost-0.2.7/astro_ghost/stellarLocus.py
--rw-r--r--   0 alexgagliano   (501) staff       (20)      302 2023-02-17 00:45:54.000000 astro_ghost-0.2.7/astro_ghost/tonry_ps1_locus.txt
-drwxr-xr-x   0 alexgagliano   (501) staff       (20)        0 2023-05-11 05:43:33.906971 astro_ghost-0.2.7/astro_ghost.egg-info/
--rw-r--r--   0 alexgagliano   (501) staff       (20)     4089 2023-05-11 05:43:33.000000 astro_ghost-0.2.7/astro_ghost.egg-info/PKG-INFO
--rw-r--r--   0 alexgagliano   (501) staff       (20)     1301 2023-05-11 05:43:33.000000 astro_ghost-0.2.7/astro_ghost.egg-info/SOURCES.txt
--rw-r--r--   0 alexgagliano   (501) staff       (20)        1 2023-05-11 05:43:33.000000 astro_ghost-0.2.7/astro_ghost.egg-info/dependency_links.txt
--rw-r--r--   0 alexgagliano   (501) staff       (20)        1 2023-05-11 05:43:33.000000 astro_ghost-0.2.7/astro_ghost.egg-info/not-zip-safe
--rw-r--r--   0 alexgagliano   (501) staff       (20)      368 2023-05-11 05:43:33.000000 astro_ghost-0.2.7/astro_ghost.egg-info/requires.txt
--rw-r--r--   0 alexgagliano   (501) staff       (20)       18 2023-05-11 05:43:33.000000 astro_ghost-0.2.7/astro_ghost.egg-info/top_level.txt
-drwxr-xr-x   0 alexgagliano   (501) staff       (20)        0 2023-05-11 05:43:33.911363 astro_ghost-0.2.7/docs/
--rw-r--r--   0 alexgagliano   (501) staff       (20)      634 2022-08-10 18:18:27.000000 astro_ghost-0.2.7/docs/Makefile
--rw-r--r--   0 alexgagliano   (501) staff       (20)     2545 2023-05-10 05:04:18.000000 astro_ghost-0.2.7/docs/conf.py
--rw-r--r--   0 alexgagliano   (501) staff       (20)     2641 2023-05-10 20:40:49.000000 astro_ghost-0.2.7/docs/index.rst
--rw-r--r--   0 alexgagliano   (501) staff       (20)      760 2022-08-10 18:18:27.000000 astro_ghost-0.2.7/docs/make.bat
-drwxr-xr-x   0 alexgagliano   (501) staff       (20)        0 2023-05-11 05:43:33.921653 astro_ghost-0.2.7/docs/source/
--rw-r--r--   0 alexgagliano   (501) staff       (20)     1402 2023-05-10 20:31:16.000000 astro_ghost-0.2.7/docs/source/associationmodules.rst
--rw-r--r--   0 alexgagliano   (501) staff       (20)     2612 2023-05-10 19:37:56.000000 astro_ghost-0.2.7/docs/source/basicusage.rst
--rw-r--r--   0 alexgagliano   (501) staff       (20)      819 2023-05-10 20:30:40.000000 astro_ghost-0.2.7/docs/source/catalogmodules.rst
--rw-r--r--   0 alexgagliano   (501) staff       (20)      124 2023-05-10 20:18:30.000000 astro_ghost-0.2.7/docs/source/detailedtutorials.rst
--rw-r--r--   0 alexgagliano   (501) staff       (20)      670 2023-05-10 20:33:11.000000 astro_ghost-0.2.7/docs/source/installation.rst
--rw-r--r--   0 alexgagliano   (501) staff       (20)      844 2023-05-10 20:31:25.000000 astro_ghost-0.2.7/docs/source/preprocessingmodules.rst
--rw-r--r--   0 alexgagliano   (501) staff       (20)      320 2023-05-10 20:31:41.000000 astro_ghost-0.2.7/docs/source/supplementalmodules.rst
--rw-r--r--   0 alexgagliano   (501) staff       (20)      268 2023-05-10 20:38:08.000000 astro_ghost-0.2.7/docs/source/wrappermodules.rst
-drwxr-xr-x   0 alexgagliano   (501) staff       (20)        0 2023-05-11 05:43:33.924429 astro_ghost-0.2.7/licenses/
--rw-r--r--   0 alexgagliano   (501) staff       (20)    37573 2022-08-10 18:18:27.000000 astro_ghost-0.2.7/licenses/LICENSE.rst
--rw-r--r--   0 alexgagliano   (501) staff       (20)      372 2022-08-10 18:18:27.000000 astro_ghost-0.2.7/licenses/README.rst
--rw-r--r--   0 alexgagliano   (501) staff       (20)      134 2022-08-10 18:18:27.000000 astro_ghost-0.2.7/pyproject.toml
--rw-r--r--   0 alexgagliano   (501) staff       (20)     1603 2023-05-11 05:43:33.929535 astro_ghost-0.2.7/setup.cfg
--rwxr-xr-x   0 alexgagliano   (501) staff       (20)     1834 2023-05-11 05:42:57.000000 astro_ghost-0.2.7/setup.py
-drwxr-xr-x   0 alexgagliano   (501) staff       (20)        0 2023-05-11 05:43:33.927621 astro_ghost-0.2.7/tests/
--rw-r--r--   0 alexgagliano   (501) staff       (20)      108 2023-02-16 19:42:21.000000 astro_ghost-0.2.7/tests/__init__.py
--rw-r--r--   0 alexgagliano   (501) staff       (20)      560 2023-05-11 05:42:33.000000 astro_ghost-0.2.7/tests/debug.py
--rw-r--r--   0 alexgagliano   (501) staff       (20)     4207 2023-05-11 05:35:01.000000 astro_ghost-0.2.7/tests/test_tutorial.py
--rw-r--r--   0 alexgagliano   (501) staff       (20)     1343 2023-05-10 20:57:05.000000 astro_ghost-0.2.7/tox.ini
+drwxr-xr-x   0 alexgagliano   (501) staff       (20)        0 2023-05-22 05:31:42.527682 astro_ghost-1.0.0/
+drwxr-xr-x   0 alexgagliano   (501) staff       (20)        0 2023-05-22 05:31:42.437688 astro_ghost-1.0.0/.github/
+drwxr-xr-x   0 alexgagliano   (501) staff       (20)        0 2023-05-22 05:31:42.444495 astro_ghost-1.0.0/.github/workflows/
+-rw-r--r--   0 alexgagliano   (501) staff       (20)      377 2022-08-10 18:18:27.000000 astro_ghost-1.0.0/.github/workflows/docs.yml
+-rw-r--r--   0 alexgagliano   (501) staff       (20)      626 2023-05-09 16:17:11.000000 astro_ghost-1.0.0/.github/workflows/tests.yml
+-rw-r--r--   0 alexgagliano   (501) staff       (20)      769 2022-08-10 18:18:27.000000 astro_ghost-1.0.0/.gitignore
+-rw-r--r--   0 alexgagliano   (501) staff       (20)      170 2022-08-10 18:18:27.000000 astro_ghost-1.0.0/.readthedocs.yml
+-rw-r--r--   0 alexgagliano   (501) staff       (20)      341 2022-08-10 18:18:27.000000 astro_ghost-1.0.0/MANIFEST.in
+-rw-r--r--   0 alexgagliano   (501) staff       (20)     4089 2023-05-22 05:31:42.532751 astro_ghost-1.0.0/PKG-INFO
+-rw-r--r--   0 alexgagliano   (501) staff       (20)     3488 2023-05-10 20:43:06.000000 astro_ghost-1.0.0/README.rst
+drwxr-xr-x   0 alexgagliano   (501) staff       (20)        0 2023-05-22 05:31:42.492051 astro_ghost-1.0.0/astro_ghost/
+-rw-r--r--   0 alexgagliano   (501) staff       (20)    14598 2023-05-22 05:20:41.000000 astro_ghost-1.0.0/astro_ghost/DLR.py
+-rw-r--r--   0 alexgagliano   (501) staff       (20)     4668 2023-05-10 23:12:18.000000 astro_ghost-1.0.0/astro_ghost/NEDQueryFunctions.py
+-rw-r--r--   0 alexgagliano   (501) staff       (20)    38679 2023-05-22 03:39:53.000000 astro_ghost-1.0.0/astro_ghost/PS1QueryFunctions.py
+-rw-r--r--   0 alexgagliano   (501) staff       (20)     1296 2023-05-10 22:09:14.000000 astro_ghost-1.0.0/astro_ghost/SimbadQueryFunctions.py
+-rw-r--r--   0 alexgagliano   (501) staff       (20) 13643353 2023-05-08 18:43:43.000000 astro_ghost-1.0.0/astro_ghost/Star_Galaxy_RealisticModel_GHOST_PS1ClassLabels.sav
+-rw-r--r--   0 alexgagliano   (501) staff       (20)     1475 2023-05-11 05:34:31.000000 astro_ghost-1.0.0/astro_ghost/TNSQueryFunctions.py
+-rw-r--r--   0 alexgagliano   (501) staff       (20)      112 2023-02-17 00:45:54.000000 astro_ghost-1.0.0/astro_ghost/__init__.py
+-rw-r--r--   0 alexgagliano   (501) staff       (20)       22 2023-05-22 03:39:53.000000 astro_ghost-1.0.0/astro_ghost/_version.py
+-rw-r--r--   0 alexgagliano   (501) staff       (20)     1957 2023-02-17 00:45:54.000000 astro_ghost-1.0.0/astro_ghost/conftest.py
+-rw-r--r--   0 alexgagliano   (501) staff       (20)    37989 2023-05-22 05:21:18.000000 astro_ghost-1.0.0/astro_ghost/ghostHelperFunctions.py
+-rw-r--r--   0 alexgagliano   (501) staff       (20)    32867 2023-05-22 05:22:39.000000 astro_ghost-1.0.0/astro_ghost/gradientAscent.py
+-rw-r--r--   0 alexgagliano   (501) staff       (20)     2838 2023-05-09 20:46:38.000000 astro_ghost-1.0.0/astro_ghost/hostMatching.py
+-rw-r--r--   0 alexgagliano   (501) staff       (20)    17727 2023-05-22 03:39:53.000000 astro_ghost-1.0.0/astro_ghost/photoz_helper.py
+-rw-r--r--   0 alexgagliano   (501) staff       (20)     9852 2023-05-22 04:36:12.000000 astro_ghost-1.0.0/astro_ghost/sourceCleaning.py
+-rw-r--r--   0 alexgagliano   (501) staff       (20)     7585 2023-05-22 05:17:09.000000 astro_ghost-1.0.0/astro_ghost/starSeparation.py
+-rw-r--r--   0 alexgagliano   (501) staff       (20)     4611 2023-05-11 04:35:06.000000 astro_ghost-1.0.0/astro_ghost/stellarLocus.py
+-rw-r--r--   0 alexgagliano   (501) staff       (20)      302 2023-02-17 00:45:54.000000 astro_ghost-1.0.0/astro_ghost/tonry_ps1_locus.txt
+drwxr-xr-x   0 alexgagliano   (501) staff       (20)        0 2023-05-22 05:31:42.495573 astro_ghost-1.0.0/astro_ghost.egg-info/
+-rw-r--r--   0 alexgagliano   (501) staff       (20)     4089 2023-05-22 05:31:42.000000 astro_ghost-1.0.0/astro_ghost.egg-info/PKG-INFO
+-rw-r--r--   0 alexgagliano   (501) staff       (20)     1318 2023-05-22 05:31:42.000000 astro_ghost-1.0.0/astro_ghost.egg-info/SOURCES.txt
+-rw-r--r--   0 alexgagliano   (501) staff       (20)        1 2023-05-22 05:31:42.000000 astro_ghost-1.0.0/astro_ghost.egg-info/dependency_links.txt
+-rw-r--r--   0 alexgagliano   (501) staff       (20)        1 2023-05-22 05:31:42.000000 astro_ghost-1.0.0/astro_ghost.egg-info/not-zip-safe
+-rw-r--r--   0 alexgagliano   (501) staff       (20)      368 2023-05-22 05:31:42.000000 astro_ghost-1.0.0/astro_ghost.egg-info/requires.txt
+-rw-r--r--   0 alexgagliano   (501) staff       (20)       18 2023-05-22 05:31:42.000000 astro_ghost-1.0.0/astro_ghost.egg-info/top_level.txt
+drwxr-xr-x   0 alexgagliano   (501) staff       (20)        0 2023-05-22 05:31:42.499203 astro_ghost-1.0.0/docs/
+-rw-r--r--   0 alexgagliano   (501) staff       (20)      634 2022-08-10 18:18:27.000000 astro_ghost-1.0.0/docs/Makefile
+-rw-r--r--   0 alexgagliano   (501) staff       (20)     2545 2023-05-10 05:04:18.000000 astro_ghost-1.0.0/docs/conf.py
+-rw-r--r--   0 alexgagliano   (501) staff       (20)     2641 2023-05-10 20:40:49.000000 astro_ghost-1.0.0/docs/index.rst
+-rw-r--r--   0 alexgagliano   (501) staff       (20)      760 2022-08-10 18:18:27.000000 astro_ghost-1.0.0/docs/make.bat
+drwxr-xr-x   0 alexgagliano   (501) staff       (20)        0 2023-05-22 05:31:42.518996 astro_ghost-1.0.0/docs/source/
+-rw-r--r--   0 alexgagliano   (501) staff       (20)     1402 2023-05-10 20:31:16.000000 astro_ghost-1.0.0/docs/source/associationmodules.rst
+-rw-r--r--   0 alexgagliano   (501) staff       (20)     2612 2023-05-10 19:37:56.000000 astro_ghost-1.0.0/docs/source/basicusage.rst
+-rw-r--r--   0 alexgagliano   (501) staff       (20)      819 2023-05-10 20:30:40.000000 astro_ghost-1.0.0/docs/source/catalogmodules.rst
+-rw-r--r--   0 alexgagliano   (501) staff       (20)      124 2023-05-10 20:18:30.000000 astro_ghost-1.0.0/docs/source/detailedtutorials.rst
+-rw-r--r--   0 alexgagliano   (501) staff       (20)      670 2023-05-10 20:33:11.000000 astro_ghost-1.0.0/docs/source/installation.rst
+-rw-r--r--   0 alexgagliano   (501) staff       (20)      844 2023-05-10 20:31:25.000000 astro_ghost-1.0.0/docs/source/preprocessingmodules.rst
+-rw-r--r--   0 alexgagliano   (501) staff       (20)      320 2023-05-10 20:31:41.000000 astro_ghost-1.0.0/docs/source/supplementalmodules.rst
+-rw-r--r--   0 alexgagliano   (501) staff       (20)      268 2023-05-10 20:38:08.000000 astro_ghost-1.0.0/docs/source/wrappermodules.rst
+drwxr-xr-x   0 alexgagliano   (501) staff       (20)        0 2023-05-22 05:31:42.522446 astro_ghost-1.0.0/licenses/
+-rw-r--r--   0 alexgagliano   (501) staff       (20)    37573 2022-08-10 18:18:27.000000 astro_ghost-1.0.0/licenses/LICENSE.rst
+-rw-r--r--   0 alexgagliano   (501) staff       (20)      372 2022-08-10 18:18:27.000000 astro_ghost-1.0.0/licenses/README.rst
+-rw-r--r--   0 alexgagliano   (501) staff       (20)      134 2022-08-10 18:18:27.000000 astro_ghost-1.0.0/pyproject.toml
+-rw-r--r--   0 alexgagliano   (501) staff       (20)     1519 2023-05-22 05:31:42.534234 astro_ghost-1.0.0/setup.cfg
+-rwxr-xr-x   0 alexgagliano   (501) staff       (20)     1834 2023-05-22 05:31:01.000000 astro_ghost-1.0.0/setup.py
+drwxr-xr-x   0 alexgagliano   (501) staff       (20)        0 2023-05-22 05:31:42.526960 astro_ghost-1.0.0/tests/
+-rw-r--r--   0 alexgagliano   (501) staff       (20)      108 2023-02-16 19:42:21.000000 astro_ghost-1.0.0/tests/__init__.py
+-rw-r--r--   0 alexgagliano   (501) staff       (20)      648 2023-05-22 03:39:53.000000 astro_ghost-1.0.0/tests/debug.py
+-rw-r--r--   0 alexgagliano   (501) staff       (20)        0 2023-05-10 21:17:11.000000 astro_ghost-1.0.0/tests/pytest.ini
+-rw-r--r--   0 alexgagliano   (501) staff       (20)     4201 2023-05-22 05:29:50.000000 astro_ghost-1.0.0/tests/test_tutorial.py
+-rw-r--r--   0 alexgagliano   (501) staff       (20)     1343 2023-05-22 03:39:53.000000 astro_ghost-1.0.0/tox.ini
```

### Comparing `astro_ghost-0.2.7/.github/workflows/tests.yml` & `astro_ghost-1.0.0/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `astro_ghost-0.2.7/.gitignore` & `astro_ghost-1.0.0/.gitignore`

 * *Files identical despite different names*

### Comparing `astro_ghost-0.2.7/PKG-INFO` & `astro_ghost-1.0.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: astro_ghost
-Version: 0.2.7
+Version: 1.0.0
 Summary: A package to associate transients with host galaxies, and a database of 16k SNe-host galaxies in PS1.
 Home-page: https://github.com/pypa/sampleproject
 Author: Alex Gagliano
 Author-email: gaglian2@illinois.edu
 License: GNU GPL v3+
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `astro_ghost-0.2.7/README.rst` & `astro_ghost-1.0.0/README.rst`

 * *Files identical despite different names*

### Comparing `astro_ghost-0.2.7/astro_ghost/DLR.py` & `astro_ghost-1.0.0/astro_ghost/DLR.py`

 * *Files 6% similar despite different names*

```diff
@@ -19,23 +19,19 @@
     :param host_df: The dataframe containing the candidate host galaxy (should just be one galaxy).
     :type host_df: Pandas DataFrame
     :return: The PS1 band with the highest S/N.
     :rtype: str
     """
 
     bands = 'grizy'
+    SNR = []
     try:
-        gSNR = float(1/host_df["gPSFMagErr"])
-        rSNR = float(1/host_df["rPSFMagErr"])
-        iSNR = float(1/host_df["iPSFMagErr"])
-        zSNR = float(1/host_df["zPSFMagErr"])
-        ySNR = float(1/host_df["yPSFMagErr"])
-
-        SNR = np.array([gSNR, rSNR, iSNR, zSNR, ySNR])
-        i = np.nanargmax(SNR)
+        for band in bands:
+             SNR.append(float(1/host_df["%sKronMagErr"%band]))
+        i = np.nanargmax(np.array(SNR))
     except:
         #if we have issues getting the band with the highest SNR, just use r-band
         i = 1
     return bands[i]
 
 def calc_DLR(ra_SN, dec_SN, ra_host, dec_host, r_a, r_b, source, best_band):
     """Calculate the directional light radius for a given galaxy and transient pair. Calculation is adapted from
@@ -60,16 +56,16 @@
     :type best_band: str
     :return: The angular separation between galaxy and transient, in arcseconds.
     :rtype: float
     :return: The normalized distance (angular separation divided by the DLR).
     :rtype: float
     """
 
-    xr = np.abs(ra_SN.deg - float(ra_host))*3600
-    yr = np.abs(dec_SN.deg - float(dec_host))*3600
+    xr = (ra_SN.deg - float(ra_host))*3600
+    yr = (dec_SN.deg - float(dec_host))*3600
 
     SNcoord = SkyCoord(ra_SN, dec_SN, frame='icrs')
     hostCoord = SkyCoord(ra_host*u.deg, dec_host*u.deg, frame='icrs')
     sep = SNcoord.separation(hostCoord)
     dist = sep.arcsecond
     badR = 10000000000.0
 
@@ -88,15 +84,16 @@
     if Q == 0:
         return dist, badR
 
     phi = 0.5*np.arctan(U/Q)
     kappa = Q**2 + U**2
     a_over_b = (1 + kappa + 2*np.sqrt(kappa))/(1 - kappa)
 
-    gam = np.arctan(yr/xr)
+    gam = np.arctan2(xr, yr)
+
     theta = phi - gam
 
     DLR = r_a/np.sqrt(((a_over_b)*np.sin(theta))**2 + (np.cos(theta))**2)
 
     R = float(dist/DLR)
 
     if (R != R):
@@ -132,28 +129,29 @@
     :return: The normalized distance (angular separation divided by the DLR).
     :rtype: float
     """
 
     # EVERYTHING IS IN ARCSECONDS
     ## taken from "Understanding Type Ia Supernovae Through Their Host Galaxies..." by Gupta
     #https://repository.upenn.edu/cgi/viewcontent.cgi?referer=https://www.google.com/&httpsredir=1&article=1916&context=edissertations
-    xr = np.abs(ra_SN.deg - float(ra_host))*3600
-    yr = np.abs(dec_SN.deg - float(dec_host))*3600
+    xr = (ra_SN.deg - float(ra_host))*3600
+    yr = (dec_SN.deg - float(dec_host))*3600
 
     SNcoord = SkyCoord(ra_SN, dec_SN, frame='icrs')
     hostCoord = SkyCoord(ra_host*u.deg, dec_host*u.deg, frame='icrs')
     sep = SNcoord.separation(hostCoord)
     dist = sep.arcsecond
     badR = 10000000000.0
 
     # if we don't have shape information for a southern-hemisphere galaxy, return
     if (float(r_a) != float(r_a)) | (float(elong) != float(elong)):
         return dist, badR
 
-    gam = np.arctan(yr/xr)
+    gam = np.arctan2(xr, yr)
+
     theta = phi - gam
 
     #elong == a/b, which allows us to substitute here
     DLR = r_a/np.sqrt(((elong)*np.sin(theta))**2 + (np.cos(theta))**2)
 
     R = float(dist/DLR)
 
@@ -235,53 +233,46 @@
                         dec_SN = Angle(transient_df["DEC"].values, unit=u.degree)
                         ra_host = host_df['raMean']
                         dec_host = host_df['decMean']
                         if len(np.array(ra_SN)) > 1:
                             ra_SN = ra_SN[0]
                             dec_SN = dec_SN[0]
                         if (dec_SN.deg > -30):
-                            #switching from kron radius to petrosian radius (more robust!)
-                            for band in 'gri':
-                                #temp_r_a = float(host_df[band + 'HalfLightRad'].values[0])
-                                try:
-                                    temp_r_a = float(host_df[band + 'petR90'].values[0])
-                                except:
-                                    temp_r_a = np.nan
-                                if (temp_r_a == temp_r_a) & (temp_r_a > 0):
-                                    #r_a = r_b = float(host_df[band + 'HalfLightRad'].values[0])
-                                    r_a = r_b = float(host_df[band + 'petR90'].values[0])
-                                    dist, R = calc_DLR(ra_SN, dec_SN, ra_host, dec_host, r_a, r_b, host_df, band)
-                                    break
+                            band = choose_band_SNR(host_df)
+                            r_a = r_b = float(host_df[band + 'KronRad'].values[0])
+                            dist, R = calc_DLR(ra_SN, dec_SN, ra_host, dec_host, r_a, r_b, host_df, band)
                         else:
                             band = choose_band_SNR(host_df)
-                            r_a = float(host_df['%sradius_frac90'%band].values[0])
+                            r_a = float(host_df['%sKronRad'%band].values[0])
                             if r_a == r_a:
                                 elong = host_df[band + "_elong"].values[0]
                                 phi = np.radians(host_df[band + "_pa"].values[0])
-                                r_a = host_df[band + 'radius_frac90'].values[0]*0.5 #plate scale
+                                r_a = host_df[band + 'KronRad'].values[0]*0.5 #plate scale
 
                                 # in arcsec, the radius containing 90% of the galaxy light.
                                 # This empirically has improved association performance
                                 # for southern-hemisphere sources.
                                 dist, R = calc_DLR_SM(ra_SN, dec_SN, ra_host, dec_host, r_a, elong, phi, host_df, band)
 
                         R_dict[tempHost] = R
                         ra_dict[tempHost] = r_a
                         dist_dict[tempHost] = dist
 
                         hosts.loc[hosts['objID'] == tempHost, 'dist/DLR'] = R
                         hosts.loc[hosts['objID'] == tempHost, 'dist'] = dist
 
+                print("\n transient = \\", file=f)
                 print(name, file=f)
-                print("transient = \\", file=f)
-                print(name, file=f)
-                print("R_dict = \\", file=f)
-                print(R_dict, file=f)
-                print("ra_dict = \\", file=f)
-                print(ra_dict, file=f)
+                print("offset/DLR = \\", file=f)
+                #round for printing purposes
+                R_dict_print = {k:round(v,2) if isinstance(v,float) else v for k,v in R_dict.items()}
+                print(R_dict_print, file=f)
+                ra_dict_print = {k:round(v,2) if isinstance(v,float) else v for k,v in ra_dict.items()}
+                print("candidate semi-major axis = \\", file=f)
+                print(ra_dict_print, file=f)
 
                 #subset so that we're less than 5 in DLR units
                 chosenHost = min(R_dict, key=R_dict.get)
                 if R_dict[chosenHost] > 5.0:
                     #If we can't find a host, say that this galaxy has no host
                     dict_mod[name] = np.nan
                     noHosts.append(name)
```

### Comparing `astro_ghost-0.2.7/astro_ghost/NEDQueryFunctions.py` & `astro_ghost-1.0.0/astro_ghost/NEDQueryFunctions.py`

 * *Files identical despite different names*

### Comparing `astro_ghost-0.2.7/astro_ghost/PS1QueryFunctions.py` & `astro_ghost-1.0.0/astro_ghost/PS1QueryFunctions.py`

 * *Files 2% similar despite different names*

```diff
@@ -230,17 +230,19 @@
     if format not in ("jpg","png"):
         raise ValueError("format must be jpg or png")
     url = geturl(ra,dec,size=size,filters=filters,output_size=output_size,format=format,color=True, type='stack')
     r = requests.get(url)
     im = Image.open(BytesIO(r.content))
     return im
 
-def get_PS1_type(ra, dec, size, band, type):
+def get_PS1_type(path, ra, dec, size, band, type):
     """Download and save PS1 imaging data in a given band of a given type.
 
+    :param path: filepath where the image will be saved.
+    :type path: str
     :param ra: Right ascension of position, in degrees.
     :type ra: float
     :param dec: Declination of position, in degrees.
     :type dec: float
     :param size: The extracted image size in pixels (0.25 arcsec/pixel)
     :type size: int
     :param band: The PS1 band.
@@ -253,19 +255,21 @@
         \\'stack.expw\\' - weighted exposure time maps
         See more information at https://outerspace.stsci.edu/display/PANSTARRS/PS1+Stack+images.
     :type type: str
     """
 
     fitsurl = geturl(ra, dec, size=size, filters="{}".format(band), format="fits", type=type)
     fh = fits.open(fitsurl[0])
-    fh.writeto('PS1_ra={}_dec={}_{}arcsec_{}_{}.fits'.format(ra, dec, int(size*0.25), band, type))
+    fh.writeto(path + '/PS1_ra={}_dec={}_{}arcsec_{}_{}.fits'.format(ra, dec, int(size*0.25), band, type))
 
-def get_PS1_Pic(objID, ra, dec, size, band, safe=False):
-    """Downloads PS1 picture (in fits) at a given position.
+def get_PS1_Pic(path, objID, ra, dec, size, band, safe=False):
+    """Downloads PS1 picture (in fits) centered at a given location.
 
+    :param path: The filepath where the fits file will be saved.
+    :type path: str
     :param objID: The PS1 objID of the object of interest (to save as filename).
     :type objID: int
     :param ra: Right ascension of position, in degrees.
     :type ra: float
     :param dec: Declination of position, in degrees.
     :type dec: float
     :param size: The extracted image size in pixels (0.25 arcsec/pixel)
@@ -276,17 +280,17 @@
         (useful when saving multiple files at comparable positions).
     :type safe: bool, optional
     """
 
     fitsurl = geturl(ra, dec, size=size, filters="{}".format(band), format="fits")
     fh = fits.open(fitsurl[0])
     if safe==True:
-        fh.writeto('PS1_{}_{}arcsec_{}.fits'.format(objID, int(size*0.25), band))
+        fh.writeto(path + '/PS1_{}_{}arcsec_{}.fits'.format(objID, int(size*0.25), band))
     else:
-        fh.writeto('PS1_ra={}_dec={}_{}arcsec_{}.fits'.format(ra, dec, int(size*0.25), band))
+        fh.writeto(path + '/PS1_ra={}_dec={}_{}arcsec_{}.fits'.format(ra, dec, int(size*0.25), band))
 
 def ps1metadata(table="mean",release="dr1",baseurl="https://catalogs.mast.stsci.edu/api/v0.1/panstarrs"):
     """Return metadata for the specified catalog and table.
 
     :param table: Table type. Can be \\'mean\\', \\'stack\\', or \\'detection\\'
     :type table: str
     :param release: The Pan-STARRS data release. Can be \\'dr1' or \\'dr2\\'.
@@ -827,14 +831,16 @@
 
     fullDF = fullDF[colSet]
 
     leftover = set(PS1_cols) - set(fullDF.columns.values)
     for col in leftover:
         fullDF[col] = np.nan
 
+    # arrange in the correct order for combining with northern-hemisphere PS1 sources
+    fullDF = fullDF[PS1_cols]
     fullDF.drop_duplicates(subset=['objID'], inplace=True)
     return fullDF
 
 def getDR2_petrosianSizes(ra_arr, dec_arr, rad):
     """Retrieves petrosian radius information from DR2 for panstarrs sources.
 
     :param ra_arr: List of right ascension values, in degrees.
```

### Comparing `astro_ghost-0.2.7/astro_ghost/SimbadQueryFunctions.py` & `astro_ghost-1.0.0/astro_ghost/SimbadQueryFunctions.py`

 * *Files identical despite different names*

### Comparing `astro_ghost-0.2.7/astro_ghost/Star_Galaxy_RealisticModel_GHOST_PS1ClassLabels.sav` & `astro_ghost-1.0.0/astro_ghost/Star_Galaxy_RealisticModel_GHOST_PS1ClassLabels.sav`

 * *Files identical despite different names*

### Comparing `astro_ghost-0.2.7/astro_ghost/TNSQueryFunctions.py` & `astro_ghost-1.0.0/astro_ghost/TNSQueryFunctions.py`

 * *Files identical despite different names*

### Comparing `astro_ghost-0.2.7/astro_ghost/conftest.py` & `astro_ghost-1.0.0/astro_ghost/conftest.py`

 * *Files identical despite different names*

### Comparing `astro_ghost-0.2.7/astro_ghost/ghostHelperFunctions.py` & `astro_ghost-1.0.0/astro_ghost/ghostHelperFunctions.py`

 * *Files 0% similar despite different names*

```diff
@@ -552,15 +552,15 @@
         found for any of the queried transients.
     :type redo_search: bool
     :return: Final dataframe of associated transients and host galaxies.
     :rtype: Pandas DataFrame
     """
 
     #if no names were passed in, add placeholder names for each transient in the search
-    if transientName == ['']:
+    if len(transientName) < 1:
         transientName = []
         print("No transient names listed, adding placeholder names...")
         for i in np.arange(len(snCoord)):
             transientName.append("Transient_%i" % (i+1))
     hostDB = None
     tempHost1 = tempHost2 = tempHost3 = None
     found_by_name = found_by_coord = found_by_manual = 0
@@ -668,23 +668,23 @@
 
     #create temp dataframe with RA and DEC corresponding to the transient
     snDF = pd.DataFrame({'Name':transientName_arr, 'RA':snRA_arr, 'DEC':snDEC_arr, 'HostName':['']*len(snDEC_arr), 'Obj. Type':snClass_arr})
     snDF.to_csv(path+fn_SN, index=False)
 
     #begin doing the heavy lifting to associate transients with hosts
     host_DF = get_hosts(path, fn_SN, fn_Host, rad)
-    halfLightSizes = getDR2_petrosianSizes(snRA_arr, snDEC_arr, rad)
-    host_DF_new = host_DF.merge(halfLightSizes, on='objID')
-    host_DF = host_DF_new if not halfLightSizes.empty else host_DF
+    #galaxySizes = getDR2_forcedGalaxySizes(snRA_arr, snDEC_arr, rad)
+    #host_DF_new = host_DF.merge(galaxySizes, on='objID',how='outer')
+    #host_DF = host_DF_new if not galaxySizes.empty else host_DF
 
     if len(host_DF) < 1:
         print("ERROR: Found no hosts in cone search during manual association!")
         return None
 
-    cuts = ["n", "quality", "coords", "duplicate"]
+    cuts = ["n", "coords", "duplicate"]
 
     transient_dict =[]
     # this bit of trickery is required to combine northern-hemisphere and
     # southern-hemisphere source dictionaries
     f = open(path+'/dictionaries/'+fn_Dict, "rb")
     try:
         while True:
@@ -746,14 +746,17 @@
 
     fn = "DLR.txt"
     transients = pd.read_csv(path+fn_SN)
 
     with open(path+"/dictionaries/checkpoint_preDLR.p", 'wb') as fp:
            dump(host_dict_nospace, fp)
 
+    #return the candidates list before DLR for debugging purposes
+    #return host_gals_DF
+
     host_DF, host_dict_nospace_postDLR, noHosts, GD_SN = chooseByDLR(path, host_gals_DF, transients, fn, host_dict_nospace, todo="r")
 
     #last-ditch effort -- for the ones with no found host, just pick the nearest NED galaxy.
     for transient in noHosts:
           tempDF = host_gals_DF[host_gals_DF['objID'].isin(desperate_dict[transient])]
           tempDF_gals = tempDF[tempDF['NED_type'].isin(['G', 'PofG', 'GPair', 'GGroup', 'GClstr'])].reset_index()
           if len(tempDF_gals) < 1:
```

### Comparing `astro_ghost-0.2.7/astro_ghost/gradientAscent.py` & `astro_ghost-1.0.0/astro_ghost/gradientAscent.py`

 * *Files 4% similar despite different names*

```diff
@@ -113,24 +113,23 @@
     tempRA = Angle(row.RA, unit=u.degree)
     tempDEC = Angle(row.DEC, unit=u.degree)
     transientRA = tempRA.degree[0]
     transientDEC = tempDEC.degree[0]
     searchRA = transientRA
     searchDEC = transientDEC
 
-    a = find_all("PS1_ra={}_dec={}_{}arcsec_{}.fits".format(searchRA, searchDEC, int(px*0.25), band), '.')
+    a = find_all("PS1_ra={}_dec={}_{}arcsec_{}.fits".format(searchRA, searchDEC, int(px*0.25), band), path)
     if not a:
-        get_PS1_Pic(searchRA, searchDEC, px, band)
-        a = find_all("PS1_ra={}_dec={}_{}arcsec_{}.fits".format(searchRA, searchDEC, int(px*0.25), band), '.')
+        get_PS1_Pic(path, 0, searchRA, searchDEC, px, band)
+        a = find_all("PS1_ra={}_dec={}_{}arcsec_{}.fits".format(searchRA, searchDEC, int(px*0.25), band), path)
     hdu = fits.open(a[0])[0]
     image_file = get_pkg_data_filename(a[0])
     image_data = fits.getdata(image_file, ext=0)
     wcs = WCS(hdu.header)
-    fig = figure(num=None, figsize=(20,20), facecolor='w', edgecolor='k')
-    fig.add_axes(projection=wcs)
+    fig = plt.figure(num=None, figsize=(20,20), facecolor='w', edgecolor='k')
     axes_coords = [0, 0, 1, 1] # plotting full width and height
     ax = fig.add_axes(axes_coords, projection=wcs)
     axes_coords2 = [-0.045, -0.03, 1.06, 1.08]
     ax_grads = fig.add_axes(axes_coords2, projection=None)
     plt.axis('off')
     for host in hostList:
         hostDF = host_df[host_df['objID'] == host]
@@ -285,19 +284,21 @@
                 e_prev = error
 
         # don't forget to update iterator
         i += 1
 
     return u
 
-def get_clean_img(ra, dec, px, band):
+def get_clean_img(path, ra, dec, px, band):
     """Takes PS1 images, removes bad pixels, and
        estimates new pixel values through a 2D
        interpolation.
 
+    :param path: filepath where the image will be saved.
+    :type path: str
     :param ra: Right ascension of image position, in degrees.
     :type ra: float
     :param dec: Declination of image position, in degrees.
     :type dec: float
     :param px: Image size, in pixels.
     :type px: int
     :param band: Passband of image.
@@ -308,26 +309,28 @@
     :rtype: wcs of image fits file.
     :return: Header of image fits file.
     :rtype: Fits header
     """
 
     #first, mask the data
     if dec > -30:
-        a = find_all("PS1_ra={}_dec={}_{}arcsec_{}.fits".format(ra, dec, int(px*0.25), band), '.')
+        a = find_all("PS1_ra={}_dec={}_{}arcsec_{}.fits".format(ra, dec, int(px*0.25), band), path)
         if not a:
-            get_PS1_Pic(0, ra, dec, px, band)
-            a = find_all("PS1_ra={}_dec={}_{}arcsec_{}.fits".format(ra, dec, int(px*0.25), band), '.')
-        b = find_all("PS1_ra={}_dec={}_{}arcsec_{}_mask.fits".format(ra, dec, int(px*0.25), band), '.')
+            get_PS1_Pic(path, 0, ra, dec, px, band)
+            a = find_all("PS1_ra={}_dec={}_{}arcsec_{}.fits".format(ra, dec, int(px*0.25), band), path)
+        b_fn = "PS1_ra={}_dec={}_{}arcsec_{}_stack.mask.fits".format(ra, dec, int(px*0.25), band)
+        b = find_all(b_fn, path)
         if not b:
-            get_PS1_type(ra, dec, px, band, 'stack.mask')
-            b = find_all("PS1_ra={}_dec={}_{}arcsec_{}_mask.fits".format(ra, dec, int(px*0.25), band), '.')
-        c = find_all("PS1_ra={}_dec={}_{}arcsec_{}_stack.num.fits".format(ra, dec, int(px*0.25), band), '.')
+            get_PS1_type(path, ra, dec, px, band, 'stack.mask')
+            b = find_all(b_fn, path)
+        c_fn = "PS1_ra={}_dec={}_{}arcsec_{}_stack.num.fits".format(ra, dec, int(px*0.25), band)
+        c = find_all(c_fn, path)
         if not c:
-            get_PS1_type(ra, dec, px, band, 'stack.num')
-            c = find_all("PS1_ra={}_dec={}_{}arcsec_{}_stack.num.fits".format(ra, dec, int(px*0.25), band), '.')
+            get_PS1_type(path, ra, dec, px, band, 'stack.num')
+            c = find_all(c_fn, path)
 
         image_data_mask = fits.open(b[0])[0].data
         image_data_num = fits.open(c[0])[0].data
         image_data = fits.open(a[0])[0].data
 
         hdu = fits.open(a[0])[0]
         wcs = WCS(hdu.header)
@@ -348,14 +351,15 @@
 
         mask = ~np.isnan(image_data_mask)
         mask_num = image_data_num
         image_masked = np.ma.masked_array(image_data, mask=mask)
         image_masked_num = np.ma.masked_array(image_masked, mask=mask_num)
 
     else:
+        print("Error! Gradient Ascent is not yet implemented for southern-hemisphere sources.")
         a = find_all("SkyMapper_ra={}_dec={}_{}arcsec_{}.fits".format(ra, dec, int(px*0.5), band), '.')
         if not a:
             get_SkyMapper_Pic(0, ra, dec, px, band)
             a = find_all("SkyMapper_ra={}_dec={}_{}arcsec_{}.fits".format(ra, dec, int(px*0.5), band), '.')
         b = find_all("SkyMapper_ra={}_dec={}_{}arcsec_{}_mask.fits".format(ra, dec, int(px*0.5), band), '.')
         if not b:
             get_SkyMapper_mask(ra, dec, px, band)
@@ -479,30 +483,30 @@
         transient_name = transientNames[i]
         print("Transient: %s"% transient_name, file=f)
 
         ra = transientDF.loc[transientDF['Name'] == transient_name, 'RA'].values[0]
         dec = transientDF.loc[transientDF['Name'] == transient_name, 'DEC'].values[0]
 
         startTime = time.time()
-        g_img, wcs, g_hdu  = get_clean_img(ra, dec, px, 'g')
+        g_img, wcs, g_hdu  = get_clean_img(path, ra, dec, px, 'g')
         g_mask = np.ma.masked_invalid(g_img).mask
-        r_img, wcs, r_hdu  = get_clean_img(ra, dec, px, 'r')
+        r_img, wcs, r_hdu  = get_clean_img(path, ra, dec, px, 'r')
         r_mask = np.ma.masked_invalid(r_img).mask
-        i_img, wcs, i_hdu  = get_clean_img(ra, dec, px, 'i')
+        i_img, wcs, i_hdu  = get_clean_img(path, ra, dec, px, 'i')
         i_mask = np.ma.masked_invalid(i_img).mask
         endTime = time.time()
         dTime = endTime - startTime
         print("Download time: %.2f\n"%dTime, file=f)
         totalDTime+=dTime
 
         # cleanup - remove the fits files when we're done using them
         for band in ['g', 'r', 'i']:
-            os.remove("PS1_ra={}_dec={}_{}arcsec_{}_stack.num.fits".format(ra, dec, int(px*0.25), band))
-            os.remove("PS1_ra={}_dec={}_{}arcsec_{}_mask.fits".format(ra, dec, int(px*0.25), band))
-            os.remove("PS1_ra={}_dec={}_{}arcsec_{}.fits".format(ra, dec, int(px*0.25), band))
+            os.remove(path + "/PS1_ra={}_dec={}_{}arcsec_{}_stack.num.fits".format(ra, dec, int(px*0.25), band))
+            os.remove(path + "/PS1_ra={}_dec={}_{}arcsec_{}_stack.mask.fits".format(ra, dec, int(px*0.25), band))
+            os.remove(path + "/PS1_ra={}_dec={}_{}arcsec_{}.fits".format(ra, dec, int(px*0.25), band))
 
         nancount = 0
         obj_interp = []
         print("Commencing DAOStarFinder:\n", file=f)
         for obj in [g_img, r_img, i_img]:
             data = obj
             mean, median, std = sigma_clipped_stats(data, sigma=15.0)
@@ -701,17 +705,17 @@
 
             col = '#D34E24'
             col2 = '#B54A24'
 
             #lookup by ra, dec
             try:
                 if size == 'large':
-                    a = query_ps1_noname(float(coords[0]), float(coords[1]), 20)
+                    a = ps1cone(float(coords[0]), float(coords[1]), 20/3600)
                 else:
-                    a = query_ps1_noname(float(coords[0]), float(coords[1]), 5)
+                    a = ps1cone(float(coords[0]), float(coords[1]), 5/3600)
             except TypeError:
                  continue
             if a:
                 print("Found a host here!", file=f)
                 a = ascii.read(a)
                 a = a.to_pandas()
                 a.sort_values(by=['distance'], inplace=True)
```

### Comparing `astro_ghost-0.2.7/astro_ghost/hostMatching.py` & `astro_ghost-1.0.0/astro_ghost/hostMatching.py`

 * *Files identical despite different names*

### Comparing `astro_ghost-0.2.7/astro_ghost/photoz_helper.py` & `astro_ghost-1.0.0/astro_ghost/photoz_helper.py`

 * *Files 14% similar despite different names*

```diff
@@ -65,15 +65,15 @@
     print("Done getting photo-z weights.")
     return
 
 def ps1objIDsearch(objID,table="mean",release="dr1",format="csv",columns=None,
            baseurl="https://catalogs.mast.stsci.edu/api/v0.1/panstarrs", verbose=False,
            **kw):
     """Do an object lookup by objID.
-
+   
     :param objID: list of objIDs (or dictionary?)
     :type objID: List of objIDs
     :param table: Can be \\'mean\\', \\'stack\\', or \\'detection\\'.
     :type table: str
     :param release: Can be 'dr1' or 'dr2'.
     :type release: str
     :param format: Can be 'csv', 'votable', or 'json'
@@ -105,26 +105,26 @@
 
         urls.append(url)
         datas.append(data)
 
     return urls, datas
 
 def fetch_information_serially(url, data, verbose=False, format='csv'):
-    """Short summary.
-
+    """A helper function called by serial_objID_search-- Queries PanStarrs API for data.
+    
     :param url: Remote PS1 url.
     :type url: str
-    :param data: Description of parameter `data`.
-    :type data:
+    :param data: List of objIDs requesting
+    :type data: list
     :param verbose: If True,
     :type verbose: bool, optional
     :param format: Can be \\'csv\\', \\'json\\', or \\'votable\\'.
-    :type format:
+    :type format: str
     :return:
-    :rtype: Same type as \\'format\\'.
+    :rtype: str in format given by \\'format\\'.
     """
 
     results = []
     for i in range(len(url)):
         r = requests.get(url[i], params=data[i])
         if verbose:
             print(r.url)
@@ -133,16 +133,16 @@
             results.append(r.json())
         else:
             results.append(r.text)
 
     return results
 
 def post_url_parallel(results,YSE_ID):
-    """Short summary.
-
+    """TODO: unused function. The querying of PS servers is the slowest part of the script. How to parallelize?
+     
     :param results: Description of parameter.
     :type results: type
     :param YSE_ID: Description of parameter.
     :type YSE_ID: type
     :return: Description of returned object.
     :rtype: Pandas DataFrame
     """
@@ -157,65 +157,65 @@
     else:
         print('No Matches')
         DF = pd.DataFrame()
     DF['YSE_id'] = np.ones(len(DF))*YSE_ID
     return DF
 
 def post_url_serial(results,YSE_ID):
-    """Short summary.
+    """A helper function called by serial_objID_search. Post-processes the data retrieved from PS1 Servers into a pandas.DataFrame object.
 
-    :param results: Description of parameter.
-    :type results: type
-    :param YSE_ID: Description of parameter.
-    :type YSE_ID: type.
-    :return:
-    :rtype:
+    :param results: The string resulting from PS1 query.
+    :type results: str
+    :param YSE_ID: local integer used for as an index tracking user objects vs retrived objects.
+    :type YSE_ID: int
+    :return: DataFrame object of the retrieved data from PS1 servers
+    :rtype: pandas.DataFrame
     """
     if type(results) != str:
         results = codecs.decode(results,'UTF-8')
     lines = results.split('\r\n')
     #print(lines)
     if len(lines) > 2:
         values = [line.strip().split(',') for line in lines]
         DF = pd.DataFrame(values[1:-1],columns=values[0])
     else:
         DF = pd.DataFrame()
     DF['id'] = np.ones(len(DF))*YSE_ID
     return DF
 
 def serial_objID_search(objIDs,table='forced_mean',release='dr2',columns=None,verbose=False,**constraints):
-    """Short summary.
-
-    :param objIDs: Description of param
-    :type objIDs: type
-    :param table: Description of param
-    :type table: type
-    :param release: Description of param
-    :type release: type
-    :param columns: Description of param
-    :type columns: type
-    :param verbose: Description of param
-    :type verbose: type.
-    :param \\*\\*constraints: Description of param
-    :type \\*\\*constraints: type.
-    :return: Description of param
-    :rtype: type
+    """Given a list of ObjIDs, queries the PS1 server these object's Forced Mean Photometry, then returns matches as a pandas.DataFrame.
+    
+    :param objIDs: list of PS1 objIDs for objects user would like to query
+    :type objIDs: list
+    :param table: Which table to perform the query on. Default 'forced_mean'
+    :type table: str
+    :param release: Which release to perform the query on. Default 'dr2'
+    :type release: str
+    :param columns: list of what data fields to include; None means use default columns. Default None
+    :type columns: list or None
+    :param verbose: boolean setting level of feedback user received. default False
+    :type verbose: bool
+    :param \\*\\*constraints: Keyword dictionary with an additional constraints for the PS1 query
+    :type \\*\\*constraints: dict
+    :return: list of pd.DataFrame objects. If a match was found, then the Dataframe contains data, else it only contains a local integer.
+    :rtype: pd.DataFrame
     """
 
     constrains=constraints.copy()
     URLS, DATAS = ps1objIDsearch(objID=objIDs,table='forced_mean',release=release,columns=columns,verbose=verbose,**constraints)
     Return = fetch_information_serially(URLS,DATAS)
     DFs=[]
     for i in range(len(Return)):
         DFs.append(post_url_serial(Return[i],i))
 
     return DFs
 
 def post_url_parallel(results,YSE_ID):
-    """Short summary.
+    """TODO: unused function. The querying of PS servers is the slowest part of the script. How to parallelize?
 
     :param results: Description of param.
     :type results: type
     :param YSE_ID: Description of param.
     :type YSE_ID: type
     :return:
     :rtype:
@@ -228,20 +228,20 @@
         DF = pd.DataFrame(values[1:-1],columns=values[0])
     else:
         DF = pd.DataFrame()
     DF['id'] = np.ones(len(DF))*YSE_ID
     return DF
 
 def get_common_constraints_columns():
-    """Short summary.
+    """Helper function that returns a dictionary of constraints used for the matching objects in PS1 archive, and the columns of data we requre.
 
-    :return: adfasdf
-    :rtype: adfasdf
-    :return: adfasdf
-    :rtype: asdfasdf
+    :return: dictionary with our constaint that we must have more than one detection
+    :rtype: dict
+    :return: List of PS1 fields required for matching and NN inputs
+    :rtype: list
     """
 
     constraints = {'nDetections.gt':1}
 
     #objects with n_detection=1 sometimes just an artifact.
     # strip blanks and weed out blank and commented-out values
     columns ="""objID, raMean, decMean, gFKronFlux, rFKronFlux, iFKronFlux, zFKronFlux, yFKronFlux,
@@ -252,24 +252,24 @@
     gFmeanflxR7, rFmeanflxR7, iFmeanflxR7, zFmeanflxR7, yFmeanflxR7""".split(',')
     columns = [x.strip() for x in columns]
     columns = [x for x in columns if x and not x.startswith('#')]
 
     return constraints, columns
 
 def preprocess(DF,PATH='../DATA/sfddata-master/', ebv=True):
-    """Short summary.
+    """Preprocesses the data inside pandas.DataFrame object returned by serial_objID_search to the space of Inputs of our Neural Network.
 
-    :param DF: asdfasdf
-    :type DF: asdfasdf
-    :param PATH: asdfasdf
-    :type PATH: asdfasdf
-    :param ebv: asdfasdf
-    :type ebv: asdfasdf
-    :return: asdfasdf
-    :rtype: asdfasdf
+    :param DF: Dataframe object containing the data for each matched objID
+    :type DF: pandas DataFrame
+    :param PATH: string path to extinction maps data
+    :type PATH: str
+    :param ebv: boolean for lookup of extinction data. If False, all extinctions set to 0.
+    :type ebv: False
+    :return: Preprocessed inputs ready to be used as input to NN
+    :rtype: numpy ndarray
     """
     if ebv:
         m = sfdmap.SFDMap(PATH)
         assert ('raMean' in DF.columns.values) and ('decMean' in DF.columns.values), 'DustMap query failed because the expected coordinates didnt'\
                                                                             'exist in DF, likely the match of any Hosts into PanStarrs failed'
         EBV = m.ebv(DF['raMean'].values.astype(np.float32),DF['decMean'].values.astype(np.float32))
 
@@ -321,22 +321,22 @@
     X[X>20] = 20
     X[X<-20] = -20
     X[np.isnan(X)] = -20
 
     return X
 
 def load_lupton_model(model_path):
-    """Short summary.
+    """Helper function that defines and loads the weights of our NN model and the output space of the NN.
 
-    :param model_path: Description of param.
+    :param model_path: path to the model weights.
     :type model_path: str
     :return: Trained photo-z MLP.
-    :rtype: keras tensorflow model.
-    :return: ??
-    :rtype:
+    :rtype: tensorflow keras Model
+    :return: Array of binned redshift space corresponding to the output space of the NN
+    :rtype: numpy ndarray
     """
 
     build_sfd_dir()
     get_photoz_weights(model_path)
     def model():
         INPUT = tf.keras.layers.Input(31)
 
@@ -369,25 +369,25 @@
 
 def evaluate(X,mymodel,range_z):
     """Evaluate the MLP for a set of PS1 inputs, and return predictions.
 
     :param X: PS1 properties of associated hosts.
     :type X: array-like
     :param mymodel: MLP model for photo-z estimation.
-    :type mymodel: keras model
+    :type mymodel: tensorflow keras Model
     :param range_z: Grid over which to evaluate the posterior distribution of photo-zs.
     :type range_z: array-like
 
     :return: Posterior distributions for the grid of redshifts defined as
         \\`np.linspace(0, 1, n)\\`
-    :rtype: ndarray shape of (df.shape[0], n)
+    :rtype: numpy ndarray shape of (df.shape[0], n)
     :return: Means
-    :rtype: ndarray shape of (df.shape[0],)
+    :rtype: numpy ndarray shape of (df.shape[0],)
     :return: Standard deviations
-    :rtype: ndarray shape of (df.shape[0],)
+    :rtype: numpy ndarray shape of (df.shape[0],)
     """
 
     posteriors = mymodel(X,training=False).numpy()
     point_estimates = np.sum(posteriors*range_z,axis=1)
     for i in range(len(posteriors)):
         posteriors[i,:] /= np.sum(posteriors[i,:])
     errors=np.ones(len(posteriors))
@@ -408,15 +408,15 @@
        error is an array that uses sampling from the posterior to estimate a std dev.
        Relies upon the sfdmap package, (which is compatible with both unix and windows),
        found at https://github.com/kbarbary/sfdmap.
 
     :param hosts: The matched hosts from GHOST.
     :type hosts: pandas DataFrame
     :return: The matched hosts from GHOST, with photo-z point estimates and uncertainties.
-    :rtype: Pandas DataFrame
+    :rtype: pandas DataFrame
     """
 
     if np.nansum(hosts['decMean'] < -30) > 0:
         print("ERROR! Photo-z estimator has not yet been implemented for southern-hemisphere sources."\
         "Please remove sources below dec=-30d and try again.")
         return hosts
     objIDs = hosts['objID'].values.tolist()
@@ -437,22 +437,22 @@
 def get_photoz(df):
     """Evaluate photo-z model for Pan-STARRS forced photometry.
 
     :param df: Pan-STARRS forced mean photometry data, you can get it using
         \\`ps1objIDsearch\\` from this module, Pan-STARRS web-portal or via
         astroquery i.e., \\`astroquery.mast.Catalogs.query_{criteria,region}(...,
         catalog=\\'Panstarrs\\',table=\\'forced_mean\\')\\`
-    :type df: Pandas DataFrame
+    :type df: pandas DataFrame
     :return: Posterior distributions for the grid of redshifts defined as
         \\`np.linspace(0, 1, n)\\`
-    :rtype: ndarray shape of (df.shape[0], n)
+    :rtype: numpy ndarray shape of (df.shape[0], n)
     :return: Means
-    :rtype: ndarray shape of (df.shape[0],)
+    :rtype: numpy ndarray shape of (df.shape[0],)
     :return: Standard deviations
-    :rtype: ndarray shape of (df.shape[0],)
+    :rtype: numpy ndarray shape of (df.shape[0],)
     """
 
     # The function load_lupton_model downloads the necessary dust models and
     # weights from the ghost server.
     dust_path = './sfddata-master'
     model_path = './MLP_lupton.hdf5'
```

### Comparing `astro_ghost-0.2.7/astro_ghost/sourceCleaning.py` & `astro_ghost-1.0.0/astro_ghost/sourceCleaning.py`

 * *Files 11% similar despite different names*

```diff
@@ -165,43 +165,37 @@
     :rtype: Pandas DataFrame
     """
 
     df.replace(-999, np.nan, inplace=True)
     df.replace(999, np.nan, inplace=True)
 
     # create color attributes for all hosts
-    df["i-z"] = df["iApMag"] - df["zApMag"]
     df["g-r"]= df["gApMag"] - df["rApMag"]
     df["r-i"]= df["rApMag"] - df["iApMag"]
-    df["g-i"] = df["gApMag"] - df["iApMag"]
+    df["i-z"] = df["iApMag"] - df["zApMag"]
+#    df["g-i"] = df["gApMag"] - df["iApMag"]
     df["z-y"] = df["zApMag"] - df["yApMag"]
 
     df['g-rErr'] = np.sqrt(df['gApMagErr']**2 + df['rApMagErr']**2)
     df['r-iErr'] = np.sqrt(df['rApMagErr']**2 + df['iApMagErr']**2)
     df['i-zErr'] = np.sqrt(df['iApMagErr']**2 + df['zApMagErr']**2)
     df['z-yErr'] = np.sqrt(df['zApMagErr']**2 + df['yApMagErr']**2)
 
     # To be sure we're getting physical colors
-    df.loc[df['i-z'] > 100, 'i-z'] = np.nan
-    df.loc[df['i-z'] < -100, 'i-z'] = np.nan
-    df.loc[df['g-r'] > 100, 'i-z'] = np.nan
-    df.loc[df['g-r'] < -100, 'i-z'] = np.nan
+    for col in ['g-r', 'r-i', 'i-z', 'z-y']:
+        df.loc[np.abs(df[col]) > 100, col] = np.nan
 
     # and PSF - Kron mag "morphology" information
-    df["gApMag_gKronMag"] = df["gApMag"] - df["gKronMag"]
-    df["rApMag_rKronMag"] = df["rApMag"] - df["rKronMag"]
-    df["iApMag_iKronMag"] = df["iApMag"] - df["iKronMag"]
-    df["zApMag_zKronMag"] = df["zApMag"] - df["zKronMag"]
-    df["yApMag_yKronMag"] = df["yApMag"] - df["yKronMag"]
-
-    # to be sure we're getting physical mags
-    df.loc[df['iApMag_iKronMag'] > 100, 'iApMag_iKronMag'] = np.nan
-    df.loc[df['iApMag_iKronMag'] < -100, 'iApMag_iKronMag'] = np.nan
-    df.loc[df['iApMag'] > 100, 'iApMag'] = np.nan
-    df.loc[df['iApMag'] < -100, 'iApMag'] = np.nan
+    for band in 'grizy':
+        # to be sure we're getting physical mags
+        col = '%sApMag_%sKronMag'%(band, band)
+        df[col] = df["%sApMag"%band] - df["%sKronMag"%band]
+        df.loc[np.abs(df[col]) > 100, col] = np.nan
+        col = '%sApMag'%band
+        df.loc[np.abs(df[col]) > 100, col] = np.nan
     return df
 
 def makeCuts(df,cuts=[],dict=""):
     """Make a series of quality cuts on the candidate host galaxies in the dataframe.
 
     :param df: PS1 properties for candidate hosts.
     :type df: Pandas DataFrame
@@ -226,19 +220,16 @@
         if cut == "n":
             df = df[df['nDetections'] >= 10]
         elif cut == "quality":
             df = df[df["qualityFlag"] < 128]
         elif cut == "coords":
             df = df.dropna(subset=['raMean', 'decMean'])
         elif cut == "mag":
-            df = df[pd.notnull(df['gApMag'])]
-            df = df[pd.notnull(df['rApMag'])]
-            df = df[pd.notnull(df['iApMag'])]
-            df = df[pd.notnull(df['zApMag'])]
-            df = df[pd.notnull(df['yApMag'])]
+            for band in 'grizy':
+                df = df[pd.notnull(df['%sApMag'%band])]
         elif cut =="primary":
             if dict != "":
                 df_mod = df[df["primaryDetection"] == 1]
                 clean_dict(dict, df_mod, np.array([]),bestDetectionCut=1)
                 clean_df_from_dict(dict, df)
             else:
                 print("Can't make a primary detection cut - no dict provided!")
```

### Comparing `astro_ghost-0.2.7/astro_ghost/starSeparation.py` & `astro_ghost-1.0.0/astro_ghost/starSeparation.py`

 * *Files 26% similar despite different names*

```diff
@@ -23,18 +23,29 @@
 
     :return: A dataframe of sources classified as galaxies.
     :rtype: Pandas DataFrame
     :return: A dataframe of sources classified as stars.
     :rtype: Pandas DataFrame
     """
 
-    # remove all sources with bad values for any required PS1 properties
-    df_dropped = df.dropna(subset=['7DCD','gApMag','gApMag_gKronMag','rApMag','rApMag_rKronMag','iApMag', 'iApMag_iKronMag'])
-    only_na = df[~df.index.isin(df_dropped.index)]
-    unsure = df_dropped.reset_index(drop=True)
+    #remove known galaxies and stars
+    NED_stars = df[df['NED_type'].isin(['*', '**', 'WD*', '!*', '!V*', 'V*', '!Nova'])]
+    NED_gals = df[df['NED_type'] == 'G']
+
+    #get the remaining objects
+    unsure = df[~df.index.isin(NED_stars.index)]
+    unsure = unsure[~unsure.index.isin(NED_gals.index)]
+
+    #also drop HII regions, QSOs, etc
+    unsure = unsure[~unsure['NED_type'].isin(['HII', 'QSO', 'SNR', 'PN'])]
+
+    #remove all sources with bad values for any required PS1 properties
+    unsure_dropped = unsure.dropna(subset=['7DCD','gApMag','gApMag_gKronMag','rApMag','rApMag_rKronMag','iApMag', 'iApMag_iKronMag'])
+    #keep track of the unknown sources with bad values - we don't want to lose them entirely
+    only_na = unsure[~unsure.index.isin(unsure_dropped.index)]
 
     # load random forest model
     modelName = "Star_Galaxy_RealisticModel_GHOST_PS1ClassLabels.sav"
     stream = importlib_resources.files(__name__).joinpath(modelName).open("rb")
     if verbose:
         print("Loading model %s."%modelName)
     model = pickle.load(stream)
@@ -46,32 +57,31 @@
 
         plt.figure(figsize=(10,8))
         plt.plot(unsure['iApMag'], unsure['iApMag_iKronMag'], 'o', alpha=0.1)
         plt.xlabel(r"Ap Mag, $i$")
         plt.ylabel(r"Ap - Kron Mag, $i$")
         plt.savefig("TNS_NoClassificationInfo.pdf")
 
-    unsure = unsure.dropna(subset=['7DCD','gApMag','gApMag_gKronMag','rApMag','rApMag_rKronMag','iApMag', 'iApMag_iKronMag'])
-    if len(unsure) <1:
+    if len(unsure_dropped) <1:
         if verbose:
             print("No sources in field with feature values, skipping star/galaxy separation...")
-        return df, unsure
-    test_X = np.asarray(unsure[['7DCD','gApMag','gApMag_gKronMag','rApMag','rApMag_rKronMag','iApMag', 'iApMag_iKronMag']])
+        return df, unsure_dropped
+    test_X = np.asarray(unsure_dropped[['7DCD','gApMag','gApMag_gKronMag','rApMag','rApMag_rKronMag','iApMag', 'iApMag_iKronMag']])
 
     # define probability threshold for classification
     cutdict = {'normal':0.5, 'aggressive':0.3, 'gentle':0.8}
 
     try:
         test_y = model.predict_proba(test_X)[:,1] > cutdict[starcut]
     except:
         print("Error! I didn't understand your starcut option.")
 
-    unsure['class'] = test_y
-    test_stars = unsure[unsure['class'] == 1]
-    test_gals = unsure[unsure['class'] == 0]
+    unsure_dropped['class'] = test_y
+    test_stars = unsure_dropped[unsure_dropped['class'] == 1]
+    test_gals = unsure_dropped[unsure_dropped['class'] == 0]
 
     # plot the distribution of classified stars and galaxies.
     if plot:
         c_gals = '#087e8b'
         c_stars = '#ffbf00'
 
         plt.figure(num=None, figsize=(8, 6), dpi=80, facecolor='w', edgecolor='k')
@@ -95,21 +105,21 @@
         plt.xlim(-1, 3)
         plt.xlabel("Ap - Kron Mag, $i$",fontsize=16)
         plt.xlim()
         plt.ylabel("N",fontsize=16)
         plt.legend(fontsize=16)
         plt.savefig("TNS_iAp_iKronMag_Histogram.pdf")
 
-    # removing the ones where we have no NED identification
-    df = df[~df['NED_type'].isnull()]
-
-    # Adding back in the ones we identified as galaxies from our clustering above:
-    df_gals = pd.concat([test_gals, only_na])
+    # Adding back in the ones we identified as galaxies from our clustering above, and the NED sources.
+    df_gals = pd.concat([test_gals, only_na, NED_gals])
     df_gals.reset_index(inplace=True, drop=True)
-    df_stars = test_stars.drop_duplicates()
+
+    # Adding back in the ones we identified as stars from our clustering above, and the NED sources.
+    df_stars = pd.concat([test_stars, NED_stars])
+    df_stars.reset_index(inplace=True, drop=True)
     return df_gals, df_stars
 
 def separateStars_South(df, plot=0, verbose=0, starcut='gentle'):
     """Star-galaxy separation in the southern hemisphere, using a simple
        SkyMapper_StarClass threshold cut.
 
     :param df: Dataframe of PS1 sources.
@@ -124,22 +134,35 @@
 
     :return: A dataframe of sources classified as galaxies.
     :rtype: Pandas DataFrame
     :return: A dataframe of sources classified as stars.
     :rtype: Pandas DataFrame
     """
 
-    df_dropped = df[df['SkyMapper_StarClass']>0]
-    only_na = df[~df.index.isin(df_dropped.index)]
+    #remove known galaxies and stars
+    NED_stars = df[df['NED_type'].isin(['*', '**', 'WD*', '!*', '!V*', 'V*', '!Nova'])]
+    NED_gals = df[df['NED_type'] == 'G']
+
+    #get the remaining objects
+    unsure = df[~df.index.isin(NED_stars.index)]
+    unsure = unsure[~unsure.index.isin(NED_gals.index)]
+
+    unsure_dropped = unsure[unsure['SkyMapper_StarClass']>0]
+    only_na = unsure[~unsure.index.isin(unsure_dropped.index)]
 
     # define probability threshold for classification
     cutdict = {'normal':0.5, 'aggressive':0.3, 'gentle':0.8}
     try:
-        df_stars = df_dropped[df_dropped['SkyMapper_StarClass']> cutdict[starcut]]
+        test_stars = unsure_dropped[unsure_dropped['SkyMapper_StarClass']> cutdict[starcut]]
     except:
         print("Error! I didn't understand your starcut option.")
 
-    df_class_gals = df_dropped[~df_dropped.index.isin(df_stars.index)]
+    test_gals = unsure_dropped[~unsure_dropped.index.isin(test_stars.index)]
+
+    # Adding back in the ones we identified as galaxies from our clustering above, and the NED sources.
+    df_gals = pd.concat([test_gals, NED_gals])
+    df_gals.reset_index(inplace=True, drop=True)
+
+    # Adding back in the ones we identified as stars from our clustering above, and the NED sources.
+    df_stars = pd.concat([test_stars, NED_stars])
     df_stars.reset_index(inplace=True, drop=True)
-    df_class_gals.reset_index(inplace=True, drop=True)
-    df_gals = pd.concat([df_class_gals, only_na], ignore_index=True).drop_duplicates()
     return df_gals, df_stars
```

### Comparing `astro_ghost-0.2.7/astro_ghost/stellarLocus.py` & `astro_ghost-1.0.0/astro_ghost/stellarLocus.py`

 * *Files identical despite different names*

### Comparing `astro_ghost-0.2.7/astro_ghost.egg-info/PKG-INFO` & `astro_ghost-1.0.0/astro_ghost.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: astro-ghost
-Version: 0.2.7
+Version: 1.0.0
 Summary: A package to associate transients with host galaxies, and a database of 16k SNe-host galaxies in PS1.
 Home-page: https://github.com/pypa/sampleproject
 Author: Alex Gagliano
 Author-email: gaglian2@illinois.edu
 License: GNU GPL v3+
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `astro_ghost-0.2.7/astro_ghost.egg-info/SOURCES.txt` & `astro_ghost-1.0.0/astro_ghost.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -43,8 +43,9 @@
 docs/source/preprocessingmodules.rst
 docs/source/supplementalmodules.rst
 docs/source/wrappermodules.rst
 licenses/LICENSE.rst
 licenses/README.rst
 tests/__init__.py
 tests/debug.py
+tests/pytest.ini
 tests/test_tutorial.py
```

### Comparing `astro_ghost-0.2.7/docs/Makefile` & `astro_ghost-1.0.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `astro_ghost-0.2.7/docs/conf.py` & `astro_ghost-1.0.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `astro_ghost-0.2.7/docs/index.rst` & `astro_ghost-1.0.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `astro_ghost-0.2.7/docs/make.bat` & `astro_ghost-1.0.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `astro_ghost-0.2.7/docs/source/associationmodules.rst` & `astro_ghost-1.0.0/docs/source/associationmodules.rst`

 * *Files identical despite different names*

### Comparing `astro_ghost-0.2.7/docs/source/basicusage.rst` & `astro_ghost-1.0.0/docs/source/basicusage.rst`

 * *Files identical despite different names*

### Comparing `astro_ghost-0.2.7/docs/source/catalogmodules.rst` & `astro_ghost-1.0.0/docs/source/catalogmodules.rst`

 * *Files identical despite different names*

### Comparing `astro_ghost-0.2.7/docs/source/installation.rst` & `astro_ghost-1.0.0/docs/source/installation.rst`

 * *Files identical despite different names*

### Comparing `astro_ghost-0.2.7/docs/source/preprocessingmodules.rst` & `astro_ghost-1.0.0/docs/source/preprocessingmodules.rst`

 * *Files identical despite different names*

### Comparing `astro_ghost-0.2.7/licenses/LICENSE.rst` & `astro_ghost-1.0.0/licenses/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `astro_ghost-0.2.7/setup.cfg` & `astro_ghost-1.0.0/setup.cfg`

 * *Files 6% similar despite different names*

```diff
@@ -49,33 +49,29 @@
 	sphinx_toolbox
 	sphinx_copybutton
 
 [options.package_data]
 astro_ghost = data/*
 
 [tool:pytest]
-testpaths = "astro_ghost" "docs"
+testpaths = "astro_ghost" "docs" "tests"
 doctest_plus = enabled
 text_file_format = rst
 addopts = --doctest-rst
 
 [coverage:run]
 omit = 
 	astro_ghost/__init*
 	astro_ghost/conftest.py
 	astro_ghost/*setup_package*
-	astro_ghost/tests/*
-	astro_ghost/*/tests/*
 	astro_ghost/extern/*
 	astro_ghost/version*
 	*/astro_ghost/__init*
 	*/astro_ghost/conftest.py
 	*/astro_ghost/*setup_package*
-	*/astro_ghost/tests/*
-	*/astro_ghost/*/tests/*
 	*/astro_ghost/extern/*
 	*/astro_ghost/version*
 
 [coverage:report]
 exclude_lines = 
 	pragma: no cover
 	except ImportError
```

### Comparing `astro_ghost-0.2.7/setup.py` & `astro_ghost-1.0.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #!/usr/bin/env python
 # Licensed under a 3-clause BSD style license - see LICENSE.rst
 
 import os
 
 from setuptools import setup
 
-version = "0.2.7"
+version = "1.0.0"
 
 VERSION_TEMPLATE = """
  Note that we need to fall back to the hard-coded version if either
  setuptools_scm can't be imported or setuptools_scm can't determine the
  version, so we catch the generic 'Exception'.
 __version__ = '{version}'
 """.lstrip()
```

### Comparing `astro_ghost-0.2.7/tests/debug.py` & `astro_ghost-1.0.0/tests/debug.py`

 * *Files 16% similar despite different names*

```diff
@@ -13,7 +13,11 @@
 import astro_ghost
 
 #we want to include print statements so we know what the algorithm is doing
 verbose = 1
 
 
 #need to generate tests for photoz_helper and gradientAscent!!
+
+t = np.linspace(0, 70)
+y = 7.*2.71828**(-(t)/50)/(1+2.71828**(-(t)/11))
+plt.plot(t, y)
```

### Comparing `astro_ghost-0.2.7/tests/test_tutorial.py` & `astro_ghost-1.0.0/tests/test_tutorial.py`

 * *Files 2% similar despite different names*

```diff
@@ -41,17 +41,17 @@
             SkyCoord(187.32867*u.deg, -23.16367*u.deg, frame='icrs'), \
             SkyCoord(186.26125*u.deg, +12.899444*u.deg, frame='icrs')]
 
     snClass = ['SN IIP', 'SN', 'SN Ia']
 
     # run the association algorithm with the DLR method!
     hosts = getTransientHosts(snName, snCoord, snClass, verbose=verbose, starcut='gentle', ascentMatch=False)
-    
-    correctHosts = [SkyCoord(14.1777425*u.deg, -9.9138756*u.deg, frame='icrs'), 
-                    SkyCoord(187.3380517*u.deg, -23.1666716*u.deg, frame='icrs'), 
+
+    correctHosts = [SkyCoord(14.1777425*u.deg, -9.9138756*u.deg, frame='icrs'),
+                    SkyCoord(187.3380517*u.deg, -23.1666716*u.deg, frame='icrs'),
                     SkyCoord(186.2655971*u.deg, 12.8869831*u.deg, frame='icrs')]
 
     sep = []
     for i in np.arange(len(correctHosts)):
        c1 = correctHosts[i]
        c2 = SkyCoord(hosts['TransientRA'].values[i]*u.deg, hosts['TransientDEC'].values[i]*u.deg, frame='icrs')
        sep.append(c2.separation(c2).arcsec)
```

### Comparing `astro_ghost-0.2.7/tox.ini` & `astro_ghost-1.0.0/tox.ini`

 * *Files identical despite different names*

