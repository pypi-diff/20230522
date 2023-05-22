# Comparing `tmp/astro_ghost-1.0.3.tar.gz` & `tmp/astro_ghost-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "astro_ghost-1.0.3.tar", last modified: Mon May 22 07:04:19 2023, max compression
+gzip compressed data, was "astro_ghost-2.0.0.tar", last modified: Mon May 22 16:29:32 2023, max compression
```

## Comparing `astro_ghost-1.0.3.tar` & `astro_ghost-2.0.0.tar`

### file list

```diff
@@ -1,61 +1,61 @@
-drwxr-xr-x   0 alexgagliano   (501) staff       (20)        0 2023-05-22 07:04:19.802250 astro_ghost-1.0.3/
-drwxr-xr-x   0 alexgagliano   (501) staff       (20)        0 2023-05-22 07:04:19.695636 astro_ghost-1.0.3/.github/
-drwxr-xr-x   0 alexgagliano   (501) staff       (20)        0 2023-05-22 07:04:19.711703 astro_ghost-1.0.3/.github/workflows/
--rw-r--r--   0 alexgagliano   (501) staff       (20)      377 2022-08-10 18:18:27.000000 astro_ghost-1.0.3/.github/workflows/docs.yml
--rw-r--r--   0 alexgagliano   (501) staff       (20)      626 2023-05-09 16:17:11.000000 astro_ghost-1.0.3/.github/workflows/tests.yml
--rw-r--r--   0 alexgagliano   (501) staff       (20)      769 2022-08-10 18:18:27.000000 astro_ghost-1.0.3/.gitignore
--rw-r--r--   0 alexgagliano   (501) staff       (20)      170 2022-08-10 18:18:27.000000 astro_ghost-1.0.3/.readthedocs.yml
--rw-r--r--   0 alexgagliano   (501) staff       (20)      341 2022-08-10 18:18:27.000000 astro_ghost-1.0.3/MANIFEST.in
--rw-r--r--   0 alexgagliano   (501) staff       (20)     4089 2023-05-22 07:04:19.802581 astro_ghost-1.0.3/PKG-INFO
--rw-r--r--   0 alexgagliano   (501) staff       (20)     3488 2023-05-10 20:43:06.000000 astro_ghost-1.0.3/README.rst
-drwxr-xr-x   0 alexgagliano   (501) staff       (20)        0 2023-05-22 07:04:19.773540 astro_ghost-1.0.3/astro_ghost/
--rw-r--r--   0 alexgagliano   (501) staff       (20)    14598 2023-05-22 05:20:41.000000 astro_ghost-1.0.3/astro_ghost/DLR.py
--rw-r--r--   0 alexgagliano   (501) staff       (20)     4668 2023-05-10 23:12:18.000000 astro_ghost-1.0.3/astro_ghost/NEDQueryFunctions.py
--rw-r--r--   0 alexgagliano   (501) staff       (20)    38679 2023-05-22 03:39:53.000000 astro_ghost-1.0.3/astro_ghost/PS1QueryFunctions.py
--rw-r--r--   0 alexgagliano   (501) staff       (20)     1296 2023-05-10 22:09:14.000000 astro_ghost-1.0.3/astro_ghost/SimbadQueryFunctions.py
--rw-r--r--   0 alexgagliano   (501) staff       (20) 13643353 2023-05-08 18:43:43.000000 astro_ghost-1.0.3/astro_ghost/Star_Galaxy_RealisticModel_GHOST_PS1ClassLabels.sav
--rw-r--r--   0 alexgagliano   (501) staff       (20)     1475 2023-05-11 05:34:31.000000 astro_ghost-1.0.3/astro_ghost/TNSQueryFunctions.py
--rw-r--r--   0 alexgagliano   (501) staff       (20)      112 2023-02-17 00:45:54.000000 astro_ghost-1.0.3/astro_ghost/__init__.py
--rw-r--r--   0 alexgagliano   (501) staff       (20)       22 2023-05-22 07:02:46.000000 astro_ghost-1.0.3/astro_ghost/_version.py
--rw-r--r--   0 alexgagliano   (501) staff       (20)     1957 2023-02-17 00:45:54.000000 astro_ghost-1.0.3/astro_ghost/conftest.py
--rw-r--r--   0 alexgagliano   (501) staff       (20)    37988 2023-05-22 07:03:33.000000 astro_ghost-1.0.3/astro_ghost/ghostHelperFunctions.py
--rw-r--r--   0 alexgagliano   (501) staff       (20)    32867 2023-05-22 05:22:39.000000 astro_ghost-1.0.3/astro_ghost/gradientAscent.py
--rw-r--r--   0 alexgagliano   (501) staff       (20)     2838 2023-05-09 20:46:38.000000 astro_ghost-1.0.3/astro_ghost/hostMatching.py
--rw-r--r--   0 alexgagliano   (501) staff       (20)    17727 2023-05-22 03:39:53.000000 astro_ghost-1.0.3/astro_ghost/photoz_helper.py
--rw-r--r--   0 alexgagliano   (501) staff       (20)     9852 2023-05-22 04:36:12.000000 astro_ghost-1.0.3/astro_ghost/sourceCleaning.py
--rw-r--r--   0 alexgagliano   (501) staff       (20)     7779 2023-05-22 06:06:54.000000 astro_ghost-1.0.3/astro_ghost/starSeparation.py
--rw-r--r--   0 alexgagliano   (501) staff       (20)     4611 2023-05-11 04:35:06.000000 astro_ghost-1.0.3/astro_ghost/stellarLocus.py
--rw-r--r--   0 alexgagliano   (501) staff       (20)      302 2023-02-17 00:45:54.000000 astro_ghost-1.0.3/astro_ghost/tonry_ps1_locus.txt
-drwxr-xr-x   0 alexgagliano   (501) staff       (20)        0 2023-05-22 07:04:19.778406 astro_ghost-1.0.3/astro_ghost.egg-info/
--rw-r--r--   0 alexgagliano   (501) staff       (20)     4089 2023-05-22 07:04:19.000000 astro_ghost-1.0.3/astro_ghost.egg-info/PKG-INFO
--rw-r--r--   0 alexgagliano   (501) staff       (20)     1318 2023-05-22 07:04:19.000000 astro_ghost-1.0.3/astro_ghost.egg-info/SOURCES.txt
--rw-r--r--   0 alexgagliano   (501) staff       (20)        1 2023-05-22 07:04:19.000000 astro_ghost-1.0.3/astro_ghost.egg-info/dependency_links.txt
--rw-r--r--   0 alexgagliano   (501) staff       (20)        1 2023-05-22 07:04:19.000000 astro_ghost-1.0.3/astro_ghost.egg-info/not-zip-safe
--rw-r--r--   0 alexgagliano   (501) staff       (20)      368 2023-05-22 07:04:19.000000 astro_ghost-1.0.3/astro_ghost.egg-info/requires.txt
--rw-r--r--   0 alexgagliano   (501) staff       (20)       18 2023-05-22 07:04:19.000000 astro_ghost-1.0.3/astro_ghost.egg-info/top_level.txt
-drwxr-xr-x   0 alexgagliano   (501) staff       (20)        0 2023-05-22 07:04:19.782780 astro_ghost-1.0.3/docs/
--rw-r--r--   0 alexgagliano   (501) staff       (20)      634 2022-08-10 18:18:27.000000 astro_ghost-1.0.3/docs/Makefile
--rw-r--r--   0 alexgagliano   (501) staff       (20)     2545 2023-05-10 05:04:18.000000 astro_ghost-1.0.3/docs/conf.py
--rw-r--r--   0 alexgagliano   (501) staff       (20)     2641 2023-05-10 20:40:49.000000 astro_ghost-1.0.3/docs/index.rst
--rw-r--r--   0 alexgagliano   (501) staff       (20)      760 2022-08-10 18:18:27.000000 astro_ghost-1.0.3/docs/make.bat
-drwxr-xr-x   0 alexgagliano   (501) staff       (20)        0 2023-05-22 07:04:19.793605 astro_ghost-1.0.3/docs/source/
--rw-r--r--   0 alexgagliano   (501) staff       (20)     1402 2023-05-10 20:31:16.000000 astro_ghost-1.0.3/docs/source/associationmodules.rst
--rw-r--r--   0 alexgagliano   (501) staff       (20)     2612 2023-05-10 19:37:56.000000 astro_ghost-1.0.3/docs/source/basicusage.rst
--rw-r--r--   0 alexgagliano   (501) staff       (20)      819 2023-05-10 20:30:40.000000 astro_ghost-1.0.3/docs/source/catalogmodules.rst
--rw-r--r--   0 alexgagliano   (501) staff       (20)      124 2023-05-10 20:18:30.000000 astro_ghost-1.0.3/docs/source/detailedtutorials.rst
--rw-r--r--   0 alexgagliano   (501) staff       (20)      670 2023-05-10 20:33:11.000000 astro_ghost-1.0.3/docs/source/installation.rst
--rw-r--r--   0 alexgagliano   (501) staff       (20)      844 2023-05-10 20:31:25.000000 astro_ghost-1.0.3/docs/source/preprocessingmodules.rst
--rw-r--r--   0 alexgagliano   (501) staff       (20)      320 2023-05-10 20:31:41.000000 astro_ghost-1.0.3/docs/source/supplementalmodules.rst
--rw-r--r--   0 alexgagliano   (501) staff       (20)      268 2023-05-10 20:38:08.000000 astro_ghost-1.0.3/docs/source/wrappermodules.rst
-drwxr-xr-x   0 alexgagliano   (501) staff       (20)        0 2023-05-22 07:04:19.797404 astro_ghost-1.0.3/licenses/
--rw-r--r--   0 alexgagliano   (501) staff       (20)    37573 2022-08-10 18:18:27.000000 astro_ghost-1.0.3/licenses/LICENSE.rst
--rw-r--r--   0 alexgagliano   (501) staff       (20)      372 2022-08-10 18:18:27.000000 astro_ghost-1.0.3/licenses/README.rst
--rw-r--r--   0 alexgagliano   (501) staff       (20)      134 2022-08-10 18:18:27.000000 astro_ghost-1.0.3/pyproject.toml
--rw-r--r--   0 alexgagliano   (501) staff       (20)     1519 2023-05-22 07:04:19.804174 astro_ghost-1.0.3/setup.cfg
--rwxr-xr-x   0 alexgagliano   (501) staff       (20)     1834 2023-05-22 07:03:00.000000 astro_ghost-1.0.3/setup.py
-drwxr-xr-x   0 alexgagliano   (501) staff       (20)        0 2023-05-22 07:04:19.801774 astro_ghost-1.0.3/tests/
--rw-r--r--   0 alexgagliano   (501) staff       (20)      108 2023-02-16 19:42:21.000000 astro_ghost-1.0.3/tests/__init__.py
--rw-r--r--   0 alexgagliano   (501) staff       (20)      648 2023-05-22 03:39:53.000000 astro_ghost-1.0.3/tests/debug.py
--rw-r--r--   0 alexgagliano   (501) staff       (20)        0 2023-05-10 21:17:11.000000 astro_ghost-1.0.3/tests/pytest.ini
--rw-r--r--   0 alexgagliano   (501) staff       (20)     4213 2023-05-22 05:37:16.000000 astro_ghost-1.0.3/tests/test_tutorial.py
--rw-r--r--   0 alexgagliano   (501) staff       (20)     1343 2023-05-22 03:39:53.000000 astro_ghost-1.0.3/tox.ini
+drwxr-xr-x   0 alexgagliano   (501) staff       (20)        0 2023-05-22 16:29:32.045274 astro_ghost-2.0.0/
+drwxr-xr-x   0 alexgagliano   (501) staff       (20)        0 2023-05-22 16:29:31.984802 astro_ghost-2.0.0/.github/
+drwxr-xr-x   0 alexgagliano   (501) staff       (20)        0 2023-05-22 16:29:31.989967 astro_ghost-2.0.0/.github/workflows/
+-rw-r--r--   0 alexgagliano   (501) staff       (20)      377 2022-08-10 18:18:27.000000 astro_ghost-2.0.0/.github/workflows/docs.yml
+-rw-r--r--   0 alexgagliano   (501) staff       (20)      626 2023-05-09 16:17:11.000000 astro_ghost-2.0.0/.github/workflows/tests.yml
+-rw-r--r--   0 alexgagliano   (501) staff       (20)      769 2022-08-10 18:18:27.000000 astro_ghost-2.0.0/.gitignore
+-rw-r--r--   0 alexgagliano   (501) staff       (20)      170 2022-08-10 18:18:27.000000 astro_ghost-2.0.0/.readthedocs.yml
+-rw-r--r--   0 alexgagliano   (501) staff       (20)      341 2022-08-10 18:18:27.000000 astro_ghost-2.0.0/MANIFEST.in
+-rw-r--r--   0 alexgagliano   (501) staff       (20)     4089 2023-05-22 16:29:32.045579 astro_ghost-2.0.0/PKG-INFO
+-rw-r--r--   0 alexgagliano   (501) staff       (20)     3488 2023-05-10 20:43:06.000000 astro_ghost-2.0.0/README.rst
+drwxr-xr-x   0 alexgagliano   (501) staff       (20)        0 2023-05-22 16:29:32.027095 astro_ghost-2.0.0/astro_ghost/
+-rw-r--r--   0 alexgagliano   (501) staff       (20)    20843 2023-05-22 16:28:30.000000 astro_ghost-2.0.0/astro_ghost/DLR.py
+-rw-r--r--   0 alexgagliano   (501) staff       (20)     4668 2023-05-22 16:28:50.000000 astro_ghost-2.0.0/astro_ghost/NEDQueryFunctions.py
+-rw-r--r--   0 alexgagliano   (501) staff       (20)    38679 2023-05-22 16:28:56.000000 astro_ghost-2.0.0/astro_ghost/PS1QueryFunctions.py
+-rw-r--r--   0 alexgagliano   (501) staff       (20)     1296 2023-05-10 22:09:14.000000 astro_ghost-2.0.0/astro_ghost/SimbadQueryFunctions.py
+-rw-r--r--   0 alexgagliano   (501) staff       (20) 13643353 2023-05-08 18:43:43.000000 astro_ghost-2.0.0/astro_ghost/Star_Galaxy_RealisticModel_GHOST_PS1ClassLabels.sav
+-rw-r--r--   0 alexgagliano   (501) staff       (20)     1475 2023-05-11 05:34:31.000000 astro_ghost-2.0.0/astro_ghost/TNSQueryFunctions.py
+-rw-r--r--   0 alexgagliano   (501) staff       (20)      112 2023-02-17 00:45:54.000000 astro_ghost-2.0.0/astro_ghost/__init__.py
+-rw-r--r--   0 alexgagliano   (501) staff       (20)       22 2023-05-22 16:29:06.000000 astro_ghost-2.0.0/astro_ghost/_version.py
+-rw-r--r--   0 alexgagliano   (501) staff       (20)     1957 2023-02-17 00:45:54.000000 astro_ghost-2.0.0/astro_ghost/conftest.py
+-rw-r--r--   0 alexgagliano   (501) staff       (20)    40036 2023-05-22 16:28:35.000000 astro_ghost-2.0.0/astro_ghost/ghostHelperFunctions.py
+-rw-r--r--   0 alexgagliano   (501) staff       (20)    32867 2023-05-22 05:22:39.000000 astro_ghost-2.0.0/astro_ghost/gradientAscent.py
+-rw-r--r--   0 alexgagliano   (501) staff       (20)     2838 2023-05-09 20:46:38.000000 astro_ghost-2.0.0/astro_ghost/hostMatching.py
+-rw-r--r--   0 alexgagliano   (501) staff       (20)    17727 2023-05-22 03:39:53.000000 astro_ghost-2.0.0/astro_ghost/photoz_helper.py
+-rw-r--r--   0 alexgagliano   (501) staff       (20)     9853 2023-05-22 16:28:44.000000 astro_ghost-2.0.0/astro_ghost/sourceCleaning.py
+-rw-r--r--   0 alexgagliano   (501) staff       (20)     7779 2023-05-22 06:06:54.000000 astro_ghost-2.0.0/astro_ghost/starSeparation.py
+-rw-r--r--   0 alexgagliano   (501) staff       (20)     4611 2023-05-11 04:35:06.000000 astro_ghost-2.0.0/astro_ghost/stellarLocus.py
+-rw-r--r--   0 alexgagliano   (501) staff       (20)      302 2023-02-17 00:45:54.000000 astro_ghost-2.0.0/astro_ghost/tonry_ps1_locus.txt
+drwxr-xr-x   0 alexgagliano   (501) staff       (20)        0 2023-05-22 16:29:32.029362 astro_ghost-2.0.0/astro_ghost.egg-info/
+-rw-r--r--   0 alexgagliano   (501) staff       (20)     4089 2023-05-22 16:29:31.000000 astro_ghost-2.0.0/astro_ghost.egg-info/PKG-INFO
+-rw-r--r--   0 alexgagliano   (501) staff       (20)     1318 2023-05-22 16:29:31.000000 astro_ghost-2.0.0/astro_ghost.egg-info/SOURCES.txt
+-rw-r--r--   0 alexgagliano   (501) staff       (20)        1 2023-05-22 16:29:31.000000 astro_ghost-2.0.0/astro_ghost.egg-info/dependency_links.txt
+-rw-r--r--   0 alexgagliano   (501) staff       (20)        1 2023-05-22 16:29:31.000000 astro_ghost-2.0.0/astro_ghost.egg-info/not-zip-safe
+-rw-r--r--   0 alexgagliano   (501) staff       (20)      368 2023-05-22 16:29:31.000000 astro_ghost-2.0.0/astro_ghost.egg-info/requires.txt
+-rw-r--r--   0 alexgagliano   (501) staff       (20)       18 2023-05-22 16:29:31.000000 astro_ghost-2.0.0/astro_ghost.egg-info/top_level.txt
+drwxr-xr-x   0 alexgagliano   (501) staff       (20)        0 2023-05-22 16:29:32.032057 astro_ghost-2.0.0/docs/
+-rw-r--r--   0 alexgagliano   (501) staff       (20)      634 2022-08-10 18:18:27.000000 astro_ghost-2.0.0/docs/Makefile
+-rw-r--r--   0 alexgagliano   (501) staff       (20)     2545 2023-05-10 05:04:18.000000 astro_ghost-2.0.0/docs/conf.py
+-rw-r--r--   0 alexgagliano   (501) staff       (20)     2641 2023-05-10 20:40:49.000000 astro_ghost-2.0.0/docs/index.rst
+-rw-r--r--   0 alexgagliano   (501) staff       (20)      760 2022-08-10 18:18:27.000000 astro_ghost-2.0.0/docs/make.bat
+drwxr-xr-x   0 alexgagliano   (501) staff       (20)        0 2023-05-22 16:29:32.038457 astro_ghost-2.0.0/docs/source/
+-rw-r--r--   0 alexgagliano   (501) staff       (20)     1402 2023-05-10 20:31:16.000000 astro_ghost-2.0.0/docs/source/associationmodules.rst
+-rw-r--r--   0 alexgagliano   (501) staff       (20)     2479 2023-05-22 07:06:49.000000 astro_ghost-2.0.0/docs/source/basicusage.rst
+-rw-r--r--   0 alexgagliano   (501) staff       (20)      819 2023-05-10 20:30:40.000000 astro_ghost-2.0.0/docs/source/catalogmodules.rst
+-rw-r--r--   0 alexgagliano   (501) staff       (20)      124 2023-05-10 20:18:30.000000 astro_ghost-2.0.0/docs/source/detailedtutorials.rst
+-rw-r--r--   0 alexgagliano   (501) staff       (20)      670 2023-05-10 20:33:11.000000 astro_ghost-2.0.0/docs/source/installation.rst
+-rw-r--r--   0 alexgagliano   (501) staff       (20)      844 2023-05-10 20:31:25.000000 astro_ghost-2.0.0/docs/source/preprocessingmodules.rst
+-rw-r--r--   0 alexgagliano   (501) staff       (20)      320 2023-05-10 20:31:41.000000 astro_ghost-2.0.0/docs/source/supplementalmodules.rst
+-rw-r--r--   0 alexgagliano   (501) staff       (20)      268 2023-05-10 20:38:08.000000 astro_ghost-2.0.0/docs/source/wrappermodules.rst
+drwxr-xr-x   0 alexgagliano   (501) staff       (20)        0 2023-05-22 16:29:32.040850 astro_ghost-2.0.0/licenses/
+-rw-r--r--   0 alexgagliano   (501) staff       (20)    37573 2022-08-10 18:18:27.000000 astro_ghost-2.0.0/licenses/LICENSE.rst
+-rw-r--r--   0 alexgagliano   (501) staff       (20)      372 2022-08-10 18:18:27.000000 astro_ghost-2.0.0/licenses/README.rst
+-rw-r--r--   0 alexgagliano   (501) staff       (20)      134 2022-08-10 18:18:27.000000 astro_ghost-2.0.0/pyproject.toml
+-rw-r--r--   0 alexgagliano   (501) staff       (20)     1519 2023-05-22 16:29:32.046539 astro_ghost-2.0.0/setup.cfg
+-rwxr-xr-x   0 alexgagliano   (501) staff       (20)     1834 2023-05-22 16:29:19.000000 astro_ghost-2.0.0/setup.py
+drwxr-xr-x   0 alexgagliano   (501) staff       (20)        0 2023-05-22 16:29:32.044257 astro_ghost-2.0.0/tests/
+-rw-r--r--   0 alexgagliano   (501) staff       (20)      108 2023-02-16 19:42:21.000000 astro_ghost-2.0.0/tests/__init__.py
+-rw-r--r--   0 alexgagliano   (501) staff       (20)      648 2023-05-22 03:39:53.000000 astro_ghost-2.0.0/tests/debug.py
+-rw-r--r--   0 alexgagliano   (501) staff       (20)        0 2023-05-10 21:17:11.000000 astro_ghost-2.0.0/tests/pytest.ini
+-rw-r--r--   0 alexgagliano   (501) staff       (20)     4213 2023-05-22 05:37:16.000000 astro_ghost-2.0.0/tests/test_tutorial.py
+-rw-r--r--   0 alexgagliano   (501) staff       (20)     1343 2023-05-22 03:39:53.000000 astro_ghost-2.0.0/tox.ini
```

### Comparing `astro_ghost-1.0.3/.github/workflows/tests.yml` & `astro_ghost-2.0.0/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `astro_ghost-1.0.3/.gitignore` & `astro_ghost-2.0.0/.gitignore`

 * *Files identical despite different names*

### Comparing `astro_ghost-1.0.3/PKG-INFO` & `astro_ghost-2.0.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: astro_ghost
-Version: 1.0.3
+Version: 2.0.0
 Summary: A package to associate transients with host galaxies, and a database of 16k SNe-host galaxies in PS1.
 Home-page: https://github.com/pypa/sampleproject
 Author: Alex Gagliano
 Author-email: gaglian2@illinois.edu
 License: GNU GPL v3+
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `astro_ghost-1.0.3/README.rst` & `astro_ghost-2.0.0/README.rst`

 * *Files identical despite different names*

### Comparing `astro_ghost-1.0.3/astro_ghost/DLR.py` & `astro_ghost-2.0.0/astro_ghost/DLR.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,16 +1,21 @@
 import numpy as np
+import pandas as pd
 import matplotlib.pyplot as plt
 import matplotlib.patches as mpatches
 from matplotlib import colors
 from astro_ghost.sourceCleaning import clean_dict
+from astro_ghost.NEDQueryFunctions import getNEDInfo
 from astropy import units as u
-from astropy.coordinates import SkyCoord, Angle
+from astropy.coordinates import SkyCoord, Angle, Distance
 from astropy.wcs import WCS
+from astropy.cosmology import FlatLambdaCDM, z_at_value
 from astropy.utils.data import get_pkg_data_filename
+from astroquery.vizier import Vizier
+
 
 def choose_band_SNR(host_df):
     """Gets the PS1 band (of grizy) with the highest SNR in PSF mag.
        From https://www.eso.org/~ohainaut/ccd/sn.html,
        Error on Mag  ~    1/  (S/N)
        So calculating S/N for each band as 1/PSFMagErr
        Estimate the S/N of each band and choose the bands
@@ -29,14 +34,62 @@
              SNR.append(float(1/host_df["%sKronMagErr"%band]))
         i = np.nanargmax(np.array(SNR))
     except:
         #if we have issues getting the band with the highest SNR, just use r-band
         i = 1
     return bands[i]
 
+def calc_DLR_glade(ra_SN, dec_SN, ra_host, dec_host, r_a, a_over_b, phi):
+    """TODO: Short summary.
+
+    Parameters
+    ----------
+    ra_SN : type
+        Description of parameter `ra_SN`.
+    dec_SN : type
+        Description of parameter `dec_SN`.
+    ra_host : type
+        Description of parameter `ra_host`.
+    dec_host : type
+        Description of parameter `dec_host`.
+    r_a : type
+        Description of parameter `r_a`.
+    a_over_b : type
+        Description of parameter `a_over_b`.
+    phi : type
+        Description of parameter `phi`.
+
+    Returns
+    -------
+    type
+        Description of returned object.
+
+    """
+    xr = (ra_SN- float(ra_host))*3600
+    yr = (dec_SN - float(dec_host))*3600
+
+    SNcoord = SkyCoord(ra_SN*u.deg, dec_SN*u.deg, frame='icrs')
+    hostCoord = SkyCoord(ra_host*u.deg, dec_host*u.deg, frame='icrs')
+    sep = SNcoord.separation(hostCoord)
+    dist = sep.arcsecond
+    badR = 10000000000.0
+
+    gam = np.arctan2(xr, yr)
+
+    theta = phi - gam
+
+    DLR = r_a/np.sqrt(((a_over_b)*np.sin(theta))**2 + (np.cos(theta))**2)
+
+    R = float(dist/DLR)
+
+    if (R != R):
+        return dist, badR
+
+    return dist, R
+
 def calc_DLR(ra_SN, dec_SN, ra_host, dec_host, r_a, r_b, source, best_band):
     """Calculate the directional light radius for a given galaxy and transient pair. Calculation is adapted from
        Gupta et al., 2013 found at
        https://repository.upenn.edu/cgi/viewcontent.cgi?referer=https://www.google.com/&httpsredir=1&article=1916&context=edissertations.
 
     :param ra_SN: The right ascension of the SN, in degrees.
     :type ra_SN: float
@@ -315,7 +368,142 @@
     if todo == "s":
         with open('../dictionaries/DLR_rankOrdered_hosts.p', 'wb') as fp:
             pickle.dump(dict_mod, fp, protocol=pickle.HIGHEST_PROTOCOL)
         hosts.to_csv("../tables/DLR_rankOrdered_hosts.csv")
         return
     elif todo =="r":
         return hosts, dict_mod, noHosts, GA_SN
+
+#new method - beta!
+def chooseByGladeDLR(path, fn, snDF, todo='r'):
+    """TODO: Short summary.
+
+    Parameters
+    ----------
+    path : type
+        Description of parameter `path`.
+    fn : type
+        Description of parameter `fn`.
+    snDF : type
+        Description of parameter `snDF`.
+    todo : type
+        Description of parameter `todo`.
+
+    Returns
+    -------
+    type
+        Description of returned object.
+
+    """
+    if todo=="s":
+        if not os.path.exists(path+'/dictionaries'):
+             os.makedirs(path+'/dictionaries')
+        if not os.path.exists(path+'/tables'):
+             os.makedirs(path+'/tables')
+
+    f = open(path+fn, 'w')
+
+    foundHostDF = []
+    noGladeHosts = []
+
+    for idx, row in snDF.iterrows():
+        name = str(row['Name'])
+        ra_SN = float(row['RA'])
+        dec_SN = float(row['DEC'])
+        class_SN = str(row['Obj. Type'])
+
+        #query the glade catalog
+        result = Vizier.query_region(SkyCoord(ra=ra_SN, dec=dec_SN,unit=(u.deg, u.deg),frame='icrs'),width="1d",catalog=["VII/275/glade1"])
+        hosts = result[0].to_pandas()
+        hosts.dropna(subset=['a_b', 'maj', 'min'], inplace=True)
+        if len(hosts)<1:
+            noGladeHosts.append(name)
+            continue
+        hosts['MajorRad'] = hosts['maj']*60/2 #in arcsec, to radius
+        hosts['MinorRad'] = hosts['min']*60/2 #in arcsec, to radius
+
+        #get names for the galaxies that match
+        hosts.rename(columns={'RAJ2000':'raMean','DEJ2000':'decMean'}, inplace=True)
+        hosts = getNEDInfo(hosts)
+
+        R_dict = {}
+        ra_dict = {}
+        dist_dict = {}
+        for idx, row in hosts.iterrows():
+            tempHost = row['NED_name']
+            phi = np.radians(row['PAHyp'])
+            r_a = row['MajorRad']
+
+            #if it's a mostly round galaxy, the position angle doesn't matter!
+            if (phi != phi) & (row['a_b'] >= 0.9):
+                phi = 0
+            dist, R = calc_DLR_glade(ra_SN, dec_SN, row['raMean'], row['decMean'], r_a, row['a_b'], phi)
+
+            R_dict[tempHost] = R
+            ra_dict[tempHost] = r_a
+            dist_dict[tempHost] = dist
+
+            hosts.loc[hosts['NED_name'] == tempHost, 'dist/DLR'] = R
+            hosts.loc[hosts['NED_name'] == tempHost, 'dist'] = dist
+
+        print("\n transient = \\", file=f)
+        print(name, file=f)
+        print("offset/DLR = \\", file=f)
+        #round for printing purposes
+        R_dict_print = {k:round(v,2) if isinstance(v,float) else v for k,v in R_dict.items()}
+        print(R_dict_print, file=f)
+        ra_dict_print = {k:round(v,2) if isinstance(v,float) else v for k,v in ra_dict.items()}
+        print("candidate semi-major axis = \\", file=f)
+        print(ra_dict_print, file=f)
+
+        #subset so that we're less than 5 in DLR units
+        chosenHost = min(R_dict, key=R_dict.get)
+        if R_dict[chosenHost] > 5.0:
+            #If we can't find a host, say that this galaxy has no host
+            noGladeHosts.append(name)
+            print("No host chosen! r/DLR > 5.0.", file=f)
+            continue
+        else:
+            print("Selecting GLADE host: %s"%chosenHost, file=f)
+            foundHost = hosts.loc[hosts['NED_name'] == chosenHost]
+
+            #add in the associated transient's information
+            foundHost['TransientRA'] = ra_SN
+            foundHost['TransientDEC'] = dec_SN
+            foundHost['TransientName'] = name
+            foundHost['TransientClass'] = class_SN
+
+            foundHostDF.append(foundHost)
+
+            f.flush()
+    if len(foundHostDF) > 0:
+        foundHostDF = pd.concat(foundHostDF)
+        # adding some relevant redshift information
+        foundHostDF['GLADE_redshift'] = np.nan
+        foundHostDF['GLADE_redshift_flag'] = ''
+
+        #assume standard cosmology
+        cosmo = FlatLambdaCDM(H0=70, Om0=0.3, Tcmb0=2.725)
+
+        for idx, row in foundHostDF.iterrows():
+            if row['Dist'] == row['Dist']:
+                dist = Distance(value=row['Dist'], unit=u.Mpc)
+                calc_z = z_at_value(cosmo.luminosity_distance, dist, zmin=1.e-5, zmax=1, method='Bounded').value
+                foundHostDF['GLADE_redshift'] = calc_z
+                if row['Flag'] <= 3:
+                    foundHostDF['GLADE_redshift_flag'] = 'SPEC'
+                else:
+                    foundHostDF['GLADE_redshift_flag'] = 'PHOT'
+        #print some relevant information to terminal
+        print("Found %i hosts in GLADE! See %s for details."%(len(foundHostDF), fn))
+        if todo == "s":
+            foundHostDF.to_csv("../tables/gladeDLR_hosts.csv")
+            return
+        elif todo == "r":
+            return foundHostDF, noGladeHosts
+
+    else:
+        foundHostDF = pd.DataFrame({'TransientName':[], 'raMean':[], 'decMean':[]})
+        print("Found no hosts in GLADE.")
+        if todo == 'r':
+            return foundHostDF, noGladeHosts
+    f.close()
```

### Comparing `astro_ghost-1.0.3/astro_ghost/NEDQueryFunctions.py` & `astro_ghost-2.0.0/astro_ghost/NEDQueryFunctions.py`

 * *Files identical despite different names*

### Comparing `astro_ghost-1.0.3/astro_ghost/PS1QueryFunctions.py` & `astro_ghost-2.0.0/astro_ghost/PS1QueryFunctions.py`

 * *Files identical despite different names*

### Comparing `astro_ghost-1.0.3/astro_ghost/SimbadQueryFunctions.py` & `astro_ghost-2.0.0/astro_ghost/SimbadQueryFunctions.py`

 * *Files identical despite different names*

### Comparing `astro_ghost-1.0.3/astro_ghost/Star_Galaxy_RealisticModel_GHOST_PS1ClassLabels.sav` & `astro_ghost-2.0.0/astro_ghost/Star_Galaxy_RealisticModel_GHOST_PS1ClassLabels.sav`

 * *Files identical despite different names*

### Comparing `astro_ghost-1.0.3/astro_ghost/TNSQueryFunctions.py` & `astro_ghost-2.0.0/astro_ghost/TNSQueryFunctions.py`

 * *Files identical despite different names*

### Comparing `astro_ghost-1.0.3/astro_ghost/conftest.py` & `astro_ghost-2.0.0/astro_ghost/conftest.py`

 * *Files identical despite different names*

### Comparing `astro_ghost-1.0.3/astro_ghost/ghostHelperFunctions.py` & `astro_ghost-2.0.0/astro_ghost/ghostHelperFunctions.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,20 +16,60 @@
 from astro_ghost.hostMatching import build_ML_df
 from astro_ghost.NEDQueryFunctions import getNEDInfo
 from astro_ghost.SimbadQueryFunctions import getSimbadInfo
 from astro_ghost.gradientAscent import gradientAscent
 from astro_ghost.starSeparation import separateStars_STRM, separateStars_South
 from astro_ghost.sourceCleaning import clean_dict, removePS1Duplicates, getColors, makeCuts
 from astro_ghost.stellarLocus import calc_7DCD
-from astro_ghost.DLR import chooseByDLR
+from astro_ghost.DLR import chooseByDLR, chooseByGladeDLR
 import requests
 import pickle
 import glob
 from datetime import datetime
 from joblib import dump, load
+import pandas as pd
+
+#we do a lot of copies, sub-selects and rewrites - no need to warn about everything!
+pd.options.mode.chained_assignment = None  # default='warn'
+
+def cleanup(path):
+    """TODO: Short summary.
+
+    Parameters
+    ----------
+    path : type
+        Description of parameter `path`.
+
+    Returns
+    -------
+    type
+        Description of returned object.
+
+    """
+    tablePath = path+"/tables/"
+    printoutPath = path+'/printouts/'
+
+    paths = [tablePath, printoutPath]
+
+    for tempPath in paths:
+        if not os.path.exists(tempPath):
+            os.mkdir(tempPath)
+
+    #move tables to the tables directory, and printouts to the printouts directory
+    printouts = glob.glob(path+'/*.txt')
+    for p in printouts:
+        fn = remove_prefix(p, path)
+        os.rename(p, printoutPath+fn)
+
+    table_ext = ['csv', 'gz']
+    for end in table_ext:
+        tables = glob.glob(path+'/*.%s'%end)
+        for t in tables:
+            fn = remove_prefix(t, path)
+            os.rename(t, tablePath+fn)
 
 def getGHOST(real=False, verbose=False, installpath='', clobber=False):
     """Downloads the GHOST database.
 
     :param real: If True, download the GHOST database. If False, write an empty files with
         relevant columns (so that every transient is manually associated).
     :type real: bool, optional
@@ -519,15 +559,15 @@
                 GHOSTpath = GHOSTpath.split("/")[:-1]
                 GHOSTpath = "/".join(GHOSTpath)
             except:
                 print("Error! I don't know where you installed GHOST -- set GHOST_PATH as an environmental variable or pass in the GHOSTpath parameter.")
     fullTable = pd.read_csv(GHOSTpath+"/database/GHOST.csv")
     return fullTable
 
-def getTransientHosts(transientName=[''], snCoord=[''], snClass=[''], verbose=True, starcut='gentle', ascentMatch=False, px=800, savepath='./', GHOSTpath='', redo_search=True):
+def getTransientHosts(transientName=[''], snCoord=[''], snClass=[''], verbose=False, starcut='normal', ascentMatch=False, px=800, savepath='./', GHOSTpath='', redo_search=True):
     """The wrapper function for the main host association pipeline. The function first
        searches the pre-existing GHOST database by transient name, then by transient coordinates, and finally
        associates the remaining transients not found.
 
     :param transientName: List of transients to associate.
     :type transientName: array-like
     :param snCoord: List of astropy SkyCoord transient positions.
@@ -652,208 +692,217 @@
     transientName_arr = np.array(transientName)
     snRA_arr = np.array(snRA)
     snDEC_arr = np.array(snDEC)
     snClass_arr = np.array(snClass)
 
     dateStr = str(datetime.today()).replace("-", '').replace(".", '').replace(":", "").replace(" ", '')
 
-    fn_Host = "SNe_TNS_%s_PS1Hosts_%iarcsec.csv" % (dateStr, rad)
-    fn_SN = 'transients_%s.csv' % dateStr
-    fn_Dict = fn_Host[:-4] + ".p"
-    dir_name = fn_SN[:-4]
+    fn_host = "SNe_TNS_%s_PS1Hosts_%iarcsec.csv" % (dateStr, rad)
+    fn_transients = 'transients_%s.csv' % dateStr
+    fn_dict = fn_host[:-4] + ".p"
+    dir_name = fn_transients[:-4]
     if not os.path.exists(savepath):
         os.mkdir(savepath)
         os.chmod(savepath, 0o777)
     os.makedirs(savepath + dir_name)
     path = savepath+dir_name+'/'
 
     #create temp dataframe with RA and DEC corresponding to the transient
     snDF = pd.DataFrame({'Name':transientName_arr, 'RA':snRA_arr, 'DEC':snDEC_arr, 'HostName':['']*len(snDEC_arr), 'Obj. Type':snClass_arr})
-    snDF.to_csv(path+fn_SN, index=False)
+    snDF.to_csv(path+fn_transients, index=False)
 
-    #begin doing the heavy lifting to associate transients with hosts
-    host_DF = get_hosts(path, fn_SN, fn_Host, rad)
-    #galaxySizes = getDR2_forcedGalaxySizes(snRA_arr, snDEC_arr, rad)
-    #host_DF_new = host_DF.merge(galaxySizes, on='objID',how='outer')
-    #host_DF = host_DF_new if not galaxySizes.empty else host_DF
-
-    if len(host_DF) < 1:
-        print("ERROR: Found no hosts in cone search during manual association!")
-        return None
-
-    cuts = ["n", "coords", "duplicate"]
-
-    transient_dict =[]
-    # this bit of trickery is required to combine northern-hemisphere and
-    # southern-hemisphere source dictionaries
-    f = open(path+'/dictionaries/'+fn_Dict, "rb")
-    try:
-        while True:
-            transient_dict.append(pickle.load(f))
-    except EOFError:
-        pass
-    temp = transient_dict[0]
-    if len(transient_dict) > 1:
-        for i in np.arange(len(transient_dict)-1):
-            temp.update(transient_dict[i+1])
-    transient_dict = {k.replace(' ', ''): v for k, v in temp.items()}
-    desperate_dict = transient_dict.copy()
+    #new method (beta) - before we do anything else, find and associate low-z hosts with GLADE
+    fn_glade = "gladeDLR.txt"
+    foundGladeHosts, noGladeHosts = chooseByGladeDLR(path, fn_glade, snDF, todo="r")
+
+    #open transients df and drop the transients already found in GLADE. We'll add these back in at the end
+    snDF = snDF[snDF['Name'].isin(noGladeHosts)]
+    fn_transients_preGLADE = fn_transients
+    fn_transients = 'transients_%s_postGlade.csv' % dateStr
+    snDF.to_csv(path+fn_transients, index=False)
+
+    if len(noGladeHosts) < 1:
+        #just return the GLADE df!
+        foundGladeHosts['GLADE_source'] = True
+        host_DF = foundGladeHosts
+    else:
+        #begin doing the heavy lifting after GLADE to associate transients with hosts
+        host_DF = get_hosts(path, fn_transients, fn_host, rad)
 
-    host_DF = getNEDInfo(host_DF)
+        if len(host_DF) < 1:
+            print("ERROR: Found no hosts in cone search during manual association!")
+            return None
+
+        cuts = ["n", "coords", "quality", "duplicate"]
+
+        transient_dict =[]
+        # this bit of trickery is required to combine northern-hemisphere and
+        # southern-hemisphere source dictionaries
+        f = open(path+'/dictionaries/'+fn_dict, "rb")
+        try:
+            while True:
+                transient_dict.append(pickle.load(f))
+        except EOFError:
+            pass
+        temp = transient_dict[0]
+        if len(transient_dict) > 1:
+            for i in np.arange(len(transient_dict)-1):
+                temp.update(transient_dict[i+1])
+        transient_dict = {k.replace(' ', ''): v for k, v in temp.items()}
+        desperate_dict = transient_dict.copy()
+
+        host_DF = getNEDInfo(host_DF)
+
+        host_DF_north = host_DF[host_DF['decMean']>-30].reset_index(drop=True)
+        host_DF_south = host_DF[host_DF['decMean']<=-30].reset_index(drop=True)
+
+        host_DF_north = makeCuts(host_DF_north, cuts, transient_dict)
 
-    host_DF_north = host_DF[host_DF['decMean']>-30].reset_index(drop=True)
-    host_DF_south = host_DF[host_DF['decMean']<=-30].reset_index(drop=True)
+        host_DF = pd.concat([host_DF_north, host_DF_south], ignore_index=True)
 
-    host_DF_north = makeCuts(host_DF_north, cuts, transient_dict)
+        cut_dict = clean_dict(transient_dict, host_DF, [])
+        desperate_dict = cut_dict.copy()
 
-    host_DF = pd.concat([host_DF_north, host_DF_south], ignore_index=True)
+        hostFrac = fracWithHosts(cut_dict)*100
+        if verbose:
+            print("Associated fraction after quality cuts: %.2f%%."%hostFrac)
 
-    cut_dict = clean_dict(transient_dict, host_DF, [])
-    desperate_dict = cut_dict.copy()
+        #automatically add to host association for gradient ascent
+        lost = np.array([k for k, v in cut_dict.items() if len(v) <1])
 
-    hostFrac = fracWithHosts(cut_dict)*100
-    if verbose:
-        print("Associated fraction after quality cuts: %.2f%%."%hostFrac)
+        host_DF_north = getColors(host_DF_north)
+        host_DF_north = removePS1Duplicates(host_DF_north)
+        host_DF_north = calc_7DCD(host_DF_north)
+
+        host_DF = pd.concat([host_DF_north, host_DF_south], ignore_index=True)
+        host_DF = getSimbadInfo(host_DF)
+        host_DF.to_csv(path+"/candidateHosts_NEDSimbad.csv", index=False)
+
+        host_DF_north = host_DF[host_DF['decMean']>-30].reset_index()
+        host_DF_south = host_DF[host_DF['decMean']<=-30].reset_index()
+
+        host_gals_DF_north, stars_DF_north = separateStars_STRM(host_DF_north, plot=0, verbose=verbose, starcut=starcut)
+        host_gals_DF_south, stars_DF_south = separateStars_South(host_DF_south, plot=0, verbose=verbose, starcut=starcut)
+        host_gals_DF = pd.concat([host_gals_DF_north, host_gals_DF_south],ignore_index=True)
+        stars_DF = pd.concat([stars_DF_north, stars_DF_south],ignore_index=True)
 
-    #automatically add to host association for gradient ascent
-    lost = np.array([k for k, v in cut_dict.items() if len(v) <1])
+        if verbose:
+            print("Removed %i stars. We now have %i candidate host galaxies."%(len(stars_DF), len(host_gals_DF)))
 
-    host_DF_north = getColors(host_DF_north)
-    host_DF_north = removePS1Duplicates(host_DF_north)
-    host_DF_north = calc_7DCD(host_DF_north)
-
-    host_DF = pd.concat([host_DF_north, host_DF_south], ignore_index=True)
-    host_DF = getSimbadInfo(host_DF)
-    host_DF.to_csv(path+"/candidateHosts_NEDSimbad.csv", index=False)
-
-    host_DF_north = host_DF[host_DF['decMean']>-30].reset_index()
-    host_DF_south = host_DF[host_DF['decMean']<=-30].reset_index()
-
-    host_gals_DF_north, stars_DF_north = separateStars_STRM(host_DF_north, plot=0, verbose=verbose, starcut=starcut)
-    host_gals_DF_south, stars_DF_south = separateStars_South(host_DF_south, plot=0, verbose=verbose, starcut=starcut)
-    host_gals_DF = pd.concat([host_gals_DF_north, host_gals_DF_south],ignore_index=True)
-    stars_DF = pd.concat([stars_DF_north, stars_DF_south],ignore_index=True)
+        cut_dict = clean_dict(cut_dict, host_gals_DF, [])
+        stars_DF.to_csv(path+"removedStars.csv",index=False)
 
-    if verbose:
-        print("Removed %i stars. We now have %i candidate host galaxies."%(len(stars_DF), len(host_gals_DF)))
+        #in debugging mode, plotting the ML-identified stars and galaxies along the
+        #stellar locus can be super helpful!!
+        #plotLocus(host_gals_DF, color=1, save=1, type="Gals", timestamp=dateStr)
+        #plotLocus(stars_DF, color=1, save=1, type="Stars", timestamp=dateStr)
+
+        host_dict_nospace = {k.replace(' ', ''): v for k, v in cut_dict.items()}
+
+        fn = "DLR.txt"
+        transients = pd.read_csv(path+fn_transients)
+
+        with open(path+"/dictionaries/checkpoint_preDLR.p", 'wb') as fp:
+               dump(host_dict_nospace, fp)
+
+        host_DF, host_dict_nospace_postDLR, noHosts, GD_SN = chooseByDLR(path, host_gals_DF, transients, fn, host_dict_nospace, todo="r")
+
+        #last-ditch effort -- for the ones with no found host, just pick the nearest NED galaxy.
+        for transient in noHosts:
+              tempDF = host_gals_DF[host_gals_DF['objID'].isin(desperate_dict[transient])]
+              tempDF_gals = tempDF[tempDF['NED_type'].isin(['G', 'PofG', 'GPair', 'GGroup', 'GClstr'])].reset_index()
+              if len(tempDF_gals) < 1:
+                 continue
+              transientRA = transients.loc[transients['Name'] == transient, 'RA'].values[0]
+              transientDEC = transients.loc[transients['Name'] == transient, 'DEC'].values[0]
+              transientCoord = SkyCoord(transientRA*u.deg, transientDEC*u.deg, frame='icrs')
+              tempHostCoords = SkyCoord(tempDF_gals['raMean'].values*u.deg, tempDF_gals['decMean'].values*u.deg, frame='icrs')
+              sep = transientCoord.separation(tempHostCoords)
+              desperateMatch = tempDF_gals.iloc[[np.argmin(sep.arcsec)]]
+              host_DF = pd.concat([host_DF, desperateMatch], ignore_index=True)
+              host_dict_nospace_postDLR[transient] = desperateMatch['objID'].values[0]
+              if verbose:
+                   print("Desperate match found for %s, %.2f arcsec away." % (transient, sep[np.argmin(sep.arcsec)].arcsec))
+
+        if len(noHosts) > 0:
+            with open(path+"/dictionaries/noHosts_fromDLR.p", 'wb') as fp:
+                dump(noHosts, fp)
+
+        if len(GD_SN) > 0:
+            with open(path+"/dictionaries/badInfo_fromDLR.p", 'wb') as fp:
+                 dump(GD_SN, fp)
 
-    cut_dict = clean_dict(cut_dict, host_gals_DF, [])
-    stars_DF.to_csv(path+"removedStars.csv",index=False)
+        #gradient ascent algorithm for the SNe that didn't pass this stage
+        SN_toReassociate = np.concatenate([np.array(noHosts), np.array(GD_SN), np.array(list(lost))])
 
-    #plotLocus(host_gals_DF, color=1, save=1, type="Gals", timestamp=dateStr)
-    #plotLocus(stars_DF, color=1, save=1, type="Stars", timestamp=dateStr)
+        if (len(SN_toReassociate) > 0) and (ascentMatch):
+            if verbose:
+                print("%i transients with no host found with DLR, %i transients with bad host data with DLR." %(len(noHosts), len(GD_SN)))
+                print("Running gradient ascent for %i remaining transients."%len(SN_toReassociate))
+                print("See GradientAscent.txt for more information.")
 
-    host_dict_nospace = {k.replace(' ', ''): v for k, v in cut_dict.items()}
-
-    fn = "DLR.txt"
-    transients = pd.read_csv(path+fn_SN)
-
-    with open(path+"/dictionaries/checkpoint_preDLR.p", 'wb') as fp:
-           dump(host_dict_nospace, fp)
-
-    #return the candidates list before DLR for debugging purposes
-    #return host_gals_DF
-
-    host_DF, host_dict_nospace_postDLR, noHosts, GD_SN = chooseByDLR(path, host_gals_DF, transients, fn, host_dict_nospace, todo="r")
-
-    #last-ditch effort -- for the ones with no found host, just pick the nearest NED galaxy.
-    for transient in noHosts:
-          tempDF = host_gals_DF[host_gals_DF['objID'].isin(desperate_dict[transient])]
-          tempDF_gals = tempDF[tempDF['NED_type'].isin(['G', 'PofG', 'GPair', 'GGroup', 'GClstr'])].reset_index()
-          if len(tempDF_gals) < 1:
-             continue
-          transientRA = transients.loc[transients['Name'] == transient, 'RA'].values[0]
-          transientDEC = transients.loc[transients['Name'] == transient, 'DEC'].values[0]
-          transientCoord = SkyCoord(transientRA*u.deg, transientDEC*u.deg, frame='icrs')
-          tempHostCoords = SkyCoord(tempDF_gals['raMean'].values*u.deg, tempDF_gals['decMean'].values*u.deg, frame='icrs')
-          sep = transientCoord.separation(tempHostCoords)
-          desperateMatch = tempDF_gals.iloc[[np.argmin(sep.arcsec)]]
-          host_DF = pd.concat([host_DF, desperateMatch], ignore_index=True)
-          host_dict_nospace_postDLR[transient] = desperateMatch['objID'].values[0]
-          if verbose:
-               print("Desperate match found for %s, %.2f arcsec away." % (transient, sep[np.argmin(sep.arcsec)].arcsec))
-
-    if len(noHosts) > 0:
-        with open(path+"/dictionaries/noHosts_fromDLR.p", 'wb') as fp:
-            dump(noHosts, fp)
-
-    if len(GD_SN) > 0:
-        with open(path+"/dictionaries/badInfo_fromDLR.p", 'wb') as fp:
-             dump(GD_SN, fp)
+            fn_GD= path+'/GradientAscent.txt'
 
-    #gradient ascent algorithm for the SNe that didn't pass this stage
-    SN_toReassociate = np.concatenate([np.array(noHosts), np.array(GD_SN), np.array(list(lost))])
+            host_dict_nospace_postDLR_GD, host_DF, unchanged = gradientAscent(path, transient_dict,  host_dict_nospace_postDLR, SN_toReassociate, host_DF, transients, fn_GD, plot=verbose, px=px)
 
-    if (len(SN_toReassociate) > 0) and (ascentMatch):
-        if verbose:
-            print("%i transients with no host found with DLR, %i transients with bad host data with DLR." %(len(noHosts), len(GD_SN)))
-            print("Running gradient ascent for %i remaining transients."%len(SN_toReassociate))
-            print("See GradientAscent.txt for more information.")
+            with open(path+"/dictionaries/gals_postGD.p", 'wb') as fp:
+                dump(host_dict_nospace_postDLR_GD, fp)
 
-        fn_GD= path+'/GradientAscent.txt'
+            if verbose:
+                print("Hosts not found for %i transients in gradient ascent. Storing names in GD_unchanged.txt" %(len(unchanged)))
 
-        host_dict_nospace_postDLR_GD, host_DF, unchanged = gradientAscent(path, transient_dict,  host_dict_nospace_postDLR, SN_toReassociate, host_DF, transients, fn_GD, plot=verbose, px=px)
+            with open(path+"/GD_unchanged.txt", 'wb') as fp:
+                dump(unchanged, fp)
 
-        with open(path+"/dictionaries/gals_postGD.p", 'wb') as fp:
-            dump(host_dict_nospace_postDLR_GD, fp)
+            hostFrac = fracWithHosts(host_dict_nospace_postDLR_GD)*100
 
-        if verbose:
-            print("Hosts not found for %i transients in gradient ascent. Storing names in GD_unchanged.txt" %(len(unchanged)))
+            if verbose:
+                print("Associated fraction after gradient ascent: %.2f%%."%hostFrac)
 
-        with open(path+"/GD_unchanged.txt", 'wb') as fp:
-            dump(unchanged, fp)
+            final_dict = host_dict_nospace_postDLR_GD.copy()
 
-        hostFrac = fracWithHosts(host_dict_nospace_postDLR_GD)*100
+        else:
+            final_dict = host_dict_nospace_postDLR.copy()
 
-        if verbose:
-            print("Associated fraction after gradient ascent: %.2f%%."%hostFrac)
+        host_DF = build_ML_df(final_dict, host_DF, transients)
 
-        final_dict = host_dict_nospace_postDLR_GD.copy()
+        # add the glade sources back in!
+        if len(foundGladeHosts) > 0:
+            if verbose:
+                print("Adding %i sources from GLADE back into the catalog..."%len(foundGladeHosts))
 
-    else:
-        final_dict = host_dict_nospace_postDLR.copy()
+            host_DF['GLADE_source'] = False
+            foundGladeHosts['GLADE_source'] = True
 
-    host_DF = build_ML_df(final_dict, host_DF, transients)
+            #kluge for lookup later
+            foundGladeHosts['objID'] = foundGladeHosts['objName'] = foundGladeHosts['NED_name']
 
-    with open(path+"/dictionaries/" + "Final_Dictionary.p", 'wb') as fp:
-           dump(final_dict, fp)
+            #combine
+            host_DF = pd.concat([host_DF, foundGladeHosts], ignore_index=True)
+
+        with open(path+"/dictionaries/" + "Final_Dictionary.p", 'wb') as fp:
+               dump(final_dict, fp)
 
     #a few final cleaning steps
     host_DF.drop_duplicates(subset=['TransientName'], inplace=True)
     host_DF = host_DF[host_DF['TransientName'] != ""]
     host_DF.reset_index(inplace=True, drop=True)
     host_DF['TransientName'] = [x.replace(" ", "") for x in host_DF['TransientName']]
 
-    matchFrac = len(host_DF)/len(transients)*100
+    allTransients = pd.read_csv(path+fn_transients_preGLADE)
+
+    matchFrac = len(host_DF)/len(allTransients)*100
     print("Found matches for %.1f%% of events."%matchFrac)
     if verbose:
         print("Saving table of hosts to %s."%(path+"tables/FinalAssociationTable.csv"))
 
     host_DF.to_csv(path+"FinalAssociationTable.csv", index=False)
 
-    tablePath = path+"/tables/"
-    printoutPath = path+'/printouts/'
-
-    paths = [tablePath, printoutPath]
+    #sort things into the relevant folders
+    cleanup(path)
 
-    for tempPath in paths:
-        if not os.path.exists(tempPath):
-            os.mkdir(tempPath)
-
-    #move tables to the tables directory, and printouts to the printouts directory
-    printouts = glob.glob(path+'/*.txt')
-    for p in printouts:
-        fn = remove_prefix(p, path)
-        os.rename(p, printoutPath+fn)
-
-    table_ext = ['csv', 'gz']
-    for end in table_ext:
-        tables = glob.glob(path+'/*.%s'%end)
-        for t in tables:
-            fn = remove_prefix(t, path)
-            os.rename(t, tablePath+fn)
     #remove if there's an extra index column
     try:
         del host_DF['index']
     except:
         pass
     return host_DF
```

### Comparing `astro_ghost-1.0.3/astro_ghost/gradientAscent.py` & `astro_ghost-2.0.0/astro_ghost/gradientAscent.py`

 * *Files identical despite different names*

### Comparing `astro_ghost-1.0.3/astro_ghost/hostMatching.py` & `astro_ghost-2.0.0/astro_ghost/hostMatching.py`

 * *Files identical despite different names*

### Comparing `astro_ghost-1.0.3/astro_ghost/photoz_helper.py` & `astro_ghost-2.0.0/astro_ghost/photoz_helper.py`

 * *Files identical despite different names*

### Comparing `astro_ghost-1.0.3/astro_ghost/sourceCleaning.py` & `astro_ghost-2.0.0/astro_ghost/sourceCleaning.py`

 * *Files 0% similar despite different names*

```diff
@@ -216,15 +216,15 @@
     :rtype: Pandas DataFrame
     """
 
     for cut in cuts:
         if cut == "n":
             df = df[df['nDetections'] >= 10]
         elif cut == "quality":
-            df = df[df["qualityFlag"] < 128]
+            df = df[df["qualityFlag"] <= 165]
         elif cut == "coords":
             df = df.dropna(subset=['raMean', 'decMean'])
         elif cut == "mag":
             for band in 'grizy':
                 df = df[pd.notnull(df['%sApMag'%band])]
         elif cut =="primary":
             if dict != "":
```

### Comparing `astro_ghost-1.0.3/astro_ghost/starSeparation.py` & `astro_ghost-2.0.0/astro_ghost/starSeparation.py`

 * *Files identical despite different names*

### Comparing `astro_ghost-1.0.3/astro_ghost/stellarLocus.py` & `astro_ghost-2.0.0/astro_ghost/stellarLocus.py`

 * *Files identical despite different names*

### Comparing `astro_ghost-1.0.3/astro_ghost.egg-info/PKG-INFO` & `astro_ghost-2.0.0/astro_ghost.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: astro-ghost
-Version: 1.0.3
+Version: 2.0.0
 Summary: A package to associate transients with host galaxies, and a database of 16k SNe-host galaxies in PS1.
 Home-page: https://github.com/pypa/sampleproject
 Author: Alex Gagliano
 Author-email: gaglian2@illinois.edu
 License: GNU GPL v3+
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `astro_ghost-1.0.3/astro_ghost.egg-info/SOURCES.txt` & `astro_ghost-2.0.0/astro_ghost.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `astro_ghost-1.0.3/docs/Makefile` & `astro_ghost-2.0.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `astro_ghost-1.0.3/docs/conf.py` & `astro_ghost-2.0.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `astro_ghost-1.0.3/docs/index.rst` & `astro_ghost-2.0.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `astro_ghost-1.0.3/docs/make.bat` & `astro_ghost-2.0.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `astro_ghost-1.0.3/docs/source/associationmodules.rst` & `astro_ghost-2.0.0/docs/source/associationmodules.rst`

 * *Files identical despite different names*

### Comparing `astro_ghost-1.0.3/docs/source/basicusage.rst` & `astro_ghost-2.0.0/docs/source/basicusage.rst`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Example Usage
 =============
 
-The database of supernova-host galaxy matches can be found at http://ghost.ncsa.illinois.edu/static/GHOST.csv, and retrieved using the getGHOST() function. This database will need to be created before running the association pipeline.
+The database of supernova-host galaxy matches can be retrieved using the getGHOST() function. This database will need to be created before running the association pipeline.
 
 .. code-block:: python
 
     import os
     import sys
     from astro_ghost.PS1QueryFunctions import getAllPostageStamps
     from astro_ghost.TNSQueryFunctions import getTNSSpectra
@@ -28,20 +28,18 @@
     #create a list of the supernova names, their skycoords, and their classes (these three are from TNS)
     snName = ['SN 2012dt', 'SN 1998bn', 'SN 1957B']
 
     snCoord = [SkyCoord(14.162*u.deg, -9.90253*u.deg, frame='icrs'), \
                 SkyCoord(187.32867*u.deg, -23.16367*u.deg, frame='icrs'), \
                 SkyCoord(186.26125*u.deg, +12.899444*u.deg, frame='icrs')]
 
-    snClass = ['SN IIP', 'SN', 'SN Ia']
-
     # run the association algorithm!
     # this first checks the GHOST database for a SN by name, then by coordinates, and
     # if we have no match then it manually associates them.
-    hosts = getTransientHosts(snName, snCoord, snClass, verbose=verbose, starcut='normal')
+    hosts = getTransientHosts(snName, snCoord, verbose=True)
 
     #create directories to store the host spectra, the transient spectra, and the postage stamps
     hSpecPath = "./hostSpectra/"
     tSpecPath = "./SNspectra/"
     psPath = "./hostPostageStamps/"
     paths = [hSpecPath, tSpecPath, psPath]
     for tempPath in paths:
```

### Comparing `astro_ghost-1.0.3/docs/source/catalogmodules.rst` & `astro_ghost-2.0.0/docs/source/catalogmodules.rst`

 * *Files identical despite different names*

### Comparing `astro_ghost-1.0.3/docs/source/installation.rst` & `astro_ghost-2.0.0/docs/source/installation.rst`

 * *Files identical despite different names*

### Comparing `astro_ghost-1.0.3/docs/source/preprocessingmodules.rst` & `astro_ghost-2.0.0/docs/source/preprocessingmodules.rst`

 * *Files identical despite different names*

### Comparing `astro_ghost-1.0.3/licenses/LICENSE.rst` & `astro_ghost-2.0.0/licenses/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `astro_ghost-1.0.3/setup.cfg` & `astro_ghost-2.0.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `astro_ghost-1.0.3/setup.py` & `astro_ghost-2.0.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #!/usr/bin/env python
 # Licensed under a 3-clause BSD style license - see LICENSE.rst
 
 import os
 
 from setuptools import setup
 
-version = "1.0.3"
+version = "2.0.0"
 
 VERSION_TEMPLATE = """
  Note that we need to fall back to the hard-coded version if either
  setuptools_scm can't be imported or setuptools_scm can't determine the
  version, so we catch the generic 'Exception'.
 __version__ = '{version}'
 """.lstrip()
```

### Comparing `astro_ghost-1.0.3/tests/debug.py` & `astro_ghost-2.0.0/tests/debug.py`

 * *Files identical despite different names*

### Comparing `astro_ghost-1.0.3/tests/test_tutorial.py` & `astro_ghost-2.0.0/tests/test_tutorial.py`

 * *Files identical despite different names*

### Comparing `astro_ghost-1.0.3/tox.ini` & `astro_ghost-2.0.0/tox.ini`

 * *Files identical despite different names*

