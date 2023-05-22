# Comparing `tmp/pyrosetta_help-0.5.6.tar.gz` & `tmp/pyrosetta_help-0.5.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyrosetta_help-0.5.6.tar", last modified: Thu Sep  1 15:12:12 2022, max compression
+gzip compressed data, was "pyrosetta_help-0.5.7.tar", last modified: Mon May 22 16:38:46 2023, max compression
```

## Comparing `pyrosetta_help-0.5.6.tar` & `pyrosetta_help-0.5.7.tar`

### file list

```diff
@@ -1,79 +1,79 @@
-drwxr-xr-x   0 matteo     (501) staff       (20)        0 2022-09-01 15:12:12.303480 pyrosetta_help-0.5.6/
--rw-r--r--   0 matteo     (501) staff       (20)     1069 2022-04-07 09:44:36.000000 pyrosetta_help-0.5.6/LICENSE
--rw-r--r--   0 matteo     (501) staff       (20)       58 2022-05-28 19:10:31.000000 pyrosetta_help-0.5.6/MANIFEST.in
--rw-r--r--   0 matteo     (501) staff       (20)    15242 2022-09-01 15:12:12.301282 pyrosetta_help-0.5.6/PKG-INFO
--rw-r--r--   0 matteo     (501) staff       (20)    14465 2022-05-28 19:22:52.000000 pyrosetta_help-0.5.6/README.md
-drwxr-xr-x   0 matteo     (501) staff       (20)        0 2022-09-01 15:12:10.431152 pyrosetta_help-0.5.6/pyrosetta_help/
--rw-r--r--   0 matteo     (501) staff       (20)      935 2022-05-18 10:53:55.000000 pyrosetta_help-0.5.6/pyrosetta_help/__init__.py
-drwxr-xr-x   0 matteo     (501) staff       (20)        0 2022-09-01 15:12:10.648051 pyrosetta_help-0.5.6/pyrosetta_help/alphafold/
--rw-r--r--   0 matteo     (501) staff       (20)      184 2022-04-07 09:44:36.000000 pyrosetta_help-0.5.6/pyrosetta_help/alphafold/__init__.py
--rw-r--r--   0 matteo     (501) staff       (20)     6661 2022-05-28 19:22:52.000000 pyrosetta_help-0.5.6/pyrosetta_help/alphafold/constraints.py
--rw-r--r--   0 matteo     (501) staff       (20)    20196 2022-06-29 18:41:39.000000 pyrosetta_help-0.5.6/pyrosetta_help/alphafold/multimodel.py
--rw-r--r--   0 matteo     (501) staff       (20)      327 2022-05-28 20:00:36.000000 pyrosetta_help-0.5.6/pyrosetta_help/alphafold/plot.py
--rw-r--r--   0 matteo     (501) staff       (20)     2228 2022-05-28 20:00:36.000000 pyrosetta_help-0.5.6/pyrosetta_help/alphafold/retrieval.py
--rw-r--r--   0 matteo     (501) staff       (20)     1741 2022-04-07 09:44:36.000000 pyrosetta_help-0.5.6/pyrosetta_help/alphafold/superimpose.py
-drwxr-xr-x   0 matteo     (501) staff       (20)        0 2022-09-01 15:12:10.963792 pyrosetta_help-0.5.6/pyrosetta_help/blueprint_maker/
--rw-r--r--   0 matteo     (501) staff       (20)     2573 2022-04-07 09:44:36.000000 pyrosetta_help-0.5.6/pyrosetta_help/blueprint_maker/__init__.py
--rw-r--r--   0 matteo     (501) staff       (20)     2578 2022-05-28 20:00:36.000000 pyrosetta_help-0.5.6/pyrosetta_help/blueprint_maker/_common.py
--rw-r--r--   0 matteo     (501) staff       (20)     4593 2022-05-28 20:00:36.000000 pyrosetta_help-0.5.6/pyrosetta_help/blueprint_maker/_expected.py
--rw-r--r--   0 matteo     (501) staff       (20)      758 2022-04-07 09:44:36.000000 pyrosetta_help-0.5.6/pyrosetta_help/blueprint_maker/_init.py
--rw-r--r--   0 matteo     (501) staff       (20)     1726 2022-04-07 09:44:36.000000 pyrosetta_help-0.5.6/pyrosetta_help/blueprint_maker/_pdb_info.py
--rw-r--r--   0 matteo     (501) staff       (20)     1462 2022-04-07 09:44:36.000000 pyrosetta_help-0.5.6/pyrosetta_help/blueprint_maker/_remodel.py
--rw-r--r--   0 matteo     (501) staff       (20)     5007 2022-04-07 09:44:36.000000 pyrosetta_help-0.5.6/pyrosetta_help/blueprint_maker/_subscripted.py
-drwxr-xr-x   0 matteo     (501) staff       (20)        0 2022-09-01 15:12:11.084704 pyrosetta_help-0.5.6/pyrosetta_help/chain_ops/
--rw-r--r--   0 matteo     (501) staff       (20)      255 2022-04-14 15:21:38.000000 pyrosetta_help-0.5.6/pyrosetta_help/chain_ops/__init__.py
--rw-r--r--   0 matteo     (501) staff       (20)     1508 2022-04-07 09:44:36.000000 pyrosetta_help-0.5.6/pyrosetta_help/chain_ops/chain_ops.py
--rw-r--r--   0 matteo     (501) staff       (20)     2769 2022-04-07 09:44:36.000000 pyrosetta_help-0.5.6/pyrosetta_help/chain_ops/transmogrifier.py
--rw-r--r--   0 matteo     (501) staff       (20)     2923 2022-05-28 19:22:52.000000 pyrosetta_help-0.5.6/pyrosetta_help/colab_ops.py
-drwxr-xr-x   0 matteo     (501) staff       (20)        0 2022-09-01 15:12:11.399036 pyrosetta_help-0.5.6/pyrosetta_help/common_ops/
--rw-r--r--   0 matteo     (501) staff       (20)      246 2022-05-11 15:35:31.000000 pyrosetta_help-0.5.6/pyrosetta_help/common_ops/__init__.py
--rw-r--r--   0 matteo     (501) staff       (20)     6100 2022-04-07 09:44:36.000000 pyrosetta_help-0.5.6/pyrosetta_help/common_ops/constraints.py
--rw-r--r--   0 matteo     (501) staff       (20)     3078 2022-05-11 16:06:29.000000 pyrosetta_help-0.5.6/pyrosetta_help/common_ops/distances.py
--rw-r--r--   0 matteo     (501) staff       (20)     2872 2022-05-25 18:09:43.000000 pyrosetta_help-0.5.6/pyrosetta_help/common_ops/downloads.py
--rw-r--r--   0 matteo     (501) staff       (20)     3960 2022-04-14 15:04:34.000000 pyrosetta_help-0.5.6/pyrosetta_help/common_ops/faux_selectors.py
--rw-r--r--   0 matteo     (501) staff       (20)     3311 2022-04-07 09:44:36.000000 pyrosetta_help-0.5.6/pyrosetta_help/common_ops/minimize.py
--rw-r--r--   0 matteo     (501) staff       (20)     4344 2022-04-07 09:44:36.000000 pyrosetta_help-0.5.6/pyrosetta_help/common_ops/nglview.py
--rw-r--r--   0 matteo     (501) staff       (20)     1366 2022-04-07 09:44:36.000000 pyrosetta_help-0.5.6/pyrosetta_help/common_ops/ss_changes.py
--rw-r--r--   0 matteo     (501) staff       (20)    11249 2022-08-31 15:51:55.000000 pyrosetta_help-0.5.6/pyrosetta_help/common_ops/utils.py
--rw-r--r--   0 matteo     (501) staff       (20)     2542 2022-09-01 09:26:02.000000 pyrosetta_help-0.5.6/pyrosetta_help/database.py
-drwxr-xr-x   0 matteo     (501) staff       (20)        0 2022-09-01 15:12:11.522493 pyrosetta_help-0.5.6/pyrosetta_help/init_ops/
--rw-r--r--   0 matteo     (501) staff       (20)      132 2022-04-07 09:44:36.000000 pyrosetta_help-0.5.6/pyrosetta_help/init_ops/__init__.py
--rw-r--r--   0 matteo     (501) staff       (20)     2308 2022-04-07 09:44:36.000000 pyrosetta_help-0.5.6/pyrosetta_help/init_ops/log.py
--rw-r--r--   0 matteo     (501) staff       (20)     1480 2022-04-07 09:44:36.000000 pyrosetta_help-0.5.6/pyrosetta_help/init_ops/make_options.py
-drwxr-xr-x   0 matteo     (501) staff       (20)        0 2022-09-01 15:12:11.609347 pyrosetta_help-0.5.6/pyrosetta_help/installer/
--rw-r--r--   0 matteo     (501) staff       (20)     7301 2022-06-06 07:23:19.000000 pyrosetta_help-0.5.6/pyrosetta_help/installer/__init__.py
--rw-r--r--   0 matteo     (501) staff       (20)     3317 2022-04-07 16:01:55.000000 pyrosetta_help-0.5.6/pyrosetta_help/installer/_aux.py
-drwxr-xr-x   0 matteo     (501) staff       (20)        0 2022-09-01 15:12:11.774443 pyrosetta_help-0.5.6/pyrosetta_help/ligands/
--rw-r--r--   0 matteo     (501) staff       (20)      109 2022-04-07 09:44:36.000000 pyrosetta_help-0.5.6/pyrosetta_help/ligands/__init__.py
--rw-r--r--   0 matteo     (501) staff       (20)     4513 2022-05-16 09:52:25.000000 pyrosetta_help-0.5.6/pyrosetta_help/ligands/hunter.py
--rw-r--r--   0 matteo     (501) staff       (20)     6588 2022-04-08 10:19:20.000000 pyrosetta_help-0.5.6/pyrosetta_help/ligands/load.py
--rw-r--r--   0 matteo     (501) staff       (20)    16412 2022-04-08 10:19:20.000000 pyrosetta_help-0.5.6/pyrosetta_help/ligands/nick.py
-drwxr-xr-x   0 matteo     (501) staff       (20)        0 2022-09-01 15:12:11.776762 pyrosetta_help-0.5.6/pyrosetta_help/per_atom/
--rw-r--r--   0 matteo     (501) staff       (20)     9448 2022-06-17 15:55:58.000000 pyrosetta_help-0.5.6/pyrosetta_help/per_atom/__init__.py
-drwxr-xr-x   0 matteo     (501) staff       (20)        0 2022-09-01 15:12:11.998283 pyrosetta_help-0.5.6/pyrosetta_help/residue_decription/
--rw-r--r--   0 matteo     (501) staff       (20)      221 2022-04-07 09:44:36.000000 pyrosetta_help-0.5.6/pyrosetta_help/residue_decription/__init__.py
--rw-r--r--   0 matteo     (501) staff       (20)     1196 2022-04-07 09:44:36.000000 pyrosetta_help-0.5.6/pyrosetta_help/residue_decription/betaturn.py
--rw-r--r--   0 matteo     (501) staff       (20)      823 2022-04-07 09:44:36.000000 pyrosetta_help-0.5.6/pyrosetta_help/residue_decription/cis.py
--rw-r--r--   0 matteo     (501) staff       (20)     1944 2022-04-07 09:44:36.000000 pyrosetta_help-0.5.6/pyrosetta_help/residue_decription/hbonds.py
--rw-r--r--   0 matteo     (501) staff       (20)      274 2022-04-07 09:44:36.000000 pyrosetta_help-0.5.6/pyrosetta_help/residue_decription/ss.py
--rw-r--r--   0 matteo     (501) staff       (20)     1876 2022-04-07 09:44:36.000000 pyrosetta_help-0.5.6/pyrosetta_help/residue_decription/xlinks.py
-drwxr-xr-x   0 matteo     (501) staff       (20)        0 2022-09-01 15:12:12.175095 pyrosetta_help-0.5.6/pyrosetta_help/score_mutants/
--rw-r--r--   0 matteo     (501) staff       (20)      311 2022-04-07 09:44:36.000000 pyrosetta_help-0.5.6/pyrosetta_help/score_mutants/__init__.py
--rw-r--r--   0 matteo     (501) staff       (20)     2353 2022-04-07 09:44:36.000000 pyrosetta_help-0.5.6/pyrosetta_help/score_mutants/mutation.py
--rw-r--r--   0 matteo     (501) staff       (20)     2008 2022-04-07 09:44:36.000000 pyrosetta_help-0.5.6/pyrosetta_help/score_mutants/scores.py
--rw-r--r--   0 matteo     (501) staff       (20)    26110 2022-05-11 17:26:52.000000 pyrosetta_help-0.5.6/pyrosetta_help/score_mutants/variant.py
-drwxr-xr-x   0 matteo     (501) staff       (20)        0 2022-09-01 15:12:12.217884 pyrosetta_help-0.5.6/pyrosetta_help/threading/
--rw-r--r--   0 matteo     (501) staff       (20)     8748 2022-04-07 09:44:36.000000 pyrosetta_help-0.5.6/pyrosetta_help/threading/__init__.py
-drwxr-xr-x   0 matteo     (501) staff       (20)        0 2022-09-01 15:12:12.299417 pyrosetta_help-0.5.6/pyrosetta_help/weights/
--rw-r--r--   0 matteo     (501) staff       (20)     6625 2022-05-18 11:16:48.000000 pyrosetta_help-0.5.6/pyrosetta_help/weights/__init__.py
--rw-r--r--   0 matteo     (501) staff       (20)     3182 2022-04-07 09:44:36.000000 pyrosetta_help-0.5.6/pyrosetta_help/weights/terms.py
-drwxr-xr-x   0 matteo     (501) staff       (20)        0 2022-09-01 15:12:10.458441 pyrosetta_help-0.5.6/pyrosetta_help.egg-info/
--rw-r--r--   0 matteo     (501) staff       (20)    15242 2022-09-01 15:12:06.000000 pyrosetta_help-0.5.6/pyrosetta_help.egg-info/PKG-INFO
--rw-r--r--   0 matteo     (501) staff       (20)     2235 2022-09-01 15:12:07.000000 pyrosetta_help-0.5.6/pyrosetta_help.egg-info/SOURCES.txt
--rw-r--r--   0 matteo     (501) staff       (20)        1 2022-09-01 15:12:06.000000 pyrosetta_help-0.5.6/pyrosetta_help.egg-info/dependency_links.txt
--rw-r--r--   0 matteo     (501) staff       (20)       69 2022-09-01 15:12:06.000000 pyrosetta_help-0.5.6/pyrosetta_help.egg-info/entry_points.txt
--rw-r--r--   0 matteo     (501) staff       (20)       56 2022-09-01 15:12:06.000000 pyrosetta_help-0.5.6/pyrosetta_help.egg-info/requires.txt
--rw-r--r--   0 matteo     (501) staff       (20)       15 2022-09-01 15:12:06.000000 pyrosetta_help-0.5.6/pyrosetta_help.egg-info/top_level.txt
--rw-r--r--   0 matteo     (501) staff       (20)       55 2022-04-08 12:13:41.000000 pyrosetta_help-0.5.6/requirements.txt
--rw-r--r--   0 matteo     (501) staff       (20)       38 2022-09-01 15:12:12.303776 pyrosetta_help-0.5.6/setup.cfg
--rw-r--r--   0 matteo     (501) staff       (20)     1766 2022-08-31 15:53:03.000000 pyrosetta_help-0.5.6/setup.py
+drwxr-xr-x   0 user       (502) staff       (20)        0 2023-05-22 16:38:46.179714 pyrosetta_help-0.5.7/
+-rw-r--r--   0 user       (502) staff       (20)     1069 2023-05-22 16:32:36.000000 pyrosetta_help-0.5.7/LICENSE
+-rw-r--r--   0 user       (502) staff       (20)       58 2023-05-22 16:32:36.000000 pyrosetta_help-0.5.7/MANIFEST.in
+-rw-r--r--   0 user       (502) staff       (20)    15223 2023-05-22 16:38:46.177866 pyrosetta_help-0.5.7/PKG-INFO
+-rw-r--r--   0 user       (502) staff       (20)    14465 2023-05-22 16:32:36.000000 pyrosetta_help-0.5.7/README.md
+drwxr-xr-x   0 user       (502) staff       (20)        0 2023-05-22 16:38:45.998278 pyrosetta_help-0.5.7/pyrosetta_help/
+-rw-r--r--   0 user       (502) staff       (20)      935 2023-05-22 16:32:36.000000 pyrosetta_help-0.5.7/pyrosetta_help/__init__.py
+drwxr-xr-x   0 user       (502) staff       (20)        0 2023-05-22 16:38:46.057685 pyrosetta_help-0.5.7/pyrosetta_help/alphafold/
+-rw-r--r--   0 user       (502) staff       (20)      184 2023-05-22 16:32:36.000000 pyrosetta_help-0.5.7/pyrosetta_help/alphafold/__init__.py
+-rw-r--r--   0 user       (502) staff       (20)     6661 2023-05-22 16:32:36.000000 pyrosetta_help-0.5.7/pyrosetta_help/alphafold/constraints.py
+-rw-r--r--   0 user       (502) staff       (20)    20196 2023-05-22 16:32:36.000000 pyrosetta_help-0.5.7/pyrosetta_help/alphafold/multimodel.py
+-rw-r--r--   0 user       (502) staff       (20)      327 2023-05-22 16:32:36.000000 pyrosetta_help-0.5.7/pyrosetta_help/alphafold/plot.py
+-rw-r--r--   0 user       (502) staff       (20)     2228 2023-05-22 16:32:36.000000 pyrosetta_help-0.5.7/pyrosetta_help/alphafold/retrieval.py
+-rw-r--r--   0 user       (502) staff       (20)     1741 2023-05-22 16:32:36.000000 pyrosetta_help-0.5.7/pyrosetta_help/alphafold/superimpose.py
+drwxr-xr-x   0 user       (502) staff       (20)        0 2023-05-22 16:38:46.080853 pyrosetta_help-0.5.7/pyrosetta_help/blueprint_maker/
+-rw-r--r--   0 user       (502) staff       (20)     2573 2023-05-22 16:32:36.000000 pyrosetta_help-0.5.7/pyrosetta_help/blueprint_maker/__init__.py
+-rw-r--r--   0 user       (502) staff       (20)     2578 2023-05-22 16:32:36.000000 pyrosetta_help-0.5.7/pyrosetta_help/blueprint_maker/_common.py
+-rw-r--r--   0 user       (502) staff       (20)     4593 2023-05-22 16:32:36.000000 pyrosetta_help-0.5.7/pyrosetta_help/blueprint_maker/_expected.py
+-rw-r--r--   0 user       (502) staff       (20)      758 2023-05-22 16:32:36.000000 pyrosetta_help-0.5.7/pyrosetta_help/blueprint_maker/_init.py
+-rw-r--r--   0 user       (502) staff       (20)     1726 2023-05-22 16:32:36.000000 pyrosetta_help-0.5.7/pyrosetta_help/blueprint_maker/_pdb_info.py
+-rw-r--r--   0 user       (502) staff       (20)     1462 2023-05-22 16:32:36.000000 pyrosetta_help-0.5.7/pyrosetta_help/blueprint_maker/_remodel.py
+-rw-r--r--   0 user       (502) staff       (20)     5007 2023-05-22 16:32:36.000000 pyrosetta_help-0.5.7/pyrosetta_help/blueprint_maker/_subscripted.py
+drwxr-xr-x   0 user       (502) staff       (20)        0 2023-05-22 16:38:46.089874 pyrosetta_help-0.5.7/pyrosetta_help/chain_ops/
+-rw-r--r--   0 user       (502) staff       (20)      255 2023-05-22 16:32:36.000000 pyrosetta_help-0.5.7/pyrosetta_help/chain_ops/__init__.py
+-rw-r--r--   0 user       (502) staff       (20)     1508 2023-05-22 16:32:36.000000 pyrosetta_help-0.5.7/pyrosetta_help/chain_ops/chain_ops.py
+-rw-r--r--   0 user       (502) staff       (20)     2769 2023-05-22 16:32:36.000000 pyrosetta_help-0.5.7/pyrosetta_help/chain_ops/transmogrifier.py
+-rw-r--r--   0 user       (502) staff       (20)     2923 2023-05-22 16:32:36.000000 pyrosetta_help-0.5.7/pyrosetta_help/colab_ops.py
+drwxr-xr-x   0 user       (502) staff       (20)        0 2023-05-22 16:38:46.111979 pyrosetta_help-0.5.7/pyrosetta_help/common_ops/
+-rw-r--r--   0 user       (502) staff       (20)      319 2023-05-22 16:36:59.000000 pyrosetta_help-0.5.7/pyrosetta_help/common_ops/__init__.py
+-rw-r--r--   0 user       (502) staff       (20)     6100 2023-05-22 16:32:36.000000 pyrosetta_help-0.5.7/pyrosetta_help/common_ops/constraints.py
+-rw-r--r--   0 user       (502) staff       (20)     3078 2023-05-22 16:32:36.000000 pyrosetta_help-0.5.7/pyrosetta_help/common_ops/distances.py
+-rw-r--r--   0 user       (502) staff       (20)     2872 2023-05-22 16:32:36.000000 pyrosetta_help-0.5.7/pyrosetta_help/common_ops/downloads.py
+-rw-r--r--   0 user       (502) staff       (20)     3960 2023-05-22 16:32:36.000000 pyrosetta_help-0.5.7/pyrosetta_help/common_ops/faux_selectors.py
+-rw-r--r--   0 user       (502) staff       (20)     3311 2023-05-22 16:32:36.000000 pyrosetta_help-0.5.7/pyrosetta_help/common_ops/minimize.py
+-rw-r--r--   0 user       (502) staff       (20)     4344 2023-05-22 16:32:36.000000 pyrosetta_help-0.5.7/pyrosetta_help/common_ops/nglview.py
+-rw-r--r--   0 user       (502) staff       (20)     1366 2023-05-22 16:32:36.000000 pyrosetta_help-0.5.7/pyrosetta_help/common_ops/ss_changes.py
+-rw-r--r--   0 user       (502) staff       (20)    11240 2023-05-22 16:32:36.000000 pyrosetta_help-0.5.7/pyrosetta_help/common_ops/utils.py
+-rw-r--r--   0 user       (502) staff       (20)     2542 2023-05-22 16:32:36.000000 pyrosetta_help-0.5.7/pyrosetta_help/database.py
+drwxr-xr-x   0 user       (502) staff       (20)        0 2023-05-22 16:38:46.121667 pyrosetta_help-0.5.7/pyrosetta_help/init_ops/
+-rw-r--r--   0 user       (502) staff       (20)      132 2023-05-22 16:32:36.000000 pyrosetta_help-0.5.7/pyrosetta_help/init_ops/__init__.py
+-rw-r--r--   0 user       (502) staff       (20)     2308 2023-05-22 16:32:36.000000 pyrosetta_help-0.5.7/pyrosetta_help/init_ops/log.py
+-rw-r--r--   0 user       (502) staff       (20)     1480 2023-05-22 16:32:36.000000 pyrosetta_help-0.5.7/pyrosetta_help/init_ops/make_options.py
+drwxr-xr-x   0 user       (502) staff       (20)        0 2023-05-22 16:38:46.127794 pyrosetta_help-0.5.7/pyrosetta_help/installer/
+-rw-r--r--   0 user       (502) staff       (20)     8342 2023-05-22 16:32:36.000000 pyrosetta_help-0.5.7/pyrosetta_help/installer/__init__.py
+-rw-r--r--   0 user       (502) staff       (20)     3317 2023-05-22 16:32:36.000000 pyrosetta_help-0.5.7/pyrosetta_help/installer/_aux.py
+drwxr-xr-x   0 user       (502) staff       (20)        0 2023-05-22 16:38:46.141708 pyrosetta_help-0.5.7/pyrosetta_help/ligands/
+-rw-r--r--   0 user       (502) staff       (20)      109 2023-05-22 16:32:36.000000 pyrosetta_help-0.5.7/pyrosetta_help/ligands/__init__.py
+-rw-r--r--   0 user       (502) staff       (20)     4513 2023-05-22 16:32:36.000000 pyrosetta_help-0.5.7/pyrosetta_help/ligands/hunter.py
+-rw-r--r--   0 user       (502) staff       (20)     6588 2023-05-22 16:32:36.000000 pyrosetta_help-0.5.7/pyrosetta_help/ligands/load.py
+-rw-r--r--   0 user       (502) staff       (20)    16412 2023-05-22 16:32:36.000000 pyrosetta_help-0.5.7/pyrosetta_help/ligands/nick.py
+drwxr-xr-x   0 user       (502) staff       (20)        0 2023-05-22 16:38:46.144558 pyrosetta_help-0.5.7/pyrosetta_help/per_atom/
+-rw-r--r--   0 user       (502) staff       (20)     9448 2023-05-22 16:32:36.000000 pyrosetta_help-0.5.7/pyrosetta_help/per_atom/__init__.py
+drwxr-xr-x   0 user       (502) staff       (20)        0 2023-05-22 16:38:46.157696 pyrosetta_help-0.5.7/pyrosetta_help/residue_decription/
+-rw-r--r--   0 user       (502) staff       (20)      221 2023-05-22 16:32:36.000000 pyrosetta_help-0.5.7/pyrosetta_help/residue_decription/__init__.py
+-rw-r--r--   0 user       (502) staff       (20)     1196 2023-05-22 16:32:36.000000 pyrosetta_help-0.5.7/pyrosetta_help/residue_decription/betaturn.py
+-rw-r--r--   0 user       (502) staff       (20)      823 2023-05-22 16:32:36.000000 pyrosetta_help-0.5.7/pyrosetta_help/residue_decription/cis.py
+-rw-r--r--   0 user       (502) staff       (20)     1944 2023-05-22 16:32:36.000000 pyrosetta_help-0.5.7/pyrosetta_help/residue_decription/hbonds.py
+-rw-r--r--   0 user       (502) staff       (20)      274 2023-05-22 16:32:36.000000 pyrosetta_help-0.5.7/pyrosetta_help/residue_decription/ss.py
+-rw-r--r--   0 user       (502) staff       (20)     1876 2023-05-22 16:32:36.000000 pyrosetta_help-0.5.7/pyrosetta_help/residue_decription/xlinks.py
+drwxr-xr-x   0 user       (502) staff       (20)        0 2023-05-22 16:38:46.169609 pyrosetta_help-0.5.7/pyrosetta_help/score_mutants/
+-rw-r--r--   0 user       (502) staff       (20)      311 2023-05-22 16:32:36.000000 pyrosetta_help-0.5.7/pyrosetta_help/score_mutants/__init__.py
+-rw-r--r--   0 user       (502) staff       (20)     2353 2023-05-22 16:32:36.000000 pyrosetta_help-0.5.7/pyrosetta_help/score_mutants/mutation.py
+-rw-r--r--   0 user       (502) staff       (20)     2008 2023-05-22 16:32:36.000000 pyrosetta_help-0.5.7/pyrosetta_help/score_mutants/scores.py
+-rw-r--r--   0 user       (502) staff       (20)    26110 2023-05-22 16:32:36.000000 pyrosetta_help-0.5.7/pyrosetta_help/score_mutants/variant.py
+drwxr-xr-x   0 user       (502) staff       (20)        0 2023-05-22 16:38:46.171574 pyrosetta_help-0.5.7/pyrosetta_help/threading/
+-rw-r--r--   0 user       (502) staff       (20)     8748 2023-05-22 16:32:36.000000 pyrosetta_help-0.5.7/pyrosetta_help/threading/__init__.py
+drwxr-xr-x   0 user       (502) staff       (20)        0 2023-05-22 16:38:46.175714 pyrosetta_help-0.5.7/pyrosetta_help/weights/
+-rw-r--r--   0 user       (502) staff       (20)     6625 2023-05-22 16:32:36.000000 pyrosetta_help-0.5.7/pyrosetta_help/weights/__init__.py
+-rw-r--r--   0 user       (502) staff       (20)     3182 2023-05-22 16:32:36.000000 pyrosetta_help-0.5.7/pyrosetta_help/weights/terms.py
+drwxr-xr-x   0 user       (502) staff       (20)        0 2023-05-22 16:38:46.036384 pyrosetta_help-0.5.7/pyrosetta_help.egg-info/
+-rw-r--r--   0 user       (502) staff       (20)    15223 2023-05-22 16:38:45.000000 pyrosetta_help-0.5.7/pyrosetta_help.egg-info/PKG-INFO
+-rw-r--r--   0 user       (502) staff       (20)     2235 2023-05-22 16:38:45.000000 pyrosetta_help-0.5.7/pyrosetta_help.egg-info/SOURCES.txt
+-rw-r--r--   0 user       (502) staff       (20)        1 2023-05-22 16:38:45.000000 pyrosetta_help-0.5.7/pyrosetta_help.egg-info/dependency_links.txt
+-rw-r--r--   0 user       (502) staff       (20)       69 2023-05-22 16:38:45.000000 pyrosetta_help-0.5.7/pyrosetta_help.egg-info/entry_points.txt
+-rw-r--r--   0 user       (502) staff       (20)       56 2023-05-22 16:38:45.000000 pyrosetta_help-0.5.7/pyrosetta_help.egg-info/requires.txt
+-rw-r--r--   0 user       (502) staff       (20)       15 2023-05-22 16:38:45.000000 pyrosetta_help-0.5.7/pyrosetta_help.egg-info/top_level.txt
+-rw-r--r--   0 user       (502) staff       (20)       55 2023-05-22 16:32:36.000000 pyrosetta_help-0.5.7/requirements.txt
+-rw-r--r--   0 user       (502) staff       (20)       38 2023-05-22 16:38:46.180010 pyrosetta_help-0.5.7/setup.cfg
+-rw-r--r--   0 user       (502) staff       (20)     1766 2023-05-22 16:36:59.000000 pyrosetta_help-0.5.7/setup.py
```

### Comparing `pyrosetta_help-0.5.6/LICENSE` & `pyrosetta_help-0.5.7/LICENSE`

 * *Files identical despite different names*

### Comparing `pyrosetta_help-0.5.6/PKG-INFO` & `pyrosetta_help-0.5.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: pyrosetta_help
-Version: 0.5.6
+Version: 0.5.7
 Summary: A variety of functions to make working with Pyrosetta easier.
 Home-page: https://github.com/matteoferla/pyrosetta_help
 Author: Matteo Ferla
 Author-email: matteo.ferla@gmail.com
 License: MIT
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Classifier: Topic :: Scientific/Engineering :: Chemistry
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
@@ -330,8 +329,7 @@
 [![Matteo Ferla orcid](https://img.shields.io/badge/orcid-0000--0002--5508--4673-a6ce39?logo=orcid)](https://orcid.org/0000--0002--5508--4673)
 [![Matteo Ferla googlescholar](https://img.shields.io/badge/google--scholar-gF--bp_cAAAAJ-success?logo=googlescholar)](https://scholar.google.com/citations?user=gF--bp_cAAAAJ&hl=en)
 [![Matteo Ferla twitter](https://img.shields.io/twitter/follow/matteoferla?label=Follow&logo=twitter)](https://twitter.com/matteoferla) 
 [![Matteo Ferla stackoverflow](https://img.shields.io/stackexchange/stackoverflow/r/4625475?logo=stackoverflow)](https://stackoverflow.com/users/4625475)
 [![Matteo Ferla stackexchange](https://img.shields.io/stackexchange/bioinformatics/r/6322?logo=stackexchange)](https://bioinformatics.stackexchange.com/users/6322) 
 [![Matteo Ferla googlemail](https://img.shields.io/badge/email-gmail-informational&logo=googlemail)](https://mailhide.io/e/Ey3RNO2G) 
 [![Matteo Ferla Oxford](https://img.shields.io/badge/email-Oxford-informational&logo=googlemail)](https://mailhide.io/e/Y1dbgyyE)
-
```

### Comparing `pyrosetta_help-0.5.6/README.md` & `pyrosetta_help-0.5.7/README.md`

 * *Files identical despite different names*

### Comparing `pyrosetta_help-0.5.6/pyrosetta_help/__init__.py` & `pyrosetta_help-0.5.7/pyrosetta_help/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrosetta_help-0.5.6/pyrosetta_help/alphafold/constraints.py` & `pyrosetta_help-0.5.7/pyrosetta_help/alphafold/constraints.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -131,20 +131,20 @@
     :param residue_index_A: first residue?
     :param residue_index_B: last residue is "-1"
     :param distance: if omitted, the midpoint of Sigmoid will be the current distance
     :param sigmoid: use sigmoid or identity/linear (bad idea)
     :return:
     """
     # get current length
+    if residue_index_B == -1:
+        residue_index_B = pose.total_residue()
     assert pose.residue(residue_index_A).is_protein, f'residue idx {residue_index_A} is not an AA'
     assert pose.residue(residue_index_B).is_protein, f'residue idx {residue_index_B} is not an AA'
     first_ca = pyrosetta.AtomID(atomno_in=pose.residue(residue_index_A).atom_index('CA'),
                                 rsd_in=residue_index_A)
-    if residue_index_B == -1:
-        residue_index_B = pose.total_residue()
     last_ca = pyrosetta.AtomID(atomno_in=pose.residue(residue_index_B).atom_index('CA'),
                                rsd_in=residue_index_B)
     first_ca_xyz = pose.residue(residue_index_A).xyz(first_ca.atomno())
     last_ca_xyz = pose.residue(residue_index_B).xyz(last_ca.atomno())
     if distance is None:
         distance = (first_ca_xyz - last_ca_xyz).norm()
     # make & add con
```

### Comparing `pyrosetta_help-0.5.6/pyrosetta_help/alphafold/multimodel.py` & `pyrosetta_help-0.5.7/pyrosetta_help/alphafold/multimodel.py`

 * *Files identical despite different names*

### Comparing `pyrosetta_help-0.5.6/pyrosetta_help/alphafold/retrieval.py` & `pyrosetta_help-0.5.7/pyrosetta_help/alphafold/retrieval.py`

 * *Files identical despite different names*

### Comparing `pyrosetta_help-0.5.6/pyrosetta_help/alphafold/superimpose.py` & `pyrosetta_help-0.5.7/pyrosetta_help/alphafold/superimpose.py`

 * *Files identical despite different names*

### Comparing `pyrosetta_help-0.5.6/pyrosetta_help/blueprint_maker/__init__.py` & `pyrosetta_help-0.5.7/pyrosetta_help/blueprint_maker/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrosetta_help-0.5.6/pyrosetta_help/blueprint_maker/_common.py` & `pyrosetta_help-0.5.7/pyrosetta_help/blueprint_maker/_common.py`

 * *Files identical despite different names*

### Comparing `pyrosetta_help-0.5.6/pyrosetta_help/blueprint_maker/_expected.py` & `pyrosetta_help-0.5.7/pyrosetta_help/blueprint_maker/_expected.py`

 * *Files identical despite different names*

### Comparing `pyrosetta_help-0.5.6/pyrosetta_help/blueprint_maker/_init.py` & `pyrosetta_help-0.5.7/pyrosetta_help/blueprint_maker/_init.py`

 * *Files identical despite different names*

### Comparing `pyrosetta_help-0.5.6/pyrosetta_help/blueprint_maker/_pdb_info.py` & `pyrosetta_help-0.5.7/pyrosetta_help/blueprint_maker/_pdb_info.py`

 * *Files identical despite different names*

### Comparing `pyrosetta_help-0.5.6/pyrosetta_help/blueprint_maker/_remodel.py` & `pyrosetta_help-0.5.7/pyrosetta_help/blueprint_maker/_remodel.py`

 * *Files identical despite different names*

### Comparing `pyrosetta_help-0.5.6/pyrosetta_help/blueprint_maker/_subscripted.py` & `pyrosetta_help-0.5.7/pyrosetta_help/blueprint_maker/_subscripted.py`

 * *Files identical despite different names*

### Comparing `pyrosetta_help-0.5.6/pyrosetta_help/chain_ops/chain_ops.py` & `pyrosetta_help-0.5.7/pyrosetta_help/chain_ops/chain_ops.py`

 * *Files identical despite different names*

### Comparing `pyrosetta_help-0.5.6/pyrosetta_help/chain_ops/transmogrifier.py` & `pyrosetta_help-0.5.7/pyrosetta_help/chain_ops/transmogrifier.py`

 * *Files identical despite different names*

### Comparing `pyrosetta_help-0.5.6/pyrosetta_help/colab_ops.py` & `pyrosetta_help-0.5.7/pyrosetta_help/colab_ops.py`

 * *Files identical despite different names*

### Comparing `pyrosetta_help-0.5.6/pyrosetta_help/common_ops/constraints.py` & `pyrosetta_help-0.5.7/pyrosetta_help/common_ops/constraints.py`

 * *Files identical despite different names*

### Comparing `pyrosetta_help-0.5.6/pyrosetta_help/common_ops/distances.py` & `pyrosetta_help-0.5.7/pyrosetta_help/common_ops/distances.py`

 * *Files identical despite different names*

### Comparing `pyrosetta_help-0.5.6/pyrosetta_help/common_ops/downloads.py` & `pyrosetta_help-0.5.7/pyrosetta_help/common_ops/downloads.py`

 * *Files identical despite different names*

### Comparing `pyrosetta_help-0.5.6/pyrosetta_help/common_ops/faux_selectors.py` & `pyrosetta_help-0.5.7/pyrosetta_help/common_ops/faux_selectors.py`

 * *Files identical despite different names*

### Comparing `pyrosetta_help-0.5.6/pyrosetta_help/common_ops/minimize.py` & `pyrosetta_help-0.5.7/pyrosetta_help/common_ops/minimize.py`

 * *Files identical despite different names*

### Comparing `pyrosetta_help-0.5.6/pyrosetta_help/common_ops/nglview.py` & `pyrosetta_help-0.5.7/pyrosetta_help/common_ops/nglview.py`

 * *Files identical despite different names*

### Comparing `pyrosetta_help-0.5.6/pyrosetta_help/common_ops/ss_changes.py` & `pyrosetta_help-0.5.7/pyrosetta_help/common_ops/ss_changes.py`

 * *Files identical despite different names*

### Comparing `pyrosetta_help-0.5.6/pyrosetta_help/common_ops/utils.py` & `pyrosetta_help-0.5.7/pyrosetta_help/common_ops/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
            'get_pdbstr',
            'pose_range',
            'fix_offset',
            'assign_chain_letter',
            'what_is_chain']
 
 from collections import Counter
-from typing import (Optional, Tuple, Union, Iterable, Counter, List)
+from typing import (Optional, Tuple, Union, Iterable, List)
 from Bio import pairwise2
 from IPython.display import display, HTML
 import string
 import numpy as np
 import pandas as pd
 import pyrosetta
 import functools
```

### Comparing `pyrosetta_help-0.5.6/pyrosetta_help/database.py` & `pyrosetta_help-0.5.7/pyrosetta_help/database.py`

 * *Files identical despite different names*

### Comparing `pyrosetta_help-0.5.6/pyrosetta_help/init_ops/log.py` & `pyrosetta_help-0.5.7/pyrosetta_help/init_ops/log.py`

 * *Files identical despite different names*

### Comparing `pyrosetta_help-0.5.6/pyrosetta_help/init_ops/make_options.py` & `pyrosetta_help-0.5.7/pyrosetta_help/init_ops/make_options.py`

 * *Files identical despite different names*

### Comparing `pyrosetta_help-0.5.6/pyrosetta_help/installer/__init__.py` & `pyrosetta_help-0.5.7/pyrosetta_help/installer/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 __doc__ = """
 This module is aimed at helping to install pyrosetta.
 If PyRosetta is installed but if it segfaults on import due to wrong GNU lib C (``glic``)
 or there's a missing dependency that is a different matter.
 """
 
 import argparse
+import subprocess
 import importlib
 import importlib.util
 import os
 import re
 import requests
 import site
 import sys
@@ -52,15 +53,18 @@
         os.rmdir(existing_path)
     else: # error or raise
         raise FileExistsError(f'There seems to be a release already downloaded ({existing_path})')
     # get url and download:
     latest_url = get_latest_release_url(username, password,
                                         wheel=True,
                                         hash_comparison_required=hash_comparison_required)
-    assert not os.system(f'curl {latest_url} | tar -xj -C {path}')
+    process: subprocess.CompletedProcess = subprocess.run(f'curl {latest_url} | tar -xj -C {path}'.split(),
+                                                          capture_output=True)
+    assert not process.returncode, f'PyRosetta download failed (via {latest_url}, error: {process.stderr.decode()}. ' +\
+                                   'Please check your internet connection and try again.'
     pyrosetta_folder = re.sub(r'.tar.\w+$', '', os.path.split(latest_url)[1])
     return os.path.join(path, pyrosetta_folder)
 
 
 def install_pyrosetta(username: Optional[str] = None,
                       password: Optional[str] = None,
                       path: str = '.',
@@ -73,23 +77,31 @@
     It checks to see if hashes of the password is correct or the Rosetta one.
     """
     if check_pyrosetta():
         print('PyRosetta is already installed.')
     # ## local version present?
     path = get_release_path(path)
     if path:
-        assert not os.system(f'yes | pip3 install -e {path}/setup/')
+        process: subprocess.CompletedProcess = subprocess.run(f'yes | pip3 install -e {path}/setup/'.split(),
+                                                                capture_output=True)
+        assert not process.returncode, f'PyRosetta installation failed ({path}, error: {process.stderr.decode()}.'
+        print('PyRosetta installed.')
         site.main()  # refresh
         return
     # ## install by download
     # get latest release
     latest_url = get_latest_release_url(username, password,
                                         wheel=True,
                                         hash_comparison_required=hash_comparison_required)
-    assert not os.system(f'yes | pip3 install {latest_url}')
+    process: subprocess.CompletedProcess = subprocess.run(f'yes | pip3 install {latest_url}'.split(),
+                                                            capture_output=True)
+    assert not process.returncode, f'PyRosetta installation failed (via {latest_url}, ' +\
+                                   f'error: {process.stderr.decode()}. ' +\
+                                   'Please check your internet connection and try again.'
+    print('PyRosetta installed.')
     site.main()  # refresh
     return
 
 
 def parse():
     """
     Parse command line arguments ``-h`` for help.
```

### Comparing `pyrosetta_help-0.5.6/pyrosetta_help/installer/_aux.py` & `pyrosetta_help-0.5.7/pyrosetta_help/installer/_aux.py`

 * *Files identical despite different names*

### Comparing `pyrosetta_help-0.5.6/pyrosetta_help/ligands/hunter.py` & `pyrosetta_help-0.5.7/pyrosetta_help/ligands/hunter.py`

 * *Files identical despite different names*

### Comparing `pyrosetta_help-0.5.6/pyrosetta_help/ligands/load.py` & `pyrosetta_help-0.5.7/pyrosetta_help/ligands/load.py`

 * *Files identical despite different names*

### Comparing `pyrosetta_help-0.5.6/pyrosetta_help/ligands/nick.py` & `pyrosetta_help-0.5.7/pyrosetta_help/ligands/nick.py`

 * *Files identical despite different names*

### Comparing `pyrosetta_help-0.5.6/pyrosetta_help/per_atom/__init__.py` & `pyrosetta_help-0.5.7/pyrosetta_help/per_atom/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrosetta_help-0.5.6/pyrosetta_help/residue_decription/betaturn.py` & `pyrosetta_help-0.5.7/pyrosetta_help/residue_decription/betaturn.py`

 * *Files identical despite different names*

### Comparing `pyrosetta_help-0.5.6/pyrosetta_help/residue_decription/cis.py` & `pyrosetta_help-0.5.7/pyrosetta_help/residue_decription/cis.py`

 * *Files identical despite different names*

### Comparing `pyrosetta_help-0.5.6/pyrosetta_help/residue_decription/hbonds.py` & `pyrosetta_help-0.5.7/pyrosetta_help/residue_decription/hbonds.py`

 * *Files identical despite different names*

### Comparing `pyrosetta_help-0.5.6/pyrosetta_help/residue_decription/xlinks.py` & `pyrosetta_help-0.5.7/pyrosetta_help/residue_decription/xlinks.py`

 * *Files identical despite different names*

### Comparing `pyrosetta_help-0.5.6/pyrosetta_help/score_mutants/mutation.py` & `pyrosetta_help-0.5.7/pyrosetta_help/score_mutants/mutation.py`

 * *Files identical despite different names*

### Comparing `pyrosetta_help-0.5.6/pyrosetta_help/score_mutants/scores.py` & `pyrosetta_help-0.5.7/pyrosetta_help/score_mutants/scores.py`

 * *Files identical despite different names*

### Comparing `pyrosetta_help-0.5.6/pyrosetta_help/score_mutants/variant.py` & `pyrosetta_help-0.5.7/pyrosetta_help/score_mutants/variant.py`

 * *Files identical despite different names*

### Comparing `pyrosetta_help-0.5.6/pyrosetta_help/threading/__init__.py` & `pyrosetta_help-0.5.7/pyrosetta_help/threading/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrosetta_help-0.5.6/pyrosetta_help/weights/__init__.py` & `pyrosetta_help-0.5.7/pyrosetta_help/weights/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrosetta_help-0.5.6/pyrosetta_help/weights/terms.py` & `pyrosetta_help-0.5.7/pyrosetta_help/weights/terms.py`

 * *Files identical despite different names*

### Comparing `pyrosetta_help-0.5.6/pyrosetta_help.egg-info/PKG-INFO` & `pyrosetta_help-0.5.7/pyrosetta_help.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: pyrosetta-help
-Version: 0.5.6
+Version: 0.5.7
 Summary: A variety of functions to make working with Pyrosetta easier.
 Home-page: https://github.com/matteoferla/pyrosetta_help
 Author: Matteo Ferla
 Author-email: matteo.ferla@gmail.com
 License: MIT
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Classifier: Topic :: Scientific/Engineering :: Chemistry
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
@@ -330,8 +329,7 @@
 [![Matteo Ferla orcid](https://img.shields.io/badge/orcid-0000--0002--5508--4673-a6ce39?logo=orcid)](https://orcid.org/0000--0002--5508--4673)
 [![Matteo Ferla googlescholar](https://img.shields.io/badge/google--scholar-gF--bp_cAAAAJ-success?logo=googlescholar)](https://scholar.google.com/citations?user=gF--bp_cAAAAJ&hl=en)
 [![Matteo Ferla twitter](https://img.shields.io/twitter/follow/matteoferla?label=Follow&logo=twitter)](https://twitter.com/matteoferla) 
 [![Matteo Ferla stackoverflow](https://img.shields.io/stackexchange/stackoverflow/r/4625475?logo=stackoverflow)](https://stackoverflow.com/users/4625475)
 [![Matteo Ferla stackexchange](https://img.shields.io/stackexchange/bioinformatics/r/6322?logo=stackexchange)](https://bioinformatics.stackexchange.com/users/6322) 
 [![Matteo Ferla googlemail](https://img.shields.io/badge/email-gmail-informational&logo=googlemail)](https://mailhide.io/e/Ey3RNO2G) 
 [![Matteo Ferla Oxford](https://img.shields.io/badge/email-Oxford-informational&logo=googlemail)](https://mailhide.io/e/Y1dbgyyE)
-
```

### Comparing `pyrosetta_help-0.5.6/pyrosetta_help.egg-info/SOURCES.txt` & `pyrosetta_help-0.5.7/pyrosetta_help.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyrosetta_help-0.5.6/setup.py` & `pyrosetta_help-0.5.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
     requirements = ['rdkit-to-params', 'xerox', 'requests', 'pandas', 'biopython']
     __doc__ = ''
 
 description = 'A variety of functions to make working with Pyrosetta easier.'
 
 setup(
     name='pyrosetta_help',
-    version='0.5.6',
+    version='0.5.7',
     python_requires='>=3.7',
     packages=find_packages(),
     install_requires=requirements,
     url='https://github.com/matteoferla/pyrosetta_help',
     license='MIT',
     author='Matteo Ferla',
     author_email='matteo.ferla@gmail.com',
```

