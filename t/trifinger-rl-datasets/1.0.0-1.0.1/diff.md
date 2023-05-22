# Comparing `tmp/trifinger_rl_datasets-1.0.0.tar.gz` & `tmp/trifinger_rl_datasets-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trifinger_rl_datasets-1.0.0.tar", last modified: Thu Apr 27 13:48:26 2023, max compression
+gzip compressed data, was "trifinger_rl_datasets-1.0.1.tar", last modified: Mon May 22 13:29:36 2023, max compression
```

## Comparing `trifinger_rl_datasets-1.0.0.tar` & `trifinger_rl_datasets-1.0.1.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxr-xr-x   0 nguertler  (7419) is        (1040)        0 2023-04-27 13:48:26.442073 trifinger_rl_datasets-1.0.0/
--rw-rw-r--   0 nguertler  (7419) is        (1040)     1532 2022-09-07 07:59:18.000000 trifinger_rl_datasets-1.0.0/LICENSE
--rw-r--r--   0 nguertler  (7419) is        (1040)     6702 2023-04-27 13:48:26.443076 trifinger_rl_datasets-1.0.0/PKG-INFO
--rw-r--r--   0 nguertler  (7419) is        (1040)     5307 2023-04-27 13:43:01.000000 trifinger_rl_datasets-1.0.0/README.md
--rw-rw-r--   0 nguertler  (7419) is        (1040)      142 2022-09-07 07:59:18.000000 trifinger_rl_datasets-1.0.0/pyproject.toml
--rw-r--r--   0 nguertler  (7419) is        (1040)      784 2023-04-27 13:48:26.446081 trifinger_rl_datasets-1.0.0/setup.cfg
--rw-r--r--   0 nguertler  (7419) is        (1040)       38 2023-03-23 14:08:48.000000 trifinger_rl_datasets-1.0.0/setup.py
-drwxr-xr-x   0 nguertler  (7419) is        (1040)        0 2023-04-27 13:48:26.297082 trifinger_rl_datasets-1.0.0/trifinger_rl_datasets/
--rw-r--r--   0 nguertler  (7419) is        (1040)     3236 2023-04-27 13:47:58.000000 trifinger_rl_datasets-1.0.0/trifinger_rl_datasets/__init__.py
-drwxr-xr-x   0 nguertler  (7419) is        (1040)        0 2023-04-27 13:48:26.416080 trifinger_rl_datasets-1.0.0/trifinger_rl_datasets/data/
--rw-r--r--   0 nguertler  (7419) is        (1040)        0 2023-01-20 15:23:15.000000 trifinger_rl_datasets-1.0.0/trifinger_rl_datasets/data/__init__.py
--rw-r--r--   0 nguertler  (7419) is        (1040)     1170 2023-02-20 18:18:55.000000 trifinger_rl_datasets-1.0.0/trifinger_rl_datasets/data/r1_camera180.yml
--rw-r--r--   0 nguertler  (7419) is        (1040)     1176 2023-02-20 18:18:55.000000 trifinger_rl_datasets-1.0.0/trifinger_rl_datasets/data/r1_camera300.yml
--rw-r--r--   0 nguertler  (7419) is        (1040)     1177 2023-02-20 18:18:55.000000 trifinger_rl_datasets-1.0.0/trifinger_rl_datasets/data/r1_camera60.yml
--rw-r--r--   0 nguertler  (7419) is        (1040)     1180 2023-02-20 18:18:55.000000 trifinger_rl_datasets-1.0.0/trifinger_rl_datasets/data/r3_camera180.yml
--rw-r--r--   0 nguertler  (7419) is        (1040)     1172 2023-02-20 18:18:55.000000 trifinger_rl_datasets-1.0.0/trifinger_rl_datasets/data/r3_camera300.yml
--rw-r--r--   0 nguertler  (7419) is        (1040)     1175 2023-02-20 18:18:55.000000 trifinger_rl_datasets-1.0.0/trifinger_rl_datasets/data/r3_camera60.yml
--rw-r--r--   0 nguertler  (7419) is        (1040)     1178 2023-02-20 18:18:55.000000 trifinger_rl_datasets-1.0.0/trifinger_rl_datasets/data/r4_camera180.yml
--rw-r--r--   0 nguertler  (7419) is        (1040)     1178 2023-02-20 18:18:55.000000 trifinger_rl_datasets-1.0.0/trifinger_rl_datasets/data/r4_camera300.yml
--rw-r--r--   0 nguertler  (7419) is        (1040)     1169 2023-02-20 18:18:55.000000 trifinger_rl_datasets-1.0.0/trifinger_rl_datasets/data/r4_camera60.yml
--rw-r--r--   0 nguertler  (7419) is        (1040)     1188 2023-02-20 18:18:55.000000 trifinger_rl_datasets-1.0.0/trifinger_rl_datasets/data/r5_camera180.yml
--rw-r--r--   0 nguertler  (7419) is        (1040)     1177 2023-02-20 18:18:55.000000 trifinger_rl_datasets-1.0.0/trifinger_rl_datasets/data/r5_camera300.yml
--rw-r--r--   0 nguertler  (7419) is        (1040)     1175 2023-02-20 18:18:55.000000 trifinger_rl_datasets-1.0.0/trifinger_rl_datasets/data/r5_camera60.yml
--rw-r--r--   0 nguertler  (7419) is        (1040)     1184 2023-02-20 18:18:55.000000 trifinger_rl_datasets-1.0.0/trifinger_rl_datasets/data/r6_camera180.yml
--rw-r--r--   0 nguertler  (7419) is        (1040)     1173 2023-02-20 18:18:55.000000 trifinger_rl_datasets-1.0.0/trifinger_rl_datasets/data/r6_camera300.yml
--rw-r--r--   0 nguertler  (7419) is        (1040)     1167 2023-02-20 18:18:55.000000 trifinger_rl_datasets-1.0.0/trifinger_rl_datasets/data/r6_camera60.yml
--rw-r--r--   0 nguertler  (7419) is        (1040)     1180 2023-02-20 18:18:56.000000 trifinger_rl_datasets-1.0.0/trifinger_rl_datasets/data/r7_camera180.yml
--rw-r--r--   0 nguertler  (7419) is        (1040)     1175 2023-02-20 18:18:56.000000 trifinger_rl_datasets-1.0.0/trifinger_rl_datasets/data/r7_camera300.yml
--rw-r--r--   0 nguertler  (7419) is        (1040)     1174 2023-02-20 18:18:56.000000 trifinger_rl_datasets-1.0.0/trifinger_rl_datasets/data/r7_camera60.yml
--rw-r--r--   0 nguertler  (7419) is        (1040)     1180 2023-02-20 18:18:56.000000 trifinger_rl_datasets-1.0.0/trifinger_rl_datasets/data/r8_camera180.yml
--rw-r--r--   0 nguertler  (7419) is        (1040)     1176 2023-02-20 18:18:56.000000 trifinger_rl_datasets-1.0.0/trifinger_rl_datasets/data/r8_camera300.yml
--rw-r--r--   0 nguertler  (7419) is        (1040)     1171 2023-02-20 18:18:56.000000 trifinger_rl_datasets-1.0.0/trifinger_rl_datasets/data/r8_camera60.yml
--rw-r--r--   0 nguertler  (7419) is        (1040)  1556408 2023-01-20 15:23:15.000000 trifinger_rl_datasets-1.0.0/trifinger_rl_datasets/data/trifingerpro_shuffle_cube_trajectory_fast.npy
--rw-r--r--   0 nguertler  (7419) is        (1040)    39661 2023-04-27 11:37:43.000000 trifinger_rl_datasets-1.0.0/trifinger_rl_datasets/dataset_env.py
--rw-r--r--   0 nguertler  (7419) is        (1040)     3104 2023-03-23 14:08:48.000000 trifinger_rl_datasets-1.0.0/trifinger_rl_datasets/evaluate_sim.py
--rw-r--r--   0 nguertler  (7419) is        (1040)     3139 2023-03-23 14:08:48.000000 trifinger_rl_datasets-1.0.0/trifinger_rl_datasets/evaluation.py
--rw-r--r--   0 nguertler  (7419) is        (1040)     2067 2023-03-23 14:08:48.000000 trifinger_rl_datasets-1.0.0/trifinger_rl_datasets/policy_base.py
--rw-r--r--   0 nguertler  (7419) is        (1040)        0 2023-01-20 15:23:15.000000 trifinger_rl_datasets-1.0.0/trifinger_rl_datasets/py.typed
--rw-r--r--   0 nguertler  (7419) is        (1040)     1673 2023-01-20 15:23:15.000000 trifinger_rl_datasets-1.0.0/trifinger_rl_datasets/sampling_utils.py
--rw-r--r--   0 nguertler  (7419) is        (1040)    27363 2023-04-26 16:31:32.000000 trifinger_rl_datasets-1.0.0/trifinger_rl_datasets/sim_env.py
--rw-r--r--   0 nguertler  (7419) is        (1040)     2743 2023-01-20 15:23:15.000000 trifinger_rl_datasets-1.0.0/trifinger_rl_datasets/utils.py
-drwxr-xr-x   0 nguertler  (7419) is        (1040)        0 2023-04-27 13:48:26.314081 trifinger_rl_datasets-1.0.0/trifinger_rl_datasets.egg-info/
--rw-r--r--   0 nguertler  (7419) is        (1040)     6702 2023-04-27 13:48:26.000000 trifinger_rl_datasets-1.0.0/trifinger_rl_datasets.egg-info/PKG-INFO
--rw-r--r--   0 nguertler  (7419) is        (1040)     1621 2023-04-27 13:48:26.000000 trifinger_rl_datasets-1.0.0/trifinger_rl_datasets.egg-info/SOURCES.txt
--rw-r--r--   0 nguertler  (7419) is        (1040)        1 2023-04-27 13:48:26.000000 trifinger_rl_datasets-1.0.0/trifinger_rl_datasets.egg-info/dependency_links.txt
--rw-r--r--   0 nguertler  (7419) is        (1040)       90 2023-04-27 13:48:26.000000 trifinger_rl_datasets-1.0.0/trifinger_rl_datasets.egg-info/requires.txt
--rw-r--r--   0 nguertler  (7419) is        (1040)       22 2023-04-27 13:48:26.000000 trifinger_rl_datasets-1.0.0/trifinger_rl_datasets.egg-info/top_level.txt
+drwxr-xr-x   0 nguertler  (7419) is        (1040)        0 2023-05-22 13:29:36.660564 trifinger_rl_datasets-1.0.1/
+-rw-rw-r--   0 nguertler  (7419) is        (1040)     1532 2022-09-07 07:59:18.000000 trifinger_rl_datasets-1.0.1/LICENSE
+-rw-r--r--   0 nguertler  (7419) is        (1040)     6924 2023-05-22 13:29:36.661561 trifinger_rl_datasets-1.0.1/PKG-INFO
+-rw-r--r--   0 nguertler  (7419) is        (1040)     5505 2023-05-19 17:16:04.000000 trifinger_rl_datasets-1.0.1/README.md
+-rw-rw-r--   0 nguertler  (7419) is        (1040)      142 2022-09-07 07:59:18.000000 trifinger_rl_datasets-1.0.1/pyproject.toml
+-rw-r--r--   0 nguertler  (7419) is        (1040)      784 2023-05-22 13:29:36.665562 trifinger_rl_datasets-1.0.1/setup.cfg
+-rw-r--r--   0 nguertler  (7419) is        (1040)       38 2023-03-23 14:08:48.000000 trifinger_rl_datasets-1.0.1/setup.py
+drwxr-xr-x   0 nguertler  (7419) is        (1040)        0 2023-05-22 13:29:36.471568 trifinger_rl_datasets-1.0.1/trifinger_rl_datasets/
+-rw-r--r--   0 nguertler  (7419) is        (1040)     3277 2023-05-22 13:27:57.000000 trifinger_rl_datasets-1.0.1/trifinger_rl_datasets/__init__.py
+drwxr-xr-x   0 nguertler  (7419) is        (1040)        0 2023-05-22 13:29:36.643568 trifinger_rl_datasets-1.0.1/trifinger_rl_datasets/data/
+-rw-r--r--   0 nguertler  (7419) is        (1040)        0 2023-01-20 15:23:15.000000 trifinger_rl_datasets-1.0.1/trifinger_rl_datasets/data/__init__.py
+-rw-r--r--   0 nguertler  (7419) is        (1040)     1170 2023-02-20 18:18:55.000000 trifinger_rl_datasets-1.0.1/trifinger_rl_datasets/data/r1_camera180.yml
+-rw-r--r--   0 nguertler  (7419) is        (1040)     1176 2023-02-20 18:18:55.000000 trifinger_rl_datasets-1.0.1/trifinger_rl_datasets/data/r1_camera300.yml
+-rw-r--r--   0 nguertler  (7419) is        (1040)     1177 2023-02-20 18:18:55.000000 trifinger_rl_datasets-1.0.1/trifinger_rl_datasets/data/r1_camera60.yml
+-rw-r--r--   0 nguertler  (7419) is        (1040)     1180 2023-02-20 18:18:55.000000 trifinger_rl_datasets-1.0.1/trifinger_rl_datasets/data/r3_camera180.yml
+-rw-r--r--   0 nguertler  (7419) is        (1040)     1172 2023-02-20 18:18:55.000000 trifinger_rl_datasets-1.0.1/trifinger_rl_datasets/data/r3_camera300.yml
+-rw-r--r--   0 nguertler  (7419) is        (1040)     1175 2023-02-20 18:18:55.000000 trifinger_rl_datasets-1.0.1/trifinger_rl_datasets/data/r3_camera60.yml
+-rw-r--r--   0 nguertler  (7419) is        (1040)     1178 2023-02-20 18:18:55.000000 trifinger_rl_datasets-1.0.1/trifinger_rl_datasets/data/r4_camera180.yml
+-rw-r--r--   0 nguertler  (7419) is        (1040)     1178 2023-02-20 18:18:55.000000 trifinger_rl_datasets-1.0.1/trifinger_rl_datasets/data/r4_camera300.yml
+-rw-r--r--   0 nguertler  (7419) is        (1040)     1169 2023-02-20 18:18:55.000000 trifinger_rl_datasets-1.0.1/trifinger_rl_datasets/data/r4_camera60.yml
+-rw-r--r--   0 nguertler  (7419) is        (1040)     1188 2023-02-20 18:18:55.000000 trifinger_rl_datasets-1.0.1/trifinger_rl_datasets/data/r5_camera180.yml
+-rw-r--r--   0 nguertler  (7419) is        (1040)     1177 2023-02-20 18:18:55.000000 trifinger_rl_datasets-1.0.1/trifinger_rl_datasets/data/r5_camera300.yml
+-rw-r--r--   0 nguertler  (7419) is        (1040)     1175 2023-02-20 18:18:55.000000 trifinger_rl_datasets-1.0.1/trifinger_rl_datasets/data/r5_camera60.yml
+-rw-r--r--   0 nguertler  (7419) is        (1040)     1184 2023-02-20 18:18:55.000000 trifinger_rl_datasets-1.0.1/trifinger_rl_datasets/data/r6_camera180.yml
+-rw-r--r--   0 nguertler  (7419) is        (1040)     1173 2023-02-20 18:18:55.000000 trifinger_rl_datasets-1.0.1/trifinger_rl_datasets/data/r6_camera300.yml
+-rw-r--r--   0 nguertler  (7419) is        (1040)     1167 2023-02-20 18:18:55.000000 trifinger_rl_datasets-1.0.1/trifinger_rl_datasets/data/r6_camera60.yml
+-rw-r--r--   0 nguertler  (7419) is        (1040)     1180 2023-02-20 18:18:56.000000 trifinger_rl_datasets-1.0.1/trifinger_rl_datasets/data/r7_camera180.yml
+-rw-r--r--   0 nguertler  (7419) is        (1040)     1175 2023-02-20 18:18:56.000000 trifinger_rl_datasets-1.0.1/trifinger_rl_datasets/data/r7_camera300.yml
+-rw-r--r--   0 nguertler  (7419) is        (1040)     1174 2023-02-20 18:18:56.000000 trifinger_rl_datasets-1.0.1/trifinger_rl_datasets/data/r7_camera60.yml
+-rw-r--r--   0 nguertler  (7419) is        (1040)     1180 2023-02-20 18:18:56.000000 trifinger_rl_datasets-1.0.1/trifinger_rl_datasets/data/r8_camera180.yml
+-rw-r--r--   0 nguertler  (7419) is        (1040)     1176 2023-02-20 18:18:56.000000 trifinger_rl_datasets-1.0.1/trifinger_rl_datasets/data/r8_camera300.yml
+-rw-r--r--   0 nguertler  (7419) is        (1040)     1171 2023-02-20 18:18:56.000000 trifinger_rl_datasets-1.0.1/trifinger_rl_datasets/data/r8_camera60.yml
+-rw-r--r--   0 nguertler  (7419) is        (1040)  1556408 2023-01-20 15:23:15.000000 trifinger_rl_datasets-1.0.1/trifinger_rl_datasets/data/trifingerpro_shuffle_cube_trajectory_fast.npy
+-rw-r--r--   0 nguertler  (7419) is        (1040)    39624 2023-05-22 13:09:31.000000 trifinger_rl_datasets-1.0.1/trifinger_rl_datasets/dataset_env.py
+-rw-r--r--   0 nguertler  (7419) is        (1040)     3104 2023-03-23 14:08:48.000000 trifinger_rl_datasets-1.0.1/trifinger_rl_datasets/evaluate_sim.py
+-rw-r--r--   0 nguertler  (7419) is        (1040)     3139 2023-03-23 14:08:48.000000 trifinger_rl_datasets-1.0.1/trifinger_rl_datasets/evaluation.py
+-rw-r--r--   0 nguertler  (7419) is        (1040)     2067 2023-03-23 14:08:48.000000 trifinger_rl_datasets-1.0.1/trifinger_rl_datasets/policy_base.py
+-rw-r--r--   0 nguertler  (7419) is        (1040)        0 2023-01-20 15:23:15.000000 trifinger_rl_datasets-1.0.1/trifinger_rl_datasets/py.typed
+-rw-r--r--   0 nguertler  (7419) is        (1040)     1673 2023-01-20 15:23:15.000000 trifinger_rl_datasets-1.0.1/trifinger_rl_datasets/sampling_utils.py
+-rw-r--r--   0 nguertler  (7419) is        (1040)    27673 2023-05-22 13:20:18.000000 trifinger_rl_datasets-1.0.1/trifinger_rl_datasets/sim_env.py
+-rw-r--r--   0 nguertler  (7419) is        (1040)     2743 2023-01-20 15:23:15.000000 trifinger_rl_datasets-1.0.1/trifinger_rl_datasets/utils.py
+drwxr-xr-x   0 nguertler  (7419) is        (1040)        0 2023-05-22 13:29:36.498564 trifinger_rl_datasets-1.0.1/trifinger_rl_datasets.egg-info/
+-rw-r--r--   0 nguertler  (7419) is        (1040)     6924 2023-05-22 13:29:36.000000 trifinger_rl_datasets-1.0.1/trifinger_rl_datasets.egg-info/PKG-INFO
+-rw-r--r--   0 nguertler  (7419) is        (1040)     1621 2023-05-22 13:29:36.000000 trifinger_rl_datasets-1.0.1/trifinger_rl_datasets.egg-info/SOURCES.txt
+-rw-r--r--   0 nguertler  (7419) is        (1040)        1 2023-05-22 13:29:36.000000 trifinger_rl_datasets-1.0.1/trifinger_rl_datasets.egg-info/dependency_links.txt
+-rw-r--r--   0 nguertler  (7419) is        (1040)       90 2023-05-22 13:29:36.000000 trifinger_rl_datasets-1.0.1/trifinger_rl_datasets.egg-info/requires.txt
+-rw-r--r--   0 nguertler  (7419) is        (1040)       22 2023-05-22 13:29:36.000000 trifinger_rl_datasets-1.0.1/trifinger_rl_datasets.egg-info/top_level.txt
```

### Comparing `trifinger_rl_datasets-1.0.0/LICENSE` & `trifinger_rl_datasets-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `trifinger_rl_datasets-1.0.0/PKG-INFO` & `trifinger_rl_datasets-1.0.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trifinger_rl_datasets
-Version: 1.0.0
+Version: 1.0.1
 Summary: Gym environments which provide offline RL datasets collected on the TriFinger system.
 Home-page: UNKNOWN
 Author: Nico Gürtler
 Author-email: nico.guertler@tuebingen.mpg.de
 License: BSD 3-Clause
 Description: # TriFinger RL Datasets
         
@@ -28,14 +28,17 @@
         This section provides short examples of how to load datasets and evaluate a policy in simulation. More details on how to work with the datasets can be found in the [documentation](https://webdav.tuebingen.mpg.de/trifinger-rl/docs/).
         
         
         ### Loading a dataset
         
         The datasets are accessible via gym environments which are automatically registered when importing the package. They are automatically downloaded when requested and stored in `~/.trifinger_rl_datasets` as Zarr files by default (see the [documentation](https://webdav.tuebingen.mpg.de/trifinger-rl/docs/) for custom paths to the datasets). The code for loading the datasets follows the interface suggested by [D4RL](https://github.com/rail-berkeley/d4rl) and extends it where needed. 
         
+        As an alternative to the automatic download, the datasets can also be downloaded
+        manually from the [Edmond repository](https://edmond.mpdl.mpg.de/dataset.xhtml?persistentId=doi:10.17617/3.DXZ7TL).
+        
         The datasets are named following the pattern `trifinger-cube-task-source-type-v0` where `task` is either `push` or `lift`, `source` is either `sim` or `real` and `type` can be either `mixed`, `weak-n-expert` or `expert`.
         
         By default the observations are loaded as flat arrays. For the simulated datasets the environment can be stepped and visualized. Example usage (also see `demo/load_dataset.py`):
         
         ```python
         import gymnasium as gym
```

### Comparing `trifinger_rl_datasets-1.0.0/README.md` & `trifinger_rl_datasets-1.0.1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -20,14 +20,17 @@
 This section provides short examples of how to load datasets and evaluate a policy in simulation. More details on how to work with the datasets can be found in the [documentation](https://webdav.tuebingen.mpg.de/trifinger-rl/docs/).
 
 
 ### Loading a dataset
 
 The datasets are accessible via gym environments which are automatically registered when importing the package. They are automatically downloaded when requested and stored in `~/.trifinger_rl_datasets` as Zarr files by default (see the [documentation](https://webdav.tuebingen.mpg.de/trifinger-rl/docs/) for custom paths to the datasets). The code for loading the datasets follows the interface suggested by [D4RL](https://github.com/rail-berkeley/d4rl) and extends it where needed. 
 
+As an alternative to the automatic download, the datasets can also be downloaded
+manually from the [Edmond repository](https://edmond.mpdl.mpg.de/dataset.xhtml?persistentId=doi:10.17617/3.DXZ7TL).
+
 The datasets are named following the pattern `trifinger-cube-task-source-type-v0` where `task` is either `push` or `lift`, `source` is either `sim` or `real` and `type` can be either `mixed`, `weak-n-expert` or `expert`.
 
 By default the observations are loaded as flat arrays. For the simulated datasets the environment can be stepped and visualized. Example usage (also see `demo/load_dataset.py`):
 
 ```python
 import gymnasium as gym
```

### Comparing `trifinger_rl_datasets-1.0.0/setup.cfg` & `trifinger_rl_datasets-1.0.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `trifinger_rl_datasets-1.0.0/trifinger_rl_datasets/__init__.py` & `trifinger_rl_datasets-1.0.1/trifinger_rl_datasets/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,15 @@
-__version__ = "1.0.0"
+__version__ = "1.0.1"
 
 from gymnasium.envs.registration import register
 
 from .dataset_env import TriFingerDatasetEnv
 from .evaluation import Evaluation
 from .policy_base import PolicyBase, PolicyConfig
+from .sim_env import SimTriFingerCubeEnv
 
 
 base_url = "https://robots.real-robot-challenge.com/public/trifinger_rl_datasets/"
 
 dataset_names = [
     "trifinger-cube-push-real-expert-v0",
     "trifinger-cube-push-real-expert-image-v0",
```

### Comparing `trifinger_rl_datasets-1.0.0/trifinger_rl_datasets/data/r1_camera180.yml` & `trifinger_rl_datasets-1.0.1/trifinger_rl_datasets/data/r1_camera180.yml`

 * *Files identical despite different names*

### Comparing `trifinger_rl_datasets-1.0.0/trifinger_rl_datasets/data/r1_camera300.yml` & `trifinger_rl_datasets-1.0.1/trifinger_rl_datasets/data/r1_camera300.yml`

 * *Files identical despite different names*

### Comparing `trifinger_rl_datasets-1.0.0/trifinger_rl_datasets/data/r1_camera60.yml` & `trifinger_rl_datasets-1.0.1/trifinger_rl_datasets/data/r1_camera60.yml`

 * *Files identical despite different names*

### Comparing `trifinger_rl_datasets-1.0.0/trifinger_rl_datasets/data/r3_camera180.yml` & `trifinger_rl_datasets-1.0.1/trifinger_rl_datasets/data/r3_camera180.yml`

 * *Files identical despite different names*

### Comparing `trifinger_rl_datasets-1.0.0/trifinger_rl_datasets/data/r3_camera300.yml` & `trifinger_rl_datasets-1.0.1/trifinger_rl_datasets/data/r3_camera300.yml`

 * *Files identical despite different names*

### Comparing `trifinger_rl_datasets-1.0.0/trifinger_rl_datasets/data/r3_camera60.yml` & `trifinger_rl_datasets-1.0.1/trifinger_rl_datasets/data/r3_camera60.yml`

 * *Files identical despite different names*

### Comparing `trifinger_rl_datasets-1.0.0/trifinger_rl_datasets/data/r4_camera180.yml` & `trifinger_rl_datasets-1.0.1/trifinger_rl_datasets/data/r4_camera180.yml`

 * *Files identical despite different names*

### Comparing `trifinger_rl_datasets-1.0.0/trifinger_rl_datasets/data/r4_camera300.yml` & `trifinger_rl_datasets-1.0.1/trifinger_rl_datasets/data/r4_camera300.yml`

 * *Files identical despite different names*

### Comparing `trifinger_rl_datasets-1.0.0/trifinger_rl_datasets/data/r4_camera60.yml` & `trifinger_rl_datasets-1.0.1/trifinger_rl_datasets/data/r4_camera60.yml`

 * *Files identical despite different names*

### Comparing `trifinger_rl_datasets-1.0.0/trifinger_rl_datasets/data/r5_camera180.yml` & `trifinger_rl_datasets-1.0.1/trifinger_rl_datasets/data/r5_camera180.yml`

 * *Files identical despite different names*

### Comparing `trifinger_rl_datasets-1.0.0/trifinger_rl_datasets/data/r5_camera300.yml` & `trifinger_rl_datasets-1.0.1/trifinger_rl_datasets/data/r5_camera300.yml`

 * *Files identical despite different names*

### Comparing `trifinger_rl_datasets-1.0.0/trifinger_rl_datasets/data/r5_camera60.yml` & `trifinger_rl_datasets-1.0.1/trifinger_rl_datasets/data/r5_camera60.yml`

 * *Files identical despite different names*

### Comparing `trifinger_rl_datasets-1.0.0/trifinger_rl_datasets/data/r6_camera180.yml` & `trifinger_rl_datasets-1.0.1/trifinger_rl_datasets/data/r6_camera180.yml`

 * *Files identical despite different names*

### Comparing `trifinger_rl_datasets-1.0.0/trifinger_rl_datasets/data/r6_camera300.yml` & `trifinger_rl_datasets-1.0.1/trifinger_rl_datasets/data/r6_camera300.yml`

 * *Files identical despite different names*

### Comparing `trifinger_rl_datasets-1.0.0/trifinger_rl_datasets/data/r6_camera60.yml` & `trifinger_rl_datasets-1.0.1/trifinger_rl_datasets/data/r6_camera60.yml`

 * *Files identical despite different names*

### Comparing `trifinger_rl_datasets-1.0.0/trifinger_rl_datasets/data/r7_camera180.yml` & `trifinger_rl_datasets-1.0.1/trifinger_rl_datasets/data/r7_camera180.yml`

 * *Files identical despite different names*

### Comparing `trifinger_rl_datasets-1.0.0/trifinger_rl_datasets/data/r7_camera300.yml` & `trifinger_rl_datasets-1.0.1/trifinger_rl_datasets/data/r7_camera300.yml`

 * *Files identical despite different names*

### Comparing `trifinger_rl_datasets-1.0.0/trifinger_rl_datasets/data/r7_camera60.yml` & `trifinger_rl_datasets-1.0.1/trifinger_rl_datasets/data/r7_camera60.yml`

 * *Files identical despite different names*

### Comparing `trifinger_rl_datasets-1.0.0/trifinger_rl_datasets/data/r8_camera180.yml` & `trifinger_rl_datasets-1.0.1/trifinger_rl_datasets/data/r8_camera180.yml`

 * *Files identical despite different names*

### Comparing `trifinger_rl_datasets-1.0.0/trifinger_rl_datasets/data/r8_camera300.yml` & `trifinger_rl_datasets-1.0.1/trifinger_rl_datasets/data/r8_camera300.yml`

 * *Files identical despite different names*

### Comparing `trifinger_rl_datasets-1.0.0/trifinger_rl_datasets/data/r8_camera60.yml` & `trifinger_rl_datasets-1.0.1/trifinger_rl_datasets/data/r8_camera60.yml`

 * *Files identical despite different names*

### Comparing `trifinger_rl_datasets-1.0.0/trifinger_rl_datasets/data/trifingerpro_shuffle_cube_trajectory_fast.npy` & `trifinger_rl_datasets-1.0.1/trifinger_rl_datasets/data/trifingerpro_shuffle_cube_trajectory_fast.npy`

 * *Files identical despite different names*

### Comparing `trifinger_rl_datasets-1.0.0/trifinger_rl_datasets/dataset_env.py` & `trifinger_rl_datasets-1.0.1/trifinger_rl_datasets/dataset_env.py`

 * *Files 2% similar despite different names*

```diff
@@ -387,28 +387,27 @@
             # scale obs
             obs = self._scale_obs(obs)
         if images is not None:
             return obs, images
         else:
             return obs
 
-    def get_obs_indices(self):
+    def get_obs_indices(self) -> Tuple[Dict, Dict]:
         """Get index ranges that correspond to the different observation components.
 
         Also returns a dictionary containing the shapes of these observation
         components.
 
         Returns:
-            A tuple containing:
             - A dictionary with keys corresponding to the observation components and
-            values being tuples of the form (start, end), where start and end are
-            the indices at which the observation component starts and ends. The
-            nested dictionary structure of the observation is preserved.
+              values being tuples of the form (start, end), where start and end are
+              the indices at which the observation component starts and ends. The
+              nested dictionary structure of the observation is preserved.
             - A dictionary of the same structure but with values being the shapes
-            of the observation components."""
+              of the observation components."""
 
         def _construct_dummy_obs(spaces_dict, counter=[0]):
             """Construct dummy observation which has an array repeating
             a different integer as the value of each component."""
             dummy_obs = {}
             for i, (k, v) in enumerate(spaces_dict.items()):
                 if isinstance(v, spaces.Dict):
@@ -438,17 +437,18 @@
     def get_dataset_stats(self, zarr_path: Union[str, os.PathLike] = None) -> Dict:
         """Get statistics of dataset such as number of timesteps.
 
         Args:
             zarr_path:  Optional path to a Zarr directory containing the dataset, which will be
                 used instead of the default.
         Returns:
-            The statistics of the dataset as a dictionary with keys:
+            The statistics of the dataset as a dictionary with keys
+
                 - n_timesteps: Number of timesteps in dataset. Corresponds to the
-                    number of observations, actions and rewards.
+                  number of observations, actions and rewards.
                 - obs_size: Size of the observation vector.
                 - action_size: Size of the action vector.
         """
         if zarr_path is None:
             zarr_path = self._download_dataset()
 
         store = zarr.LMDBStore(zarr_path, readonly=True)
@@ -463,22 +463,23 @@
     def get_image_stats(self, zarr_path: Union[str, os.PathLike] = None) -> Dict:
         """Get statistics of image data in dataset.
 
         Args:
             zarr_path:  Optional path to a Zarr directory containing the dataset, which will be
                 used instead of the default.
         Returns:
-            The statistics of the image data as a dictionary with keys:
+            The statistics of the image data as a dictionary with keys
+
                 - n_images: Number of images in the dataset.
                 - n_cameras: Number of cameras used to capture the images.
                 - n_channels: Number of channels in the images.
                 - image_shape: Shape of the images in the format (height, width).
                 - reorder_pixels: Whether the pixels in the images have been reordered
-                    to have the pixels corresponding to one color in the Bayer pattern
-                    together in blocks (to improve image compression).
+                  to have the pixels corresponding to one color in the Bayer pattern
+                  together in blocks (to improve image compression).
         """
         if zarr_path is None:
             zarr_path = self._download_dataset()
 
         store = zarr.LMDBStore(zarr_path, readonly=True)
         with zarr.open(store=store) as root:
             image_stats = {
@@ -620,30 +621,31 @@
                 dataset is returned.
             indices: Optional array of timestep indices for which to load data. rng
                 and indices are mutually exclusive, only one of them can be set.
             n_threads: Number of threads to use for processing the images. If None,
                 the number of threads is set to the number of CPUs available to the
                 process.
         Returns:
-            A dictionary with the following items:
+            A dictionary containing the following keys
+
                 - observations: Either an array or a list of dictionaries
-                    containing the observations depending on whether
-                    `flatten_obs` is True or False.
+                  containing the observations depending on whether
+                  `flatten_obs` is True or False.
                 - actions: Array containing the actions.
                 - rewards: Array containing the rewards.
                 - timeouts: Array containing the timeouts (True only at
-                    the end of an episode by default. Always False if
-                    `set_terminals` is True).
+                  the end of an episode by default. Always False if
+                  `set_terminals` is True).
                 - terminals: Array containing the terminals (Always
-                    False by default. If `set_terminals` is True, only
-                    True at the last timestep of an episode).
+                  False by default. If `set_terminals` is True, only
+                  True at the last timestep of an episode).
                 - images (only if present in dataset): Array of the
-                    shape (n_control_timesteps, n_cameras, n_channels,
-                    height, width) containing the image data. The cannels
-                    are ordered as RGB.
+                  shape (n_control_timesteps, n_cameras, n_channels,
+                  height, width) containing the image data. The cannels
+                  are ordered as RGB.
         """
 
         # The offline RL dataset is loaded from a Zarr directory which contains
         # the following Zarr arrays (this is an implementation detail and
         # not necessary to understand for users of the class):
         # - observations: Two-dimensional array of shape
         #     `(n_control_timesteps, n_obs)` containing the observations as
@@ -829,29 +831,32 @@
         """Execute one step.
 
         Args:
             action: Array of 9 torque commands, one for each robot joint.
 
         Returns:
             A tuple with
+
             - observation (dict or tuple): agent's observation of the current
-                environment.  If `self.flatten_obs` is False then as a dictionary.
-                If `self.flatten_obs` is True then either as a 1D NumPy array
-                (if no images are to be included) or as a tuple (if images are
-                to be included) consisting of
-                * a 1D NumPy array containing all observations except the
+              environment.  If `self.flatten_obs` is False then as a dictionary.
+              If `self.flatten_obs` is True then either as a 1D NumPy array
+              (if no images are to be included) or as a tuple (if images are
+              to be included) consisting of
+
+              * a 1D NumPy array containing all observations except the
                 camera images, and
-                * a NumPy array of shape (n_cameras, n_channels, height, width)
+              * a NumPy array of shape (n_cameras, n_channels, height, width)
                 containing the camera images.
+
             - reward (float): amount of reward returned after previous action.
             - terminated (bool): whether the MDP has reached a terminal state. If true,
-                the user needs to call `reset()`.
+              the user needs to call `reset()`.
             - truncated (bool): Whether the truncation condition outside the scope
-                of the MDP is satisfied. For this environment this corresponds to a
-                timeout. If true, the user needs to call `reset()`.
+              of the MDP is satisfied. For this environment this corresponds to a
+              timeout. If true, the user needs to call `reset()`.
             - info (dict): info dictionary containing the current time index.
         """
         if self.real_robot:
             raise NotImplementedError(
                 "The step method is not available for real-robot data."
             )
         obs, rew, terminated, truncated, info = self.sim_env.step(action, **kwargs)
```

### Comparing `trifinger_rl_datasets-1.0.0/trifinger_rl_datasets/evaluate_sim.py` & `trifinger_rl_datasets-1.0.1/trifinger_rl_datasets/evaluate_sim.py`

 * *Files identical despite different names*

### Comparing `trifinger_rl_datasets-1.0.0/trifinger_rl_datasets/evaluation.py` & `trifinger_rl_datasets-1.0.1/trifinger_rl_datasets/evaluation.py`

 * *Files identical despite different names*

### Comparing `trifinger_rl_datasets-1.0.0/trifinger_rl_datasets/policy_base.py` & `trifinger_rl_datasets-1.0.1/trifinger_rl_datasets/policy_base.py`

 * *Files identical despite different names*

### Comparing `trifinger_rl_datasets-1.0.0/trifinger_rl_datasets/sampling_utils.py` & `trifinger_rl_datasets-1.0.1/trifinger_rl_datasets/sampling_utils.py`

 * *Files identical despite different names*

### Comparing `trifinger_rl_datasets-1.0.0/trifinger_rl_datasets/sim_env.py` & `trifinger_rl_datasets-1.0.1/trifinger_rl_datasets/sim_env.py`

 * *Files 2% similar despite different names*

```diff
@@ -372,21 +372,22 @@
         Args:
             action: An action provided by the agent
             preappend_actions (bool): Whether to already append actions that
                 will be executed during obs-action delay to action queue.
 
         Returns:
             tuple:
+
             - observation (dict): agent's observation of the current environment.
             - reward (float): amount of reward returned after previous action.
             - terminated (bool): whether the MDP has reached a terminal state. If true,
-                the user needs to call `reset()`.
+              the user needs to call `reset()`.
             - truncated (bool): Whether the truncation condition outside the scope
-                of the MDP is satisfied. For this environment this corresponds to a
-                timeout. If true, the user needs to call `reset()`.
+              of the MDP is satisfied. For this environment this corresponds to a
+              timeout. If true, the user needs to call `reset()`.
             - info (dict): info dictionary containing the current time index.
         """
         if self.platform is None:
             raise RuntimeError("Call `reset()` before starting to step.")
 
         if not self._check_action(action):
             raise ValueError("Given action is not contained in the action space.")
@@ -436,18 +437,21 @@
         observation, info = self._create_observation(self.t_obs, action)
         reward = self.compute_reward(
             observation["achieved_goal"], observation["desired_goal"], info
         )
         truncated = self.step_count >= self.episode_length
 
         if not truncated and preappend_actions:
+            t_now = self.platform.get_current_timeindex()
             # Append action to action queue of robot for as many time
             # steps as the obs_action_delay dictates. This gives the
             # user time to evaluate the policy.
-            for _ in range(self.obs_action_delay):
+            # Also take time into account that might have already passed
+            # while the observation was processed.
+            for _ in range(max(self.obs_action_delay - (t_now - self.t_obs), 0)):
                 self._append_desired_action(robot_action)
 
         return observation, reward, False, truncated, info
 
     def reset(  # type: ignore
         self, preappend_actions: bool = True
     ):
@@ -655,14 +659,16 @@
         assert self.platform is not None, "Environment is not initialised."
 
         # robot action is torque
         robot_action = self.platform.Action(torque=gym_action)
         return robot_action
 
     def render(self, mode: str = "human"):
+        """Does nothing. See :class:`SimTriFingerCubeEnv` for how to enable
+        visualization."""
         pass
 
     def reset_cube(self):
         """Replay a recorded trajectory to move cube to center of arena."""
 
         for position in self._cube_reset_traj[: self._reset_trajectory_length : 2]:
             robot_action = self.platform.Action(position=position)
```

### Comparing `trifinger_rl_datasets-1.0.0/trifinger_rl_datasets/utils.py` & `trifinger_rl_datasets-1.0.1/trifinger_rl_datasets/utils.py`

 * *Files identical despite different names*

### Comparing `trifinger_rl_datasets-1.0.0/trifinger_rl_datasets.egg-info/PKG-INFO` & `trifinger_rl_datasets-1.0.1/trifinger_rl_datasets.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trifinger-rl-datasets
-Version: 1.0.0
+Version: 1.0.1
 Summary: Gym environments which provide offline RL datasets collected on the TriFinger system.
 Home-page: UNKNOWN
 Author: Nico Gürtler
 Author-email: nico.guertler@tuebingen.mpg.de
 License: BSD 3-Clause
 Description: # TriFinger RL Datasets
         
@@ -28,14 +28,17 @@
         This section provides short examples of how to load datasets and evaluate a policy in simulation. More details on how to work with the datasets can be found in the [documentation](https://webdav.tuebingen.mpg.de/trifinger-rl/docs/).
         
         
         ### Loading a dataset
         
         The datasets are accessible via gym environments which are automatically registered when importing the package. They are automatically downloaded when requested and stored in `~/.trifinger_rl_datasets` as Zarr files by default (see the [documentation](https://webdav.tuebingen.mpg.de/trifinger-rl/docs/) for custom paths to the datasets). The code for loading the datasets follows the interface suggested by [D4RL](https://github.com/rail-berkeley/d4rl) and extends it where needed. 
         
+        As an alternative to the automatic download, the datasets can also be downloaded
+        manually from the [Edmond repository](https://edmond.mpdl.mpg.de/dataset.xhtml?persistentId=doi:10.17617/3.DXZ7TL).
+        
         The datasets are named following the pattern `trifinger-cube-task-source-type-v0` where `task` is either `push` or `lift`, `source` is either `sim` or `real` and `type` can be either `mixed`, `weak-n-expert` or `expert`.
         
         By default the observations are loaded as flat arrays. For the simulated datasets the environment can be stepped and visualized. Example usage (also see `demo/load_dataset.py`):
         
         ```python
         import gymnasium as gym
```

### Comparing `trifinger_rl_datasets-1.0.0/trifinger_rl_datasets.egg-info/SOURCES.txt` & `trifinger_rl_datasets-1.0.1/trifinger_rl_datasets.egg-info/SOURCES.txt`

 * *Files identical despite different names*

