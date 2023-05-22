# Comparing `tmp/cleanrl-1.1.0.tar.gz` & `tmp/cleanrl-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cleanrl-1.1.0.tar", max compression
+gzip compressed data, was "cleanrl-1.2.0.tar", max compression
```

## Comparing `cleanrl-1.1.0.tar` & `cleanrl-1.2.0.tar`

### file list

```diff
@@ -1,56 +1,56 @@
--rw-r--r--   0        0        0    14815 2022-08-22 02:00:00.815487 cleanrl-1.1.0/LICENSE
--rw-r--r--   0        0        0    13542 2023-01-04 20:11:32.885060 cleanrl-1.1.0/README.md
--rwxr-xr-x   0        0        0    12433 2023-01-04 20:06:20.974955 cleanrl-1.1.0/cleanrl/c51.py
--rwxr-xr-x   0        0        0    13178 2023-01-04 20:06:24.394978 cleanrl-1.1.0/cleanrl/c51_atari.py
--rw-r--r--   0        0        0    14234 2023-01-04 20:06:24.394978 cleanrl-1.1.0/cleanrl/c51_atari_jax.py
--rw-r--r--   0        0        0    13011 2023-01-04 20:06:24.394978 cleanrl-1.1.0/cleanrl/c51_jax.py
--rw-r--r--   0        0        0     1350 2022-09-14 02:53:34.472860 cleanrl-1.1.0/cleanrl/dd.py
--rw-r--r--   0        0        0    10312 2023-01-01 15:15:05.929174 cleanrl-1.1.0/cleanrl/ddpg_continuous_action.py
--rw-r--r--   0        0        0    11181 2023-01-01 15:15:05.929174 cleanrl-1.1.0/cleanrl/ddpg_continuous_action_jax.py
--rw-r--r--   0        0        0    10371 2023-01-04 20:06:20.978955 cleanrl-1.1.0/cleanrl/dqn.py
--rw-r--r--   0        0        0    11117 2023-01-04 20:06:20.978955 cleanrl-1.1.0/cleanrl/dqn_atari.py
--rw-r--r--   0        0        0    12185 2023-01-04 20:06:20.978955 cleanrl-1.1.0/cleanrl/dqn_atari_jax.py
--rw-r--r--   0        0        0    11080 2023-01-04 20:06:20.978955 cleanrl-1.1.0/cleanrl/dqn_jax.py
--rw-r--r--   0        0        0    23840 2022-10-05 19:12:38.666639 cleanrl-1.1.0/cleanrl/ppg_procgen.py
--rw-r--r--   0        0        0    14014 2023-01-01 15:12:56.352358 cleanrl-1.1.0/cleanrl/ppo.py
--rw-r--r--   0        0        0    14623 2022-12-21 03:41:15.349230 cleanrl-1.1.0/cleanrl/ppo_atari.py
--rw-r--r--   0        0        0    15392 2022-10-06 19:12:22.753906 cleanrl-1.1.0/cleanrl/ppo_atari_envpool.py
--rw-r--r--   0        0        0    19259 2022-10-06 19:12:22.753906 cleanrl-1.1.0/cleanrl/ppo_atari_envpool_xla_jax.py
--rw-r--r--   0        0        0    21797 2023-01-04 20:06:20.978955 cleanrl-1.1.0/cleanrl/ppo_atari_envpool_xla_jax_scan.py
--rw-r--r--   0        0        0    16725 2022-10-05 19:12:38.666639 cleanrl-1.1.0/cleanrl/ppo_atari_lstm.py
--rw-r--r--   0        0        0    17959 2022-11-09 02:56:21.142068 cleanrl-1.1.0/cleanrl/ppo_atari_multigpu.py
--rw-r--r--   0        0        0    15390 2023-01-01 15:15:13.537222 cleanrl-1.1.0/cleanrl/ppo_continuous_action.py
--rw-r--r--   0        0        0    41717 2022-10-05 19:12:38.666639 cleanrl-1.1.0/cleanrl/ppo_continuous_action_isaacgym/isaacgym/poetry.lock
--rw-r--r--   0        0        0      561 2023-01-01 15:15:13.537222 cleanrl-1.1.0/cleanrl/ppo_continuous_action_isaacgym/isaacgym/pyproject.toml
--rw-r--r--   0        0        0    18325 2022-10-05 19:12:38.666639 cleanrl-1.1.0/cleanrl/ppo_continuous_action_isaacgym/ppo_continuous_action_isaacgym.py
--rw-r--r--   0        0        0    14579 2022-10-05 19:12:38.666639 cleanrl-1.1.0/cleanrl/ppo_pettingzoo_ma_atari.py
--rw-r--r--   0        0        0    15830 2023-01-01 15:12:49.020312 cleanrl-1.1.0/cleanrl/ppo_procgen.py
--rw-r--r--   0        0        0    23642 2022-10-06 19:12:22.753906 cleanrl-1.1.0/cleanrl/ppo_rnd_envpool.py
--rw-r--r--   0        0        0    13911 2023-01-01 15:15:05.933174 cleanrl-1.1.0/cleanrl/sac_continuous_action.py
--rw-r--r--   0        0        0    11719 2023-01-01 15:15:05.933174 cleanrl-1.1.0/cleanrl/td3_continuous_action.py
--rw-r--r--   0        0        0    13080 2023-01-01 15:15:05.933174 cleanrl-1.1.0/cleanrl/td3_continuous_action_jax.py
--rw-r--r--   0        0        0       88 2022-11-05 17:08:35.390801 cleanrl-1.1.0/cleanrl/timm_app.py
--rw-r--r--   0        0        0        0 2021-09-18 15:33:51.963185 cleanrl-1.1.0/cleanrl_utils/__init__.py
--rw-r--r--   0        0        0      920 2022-07-04 01:09:13.204168 cleanrl-1.1.0/cleanrl_utils/add_header.py
--rw-r--r--   0        0        0     3406 2023-01-01 15:15:05.933174 cleanrl-1.1.0/cleanrl_utils/benchmark.py
--rw-r--r--   0        0        0    28128 2022-07-04 01:09:13.204168 cleanrl-1.1.0/cleanrl_utils/buffers.py
--rw-r--r--   0        0        0      286 2022-07-04 01:09:13.204168 cleanrl-1.1.0/cleanrl_utils/docker_build.py
--rwxr-xr-x   0        0        0     2915 2022-07-04 01:09:13.204168 cleanrl-1.1.0/cleanrl_utils/docker_queue.py
--rw-r--r--   0        0        0     1877 2023-01-04 20:06:20.978955 cleanrl-1.1.0/cleanrl_utils/enjoy.py
--rw-r--r--   0        0        0     2319 2023-01-04 20:06:24.394978 cleanrl-1.1.0/cleanrl_utils/evals/__init__.py
--rw-r--r--   0        0        0     1876 2023-01-04 20:06:20.978955 cleanrl-1.1.0/cleanrl_utils/evals/c51_eval.py
--rw-r--r--   0        0        0     2126 2023-01-04 20:06:20.978955 cleanrl-1.1.0/cleanrl_utils/evals/c51_jax_eval.py
--rw-r--r--   0        0        0     1696 2023-01-04 20:06:20.978955 cleanrl-1.1.0/cleanrl_utils/evals/dqn_eval.py
--rw-r--r--   0        0        0     1847 2023-01-04 20:06:20.978955 cleanrl-1.1.0/cleanrl_utils/evals/dqn_jax_eval.py
--rw-r--r--   0        0        0     3842 2023-01-04 20:06:20.978955 cleanrl-1.1.0/cleanrl_utils/evals/ppo_envpool_jax_eval.py
--rw-r--r--   0        0        0     4780 2023-01-04 20:06:20.978955 cleanrl-1.1.0/cleanrl_utils/huggingface.py
--rw-r--r--   0        0        0    13067 2022-07-04 01:09:13.204168 cleanrl-1.1.0/cleanrl_utils/paper_plot.py
--rw-r--r--   0        0        0    12337 2022-07-04 01:09:13.204168 cleanrl-1.1.0/cleanrl_utils/plot.py
--rw-r--r--   0        0        0    13614 2022-07-04 01:09:13.204168 cleanrl-1.1.0/cleanrl_utils/plot_individual.py
--rw-r--r--   0        0        0     1569 2022-07-04 01:09:13.204168 cleanrl-1.1.0/cleanrl_utils/reproduce.py
--rw-r--r--   0        0        0     4562 2022-07-04 01:09:13.204168 cleanrl-1.1.0/cleanrl_utils/resume.py
--rw-r--r--   0        0        0     5703 2022-07-04 01:09:13.204168 cleanrl-1.1.0/cleanrl_utils/submit_exp.py
--rw-r--r--   0        0        0     6147 2023-01-04 20:06:20.978955 cleanrl-1.1.0/cleanrl_utils/tuner.py
--rw-r--r--   0        0        0     5158 2023-01-04 20:14:28.346155 cleanrl-1.1.0/pyproject.toml
--rw-r--r--   0        0        0    17332 1970-01-01 00:00:00.000000 cleanrl-1.1.0/setup.py
--rw-r--r--   0        0        0    17529 1970-01-01 00:00:00.000000 cleanrl-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0    14815 2022-09-13 01:35:10.772194 cleanrl-1.2.0/LICENSE
+-rw-r--r--   0        0        0    14100 2023-05-22 01:45:25.925500 cleanrl-1.2.0/README.md
+-rwxr-xr-x   0        0        0    12439 2023-05-07 17:24:54.312034 cleanrl-1.2.0/cleanrl/c51.py
+-rwxr-xr-x   0        0        0    13184 2023-05-07 17:24:54.312034 cleanrl-1.2.0/cleanrl/c51_atari.py
+-rw-r--r--   0        0        0    14240 2023-05-07 17:24:54.312034 cleanrl-1.2.0/cleanrl/c51_atari_jax.py
+-rw-r--r--   0        0        0    13017 2023-05-07 17:24:54.312034 cleanrl-1.2.0/cleanrl/c51_jax.py
+-rw-r--r--   0        0        0    10684 2023-05-22 01:45:25.925500 cleanrl-1.2.0/cleanrl/ddpg_continuous_action.py
+-rw-r--r--   0        0        0    11543 2023-05-22 01:45:25.925500 cleanrl-1.2.0/cleanrl/ddpg_continuous_action_jax.py
+-rw-r--r--   0        0        0    11357 2023-05-07 17:24:54.312034 cleanrl-1.2.0/cleanrl/dqn.py
+-rw-r--r--   0        0        0    12167 2023-05-07 17:24:54.312034 cleanrl-1.2.0/cleanrl/dqn_atari.py
+-rw-r--r--   0        0        0    13072 2023-05-07 17:24:54.312034 cleanrl-1.2.0/cleanrl/dqn_atari_jax.py
+-rw-r--r--   0        0        0    11903 2023-05-07 17:24:54.312034 cleanrl-1.2.0/cleanrl/dqn_jax.py
+-rw-r--r--   0        0        0    23840 2023-05-07 17:24:54.312034 cleanrl-1.2.0/cleanrl/ppg_procgen.py
+-rw-r--r--   0        0        0    14013 2023-05-07 17:24:54.312034 cleanrl-1.2.0/cleanrl/ppo.py
+-rw-r--r--   0        0        0    14623 2023-05-07 17:24:54.312034 cleanrl-1.2.0/cleanrl/ppo_atari.py
+-rw-r--r--   0        0        0    15392 2023-05-07 17:24:54.312034 cleanrl-1.2.0/cleanrl/ppo_atari_envpool.py
+-rw-r--r--   0        0        0    19259 2023-05-07 17:24:54.312034 cleanrl-1.2.0/cleanrl/ppo_atari_envpool_xla_jax.py
+-rw-r--r--   0        0        0    21797 2023-05-07 17:24:54.316033 cleanrl-1.2.0/cleanrl/ppo_atari_envpool_xla_jax_scan.py
+-rw-r--r--   0        0        0    16725 2023-05-07 17:24:54.316033 cleanrl-1.2.0/cleanrl/ppo_atari_lstm.py
+-rw-r--r--   0        0        0    17959 2023-05-07 17:24:54.316033 cleanrl-1.2.0/cleanrl/ppo_atari_multigpu.py
+-rw-r--r--   0        0        0    15000 2023-05-22 01:45:25.925500 cleanrl-1.2.0/cleanrl/ppo_continuous_action.py
+-rw-r--r--   0        0        0    41711 2023-05-22 01:45:25.925500 cleanrl-1.2.0/cleanrl/ppo_continuous_action_isaacgym/isaacgym/poetry.lock
+-rw-r--r--   0        0        0      555 2023-05-22 01:45:25.925500 cleanrl-1.2.0/cleanrl/ppo_continuous_action_isaacgym/isaacgym/pyproject.toml
+-rw-r--r--   0        0        0    18325 2023-05-07 17:24:54.316033 cleanrl-1.2.0/cleanrl/ppo_continuous_action_isaacgym/ppo_continuous_action_isaacgym.py
+-rw-r--r--   0        0        0    14579 2023-05-07 17:24:54.316033 cleanrl-1.2.0/cleanrl/ppo_pettingzoo_ma_atari.py
+-rw-r--r--   0        0        0    15830 2023-05-07 17:24:54.316033 cleanrl-1.2.0/cleanrl/ppo_procgen.py
+-rw-r--r--   0        0        0    23642 2023-05-07 17:24:54.316033 cleanrl-1.2.0/cleanrl/ppo_rnd_envpool.py
+-rw-r--r--   0        0        0    15450 2023-05-22 01:45:25.925500 cleanrl-1.2.0/cleanrl/rpo_continuous_action.py
+-rw-r--r--   0        0        0    15266 2023-05-07 17:24:54.316033 cleanrl-1.2.0/cleanrl/sac_atari.py
+-rw-r--r--   0        0        0    13754 2023-05-22 01:45:25.925500 cleanrl-1.2.0/cleanrl/sac_continuous_action.py
+-rw-r--r--   0        0        0    11681 2023-05-22 01:45:25.925500 cleanrl-1.2.0/cleanrl/td3_continuous_action.py
+-rw-r--r--   0        0        0    13051 2023-05-22 01:45:25.925500 cleanrl-1.2.0/cleanrl/td3_continuous_action_jax.py
+-rw-r--r--   0        0        0        0 2022-09-13 01:35:10.776194 cleanrl-1.2.0/cleanrl_utils/__init__.py
+-rw-r--r--   0        0        0      920 2022-09-13 01:35:10.776194 cleanrl-1.2.0/cleanrl_utils/add_header.py
+-rw-r--r--   0        0        0     3406 2023-05-07 17:24:54.316033 cleanrl-1.2.0/cleanrl_utils/benchmark.py
+-rw-r--r--   0        0        0    28128 2022-09-13 01:35:10.776194 cleanrl-1.2.0/cleanrl_utils/buffers.py
+-rw-r--r--   0        0        0      286 2022-09-13 01:35:10.776194 cleanrl-1.2.0/cleanrl_utils/docker_build.py
+-rwxr-xr-x   0        0        0     2915 2022-09-13 01:35:10.776194 cleanrl-1.2.0/cleanrl_utils/docker_queue.py
+-rw-r--r--   0        0        0     1877 2023-05-07 17:24:54.316033 cleanrl-1.2.0/cleanrl_utils/enjoy.py
+-rw-r--r--   0        0        0     2319 2023-05-07 17:24:54.316033 cleanrl-1.2.0/cleanrl_utils/evals/__init__.py
+-rw-r--r--   0        0        0     1876 2023-05-07 17:24:54.316033 cleanrl-1.2.0/cleanrl_utils/evals/c51_eval.py
+-rw-r--r--   0        0        0     2126 2023-05-07 17:24:54.316033 cleanrl-1.2.0/cleanrl_utils/evals/c51_jax_eval.py
+-rw-r--r--   0        0        0     1797 2023-05-07 17:24:54.316033 cleanrl-1.2.0/cleanrl_utils/evals/dqn_eval.py
+-rw-r--r--   0        0        0     1948 2023-05-07 17:24:54.316033 cleanrl-1.2.0/cleanrl_utils/evals/dqn_jax_eval.py
+-rw-r--r--   0        0        0     3842 2023-05-07 17:24:54.316033 cleanrl-1.2.0/cleanrl_utils/evals/ppo_envpool_jax_eval.py
+-rw-r--r--   0        0        0     4780 2023-05-07 17:24:54.316033 cleanrl-1.2.0/cleanrl_utils/huggingface.py
+-rw-r--r--   0        0        0    13067 2022-09-13 01:35:10.776194 cleanrl-1.2.0/cleanrl_utils/paper_plot.py
+-rw-r--r--   0        0        0    12337 2022-09-13 01:35:10.776194 cleanrl-1.2.0/cleanrl_utils/plot.py
+-rw-r--r--   0        0        0    13614 2022-09-13 01:35:10.776194 cleanrl-1.2.0/cleanrl_utils/plot_individual.py
+-rw-r--r--   0        0        0     1569 2022-09-13 01:35:10.776194 cleanrl-1.2.0/cleanrl_utils/reproduce.py
+-rw-r--r--   0        0        0     4562 2022-09-13 01:35:10.776194 cleanrl-1.2.0/cleanrl_utils/resume.py
+-rw-r--r--   0        0        0     5703 2022-09-13 01:35:10.776194 cleanrl-1.2.0/cleanrl_utils/submit_exp.py
+-rw-r--r--   0        0        0     6147 2023-05-07 17:24:54.316033 cleanrl-1.2.0/cleanrl_utils/tuner.py
+-rw-r--r--   0        0        0     3484 2023-05-22 01:45:46.329632 cleanrl-1.2.0/pyproject.toml
+-rw-r--r--   0        0        0    17843 1970-01-01 00:00:00.000000 cleanrl-1.2.0/setup.py
+-rw-r--r--   0        0        0    18053 1970-01-01 00:00:00.000000 cleanrl-1.2.0/PKG-INFO
```

### Comparing `cleanrl-1.1.0/LICENSE` & `cleanrl-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cleanrl-1.1.0/README.md` & `cleanrl-1.2.0/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 [![tests](https://github.com/vwxyzjn/cleanrl/actions/workflows/tests.yaml/badge.svg)](https://github.com/vwxyzjn/cleanrl/actions/workflows/tests.yaml)
 [![docs](https://img.shields.io/github/deployments/vwxyzjn/cleanrl/Production?label=docs&logo=vercel)](https://docs.cleanrl.dev/)
 [<img src="https://img.shields.io/discord/767863440248143916?label=discord">](https://discord.gg/D6RCjA6sVT)
 [<img src="https://img.shields.io/youtube/channel/views/UCDdC6BIFRI0jvcwuhi3aI6w?style=social">](https://www.youtube.com/channel/UCDdC6BIFRI0jvcwuhi3aI6w/videos)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![Imports: isort](https://img.shields.io/badge/%20imports-isort-%231674b1?style=flat&labelColor=ef8336)](https://pycqa.github.io/isort/)
 [<img src="https://img.shields.io/badge/%F0%9F%A4%97%20Models-Huggingface-F8D521">](https://huggingface.co/cleanrl)
-[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/vwxyzjn/cleanrl/blob/hf-integration/docs/get-started/CleanRL_Huggingface_Integration_Demo.ipynb)
+[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/vwxyzjn/cleanrl/blob/master/docs/get-started/CleanRL_Huggingface_Integration_Demo.ipynb)
 
 
 CleanRL is a Deep Reinforcement Learning library that provides high-quality single-file implementation with research-friendly features. The implementation is clean and simple, yet we can scale it to run thousands of experiments using AWS Batch. The highlight features of CleanRL are:
 
 
 
 * 📜 Single-file implementation
@@ -26,24 +26,23 @@
 * 🧫 Experiment Management with [Weights and Biases](https://wandb.ai/site)
 * 💸 Cloud Integration with docker and AWS 
 
 You can read more about CleanRL in our [JMLR paper](https://www.jmlr.org/papers/volume23/21-1342/21-1342.pdf) and [documentation](https://docs.cleanrl.dev/).
 
 CleanRL only contains implementations of **online** deep reinforcement learning algorithms. If you are looking for **offline** algorithms, please check out [tinkoff-ai/CORL](https://github.com/tinkoff-ai/CORL), which shares a similar design philosophy as CleanRL.
 
-> ℹ️ **Support for Gymnasium**: [Farama-Foundation/Gymnasium](https://github.com/Farama-Foundation/Gymnasium) is the next generation of [`openai/gym`](https://github.com/openai/gym) that will continue to be maintained and introduce new features. Please see their [announcement](https://farama.org/Announcing-The-Farama-Foundation) for further detail. We are migrating to `gymnasium` and the progress can be tracked in [vwxyzjn/cleanrl#277](https://github.com/vwxyzjn/cleanrl/pull/277).
-
+> ℹ️ **Support for Gymnasium**: [Farama-Foundation/Gymnasium](https://github.com/Farama-Foundation/Gymnasium) is the next generation of [`openai/gym`](https://github.com/openai/gym) that will continue to be maintained and introduce new features. Please see their [announcement](https://farama.org/Announcing-The-Farama-Foundation) for further detail. We are migrating to `gymnasium` and the progress can be tracked in [vwxyzjn/cleanrl#277](https://github.com/vwxyzjn/cleanrl/pull/277). 
 
 
 > ⚠️ **NOTE**: CleanRL is *not* a modular library and therefore it is not meant to be imported. At the cost of duplicate code, we make all implementation details of a DRL algorithm variant easy to understand, so CleanRL comes with its own pros and cons. You should consider using CleanRL if you want to 1) understand all implementation details of an algorithm's varaint or 2) prototype advanced features that other modular DRL libraries do not support (CleanRL has minimal lines of code so it gives you great debugging experience and you don't have do a lot of subclassing like sometimes in modular DRL libraries).
 
 ## Get started
 
 Prerequisites:
-* Python >=3.7.1,<3.10 (not yet 3.10)
+* Python >=3.7.1,<3.11
 * [Poetry 1.2.1+](https://python-poetry.org)
 
 To run experiments locally, give the following a try:
 
 ```bash
 git clone https://github.com/vwxyzjn/cleanrl.git && cd cleanrl
 poetry install
@@ -66,50 +65,63 @@
     --seed 1 \
     --env-id CartPole-v0 \
     --total-timesteps 50000 \
     --track \
     --wandb-project-name cleanrltest
 ```
 
+If you are not using `poetry`, you can install CleanRL with `requirements.txt`:
+
+```bash
+# core dependencies
+pip install -r requirements/requirements.txt
+
+# optional dependencies
+pip install -r requirements/requirements-atari.txt
+pip install -r requirements/requirements-mujoco.txt
+pip install -r requirements/requirements-mujoco_py.txt
+pip install -r requirements/requirements-procgen.txt
+pip install -r requirements/requirements-envpool.txt
+pip install -r requirements/requirements-pettingzoo.txt
+pip install -r requirements/requirements-jax.txt
+pip install -r requirements/requirements-docs.txt
+pip install -r requirements/requirements-cloud.txt
+```
+
 To run training scripts in other games:
 ```
 poetry shell
 
 # classic control
 python cleanrl/dqn.py --env-id CartPole-v1
 python cleanrl/ppo.py --env-id CartPole-v1
 python cleanrl/c51.py --env-id CartPole-v1
 
 # atari
-poetry install --with atari
+poetry install -E atari
 python cleanrl/dqn_atari.py --env-id BreakoutNoFrameskip-v4
 python cleanrl/c51_atari.py --env-id BreakoutNoFrameskip-v4
 python cleanrl/ppo_atari.py --env-id BreakoutNoFrameskip-v4
+python cleanrl/sac_atari.py --env-id BreakoutNoFrameskip-v4
 
 # NEW: 3-4x side-effects free speed up with envpool's atari (only available to linux)
-poetry install --with envpool
+poetry install -E envpool
 python cleanrl/ppo_atari_envpool.py --env-id BreakoutNoFrameskip-v4
 # Learn Pong-v5 in ~5-10 mins
 # Side effects such as lower sample efficiency might occur
 poetry run python ppo_atari_envpool.py --clip-coef=0.2 --num-envs=16 --num-minibatches=8 --num-steps=128 --update-epochs=3
 
-# pybullet
-poetry install --with pybullet
-python cleanrl/td3_continuous_action.py --env-id MinitaurBulletDuckEnv-v0
-python cleanrl/ddpg_continuous_action.py --env-id MinitaurBulletDuckEnv-v0
-python cleanrl/sac_continuous_action.py --env-id MinitaurBulletDuckEnv-v0
-
 # procgen
-poetry install --with procgen
+poetry install -E procgen
 python cleanrl/ppo_procgen.py --env-id starpilot
 python cleanrl/ppg_procgen.py --env-id starpilot
 
 # ppo + lstm
+poetry install -E atari
 python cleanrl/ppo_atari_lstm.py --env-id BreakoutNoFrameskip-v4
-python cleanrl/ppo_memory_env_lstm.py
 ```
 
 You may also use a prebuilt development environment hosted in Gitpod:
 
 [![Open in Gitpod](https://gitpod.io/button/open-in-gitpod.svg)](https://gitpod.io/#https://github.com/vwxyzjn/cleanrl)
 
 ## Algorithms Implemented
@@ -125,22 +137,23 @@
 | | [`ppo_atari_envpool_xla_jax.py`](https://github.com/vwxyzjn/cleanrl/blob/master/cleanrl/ppo_atari_envpool_xla_jax.py), [docs](https://docs.cleanrl.dev/rl-algorithms/ppo/#ppo_atari_envpool_xla_jaxpy)
 | | [`ppo_atari_envpool_xla_jax_scan.py`](https://github.com/vwxyzjn/cleanrl/blob/master/cleanrl/ppo_atari_envpool_xla_jax_scan.py), [docs](https://docs.cleanrl.dev/rl-algorithms/ppo/#ppo_atari_envpool_xla_jax_scanpy))
 | |  [`ppo_procgen.py`](https://github.com/vwxyzjn/cleanrl/blob/master/cleanrl/ppo_procgen.py),   [docs](https://docs.cleanrl.dev/rl-algorithms/ppo/#ppo_procgenpy)
 | |  [`ppo_atari_multigpu.py`](https://github.com/vwxyzjn/cleanrl/blob/master/cleanrl/ppo_atari_multigpu.py),  [docs](https://docs.cleanrl.dev/rl-algorithms/ppo/#ppo_atari_multigpupy)
 | | [`ppo_pettingzoo_ma_atari.py`](https://github.com/vwxyzjn/cleanrl/blob/master/cleanrl/ppo_pettingzoo_ma_atari.py),  [docs](https://docs.cleanrl.dev/rl-algorithms/ppo/#ppo_pettingzoo_ma_ataripy)
 | | [`ppo_continuous_action_isaacgym.py`](https://github.com/vwxyzjn/cleanrl/blob/master/cleanrl/ppo_continuous_action_isaacgym/ppo_continuous_action_isaacgym.py),  [docs](https://docs.cleanrl.dev/rl-algorithms/ppo/#ppo_continuous_action_isaacgympy)
 | ✅ [Deep Q-Learning (DQN)](https://web.stanford.edu/class/psych209/Readings/MnihEtAlHassibis15NatureControlDeepRL.pdf) |  [`dqn.py`](https://github.com/vwxyzjn/cleanrl/blob/master/cleanrl/dqn.py),  [docs](https://docs.cleanrl.dev/rl-algorithms/dqn/#dqnpy) |
-| |  [`dqn_atari.py`](https://github.com/vwxyzjn/cleanrl/blob/master/cleanrl/dqn_atari.py),  [docs](https://docs.cleanrl.dev/rl-algorithms/dqn/#dqn_ataripy) |
+| | [`dqn_atari.py`](https://github.com/vwxyzjn/cleanrl/blob/master/cleanrl/dqn_atari.py),  [docs](https://docs.cleanrl.dev/rl-algorithms/dqn/#dqn_ataripy) |
 | | [`dqn_jax.py`](https://github.com/vwxyzjn/cleanrl/blob/master/cleanrl/dqn_jax.py), [docs](https://docs.cleanrl.dev/rl-algorithms/dqn/#dqn_jaxpy) |
 | | [`dqn_atari_jax.py`](https://github.com/vwxyzjn/cleanrl/blob/master/cleanrl/dqn_atari_jax.py), [docs](https://docs.cleanrl.dev/rl-algorithms/dqn/#dqn_atari_jaxpy) |
 | ✅ [Categorical DQN (C51)](https://arxiv.org/pdf/1707.06887.pdf) |  [`c51.py`](https://github.com/vwxyzjn/cleanrl/blob/master/cleanrl/c51.py),  [docs](https://docs.cleanrl.dev/rl-algorithms/c51/#c51py) |
 | |  [`c51_atari.py`](https://github.com/vwxyzjn/cleanrl/blob/master/cleanrl/c51_atari.py),  [docs](https://docs.cleanrl.dev/rl-algorithms/c51/#c51_ataripy) |
 | | [`c51_jax.py`](https://github.com/vwxyzjn/cleanrl/blob/master/cleanrl/c51_jax.py), [docs](https://docs.cleanrl.dev/rl-algorithms/c51/#c51_jaxpy) |
 | | [`c51_atari_jax.py`](https://github.com/vwxyzjn/cleanrl/blob/master/cleanrl/c51_atari_jax.py), [docs](https://docs.cleanrl.dev/rl-algorithms/c51/#c51_atari_jaxpy) |
 | ✅ [Soft Actor-Critic (SAC)](https://arxiv.org/pdf/1812.05905.pdf) |  [`sac_continuous_action.py`](https://github.com/vwxyzjn/cleanrl/blob/master/cleanrl/sac_continuous_action.py),  [docs](https://docs.cleanrl.dev/rl-algorithms/sac/#sac_continuous_actionpy) |
+| |  [`sac_atari.py`](https://github.com/vwxyzjn/cleanrl/blob/master/cleanrl/sac_atari.py),  [docs](https://docs.cleanrl.dev/rl-algorithms/sac/#sac_atarinpy) |
 | ✅ [Deep Deterministic Policy Gradient (DDPG)](https://arxiv.org/pdf/1509.02971.pdf) |  [`ddpg_continuous_action.py`](https://github.com/vwxyzjn/cleanrl/blob/master/cleanrl/ddpg_continuous_action.py),  [docs](https://docs.cleanrl.dev/rl-algorithms/ddpg/#ddpg_continuous_actionpy) |
 | | [`ddpg_continuous_action_jax.py`](https://github.com/vwxyzjn/cleanrl/blob/master/cleanrl/ddpg_continuous_action_jax.py),  [docs](https://docs.cleanrl.dev/rl-algorithms/ddpg/#ddpg_continuous_action_jaxpy)
 | ✅ [Twin Delayed Deep Deterministic Policy Gradient (TD3)](https://arxiv.org/pdf/1802.09477.pdf) |  [`td3_continuous_action.py`](https://github.com/vwxyzjn/cleanrl/blob/master/cleanrl/td3_continuous_action.py),  [docs](https://docs.cleanrl.dev/rl-algorithms/td3/#td3_continuous_actionpy) |
 |  | [`td3_continuous_action_jax.py`](https://github.com/vwxyzjn/cleanrl/blob/master/cleanrl/td3_continuous_action_jax.py),  [docs](https://docs.cleanrl.dev/rl-algorithms/td3/#td3_continuous_action_jaxpy) |
 | ✅ [Phasic Policy Gradient (PPG)](https://arxiv.org/abs/2009.04416) |  [`ppg_procgen.py`](https://github.com/vwxyzjn/cleanrl/blob/master/cleanrl/ppg_procgen.py),  [docs](https://docs.cleanrl.dev/rl-algorithms/ppg/#ppg_procgenpy) |
 | ✅ [Random Network Distillation (RND)](https://arxiv.org/abs/1810.12894) |  [`ppo_rnd_envpool.py`](https://github.com/vwxyzjn/cleanrl/blob/master/cleanrl/ppo_rnd_envpool.py),  [docs](/rl-algorithms/ppo-rnd/#ppo_rnd_envpoolpy) |
```

### Comparing `cleanrl-1.1.0/cleanrl/c51.py` & `cleanrl-1.2.0/cleanrl/c51.py`

 * *Files 1% similar despite different names*

```diff
@@ -46,17 +46,17 @@
     parser.add_argument("--total-timesteps", type=int, default=500000,
         help="total timesteps of the experiments")
     parser.add_argument("--learning-rate", type=float, default=2.5e-4,
         help="the learning rate of the optimizer")
     parser.add_argument("--n-atoms", type=int, default=101,
         help="the number of atoms")
     parser.add_argument("--v-min", type=float, default=-100,
-        help="the number of atoms")
+        help="the return lower bound")
     parser.add_argument("--v-max", type=float, default=100,
-        help="the number of atoms")
+        help="the return upper bound")
     parser.add_argument("--buffer-size", type=int, default=10000,
         help="the replay memory buffer size")
     parser.add_argument("--gamma", type=float, default=0.99,
         help="the discount factor gamma")
     parser.add_argument("--target-network-frequency", type=int, default=500,
         help="the timesteps it takes to update the target network")
     parser.add_argument("--batch-size", type=int, default=128,
```

### Comparing `cleanrl-1.1.0/cleanrl/c51_atari.py` & `cleanrl-1.2.0/cleanrl/c51_atari.py`

 * *Files 1% similar despite different names*

```diff
@@ -53,17 +53,17 @@
     parser.add_argument("--total-timesteps", type=int, default=10000000,
         help="total timesteps of the experiments")
     parser.add_argument("--learning-rate", type=float, default=2.5e-4,
         help="the learning rate of the optimizer")
     parser.add_argument("--n-atoms", type=int, default=51,
         help="the number of atoms")
     parser.add_argument("--v-min", type=float, default=-10,
-        help="the number of atoms")
+        help="the return lower bound")
     parser.add_argument("--v-max", type=float, default=10,
-        help="the number of atoms")
+        help="the return upper bound")
     parser.add_argument("--buffer-size", type=int, default=1000000,
         help="the replay memory buffer size")
     parser.add_argument("--gamma", type=float, default=0.99,
         help="the discount factor gamma")
     parser.add_argument("--target-network-frequency", type=int, default=10000,
         help="the timesteps it takes to update the target network")
     parser.add_argument("--batch-size", type=int, default=32,
```

### Comparing `cleanrl-1.1.0/cleanrl/c51_atari_jax.py` & `cleanrl-1.2.0/cleanrl/c51_atari_jax.py`

 * *Files 1% similar despite different names*

```diff
@@ -56,17 +56,17 @@
     parser.add_argument("--total-timesteps", type=int, default=10000000,
         help="total timesteps of the experiments")
     parser.add_argument("--learning-rate", type=float, default=2.5e-4,
         help="the learning rate of the optimizer")
     parser.add_argument("--n-atoms", type=int, default=51,
         help="the number of atoms")
     parser.add_argument("--v-min", type=float, default=-10,
-        help="the number of atoms")
+        help="the return lower bound")
     parser.add_argument("--v-max", type=float, default=10,
-        help="the number of atoms")
+        help="the return upper bound")
     parser.add_argument("--buffer-size", type=int, default=1000000,
         help="the replay memory buffer size")
     parser.add_argument("--gamma", type=float, default=0.99,
         help="the discount factor gamma")
     parser.add_argument("--target-network-frequency", type=int, default=10000,
         help="the timesteps it takes to update the target network")
     parser.add_argument("--batch-size", type=int, default=32,
```

### Comparing `cleanrl-1.1.0/cleanrl/c51_jax.py` & `cleanrl-1.2.0/cleanrl/c51_jax.py`

 * *Files 3% similar despite different names*

```diff
@@ -45,17 +45,17 @@
     parser.add_argument("--total-timesteps", type=int, default=500000,
         help="total timesteps of the experiments")
     parser.add_argument("--learning-rate", type=float, default=2.5e-4,
         help="the learning rate of the optimizer")
     parser.add_argument("--n-atoms", type=int, default=101,
         help="the number of atoms")
     parser.add_argument("--v-min", type=float, default=-100,
-        help="the number of atoms")
+        help="the return lower bound")
     parser.add_argument("--v-max", type=float, default=100,
-        help="the number of atoms")
+        help="the return upper bound")
     parser.add_argument("--buffer-size", type=int, default=10000,
         help="the replay memory buffer size")
     parser.add_argument("--gamma", type=float, default=0.99,
         help="the discount factor gamma")
     parser.add_argument("--target-network-frequency", type=int, default=500,
         help="the timesteps it takes to update the target network")
     parser.add_argument("--batch-size", type=int, default=128,
```

### Comparing `cleanrl-1.1.0/cleanrl/ddpg_continuous_action.py` & `cleanrl-1.2.0/cleanrl/ddpg_continuous_action.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 # docs and experiment results can be found at https://docs.cleanrl.dev/rl-algorithms/ddpg/#ddpg_continuous_actionpy
 import argparse
 import os
 import random
 import time
 from distutils.util import strtobool
 
-import gym
+import gymnasium as gym
 import numpy as np
-import pybullet_envs  # noqa
 import torch
 import torch.nn as nn
 import torch.nn.functional as F
 import torch.optim as optim
 from stable_baselines3.common.buffers import ReplayBuffer
 from torch.utils.tensorboard import SummaryWriter
 
@@ -33,15 +32,15 @@
         help="the wandb's project name")
     parser.add_argument("--wandb-entity", type=str, default=None,
         help="the entity (team) of wandb's project")
     parser.add_argument("--capture-video", type=lambda x: bool(strtobool(x)), default=False, nargs="?", const=True,
         help="whether to capture videos of the agent performances (check out `videos` folder)")
 
     # Algorithm specific arguments
-    parser.add_argument("--env-id", type=str, default="HopperBulletEnv-v0",
+    parser.add_argument("--env-id", type=str, default="HalfCheetah-v4",
         help="the id of the environment")
     parser.add_argument("--total-timesteps", type=int, default=1000000,
         help="total timesteps of the experiments")
     parser.add_argument("--learning-rate", type=float, default=3e-4,
         help="the learning rate of the optimizer")
     parser.add_argument("--buffer-size", type=int, default=int(1e6),
         help="the replay memory buffer size")
@@ -62,20 +61,22 @@
     args = parser.parse_args()
     # fmt: on
     return args
 
 
 def make_env(env_id, seed, idx, capture_video, run_name):
     def thunk():
-        env = gym.make(env_id)
+        if capture_video:
+            env = gym.make(env_id, render_mode="rgb_array")
+        else:
+            env = gym.make(env_id)
         env = gym.wrappers.RecordEpisodeStatistics(env)
         if capture_video:
             if idx == 0:
                 env = gym.wrappers.RecordVideo(env, f"videos/{run_name}")
-        env.seed(seed)
         env.action_space.seed(seed)
         env.observation_space.seed(seed)
         return env
 
     return thunk
 
 
@@ -113,14 +114,23 @@
         x = F.relu(self.fc1(x))
         x = F.relu(self.fc2(x))
         x = torch.tanh(self.fc_mu(x))
         return x * self.action_scale + self.action_bias
 
 
 if __name__ == "__main__":
+    import stable_baselines3 as sb3
+
+    if sb3.__version__ < "2.0":
+        raise ValueError(
+            """Ongoing migration: run the following command to install the new dependencies:
+
+poetry run pip install "stable_baselines3==2.0.0a1"
+"""
+        )
     args = parse_args()
     run_name = f"{args.env_id}__{args.exp_name}__{args.seed}__{int(time.time())}"
     if args.track:
         import wandb
 
         wandb.init(
             project=args.wandb_project_name,
@@ -160,47 +170,48 @@
 
     envs.single_observation_space.dtype = np.float32
     rb = ReplayBuffer(
         args.buffer_size,
         envs.single_observation_space,
         envs.single_action_space,
         device,
-        handle_timeout_termination=True,
+        handle_timeout_termination=False,
     )
     start_time = time.time()
 
     # TRY NOT TO MODIFY: start the game
-    obs = envs.reset()
+    obs, _ = envs.reset(seed=args.seed)
     for global_step in range(args.total_timesteps):
         # ALGO LOGIC: put action logic here
         if global_step < args.learning_starts:
             actions = np.array([envs.single_action_space.sample() for _ in range(envs.num_envs)])
         else:
             with torch.no_grad():
                 actions = actor(torch.Tensor(obs).to(device))
                 actions += torch.normal(0, actor.action_scale * args.exploration_noise)
                 actions = actions.cpu().numpy().clip(envs.single_action_space.low, envs.single_action_space.high)
 
         # TRY NOT TO MODIFY: execute the game and log data.
-        next_obs, rewards, dones, infos = envs.step(actions)
+        next_obs, rewards, terminateds, truncateds, infos = envs.step(actions)
 
         # TRY NOT TO MODIFY: record rewards for plotting purposes
-        for info in infos:
-            if "episode" in info.keys():
+
+        if "final_info" in infos:
+            for info in infos["final_info"]:
                 print(f"global_step={global_step}, episodic_return={info['episode']['r']}")
                 writer.add_scalar("charts/episodic_return", info["episode"]["r"], global_step)
                 writer.add_scalar("charts/episodic_length", info["episode"]["l"], global_step)
                 break
 
         # TRY NOT TO MODIFY: save data to reply buffer; handle `terminal_observation`
         real_next_obs = next_obs.copy()
-        for idx, d in enumerate(dones):
+        for idx, d in enumerate(truncateds):
             if d:
-                real_next_obs[idx] = infos[idx]["terminal_observation"]
-        rb.add(obs, real_next_obs, actions, rewards, dones, infos)
+                real_next_obs[idx] = infos["final_observation"][idx]
+        rb.add(obs, real_next_obs, actions, rewards, terminateds, infos)
 
         # TRY NOT TO MODIFY: CRUCIAL step easy to overlook
         obs = next_obs
 
         # ALGO LOGIC: training.
         if global_step > args.learning_starts:
             data = rb.sample(args.batch_size)
```

### Comparing `cleanrl-1.1.0/cleanrl/ddpg_continuous_action_jax.py` & `cleanrl-1.2.0/cleanrl/td3_continuous_action_jax.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,23 +1,22 @@
-# docs and experiment results can be found at https://docs.cleanrl.dev/rl-algorithms/ddpg/#ddpg_continuous_action_jaxpy
+# docs and experiment results can be found at https://docs.cleanrl.dev/rl-algorithms/td3/#td3_continuous_action_jaxpy
 import argparse
 import os
 import random
 import time
 from distutils.util import strtobool
 from typing import Sequence
 
 import flax
 import flax.linen as nn
 import gym
 import jax
 import jax.numpy as jnp
 import numpy as np
 import optax
-import pybullet_envs  # noqa
 from flax.training.train_state import TrainState
 from stable_baselines3.common.buffers import ReplayBuffer
 from torch.utils.tensorboard import SummaryWriter
 
 
 def parse_args():
     # fmt: off
@@ -44,14 +43,16 @@
         help="the learning rate of the optimizer")
     parser.add_argument("--buffer-size", type=int, default=int(1e6),
         help="the replay memory buffer size")
     parser.add_argument("--gamma", type=float, default=0.99,
         help="the discount factor gamma")
     parser.add_argument("--tau", type=float, default=0.005,
         help="target smoothing coefficient (default: 0.005)")
+    parser.add_argument("--policy-noise", type=float, default=0.2,
+        help="the scale of policy noise")
     parser.add_argument("--batch-size", type=int, default=256,
         help="the batch size of sample from the reply memory")
     parser.add_argument("--exploration-noise", type=float, default=0.1,
         help="the scale of exploration noise")
     parser.add_argument("--learning-starts", type=int, default=25e3,
         help="timestep to start learning")
     parser.add_argument("--policy-frequency", type=int, default=2,
@@ -133,15 +134,15 @@
         "|param|value|\n|-|-|\n%s" % ("\n".join([f"|{key}|{value}|" for key, value in vars(args).items()])),
     )
 
     # TRY NOT TO MODIFY: seeding
     random.seed(args.seed)
     np.random.seed(args.seed)
     key = jax.random.PRNGKey(args.seed)
-    key, actor_key, qf1_key = jax.random.split(key, 3)
+    key, actor_key, qf1_key, qf2_key = jax.random.split(key, 4)
 
     # env setup
     envs = gym.vector.SyncVectorEnv([make_env(args.env_id, args.seed, 0, args.capture_video, run_name)])
     assert isinstance(envs.single_action_space, gym.spaces.Box), "only continuous action space is supported"
 
     max_action = float(envs.single_action_space.high[0])
     envs.single_observation_space.dtype = np.float32
@@ -151,135 +152,173 @@
         envs.single_action_space,
         device="cpu",
         handle_timeout_termination=True,
     )
 
     # TRY NOT TO MODIFY: start the game
     obs = envs.reset()
-    action_scale = np.array((envs.action_space.high - envs.action_space.low) / 2.0)
-    action_bias = np.array((envs.action_space.high + envs.action_space.low) / 2.0)
     actor = Actor(
         action_dim=np.prod(envs.single_action_space.shape),
-        action_scale=action_scale,
-        action_bias=action_bias,
+        action_scale=jnp.array((envs.action_space.high - envs.action_space.low) / 2.0),
+        action_bias=jnp.array((envs.action_space.high + envs.action_space.low) / 2.0),
     )
-    qf1 = QNetwork()
     actor_state = TrainState.create(
         apply_fn=actor.apply,
         params=actor.init(actor_key, obs),
         target_params=actor.init(actor_key, obs),
         tx=optax.adam(learning_rate=args.learning_rate),
     )
+    qf = QNetwork()
     qf1_state = TrainState.create(
-        apply_fn=qf1.apply,
-        params=qf1.init(qf1_key, obs, envs.action_space.sample()),
-        target_params=qf1.init(qf1_key, obs, envs.action_space.sample()),
+        apply_fn=qf.apply,
+        params=qf.init(qf1_key, obs, envs.action_space.sample()),
+        target_params=qf.init(qf1_key, obs, envs.action_space.sample()),
+        tx=optax.adam(learning_rate=args.learning_rate),
+    )
+    qf2_state = TrainState.create(
+        apply_fn=qf.apply,
+        params=qf.init(qf2_key, obs, envs.action_space.sample()),
+        target_params=qf.init(qf2_key, obs, envs.action_space.sample()),
         tx=optax.adam(learning_rate=args.learning_rate),
     )
     actor.apply = jax.jit(actor.apply)
-    qf1.apply = jax.jit(qf1.apply)
+    qf.apply = jax.jit(qf.apply)
 
     @jax.jit
     def update_critic(
         actor_state: TrainState,
         qf1_state: TrainState,
+        qf2_state: TrainState,
         observations: np.ndarray,
         actions: np.ndarray,
         next_observations: np.ndarray,
         rewards: np.ndarray,
         dones: np.ndarray,
+        key: jnp.ndarray,
     ):
-        next_state_actions = (actor.apply(actor_state.target_params, next_observations)).clip(-1, 1)  # TODO: proper clip
-        qf1_next_target = qf1.apply(qf1_state.target_params, next_observations, next_state_actions).reshape(-1)
-        next_q_value = (rewards + (1 - dones) * args.gamma * (qf1_next_target)).reshape(-1)
+        # TODO Maybe pre-generate a lot of random keys
+        # also check https://jax.readthedocs.io/en/latest/jax.random.html
+        key, noise_key = jax.random.split(key, 2)
+        clipped_noise = (
+            jnp.clip(
+                (jax.random.normal(noise_key, actions.shape) * args.policy_noise),
+                -args.noise_clip,
+                args.noise_clip,
+            )
+            * actor.action_scale
+        )
+        next_state_actions = jnp.clip(
+            actor.apply(actor_state.target_params, next_observations) + clipped_noise,
+            envs.single_action_space.low[0],
+            envs.single_action_space.high[0],
+        )
+        qf1_next_target = qf.apply(qf1_state.target_params, next_observations, next_state_actions).reshape(-1)
+        qf2_next_target = qf.apply(qf2_state.target_params, next_observations, next_state_actions).reshape(-1)
+        min_qf_next_target = jnp.minimum(qf1_next_target, qf2_next_target)
+        next_q_value = (rewards + (1 - dones) * args.gamma * (min_qf_next_target)).reshape(-1)
 
         def mse_loss(params):
-            qf1_a_values = qf1.apply(params, observations, actions).squeeze()
-            return ((qf1_a_values - next_q_value) ** 2).mean(), qf1_a_values.mean()
+            qf_a_values = qf.apply(params, observations, actions).squeeze()
+            return ((qf_a_values - next_q_value) ** 2).mean(), qf_a_values.mean()
+
+        (qf1_loss_value, qf1_a_values), grads1 = jax.value_and_grad(mse_loss, has_aux=True)(qf1_state.params)
+        (qf2_loss_value, qf2_a_values), grads2 = jax.value_and_grad(mse_loss, has_aux=True)(qf2_state.params)
+        qf1_state = qf1_state.apply_gradients(grads=grads1)
+        qf2_state = qf2_state.apply_gradients(grads=grads2)
 
-        (qf1_loss_value, qf1_a_values), grads = jax.value_and_grad(mse_loss, has_aux=True)(qf1_state.params)
-        qf1_state = qf1_state.apply_gradients(grads=grads)
-        return qf1_state, qf1_loss_value, qf1_a_values
+        return (qf1_state, qf2_state), (qf1_loss_value, qf2_loss_value), (qf1_a_values, qf2_a_values), key
 
     @jax.jit
     def update_actor(
         actor_state: TrainState,
         qf1_state: TrainState,
+        qf2_state: TrainState,
         observations: np.ndarray,
     ):
         def actor_loss(params):
-            return -qf1.apply(qf1_state.params, observations, actor.apply(params, observations)).mean()
+            return -qf.apply(qf1_state.params, observations, actor.apply(params, observations)).mean()
 
         actor_loss_value, grads = jax.value_and_grad(actor_loss)(actor_state.params)
         actor_state = actor_state.apply_gradients(grads=grads)
         actor_state = actor_state.replace(
             target_params=optax.incremental_update(actor_state.params, actor_state.target_params, args.tau)
         )
+
         qf1_state = qf1_state.replace(
             target_params=optax.incremental_update(qf1_state.params, qf1_state.target_params, args.tau)
         )
-        return actor_state, qf1_state, actor_loss_value
+        qf2_state = qf2_state.replace(
+            target_params=optax.incremental_update(qf2_state.params, qf2_state.target_params, args.tau)
+        )
+        return actor_state, (qf1_state, qf2_state), actor_loss_value
 
     start_time = time.time()
     for global_step in range(args.total_timesteps):
         # ALGO LOGIC: put action logic here
         if global_step < args.learning_starts:
             actions = np.array([envs.single_action_space.sample() for _ in range(envs.num_envs)])
         else:
             actions = actor.apply(actor_state.params, obs)
             actions = np.array(
                 [
-                    (jax.device_get(actions)[0] + np.random.normal(0, action_scale * args.exploration_noise)[0]).clip(
-                        envs.single_action_space.low, envs.single_action_space.high
-                    )
+                    (
+                        jax.device_get(actions)[0]
+                        + np.random.normal(0, max_action * args.exploration_noise, size=envs.single_action_space.shape[0])
+                    ).clip(envs.single_action_space.low, envs.single_action_space.high)
                 ]
             )
 
         # TRY NOT TO MODIFY: execute the game and log data.
         next_obs, rewards, dones, infos = envs.step(actions)
 
         # TRY NOT TO MODIFY: record rewards for plotting purposes
         for info in infos:
             if "episode" in info.keys():
                 print(f"global_step={global_step}, episodic_return={info['episode']['r']}")
                 writer.add_scalar("charts/episodic_return", info["episode"]["r"], global_step)
                 writer.add_scalar("charts/episodic_length", info["episode"]["l"], global_step)
                 break
 
-        # TRY NOT TO MODIFY: save data to reply buffer; handle `terminal_observation`
+        # TRY NOT TO MODIFY: save data to replay buffer; handle `terminal_observation`
         real_next_obs = next_obs.copy()
         for idx, d in enumerate(dones):
             if d:
                 real_next_obs[idx] = infos[idx]["terminal_observation"]
         rb.add(obs, real_next_obs, actions, rewards, dones, infos)
 
         # TRY NOT TO MODIFY: CRUCIAL step easy to overlook
         obs = next_obs
 
         # ALGO LOGIC: training.
         if global_step > args.learning_starts:
             data = rb.sample(args.batch_size)
-            qf1_state, qf1_loss_value, qf1_a_values = update_critic(
+
+            (qf1_state, qf2_state), (qf1_loss_value, qf2_loss_value), (qf1_a_values, qf2_a_values), key = update_critic(
                 actor_state,
                 qf1_state,
+                qf2_state,
                 data.observations.numpy(),
                 data.actions.numpy(),
                 data.next_observations.numpy(),
                 data.rewards.flatten().numpy(),
                 data.dones.flatten().numpy(),
+                key,
             )
+
             if global_step % args.policy_frequency == 0:
-                actor_state, qf1_state, actor_loss_value = update_actor(
+                actor_state, (qf1_state, qf2_state), actor_loss_value = update_actor(
                     actor_state,
                     qf1_state,
+                    qf2_state,
                     data.observations.numpy(),
                 )
-
             if global_step % 100 == 0:
                 writer.add_scalar("losses/qf1_loss", qf1_loss_value.item(), global_step)
-                writer.add_scalar("losses/actor_loss", actor_loss_value.item(), global_step)
+                writer.add_scalar("losses/qf2_loss", qf2_loss_value.item(), global_step)
                 writer.add_scalar("losses/qf1_values", qf1_a_values.item(), global_step)
+                writer.add_scalar("losses/qf2_values", qf2_a_values.item(), global_step)
+                writer.add_scalar("losses/actor_loss", actor_loss_value.item(), global_step)
                 print("SPS:", int(global_step / (time.time() - start_time)))
                 writer.add_scalar("charts/SPS", int(global_step / (time.time() - start_time)), global_step)
 
     envs.close()
     writer.close()
```

### Comparing `cleanrl-1.1.0/cleanrl/dqn.py` & `cleanrl-1.2.0/cleanrl/dqn.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # docs and experiment results can be found at https://docs.cleanrl.dev/rl-algorithms/dqn/#dqnpy
 import argparse
 import os
 import random
 import time
 from distutils.util import strtobool
 
-import gym
+import gymnasium as gym
 import numpy as np
 import torch
 import torch.nn as nn
 import torch.nn.functional as F
 import torch.optim as optim
 from stable_baselines3.common.buffers import ReplayBuffer
 from torch.utils.tensorboard import SummaryWriter
@@ -44,18 +44,22 @@
     # Algorithm specific arguments
     parser.add_argument("--env-id", type=str, default="CartPole-v1",
         help="the id of the environment")
     parser.add_argument("--total-timesteps", type=int, default=500000,
         help="total timesteps of the experiments")
     parser.add_argument("--learning-rate", type=float, default=2.5e-4,
         help="the learning rate of the optimizer")
+    parser.add_argument("--num-envs", type=int, default=1,
+        help="the number of parallel game environments")
     parser.add_argument("--buffer-size", type=int, default=10000,
         help="the replay memory buffer size")
     parser.add_argument("--gamma", type=float, default=0.99,
         help="the discount factor gamma")
+    parser.add_argument("--tau", type=float, default=1.,
+        help="the target network update rate")
     parser.add_argument("--target-network-frequency", type=int, default=500,
         help="the timesteps it takes to update the target network")
     parser.add_argument("--batch-size", type=int, default=128,
         help="the batch size of sample from the reply memory")
     parser.add_argument("--start-e", type=float, default=1,
         help="the starting epsilon for exploration")
     parser.add_argument("--end-e", type=float, default=0.05,
@@ -64,27 +68,29 @@
         help="the fraction of `total-timesteps` it takes from start-e to go end-e")
     parser.add_argument("--learning-starts", type=int, default=10000,
         help="timestep to start learning")
     parser.add_argument("--train-frequency", type=int, default=10,
         help="the frequency of training")
     args = parser.parse_args()
     # fmt: on
+    assert args.num_envs == 1, "vectorized envs are not supported at the moment"
+
     return args
 
 
 def make_env(env_id, seed, idx, capture_video, run_name):
     def thunk():
-        env = gym.make(env_id)
+        if capture_video and idx == 0:
+            env = gym.make(env_id, render_mode="rgb_array")
+            env = gym.wrappers.RecordVideo(env, f"videos/{run_name}")
+        else:
+            env = gym.make(env_id)
         env = gym.wrappers.RecordEpisodeStatistics(env)
-        if capture_video:
-            if idx == 0:
-                env = gym.wrappers.RecordVideo(env, f"videos/{run_name}")
-        env.seed(seed)
         env.action_space.seed(seed)
-        env.observation_space.seed(seed)
+
         return env
 
     return thunk
 
 
 # ALGO LOGIC: initialize agent here:
 class QNetwork(nn.Module):
@@ -104,14 +110,23 @@
 
 def linear_schedule(start_e: float, end_e: float, duration: int, t: int):
     slope = (end_e - start_e) / duration
     return max(slope * t + start_e, end_e)
 
 
 if __name__ == "__main__":
+    import stable_baselines3 as sb3
+
+    if sb3.__version__ < "2.0":
+        raise ValueError(
+            """Ongoing migration: run the following command to install the new dependencies:
+
+poetry run pip install "stable_baselines3==2.0.0a1"
+"""
+        )
     args = parse_args()
     run_name = f"{args.env_id}__{args.exp_name}__{args.seed}__{int(time.time())}"
     if args.track:
         import wandb
 
         wandb.init(
             project=args.wandb_project_name,
@@ -133,60 +148,64 @@
     np.random.seed(args.seed)
     torch.manual_seed(args.seed)
     torch.backends.cudnn.deterministic = args.torch_deterministic
 
     device = torch.device("cuda" if torch.cuda.is_available() and args.cuda else "cpu")
 
     # env setup
-    envs = gym.vector.SyncVectorEnv([make_env(args.env_id, args.seed, 0, args.capture_video, run_name)])
+    envs = gym.vector.SyncVectorEnv(
+        [make_env(args.env_id, args.seed + i, i, args.capture_video, run_name) for i in range(args.num_envs)]
+    )
     assert isinstance(envs.single_action_space, gym.spaces.Discrete), "only discrete action space is supported"
 
     q_network = QNetwork(envs).to(device)
     optimizer = optim.Adam(q_network.parameters(), lr=args.learning_rate)
     target_network = QNetwork(envs).to(device)
     target_network.load_state_dict(q_network.state_dict())
 
     rb = ReplayBuffer(
         args.buffer_size,
         envs.single_observation_space,
         envs.single_action_space,
         device,
-        handle_timeout_termination=True,
+        handle_timeout_termination=False,
     )
     start_time = time.time()
 
     # TRY NOT TO MODIFY: start the game
-    obs = envs.reset()
+    obs, _ = envs.reset(seed=args.seed)
     for global_step in range(args.total_timesteps):
         # ALGO LOGIC: put action logic here
         epsilon = linear_schedule(args.start_e, args.end_e, args.exploration_fraction * args.total_timesteps, global_step)
         if random.random() < epsilon:
             actions = np.array([envs.single_action_space.sample() for _ in range(envs.num_envs)])
         else:
             q_values = q_network(torch.Tensor(obs).to(device))
             actions = torch.argmax(q_values, dim=1).cpu().numpy()
 
         # TRY NOT TO MODIFY: execute the game and log data.
-        next_obs, rewards, dones, infos = envs.step(actions)
+        next_obs, rewards, terminated, truncated, infos = envs.step(actions)
 
         # TRY NOT TO MODIFY: record rewards for plotting purposes
-        for info in infos:
-            if "episode" in info.keys():
+        if "final_info" in infos:
+            for info in infos["final_info"]:
+                # Skip the envs that are not done
+                if "episode" not in info:
+                    continue
                 print(f"global_step={global_step}, episodic_return={info['episode']['r']}")
                 writer.add_scalar("charts/episodic_return", info["episode"]["r"], global_step)
                 writer.add_scalar("charts/episodic_length", info["episode"]["l"], global_step)
                 writer.add_scalar("charts/epsilon", epsilon, global_step)
-                break
 
-        # TRY NOT TO MODIFY: save data to reply buffer; handle `terminal_observation`
+        # TRY NOT TO MODIFY: save data to reply buffer; handle `final_observation`
         real_next_obs = next_obs.copy()
-        for idx, d in enumerate(dones):
+        for idx, d in enumerate(truncated):
             if d:
-                real_next_obs[idx] = infos[idx]["terminal_observation"]
-        rb.add(obs, real_next_obs, actions, rewards, dones, infos)
+                real_next_obs[idx] = infos["final_observation"][idx]
+        rb.add(obs, real_next_obs, actions, rewards, terminated, infos)
 
         # TRY NOT TO MODIFY: CRUCIAL step easy to overlook
         obs = next_obs
 
         # ALGO LOGIC: training.
         if global_step > args.learning_starts:
             if global_step % args.train_frequency == 0:
@@ -204,17 +223,20 @@
                     writer.add_scalar("charts/SPS", int(global_step / (time.time() - start_time)), global_step)
 
                 # optimize the model
                 optimizer.zero_grad()
                 loss.backward()
                 optimizer.step()
 
-            # update the target network
+            # update target network
             if global_step % args.target_network_frequency == 0:
-                target_network.load_state_dict(q_network.state_dict())
+                for target_network_param, q_network_param in zip(target_network.parameters(), q_network.parameters()):
+                    target_network_param.data.copy_(
+                        args.tau * q_network_param.data + (1.0 - args.tau) * target_network_param.data
+                    )
 
     if args.save_model:
         model_path = f"runs/{run_name}/{args.exp_name}.cleanrl_model"
         torch.save(q_network.state_dict(), model_path)
         print(f"model saved to {model_path}")
         from cleanrl_utils.evals.dqn_eval import evaluate
```

### Comparing `cleanrl-1.1.0/cleanrl/dqn_atari.py` & `cleanrl-1.2.0/cleanrl/dqn_atari.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # docs and experiment results can be found at https://docs.cleanrl.dev/rl-algorithms/dqn/#dqn_ataripy
 import argparse
 import os
 import random
 import time
 from distutils.util import strtobool
 
-import gym
+import gymnasium as gym
 import numpy as np
 import torch
 import torch.nn as nn
 import torch.nn.functional as F
 import torch.optim as optim
 from stable_baselines3.common.atari_wrappers import (
     ClipRewardEnv,
@@ -51,18 +51,22 @@
     # Algorithm specific arguments
     parser.add_argument("--env-id", type=str, default="BreakoutNoFrameskip-v4",
         help="the id of the environment")
     parser.add_argument("--total-timesteps", type=int, default=10000000,
         help="total timesteps of the experiments")
     parser.add_argument("--learning-rate", type=float, default=1e-4,
         help="the learning rate of the optimizer")
+    parser.add_argument("--num-envs", type=int, default=1,
+        help="the number of parallel game environments")
     parser.add_argument("--buffer-size", type=int, default=1000000,
         help="the replay memory buffer size")
     parser.add_argument("--gamma", type=float, default=0.99,
         help="the discount factor gamma")
+    parser.add_argument("--tau", type=float, default=1.,
+        help="the target network update rate")
     parser.add_argument("--target-network-frequency", type=int, default=1000,
         help="the timesteps it takes to update the target network")
     parser.add_argument("--batch-size", type=int, default=32,
         help="the batch size of sample from the reply memory")
     parser.add_argument("--start-e", type=float, default=1,
         help="the starting epsilon for exploration")
     parser.add_argument("--end-e", type=float, default=0.01,
@@ -71,36 +75,38 @@
         help="the fraction of `total-timesteps` it takes from start-e to go end-e")
     parser.add_argument("--learning-starts", type=int, default=80000,
         help="timestep to start learning")
     parser.add_argument("--train-frequency", type=int, default=4,
         help="the frequency of training")
     args = parser.parse_args()
     # fmt: on
+    assert args.num_envs == 1, "vectorized envs are not supported at the moment"
+
     return args
 
 
 def make_env(env_id, seed, idx, capture_video, run_name):
     def thunk():
-        env = gym.make(env_id)
+        if capture_video and idx == 0:
+            env = gym.make(env_id, render_mode="rgb_array")
+            env = gym.wrappers.RecordVideo(env, f"videos/{run_name}")
+        else:
+            env = gym.make(env_id)
         env = gym.wrappers.RecordEpisodeStatistics(env)
-        if capture_video:
-            if idx == 0:
-                env = gym.wrappers.RecordVideo(env, f"videos/{run_name}")
         env = NoopResetEnv(env, noop_max=30)
         env = MaxAndSkipEnv(env, skip=4)
         env = EpisodicLifeEnv(env)
         if "FIRE" in env.unwrapped.get_action_meanings():
             env = FireResetEnv(env)
         env = ClipRewardEnv(env)
         env = gym.wrappers.ResizeObservation(env, (84, 84))
         env = gym.wrappers.GrayScaleObservation(env)
         env = gym.wrappers.FrameStack(env, 4)
-        env.seed(seed)
         env.action_space.seed(seed)
-        env.observation_space.seed(seed)
+
         return env
 
     return thunk
 
 
 # ALGO LOGIC: initialize agent here:
 class QNetwork(nn.Module):
@@ -125,14 +131,23 @@
 
 def linear_schedule(start_e: float, end_e: float, duration: int, t: int):
     slope = (end_e - start_e) / duration
     return max(slope * t + start_e, end_e)
 
 
 if __name__ == "__main__":
+    import stable_baselines3 as sb3
+
+    if sb3.__version__ < "2.0":
+        raise ValueError(
+            """Ongoing migration: run the following command to install the new dependencies:
+
+poetry run pip install "stable_baselines3==2.0.0a1" "gymnasium[atari,accept-rom-license]==0.28.1"  "ale-py==0.8.1" 
+"""
+        )
     args = parse_args()
     run_name = f"{args.env_id}__{args.exp_name}__{args.seed}__{int(time.time())}"
     if args.track:
         import wandb
 
         wandb.init(
             project=args.wandb_project_name,
@@ -154,61 +169,65 @@
     np.random.seed(args.seed)
     torch.manual_seed(args.seed)
     torch.backends.cudnn.deterministic = args.torch_deterministic
 
     device = torch.device("cuda" if torch.cuda.is_available() and args.cuda else "cpu")
 
     # env setup
-    envs = gym.vector.SyncVectorEnv([make_env(args.env_id, args.seed, 0, args.capture_video, run_name)])
+    envs = gym.vector.SyncVectorEnv(
+        [make_env(args.env_id, args.seed + i, i, args.capture_video, run_name) for i in range(args.num_envs)]
+    )
     assert isinstance(envs.single_action_space, gym.spaces.Discrete), "only discrete action space is supported"
 
     q_network = QNetwork(envs).to(device)
     optimizer = optim.Adam(q_network.parameters(), lr=args.learning_rate)
     target_network = QNetwork(envs).to(device)
     target_network.load_state_dict(q_network.state_dict())
 
     rb = ReplayBuffer(
         args.buffer_size,
         envs.single_observation_space,
         envs.single_action_space,
         device,
         optimize_memory_usage=True,
-        handle_timeout_termination=True,
+        handle_timeout_termination=False,
     )
     start_time = time.time()
 
     # TRY NOT TO MODIFY: start the game
-    obs = envs.reset()
+    obs, _ = envs.reset(seed=args.seed)
     for global_step in range(args.total_timesteps):
         # ALGO LOGIC: put action logic here
         epsilon = linear_schedule(args.start_e, args.end_e, args.exploration_fraction * args.total_timesteps, global_step)
         if random.random() < epsilon:
             actions = np.array([envs.single_action_space.sample() for _ in range(envs.num_envs)])
         else:
             q_values = q_network(torch.Tensor(obs).to(device))
             actions = torch.argmax(q_values, dim=1).cpu().numpy()
 
         # TRY NOT TO MODIFY: execute the game and log data.
-        next_obs, rewards, dones, infos = envs.step(actions)
+        next_obs, rewards, terminated, truncated, infos = envs.step(actions)
 
         # TRY NOT TO MODIFY: record rewards for plotting purposes
-        for info in infos:
-            if "episode" in info.keys():
+        if "final_info" in infos:
+            for info in infos["final_info"]:
+                # Skip the envs that are not done
+                if "episode" not in info:
+                    continue
                 print(f"global_step={global_step}, episodic_return={info['episode']['r']}")
                 writer.add_scalar("charts/episodic_return", info["episode"]["r"], global_step)
                 writer.add_scalar("charts/episodic_length", info["episode"]["l"], global_step)
                 writer.add_scalar("charts/epsilon", epsilon, global_step)
-                break
 
-        # TRY NOT TO MODIFY: save data to reply buffer; handle `terminal_observation`
+        # TRY NOT TO MODIFY: save data to reply buffer; handle `final_observation`
         real_next_obs = next_obs.copy()
-        for idx, d in enumerate(dones):
+        for idx, d in enumerate(truncated):
             if d:
-                real_next_obs[idx] = infos[idx]["terminal_observation"]
-        rb.add(obs, real_next_obs, actions, rewards, dones, infos)
+                real_next_obs[idx] = infos["final_observation"][idx]
+        rb.add(obs, real_next_obs, actions, rewards, terminated, infos)
 
         # TRY NOT TO MODIFY: CRUCIAL step easy to overlook
         obs = next_obs
 
         # ALGO LOGIC: training.
         if global_step > args.learning_starts:
             if global_step % args.train_frequency == 0:
@@ -226,17 +245,20 @@
                     writer.add_scalar("charts/SPS", int(global_step / (time.time() - start_time)), global_step)
 
                 # optimize the model
                 optimizer.zero_grad()
                 loss.backward()
                 optimizer.step()
 
-            # update the target network
+            # update target network
             if global_step % args.target_network_frequency == 0:
-                target_network.load_state_dict(q_network.state_dict())
+                for target_network_param, q_network_param in zip(target_network.parameters(), q_network.parameters()):
+                    target_network_param.data.copy_(
+                        args.tau * q_network_param.data + (1.0 - args.tau) * target_network_param.data
+                    )
 
     if args.save_model:
         model_path = f"runs/{run_name}/{args.exp_name}.cleanrl_model"
         torch.save(q_network.state_dict(), model_path)
         print(f"model saved to {model_path}")
         from cleanrl_utils.evals.dqn_eval import evaluate
```

### Comparing `cleanrl-1.1.0/cleanrl/dqn_atari_jax.py` & `cleanrl-1.2.0/cleanrl/dqn_atari_jax.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 os.environ[
     "XLA_PYTHON_CLIENT_MEM_FRACTION"
 ] = "0.7"  # see https://github.com/google/jax/discussions/6332#discussioncomment-1279991
 
 import flax
 import flax.linen as nn
-import gym
+import gymnasium as gym
 import jax
 import jax.numpy as jnp
 import numpy as np
 import optax
 from flax.training.train_state import TrainState
 from stable_baselines3.common.atari_wrappers import (
     ClipRewardEnv,
@@ -53,18 +53,22 @@
     # Algorithm specific arguments
     parser.add_argument("--env-id", type=str, default="BreakoutNoFrameskip-v4",
         help="the id of the environment")
     parser.add_argument("--total-timesteps", type=int, default=10000000,
         help="total timesteps of the experiments")
     parser.add_argument("--learning-rate", type=float, default=1e-4,
         help="the learning rate of the optimizer")
+    parser.add_argument("--num-envs", type=int, default=1,
+        help="the number of parallel game environments")
     parser.add_argument("--buffer-size", type=int, default=1000000,
         help="the replay memory buffer size")
     parser.add_argument("--gamma", type=float, default=0.99,
         help="the discount factor gamma")
+    parser.add_argument("--tau", type=float, default=1.,
+        help="the target network update rate")
     parser.add_argument("--target-network-frequency", type=int, default=1000,
         help="the timesteps it takes to update the target network")
     parser.add_argument("--batch-size", type=int, default=32,
         help="the batch size of sample from the reply memory")
     parser.add_argument("--start-e", type=float, default=1,
         help="the starting epsilon for exploration")
     parser.add_argument("--end-e", type=float, default=0.01,
@@ -73,36 +77,38 @@
         help="the fraction of `total-timesteps` it takes from start-e to go end-e")
     parser.add_argument("--learning-starts", type=int, default=80000,
         help="timestep to start learning")
     parser.add_argument("--train-frequency", type=int, default=4,
         help="the frequency of training")
     args = parser.parse_args()
     # fmt: on
+    assert args.num_envs == 1, "vectorized envs are not supported at the moment"
+
     return args
 
 
 def make_env(env_id, seed, idx, capture_video, run_name):
     def thunk():
-        env = gym.make(env_id)
+        if capture_video and idx == 0:
+            env = gym.make(env_id, render_mode="rgb_array")
+            env = gym.wrappers.RecordVideo(env, f"videos/{run_name}")
+        else:
+            env = gym.make(env_id)
         env = gym.wrappers.RecordEpisodeStatistics(env)
-        if capture_video:
-            if idx == 0:
-                env = gym.wrappers.RecordVideo(env, f"videos/{run_name}")
         env = NoopResetEnv(env, noop_max=30)
         env = MaxAndSkipEnv(env, skip=4)
         env = EpisodicLifeEnv(env)
         if "FIRE" in env.unwrapped.get_action_meanings():
             env = FireResetEnv(env)
         env = ClipRewardEnv(env)
         env = gym.wrappers.ResizeObservation(env, (84, 84))
         env = gym.wrappers.GrayScaleObservation(env)
         env = gym.wrappers.FrameStack(env, 4)
-        env.seed(seed)
         env.action_space.seed(seed)
-        env.observation_space.seed(seed)
+
         return env
 
     return thunk
 
 
 # ALGO LOGIC: initialize agent here:
 class QNetwork(nn.Module):
@@ -131,14 +137,23 @@
 
 def linear_schedule(start_e: float, end_e: float, duration: int, t: int):
     slope = (end_e - start_e) / duration
     return max(slope * t + start_e, end_e)
 
 
 if __name__ == "__main__":
+    import stable_baselines3 as sb3
+
+    if sb3.__version__ < "2.0":
+        raise ValueError(
+            """Ongoing migration: run the following command to install the new dependencies:
+
+poetry run pip install "stable_baselines3==2.0.0a1" "gymnasium[atari,accept-rom-license]==0.28.1"  "ale-py==0.8.1" 
+"""
+        )
     args = parse_args()
     run_name = f"{args.env_id}__{args.exp_name}__{args.seed}__{int(time.time())}"
     if args.track:
         import wandb
 
         wandb.init(
             project=args.wandb_project_name,
@@ -158,18 +173,20 @@
     # TRY NOT TO MODIFY: seeding
     random.seed(args.seed)
     np.random.seed(args.seed)
     key = jax.random.PRNGKey(args.seed)
     key, q_key = jax.random.split(key, 2)
 
     # env setup
-    envs = gym.vector.SyncVectorEnv([make_env(args.env_id, args.seed, 0, args.capture_video, run_name)])
+    envs = gym.vector.SyncVectorEnv(
+        [make_env(args.env_id, args.seed + i, i, args.capture_video, run_name) for i in range(args.num_envs)]
+    )
     assert isinstance(envs.single_action_space, gym.spaces.Discrete), "only discrete action space is supported"
 
-    obs = envs.reset()
+    obs, _ = envs.reset(seed=args.seed)
 
     q_network = QNetwork(action_dim=envs.single_action_space.n)
 
     q_state = TrainState.create(
         apply_fn=q_network.apply,
         params=q_network.init(q_key, obs),
         target_params=q_network.init(q_key, obs),
@@ -182,64 +199,66 @@
 
     rb = ReplayBuffer(
         args.buffer_size,
         envs.single_observation_space,
         envs.single_action_space,
         "cpu",
         optimize_memory_usage=True,
-        handle_timeout_termination=True,
+        handle_timeout_termination=False,
     )
 
     @jax.jit
     def update(q_state, observations, actions, next_observations, rewards, dones):
         q_next_target = q_network.apply(q_state.target_params, next_observations)  # (batch_size, num_actions)
         q_next_target = jnp.max(q_next_target, axis=-1)  # (batch_size,)
         next_q_value = rewards + (1 - dones) * args.gamma * q_next_target
 
         def mse_loss(params):
             q_pred = q_network.apply(params, observations)  # (batch_size, num_actions)
-            q_pred = q_pred[np.arange(q_pred.shape[0]), actions.squeeze()]  # (batch_size,)
+            q_pred = q_pred[jnp.arange(q_pred.shape[0]), actions.squeeze()]  # (batch_size,)
             return ((q_pred - next_q_value) ** 2).mean(), q_pred
 
         (loss_value, q_pred), grads = jax.value_and_grad(mse_loss, has_aux=True)(q_state.params)
         q_state = q_state.apply_gradients(grads=grads)
         return loss_value, q_pred, q_state
 
     start_time = time.time()
 
     # TRY NOT TO MODIFY: start the game
-    obs = envs.reset()
+    obs, _ = envs.reset(seed=args.seed)
     for global_step in range(args.total_timesteps):
         # ALGO LOGIC: put action logic here
         epsilon = linear_schedule(args.start_e, args.end_e, args.exploration_fraction * args.total_timesteps, global_step)
         if random.random() < epsilon:
             actions = np.array([envs.single_action_space.sample() for _ in range(envs.num_envs)])
         else:
             q_values = q_network.apply(q_state.params, obs)
             actions = q_values.argmax(axis=-1)
             actions = jax.device_get(actions)
 
         # TRY NOT TO MODIFY: execute the game and log data.
-        next_obs, rewards, dones, infos = envs.step(actions)
+        next_obs, rewards, terminated, truncated, infos = envs.step(actions)
 
         # TRY NOT TO MODIFY: record rewards for plotting purposes
-        for info in infos:
-            if "episode" in info.keys():
+        if "final_info" in infos:
+            for info in infos["final_info"]:
+                # Skip the envs that are not done
+                if "episode" not in info:
+                    continue
                 print(f"global_step={global_step}, episodic_return={info['episode']['r']}")
                 writer.add_scalar("charts/episodic_return", info["episode"]["r"], global_step)
                 writer.add_scalar("charts/episodic_length", info["episode"]["l"], global_step)
                 writer.add_scalar("charts/epsilon", epsilon, global_step)
-                break
 
-        # TRY NOT TO MODIFY: save data to reply buffer; handle `terminal_observation`
+        # TRY NOT TO MODIFY: save data to reply buffer; handle `final_observation`
         real_next_obs = next_obs.copy()
-        for idx, d in enumerate(dones):
+        for idx, d in enumerate(truncated):
             if d:
-                real_next_obs[idx] = infos[idx]["terminal_observation"]
-        rb.add(obs, real_next_obs, actions, rewards, dones, infos)
+                real_next_obs[idx] = infos["final_observation"][idx]
+        rb.add(obs, real_next_obs, actions, rewards, terminated, infos)
 
         # TRY NOT TO MODIFY: CRUCIAL step easy to overlook
         obs = next_obs
 
         # ALGO LOGIC: training.
         if global_step > args.learning_starts:
             if global_step % args.train_frequency == 0:
@@ -256,17 +275,19 @@
 
                 if global_step % 100 == 0:
                     writer.add_scalar("losses/td_loss", jax.device_get(loss), global_step)
                     writer.add_scalar("losses/q_values", jax.device_get(old_val).mean(), global_step)
                     print("SPS:", int(global_step / (time.time() - start_time)))
                     writer.add_scalar("charts/SPS", int(global_step / (time.time() - start_time)), global_step)
 
-            # update the target network
+            # update target network
             if global_step % args.target_network_frequency == 0:
-                q_state = q_state.replace(target_params=optax.incremental_update(q_state.params, q_state.target_params, 1))
+                q_state = q_state.replace(
+                    target_params=optax.incremental_update(q_state.params, q_state.target_params, args.tau)
+                )
 
     if args.save_model:
         model_path = f"runs/{run_name}/{args.exp_name}.cleanrl_model"
         with open(model_path, "wb") as f:
             f.write(flax.serialization.to_bytes(q_state.params))
         print(f"model saved to {model_path}")
         from cleanrl_utils.evals.dqn_jax_eval import evaluate
```

### Comparing `cleanrl-1.1.0/cleanrl/dqn_jax.py` & `cleanrl-1.2.0/cleanrl/dqn_jax.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import os
 import random
 import time
 from distutils.util import strtobool
 
 import flax
 import flax.linen as nn
-import gym
+import gymnasium as gym
 import jax
 import jax.numpy as jnp
 import numpy as np
 import optax
 from flax.training.train_state import TrainState
 from stable_baselines3.common.buffers import ReplayBuffer
 from torch.utils.tensorboard import SummaryWriter
@@ -42,18 +42,22 @@
     # Algorithm specific arguments
     parser.add_argument("--env-id", type=str, default="CartPole-v1",
         help="the id of the environment")
     parser.add_argument("--total-timesteps", type=int, default=500000,
         help="total timesteps of the experiments")
     parser.add_argument("--learning-rate", type=float, default=2.5e-4,
         help="the learning rate of the optimizer")
+    parser.add_argument("--num-envs", type=int, default=1,
+        help="the number of parallel game environments")
     parser.add_argument("--buffer-size", type=int, default=10000,
         help="the replay memory buffer size")
     parser.add_argument("--gamma", type=float, default=0.99,
         help="the discount factor gamma")
+    parser.add_argument("--tau", type=float, default=1.,
+        help="the target network update rate")
     parser.add_argument("--target-network-frequency", type=int, default=500,
         help="the timesteps it takes to update the target network")
     parser.add_argument("--batch-size", type=int, default=128,
         help="the batch size of sample from the reply memory")
     parser.add_argument("--start-e", type=float, default=1,
         help="the starting epsilon for exploration")
     parser.add_argument("--end-e", type=float, default=0.05,
@@ -62,27 +66,29 @@
         help="the fraction of `total-timesteps` it takes from start-e to go end-e")
     parser.add_argument("--learning-starts", type=int, default=10000,
         help="timestep to start learning")
     parser.add_argument("--train-frequency", type=int, default=10,
         help="the frequency of training")
     args = parser.parse_args()
     # fmt: on
+    assert args.num_envs == 1, "vectorized envs are not supported at the moment"
+
     return args
 
 
 def make_env(env_id, seed, idx, capture_video, run_name):
     def thunk():
-        env = gym.make(env_id)
+        if capture_video and idx == 0:
+            env = gym.make(env_id, render_mode="rgb_array")
+            env = gym.wrappers.RecordVideo(env, f"videos/{run_name}")
+        else:
+            env = gym.make(env_id)
         env = gym.wrappers.RecordEpisodeStatistics(env)
-        if capture_video:
-            if idx == 0:
-                env = gym.wrappers.RecordVideo(env, f"videos/{run_name}")
-        env.seed(seed)
         env.action_space.seed(seed)
-        env.observation_space.seed(seed)
+
         return env
 
     return thunk
 
 
 # ALGO LOGIC: initialize agent here:
 class QNetwork(nn.Module):
@@ -104,14 +110,23 @@
 
 def linear_schedule(start_e: float, end_e: float, duration: int, t: int):
     slope = (end_e - start_e) / duration
     return max(slope * t + start_e, end_e)
 
 
 if __name__ == "__main__":
+    import stable_baselines3 as sb3
+
+    if sb3.__version__ < "2.0":
+        raise ValueError(
+            """Ongoing migration: run the following command to install the new dependencies:
+
+poetry run pip install "stable_baselines3==2.0.0a1"
+"""
+        )
     args = parse_args()
     run_name = f"{args.env_id}__{args.exp_name}__{args.seed}__{int(time.time())}"
     if args.track:
         import wandb
 
         wandb.init(
             project=args.wandb_project_name,
@@ -131,18 +146,20 @@
     # TRY NOT TO MODIFY: seeding
     random.seed(args.seed)
     np.random.seed(args.seed)
     key = jax.random.PRNGKey(args.seed)
     key, q_key = jax.random.split(key, 2)
 
     # env setup
-    envs = gym.vector.SyncVectorEnv([make_env(args.env_id, args.seed, 0, args.capture_video, run_name)])
+    envs = gym.vector.SyncVectorEnv(
+        [make_env(args.env_id, args.seed + i, i, args.capture_video, run_name) for i in range(args.num_envs)]
+    )
     assert isinstance(envs.single_action_space, gym.spaces.Discrete), "only discrete action space is supported"
 
-    obs = envs.reset()
+    obs, _ = envs.reset(seed=args.seed)
 
     q_network = QNetwork(action_dim=envs.single_action_space.n)
 
     q_state = TrainState.create(
         apply_fn=q_network.apply,
         params=q_network.init(q_key, obs),
         target_params=q_network.init(q_key, obs),
@@ -154,64 +171,66 @@
     q_state = q_state.replace(target_params=optax.incremental_update(q_state.params, q_state.target_params, 1))
 
     rb = ReplayBuffer(
         args.buffer_size,
         envs.single_observation_space,
         envs.single_action_space,
         "cpu",
-        handle_timeout_termination=True,
+        handle_timeout_termination=False,
     )
 
     @jax.jit
     def update(q_state, observations, actions, next_observations, rewards, dones):
         q_next_target = q_network.apply(q_state.target_params, next_observations)  # (batch_size, num_actions)
         q_next_target = jnp.max(q_next_target, axis=-1)  # (batch_size,)
         next_q_value = rewards + (1 - dones) * args.gamma * q_next_target
 
         def mse_loss(params):
             q_pred = q_network.apply(params, observations)  # (batch_size, num_actions)
-            q_pred = q_pred[np.arange(q_pred.shape[0]), actions.squeeze()]  # (batch_size,)
+            q_pred = q_pred[jnp.arange(q_pred.shape[0]), actions.squeeze()]  # (batch_size,)
             return ((q_pred - next_q_value) ** 2).mean(), q_pred
 
         (loss_value, q_pred), grads = jax.value_and_grad(mse_loss, has_aux=True)(q_state.params)
         q_state = q_state.apply_gradients(grads=grads)
         return loss_value, q_pred, q_state
 
     start_time = time.time()
 
     # TRY NOT TO MODIFY: start the game
-    obs = envs.reset()
+    obs, _ = envs.reset(seed=args.seed)
     for global_step in range(args.total_timesteps):
         # ALGO LOGIC: put action logic here
         epsilon = linear_schedule(args.start_e, args.end_e, args.exploration_fraction * args.total_timesteps, global_step)
         if random.random() < epsilon:
             actions = np.array([envs.single_action_space.sample() for _ in range(envs.num_envs)])
         else:
             q_values = q_network.apply(q_state.params, obs)
             actions = q_values.argmax(axis=-1)
             actions = jax.device_get(actions)
 
         # TRY NOT TO MODIFY: execute the game and log data.
-        next_obs, rewards, dones, infos = envs.step(actions)
+        next_obs, rewards, terminated, truncated, infos = envs.step(actions)
 
         # TRY NOT TO MODIFY: record rewards for plotting purposes
-        for info in infos:
-            if "episode" in info.keys():
+        if "final_info" in infos:
+            for info in infos["final_info"]:
+                # Skip the envs that are not done
+                if "episode" not in info:
+                    continue
                 print(f"global_step={global_step}, episodic_return={info['episode']['r']}")
                 writer.add_scalar("charts/episodic_return", info["episode"]["r"], global_step)
                 writer.add_scalar("charts/episodic_length", info["episode"]["l"], global_step)
                 writer.add_scalar("charts/epsilon", epsilon, global_step)
-                break
 
-        # TRY NOT TO MODIFY: save data to reply buffer; handle `terminal_observation`
+        # TRY NOT TO MODIFY: save data to reply buffer; handle `final_observation`
         real_next_obs = next_obs.copy()
-        for idx, d in enumerate(dones):
+        for idx, d in enumerate(truncated):
             if d:
-                real_next_obs[idx] = infos[idx]["terminal_observation"]
-        rb.add(obs, real_next_obs, actions, rewards, dones, infos)
+                real_next_obs[idx] = infos["final_observation"][idx]
+        rb.add(obs, real_next_obs, actions, rewards, terminated, infos)
 
         # TRY NOT TO MODIFY: CRUCIAL step easy to overlook
         obs = next_obs
 
         # ALGO LOGIC: training.
         if global_step > args.learning_starts:
             if global_step % args.train_frequency == 0:
@@ -228,17 +247,19 @@
 
                 if global_step % 100 == 0:
                     writer.add_scalar("losses/td_loss", jax.device_get(loss), global_step)
                     writer.add_scalar("losses/q_values", jax.device_get(old_val).mean(), global_step)
                     print("SPS:", int(global_step / (time.time() - start_time)))
                     writer.add_scalar("charts/SPS", int(global_step / (time.time() - start_time)), global_step)
 
-            # update the target network
+            # update target network
             if global_step % args.target_network_frequency == 0:
-                q_state = q_state.replace(target_params=optax.incremental_update(q_state.params, q_state.target_params, 1))
+                q_state = q_state.replace(
+                    target_params=optax.incremental_update(q_state.params, q_state.target_params, args.tau)
+                )
 
     if args.save_model:
         model_path = f"runs/{run_name}/{args.exp_name}.cleanrl_model"
         with open(model_path, "wb") as f:
             f.write(flax.serialization.to_bytes(q_state.params))
         print(f"model saved to {model_path}")
         from cleanrl_utils.evals.dqn_jax_eval import evaluate
```

### Comparing `cleanrl-1.1.0/cleanrl/ppg_procgen.py` & `cleanrl-1.2.0/cleanrl/ppg_procgen.py`

 * *Files identical despite different names*

### Comparing `cleanrl-1.1.0/cleanrl/ppo.py` & `cleanrl-1.2.0/cleanrl/ppo.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 # docs and experiment results can be found at https://docs.cleanrl.dev/rl-algorithms/ppo/#ppopy
-
 import argparse
 import os
 import random
 import time
 from distutils.util import strtobool
 
 import gym
```

### Comparing `cleanrl-1.1.0/cleanrl/ppo_atari.py` & `cleanrl-1.2.0/cleanrl/ppo_atari.py`

 * *Files identical despite different names*

### Comparing `cleanrl-1.1.0/cleanrl/ppo_atari_envpool.py` & `cleanrl-1.2.0/cleanrl/ppo_atari_envpool.py`

 * *Files identical despite different names*

### Comparing `cleanrl-1.1.0/cleanrl/ppo_atari_envpool_xla_jax.py` & `cleanrl-1.2.0/cleanrl/ppo_atari_envpool_xla_jax.py`

 * *Files identical despite different names*

### Comparing `cleanrl-1.1.0/cleanrl/ppo_atari_envpool_xla_jax_scan.py` & `cleanrl-1.2.0/cleanrl/ppo_atari_envpool_xla_jax_scan.py`

 * *Files identical despite different names*

### Comparing `cleanrl-1.1.0/cleanrl/ppo_atari_lstm.py` & `cleanrl-1.2.0/cleanrl/ppo_atari_lstm.py`

 * *Files identical despite different names*

### Comparing `cleanrl-1.1.0/cleanrl/ppo_atari_multigpu.py` & `cleanrl-1.2.0/cleanrl/ppo_atari_multigpu.py`

 * *Files identical despite different names*

### Comparing `cleanrl-1.1.0/cleanrl/ppo_continuous_action.py` & `cleanrl-1.2.0/cleanrl/ppo_continuous_action.py`

 * *Files 1% similar despite different names*

```diff
@@ -143,15 +143,15 @@
 
         wandb.init(
             project=args.wandb_project_name,
             entity=args.wandb_entity,
             sync_tensorboard=True,
             config=vars(args),
             name=run_name,
-            # monitor_gym=True, no longer works for gymnasium
+            monitor_gym=True,
             save_code=True,
         )
     writer = SummaryWriter(f"runs/{run_name}")
     writer.add_text(
         "hyperparameters",
         "|param|value|\n|-|-|\n%s" % ("\n".join([f"|{key}|{value}|" for key, value in vars(args).items()])),
     )
@@ -184,15 +184,14 @@
     # TRY NOT TO MODIFY: start the game
     global_step = 0
     start_time = time.time()
     next_obs, _ = envs.reset(seed=args.seed)
     next_obs = torch.Tensor(next_obs).to(device)
     next_done = torch.zeros(args.num_envs).to(device)
     num_updates = args.total_timesteps // args.batch_size
-    video_filenames = set()
 
     for update in range(1, num_updates + 1):
         # Annealing the rate if instructed to do so.
         if args.anneal_lr:
             frac = 1.0 - (update - 1.0) / num_updates
             lrnow = frac * args.learning_rate
             optimizer.param_groups[0]["lr"] = lrnow
@@ -318,15 +317,9 @@
         writer.add_scalar("losses/old_approx_kl", old_approx_kl.item(), global_step)
         writer.add_scalar("losses/approx_kl", approx_kl.item(), global_step)
         writer.add_scalar("losses/clipfrac", np.mean(clipfracs), global_step)
         writer.add_scalar("losses/explained_variance", explained_var, global_step)
         print("SPS:", int(global_step / (time.time() - start_time)))
         writer.add_scalar("charts/SPS", int(global_step / (time.time() - start_time)), global_step)
 
-        if args.track and args.capture_video:
-            for filename in os.listdir(f"videos/{run_name}"):
-                if filename not in video_filenames and filename.endswith(".mp4"):
-                    wandb.log({f"videos": wandb.Video(f"videos/{run_name}/{filename}")})
-                    video_filenames.add(filename)
-
     envs.close()
     writer.close()
```

### Comparing `cleanrl-1.1.0/cleanrl/ppo_continuous_action_isaacgym/isaacgym/poetry.lock` & `cleanrl-1.2.0/cleanrl/ppo_continuous_action_isaacgym/isaacgym/poetry.lock`

 * *Files 0% similar despite different names*

```diff
@@ -240,15 +240,15 @@
 
 [package.extras]
 docs = ["jaraco.packaging (>=9)", "jaraco.tidelift (>=1.4)", "rst.linker (>=1.9)", "sphinx"]
 testing = ["func-timeout", "jaraco.itertools", "pytest (>=6)", "pytest-black (>=0.3.7)", "pytest-checkdocs (>=2.4)", "pytest-cov", "pytest-enabler (>=1.3)", "pytest-flake8", "pytest-mypy (>=0.9.1)"]
 
 [metadata]
 lock-version = "1.1"
-python-versions = ">=3.7.1,<3.10"
+python-versions = ">=3.7.1"
 content-hash = "f7be23a52835151338ab66c16f5782ef2a739d9a9a183cdf51ae18879bb558ff"
 
 [metadata.files]
 certifi = [
     {file = "certifi-2022.9.24-py3-none-any.whl", hash = "sha256:90c1a32f1d68f940488354e36370f6cca89f0f106db09518524c88d6ed83f382"},
     {file = "certifi-2022.9.24.tar.gz", hash = "sha256:0d9c601124e5a6ba9712dbc60d9c53c21e34f5f641fe83002317394311bdce14"},
 ]
```

### Comparing `cleanrl-1.1.0/cleanrl/ppo_continuous_action_isaacgym/ppo_continuous_action_isaacgym.py` & `cleanrl-1.2.0/cleanrl/ppo_continuous_action_isaacgym/ppo_continuous_action_isaacgym.py`

 * *Files identical despite different names*

### Comparing `cleanrl-1.1.0/cleanrl/ppo_pettingzoo_ma_atari.py` & `cleanrl-1.2.0/cleanrl/ppo_pettingzoo_ma_atari.py`

 * *Files identical despite different names*

### Comparing `cleanrl-1.1.0/cleanrl/ppo_procgen.py` & `cleanrl-1.2.0/cleanrl/ppo_procgen.py`

 * *Files identical despite different names*

### Comparing `cleanrl-1.1.0/cleanrl/ppo_rnd_envpool.py` & `cleanrl-1.2.0/cleanrl/ppo_rnd_envpool.py`

 * *Files identical despite different names*

### Comparing `cleanrl-1.1.0/cleanrl/sac_continuous_action.py` & `cleanrl-1.2.0/cleanrl/sac_continuous_action.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 import os
 import random
 import time
 from distutils.util import strtobool
 
 import gym
 import numpy as np
-import pybullet_envs  # noqa
 import torch
 import torch.nn as nn
 import torch.nn.functional as F
 import torch.optim as optim
 from stable_baselines3.common.buffers import ReplayBuffer
 from torch.utils.tensorboard import SummaryWriter
 
@@ -33,28 +32,26 @@
         help="the wandb's project name")
     parser.add_argument("--wandb-entity", type=str, default=None,
         help="the entity (team) of wandb's project")
     parser.add_argument("--capture-video", type=lambda x: bool(strtobool(x)), default=False, nargs="?", const=True,
         help="whether to capture videos of the agent performances (check out `videos` folder)")
 
     # Algorithm specific arguments
-    parser.add_argument("--env-id", type=str, default="HopperBulletEnv-v0",
+    parser.add_argument("--env-id", type=str, default="Hopper-v4",
         help="the id of the environment")
     parser.add_argument("--total-timesteps", type=int, default=1000000,
         help="total timesteps of the experiments")
     parser.add_argument("--buffer-size", type=int, default=int(1e6),
         help="the replay memory buffer size")
     parser.add_argument("--gamma", type=float, default=0.99,
         help="the discount factor gamma")
     parser.add_argument("--tau", type=float, default=0.005,
         help="target smoothing coefficient (default: 0.005)")
     parser.add_argument("--batch-size", type=int, default=256,
         help="the batch size of sample from the reply memory")
-    parser.add_argument("--exploration-noise", type=float, default=0.1,
-        help="the scale of exploration noise")
     parser.add_argument("--learning-starts", type=int, default=5e3,
         help="timestep to start learning")
     parser.add_argument("--policy-lr", type=float, default=3e-4,
         help="the learning rate of the policy network optimizer")
     parser.add_argument("--q-lr", type=float, default=1e-3,
         help="the learning rate of the Q network network optimizer")
     parser.add_argument("--policy-frequency", type=int, default=2,
```

### Comparing `cleanrl-1.1.0/cleanrl/td3_continuous_action.py` & `cleanrl-1.2.0/cleanrl/td3_continuous_action.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 import os
 import random
 import time
 from distutils.util import strtobool
 
 import gym
 import numpy as np
-import pybullet_envs  # noqa
 import torch
 import torch.nn as nn
 import torch.nn.functional as F
 import torch.optim as optim
 from stable_baselines3.common.buffers import ReplayBuffer
 from torch.utils.tensorboard import SummaryWriter
 
@@ -33,15 +32,15 @@
         help="the wandb's project name")
     parser.add_argument("--wandb-entity", type=str, default=None,
         help="the entity (team) of wandb's project")
     parser.add_argument("--capture-video", type=lambda x: bool(strtobool(x)), default=False, nargs="?", const=True,
         help="whether to capture videos of the agent performances (check out `videos` folder)")
 
     # Algorithm specific arguments
-    parser.add_argument("--env-id", type=str, default="HopperBulletEnv-v0",
+    parser.add_argument("--env-id", type=str, default="Hopper-v4",
         help="the id of the environment")
     parser.add_argument("--total-timesteps", type=int, default=1000000,
         help="total timesteps of the experiments")
     parser.add_argument("--learning-rate", type=float, default=3e-4,
         help="the learning rate of the optimizer")
     parser.add_argument("--buffer-size", type=int, default=int(1e6),
         help="the replay memory buffer size")
```

### Comparing `cleanrl-1.1.0/cleanrl/td3_continuous_action_jax.py` & `cleanrl-1.2.0/cleanrl/ddpg_continuous_action_jax.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,23 +1,22 @@
-# docs and experiment results can be found at https://docs.cleanrl.dev/rl-algorithms/td3/#td3_continuous_action_jaxpy
+# docs and experiment results can be found at https://docs.cleanrl.dev/rl-algorithms/ddpg/#ddpg_continuous_action_jaxpy
 import argparse
 import os
 import random
 import time
 from distutils.util import strtobool
 from typing import Sequence
 
 import flax
 import flax.linen as nn
-import gym
+import gymnasium as gym
 import jax
 import jax.numpy as jnp
 import numpy as np
 import optax
-import pybullet_envs  # noqa
 from flax.training.train_state import TrainState
 from stable_baselines3.common.buffers import ReplayBuffer
 from torch.utils.tensorboard import SummaryWriter
 
 
 def parse_args():
     # fmt: off
@@ -32,28 +31,26 @@
         help="the wandb's project name")
     parser.add_argument("--wandb-entity", type=str, default=None,
         help="the entity (team) of wandb's project")
     parser.add_argument("--capture-video", type=lambda x: bool(strtobool(x)), default=False, nargs="?", const=True,
         help="whether to capture videos of the agent performances (check out `videos` folder)")
 
     # Algorithm specific arguments
-    parser.add_argument("--env-id", type=str, default="HalfCheetah-v2",
+    parser.add_argument("--env-id", type=str, default="HalfCheetah-v4",
         help="the id of the environment")
     parser.add_argument("--total-timesteps", type=int, default=1000000,
         help="total timesteps of the experiments")
     parser.add_argument("--learning-rate", type=float, default=3e-4,
         help="the learning rate of the optimizer")
     parser.add_argument("--buffer-size", type=int, default=int(1e6),
         help="the replay memory buffer size")
     parser.add_argument("--gamma", type=float, default=0.99,
         help="the discount factor gamma")
     parser.add_argument("--tau", type=float, default=0.005,
         help="target smoothing coefficient (default: 0.005)")
-    parser.add_argument("--policy-noise", type=float, default=0.2,
-        help="the scale of policy noise")
     parser.add_argument("--batch-size", type=int, default=256,
         help="the batch size of sample from the reply memory")
     parser.add_argument("--exploration-noise", type=float, default=0.1,
         help="the scale of exploration noise")
     parser.add_argument("--learning-starts", type=int, default=25e3,
         help="timestep to start learning")
     parser.add_argument("--policy-frequency", type=int, default=2,
@@ -63,20 +60,22 @@
     args = parser.parse_args()
     # fmt: on
     return args
 
 
 def make_env(env_id, seed, idx, capture_video, run_name):
     def thunk():
-        env = gym.make(env_id)
+        if capture_video:
+            env = gym.make(env_id, render_mode="rgb_array")
+        else:
+            env = gym.make(env_id)
         env = gym.wrappers.RecordEpisodeStatistics(env)
         if capture_video:
             if idx == 0:
                 env = gym.wrappers.RecordVideo(env, f"videos/{run_name}")
-        env.seed(seed)
         env.action_space.seed(seed)
         env.observation_space.seed(seed)
         return env
 
     return thunk
 
 
@@ -111,14 +110,23 @@
 
 
 class TrainState(TrainState):
     target_params: flax.core.FrozenDict
 
 
 if __name__ == "__main__":
+    import stable_baselines3 as sb3
+
+    if sb3.__version__ < "2.0":
+        raise ValueError(
+            """Ongoing migration: run the following command to install the new dependencies:
+
+poetry run pip install "stable_baselines3==2.0.0a1"
+"""
+        )
     args = parse_args()
     run_name = f"{args.env_id}__{args.exp_name}__{args.seed}__{int(time.time())}"
     if args.track:
         import wandb
 
         wandb.init(
             project=args.wandb_project_name,
@@ -135,191 +143,154 @@
         "|param|value|\n|-|-|\n%s" % ("\n".join([f"|{key}|{value}|" for key, value in vars(args).items()])),
     )
 
     # TRY NOT TO MODIFY: seeding
     random.seed(args.seed)
     np.random.seed(args.seed)
     key = jax.random.PRNGKey(args.seed)
-    key, actor_key, qf1_key, qf2_key = jax.random.split(key, 4)
+    key, actor_key, qf1_key = jax.random.split(key, 3)
 
     # env setup
     envs = gym.vector.SyncVectorEnv([make_env(args.env_id, args.seed, 0, args.capture_video, run_name)])
     assert isinstance(envs.single_action_space, gym.spaces.Box), "only continuous action space is supported"
 
     max_action = float(envs.single_action_space.high[0])
     envs.single_observation_space.dtype = np.float32
     rb = ReplayBuffer(
         args.buffer_size,
         envs.single_observation_space,
         envs.single_action_space,
         device="cpu",
-        handle_timeout_termination=True,
+        handle_timeout_termination=False,
     )
 
     # TRY NOT TO MODIFY: start the game
-    obs = envs.reset()
+    obs, _ = envs.reset()
+
+    action_scale = np.array((envs.action_space.high - envs.action_space.low) / 2.0)
+    action_bias = np.array((envs.action_space.high + envs.action_space.low) / 2.0)
     actor = Actor(
         action_dim=np.prod(envs.single_action_space.shape),
-        action_scale=jnp.array((envs.action_space.high - envs.action_space.low) / 2.0),
-        action_bias=jnp.array((envs.action_space.high + envs.action_space.low) / 2.0),
+        action_scale=action_scale,
+        action_bias=action_bias,
     )
+    qf1 = QNetwork()
     actor_state = TrainState.create(
         apply_fn=actor.apply,
         params=actor.init(actor_key, obs),
         target_params=actor.init(actor_key, obs),
         tx=optax.adam(learning_rate=args.learning_rate),
     )
-    qf = QNetwork()
     qf1_state = TrainState.create(
-        apply_fn=qf.apply,
-        params=qf.init(qf1_key, obs, envs.action_space.sample()),
-        target_params=qf.init(qf1_key, obs, envs.action_space.sample()),
-        tx=optax.adam(learning_rate=args.learning_rate),
-    )
-    qf2_state = TrainState.create(
-        apply_fn=qf.apply,
-        params=qf.init(qf2_key, obs, envs.action_space.sample()),
-        target_params=qf.init(qf2_key, obs, envs.action_space.sample()),
+        apply_fn=qf1.apply,
+        params=qf1.init(qf1_key, obs, envs.action_space.sample()),
+        target_params=qf1.init(qf1_key, obs, envs.action_space.sample()),
         tx=optax.adam(learning_rate=args.learning_rate),
     )
     actor.apply = jax.jit(actor.apply)
-    qf.apply = jax.jit(qf.apply)
+    qf1.apply = jax.jit(qf1.apply)
 
     @jax.jit
     def update_critic(
         actor_state: TrainState,
         qf1_state: TrainState,
-        qf2_state: TrainState,
         observations: np.ndarray,
         actions: np.ndarray,
         next_observations: np.ndarray,
         rewards: np.ndarray,
         dones: np.ndarray,
-        key: jnp.ndarray,
     ):
-        # TODO Maybe pre-generate a lot of random keys
-        # also check https://jax.readthedocs.io/en/latest/jax.random.html
-        key, noise_key = jax.random.split(key, 2)
-        clipped_noise = (
-            jnp.clip(
-                (jax.random.normal(noise_key, actions.shape) * args.policy_noise),
-                -args.noise_clip,
-                args.noise_clip,
-            )
-            * actor.action_scale
-        )
-        next_state_actions = jnp.clip(
-            actor.apply(actor_state.target_params, next_observations) + clipped_noise,
-            envs.single_action_space.low[0],
-            envs.single_action_space.high[0],
-        )
-        qf1_next_target = qf.apply(qf1_state.target_params, next_observations, next_state_actions).reshape(-1)
-        qf2_next_target = qf.apply(qf2_state.target_params, next_observations, next_state_actions).reshape(-1)
-        min_qf_next_target = jnp.minimum(qf1_next_target, qf2_next_target)
-        next_q_value = (rewards + (1 - dones) * args.gamma * (min_qf_next_target)).reshape(-1)
+        next_state_actions = (actor.apply(actor_state.target_params, next_observations)).clip(-1, 1)  # TODO: proper clip
+        qf1_next_target = qf1.apply(qf1_state.target_params, next_observations, next_state_actions).reshape(-1)
+        next_q_value = (rewards + (1 - dones) * args.gamma * (qf1_next_target)).reshape(-1)
 
         def mse_loss(params):
-            qf_a_values = qf.apply(params, observations, actions).squeeze()
-            return ((qf_a_values - next_q_value) ** 2).mean(), qf_a_values.mean()
-
-        (qf1_loss_value, qf1_a_values), grads1 = jax.value_and_grad(mse_loss, has_aux=True)(qf1_state.params)
-        (qf2_loss_value, qf2_a_values), grads2 = jax.value_and_grad(mse_loss, has_aux=True)(qf2_state.params)
-        qf1_state = qf1_state.apply_gradients(grads=grads1)
-        qf2_state = qf2_state.apply_gradients(grads=grads2)
+            qf1_a_values = qf1.apply(params, observations, actions).squeeze()
+            return ((qf1_a_values - next_q_value) ** 2).mean(), qf1_a_values.mean()
 
-        return (qf1_state, qf2_state), (qf1_loss_value, qf2_loss_value), (qf1_a_values, qf2_a_values), key
+        (qf1_loss_value, qf1_a_values), grads = jax.value_and_grad(mse_loss, has_aux=True)(qf1_state.params)
+        qf1_state = qf1_state.apply_gradients(grads=grads)
+        return qf1_state, qf1_loss_value, qf1_a_values
 
     @jax.jit
     def update_actor(
         actor_state: TrainState,
         qf1_state: TrainState,
-        qf2_state: TrainState,
         observations: np.ndarray,
     ):
         def actor_loss(params):
-            return -qf.apply(qf1_state.params, observations, actor.apply(params, observations)).mean()
+            return -qf1.apply(qf1_state.params, observations, actor.apply(params, observations)).mean()
 
         actor_loss_value, grads = jax.value_and_grad(actor_loss)(actor_state.params)
         actor_state = actor_state.apply_gradients(grads=grads)
         actor_state = actor_state.replace(
             target_params=optax.incremental_update(actor_state.params, actor_state.target_params, args.tau)
         )
-
         qf1_state = qf1_state.replace(
             target_params=optax.incremental_update(qf1_state.params, qf1_state.target_params, args.tau)
         )
-        qf2_state = qf2_state.replace(
-            target_params=optax.incremental_update(qf2_state.params, qf2_state.target_params, args.tau)
-        )
-        return actor_state, (qf1_state, qf2_state), actor_loss_value
+        return actor_state, qf1_state, actor_loss_value
 
     start_time = time.time()
     for global_step in range(args.total_timesteps):
         # ALGO LOGIC: put action logic here
         if global_step < args.learning_starts:
             actions = np.array([envs.single_action_space.sample() for _ in range(envs.num_envs)])
         else:
             actions = actor.apply(actor_state.params, obs)
             actions = np.array(
                 [
-                    (
-                        jax.device_get(actions)[0]
-                        + np.random.normal(0, max_action * args.exploration_noise, size=envs.single_action_space.shape[0])
-                    ).clip(envs.single_action_space.low, envs.single_action_space.high)
+                    (jax.device_get(actions)[0] + np.random.normal(0, action_scale * args.exploration_noise)[0]).clip(
+                        envs.single_action_space.low, envs.single_action_space.high
+                    )
                 ]
             )
 
         # TRY NOT TO MODIFY: execute the game and log data.
-        next_obs, rewards, dones, infos = envs.step(actions)
+        next_obs, rewards, terminateds, truncateds, infos = envs.step(actions)
 
         # TRY NOT TO MODIFY: record rewards for plotting purposes
-        for info in infos:
-            if "episode" in info.keys():
+        if "final_info" in infos:
+            for info in infos["final_info"]:
                 print(f"global_step={global_step}, episodic_return={info['episode']['r']}")
                 writer.add_scalar("charts/episodic_return", info["episode"]["r"], global_step)
                 writer.add_scalar("charts/episodic_length", info["episode"]["l"], global_step)
                 break
 
-        # TRY NOT TO MODIFY: save data to replay buffer; handle `terminal_observation`
+        # TRY NOT TO MODIFY: save data to reply buffer; handle `terminal_observation`
         real_next_obs = next_obs.copy()
-        for idx, d in enumerate(dones):
+        for idx, d in enumerate(truncateds):
             if d:
-                real_next_obs[idx] = infos[idx]["terminal_observation"]
-        rb.add(obs, real_next_obs, actions, rewards, dones, infos)
+                real_next_obs[idx] = infos["final_observation"][idx]
+        rb.add(obs, real_next_obs, actions, rewards, terminateds, infos)
 
         # TRY NOT TO MODIFY: CRUCIAL step easy to overlook
         obs = next_obs
 
         # ALGO LOGIC: training.
         if global_step > args.learning_starts:
             data = rb.sample(args.batch_size)
-
-            (qf1_state, qf2_state), (qf1_loss_value, qf2_loss_value), (qf1_a_values, qf2_a_values), key = update_critic(
+            qf1_state, qf1_loss_value, qf1_a_values = update_critic(
                 actor_state,
                 qf1_state,
-                qf2_state,
                 data.observations.numpy(),
                 data.actions.numpy(),
                 data.next_observations.numpy(),
                 data.rewards.flatten().numpy(),
                 data.dones.flatten().numpy(),
-                key,
             )
-
             if global_step % args.policy_frequency == 0:
-                actor_state, (qf1_state, qf2_state), actor_loss_value = update_actor(
+                actor_state, qf1_state, actor_loss_value = update_actor(
                     actor_state,
                     qf1_state,
-                    qf2_state,
                     data.observations.numpy(),
                 )
+
             if global_step % 100 == 0:
                 writer.add_scalar("losses/qf1_loss", qf1_loss_value.item(), global_step)
-                writer.add_scalar("losses/qf2_loss", qf2_loss_value.item(), global_step)
-                writer.add_scalar("losses/qf1_values", qf1_a_values.item(), global_step)
-                writer.add_scalar("losses/qf2_values", qf2_a_values.item(), global_step)
                 writer.add_scalar("losses/actor_loss", actor_loss_value.item(), global_step)
+                writer.add_scalar("losses/qf1_values", qf1_a_values.item(), global_step)
                 print("SPS:", int(global_step / (time.time() - start_time)))
                 writer.add_scalar("charts/SPS", int(global_step / (time.time() - start_time)), global_step)
 
     envs.close()
     writer.close()
```

### Comparing `cleanrl-1.1.0/cleanrl_utils/add_header.py` & `cleanrl-1.2.0/cleanrl_utils/add_header.py`

 * *Files identical despite different names*

### Comparing `cleanrl-1.1.0/cleanrl_utils/benchmark.py` & `cleanrl-1.2.0/cleanrl_utils/benchmark.py`

 * *Files identical despite different names*

### Comparing `cleanrl-1.1.0/cleanrl_utils/buffers.py` & `cleanrl-1.2.0/cleanrl_utils/buffers.py`

 * *Files identical despite different names*

### Comparing `cleanrl-1.1.0/cleanrl_utils/docker_queue.py` & `cleanrl-1.2.0/cleanrl_utils/docker_queue.py`

 * *Files identical despite different names*

### Comparing `cleanrl-1.1.0/cleanrl_utils/enjoy.py` & `cleanrl-1.2.0/cleanrl_utils/enjoy.py`

 * *Files identical despite different names*

### Comparing `cleanrl-1.1.0/cleanrl_utils/evals/__init__.py` & `cleanrl-1.2.0/cleanrl_utils/evals/__init__.py`

 * *Files identical despite different names*

### Comparing `cleanrl-1.1.0/cleanrl_utils/evals/c51_eval.py` & `cleanrl-1.2.0/cleanrl_utils/evals/c51_eval.py`

 * *Files identical despite different names*

### Comparing `cleanrl-1.1.0/cleanrl_utils/evals/c51_jax_eval.py` & `cleanrl-1.2.0/cleanrl_utils/evals/c51_jax_eval.py`

 * *Files identical despite different names*

### Comparing `cleanrl-1.1.0/cleanrl_utils/evals/dqn_eval.py` & `cleanrl-1.2.0/cleanrl_utils/evals/dqn_eval.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import random
 from typing import Callable
 
-import gym
+import gymnasium as gym
 import numpy as np
 import torch
 
 
 def evaluate(
     model_path: str,
     make_env: Callable,
@@ -18,25 +18,27 @@
     capture_video: bool = True,
 ):
     envs = gym.vector.SyncVectorEnv([make_env(env_id, 0, 0, capture_video, run_name)])
     model = Model(envs).to(device)
     model.load_state_dict(torch.load(model_path, map_location=device))
     model.eval()
 
-    obs = envs.reset()
+    obs, _ = envs.reset()
     episodic_returns = []
     while len(episodic_returns) < eval_episodes:
         if random.random() < epsilon:
             actions = np.array([envs.single_action_space.sample() for _ in range(envs.num_envs)])
         else:
             q_values = model(torch.Tensor(obs).to(device))
             actions = torch.argmax(q_values, dim=1).cpu().numpy()
-        next_obs, _, _, infos = envs.step(actions)
-        for info in infos:
-            if "episode" in info.keys():
+        next_obs, _, _, _, infos = envs.step(actions)
+        if "final_info" in infos:
+            for info in infos["final_info"]:
+                if "episode" not in info:
+                    continue
                 print(f"eval_episode={len(episodic_returns)}, episodic_return={info['episode']['r']}")
                 episodic_returns += [info["episode"]["r"]]
         obs = next_obs
 
     return episodic_returns
```

### Comparing `cleanrl-1.1.0/cleanrl_utils/evals/dqn_jax_eval.py` & `cleanrl-1.2.0/cleanrl_utils/evals/dqn_jax_eval.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import random
 from typing import Callable
 
 import flax
 import flax.linen as nn
-import gym
+import gymnasium as gym
 import jax
 import numpy as np
 
 
 def evaluate(
     model_path: str,
     make_env: Callable,
@@ -16,15 +16,15 @@
     run_name: str,
     Model: nn.Module,
     epsilon: float = 0.05,
     capture_video: bool = True,
     seed=1,
 ):
     envs = gym.vector.SyncVectorEnv([make_env(env_id, 0, 0, capture_video, run_name)])
-    obs = envs.reset()
+    obs, _ = envs.reset()
     model = Model(action_dim=envs.single_action_space.n)
     q_key = jax.random.PRNGKey(seed)
     params = model.init(q_key, obs)
     with open(model_path, "rb") as f:
         params = flax.serialization.from_bytes(params, f.read())
     model.apply = jax.jit(model.apply)
 
@@ -32,17 +32,19 @@
     while len(episodic_returns) < eval_episodes:
         if random.random() < epsilon:
             actions = np.array([envs.single_action_space.sample() for _ in range(envs.num_envs)])
         else:
             q_values = model.apply(params, obs)
             actions = q_values.argmax(axis=-1)
             actions = jax.device_get(actions)
-        next_obs, _, _, infos = envs.step(actions)
-        for info in infos:
-            if "episode" in info.keys():
+        next_obs, _, _, _, infos = envs.step(actions)
+        if "final_info" in infos:
+            for info in infos["final_info"]:
+                if "episode" not in info:
+                    continue
                 print(f"eval_episode={len(episodic_returns)}, episodic_return={info['episode']['r']}")
                 episodic_returns += [info["episode"]["r"]]
         obs = next_obs
 
     return episodic_returns
```

### Comparing `cleanrl-1.1.0/cleanrl_utils/evals/ppo_envpool_jax_eval.py` & `cleanrl-1.2.0/cleanrl_utils/evals/ppo_envpool_jax_eval.py`

 * *Files identical despite different names*

### Comparing `cleanrl-1.1.0/cleanrl_utils/huggingface.py` & `cleanrl-1.2.0/cleanrl_utils/huggingface.py`

 * *Files identical despite different names*

### Comparing `cleanrl-1.1.0/cleanrl_utils/paper_plot.py` & `cleanrl-1.2.0/cleanrl_utils/paper_plot.py`

 * *Files identical despite different names*

### Comparing `cleanrl-1.1.0/cleanrl_utils/plot.py` & `cleanrl-1.2.0/cleanrl_utils/plot.py`

 * *Files identical despite different names*

### Comparing `cleanrl-1.1.0/cleanrl_utils/plot_individual.py` & `cleanrl-1.2.0/cleanrl_utils/plot_individual.py`

 * *Files identical despite different names*

### Comparing `cleanrl-1.1.0/cleanrl_utils/reproduce.py` & `cleanrl-1.2.0/cleanrl_utils/reproduce.py`

 * *Files identical despite different names*

### Comparing `cleanrl-1.1.0/cleanrl_utils/resume.py` & `cleanrl-1.2.0/cleanrl_utils/resume.py`

 * *Files identical despite different names*

### Comparing `cleanrl-1.1.0/cleanrl_utils/submit_exp.py` & `cleanrl-1.2.0/cleanrl_utils/submit_exp.py`

 * *Files identical despite different names*

### Comparing `cleanrl-1.1.0/cleanrl_utils/tuner.py` & `cleanrl-1.2.0/cleanrl_utils/tuner.py`

 * *Files identical despite different names*

### Comparing `cleanrl-1.1.0/setup.py` & `cleanrl-1.2.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,89 +4,92 @@
 packages = \
 ['cleanrl',
  'cleanrl.ppo_continuous_action_isaacgym',
  'cleanrl_utils',
  'cleanrl_utils.evals']
 
 package_data = \
-{'': ['*'],
- 'cleanrl.ppo_continuous_action_isaacgym': ['isaacgym/poetry.lock',
-                                            'isaacgym/poetry.lock',
-                                            'isaacgym/pyproject.toml',
-                                            'isaacgym/pyproject.toml']}
+{'': ['*'], 'cleanrl.ppo_continuous_action_isaacgym': ['isaacgym/*']}
 
 install_requires = \
 ['gym==0.23.1',
- 'gymnasium>=0.26.3,<0.27.0',
+ 'gymnasium>=0.28.1',
  'huggingface-hub>=0.11.1,<0.12.0',
  'moviepy>=1.0.3,<2.0.0',
  'pygame==2.1.0',
  'stable-baselines3==1.2.0',
  'tensorboard>=2.10.0,<3.0.0',
  'torch>=1.12.1',
- 'wandb>=0.13.6,<0.14.0']
+ 'wandb>=0.13.11,<0.14.0']
 
 extras_require = \
-{':extra == "atari" or extra == "dqn-atari" or extra == "dqn-atari-jax" or extra == "c51-atari" or extra == "c51-atari-jax" or extra == "ppo-atari-envpool-xla-jax-scan"': ['AutoROM[accept-rom-license]>=0.4.2,<0.5.0'],
- 'atari': ['ale-py==0.7.4', 'opencv-python>=4.6.0.66,<5.0.0.0'],
- 'c51-atari': ['ale-py==0.7.4', 'opencv-python>=4.6.0.66,<5.0.0.0'],
+{'atari': ['ale-py==0.7.4',
+           'AutoROM[accept-rom-license]>=0.4.2,<0.5.0',
+           'opencv-python>=4.6.0.66,<5.0.0.0'],
+ 'c51-atari': ['ale-py==0.7.4',
+               'AutoROM[accept-rom-license]>=0.4.2,<0.5.0',
+               'opencv-python>=4.6.0.66,<5.0.0.0'],
  'c51-atari-jax': ['ale-py==0.7.4',
+                   'AutoROM[accept-rom-license]>=0.4.2,<0.5.0',
                    'opencv-python>=4.6.0.66,<5.0.0.0',
                    'jax>=0.3.17,<0.4.0',
                    'jaxlib>=0.3.15,<0.4.0',
                    'flax>=0.6.0,<0.7.0'],
  'c51-jax': ['jax>=0.3.17,<0.4.0',
              'jaxlib>=0.3.15,<0.4.0',
              'flax>=0.6.0,<0.7.0'],
  'cloud': ['boto3>=1.24.70,<2.0.0', 'awscli>=1.25.71,<2.0.0'],
- 'dm-control': ['mujoco>=2.2,<3.0',
-                'shimmy>=0.1.0,<0.2.0',
-                'dm-control>=1.0.8,<2.0.0'],
- 'docs': ['mkdocs-material>=8.4.3,<9.0.0', 'markdown-include>=0.7.0,<0.8.0'],
- 'dqn-atari': ['ale-py==0.7.4', 'opencv-python>=4.6.0.66,<5.0.0.0'],
+ 'dm-control': ['mujoco<=2.3.3', 'shimmy[dm-control]>=1.0.0'],
+ 'docs': ['mkdocs-material>=8.4.3,<9.0.0',
+          'markdown-include>=0.7.0,<0.8.0',
+          'openrlbenchmark>=0.1.1b4,<0.2.0'],
+ 'dqn-atari': ['ale-py==0.7.4',
+               'AutoROM[accept-rom-license]>=0.4.2,<0.5.0',
+               'opencv-python>=4.6.0.66,<5.0.0.0'],
  'dqn-atari-jax': ['ale-py==0.7.4',
+                   'AutoROM[accept-rom-license]>=0.4.2,<0.5.0',
                    'opencv-python>=4.6.0.66,<5.0.0.0',
                    'jax>=0.3.17,<0.4.0',
                    'jaxlib>=0.3.15,<0.4.0',
                    'flax>=0.6.0,<0.7.0'],
  'dqn-jax': ['jax>=0.3.17,<0.4.0',
              'jaxlib>=0.3.15,<0.4.0',
              'flax>=0.6.0,<0.7.0'],
  'envpool': ['envpool>=0.6.4,<0.7.0'],
  'jax': ['jax>=0.3.17,<0.4.0', 'jaxlib>=0.3.15,<0.4.0', 'flax>=0.6.0,<0.7.0'],
- 'mujoco': ['mujoco>=2.2,<3.0', 'imageio>=2.14.1,<3.0.0'],
+ 'mujoco': ['mujoco<=2.3.3', 'imageio>=2.14.1,<3.0.0'],
  'mujoco-py': ['free-mujoco-py>=2.1.6,<3.0.0'],
  'optuna': ['optuna>=3.0.1,<4.0.0',
             'optuna-dashboard>=0.7.2,<0.8.0',
             'rich<12.0'],
  'pettingzoo': ['PettingZoo==1.18.1',
                 'SuperSuit==3.4.0',
                 'multi-agent-ale-py==0.1.11'],
  'ppo-atari-envpool-xla-jax-scan': ['ale-py==0.7.4',
+                                    'AutoROM[accept-rom-license]>=0.4.2,<0.5.0',
                                     'opencv-python>=4.6.0.66,<5.0.0.0',
                                     'jax>=0.3.17,<0.4.0',
                                     'jaxlib>=0.3.15,<0.4.0',
                                     'flax>=0.6.0,<0.7.0',
                                     'envpool>=0.6.4,<0.7.0'],
  'procgen': ['procgen>=0.10.7,<0.11.0'],
- 'pybullet': ['pybullet==3.1.8'],
  'pytest': ['pytest>=7.1.3,<8.0.0']}
 
 setup_kwargs = {
     'name': 'cleanrl',
-    'version': '1.1.0',
+    'version': '1.2.0',
     'description': 'High-quality single file implementation of Deep Reinforcement Learning algorithms with research-friendly features',
-    'long_description': '# CleanRL (Clean Implementation of RL Algorithms)\n\n\n[<img src="https://img.shields.io/badge/license-MIT-blue">](https://github.com/vwxyzjn/cleanrl)\n[![tests](https://github.com/vwxyzjn/cleanrl/actions/workflows/tests.yaml/badge.svg)](https://github.com/vwxyzjn/cleanrl/actions/workflows/tests.yaml)\n[![docs](https://img.shields.io/github/deployments/vwxyzjn/cleanrl/Production?label=docs&logo=vercel)](https://docs.cleanrl.dev/)\n[<img src="https://img.shields.io/discord/767863440248143916?label=discord">](https://discord.gg/D6RCjA6sVT)\n[<img src="https://img.shields.io/youtube/channel/views/UCDdC6BIFRI0jvcwuhi3aI6w?style=social">](https://www.youtube.com/channel/UCDdC6BIFRI0jvcwuhi3aI6w/videos)\n[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)\n[![Imports: isort](https://img.shields.io/badge/%20imports-isort-%231674b1?style=flat&labelColor=ef8336)](https://pycqa.github.io/isort/)\n[<img src="https://img.shields.io/badge/%F0%9F%A4%97%20Models-Huggingface-F8D521">](https://huggingface.co/cleanrl)\n[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/vwxyzjn/cleanrl/blob/hf-integration/docs/get-started/CleanRL_Huggingface_Integration_Demo.ipynb)\n\n\nCleanRL is a Deep Reinforcement Learning library that provides high-quality single-file implementation with research-friendly features. The implementation is clean and simple, yet we can scale it to run thousands of experiments using AWS Batch. The highlight features of CleanRL are:\n\n\n\n* 📜 Single-file implementation\n   * *Every detail about an algorithm variant is put into a single standalone file.* \n   * For example, our `ppo_atari.py` only has 340 lines of code but contains all implementation details on how PPO works with Atari games, **so it is a great reference implementation to read for folks who do not wish to read an entire modular library**.\n* 📊 Benchmarked Implementation (7+ algorithms and 34+ games at https://benchmark.cleanrl.dev)\n* 📈 Tensorboard Logging\n* 🪛 Local Reproducibility via Seeding\n* 🎮 Videos of Gameplay Capturing\n* 🧫 Experiment Management with [Weights and Biases](https://wandb.ai/site)\n* 💸 Cloud Integration with docker and AWS \n\nYou can read more about CleanRL in our [JMLR paper](https://www.jmlr.org/papers/volume23/21-1342/21-1342.pdf) and [documentation](https://docs.cleanrl.dev/).\n\nCleanRL only contains implementations of **online** deep reinforcement learning algorithms. If you are looking for **offline** algorithms, please check out [tinkoff-ai/CORL](https://github.com/tinkoff-ai/CORL), which shares a similar design philosophy as CleanRL.\n\n> ℹ️ **Support for Gymnasium**: [Farama-Foundation/Gymnasium](https://github.com/Farama-Foundation/Gymnasium) is the next generation of [`openai/gym`](https://github.com/openai/gym) that will continue to be maintained and introduce new features. Please see their [announcement](https://farama.org/Announcing-The-Farama-Foundation) for further detail. We are migrating to `gymnasium` and the progress can be tracked in [vwxyzjn/cleanrl#277](https://github.com/vwxyzjn/cleanrl/pull/277).\n\n\n\n> ⚠️ **NOTE**: CleanRL is *not* a modular library and therefore it is not meant to be imported. At the cost of duplicate code, we make all implementation details of a DRL algorithm variant easy to understand, so CleanRL comes with its own pros and cons. You should consider using CleanRL if you want to 1) understand all implementation details of an algorithm\'s varaint or 2) prototype advanced features that other modular DRL libraries do not support (CleanRL has minimal lines of code so it gives you great debugging experience and you don\'t have do a lot of subclassing like sometimes in modular DRL libraries).\n\n## Get started\n\nPrerequisites:\n* Python >=3.7.1,<3.10 (not yet 3.10)\n* [Poetry 1.2.1+](https://python-poetry.org)\n\nTo run experiments locally, give the following a try:\n\n```bash\ngit clone https://github.com/vwxyzjn/cleanrl.git && cd cleanrl\npoetry install\n\n# alternatively, you could use `poetry shell` and do\n# `python run cleanrl/ppo.py`\npoetry run python cleanrl/ppo.py \\\n    --seed 1 \\\n    --env-id CartPole-v0 \\\n    --total-timesteps 50000\n\n# open another temrminal and enter `cd cleanrl/cleanrl`\ntensorboard --logdir runs\n```\n\nTo use experiment tracking with wandb, run\n```bash\nwandb login # only required for the first time\npoetry run python cleanrl/ppo.py \\\n    --seed 1 \\\n    --env-id CartPole-v0 \\\n    --total-timesteps 50000 \\\n    --track \\\n    --wandb-project-name cleanrltest\n```\n\nTo run training scripts in other games:\n```\npoetry shell\n\n# classic control\npython cleanrl/dqn.py --env-id CartPole-v1\npython cleanrl/ppo.py --env-id CartPole-v1\npython cleanrl/c51.py --env-id CartPole-v1\n\n# atari\npoetry install --with atari\npython cleanrl/dqn_atari.py --env-id BreakoutNoFrameskip-v4\npython cleanrl/c51_atari.py --env-id BreakoutNoFrameskip-v4\npython cleanrl/ppo_atari.py --env-id BreakoutNoFrameskip-v4\n\n# NEW: 3-4x side-effects free speed up with envpool\'s atari (only available to linux)\npoetry install --with envpool\npython cleanrl/ppo_atari_envpool.py --env-id BreakoutNoFrameskip-v4\n# Learn Pong-v5 in ~5-10 mins\n# Side effects such as lower sample efficiency might occur\npoetry run python ppo_atari_envpool.py --clip-coef=0.2 --num-envs=16 --num-minibatches=8 --num-steps=128 --update-epochs=3\n\n# pybullet\npoetry install --with pybullet\npython cleanrl/td3_continuous_action.py --env-id MinitaurBulletDuckEnv-v0\npython cleanrl/ddpg_continuous_action.py --env-id MinitaurBulletDuckEnv-v0\npython cleanrl/sac_continuous_action.py --env-id MinitaurBulletDuckEnv-v0\n\n# procgen\npoetry install --with procgen\npython cleanrl/ppo_procgen.py --env-id starpilot\npython cleanrl/ppg_procgen.py --env-id starpilot\n\n# ppo + lstm\npython cleanrl/ppo_atari_lstm.py --env-id BreakoutNoFrameskip-v4\npython cleanrl/ppo_memory_env_lstm.py\n```\n\nYou may also use a prebuilt development environment hosted in Gitpod:\n\n[![Open in Gitpod](https://gitpod.io/button/open-in-gitpod.svg)](https://gitpod.io/#https://github.com/vwxyzjn/cleanrl)\n\n## Algorithms Implemented\n\n\n| Algorithm      | Variants Implemented |\n| ----------- | ----------- |\n| ✅ [Proximal Policy Gradient (PPO)](https://arxiv.org/pdf/1707.06347.pdf)  |  [`ppo.py`](https://github.com/vwxyzjn/cleanrl/blob/master/cleanrl/ppo.py),   [docs](https://docs.cleanrl.dev/rl-algorithms/ppo/#ppopy) |\n| |  [`ppo_atari.py`](https://github.com/vwxyzjn/cleanrl/blob/master/cleanrl/ppo_atari.py),   [docs](https://docs.cleanrl.dev/rl-algorithms/ppo/#ppo_ataripy)\n| |  [`ppo_continuous_action.py`](https://github.com/vwxyzjn/cleanrl/blob/master/cleanrl/ppo_continuous_action.py),   [docs](https://docs.cleanrl.dev/rl-algorithms/ppo/#ppo_continuous_actionpy)\n| |  [`ppo_atari_lstm.py`](https://github.com/vwxyzjn/cleanrl/blob/master/cleanrl/ppo_atari_lstm.py),   [docs](https://docs.cleanrl.dev/rl-algorithms/ppo/#ppo_atari_lstmpy)\n| |  [`ppo_atari_envpool.py`](https://github.com/vwxyzjn/cleanrl/blob/master/cleanrl/ppo_atari_envpool.py),   [docs](https://docs.cleanrl.dev/rl-algorithms/ppo/#ppo_atari_envpoolpy)\n| | [`ppo_atari_envpool_xla_jax.py`](https://github.com/vwxyzjn/cleanrl/blob/master/cleanrl/ppo_atari_envpool_xla_jax.py), [docs](https://docs.cleanrl.dev/rl-algorithms/ppo/#ppo_atari_envpool_xla_jaxpy)\n| | [`ppo_atari_envpool_xla_jax_scan.py`](https://github.com/vwxyzjn/cleanrl/blob/master/cleanrl/ppo_atari_envpool_xla_jax_scan.py), [docs](https://docs.cleanrl.dev/rl-algorithms/ppo/#ppo_atari_envpool_xla_jax_scanpy))\n| |  [`ppo_procgen.py`](https://github.com/vwxyzjn/cleanrl/blob/master/cleanrl/ppo_procgen.py),   [docs](https://docs.cleanrl.dev/rl-algorithms/ppo/#ppo_procgenpy)\n| |  [`ppo_atari_multigpu.py`](https://github.com/vwxyzjn/cleanrl/blob/master/cleanrl/ppo_atari_multigpu.py),  [docs](https://docs.cleanrl.dev/rl-algorithms/ppo/#ppo_atari_multigpupy)\n| | [`ppo_pettingzoo_ma_atari.py`](https://github.com/vwxyzjn/cleanrl/blob/master/cleanrl/ppo_pettingzoo_ma_atari.py),  [docs](https://docs.cleanrl.dev/rl-algorithms/ppo/#ppo_pettingzoo_ma_ataripy)\n| | [`ppo_continuous_action_isaacgym.py`](https://github.com/vwxyzjn/cleanrl/blob/master/cleanrl/ppo_continuous_action_isaacgym/ppo_continuous_action_isaacgym.py),  [docs](https://docs.cleanrl.dev/rl-algorithms/ppo/#ppo_continuous_action_isaacgympy)\n| ✅ [Deep Q-Learning (DQN)](https://web.stanford.edu/class/psych209/Readings/MnihEtAlHassibis15NatureControlDeepRL.pdf) |  [`dqn.py`](https://github.com/vwxyzjn/cleanrl/blob/master/cleanrl/dqn.py),  [docs](https://docs.cleanrl.dev/rl-algorithms/dqn/#dqnpy) |\n| |  [`dqn_atari.py`](https://github.com/vwxyzjn/cleanrl/blob/master/cleanrl/dqn_atari.py),  [docs](https://docs.cleanrl.dev/rl-algorithms/dqn/#dqn_ataripy) |\n| | [`dqn_jax.py`](https://github.com/vwxyzjn/cleanrl/blob/master/cleanrl/dqn_jax.py), [docs](https://docs.cleanrl.dev/rl-algorithms/dqn/#dqn_jaxpy) |\n| | [`dqn_atari_jax.py`](https://github.com/vwxyzjn/cleanrl/blob/master/cleanrl/dqn_atari_jax.py), [docs](https://docs.cleanrl.dev/rl-algorithms/dqn/#dqn_atari_jaxpy) |\n| ✅ [Categorical DQN (C51)](https://arxiv.org/pdf/1707.06887.pdf) |  [`c51.py`](https://github.com/vwxyzjn/cleanrl/blob/master/cleanrl/c51.py),  [docs](https://docs.cleanrl.dev/rl-algorithms/c51/#c51py) |\n| |  [`c51_atari.py`](https://github.com/vwxyzjn/cleanrl/blob/master/cleanrl/c51_atari.py),  [docs](https://docs.cleanrl.dev/rl-algorithms/c51/#c51_ataripy) |\n| | [`c51_jax.py`](https://github.com/vwxyzjn/cleanrl/blob/master/cleanrl/c51_jax.py), [docs](https://docs.cleanrl.dev/rl-algorithms/c51/#c51_jaxpy) |\n| | [`c51_atari_jax.py`](https://github.com/vwxyzjn/cleanrl/blob/master/cleanrl/c51_atari_jax.py), [docs](https://docs.cleanrl.dev/rl-algorithms/c51/#c51_atari_jaxpy) |\n| ✅ [Soft Actor-Critic (SAC)](https://arxiv.org/pdf/1812.05905.pdf) |  [`sac_continuous_action.py`](https://github.com/vwxyzjn/cleanrl/blob/master/cleanrl/sac_continuous_action.py),  [docs](https://docs.cleanrl.dev/rl-algorithms/sac/#sac_continuous_actionpy) |\n| ✅ [Deep Deterministic Policy Gradient (DDPG)](https://arxiv.org/pdf/1509.02971.pdf) |  [`ddpg_continuous_action.py`](https://github.com/vwxyzjn/cleanrl/blob/master/cleanrl/ddpg_continuous_action.py),  [docs](https://docs.cleanrl.dev/rl-algorithms/ddpg/#ddpg_continuous_actionpy) |\n| | [`ddpg_continuous_action_jax.py`](https://github.com/vwxyzjn/cleanrl/blob/master/cleanrl/ddpg_continuous_action_jax.py),  [docs](https://docs.cleanrl.dev/rl-algorithms/ddpg/#ddpg_continuous_action_jaxpy)\n| ✅ [Twin Delayed Deep Deterministic Policy Gradient (TD3)](https://arxiv.org/pdf/1802.09477.pdf) |  [`td3_continuous_action.py`](https://github.com/vwxyzjn/cleanrl/blob/master/cleanrl/td3_continuous_action.py),  [docs](https://docs.cleanrl.dev/rl-algorithms/td3/#td3_continuous_actionpy) |\n|  | [`td3_continuous_action_jax.py`](https://github.com/vwxyzjn/cleanrl/blob/master/cleanrl/td3_continuous_action_jax.py),  [docs](https://docs.cleanrl.dev/rl-algorithms/td3/#td3_continuous_action_jaxpy) |\n| ✅ [Phasic Policy Gradient (PPG)](https://arxiv.org/abs/2009.04416) |  [`ppg_procgen.py`](https://github.com/vwxyzjn/cleanrl/blob/master/cleanrl/ppg_procgen.py),  [docs](https://docs.cleanrl.dev/rl-algorithms/ppg/#ppg_procgenpy) |\n| ✅ [Random Network Distillation (RND)](https://arxiv.org/abs/1810.12894) |  [`ppo_rnd_envpool.py`](https://github.com/vwxyzjn/cleanrl/blob/master/cleanrl/ppo_rnd_envpool.py),  [docs](/rl-algorithms/ppo-rnd/#ppo_rnd_envpoolpy) |\n\n\n## Open RL Benchmark\n\nTo make our experimental data transparent, CleanRL participates in a related project called [Open RL Benchmark](https://github.com/openrlbenchmark/openrlbenchmark), which contains tracked experiments from popular DRL libraries such as ours, [Stable-baselines3](https://github.com/DLR-RM/stable-baselines3), [openai/baselines](https://github.com/openai/baselines), [jaxrl](https://github.com/ikostrikov/jaxrl), and others. \n\nCheck out https://benchmark.cleanrl.dev/ for a collection of Weights and Biases reports showcasing tracked DRL experiments. The reports are interactive, and researchers can easily query information such as GPU utilization and videos of an agent\'s gameplay that are normally hard to acquire in other RL benchmarks. In the future, Open RL Benchmark will likely provide an dataset API for researchers to easily access the data (see [repo](https://github.com/openrlbenchmark/openrlbenchmark)).\n\n![](docs/static/o1.png)\n![](docs/static/o2.png)\n![](docs/static/o3.png)\n\n\n## Support and get involved\n\nWe have a [Discord Community](https://discord.gg/D6RCjA6sVT) for support. Feel free to ask questions. Posting in [Github Issues](https://github.com/vwxyzjn/cleanrl/issues) and PRs are also welcome. Also our past video recordings are available at [YouTube](https://www.youtube.com/watch?v=dm4HdGujpPs&list=PLQpKd36nzSuMynZLU2soIpNSMeXMplnKP&index=2)\n\n## Citing CleanRL\n\nIf you use CleanRL in your work, please cite our technical [paper](https://www.jmlr.org/papers/v23/21-1342.html):\n\n```bibtex\n@article{huang2022cleanrl,\n  author  = {Shengyi Huang and Rousslan Fernand Julien Dossa and Chang Ye and Jeff Braga and Dipam Chakraborty and Kinal Mehta and João G.M. Araújo},\n  title   = {CleanRL: High-quality Single-file Implementations of Deep Reinforcement Learning Algorithms},\n  journal = {Journal of Machine Learning Research},\n  year    = {2022},\n  volume  = {23},\n  number  = {274},\n  pages   = {1--18},\n  url     = {http://jmlr.org/papers/v23/21-1342.html}\n}\n```\n',
+    'long_description': '# CleanRL (Clean Implementation of RL Algorithms)\n\n\n[<img src="https://img.shields.io/badge/license-MIT-blue">](https://github.com/vwxyzjn/cleanrl)\n[![tests](https://github.com/vwxyzjn/cleanrl/actions/workflows/tests.yaml/badge.svg)](https://github.com/vwxyzjn/cleanrl/actions/workflows/tests.yaml)\n[![docs](https://img.shields.io/github/deployments/vwxyzjn/cleanrl/Production?label=docs&logo=vercel)](https://docs.cleanrl.dev/)\n[<img src="https://img.shields.io/discord/767863440248143916?label=discord">](https://discord.gg/D6RCjA6sVT)\n[<img src="https://img.shields.io/youtube/channel/views/UCDdC6BIFRI0jvcwuhi3aI6w?style=social">](https://www.youtube.com/channel/UCDdC6BIFRI0jvcwuhi3aI6w/videos)\n[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)\n[![Imports: isort](https://img.shields.io/badge/%20imports-isort-%231674b1?style=flat&labelColor=ef8336)](https://pycqa.github.io/isort/)\n[<img src="https://img.shields.io/badge/%F0%9F%A4%97%20Models-Huggingface-F8D521">](https://huggingface.co/cleanrl)\n[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/vwxyzjn/cleanrl/blob/master/docs/get-started/CleanRL_Huggingface_Integration_Demo.ipynb)\n\n\nCleanRL is a Deep Reinforcement Learning library that provides high-quality single-file implementation with research-friendly features. The implementation is clean and simple, yet we can scale it to run thousands of experiments using AWS Batch. The highlight features of CleanRL are:\n\n\n\n* 📜 Single-file implementation\n   * *Every detail about an algorithm variant is put into a single standalone file.* \n   * For example, our `ppo_atari.py` only has 340 lines of code but contains all implementation details on how PPO works with Atari games, **so it is a great reference implementation to read for folks who do not wish to read an entire modular library**.\n* 📊 Benchmarked Implementation (7+ algorithms and 34+ games at https://benchmark.cleanrl.dev)\n* 📈 Tensorboard Logging\n* 🪛 Local Reproducibility via Seeding\n* 🎮 Videos of Gameplay Capturing\n* 🧫 Experiment Management with [Weights and Biases](https://wandb.ai/site)\n* 💸 Cloud Integration with docker and AWS \n\nYou can read more about CleanRL in our [JMLR paper](https://www.jmlr.org/papers/volume23/21-1342/21-1342.pdf) and [documentation](https://docs.cleanrl.dev/).\n\nCleanRL only contains implementations of **online** deep reinforcement learning algorithms. If you are looking for **offline** algorithms, please check out [tinkoff-ai/CORL](https://github.com/tinkoff-ai/CORL), which shares a similar design philosophy as CleanRL.\n\n> ℹ️ **Support for Gymnasium**: [Farama-Foundation/Gymnasium](https://github.com/Farama-Foundation/Gymnasium) is the next generation of [`openai/gym`](https://github.com/openai/gym) that will continue to be maintained and introduce new features. Please see their [announcement](https://farama.org/Announcing-The-Farama-Foundation) for further detail. We are migrating to `gymnasium` and the progress can be tracked in [vwxyzjn/cleanrl#277](https://github.com/vwxyzjn/cleanrl/pull/277). \n\n\n> ⚠️ **NOTE**: CleanRL is *not* a modular library and therefore it is not meant to be imported. At the cost of duplicate code, we make all implementation details of a DRL algorithm variant easy to understand, so CleanRL comes with its own pros and cons. You should consider using CleanRL if you want to 1) understand all implementation details of an algorithm\'s varaint or 2) prototype advanced features that other modular DRL libraries do not support (CleanRL has minimal lines of code so it gives you great debugging experience and you don\'t have do a lot of subclassing like sometimes in modular DRL libraries).\n\n## Get started\n\nPrerequisites:\n* Python >=3.7.1,<3.11\n* [Poetry 1.2.1+](https://python-poetry.org)\n\nTo run experiments locally, give the following a try:\n\n```bash\ngit clone https://github.com/vwxyzjn/cleanrl.git && cd cleanrl\npoetry install\n\n# alternatively, you could use `poetry shell` and do\n# `python run cleanrl/ppo.py`\npoetry run python cleanrl/ppo.py \\\n    --seed 1 \\\n    --env-id CartPole-v0 \\\n    --total-timesteps 50000\n\n# open another temrminal and enter `cd cleanrl/cleanrl`\ntensorboard --logdir runs\n```\n\nTo use experiment tracking with wandb, run\n```bash\nwandb login # only required for the first time\npoetry run python cleanrl/ppo.py \\\n    --seed 1 \\\n    --env-id CartPole-v0 \\\n    --total-timesteps 50000 \\\n    --track \\\n    --wandb-project-name cleanrltest\n```\n\nIf you are not using `poetry`, you can install CleanRL with `requirements.txt`:\n\n```bash\n# core dependencies\npip install -r requirements/requirements.txt\n\n# optional dependencies\npip install -r requirements/requirements-atari.txt\npip install -r requirements/requirements-mujoco.txt\npip install -r requirements/requirements-mujoco_py.txt\npip install -r requirements/requirements-procgen.txt\npip install -r requirements/requirements-envpool.txt\npip install -r requirements/requirements-pettingzoo.txt\npip install -r requirements/requirements-jax.txt\npip install -r requirements/requirements-docs.txt\npip install -r requirements/requirements-cloud.txt\n```\n\nTo run training scripts in other games:\n```\npoetry shell\n\n# classic control\npython cleanrl/dqn.py --env-id CartPole-v1\npython cleanrl/ppo.py --env-id CartPole-v1\npython cleanrl/c51.py --env-id CartPole-v1\n\n# atari\npoetry install -E atari\npython cleanrl/dqn_atari.py --env-id BreakoutNoFrameskip-v4\npython cleanrl/c51_atari.py --env-id BreakoutNoFrameskip-v4\npython cleanrl/ppo_atari.py --env-id BreakoutNoFrameskip-v4\npython cleanrl/sac_atari.py --env-id BreakoutNoFrameskip-v4\n\n# NEW: 3-4x side-effects free speed up with envpool\'s atari (only available to linux)\npoetry install -E envpool\npython cleanrl/ppo_atari_envpool.py --env-id BreakoutNoFrameskip-v4\n# Learn Pong-v5 in ~5-10 mins\n# Side effects such as lower sample efficiency might occur\npoetry run python ppo_atari_envpool.py --clip-coef=0.2 --num-envs=16 --num-minibatches=8 --num-steps=128 --update-epochs=3\n\n# procgen\npoetry install -E procgen\npython cleanrl/ppo_procgen.py --env-id starpilot\npython cleanrl/ppg_procgen.py --env-id starpilot\n\n# ppo + lstm\npoetry install -E atari\npython cleanrl/ppo_atari_lstm.py --env-id BreakoutNoFrameskip-v4\n```\n\nYou may also use a prebuilt development environment hosted in Gitpod:\n\n[![Open in Gitpod](https://gitpod.io/button/open-in-gitpod.svg)](https://gitpod.io/#https://github.com/vwxyzjn/cleanrl)\n\n## Algorithms Implemented\n\n\n| Algorithm      | Variants Implemented |\n| ----------- | ----------- |\n| ✅ [Proximal Policy Gradient (PPO)](https://arxiv.org/pdf/1707.06347.pdf)  |  [`ppo.py`](https://github.com/vwxyzjn/cleanrl/blob/master/cleanrl/ppo.py),   [docs](https://docs.cleanrl.dev/rl-algorithms/ppo/#ppopy) |\n| |  [`ppo_atari.py`](https://github.com/vwxyzjn/cleanrl/blob/master/cleanrl/ppo_atari.py),   [docs](https://docs.cleanrl.dev/rl-algorithms/ppo/#ppo_ataripy)\n| |  [`ppo_continuous_action.py`](https://github.com/vwxyzjn/cleanrl/blob/master/cleanrl/ppo_continuous_action.py),   [docs](https://docs.cleanrl.dev/rl-algorithms/ppo/#ppo_continuous_actionpy)\n| |  [`ppo_atari_lstm.py`](https://github.com/vwxyzjn/cleanrl/blob/master/cleanrl/ppo_atari_lstm.py),   [docs](https://docs.cleanrl.dev/rl-algorithms/ppo/#ppo_atari_lstmpy)\n| |  [`ppo_atari_envpool.py`](https://github.com/vwxyzjn/cleanrl/blob/master/cleanrl/ppo_atari_envpool.py),   [docs](https://docs.cleanrl.dev/rl-algorithms/ppo/#ppo_atari_envpoolpy)\n| | [`ppo_atari_envpool_xla_jax.py`](https://github.com/vwxyzjn/cleanrl/blob/master/cleanrl/ppo_atari_envpool_xla_jax.py), [docs](https://docs.cleanrl.dev/rl-algorithms/ppo/#ppo_atari_envpool_xla_jaxpy)\n| | [`ppo_atari_envpool_xla_jax_scan.py`](https://github.com/vwxyzjn/cleanrl/blob/master/cleanrl/ppo_atari_envpool_xla_jax_scan.py), [docs](https://docs.cleanrl.dev/rl-algorithms/ppo/#ppo_atari_envpool_xla_jax_scanpy))\n| |  [`ppo_procgen.py`](https://github.com/vwxyzjn/cleanrl/blob/master/cleanrl/ppo_procgen.py),   [docs](https://docs.cleanrl.dev/rl-algorithms/ppo/#ppo_procgenpy)\n| |  [`ppo_atari_multigpu.py`](https://github.com/vwxyzjn/cleanrl/blob/master/cleanrl/ppo_atari_multigpu.py),  [docs](https://docs.cleanrl.dev/rl-algorithms/ppo/#ppo_atari_multigpupy)\n| | [`ppo_pettingzoo_ma_atari.py`](https://github.com/vwxyzjn/cleanrl/blob/master/cleanrl/ppo_pettingzoo_ma_atari.py),  [docs](https://docs.cleanrl.dev/rl-algorithms/ppo/#ppo_pettingzoo_ma_ataripy)\n| | [`ppo_continuous_action_isaacgym.py`](https://github.com/vwxyzjn/cleanrl/blob/master/cleanrl/ppo_continuous_action_isaacgym/ppo_continuous_action_isaacgym.py),  [docs](https://docs.cleanrl.dev/rl-algorithms/ppo/#ppo_continuous_action_isaacgympy)\n| ✅ [Deep Q-Learning (DQN)](https://web.stanford.edu/class/psych209/Readings/MnihEtAlHassibis15NatureControlDeepRL.pdf) |  [`dqn.py`](https://github.com/vwxyzjn/cleanrl/blob/master/cleanrl/dqn.py),  [docs](https://docs.cleanrl.dev/rl-algorithms/dqn/#dqnpy) |\n| | [`dqn_atari.py`](https://github.com/vwxyzjn/cleanrl/blob/master/cleanrl/dqn_atari.py),  [docs](https://docs.cleanrl.dev/rl-algorithms/dqn/#dqn_ataripy) |\n| | [`dqn_jax.py`](https://github.com/vwxyzjn/cleanrl/blob/master/cleanrl/dqn_jax.py), [docs](https://docs.cleanrl.dev/rl-algorithms/dqn/#dqn_jaxpy) |\n| | [`dqn_atari_jax.py`](https://github.com/vwxyzjn/cleanrl/blob/master/cleanrl/dqn_atari_jax.py), [docs](https://docs.cleanrl.dev/rl-algorithms/dqn/#dqn_atari_jaxpy) |\n| ✅ [Categorical DQN (C51)](https://arxiv.org/pdf/1707.06887.pdf) |  [`c51.py`](https://github.com/vwxyzjn/cleanrl/blob/master/cleanrl/c51.py),  [docs](https://docs.cleanrl.dev/rl-algorithms/c51/#c51py) |\n| |  [`c51_atari.py`](https://github.com/vwxyzjn/cleanrl/blob/master/cleanrl/c51_atari.py),  [docs](https://docs.cleanrl.dev/rl-algorithms/c51/#c51_ataripy) |\n| | [`c51_jax.py`](https://github.com/vwxyzjn/cleanrl/blob/master/cleanrl/c51_jax.py), [docs](https://docs.cleanrl.dev/rl-algorithms/c51/#c51_jaxpy) |\n| | [`c51_atari_jax.py`](https://github.com/vwxyzjn/cleanrl/blob/master/cleanrl/c51_atari_jax.py), [docs](https://docs.cleanrl.dev/rl-algorithms/c51/#c51_atari_jaxpy) |\n| ✅ [Soft Actor-Critic (SAC)](https://arxiv.org/pdf/1812.05905.pdf) |  [`sac_continuous_action.py`](https://github.com/vwxyzjn/cleanrl/blob/master/cleanrl/sac_continuous_action.py),  [docs](https://docs.cleanrl.dev/rl-algorithms/sac/#sac_continuous_actionpy) |\n| |  [`sac_atari.py`](https://github.com/vwxyzjn/cleanrl/blob/master/cleanrl/sac_atari.py),  [docs](https://docs.cleanrl.dev/rl-algorithms/sac/#sac_atarinpy) |\n| ✅ [Deep Deterministic Policy Gradient (DDPG)](https://arxiv.org/pdf/1509.02971.pdf) |  [`ddpg_continuous_action.py`](https://github.com/vwxyzjn/cleanrl/blob/master/cleanrl/ddpg_continuous_action.py),  [docs](https://docs.cleanrl.dev/rl-algorithms/ddpg/#ddpg_continuous_actionpy) |\n| | [`ddpg_continuous_action_jax.py`](https://github.com/vwxyzjn/cleanrl/blob/master/cleanrl/ddpg_continuous_action_jax.py),  [docs](https://docs.cleanrl.dev/rl-algorithms/ddpg/#ddpg_continuous_action_jaxpy)\n| ✅ [Twin Delayed Deep Deterministic Policy Gradient (TD3)](https://arxiv.org/pdf/1802.09477.pdf) |  [`td3_continuous_action.py`](https://github.com/vwxyzjn/cleanrl/blob/master/cleanrl/td3_continuous_action.py),  [docs](https://docs.cleanrl.dev/rl-algorithms/td3/#td3_continuous_actionpy) |\n|  | [`td3_continuous_action_jax.py`](https://github.com/vwxyzjn/cleanrl/blob/master/cleanrl/td3_continuous_action_jax.py),  [docs](https://docs.cleanrl.dev/rl-algorithms/td3/#td3_continuous_action_jaxpy) |\n| ✅ [Phasic Policy Gradient (PPG)](https://arxiv.org/abs/2009.04416) |  [`ppg_procgen.py`](https://github.com/vwxyzjn/cleanrl/blob/master/cleanrl/ppg_procgen.py),  [docs](https://docs.cleanrl.dev/rl-algorithms/ppg/#ppg_procgenpy) |\n| ✅ [Random Network Distillation (RND)](https://arxiv.org/abs/1810.12894) |  [`ppo_rnd_envpool.py`](https://github.com/vwxyzjn/cleanrl/blob/master/cleanrl/ppo_rnd_envpool.py),  [docs](/rl-algorithms/ppo-rnd/#ppo_rnd_envpoolpy) |\n\n\n## Open RL Benchmark\n\nTo make our experimental data transparent, CleanRL participates in a related project called [Open RL Benchmark](https://github.com/openrlbenchmark/openrlbenchmark), which contains tracked experiments from popular DRL libraries such as ours, [Stable-baselines3](https://github.com/DLR-RM/stable-baselines3), [openai/baselines](https://github.com/openai/baselines), [jaxrl](https://github.com/ikostrikov/jaxrl), and others. \n\nCheck out https://benchmark.cleanrl.dev/ for a collection of Weights and Biases reports showcasing tracked DRL experiments. The reports are interactive, and researchers can easily query information such as GPU utilization and videos of an agent\'s gameplay that are normally hard to acquire in other RL benchmarks. In the future, Open RL Benchmark will likely provide an dataset API for researchers to easily access the data (see [repo](https://github.com/openrlbenchmark/openrlbenchmark)).\n\n![](docs/static/o1.png)\n![](docs/static/o2.png)\n![](docs/static/o3.png)\n\n\n## Support and get involved\n\nWe have a [Discord Community](https://discord.gg/D6RCjA6sVT) for support. Feel free to ask questions. Posting in [Github Issues](https://github.com/vwxyzjn/cleanrl/issues) and PRs are also welcome. Also our past video recordings are available at [YouTube](https://www.youtube.com/watch?v=dm4HdGujpPs&list=PLQpKd36nzSuMynZLU2soIpNSMeXMplnKP&index=2)\n\n## Citing CleanRL\n\nIf you use CleanRL in your work, please cite our technical [paper](https://www.jmlr.org/papers/v23/21-1342.html):\n\n```bibtex\n@article{huang2022cleanrl,\n  author  = {Shengyi Huang and Rousslan Fernand Julien Dossa and Chang Ye and Jeff Braga and Dipam Chakraborty and Kinal Mehta and João G.M. Araújo},\n  title   = {CleanRL: High-quality Single-file Implementations of Deep Reinforcement Learning Algorithms},\n  journal = {Journal of Machine Learning Research},\n  year    = {2022},\n  volume  = {23},\n  number  = {274},\n  pages   = {1--18},\n  url     = {http://jmlr.org/papers/v23/21-1342.html}\n}\n```\n',
     'author': 'Costa Huang',
     'author_email': 'costa.huang@outlook.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
     'packages': packages,
     'package_data': package_data,
     'install_requires': install_requires,
     'extras_require': extras_require,
-    'python_requires': '>=3.7.1,<3.10',
+    'python_requires': '>=3.7.1,<3.11',
 }
 
 
 setup(**setup_kwargs)
```

### Comparing `cleanrl-1.1.0/PKG-INFO` & `cleanrl-1.2.0/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 Metadata-Version: 2.1
 Name: cleanrl
-Version: 1.1.0
+Version: 1.2.0
 Summary: High-quality single file implementation of Deep Reinforcement Learning algorithms with research-friendly features
 License: MIT
 Keywords: reinforcement,machine,learning,research
 Author: Costa Huang
 Author-email: costa.huang@outlook.com
-Requires-Python: >=3.7.1,<3.10
+Requires-Python: >=3.7.1,<3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Provides-Extra: atari
 Provides-Extra: c51
 Provides-Extra: c51-atari
 Provides-Extra: c51-atari-jax
 Provides-Extra: c51-jax
 Provides-Extra: cloud
 Provides-Extra: dm-control
@@ -28,64 +29,62 @@
 Provides-Extra: mujoco
 Provides-Extra: mujoco-py
 Provides-Extra: optuna
 Provides-Extra: pettingzoo
 Provides-Extra: plot
 Provides-Extra: ppo-atari-envpool-xla-jax-scan
 Provides-Extra: procgen
-Provides-Extra: pybullet
 Provides-Extra: pytest
 Requires-Dist: AutoROM[accept-rom-license] (>=0.4.2,<0.5.0) ; extra == "atari" or extra == "dqn-atari" or extra == "dqn-atari-jax" or extra == "c51-atari" or extra == "c51-atari-jax" or extra == "ppo-atari-envpool-xla-jax-scan"
 Requires-Dist: PettingZoo (==1.18.1) ; extra == "pettingzoo"
 Requires-Dist: SuperSuit (==3.4.0) ; extra == "pettingzoo"
 Requires-Dist: ale-py (==0.7.4) ; extra == "atari" or extra == "dqn-atari" or extra == "dqn-atari-jax" or extra == "c51-atari" or extra == "c51-atari-jax" or extra == "ppo-atari-envpool-xla-jax-scan"
 Requires-Dist: awscli (>=1.25.71,<2.0.0) ; extra == "cloud"
 Requires-Dist: boto3 (>=1.24.70,<2.0.0) ; extra == "cloud"
-Requires-Dist: dm-control (>=1.0.8,<2.0.0) ; extra == "dm-control"
 Requires-Dist: envpool (>=0.6.4,<0.7.0) ; extra == "envpool" or extra == "ppo-atari-envpool-xla-jax-scan"
 Requires-Dist: flax (>=0.6.0,<0.7.0) ; extra == "jax" or extra == "dqn-jax" or extra == "dqn-atari-jax" or extra == "c51-jax" or extra == "c51-atari-jax" or extra == "ppo-atari-envpool-xla-jax-scan"
 Requires-Dist: free-mujoco-py (>=2.1.6,<3.0.0) ; extra == "mujoco-py"
 Requires-Dist: gym (==0.23.1)
-Requires-Dist: gymnasium (>=0.26.3,<0.27.0)
+Requires-Dist: gymnasium (>=0.28.1)
 Requires-Dist: huggingface-hub (>=0.11.1,<0.12.0)
 Requires-Dist: imageio (>=2.14.1,<3.0.0) ; extra == "mujoco"
 Requires-Dist: jax (>=0.3.17,<0.4.0) ; extra == "jax" or extra == "dqn-jax" or extra == "dqn-atari-jax" or extra == "c51-jax" or extra == "c51-atari-jax" or extra == "ppo-atari-envpool-xla-jax-scan"
 Requires-Dist: jaxlib (>=0.3.15,<0.4.0) ; extra == "jax" or extra == "dqn-jax" or extra == "dqn-atari-jax" or extra == "c51-jax" or extra == "c51-atari-jax" or extra == "ppo-atari-envpool-xla-jax-scan"
 Requires-Dist: markdown-include (>=0.7.0,<0.8.0) ; extra == "docs"
 Requires-Dist: mkdocs-material (>=8.4.3,<9.0.0) ; extra == "docs"
 Requires-Dist: moviepy (>=1.0.3,<2.0.0)
-Requires-Dist: mujoco (>=2.2,<3.0) ; extra == "mujoco" or extra == "dm-control"
+Requires-Dist: mujoco (<=2.3.3) ; extra == "mujoco" or extra == "dm-control"
 Requires-Dist: multi-agent-ale-py (==0.1.11) ; extra == "pettingzoo"
 Requires-Dist: opencv-python (>=4.6.0.66,<5.0.0.0) ; extra == "atari" or extra == "dqn-atari" or extra == "dqn-atari-jax" or extra == "c51-atari" or extra == "c51-atari-jax" or extra == "ppo-atari-envpool-xla-jax-scan"
+Requires-Dist: openrlbenchmark (>=0.1.1b4,<0.2.0) ; extra == "docs"
 Requires-Dist: optuna (>=3.0.1,<4.0.0) ; extra == "optuna"
 Requires-Dist: optuna-dashboard (>=0.7.2,<0.8.0) ; extra == "optuna"
 Requires-Dist: procgen (>=0.10.7,<0.11.0) ; extra == "procgen"
-Requires-Dist: pybullet (==3.1.8) ; extra == "pybullet"
 Requires-Dist: pygame (==2.1.0)
 Requires-Dist: pytest (>=7.1.3,<8.0.0) ; extra == "pytest"
 Requires-Dist: rich (<12.0) ; extra == "optuna"
-Requires-Dist: shimmy (>=0.1.0,<0.2.0) ; extra == "dm-control"
+Requires-Dist: shimmy[dm-control] (>=1.0.0) ; extra == "dm-control"
 Requires-Dist: stable-baselines3 (==1.2.0)
 Requires-Dist: tensorboard (>=2.10.0,<3.0.0)
 Requires-Dist: torch (>=1.12.1)
-Requires-Dist: wandb (>=0.13.6,<0.14.0)
+Requires-Dist: wandb (>=0.13.11,<0.14.0)
 Description-Content-Type: text/markdown
 
 # CleanRL (Clean Implementation of RL Algorithms)
 
 
 [<img src="https://img.shields.io/badge/license-MIT-blue">](https://github.com/vwxyzjn/cleanrl)
 [![tests](https://github.com/vwxyzjn/cleanrl/actions/workflows/tests.yaml/badge.svg)](https://github.com/vwxyzjn/cleanrl/actions/workflows/tests.yaml)
 [![docs](https://img.shields.io/github/deployments/vwxyzjn/cleanrl/Production?label=docs&logo=vercel)](https://docs.cleanrl.dev/)
 [<img src="https://img.shields.io/discord/767863440248143916?label=discord">](https://discord.gg/D6RCjA6sVT)
 [<img src="https://img.shields.io/youtube/channel/views/UCDdC6BIFRI0jvcwuhi3aI6w?style=social">](https://www.youtube.com/channel/UCDdC6BIFRI0jvcwuhi3aI6w/videos)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![Imports: isort](https://img.shields.io/badge/%20imports-isort-%231674b1?style=flat&labelColor=ef8336)](https://pycqa.github.io/isort/)
 [<img src="https://img.shields.io/badge/%F0%9F%A4%97%20Models-Huggingface-F8D521">](https://huggingface.co/cleanrl)
-[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/vwxyzjn/cleanrl/blob/hf-integration/docs/get-started/CleanRL_Huggingface_Integration_Demo.ipynb)
+[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/vwxyzjn/cleanrl/blob/master/docs/get-started/CleanRL_Huggingface_Integration_Demo.ipynb)
 
 
 CleanRL is a Deep Reinforcement Learning library that provides high-quality single-file implementation with research-friendly features. The implementation is clean and simple, yet we can scale it to run thousands of experiments using AWS Batch. The highlight features of CleanRL are:
 
 
 
 * 📜 Single-file implementation
@@ -98,24 +97,23 @@
 * 🧫 Experiment Management with [Weights and Biases](https://wandb.ai/site)
 * 💸 Cloud Integration with docker and AWS 
 
 You can read more about CleanRL in our [JMLR paper](https://www.jmlr.org/papers/volume23/21-1342/21-1342.pdf) and [documentation](https://docs.cleanrl.dev/).
 
 CleanRL only contains implementations of **online** deep reinforcement learning algorithms. If you are looking for **offline** algorithms, please check out [tinkoff-ai/CORL](https://github.com/tinkoff-ai/CORL), which shares a similar design philosophy as CleanRL.
 
-> ℹ️ **Support for Gymnasium**: [Farama-Foundation/Gymnasium](https://github.com/Farama-Foundation/Gymnasium) is the next generation of [`openai/gym`](https://github.com/openai/gym) that will continue to be maintained and introduce new features. Please see their [announcement](https://farama.org/Announcing-The-Farama-Foundation) for further detail. We are migrating to `gymnasium` and the progress can be tracked in [vwxyzjn/cleanrl#277](https://github.com/vwxyzjn/cleanrl/pull/277).
-
+> ℹ️ **Support for Gymnasium**: [Farama-Foundation/Gymnasium](https://github.com/Farama-Foundation/Gymnasium) is the next generation of [`openai/gym`](https://github.com/openai/gym) that will continue to be maintained and introduce new features. Please see their [announcement](https://farama.org/Announcing-The-Farama-Foundation) for further detail. We are migrating to `gymnasium` and the progress can be tracked in [vwxyzjn/cleanrl#277](https://github.com/vwxyzjn/cleanrl/pull/277). 
 
 
 > ⚠️ **NOTE**: CleanRL is *not* a modular library and therefore it is not meant to be imported. At the cost of duplicate code, we make all implementation details of a DRL algorithm variant easy to understand, so CleanRL comes with its own pros and cons. You should consider using CleanRL if you want to 1) understand all implementation details of an algorithm's varaint or 2) prototype advanced features that other modular DRL libraries do not support (CleanRL has minimal lines of code so it gives you great debugging experience and you don't have do a lot of subclassing like sometimes in modular DRL libraries).
 
 ## Get started
 
 Prerequisites:
-* Python >=3.7.1,<3.10 (not yet 3.10)
+* Python >=3.7.1,<3.11
 * [Poetry 1.2.1+](https://python-poetry.org)
 
 To run experiments locally, give the following a try:
 
 ```bash
 git clone https://github.com/vwxyzjn/cleanrl.git && cd cleanrl
 poetry install
@@ -138,50 +136,63 @@
     --seed 1 \
     --env-id CartPole-v0 \
     --total-timesteps 50000 \
     --track \
     --wandb-project-name cleanrltest
 ```
 
+If you are not using `poetry`, you can install CleanRL with `requirements.txt`:
+
+```bash
+# core dependencies
+pip install -r requirements/requirements.txt
+
+# optional dependencies
+pip install -r requirements/requirements-atari.txt
+pip install -r requirements/requirements-mujoco.txt
+pip install -r requirements/requirements-mujoco_py.txt
+pip install -r requirements/requirements-procgen.txt
+pip install -r requirements/requirements-envpool.txt
+pip install -r requirements/requirements-pettingzoo.txt
+pip install -r requirements/requirements-jax.txt
+pip install -r requirements/requirements-docs.txt
+pip install -r requirements/requirements-cloud.txt
+```
+
 To run training scripts in other games:
 ```
 poetry shell
 
 # classic control
 python cleanrl/dqn.py --env-id CartPole-v1
 python cleanrl/ppo.py --env-id CartPole-v1
 python cleanrl/c51.py --env-id CartPole-v1
 
 # atari
-poetry install --with atari
+poetry install -E atari
 python cleanrl/dqn_atari.py --env-id BreakoutNoFrameskip-v4
 python cleanrl/c51_atari.py --env-id BreakoutNoFrameskip-v4
 python cleanrl/ppo_atari.py --env-id BreakoutNoFrameskip-v4
+python cleanrl/sac_atari.py --env-id BreakoutNoFrameskip-v4
 
 # NEW: 3-4x side-effects free speed up with envpool's atari (only available to linux)
-poetry install --with envpool
+poetry install -E envpool
 python cleanrl/ppo_atari_envpool.py --env-id BreakoutNoFrameskip-v4
 # Learn Pong-v5 in ~5-10 mins
 # Side effects such as lower sample efficiency might occur
 poetry run python ppo_atari_envpool.py --clip-coef=0.2 --num-envs=16 --num-minibatches=8 --num-steps=128 --update-epochs=3
 
-# pybullet
-poetry install --with pybullet
-python cleanrl/td3_continuous_action.py --env-id MinitaurBulletDuckEnv-v0
-python cleanrl/ddpg_continuous_action.py --env-id MinitaurBulletDuckEnv-v0
-python cleanrl/sac_continuous_action.py --env-id MinitaurBulletDuckEnv-v0
-
 # procgen
-poetry install --with procgen
+poetry install -E procgen
 python cleanrl/ppo_procgen.py --env-id starpilot
 python cleanrl/ppg_procgen.py --env-id starpilot
 
 # ppo + lstm
+poetry install -E atari
 python cleanrl/ppo_atari_lstm.py --env-id BreakoutNoFrameskip-v4
-python cleanrl/ppo_memory_env_lstm.py
 ```
 
 You may also use a prebuilt development environment hosted in Gitpod:
 
 [![Open in Gitpod](https://gitpod.io/button/open-in-gitpod.svg)](https://gitpod.io/#https://github.com/vwxyzjn/cleanrl)
 
 ## Algorithms Implemented
@@ -197,22 +208,23 @@
 | | [`ppo_atari_envpool_xla_jax.py`](https://github.com/vwxyzjn/cleanrl/blob/master/cleanrl/ppo_atari_envpool_xla_jax.py), [docs](https://docs.cleanrl.dev/rl-algorithms/ppo/#ppo_atari_envpool_xla_jaxpy)
 | | [`ppo_atari_envpool_xla_jax_scan.py`](https://github.com/vwxyzjn/cleanrl/blob/master/cleanrl/ppo_atari_envpool_xla_jax_scan.py), [docs](https://docs.cleanrl.dev/rl-algorithms/ppo/#ppo_atari_envpool_xla_jax_scanpy))
 | |  [`ppo_procgen.py`](https://github.com/vwxyzjn/cleanrl/blob/master/cleanrl/ppo_procgen.py),   [docs](https://docs.cleanrl.dev/rl-algorithms/ppo/#ppo_procgenpy)
 | |  [`ppo_atari_multigpu.py`](https://github.com/vwxyzjn/cleanrl/blob/master/cleanrl/ppo_atari_multigpu.py),  [docs](https://docs.cleanrl.dev/rl-algorithms/ppo/#ppo_atari_multigpupy)
 | | [`ppo_pettingzoo_ma_atari.py`](https://github.com/vwxyzjn/cleanrl/blob/master/cleanrl/ppo_pettingzoo_ma_atari.py),  [docs](https://docs.cleanrl.dev/rl-algorithms/ppo/#ppo_pettingzoo_ma_ataripy)
 | | [`ppo_continuous_action_isaacgym.py`](https://github.com/vwxyzjn/cleanrl/blob/master/cleanrl/ppo_continuous_action_isaacgym/ppo_continuous_action_isaacgym.py),  [docs](https://docs.cleanrl.dev/rl-algorithms/ppo/#ppo_continuous_action_isaacgympy)
 | ✅ [Deep Q-Learning (DQN)](https://web.stanford.edu/class/psych209/Readings/MnihEtAlHassibis15NatureControlDeepRL.pdf) |  [`dqn.py`](https://github.com/vwxyzjn/cleanrl/blob/master/cleanrl/dqn.py),  [docs](https://docs.cleanrl.dev/rl-algorithms/dqn/#dqnpy) |
-| |  [`dqn_atari.py`](https://github.com/vwxyzjn/cleanrl/blob/master/cleanrl/dqn_atari.py),  [docs](https://docs.cleanrl.dev/rl-algorithms/dqn/#dqn_ataripy) |
+| | [`dqn_atari.py`](https://github.com/vwxyzjn/cleanrl/blob/master/cleanrl/dqn_atari.py),  [docs](https://docs.cleanrl.dev/rl-algorithms/dqn/#dqn_ataripy) |
 | | [`dqn_jax.py`](https://github.com/vwxyzjn/cleanrl/blob/master/cleanrl/dqn_jax.py), [docs](https://docs.cleanrl.dev/rl-algorithms/dqn/#dqn_jaxpy) |
 | | [`dqn_atari_jax.py`](https://github.com/vwxyzjn/cleanrl/blob/master/cleanrl/dqn_atari_jax.py), [docs](https://docs.cleanrl.dev/rl-algorithms/dqn/#dqn_atari_jaxpy) |
 | ✅ [Categorical DQN (C51)](https://arxiv.org/pdf/1707.06887.pdf) |  [`c51.py`](https://github.com/vwxyzjn/cleanrl/blob/master/cleanrl/c51.py),  [docs](https://docs.cleanrl.dev/rl-algorithms/c51/#c51py) |
 | |  [`c51_atari.py`](https://github.com/vwxyzjn/cleanrl/blob/master/cleanrl/c51_atari.py),  [docs](https://docs.cleanrl.dev/rl-algorithms/c51/#c51_ataripy) |
 | | [`c51_jax.py`](https://github.com/vwxyzjn/cleanrl/blob/master/cleanrl/c51_jax.py), [docs](https://docs.cleanrl.dev/rl-algorithms/c51/#c51_jaxpy) |
 | | [`c51_atari_jax.py`](https://github.com/vwxyzjn/cleanrl/blob/master/cleanrl/c51_atari_jax.py), [docs](https://docs.cleanrl.dev/rl-algorithms/c51/#c51_atari_jaxpy) |
 | ✅ [Soft Actor-Critic (SAC)](https://arxiv.org/pdf/1812.05905.pdf) |  [`sac_continuous_action.py`](https://github.com/vwxyzjn/cleanrl/blob/master/cleanrl/sac_continuous_action.py),  [docs](https://docs.cleanrl.dev/rl-algorithms/sac/#sac_continuous_actionpy) |
+| |  [`sac_atari.py`](https://github.com/vwxyzjn/cleanrl/blob/master/cleanrl/sac_atari.py),  [docs](https://docs.cleanrl.dev/rl-algorithms/sac/#sac_atarinpy) |
 | ✅ [Deep Deterministic Policy Gradient (DDPG)](https://arxiv.org/pdf/1509.02971.pdf) |  [`ddpg_continuous_action.py`](https://github.com/vwxyzjn/cleanrl/blob/master/cleanrl/ddpg_continuous_action.py),  [docs](https://docs.cleanrl.dev/rl-algorithms/ddpg/#ddpg_continuous_actionpy) |
 | | [`ddpg_continuous_action_jax.py`](https://github.com/vwxyzjn/cleanrl/blob/master/cleanrl/ddpg_continuous_action_jax.py),  [docs](https://docs.cleanrl.dev/rl-algorithms/ddpg/#ddpg_continuous_action_jaxpy)
 | ✅ [Twin Delayed Deep Deterministic Policy Gradient (TD3)](https://arxiv.org/pdf/1802.09477.pdf) |  [`td3_continuous_action.py`](https://github.com/vwxyzjn/cleanrl/blob/master/cleanrl/td3_continuous_action.py),  [docs](https://docs.cleanrl.dev/rl-algorithms/td3/#td3_continuous_actionpy) |
 |  | [`td3_continuous_action_jax.py`](https://github.com/vwxyzjn/cleanrl/blob/master/cleanrl/td3_continuous_action_jax.py),  [docs](https://docs.cleanrl.dev/rl-algorithms/td3/#td3_continuous_action_jaxpy) |
 | ✅ [Phasic Policy Gradient (PPG)](https://arxiv.org/abs/2009.04416) |  [`ppg_procgen.py`](https://github.com/vwxyzjn/cleanrl/blob/master/cleanrl/ppg_procgen.py),  [docs](https://docs.cleanrl.dev/rl-algorithms/ppg/#ppg_procgenpy) |
 | ✅ [Random Network Distillation (RND)](https://arxiv.org/abs/1810.12894) |  [`ppo_rnd_envpool.py`](https://github.com/vwxyzjn/cleanrl/blob/master/cleanrl/ppo_rnd_envpool.py),  [docs](/rl-algorithms/ppo-rnd/#ppo_rnd_envpoolpy) |
```

