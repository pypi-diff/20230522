# Comparing `tmp/astro_ghost-1.0.0.tar.gz` & `tmp/astro_ghost-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "astro_ghost-1.0.0.tar", last modified: Mon May 22 05:31:42 2023, max compression
+gzip compressed data, was "astro_ghost-1.0.1.tar", last modified: Mon May 22 05:38:09 2023, max compression
```

## Comparing `astro_ghost-1.0.0.tar` & `astro_ghost-1.0.1.tar`

### file list

```diff
@@ -1,61 +1,61 @@
-drwxr-xr-x   0 alexgagliano   (501) staff       (20)        0 2023-05-22 05:31:42.527682 astro_ghost-1.0.0/
-drwxr-xr-x   0 alexgagliano   (501) staff       (20)        0 2023-05-22 05:31:42.437688 astro_ghost-1.0.0/.github/
-drwxr-xr-x   0 alexgagliano   (501) staff       (20)        0 2023-05-22 05:31:42.444495 astro_ghost-1.0.0/.github/workflows/
--rw-r--r--   0 alexgagliano   (501) staff       (20)      377 2022-08-10 18:18:27.000000 astro_ghost-1.0.0/.github/workflows/docs.yml
--rw-r--r--   0 alexgagliano   (501) staff       (20)      626 2023-05-09 16:17:11.000000 astro_ghost-1.0.0/.github/workflows/tests.yml
--rw-r--r--   0 alexgagliano   (501) staff       (20)      769 2022-08-10 18:18:27.000000 astro_ghost-1.0.0/.gitignore
--rw-r--r--   0 alexgagliano   (501) staff       (20)      170 2022-08-10 18:18:27.000000 astro_ghost-1.0.0/.readthedocs.yml
--rw-r--r--   0 alexgagliano   (501) staff       (20)      341 2022-08-10 18:18:27.000000 astro_ghost-1.0.0/MANIFEST.in
--rw-r--r--   0 alexgagliano   (501) staff       (20)     4089 2023-05-22 05:31:42.532751 astro_ghost-1.0.0/PKG-INFO
--rw-r--r--   0 alexgagliano   (501) staff       (20)     3488 2023-05-10 20:43:06.000000 astro_ghost-1.0.0/README.rst
-drwxr-xr-x   0 alexgagliano   (501) staff       (20)        0 2023-05-22 05:31:42.492051 astro_ghost-1.0.0/astro_ghost/
--rw-r--r--   0 alexgagliano   (501) staff       (20)    14598 2023-05-22 05:20:41.000000 astro_ghost-1.0.0/astro_ghost/DLR.py
--rw-r--r--   0 alexgagliano   (501) staff       (20)     4668 2023-05-10 23:12:18.000000 astro_ghost-1.0.0/astro_ghost/NEDQueryFunctions.py
--rw-r--r--   0 alexgagliano   (501) staff       (20)    38679 2023-05-22 03:39:53.000000 astro_ghost-1.0.0/astro_ghost/PS1QueryFunctions.py
--rw-r--r--   0 alexgagliano   (501) staff       (20)     1296 2023-05-10 22:09:14.000000 astro_ghost-1.0.0/astro_ghost/SimbadQueryFunctions.py
--rw-r--r--   0 alexgagliano   (501) staff       (20) 13643353 2023-05-08 18:43:43.000000 astro_ghost-1.0.0/astro_ghost/Star_Galaxy_RealisticModel_GHOST_PS1ClassLabels.sav
--rw-r--r--   0 alexgagliano   (501) staff       (20)     1475 2023-05-11 05:34:31.000000 astro_ghost-1.0.0/astro_ghost/TNSQueryFunctions.py
--rw-r--r--   0 alexgagliano   (501) staff       (20)      112 2023-02-17 00:45:54.000000 astro_ghost-1.0.0/astro_ghost/__init__.py
--rw-r--r--   0 alexgagliano   (501) staff       (20)       22 2023-05-22 03:39:53.000000 astro_ghost-1.0.0/astro_ghost/_version.py
--rw-r--r--   0 alexgagliano   (501) staff       (20)     1957 2023-02-17 00:45:54.000000 astro_ghost-1.0.0/astro_ghost/conftest.py
--rw-r--r--   0 alexgagliano   (501) staff       (20)    37989 2023-05-22 05:21:18.000000 astro_ghost-1.0.0/astro_ghost/ghostHelperFunctions.py
--rw-r--r--   0 alexgagliano   (501) staff       (20)    32867 2023-05-22 05:22:39.000000 astro_ghost-1.0.0/astro_ghost/gradientAscent.py
--rw-r--r--   0 alexgagliano   (501) staff       (20)     2838 2023-05-09 20:46:38.000000 astro_ghost-1.0.0/astro_ghost/hostMatching.py
--rw-r--r--   0 alexgagliano   (501) staff       (20)    17727 2023-05-22 03:39:53.000000 astro_ghost-1.0.0/astro_ghost/photoz_helper.py
--rw-r--r--   0 alexgagliano   (501) staff       (20)     9852 2023-05-22 04:36:12.000000 astro_ghost-1.0.0/astro_ghost/sourceCleaning.py
--rw-r--r--   0 alexgagliano   (501) staff       (20)     7585 2023-05-22 05:17:09.000000 astro_ghost-1.0.0/astro_ghost/starSeparation.py
--rw-r--r--   0 alexgagliano   (501) staff       (20)     4611 2023-05-11 04:35:06.000000 astro_ghost-1.0.0/astro_ghost/stellarLocus.py
--rw-r--r--   0 alexgagliano   (501) staff       (20)      302 2023-02-17 00:45:54.000000 astro_ghost-1.0.0/astro_ghost/tonry_ps1_locus.txt
-drwxr-xr-x   0 alexgagliano   (501) staff       (20)        0 2023-05-22 05:31:42.495573 astro_ghost-1.0.0/astro_ghost.egg-info/
--rw-r--r--   0 alexgagliano   (501) staff       (20)     4089 2023-05-22 05:31:42.000000 astro_ghost-1.0.0/astro_ghost.egg-info/PKG-INFO
--rw-r--r--   0 alexgagliano   (501) staff       (20)     1318 2023-05-22 05:31:42.000000 astro_ghost-1.0.0/astro_ghost.egg-info/SOURCES.txt
--rw-r--r--   0 alexgagliano   (501) staff       (20)        1 2023-05-22 05:31:42.000000 astro_ghost-1.0.0/astro_ghost.egg-info/dependency_links.txt
--rw-r--r--   0 alexgagliano   (501) staff       (20)        1 2023-05-22 05:31:42.000000 astro_ghost-1.0.0/astro_ghost.egg-info/not-zip-safe
--rw-r--r--   0 alexgagliano   (501) staff       (20)      368 2023-05-22 05:31:42.000000 astro_ghost-1.0.0/astro_ghost.egg-info/requires.txt
--rw-r--r--   0 alexgagliano   (501) staff       (20)       18 2023-05-22 05:31:42.000000 astro_ghost-1.0.0/astro_ghost.egg-info/top_level.txt
-drwxr-xr-x   0 alexgagliano   (501) staff       (20)        0 2023-05-22 05:31:42.499203 astro_ghost-1.0.0/docs/
--rw-r--r--   0 alexgagliano   (501) staff       (20)      634 2022-08-10 18:18:27.000000 astro_ghost-1.0.0/docs/Makefile
--rw-r--r--   0 alexgagliano   (501) staff       (20)     2545 2023-05-10 05:04:18.000000 astro_ghost-1.0.0/docs/conf.py
--rw-r--r--   0 alexgagliano   (501) staff       (20)     2641 2023-05-10 20:40:49.000000 astro_ghost-1.0.0/docs/index.rst
--rw-r--r--   0 alexgagliano   (501) staff       (20)      760 2022-08-10 18:18:27.000000 astro_ghost-1.0.0/docs/make.bat
-drwxr-xr-x   0 alexgagliano   (501) staff       (20)        0 2023-05-22 05:31:42.518996 astro_ghost-1.0.0/docs/source/
--rw-r--r--   0 alexgagliano   (501) staff       (20)     1402 2023-05-10 20:31:16.000000 astro_ghost-1.0.0/docs/source/associationmodules.rst
--rw-r--r--   0 alexgagliano   (501) staff       (20)     2612 2023-05-10 19:37:56.000000 astro_ghost-1.0.0/docs/source/basicusage.rst
--rw-r--r--   0 alexgagliano   (501) staff       (20)      819 2023-05-10 20:30:40.000000 astro_ghost-1.0.0/docs/source/catalogmodules.rst
--rw-r--r--   0 alexgagliano   (501) staff       (20)      124 2023-05-10 20:18:30.000000 astro_ghost-1.0.0/docs/source/detailedtutorials.rst
--rw-r--r--   0 alexgagliano   (501) staff       (20)      670 2023-05-10 20:33:11.000000 astro_ghost-1.0.0/docs/source/installation.rst
--rw-r--r--   0 alexgagliano   (501) staff       (20)      844 2023-05-10 20:31:25.000000 astro_ghost-1.0.0/docs/source/preprocessingmodules.rst
--rw-r--r--   0 alexgagliano   (501) staff       (20)      320 2023-05-10 20:31:41.000000 astro_ghost-1.0.0/docs/source/supplementalmodules.rst
--rw-r--r--   0 alexgagliano   (501) staff       (20)      268 2023-05-10 20:38:08.000000 astro_ghost-1.0.0/docs/source/wrappermodules.rst
-drwxr-xr-x   0 alexgagliano   (501) staff       (20)        0 2023-05-22 05:31:42.522446 astro_ghost-1.0.0/licenses/
--rw-r--r--   0 alexgagliano   (501) staff       (20)    37573 2022-08-10 18:18:27.000000 astro_ghost-1.0.0/licenses/LICENSE.rst
--rw-r--r--   0 alexgagliano   (501) staff       (20)      372 2022-08-10 18:18:27.000000 astro_ghost-1.0.0/licenses/README.rst
--rw-r--r--   0 alexgagliano   (501) staff       (20)      134 2022-08-10 18:18:27.000000 astro_ghost-1.0.0/pyproject.toml
--rw-r--r--   0 alexgagliano   (501) staff       (20)     1519 2023-05-22 05:31:42.534234 astro_ghost-1.0.0/setup.cfg
--rwxr-xr-x   0 alexgagliano   (501) staff       (20)     1834 2023-05-22 05:31:01.000000 astro_ghost-1.0.0/setup.py
-drwxr-xr-x   0 alexgagliano   (501) staff       (20)        0 2023-05-22 05:31:42.526960 astro_ghost-1.0.0/tests/
--rw-r--r--   0 alexgagliano   (501) staff       (20)      108 2023-02-16 19:42:21.000000 astro_ghost-1.0.0/tests/__init__.py
--rw-r--r--   0 alexgagliano   (501) staff       (20)      648 2023-05-22 03:39:53.000000 astro_ghost-1.0.0/tests/debug.py
--rw-r--r--   0 alexgagliano   (501) staff       (20)        0 2023-05-10 21:17:11.000000 astro_ghost-1.0.0/tests/pytest.ini
--rw-r--r--   0 alexgagliano   (501) staff       (20)     4201 2023-05-22 05:29:50.000000 astro_ghost-1.0.0/tests/test_tutorial.py
--rw-r--r--   0 alexgagliano   (501) staff       (20)     1343 2023-05-22 03:39:53.000000 astro_ghost-1.0.0/tox.ini
+drwxr-xr-x   0 alexgagliano   (501) staff       (20)        0 2023-05-22 05:38:09.028988 astro_ghost-1.0.1/
+drwxr-xr-x   0 alexgagliano   (501) staff       (20)        0 2023-05-22 05:38:08.927014 astro_ghost-1.0.1/.github/
+drwxr-xr-x   0 alexgagliano   (501) staff       (20)        0 2023-05-22 05:38:08.935577 astro_ghost-1.0.1/.github/workflows/
+-rw-r--r--   0 alexgagliano   (501) staff       (20)      377 2022-08-10 18:18:27.000000 astro_ghost-1.0.1/.github/workflows/docs.yml
+-rw-r--r--   0 alexgagliano   (501) staff       (20)      626 2023-05-09 16:17:11.000000 astro_ghost-1.0.1/.github/workflows/tests.yml
+-rw-r--r--   0 alexgagliano   (501) staff       (20)      769 2022-08-10 18:18:27.000000 astro_ghost-1.0.1/.gitignore
+-rw-r--r--   0 alexgagliano   (501) staff       (20)      170 2022-08-10 18:18:27.000000 astro_ghost-1.0.1/.readthedocs.yml
+-rw-r--r--   0 alexgagliano   (501) staff       (20)      341 2022-08-10 18:18:27.000000 astro_ghost-1.0.1/MANIFEST.in
+-rw-r--r--   0 alexgagliano   (501) staff       (20)     4089 2023-05-22 05:38:09.029389 astro_ghost-1.0.1/PKG-INFO
+-rw-r--r--   0 alexgagliano   (501) staff       (20)     3488 2023-05-10 20:43:06.000000 astro_ghost-1.0.1/README.rst
+drwxr-xr-x   0 alexgagliano   (501) staff       (20)        0 2023-05-22 05:38:09.008074 astro_ghost-1.0.1/astro_ghost/
+-rw-r--r--   0 alexgagliano   (501) staff       (20)    14598 2023-05-22 05:20:41.000000 astro_ghost-1.0.1/astro_ghost/DLR.py
+-rw-r--r--   0 alexgagliano   (501) staff       (20)     4668 2023-05-10 23:12:18.000000 astro_ghost-1.0.1/astro_ghost/NEDQueryFunctions.py
+-rw-r--r--   0 alexgagliano   (501) staff       (20)    38679 2023-05-22 03:39:53.000000 astro_ghost-1.0.1/astro_ghost/PS1QueryFunctions.py
+-rw-r--r--   0 alexgagliano   (501) staff       (20)     1296 2023-05-10 22:09:14.000000 astro_ghost-1.0.1/astro_ghost/SimbadQueryFunctions.py
+-rw-r--r--   0 alexgagliano   (501) staff       (20) 13643353 2023-05-08 18:43:43.000000 astro_ghost-1.0.1/astro_ghost/Star_Galaxy_RealisticModel_GHOST_PS1ClassLabels.sav
+-rw-r--r--   0 alexgagliano   (501) staff       (20)     1475 2023-05-11 05:34:31.000000 astro_ghost-1.0.1/astro_ghost/TNSQueryFunctions.py
+-rw-r--r--   0 alexgagliano   (501) staff       (20)      112 2023-02-17 00:45:54.000000 astro_ghost-1.0.1/astro_ghost/__init__.py
+-rw-r--r--   0 alexgagliano   (501) staff       (20)       22 2023-05-22 05:37:32.000000 astro_ghost-1.0.1/astro_ghost/_version.py
+-rw-r--r--   0 alexgagliano   (501) staff       (20)     1957 2023-02-17 00:45:54.000000 astro_ghost-1.0.1/astro_ghost/conftest.py
+-rw-r--r--   0 alexgagliano   (501) staff       (20)    37989 2023-05-22 05:21:18.000000 astro_ghost-1.0.1/astro_ghost/ghostHelperFunctions.py
+-rw-r--r--   0 alexgagliano   (501) staff       (20)    32867 2023-05-22 05:22:39.000000 astro_ghost-1.0.1/astro_ghost/gradientAscent.py
+-rw-r--r--   0 alexgagliano   (501) staff       (20)     2838 2023-05-09 20:46:38.000000 astro_ghost-1.0.1/astro_ghost/hostMatching.py
+-rw-r--r--   0 alexgagliano   (501) staff       (20)    17727 2023-05-22 03:39:53.000000 astro_ghost-1.0.1/astro_ghost/photoz_helper.py
+-rw-r--r--   0 alexgagliano   (501) staff       (20)     9852 2023-05-22 04:36:12.000000 astro_ghost-1.0.1/astro_ghost/sourceCleaning.py
+-rw-r--r--   0 alexgagliano   (501) staff       (20)     7788 2023-05-22 05:37:05.000000 astro_ghost-1.0.1/astro_ghost/starSeparation.py
+-rw-r--r--   0 alexgagliano   (501) staff       (20)     4611 2023-05-11 04:35:06.000000 astro_ghost-1.0.1/astro_ghost/stellarLocus.py
+-rw-r--r--   0 alexgagliano   (501) staff       (20)      302 2023-02-17 00:45:54.000000 astro_ghost-1.0.1/astro_ghost/tonry_ps1_locus.txt
+drwxr-xr-x   0 alexgagliano   (501) staff       (20)        0 2023-05-22 05:38:09.011767 astro_ghost-1.0.1/astro_ghost.egg-info/
+-rw-r--r--   0 alexgagliano   (501) staff       (20)     4089 2023-05-22 05:38:08.000000 astro_ghost-1.0.1/astro_ghost.egg-info/PKG-INFO
+-rw-r--r--   0 alexgagliano   (501) staff       (20)     1318 2023-05-22 05:38:08.000000 astro_ghost-1.0.1/astro_ghost.egg-info/SOURCES.txt
+-rw-r--r--   0 alexgagliano   (501) staff       (20)        1 2023-05-22 05:38:08.000000 astro_ghost-1.0.1/astro_ghost.egg-info/dependency_links.txt
+-rw-r--r--   0 alexgagliano   (501) staff       (20)        1 2023-05-22 05:38:08.000000 astro_ghost-1.0.1/astro_ghost.egg-info/not-zip-safe
+-rw-r--r--   0 alexgagliano   (501) staff       (20)      368 2023-05-22 05:38:08.000000 astro_ghost-1.0.1/astro_ghost.egg-info/requires.txt
+-rw-r--r--   0 alexgagliano   (501) staff       (20)       18 2023-05-22 05:38:08.000000 astro_ghost-1.0.1/astro_ghost.egg-info/top_level.txt
+drwxr-xr-x   0 alexgagliano   (501) staff       (20)        0 2023-05-22 05:38:09.015351 astro_ghost-1.0.1/docs/
+-rw-r--r--   0 alexgagliano   (501) staff       (20)      634 2022-08-10 18:18:27.000000 astro_ghost-1.0.1/docs/Makefile
+-rw-r--r--   0 alexgagliano   (501) staff       (20)     2545 2023-05-10 05:04:18.000000 astro_ghost-1.0.1/docs/conf.py
+-rw-r--r--   0 alexgagliano   (501) staff       (20)     2641 2023-05-10 20:40:49.000000 astro_ghost-1.0.1/docs/index.rst
+-rw-r--r--   0 alexgagliano   (501) staff       (20)      760 2022-08-10 18:18:27.000000 astro_ghost-1.0.1/docs/make.bat
+drwxr-xr-x   0 alexgagliano   (501) staff       (20)        0 2023-05-22 05:38:09.022611 astro_ghost-1.0.1/docs/source/
+-rw-r--r--   0 alexgagliano   (501) staff       (20)     1402 2023-05-10 20:31:16.000000 astro_ghost-1.0.1/docs/source/associationmodules.rst
+-rw-r--r--   0 alexgagliano   (501) staff       (20)     2612 2023-05-10 19:37:56.000000 astro_ghost-1.0.1/docs/source/basicusage.rst
+-rw-r--r--   0 alexgagliano   (501) staff       (20)      819 2023-05-10 20:30:40.000000 astro_ghost-1.0.1/docs/source/catalogmodules.rst
+-rw-r--r--   0 alexgagliano   (501) staff       (20)      124 2023-05-10 20:18:30.000000 astro_ghost-1.0.1/docs/source/detailedtutorials.rst
+-rw-r--r--   0 alexgagliano   (501) staff       (20)      670 2023-05-10 20:33:11.000000 astro_ghost-1.0.1/docs/source/installation.rst
+-rw-r--r--   0 alexgagliano   (501) staff       (20)      844 2023-05-10 20:31:25.000000 astro_ghost-1.0.1/docs/source/preprocessingmodules.rst
+-rw-r--r--   0 alexgagliano   (501) staff       (20)      320 2023-05-10 20:31:41.000000 astro_ghost-1.0.1/docs/source/supplementalmodules.rst
+-rw-r--r--   0 alexgagliano   (501) staff       (20)      268 2023-05-10 20:38:08.000000 astro_ghost-1.0.1/docs/source/wrappermodules.rst
+drwxr-xr-x   0 alexgagliano   (501) staff       (20)        0 2023-05-22 05:38:09.025156 astro_ghost-1.0.1/licenses/
+-rw-r--r--   0 alexgagliano   (501) staff       (20)    37573 2022-08-10 18:18:27.000000 astro_ghost-1.0.1/licenses/LICENSE.rst
+-rw-r--r--   0 alexgagliano   (501) staff       (20)      372 2022-08-10 18:18:27.000000 astro_ghost-1.0.1/licenses/README.rst
+-rw-r--r--   0 alexgagliano   (501) staff       (20)      134 2022-08-10 18:18:27.000000 astro_ghost-1.0.1/pyproject.toml
+-rw-r--r--   0 alexgagliano   (501) staff       (20)     1519 2023-05-22 05:38:09.031774 astro_ghost-1.0.1/setup.cfg
+-rwxr-xr-x   0 alexgagliano   (501) staff       (20)     1834 2023-05-22 05:37:42.000000 astro_ghost-1.0.1/setup.py
+drwxr-xr-x   0 alexgagliano   (501) staff       (20)        0 2023-05-22 05:38:09.028463 astro_ghost-1.0.1/tests/
+-rw-r--r--   0 alexgagliano   (501) staff       (20)      108 2023-02-16 19:42:21.000000 astro_ghost-1.0.1/tests/__init__.py
+-rw-r--r--   0 alexgagliano   (501) staff       (20)      648 2023-05-22 03:39:53.000000 astro_ghost-1.0.1/tests/debug.py
+-rw-r--r--   0 alexgagliano   (501) staff       (20)        0 2023-05-10 21:17:11.000000 astro_ghost-1.0.1/tests/pytest.ini
+-rw-r--r--   0 alexgagliano   (501) staff       (20)     4213 2023-05-22 05:37:16.000000 astro_ghost-1.0.1/tests/test_tutorial.py
+-rw-r--r--   0 alexgagliano   (501) staff       (20)     1343 2023-05-22 03:39:53.000000 astro_ghost-1.0.1/tox.ini
```

### Comparing `astro_ghost-1.0.0/.github/workflows/tests.yml` & `astro_ghost-1.0.1/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `astro_ghost-1.0.0/.gitignore` & `astro_ghost-1.0.1/.gitignore`

 * *Files identical despite different names*

### Comparing `astro_ghost-1.0.0/PKG-INFO` & `astro_ghost-1.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: astro_ghost
-Version: 1.0.0
+Version: 1.0.1
 Summary: A package to associate transients with host galaxies, and a database of 16k SNe-host galaxies in PS1.
 Home-page: https://github.com/pypa/sampleproject
 Author: Alex Gagliano
 Author-email: gaglian2@illinois.edu
 License: GNU GPL v3+
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `astro_ghost-1.0.0/README.rst` & `astro_ghost-1.0.1/README.rst`

 * *Files identical despite different names*

### Comparing `astro_ghost-1.0.0/astro_ghost/DLR.py` & `astro_ghost-1.0.1/astro_ghost/DLR.py`

 * *Files identical despite different names*

### Comparing `astro_ghost-1.0.0/astro_ghost/NEDQueryFunctions.py` & `astro_ghost-1.0.1/astro_ghost/NEDQueryFunctions.py`

 * *Files identical despite different names*

### Comparing `astro_ghost-1.0.0/astro_ghost/PS1QueryFunctions.py` & `astro_ghost-1.0.1/astro_ghost/PS1QueryFunctions.py`

 * *Files identical despite different names*

### Comparing `astro_ghost-1.0.0/astro_ghost/SimbadQueryFunctions.py` & `astro_ghost-1.0.1/astro_ghost/SimbadQueryFunctions.py`

 * *Files identical despite different names*

### Comparing `astro_ghost-1.0.0/astro_ghost/Star_Galaxy_RealisticModel_GHOST_PS1ClassLabels.sav` & `astro_ghost-1.0.1/astro_ghost/Star_Galaxy_RealisticModel_GHOST_PS1ClassLabels.sav`

 * *Files identical despite different names*

### Comparing `astro_ghost-1.0.0/astro_ghost/TNSQueryFunctions.py` & `astro_ghost-1.0.1/astro_ghost/TNSQueryFunctions.py`

 * *Files identical despite different names*

### Comparing `astro_ghost-1.0.0/astro_ghost/conftest.py` & `astro_ghost-1.0.1/astro_ghost/conftest.py`

 * *Files identical despite different names*

### Comparing `astro_ghost-1.0.0/astro_ghost/ghostHelperFunctions.py` & `astro_ghost-1.0.1/astro_ghost/ghostHelperFunctions.py`

 * *Files identical despite different names*

### Comparing `astro_ghost-1.0.0/astro_ghost/gradientAscent.py` & `astro_ghost-1.0.1/astro_ghost/gradientAscent.py`

 * *Files identical despite different names*

### Comparing `astro_ghost-1.0.0/astro_ghost/hostMatching.py` & `astro_ghost-1.0.1/astro_ghost/hostMatching.py`

 * *Files identical despite different names*

### Comparing `astro_ghost-1.0.0/astro_ghost/photoz_helper.py` & `astro_ghost-1.0.1/astro_ghost/photoz_helper.py`

 * *Files identical despite different names*

### Comparing `astro_ghost-1.0.0/astro_ghost/sourceCleaning.py` & `astro_ghost-1.0.1/astro_ghost/sourceCleaning.py`

 * *Files identical despite different names*

### Comparing `astro_ghost-1.0.0/astro_ghost/starSeparation.py` & `astro_ghost-1.0.1/astro_ghost/starSeparation.py`

 * *Files 3% similar despite different names*

```diff
@@ -27,14 +27,18 @@
     :rtype: Pandas DataFrame
     """
 
     #remove known galaxies and stars
     NED_stars = df[df['NED_type'].isin(['*', '**', 'WD*', '!*', '!V*', 'V*', '!Nova'])]
     NED_gals = df[df['NED_type'] == 'G']
 
+    #label the sources we know to be stars and galaxies
+    NED_stars['sourceClass'] = 1
+    NED_gals['sourceClass'] = 0
+
     #get the remaining objects
     unsure = df[~df.index.isin(NED_stars.index)]
     unsure = unsure[~unsure.index.isin(NED_gals.index)]
 
     #also drop HII regions, QSOs, etc
     unsure = unsure[~unsure['NED_type'].isin(['HII', 'QSO', 'SNR', 'PN'])]
 
@@ -71,17 +75,17 @@
     cutdict = {'normal':0.5, 'aggressive':0.3, 'gentle':0.8}
 
     try:
         test_y = model.predict_proba(test_X)[:,1] > cutdict[starcut]
     except:
         print("Error! I didn't understand your starcut option.")
 
-    unsure_dropped['class'] = test_y
-    test_stars = unsure_dropped[unsure_dropped['class'] == 1]
-    test_gals = unsure_dropped[unsure_dropped['class'] == 0]
+    unsure_dropped['sourceClass'] = test_y
+    test_stars = unsure_dropped[unsure_dropped['sourceClass'] == 1]
+    test_gals = unsure_dropped[unsure_dropped['sourceClass'] == 0]
 
     # plot the distribution of classified stars and galaxies.
     if plot:
         c_gals = '#087e8b'
         c_stars = '#ffbf00'
 
         plt.figure(num=None, figsize=(8, 6), dpi=80, facecolor='w', edgecolor='k')
@@ -156,13 +160,15 @@
     except:
         print("Error! I didn't understand your starcut option.")
 
     test_gals = unsure_dropped[~unsure_dropped.index.isin(test_stars.index)]
 
     # Adding back in the ones we identified as galaxies from our clustering above, and the NED sources.
     df_gals = pd.concat([test_gals, NED_gals])
+    df_gals['sourceClass'] = 0
     df_gals.reset_index(inplace=True, drop=True)
 
     # Adding back in the ones we identified as stars from our clustering above, and the NED sources.
     df_stars = pd.concat([test_stars, NED_stars])
+    df_stars['sourceClass'] = 1
     df_stars.reset_index(inplace=True, drop=True)
     return df_gals, df_stars
```

### Comparing `astro_ghost-1.0.0/astro_ghost/stellarLocus.py` & `astro_ghost-1.0.1/astro_ghost/stellarLocus.py`

 * *Files identical despite different names*

### Comparing `astro_ghost-1.0.0/astro_ghost.egg-info/PKG-INFO` & `astro_ghost-1.0.1/astro_ghost.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: astro-ghost
-Version: 1.0.0
+Version: 1.0.1
 Summary: A package to associate transients with host galaxies, and a database of 16k SNe-host galaxies in PS1.
 Home-page: https://github.com/pypa/sampleproject
 Author: Alex Gagliano
 Author-email: gaglian2@illinois.edu
 License: GNU GPL v3+
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `astro_ghost-1.0.0/astro_ghost.egg-info/SOURCES.txt` & `astro_ghost-1.0.1/astro_ghost.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `astro_ghost-1.0.0/docs/Makefile` & `astro_ghost-1.0.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `astro_ghost-1.0.0/docs/conf.py` & `astro_ghost-1.0.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `astro_ghost-1.0.0/docs/index.rst` & `astro_ghost-1.0.1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `astro_ghost-1.0.0/docs/make.bat` & `astro_ghost-1.0.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `astro_ghost-1.0.0/docs/source/associationmodules.rst` & `astro_ghost-1.0.1/docs/source/associationmodules.rst`

 * *Files identical despite different names*

### Comparing `astro_ghost-1.0.0/docs/source/basicusage.rst` & `astro_ghost-1.0.1/docs/source/basicusage.rst`

 * *Files identical despite different names*

### Comparing `astro_ghost-1.0.0/docs/source/catalogmodules.rst` & `astro_ghost-1.0.1/docs/source/catalogmodules.rst`

 * *Files identical despite different names*

### Comparing `astro_ghost-1.0.0/docs/source/installation.rst` & `astro_ghost-1.0.1/docs/source/installation.rst`

 * *Files identical despite different names*

### Comparing `astro_ghost-1.0.0/docs/source/preprocessingmodules.rst` & `astro_ghost-1.0.1/docs/source/preprocessingmodules.rst`

 * *Files identical despite different names*

### Comparing `astro_ghost-1.0.0/licenses/LICENSE.rst` & `astro_ghost-1.0.1/licenses/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `astro_ghost-1.0.0/setup.cfg` & `astro_ghost-1.0.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `astro_ghost-1.0.0/setup.py` & `astro_ghost-1.0.1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #!/usr/bin/env python
 # Licensed under a 3-clause BSD style license - see LICENSE.rst
 
 import os
 
 from setuptools import setup
 
-version = "1.0.0"
+version = "1.0.1"
 
 VERSION_TEMPLATE = """
  Note that we need to fall back to the hard-coded version if either
  setuptools_scm can't be imported or setuptools_scm can't determine the
  version, so we catch the generic 'Exception'.
 __version__ = '{version}'
 """.lstrip()
```

### Comparing `astro_ghost-1.0.0/tests/debug.py` & `astro_ghost-1.0.1/tests/debug.py`

 * *Files identical despite different names*

### Comparing `astro_ghost-1.0.0/tests/test_tutorial.py` & `astro_ghost-1.0.1/tests/test_tutorial.py`

 * *Files 2% similar despite different names*

```diff
@@ -72,17 +72,17 @@
         sourceSet.append(a.to_pandas().iloc[[0]])
     sourceDF = pd.concat(sourceSet, ignore_index=True)
     sourceDF['trueSourceClass'] = sourceType
     sourceDF = getColors(sourceDF)
     sourceDF = calc_7DCD(sourceDF)
     sourceDF = getNEDInfo(sourceDF)
     gals, stars = separateStars_STRM(sourceDF)
-    #True is stars, False is gals. Passes if all gals are False and all stars are True!
-    assert (np.nansum(gals['class'] == False) + np.nansum(stars['class'])) == len(sourceDF)
 
+    #True is stars, False is gals. Passes if all gals are False and all stars are True!
+    assert (np.nansum(gals['sourceClass'] == False) + np.nansum(stars['sourceClass'])) == len(sourceDF)
 
 def test_plotLocus():
     #plot a subset of GHOST data compared to the tonry stellar locus
     GHOST = fullData()
     plotLocus(GHOST.iloc[0:500], color=False, save=True, type="Gals", timestamp="")
     assert len(glob.glob(os.path.join(os.getcwd(), 'PS1_Gals_StellarLocus_.pdf'))) > 0
```

### Comparing `astro_ghost-1.0.0/tox.ini` & `astro_ghost-1.0.1/tox.ini`

 * *Files identical despite different names*

