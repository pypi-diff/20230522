# Comparing `tmp/anchor_droplet_chip-0.3.2.tar.gz` & `tmp/anchor_droplet_chip-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "anchor_droplet_chip-0.3.2.tar", last modified: Fri May 12 10:06:12 2023, max compression
+gzip compressed data, was "anchor_droplet_chip-0.4.0.tar", last modified: Mon May 22 19:30:32 2023, max compression
```

## Comparing `anchor_droplet_chip-0.3.2.tar` & `anchor_droplet_chip-0.4.0.tar`

### file list

```diff
@@ -1,66 +1,67 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 10:06:12.830088 anchor_droplet_chip-0.3.2/
--rw-r--r--   0 runner    (1001) docker     (123)      195 2023-05-12 10:05:50.000000 anchor_droplet_chip-0.3.2/-- SQLite.sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 10:06:12.806088 anchor_droplet_chip-0.3.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 10:06:12.814088 anchor_droplet_chip-0.3.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     2844 2023-05-12 10:05:50.000000 anchor_droplet_chip-0.3.2/.github/workflows/python-package.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1880 2023-05-12 10:05:50.000000 anchor_droplet_chip-0.3.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1304 2023-05-12 10:05:50.000000 anchor_droplet_chip-0.3.2/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1567 2023-05-12 10:05:50.000000 anchor_droplet_chip-0.3.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5632 2023-05-12 10:06:12.830088 anchor_droplet_chip-0.3.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4724 2023-05-12 10:05:50.000000 anchor_droplet_chip-0.3.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1821 2023-05-12 10:05:50.000000 anchor_droplet_chip-0.3.2/Snakefile
--rw-r--r--   0 runner    (1001) docker     (123)    75936 2023-05-12 10:05:50.000000 anchor_droplet_chip-0.3.2/example.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)   223486 2023-05-12 10:05:50.000000 anchor_droplet_chip-0.3.2/find_all_big_nd2.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)      439 2023-05-12 10:05:50.000000 anchor_droplet_chip-0.3.2/logging.conf
--rw-r--r--   0 runner    (1001) docker     (123)      264 2023-05-12 10:05:50.000000 anchor_droplet_chip-0.3.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-12 10:05:50.000000 anchor_droplet_chip-0.3.2/runtime.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 10:06:12.818088 anchor_droplet_chip-0.3.2/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)      509 2023-05-12 10:05:50.000000 anchor_droplet_chip-0.3.2/scripts/merge_all.py
--rw-r--r--   0 runner    (1001) docker     (123)      514 2023-05-12 10:05:50.000000 anchor_droplet_chip-0.3.2/scripts/zarr.py
--rw-r--r--   0 runner    (1001) docker     (123)     1365 2023-05-12 10:06:12.830088 anchor_droplet_chip-0.3.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-05-12 10:05:50.000000 anchor_droplet_chip-0.3.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 10:06:12.810088 anchor_droplet_chip-0.3.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 10:06:12.822088 anchor_droplet_chip-0.3.2/src/adc/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 10:05:50.000000 anchor_droplet_chip-0.3.2/src/adc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6339 2023-05-12 10:05:50.000000 anchor_droplet_chip-0.3.2/src/adc/_align_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)     4470 2023-05-12 10:05:50.000000 anchor_droplet_chip-0.3.2/src/adc/_combine_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)     6206 2023-05-12 10:05:50.000000 anchor_droplet_chip-0.3.2/src/adc/_count_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)     3959 2023-05-12 10:05:50.000000 anchor_droplet_chip-0.3.2/src/adc/_manual_rois.py
--rw-r--r--   0 runner    (1001) docker     (123)     1493 2023-05-12 10:05:50.000000 anchor_droplet_chip-0.3.2/src/adc/_progress_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)     5131 2023-05-12 10:05:50.000000 anchor_droplet_chip-0.3.2/src/adc/_projection_stack.py
--rw-r--r--   0 runner    (1001) docker     (123)     8235 2023-05-12 10:05:50.000000 anchor_droplet_chip-0.3.2/src/adc/_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)     1715 2023-05-12 10:05:50.000000 anchor_droplet_chip-0.3.2/src/adc/_sample_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     9656 2023-05-12 10:05:50.000000 anchor_droplet_chip-0.3.2/src/adc/_split_stack.py
--rw-r--r--   0 runner    (1001) docker     (123)     8224 2023-05-12 10:05:50.000000 anchor_droplet_chip-0.3.2/src/adc/_sub_stack.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-12 10:06:12.000000 anchor_droplet_chip-0.3.2/src/adc/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)    10789 2023-05-12 10:05:50.000000 anchor_droplet_chip-0.3.2/src/adc/align.py
--rw-r--r--   0 runner    (1001) docker     (123)     8200 2023-05-12 10:05:50.000000 anchor_droplet_chip-0.3.2/src/adc/count.py
--rw-r--r--   0 runner    (1001) docker     (123)     1396 2023-05-12 10:05:50.000000 anchor_droplet_chip-0.3.2/src/adc/fit.py
--rw-r--r--   0 runner    (1001) docker     (123)     1117 2023-05-12 10:05:50.000000 anchor_droplet_chip-0.3.2/src/adc/io.py
--rw-r--r--   0 runner    (1001) docker     (123)     3756 2023-05-12 10:05:50.000000 anchor_droplet_chip-0.3.2/src/adc/merge.py
--rw-r--r--   0 runner    (1001) docker     (123)     2482 2023-05-12 10:05:50.000000 anchor_droplet_chip-0.3.2/src/adc/napari.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1494 2023-05-12 10:05:50.000000 anchor_droplet_chip-0.3.2/src/adc/plot.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 10:06:12.826088 anchor_droplet_chip-0.3.2/src/adc/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 10:05:50.000000 anchor_droplet_chip-0.3.2/src/adc/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1510 2023-05-12 10:05:50.000000 anchor_droplet_chip-0.3.2/src/adc/tests/test_align.py
--rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-05-12 10:05:50.000000 anchor_droplet_chip-0.3.2/src/adc/tests/test_count.py
--rw-r--r--   0 runner    (1001) docker     (123)      736 2023-05-12 10:05:50.000000 anchor_droplet_chip-0.3.2/src/adc/tests/test_projection.py
--rw-r--r--   0 runner    (1001) docker     (123)     2090 2023-05-12 10:05:50.000000 anchor_droplet_chip-0.3.2/src/adc/tests/test_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)      842 2023-05-12 10:05:50.000000 anchor_droplet_chip-0.3.2/src/adc/tests/test_split.py
--rw-r--r--   0 runner    (1001) docker     (123)     3014 2023-05-12 10:05:50.000000 anchor_droplet_chip-0.3.2/src/adc/tests/test_stack.py
--rw-r--r--   0 runner    (1001) docker     (123)      601 2023-05-12 10:05:50.000000 anchor_droplet_chip-0.3.2/src/adc/tests/test_substack.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 10:06:12.830088 anchor_droplet_chip-0.3.2/src/anchor_droplet_chip.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5632 2023-05-12 10:06:12.000000 anchor_droplet_chip-0.3.2/src/anchor_droplet_chip.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1294 2023-05-12 10:06:12.000000 anchor_droplet_chip-0.3.2/src/anchor_droplet_chip.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-12 10:06:12.000000 anchor_droplet_chip-0.3.2/src/anchor_droplet_chip.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-05-12 10:06:12.000000 anchor_droplet_chip-0.3.2/src/anchor_droplet_chip.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      137 2023-05-12 10:06:12.000000 anchor_droplet_chip-0.3.2/src/anchor_droplet_chip.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-12 10:06:12.000000 anchor_droplet_chip-0.3.2/src/anchor_droplet_chip.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 10:06:12.830088 anchor_droplet_chip-0.3.2/src/imreg_dft/
--rw-r--r--   0 runner    (1001) docker     (123)      426 2023-05-12 10:05:50.000000 anchor_droplet_chip-0.3.2/src/imreg_dft/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    26470 2023-05-12 10:05:50.000000 anchor_droplet_chip-0.3.2/src/imreg_dft/imreg.py
--rw-r--r--   0 runner    (1001) docker     (123)    28749 2023-05-12 10:05:50.000000 anchor_droplet_chip-0.3.2/src/imreg_dft/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      622 2023-05-12 10:05:50.000000 anchor_droplet_chip-0.3.2/test_data_0h.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      633 2023-05-12 10:05:50.000000 anchor_droplet_chip-0.3.2/test_data_24h.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      771 2023-05-12 10:05:50.000000 anchor_droplet_chip-0.3.2/tox.ini
--rw-r--r--   0 runner    (1001) docker     (123)    17856 2023-05-12 10:05:50.000000 anchor_droplet_chip-0.3.2/zenodo.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 19:30:32.596392 anchor_droplet_chip-0.4.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      195 2023-05-22 19:30:14.000000 anchor_droplet_chip-0.4.0/-- SQLite.sql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 19:30:32.584392 anchor_droplet_chip-0.4.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 19:30:32.588392 anchor_droplet_chip-0.4.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     2844 2023-05-22 19:30:14.000000 anchor_droplet_chip-0.4.0/.github/workflows/python-package.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1880 2023-05-22 19:30:14.000000 anchor_droplet_chip-0.4.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1304 2023-05-22 19:30:14.000000 anchor_droplet_chip-0.4.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1567 2023-05-22 19:30:14.000000 anchor_droplet_chip-0.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5632 2023-05-22 19:30:32.596392 anchor_droplet_chip-0.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4724 2023-05-22 19:30:14.000000 anchor_droplet_chip-0.4.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1821 2023-05-22 19:30:14.000000 anchor_droplet_chip-0.4.0/Snakefile
+-rw-r--r--   0 runner    (1001) docker     (123)    75936 2023-05-22 19:30:14.000000 anchor_droplet_chip-0.4.0/example.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)   223486 2023-05-22 19:30:14.000000 anchor_droplet_chip-0.4.0/find_all_big_nd2.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)      439 2023-05-22 19:30:14.000000 anchor_droplet_chip-0.4.0/logging.conf
+-rw-r--r--   0 runner    (1001) docker     (123)      264 2023-05-22 19:30:14.000000 anchor_droplet_chip-0.4.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     4165 2023-05-22 19:30:14.000000 anchor_droplet_chip-0.4.0/recursion.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-22 19:30:14.000000 anchor_droplet_chip-0.4.0/runtime.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 19:30:32.588392 anchor_droplet_chip-0.4.0/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)      509 2023-05-22 19:30:14.000000 anchor_droplet_chip-0.4.0/scripts/merge_all.py
+-rw-r--r--   0 runner    (1001) docker     (123)      514 2023-05-22 19:30:14.000000 anchor_droplet_chip-0.4.0/scripts/zarr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1365 2023-05-22 19:30:32.596392 anchor_droplet_chip-0.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-05-22 19:30:14.000000 anchor_droplet_chip-0.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 19:30:32.584392 anchor_droplet_chip-0.4.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 19:30:32.596392 anchor_droplet_chip-0.4.0/src/adc/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 19:30:14.000000 anchor_droplet_chip-0.4.0/src/adc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6359 2023-05-22 19:30:14.000000 anchor_droplet_chip-0.4.0/src/adc/_align_widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4470 2023-05-22 19:30:14.000000 anchor_droplet_chip-0.4.0/src/adc/_combine_widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6658 2023-05-22 19:30:14.000000 anchor_droplet_chip-0.4.0/src/adc/_count_widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3959 2023-05-22 19:30:14.000000 anchor_droplet_chip-0.4.0/src/adc/_manual_rois.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1493 2023-05-22 19:30:14.000000 anchor_droplet_chip-0.4.0/src/adc/_progress_widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5131 2023-05-22 19:30:14.000000 anchor_droplet_chip-0.4.0/src/adc/_projection_stack.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8617 2023-05-22 19:30:14.000000 anchor_droplet_chip-0.4.0/src/adc/_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1715 2023-05-22 19:30:14.000000 anchor_droplet_chip-0.4.0/src/adc/_sample_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9656 2023-05-22 19:30:14.000000 anchor_droplet_chip-0.4.0/src/adc/_split_stack.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8329 2023-05-22 19:30:14.000000 anchor_droplet_chip-0.4.0/src/adc/_sub_stack.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-22 19:30:32.000000 anchor_droplet_chip-0.4.0/src/adc/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11429 2023-05-22 19:30:14.000000 anchor_droplet_chip-0.4.0/src/adc/align.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14100 2023-05-22 19:30:14.000000 anchor_droplet_chip-0.4.0/src/adc/count.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1396 2023-05-22 19:30:14.000000 anchor_droplet_chip-0.4.0/src/adc/fit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1117 2023-05-22 19:30:14.000000 anchor_droplet_chip-0.4.0/src/adc/io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3756 2023-05-22 19:30:14.000000 anchor_droplet_chip-0.4.0/src/adc/merge.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2482 2023-05-22 19:30:14.000000 anchor_droplet_chip-0.4.0/src/adc/napari.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1494 2023-05-22 19:30:14.000000 anchor_droplet_chip-0.4.0/src/adc/plot.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 19:30:32.596392 anchor_droplet_chip-0.4.0/src/adc/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 19:30:14.000000 anchor_droplet_chip-0.4.0/src/adc/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1031 2023-05-22 19:30:14.000000 anchor_droplet_chip-0.4.0/src/adc/tests/test_align.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2127 2023-05-22 19:30:14.000000 anchor_droplet_chip-0.4.0/src/adc/tests/test_count.py
+-rw-r--r--   0 runner    (1001) docker     (123)      736 2023-05-22 19:30:14.000000 anchor_droplet_chip-0.4.0/src/adc/tests/test_projection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2090 2023-05-22 19:30:14.000000 anchor_droplet_chip-0.4.0/src/adc/tests/test_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)      842 2023-05-22 19:30:14.000000 anchor_droplet_chip-0.4.0/src/adc/tests/test_split.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3014 2023-05-22 19:30:14.000000 anchor_droplet_chip-0.4.0/src/adc/tests/test_stack.py
+-rw-r--r--   0 runner    (1001) docker     (123)      601 2023-05-22 19:30:14.000000 anchor_droplet_chip-0.4.0/src/adc/tests/test_substack.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 19:30:32.596392 anchor_droplet_chip-0.4.0/src/anchor_droplet_chip.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5632 2023-05-22 19:30:32.000000 anchor_droplet_chip-0.4.0/src/anchor_droplet_chip.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1310 2023-05-22 19:30:32.000000 anchor_droplet_chip-0.4.0/src/anchor_droplet_chip.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 19:30:32.000000 anchor_droplet_chip-0.4.0/src/anchor_droplet_chip.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-05-22 19:30:32.000000 anchor_droplet_chip-0.4.0/src/anchor_droplet_chip.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-05-22 19:30:32.000000 anchor_droplet_chip-0.4.0/src/anchor_droplet_chip.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-22 19:30:32.000000 anchor_droplet_chip-0.4.0/src/anchor_droplet_chip.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 19:30:32.596392 anchor_droplet_chip-0.4.0/src/imreg_dft/
+-rw-r--r--   0 runner    (1001) docker     (123)      426 2023-05-22 19:30:14.000000 anchor_droplet_chip-0.4.0/src/imreg_dft/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26470 2023-05-22 19:30:14.000000 anchor_droplet_chip-0.4.0/src/imreg_dft/imreg.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28749 2023-05-22 19:30:14.000000 anchor_droplet_chip-0.4.0/src/imreg_dft/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      622 2023-05-22 19:30:14.000000 anchor_droplet_chip-0.4.0/test_data_0h.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      633 2023-05-22 19:30:14.000000 anchor_droplet_chip-0.4.0/test_data_24h.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      771 2023-05-22 19:30:14.000000 anchor_droplet_chip-0.4.0/tox.ini
+-rw-r--r--   0 runner    (1001) docker     (123)    17856 2023-05-22 19:30:14.000000 anchor_droplet_chip-0.4.0/zenodo.ipynb
```

### Comparing `anchor_droplet_chip-0.3.2/.github/workflows/python-package.yml` & `anchor_droplet_chip-0.4.0/.github/workflows/python-package.yml`

 * *Files identical despite different names*

### Comparing `anchor_droplet_chip-0.3.2/.gitignore` & `anchor_droplet_chip-0.4.0/.gitignore`

 * *Files identical despite different names*

### Comparing `anchor_droplet_chip-0.3.2/.pre-commit-config.yaml` & `anchor_droplet_chip-0.4.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `anchor_droplet_chip-0.3.2/LICENSE` & `anchor_droplet_chip-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `anchor_droplet_chip-0.3.2/PKG-INFO` & `anchor_droplet_chip-0.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: anchor_droplet_chip
-Version: 0.3.2
+Version: 0.4.0
 Summary: Segment organoids and measure intensities
 Home-page: https://github.com/BaroudLab/anchor-driplet-chip
 Author: Andrey Aristov
 Author-email: aaristov@pasteur.fr
 License: BSD-3-Clause
 Project-URL: Source Code, https://github.com/BaroudLab/anchor-droplet-chip
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `anchor_droplet_chip-0.3.2/README.md` & `anchor_droplet_chip-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `anchor_droplet_chip-0.3.2/Snakefile` & `anchor_droplet_chip-0.4.0/Snakefile`

 * *Files identical despite different names*

### Comparing `anchor_droplet_chip-0.3.2/example.ipynb` & `anchor_droplet_chip-0.4.0/example.ipynb`

 * *Files identical despite different names*

### Comparing `anchor_droplet_chip-0.3.2/find_all_big_nd2.ipynb` & `anchor_droplet_chip-0.4.0/find_all_big_nd2.ipynb`

 * *Files identical despite different names*

### Comparing `anchor_droplet_chip-0.3.2/scripts/zarr.py` & `anchor_droplet_chip-0.4.0/scripts/zarr.py`

 * *Files identical despite different names*

### Comparing `anchor_droplet_chip-0.3.2/setup.cfg` & `anchor_droplet_chip-0.4.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `anchor_droplet_chip-0.3.2/src/adc/_align_widget.py` & `anchor_droplet_chip-0.4.0/src/adc/_align_widget.py`

 * *Files 2% similar despite different names*

```diff
@@ -180,22 +180,23 @@
         - tvec["tvec"]
         + np.array(figure_size) / 2.0
     )
 
 
 def locate_wells(bf, template, ccenters):
     try:
-        tvec = align.reg.similarity(
-            align.pad(template, bf.shape),
-            bf,
+        tvec = align.get_transform(
+            image=bf, 
+            template=template,
             constraints={
                 "scale": [1, 0.1],
                 "tx": [0, 150],
                 "ty": [0, 150],
                 "angle": [0, 10],
             },
+            pad_ratio=1.3
         )
         logger.info(tvec)
         return move_centers(ccenters, tvec, bf.shape)
     except Exception as e:
         logger.error("Error locating wells: ", e)
         return ccenters
```

### Comparing `anchor_droplet_chip-0.3.2/src/adc/_combine_widget.py` & `anchor_droplet_chip-0.4.0/src/adc/_combine_widget.py`

 * *Files identical despite different names*

### Comparing `anchor_droplet_chip-0.3.2/src/adc/_count_widget.py` & `anchor_droplet_chip-0.4.0/src/adc/_count_widget.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 import json
 import logging
 import os
 from asyncio.log import logger
-from functools import partial, reduce
-from operator import add
 
 import dask.array as da
 import numpy as np
 import pandas as pd
 from magicgui.widgets import Container, create_widget
 from napari import Viewer
 from napari.layers import Image, Points
 from napari.utils import progress
 from napari.utils.notifications import show_error, show_info
 from qtpy.QtWidgets import QLineEdit, QPushButton, QVBoxLayout, QWidget
 
 from adc import count
 
+from ._align_widget import DROPLETS_CSV_SUFFIX
+
+TABLE_NAME = "table.csv"
+
 COUNTS_LAYER_PROPS = dict(
-    name="Counts",
-    face_color="#ffffff00",
-    edge_color="#ff007f00",
+    name="Counts", size=300, face_color="#00000000", edge_color="#00880088"
 )
 COUNTS_JSON_SUFFIX = ".counts.json"
 
 DETECTION_LAYER_PROPS = dict(
     name="Detections",
     size=20,
     face_color="#ffffff00",
@@ -47,105 +47,106 @@
             label="TRITC",
         )
         self.radius = 300
         self.select_centers = create_widget(label="centers", annotation=Points)
         self.container = Container(
             widgets=[self.select_TRITC, self.select_centers]
         )
+        self.out = []
+        self.counts_layer = None
+        self.detections_layer = None
 
         self.out_path = ""
         self.output_filename_widget = QLineEdit("path")
         self.btn = QPushButton("Localize!")
-        self.btn.clicked.connect(self._update_detections)
+        self.btn.clicked.connect(self.process_stack)
         self.layout = QVBoxLayout()
         self.layout.addWidget(self.container.native)
         self.layout.addWidget(self.btn)
         self.layout.addStretch()
 
         # self.viewer.layers.events.inserted.connect(self.reset_choices)
         # self.viewer.layers.events.removed.connect(self.reset_choices)
         # self.reset_choices(self.viewer.layers.events.inserted)
 
         self.setLayout(self.layout)
 
-    def _update_detections(self):
-        show_info("Loading the data")
-        with progress(desc="Loading data") as prb:
-            selected_layer = self.viewer.layers[
-                self.select_TRITC.current_choice
-            ]
-            logger.debug(f"selected_layer: {selected_layer}")
-            if selected_layer.multiscale:
-                ddata = selected_layer.data[0]
-                logger.debug(
-                    f"multiscale data: selecting highest resolution: {ddata}"
-                )
-            else:
-                ddata = selected_layer.data
-                logger.debug(f"not multiscale data: {ddata}")
-            if isinstance(ddata, da.Array):
-                ddata = ddata.compute()
-                logger.debug(f"compute dask array: {ddata}")
-            if ddata.ndim == 2:
-                ddata = np.reshape(ddata, (1, *ddata.shape))
-                logger.debug(f"reshaping: {ddata}")
-            else:
-                logger.debug("Finished data loading")
-            prb.close()
-
-        centers = (
-            centers_layer := self.viewer.layers[
-                self.select_centers.current_choice
-            ]
-        ).data
-        logger.debug(f"selected centers: {centers}")
-        try:
-            logger.debug(f"creating dataframe with columns ['chip', 'y', 'x']")
-            self.df = pd.DataFrame(data=centers, columns=["chip", "y", "x"])
-            logger.debug(f"created dataframe {self.df}")
-        except ValueError as e:
-            logger.debug(f"problem with dataframe {e}")
-            show_error("Choose the right layer with actual localizations")
-            return
+    def process_stack(self):
+        self._pick_data_ref()
+        self._pick_centers()
+
         show_info("Data loaded. Counting")
+
         self.viewer.window._status_bar._toggle_activity_dock(True)
-        peaks_raw = list(
-            map(
-                partial(
-                    count.get_global_coordinates_from_well_coordinates,
-                    fluo=ddata,
-                    size=self.radius,
-                ),
-                progress(centers, desc="Localizing:"),
+
+        self._update_detections()
+
+    def _pick_data_ref(self):
+        "Get dask array to know the shape etc"
+        self.selected_layer = self.viewer.layers[
+            self.select_TRITC.current_choice
+        ]
+        logger.debug(f"selected_layer: {self.selected_layer}")
+        if self.selected_layer.multiscale:
+            self.ddata_ref = self.selected_layer.data[0]
+            logger.debug(
+                f"multiscale data: selecting highest resolution: {self.ddata_ref}"
             )
-        )
-        show_info("Done localizing")
-        n_peaks_per_well = list(map(len, peaks_raw))
-        detections = reduce(add, peaks_raw)
+        else:
+            self.ddata_ref = self.selected_layer.data
+            logger.debug(f"not multiscale data: {self.ddata_ref}")
+
+    def _pick_centers(self):
+        self.centers_layer = self.viewer.layers[
+            self.select_centers.current_choice
+        ]
+        self.centers = self.centers_layer.data
+        logger.debug(f"selected centers: {len(self.centers)}")
 
-        counts_layer = self.viewer.add_points(
-            centers_layer.data, text=n_peaks_per_well, **COUNTS_LAYER_PROPS
+    def _update_detections(self):
+        logger.debug("Creating output layers")
+        self.detections_layer = self.viewer.add_points(
+            data=[[0, 0, 0, 0]], **DETECTION_LAYER_PROPS
         )
-
-        detections_layer = self.viewer.add_points(
-            detections, **DETECTION_LAYER_PROPS
+        self.counts_layer = self.viewer.add_points(
+            data=[[0, 0, 0, 0]], text=[], **COUNTS_LAYER_PROPS
         )
+        logger.debug("Creating worker")
+        self.out = count.count_recursive(
+            data=self.ddata_ref,
+            positions=self.centers,
+            size=self.radius,
+            progress=progress,
+        )
+        self.save_results()
+
+    def save_results(self):
+        show_info("Done localizing ")
+
+        locs, n_peaks_per_well, drops, table_df = self.out
+
+        self.detections_layer.data = locs
+        self.counts_layer.data = drops
+        self.counts_layer.text = n_peaks_per_well
+
         try:
-            path = selected_layer.source.path
-            detections_layer.save(
+            path = self.selected_layer.source.path
+            if path is None:
+                try:
+                    path = self.selected_layer.metadata["path"]
+                except KeyError:
+                    show_error("Unable to find the path")
+                    return
+            self.detections_layer.save(
                 ppp := os.path.join(path, DETECTION_CSV_SUFFIX)
             )
-            with open(
-                pppc := os.path.join(path, COUNTS_JSON_SUFFIX), "w"
-            ) as fp:
-                json.dump(n_peaks_per_well, fp, indent=2)
         except Exception as e:
             logger.debug(f"Unable to save detections inside the zarr: {e}")
             logger.debug(f"Saving in a separate file")
-            detections_layer.save(
+            self.detections_layer.save(
                 ppp := os.path.join(path + DETECTION_CSV_SUFFIX)
             )
         logger.info(f"Saving detections into {ppp}")
 
         try:
             with open(
                 ppp := os.path.join(path, COUNTS_JSON_SUFFIX), "w"
@@ -155,14 +156,35 @@
             logger.debug(f"Unable to save counts inside the zarr: {e}")
             logger.debug(f"Saving in a separate file")
 
             with open(ppp := path + COUNTS_JSON_SUFFIX, "w") as fp:
                 json.dump(n_peaks_per_well, fp, indent=2)
         logger.info(f"Saving counts into {ppp}")
 
+        try:
+            ppp = os.path.join(path, DROPLETS_CSV_SUFFIX)
+            droplets_df = pd.DataFrame(
+                data=drops, columns=[f"axis-{i}" for i in range(len(drops[0]))]
+            )
+            droplets_df.to_csv(ppp)
+        except Exception as e:
+            logger.debug(f"Unable to save droplets inside the zarr: {e}")
+            logger.debug(f"Saving in a separate file")
+
+            droplets_df.to_csv(ppp := path + DROPLETS_CSV_SUFFIX)
+        logger.info(f"Saving counts into {ppp}")
+
+        try:
+            ppp = os.path.join(os.path.dirname(path), TABLE_NAME)
+
+            table_df.to_csv(ppp)
+            logger.info(f"Saving table into {ppp}")
+        except Exception as e:
+            logger.error(f"Unable to save table into {ppp}: {e}")
+
     def show_counts(self, counts):
         self.counts = counts
         logger.debug(counts)
 
     def _update_path(self):
         BF = self.select_BF.current_choice
         TRITC = self.select_TRITC.current_choice
```

### Comparing `anchor_droplet_chip-0.3.2/src/adc/_manual_rois.py` & `anchor_droplet_chip-0.4.0/src/adc/_manual_rois.py`

 * *Files identical despite different names*

### Comparing `anchor_droplet_chip-0.3.2/src/adc/_progress_widget.py` & `anchor_droplet_chip-0.4.0/src/adc/_progress_widget.py`

 * *Files identical despite different names*

### Comparing `anchor_droplet_chip-0.3.2/src/adc/_projection_stack.py` & `anchor_droplet_chip-0.4.0/src/adc/_projection_stack.py`

 * *Files identical despite different names*

### Comparing `anchor_droplet_chip-0.3.2/src/adc/_reader.py` & `anchor_droplet_chip-0.4.0/src/adc/_reader.py`

 * *Files 10% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 
 from ._align_widget import DROPLETS_CSV_SUFFIX, DROPLETS_LAYER_PROPS
 from ._count_widget import (
     COUNTS_JSON_SUFFIX,
     COUNTS_LAYER_PROPS,
     DETECTION_CSV_SUFFIX,
     DETECTION_LAYER_PROPS,
+    TABLE_NAME,
 )
 
 logger = logging.getLogger(__name__)
 # logger.setLevel(logging.DEBUG)
 
 
 def napari_get_reader(path):
@@ -218,50 +219,63 @@
     ]
 
     if os.path.exists(det_path := os.path.join(path, DETECTION_CSV_SUFFIX)):
         try:
             table = pd.read_csv(det_path, index_col=0)
             output.append(
                 (
-                    table[["axis-0", "axis-1", "axis-2"]].values,
+                    table.values,
                     {"metadata": {"path": det_path}, **DETECTION_LAYER_PROPS},
                     "points",
                 )
             )
         except Exception as e:
             print(f"no detections found: {e}")
     else:
         print(f"{det_path} doesn't exists")
 
-    if os.path.exists(det_path := os.path.join(path, DROPLETS_CSV_SUFFIX)):
+    if os.path.exists(droplet_path := os.path.join(path, DROPLETS_CSV_SUFFIX)):
         try:
-            table = pd.read_csv(det_path, index_col=0)
+            droplets_df = pd.read_csv(droplet_path, index_col=0)
             if os.path.exists(
                 count_path := os.path.join(path, COUNTS_JSON_SUFFIX)
             ):
                 with open(count_path) as fp:
                     counts = json.load(fp)
             else:
                 counts = None
             output.append(
                 (
-                    table[["axis-0", "axis-1", "axis-2"]].values,
+                    droplets_df.values,
                     {
                         "metadata": {"path": det_path},
                         "text": counts,
                         **COUNTS_LAYER_PROPS,
                     },
                     "points",
                 )
             )
         except Exception as e:
             print(f"no detections found: {e}")
     else:
         print(f"{det_path} doesn't exists")
 
+    if not os.path.exists(
+        ppp := os.path.join(os.path.dirname(path), TABLE_NAME)
+    ):
+        from .count import make_table
+
+        try:
+            df = make_table(droplets_out=droplets_df.values, counts=counts)
+            df.to_csv(ppp)
+            print(f"Saved table to {ppp}")
+        except Exception as e:
+            print(f"Unable to create table")
+    else:
+        print("Table found")
     return output
 
 
 def read_nd2(path):
     print(f"opening {path}")
     data = nd2.ND2File(path)
     print(data.sizes)
```

### Comparing `anchor_droplet_chip-0.3.2/src/adc/_sample_data.py` & `anchor_droplet_chip-0.4.0/src/adc/_sample_data.py`

 * *Files identical despite different names*

### Comparing `anchor_droplet_chip-0.3.2/src/adc/_split_stack.py` & `anchor_droplet_chip-0.4.0/src/adc/_split_stack.py`

 * *Files identical despite different names*

### Comparing `anchor_droplet_chip-0.3.2/src/adc/_sub_stack.py` & `anchor_droplet_chip-0.4.0/src/adc/_sub_stack.py`

 * *Files 2% similar despite different names*

```diff
@@ -187,18 +187,23 @@
             logger.debug(f"set pixel_size_um to None")
             show_warning(f"No pixel_size_um found in metadata")
         try:
             self.dask_array = self.selected_layer.metadata["dask_data"]
             logger.debug(f"dask array from metadata {self.dask_array}")
 
         except KeyError:
-            if not isinstance(self.selected_layer.data, da.Array):
-                self.dask_array = da.from_array(self.selected_layer.data)
+            if self.selected_layer.multiscale:
+                data = self.selected_layer.data[0]
             else:
-                self.dask_array = self.selected_layer.data
+                data = self.selected_layer.data
+
+            if not isinstance(data, da.Array):
+                self.dask_array = da.from_array(data)
+            else:
+                self.dask_array = data
             show_warning(
                 f"No dask_data found in metadata {self.selected_layer.metadata}, creating one {self.dask_array}"
             )
             logger.debug(f"dask array from array {self.dask_array}")
 
         self.out_dask = self.dask_array
         self.populate_dims()
```

### Comparing `anchor_droplet_chip-0.3.2/src/adc/align.py` & `anchor_droplet_chip-0.4.0/src/adc/align.py`

 * *Files 5% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 
 try:
     __version__ = version("anchor-droplet-chip")
 except PackageNotFoundError:
     # package is not installed
     __version__ = "Unknown"
 logger = logging.getLogger("adc.align")
+logger.setLevel(logging.DEBUG)
 
 
 GREY = np.array([np.arange(256)] * 3, dtype="uint8")
 RED = np.array(
     [np.arange(256), np.zeros((256,)), np.zeros((256,))], dtype="uint8"
 )
 GREEN = np.array(
@@ -49,14 +50,17 @@
     "scale": [1, 0.2],
     "tx": [0, 50],
     "ty": [0, 50],
     "angle": [0, 30],
 }
 
 
+class PaddingError(Exception):
+    pass
+
 def align_stack(
     data: np.ndarray,
     template16: np.ndarray,
     mask2: np.ndarray,
     plot: bool = False,
     path_to_save: str = None,
     binnings: Tuple = (2, 16, 2),
@@ -129,15 +133,15 @@
         )
         logger.info(f"Applying the transform to the fluorescence channel")
         aligned_bf = unpad(
             transform(bf[::stack_mask_scale, ::stack_mask_scale], tvec),
             mask2.shape,
         )
     except ValueError as e:
-        logger.debug("stack_mask_scale: ", stack_mask_scale)
+        print("stack_mask_scale: ", stack_mask_scale)
         logger.error(e.args)
         raise e
 
     if plot:
         plt.figure(dpi=300)
         plt.imshow(
             aligned_tritc,
@@ -162,25 +166,35 @@
 
 
 def get_transform(
     image,
     template,
     constraints,
     plot=False,
-    pad_ratio=1.2,
+    pad_ratio=1.5,
     figsize=(10, 5),
     dpi=300,
 ):
     """
     Pads image and template, registers and returns tvec
     """
-    padded_template = pad(template, (s := increase(image.shape, pad_ratio)))
+    print(f"padding to image.shape {image.shape} * pad_ratio {pad_ratio}")
+    s = increase(image.shape, pad_ratio)
+    print(f"new increased shape: {s}")
+
+    print(f"padding template: {template.shape}")
+    padded_template = pad(template, s)
+    print(f"padded template: {padded_template.shape}")
+
+    print(f"padding image: {image.shape}")
     padded_image = pad(image, s)
+    print(f"padded image: {padded_image.shape}")
+    
     tvec = register(padded_image, padded_template, constraints)
-    logger.debug(f"Found transform: {tvec}")
+    print(f"Found transform: {tvec}")
     if plot:
         aligned_bf = unpad(tvec["timg"], template.shape)
         plt.figure(figsize=figsize, dpi=dpi)
         plt.imshow(aligned_bf, cmap="gray")
     return tvec
 
 
@@ -196,16 +210,22 @@
     return reg.similarity(template, image, constraints=constraints)
 
 
 def pad(image: np.ndarray, to_shape: tuple = None, padding: tuple = None):
     """
     Pad the data to desired shape
     """
+    print(f"padding image {image.shape} to shape {to_shape}")
     if padding is None:
-        padding = calculate_padding(image.shape, to_shape)
+        try:
+            padding = calculate_padding(image.shape, to_shape)
+        except PaddingError as e:
+            new_to_shape = tuple(max(i,j) for i, j in zip(image.shape, to_shape))
+            logger.error(f"Error padding {e.args} try to_shape {new_to_shape}")
+
     try:
         padded = np.pad(image, padding, "edge")
     except TypeError as e:
         logger.error(f"padding {padding} failed: {e.args}")
         raise e
     return padded
 
@@ -235,22 +255,19 @@
 def calculate_padding(shape1: tuple, shape2: tuple):
     """
     Calculates padding to get shape2 from shape1
     Return:
     2D tuple of indices
     """
     dif = np.array(shape2) - np.array(shape1)
-    assert all(
-        dif >= 0
-    ), f"Shape2 must be bigger than shape1, got {shape2}, {shape1}"
+    if not all(dif >= 0): 
+        raise PaddingError(f"Shape2 {shape2} must be bigger than shape1 {shape1}")
     mid = dif // 2
     rest = dif - mid
-    y = mid[0], rest[0]
-    x = mid[1], rest[1]
-    return y, x
+    return (mid[0], rest[0]), (mid[1], rest[1])
 
 
 def scale_tvec(tvec, scale=8):
     """
     Scale up transform vector from imreg_dft
     """
     tvec_8x = tvec.copy()
@@ -263,15 +280,15 @@
         return tvec_8x
 
 
 def transform(image, tvec):
     """
     apply transform
     """
-    logger.debug(f"transform {image.shape}")
+    print(f"transform {image.shape}")
     fluo = reg.transform_img_dict(image, tvec)
     return fluo.astype("uint")
 
 
 def main(
     data_path: PathLike,
     template_path: PathLike,
```

### Comparing `anchor_droplet_chip-0.3.2/src/adc/fit.py` & `anchor_droplet_chip-0.4.0/src/adc/fit.py`

 * *Files identical despite different names*

### Comparing `anchor_droplet_chip-0.3.2/src/adc/io.py` & `anchor_droplet_chip-0.4.0/src/adc/io.py`

 * *Files identical despite different names*

### Comparing `anchor_droplet_chip-0.3.2/src/adc/merge.py` & `anchor_droplet_chip-0.4.0/src/adc/merge.py`

 * *Files identical despite different names*

### Comparing `anchor_droplet_chip-0.3.2/src/adc/napari.yaml` & `anchor_droplet_chip-0.4.0/src/adc/napari.yaml`

 * *Files identical despite different names*

### Comparing `anchor_droplet_chip-0.3.2/src/adc/plot.py` & `anchor_droplet_chip-0.4.0/src/adc/plot.py`

 * *Files identical despite different names*

### Comparing `anchor_droplet_chip-0.3.2/src/adc/tests/test_projection.py` & `anchor_droplet_chip-0.4.0/src/adc/tests/test_projection.py`

 * *Files identical despite different names*

### Comparing `anchor_droplet_chip-0.3.2/src/adc/tests/test_reader.py` & `anchor_droplet_chip-0.4.0/src/adc/tests/test_reader.py`

 * *Files identical despite different names*

### Comparing `anchor_droplet_chip-0.3.2/src/adc/tests/test_split.py` & `anchor_droplet_chip-0.4.0/src/adc/tests/test_split.py`

 * *Files identical despite different names*

### Comparing `anchor_droplet_chip-0.3.2/src/adc/tests/test_stack.py` & `anchor_droplet_chip-0.4.0/src/adc/tests/test_stack.py`

 * *Files identical despite different names*

### Comparing `anchor_droplet_chip-0.3.2/src/adc/tests/test_substack.py` & `anchor_droplet_chip-0.4.0/src/adc/tests/test_substack.py`

 * *Files identical despite different names*

### Comparing `anchor_droplet_chip-0.3.2/src/anchor_droplet_chip.egg-info/PKG-INFO` & `anchor_droplet_chip-0.4.0/src/anchor_droplet_chip.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: anchor-droplet-chip
-Version: 0.3.2
+Version: 0.4.0
 Summary: Segment organoids and measure intensities
 Home-page: https://github.com/BaroudLab/anchor-driplet-chip
 Author: Andrey Aristov
 Author-email: aaristov@pasteur.fr
 License: BSD-3-Clause
 Project-URL: Source Code, https://github.com/BaroudLab/anchor-droplet-chip
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `anchor_droplet_chip-0.3.2/src/anchor_droplet_chip.egg-info/SOURCES.txt` & `anchor_droplet_chip-0.4.0/src/anchor_droplet_chip.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 LICENSE
 README.md
 Snakefile
 example.ipynb
 find_all_big_nd2.ipynb
 logging.conf
 pyproject.toml
+recursion.ipynb
 runtime.txt
 setup.cfg
 setup.py
 test_data_0h.yaml
 test_data_24h.yaml
 tox.ini
 zenodo.ipynb
```

### Comparing `anchor_droplet_chip-0.3.2/src/imreg_dft/imreg.py` & `anchor_droplet_chip-0.4.0/src/imreg_dft/imreg.py`

 * *Files identical despite different names*

### Comparing `anchor_droplet_chip-0.3.2/src/imreg_dft/utils.py` & `anchor_droplet_chip-0.4.0/src/imreg_dft/utils.py`

 * *Files identical despite different names*

### Comparing `anchor_droplet_chip-0.3.2/test_data_0h.yaml` & `anchor_droplet_chip-0.4.0/test_data_0h.yaml`

 * *Files identical despite different names*

### Comparing `anchor_droplet_chip-0.3.2/test_data_24h.yaml` & `anchor_droplet_chip-0.4.0/test_data_24h.yaml`

 * *Files identical despite different names*

### Comparing `anchor_droplet_chip-0.3.2/tox.ini` & `anchor_droplet_chip-0.4.0/tox.ini`

 * *Files identical despite different names*

### Comparing `anchor_droplet_chip-0.3.2/zenodo.ipynb` & `anchor_droplet_chip-0.4.0/zenodo.ipynb`

 * *Files identical despite different names*

