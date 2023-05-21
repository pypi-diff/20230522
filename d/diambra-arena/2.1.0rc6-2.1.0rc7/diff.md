# Comparing `tmp/diambra-arena-2.1.0rc6.tar.gz` & `tmp/diambra-arena-2.1.0rc7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "diambra-arena-2.1.0rc6.tar", last modified: Thu May  4 18:11:27 2023, max compression
+gzip compressed data, was "diambra-arena-2.1.0rc7.tar", last modified: Sun May 21 23:56:49 2023, max compression
```

## Comparing `diambra-arena-2.1.0rc6.tar` & `diambra-arena-2.1.0rc7.tar`

### file list

```diff
@@ -1,63 +1,63 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 18:11:27.097343 diambra-arena-2.1.0rc6/
--rw-r--r--   0 runner    (1001) docker     (123)     3365 2023-05-04 18:11:01.000000 diambra-arena-2.1.0rc6/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-05-04 18:11:01.000000 diambra-arena-2.1.0rc6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    16900 2023-05-04 18:11:27.097343 diambra-arena-2.1.0rc6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    15935 2023-05-04 18:11:01.000000 diambra-arena-2.1.0rc6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 18:11:27.081343 diambra-arena-2.1.0rc6/diambra/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 18:11:01.000000 diambra-arena-2.1.0rc6/diambra/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 18:11:27.081343 diambra-arena-2.1.0rc6/diambra/arena/
--rw-r--r--   0 runner    (1001) docker     (123)      207 2023-05-04 18:11:01.000000 diambra-arena-2.1.0rc6/diambra/arena/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21897 2023-05-04 18:11:01.000000 diambra-arena-2.1.0rc6/diambra/arena/arena_gym.py
--rw-r--r--   0 runner    (1001) docker     (123)    16522 2023-05-04 18:11:01.000000 diambra-arena-2.1.0rc6/diambra/arena/arena_imitation_learning_gym.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 18:11:27.081343 diambra-arena-2.1.0rc6/diambra/arena/engine/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 18:11:01.000000 diambra-arena-2.1.0rc6/diambra/arena/engine/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11077 2023-05-04 18:11:01.000000 diambra-arena-2.1.0rc6/diambra/arena/engine/interface.py
--rw-r--r--   0 runner    (1001) docker     (123)     8098 2023-05-04 18:11:01.000000 diambra-arena-2.1.0rc6/diambra/arena/env_settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     3091 2023-05-04 18:11:01.000000 diambra-arena-2.1.0rc6/diambra/arena/make_env.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 18:11:27.085343 diambra-arena-2.1.0rc6/diambra/arena/ray_rllib/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 18:11:01.000000 diambra-arena-2.1.0rc6/diambra/arena/ray_rllib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8024 2023-05-04 18:11:01.000000 diambra-arena-2.1.0rc6/diambra/arena/ray_rllib/make_ray_env.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 18:11:27.085343 diambra-arena-2.1.0rc6/diambra/arena/stable_baselines/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 18:11:01.000000 diambra-arena-2.1.0rc6/diambra/arena/stable_baselines/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3759 2023-05-04 18:11:01.000000 diambra-arena-2.1.0rc6/diambra/arena/stable_baselines/make_sb_env.py
--rw-r--r--   0 runner    (1001) docker     (123)     7529 2023-05-04 18:11:01.000000 diambra-arena-2.1.0rc6/diambra/arena/stable_baselines/sb_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 18:11:27.085343 diambra-arena-2.1.0rc6/diambra/arena/stable_baselines/wrappers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 18:11:01.000000 diambra-arena-2.1.0rc6/diambra/arena/stable_baselines/wrappers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5796 2023-05-04 18:11:01.000000 diambra-arena-2.1.0rc6/diambra/arena/stable_baselines/wrappers/add_obs_wrap.py
--rw-r--r--   0 runner    (1001) docker     (123)     2747 2023-05-04 18:11:01.000000 diambra-arena-2.1.0rc6/diambra/arena/stable_baselines/wrappers/p2_wrap.py
--rw-r--r--   0 runner    (1001) docker     (123)     3867 2023-05-04 18:11:01.000000 diambra-arena-2.1.0rc6/diambra/arena/stable_baselines/wrappers/tektag_rew_wrap.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 18:11:27.085343 diambra-arena-2.1.0rc6/diambra/arena/stable_baselines3/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 18:11:01.000000 diambra-arena-2.1.0rc6/diambra/arena/stable_baselines3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2642 2023-05-04 18:11:01.000000 diambra-arena-2.1.0rc6/diambra/arena/stable_baselines3/make_sb3_env.py
--rw-r--r--   0 runner    (1001) docker     (123)     1712 2023-05-04 18:11:01.000000 diambra-arena-2.1.0rc6/diambra/arena/stable_baselines3/sb3_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 18:11:27.089343 diambra-arena-2.1.0rc6/diambra/arena/utils/
--rw-r--r--   0 runner    (1001) docker     (123)    55998 2023-05-04 18:11:01.000000 diambra-arena-2.1.0rc6/diambra/arena/utils/.splashScreen.gif
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 18:11:01.000000 diambra-arena-2.1.0rc6/diambra/arena/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    39134 2023-05-04 18:11:01.000000 diambra-arena-2.1.0rc6/diambra/arena/utils/controller.py
--rw-r--r--   0 runner    (1001) docker     (123)    10731 2023-05-04 18:11:01.000000 diambra-arena-2.1.0rc6/diambra/arena/utils/gym_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     8352 2023-05-04 18:11:01.000000 diambra-arena-2.1.0rc6/diambra/arena/utils/integratedGames.json
--rw-r--r--   0 runner    (1001) docker     (123)     4193 2023-05-04 18:11:01.000000 diambra-arena-2.1.0rc6/diambra/arena/utils/policies.py
--rw-r--r--   0 runner    (1001) docker     (123)     2427 2023-05-04 18:11:01.000000 diambra-arena-2.1.0rc6/diambra/arena/utils/splash_screen.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 18:11:27.093343 diambra-arena-2.1.0rc6/diambra/arena/wrappers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 18:11:01.000000 diambra-arena-2.1.0rc6/diambra/arena/wrappers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7755 2023-05-04 18:11:01.000000 diambra-arena-2.1.0rc6/diambra/arena/wrappers/arena_wrappers.py
--rw-r--r--   0 runner    (1001) docker     (123)    16154 2023-05-04 18:11:01.000000 diambra-arena-2.1.0rc6/diambra/arena/wrappers/obs_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     6630 2023-05-04 18:11:01.000000 diambra-arena-2.1.0rc6/diambra/arena/wrappers/obs_wrapper_hardcore.py
--rw-r--r--   0 runner    (1001) docker     (123)     6791 2023-05-04 18:11:01.000000 diambra-arena-2.1.0rc6/diambra/arena/wrappers/traj_rec_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     5617 2023-05-04 18:11:01.000000 diambra-arena-2.1.0rc6/diambra/arena/wrappers/traj_rec_wrapper_hardcore.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 18:11:27.093343 diambra-arena-2.1.0rc6/diambra_arena.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    16900 2023-05-04 18:11:27.000000 diambra-arena-2.1.0rc6/diambra_arena.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1726 2023-05-04 18:11:27.000000 diambra-arena-2.1.0rc6/diambra_arena.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 18:11:27.000000 diambra-arena-2.1.0rc6/diambra_arena.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      430 2023-05-04 18:11:27.000000 diambra-arena-2.1.0rc6/diambra_arena.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-04 18:11:27.000000 diambra-arena-2.1.0rc6/diambra_arena.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-04 18:11:27.097343 diambra-arena-2.1.0rc6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2178 2023-05-04 18:11:01.000000 diambra-arena-2.1.0rc6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 18:11:27.097343 diambra-arena-2.1.0rc6/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     5228 2023-05-04 18:11:01.000000 diambra-arena-2.1.0rc6/tests/test_gym_settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     4697 2023-05-04 18:11:01.000000 diambra-arena-2.1.0rc6/tests/test_imitation_learning.py
--rw-r--r--   0 runner    (1001) docker     (123)     4786 2023-05-04 18:11:01.000000 diambra-arena-2.1.0rc6/tests/test_integration.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6112 2023-05-04 18:11:01.000000 diambra-arena-2.1.0rc6/tests/test_random.py
--rw-r--r--   0 runner    (1001) docker     (123)     4200 2023-05-04 18:11:01.000000 diambra-arena-2.1.0rc6/tests/test_recording_settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     4562 2023-05-04 18:11:01.000000 diambra-arena-2.1.0rc6/tests/test_speed.py
--rw-r--r--   0 runner    (1001) docker     (123)     5588 2023-05-04 18:11:01.000000 diambra-arena-2.1.0rc6/tests/test_wrappers_settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 23:56:49.508239 diambra-arena-2.1.0rc7/
+-rw-r--r--   0 runner    (1001) docker     (123)     3346 2023-05-21 23:56:26.000000 diambra-arena-2.1.0rc7/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-05-21 23:56:26.000000 diambra-arena-2.1.0rc7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    16886 2023-05-21 23:56:49.508239 diambra-arena-2.1.0rc7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    15921 2023-05-21 23:56:26.000000 diambra-arena-2.1.0rc7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 23:56:49.480239 diambra-arena-2.1.0rc7/diambra/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-21 23:56:26.000000 diambra-arena-2.1.0rc7/diambra/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 23:56:49.484238 diambra-arena-2.1.0rc7/diambra/arena/
+-rw-r--r--   0 runner    (1001) docker     (123)      207 2023-05-21 23:56:26.000000 diambra-arena-2.1.0rc7/diambra/arena/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21897 2023-05-21 23:56:26.000000 diambra-arena-2.1.0rc7/diambra/arena/arena_gym.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16522 2023-05-21 23:56:26.000000 diambra-arena-2.1.0rc7/diambra/arena/arena_imitation_learning_gym.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 23:56:49.484238 diambra-arena-2.1.0rc7/diambra/arena/engine/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-21 23:56:26.000000 diambra-arena-2.1.0rc7/diambra/arena/engine/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11077 2023-05-21 23:56:26.000000 diambra-arena-2.1.0rc7/diambra/arena/engine/interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8098 2023-05-21 23:56:26.000000 diambra-arena-2.1.0rc7/diambra/arena/env_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3091 2023-05-21 23:56:26.000000 diambra-arena-2.1.0rc7/diambra/arena/make_env.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 23:56:49.484238 diambra-arena-2.1.0rc7/diambra/arena/ray_rllib/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-21 23:56:26.000000 diambra-arena-2.1.0rc7/diambra/arena/ray_rllib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8024 2023-05-21 23:56:26.000000 diambra-arena-2.1.0rc7/diambra/arena/ray_rllib/make_ray_env.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 23:56:49.488238 diambra-arena-2.1.0rc7/diambra/arena/stable_baselines/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-21 23:56:26.000000 diambra-arena-2.1.0rc7/diambra/arena/stable_baselines/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3759 2023-05-21 23:56:26.000000 diambra-arena-2.1.0rc7/diambra/arena/stable_baselines/make_sb_env.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7693 2023-05-21 23:56:26.000000 diambra-arena-2.1.0rc7/diambra/arena/stable_baselines/sb_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 23:56:49.492239 diambra-arena-2.1.0rc7/diambra/arena/stable_baselines/wrappers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-21 23:56:26.000000 diambra-arena-2.1.0rc7/diambra/arena/stable_baselines/wrappers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5796 2023-05-21 23:56:26.000000 diambra-arena-2.1.0rc7/diambra/arena/stable_baselines/wrappers/add_obs_wrap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2747 2023-05-21 23:56:26.000000 diambra-arena-2.1.0rc7/diambra/arena/stable_baselines/wrappers/p2_wrap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3867 2023-05-21 23:56:26.000000 diambra-arena-2.1.0rc7/diambra/arena/stable_baselines/wrappers/tektag_rew_wrap.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 23:56:49.492239 diambra-arena-2.1.0rc7/diambra/arena/stable_baselines3/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-21 23:56:26.000000 diambra-arena-2.1.0rc7/diambra/arena/stable_baselines3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2642 2023-05-21 23:56:26.000000 diambra-arena-2.1.0rc7/diambra/arena/stable_baselines3/make_sb3_env.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1844 2023-05-21 23:56:26.000000 diambra-arena-2.1.0rc7/diambra/arena/stable_baselines3/sb3_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 23:56:49.496239 diambra-arena-2.1.0rc7/diambra/arena/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)    55998 2023-05-21 23:56:26.000000 diambra-arena-2.1.0rc7/diambra/arena/utils/.splashScreen.gif
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-21 23:56:26.000000 diambra-arena-2.1.0rc7/diambra/arena/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39134 2023-05-21 23:56:26.000000 diambra-arena-2.1.0rc7/diambra/arena/utils/controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10731 2023-05-21 23:56:26.000000 diambra-arena-2.1.0rc7/diambra/arena/utils/gym_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8352 2023-05-21 23:56:26.000000 diambra-arena-2.1.0rc7/diambra/arena/utils/integratedGames.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4193 2023-05-21 23:56:26.000000 diambra-arena-2.1.0rc7/diambra/arena/utils/policies.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2427 2023-05-21 23:56:26.000000 diambra-arena-2.1.0rc7/diambra/arena/utils/splash_screen.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 23:56:49.500239 diambra-arena-2.1.0rc7/diambra/arena/wrappers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-21 23:56:26.000000 diambra-arena-2.1.0rc7/diambra/arena/wrappers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7755 2023-05-21 23:56:26.000000 diambra-arena-2.1.0rc7/diambra/arena/wrappers/arena_wrappers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16154 2023-05-21 23:56:26.000000 diambra-arena-2.1.0rc7/diambra/arena/wrappers/obs_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6630 2023-05-21 23:56:26.000000 diambra-arena-2.1.0rc7/diambra/arena/wrappers/obs_wrapper_hardcore.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6791 2023-05-21 23:56:26.000000 diambra-arena-2.1.0rc7/diambra/arena/wrappers/traj_rec_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5617 2023-05-21 23:56:26.000000 diambra-arena-2.1.0rc7/diambra/arena/wrappers/traj_rec_wrapper_hardcore.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 23:56:49.504239 diambra-arena-2.1.0rc7/diambra_arena.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    16886 2023-05-21 23:56:49.000000 diambra-arena-2.1.0rc7/diambra_arena.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1726 2023-05-21 23:56:49.000000 diambra-arena-2.1.0rc7/diambra_arena.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-21 23:56:49.000000 diambra-arena-2.1.0rc7/diambra_arena.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      430 2023-05-21 23:56:49.000000 diambra-arena-2.1.0rc7/diambra_arena.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-21 23:56:49.000000 diambra-arena-2.1.0rc7/diambra_arena.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-21 23:56:49.508239 diambra-arena-2.1.0rc7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2178 2023-05-21 23:56:27.000000 diambra-arena-2.1.0rc7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 23:56:49.508239 diambra-arena-2.1.0rc7/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     5228 2023-05-21 23:56:27.000000 diambra-arena-2.1.0rc7/tests/test_gym_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4697 2023-05-21 23:56:27.000000 diambra-arena-2.1.0rc7/tests/test_imitation_learning.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4786 2023-05-21 23:56:27.000000 diambra-arena-2.1.0rc7/tests/test_integration.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6112 2023-05-21 23:56:27.000000 diambra-arena-2.1.0rc7/tests/test_random.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4200 2023-05-21 23:56:27.000000 diambra-arena-2.1.0rc7/tests/test_recording_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4562 2023-05-21 23:56:27.000000 diambra-arena-2.1.0rc7/tests/test_speed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5588 2023-05-21 23:56:27.000000 diambra-arena-2.1.0rc7/tests/test_wrappers_settings.py
```

### Comparing `diambra-arena-2.1.0rc6/LICENSE.txt` & `diambra-arena-2.1.0rc7/LICENSE.txt`

 * *Files 5% similar despite different names*

```diff
@@ -1,26 +1,26 @@
-© 2018-2023, DIAMBRA | Dueling AI Arena, https://diambra.ai
+© 2018-2023, DIAMBRA Inc., https://diambra.ai
 
 Redistribution and use in source and binary forms, with or without modification, 
 are permitted provided that the following conditions are met:
 
 - Commercial use is forbidden without specific prior written permission received 
-  from DIAMBRA Team. In this context and for the purpose of this LICENSE, 
+  from DIAMBRA, Inc. In this context and for the purpose of this LICENSE, 
   "Commercial use" includes (but is not limited to): using this software to 
   organize Tournaments or Competitions of any type, selling services or 
   products that make use of this software (like providing it as a service, or 
   enclosed in a wrapper accessible via network of any type), and creating
   content through it that can be commercialized in any way
 - Redistributions of source code must retain the above copyright notice, this 
   list of conditions and the following disclaimer.
 - Redistributions in binary form must reproduce the above copyright notice, this 
   list of conditions and the following disclaimer in the documentation and/or 
   other materials provided with the distribution.
 - Distribution of derivative work is forbidden without specific prior written
-  permission received from DIAMBRA Team.
+  permission received from DIAMBRA, Inc.
 - Neither the name DIAMBRA | Dueling AI Arena nor the names of its contributors 
   may be used to endorse or promote products derived from this software without 
   specific prior written permission.
 
 BEGIN OF DISCLAIMER 
 
   THERE IS NO WARRANTY FOR THE PROGRAM, TO THE EXTENT PERMITTED BY
@@ -44,13 +44,13 @@
 
 This program is a mere software interface to existing video games, and cannot 
 work as a standalone application. As such, it requires the User to own software
 elements protected by copyright, and to interface them with it. 
 It is the case, for example, of Game ROMS required to execute the corresponding 
 Game-related Environment. In such cases, it is sole and only responsibility of 
 the User to comply with all the laws and regulations, and to make sure he has the 
-right to use such copyright-protected material. DIAMBRA members do not support 
+right to use such copyright-protected material. DIAMBRA, Inc. does not support 
 in any way piracy, and illegal distribution of copyright-protected material, 
-thus they will spend their maximum effort in avoiding illegal distribution of 
-such material, and are by no means responsible for copyright infringement.
+thus it will spend its maximum effort in avoiding illegal distribution of 
+such material, and is by no means responsible for copyright infringement.
 
 END OF DISCLAIMER
```

### Comparing `diambra-arena-2.1.0rc6/PKG-INFO` & `diambra-arena-2.1.0rc7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: diambra-arena
-Version: 2.1.0rc6
+Version: 2.1.0rc7
 Summary: DIAMBRA™ Arena. Built with OpenAI Gym Python interface, easy to use, transforms popular video games into Reinforcement Learning environments
 Home-page: https://github.com/diambra/arena
 Author: DIAMBRA Team
 Author-email: info@diambra.ai
 License: Custom
 Classifier: Development Status :: 3 - Alpha
 Classifier: Operating System :: OS Independent
@@ -256,8 +256,8 @@
  }
 ```
 
 ## Terms of Use
 
 DIAMBRA Arena software package is subject to our <a href="https://diambra.ai/terms" target="_blank">Terms of Use</a>. By using it, you accept them in full.
 
-###### DIAMBRA™ is a Trade Mark, © Copyright 2018-2023. All Rights Reserved.
+###### DIAMBRA, Inc. © Copyright 2018-2023. All Rights Reserved.
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: diambra-arena Version: 2.1.0rc6 Summary: DIAMBRAâ¢
+Metadata-Version: 2.1 Name: diambra-arena Version: 2.1.0rc7 Summary: DIAMBRAâ¢
 Arena. Built with OpenAI Gym Python interface, easy to use, transforms popular
 video games into Reinforcement Learning environments Home-page: https://
 github.com/diambra/arena Author: DIAMBRA Team Author-email: info@diambra.ai
 License: Custom Classifier: Development Status :: 3 - Alpha Classifier:
 Operating System :: OS Independent Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3 Classifier: Topic ::
 Scientific/Engineering :: Artificial Intelligence Classifier: Topic ::
@@ -153,9 +153,8 @@
 ```LaTex @article{Palmas22, author = {{Palmas}, Alessandro}, title = "{DIAMBRA
 Arena: a New Reinforcement Learning Platform for Research and
 Experimentation}", journal = {arXiv e-prints}, keywords = {reinforcement
 learning, transfer learning, multi-agent, games}, year = 2022, month = oct, eid
 = {arXiv:2210.10595}, pages = {arXiv:2210.10595}, archivePrefix = {arXiv},
 eprint = {2210.10595}, primaryClass = {cs.AI} } ``` ## Terms of Use DIAMBRA
 Arena software package is subject to our Terms_of_Use. By using it, you accept
-them in full. ###### DIAMBRAâ¢ is a Trade Mark, Â© Copyright 2018-2023. All
-Rights Reserved.
+them in full. ###### DIAMBRA, Inc. Â© Copyright 2018-2023. All Rights Reserved.
```

### Comparing `diambra-arena-2.1.0rc6/README.md` & `diambra-arena-2.1.0rc7/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -231,8 +231,8 @@
  }
 ```
 
 ## Terms of Use
 
 DIAMBRA Arena software package is subject to our <a href="https://diambra.ai/terms" target="_blank">Terms of Use</a>. By using it, you accept them in full.
 
-###### DIAMBRA™ is a Trade Mark, © Copyright 2018-2023. All Rights Reserved.
+###### DIAMBRA, Inc. © Copyright 2018-2023. All Rights Reserved.
```

#### html2text {}

```diff
@@ -141,9 +141,8 @@
 ```LaTex @article{Palmas22, author = {{Palmas}, Alessandro}, title = "{DIAMBRA
 Arena: a New Reinforcement Learning Platform for Research and
 Experimentation}", journal = {arXiv e-prints}, keywords = {reinforcement
 learning, transfer learning, multi-agent, games}, year = 2022, month = oct, eid
 = {arXiv:2210.10595}, pages = {arXiv:2210.10595}, archivePrefix = {arXiv},
 eprint = {2210.10595}, primaryClass = {cs.AI} } ``` ## Terms of Use DIAMBRA
 Arena software package is subject to our Terms_of_Use. By using it, you accept
-them in full. ###### DIAMBRAâ¢ is a Trade Mark, Â© Copyright 2018-2023. All
-Rights Reserved.
+them in full. ###### DIAMBRA, Inc. Â© Copyright 2018-2023. All Rights Reserved.
```

### Comparing `diambra-arena-2.1.0rc6/diambra/arena/arena_gym.py` & `diambra-arena-2.1.0rc7/diambra/arena/arena_gym.py`

 * *Files identical despite different names*

### Comparing `diambra-arena-2.1.0rc6/diambra/arena/arena_imitation_learning_gym.py` & `diambra-arena-2.1.0rc7/diambra/arena/arena_imitation_learning_gym.py`

 * *Files identical despite different names*

### Comparing `diambra-arena-2.1.0rc6/diambra/arena/engine/interface.py` & `diambra-arena-2.1.0rc7/diambra/arena/engine/interface.py`

 * *Files identical despite different names*

### Comparing `diambra-arena-2.1.0rc6/diambra/arena/env_settings.py` & `diambra-arena-2.1.0rc7/diambra/arena/env_settings.py`

 * *Files identical despite different names*

### Comparing `diambra-arena-2.1.0rc6/diambra/arena/make_env.py` & `diambra-arena-2.1.0rc7/diambra/arena/make_env.py`

 * *Files identical despite different names*

### Comparing `diambra-arena-2.1.0rc6/diambra/arena/ray_rllib/make_ray_env.py` & `diambra-arena-2.1.0rc7/diambra/arena/ray_rllib/make_ray_env.py`

 * *Files identical despite different names*

### Comparing `diambra-arena-2.1.0rc6/diambra/arena/stable_baselines/make_sb_env.py` & `diambra-arena-2.1.0rc7/diambra/arena/stable_baselines/make_sb_env.py`

 * *Files identical despite different names*

### Comparing `diambra-arena-2.1.0rc6/diambra/arena/stable_baselines/sb_utils.py` & `diambra-arena-2.1.0rc7/diambra/arena/stable_baselines/sb_utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from stable_baselines.common.callbacks import BaseCallback
 import cv2
 import os
 import time
 import json
 import numpy as np
+from pathlib import Path
 
 # Visualize Obs content
 
 
 def show_obs(observation, key_to_add, key_to_add_count, actions_stack,
              n_actions, wait_key, viz, char_list, hardcore, idx_list):
 
@@ -64,16 +65,14 @@
     num_add_par_p2 = int(observation[start_idx])
     add_par_p2 = observation[start_idx:start_idx + num_add_par_p2 + 1]
     observation[0:num_add_par_p2 + 1] = add_par_p2
     observation = np.reshape(observation, (shp[0], -1))
     return observation
 
 # Linear scheduler for RL agent parameters
-
-
 def linear_schedule(initial_value, final_value=0.0):
     """
     Linear learning rate schedule.
     :param initial_value: (float or str)
     :return: (function)
     """
     if isinstance(initial_value, str):
@@ -88,36 +87,36 @@
         :return: (float)
         """
         return final_value + progress * (initial_value - final_value)
 
     return func
 
 # AutoSave Callback
-
-
 class AutoSave(BaseCallback):
     """
     Callback for saving a model, it is saved every ``check_freq`` steps
 
     :param check_freq: (int)
     :param save_path: (str) Path to the folder where the model will be saved.
+    :filename_prefix: (str) Filename prefix
     :param verbose: (int)
     """
-    def __init__(self, check_freq: int, num_env: int, save_path: str, verbose=1):
+    def __init__(self, check_freq: int, num_envs: int, save_path: str, filename_prefix: str="", verbose: int=1):
         super(AutoSave, self).__init__(verbose)
-        self.check_freq = int(check_freq / num_env)
-        self.num_env = num_env
-        self.save_path_base = save_path + 'autoSave_'
+        self.check_freq = int(check_freq / num_envs)
+        self.num_envs = num_envs
+        self.save_path_base = Path(save_path)
+        self.filename = filename_prefix + "autosave_"
 
     def _on_step(self) -> bool:
         if self.n_calls % self.check_freq == 0:
             if self.verbose > 0:
                 print("Saving latest model to {}".format(self.save_path_base))
             # Save the agent
-            self.model.save(self.save_path_base + str(self.n_calls * self.num_env))
+            self.model.save(self.save_path_base / (self.filename + str(self.n_calls * self.num_envs)))
 
         return True
 
 # Update p2Brain model Callback
 
 
 class UpdateRLPolicyWeights(BaseCallback):
```

### Comparing `diambra-arena-2.1.0rc6/diambra/arena/stable_baselines/wrappers/add_obs_wrap.py` & `diambra-arena-2.1.0rc7/diambra/arena/stable_baselines/wrappers/add_obs_wrap.py`

 * *Files identical despite different names*

### Comparing `diambra-arena-2.1.0rc6/diambra/arena/stable_baselines/wrappers/p2_wrap.py` & `diambra-arena-2.1.0rc7/diambra/arena/stable_baselines/wrappers/p2_wrap.py`

 * *Files identical despite different names*

### Comparing `diambra-arena-2.1.0rc6/diambra/arena/stable_baselines/wrappers/tektag_rew_wrap.py` & `diambra-arena-2.1.0rc7/diambra/arena/stable_baselines/wrappers/tektag_rew_wrap.py`

 * *Files identical despite different names*

### Comparing `diambra-arena-2.1.0rc6/diambra/arena/stable_baselines3/make_sb3_env.py` & `diambra-arena-2.1.0rc7/diambra/arena/stable_baselines3/make_sb3_env.py`

 * *Files identical despite different names*

### Comparing `diambra-arena-2.1.0rc6/diambra/arena/utils/.splashScreen.gif` & `diambra-arena-2.1.0rc7/diambra/arena/utils/.splashScreen.gif`

 * *Files identical despite different names*

### Comparing `diambra-arena-2.1.0rc6/diambra/arena/utils/controller.py` & `diambra-arena-2.1.0rc7/diambra/arena/utils/controller.py`

 * *Files identical despite different names*

### Comparing `diambra-arena-2.1.0rc6/diambra/arena/utils/gym_utils.py` & `diambra-arena-2.1.0rc7/diambra/arena/utils/gym_utils.py`

 * *Files identical despite different names*

### Comparing `diambra-arena-2.1.0rc6/diambra/arena/utils/integratedGames.json` & `diambra-arena-2.1.0rc7/diambra/arena/utils/integratedGames.json`

 * *Files identical despite different names*

### Comparing `diambra-arena-2.1.0rc6/diambra/arena/utils/policies.py` & `diambra-arena-2.1.0rc7/diambra/arena/utils/policies.py`

 * *Files identical despite different names*

### Comparing `diambra-arena-2.1.0rc6/diambra/arena/utils/splash_screen.py` & `diambra-arena-2.1.0rc7/diambra/arena/utils/splash_screen.py`

 * *Files identical despite different names*

### Comparing `diambra-arena-2.1.0rc6/diambra/arena/wrappers/arena_wrappers.py` & `diambra-arena-2.1.0rc7/diambra/arena/wrappers/arena_wrappers.py`

 * *Files identical despite different names*

### Comparing `diambra-arena-2.1.0rc6/diambra/arena/wrappers/obs_wrapper.py` & `diambra-arena-2.1.0rc7/diambra/arena/wrappers/obs_wrapper.py`

 * *Files identical despite different names*

### Comparing `diambra-arena-2.1.0rc6/diambra/arena/wrappers/obs_wrapper_hardcore.py` & `diambra-arena-2.1.0rc7/diambra/arena/wrappers/obs_wrapper_hardcore.py`

 * *Files identical despite different names*

### Comparing `diambra-arena-2.1.0rc6/diambra/arena/wrappers/traj_rec_wrapper.py` & `diambra-arena-2.1.0rc7/diambra/arena/wrappers/traj_rec_wrapper.py`

 * *Files identical despite different names*

### Comparing `diambra-arena-2.1.0rc6/diambra/arena/wrappers/traj_rec_wrapper_hardcore.py` & `diambra-arena-2.1.0rc7/diambra/arena/wrappers/traj_rec_wrapper_hardcore.py`

 * *Files identical despite different names*

### Comparing `diambra-arena-2.1.0rc6/diambra_arena.egg-info/PKG-INFO` & `diambra-arena-2.1.0rc7/diambra_arena.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: diambra-arena
-Version: 2.1.0rc6
+Version: 2.1.0rc7
 Summary: DIAMBRA™ Arena. Built with OpenAI Gym Python interface, easy to use, transforms popular video games into Reinforcement Learning environments
 Home-page: https://github.com/diambra/arena
 Author: DIAMBRA Team
 Author-email: info@diambra.ai
 License: Custom
 Classifier: Development Status :: 3 - Alpha
 Classifier: Operating System :: OS Independent
@@ -256,8 +256,8 @@
  }
 ```
 
 ## Terms of Use
 
 DIAMBRA Arena software package is subject to our <a href="https://diambra.ai/terms" target="_blank">Terms of Use</a>. By using it, you accept them in full.
 
-###### DIAMBRA™ is a Trade Mark, © Copyright 2018-2023. All Rights Reserved.
+###### DIAMBRA, Inc. © Copyright 2018-2023. All Rights Reserved.
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: diambra-arena Version: 2.1.0rc6 Summary: DIAMBRAâ¢
+Metadata-Version: 2.1 Name: diambra-arena Version: 2.1.0rc7 Summary: DIAMBRAâ¢
 Arena. Built with OpenAI Gym Python interface, easy to use, transforms popular
 video games into Reinforcement Learning environments Home-page: https://
 github.com/diambra/arena Author: DIAMBRA Team Author-email: info@diambra.ai
 License: Custom Classifier: Development Status :: 3 - Alpha Classifier:
 Operating System :: OS Independent Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3 Classifier: Topic ::
 Scientific/Engineering :: Artificial Intelligence Classifier: Topic ::
@@ -153,9 +153,8 @@
 ```LaTex @article{Palmas22, author = {{Palmas}, Alessandro}, title = "{DIAMBRA
 Arena: a New Reinforcement Learning Platform for Research and
 Experimentation}", journal = {arXiv e-prints}, keywords = {reinforcement
 learning, transfer learning, multi-agent, games}, year = 2022, month = oct, eid
 = {arXiv:2210.10595}, pages = {arXiv:2210.10595}, archivePrefix = {arXiv},
 eprint = {2210.10595}, primaryClass = {cs.AI} } ``` ## Terms of Use DIAMBRA
 Arena software package is subject to our Terms_of_Use. By using it, you accept
-them in full. ###### DIAMBRAâ¢ is a Trade Mark, Â© Copyright 2018-2023. All
-Rights Reserved.
+them in full. ###### DIAMBRA, Inc. Â© Copyright 2018-2023. All Rights Reserved.
```

### Comparing `diambra-arena-2.1.0rc6/diambra_arena.egg-info/SOURCES.txt` & `diambra-arena-2.1.0rc7/diambra_arena.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `diambra-arena-2.1.0rc6/setup.py` & `diambra-arena-2.1.0rc7/setup.py`

 * *Files identical despite different names*

### Comparing `diambra-arena-2.1.0rc6/tests/test_gym_settings.py` & `diambra-arena-2.1.0rc7/tests/test_gym_settings.py`

 * *Files identical despite different names*

### Comparing `diambra-arena-2.1.0rc6/tests/test_imitation_learning.py` & `diambra-arena-2.1.0rc7/tests/test_imitation_learning.py`

 * *Files identical despite different names*

### Comparing `diambra-arena-2.1.0rc6/tests/test_integration.py` & `diambra-arena-2.1.0rc7/tests/test_integration.py`

 * *Files identical despite different names*

### Comparing `diambra-arena-2.1.0rc6/tests/test_random.py` & `diambra-arena-2.1.0rc7/tests/test_random.py`

 * *Files identical despite different names*

### Comparing `diambra-arena-2.1.0rc6/tests/test_recording_settings.py` & `diambra-arena-2.1.0rc7/tests/test_recording_settings.py`

 * *Files identical despite different names*

### Comparing `diambra-arena-2.1.0rc6/tests/test_speed.py` & `diambra-arena-2.1.0rc7/tests/test_speed.py`

 * *Files identical despite different names*

### Comparing `diambra-arena-2.1.0rc6/tests/test_wrappers_settings.py` & `diambra-arena-2.1.0rc7/tests/test_wrappers_settings.py`

 * *Files identical despite different names*

