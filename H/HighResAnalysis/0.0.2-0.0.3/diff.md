# Comparing `tmp/HighResAnalysis-0.0.2.tar.gz` & `tmp/HighResAnalysis-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "HighResAnalysis-0.0.2.tar", last modified: Thu Mar 16 16:04:10 2023, max compression
+gzip compressed data, was "HighResAnalysis-0.0.3.tar", last modified: Mon May 22 12:51:03 2023, max compression
```

## Comparing `HighResAnalysis-0.0.2.tar` & `HighResAnalysis-0.0.3.tar`

### file list

```diff
@@ -1,80 +1,80 @@
-drwxr-xr-x   0 hits       (501) staff       (20)        0 2023-03-16 16:04:10.746018 HighResAnalysis-0.0.2/
-drwxr-xr-x   0 hits       (501) staff       (20)        0 2023-03-16 16:04:10.733273 HighResAnalysis-0.0.2/HighResAnalysis/
--rw-r--r--   0 hits       (501) staff       (20)       22 2023-03-16 16:03:46.000000 HighResAnalysis-0.0.2/HighResAnalysis/__init__.py
--rw-r--r--   0 hits       (501) staff       (20)   319156 2023-03-16 16:03:46.000000 HighResAnalysis-0.0.2/HighResAnalysis/_modidx.py
--rw-r--r--   0 hits       (501) staff       (20)     4244 2023-03-16 16:03:46.000000 HighResAnalysis-0.0.2/HighResAnalysis/analyse.py
-drwxr-xr-x   0 hits       (501) staff       (20)        0 2023-03-16 16:04:10.737532 HighResAnalysis-0.0.2/HighResAnalysis/cern/
--rw-r--r--   0 hits       (501) staff       (20)        0 2023-03-16 16:03:46.000000 HighResAnalysis-0.0.2/HighResAnalysis/cern/__init__.py
--rw-r--r--   0 hits       (501) staff       (20)     3085 2023-03-16 16:03:46.000000 HighResAnalysis-0.0.2/HighResAnalysis/cern/adc.py
--rw-r--r--   0 hits       (501) staff       (20)      921 2023-03-16 16:03:46.000000 HighResAnalysis-0.0.2/HighResAnalysis/cern/calibration.py
--rw-r--r--   0 hits       (501) staff       (20)     3984 2023-03-16 16:03:46.000000 HighResAnalysis-0.0.2/HighResAnalysis/cern/converter.py
--rw-r--r--   0 hits       (501) staff       (20)     3889 2023-03-16 16:03:46.000000 HighResAnalysis-0.0.2/HighResAnalysis/cern/event_alignment.py
--rw-r--r--   0 hits       (501) staff       (20)     1324 2023-03-16 16:03:46.000000 HighResAnalysis-0.0.2/HighResAnalysis/cern/raw.py
--rw-r--r--   0 hits       (501) staff       (20)     1611 2023-03-16 16:03:46.000000 HighResAnalysis-0.0.2/HighResAnalysis/cern/ref.py
--rw-r--r--   0 hits       (501) staff       (20)     7345 2023-03-16 16:03:46.000000 HighResAnalysis-0.0.2/HighResAnalysis/convert.py
-drwxr-xr-x   0 hits       (501) staff       (20)        0 2023-03-16 16:04:10.740255 HighResAnalysis-0.0.2/HighResAnalysis/mod/
--rw-r--r--   0 hits       (501) staff       (20)        0 2023-03-16 16:03:46.000000 HighResAnalysis-0.0.2/HighResAnalysis/mod/__init__.py
--rw-r--r--   0 hits       (501) staff       (20)    15122 2023-03-16 16:03:46.000000 HighResAnalysis-0.0.2/HighResAnalysis/mod/dut_cuts.py
--rw-r--r--   0 hits       (501) staff       (20)     4883 2023-03-16 16:03:46.000000 HighResAnalysis-0.0.2/HighResAnalysis/mod/efficiency.py
--rw-r--r--   0 hits       (501) staff       (20)      439 2023-03-16 16:03:46.000000 HighResAnalysis-0.0.2/HighResAnalysis/mod/ref_cuts.py
--rw-r--r--   0 hits       (501) staff       (20)     1838 2023-03-16 16:03:46.000000 HighResAnalysis-0.0.2/HighResAnalysis/mod/reference.py
--rw-r--r--   0 hits       (501) staff       (20)    12333 2023-03-16 16:03:46.000000 HighResAnalysis-0.0.2/HighResAnalysis/mod/residuals.py
--rw-r--r--   0 hits       (501) staff       (20)      880 2023-03-16 16:03:46.000000 HighResAnalysis-0.0.2/HighResAnalysis/mod/reso_cuts.py
--rw-r--r--   0 hits       (501) staff       (20)     3576 2023-03-16 16:03:46.000000 HighResAnalysis-0.0.2/HighResAnalysis/mod/resolution.py
--rw-r--r--   0 hits       (501) staff       (20)      567 2023-03-16 16:03:46.000000 HighResAnalysis-0.0.2/HighResAnalysis/mod/tel_cuts.py
--rw-r--r--   0 hits       (501) staff       (20)     2161 2023-03-16 16:03:46.000000 HighResAnalysis-0.0.2/HighResAnalysis/mod/telescope.py
--rw-r--r--   0 hits       (501) staff       (20)     2463 2023-03-16 16:03:46.000000 HighResAnalysis-0.0.2/HighResAnalysis/mod/track_cuts.py
--rw-r--r--   0 hits       (501) staff       (20)     4297 2023-03-16 16:03:46.000000 HighResAnalysis-0.0.2/HighResAnalysis/mod/tracks.py
-drwxr-xr-x   0 hits       (501) staff       (20)        0 2023-03-16 16:04:10.742467 HighResAnalysis-0.0.2/HighResAnalysis/plotting/
--rw-r--r--   0 hits       (501) staff       (20)        0 2023-03-16 16:03:46.000000 HighResAnalysis-0.0.2/HighResAnalysis/plotting/__init__.py
--rw-r--r--   0 hits       (501) staff       (20)     5770 2023-03-16 16:03:46.000000 HighResAnalysis-0.0.2/HighResAnalysis/plotting/binning.py
--rw-r--r--   0 hits       (501) staff       (20)    71255 2023-03-16 16:03:46.000000 HighResAnalysis-0.0.2/HighResAnalysis/plotting/draw.py
--rw-r--r--   0 hits       (501) staff       (20)    17384 2023-03-16 16:03:46.000000 HighResAnalysis-0.0.2/HighResAnalysis/plotting/fit.py
--rw-r--r--   0 hits       (501) staff       (20)    13156 2023-03-16 16:03:46.000000 HighResAnalysis-0.0.2/HighResAnalysis/plotting/html.py
--rw-r--r--   0 hits       (501) staff       (20)     2473 2023-03-16 16:03:46.000000 HighResAnalysis-0.0.2/HighResAnalysis/plotting/info.py
--rw-r--r--   0 hits       (501) staff       (20)     3057 2023-03-16 16:03:46.000000 HighResAnalysis-0.0.2/HighResAnalysis/plotting/latex.py
--rw-r--r--   0 hits       (501) staff       (20)     8232 2023-03-16 16:03:46.000000 HighResAnalysis-0.0.2/HighResAnalysis/plotting/save.py
--rw-r--r--   0 hits       (501) staff       (20)    15573 2023-03-16 16:03:46.000000 HighResAnalysis-0.0.2/HighResAnalysis/plotting/utils.py
-drwxr-xr-x   0 hits       (501) staff       (20)        0 2023-03-16 16:04:10.745231 HighResAnalysis-0.0.2/HighResAnalysis/src/
--rw-r--r--   0 hits       (501) staff       (20)        0 2023-03-16 16:03:46.000000 HighResAnalysis-0.0.2/HighResAnalysis/src/__init__.py
--rw-r--r--   0 hits       (501) staff       (20)     5836 2023-03-16 16:03:46.000000 HighResAnalysis-0.0.2/HighResAnalysis/src/analysis.py
--rw-r--r--   0 hits       (501) staff       (20)     2377 2023-03-16 16:03:46.000000 HighResAnalysis-0.0.2/HighResAnalysis/src/batch_analysis.py
--rw-r--r--   0 hits       (501) staff       (20)     4056 2023-03-16 16:03:46.000000 HighResAnalysis-0.0.2/HighResAnalysis/src/bins.py
--rw-r--r--   0 hits       (501) staff       (20)    10064 2023-03-16 16:03:46.000000 HighResAnalysis-0.0.2/HighResAnalysis/src/calibration.py
--rw-r--r--   0 hits       (501) staff       (20)    18450 2023-03-16 16:03:46.000000 HighResAnalysis-0.0.2/HighResAnalysis/src/converter.py
--rw-r--r--   0 hits       (501) staff       (20)    14848 2023-03-16 16:03:46.000000 HighResAnalysis-0.0.2/HighResAnalysis/src/currents.py
--rw-r--r--   0 hits       (501) staff       (20)     6652 2023-03-16 16:03:46.000000 HighResAnalysis-0.0.2/HighResAnalysis/src/cut.py
--rw-r--r--   0 hits       (501) staff       (20)     5153 2023-03-16 16:03:46.000000 HighResAnalysis-0.0.2/HighResAnalysis/src/dut.py
--rw-r--r--   0 hits       (501) staff       (20)    36199 2023-03-16 16:03:46.000000 HighResAnalysis-0.0.2/HighResAnalysis/src/dut_analysis.py
--rw-r--r--   0 hits       (501) staff       (20)    12991 2023-03-16 16:03:46.000000 HighResAnalysis-0.0.2/HighResAnalysis/src/proteus.py
--rw-r--r--   0 hits       (501) staff       (20)      739 2023-03-16 16:03:46.000000 HighResAnalysis-0.0.2/HighResAnalysis/src/raw.py
--rw-r--r--   0 hits       (501) staff       (20)    11687 2023-03-16 16:03:46.000000 HighResAnalysis-0.0.2/HighResAnalysis/src/run.py
--rw-r--r--   0 hits       (501) staff       (20)     5600 2023-03-16 16:03:46.000000 HighResAnalysis-0.0.2/HighResAnalysis/src/scan.py
--rw-r--r--   0 hits       (501) staff       (20)     5869 2023-03-16 16:03:46.000000 HighResAnalysis-0.0.2/HighResAnalysis/src/spreadsheet.py
-drwxr-xr-x   0 hits       (501) staff       (20)        0 2023-03-16 16:04:10.745616 HighResAnalysis-0.0.2/HighResAnalysis/utility/
--rw-r--r--   0 hits       (501) staff       (20)        0 2023-03-16 16:03:46.000000 HighResAnalysis-0.0.2/HighResAnalysis/utility/__init__.py
--rw-r--r--   0 hits       (501) staff       (20)     1979 2023-03-16 16:03:46.000000 HighResAnalysis-0.0.2/HighResAnalysis/utility/affine_transformations.py
--rw-r--r--   0 hits       (501) staff       (20)    20836 2023-03-16 16:03:46.000000 HighResAnalysis-0.0.2/HighResAnalysis/utility/utils.py
-drwxr-xr-x   0 hits       (501) staff       (20)        0 2023-03-16 16:04:10.734493 HighResAnalysis-0.0.2/HighResAnalysis.egg-info/
-drwxr-xr-x   0 hits       (501) staff       (20)        0 2023-03-16 16:04:10.736242 HighResAnalysis-0.0.2/HighResAnalysis.egg-info/.ipynb_checkpoints/
--rw-r--r--   0 hits       (501) staff       (20)     1865 2023-02-13 09:10:21.000000 HighResAnalysis-0.0.2/HighResAnalysis.egg-info/.ipynb_checkpoints/PKG-INFO-checkpoint
--rw-r--r--   0 hits       (501) staff       (20)     1691 2023-02-13 09:10:21.000000 HighResAnalysis-0.0.2/HighResAnalysis.egg-info/.ipynb_checkpoints/SOURCES-checkpoint.txt
--rw-r--r--   0 hits       (501) staff       (20)        1 2023-02-13 09:10:21.000000 HighResAnalysis-0.0.2/HighResAnalysis.egg-info/.ipynb_checkpoints/dependency_links-checkpoint.txt
--rw-r--r--   0 hits       (501) staff       (20)       52 2023-02-13 09:10:21.000000 HighResAnalysis-0.0.2/HighResAnalysis.egg-info/.ipynb_checkpoints/entry_points-checkpoint.txt
--rw-r--r--   0 hits       (501) staff       (20)        1 2023-02-12 17:27:26.000000 HighResAnalysis-0.0.2/HighResAnalysis.egg-info/.ipynb_checkpoints/not-zip-safe-checkpoint
--rw-r--r--   0 hits       (501) staff       (20)      136 2023-02-13 09:10:21.000000 HighResAnalysis-0.0.2/HighResAnalysis.egg-info/.ipynb_checkpoints/requires-checkpoint.txt
--rw-r--r--   0 hits       (501) staff       (20)       16 2023-02-13 09:10:21.000000 HighResAnalysis-0.0.2/HighResAnalysis.egg-info/.ipynb_checkpoints/top_level-checkpoint.txt
--rw-r--r--   0 hits       (501) staff       (20)     2032 2023-03-16 16:04:10.000000 HighResAnalysis-0.0.2/HighResAnalysis.egg-info/PKG-INFO
--rw-r--r--   0 hits       (501) staff       (20)     2429 2023-03-16 16:04:10.000000 HighResAnalysis-0.0.2/HighResAnalysis.egg-info/SOURCES.txt
--rw-r--r--   0 hits       (501) staff       (20)        1 2023-03-16 16:04:10.000000 HighResAnalysis-0.0.2/HighResAnalysis.egg-info/dependency_links.txt
--rw-r--r--   0 hits       (501) staff       (20)      110 2023-03-16 16:04:10.000000 HighResAnalysis-0.0.2/HighResAnalysis.egg-info/entry_points.txt
--rw-r--r--   0 hits       (501) staff       (20)        1 2023-02-12 17:27:26.000000 HighResAnalysis-0.0.2/HighResAnalysis.egg-info/not-zip-safe
--rw-r--r--   0 hits       (501) staff       (20)      145 2023-03-16 16:04:10.000000 HighResAnalysis-0.0.2/HighResAnalysis.egg-info/requires.txt
--rw-r--r--   0 hits       (501) staff       (20)       16 2023-03-16 16:04:10.000000 HighResAnalysis-0.0.2/HighResAnalysis.egg-info/top_level.txt
--rw-rw-r--   0 hits       (501) staff       (20)    11337 2023-01-20 02:50:04.000000 HighResAnalysis-0.0.2/LICENSE
--rw-rw-r--   0 hits       (501) staff       (20)      111 2023-01-20 02:50:04.000000 HighResAnalysis-0.0.2/MANIFEST.in
--rw-r--r--   0 hits       (501) staff       (20)     2032 2023-03-16 16:04:10.745875 HighResAnalysis-0.0.2/PKG-INFO
--rw-r--r--   0 hits       (501) staff       (20)     1184 2023-02-22 12:25:04.000000 HighResAnalysis-0.0.2/README.md
--rw-r--r--   0 hits       (501) staff       (20)     1131 2023-03-16 16:03:46.000000 HighResAnalysis-0.0.2/settings.ini
--rw-r--r--   0 hits       (501) staff       (20)       38 2023-03-16 16:04:10.746063 HighResAnalysis-0.0.2/setup.cfg
--rw-rw-r--   0 hits       (501) staff       (20)     2560 2023-01-20 02:50:04.000000 HighResAnalysis-0.0.2/setup.py
+drwxr-xr-x   0 hits       (501) staff       (20)        0 2023-05-22 12:51:03.047952 HighResAnalysis-0.0.3/
+drwxr-xr-x   0 hits       (501) staff       (20)        0 2023-05-22 12:51:03.039248 HighResAnalysis-0.0.3/HighResAnalysis/
+-rw-r--r--   0 hits       (501) staff       (20)       22 2023-05-22 12:50:44.000000 HighResAnalysis-0.0.3/HighResAnalysis/__init__.py
+-rw-r--r--   0 hits       (501) staff       (20)   319156 2023-05-22 12:50:44.000000 HighResAnalysis-0.0.3/HighResAnalysis/_modidx.py
+-rw-r--r--   0 hits       (501) staff       (20)     4272 2023-05-22 12:50:44.000000 HighResAnalysis-0.0.3/HighResAnalysis/analyse.py
+drwxr-xr-x   0 hits       (501) staff       (20)        0 2023-05-22 12:51:03.042796 HighResAnalysis-0.0.3/HighResAnalysis/cern/
+-rw-r--r--   0 hits       (501) staff       (20)        0 2023-05-22 12:50:44.000000 HighResAnalysis-0.0.3/HighResAnalysis/cern/__init__.py
+-rw-r--r--   0 hits       (501) staff       (20)     3085 2023-05-22 12:50:44.000000 HighResAnalysis-0.0.3/HighResAnalysis/cern/adc.py
+-rw-r--r--   0 hits       (501) staff       (20)      921 2023-05-22 12:50:44.000000 HighResAnalysis-0.0.3/HighResAnalysis/cern/calibration.py
+-rw-r--r--   0 hits       (501) staff       (20)     3984 2023-05-22 12:50:44.000000 HighResAnalysis-0.0.3/HighResAnalysis/cern/converter.py
+-rw-r--r--   0 hits       (501) staff       (20)     3889 2023-05-22 12:50:44.000000 HighResAnalysis-0.0.3/HighResAnalysis/cern/event_alignment.py
+-rw-r--r--   0 hits       (501) staff       (20)     1324 2023-05-22 12:50:44.000000 HighResAnalysis-0.0.3/HighResAnalysis/cern/raw.py
+-rw-r--r--   0 hits       (501) staff       (20)     1611 2023-05-22 12:50:44.000000 HighResAnalysis-0.0.3/HighResAnalysis/cern/ref.py
+-rw-r--r--   0 hits       (501) staff       (20)     7345 2023-05-22 12:50:44.000000 HighResAnalysis-0.0.3/HighResAnalysis/convert.py
+drwxr-xr-x   0 hits       (501) staff       (20)        0 2023-05-22 12:51:03.044185 HighResAnalysis-0.0.3/HighResAnalysis/mod/
+-rw-r--r--   0 hits       (501) staff       (20)        0 2023-05-22 12:50:44.000000 HighResAnalysis-0.0.3/HighResAnalysis/mod/__init__.py
+-rw-r--r--   0 hits       (501) staff       (20)    15122 2023-05-22 12:50:44.000000 HighResAnalysis-0.0.3/HighResAnalysis/mod/dut_cuts.py
+-rw-r--r--   0 hits       (501) staff       (20)     4883 2023-05-22 12:50:44.000000 HighResAnalysis-0.0.3/HighResAnalysis/mod/efficiency.py
+-rw-r--r--   0 hits       (501) staff       (20)      439 2023-05-22 12:50:44.000000 HighResAnalysis-0.0.3/HighResAnalysis/mod/ref_cuts.py
+-rw-r--r--   0 hits       (501) staff       (20)     1838 2023-05-22 12:50:44.000000 HighResAnalysis-0.0.3/HighResAnalysis/mod/reference.py
+-rw-r--r--   0 hits       (501) staff       (20)    12333 2023-05-22 12:50:44.000000 HighResAnalysis-0.0.3/HighResAnalysis/mod/residuals.py
+-rw-r--r--   0 hits       (501) staff       (20)      880 2023-05-22 12:50:44.000000 HighResAnalysis-0.0.3/HighResAnalysis/mod/reso_cuts.py
+-rw-r--r--   0 hits       (501) staff       (20)     3576 2023-05-22 12:50:44.000000 HighResAnalysis-0.0.3/HighResAnalysis/mod/resolution.py
+-rw-r--r--   0 hits       (501) staff       (20)      567 2023-05-22 12:50:44.000000 HighResAnalysis-0.0.3/HighResAnalysis/mod/tel_cuts.py
+-rw-r--r--   0 hits       (501) staff       (20)     2161 2023-05-22 12:50:44.000000 HighResAnalysis-0.0.3/HighResAnalysis/mod/telescope.py
+-rw-r--r--   0 hits       (501) staff       (20)     2463 2023-05-22 12:50:44.000000 HighResAnalysis-0.0.3/HighResAnalysis/mod/track_cuts.py
+-rw-r--r--   0 hits       (501) staff       (20)     4297 2023-05-22 12:50:44.000000 HighResAnalysis-0.0.3/HighResAnalysis/mod/tracks.py
+drwxr-xr-x   0 hits       (501) staff       (20)        0 2023-05-22 12:51:03.045275 HighResAnalysis-0.0.3/HighResAnalysis/plotting/
+-rw-r--r--   0 hits       (501) staff       (20)        0 2023-05-22 12:50:44.000000 HighResAnalysis-0.0.3/HighResAnalysis/plotting/__init__.py
+-rw-r--r--   0 hits       (501) staff       (20)     5770 2023-05-22 12:50:44.000000 HighResAnalysis-0.0.3/HighResAnalysis/plotting/binning.py
+-rw-r--r--   0 hits       (501) staff       (20)    71626 2023-05-22 12:50:44.000000 HighResAnalysis-0.0.3/HighResAnalysis/plotting/draw.py
+-rw-r--r--   0 hits       (501) staff       (20)    17384 2023-05-22 12:50:44.000000 HighResAnalysis-0.0.3/HighResAnalysis/plotting/fit.py
+-rw-r--r--   0 hits       (501) staff       (20)    13156 2023-05-22 12:50:44.000000 HighResAnalysis-0.0.3/HighResAnalysis/plotting/html.py
+-rw-r--r--   0 hits       (501) staff       (20)     2473 2023-05-22 12:50:44.000000 HighResAnalysis-0.0.3/HighResAnalysis/plotting/info.py
+-rw-r--r--   0 hits       (501) staff       (20)     3057 2023-05-22 12:50:44.000000 HighResAnalysis-0.0.3/HighResAnalysis/plotting/latex.py
+-rw-r--r--   0 hits       (501) staff       (20)     8211 2023-05-22 12:50:44.000000 HighResAnalysis-0.0.3/HighResAnalysis/plotting/save.py
+-rw-r--r--   0 hits       (501) staff       (20)    15920 2023-05-22 12:50:44.000000 HighResAnalysis-0.0.3/HighResAnalysis/plotting/utils.py
+drwxr-xr-x   0 hits       (501) staff       (20)        0 2023-05-22 12:51:03.047243 HighResAnalysis-0.0.3/HighResAnalysis/src/
+-rw-r--r--   0 hits       (501) staff       (20)        0 2023-05-22 12:50:44.000000 HighResAnalysis-0.0.3/HighResAnalysis/src/__init__.py
+-rw-r--r--   0 hits       (501) staff       (20)     5893 2023-05-22 12:50:44.000000 HighResAnalysis-0.0.3/HighResAnalysis/src/analysis.py
+-rw-r--r--   0 hits       (501) staff       (20)     2377 2023-05-22 12:50:44.000000 HighResAnalysis-0.0.3/HighResAnalysis/src/batch_analysis.py
+-rw-r--r--   0 hits       (501) staff       (20)     4056 2023-05-22 12:50:44.000000 HighResAnalysis-0.0.3/HighResAnalysis/src/bins.py
+-rw-r--r--   0 hits       (501) staff       (20)    10064 2023-05-22 12:50:44.000000 HighResAnalysis-0.0.3/HighResAnalysis/src/calibration.py
+-rw-r--r--   0 hits       (501) staff       (20)    18450 2023-05-22 12:50:44.000000 HighResAnalysis-0.0.3/HighResAnalysis/src/converter.py
+-rw-r--r--   0 hits       (501) staff       (20)    14848 2023-05-22 12:50:44.000000 HighResAnalysis-0.0.3/HighResAnalysis/src/currents.py
+-rw-r--r--   0 hits       (501) staff       (20)     6652 2023-05-22 12:50:44.000000 HighResAnalysis-0.0.3/HighResAnalysis/src/cut.py
+-rw-r--r--   0 hits       (501) staff       (20)     5153 2023-05-22 12:50:44.000000 HighResAnalysis-0.0.3/HighResAnalysis/src/dut.py
+-rw-r--r--   0 hits       (501) staff       (20)    36228 2023-05-22 12:50:44.000000 HighResAnalysis-0.0.3/HighResAnalysis/src/dut_analysis.py
+-rw-r--r--   0 hits       (501) staff       (20)    12991 2023-05-22 12:50:44.000000 HighResAnalysis-0.0.3/HighResAnalysis/src/proteus.py
+-rw-r--r--   0 hits       (501) staff       (20)      739 2023-05-22 12:50:44.000000 HighResAnalysis-0.0.3/HighResAnalysis/src/raw.py
+-rw-r--r--   0 hits       (501) staff       (20)    11867 2023-05-22 12:50:44.000000 HighResAnalysis-0.0.3/HighResAnalysis/src/run.py
+-rw-r--r--   0 hits       (501) staff       (20)     5600 2023-05-22 12:50:44.000000 HighResAnalysis-0.0.3/HighResAnalysis/src/scan.py
+-rw-r--r--   0 hits       (501) staff       (20)     5869 2023-05-22 12:50:44.000000 HighResAnalysis-0.0.3/HighResAnalysis/src/spreadsheet.py
+drwxr-xr-x   0 hits       (501) staff       (20)        0 2023-05-22 12:51:03.047583 HighResAnalysis-0.0.3/HighResAnalysis/utility/
+-rw-r--r--   0 hits       (501) staff       (20)        0 2023-05-22 12:50:44.000000 HighResAnalysis-0.0.3/HighResAnalysis/utility/__init__.py
+-rw-r--r--   0 hits       (501) staff       (20)     1979 2023-05-22 12:50:44.000000 HighResAnalysis-0.0.3/HighResAnalysis/utility/affine_transformations.py
+-rw-r--r--   0 hits       (501) staff       (20)    21164 2023-05-22 12:50:44.000000 HighResAnalysis-0.0.3/HighResAnalysis/utility/utils.py
+drwxr-xr-x   0 hits       (501) staff       (20)        0 2023-05-22 12:51:03.040299 HighResAnalysis-0.0.3/HighResAnalysis.egg-info/
+drwxr-xr-x   0 hits       (501) staff       (20)        0 2023-05-22 12:51:03.041872 HighResAnalysis-0.0.3/HighResAnalysis.egg-info/.ipynb_checkpoints/
+-rw-r--r--   0 hits       (501) staff       (20)     1865 2023-02-13 09:10:21.000000 HighResAnalysis-0.0.3/HighResAnalysis.egg-info/.ipynb_checkpoints/PKG-INFO-checkpoint
+-rw-r--r--   0 hits       (501) staff       (20)     1691 2023-02-13 09:10:21.000000 HighResAnalysis-0.0.3/HighResAnalysis.egg-info/.ipynb_checkpoints/SOURCES-checkpoint.txt
+-rw-r--r--   0 hits       (501) staff       (20)        1 2023-02-13 09:10:21.000000 HighResAnalysis-0.0.3/HighResAnalysis.egg-info/.ipynb_checkpoints/dependency_links-checkpoint.txt
+-rw-r--r--   0 hits       (501) staff       (20)       52 2023-02-13 09:10:21.000000 HighResAnalysis-0.0.3/HighResAnalysis.egg-info/.ipynb_checkpoints/entry_points-checkpoint.txt
+-rw-r--r--   0 hits       (501) staff       (20)        1 2023-02-12 17:27:26.000000 HighResAnalysis-0.0.3/HighResAnalysis.egg-info/.ipynb_checkpoints/not-zip-safe-checkpoint
+-rw-r--r--   0 hits       (501) staff       (20)      136 2023-02-13 09:10:21.000000 HighResAnalysis-0.0.3/HighResAnalysis.egg-info/.ipynb_checkpoints/requires-checkpoint.txt
+-rw-r--r--   0 hits       (501) staff       (20)       16 2023-02-13 09:10:21.000000 HighResAnalysis-0.0.3/HighResAnalysis.egg-info/.ipynb_checkpoints/top_level-checkpoint.txt
+-rw-r--r--   0 hits       (501) staff       (20)     3349 2023-05-22 12:51:02.000000 HighResAnalysis-0.0.3/HighResAnalysis.egg-info/PKG-INFO
+-rw-r--r--   0 hits       (501) staff       (20)     2429 2023-05-22 12:51:03.000000 HighResAnalysis-0.0.3/HighResAnalysis.egg-info/SOURCES.txt
+-rw-r--r--   0 hits       (501) staff       (20)        1 2023-05-22 12:51:02.000000 HighResAnalysis-0.0.3/HighResAnalysis.egg-info/dependency_links.txt
+-rw-r--r--   0 hits       (501) staff       (20)      110 2023-05-22 12:51:02.000000 HighResAnalysis-0.0.3/HighResAnalysis.egg-info/entry_points.txt
+-rw-r--r--   0 hits       (501) staff       (20)        1 2023-02-12 17:27:26.000000 HighResAnalysis-0.0.3/HighResAnalysis.egg-info/not-zip-safe
+-rw-r--r--   0 hits       (501) staff       (20)      145 2023-05-22 12:51:02.000000 HighResAnalysis-0.0.3/HighResAnalysis.egg-info/requires.txt
+-rw-r--r--   0 hits       (501) staff       (20)       16 2023-05-22 12:51:02.000000 HighResAnalysis-0.0.3/HighResAnalysis.egg-info/top_level.txt
+-rw-rw-r--   0 hits       (501) staff       (20)    11337 2023-01-20 02:50:04.000000 HighResAnalysis-0.0.3/LICENSE
+-rw-rw-r--   0 hits       (501) staff       (20)      111 2023-01-20 02:50:04.000000 HighResAnalysis-0.0.3/MANIFEST.in
+-rw-r--r--   0 hits       (501) staff       (20)     3349 2023-05-22 12:51:03.047801 HighResAnalysis-0.0.3/PKG-INFO
+-rw-r--r--   0 hits       (501) staff       (20)     2501 2023-05-22 12:45:33.000000 HighResAnalysis-0.0.3/README.md
+-rw-r--r--   0 hits       (501) staff       (20)     1131 2023-05-22 12:50:44.000000 HighResAnalysis-0.0.3/settings.ini
+-rw-r--r--   0 hits       (501) staff       (20)       38 2023-05-22 12:51:03.047994 HighResAnalysis-0.0.3/setup.cfg
+-rw-rw-r--   0 hits       (501) staff       (20)     2560 2023-01-20 02:50:04.000000 HighResAnalysis-0.0.3/setup.py
```

### Comparing `HighResAnalysis-0.0.2/HighResAnalysis/_modidx.py` & `HighResAnalysis-0.0.3/HighResAnalysis/_modidx.py`

 * *Files identical despite different names*

### Comparing `HighResAnalysis-0.0.2/HighResAnalysis/analyse.py` & `HighResAnalysis-0.0.3/HighResAnalysis/analyse.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 from .src.dut_analysis import DUTAnalysis, Analysis
 from .src.batch_analysis import BatchAnalysis
 from .src.run import load_nrs
 from .src.scan import Ensemble, Scan, VScan, TScan
 from .utility.utils import *  # noqa
 from .src.spreadsheet import make
 from .plotting.utils import load_json
+from nbdev.showdoc import *
 
 from fastcore.script import *
 
 # %% ../nbs/00_analyse.ipynb 4
 t_start = time()
 
 # %% ../nbs/00_analyse.ipynb 7
```

### Comparing `HighResAnalysis-0.0.2/HighResAnalysis/cern/adc.py` & `HighResAnalysis-0.0.3/HighResAnalysis/cern/adc.py`

 * *Files identical despite different names*

### Comparing `HighResAnalysis-0.0.2/HighResAnalysis/cern/calibration.py` & `HighResAnalysis-0.0.3/HighResAnalysis/cern/calibration.py`

 * *Files identical despite different names*

### Comparing `HighResAnalysis-0.0.2/HighResAnalysis/cern/converter.py` & `HighResAnalysis-0.0.3/HighResAnalysis/cern/converter.py`

 * *Files identical despite different names*

### Comparing `HighResAnalysis-0.0.2/HighResAnalysis/cern/event_alignment.py` & `HighResAnalysis-0.0.3/HighResAnalysis/cern/event_alignment.py`

 * *Files identical despite different names*

### Comparing `HighResAnalysis-0.0.2/HighResAnalysis/cern/raw.py` & `HighResAnalysis-0.0.3/HighResAnalysis/cern/raw.py`

 * *Files identical despite different names*

### Comparing `HighResAnalysis-0.0.2/HighResAnalysis/cern/ref.py` & `HighResAnalysis-0.0.3/HighResAnalysis/cern/ref.py`

 * *Files identical despite different names*

### Comparing `HighResAnalysis-0.0.2/HighResAnalysis/convert.py` & `HighResAnalysis-0.0.3/HighResAnalysis/convert.py`

 * *Files identical despite different names*

### Comparing `HighResAnalysis-0.0.2/HighResAnalysis/mod/dut_cuts.py` & `HighResAnalysis-0.0.3/HighResAnalysis/mod/dut_cuts.py`

 * *Files identical despite different names*

### Comparing `HighResAnalysis-0.0.2/HighResAnalysis/mod/efficiency.py` & `HighResAnalysis-0.0.3/HighResAnalysis/mod/efficiency.py`

 * *Files identical despite different names*

### Comparing `HighResAnalysis-0.0.2/HighResAnalysis/mod/reference.py` & `HighResAnalysis-0.0.3/HighResAnalysis/mod/reference.py`

 * *Files identical despite different names*

### Comparing `HighResAnalysis-0.0.2/HighResAnalysis/mod/residuals.py` & `HighResAnalysis-0.0.3/HighResAnalysis/mod/residuals.py`

 * *Files identical despite different names*

### Comparing `HighResAnalysis-0.0.2/HighResAnalysis/mod/reso_cuts.py` & `HighResAnalysis-0.0.3/HighResAnalysis/mod/reso_cuts.py`

 * *Files identical despite different names*

### Comparing `HighResAnalysis-0.0.2/HighResAnalysis/mod/resolution.py` & `HighResAnalysis-0.0.3/HighResAnalysis/mod/resolution.py`

 * *Files identical despite different names*

### Comparing `HighResAnalysis-0.0.2/HighResAnalysis/mod/tel_cuts.py` & `HighResAnalysis-0.0.3/HighResAnalysis/mod/tel_cuts.py`

 * *Files identical despite different names*

### Comparing `HighResAnalysis-0.0.2/HighResAnalysis/mod/telescope.py` & `HighResAnalysis-0.0.3/HighResAnalysis/mod/telescope.py`

 * *Files identical despite different names*

### Comparing `HighResAnalysis-0.0.2/HighResAnalysis/mod/track_cuts.py` & `HighResAnalysis-0.0.3/HighResAnalysis/mod/track_cuts.py`

 * *Files identical despite different names*

### Comparing `HighResAnalysis-0.0.2/HighResAnalysis/mod/tracks.py` & `HighResAnalysis-0.0.3/HighResAnalysis/mod/tracks.py`

 * *Files identical despite different names*

### Comparing `HighResAnalysis-0.0.2/HighResAnalysis/plotting/binning.py` & `HighResAnalysis-0.0.3/HighResAnalysis/plotting/binning.py`

 * *Files identical despite different names*

### Comparing `HighResAnalysis-0.0.2/HighResAnalysis/plotting/draw.py` & `HighResAnalysis-0.0.3/HighResAnalysis/plotting/draw.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,14 +22,15 @@
 from fastcore.script import *
 from functools import partial
 from inspect import signature
 from typing import Any
 from warnings import catch_warnings, simplefilter
 from pathlib import Path
 from os.path import join
+from os import environ
 from copy import deepcopy
 from datetime import datetime
 
 from ROOT import TGraphErrors, TGaxis, TLatex, TGraphAsymmErrors, TCanvas, gStyle, TLegend, TArrow, TPad, TCutG, TLine, TPaveText, TPaveStats, TH1F, TEllipse, TColor, TProfile
 from ROOT import TProfile2D, TH2F, TH3F, THStack, TMultiGraph, TPie, gROOT, TF1
 from numpy import sign, linspace, ones, ceil, append, tile, absolute, rot90, flip, argsort, ndarray, arange, diff, pi, concatenate, where, roll, indices, array_split, isnan, frombuffer, column_stack
 from scipy.stats import binned_statistic
@@ -116,18 +117,23 @@
     blue = array([0. / 255., 0. / 255., 0. / 255.], 'd')
     red = array([180. / 255., 200. / 255., 0. / 255.], 'd')
     color_gradient = TColor.CreateGradientColorTable(len(stops), stops, red, green, blue, 255)
     return array([color_gradient + ij for ij in range(255)])
 
 # %% ../../nbs/09_plotting.draw.ipynb 6
 class Draw(object):
-    try:
-        Dir = Path(__file__).resolve().parent
-    except NameError:
-        Dir = Path().resolve().parent/"HighResAnalysis"/"config"
+    if environ.get('ANALYSIS_DIR'):
+        Dir = Path(environ.get('ANALYSIS_DIR'))/"config"
+    else:
+        try:
+            Dir = Path(__file__).resolve().parent
+        except NameError:
+            Dir = Path().resolve().parent/"HighResAnalysis"/"config"
+        if 'site-packages' in str(Dir):
+            raise RuntimeError('Cannot run from the install directory. Please eihter setup an analysis dir and set $ANALYSIS_DIR variable pointing to it or run from the cloned GitHub dir')
     Verbose = False
     Config = None
     Monitor = None
     Res = None
 
     Count = {}
     Colors = get_color_gradient()
```

### Comparing `HighResAnalysis-0.0.2/HighResAnalysis/plotting/fit.py` & `HighResAnalysis-0.0.3/HighResAnalysis/plotting/fit.py`

 * *Files identical despite different names*

### Comparing `HighResAnalysis-0.0.2/HighResAnalysis/plotting/html.py` & `HighResAnalysis-0.0.3/HighResAnalysis/plotting/html.py`

 * *Files identical despite different names*

### Comparing `HighResAnalysis-0.0.2/HighResAnalysis/plotting/info.py` & `HighResAnalysis-0.0.3/HighResAnalysis/plotting/info.py`

 * *Files identical despite different names*

### Comparing `HighResAnalysis-0.0.2/HighResAnalysis/plotting/latex.py` & `HighResAnalysis-0.0.3/HighResAnalysis/plotting/latex.py`

 * *Files identical despite different names*

### Comparing `HighResAnalysis-0.0.2/HighResAnalysis/plotting/save.py` & `HighResAnalysis-0.0.3/HighResAnalysis/plotting/save.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,16 @@
 
 # %% ../../nbs/02_plotting.save.ipynb 3
 from ROOT import TFile
 from fastcore.script import *
 from os.path import join
 from . import html
 from .draw import *
-from .utils import BaseDir, remove_file, ensure_dir, choose, prep_kw
+from .utils import *
+from .utils import BaseDir
 from pathlib import Path
 
 # %% ../../nbs/02_plotting.save.ipynb 4
 class SaveDraw(Draw):
 
     Save = True
     SaveOnServer = True
```

### Comparing `HighResAnalysis-0.0.2/HighResAnalysis/plotting/utils.py` & `HighResAnalysis-0.0.3/HighResAnalysis/plotting/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,187 +9,192 @@
 
 # %% ../../nbs/06_plotting.utils.ipynb 2
 from configparser import ConfigParser, NoOptionError, NoSectionError
 from copy import deepcopy
 from datetime import datetime
 from time import time
 from json import loads, load
-from os import _exit, makedirs, remove
+from os import _exit, makedirs, remove, environ
 from os.path import exists, isfile, join, sep
 from pathlib import Path
 from subprocess import check_call, check_output
 
 from numpy import array, zeros, count_nonzero, sqrt, average, full, all, arctan2, cos, sin, corrcoef, mean
 from uncertainties import ufloat_fromstr, ufloat
 from uncertainties.core import Variable, AffineScalarFunc
 from inspect import getframeinfo, stack
 
 # %% ../../nbs/06_plotting.utils.ipynb 3
-try:
-    BaseDir = Path(__file__).resolve().parent.parent
-except NameError:
-    BaseDir = Path()
+if environ.get('ANALYSIS_DIR'):
+    BaseDir = Path(environ.get('ANALYSIS_DIR'))
+else:
+    try:
+        BaseDir = Path(__file__).resolve().parent.parent
+    except NameError:
+        BaseDir = Path().resolve()
+    if 'site-packages' in str(BaseDir):
+        raise RuntimeError('Cannot run from the install directory. Please eihter setup an analysis dir and set $ANALYSIS_DIR variable pointing to it or run from the cloned GitHub dir')
 
-# %% ../../nbs/06_plotting.utils.ipynb 4
+# %% ../../nbs/06_plotting.utils.ipynb 5
 ON = True
 
-# %% ../../nbs/06_plotting.utils.ipynb 5
+# %% ../../nbs/06_plotting.utils.ipynb 6
 OFF = False
 
-# %% ../../nbs/06_plotting.utils.ipynb 6
+# %% ../../nbs/06_plotting.utils.ipynb 7
 GREEN = '\033[92m'
 
-# %% ../../nbs/06_plotting.utils.ipynb 7
+# %% ../../nbs/06_plotting.utils.ipynb 8
 WHITE = '\033[98m'
 
-# %% ../../nbs/06_plotting.utils.ipynb 8
+# %% ../../nbs/06_plotting.utils.ipynb 9
 ENDC = '\033[0m'
 
-# %% ../../nbs/06_plotting.utils.ipynb 9
+# %% ../../nbs/06_plotting.utils.ipynb 10
 YELLOW = '\033[93m'
 
-# %% ../../nbs/06_plotting.utils.ipynb 10
+# %% ../../nbs/06_plotting.utils.ipynb 11
 CYAN = '\033[96m'
 
-# %% ../../nbs/06_plotting.utils.ipynb 11
+# %% ../../nbs/06_plotting.utils.ipynb 12
 RED = '\033[91m'
 
-# %% ../../nbs/06_plotting.utils.ipynb 12
+# %% ../../nbs/06_plotting.utils.ipynb 13
 UP1 = '\033[1A'
 
-# %% ../../nbs/06_plotting.utils.ipynb 13
+# %% ../../nbs/06_plotting.utils.ipynb 14
 ERASE = '\033[K'
 
-# %% ../../nbs/06_plotting.utils.ipynb 14
+# %% ../../nbs/06_plotting.utils.ipynb 15
 COUNT = 0
 
-# %% ../../nbs/06_plotting.utils.ipynb 15
+# %% ../../nbs/06_plotting.utils.ipynb 16
 def get_t_str():
     return datetime.now().strftime('%H:%M:%S')
 
-# %% ../../nbs/06_plotting.utils.ipynb 16
+# %% ../../nbs/06_plotting.utils.ipynb 17
 def colored(txt, color=None):
     return f'{color}{txt}{ENDC}' if color else txt
 
-# %% ../../nbs/06_plotting.utils.ipynb 17
+# %% ../../nbs/06_plotting.utils.ipynb 18
 def prnt_msg(txt, head='', color=None, blank_lines=0, endl=True, prnt=True):
     if prnt:
         print('\n' * blank_lines + f'\r{colored(f"{head}:", color):<18} {get_t_str()} --> {txt}', end='\n' if endl else ' ')
 
-# %% ../../nbs/06_plotting.utils.ipynb 18
+# %% ../../nbs/06_plotting.utils.ipynb 19
 def info(txt, blank_lines=0, endl=True, prnt=True):
     prnt_msg(txt, 'INFO', GREEN, blank_lines, endl, prnt)
     return time()
 
-# %% ../../nbs/06_plotting.utils.ipynb 19
+# %% ../../nbs/06_plotting.utils.ipynb 20
 def add_to_info(t, msg='Done', color=None, prnt=True):
     print(colored(f'{msg} ({time() - t:2.2f} s)', color)) if prnt else do_nothing()
 
-# %% ../../nbs/06_plotting.utils.ipynb 20
+# %% ../../nbs/06_plotting.utils.ipynb 21
 def warning(txt, blank_lines=0, prnt=True):
     prnt_msg(txt, 'WARNING', YELLOW, blank_lines, prnt=prnt)
 
-# %% ../../nbs/06_plotting.utils.ipynb 21
+# %% ../../nbs/06_plotting.utils.ipynb 22
 def critical(txt):
     i = getframeinfo(stack()[1][0])
     print(f'{sep.join(Path(i.filename).parts[-2:])}: {i.lineno}')
     prnt_msg(txt, 'CRITICAL', RED)
     _exit(2)
 
-# %% ../../nbs/06_plotting.utils.ipynb 22
+# %% ../../nbs/06_plotting.utils.ipynb 23
 def get_stat(status):
     return 'ON' if status else 'OFF'
 
-# %% ../../nbs/06_plotting.utils.ipynb 23
+# %% ../../nbs/06_plotting.utils.ipynb 24
 def choose(v, default, decider='None', *args, **kwargs):
     use_default = decider is None if decider != 'None' else v is None  # noqa
     if callable(default) and use_default:
         default = default(*args, **kwargs)
     return default if use_default else v(*args, **kwargs) if callable(v) else v
 
-# %% ../../nbs/06_plotting.utils.ipynb 25
+# %% ../../nbs/06_plotting.utils.ipynb 26
 def round_up_to(num, val=1):
     return int(num) // val * val + val
 
-# %% ../../nbs/06_plotting.utils.ipynb 26
+# %% ../../nbs/06_plotting.utils.ipynb 27
 def do(fs, pars, exe=-1):
     fs, pars = ([fs], [pars]) if type(fs) is not list else (fs, pars)  # noqa
     exe = pars if exe == -1 else [exe]
     for f, p, e in zip(fs, pars, exe):
         f(p) if e is not None else do_nothing()
 
-# %% ../../nbs/06_plotting.utils.ipynb 27
+# %% ../../nbs/06_plotting.utils.ipynb 28
 def do_nothing():
     pass
 
-# %% ../../nbs/06_plotting.utils.ipynb 28
+# %% ../../nbs/06_plotting.utils.ipynb 29
 def is_iter(v):
     try:
         iter(v)
         return True
     except TypeError:
         return False
 
-# %% ../../nbs/06_plotting.utils.ipynb 29
+# %% ../../nbs/06_plotting.utils.ipynb 30
 def is_ufloat(value):
     return type(value) in [Variable, AffineScalarFunc, AsymVar]
 
-# %% ../../nbs/06_plotting.utils.ipynb 30
+# %% ../../nbs/06_plotting.utils.ipynb 31
 def uarr2n(x):
     return array([i.n for i in x]) if len(x) and is_ufloat(x[0]) else x
 
-# %% ../../nbs/06_plotting.utils.ipynb 31
+# %% ../../nbs/06_plotting.utils.ipynb 32
 def uarr2s(arr):
     return array([i.s for i in arr]) if len(arr) and is_ufloat(arr[0]) else arr
 
-# %% ../../nbs/06_plotting.utils.ipynb 32
+# %% ../../nbs/06_plotting.utils.ipynb 33
 def arr2u(x, ex):
     return array([ufloat(i, e) for i, e in zip(x, ex)])
 
-# %% ../../nbs/06_plotting.utils.ipynb 33
+# %% ../../nbs/06_plotting.utils.ipynb 34
 def add_err(u, e):
     return u + ufloat(0, e)
 
-# %% ../../nbs/06_plotting.utils.ipynb 34
+# %% ../../nbs/06_plotting.utils.ipynb 35
 def add_perr(u, e):
     return u * ufloat(1, e)
 
-# %% ../../nbs/06_plotting.utils.ipynb 35
+# %% ../../nbs/06_plotting.utils.ipynb 36
 def eff2u(eff):
     return ufloat(eff[0], mean(eff[1:])) if eff.shape == (3,) else array([eff2u(e) for e in eff])
 
-# %% ../../nbs/06_plotting.utils.ipynb 36
+# %% ../../nbs/06_plotting.utils.ipynb 37
 def make_ufloat(n, s=0):
     return (eff2u(n) if len(n) == 3 and s == 0 else array([ufloat(*v) for v in array([n, s]).T])) if is_iter(n) else n if is_ufloat(n) else ufloat(n, s)
 
-# %% ../../nbs/06_plotting.utils.ipynb 37
+# %% ../../nbs/06_plotting.utils.ipynb 38
 def make_list(value):
     return array([value], dtype=object).flatten()
 
-# %% ../../nbs/06_plotting.utils.ipynb 38
+# %% ../../nbs/06_plotting.utils.ipynb 39
 def prep_kw(dic, **default):
     d = deepcopy(dic)
     for kw, value in default.items():
         if kw not in d:
             d[kw] = value
     return d
 
-# %% ../../nbs/06_plotting.utils.ipynb 39
+# %% ../../nbs/06_plotting.utils.ipynb 40
 def get_kw(kw, kwargs, default=None):
     return kwargs[kw] if kw in kwargs else default
 
-# %% ../../nbs/06_plotting.utils.ipynb 40
+# %% ../../nbs/06_plotting.utils.ipynb 41
 def rm_key(d, *key):
     d = deepcopy(d)
     for k in key:
         if k in d:
             del d[k]
     return d
 
-# %% ../../nbs/06_plotting.utils.ipynb 41
+# %% ../../nbs/06_plotting.utils.ipynb 42
 def mean_sigma(values, weights=None, err=True):
     """ Return the weighted average and standard deviation. values, weights -- Numpy ndarrays with the same shape. """
     if len(values) == 1:
         value = make_ufloat(values[0])
         return (value, ufloat(value.s, 0)) if err else (value.n, value.s)
     weights = full(len(values), 1) if weights is None else weights
     # variance defined weights: https://en.wikipedia.org/wiki/Inverse-variance_weighting
@@ -202,88 +207,88 @@
         return [0, 0]
     n, avrg = values.size, average(values, weights=weights)
     sigma = sqrt(n / (n - 1) * average((values - avrg) ** 2, weights=weights))  # Fast and numerically precise
     m = ufloat(avrg, sqrt(1 / sum(weights))) if use_variance else ufloat(avrg, sigma / sqrt(len(values) - 1))
     s = ufloat(sigma, sigma / sqrt(2 * len(values)))
     return (m, s) if err else (m.n, s.n)
 
-# %% ../../nbs/06_plotting.utils.ipynb 42
+# %% ../../nbs/06_plotting.utils.ipynb 43
 def calc_eff(k=0, n=0, values=None):
     values = array(values) if values is not None else None
     if n == 0 and (values is None or not values.size):
         return zeros(3)
     k = float(k if values is None else count_nonzero(values))
     n = float(n if values is None else values.size)
     m = (k + 1) / (n + 2)
     mode = k / n
     s = sqrt(((k + 1) / (n + 2) * (k + 2) / (n + 3) - ((k + 1) ** 2) / ((n + 2) ** 2)))
     return array([mode, max(s + (mode - m), 0), max(s - (mode - m), 0)]) * 100
 
-# %% ../../nbs/06_plotting.utils.ipynb 43
+# %% ../../nbs/06_plotting.utils.ipynb 44
 def cart2pol(x, y):
     return array([sqrt(x ** 2 + y ** 2), arctan2(y, x)])
 
-# %% ../../nbs/06_plotting.utils.ipynb 44
+# %% ../../nbs/06_plotting.utils.ipynb 45
 def pol2cart(rho, phi):
     return array([rho * cos(phi), rho * sin(phi)])
 
-# %% ../../nbs/06_plotting.utils.ipynb 45
+# %% ../../nbs/06_plotting.utils.ipynb 46
 def get_x(x1, x2, y1, y2, y):
     return (x2 - x1) / (y2 - y1) * (y - y1) + x1
 
-# %% ../../nbs/06_plotting.utils.ipynb 46
+# %% ../../nbs/06_plotting.utils.ipynb 47
 def get_y(x1, x2, y1, y2, x):
     return get_x(y1, y2, x1, x2, x)
 
-# %% ../../nbs/06_plotting.utils.ipynb 47
+# %% ../../nbs/06_plotting.utils.ipynb 48
 def ensure_dir(path):
     if not exists(path):
         info('Creating directory: {d}'.format(d=path))
         makedirs(path)
     return path
 
-# %% ../../nbs/06_plotting.utils.ipynb 48
+# %% ../../nbs/06_plotting.utils.ipynb 49
 def remove_file(*file_path, string=None, warn=True):
     for f in file_path:
         if Path(f).exists():
             warning(f'removing {choose(string, f)}', prnt=warn)
             remove(f)
 
-# %% ../../nbs/06_plotting.utils.ipynb 49
+# %% ../../nbs/06_plotting.utils.ipynb 50
 def correlate(l1, l2):
     if len(l1.shape) == 2:
         x, y = l1.flatten(), l2.flatten()
         cut, s = (x > 0) & (y > 0), count_nonzero(x)
         return correlate(x[cut], y[cut]) if count_nonzero(cut) > .6 * s else 0
     return corrcoef(l1, l2)[0][1]
 
-# %% ../../nbs/06_plotting.utils.ipynb 50
+# %% ../../nbs/06_plotting.utils.ipynb 51
 def add_spaces(s):
     return ''.join(f' {s[i]}' if i and (s[i].isupper() or s[i].isdigit()) and not s[i - 1].isdigit() and not s[i - 1].isupper() else s[i] for i in range(len(s)))
 
-# %% ../../nbs/06_plotting.utils.ipynb 51
+# %% ../../nbs/06_plotting.utils.ipynb 52
 def print_check(reset=False):
     global COUNT
     COUNT = 0 if reset else COUNT
     print('======={}========'.format(COUNT))
     COUNT += 1
 
-# %% ../../nbs/06_plotting.utils.ipynb 52
+# %% ../../nbs/06_plotting.utils.ipynb 53
 def sum_times(t, fmt='%H:%M:%S'):
     return sum(array([datetime.strptime(i, fmt) for i in t]) - datetime.strptime('0', '%H'))
 
-# %% ../../nbs/06_plotting.utils.ipynb 53
+# %% ../../nbs/06_plotting.utils.ipynb 54
 def load_json(filename):
     if not isfile(filename):
         warning(f'json file does not exist: {filename}')
         return {}
     with open(filename) as f:
         return load(f)
 
-# %% ../../nbs/06_plotting.utils.ipynb 54
+# %% ../../nbs/06_plotting.utils.ipynb 55
 class Config(ConfigParser):
 
     def __init__(self, file_name, section=None, from_json=False, required=False, **kwargs):
         super(Config, self).__init__(**kwargs)
         self.FilePath = Path(file_name)
         if required and not self.FilePath.exists():
             critical(f'{self!r} does not exist!')
@@ -335,15 +340,15 @@
                 print(f'{option} = {self.get(key, option)}')
             print()
 
     def write(self, file_name=None, space_around_delimiters=True):
         with open(choose(file_name, self.FilePath), 'w') as f:
             super(Config, self).write(f, space_around_delimiters)
 
-# %% ../../nbs/06_plotting.utils.ipynb 55
+# %% ../../nbs/06_plotting.utils.ipynb 56
 class AsymVar:
 
     def __init__(self, value, err_down, err_up, fmt='.2f'):
         self.NominalValue = float(value)
         self.ErrDown = float(err_down)
         self.ErrUp = float(err_up)
         self.Format = fmt
@@ -439,19 +444,19 @@
     s = error
 
     @property
     def flip_errors(self):
         return AsymVar(self.n, self.s1, self.s0)
     f = flip_errors
 
-# %% ../../nbs/06_plotting.utils.ipynb 56
+# %% ../../nbs/06_plotting.utils.ipynb 57
 def aufloat(n, s0=0, s1=0):
     return AsymVar(n, s0, s1)
 
-# %% ../../nbs/06_plotting.utils.ipynb 57
+# %% ../../nbs/06_plotting.utils.ipynb 58
 def add_asym_error(v, s0=0, s1=0):
     return array([add_asym_error(i, s0, s1) for i in v], dtype=AsymVar) if is_iter(v) else AsymVar(0, s0, s1) + v
 
-# %% ../../nbs/06_plotting.utils.ipynb 58
+# %% ../../nbs/06_plotting.utils.ipynb 59
 def download_file(server, loc, target, out=True):
     cmd = f'rsync -aPvL {server}:{loc} {target}'
     return (check_call if out else check_output)(cmd, shell=True)
```

### Comparing `HighResAnalysis-0.0.2/HighResAnalysis/src/analysis.py` & `HighResAnalysis-0.0.3/HighResAnalysis/src/analysis.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 from ..plotting.save import *
 from ..plotting.utils import warning, Config, choose, info, add_to_info, GREEN, RED
 from ..utility.utils import Dir, print_banner, byte2str, ensure_dir
 
 # %% ../../nbs/32_src.analysis.ipynb 3
 class BeamTest:
-
+    " structure containing information about a beam test"
     def __init__(self, p: Path):
 
         self.Path = p
         self.Location = p.parts[-2].upper()
         self.T = datetime.strptime(p.stem, '%Y-%m')
         self.Year = self.T.year
         self.Tag = self.T.strftime('%Y%m')
```

### Comparing `HighResAnalysis-0.0.2/HighResAnalysis/src/batch_analysis.py` & `HighResAnalysis-0.0.3/HighResAnalysis/src/batch_analysis.py`

 * *Files identical despite different names*

### Comparing `HighResAnalysis-0.0.2/HighResAnalysis/src/bins.py` & `HighResAnalysis-0.0.3/HighResAnalysis/src/bins.py`

 * *Files identical despite different names*

### Comparing `HighResAnalysis-0.0.2/HighResAnalysis/src/calibration.py` & `HighResAnalysis-0.0.3/HighResAnalysis/src/calibration.py`

 * *Files identical despite different names*

### Comparing `HighResAnalysis-0.0.2/HighResAnalysis/src/converter.py` & `HighResAnalysis-0.0.3/HighResAnalysis/src/converter.py`

 * *Files identical despite different names*

### Comparing `HighResAnalysis-0.0.2/HighResAnalysis/src/currents.py` & `HighResAnalysis-0.0.3/HighResAnalysis/src/currents.py`

 * *Files identical despite different names*

### Comparing `HighResAnalysis-0.0.2/HighResAnalysis/src/cut.py` & `HighResAnalysis-0.0.3/HighResAnalysis/src/cut.py`

 * *Files identical despite different names*

### Comparing `HighResAnalysis-0.0.2/HighResAnalysis/src/dut.py` & `HighResAnalysis-0.0.3/HighResAnalysis/src/dut.py`

 * *Files identical despite different names*

### Comparing `HighResAnalysis-0.0.2/HighResAnalysis/src/dut_analysis.py` & `HighResAnalysis-0.0.3/HighResAnalysis/src/dut_analysis.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 
 # %% ../../nbs/29_src.dut_analysis.ipynb 3
 import h5py
 from typing import Any
 from pathlib import Path
 from datetime import timedelta, time, datetime
 from numpy import zeros, array, mean, sqrt
+from fastcore.utils import *
 
 import HighResAnalysis.cern.converter
 import HighResAnalysis.src.converter
 
 import HighResAnalysis.plotting.latex as tex
 import HighResAnalysis.src.bins as bins
```

### Comparing `HighResAnalysis-0.0.2/HighResAnalysis/src/proteus.py` & `HighResAnalysis-0.0.3/HighResAnalysis/src/proteus.py`

 * *Files identical despite different names*

### Comparing `HighResAnalysis-0.0.2/HighResAnalysis/src/raw.py` & `HighResAnalysis-0.0.3/HighResAnalysis/src/raw.py`

 * *Files identical despite different names*

### Comparing `HighResAnalysis-0.0.2/HighResAnalysis/src/run.py` & `HighResAnalysis-0.0.3/HighResAnalysis/src/run.py`

 * *Files 1% similar despite different names*

```diff
@@ -67,15 +67,19 @@
 
 # %% ../../nbs/30_src.run.ipynb 8
 class Batch:
     """ class containing the run infos of a single batch. """
 
     DUTName = None
 
-    def __init__(self, name, dut_nr, beam_test: BeamTest, log=None):
+    def __init__(self, name:str, # Name of the batch
+                 dut_nr:int, # DUT number
+                 beam_test: BeamTest, # Structure containing `BeamTest` info 
+                 log=None # Runlog in JSON string format
+                ):
         self.Name = name
         self.BeamTest = beam_test
         self.DataDir = beam_test.Path
         self.Log = load_runlog(self.DataDir) if log is None else log
 
         self.Runs = self.load_runs(dut_nr)
         self.FirstRun = self.Runs[0]
```

### Comparing `HighResAnalysis-0.0.2/HighResAnalysis/src/scan.py` & `HighResAnalysis-0.0.3/HighResAnalysis/src/scan.py`

 * *Files identical despite different names*

### Comparing `HighResAnalysis-0.0.2/HighResAnalysis/src/spreadsheet.py` & `HighResAnalysis-0.0.3/HighResAnalysis/src/spreadsheet.py`

 * *Files identical despite different names*

### Comparing `HighResAnalysis-0.0.2/HighResAnalysis/utility/affine_transformations.py` & `HighResAnalysis-0.0.3/HighResAnalysis/utility/affine_transformations.py`

 * *Files identical despite different names*

### Comparing `HighResAnalysis-0.0.2/HighResAnalysis/utility/utils.py` & `HighResAnalysis-0.0.3/HighResAnalysis/utility/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,274 +34,279 @@
 
 from ..plotting.utils import info, critical, add_to_info, get_kw, remove_file
 
 # %% ../../nbs/28_utility.utils.ipynb 3
 ROOT.PyConfig.IgnoreCommandLineOptions = True  # disable ROOT overwriting the help settings...
 
 # %% ../../nbs/28_utility.utils.ipynb 4
-try:
-    Dir = Path(__file__).resolve().parent.parent.parent
-except NameError:
-    Dir = Path().resolve().parent
+if environ.get('ANALYSIS_DIR'):
+    Dir = Path(environ.get('ANALYSIS_DIR'))
+else:
+    try:
+        Dir = Path(__file__).resolve().parent.parent.parent
+    except NameError:
+        Dir = Path().resolve().parent
+        if 'site-packages' in str(Dir):
+            raise RuntimeError('Cannot run from the install directory. Please eihter setup an analysis dir and set $ANALYSIS_DIR variable pointing to it or run from the cloned GitHub dir')
 
-# %% ../../nbs/28_utility.utils.ipynb 5
+# %% ../../nbs/28_utility.utils.ipynb 6
 type_dict = {'int32': 'I',
              'uint16': 's',
              'float64': 'D',
              'int64': 'L'}
 
-# %% ../../nbs/28_utility.utils.ipynb 6
+# %% ../../nbs/28_utility.utils.ipynb 7
 GREEN = '\033[92m'
 WHITE = '\033[98m'
 ENDC = '\033[0m'
 YELLOW = '\033[93m'
 CYAN = '\033[96m'
 RED = '\033[91m'
 UP1 = '\033[1A'
 ERASE = '\033[K'
 
-# %% ../../nbs/28_utility.utils.ipynb 7
+# %% ../../nbs/28_utility.utils.ipynb 8
 def move_up(n):
     print('\033[{}A'.format(n))
 
-# %% ../../nbs/28_utility.utils.ipynb 8
+# %% ../../nbs/28_utility.utils.ipynb 9
 def file_exists(filename):
     return isfile(filename)
 
-# %% ../../nbs/28_utility.utils.ipynb 9
+# %% ../../nbs/28_utility.utils.ipynb 10
 def dir_exists(path):
     return isdir(path)
 
-# %% ../../nbs/28_utility.utils.ipynb 10
+# %% ../../nbs/28_utility.utils.ipynb 11
 def time_stamp(dt, off=None):
     t = float(dt.strftime('%s'))
     return t if off is None else t - (off if off > 1 else dt.utcoffset().seconds)
 
-# %% ../../nbs/28_utility.utils.ipynb 11
+# %% ../../nbs/28_utility.utils.ipynb 12
 def print_elapsed_time(start, what='This', show=True, color=WHITE):
     string = f'Elapsed time for {what}: {get_elapsed_time(start)}'
     print_banner(string, color=color) if show else do_nothing()
     return time()
 
-# %% ../../nbs/28_utility.utils.ipynb 12
+# %% ../../nbs/28_utility.utils.ipynb 13
 def get_elapsed_time(start, hrs=False):
     t = str(timedelta(seconds=round(time() - start, 0 if hrs else 2)))
     return t if hrs else t[2:-4]
 
-# %% ../../nbs/28_utility.utils.ipynb 13
+# %% ../../nbs/28_utility.utils.ipynb 14
 def average_list(lst, n):
     return [mean(lst[i:i+n]) for i in arange(0, len(lst), n)] if n > 1 else lst
 
-# %% ../../nbs/28_utility.utils.ipynb 14
+# %% ../../nbs/28_utility.utils.ipynb 15
 def round_down_to(num, val=1):
     return int(num) // val * val
 
-# %% ../../nbs/28_utility.utils.ipynb 15
+# %% ../../nbs/28_utility.utils.ipynb 16
 def round_up_to(num, val=1):
     return int(num) // val * val + val
 
-# %% ../../nbs/28_utility.utils.ipynb 16
+# %% ../../nbs/28_utility.utils.ipynb 17
 def get_base_dir():
     return dirname(dirname(realpath(__file__)))
 
-# %% ../../nbs/28_utility.utils.ipynb 17
+# %% ../../nbs/28_utility.utils.ipynb 18
 def ensure_dir(path):
     if not exists(path):
         info('Creating directory: {d}'.format(d=path))
         makedirs(path)
     return path
 
-# %% ../../nbs/28_utility.utils.ipynb 18
+# %% ../../nbs/28_utility.utils.ipynb 19
 def isint(x):
     try:
         return float(x) == int(x)
     except (ValueError, TypeError):
         return False
 
-# %% ../../nbs/28_utility.utils.ipynb 19
+# %% ../../nbs/28_utility.utils.ipynb 20
 def is_iter(v):
     try:
         iter(v)
         return True
     except TypeError:
         return False
 
-# %% ../../nbs/28_utility.utils.ipynb 20
+# %% ../../nbs/28_utility.utils.ipynb 21
 def is_num(string):
     try:
         float(string)
         return True
     except ValueError:
         return False
 
-# %% ../../nbs/28_utility.utils.ipynb 21
+# %% ../../nbs/28_utility.utils.ipynb 22
 def colored(string, color=None):
     return string if color is None else '{}{}{}'.format(color, string, ENDC)
 
-# %% ../../nbs/28_utility.utils.ipynb 22
+# %% ../../nbs/28_utility.utils.ipynb 23
 def small_banner(msg, symbol='-', color=None):
     print(colored('\n{delim}\n{msg}\n'.format(delim=len(str(msg)) * symbol, msg=msg), color))
 
-# %% ../../nbs/28_utility.utils.ipynb 23
+# %% ../../nbs/28_utility.utils.ipynb 24
 def print_banner(msg, symbol='~', new_lines=1, color=None):
     msg = '{} |'.format(msg)
     print(colored('{n}{delim}\n{msg}\n{delim}{n}'.format(delim=len(str(msg)) * symbol, msg=msg, n='\n' * new_lines), color))
 
-# %% ../../nbs/28_utility.utils.ipynb 24
+# %% ../../nbs/28_utility.utils.ipynb 25
 def prime_factors(n):
     factors = []
     while n % 2 == 0:  # even dividers
         factors.append(2)
         n /= 2
     for i in range(3, int(sqrt(n)) + 1, 2):  # odd dividers
         while n % i == 0:
             factors.append(i)
             n /= i
     if n > 2:
         factors.append(int(n))
     return factors
 
-# %% ../../nbs/28_utility.utils.ipynb 25
+# %% ../../nbs/28_utility.utils.ipynb 26
 def do_nothing():
     pass
 
-# %% ../../nbs/28_utility.utils.ipynb 26
+# %% ../../nbs/28_utility.utils.ipynb 27
 def has_root():
     try:
         import ROOT
         return True
     except ImportError:
         return False
 
-# %% ../../nbs/28_utility.utils.ipynb 27
+# %% ../../nbs/28_utility.utils.ipynb 28
 def open_root_file(filename, option=''):
     if file_exists(filename):
         return TFile(str(filename), option)
     critical(f'The file: "{filename}" does not exist...')
 
-# %% ../../nbs/28_utility.utils.ipynb 28
+# %% ../../nbs/28_utility.utils.ipynb 29
 def create_root_file(filename, option='recreate'):
     return TFile(str(filename), option)
 
-# %% ../../nbs/28_utility.utils.ipynb 29
+# %% ../../nbs/28_utility.utils.ipynb 30
 def choose(v, default, decider='None', *args, **kwargs):
     use_default = decider is None if decider != 'None' else v is None
     if callable(default) and use_default:
         default = default(*args, **kwargs)
     return default if use_default else v
 
-# %% ../../nbs/28_utility.utils.ipynb 30
+# %% ../../nbs/28_utility.utils.ipynb 31
 def remove_letters(string):
     return ''.join(filter(lambda x: x.isdigit(), string))
 
-# %% ../../nbs/28_utility.utils.ipynb 31
+# %% ../../nbs/28_utility.utils.ipynb 32
 def remove_digits(string):
     return ''.join(filter(lambda x: not x.isdigit(), string))
 
-# %% ../../nbs/28_utility.utils.ipynb 32
+# %% ../../nbs/28_utility.utils.ipynb 33
 def interpolate_two_points(x1, y1, x2, y2, name=''):
     # f = p1*x + p0
     p1 = (y1 - y2) / (x1 - x2)
     p0 = y1 - x1 * p1
     w = abs(x2 - x1)
     fit_range = array(sorted([x1, x2])) + [-w / 3., w / 3.]
     f = TF1('fpol1{}'.format(name), 'pol1', *fit_range)
     f.SetParameters(p0, p1)
     return f
 
-# %% ../../nbs/28_utility.utils.ipynb 33
+# %% ../../nbs/28_utility.utils.ipynb 34
 def interpolate_x(x1, x2, y1, y2, y):
     p1 = get_p1(x1, x2, y1, y2)
     p0 = get_p0(x1, y1, p1)
     return (y - p0) / p1 if p1 else 0
 
-# %% ../../nbs/28_utility.utils.ipynb 34
+# %% ../../nbs/28_utility.utils.ipynb 35
 def interpolate(x1, x2, y1, y2, x):
     x1, x2, y1, y2 = [float(i) for i in [x1, x2, y1, y2]]
     p1 = get_p1(float(x1), x2, y1, y2)
     p0 = get_p0(x1, y1, p1)
     return p1 * x + p0
 
-# %% ../../nbs/28_utility.utils.ipynb 35
+# %% ../../nbs/28_utility.utils.ipynb 36
 def get_p1(x1, x2, y1, y2):
     return (y1 - y2) / (x1 - x2) if x1 != x2 else 0
 
-# %% ../../nbs/28_utility.utils.ipynb 36
+# %% ../../nbs/28_utility.utils.ipynb 37
 def get_p0(x1, y1, p1):
     return y1 - x1 * p1
 
-# %% ../../nbs/28_utility.utils.ipynb 37
+# %% ../../nbs/28_utility.utils.ipynb 38
 def make_ufloat(n, s=0):
     return array([ufloat(*v) for v in array([n, s]).T]) if is_iter(n) else n if is_ufloat(n) else ufloat(n, s)
 
-# %% ../../nbs/28_utility.utils.ipynb 38
+# %% ../../nbs/28_utility.utils.ipynb 39
 def is_ufloat(value):
     return type(value) in [Variable, AffineScalarFunc]
 
-# %% ../../nbs/28_utility.utils.ipynb 39
+# %% ../../nbs/28_utility.utils.ipynb 40
 def byte2str(v):
     n = int(log2(v) // 10) if v else 0
     return '{:1.1f} {}'.format(v / 2 ** (10 * n), ['B', 'kB', 'MB', 'GB'][n])
 
-# %% ../../nbs/28_utility.utils.ipynb 40
+# %% ../../nbs/28_utility.utils.ipynb 41
 def ev2str(v):
     n = int(log10(v) // 3)
     return f'{v / 10 ** (3 * n):.{2 if n > 1 else 0}f}{["", "k", "M"][n]}'
 
-# %% ../../nbs/28_utility.utils.ipynb 41
+# %% ../../nbs/28_utility.utils.ipynb 42
 def bias2str(*bias):
     return array([f'{i:+.0f} V' for i in bias])[... if len(bias) > 1 else 0]
 
-# %% ../../nbs/28_utility.utils.ipynb 42
+# %% ../../nbs/28_utility.utils.ipynb 43
 def bias2rootstr(*bias):
     return array([f'{i:+.0f} V'.replace('+-', '#pm').replace('+/-', '#pm').replace('+', '#plus').replace('-', '#minus') for i in bias])[... if len(bias) > 1 else 0]
 
-# %% ../../nbs/28_utility.utils.ipynb 43
+# %% ../../nbs/28_utility.utils.ipynb 44
 def get_buf(buf, n, dtype=None):
     return frombuffer(buf, dtype=buf.typecode, count=n).astype(dtype)
 
-# %% ../../nbs/28_utility.utils.ipynb 44
+# %% ../../nbs/28_utility.utils.ipynb 45
 def get_tree_vec(tree, var, cut='', dtype=None, nentries=None, firstentry=0):
     strings = make_list(var)
     n = tree.Draw(':'.join(strings), cut, 'goff', choose(nentries, tree.kMaxEntries), firstentry)
     dtypes = dtype if type(dtype) in [list, ndarray] else full(len(strings), dtype)
     vals = [get_buf(tree.GetVal(i), n, dtypes[i]) for i in range(len(strings))]
     return vals[0] if len(vals) == 1 else vals
 
-# %% ../../nbs/28_utility.utils.ipynb 45
+# %% ../../nbs/28_utility.utils.ipynb 46
 def make_list(value, dtype=None):
     v = value if is_iter(value) and not type(value) is str else array([choose(value, [])]).flatten()
     return v.tolist() if dtype == list else v.astype(dtype) if dtype is not None else v
 
-# %% ../../nbs/28_utility.utils.ipynb 46
+# %% ../../nbs/28_utility.utils.ipynb 47
 def uarr2n(arr):
     return array([i.n for i in arr]) if len(arr) and is_ufloat(arr[0]) else arr
 
-# %% ../../nbs/28_utility.utils.ipynb 47
+# %% ../../nbs/28_utility.utils.ipynb 48
 def uarr2s(arr):
     return array([i.s for i in arr]) if len(arr) and is_ufloat(arr[0]) else arr
 
-# %% ../../nbs/28_utility.utils.ipynb 48
+# %% ../../nbs/28_utility.utils.ipynb 49
 def gauss(x, scale, mean_, sigma, off=0):
     return scale * exp(-.5 * ((x - mean_) / sigma) ** 2) + off
 
-# %% ../../nbs/28_utility.utils.ipynb 49
+# %% ../../nbs/28_utility.utils.ipynb 50
 def do_hdf5(path, func, redo=False, *args, **kwargs):
     if file_exists(path) and redo:
         remove_file(path)
     if file_exists(path) and not redo:
         return h5py.File(path, 'r')['data']
     else:
         data = func(*args, **kwargs)
         f = h5py.File(path, 'w')
         info('creating {}'.format(join(basename(dirname(path)), basename(path))))
         f.create_dataset('data', data=data)
         return f['data']
 
-# %% ../../nbs/28_utility.utils.ipynb 50
+# %% ../../nbs/28_utility.utils.ipynb 51
 def do_pickle(path, func=None, value=None, redo=False, *args, **kwargs):
     if value is not None:
         with open(path, 'wb') as f:
             pickle.dump(value, f)
         return value
     try:
         if file_exists(path) and not redo:
@@ -310,50 +315,50 @@
     except ImportError:
         pass
     ret_val = func(*args, **kwargs)
     with open(path, 'wb') as f:
         pickle.dump(ret_val, f)
     return ret_val
 
-# %% ../../nbs/28_utility.utils.ipynb 51
+# %% ../../nbs/28_utility.utils.ipynb 52
 def print_table(rows, header=None, footer=None, prnt=True):
     head, foot = [choose([v], zeros((0, len(rows[0]))), v) for v in [header, footer]]
     t = concatenate([head, rows, foot]).astype('str')
     col_width = [len(max(t[:, i], key=len)) for i in range(t.shape[1])]
     total_width = sum(col_width) + len(col_width) * 3 + 1
     hline = '{}'.format('~' * total_width)
     if prnt:
         for i, row in enumerate(t):
             if i in [0] + choose([1], [], header) + choose([t.shape[0] - 1], [], footer):
                 print(hline)
             print('| {r} |'.format(r=' | '.join(word.ljust(n) for word, n in zip(row, col_width))))
         print('{}\n'.format(hline))
     return rows
 
-# %% ../../nbs/28_utility.utils.ipynb 52
+# %% ../../nbs/28_utility.utils.ipynb 53
 def merge_root_files(files, new_file_name):
     with open(devnull, 'w') as f:
         call([join(environ.get('ROOTSYS'), 'bin', 'hadd'), '-f', new_file_name] + files, stdout=f)
     info('successfully merged the single files to "{}"'.format(basename(new_file_name)))
 
 
 # ----------------------------------------
 # region CLASSES
 
-# %% ../../nbs/28_utility.utils.ipynb 53
+# %% ../../nbs/28_utility.utils.ipynb 54
 def update_pbar(func):
     @wraps(func)
     def my_func(*args, **kwargs):
         value = func(*args, **kwargs)
         if PBAR is not None and PBAR.PBar is not None and not PBAR.is_finished():
             PBAR.update()
         return value
     return my_func
 
-# %% ../../nbs/28_utility.utils.ipynb 54
+# %% ../../nbs/28_utility.utils.ipynb 55
 class PBar(object):
     def __init__(self, start=None, counter=False, t=None):
         self.PBar = None
         self.Widgets = self.init_widgets(counter, t)
         self.Step = 0
         self.N = 0
         self.start(start)
@@ -397,67 +402,67 @@
     def is_finished(self):
         return self.PBar.currval == self.N
 
     def eta(self, i, h, m, s=0):
         self.PBar.start_time = time_stamp(datetime.now() - timedelta(hours=h, minutes=m, seconds=s))
         self.update(i - 1)
 
-# %% ../../nbs/28_utility.utils.ipynb 55
+# %% ../../nbs/28_utility.utils.ipynb 56
 class EventSpeed(Widget):
     """Widget for showing the event speed (useful for slow updates)."""
 
     def __init__(self, t='s'):
         self.unit = t
         self.factor = {'s': 1, 'min': 60, 'h': 60 * 60}[t]
 
     def update(self, pbar):
         value = 0
         if pbar.seconds_elapsed > 2e-6 and pbar.currval > 2e-6:
             value = pbar.currval / pbar.seconds_elapsed * self.factor
         return f'{value:4.1f} E/{self.unit}'
 
-# %% ../../nbs/28_utility.utils.ipynb 56
+# %% ../../nbs/28_utility.utils.ipynb 57
 PBAR = PBar()
 # endregion CLASSES
 # ----------------------------------------
 
-# %% ../../nbs/28_utility.utils.ipynb 57
+# %% ../../nbs/28_utility.utils.ipynb 58
 def prep_kw(dic, **default):
     d = deepcopy(dic)
     for kw, value in default.items():
         if kw not in d:
             d[kw] = value
     return d
 
-# %% ../../nbs/28_utility.utils.ipynb 58
+# %% ../../nbs/28_utility.utils.ipynb 59
 def get_field(obj, field: str):
     if '.' in field:
         return get_field(getattr(obj, field.split('.')[0]), '.'.join(field.split('.')[1:]))
     return getattr(obj, field) if hasattr(obj, field) else None
 
-# %% ../../nbs/28_utility.utils.ipynb 59
+# %% ../../nbs/28_utility.utils.ipynb 60
 def make_suffix(*values):
     vals = [md5(val).hexdigest() if type(val) is ndarray else f'{int(val):.0f}' if isint(val) else val for val in values if val is not None]
     return '_'.join(str(val) for val in vals)
 
-# %% ../../nbs/28_utility.utils.ipynb 60
+# %% ../../nbs/28_utility.utils.ipynb 61
 def prep_suffix(f, ana, args, kwargs, suf_args, field=None):
     def_pars = signature(f).parameters
     names, values = list(def_pars.keys())[1:], [par.default for par in def_pars.values()][1:]  # first par is class instance
     i_arg = arange(len([n for n in names if n not in ['self', '_redo', '_save']])) if suf_args == 'all' else make_list(loads(str(suf_args)))
     suf_vals = [args[i] if len(args) > i else kwargs[names[i]] if names[i] in kwargs else values[i] for i in i_arg]
     suf_vals += [] if field is None else [get_field(ana, field)]
     return make_suffix(*suf_vals)
 
-# %% ../../nbs/28_utility.utils.ipynb 61
+# %% ../../nbs/28_utility.utils.ipynb 62
 def load_pickle(file_name):
     with open(file_name, 'rb') as f:
         return pickle.load(f)
 
-# %% ../../nbs/28_utility.utils.ipynb 62
+# %% ../../nbs/28_utility.utils.ipynb 63
 def save_pickle(*pargs, print_dur=False, low_rate=False, high_rate=False, suf_args='[]', field=None, verbose=False, **pkwargs):
     def inner(func):
         @wraps(func)
         def wrapper(ana, *args, **kwargs):
             run = ana.Run.get_high_rate_run(high=not low_rate) if low_rate or high_rate else None
             pickle_path = ana.make_pickle_path(*pargs, **prep_kw(pkwargs, run=run, suf=prep_suffix(func, ana, args, kwargs, suf_args, field)))
             info(f'Pickle path: {pickle_path}', prnt=verbose)
@@ -472,15 +477,15 @@
             with open(pickle_path, 'wb') as f:
                 pickle.dump(value, f)
             (ana.add_to_info if hasattr(ana, 'add_to_info') else add_to_info)(t, prnt=prnt)
             return value
         return wrapper
     return inner
 
-# %% ../../nbs/28_utility.utils.ipynb 63
+# %% ../../nbs/28_utility.utils.ipynb 64
 def save_hdf5(*pargs, arr=False, dtype=None, suf_args='[]', field=None, verbose=False, **pkwargs):
     def inner(f):
         @wraps(f)
         def wrapper(ana, *args, **kwargs):
             file_path = ana.make_hdf5_path(*pargs, **prep_kw(pkwargs, suf=prep_suffix(f, ana, args, kwargs, suf_args, field)))
             info(f'HDF5 path: {file_path}', prnt=verbose)
             redo = kwargs['_redo'] if '_redo' in kwargs else False
@@ -495,15 +500,15 @@
             remove_file(file_path)
             hf = h5py.File(file_path, 'w')
             hf.create_dataset('data', data=data.astype(choose(dtype, data.dtype)))
             return array(hf['data']) if arr else hf['data']
         return wrapper
     return inner
 
-# %% ../../nbs/28_utility.utils.ipynb 64
+# %% ../../nbs/28_utility.utils.ipynb 65
 def parallel(fp, what='something'):
     def inner(f):
         @wraps(f)
         def my_f(ana, *args, **kwargs):
             with Pool() as pool:
                 ana.info(f'generate {what} for {ana}')
                 r = f(ana, *args, **kwargs)
@@ -511,45 +516,45 @@
                 pbar = PBar(d.shape[0] // cpu_count())
                 f_ = getattr(ana.__class__, fp)
                 result = pool.starmap(_parallel, [(f_, d, i, pbar, *fargs) for i in array_split(arange(d.shape[0]), cpu_count())])
                 return concatenate(result)
         return my_f
     return inner
 
-# %% ../../nbs/28_utility.utils.ipynb 65
+# %% ../../nbs/28_utility.utils.ipynb 66
 def _parallel(f, d, i, pbar, *args):
     ret = []
     use_pbar = i[0] == 0
     for v in d[i]:
         if use_pbar:
             pbar.update()
         ret.append(f(v, *args))
     return ret
 
-# %% ../../nbs/28_utility.utils.ipynb 66
+# %% ../../nbs/28_utility.utils.ipynb 67
 def eff2u(eff):
     return ufloat(eff[0], mean(eff[1:]))
 
-# %% ../../nbs/28_utility.utils.ipynb 67
+# %% ../../nbs/28_utility.utils.ipynb 68
 def eff2str(eff, u='\\percent', f='.2f'):
     return f'\\SIerr{{{eff[0]:{f}}}}{{{eff[2]:{f}}}}{{{eff[1]:{f}}}}{{{u}}}'
 
-# %% ../../nbs/28_utility.utils.ipynb 68
+# %% ../../nbs/28_utility.utils.ipynb 69
 def show_hdf5(f: h5py.File, *include, ex_str=None):
     print('.')
     for i0, (key, grp) in enumerate(f.items()):
         if any([key == word for word in include]) or ex_str is None or ex_str not in key:
             print(f'├── {key}')
             for k, g in grp.items():
                 print(f'{"│" if i0 < len(f.keys()) - 1 else " "}   ├── {k}')
                 if hasattr(g, 'keys'):
                     for i in g.keys():
                         print(f'│   │   ├── {i}')
 
-# %% ../../nbs/28_utility.utils.ipynb 69
+# %% ../../nbs/28_utility.utils.ipynb 70
 def file_hash(fname, block_size=65536):
 
     fhash = sha256()
     with open(fname, 'rb') as f:
         fb = f.read(block_size)     # Read from the file. Take in the amount declared above
         while len(fb) > 0:          # While there is still data being read from the file
             fhash.update(fb)        # Update the hash
```

### Comparing `HighResAnalysis-0.0.2/HighResAnalysis.egg-info/.ipynb_checkpoints/PKG-INFO-checkpoint` & `HighResAnalysis-0.0.3/HighResAnalysis.egg-info/.ipynb_checkpoints/PKG-INFO-checkpoint`

 * *Files identical despite different names*

### Comparing `HighResAnalysis-0.0.2/HighResAnalysis.egg-info/.ipynb_checkpoints/SOURCES-checkpoint.txt` & `HighResAnalysis-0.0.3/HighResAnalysis.egg-info/.ipynb_checkpoints/SOURCES-checkpoint.txt`

 * *Files identical despite different names*

### Comparing `HighResAnalysis-0.0.2/HighResAnalysis.egg-info/SOURCES.txt` & `HighResAnalysis-0.0.3/HighResAnalysis.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `HighResAnalysis-0.0.2/LICENSE` & `HighResAnalysis-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `HighResAnalysis-0.0.2/settings.ini` & `HighResAnalysis-0.0.3/settings.ini`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [DEFAULT]
 repo = HighResAnalysis
 lib_name = HighResAnalysis
-version = 0.0.2
+version = 0.0.3
 min_python = 3.7
 license = apache2
 black_formatting = False
 doc_path = _docs
 lib_path = HighResAnalysis
 nbs_path = nbs
 recursive = True
```

### Comparing `HighResAnalysis-0.0.2/setup.py` & `HighResAnalysis-0.0.3/setup.py`

 * *Files identical despite different names*

