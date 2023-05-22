# Comparing `tmp/xuanpolicy-0.1.5.tar.gz` & `tmp/xuanpolicy-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/xuanpolicy-0.1.5.tar", last modified: Mon May 22 01:37:03 2023, max compression
+gzip compressed data, was "dist/xuanpolicy-0.1.6.tar", last modified: Mon May 22 12:59:05 2023, max compression
```

## Comparing `xuanpolicy-0.1.5.tar` & `xuanpolicy-0.1.6.tar`

### file list

```diff
@@ -1,558 +1,571 @@
-drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2023-05-22 01:37:03.000000 xuanpolicy-0.1.5/
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1075 2023-05-19 14:11:29.000000 xuanpolicy-0.1.5/LICENSE.txt
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      864 2023-05-22 01:37:03.000000 xuanpolicy-0.1.5/PKG-INFO
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)    14396 2023-05-21 10:58:46.000000 xuanpolicy-0.1.5/README.md
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)       79 2023-05-22 01:37:03.000000 xuanpolicy-0.1.5/setup.cfg
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1945 2023-05-22 01:33:51.000000 xuanpolicy-0.1.5/setup.py
-drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2023-05-22 01:37:03.000000 xuanpolicy-0.1.5/xuanpolicy/
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      176 2023-05-20 02:58:51.000000 xuanpolicy-0.1.5/xuanpolicy/__init__.py
-drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2023-05-22 01:37:03.000000 xuanpolicy-0.1.5/xuanpolicy/common/
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      233 2023-05-20 06:35:52.000000 xuanpolicy-0.1.5/xuanpolicy/common/__init__.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     7354 2023-05-21 10:28:36.000000 xuanpolicy-0.1.5/xuanpolicy/common/common_tools.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)    16545 2023-05-20 04:14:13.000000 xuanpolicy-0.1.5/xuanpolicy/common/memory_tools.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)    20041 2023-05-19 09:59:24.000000 xuanpolicy-0.1.5/xuanpolicy/common/memory_tools_marl.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     2879 2023-05-19 09:59:24.000000 xuanpolicy-0.1.5/xuanpolicy/common/segtree_tool.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     5059 2023-05-19 09:59:24.000000 xuanpolicy-0.1.5/xuanpolicy/common/statistic_tools.py
-drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2023-05-22 01:37:03.000000 xuanpolicy-0.1.5/xuanpolicy/configs/
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)        0 2023-05-20 06:49:02.000000 xuanpolicy-0.1.5/xuanpolicy/configs/__init__.py
-drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2023-05-22 01:37:03.000000 xuanpolicy-0.1.5/xuanpolicy/configs/a2c/
-drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2023-05-22 01:37:03.000000 xuanpolicy-0.1.5/xuanpolicy/configs/a2c/mujoco/
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      589 2023-05-19 10:00:26.000000 xuanpolicy-0.1.5/xuanpolicy/configs/a2c/mujoco/InvertedPendulum-v2.yaml
-drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2023-05-22 01:37:03.000000 xuanpolicy-0.1.5/xuanpolicy/configs/a2c/toy/
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      565 2023-05-19 10:00:26.000000 xuanpolicy-0.1.5/xuanpolicy/configs/a2c/toy/CartPole-v0.yaml
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      566 2023-05-20 08:17:00.000000 xuanpolicy-0.1.5/xuanpolicy/configs/basic.yaml
-drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2023-05-22 01:37:03.000000 xuanpolicy-0.1.5/xuanpolicy/configs/c51/
-drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2023-05-22 01:37:03.000000 xuanpolicy-0.1.5/xuanpolicy/configs/c51/toy/
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      500 2023-05-19 10:00:25.000000 xuanpolicy-0.1.5/xuanpolicy/configs/c51/toy/Acrobot-v1.yaml
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      501 2023-05-19 10:00:25.000000 xuanpolicy-0.1.5/xuanpolicy/configs/c51/toy/CartPole-v0.yaml
-drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2023-05-22 01:37:03.000000 xuanpolicy-0.1.5/xuanpolicy/configs/cdqn/
-drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2023-05-22 01:37:03.000000 xuanpolicy-0.1.5/xuanpolicy/configs/cdqn/toy/
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      467 2023-05-19 10:00:23.000000 xuanpolicy-0.1.5/xuanpolicy/configs/cdqn/toy/CartPole-v0.yaml
-drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2023-05-22 01:37:03.000000 xuanpolicy-0.1.5/xuanpolicy/configs/cldqn/
-drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2023-05-22 01:37:03.000000 xuanpolicy-0.1.5/xuanpolicy/configs/cldqn/toy/
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      471 2023-05-19 10:00:25.000000 xuanpolicy-0.1.5/xuanpolicy/configs/cldqn/toy/CartPole-v0.yaml
-drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2023-05-22 01:37:03.000000 xuanpolicy-0.1.5/xuanpolicy/configs/coma/
-drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2023-05-22 01:37:03.000000 xuanpolicy-0.1.5/xuanpolicy/configs/coma/mpe/
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      929 2023-05-20 08:41:30.000000 xuanpolicy-0.1.5/xuanpolicy/configs/coma/mpe/simple_spread.yaml
-drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2023-05-22 01:37:03.000000 xuanpolicy-0.1.5/xuanpolicy/configs/cwqmix/
-drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2023-05-22 01:37:03.000000 xuanpolicy-0.1.5/xuanpolicy/configs/cwqmix/mpe/
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      953 2023-05-20 08:41:40.000000 xuanpolicy-0.1.5/xuanpolicy/configs/cwqmix/mpe/simple_spread.yaml
-drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2023-05-22 01:37:03.000000 xuanpolicy-0.1.5/xuanpolicy/configs/dcg/
-drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2023-05-22 01:37:03.000000 xuanpolicy-0.1.5/xuanpolicy/configs/dcg/mpe/
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1391 2023-05-20 08:41:51.000000 xuanpolicy-0.1.5/xuanpolicy/configs/dcg/mpe/simple_spread.yaml
-drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2023-05-22 01:37:03.000000 xuanpolicy-0.1.5/xuanpolicy/configs/ddpg/
-drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2023-05-22 01:37:03.000000 xuanpolicy-0.1.5/xuanpolicy/configs/ddpg/mujoco/
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      556 2023-05-19 10:00:23.000000 xuanpolicy-0.1.5/xuanpolicy/configs/ddpg/mujoco/HalfCheetah-v3.yaml
-drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2023-05-22 01:37:03.000000 xuanpolicy-0.1.5/xuanpolicy/configs/ddpg/toy/
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      548 2023-05-19 10:00:23.000000 xuanpolicy-0.1.5/xuanpolicy/configs/ddpg/toy/Pendulum-v1.yaml
-drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2023-05-22 01:37:03.000000 xuanpolicy-0.1.5/xuanpolicy/configs/ddqn/
-drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2023-05-22 01:37:03.000000 xuanpolicy-0.1.5/xuanpolicy/configs/ddqn/toy/
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      471 2023-05-19 10:00:25.000000 xuanpolicy-0.1.5/xuanpolicy/configs/ddqn/toy/Acrobot-v1.yaml
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      472 2023-05-19 10:00:25.000000 xuanpolicy-0.1.5/xuanpolicy/configs/ddqn/toy/CartPole-v0.yaml
-drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2023-05-22 01:37:03.000000 xuanpolicy-0.1.5/xuanpolicy/configs/dqn/
-drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2023-05-22 01:37:03.000000 xuanpolicy-0.1.5/xuanpolicy/configs/dqn/toy/
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      487 2023-05-20 09:18:32.000000 xuanpolicy-0.1.5/xuanpolicy/configs/dqn/toy/CartPole-v0.yaml
-drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2023-05-22 01:37:03.000000 xuanpolicy-0.1.5/xuanpolicy/configs/dueldqn/
-drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2023-05-22 01:37:03.000000 xuanpolicy-0.1.5/xuanpolicy/configs/dueldqn/toy/
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      480 2023-05-19 10:00:26.000000 xuanpolicy-0.1.5/xuanpolicy/configs/dueldqn/toy/Acrobot-v1.yaml
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      481 2023-05-19 10:00:26.000000 xuanpolicy-0.1.5/xuanpolicy/configs/dueldqn/toy/CartPole-v0.yaml
-drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2023-05-22 01:37:03.000000 xuanpolicy-0.1.5/xuanpolicy/configs/iddpg/
-drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2023-05-22 01:37:03.000000 xuanpolicy-0.1.5/xuanpolicy/configs/iddpg/mpe/
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      903 2023-05-20 08:42:25.000000 xuanpolicy-0.1.5/xuanpolicy/configs/iddpg/mpe/simple_spread.yaml
-drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2023-05-22 01:37:03.000000 xuanpolicy-0.1.5/xuanpolicy/configs/iql/
-drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2023-05-22 01:37:03.000000 xuanpolicy-0.1.5/xuanpolicy/configs/iql/mpe/
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      809 2023-05-20 08:42:37.000000 xuanpolicy-0.1.5/xuanpolicy/configs/iql/mpe/simple_spread.yaml
-drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2023-05-22 01:37:03.000000 xuanpolicy-0.1.5/xuanpolicy/configs/isac/
-drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2023-05-22 01:37:03.000000 xuanpolicy-0.1.5/xuanpolicy/configs/isac/mpe/
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      910 2023-05-20 08:42:53.000000 xuanpolicy-0.1.5/xuanpolicy/configs/isac/mpe/simple_spread.yaml
-drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2023-05-22 01:37:03.000000 xuanpolicy-0.1.5/xuanpolicy/configs/ldqn/
-drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2023-05-22 01:37:03.000000 xuanpolicy-0.1.5/xuanpolicy/configs/ldqn/toy/
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      467 2023-05-19 10:00:21.000000 xuanpolicy-0.1.5/xuanpolicy/configs/ldqn/toy/CartPole-v0.yaml
-drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2023-05-22 01:37:03.000000 xuanpolicy-0.1.5/xuanpolicy/configs/maddpg/
-drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2023-05-22 01:37:03.000000 xuanpolicy-0.1.5/xuanpolicy/configs/maddpg/mpe/
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      944 2023-05-20 09:18:32.000000 xuanpolicy-0.1.5/xuanpolicy/configs/maddpg/mpe/simple_spread.yaml
-drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2023-05-22 01:37:03.000000 xuanpolicy-0.1.5/xuanpolicy/configs/mappoclip/
-drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2023-05-22 01:37:03.000000 xuanpolicy-0.1.5/xuanpolicy/configs/mappoclip/mpe/
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1089 2023-05-20 08:43:44.000000 xuanpolicy-0.1.5/xuanpolicy/configs/mappoclip/mpe/simple_spread.yaml
-drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2023-05-22 01:37:03.000000 xuanpolicy-0.1.5/xuanpolicy/configs/mappokl/
-drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2023-05-22 01:37:03.000000 xuanpolicy-0.1.5/xuanpolicy/configs/mappokl/mpe/
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1080 2023-05-20 08:43:53.000000 xuanpolicy-0.1.5/xuanpolicy/configs/mappokl/mpe/simple_spread.yaml
-drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2023-05-22 01:37:03.000000 xuanpolicy-0.1.5/xuanpolicy/configs/masac/
-drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2023-05-22 01:37:03.000000 xuanpolicy-0.1.5/xuanpolicy/configs/masac/mpe/
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      914 2023-05-20 08:44:07.000000 xuanpolicy-0.1.5/xuanpolicy/configs/masac/mpe/simple_spread.yaml
-drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2023-05-22 01:37:03.000000 xuanpolicy-0.1.5/xuanpolicy/configs/matd3/
-drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2023-05-22 01:37:03.000000 xuanpolicy-0.1.5/xuanpolicy/configs/matd3/mpe/
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      892 2023-05-20 08:44:18.000000 xuanpolicy-0.1.5/xuanpolicy/configs/matd3/mpe/simple_spread.yaml
-drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2023-05-22 01:37:03.000000 xuanpolicy-0.1.5/xuanpolicy/configs/mfac/
-drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2023-05-22 01:37:03.000000 xuanpolicy-0.1.5/xuanpolicy/configs/mfac/mpe/
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      949 2023-05-20 08:44:25.000000 xuanpolicy-0.1.5/xuanpolicy/configs/mfac/mpe/simple_spread.yaml
-drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2023-05-22 01:37:03.000000 xuanpolicy-0.1.5/xuanpolicy/configs/mfq/
-drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2023-05-22 01:37:03.000000 xuanpolicy-0.1.5/xuanpolicy/configs/mfq/mpe/
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      806 2023-05-20 08:44:34.000000 xuanpolicy-0.1.5/xuanpolicy/configs/mfq/mpe/simple_spread.yaml
-drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2023-05-22 01:37:03.000000 xuanpolicy-0.1.5/xuanpolicy/configs/mpdqn/
-drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2023-05-22 01:37:03.000000 xuanpolicy-0.1.5/xuanpolicy/configs/mpdqn/toy/
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      519 2023-05-19 10:00:23.000000 xuanpolicy-0.1.5/xuanpolicy/configs/mpdqn/toy/Platform-v0.yaml
-drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2023-05-22 01:37:03.000000 xuanpolicy-0.1.5/xuanpolicy/configs/noisydqn/
-drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2023-05-22 01:37:03.000000 xuanpolicy-0.1.5/xuanpolicy/configs/noisydqn/toy/
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      482 2023-05-19 10:00:22.000000 xuanpolicy-0.1.5/xuanpolicy/configs/noisydqn/toy/Acrobot-v1.yaml
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      483 2023-05-19 10:00:22.000000 xuanpolicy-0.1.5/xuanpolicy/configs/noisydqn/toy/CartPole-v0.yaml
-drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2023-05-22 01:37:03.000000 xuanpolicy-0.1.5/xuanpolicy/configs/owqmix/
-drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2023-05-22 01:37:03.000000 xuanpolicy-0.1.5/xuanpolicy/configs/owqmix/mpe/
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      953 2023-05-20 08:44:43.000000 xuanpolicy-0.1.5/xuanpolicy/configs/owqmix/mpe/simple_spread.yaml
-drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2023-05-22 01:37:03.000000 xuanpolicy-0.1.5/xuanpolicy/configs/pdqn/
-drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2023-05-22 01:37:03.000000 xuanpolicy-0.1.5/xuanpolicy/configs/pdqn/toy/
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      515 2023-05-19 10:00:21.000000 xuanpolicy-0.1.5/xuanpolicy/configs/pdqn/toy/Platform-v0.yaml
-drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2023-05-22 01:37:03.000000 xuanpolicy-0.1.5/xuanpolicy/configs/perdqn/
-drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2023-05-22 01:37:03.000000 xuanpolicy-0.1.5/xuanpolicy/configs/perdqn/toy/
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      508 2023-05-19 10:00:21.000000 xuanpolicy-0.1.5/xuanpolicy/configs/perdqn/toy/CartPole-v0.yaml
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      511 2023-05-19 10:00:21.000000 xuanpolicy-0.1.5/xuanpolicy/configs/perdqn/toy/MountainCar-v0.yaml
-drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2023-05-22 01:37:03.000000 xuanpolicy-0.1.5/xuanpolicy/configs/pg/
-drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2023-05-22 01:37:03.000000 xuanpolicy-0.1.5/xuanpolicy/configs/pg/mujoco/
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      549 2023-05-19 10:00:24.000000 xuanpolicy-0.1.5/xuanpolicy/configs/pg/mujoco/InvertedPendulum-v2.yaml
-drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2023-05-22 01:37:03.000000 xuanpolicy-0.1.5/xuanpolicy/configs/pg/toy/
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      511 2023-05-19 10:00:24.000000 xuanpolicy-0.1.5/xuanpolicy/configs/pg/toy/CartPole-v0.yaml
-drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2023-05-22 01:37:03.000000 xuanpolicy-0.1.5/xuanpolicy/configs/ppg/
-drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2023-05-22 01:37:03.000000 xuanpolicy-0.1.5/xuanpolicy/configs/ppg/mujoco/
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      546 2023-05-19 10:00:26.000000 xuanpolicy-0.1.5/xuanpolicy/configs/ppg/mujoco/InvertedPendulum-v2.yaml
-drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2023-05-22 01:37:03.000000 xuanpolicy-0.1.5/xuanpolicy/configs/ppg/toy/
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      509 2023-05-19 10:00:26.000000 xuanpolicy-0.1.5/xuanpolicy/configs/ppg/toy/CartPole-v0.yaml
-drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2023-05-22 01:37:03.000000 xuanpolicy-0.1.5/xuanpolicy/configs/ppoclip/
-drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2023-05-22 01:37:03.000000 xuanpolicy-0.1.5/xuanpolicy/configs/ppoclip/atari/
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      587 2023-05-19 10:00:21.000000 xuanpolicy-0.1.5/xuanpolicy/configs/ppoclip/atari/PongNoFrameskip-v4.yaml
-drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2023-05-22 01:37:03.000000 xuanpolicy-0.1.5/xuanpolicy/configs/ppoclip/mujoco/
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      514 2023-05-19 10:00:22.000000 xuanpolicy-0.1.5/xuanpolicy/configs/ppoclip/mujoco/InvertedPendulum-v2.yaml
-drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2023-05-22 01:37:03.000000 xuanpolicy-0.1.5/xuanpolicy/configs/ppoclip/toy/
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      474 2023-05-19 10:00:21.000000 xuanpolicy-0.1.5/xuanpolicy/configs/ppoclip/toy/CartPole-v0.yaml
-drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2023-05-22 01:37:03.000000 xuanpolicy-0.1.5/xuanpolicy/configs/ppokl/
-drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2023-05-22 01:37:03.000000 xuanpolicy-0.1.5/xuanpolicy/configs/ppokl/mujoco/
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      506 2023-05-19 10:00:22.000000 xuanpolicy-0.1.5/xuanpolicy/configs/ppokl/mujoco/InvertedPendulum-v2.yaml
-drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2023-05-22 01:37:03.000000 xuanpolicy-0.1.5/xuanpolicy/configs/ppokl/toy/
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      468 2023-05-19 10:00:22.000000 xuanpolicy-0.1.5/xuanpolicy/configs/ppokl/toy/CartPole-v0.yaml
-drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2023-05-22 01:37:03.000000 xuanpolicy-0.1.5/xuanpolicy/configs/qmix/
-drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2023-05-22 01:37:03.000000 xuanpolicy-0.1.5/xuanpolicy/configs/qmix/mpe/
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      903 2023-05-20 08:31:40.000000 xuanpolicy-0.1.5/xuanpolicy/configs/qmix/mpe/simple_spread.yaml
-drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2023-05-22 01:37:03.000000 xuanpolicy-0.1.5/xuanpolicy/configs/qrdqn/
-drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2023-05-22 01:37:03.000000 xuanpolicy-0.1.5/xuanpolicy/configs/qrdqn/toy/
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      488 2023-05-19 10:00:23.000000 xuanpolicy-0.1.5/xuanpolicy/configs/qrdqn/toy/Acrobot-v1.yaml
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      489 2023-05-19 10:00:24.000000 xuanpolicy-0.1.5/xuanpolicy/configs/qrdqn/toy/CartPole-v0.yaml
-drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2023-05-22 01:37:03.000000 xuanpolicy-0.1.5/xuanpolicy/configs/qtran/
-drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2023-05-22 01:37:03.000000 xuanpolicy-0.1.5/xuanpolicy/configs/qtran/mpe/
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      883 2023-05-20 08:44:57.000000 xuanpolicy-0.1.5/xuanpolicy/configs/qtran/mpe/simple_spread.yaml
-drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2023-05-22 01:37:03.000000 xuanpolicy-0.1.5/xuanpolicy/configs/sac/
-drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2023-05-22 01:37:03.000000 xuanpolicy-0.1.5/xuanpolicy/configs/sac/mujoco/
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      566 2023-05-19 10:00:22.000000 xuanpolicy-0.1.5/xuanpolicy/configs/sac/mujoco/HalfCheetah-v3.yaml
-drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2023-05-22 01:37:03.000000 xuanpolicy-0.1.5/xuanpolicy/configs/sac/toy/
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      499 2023-05-19 10:00:22.000000 xuanpolicy-0.1.5/xuanpolicy/configs/sac/toy/Pendulum-v1.yaml
-drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2023-05-22 01:37:03.000000 xuanpolicy-0.1.5/xuanpolicy/configs/sacdis/
-drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2023-05-22 01:37:03.000000 xuanpolicy-0.1.5/xuanpolicy/configs/sacdis/toy/
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      566 2023-05-19 10:00:23.000000 xuanpolicy-0.1.5/xuanpolicy/configs/sacdis/toy/CartPole-v0.yaml
-drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2023-05-22 01:37:03.000000 xuanpolicy-0.1.5/xuanpolicy/configs/spdqn/
-drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2023-05-22 01:37:03.000000 xuanpolicy-0.1.5/xuanpolicy/configs/spdqn/toy/
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      519 2023-05-19 10:00:25.000000 xuanpolicy-0.1.5/xuanpolicy/configs/spdqn/toy/Platform-v0.yaml
-drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2023-05-22 01:37:03.000000 xuanpolicy-0.1.5/xuanpolicy/configs/td3/
-drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2023-05-22 01:37:03.000000 xuanpolicy-0.1.5/xuanpolicy/configs/td3/mujoco/
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      557 2023-05-19 10:00:27.000000 xuanpolicy-0.1.5/xuanpolicy/configs/td3/mujoco/InvertedPendulum-v2.yaml
-drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2023-05-22 01:37:03.000000 xuanpolicy-0.1.5/xuanpolicy/configs/td3/toy/
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      510 2023-05-19 10:00:27.000000 xuanpolicy-0.1.5/xuanpolicy/configs/td3/toy/Pendulum-v1.yaml
-drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2023-05-22 01:37:03.000000 xuanpolicy-0.1.5/xuanpolicy/configs/vdac/
-drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2023-05-22 01:37:03.000000 xuanpolicy-0.1.5/xuanpolicy/configs/vdac/mpe/
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      973 2023-05-20 08:45:09.000000 xuanpolicy-0.1.5/xuanpolicy/configs/vdac/mpe/simple_spread.yaml
-drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2023-05-22 01:37:03.000000 xuanpolicy-0.1.5/xuanpolicy/configs/vdn/
-drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2023-05-22 01:37:03.000000 xuanpolicy-0.1.5/xuanpolicy/configs/vdn/mpe/
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      804 2023-05-20 08:45:16.000000 xuanpolicy-0.1.5/xuanpolicy/configs/vdn/mpe/simple_spread.yaml
-drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2023-05-22 01:37:03.000000 xuanpolicy-0.1.5/xuanpolicy/environment/
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     2086 2023-05-22 01:36:14.000000 xuanpolicy-0.1.5/xuanpolicy/environment/__init__.py
-drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2023-05-22 01:37:03.000000 xuanpolicy-0.1.5/xuanpolicy/environment/custom_envs/
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     5124 2023-05-19 09:59:27.000000 xuanpolicy-0.1.5/xuanpolicy/environment/custom_envs/USVmodel.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)        0 2023-05-20 02:01:16.000000 xuanpolicy-0.1.5/xuanpolicy/environment/custom_envs/__init__.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     3341 2023-05-19 09:59:27.000000 xuanpolicy-0.1.5/xuanpolicy/environment/custom_envs/atari_env.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1429 2023-05-19 09:59:27.000000 xuanpolicy-0.1.5/xuanpolicy/environment/custom_envs/mujoco_env.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     5202 2023-05-20 09:08:07.000000 xuanpolicy-0.1.5/xuanpolicy/environment/custom_envs/pettingzoo_env.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      316 2023-05-19 09:59:27.000000 xuanpolicy-0.1.5/xuanpolicy/environment/custom_envs/robotics_env.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      981 2023-05-19 09:59:27.000000 xuanpolicy-0.1.5/xuanpolicy/environment/custom_envs/toy_env.py
-drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2023-05-22 01:37:03.000000 xuanpolicy-0.1.5/xuanpolicy/environment/vector_envs/
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)        0 2023-05-20 05:13:59.000000 xuanpolicy-0.1.5/xuanpolicy/environment/vector_envs/__init__.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     8959 2023-05-20 09:08:36.000000 xuanpolicy-0.1.5/xuanpolicy/environment/vector_envs/dummy_vec_env.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     3981 2023-05-19 09:59:27.000000 xuanpolicy-0.1.5/xuanpolicy/environment/vector_envs/env_utils.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     6166 2023-05-19 09:59:27.000000 xuanpolicy-0.1.5/xuanpolicy/environment/vector_envs/subproc_vec_env.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     3396 2023-05-19 09:59:27.000000 xuanpolicy-0.1.5/xuanpolicy/environment/vector_envs/vector_env.py
-drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2023-05-22 01:37:03.000000 xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_ms/
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)        0 2023-05-19 15:23:02.000000 xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_ms/__init__.py
-drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2023-05-22 01:37:03.000000 xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_ms/agents/
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     4240 2023-05-19 11:38:49.000000 xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_ms/agents/__init__.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1240 2023-05-19 11:38:52.000000 xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_ms/agents/agent.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     3670 2023-05-19 11:38:56.000000 xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_ms/agents/agents_marl.py
-drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2023-05-22 01:37:03.000000 xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_ms/agents/multi_agent_rl/
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)        0 2023-05-20 05:14:19.000000 xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_ms/agents/multi_agent_rl/__init__.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     5598 2023-05-19 11:34:21.000000 xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_ms/agents/multi_agent_rl/coma_agents.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     5206 2023-05-19 11:34:25.000000 xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_ms/agents/multi_agent_rl/dcg_agents.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     4234 2023-05-19 11:34:29.000000 xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_ms/agents/multi_agent_rl/iddpg_agents.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     4084 2023-05-19 11:34:32.000000 xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_ms/agents/multi_agent_rl/iql_agents.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     4210 2023-05-19 11:34:35.000000 xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_ms/agents/multi_agent_rl/isac_agents.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     4238 2023-05-19 11:36:37.000000 xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_ms/agents/multi_agent_rl/maddpg_agents.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     4998 2023-05-19 11:36:39.000000 xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_ms/agents/multi_agent_rl/mappoclip_agents.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     5127 2023-05-19 11:36:42.000000 xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_ms/agents/multi_agent_rl/mappokl_agents.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     4214 2023-05-19 11:36:45.000000 xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_ms/agents/multi_agent_rl/masac_agents.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     4537 2023-05-19 11:36:47.000000 xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_ms/agents/multi_agent_rl/matd3_agents.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     5707 2023-05-19 11:36:50.000000 xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_ms/agents/multi_agent_rl/mfac_agents.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     5867 2023-05-19 11:36:54.000000 xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_ms/agents/multi_agent_rl/mfq_agents.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     4245 2023-05-19 11:37:00.000000 xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_ms/agents/multi_agent_rl/qmix_agents.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     4722 2023-05-19 11:37:04.000000 xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_ms/agents/multi_agent_rl/qtran_agents.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     5336 2023-05-19 11:37:07.000000 xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_ms/agents/multi_agent_rl/vdac_agents.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     4118 2023-05-19 11:37:13.000000 xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_ms/agents/multi_agent_rl/vdn_agents.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     4437 2023-05-19 11:37:18.000000 xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_ms/agents/multi_agent_rl/wqmix_agents.py
-drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2023-05-22 01:37:03.000000 xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_ms/agents/policy_gradient/
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)        0 2023-05-20 05:14:30.000000 xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_ms/agents/policy_gradient/__init__.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     6376 2023-05-19 11:37:22.000000 xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_ms/agents/policy_gradient/a2c_agent.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     6316 2023-05-19 11:37:25.000000 xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_ms/agents/policy_gradient/ddpg_agent.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     8971 2023-05-19 11:37:29.000000 xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_ms/agents/policy_gradient/mpdqn_agent.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     8210 2023-05-19 11:37:31.000000 xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_ms/agents/policy_gradient/pdqn_agent.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     6132 2023-05-19 11:37:34.000000 xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_ms/agents/policy_gradient/pg_agent.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     7942 2023-05-19 11:37:37.000000 xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_ms/agents/policy_gradient/ppg_agent.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     6591 2023-05-19 11:37:40.000000 xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_ms/agents/policy_gradient/ppoclip_agent.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     6571 2023-05-19 11:37:42.000000 xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_ms/agents/policy_gradient/ppokl_agent.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     6176 2023-05-19 11:37:46.000000 xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_ms/agents/policy_gradient/sac_agent.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     6291 2023-05-19 11:37:50.000000 xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_ms/agents/policy_gradient/sacdis_agent.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     9264 2023-05-19 11:37:54.000000 xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_ms/agents/policy_gradient/spdqn_agent.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     6368 2023-05-19 11:37:58.000000 xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_ms/agents/policy_gradient/td3_agent.py
-drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2023-05-22 01:37:03.000000 xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_ms/agents/qlearning_family/
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     6292 2023-05-19 11:38:02.000000 xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_ms/agents/qlearning_family/C51_agent.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)        0 2023-05-20 05:14:40.000000 xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_ms/agents/qlearning_family/__init__.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     6294 2023-05-19 11:38:06.000000 xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_ms/agents/qlearning_family/cdqn_agent.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     6296 2023-05-19 11:38:10.000000 xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_ms/agents/qlearning_family/cldqn_agent.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     6303 2023-05-19 11:38:12.000000 xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_ms/agents/qlearning_family/ddqn_agent.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     6292 2023-05-19 11:38:14.000000 xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_ms/agents/qlearning_family/dqn_agent.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     6386 2023-05-19 11:38:17.000000 xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_ms/agents/qlearning_family/dueldqn_agent.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     6294 2023-05-19 11:38:19.000000 xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_ms/agents/qlearning_family/ldqn_agent.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     6281 2023-05-19 11:38:22.000000 xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_ms/agents/qlearning_family/noisydqn_agent.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     6603 2023-05-19 11:38:25.000000 xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_ms/agents/qlearning_family/perdqn_agent.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     6298 2023-05-19 11:38:29.000000 xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_ms/agents/qlearning_family/qrdqn_agent.py
-drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2023-05-22 01:37:03.000000 xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_ms/learners/
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     2517 2023-05-19 11:45:53.000000 xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_ms/learners/__init__.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     3496 2023-05-19 09:59:25.000000 xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_ms/learners/learner.py
-drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2023-05-22 01:37:03.000000 xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_ms/learners/multi_agent_rl/
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)        0 2023-05-20 05:14:54.000000 xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_ms/learners/multi_agent_rl/__init__.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     7059 2023-05-19 11:39:03.000000 xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_ms/learners/multi_agent_rl/coma_learner.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     8730 2023-05-19 11:39:06.000000 xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_ms/learners/multi_agent_rl/dcg_learner.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     4002 2023-05-19 11:39:09.000000 xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_ms/learners/multi_agent_rl/iddpg_learner.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     3080 2023-05-19 11:39:14.000000 xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_ms/learners/multi_agent_rl/iql_learner.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     4877 2023-05-19 11:39:17.000000 xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_ms/learners/multi_agent_rl/isac_learner.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     4632 2023-05-19 11:39:20.000000 xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_ms/learners/multi_agent_rl/maddpg_learner.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     4681 2023-05-19 11:39:23.000000 xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_ms/learners/multi_agent_rl/mappoclip_learner.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     5220 2023-05-19 11:39:26.000000 xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_ms/learners/multi_agent_rl/mappokl_learner.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     4881 2023-05-19 11:39:30.000000 xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_ms/learners/multi_agent_rl/masac_learner.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     5667 2023-05-19 11:39:32.000000 xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_ms/learners/multi_agent_rl/matd3_learner.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     6181 2023-05-19 11:39:35.000000 xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_ms/learners/multi_agent_rl/mfac_learner.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     3615 2023-05-19 11:39:38.000000 xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_ms/learners/multi_agent_rl/mfq_learner.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     3486 2023-05-19 11:39:43.000000 xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_ms/learners/multi_agent_rl/qmix_learner.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     6449 2023-05-19 11:39:47.000000 xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_ms/learners/multi_agent_rl/qtran_learner.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     2926 2023-05-19 11:39:50.000000 xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_ms/learners/multi_agent_rl/vdac_learner.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     3376 2023-05-19 11:39:53.000000 xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_ms/learners/multi_agent_rl/vdn_learner.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     5034 2023-05-19 11:39:55.000000 xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_ms/learners/multi_agent_rl/wqmix_learner.py
-drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2023-05-22 01:37:03.000000 xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_ms/learners/policy_gradient/
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)        0 2023-05-20 05:14:54.000000 xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_ms/learners/policy_gradient/__init__.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     2857 2023-05-19 11:42:14.000000 xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_ms/learners/policy_gradient/a2c_learner.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     2968 2023-05-19 11:43:24.000000 xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_ms/learners/policy_gradient/ddpg_learner.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     4741 2023-05-19 11:43:35.000000 xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_ms/learners/policy_gradient/mpdqn_learner.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     3410 2023-05-19 11:43:45.000000 xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_ms/learners/policy_gradient/pdqn_learner.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     2401 2023-05-19 11:44:14.000000 xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_ms/learners/policy_gradient/pg_learner.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     4603 2023-05-19 11:44:20.000000 xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_ms/learners/policy_gradient/ppg_learner.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     3316 2023-05-19 11:44:24.000000 xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_ms/learners/policy_gradient/ppoclip_learner.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     2804 2023-05-19 11:44:28.000000 xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_ms/learners/policy_gradient/ppokl_learner.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     2903 2023-05-19 11:44:31.000000 xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_ms/learners/policy_gradient/sac_learner.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     3355 2023-05-19 11:44:38.000000 xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_ms/learners/policy_gradient/sacdis_learner.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     4753 2023-05-19 11:44:43.000000 xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_ms/learners/policy_gradient/spdqn_learner.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     3344 2023-05-19 11:44:50.000000 xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_ms/learners/policy_gradient/td3_learner.py
-drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2023-05-22 01:37:03.000000 xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_ms/learners/qlearning_family/
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)        0 2023-05-20 05:14:54.000000 xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_ms/learners/qlearning_family/__init__.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     3716 2023-05-19 11:44:56.000000 xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_ms/learners/qlearning_family/c51_learner.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     2480 2023-05-19 11:45:03.000000 xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_ms/learners/qlearning_family/cdqn_learner.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     2483 2023-05-19 11:45:10.000000 xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_ms/learners/qlearning_family/cldqn_learner.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     2490 2023-05-19 11:45:13.000000 xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_ms/learners/qlearning_family/ddqn_learner.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     2477 2023-05-19 11:45:18.000000 xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_ms/learners/qlearning_family/dqn_learner.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     2356 2023-05-19 11:45:21.000000 xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_ms/learners/qlearning_family/dueldqn_learner.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     2480 2023-05-19 11:45:26.000000 xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_ms/learners/qlearning_family/ldqn_learner.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     2752 2023-05-19 11:45:31.000000 xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_ms/learners/qlearning_family/perdqn_learner.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     3104 2023-05-19 11:45:36.000000 xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_ms/learners/qlearning_family/qrdqn_learner.py
-drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2023-05-22 01:37:03.000000 xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_ms/policies/
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     9030 2023-05-19 09:59:25.000000 xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_ms/policies/__init__.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)    13628 2023-05-19 11:46:18.000000 xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_ms/policies/categorical.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)    13942 2023-05-19 11:46:15.000000 xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_ms/policies/categorical_marl.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)    37569 2023-05-19 11:46:29.000000 xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_ms/policies/deterministic.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)    24973 2023-05-19 11:46:25.000000 xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_ms/policies/deterministic_marl.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)    10533 2023-05-19 11:46:43.000000 xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_ms/policies/gaussian.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)    13858 2023-05-19 11:46:34.000000 xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_ms/policies/gaussian_marl.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)    11317 2023-05-19 09:59:25.000000 xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_ms/policies/mixers.py
-drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2023-05-22 01:37:03.000000 xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_ms/representations/
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1428 2023-05-19 09:59:24.000000 xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_ms/representations/__init__.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)    13453 2023-05-19 11:46:55.000000 xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_ms/representations/networks.py
-drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2023-05-22 01:37:03.000000 xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_ms/runners/
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      190 2023-05-19 09:59:25.000000 xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_ms/runners/__init__.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     3913 2023-05-19 11:34:14.000000 xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_ms/runners/runner_basic.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     4868 2023-05-19 11:47:17.000000 xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_ms/runners/runner_drl.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     6659 2023-05-19 11:47:23.000000 xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_ms/runners/runner_marl.py
-drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2023-05-22 01:37:03.000000 xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_ms/utils/
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)       47 2023-05-19 09:59:25.000000 xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_ms/utils/__init__.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1726 2023-05-19 09:59:25.000000 xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_ms/utils/distributions.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     4291 2023-05-19 11:47:59.000000 xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_ms/utils/input_reformat.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     3583 2023-05-19 09:59:25.000000 xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_ms/utils/layers.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     2029 2023-05-19 09:59:25.000000 xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_ms/utils/operations.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1536 2023-05-19 09:59:25.000000 xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_ms/utils/set_trainer.py
-drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2023-05-22 01:37:03.000000 xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_tf/
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)        0 2023-05-19 15:23:26.000000 xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_tf/__init__.py
-drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2023-05-22 01:37:03.000000 xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_tf/agents/
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     4371 2023-05-19 11:06:18.000000 xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_tf/agents/__init__.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1618 2023-05-19 11:04:53.000000 xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_tf/agents/agent.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     3697 2023-05-19 11:05:03.000000 xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_tf/agents/agents_marl.py
-drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2023-05-22 01:37:03.000000 xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_tf/agents/multi_agent_rl/
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)        0 2023-05-20 05:14:54.000000 xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_tf/agents/multi_agent_rl/__init__.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     5728 2023-05-19 10:55:48.000000 xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_tf/agents/multi_agent_rl/coma_agents.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     5563 2023-05-19 10:55:52.000000 xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_tf/agents/multi_agent_rl/dcg_agents.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     4336 2023-05-19 10:55:55.000000 xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_tf/agents/multi_agent_rl/iddpg_agents.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     4345 2023-05-19 10:55:59.000000 xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_tf/agents/multi_agent_rl/iql_agents.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     4243 2023-05-19 10:56:02.000000 xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_tf/agents/multi_agent_rl/isac_agents.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     4341 2023-05-19 10:56:25.000000 xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_tf/agents/multi_agent_rl/maddpg_agents.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     5047 2023-05-19 10:56:40.000000 xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_tf/agents/multi_agent_rl/mappoclip_agents.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     5003 2023-05-19 10:56:44.000000 xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_tf/agents/multi_agent_rl/mappokl_agents.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     4247 2023-05-19 10:56:47.000000 xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_tf/agents/multi_agent_rl/masac_agents.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     4338 2023-05-19 10:56:51.000000 xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_tf/agents/multi_agent_rl/matd3_agents.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     5420 2023-05-19 10:56:55.000000 xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_tf/agents/multi_agent_rl/mfac_agents.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     5780 2023-05-19 10:57:00.000000 xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_tf/agents/multi_agent_rl/mfq_agents.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     4539 2023-05-19 10:57:04.000000 xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_tf/agents/multi_agent_rl/qmix_agents.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     4975 2023-05-19 10:57:09.000000 xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_tf/agents/multi_agent_rl/qtran_agents.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     5420 2023-05-19 10:57:12.000000 xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_tf/agents/multi_agent_rl/vdac_agents.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     4410 2023-05-19 10:57:16.000000 xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_tf/agents/multi_agent_rl/vdn_agents.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     4690 2023-05-19 10:57:23.000000 xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_tf/agents/multi_agent_rl/wqmix_agents.py
-drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2023-05-22 01:37:03.000000 xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_tf/agents/policy_gradient/
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)        0 2023-05-20 05:14:54.000000 xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_tf/agents/policy_gradient/__init__.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     6195 2023-05-19 10:57:27.000000 xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_tf/agents/policy_gradient/a2c_agent.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     6163 2023-05-19 10:57:31.000000 xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_tf/agents/policy_gradient/ddpg_agent.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     8626 2023-05-19 10:57:34.000000 xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_tf/agents/policy_gradient/mpdqn_agent.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     8570 2023-05-19 10:57:37.000000 xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_tf/agents/policy_gradient/pdqn_agent.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     5987 2023-05-19 10:57:39.000000 xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_tf/agents/policy_gradient/pg_agent.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     7650 2023-05-19 10:57:42.000000 xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_tf/agents/policy_gradient/ppg_agent.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     6440 2023-05-19 10:57:45.000000 xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_tf/agents/policy_gradient/ppoclip_agent.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     6372 2023-05-19 10:57:48.000000 xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_tf/agents/policy_gradient/ppokl_agent.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     6141 2023-05-19 10:57:51.000000 xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_tf/agents/policy_gradient/sac_agent.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     6289 2023-05-19 10:57:53.000000 xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_tf/agents/policy_gradient/sacdis_agent.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     8857 2023-05-19 10:57:57.000000 xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_tf/agents/policy_gradient/spdqn_agent.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     6392 2023-05-19 10:57:59.000000 xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_tf/agents/policy_gradient/td3_agent.py
-drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2023-05-22 01:37:03.000000 xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_tf/agents/qlearning_family/
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)        0 2023-05-20 05:14:54.000000 xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_tf/agents/qlearning_family/__init__.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     6251 2023-05-19 10:58:08.000000 xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_tf/agents/qlearning_family/c51_agent.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     6204 2023-05-19 10:58:11.000000 xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_tf/agents/qlearning_family/cdqn_agent.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     6177 2023-05-19 10:58:13.000000 xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_tf/agents/qlearning_family/cldqn_agent.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     6119 2023-05-19 10:58:16.000000 xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_tf/agents/qlearning_family/ddqn_agent.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     6240 2023-05-19 10:58:19.000000 xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_tf/agents/qlearning_family/dqn_agent.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     6160 2023-05-19 10:58:22.000000 xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_tf/agents/qlearning_family/dueldqn_agent.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     6204 2023-05-19 10:58:25.000000 xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_tf/agents/qlearning_family/ldqn_agent.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     6247 2023-05-19 10:58:27.000000 xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_tf/agents/qlearning_family/noisydqn_agent.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     6584 2023-05-19 10:58:30.000000 xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_tf/agents/qlearning_family/perdqn_agent.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     6220 2023-05-19 10:58:34.000000 xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_tf/agents/qlearning_family/qrdqn_agent.py
-drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2023-05-22 01:37:03.000000 xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_tf/learners/
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     3183 2023-05-19 09:59:26.000000 xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_tf/learners/__init__.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     2977 2023-05-19 10:52:57.000000 xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_tf/learners/learner.py
-drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2023-05-22 01:37:03.000000 xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_tf/learners/multi_agent_rl/
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)        0 2023-05-20 05:14:54.000000 xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_tf/learners/multi_agent_rl/__init__.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     7551 2023-05-19 10:58:59.000000 xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_tf/learners/multi_agent_rl/coma_learner.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)    10671 2023-05-19 10:59:04.000000 xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_tf/learners/multi_agent_rl/dcg_learner.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     4594 2023-05-19 10:59:08.000000 xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_tf/learners/multi_agent_rl/iddpg_learner.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     3604 2023-05-19 10:59:11.000000 xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_tf/learners/multi_agent_rl/iql_learner.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     4924 2023-05-19 10:59:14.000000 xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_tf/learners/multi_agent_rl/isac_learner.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     3862 2023-05-19 10:59:20.000000 xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_tf/learners/multi_agent_rl/maac_learner.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     4724 2023-05-19 10:59:23.000000 xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_tf/learners/multi_agent_rl/maddpg_learner.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     2642 2023-05-19 10:59:26.000000 xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_tf/learners/multi_agent_rl/madqn_learner.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     4674 2023-05-19 10:59:29.000000 xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_tf/learners/multi_agent_rl/mappoclip_learner.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     5063 2023-05-19 10:59:34.000000 xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_tf/learners/multi_agent_rl/mappokl_learner.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     4927 2023-05-19 10:59:38.000000 xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_tf/learners/multi_agent_rl/masac_learner.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     4803 2023-05-19 10:59:41.000000 xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_tf/learners/multi_agent_rl/matd3_learner.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     5847 2023-05-19 10:59:44.000000 xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_tf/learners/multi_agent_rl/mfac_learner.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     4530 2023-05-19 10:59:47.000000 xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_tf/learners/multi_agent_rl/mfq_learner.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     4044 2023-05-19 10:59:50.000000 xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_tf/learners/multi_agent_rl/qmix_learner.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     6819 2023-05-19 10:59:53.000000 xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_tf/learners/multi_agent_rl/qtran_learner.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     3738 2023-05-19 10:59:56.000000 xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_tf/learners/multi_agent_rl/vdac_learner.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     3774 2023-05-19 10:59:59.000000 xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_tf/learners/multi_agent_rl/vdn_learner.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     5695 2023-05-19 11:00:05.000000 xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_tf/learners/multi_agent_rl/wqmix_learner.py
-drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2023-05-22 01:37:03.000000 xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_tf/learners/policy_gradient/
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)        0 2023-05-20 05:14:54.000000 xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_tf/learners/policy_gradient/__init__.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     2284 2023-05-19 10:55:16.000000 xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_tf/learners/policy_gradient/a2c_learner.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     3326 2023-05-19 11:00:15.000000 xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_tf/learners/policy_gradient/ddpg_learner.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     3884 2023-05-19 11:00:18.000000 xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_tf/learners/policy_gradient/mpdqn_learner.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     3968 2023-05-19 11:00:41.000000 xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_tf/learners/policy_gradient/pdqn_learner.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1846 2023-05-19 10:53:06.000000 xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_tf/learners/policy_gradient/pg_learner.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     6707 2023-05-19 11:00:51.000000 xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_tf/learners/policy_gradient/ppg_learner.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     2614 2023-05-19 10:55:24.000000 xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_tf/learners/policy_gradient/ppoclip_learner.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     3029 2023-05-19 11:00:57.000000 xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_tf/learners/policy_gradient/ppokl_learner.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     3561 2023-05-19 11:01:01.000000 xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_tf/learners/policy_gradient/sac_learner.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     3930 2023-05-19 11:01:03.000000 xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_tf/learners/policy_gradient/sacdis_learner.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     4110 2023-05-19 11:01:06.000000 xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_tf/learners/policy_gradient/spdqn_learner.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     3666 2023-05-19 11:01:11.000000 xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_tf/learners/policy_gradient/td3_learner.py
-drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2023-05-22 01:37:03.000000 xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_tf/learners/qlearning_family/
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)        0 2023-05-20 05:14:54.000000 xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_tf/learners/qlearning_family/__init__.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     2631 2023-05-19 11:01:16.000000 xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_tf/learners/qlearning_family/c51_learner.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     2186 2023-05-19 11:01:18.000000 xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_tf/learners/qlearning_family/cdqn_learner.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     2217 2023-05-19 11:01:22.000000 xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_tf/learners/qlearning_family/cldqn_learner.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     2286 2023-05-19 11:01:25.000000 xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_tf/learners/qlearning_family/ddqn_learner.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     2198 2023-05-19 11:01:28.000000 xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_tf/learners/qlearning_family/dqn_learner.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     2211 2023-05-19 11:01:30.000000 xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_tf/learners/qlearning_family/dueldqn_learner.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     2200 2023-05-19 11:01:33.000000 xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_tf/learners/qlearning_family/ldqn_learner.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     2305 2023-05-19 11:01:37.000000 xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_tf/learners/qlearning_family/perdqn_learner.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     2453 2023-05-19 11:01:42.000000 xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_tf/learners/qlearning_family/qrdqn_learner.py
-drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2023-05-22 01:37:03.000000 xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_tf/policies/
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)    10268 2023-05-19 09:59:26.000000 xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_tf/policies/__init__.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)    10671 2023-05-19 11:02:18.000000 xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_tf/policies/categorical.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)    14795 2023-05-19 11:02:12.000000 xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_tf/policies/categorical_marl.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)    38579 2023-05-19 11:02:29.000000 xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_tf/policies/deterministic.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)    41165 2023-05-19 11:02:23.000000 xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_tf/policies/deterministic_marl.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)    11522 2023-05-19 11:02:42.000000 xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_tf/policies/gaussian.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)    12378 2023-05-19 11:02:36.000000 xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_tf/policies/gaussian_marl.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)    12868 2023-05-19 09:59:26.000000 xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_tf/policies/mixers.py
-drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2023-05-22 01:37:03.000000 xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_tf/representations/
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1706 2023-05-19 11:04:26.000000 xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_tf/representations/__init__.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)    15038 2023-05-19 11:02:57.000000 xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_tf/representations/networks.py
-drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2023-05-22 01:37:03.000000 xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_tf/runners/
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      191 2023-05-19 09:59:26.000000 xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_tf/runners/__init__.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     4560 2023-05-19 10:47:21.000000 xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_tf/runners/runner_basic.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     4508 2023-05-19 11:03:17.000000 xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_tf/runners/runner_drl.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     6633 2023-05-19 11:03:23.000000 xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_tf/runners/runner_marl.py
-drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2023-05-22 01:37:03.000000 xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_tf/utils/
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)       76 2023-05-19 09:59:25.000000 xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_tf/utils/__init__.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     2717 2023-05-19 09:59:25.000000 xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_tf/utils/distributions.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     4361 2023-05-19 11:04:42.000000 xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_tf/utils/input_reformat.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     4512 2023-05-19 09:59:25.000000 xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_tf/utils/layers.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     2500 2023-05-19 09:59:25.000000 xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_tf/utils/operations.py
-drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2023-05-22 01:37:03.000000 xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_torch/
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)        0 2023-05-19 15:23:28.000000 xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_torch/__init__.py
-drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2023-05-22 01:37:03.000000 xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_torch/agents/
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     4211 2023-05-19 09:59:26.000000 xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_torch/agents/__init__.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1347 2023-05-19 09:59:26.000000 xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_torch/agents/agent.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     3711 2023-05-19 09:59:26.000000 xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_torch/agents/agents_marl.py
-drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2023-05-22 01:37:03.000000 xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_torch/agents/multi_agent_rl/
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)        0 2023-05-20 05:14:54.000000 xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_torch/agents/multi_agent_rl/__init__.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     5854 2023-05-19 10:00:17.000000 xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_torch/agents/multi_agent_rl/coma_agents.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     5716 2023-05-21 08:32:23.000000 xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_torch/agents/multi_agent_rl/dcg_agents.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     4424 2023-05-19 10:00:17.000000 xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_torch/agents/multi_agent_rl/iddpg_agents.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     4303 2023-05-19 10:00:17.000000 xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_torch/agents/multi_agent_rl/iql_agents.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     4347 2023-05-19 10:00:17.000000 xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_torch/agents/multi_agent_rl/isac_agents.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     4429 2023-05-19 10:00:17.000000 xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_torch/agents/multi_agent_rl/maddpg_agents.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     7234 2023-05-19 10:00:17.000000 xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_torch/agents/multi_agent_rl/madqn_agents.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     4994 2023-05-19 10:00:17.000000 xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_torch/agents/multi_agent_rl/mappoclip_agents.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     4939 2023-05-19 10:00:17.000000 xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_torch/agents/multi_agent_rl/mappokl_agents.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     4350 2023-05-19 10:00:17.000000 xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_torch/agents/multi_agent_rl/masac_agents.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     4745 2023-05-19 10:00:17.000000 xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_torch/agents/multi_agent_rl/matd3_agents.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     5885 2023-05-19 10:00:17.000000 xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_torch/agents/multi_agent_rl/mfac_agents.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     6073 2023-05-19 10:00:17.000000 xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_torch/agents/multi_agent_rl/mfq_agents.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     4475 2023-05-19 10:00:17.000000 xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_torch/agents/multi_agent_rl/qmix_agents.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     4925 2023-05-19 10:00:17.000000 xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_torch/agents/multi_agent_rl/qtran_agents.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     5419 2023-05-19 10:00:17.000000 xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_torch/agents/multi_agent_rl/vdac_agents.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     4338 2023-05-19 10:00:17.000000 xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_torch/agents/multi_agent_rl/vdn_agents.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     4634 2023-05-19 10:00:17.000000 xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_torch/agents/multi_agent_rl/wqmix_agents.py
-drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2023-05-22 01:37:03.000000 xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_torch/agents/policy_gradient/
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)        0 2023-05-20 05:14:54.000000 xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_torch/agents/policy_gradient/__init__.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     6336 2023-05-19 10:00:17.000000 xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_torch/agents/policy_gradient/a2c_agent.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     6377 2023-05-19 10:00:17.000000 xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_torch/agents/policy_gradient/ddpg_agent.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     8623 2023-05-19 10:00:17.000000 xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_torch/agents/policy_gradient/mpdqn_agent.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     8612 2023-05-19 10:00:17.000000 xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_torch/agents/policy_gradient/pdqn_agent.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     6136 2023-05-19 10:00:17.000000 xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_torch/agents/policy_gradient/pg_agent.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     7564 2023-05-19 10:00:17.000000 xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_torch/agents/policy_gradient/ppg_agent.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     6602 2023-05-19 10:00:17.000000 xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_torch/agents/policy_gradient/ppoclip_agent.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     6517 2023-05-19 10:00:17.000000 xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_torch/agents/policy_gradient/ppokl_agent.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     6361 2023-05-19 10:00:17.000000 xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_torch/agents/policy_gradient/sac_agent.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     6505 2023-05-19 10:00:17.000000 xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_torch/agents/policy_gradient/sacdis_agent.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     8594 2023-05-19 10:00:17.000000 xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_torch/agents/policy_gradient/spdqn_agent.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     6570 2023-05-19 10:00:17.000000 xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_torch/agents/policy_gradient/td3_agent.py
-drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2023-05-22 01:37:03.000000 xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_torch/agents/qlearning_family/
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)        0 2023-05-20 05:14:54.000000 xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_torch/agents/qlearning_family/__init__.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     6365 2023-05-19 10:00:18.000000 xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_torch/agents/qlearning_family/c51_agent.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     6367 2023-05-19 10:00:18.000000 xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_torch/agents/qlearning_family/cdqn_agent.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     6369 2023-05-19 10:00:18.000000 xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_torch/agents/qlearning_family/cldqn_agent.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     6294 2023-05-19 10:00:18.000000 xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_torch/agents/qlearning_family/ddqn_agent.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     6365 2023-05-19 10:00:18.000000 xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_torch/agents/qlearning_family/dqn_agent.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     6367 2023-05-19 10:00:18.000000 xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_torch/agents/qlearning_family/dueldqn_agent.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     6367 2023-05-19 10:00:18.000000 xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_torch/agents/qlearning_family/ldqn_agent.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     6381 2023-05-19 10:00:18.000000 xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_torch/agents/qlearning_family/noisydqn_agent.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     6707 2023-05-19 10:00:18.000000 xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_torch/agents/qlearning_family/perdqn_agent.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     6385 2023-05-19 10:00:18.000000 xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_torch/agents/qlearning_family/qrdqn_agent.py
-drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2023-05-22 01:37:03.000000 xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_torch/learners/
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     2500 2023-05-21 08:10:27.000000 xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_torch/learners/__init__.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     3490 2023-05-19 09:59:26.000000 xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_torch/learners/learner.py
-drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2023-05-22 01:37:03.000000 xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_torch/learners/multi_agent_rl/
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)        0 2023-05-20 05:14:54.000000 xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_torch/learners/multi_agent_rl/__init__.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     6343 2023-05-19 10:00:19.000000 xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_torch/learners/multi_agent_rl/coma_learner.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     6622 2023-05-19 10:00:19.000000 xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_torch/learners/multi_agent_rl/dcg_learner.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     3627 2023-05-19 10:00:19.000000 xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_torch/learners/multi_agent_rl/iddpg_learner.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     2882 2023-05-19 10:00:19.000000 xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_torch/learners/multi_agent_rl/iql_learner.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     4143 2023-05-19 10:00:19.000000 xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_torch/learners/multi_agent_rl/isac_learner.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     3859 2023-05-19 10:00:19.000000 xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_torch/learners/multi_agent_rl/maddpg_learner.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     2674 2023-05-19 10:00:19.000000 xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_torch/learners/multi_agent_rl/madqn_learner.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     3867 2023-05-19 10:00:19.000000 xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_torch/learners/multi_agent_rl/mappoclip_learner.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     4207 2023-05-19 10:00:19.000000 xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_torch/learners/multi_agent_rl/mappokl_learner.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     4146 2023-05-19 10:00:19.000000 xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_torch/learners/multi_agent_rl/masac_learner.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     4185 2023-05-19 10:00:19.000000 xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_torch/learners/multi_agent_rl/matd3_learner.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     4909 2023-05-19 10:00:19.000000 xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_torch/learners/multi_agent_rl/mfac_learner.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     3402 2023-05-19 10:00:19.000000 xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_torch/learners/multi_agent_rl/mfq_learner.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     3262 2023-05-19 10:00:19.000000 xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_torch/learners/multi_agent_rl/qmix_learner.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     5772 2023-05-19 10:00:19.000000 xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_torch/learners/multi_agent_rl/qtran_learner.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     2900 2023-05-19 10:00:19.000000 xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_torch/learners/multi_agent_rl/vdac_learner.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     3033 2023-05-19 10:00:19.000000 xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_torch/learners/multi_agent_rl/vdn_learner.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     4702 2023-05-19 10:00:19.000000 xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_torch/learners/multi_agent_rl/wqmix_learner.py
-drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2023-05-22 01:37:03.000000 xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_torch/learners/policy_gradient/
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)        0 2023-05-20 05:14:54.000000 xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_torch/learners/policy_gradient/__init__.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     2113 2023-05-19 10:00:20.000000 xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_torch/learners/policy_gradient/a2c_learner.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     2273 2023-05-19 10:00:20.000000 xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_torch/learners/policy_gradient/ddpg_learner.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     2516 2023-05-19 10:00:20.000000 xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_torch/learners/policy_gradient/mpdqn_learner.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)        0 2023-05-19 10:00:20.000000 xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_torch/learners/policy_gradient/npg_learner.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     2528 2023-05-19 10:00:20.000000 xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_torch/learners/policy_gradient/pdqn_learner.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1718 2023-05-19 10:00:20.000000 xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_torch/learners/policy_gradient/pg_learner.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     3779 2023-05-19 10:00:20.000000 xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_torch/learners/policy_gradient/ppg_learner.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     2528 2023-05-19 10:00:19.000000 xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_torch/learners/policy_gradient/ppoclip_learner.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     2698 2023-05-19 10:00:20.000000 xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_torch/learners/policy_gradient/ppokl_learner.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     2360 2023-05-19 10:00:19.000000 xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_torch/learners/policy_gradient/sac_learner.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     2802 2023-05-19 10:00:19.000000 xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_torch/learners/policy_gradient/sacdis_learner.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     2516 2023-05-19 10:00:19.000000 xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_torch/learners/policy_gradient/spdqn_learner.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     2656 2023-05-19 10:00:20.000000 xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_torch/learners/policy_gradient/td3_learner.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)        0 2023-05-19 10:00:19.000000 xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_torch/learners/policy_gradient/trpo_learner.py
-drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2023-05-22 01:37:03.000000 xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_torch/learners/qlearning_family/
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)        0 2023-05-20 05:14:54.000000 xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_torch/learners/qlearning_family/__init__.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     2373 2023-05-19 10:00:20.000000 xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_torch/learners/qlearning_family/c51_learner.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1965 2023-05-19 10:00:20.000000 xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_torch/learners/qlearning_family/cdqn_learner.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1967 2023-05-19 10:00:20.000000 xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_torch/learners/qlearning_family/cldqn_learner.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     2033 2023-05-19 10:00:20.000000 xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_torch/learners/qlearning_family/ddqn_learner.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1963 2023-05-19 10:00:20.000000 xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_torch/learners/qlearning_family/dqn_learner.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1971 2023-05-19 10:00:20.000000 xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_torch/learners/qlearning_family/dueldqn_learner.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1965 2023-05-19 10:00:20.000000 xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_torch/learners/qlearning_family/ldqn_learner.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     2071 2023-05-19 10:00:20.000000 xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_torch/learners/qlearning_family/perdqn_learner.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     2030 2023-05-19 10:00:20.000000 xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_torch/learners/qlearning_family/qrdqn_learner.py
-drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2023-05-22 01:37:03.000000 xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_torch/learners/ssl_rl/
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)        0 2023-05-20 05:14:54.000000 xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_torch/learners/ssl_rl/__init__.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)        0 2023-05-19 10:00:20.000000 xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_torch/learners/ssl_rl/curl_learner.py
-drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2023-05-22 01:37:03.000000 xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_torch/policies/
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     9885 2023-05-19 09:59:26.000000 xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_torch/policies/__init__.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)    11017 2023-05-19 09:59:26.000000 xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_torch/policies/categorical.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)    12561 2023-05-19 09:59:26.000000 xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_torch/policies/categorical_marl.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     3963 2023-05-21 08:32:23.000000 xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_torch/policies/coordination_graph.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)    35481 2023-05-19 09:59:26.000000 xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_torch/policies/deterministic.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)    24444 2023-05-21 08:38:03.000000 xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_torch/policies/deterministic_marl.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)    11121 2023-05-19 09:59:26.000000 xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_torch/policies/gaussian.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)    10660 2023-05-19 09:59:26.000000 xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_torch/policies/gaussian_marl.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     6643 2023-05-21 08:32:23.000000 xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_torch/policies/mixers.py
-drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2023-05-22 01:37:03.000000 xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_torch/representations/
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1792 2023-05-19 09:59:26.000000 xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_torch/representations/__init__.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)    15015 2023-05-19 09:59:26.000000 xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_torch/representations/networks.py
-drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2023-05-22 01:37:03.000000 xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_torch/runners/
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      188 2023-05-19 09:59:26.000000 xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_torch/runners/__init__.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     4213 2023-05-20 08:50:30.000000 xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_torch/runners/runner_basic.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     4901 2023-05-19 09:59:26.000000 xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_torch/runners/runner_drl.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     6683 2023-05-20 08:53:24.000000 xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_torch/runners/runner_marl.py
-drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2023-05-22 01:37:03.000000 xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_torch/utils/
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)       76 2023-05-19 09:59:26.000000 xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_torch/utils/__init__.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     2700 2023-05-19 09:59:26.000000 xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_torch/utils/distributions.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     4281 2023-05-19 09:59:26.000000 xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_torch/utils/input_reformat.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     4024 2023-05-19 09:59:26.000000 xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_torch/utils/layers.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     2441 2023-05-19 09:59:26.000000 xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_torch/utils/operations.py
-drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2023-05-22 01:37:03.000000 xuanpolicy-0.1.5/xuanpolicy.egg-info/
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      864 2023-05-22 01:37:03.000000 xuanpolicy-0.1.5/xuanpolicy.egg-info/PKG-INFO
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)    24242 2023-05-22 01:37:03.000000 xuanpolicy-0.1.5/xuanpolicy.egg-info/SOURCES.txt
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)        1 2023-05-22 01:37:03.000000 xuanpolicy-0.1.5/xuanpolicy.egg-info/dependency_links.txt
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      295 2023-05-22 01:37:03.000000 xuanpolicy-0.1.5/xuanpolicy.egg-info/requires.txt
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)       11 2023-05-22 01:37:03.000000 xuanpolicy-0.1.5/xuanpolicy.egg-info/top_level.txt
+drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2023-05-22 12:59:05.000000 xuanpolicy-0.1.6/
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1075 2023-05-19 14:11:29.000000 xuanpolicy-0.1.6/LICENSE.txt
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      864 2023-05-22 12:59:05.000000 xuanpolicy-0.1.6/PKG-INFO
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)    14400 2023-05-22 09:09:41.000000 xuanpolicy-0.1.6/README.md
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)       79 2023-05-22 12:59:05.000000 xuanpolicy-0.1.6/setup.cfg
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1945 2023-05-22 12:58:02.000000 xuanpolicy-0.1.6/setup.py
+drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2023-05-22 12:59:05.000000 xuanpolicy-0.1.6/xuanpolicy/
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      158 2023-05-22 02:23:34.000000 xuanpolicy-0.1.6/xuanpolicy/__init__.py
+drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2023-05-22 12:59:05.000000 xuanpolicy-0.1.6/xuanpolicy/common/
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      233 2023-05-20 06:35:52.000000 xuanpolicy-0.1.6/xuanpolicy/common/__init__.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     7615 2023-05-22 12:28:36.000000 xuanpolicy-0.1.6/xuanpolicy/common/common_tools.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)    16545 2023-05-20 04:14:13.000000 xuanpolicy-0.1.6/xuanpolicy/common/memory_tools.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)    20041 2023-05-19 09:59:24.000000 xuanpolicy-0.1.6/xuanpolicy/common/memory_tools_marl.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     2879 2023-05-19 09:59:24.000000 xuanpolicy-0.1.6/xuanpolicy/common/segtree_tool.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     5059 2023-05-19 09:59:24.000000 xuanpolicy-0.1.6/xuanpolicy/common/statistic_tools.py
+drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2023-05-22 12:59:05.000000 xuanpolicy-0.1.6/xuanpolicy/configs/
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)        0 2023-05-20 06:49:02.000000 xuanpolicy-0.1.6/xuanpolicy/configs/__init__.py
+drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2023-05-22 12:59:05.000000 xuanpolicy-0.1.6/xuanpolicy/configs/a2c/
+drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2023-05-22 12:59:05.000000 xuanpolicy-0.1.6/xuanpolicy/configs/a2c/mujoco/
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      589 2023-05-19 10:00:26.000000 xuanpolicy-0.1.6/xuanpolicy/configs/a2c/mujoco/InvertedPendulum-v2.yaml
+drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2023-05-22 12:59:05.000000 xuanpolicy-0.1.6/xuanpolicy/configs/a2c/toy/
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      569 2023-05-22 09:09:41.000000 xuanpolicy-0.1.6/xuanpolicy/configs/a2c/toy/CartPole-v0.yaml
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      584 2023-05-22 10:37:37.000000 xuanpolicy-0.1.6/xuanpolicy/configs/basic.yaml
+drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2023-05-22 12:59:05.000000 xuanpolicy-0.1.6/xuanpolicy/configs/c51/
+drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2023-05-22 12:59:05.000000 xuanpolicy-0.1.6/xuanpolicy/configs/c51/toy/
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      504 2023-05-22 09:09:41.000000 xuanpolicy-0.1.6/xuanpolicy/configs/c51/toy/Acrobot-v1.yaml
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      505 2023-05-22 09:09:41.000000 xuanpolicy-0.1.6/xuanpolicy/configs/c51/toy/CartPole-v0.yaml
+drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2023-05-22 12:59:05.000000 xuanpolicy-0.1.6/xuanpolicy/configs/cdqn/
+drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2023-05-22 12:59:05.000000 xuanpolicy-0.1.6/xuanpolicy/configs/cdqn/toy/
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      471 2023-05-22 09:09:41.000000 xuanpolicy-0.1.6/xuanpolicy/configs/cdqn/toy/CartPole-v0.yaml
+drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2023-05-22 12:59:05.000000 xuanpolicy-0.1.6/xuanpolicy/configs/cldqn/
+drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2023-05-22 12:59:05.000000 xuanpolicy-0.1.6/xuanpolicy/configs/cldqn/toy/
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      475 2023-05-22 09:09:41.000000 xuanpolicy-0.1.6/xuanpolicy/configs/cldqn/toy/CartPole-v0.yaml
+drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2023-05-22 12:59:05.000000 xuanpolicy-0.1.6/xuanpolicy/configs/coma/
+drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2023-05-22 12:59:05.000000 xuanpolicy-0.1.6/xuanpolicy/configs/coma/mpe/
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      929 2023-05-20 08:41:30.000000 xuanpolicy-0.1.6/xuanpolicy/configs/coma/mpe/simple_spread.yaml
+drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2023-05-22 12:59:05.000000 xuanpolicy-0.1.6/xuanpolicy/configs/cwqmix/
+drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2023-05-22 12:59:05.000000 xuanpolicy-0.1.6/xuanpolicy/configs/cwqmix/mpe/
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      953 2023-05-20 08:41:40.000000 xuanpolicy-0.1.6/xuanpolicy/configs/cwqmix/mpe/simple_spread.yaml
+drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2023-05-22 12:59:05.000000 xuanpolicy-0.1.6/xuanpolicy/configs/dcg/
+drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2023-05-22 12:59:05.000000 xuanpolicy-0.1.6/xuanpolicy/configs/dcg/mpe/
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1391 2023-05-20 08:41:51.000000 xuanpolicy-0.1.6/xuanpolicy/configs/dcg/mpe/simple_spread.yaml
+drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2023-05-22 12:59:05.000000 xuanpolicy-0.1.6/xuanpolicy/configs/ddpg/
+drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2023-05-22 12:59:05.000000 xuanpolicy-0.1.6/xuanpolicy/configs/ddpg/mujoco/
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      556 2023-05-19 10:00:23.000000 xuanpolicy-0.1.6/xuanpolicy/configs/ddpg/mujoco/HalfCheetah-v3.yaml
+drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2023-05-22 12:59:05.000000 xuanpolicy-0.1.6/xuanpolicy/configs/ddpg/toy/
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      552 2023-05-22 09:09:41.000000 xuanpolicy-0.1.6/xuanpolicy/configs/ddpg/toy/Pendulum-v1.yaml
+drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2023-05-22 12:59:05.000000 xuanpolicy-0.1.6/xuanpolicy/configs/ddqn/
+drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2023-05-22 12:59:05.000000 xuanpolicy-0.1.6/xuanpolicy/configs/ddqn/toy/
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      475 2023-05-22 09:09:41.000000 xuanpolicy-0.1.6/xuanpolicy/configs/ddqn/toy/Acrobot-v1.yaml
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      476 2023-05-22 09:09:41.000000 xuanpolicy-0.1.6/xuanpolicy/configs/ddqn/toy/CartPole-v0.yaml
+drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2023-05-22 12:59:05.000000 xuanpolicy-0.1.6/xuanpolicy/configs/dqn/
+drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2023-05-22 12:59:05.000000 xuanpolicy-0.1.6/xuanpolicy/configs/dqn/toy/
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      491 2023-05-22 09:09:41.000000 xuanpolicy-0.1.6/xuanpolicy/configs/dqn/toy/CartPole-v0.yaml
+drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2023-05-22 12:59:05.000000 xuanpolicy-0.1.6/xuanpolicy/configs/dueldqn/
+drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2023-05-22 12:59:05.000000 xuanpolicy-0.1.6/xuanpolicy/configs/dueldqn/toy/
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      484 2023-05-22 09:09:41.000000 xuanpolicy-0.1.6/xuanpolicy/configs/dueldqn/toy/Acrobot-v1.yaml
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      485 2023-05-22 09:09:41.000000 xuanpolicy-0.1.6/xuanpolicy/configs/dueldqn/toy/CartPole-v0.yaml
+drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2023-05-22 12:59:05.000000 xuanpolicy-0.1.6/xuanpolicy/configs/iddpg/
+drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2023-05-22 12:59:05.000000 xuanpolicy-0.1.6/xuanpolicy/configs/iddpg/mpe/
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      906 2023-05-22 10:48:31.000000 xuanpolicy-0.1.6/xuanpolicy/configs/iddpg/mpe/simple_adversary.yaml
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      901 2023-05-22 10:17:25.000000 xuanpolicy-0.1.6/xuanpolicy/configs/iddpg/mpe/simple_push.yaml
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      903 2023-05-20 08:42:25.000000 xuanpolicy-0.1.6/xuanpolicy/configs/iddpg/mpe/simple_spread.yaml
+drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2023-05-22 12:59:05.000000 xuanpolicy-0.1.6/xuanpolicy/configs/iql/
+drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2023-05-22 12:59:05.000000 xuanpolicy-0.1.6/xuanpolicy/configs/iql/mpe/
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      809 2023-05-20 08:42:37.000000 xuanpolicy-0.1.6/xuanpolicy/configs/iql/mpe/simple_spread.yaml
+drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2023-05-22 12:59:05.000000 xuanpolicy-0.1.6/xuanpolicy/configs/isac/
+drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2023-05-22 12:59:05.000000 xuanpolicy-0.1.6/xuanpolicy/configs/isac/mpe/
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      913 2023-05-22 10:50:16.000000 xuanpolicy-0.1.6/xuanpolicy/configs/isac/mpe/simple_adversary.yaml
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      908 2023-05-22 10:17:25.000000 xuanpolicy-0.1.6/xuanpolicy/configs/isac/mpe/simple_push.yaml
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      910 2023-05-20 08:42:53.000000 xuanpolicy-0.1.6/xuanpolicy/configs/isac/mpe/simple_spread.yaml
+drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2023-05-22 12:59:05.000000 xuanpolicy-0.1.6/xuanpolicy/configs/ldqn/
+drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2023-05-22 12:59:05.000000 xuanpolicy-0.1.6/xuanpolicy/configs/ldqn/toy/
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      471 2023-05-22 09:09:41.000000 xuanpolicy-0.1.6/xuanpolicy/configs/ldqn/toy/CartPole-v0.yaml
+drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2023-05-22 12:59:05.000000 xuanpolicy-0.1.6/xuanpolicy/configs/maddpg/
+drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2023-05-22 12:59:05.000000 xuanpolicy-0.1.6/xuanpolicy/configs/maddpg/mpe/
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      947 2023-05-22 10:50:16.000000 xuanpolicy-0.1.6/xuanpolicy/configs/maddpg/mpe/simple_adversary.yaml
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      942 2023-05-22 10:17:25.000000 xuanpolicy-0.1.6/xuanpolicy/configs/maddpg/mpe/simple_push.yaml
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      944 2023-05-20 09:18:32.000000 xuanpolicy-0.1.6/xuanpolicy/configs/maddpg/mpe/simple_spread.yaml
+drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2023-05-22 12:59:05.000000 xuanpolicy-0.1.6/xuanpolicy/configs/mappoclip/
+drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2023-05-22 12:59:05.000000 xuanpolicy-0.1.6/xuanpolicy/configs/mappoclip/mpe/
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1089 2023-05-20 08:43:44.000000 xuanpolicy-0.1.6/xuanpolicy/configs/mappoclip/mpe/simple_spread.yaml
+drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2023-05-22 12:59:05.000000 xuanpolicy-0.1.6/xuanpolicy/configs/mappokl/
+drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2023-05-22 12:59:05.000000 xuanpolicy-0.1.6/xuanpolicy/configs/mappokl/mpe/
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1080 2023-05-20 08:43:53.000000 xuanpolicy-0.1.6/xuanpolicy/configs/mappokl/mpe/simple_spread.yaml
+drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2023-05-22 12:59:05.000000 xuanpolicy-0.1.6/xuanpolicy/configs/masac/
+drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2023-05-22 12:59:05.000000 xuanpolicy-0.1.6/xuanpolicy/configs/masac/mpe/
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      912 2023-05-22 10:17:25.000000 xuanpolicy-0.1.6/xuanpolicy/configs/masac/mpe/simple_push.yaml
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      914 2023-05-20 08:44:07.000000 xuanpolicy-0.1.6/xuanpolicy/configs/masac/mpe/simple_spread.yaml
+drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2023-05-22 12:59:05.000000 xuanpolicy-0.1.6/xuanpolicy/configs/matd3/
+drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2023-05-22 12:59:05.000000 xuanpolicy-0.1.6/xuanpolicy/configs/matd3/mpe/
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      890 2023-05-22 10:17:25.000000 xuanpolicy-0.1.6/xuanpolicy/configs/matd3/mpe/simple_push.yaml
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      892 2023-05-20 08:44:18.000000 xuanpolicy-0.1.6/xuanpolicy/configs/matd3/mpe/simple_spread.yaml
+drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2023-05-22 12:59:05.000000 xuanpolicy-0.1.6/xuanpolicy/configs/mfac/
+drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2023-05-22 12:59:05.000000 xuanpolicy-0.1.6/xuanpolicy/configs/mfac/mpe/
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      949 2023-05-20 08:44:25.000000 xuanpolicy-0.1.6/xuanpolicy/configs/mfac/mpe/simple_spread.yaml
+drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2023-05-22 12:59:05.000000 xuanpolicy-0.1.6/xuanpolicy/configs/mfq/
+drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2023-05-22 12:59:05.000000 xuanpolicy-0.1.6/xuanpolicy/configs/mfq/mpe/
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      806 2023-05-20 08:44:34.000000 xuanpolicy-0.1.6/xuanpolicy/configs/mfq/mpe/simple_spread.yaml
+drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2023-05-22 12:59:05.000000 xuanpolicy-0.1.6/xuanpolicy/configs/mpdqn/
+drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2023-05-22 12:59:05.000000 xuanpolicy-0.1.6/xuanpolicy/configs/mpdqn/toy/
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      523 2023-05-22 09:09:41.000000 xuanpolicy-0.1.6/xuanpolicy/configs/mpdqn/toy/Platform-v0.yaml
+drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2023-05-22 12:59:05.000000 xuanpolicy-0.1.6/xuanpolicy/configs/noisydqn/
+drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2023-05-22 12:59:05.000000 xuanpolicy-0.1.6/xuanpolicy/configs/noisydqn/toy/
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      486 2023-05-22 09:09:41.000000 xuanpolicy-0.1.6/xuanpolicy/configs/noisydqn/toy/Acrobot-v1.yaml
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      487 2023-05-22 09:09:41.000000 xuanpolicy-0.1.6/xuanpolicy/configs/noisydqn/toy/CartPole-v0.yaml
+drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2023-05-22 12:59:05.000000 xuanpolicy-0.1.6/xuanpolicy/configs/owqmix/
+drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2023-05-22 12:59:05.000000 xuanpolicy-0.1.6/xuanpolicy/configs/owqmix/mpe/
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      953 2023-05-20 08:44:43.000000 xuanpolicy-0.1.6/xuanpolicy/configs/owqmix/mpe/simple_spread.yaml
+drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2023-05-22 12:59:05.000000 xuanpolicy-0.1.6/xuanpolicy/configs/pdqn/
+drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2023-05-22 12:59:05.000000 xuanpolicy-0.1.6/xuanpolicy/configs/pdqn/toy/
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      519 2023-05-22 09:09:41.000000 xuanpolicy-0.1.6/xuanpolicy/configs/pdqn/toy/Platform-v0.yaml
+drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2023-05-22 12:59:05.000000 xuanpolicy-0.1.6/xuanpolicy/configs/perdqn/
+drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2023-05-22 12:59:05.000000 xuanpolicy-0.1.6/xuanpolicy/configs/perdqn/toy/
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      512 2023-05-22 09:09:41.000000 xuanpolicy-0.1.6/xuanpolicy/configs/perdqn/toy/CartPole-v0.yaml
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      515 2023-05-22 09:09:41.000000 xuanpolicy-0.1.6/xuanpolicy/configs/perdqn/toy/MountainCar-v0.yaml
+drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2023-05-22 12:59:05.000000 xuanpolicy-0.1.6/xuanpolicy/configs/pg/
+drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2023-05-22 12:59:05.000000 xuanpolicy-0.1.6/xuanpolicy/configs/pg/mujoco/
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      549 2023-05-19 10:00:24.000000 xuanpolicy-0.1.6/xuanpolicy/configs/pg/mujoco/InvertedPendulum-v2.yaml
+drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2023-05-22 12:59:05.000000 xuanpolicy-0.1.6/xuanpolicy/configs/pg/toy/
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      515 2023-05-22 09:09:41.000000 xuanpolicy-0.1.6/xuanpolicy/configs/pg/toy/CartPole-v0.yaml
+drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2023-05-22 12:59:05.000000 xuanpolicy-0.1.6/xuanpolicy/configs/ppg/
+drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2023-05-22 12:59:05.000000 xuanpolicy-0.1.6/xuanpolicy/configs/ppg/mujoco/
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      546 2023-05-19 10:00:26.000000 xuanpolicy-0.1.6/xuanpolicy/configs/ppg/mujoco/InvertedPendulum-v2.yaml
+drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2023-05-22 12:59:05.000000 xuanpolicy-0.1.6/xuanpolicy/configs/ppg/toy/
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      513 2023-05-22 09:09:42.000000 xuanpolicy-0.1.6/xuanpolicy/configs/ppg/toy/CartPole-v0.yaml
+drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2023-05-22 12:59:05.000000 xuanpolicy-0.1.6/xuanpolicy/configs/ppoclip/
+drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2023-05-22 12:59:05.000000 xuanpolicy-0.1.6/xuanpolicy/configs/ppoclip/atari/
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      587 2023-05-19 10:00:21.000000 xuanpolicy-0.1.6/xuanpolicy/configs/ppoclip/atari/PongNoFrameskip-v4.yaml
+drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2023-05-22 12:59:05.000000 xuanpolicy-0.1.6/xuanpolicy/configs/ppoclip/mujoco/
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      514 2023-05-19 10:00:22.000000 xuanpolicy-0.1.6/xuanpolicy/configs/ppoclip/mujoco/InvertedPendulum-v2.yaml
+drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2023-05-22 12:59:05.000000 xuanpolicy-0.1.6/xuanpolicy/configs/ppoclip/toy/
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      478 2023-05-22 09:09:41.000000 xuanpolicy-0.1.6/xuanpolicy/configs/ppoclip/toy/CartPole-v0.yaml
+drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2023-05-22 12:59:05.000000 xuanpolicy-0.1.6/xuanpolicy/configs/ppokl/
+drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2023-05-22 12:59:05.000000 xuanpolicy-0.1.6/xuanpolicy/configs/ppokl/mujoco/
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      506 2023-05-19 10:00:22.000000 xuanpolicy-0.1.6/xuanpolicy/configs/ppokl/mujoco/InvertedPendulum-v2.yaml
+drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2023-05-22 12:59:05.000000 xuanpolicy-0.1.6/xuanpolicy/configs/ppokl/toy/
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      472 2023-05-22 09:09:41.000000 xuanpolicy-0.1.6/xuanpolicy/configs/ppokl/toy/CartPole-v0.yaml
+drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2023-05-22 12:59:05.000000 xuanpolicy-0.1.6/xuanpolicy/configs/qmix/
+drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2023-05-22 12:59:05.000000 xuanpolicy-0.1.6/xuanpolicy/configs/qmix/mpe/
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      903 2023-05-20 08:31:40.000000 xuanpolicy-0.1.6/xuanpolicy/configs/qmix/mpe/simple_spread.yaml
+drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2023-05-22 12:59:05.000000 xuanpolicy-0.1.6/xuanpolicy/configs/qrdqn/
+drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2023-05-22 12:59:05.000000 xuanpolicy-0.1.6/xuanpolicy/configs/qrdqn/toy/
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      492 2023-05-22 09:09:41.000000 xuanpolicy-0.1.6/xuanpolicy/configs/qrdqn/toy/Acrobot-v1.yaml
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      493 2023-05-22 09:09:42.000000 xuanpolicy-0.1.6/xuanpolicy/configs/qrdqn/toy/CartPole-v0.yaml
+drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2023-05-22 12:59:05.000000 xuanpolicy-0.1.6/xuanpolicy/configs/qtran/
+drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2023-05-22 12:59:05.000000 xuanpolicy-0.1.6/xuanpolicy/configs/qtran/mpe/
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      883 2023-05-20 08:44:57.000000 xuanpolicy-0.1.6/xuanpolicy/configs/qtran/mpe/simple_spread.yaml
+drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2023-05-22 12:59:05.000000 xuanpolicy-0.1.6/xuanpolicy/configs/random/
+drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2023-05-22 12:59:05.000000 xuanpolicy-0.1.6/xuanpolicy/configs/random/mpe/
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      104 2023-05-22 12:30:21.000000 xuanpolicy-0.1.6/xuanpolicy/configs/random/mpe/simple_adversary.yaml
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)       99 2023-05-22 12:30:21.000000 xuanpolicy-0.1.6/xuanpolicy/configs/random/mpe/simple_push.yaml
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      101 2023-05-22 12:30:21.000000 xuanpolicy-0.1.6/xuanpolicy/configs/random/mpe/simple_spread.yaml
+drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2023-05-22 12:59:05.000000 xuanpolicy-0.1.6/xuanpolicy/configs/sac/
+drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2023-05-22 12:59:05.000000 xuanpolicy-0.1.6/xuanpolicy/configs/sac/mujoco/
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      566 2023-05-19 10:00:22.000000 xuanpolicy-0.1.6/xuanpolicy/configs/sac/mujoco/HalfCheetah-v3.yaml
+drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2023-05-22 12:59:05.000000 xuanpolicy-0.1.6/xuanpolicy/configs/sac/toy/
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      503 2023-05-22 09:09:42.000000 xuanpolicy-0.1.6/xuanpolicy/configs/sac/toy/Pendulum-v1.yaml
+drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2023-05-22 12:59:05.000000 xuanpolicy-0.1.6/xuanpolicy/configs/sacdis/
+drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2023-05-22 12:59:05.000000 xuanpolicy-0.1.6/xuanpolicy/configs/sacdis/toy/
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      570 2023-05-22 09:09:42.000000 xuanpolicy-0.1.6/xuanpolicy/configs/sacdis/toy/CartPole-v0.yaml
+drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2023-05-22 12:59:05.000000 xuanpolicy-0.1.6/xuanpolicy/configs/spdqn/
+drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2023-05-22 12:59:05.000000 xuanpolicy-0.1.6/xuanpolicy/configs/spdqn/toy/
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      523 2023-05-22 09:09:41.000000 xuanpolicy-0.1.6/xuanpolicy/configs/spdqn/toy/Platform-v0.yaml
+drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2023-05-22 12:59:05.000000 xuanpolicy-0.1.6/xuanpolicy/configs/td3/
+drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2023-05-22 12:59:05.000000 xuanpolicy-0.1.6/xuanpolicy/configs/td3/mujoco/
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      557 2023-05-19 10:00:27.000000 xuanpolicy-0.1.6/xuanpolicy/configs/td3/mujoco/InvertedPendulum-v2.yaml
+drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2023-05-22 12:59:05.000000 xuanpolicy-0.1.6/xuanpolicy/configs/td3/toy/
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      514 2023-05-22 09:09:41.000000 xuanpolicy-0.1.6/xuanpolicy/configs/td3/toy/Pendulum-v1.yaml
+drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2023-05-22 12:59:05.000000 xuanpolicy-0.1.6/xuanpolicy/configs/vdac/
+drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2023-05-22 12:59:05.000000 xuanpolicy-0.1.6/xuanpolicy/configs/vdac/mpe/
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      973 2023-05-20 08:45:09.000000 xuanpolicy-0.1.6/xuanpolicy/configs/vdac/mpe/simple_spread.yaml
+drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2023-05-22 12:59:05.000000 xuanpolicy-0.1.6/xuanpolicy/configs/vdn/
+drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2023-05-22 12:59:05.000000 xuanpolicy-0.1.6/xuanpolicy/configs/vdn/mpe/
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      804 2023-05-20 08:45:16.000000 xuanpolicy-0.1.6/xuanpolicy/configs/vdn/mpe/simple_spread.yaml
+drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2023-05-22 12:59:05.000000 xuanpolicy-0.1.6/xuanpolicy/environment/
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     2038 2023-05-22 08:00:32.000000 xuanpolicy-0.1.6/xuanpolicy/environment/__init__.py
+drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2023-05-22 12:59:05.000000 xuanpolicy-0.1.6/xuanpolicy/environment/custom_envs/
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     5124 2023-05-19 09:59:27.000000 xuanpolicy-0.1.6/xuanpolicy/environment/custom_envs/USVmodel.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)        0 2023-05-20 02:01:16.000000 xuanpolicy-0.1.6/xuanpolicy/environment/custom_envs/__init__.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     3341 2023-05-19 09:59:27.000000 xuanpolicy-0.1.6/xuanpolicy/environment/custom_envs/atari_env.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1429 2023-05-19 09:59:27.000000 xuanpolicy-0.1.6/xuanpolicy/environment/custom_envs/mujoco_env.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     5424 2023-05-22 08:23:29.000000 xuanpolicy-0.1.6/xuanpolicy/environment/custom_envs/pettingzoo_env.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      316 2023-05-19 09:59:27.000000 xuanpolicy-0.1.6/xuanpolicy/environment/custom_envs/robotics_env.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      981 2023-05-19 09:59:27.000000 xuanpolicy-0.1.6/xuanpolicy/environment/custom_envs/toy_env.py
+drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2023-05-22 12:59:05.000000 xuanpolicy-0.1.6/xuanpolicy/environment/vector_envs/
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)        0 2023-05-20 05:13:59.000000 xuanpolicy-0.1.6/xuanpolicy/environment/vector_envs/__init__.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     8938 2023-05-22 07:52:19.000000 xuanpolicy-0.1.6/xuanpolicy/environment/vector_envs/dummy_vec_env.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     3981 2023-05-19 09:59:27.000000 xuanpolicy-0.1.6/xuanpolicy/environment/vector_envs/env_utils.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     6166 2023-05-19 09:59:27.000000 xuanpolicy-0.1.6/xuanpolicy/environment/vector_envs/subproc_vec_env.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     3396 2023-05-19 09:59:27.000000 xuanpolicy-0.1.6/xuanpolicy/environment/vector_envs/vector_env.py
+drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2023-05-22 12:59:05.000000 xuanpolicy-0.1.6/xuanpolicy/mindspore/
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)        0 2023-05-19 15:23:02.000000 xuanpolicy-0.1.6/xuanpolicy/mindspore/__init__.py
+drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2023-05-22 12:59:05.000000 xuanpolicy-0.1.6/xuanpolicy/mindspore/agents/
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     4216 2023-05-22 02:23:07.000000 xuanpolicy-0.1.6/xuanpolicy/mindspore/agents/__init__.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1236 2023-05-22 02:23:07.000000 xuanpolicy-0.1.6/xuanpolicy/mindspore/agents/agent.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     3666 2023-05-22 02:23:07.000000 xuanpolicy-0.1.6/xuanpolicy/mindspore/agents/agents_marl.py
+drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2023-05-22 12:59:05.000000 xuanpolicy-0.1.6/xuanpolicy/mindspore/agents/multi_agent_rl/
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)        0 2023-05-20 05:14:19.000000 xuanpolicy-0.1.6/xuanpolicy/mindspore/agents/multi_agent_rl/__init__.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     5590 2023-05-22 02:23:06.000000 xuanpolicy-0.1.6/xuanpolicy/mindspore/agents/multi_agent_rl/coma_agents.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     5198 2023-05-22 02:23:07.000000 xuanpolicy-0.1.6/xuanpolicy/mindspore/agents/multi_agent_rl/dcg_agents.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     4623 2023-05-22 09:46:56.000000 xuanpolicy-0.1.6/xuanpolicy/mindspore/agents/multi_agent_rl/iddpg_agents.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     4076 2023-05-22 02:23:07.000000 xuanpolicy-0.1.6/xuanpolicy/mindspore/agents/multi_agent_rl/iql_agents.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     4595 2023-05-22 09:46:56.000000 xuanpolicy-0.1.6/xuanpolicy/mindspore/agents/multi_agent_rl/isac_agents.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     4627 2023-05-22 09:46:56.000000 xuanpolicy-0.1.6/xuanpolicy/mindspore/agents/multi_agent_rl/maddpg_agents.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     4994 2023-05-22 02:23:07.000000 xuanpolicy-0.1.6/xuanpolicy/mindspore/agents/multi_agent_rl/mappoclip_agents.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     5123 2023-05-22 02:23:06.000000 xuanpolicy-0.1.6/xuanpolicy/mindspore/agents/multi_agent_rl/mappokl_agents.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     4599 2023-05-22 09:46:56.000000 xuanpolicy-0.1.6/xuanpolicy/mindspore/agents/multi_agent_rl/masac_agents.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     4926 2023-05-22 09:46:56.000000 xuanpolicy-0.1.6/xuanpolicy/mindspore/agents/multi_agent_rl/matd3_agents.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     5703 2023-05-22 02:23:07.000000 xuanpolicy-0.1.6/xuanpolicy/mindspore/agents/multi_agent_rl/mfac_agents.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     5859 2023-05-22 02:23:07.000000 xuanpolicy-0.1.6/xuanpolicy/mindspore/agents/multi_agent_rl/mfq_agents.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     4237 2023-05-22 02:23:08.000000 xuanpolicy-0.1.6/xuanpolicy/mindspore/agents/multi_agent_rl/qmix_agents.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     4714 2023-05-22 02:23:06.000000 xuanpolicy-0.1.6/xuanpolicy/mindspore/agents/multi_agent_rl/qtran_agents.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     5332 2023-05-22 02:23:06.000000 xuanpolicy-0.1.6/xuanpolicy/mindspore/agents/multi_agent_rl/vdac_agents.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     4110 2023-05-22 02:23:06.000000 xuanpolicy-0.1.6/xuanpolicy/mindspore/agents/multi_agent_rl/vdn_agents.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     4429 2023-05-22 02:23:07.000000 xuanpolicy-0.1.6/xuanpolicy/mindspore/agents/multi_agent_rl/wqmix_agents.py
+drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2023-05-22 12:59:05.000000 xuanpolicy-0.1.6/xuanpolicy/mindspore/agents/policy_gradient/
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)        0 2023-05-20 05:14:30.000000 xuanpolicy-0.1.6/xuanpolicy/mindspore/agents/policy_gradient/__init__.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     6372 2023-05-22 02:23:07.000000 xuanpolicy-0.1.6/xuanpolicy/mindspore/agents/policy_gradient/a2c_agent.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     6312 2023-05-22 02:23:06.000000 xuanpolicy-0.1.6/xuanpolicy/mindspore/agents/policy_gradient/ddpg_agent.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     8967 2023-05-22 02:23:08.000000 xuanpolicy-0.1.6/xuanpolicy/mindspore/agents/policy_gradient/mpdqn_agent.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     8206 2023-05-22 02:23:06.000000 xuanpolicy-0.1.6/xuanpolicy/mindspore/agents/policy_gradient/pdqn_agent.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     6128 2023-05-22 02:23:07.000000 xuanpolicy-0.1.6/xuanpolicy/mindspore/agents/policy_gradient/pg_agent.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     7934 2023-05-22 02:23:06.000000 xuanpolicy-0.1.6/xuanpolicy/mindspore/agents/policy_gradient/ppg_agent.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     6587 2023-05-22 02:23:07.000000 xuanpolicy-0.1.6/xuanpolicy/mindspore/agents/policy_gradient/ppoclip_agent.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     6567 2023-05-22 02:23:07.000000 xuanpolicy-0.1.6/xuanpolicy/mindspore/agents/policy_gradient/ppokl_agent.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     6172 2023-05-22 02:23:06.000000 xuanpolicy-0.1.6/xuanpolicy/mindspore/agents/policy_gradient/sac_agent.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     6283 2023-05-22 02:23:07.000000 xuanpolicy-0.1.6/xuanpolicy/mindspore/agents/policy_gradient/sacdis_agent.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     9260 2023-05-22 02:23:07.000000 xuanpolicy-0.1.6/xuanpolicy/mindspore/agents/policy_gradient/spdqn_agent.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     6364 2023-05-22 02:23:07.000000 xuanpolicy-0.1.6/xuanpolicy/mindspore/agents/policy_gradient/td3_agent.py
+drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2023-05-22 12:59:05.000000 xuanpolicy-0.1.6/xuanpolicy/mindspore/agents/qlearning_family/
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     6288 2023-05-22 02:23:07.000000 xuanpolicy-0.1.6/xuanpolicy/mindspore/agents/qlearning_family/C51_agent.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)        0 2023-05-20 05:14:40.000000 xuanpolicy-0.1.6/xuanpolicy/mindspore/agents/qlearning_family/__init__.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     6290 2023-05-22 02:23:06.000000 xuanpolicy-0.1.6/xuanpolicy/mindspore/agents/qlearning_family/cdqn_agent.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     6292 2023-05-22 02:23:06.000000 xuanpolicy-0.1.6/xuanpolicy/mindspore/agents/qlearning_family/cldqn_agent.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     6299 2023-05-22 02:23:06.000000 xuanpolicy-0.1.6/xuanpolicy/mindspore/agents/qlearning_family/ddqn_agent.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     6288 2023-05-22 02:23:07.000000 xuanpolicy-0.1.6/xuanpolicy/mindspore/agents/qlearning_family/dqn_agent.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     6382 2023-05-22 02:23:07.000000 xuanpolicy-0.1.6/xuanpolicy/mindspore/agents/qlearning_family/dueldqn_agent.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     6290 2023-05-22 02:23:06.000000 xuanpolicy-0.1.6/xuanpolicy/mindspore/agents/qlearning_family/ldqn_agent.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     6277 2023-05-22 02:23:07.000000 xuanpolicy-0.1.6/xuanpolicy/mindspore/agents/qlearning_family/noisydqn_agent.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     6599 2023-05-22 02:23:07.000000 xuanpolicy-0.1.6/xuanpolicy/mindspore/agents/qlearning_family/perdqn_agent.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     6294 2023-05-22 02:23:07.000000 xuanpolicy-0.1.6/xuanpolicy/mindspore/agents/qlearning_family/qrdqn_agent.py
+drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2023-05-22 12:59:05.000000 xuanpolicy-0.1.6/xuanpolicy/mindspore/learners/
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     2513 2023-05-22 02:23:07.000000 xuanpolicy-0.1.6/xuanpolicy/mindspore/learners/__init__.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     3496 2023-05-19 09:59:25.000000 xuanpolicy-0.1.6/xuanpolicy/mindspore/learners/learner.py
+drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2023-05-22 12:59:05.000000 xuanpolicy-0.1.6/xuanpolicy/mindspore/learners/multi_agent_rl/
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)        0 2023-05-20 05:14:54.000000 xuanpolicy-0.1.6/xuanpolicy/mindspore/learners/multi_agent_rl/__init__.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     7055 2023-05-22 02:23:06.000000 xuanpolicy-0.1.6/xuanpolicy/mindspore/learners/multi_agent_rl/coma_learner.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     8726 2023-05-22 02:23:07.000000 xuanpolicy-0.1.6/xuanpolicy/mindspore/learners/multi_agent_rl/dcg_learner.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     3998 2023-05-22 02:23:07.000000 xuanpolicy-0.1.6/xuanpolicy/mindspore/learners/multi_agent_rl/iddpg_learner.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     3076 2023-05-22 02:23:07.000000 xuanpolicy-0.1.6/xuanpolicy/mindspore/learners/multi_agent_rl/iql_learner.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     4873 2023-05-22 02:23:07.000000 xuanpolicy-0.1.6/xuanpolicy/mindspore/learners/multi_agent_rl/isac_learner.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     4628 2023-05-22 02:23:06.000000 xuanpolicy-0.1.6/xuanpolicy/mindspore/learners/multi_agent_rl/maddpg_learner.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     4677 2023-05-22 02:23:06.000000 xuanpolicy-0.1.6/xuanpolicy/mindspore/learners/multi_agent_rl/mappoclip_learner.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     5216 2023-05-22 02:23:07.000000 xuanpolicy-0.1.6/xuanpolicy/mindspore/learners/multi_agent_rl/mappokl_learner.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     4877 2023-05-22 02:23:06.000000 xuanpolicy-0.1.6/xuanpolicy/mindspore/learners/multi_agent_rl/masac_learner.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     5663 2023-05-22 02:23:08.000000 xuanpolicy-0.1.6/xuanpolicy/mindspore/learners/multi_agent_rl/matd3_learner.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     6177 2023-05-22 02:23:06.000000 xuanpolicy-0.1.6/xuanpolicy/mindspore/learners/multi_agent_rl/mfac_learner.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     3611 2023-05-22 02:23:07.000000 xuanpolicy-0.1.6/xuanpolicy/mindspore/learners/multi_agent_rl/mfq_learner.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     3482 2023-05-22 02:23:07.000000 xuanpolicy-0.1.6/xuanpolicy/mindspore/learners/multi_agent_rl/qmix_learner.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     6445 2023-05-22 02:23:07.000000 xuanpolicy-0.1.6/xuanpolicy/mindspore/learners/multi_agent_rl/qtran_learner.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     2922 2023-05-22 02:23:07.000000 xuanpolicy-0.1.6/xuanpolicy/mindspore/learners/multi_agent_rl/vdac_learner.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     3372 2023-05-22 02:23:06.000000 xuanpolicy-0.1.6/xuanpolicy/mindspore/learners/multi_agent_rl/vdn_learner.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     5030 2023-05-22 02:23:08.000000 xuanpolicy-0.1.6/xuanpolicy/mindspore/learners/multi_agent_rl/wqmix_learner.py
+drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2023-05-22 12:59:05.000000 xuanpolicy-0.1.6/xuanpolicy/mindspore/learners/policy_gradient/
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)        0 2023-05-20 05:14:54.000000 xuanpolicy-0.1.6/xuanpolicy/mindspore/learners/policy_gradient/__init__.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     2853 2023-05-22 02:23:08.000000 xuanpolicy-0.1.6/xuanpolicy/mindspore/learners/policy_gradient/a2c_learner.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     2964 2023-05-22 02:23:07.000000 xuanpolicy-0.1.6/xuanpolicy/mindspore/learners/policy_gradient/ddpg_learner.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     4737 2023-05-22 02:23:06.000000 xuanpolicy-0.1.6/xuanpolicy/mindspore/learners/policy_gradient/mpdqn_learner.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     3406 2023-05-22 02:23:07.000000 xuanpolicy-0.1.6/xuanpolicy/mindspore/learners/policy_gradient/pdqn_learner.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     2397 2023-05-22 02:23:06.000000 xuanpolicy-0.1.6/xuanpolicy/mindspore/learners/policy_gradient/pg_learner.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     4595 2023-05-22 02:23:08.000000 xuanpolicy-0.1.6/xuanpolicy/mindspore/learners/policy_gradient/ppg_learner.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     3312 2023-05-22 02:23:07.000000 xuanpolicy-0.1.6/xuanpolicy/mindspore/learners/policy_gradient/ppoclip_learner.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     2800 2023-05-22 02:23:07.000000 xuanpolicy-0.1.6/xuanpolicy/mindspore/learners/policy_gradient/ppokl_learner.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     2899 2023-05-22 02:23:07.000000 xuanpolicy-0.1.6/xuanpolicy/mindspore/learners/policy_gradient/sac_learner.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     3351 2023-05-22 02:23:06.000000 xuanpolicy-0.1.6/xuanpolicy/mindspore/learners/policy_gradient/sacdis_learner.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     4749 2023-05-22 02:23:07.000000 xuanpolicy-0.1.6/xuanpolicy/mindspore/learners/policy_gradient/spdqn_learner.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     3340 2023-05-22 02:23:07.000000 xuanpolicy-0.1.6/xuanpolicy/mindspore/learners/policy_gradient/td3_learner.py
+drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2023-05-22 12:59:05.000000 xuanpolicy-0.1.6/xuanpolicy/mindspore/learners/qlearning_family/
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)        0 2023-05-20 05:14:54.000000 xuanpolicy-0.1.6/xuanpolicy/mindspore/learners/qlearning_family/__init__.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     3712 2023-05-22 02:23:07.000000 xuanpolicy-0.1.6/xuanpolicy/mindspore/learners/qlearning_family/c51_learner.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     2476 2023-05-22 02:23:07.000000 xuanpolicy-0.1.6/xuanpolicy/mindspore/learners/qlearning_family/cdqn_learner.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     2479 2023-05-22 02:23:07.000000 xuanpolicy-0.1.6/xuanpolicy/mindspore/learners/qlearning_family/cldqn_learner.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     2486 2023-05-22 02:23:07.000000 xuanpolicy-0.1.6/xuanpolicy/mindspore/learners/qlearning_family/ddqn_learner.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     2473 2023-05-22 02:23:07.000000 xuanpolicy-0.1.6/xuanpolicy/mindspore/learners/qlearning_family/dqn_learner.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     2352 2023-05-22 02:23:06.000000 xuanpolicy-0.1.6/xuanpolicy/mindspore/learners/qlearning_family/dueldqn_learner.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     2476 2023-05-22 02:23:07.000000 xuanpolicy-0.1.6/xuanpolicy/mindspore/learners/qlearning_family/ldqn_learner.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     2748 2023-05-22 02:23:06.000000 xuanpolicy-0.1.6/xuanpolicy/mindspore/learners/qlearning_family/perdqn_learner.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     3100 2023-05-22 02:23:08.000000 xuanpolicy-0.1.6/xuanpolicy/mindspore/learners/qlearning_family/qrdqn_learner.py
+drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2023-05-22 12:59:05.000000 xuanpolicy-0.1.6/xuanpolicy/mindspore/policies/
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     9030 2023-05-19 09:59:25.000000 xuanpolicy-0.1.6/xuanpolicy/mindspore/policies/__init__.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)    13620 2023-05-22 02:23:07.000000 xuanpolicy-0.1.6/xuanpolicy/mindspore/policies/categorical.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)    13930 2023-05-22 02:23:07.000000 xuanpolicy-0.1.6/xuanpolicy/mindspore/policies/categorical_marl.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)    37561 2023-05-22 02:23:06.000000 xuanpolicy-0.1.6/xuanpolicy/mindspore/policies/deterministic.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)    24961 2023-05-22 02:23:06.000000 xuanpolicy-0.1.6/xuanpolicy/mindspore/policies/deterministic_marl.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)    10525 2023-05-22 02:23:07.000000 xuanpolicy-0.1.6/xuanpolicy/mindspore/policies/gaussian.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)    13846 2023-05-22 02:23:06.000000 xuanpolicy-0.1.6/xuanpolicy/mindspore/policies/gaussian_marl.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)    11317 2023-05-19 09:59:25.000000 xuanpolicy-0.1.6/xuanpolicy/mindspore/policies/mixers.py
+drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2023-05-22 12:59:05.000000 xuanpolicy-0.1.6/xuanpolicy/mindspore/representations/
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1428 2023-05-19 09:59:24.000000 xuanpolicy-0.1.6/xuanpolicy/mindspore/representations/__init__.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)    13449 2023-05-22 02:23:06.000000 xuanpolicy-0.1.6/xuanpolicy/mindspore/representations/networks.py
+drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2023-05-22 12:59:05.000000 xuanpolicy-0.1.6/xuanpolicy/mindspore/runners/
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      190 2023-05-19 09:59:25.000000 xuanpolicy-0.1.6/xuanpolicy/mindspore/runners/__init__.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     4316 2023-05-22 12:08:13.000000 xuanpolicy-0.1.6/xuanpolicy/mindspore/runners/runner_basic.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     4894 2023-05-22 02:32:45.000000 xuanpolicy-0.1.6/xuanpolicy/mindspore/runners/runner_drl.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     6677 2023-05-22 08:07:51.000000 xuanpolicy-0.1.6/xuanpolicy/mindspore/runners/runner_marl.py
+drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2023-05-22 12:59:05.000000 xuanpolicy-0.1.6/xuanpolicy/mindspore/utils/
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)       47 2023-05-19 09:59:25.000000 xuanpolicy-0.1.6/xuanpolicy/mindspore/utils/__init__.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1726 2023-05-19 09:59:25.000000 xuanpolicy-0.1.6/xuanpolicy/mindspore/utils/distributions.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     4283 2023-05-22 02:23:08.000000 xuanpolicy-0.1.6/xuanpolicy/mindspore/utils/input_reformat.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     3583 2023-05-19 09:59:25.000000 xuanpolicy-0.1.6/xuanpolicy/mindspore/utils/layers.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     2029 2023-05-19 09:59:25.000000 xuanpolicy-0.1.6/xuanpolicy/mindspore/utils/operations.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1536 2023-05-19 09:59:25.000000 xuanpolicy-0.1.6/xuanpolicy/mindspore/utils/set_trainer.py
+drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2023-05-22 12:59:05.000000 xuanpolicy-0.1.6/xuanpolicy/tensorflow/
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)        0 2023-05-19 15:23:26.000000 xuanpolicy-0.1.6/xuanpolicy/tensorflow/__init__.py
+drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2023-05-22 12:59:05.000000 xuanpolicy-0.1.6/xuanpolicy/tensorflow/agents/
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     4350 2023-05-22 02:23:34.000000 xuanpolicy-0.1.6/xuanpolicy/tensorflow/agents/__init__.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1615 2023-05-22 02:23:34.000000 xuanpolicy-0.1.6/xuanpolicy/tensorflow/agents/agent.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     3694 2023-05-22 02:23:34.000000 xuanpolicy-0.1.6/xuanpolicy/tensorflow/agents/agents_marl.py
+drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2023-05-22 12:59:05.000000 xuanpolicy-0.1.6/xuanpolicy/tensorflow/agents/multi_agent_rl/
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)        0 2023-05-20 05:14:54.000000 xuanpolicy-0.1.6/xuanpolicy/tensorflow/agents/multi_agent_rl/__init__.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     5722 2023-05-22 02:23:34.000000 xuanpolicy-0.1.6/xuanpolicy/tensorflow/agents/multi_agent_rl/coma_agents.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     5557 2023-05-22 02:23:34.000000 xuanpolicy-0.1.6/xuanpolicy/tensorflow/agents/multi_agent_rl/dcg_agents.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     4624 2023-05-22 09:46:56.000000 xuanpolicy-0.1.6/xuanpolicy/tensorflow/agents/multi_agent_rl/iddpg_agents.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     4339 2023-05-22 02:23:34.000000 xuanpolicy-0.1.6/xuanpolicy/tensorflow/agents/multi_agent_rl/iql_agents.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     4629 2023-05-22 09:46:56.000000 xuanpolicy-0.1.6/xuanpolicy/tensorflow/agents/multi_agent_rl/isac_agents.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     4731 2023-05-22 09:46:56.000000 xuanpolicy-0.1.6/xuanpolicy/tensorflow/agents/multi_agent_rl/maddpg_agents.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     5044 2023-05-22 02:23:34.000000 xuanpolicy-0.1.6/xuanpolicy/tensorflow/agents/multi_agent_rl/mappoclip_agents.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     5000 2023-05-22 02:23:34.000000 xuanpolicy-0.1.6/xuanpolicy/tensorflow/agents/multi_agent_rl/mappokl_agents.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     4633 2023-05-22 09:46:56.000000 xuanpolicy-0.1.6/xuanpolicy/tensorflow/agents/multi_agent_rl/masac_agents.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     4728 2023-05-22 09:46:56.000000 xuanpolicy-0.1.6/xuanpolicy/tensorflow/agents/multi_agent_rl/matd3_agents.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     5417 2023-05-22 02:23:34.000000 xuanpolicy-0.1.6/xuanpolicy/tensorflow/agents/multi_agent_rl/mfac_agents.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     5774 2023-05-22 02:23:34.000000 xuanpolicy-0.1.6/xuanpolicy/tensorflow/agents/multi_agent_rl/mfq_agents.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     4533 2023-05-22 02:23:34.000000 xuanpolicy-0.1.6/xuanpolicy/tensorflow/agents/multi_agent_rl/qmix_agents.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     4969 2023-05-22 02:23:34.000000 xuanpolicy-0.1.6/xuanpolicy/tensorflow/agents/multi_agent_rl/qtran_agents.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     5417 2023-05-22 02:23:34.000000 xuanpolicy-0.1.6/xuanpolicy/tensorflow/agents/multi_agent_rl/vdac_agents.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     4404 2023-05-22 02:23:34.000000 xuanpolicy-0.1.6/xuanpolicy/tensorflow/agents/multi_agent_rl/vdn_agents.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     4684 2023-05-22 02:23:34.000000 xuanpolicy-0.1.6/xuanpolicy/tensorflow/agents/multi_agent_rl/wqmix_agents.py
+drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2023-05-22 12:59:05.000000 xuanpolicy-0.1.6/xuanpolicy/tensorflow/agents/policy_gradient/
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)        0 2023-05-20 05:14:54.000000 xuanpolicy-0.1.6/xuanpolicy/tensorflow/agents/policy_gradient/__init__.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     6192 2023-05-22 02:23:34.000000 xuanpolicy-0.1.6/xuanpolicy/tensorflow/agents/policy_gradient/a2c_agent.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     6160 2023-05-22 02:23:34.000000 xuanpolicy-0.1.6/xuanpolicy/tensorflow/agents/policy_gradient/ddpg_agent.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     8623 2023-05-22 02:23:34.000000 xuanpolicy-0.1.6/xuanpolicy/tensorflow/agents/policy_gradient/mpdqn_agent.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     8567 2023-05-22 02:23:34.000000 xuanpolicy-0.1.6/xuanpolicy/tensorflow/agents/policy_gradient/pdqn_agent.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     5984 2023-05-22 02:23:34.000000 xuanpolicy-0.1.6/xuanpolicy/tensorflow/agents/policy_gradient/pg_agent.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     7647 2023-05-22 02:23:34.000000 xuanpolicy-0.1.6/xuanpolicy/tensorflow/agents/policy_gradient/ppg_agent.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     6437 2023-05-22 02:23:34.000000 xuanpolicy-0.1.6/xuanpolicy/tensorflow/agents/policy_gradient/ppoclip_agent.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     6369 2023-05-22 02:23:34.000000 xuanpolicy-0.1.6/xuanpolicy/tensorflow/agents/policy_gradient/ppokl_agent.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     6138 2023-05-22 02:23:34.000000 xuanpolicy-0.1.6/xuanpolicy/tensorflow/agents/policy_gradient/sac_agent.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     6286 2023-05-22 02:23:34.000000 xuanpolicy-0.1.6/xuanpolicy/tensorflow/agents/policy_gradient/sacdis_agent.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     8854 2023-05-22 02:23:34.000000 xuanpolicy-0.1.6/xuanpolicy/tensorflow/agents/policy_gradient/spdqn_agent.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     6389 2023-05-22 02:23:34.000000 xuanpolicy-0.1.6/xuanpolicy/tensorflow/agents/policy_gradient/td3_agent.py
+drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2023-05-22 12:59:05.000000 xuanpolicy-0.1.6/xuanpolicy/tensorflow/agents/qlearning_family/
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)        0 2023-05-20 05:14:54.000000 xuanpolicy-0.1.6/xuanpolicy/tensorflow/agents/qlearning_family/__init__.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     6248 2023-05-22 02:23:34.000000 xuanpolicy-0.1.6/xuanpolicy/tensorflow/agents/qlearning_family/c51_agent.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     6201 2023-05-22 02:23:34.000000 xuanpolicy-0.1.6/xuanpolicy/tensorflow/agents/qlearning_family/cdqn_agent.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     6174 2023-05-22 02:23:34.000000 xuanpolicy-0.1.6/xuanpolicy/tensorflow/agents/qlearning_family/cldqn_agent.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     6116 2023-05-22 02:23:34.000000 xuanpolicy-0.1.6/xuanpolicy/tensorflow/agents/qlearning_family/ddqn_agent.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     6237 2023-05-22 02:23:34.000000 xuanpolicy-0.1.6/xuanpolicy/tensorflow/agents/qlearning_family/dqn_agent.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     6157 2023-05-22 02:23:34.000000 xuanpolicy-0.1.6/xuanpolicy/tensorflow/agents/qlearning_family/dueldqn_agent.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     6201 2023-05-22 02:23:34.000000 xuanpolicy-0.1.6/xuanpolicy/tensorflow/agents/qlearning_family/ldqn_agent.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     6244 2023-05-22 02:23:34.000000 xuanpolicy-0.1.6/xuanpolicy/tensorflow/agents/qlearning_family/noisydqn_agent.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     6581 2023-05-22 02:23:34.000000 xuanpolicy-0.1.6/xuanpolicy/tensorflow/agents/qlearning_family/perdqn_agent.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     6217 2023-05-22 02:23:34.000000 xuanpolicy-0.1.6/xuanpolicy/tensorflow/agents/qlearning_family/qrdqn_agent.py
+drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2023-05-22 12:59:05.000000 xuanpolicy-0.1.6/xuanpolicy/tensorflow/learners/
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     3183 2023-05-19 09:59:26.000000 xuanpolicy-0.1.6/xuanpolicy/tensorflow/learners/__init__.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     2974 2023-05-22 02:23:34.000000 xuanpolicy-0.1.6/xuanpolicy/tensorflow/learners/learner.py
+drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2023-05-22 12:59:05.000000 xuanpolicy-0.1.6/xuanpolicy/tensorflow/learners/multi_agent_rl/
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)        0 2023-05-20 05:14:54.000000 xuanpolicy-0.1.6/xuanpolicy/tensorflow/learners/multi_agent_rl/__init__.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     7548 2023-05-22 02:23:34.000000 xuanpolicy-0.1.6/xuanpolicy/tensorflow/learners/multi_agent_rl/coma_learner.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)    10668 2023-05-22 02:23:34.000000 xuanpolicy-0.1.6/xuanpolicy/tensorflow/learners/multi_agent_rl/dcg_learner.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     4591 2023-05-22 02:23:34.000000 xuanpolicy-0.1.6/xuanpolicy/tensorflow/learners/multi_agent_rl/iddpg_learner.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     3601 2023-05-22 02:23:34.000000 xuanpolicy-0.1.6/xuanpolicy/tensorflow/learners/multi_agent_rl/iql_learner.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     4921 2023-05-22 02:23:34.000000 xuanpolicy-0.1.6/xuanpolicy/tensorflow/learners/multi_agent_rl/isac_learner.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     3851 2023-05-22 02:23:07.000000 xuanpolicy-0.1.6/xuanpolicy/tensorflow/learners/multi_agent_rl/maac_learner.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     4721 2023-05-22 02:23:34.000000 xuanpolicy-0.1.6/xuanpolicy/tensorflow/learners/multi_agent_rl/maddpg_learner.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     2631 2023-05-22 02:23:07.000000 xuanpolicy-0.1.6/xuanpolicy/tensorflow/learners/multi_agent_rl/madqn_learner.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     4671 2023-05-22 02:23:34.000000 xuanpolicy-0.1.6/xuanpolicy/tensorflow/learners/multi_agent_rl/mappoclip_learner.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     5057 2023-05-22 02:23:34.000000 xuanpolicy-0.1.6/xuanpolicy/tensorflow/learners/multi_agent_rl/mappokl_learner.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     4924 2023-05-22 02:23:34.000000 xuanpolicy-0.1.6/xuanpolicy/tensorflow/learners/multi_agent_rl/masac_learner.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     4800 2023-05-22 02:23:34.000000 xuanpolicy-0.1.6/xuanpolicy/tensorflow/learners/multi_agent_rl/matd3_learner.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     5844 2023-05-22 02:23:34.000000 xuanpolicy-0.1.6/xuanpolicy/tensorflow/learners/multi_agent_rl/mfac_learner.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     4527 2023-05-22 02:23:34.000000 xuanpolicy-0.1.6/xuanpolicy/tensorflow/learners/multi_agent_rl/mfq_learner.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     4041 2023-05-22 02:23:34.000000 xuanpolicy-0.1.6/xuanpolicy/tensorflow/learners/multi_agent_rl/qmix_learner.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     6816 2023-05-22 02:23:34.000000 xuanpolicy-0.1.6/xuanpolicy/tensorflow/learners/multi_agent_rl/qtran_learner.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     3735 2023-05-22 02:23:34.000000 xuanpolicy-0.1.6/xuanpolicy/tensorflow/learners/multi_agent_rl/vdac_learner.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     3771 2023-05-22 02:23:34.000000 xuanpolicy-0.1.6/xuanpolicy/tensorflow/learners/multi_agent_rl/vdn_learner.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     5692 2023-05-22 02:23:34.000000 xuanpolicy-0.1.6/xuanpolicy/tensorflow/learners/multi_agent_rl/wqmix_learner.py
+drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2023-05-22 12:59:05.000000 xuanpolicy-0.1.6/xuanpolicy/tensorflow/learners/policy_gradient/
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)        0 2023-05-20 05:14:54.000000 xuanpolicy-0.1.6/xuanpolicy/tensorflow/learners/policy_gradient/__init__.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     2281 2023-05-22 02:23:34.000000 xuanpolicy-0.1.6/xuanpolicy/tensorflow/learners/policy_gradient/a2c_learner.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     3323 2023-05-22 02:23:34.000000 xuanpolicy-0.1.6/xuanpolicy/tensorflow/learners/policy_gradient/ddpg_learner.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     3881 2023-05-22 02:23:34.000000 xuanpolicy-0.1.6/xuanpolicy/tensorflow/learners/policy_gradient/mpdqn_learner.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     3965 2023-05-22 02:23:34.000000 xuanpolicy-0.1.6/xuanpolicy/tensorflow/learners/policy_gradient/pdqn_learner.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1843 2023-05-22 02:23:34.000000 xuanpolicy-0.1.6/xuanpolicy/tensorflow/learners/policy_gradient/pg_learner.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     6701 2023-05-22 02:23:34.000000 xuanpolicy-0.1.6/xuanpolicy/tensorflow/learners/policy_gradient/ppg_learner.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     2611 2023-05-22 02:23:34.000000 xuanpolicy-0.1.6/xuanpolicy/tensorflow/learners/policy_gradient/ppoclip_learner.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     3023 2023-05-22 02:23:34.000000 xuanpolicy-0.1.6/xuanpolicy/tensorflow/learners/policy_gradient/ppokl_learner.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     3558 2023-05-22 02:23:34.000000 xuanpolicy-0.1.6/xuanpolicy/tensorflow/learners/policy_gradient/sac_learner.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     3927 2023-05-22 02:23:34.000000 xuanpolicy-0.1.6/xuanpolicy/tensorflow/learners/policy_gradient/sacdis_learner.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     4107 2023-05-22 02:23:34.000000 xuanpolicy-0.1.6/xuanpolicy/tensorflow/learners/policy_gradient/spdqn_learner.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     3663 2023-05-22 02:23:34.000000 xuanpolicy-0.1.6/xuanpolicy/tensorflow/learners/policy_gradient/td3_learner.py
+drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2023-05-22 12:59:05.000000 xuanpolicy-0.1.6/xuanpolicy/tensorflow/learners/qlearning_family/
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)        0 2023-05-20 05:14:54.000000 xuanpolicy-0.1.6/xuanpolicy/tensorflow/learners/qlearning_family/__init__.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     2628 2023-05-22 02:23:34.000000 xuanpolicy-0.1.6/xuanpolicy/tensorflow/learners/qlearning_family/c51_learner.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     2183 2023-05-22 02:23:34.000000 xuanpolicy-0.1.6/xuanpolicy/tensorflow/learners/qlearning_family/cdqn_learner.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     2214 2023-05-22 02:23:34.000000 xuanpolicy-0.1.6/xuanpolicy/tensorflow/learners/qlearning_family/cldqn_learner.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     2283 2023-05-22 02:23:34.000000 xuanpolicy-0.1.6/xuanpolicy/tensorflow/learners/qlearning_family/ddqn_learner.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     2195 2023-05-22 02:23:34.000000 xuanpolicy-0.1.6/xuanpolicy/tensorflow/learners/qlearning_family/dqn_learner.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     2208 2023-05-22 02:23:34.000000 xuanpolicy-0.1.6/xuanpolicy/tensorflow/learners/qlearning_family/dueldqn_learner.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     2197 2023-05-22 02:23:34.000000 xuanpolicy-0.1.6/xuanpolicy/tensorflow/learners/qlearning_family/ldqn_learner.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     2302 2023-05-22 02:23:34.000000 xuanpolicy-0.1.6/xuanpolicy/tensorflow/learners/qlearning_family/perdqn_learner.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     2450 2023-05-22 02:23:34.000000 xuanpolicy-0.1.6/xuanpolicy/tensorflow/learners/qlearning_family/qrdqn_learner.py
+drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2023-05-22 12:59:05.000000 xuanpolicy-0.1.6/xuanpolicy/tensorflow/policies/
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)    10268 2023-05-19 09:59:26.000000 xuanpolicy-0.1.6/xuanpolicy/tensorflow/policies/__init__.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)    10665 2023-05-22 02:23:34.000000 xuanpolicy-0.1.6/xuanpolicy/tensorflow/policies/categorical.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)    14786 2023-05-22 02:23:34.000000 xuanpolicy-0.1.6/xuanpolicy/tensorflow/policies/categorical_marl.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)    38567 2023-05-22 02:23:34.000000 xuanpolicy-0.1.6/xuanpolicy/tensorflow/policies/deterministic.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)    41156 2023-05-22 02:23:34.000000 xuanpolicy-0.1.6/xuanpolicy/tensorflow/policies/deterministic_marl.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)    11513 2023-05-22 02:23:34.000000 xuanpolicy-0.1.6/xuanpolicy/tensorflow/policies/gaussian.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)    12369 2023-05-22 02:23:34.000000 xuanpolicy-0.1.6/xuanpolicy/tensorflow/policies/gaussian_marl.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)    12868 2023-05-19 09:59:26.000000 xuanpolicy-0.1.6/xuanpolicy/tensorflow/policies/mixers.py
+drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2023-05-22 12:59:05.000000 xuanpolicy-0.1.6/xuanpolicy/tensorflow/representations/
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1703 2023-05-22 02:23:34.000000 xuanpolicy-0.1.6/xuanpolicy/tensorflow/representations/__init__.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)    15035 2023-05-22 02:23:34.000000 xuanpolicy-0.1.6/xuanpolicy/tensorflow/representations/networks.py
+drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2023-05-22 12:59:05.000000 xuanpolicy-0.1.6/xuanpolicy/tensorflow/runners/
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      191 2023-05-19 09:59:26.000000 xuanpolicy-0.1.6/xuanpolicy/tensorflow/runners/__init__.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     4938 2023-05-22 12:08:13.000000 xuanpolicy-0.1.6/xuanpolicy/tensorflow/runners/runner_basic.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     4539 2023-05-22 02:32:45.000000 xuanpolicy-0.1.6/xuanpolicy/tensorflow/runners/runner_drl.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     6652 2023-05-22 08:07:51.000000 xuanpolicy-0.1.6/xuanpolicy/tensorflow/runners/runner_marl.py
+drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2023-05-22 12:59:05.000000 xuanpolicy-0.1.6/xuanpolicy/tensorflow/utils/
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)       76 2023-05-19 09:59:25.000000 xuanpolicy-0.1.6/xuanpolicy/tensorflow/utils/__init__.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     2717 2023-05-19 09:59:25.000000 xuanpolicy-0.1.6/xuanpolicy/tensorflow/utils/distributions.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     4355 2023-05-22 02:23:34.000000 xuanpolicy-0.1.6/xuanpolicy/tensorflow/utils/input_reformat.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     4512 2023-05-19 09:59:25.000000 xuanpolicy-0.1.6/xuanpolicy/tensorflow/utils/layers.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     2500 2023-05-19 09:59:25.000000 xuanpolicy-0.1.6/xuanpolicy/tensorflow/utils/operations.py
+drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2023-05-22 12:59:05.000000 xuanpolicy-0.1.6/xuanpolicy/torch/
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)        0 2023-05-19 15:23:28.000000 xuanpolicy-0.1.6/xuanpolicy/torch/__init__.py
+drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2023-05-22 12:59:05.000000 xuanpolicy-0.1.6/xuanpolicy/torch/agents/
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     4145 2023-05-22 02:23:07.000000 xuanpolicy-0.1.6/xuanpolicy/torch/agents/__init__.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1336 2023-05-22 02:23:07.000000 xuanpolicy-0.1.6/xuanpolicy/torch/agents/agent.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     3908 2023-05-22 12:50:47.000000 xuanpolicy-0.1.6/xuanpolicy/torch/agents/agents_marl.py
+drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2023-05-22 12:59:05.000000 xuanpolicy-0.1.6/xuanpolicy/torch/agents/multi_agent_rl/
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)        0 2023-05-20 05:14:54.000000 xuanpolicy-0.1.6/xuanpolicy/torch/agents/multi_agent_rl/__init__.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     5832 2023-05-22 02:23:07.000000 xuanpolicy-0.1.6/xuanpolicy/torch/agents/multi_agent_rl/coma_agents.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     5672 2023-05-22 02:23:06.000000 xuanpolicy-0.1.6/xuanpolicy/torch/agents/multi_agent_rl/dcg_agents.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     4806 2023-05-22 09:43:36.000000 xuanpolicy-0.1.6/xuanpolicy/torch/agents/multi_agent_rl/iddpg_agents.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     4281 2023-05-22 02:23:07.000000 xuanpolicy-0.1.6/xuanpolicy/torch/agents/multi_agent_rl/iql_agents.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     4725 2023-05-22 09:43:36.000000 xuanpolicy-0.1.6/xuanpolicy/torch/agents/multi_agent_rl/isac_agents.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     4811 2023-05-22 09:43:36.000000 xuanpolicy-0.1.6/xuanpolicy/torch/agents/multi_agent_rl/maddpg_agents.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     7223 2023-05-22 02:23:06.000000 xuanpolicy-0.1.6/xuanpolicy/torch/agents/multi_agent_rl/madqn_agents.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     4983 2023-05-22 02:23:07.000000 xuanpolicy-0.1.6/xuanpolicy/torch/agents/multi_agent_rl/mappoclip_agents.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     4928 2023-05-22 02:23:07.000000 xuanpolicy-0.1.6/xuanpolicy/torch/agents/multi_agent_rl/mappokl_agents.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     4728 2023-05-22 09:43:36.000000 xuanpolicy-0.1.6/xuanpolicy/torch/agents/multi_agent_rl/masac_agents.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     5127 2023-05-22 09:43:36.000000 xuanpolicy-0.1.6/xuanpolicy/torch/agents/multi_agent_rl/matd3_agents.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     5874 2023-05-22 02:23:06.000000 xuanpolicy-0.1.6/xuanpolicy/torch/agents/multi_agent_rl/mfac_agents.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     6051 2023-05-22 02:23:06.000000 xuanpolicy-0.1.6/xuanpolicy/torch/agents/multi_agent_rl/mfq_agents.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     4453 2023-05-22 02:23:06.000000 xuanpolicy-0.1.6/xuanpolicy/torch/agents/multi_agent_rl/qmix_agents.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     4903 2023-05-22 02:23:06.000000 xuanpolicy-0.1.6/xuanpolicy/torch/agents/multi_agent_rl/qtran_agents.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     5408 2023-05-22 02:23:07.000000 xuanpolicy-0.1.6/xuanpolicy/torch/agents/multi_agent_rl/vdac_agents.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     4316 2023-05-22 02:23:07.000000 xuanpolicy-0.1.6/xuanpolicy/torch/agents/multi_agent_rl/vdn_agents.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     4612 2023-05-22 02:23:08.000000 xuanpolicy-0.1.6/xuanpolicy/torch/agents/multi_agent_rl/wqmix_agents.py
+drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2023-05-22 12:59:05.000000 xuanpolicy-0.1.6/xuanpolicy/torch/agents/policy_gradient/
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)        0 2023-05-20 05:14:54.000000 xuanpolicy-0.1.6/xuanpolicy/torch/agents/policy_gradient/__init__.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     6325 2023-05-22 02:23:06.000000 xuanpolicy-0.1.6/xuanpolicy/torch/agents/policy_gradient/a2c_agent.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     6366 2023-05-22 02:23:08.000000 xuanpolicy-0.1.6/xuanpolicy/torch/agents/policy_gradient/ddpg_agent.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     8612 2023-05-22 02:23:06.000000 xuanpolicy-0.1.6/xuanpolicy/torch/agents/policy_gradient/mpdqn_agent.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     8601 2023-05-22 02:23:07.000000 xuanpolicy-0.1.6/xuanpolicy/torch/agents/policy_gradient/pdqn_agent.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     6125 2023-05-22 02:23:07.000000 xuanpolicy-0.1.6/xuanpolicy/torch/agents/policy_gradient/pg_agent.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     7553 2023-05-22 02:23:07.000000 xuanpolicy-0.1.6/xuanpolicy/torch/agents/policy_gradient/ppg_agent.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     6591 2023-05-22 02:23:07.000000 xuanpolicy-0.1.6/xuanpolicy/torch/agents/policy_gradient/ppoclip_agent.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     6506 2023-05-22 02:23:06.000000 xuanpolicy-0.1.6/xuanpolicy/torch/agents/policy_gradient/ppokl_agent.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     6350 2023-05-22 02:23:06.000000 xuanpolicy-0.1.6/xuanpolicy/torch/agents/policy_gradient/sac_agent.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     6494 2023-05-22 02:23:07.000000 xuanpolicy-0.1.6/xuanpolicy/torch/agents/policy_gradient/sacdis_agent.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     8583 2023-05-22 02:23:07.000000 xuanpolicy-0.1.6/xuanpolicy/torch/agents/policy_gradient/spdqn_agent.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     6559 2023-05-22 02:23:06.000000 xuanpolicy-0.1.6/xuanpolicy/torch/agents/policy_gradient/td3_agent.py
+drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2023-05-22 12:59:05.000000 xuanpolicy-0.1.6/xuanpolicy/torch/agents/qlearning_family/
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)        0 2023-05-20 05:14:54.000000 xuanpolicy-0.1.6/xuanpolicy/torch/agents/qlearning_family/__init__.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     6354 2023-05-22 02:23:07.000000 xuanpolicy-0.1.6/xuanpolicy/torch/agents/qlearning_family/c51_agent.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     6356 2023-05-22 02:23:06.000000 xuanpolicy-0.1.6/xuanpolicy/torch/agents/qlearning_family/cdqn_agent.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     6358 2023-05-22 02:23:06.000000 xuanpolicy-0.1.6/xuanpolicy/torch/agents/qlearning_family/cldqn_agent.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     6283 2023-05-22 02:23:07.000000 xuanpolicy-0.1.6/xuanpolicy/torch/agents/qlearning_family/ddqn_agent.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     6354 2023-05-22 02:23:07.000000 xuanpolicy-0.1.6/xuanpolicy/torch/agents/qlearning_family/dqn_agent.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     6356 2023-05-22 02:23:08.000000 xuanpolicy-0.1.6/xuanpolicy/torch/agents/qlearning_family/dueldqn_agent.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     6356 2023-05-22 02:23:07.000000 xuanpolicy-0.1.6/xuanpolicy/torch/agents/qlearning_family/ldqn_agent.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     6370 2023-05-22 02:23:08.000000 xuanpolicy-0.1.6/xuanpolicy/torch/agents/qlearning_family/noisydqn_agent.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     6696 2023-05-22 02:23:07.000000 xuanpolicy-0.1.6/xuanpolicy/torch/agents/qlearning_family/perdqn_agent.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     6374 2023-05-22 02:23:07.000000 xuanpolicy-0.1.6/xuanpolicy/torch/agents/qlearning_family/qrdqn_agent.py
+drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2023-05-22 12:59:05.000000 xuanpolicy-0.1.6/xuanpolicy/torch/learners/
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     2500 2023-05-21 08:10:27.000000 xuanpolicy-0.1.6/xuanpolicy/torch/learners/__init__.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     3490 2023-05-19 09:59:26.000000 xuanpolicy-0.1.6/xuanpolicy/torch/learners/learner.py
+drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2023-05-22 12:59:05.000000 xuanpolicy-0.1.6/xuanpolicy/torch/learners/multi_agent_rl/
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)        0 2023-05-20 05:14:54.000000 xuanpolicy-0.1.6/xuanpolicy/torch/learners/multi_agent_rl/__init__.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     6332 2023-05-22 02:23:07.000000 xuanpolicy-0.1.6/xuanpolicy/torch/learners/multi_agent_rl/coma_learner.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     6611 2023-05-22 02:23:07.000000 xuanpolicy-0.1.6/xuanpolicy/torch/learners/multi_agent_rl/dcg_learner.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     3616 2023-05-22 02:23:06.000000 xuanpolicy-0.1.6/xuanpolicy/torch/learners/multi_agent_rl/iddpg_learner.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     2871 2023-05-22 02:23:07.000000 xuanpolicy-0.1.6/xuanpolicy/torch/learners/multi_agent_rl/iql_learner.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     4132 2023-05-22 02:23:06.000000 xuanpolicy-0.1.6/xuanpolicy/torch/learners/multi_agent_rl/isac_learner.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     3848 2023-05-22 02:23:07.000000 xuanpolicy-0.1.6/xuanpolicy/torch/learners/multi_agent_rl/maddpg_learner.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     2663 2023-05-22 02:23:07.000000 xuanpolicy-0.1.6/xuanpolicy/torch/learners/multi_agent_rl/madqn_learner.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     3856 2023-05-22 02:23:07.000000 xuanpolicy-0.1.6/xuanpolicy/torch/learners/multi_agent_rl/mappoclip_learner.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     4185 2023-05-22 02:23:07.000000 xuanpolicy-0.1.6/xuanpolicy/torch/learners/multi_agent_rl/mappokl_learner.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     4135 2023-05-22 02:23:07.000000 xuanpolicy-0.1.6/xuanpolicy/torch/learners/multi_agent_rl/masac_learner.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     4174 2023-05-22 02:23:08.000000 xuanpolicy-0.1.6/xuanpolicy/torch/learners/multi_agent_rl/matd3_learner.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     4898 2023-05-22 02:23:06.000000 xuanpolicy-0.1.6/xuanpolicy/torch/learners/multi_agent_rl/mfac_learner.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     3391 2023-05-22 02:23:06.000000 xuanpolicy-0.1.6/xuanpolicy/torch/learners/multi_agent_rl/mfq_learner.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     3251 2023-05-22 02:23:07.000000 xuanpolicy-0.1.6/xuanpolicy/torch/learners/multi_agent_rl/qmix_learner.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     5761 2023-05-22 02:23:07.000000 xuanpolicy-0.1.6/xuanpolicy/torch/learners/multi_agent_rl/qtran_learner.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     2889 2023-05-22 02:23:08.000000 xuanpolicy-0.1.6/xuanpolicy/torch/learners/multi_agent_rl/vdac_learner.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     3022 2023-05-22 02:23:07.000000 xuanpolicy-0.1.6/xuanpolicy/torch/learners/multi_agent_rl/vdn_learner.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     4691 2023-05-22 02:23:07.000000 xuanpolicy-0.1.6/xuanpolicy/torch/learners/multi_agent_rl/wqmix_learner.py
+drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2023-05-22 12:59:05.000000 xuanpolicy-0.1.6/xuanpolicy/torch/learners/policy_gradient/
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)        0 2023-05-20 05:14:54.000000 xuanpolicy-0.1.6/xuanpolicy/torch/learners/policy_gradient/__init__.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     2102 2023-05-22 02:23:07.000000 xuanpolicy-0.1.6/xuanpolicy/torch/learners/policy_gradient/a2c_learner.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     2262 2023-05-22 02:23:07.000000 xuanpolicy-0.1.6/xuanpolicy/torch/learners/policy_gradient/ddpg_learner.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     2505 2023-05-22 02:23:07.000000 xuanpolicy-0.1.6/xuanpolicy/torch/learners/policy_gradient/mpdqn_learner.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)        0 2023-05-19 10:00:20.000000 xuanpolicy-0.1.6/xuanpolicy/torch/learners/policy_gradient/npg_learner.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     2517 2023-05-22 02:23:07.000000 xuanpolicy-0.1.6/xuanpolicy/torch/learners/policy_gradient/pdqn_learner.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1707 2023-05-22 02:23:06.000000 xuanpolicy-0.1.6/xuanpolicy/torch/learners/policy_gradient/pg_learner.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     3757 2023-05-22 02:23:07.000000 xuanpolicy-0.1.6/xuanpolicy/torch/learners/policy_gradient/ppg_learner.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     2517 2023-05-22 02:23:07.000000 xuanpolicy-0.1.6/xuanpolicy/torch/learners/policy_gradient/ppoclip_learner.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     2676 2023-05-22 02:23:07.000000 xuanpolicy-0.1.6/xuanpolicy/torch/learners/policy_gradient/ppokl_learner.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     2349 2023-05-22 02:23:07.000000 xuanpolicy-0.1.6/xuanpolicy/torch/learners/policy_gradient/sac_learner.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     2791 2023-05-22 02:23:07.000000 xuanpolicy-0.1.6/xuanpolicy/torch/learners/policy_gradient/sacdis_learner.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     2505 2023-05-22 02:23:07.000000 xuanpolicy-0.1.6/xuanpolicy/torch/learners/policy_gradient/spdqn_learner.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     2645 2023-05-22 02:23:06.000000 xuanpolicy-0.1.6/xuanpolicy/torch/learners/policy_gradient/td3_learner.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)        0 2023-05-19 10:00:19.000000 xuanpolicy-0.1.6/xuanpolicy/torch/learners/policy_gradient/trpo_learner.py
+drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2023-05-22 12:59:05.000000 xuanpolicy-0.1.6/xuanpolicy/torch/learners/qlearning_family/
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)        0 2023-05-20 05:14:54.000000 xuanpolicy-0.1.6/xuanpolicy/torch/learners/qlearning_family/__init__.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     2362 2023-05-22 02:23:07.000000 xuanpolicy-0.1.6/xuanpolicy/torch/learners/qlearning_family/c51_learner.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1954 2023-05-22 02:23:07.000000 xuanpolicy-0.1.6/xuanpolicy/torch/learners/qlearning_family/cdqn_learner.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1956 2023-05-22 02:23:07.000000 xuanpolicy-0.1.6/xuanpolicy/torch/learners/qlearning_family/cldqn_learner.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     2022 2023-05-22 02:23:07.000000 xuanpolicy-0.1.6/xuanpolicy/torch/learners/qlearning_family/ddqn_learner.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1952 2023-05-22 02:23:06.000000 xuanpolicy-0.1.6/xuanpolicy/torch/learners/qlearning_family/dqn_learner.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1960 2023-05-22 02:23:07.000000 xuanpolicy-0.1.6/xuanpolicy/torch/learners/qlearning_family/dueldqn_learner.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1954 2023-05-22 02:23:07.000000 xuanpolicy-0.1.6/xuanpolicy/torch/learners/qlearning_family/ldqn_learner.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     2060 2023-05-22 02:23:08.000000 xuanpolicy-0.1.6/xuanpolicy/torch/learners/qlearning_family/perdqn_learner.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     2019 2023-05-22 02:23:07.000000 xuanpolicy-0.1.6/xuanpolicy/torch/learners/qlearning_family/qrdqn_learner.py
+drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2023-05-22 12:59:05.000000 xuanpolicy-0.1.6/xuanpolicy/torch/learners/ssl_rl/
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)        0 2023-05-20 05:14:54.000000 xuanpolicy-0.1.6/xuanpolicy/torch/learners/ssl_rl/__init__.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)        0 2023-05-19 10:00:20.000000 xuanpolicy-0.1.6/xuanpolicy/torch/learners/ssl_rl/curl_learner.py
+drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2023-05-22 12:59:05.000000 xuanpolicy-0.1.6/xuanpolicy/torch/policies/
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     9885 2023-05-19 09:59:26.000000 xuanpolicy-0.1.6/xuanpolicy/torch/policies/__init__.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)    10984 2023-05-22 02:23:06.000000 xuanpolicy-0.1.6/xuanpolicy/torch/policies/categorical.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)    12528 2023-05-22 02:23:08.000000 xuanpolicy-0.1.6/xuanpolicy/torch/policies/categorical_marl.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     3963 2023-05-21 08:32:23.000000 xuanpolicy-0.1.6/xuanpolicy/torch/policies/coordination_graph.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)    35437 2023-05-22 02:23:08.000000 xuanpolicy-0.1.6/xuanpolicy/torch/policies/deterministic.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)    24455 2023-05-22 07:09:22.000000 xuanpolicy-0.1.6/xuanpolicy/torch/policies/deterministic_marl.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)    11088 2023-05-22 02:23:06.000000 xuanpolicy-0.1.6/xuanpolicy/torch/policies/gaussian.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)    10704 2023-05-22 10:40:39.000000 xuanpolicy-0.1.6/xuanpolicy/torch/policies/gaussian_marl.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     6643 2023-05-21 08:32:23.000000 xuanpolicy-0.1.6/xuanpolicy/torch/policies/mixers.py
+drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2023-05-22 12:59:05.000000 xuanpolicy-0.1.6/xuanpolicy/torch/representations/
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1781 2023-05-22 02:23:07.000000 xuanpolicy-0.1.6/xuanpolicy/torch/representations/__init__.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)    15004 2023-05-22 02:23:07.000000 xuanpolicy-0.1.6/xuanpolicy/torch/representations/networks.py
+drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2023-05-22 12:59:05.000000 xuanpolicy-0.1.6/xuanpolicy/torch/runners/
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      188 2023-05-19 09:59:26.000000 xuanpolicy-0.1.6/xuanpolicy/torch/runners/__init__.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     4317 2023-05-22 12:08:13.000000 xuanpolicy-0.1.6/xuanpolicy/torch/runners/runner_basic.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     4892 2023-05-22 02:31:54.000000 xuanpolicy-0.1.6/xuanpolicy/torch/runners/runner_drl.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     7197 2023-05-22 12:52:34.000000 xuanpolicy-0.1.6/xuanpolicy/torch/runners/runner_marl.py
+drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2023-05-22 12:59:05.000000 xuanpolicy-0.1.6/xuanpolicy/torch/utils/
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)       76 2023-05-19 09:59:26.000000 xuanpolicy-0.1.6/xuanpolicy/torch/utils/__init__.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     2700 2023-05-19 09:59:26.000000 xuanpolicy-0.1.6/xuanpolicy/torch/utils/distributions.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     4259 2023-05-22 02:23:08.000000 xuanpolicy-0.1.6/xuanpolicy/torch/utils/input_reformat.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     4024 2023-05-19 09:59:26.000000 xuanpolicy-0.1.6/xuanpolicy/torch/utils/layers.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     2441 2023-05-19 09:59:26.000000 xuanpolicy-0.1.6/xuanpolicy/torch/utils/operations.py
+drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2023-05-22 12:59:05.000000 xuanpolicy-0.1.6/xuanpolicy.egg-info/
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      864 2023-05-22 12:59:05.000000 xuanpolicy-0.1.6/xuanpolicy.egg-info/PKG-INFO
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)    22742 2023-05-22 12:59:05.000000 xuanpolicy-0.1.6/xuanpolicy.egg-info/SOURCES.txt
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)        1 2023-05-22 12:59:05.000000 xuanpolicy-0.1.6/xuanpolicy.egg-info/dependency_links.txt
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      295 2023-05-22 12:59:05.000000 xuanpolicy-0.1.6/xuanpolicy.egg-info/requires.txt
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)       11 2023-05-22 12:59:05.000000 xuanpolicy-0.1.6/xuanpolicy.egg-info/top_level.txt
```

### Comparing `xuanpolicy-0.1.5/LICENSE.txt` & `xuanpolicy-0.1.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `xuanpolicy-0.1.5/PKG-INFO` & `xuanpolicy-0.1.6/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xuanpolicy
-Version: 0.1.5
+Version: 0.1.6
 Summary: XuanPolicy: A Comprehensive Deep Reinforcement Learning Library.
 Home-page: 
 Download-URL: 
 Author: Wenzhang Liu, Wenzhe Cai, Kun Jiang, etc.
 Author-email: 
 License: MIT
 Keywords: deep reinforcement learning,software library,platform
```

### Comparing `xuanpolicy-0.1.5/README.md` & `xuanpolicy-0.1.6/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -91,15 +91,15 @@
 
 ## Basic Usage ##
 
 ### Quickly Start ###
 ```python
 import xuanpolicy as xp
 
-runner = xp.get_runner(agent_name='dqn', env_name='toy/CartPole-v0', is_test=False)
+runner = xp.get_runner(agent_name='dqn', env_name='toy_env/CartPole-v0', is_test=False)
 runner.run()
 ```
 
 [//]: # (### Run a Demo ###)
 
 [//]: # (The following four lines of code are enough to start training an RL agent.)
```

### Comparing `xuanpolicy-0.1.5/setup.py` & `xuanpolicy-0.1.6/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import find_packages, setup
 
 setup(
     name='xuanpolicy',
     packages=find_packages(include=['xuanpolicy', 'xuanpolicy.*']),
     package_data={"xuanpolicy": ["configs/*.yaml", "configs/*/*/*.yaml"]},
-    version='0.1.5',
+    version='0.1.6',
     description='XuanPolicy: A Comprehensive Deep Reinforcement Learning Library.',
     author='Wenzhang Liu, Wenzhe Cai, Kun Jiang, etc.',
     author_email='',
     license='MIT',
     url='',
     download_url='',
     keywords=['deep reinforcement learning', 'software library', 'platform'],
@@ -22,19 +22,19 @@
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
     ],
     extras_require={
         "torch": ["torch >= 1.13.0"],
-        "tensorflow": ["tensorflow >= 2.6.0"],
+        "tensorflow": ["tensorflow == 2.6.0"],
         "mindspore": ["mindspore >= 1.10.1"],
         "all": [
             "torch >= 1.13.0",
-            "tensorflow >= 2.6.0",
+            "tensorflow == 2.6.0",
             "mindspore >= 1.10.1"
         ]
     },
     install_requires=[
         "numpy >= 1.19.5",
         "scipy >= 1.7.3",
         "PyYAML >= 6.0",
```

### Comparing `xuanpolicy-0.1.5/xuanpolicy/common/common_tools.py` & `xuanpolicy-0.1.6/xuanpolicy/common/common_tools.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 import scipy.signal
 import yaml
 import itertools
 from gym.spaces import Space, Dict
 from typing import Sequence
 from types import SimpleNamespace as SN
 from copy import deepcopy
+EPS = 1e-8
 
 
 def recursive_dict_update(basic_dict, target_dict):
     out_dict = deepcopy(basic_dict)
     for key, value in target_dict.items():
         if isinstance(value, dict):
             out_dict[key] = recursive_dict_update(out_dict.get(key, {}), value)
@@ -84,56 +85,63 @@
     args = get_arguments(agent_name, env_name, config_path, parser_args)
 
     device = args[0].device if type(args) == list else args.device
     dl_toolbox = args[0].dl_toolbox if type(args) == list else args.dl_toolbox
     print("Calculating device:", device)
 
     if dl_toolbox == "torch":
-        from xuanpolicy.xuanpolicy_torch.runners import REGISTRY as run_REGISTRY
+        from xuanpolicy.torch.runners import REGISTRY as run_REGISTRY
         print("Deep learning toolbox: PyTorch.")
     elif dl_toolbox == "mindspore":
-        from xuanpolicy.xuanpolicy_ms.runners import REGISTRY as run_REGISTRY
+        from xuanpolicy.mindspore.runners import REGISTRY as run_REGISTRY
         from mindspore import context
         print("Deep learning toolbox: MindSpore.")
         if device != "Auto":
             if device in ["cpu", "CPU", "gpu", "GPU"]:
                 device = "CPU"
             context.set_context(device_target=device)
         # context.set_context(enable_graph_kernel=True)
         context.set_context(mode=context.GRAPH_MODE)  # 静态图（断点无法进入）
         # context.set_context(mode=context.PYNATIVE_MODE)  # 动态图（便于调试）
     elif dl_toolbox == "tensorflow":
-        from xuanpolicy.xuanpolicy_tf.runners import REGISTRY as run_REGISTRY
+        from xuanpolicy.tensorflow.runners import REGISTRY as run_REGISTRY
         print("Deep learning toolbox: TensorFlow.")
         if device in ["cpu", "CPU"]:
             os.environ["CUDA_VISIBLE_DEVICES"] = "-1"
     else:
         if dl_toolbox == '':
             raise AttributeError("You have to assign a deep learning toolbox")
         else:
             raise AttributeError("Cannot find a deep learning toolbox named " + dl_toolbox)
 
     if type(args) == list:
+        agents_name_string = []
         for i_alg in range(len(agent_name)):
+            if i_alg < len(agent_name) - 1:
+                agents_name_string.append(args[i_alg].agent + " vs")
+            else:
+                agents_name_string.append(args[i_alg].agent)
             args[i_alg].agent_name = agent_name[i_alg]
             notation = args[i_alg].dl_toolbox + '/'
             args[i_alg].modeldir = os.path.join(os.getcwd(), args[i_alg].modeldir + notation + args[i_alg].env_id + '/')
             args[i_alg].logdir = args[i_alg].logdir + notation + args[i_alg].env_id + '/'
-            if is_test is not None:
+            if is_test is True:
                 args[i_alg].test_mode = int(is_test)
                 args[i_alg].parallels = 1
-        print("Algorithm:", *[arg.agent for arg in args])
+
+        # print("Algorithm:", *[arg.agent for arg in args])
+        print("Algorithm:", *agents_name_string)
         print("Environment:", args[0].env_name)
         print("Scenario:", args[0].env_id)
     else:
         args.agent_name = agent_name
         notation = args.dl_toolbox + '/'
         args.modeldir = os.path.join(os.getcwd(), args.modeldir + notation + args.env_id + '/')
         args.logdir = args.logdir + notation + args.env_id + '/'
-        if is_test is not None:
+        if is_test is True:
             args.test_mode = int(is_test)
             args.parallels = 1
         print("Algorithm:", args.agent)
         print("Environment:", args.env_name)
         print("Scenario:", args.env_id)
 
     runner = run_REGISTRY[args[0].runner](args) if type(args) == list else run_REGISTRY[args.runner](args)
```

### Comparing `xuanpolicy-0.1.5/xuanpolicy/common/memory_tools.py` & `xuanpolicy-0.1.6/xuanpolicy/common/memory_tools.py`

 * *Files identical despite different names*

### Comparing `xuanpolicy-0.1.5/xuanpolicy/common/memory_tools_marl.py` & `xuanpolicy-0.1.6/xuanpolicy/common/memory_tools_marl.py`

 * *Files identical despite different names*

### Comparing `xuanpolicy-0.1.5/xuanpolicy/common/segtree_tool.py` & `xuanpolicy-0.1.6/xuanpolicy/common/segtree_tool.py`

 * *Files identical despite different names*

### Comparing `xuanpolicy-0.1.5/xuanpolicy/common/statistic_tools.py` & `xuanpolicy-0.1.6/xuanpolicy/common/statistic_tools.py`

 * *Files identical despite different names*

### Comparing `xuanpolicy-0.1.5/xuanpolicy/configs/a2c/mujoco/InvertedPendulum-v2.yaml` & `xuanpolicy-0.1.6/xuanpolicy/configs/a2c/mujoco/InvertedPendulum-v2.yaml`

 * *Files identical despite different names*

### Comparing `xuanpolicy-0.1.5/xuanpolicy/configs/a2c/toy/CartPole-v0.yaml` & `xuanpolicy-0.1.6/xuanpolicy/configs/a2c/toy/CartPole-v0.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 agent: "A2C"
-env_name: "toy"
+env_name: "toy_env"
 env_id: "CartPole-v0"
 policy: "Categorical_AC"
 representation: "Basic_MLP"
 
 representation_hidden_size: [256,]
 actor_hidden_size: [256,]
 critic_hidden_size: [256,]
```

### Comparing `xuanpolicy-0.1.5/xuanpolicy/configs/coma/mpe/simple_spread.yaml` & `xuanpolicy-0.1.6/xuanpolicy/configs/coma/mpe/simple_spread.yaml`

 * *Files identical despite different names*

### Comparing `xuanpolicy-0.1.5/xuanpolicy/configs/cwqmix/mpe/simple_spread.yaml` & `xuanpolicy-0.1.6/xuanpolicy/configs/cwqmix/mpe/simple_spread.yaml`

 * *Files identical despite different names*

### Comparing `xuanpolicy-0.1.5/xuanpolicy/configs/dcg/mpe/simple_spread.yaml` & `xuanpolicy-0.1.6/xuanpolicy/configs/dcg/mpe/simple_spread.yaml`

 * *Files identical despite different names*

### Comparing `xuanpolicy-0.1.5/xuanpolicy/configs/ddpg/mujoco/HalfCheetah-v3.yaml` & `xuanpolicy-0.1.6/xuanpolicy/configs/ddpg/mujoco/HalfCheetah-v3.yaml`

 * *Files identical despite different names*

### Comparing `xuanpolicy-0.1.5/xuanpolicy/configs/ddpg/toy/Pendulum-v1.yaml` & `xuanpolicy-0.1.6/xuanpolicy/configs/ddpg/toy/Pendulum-v1.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 agent: "DDPG"
-env_name: "toy"
+env_name: "toy_env"
 env_id: "Pendulum-v1"
 policy: "DDPG_Policy"
 representation: "Basic_MLP"
 
 representation_hidden_size: [128,]
 actor_hidden_size: [400,300]
 critic_hidden_size: [400,300]
```

### Comparing `xuanpolicy-0.1.5/xuanpolicy/configs/iddpg/mpe/simple_spread.yaml` & `xuanpolicy-0.1.6/xuanpolicy/configs/iddpg/mpe/simple_spread.yaml`

 * *Files identical despite different names*

### Comparing `xuanpolicy-0.1.5/xuanpolicy/configs/iql/mpe/simple_spread.yaml` & `xuanpolicy-0.1.6/xuanpolicy/configs/iql/mpe/simple_spread.yaml`

 * *Files identical despite different names*

### Comparing `xuanpolicy-0.1.5/xuanpolicy/configs/isac/mpe/simple_spread.yaml` & `xuanpolicy-0.1.6/xuanpolicy/configs/isac/mpe/simple_spread.yaml`

 * *Files identical despite different names*

### Comparing `xuanpolicy-0.1.5/xuanpolicy/configs/maddpg/mpe/simple_spread.yaml` & `xuanpolicy-0.1.6/xuanpolicy/configs/maddpg/mpe/simple_spread.yaml`

 * *Files identical despite different names*

### Comparing `xuanpolicy-0.1.5/xuanpolicy/configs/mappoclip/mpe/simple_spread.yaml` & `xuanpolicy-0.1.6/xuanpolicy/configs/mappoclip/mpe/simple_spread.yaml`

 * *Files identical despite different names*

### Comparing `xuanpolicy-0.1.5/xuanpolicy/configs/mappokl/mpe/simple_spread.yaml` & `xuanpolicy-0.1.6/xuanpolicy/configs/mappokl/mpe/simple_spread.yaml`

 * *Files identical despite different names*

### Comparing `xuanpolicy-0.1.5/xuanpolicy/configs/masac/mpe/simple_spread.yaml` & `xuanpolicy-0.1.6/xuanpolicy/configs/masac/mpe/simple_spread.yaml`

 * *Files identical despite different names*

### Comparing `xuanpolicy-0.1.5/xuanpolicy/configs/matd3/mpe/simple_spread.yaml` & `xuanpolicy-0.1.6/xuanpolicy/configs/matd3/mpe/simple_spread.yaml`

 * *Files identical despite different names*

### Comparing `xuanpolicy-0.1.5/xuanpolicy/configs/mfac/mpe/simple_spread.yaml` & `xuanpolicy-0.1.6/xuanpolicy/configs/mfac/mpe/simple_spread.yaml`

 * *Files identical despite different names*

### Comparing `xuanpolicy-0.1.5/xuanpolicy/configs/mfq/mpe/simple_spread.yaml` & `xuanpolicy-0.1.6/xuanpolicy/configs/mfq/mpe/simple_spread.yaml`

 * *Files identical despite different names*

### Comparing `xuanpolicy-0.1.5/xuanpolicy/configs/mpdqn/toy/Platform-v0.yaml` & `xuanpolicy-0.1.6/xuanpolicy/configs/spdqn/toy/Platform-v0.yaml`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-agent: "MPDQN"
-env_name: "toy"
+agent: "SPDQN"
+env_name: "toy_env"
 env_id: "Platform-v0"
-policy: "MPDQN_Policy"
+policy: "SPDQN_Policy"
 representation: "Basic_MLP"
 
 representation_hidden_size: [128,]
 conactor_hidden_size: [128,]
 qnetwork_hidden_size: [128, ]
 
 nsize: 20000
@@ -21,11 +21,11 @@
 start_training: 1000
 
 use_obsnorm: False
 use_rewnorm: False
 obsnorm_range: 5
 rewnorm_range: 5
 
-logdir: "./logs/mpdqn/"
-modeldir: "./models/mpdqn/"
+logdir: "./logs/spdqn/"
+modeldir: "./models/spdqn/"
 
 vectorize: NOREQUIRED
```

### Comparing `xuanpolicy-0.1.5/xuanpolicy/configs/owqmix/mpe/simple_spread.yaml` & `xuanpolicy-0.1.6/xuanpolicy/configs/owqmix/mpe/simple_spread.yaml`

 * *Files identical despite different names*

### Comparing `xuanpolicy-0.1.5/xuanpolicy/configs/pdqn/toy/Platform-v0.yaml` & `xuanpolicy-0.1.6/xuanpolicy/configs/pdqn/toy/Platform-v0.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 agent: "PDQN"
-env_name: "toy"
+env_name: "toy_env"
 env_id: "Platform-v0"
 policy: "PDQN_Policy"
 representation: "Basic_MLP"
 
 representation_hidden_size: [128,]
 conactor_hidden_size: [128,]
 qnetwork_hidden_size: [128, ]
```

### Comparing `xuanpolicy-0.1.5/xuanpolicy/configs/pg/mujoco/InvertedPendulum-v2.yaml` & `xuanpolicy-0.1.6/xuanpolicy/configs/pg/mujoco/InvertedPendulum-v2.yaml`

 * *Files identical despite different names*

### Comparing `xuanpolicy-0.1.5/xuanpolicy/configs/ppg/mujoco/InvertedPendulum-v2.yaml` & `xuanpolicy-0.1.6/xuanpolicy/configs/ppg/mujoco/InvertedPendulum-v2.yaml`

 * *Files identical despite different names*

### Comparing `xuanpolicy-0.1.5/xuanpolicy/configs/ppoclip/atari/PongNoFrameskip-v4.yaml` & `xuanpolicy-0.1.6/xuanpolicy/configs/ppoclip/atari/PongNoFrameskip-v4.yaml`

 * *Files identical despite different names*

### Comparing `xuanpolicy-0.1.5/xuanpolicy/configs/ppoclip/mujoco/InvertedPendulum-v2.yaml` & `xuanpolicy-0.1.6/xuanpolicy/configs/ppoclip/mujoco/InvertedPendulum-v2.yaml`

 * *Files identical despite different names*

### Comparing `xuanpolicy-0.1.5/xuanpolicy/configs/qmix/mpe/simple_spread.yaml` & `xuanpolicy-0.1.6/xuanpolicy/configs/qmix/mpe/simple_spread.yaml`

 * *Files identical despite different names*

### Comparing `xuanpolicy-0.1.5/xuanpolicy/configs/qtran/mpe/simple_spread.yaml` & `xuanpolicy-0.1.6/xuanpolicy/configs/qtran/mpe/simple_spread.yaml`

 * *Files identical despite different names*

### Comparing `xuanpolicy-0.1.5/xuanpolicy/configs/sac/mujoco/HalfCheetah-v3.yaml` & `xuanpolicy-0.1.6/xuanpolicy/configs/sac/mujoco/HalfCheetah-v3.yaml`

 * *Files identical despite different names*

### Comparing `xuanpolicy-0.1.5/xuanpolicy/configs/sacdis/toy/CartPole-v0.yaml` & `xuanpolicy-0.1.6/xuanpolicy/configs/sacdis/toy/CartPole-v0.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 agent: "SACDIS"
-env_name: "toy"
+env_name: "toy_env"
 env_id: "CartPole-v0"
 policy: "Discrete_SAC"
 representation: "Basic_Identical"
 
 representation_hidden_size: [256,]
 
 actor_hidden_size: [128,128,]
```

### Comparing `xuanpolicy-0.1.5/xuanpolicy/configs/spdqn/toy/Platform-v0.yaml` & `xuanpolicy-0.1.6/xuanpolicy/configs/mpdqn/toy/Platform-v0.yaml`

 * *Files 26% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-agent: "SPDQN"
-env_name: "toy"
+agent: "MPDQN"
+env_name: "toy_env"
 env_id: "Platform-v0"
-policy: "SPDQN_Policy"
+policy: "MPDQN_Policy"
 representation: "Basic_MLP"
 
 representation_hidden_size: [128,]
 conactor_hidden_size: [128,]
 qnetwork_hidden_size: [128, ]
 
 nsize: 20000
@@ -21,11 +21,11 @@
 start_training: 1000
 
 use_obsnorm: False
 use_rewnorm: False
 obsnorm_range: 5
 rewnorm_range: 5
 
-logdir: "./logs/spdqn/"
-modeldir: "./models/spdqn/"
+logdir: "./logs/mpdqn/"
+modeldir: "./models/mpdqn/"
 
 vectorize: NOREQUIRED
```

### Comparing `xuanpolicy-0.1.5/xuanpolicy/configs/td3/mujoco/InvertedPendulum-v2.yaml` & `xuanpolicy-0.1.6/xuanpolicy/configs/td3/mujoco/InvertedPendulum-v2.yaml`

 * *Files identical despite different names*

### Comparing `xuanpolicy-0.1.5/xuanpolicy/configs/vdac/mpe/simple_spread.yaml` & `xuanpolicy-0.1.6/xuanpolicy/configs/vdac/mpe/simple_spread.yaml`

 * *Files identical despite different names*

### Comparing `xuanpolicy-0.1.5/xuanpolicy/configs/vdn/mpe/simple_spread.yaml` & `xuanpolicy-0.1.6/xuanpolicy/configs/vdn/mpe/simple_spread.yaml`

 * *Files identical despite different names*

### Comparing `xuanpolicy-0.1.5/xuanpolicy/environment/__init__.py` & `xuanpolicy-0.1.6/xuanpolicy/environment/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,45 +1,44 @@
 import importlib
 
 from .custom_envs.toy_env import Toy_Env
 from .custom_envs.mujoco_env import MuJoCo_Env
 from .custom_envs.atari_env import Atari_Env
-from .custom_envs.pettingzoo_env import PettingZooWrapper
+from .custom_envs.pettingzoo_env import PettingZoo_Env
 
 from .custom_envs.atari_env import ENVIRONMENT_IDS as ATARI_ENVIRONMENTS
 from .custom_envs.mujoco_env import ENVIRONMENT_IDS as MUJOCO_ENVIRONMENTS
 from .custom_envs.robotics_env import ENVIRONMENT_IDS as ROBOTICS_ENVIRONMENTS
 from .custom_envs.toy_env import ENVIRONMENT_IDS as TOY_ENVIRONMENTS
-from .custom_envs.pettingzoo_env import PETTINGZOO_ENVS
+from .custom_envs.pettingzoo_env import PETTINGZOO_ENVIRONMENTS
 
 from .vector_envs.vector_env import VecEnv
 from .vector_envs.dummy_vec_env import DummyVecEnv, DummyVecEnv_MAS
 from .vector_envs.subproc_vec_env import SubprocVecEnv
 
 
 def make_envs(env_name: str,
               env_id: str,
               seed: int,
               vectorize: str,
               parallels: int,
               continuous_action: bool = False,
-              render_mode: str = 'human',
+              render_mode: str = 'rgb_array',
               ):
     def _thunk():
         if env_id in TOY_ENVIRONMENTS:
             env = Toy_Env(env_id, seed)
         elif env_id in MUJOCO_ENVIRONMENTS:
             env = MuJoCo_Env(env_id, seed)
         elif env_id in ATARI_ENVIRONMENTS:
             env = Atari_Env(env_id, seed)
-        elif env_name in PETTINGZOO_ENVS:
+        elif env_name in PETTINGZOO_ENVIRONMENTS:
             scienario = importlib.import_module('pettingzoo.' + env_name + '.' + env_id)
-            env = PettingZooWrapper(scienario.parallel_env(continuous_actions=continuous_action,
-                                                           render_mode=render_mode),
-                                    env_name+'.'+env_id)
+            env = PettingZoo_Env(scienario.parallel_env(continuous_actions=continuous_action, render_mode=render_mode),
+                                 env_name+'.'+env_id)
         else:
             raise NotImplementedError
         return env
 
     if vectorize == "Subproc":
         return SubprocVecEnv([_thunk for _ in range(parallels)])
     elif vectorize == "Dummy":
```

### Comparing `xuanpolicy-0.1.5/xuanpolicy/environment/custom_envs/USVmodel.py` & `xuanpolicy-0.1.6/xuanpolicy/environment/custom_envs/USVmodel.py`

 * *Files identical despite different names*

### Comparing `xuanpolicy-0.1.5/xuanpolicy/environment/custom_envs/atari_env.py` & `xuanpolicy-0.1.6/xuanpolicy/environment/custom_envs/atari_env.py`

 * *Files identical despite different names*

### Comparing `xuanpolicy-0.1.5/xuanpolicy/environment/custom_envs/mujoco_env.py` & `xuanpolicy-0.1.6/xuanpolicy/environment/custom_envs/mujoco_env.py`

 * *Files identical despite different names*

### Comparing `xuanpolicy-0.1.5/xuanpolicy/environment/custom_envs/pettingzoo_env.py` & `xuanpolicy-0.1.6/xuanpolicy/environment/custom_envs/pettingzoo_env.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-import gym
+from pettingzoo.utils.env import ParallelEnv
 import numpy as np
 import ctypes
 
 MPE_N_HANDLE_DICT = {
     "mpe.simple_adversary_v3": 2,
     "mpe.simple_crypto_v3": 3,
     "mpe.simple_push_v3": 2,
@@ -37,55 +37,60 @@
                      'go_v5', 'hanabi_v4', 'leduc_holdem_v4', 'mahjong_v4', 'rps_v2', 'texas_holdem_no_limit_v5',
                      'texas_holdem_v4', 'tictactoe_v3', 'uno_v4']
 MAGENT_ENVS_LARGE_SCALE_MARL = ['adversarial_pursuit_v3', 'battlefield_v3', 'battle_v3', 'combined_arms_v5',
                                 'gather_v3', 'magent_env', 'tiger_deer_v3']
 MPE_ENVS_MARL = ['simple_adversary_v2', 'simple_crypto_v2', 'simple_push_v2', 'simple_reference_v2',
                  'simple_speaker_listener_v3', 'simple_spread_v2', 'simple_tag_v2', 'simple_v2', 'simple_world_comm_v2']
 SISL_ENVS_MARL = ['multiwalker_v7', 'pursuit_v3', 'waterworld_v3']
-PETTINGZOO_ENVS = ['atari', 'butterfly', 'classic', 'magent', 'mpe', 'sisl']
+PETTINGZOO_ENVIRONMENTS = ['atari', 'butterfly', 'classic', 'magent', 'mpe', 'sisl']
 
 
-class PettingZooWrapper(gym.Wrapper):
+class PettingZoo_Env(ParallelEnv):
     def __init__(self, env, scenario_name):
-        # super(PettingZooWrapper, self).__init__(env)
+        super(PettingZoo_Env, self).__init__()
         self.env = env
         self.scenario_name = scenario_name
         self.env.reset()
 
         try:
             self.state_space = self.env.state_space
         except:
             self.state_space = None
-        self.action_spaces = self.env.action_spaces
-        self.observation_spaces = self.env.observation_spaces
-        self.agents = self.env.action_spaces.keys()
+
+        self.action_spaces = {k: self.env.action_space(k) for k in self.env.agents}
+        self.observation_spaces = {k: self.env.observation_space(k) for k in self.env.agents}
+        self.agents = self.env.agents
         self.n_agents_all = len(self.agents)
 
         self.handles = self.get_handles()
 
         self.agent_ids = [self.get_ids(h) for h in self.handles]
         self.n_agents = [self.get_num(h) for h in self.handles]
 
         # self.reward_range = env.reward_range
         self.metadata = env.metadata
         # self._warn_double_wrap()
 
-        self.episode_length = 0
+        self.step_count = 0
         # assert self.spec.id in ENVIRONMENTS
 
         self.max_cycles = self.env.aec_env.env.env.max_cycles
 
     def step(self, action):
-        self.episode_length += 1
+        self.step_count += 1
         observations, rewards, terminations, truncations, infos = self.env.step(action)
+        for k, v in truncations.items():
+            if v is True:
+                terminations[k] = v
         return observations, rewards, terminations, truncations, infos
 
-    def reset(self):
-        self.episode_length = 0
-        return self.env.reset()
+    def reset(self, seed=None, options=None):
+        self.step_count = 0
+        observations, infos = self.env.reset()
+        return observations
 
     def state(self):
         try:
             return self.env.state()
         except:
             return None
 
@@ -118,14 +123,15 @@
                     alive_ids = self.get_ids(handle)
                     mask[alive_ids] = True  # get alive agents
                 except AttributeError("Cannot get the ids for alive agents!"):
                     return
         return mask
 
     def get_handles(self):
-        try: return self.env.handles
-        except:
-            try: return self.env.env.get_handles()
+        if hasattr(self.env, 'handles'):
+            return self.env.handles
+        else:
+            try:
+                return self.env.env.get_handles()
             except:
                 handles = [ctypes.c_int(h) for h in range(MPE_N_HANDLE_DICT[self.scenario_name])]
-                # print("env.handles is None, now is set as: ", handles)
                 return handles
```

### Comparing `xuanpolicy-0.1.5/xuanpolicy/environment/custom_envs/toy_env.py` & `xuanpolicy-0.1.6/xuanpolicy/environment/custom_envs/toy_env.py`

 * *Files identical despite different names*

### Comparing `xuanpolicy-0.1.5/xuanpolicy/environment/vector_envs/dummy_vec_env.py` & `xuanpolicy-0.1.6/xuanpolicy/environment/vector_envs/dummy_vec_env.py`

 * *Files 1% similar despite different names*

```diff
@@ -128,15 +128,15 @@
         self.buf_rews_dict[i_env] = {k: 0.0 for k in self.keys}
         self.buf_dones_dict[i_env] = {k: False for k in self.keys}
         self.buf_infos_dict[i_env] = {k: {} for k in self.keys}
 
     def reset(self):
         for e in range(self.num_envs):
             o = self.envs[e].reset()
-            self.buf_obs_dict[e].update(o[0])
+            self.buf_obs_dict[e].update(o)
             for h, agent_keys_h in enumerate(self.agent_keys):
                 self.buf_obs[h][e] = itemgetter(*agent_keys_h)(self.buf_obs_dict[e])
 
         return self.buf_obs
 
     def reset_one_env(self, e):
         o = self.envs[e].reset()
@@ -195,17 +195,17 @@
             try:
                 done_all.append(all(itemgetter(*list(self.keys))(self.buf_dones_dict[e])))
             except:
                 done_all.append(itemgetter(*list(self.keys))(self.buf_dones_dict[e]))
 
         return self.buf_obs, self.buf_rews, self.buf_dones, done_all, self.buf_infos
 
-    def render(self, time_delay=0.0, mode='human'):
+    def render(self, time_delay=0.0):
         time.sleep(time_delay)
-        return [env.render(mode) for env in self.envs]
+        return [env.render() for env in self.envs]
 
     def global_state(self):
         return np.array([env.state() for env in self.envs])
 
     def global_state_one_env(self, e):
         return np.array(self.envs[e].state())
```

### Comparing `xuanpolicy-0.1.5/xuanpolicy/environment/vector_envs/env_utils.py` & `xuanpolicy-0.1.6/xuanpolicy/environment/vector_envs/env_utils.py`

 * *Files identical despite different names*

### Comparing `xuanpolicy-0.1.5/xuanpolicy/environment/vector_envs/subproc_vec_env.py` & `xuanpolicy-0.1.6/xuanpolicy/environment/vector_envs/subproc_vec_env.py`

 * *Files identical despite different names*

### Comparing `xuanpolicy-0.1.5/xuanpolicy/environment/vector_envs/vector_env.py` & `xuanpolicy-0.1.6/xuanpolicy/environment/vector_envs/vector_env.py`

 * *Files identical despite different names*

### Comparing `xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_ms/agents/__init__.py` & `xuanpolicy-0.1.6/xuanpolicy/mindspore/agents/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,20 +5,20 @@
 from tqdm import tqdm
 from torch.utils.tensorboard import SummaryWriter
 import mindspore as ms
 import mindspore.nn as nn
 from mindspore import context
 from xuanpolicy.common import *
 from xuanpolicy.environment import *
-from xuanpolicy.xuanpolicy_ms.learners import *
-from xuanpolicy.xuanpolicy_ms.utils import *
-from xuanpolicy.xuanpolicy_ms.policies import *
-from xuanpolicy.xuanpolicy_ms.policies import REGISTRY as REGISTRY_Policy
-from xuanpolicy.xuanpolicy_ms.utils.input_reformat import get_repre_in, get_policy_in_marl
-from xuanpolicy.xuanpolicy_ms.representations import REGISTRY as REGISTRY_Representation
+from xuanpolicy.mindspore.learners import *
+from xuanpolicy.mindspore.utils import *
+from xuanpolicy.mindspore.policies import *
+from xuanpolicy.mindspore.policies import REGISTRY as REGISTRY_Policy
+from xuanpolicy.mindspore.utils.input_reformat import get_repre_in, get_policy_in_marl
+from xuanpolicy.mindspore.representations import REGISTRY as REGISTRY_Representation
 from mindspore.nn import Adam
 from mindspore.nn.learning_rate_schedule import ExponentialDecayLR as lr_decay_model
 
 from .agent import Agent
 from .agents_marl import MARLAgents, RandomAgents, get_total_iters
 
 '''
```

### Comparing `xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_ms/agents/agent.py` & `xuanpolicy-0.1.6/xuanpolicy/torch/agents/agent.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,25 +1,27 @@
-from xuanpolicy.xuanpolicy_ms.agents import *
+from xuanpolicy.torch.agents import *
 
 
 class Agent(ABC):
     def __init__(self,
                  envs: VecEnv,
-                 policy: nn.Cell,
+                 policy: nn.Module,
                  memory: Buffer,
                  learner: Learner,
                  writer: SummaryWriter,
+                 device: Optional[Union[str, int, torch.device]] = None,
                  logdir: str = "./logs/",
                  modeldir: str = "./models/",
                  ):
         self.envs = envs
         self.policy = policy
         self.memory = memory
         self.learner = learner
         self.writer = writer
+        self.device = device
         self.logdir = logdir
         self.modeldir = modeldir
         create_directory(logdir)
         create_directory(modeldir)
 
     def save_model(self):
         self.learner.save_model()
```

### Comparing `xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_ms/agents/agents_marl.py` & `xuanpolicy-0.1.6/xuanpolicy/mindspore/agents/agents_marl.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import mindspore as ms
 import mindspore.ops as ops
 from mindspore import Tensor
-from xuanpolicy.xuanpolicy_ms.agents import *
+from xuanpolicy.mindspore.agents import *
 
 
 class MARLAgents(object):
     def __init__(self,
                  config: Namespace,
                  envs: DummyVecEnv_MAS,
                  policy: nn.Cell,
```

### Comparing `xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_ms/agents/multi_agent_rl/coma_agents.py` & `xuanpolicy-0.1.6/xuanpolicy/mindspore/agents/multi_agent_rl/coma_agents.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-from xuanpolicy.xuanpolicy_ms.agents import *
-from xuanpolicy.xuanpolicy_ms.agents.agents_marl import linear_decay_or_increase
+from xuanpolicy.mindspore.agents import *
+from xuanpolicy.mindspore.agents.agents_marl import linear_decay_or_increase
 
 
 class COMA_Agents(MARLAgents):
     def __init__(self,
                  config: Namespace,
                  envs: DummyVecEnv_MAS):
         self.comm = MPI.COMM_WORLD
```

### Comparing `xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_ms/agents/multi_agent_rl/dcg_agents.py` & `xuanpolicy-0.1.6/xuanpolicy/mindspore/agents/multi_agent_rl/dcg_agents.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-from xuanpolicy.xuanpolicy_ms.agents import *
-from xuanpolicy.xuanpolicy_ms.agents.agents_marl import linear_decay_or_increase
+from xuanpolicy.mindspore.agents import *
+from xuanpolicy.mindspore.agents.agents_marl import linear_decay_or_increase
 
 
 class DCG_Agents(MARLAgents):
     def __init__(self,
                  config: Namespace,
                  envs: DummyVecEnv_MAS):
         self.comm = MPI.COMM_WORLD
```

### Comparing `xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_ms/agents/multi_agent_rl/iddpg_agents.py` & `xuanpolicy-0.1.6/xuanpolicy/mindspore/agents/multi_agent_rl/matd3_agents.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-from xuanpolicy.xuanpolicy_ms.agents import *
+from xuanpolicy.mindspore.agents import *
 
 
-class IDDPG_Agents(MARLAgents):
+class MATD3_Agents(MARLAgents):
     def __init__(self,
                  config: Namespace,
                  envs: DummyVecEnv_MAS):
         self.comm = MPI.COMM_WORLD
 
         self.gamma = config.gamma
         self.use_obsnorm = config.use_obsnorm
@@ -16,19 +16,28 @@
         input_representation = get_repre_in(config)
         representation = REGISTRY_Representation[config.representation](*input_representation)
         input_policy = get_policy_in_marl(config, representation, config.agent_keys)
         policy = REGISTRY_Policy[config.policy](*input_policy)
         scheduler = [lr_decay_model(learning_rate=config.lr_a, decay_rate=0.5,
                                     decay_steps=get_total_iters(config.agent_name, config)),
                      lr_decay_model(learning_rate=config.lr_c, decay_rate=0.5,
+                                    decay_steps=get_total_iters(config.agent_name, config)),
+                     lr_decay_model(learning_rate=config.lr_c, decay_rate=0.5,
                                     decay_steps=get_total_iters(config.agent_name, config))]
         optimizer = [Adam(policy.parameters_actor, scheduler[0], eps=1e-5),
-                     Adam(policy.parameters_critic, scheduler[1], eps=1e-5)]
+                     Adam(policy.parameters_critic_A, scheduler[1], eps=1e-5),
+                     Adam(policy.parameters_critic_B, scheduler[2], eps=1e-5)]
+
         self.observation_space = envs.observation_space
         self.action_space = envs.action_space
+        self.actions_high, self.actions_low = [], []
+        for k in config.agent_keys:
+            self.actions_high.append(self.action_space[k].high)
+            self.actions_low.append(self.action_space[k].low)
+        self.actions_high, self.actions_low = np.array(self.actions_high), np.array(self.actions_low)
         self.representation_info_shape = policy.representation.output_shapes
         self.auxiliary_info_shape = {}
 
         writer = SummaryWriter(config.logdir)
         if config.state_space is not None:
             config.dim_state, state_shape = config.state_space.shape, config.state_space.shape
         else:
@@ -37,21 +46,22 @@
                                       config.obs_shape,
                                       config.act_shape,
                                       config.rew_shape,
                                       config.done_shape,
                                       envs.num_envs,
                                       config.buffer_size,
                                       config.batch_size)
-        learner = IDDPG_Learner(config, policy, optimizer, scheduler, writer, config.modeldir, config.gamma)
+        learner = MATD3_Learner(config, policy, optimizer, scheduler, writer,
+                                 config.device, config.modeldir, config.gamma)
 
         self.obs_rms = RunningMeanStd(shape=space2shape(self.observation_space[config.agent_keys[0]]),
                                       comm=self.comm, use_mpi=False)
         self.ret_rms = RunningMeanStd(shape=(), comm=self.comm, use_mpi=False)
-        super(IDDPG_Agents, self).__init__(config, envs, policy, memory, learner, writer,
-                                           config.logdir, config.modeldir)
+        super(MATD3_Agents, self).__init__(config, envs, policy, memory, learner, writer,
+                                            config.logdir, config.modeldir)
 
     def _process_observation(self, observations):
         if self.use_obsnorm:
             if isinstance(self.observation_space, Dict):
                 for key in self.observation_space.spaces.keys():
                     observations[key] = np.clip(
                         (observations[key] - self.obs_rms.mean[key]) / (self.obs_rms.std[key] + EPS),
@@ -72,13 +82,14 @@
         batch_size = len(obs_n)
         agents_id = ops.broadcast_to(self.expand_dims(self.eye(self.n_agents, self.n_agents, ms.float32), 0),
                                      (batch_size, -1, -1))
         _, actions = self.policy(Tensor(obs_n), agents_id)
         actions = actions.asnumpy()
         if noise:
             actions += np.random.normal(0, self.args.sigma, size=actions.shape)
+            actions = np.clip(actions, self.actions_low, self.actions_high)
         return actions
 
     def train(self, i_episode):
         if self.memory.can_sample(self.args.batch_size):
             sample = self.memory.sample()
             self.learner.update(sample)
```

### Comparing `xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_ms/agents/multi_agent_rl/iql_agents.py` & `xuanpolicy-0.1.6/xuanpolicy/mindspore/agents/multi_agent_rl/iql_agents.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-from xuanpolicy.xuanpolicy_ms.agents import *
-from xuanpolicy.xuanpolicy_ms.agents.agents_marl import linear_decay_or_increase
+from xuanpolicy.mindspore.agents import *
+from xuanpolicy.mindspore.agents.agents_marl import linear_decay_or_increase
 
 
 class IQL_Agents(MARLAgents):
     def __init__(self,
                  config: Namespace,
                  envs: DummyVecEnv_MAS):
         self.comm = MPI.COMM_WORLD
```

### Comparing `xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_ms/agents/multi_agent_rl/isac_agents.py` & `xuanpolicy-0.1.6/xuanpolicy/mindspore/agents/multi_agent_rl/iddpg_agents.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-from xuanpolicy.xuanpolicy_ms.agents import *
+from xuanpolicy.mindspore.agents import *
 
 
-class ISAC_Agents(MARLAgents):
+class IDDPG_Agents(MARLAgents):
     def __init__(self,
                  config: Namespace,
                  envs: DummyVecEnv_MAS):
         self.comm = MPI.COMM_WORLD
 
         self.gamma = config.gamma
         self.use_obsnorm = config.use_obsnorm
@@ -21,14 +21,19 @@
                                     decay_steps=get_total_iters(config.agent_name, config)),
                      lr_decay_model(learning_rate=config.lr_c, decay_rate=0.5,
                                     decay_steps=get_total_iters(config.agent_name, config))]
         optimizer = [Adam(policy.parameters_actor, scheduler[0], eps=1e-5),
                      Adam(policy.parameters_critic, scheduler[1], eps=1e-5)]
         self.observation_space = envs.observation_space
         self.action_space = envs.action_space
+        self.actions_high, self.actions_low = [], []
+        for k in config.agent_keys:
+            self.actions_high.append(self.action_space[k].high)
+            self.actions_low.append(self.action_space[k].low)
+        self.actions_high, self.actions_low = np.array(self.actions_high), np.array(self.actions_low)
         self.representation_info_shape = policy.representation.output_shapes
         self.auxiliary_info_shape = {}
 
         writer = SummaryWriter(config.logdir)
         if config.state_space is not None:
             config.dim_state, state_shape = config.state_space.shape, config.state_space.shape
         else:
@@ -37,21 +42,21 @@
                                       config.obs_shape,
                                       config.act_shape,
                                       config.rew_shape,
                                       config.done_shape,
                                       envs.num_envs,
                                       config.buffer_size,
                                       config.batch_size)
-        learner = ISAC_Learner(config, policy, optimizer, scheduler, writer, config.modeldir, config.gamma)
+        learner = IDDPG_Learner(config, policy, optimizer, scheduler, writer, config.modeldir, config.gamma)
 
         self.obs_rms = RunningMeanStd(shape=space2shape(self.observation_space[config.agent_keys[0]]),
                                       comm=self.comm, use_mpi=False)
         self.ret_rms = RunningMeanStd(shape=(), comm=self.comm, use_mpi=False)
-        super(ISAC_Agents, self).__init__(config, envs, policy, memory, learner, writer,
-                                          config.logdir, config.modeldir)
+        super(IDDPG_Agents, self).__init__(config, envs, policy, memory, learner, writer,
+                                           config.logdir, config.modeldir)
 
     def _process_observation(self, observations):
         if self.use_obsnorm:
             if isinstance(self.observation_space, Dict):
                 for key in self.observation_space.spaces.keys():
                     observations[key] = np.clip(
                         (observations[key] - self.obs_rms.mean[key]) / (self.obs_rms.std[key] + EPS),
@@ -64,20 +69,22 @@
 
     def _process_reward(self, rewards):
         if self.use_rewnorm:
             std = np.clip(self.ret_rms.std, 0.1, 100)
             return np.clip(rewards / std, -self.rewnorm_range, self.rewnorm_range)
         return rewards
 
-    def act(self, obs_n, episode, test_mode, state=None, noise=False):
+    def act(self, obs_n, episode, test_mode, noise=False):
         batch_size = len(obs_n)
         agents_id = ops.broadcast_to(self.expand_dims(self.eye(self.n_agents, self.n_agents, ms.float32), 0),
                                      (batch_size, -1, -1))
-        _, act_mu, act_std = self.policy(Tensor(obs_n), agents_id)
-        acts = self.policy.actor_net.sample(act_mu, act_std)
-        actions = acts.asnumpy()
+        _, actions = self.policy(Tensor(obs_n), agents_id)
+        actions = actions.asnumpy()
+        if noise:
+            actions += np.random.normal(0, self.args.sigma, size=actions.shape)
+            actions = np.clip(actions, self.actions_low, self.actions_high)
         return actions
 
     def train(self, i_episode):
         if self.memory.can_sample(self.args.batch_size):
             sample = self.memory.sample()
             self.learner.update(sample)
```

### Comparing `xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_ms/agents/multi_agent_rl/maddpg_agents.py` & `xuanpolicy-0.1.6/xuanpolicy/mindspore/agents/multi_agent_rl/qmix_agents.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,57 +1,64 @@
-from xuanpolicy.xuanpolicy_ms.agents import *
+from xuanpolicy.mindspore.agents import *
+from xuanpolicy.mindspore.agents.agents_marl import linear_decay_or_increase
 
 
-class MADDPG_Agents(MARLAgents):
+class QMIX_Agents(MARLAgents):
     def __init__(self,
                  config: Namespace,
                  envs: DummyVecEnv_MAS):
         self.comm = MPI.COMM_WORLD
 
         self.gamma = config.gamma
         self.use_obsnorm = config.use_obsnorm
         self.use_rewnorm = config.use_rewnorm
         self.obsnorm_range = config.obsnorm_range
         self.rewnorm_range = config.rewnorm_range
 
+        self.start_greedy = config.start_greedy
+        self.end_greedy = config.end_greedy
+        self.egreedy = config.start_greedy
+        if config.state_space is not None:
+            config.dim_state, state_shape = config.state_space.shape, config.state_space.shape
+        else:
+            config.dim_state, state_shape = None, None
+
         input_representation = get_repre_in(config)
         representation = REGISTRY_Representation[config.representation](*input_representation)
-        input_policy = get_policy_in_marl(config, representation, config.agent_keys)
+        mixer = QMIX_mixer(config.dim_state[0], config.hidden_dim_mixing_net, config.hidden_dim_hyper_net,
+                           config.n_agents)
+        input_policy = get_policy_in_marl(config, representation, config.agent_keys, mixer)
         policy = REGISTRY_Policy[config.policy](*input_policy)
-        scheduler = [lr_decay_model(learning_rate=config.lr_a, decay_rate=0.5,
-                                    decay_steps=get_total_iters(config.agent_name, config)),
-                     lr_decay_model(learning_rate=config.lr_c, decay_rate=0.5,
-                                    decay_steps=get_total_iters(config.agent_name, config))]
-        optimizer = [Adam(policy.parameters_actor, scheduler[0], eps=1e-5),
-                     Adam(policy.parameters_critic, scheduler[1], eps=1e-5)]
+
+        scheduler = lr_decay_model(learning_rate=config.learning_rate, decay_rate=0.5,
+                                   decay_steps=get_total_iters(config.agent_name, config))
+        optimizer = Adam(policy.trainable_params(), scheduler, eps=1e-5)
         self.observation_space = envs.observation_space
         self.action_space = envs.action_space
         self.representation_info_shape = policy.representation.output_shapes
         self.auxiliary_info_shape = {}
 
         writer = SummaryWriter(config.logdir)
-        if config.state_space is not None:
-            config.dim_state, state_shape = config.state_space.shape, config.state_space.shape
-        else:
-            config.dim_state, state_shape = None, None
         memory = MARL_OffPolicyBuffer(state_shape,
                                       config.obs_shape,
                                       config.act_shape,
                                       config.rew_shape,
                                       config.done_shape,
                                       envs.num_envs,
                                       config.buffer_size,
                                       config.batch_size)
-        learner = MADDPG_Learner(config, policy, optimizer, scheduler, writer, config.modeldir, config.gamma)
+        learner = QMIX_Learner(config, policy, optimizer, scheduler, writer,
+                               config.modeldir, config.gamma, config.sync_frequency)
 
         self.obs_rms = RunningMeanStd(shape=space2shape(self.observation_space[config.agent_keys[0]]),
                                       comm=self.comm, use_mpi=False)
         self.ret_rms = RunningMeanStd(shape=(), comm=self.comm, use_mpi=False)
-        super(MADDPG_Agents, self).__init__(config, envs, policy, memory, learner, writer,
-                                            config.logdir, config.modeldir)
+        self.epsilon_decay = linear_decay_or_increase(config.start_greedy, config.end_greedy,
+                                                      config.greedy_update_steps)
+        super(QMIX_Agents, self).__init__(config, envs, policy, memory, learner, writer, config.logdir, config.modeldir)
 
     def _process_observation(self, observations):
         if self.use_obsnorm:
             if isinstance(self.observation_space, Dict):
                 for key in self.observation_space.spaces.keys():
                     observations[key] = np.clip(
                         (observations[key] - self.obs_rms.mean[key]) / (self.obs_rms.std[key] + EPS),
@@ -64,21 +71,14 @@
 
     def _process_reward(self, rewards):
         if self.use_rewnorm:
             std = np.clip(self.ret_rms.std, 0.1, 100)
             return np.clip(rewards / std, -self.rewnorm_range, self.rewnorm_range)
         return rewards
 
-    def act(self, obs_n, episode, test_mode, noise=False):
-        batch_size = len(obs_n)
-        agents_id = ops.broadcast_to(self.expand_dims(self.eye(self.n_agents, self.n_agents, ms.float32), 0),
-                                     (batch_size, -1, -1))
-        _, actions = self.policy(Tensor(obs_n), agents_id)
-        actions = actions.asnumpy()
-        if noise:
-            actions += np.random.normal(0, self.args.sigma, size=actions.shape)
-        return actions
-
     def train(self, i_episode):
+        self.epsilon_decay.update()
+        for i in range(self.nenvs):
+            self.writer.add_scalars("epsilon", {"env-%d" % i: self.epsilon_decay.epsilon}, i_episode)
         if self.memory.can_sample(self.args.batch_size):
             sample = self.memory.sample()
             self.learner.update(sample)
```

### Comparing `xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_ms/agents/multi_agent_rl/mappoclip_agents.py` & `xuanpolicy-0.1.6/xuanpolicy/mindspore/agents/multi_agent_rl/mappoclip_agents.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from xuanpolicy.xuanpolicy_ms.agents import *
+from xuanpolicy.mindspore.agents import *
 
 
 class MAPPO_Clip_Agents(MARLAgents):
     def __init__(self,
                  config: Namespace,
                  envs: DummyVecEnv_MAS):
         self.comm = MPI.COMM_WORLD
```

### Comparing `xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_ms/agents/multi_agent_rl/mappokl_agents.py` & `xuanpolicy-0.1.6/xuanpolicy/mindspore/agents/multi_agent_rl/mappokl_agents.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from xuanpolicy.xuanpolicy_ms.agents import *
+from xuanpolicy.mindspore.agents import *
 
 
 class MAPPO_KL_Agents(MARLAgents):
     def __init__(self,
                  config: Namespace,
                  envs: DummyVecEnv_MAS):
         self.comm = MPI.COMM_WORLD
```

### Comparing `xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_ms/agents/multi_agent_rl/masac_agents.py` & `xuanpolicy-0.1.6/xuanpolicy/tensorflow/agents/multi_agent_rl/iql_agents.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,32 +1,37 @@
-from xuanpolicy.xuanpolicy_ms.agents import *
+from xuanpolicy.tensorflow.agents import *
+from xuanpolicy.tensorflow.agents.agents_marl import linear_decay_or_increase
 
 
-class MASAC_Agents(MARLAgents):
+class IQL_Agents(MARLAgents):
     def __init__(self,
                  config: Namespace,
-                 envs: DummyVecEnv_MAS):
+                 envs: DummyVecEnv_MAS,
+                 device: str = "cpu:0"):
         self.comm = MPI.COMM_WORLD
 
         self.gamma = config.gamma
         self.use_obsnorm = config.use_obsnorm
         self.use_rewnorm = config.use_rewnorm
         self.obsnorm_range = config.obsnorm_range
         self.rewnorm_range = config.rewnorm_range
 
+        self.start_greedy = config.start_greedy
+        self.end_greedy = config.end_greedy
+        self.egreedy = config.start_greedy
+
         input_representation = get_repre_in(config)
         representation = REGISTRY_Representation[config.representation](*input_representation)
         input_policy = get_policy_in_marl(config, representation, config.agent_keys)
         policy = REGISTRY_Policy[config.policy](*input_policy)
-        scheduler = [lr_decay_model(learning_rate=config.lr_a, decay_rate=0.5,
-                                    decay_steps=get_total_iters(config.agent_name, config)),
-                     lr_decay_model(learning_rate=config.lr_c, decay_rate=0.5,
-                                    decay_steps=get_total_iters(config.agent_name, config))]
-        optimizer = [Adam(policy.parameters_actor, scheduler[0], eps=1e-5),
-                     Adam(policy.parameters_critic, scheduler[1], eps=1e-5)]
+        # lr_scheduler = tk.optimizers.schedules.ExponentialDecay(config.learning_rate, decay_steps=1000,
+        #                                                         decay_rate=0.9)
+        lr_scheduler = MyLinearLR(config.learning_rate, start_factor=1.0, end_factor=0.5,
+                                  total_iters=get_total_iters(config.agent_name, config))
+        optimizer = tk.optimizers.Adam(lr_scheduler)
         self.observation_space = envs.observation_space
         self.action_space = envs.action_space
         self.representation_info_shape = policy.representation.output_shapes
         self.auxiliary_info_shape = {}
 
         writer = SummaryWriter(config.logdir)
         if config.state_space is not None:
@@ -37,21 +42,24 @@
                                       config.obs_shape,
                                       config.act_shape,
                                       config.rew_shape,
                                       config.done_shape,
                                       envs.num_envs,
                                       config.buffer_size,
                                       config.batch_size)
-        learner = MASAC_Learner(config, policy, optimizer, scheduler, writer, config.modeldir, config.gamma)
+        learner = IQL_Learner(config, policy, optimizer, writer,
+                              config.device, config.modeldir, config.gamma, config.sync_frequency)
 
         self.obs_rms = RunningMeanStd(shape=space2shape(self.observation_space[config.agent_keys[0]]),
                                       comm=self.comm, use_mpi=False)
         self.ret_rms = RunningMeanStd(shape=(), comm=self.comm, use_mpi=False)
-        super(MASAC_Agents, self).__init__(config, envs, policy, memory, learner, writer,
-                                           config.logdir, config.modeldir)
+        self.epsilon_decay = linear_decay_or_increase(config.start_greedy, config.end_greedy,
+                                                      config.greedy_update_steps)
+        super(IQL_Agents, self).__init__(config, envs, policy, memory, learner, writer, device,
+                                         config.logdir, config.modeldir)
 
     def _process_observation(self, observations):
         if self.use_obsnorm:
             if isinstance(self.observation_space, Dict):
                 for key in self.observation_space.spaces.keys():
                     observations[key] = np.clip(
                         (observations[key] - self.obs_rms.mean[key]) / (self.obs_rms.std[key] + EPS),
@@ -64,20 +72,14 @@
 
     def _process_reward(self, rewards):
         if self.use_rewnorm:
             std = np.clip(self.ret_rms.std, 0.1, 100)
             return np.clip(rewards / std, -self.rewnorm_range, self.rewnorm_range)
         return rewards
 
-    def act(self, obs_n, episode, test_mode, state=None, noise=False):
-        batch_size = len(obs_n)
-        agents_id = ops.broadcast_to(self.expand_dims(self.eye(self.n_agents, self.n_agents, ms.float32), 0),
-                                     (batch_size, -1, -1))
-        _, act_mu, act_std = self.policy(Tensor(obs_n), agents_id)
-        acts = self.policy.actor_net.sample(act_mu, act_std)
-        actions = acts.asnumpy()
-        return actions
-
     def train(self, i_episode):
+        self.epsilon_decay.update()
+        for i in range(self.nenvs):
+            self.writer.add_scalars("epsilon", {"env-%d" % i: self.epsilon_decay.epsilon}, i_episode)
         if self.memory.can_sample(self.args.batch_size):
             sample = self.memory.sample()
             self.learner.update(sample)
```

### Comparing `xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_ms/agents/multi_agent_rl/matd3_agents.py` & `xuanpolicy-0.1.6/xuanpolicy/tensorflow/agents/multi_agent_rl/mappoclip_agents.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,62 +1,57 @@
-from xuanpolicy.xuanpolicy_ms.agents import *
+from xuanpolicy.tensorflow.agents import *
 
 
-class MATD3_Agents(MARLAgents):
+class MAPPO_Clip_Agents(MARLAgents):
     def __init__(self,
                  config: Namespace,
-                 envs: DummyVecEnv_MAS):
+                 envs: DummyVecEnv_MAS,
+                 device: str = "cpu:0"):
         self.comm = MPI.COMM_WORLD
 
         self.gamma = config.gamma
         self.use_obsnorm = config.use_obsnorm
         self.use_rewnorm = config.use_rewnorm
         self.obsnorm_range = config.obsnorm_range
         self.rewnorm_range = config.rewnorm_range
 
+        if config.state_space is not None:
+            config.dim_state, state_shape = config.state_space.shape, config.state_space.shape
+        else:
+            config.dim_state, state_shape = None, None
+
         input_representation = get_repre_in(config)
         representation = REGISTRY_Representation[config.representation](*input_representation)
+
         input_policy = get_policy_in_marl(config, representation, config.agent_keys)
         policy = REGISTRY_Policy[config.policy](*input_policy)
-        scheduler = [lr_decay_model(learning_rate=config.lr_a, decay_rate=0.5,
-                                    decay_steps=get_total_iters(config.agent_name, config)),
-                     lr_decay_model(learning_rate=config.lr_c, decay_rate=0.5,
-                                    decay_steps=get_total_iters(config.agent_name, config)),
-                     lr_decay_model(learning_rate=config.lr_c, decay_rate=0.5,
-                                    decay_steps=get_total_iters(config.agent_name, config))]
-        optimizer = [Adam(policy.parameters_actor, scheduler[0], eps=1e-5),
-                     Adam(policy.parameters_critic_A, scheduler[1], eps=1e-5),
-                     Adam(policy.parameters_critic_B, scheduler[2], eps=1e-5)]
-
+        lr_scheduler = MyLinearLR(config.learning_rate, start_factor=1.0, end_factor=0.5,
+                                  total_iters=get_total_iters(config.agent_name, config))
+        optimizer = tk.optimizers.Adam(lr_scheduler)
         self.observation_space = envs.observation_space
         self.action_space = envs.action_space
         self.representation_info_shape = policy.representation.output_shapes
         self.auxiliary_info_shape = {}
 
         writer = SummaryWriter(config.logdir)
         if config.state_space is not None:
             config.dim_state, state_shape = config.state_space.shape, config.state_space.shape
         else:
             config.dim_state, state_shape = None, None
-        memory = MARL_OffPolicyBuffer(state_shape,
-                                      config.obs_shape,
-                                      config.act_shape,
-                                      config.rew_shape,
-                                      config.done_shape,
-                                      envs.num_envs,
-                                      config.buffer_size,
-                                      config.batch_size)
-        learner = MATD3_Learner(config, policy, optimizer, scheduler, writer,
-                                 config.device, config.modeldir, config.gamma)
+        memory = MARL_OnPolicyBuffer(state_shape, config.obs_shape, config.act_shape, config.rew_shape,
+                                     config.done_shape, envs.num_envs, config.nsteps, config.nminibatch,
+                                     config.use_gae, config.use_advnorm, config.gamma, config.lam)
+        learner = MAPPO_Clip_Learner(config, policy, optimizer, writer,
+                                     config.device, config.modeldir, config.gamma)
 
         self.obs_rms = RunningMeanStd(shape=space2shape(self.observation_space[config.agent_keys[0]]),
                                       comm=self.comm, use_mpi=False)
         self.ret_rms = RunningMeanStd(shape=(), comm=self.comm, use_mpi=False)
-        super(MATD3_Agents, self).__init__(config, envs, policy, memory, learner, writer,
-                                            config.logdir, config.modeldir)
+        super(MAPPO_Clip_Agents, self).__init__(config, envs, policy, memory, learner, writer, device,
+                                                config.logdir, config.modeldir)
 
     def _process_observation(self, observations):
         if self.use_obsnorm:
             if isinstance(self.observation_space, Dict):
                 for key in self.observation_space.spaces.keys():
                     observations[key] = np.clip(
                         (observations[key] - self.obs_rms.mean[key]) / (self.obs_rms.std[key] + EPS),
@@ -69,21 +64,36 @@
 
     def _process_reward(self, rewards):
         if self.use_rewnorm:
             std = np.clip(self.ret_rms.std, 0.1, 100)
             return np.clip(rewards / std, -self.rewnorm_range, self.rewnorm_range)
         return rewards
 
-    def act(self, obs_n, episode, test_mode, noise=False):
+    def act(self, obs_n, episode, test_mode, state=None, noise=False):
         batch_size = len(obs_n)
-        agents_id = ops.broadcast_to(self.expand_dims(self.eye(self.n_agents, self.n_agents, ms.float32), 0),
-                                     (batch_size, -1, -1))
-        _, actions = self.policy(Tensor(obs_n), agents_id)
-        actions = actions.asnumpy()
-        if noise:
-            actions += np.random.normal(0, self.args.sigma, size=actions.shape)
-        return actions
+        with tf.device(self.device):
+            agents_id = tf.tile(tf.expand_dims(tf.eye(self.n_agents), axis=0), multiples=(batch_size, 1, 1))
+            inputs_policy = {"obs": tf.convert_to_tensor(obs_n), "ids": agents_id}
+            _, dists = self.policy(inputs_policy)
+            acts = dists.stochastic_sample()
+            log_pi_a = dists.log_prob(acts)
+            state = tf.convert_to_tensor(state)
+            state_expand = tf.tile(tf.expand_dims(state, axis=-2), (1, self.n_agents, 1))
+            vs = self.policy.values(state_expand, agents_id)
+        return acts.numpy(), log_pi_a.numpy(), vs.numpy()
+
+    def value(self, obs, state):
+        batch_size = len(state)
+        agents_id = tf.tile(tf.expand_dims(tf.eye(self.n_agents), axis=0), multiples=(batch_size, 1, 1))
+        repre_out = self.policy.representation(obs)
+        critic_input = tf.concat([torch.Tensor(repre_out['state']), agents_id], axis=-1)
+        values_n = self.policy.critic(critic_input)
+        values = self.policy.value_tot(values_n, global_state=state)
+        values = tf.expand_dims(tf.tile(tf.reshape(values, (-1, 1)), (1, self.n_agents)), axis=-1)
+        return values.numpy()
 
     def train(self, i_episode):
-        if self.memory.can_sample(self.args.batch_size):
-            sample = self.memory.sample()
-            self.learner.update(sample)
+        if self.memory.full:
+            for _ in range(self.args.nminibatch * self.args.nepoch):
+                sample = self.memory.sample()
+                self.learner.update(sample)
+            self.memory.clear()
```

### Comparing `xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_ms/agents/multi_agent_rl/mfac_agents.py` & `xuanpolicy-0.1.6/xuanpolicy/mindspore/agents/multi_agent_rl/mfac_agents.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from xuanpolicy.xuanpolicy_ms.agents import *
+from xuanpolicy.mindspore.agents import *
 
 
 class MFAC_Agents(MARLAgents):
     def __init__(self,
                  config: Namespace,
                  envs: DummyVecEnv_MAS):
         self.comm = MPI.COMM_WORLD
```

### Comparing `xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_ms/agents/multi_agent_rl/mfq_agents.py` & `xuanpolicy-0.1.6/xuanpolicy/mindspore/agents/multi_agent_rl/mfq_agents.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-from xuanpolicy.xuanpolicy_ms.agents import *
-from xuanpolicy.xuanpolicy_ms.agents.agents_marl import linear_decay_or_increase
+from xuanpolicy.mindspore.agents import *
+from xuanpolicy.mindspore.agents.agents_marl import linear_decay_or_increase
 
 
 class MFQ_Agents(MARLAgents):
     def __init__(self,
                  config: Namespace,
                  envs: DummyVecEnv_MAS):
         self.comm = MPI.COMM_WORLD
```

### Comparing `xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_ms/agents/multi_agent_rl/qmix_agents.py` & `xuanpolicy-0.1.6/xuanpolicy/mindspore/agents/multi_agent_rl/vdn_agents.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,64 +1,63 @@
-from xuanpolicy.xuanpolicy_ms.agents import *
-from xuanpolicy.xuanpolicy_ms.agents.agents_marl import linear_decay_or_increase
+from xuanpolicy.mindspore.agents import *
+from xuanpolicy.mindspore.agents.agents_marl import linear_decay_or_increase
 
 
-class QMIX_Agents(MARLAgents):
+class VDN_Agents(MARLAgents):
     def __init__(self,
                  config: Namespace,
                  envs: DummyVecEnv_MAS):
         self.comm = MPI.COMM_WORLD
 
         self.gamma = config.gamma
         self.use_obsnorm = config.use_obsnorm
         self.use_rewnorm = config.use_rewnorm
         self.obsnorm_range = config.obsnorm_range
         self.rewnorm_range = config.rewnorm_range
 
         self.start_greedy = config.start_greedy
         self.end_greedy = config.end_greedy
         self.egreedy = config.start_greedy
-        if config.state_space is not None:
-            config.dim_state, state_shape = config.state_space.shape, config.state_space.shape
-        else:
-            config.dim_state, state_shape = None, None
 
         input_representation = get_repre_in(config)
         representation = REGISTRY_Representation[config.representation](*input_representation)
-        mixer = QMIX_mixer(config.dim_state[0], config.hidden_dim_mixing_net, config.hidden_dim_hyper_net,
-                           config.n_agents)
+        mixer = VDN_mixer()
         input_policy = get_policy_in_marl(config, representation, config.agent_keys, mixer)
         policy = REGISTRY_Policy[config.policy](*input_policy)
 
         scheduler = lr_decay_model(learning_rate=config.learning_rate, decay_rate=0.5,
                                    decay_steps=get_total_iters(config.agent_name, config))
         optimizer = Adam(policy.trainable_params(), scheduler, eps=1e-5)
         self.observation_space = envs.observation_space
         self.action_space = envs.action_space
         self.representation_info_shape = policy.representation.output_shapes
         self.auxiliary_info_shape = {}
 
         writer = SummaryWriter(config.logdir)
+        if config.state_space is not None:
+            config.dim_state, state_shape = config.state_space.shape, config.state_space.shape
+        else:
+            config.dim_state, state_shape = None, None
         memory = MARL_OffPolicyBuffer(state_shape,
                                       config.obs_shape,
                                       config.act_shape,
                                       config.rew_shape,
                                       config.done_shape,
                                       envs.num_envs,
                                       config.buffer_size,
                                       config.batch_size)
-        learner = QMIX_Learner(config, policy, optimizer, scheduler, writer,
-                               config.modeldir, config.gamma, config.sync_frequency)
+        learner = VDN_Learner(config, policy, optimizer, scheduler, writer,
+                              config.modeldir, config.gamma, config.sync_frequency)
 
         self.obs_rms = RunningMeanStd(shape=space2shape(self.observation_space[config.agent_keys[0]]),
                                       comm=self.comm, use_mpi=False)
         self.ret_rms = RunningMeanStd(shape=(), comm=self.comm, use_mpi=False)
         self.epsilon_decay = linear_decay_or_increase(config.start_greedy, config.end_greedy,
                                                       config.greedy_update_steps)
-        super(QMIX_Agents, self).__init__(config, envs, policy, memory, learner, writer, config.logdir, config.modeldir)
+        super(VDN_Agents, self).__init__(config, envs, policy, memory, learner, writer, config.logdir, config.modeldir)
 
     def _process_observation(self, observations):
         if self.use_obsnorm:
             if isinstance(self.observation_space, Dict):
                 for key in self.observation_space.spaces.keys():
                     observations[key] = np.clip(
                         (observations[key] - self.obs_rms.mean[key]) / (self.obs_rms.std[key] + EPS),
```

### Comparing `xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_ms/agents/multi_agent_rl/qtran_agents.py` & `xuanpolicy-0.1.6/xuanpolicy/mindspore/agents/multi_agent_rl/qtran_agents.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-from xuanpolicy.xuanpolicy_ms.agents import *
-from xuanpolicy.xuanpolicy_ms.agents.agents_marl import linear_decay_or_increase
+from xuanpolicy.mindspore.agents import *
+from xuanpolicy.mindspore.agents.agents_marl import linear_decay_or_increase
 
 
 class QTRAN_Agents(MARLAgents):
     def __init__(self,
                  config: Namespace,
                  envs: DummyVecEnv_MAS):
         self.comm = MPI.COMM_WORLD
```

### Comparing `xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_ms/agents/multi_agent_rl/vdac_agents.py` & `xuanpolicy-0.1.6/xuanpolicy/mindspore/agents/multi_agent_rl/vdac_agents.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from xuanpolicy.xuanpolicy_ms.agents import *
+from xuanpolicy.mindspore.agents import *
 
 
 class VDAC_Agents(MARLAgents):
     def __init__(self,
                  config: Namespace,
                  envs: DummyVecEnv_MAS):
         self.comm = MPI.COMM_WORLD
```

### Comparing `xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_ms/agents/multi_agent_rl/vdn_agents.py` & `xuanpolicy-0.1.6/xuanpolicy/tensorflow/agents/multi_agent_rl/qmix_agents.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,63 +1,68 @@
-from xuanpolicy.xuanpolicy_ms.agents import *
-from xuanpolicy.xuanpolicy_ms.agents.agents_marl import linear_decay_or_increase
+from xuanpolicy.tensorflow.agents import *
+from xuanpolicy.tensorflow.agents.agents_marl import linear_decay_or_increase
 
 
-class VDN_Agents(MARLAgents):
+class QMIX_Agents(MARLAgents):
     def __init__(self,
                  config: Namespace,
-                 envs: DummyVecEnv_MAS):
+                 envs: DummyVecEnv_MAS,
+                 device: str = "cpu:0"):
         self.comm = MPI.COMM_WORLD
 
         self.gamma = config.gamma
         self.use_obsnorm = config.use_obsnorm
         self.use_rewnorm = config.use_rewnorm
         self.obsnorm_range = config.obsnorm_range
         self.rewnorm_range = config.rewnorm_range
 
         self.start_greedy = config.start_greedy
         self.end_greedy = config.end_greedy
         self.egreedy = config.start_greedy
+        if config.state_space is not None:
+            config.dim_state, state_shape = config.state_space.shape, config.state_space.shape
+        else:
+            config.dim_state, state_shape = None, None
 
         input_representation = get_repre_in(config)
         representation = REGISTRY_Representation[config.representation](*input_representation)
-        mixer = VDN_mixer()
+        mixer = QMIX_mixer(config.dim_state[0], config.hidden_dim_mixing_net, config.hidden_dim_hyper_net,
+                           config.n_agents)
         input_policy = get_policy_in_marl(config, representation, config.agent_keys, mixer)
         policy = REGISTRY_Policy[config.policy](*input_policy)
-
-        scheduler = lr_decay_model(learning_rate=config.learning_rate, decay_rate=0.5,
-                                   decay_steps=get_total_iters(config.agent_name, config))
-        optimizer = Adam(policy.trainable_params(), scheduler, eps=1e-5)
+        # lr_scheduler = tk.optimizers.schedules.ExponentialDecay(config.learning_rate, decay_steps=1000,
+        #                                                         decay_rate=0.9)
+        lr_scheduler = MyLinearLR(config.learning_rate, start_factor=1.0, end_factor=0.5,
+                                  total_iters=get_total_iters(config.agent_name, config))
+        optimizer = tk.optimizers.Adam(lr_scheduler)
         self.observation_space = envs.observation_space
         self.action_space = envs.action_space
         self.representation_info_shape = policy.representation.output_shapes
         self.auxiliary_info_shape = {}
 
         writer = SummaryWriter(config.logdir)
-        if config.state_space is not None:
-            config.dim_state, state_shape = config.state_space.shape, config.state_space.shape
-        else:
-            config.dim_state, state_shape = None, None
         memory = MARL_OffPolicyBuffer(state_shape,
                                       config.obs_shape,
                                       config.act_shape,
                                       config.rew_shape,
                                       config.done_shape,
                                       envs.num_envs,
                                       config.buffer_size,
                                       config.batch_size)
-        learner = VDN_Learner(config, policy, optimizer, scheduler, writer,
-                              config.modeldir, config.gamma, config.sync_frequency)
+        learner = QMIX_Learner(config, policy, optimizer, writer,
+                               config.device, config.modeldir, config.gamma,
+                               config.sync_frequency)
 
         self.obs_rms = RunningMeanStd(shape=space2shape(self.observation_space[config.agent_keys[0]]),
                                       comm=self.comm, use_mpi=False)
         self.ret_rms = RunningMeanStd(shape=(), comm=self.comm, use_mpi=False)
         self.epsilon_decay = linear_decay_or_increase(config.start_greedy, config.end_greedy,
                                                       config.greedy_update_steps)
-        super(VDN_Agents, self).__init__(config, envs, policy, memory, learner, writer, config.logdir, config.modeldir)
+        super(QMIX_Agents, self).__init__(config, envs, policy, memory, learner, writer, device,
+                                          config.logdir, config.modeldir)
 
     def _process_observation(self, observations):
         if self.use_obsnorm:
             if isinstance(self.observation_space, Dict):
                 for key in self.observation_space.spaces.keys():
                     observations[key] = np.clip(
                         (observations[key] - self.obs_rms.mean[key]) / (self.obs_rms.std[key] + EPS),
```

### Comparing `xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_ms/agents/multi_agent_rl/wqmix_agents.py` & `xuanpolicy-0.1.6/xuanpolicy/mindspore/agents/multi_agent_rl/wqmix_agents.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-from xuanpolicy.xuanpolicy_ms.agents import *
-from xuanpolicy.xuanpolicy_ms.agents.agents_marl import linear_decay_or_increase
+from xuanpolicy.mindspore.agents import *
+from xuanpolicy.mindspore.agents.agents_marl import linear_decay_or_increase
 
 
 class WQMIX_Agents(MARLAgents):
     def __init__(self,
                  config: Namespace,
                  envs: DummyVecEnv_MAS):
         self.comm = MPI.COMM_WORLD
```

### Comparing `xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_ms/agents/policy_gradient/a2c_agent.py` & `xuanpolicy-0.1.6/xuanpolicy/mindspore/agents/policy_gradient/a2c_agent.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from xuanpolicy.xuanpolicy_ms.agents import *
+from xuanpolicy.mindspore.agents import *
 
 
 class A2C_Agent(Agent):
     def __init__(self,
                  config: Namespace,
                  envs: VecEnv,
                  policy: nn.Cell,
```

### Comparing `xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_ms/agents/policy_gradient/ddpg_agent.py` & `xuanpolicy-0.1.6/xuanpolicy/mindspore/agents/policy_gradient/ddpg_agent.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from xuanpolicy.xuanpolicy_ms.agents import *
+from xuanpolicy.mindspore.agents import *
 
 
 class DDPG_Agent(Agent):
     def __init__(self,
                  config: Namespace,
                  envs: VecEnv,
                  policy: nn.Cell,
```

### Comparing `xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_ms/agents/policy_gradient/mpdqn_agent.py` & `xuanpolicy-0.1.6/xuanpolicy/mindspore/agents/policy_gradient/mpdqn_agent.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from xuanpolicy.xuanpolicy_ms.agents import *
+from xuanpolicy.mindspore.agents import *
 import gym
 from gym import spaces
 
 class MPDQN_Agent(Agent):
     def __init__(self,
                  config: Namespace,
                  envs: Toy_Env,
```

### Comparing `xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_ms/agents/policy_gradient/pdqn_agent.py` & `xuanpolicy-0.1.6/xuanpolicy/mindspore/agents/policy_gradient/pdqn_agent.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from xuanpolicy.xuanpolicy_ms.agents import *
+from xuanpolicy.mindspore.agents import *
 import gym
 from gym import spaces
 
 class PDQN_Agent(Agent):
     def __init__(self,
                  config: Namespace,
                  envs: Toy_Env,
```

### Comparing `xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_ms/agents/policy_gradient/pg_agent.py` & `xuanpolicy-0.1.6/xuanpolicy/mindspore/agents/policy_gradient/pg_agent.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from xuanpolicy.xuanpolicy_ms.agents import *
+from xuanpolicy.mindspore.agents import *
 
 
 class PG_Agent(Agent):
     def __init__(self,
                  config: Namespace,
                  envs: VecEnv,
                  policy: nn.Cell,
```

### Comparing `xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_ms/agents/policy_gradient/ppg_agent.py` & `xuanpolicy-0.1.6/xuanpolicy/tensorflow/agents/policy_gradient/ppg_agent.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,27 +1,26 @@
-from xuanpolicy.xuanpolicy_ms.agents import *
-from xuanpolicy.xuanpolicy_ms.utils.distributions import CategoricalDistribution
+from xuanpolicy.tensorflow.agents import *
 
 
 class PPG_Agent(Agent):
     def __init__(self,
                  config: Namespace,
                  envs: VecEnv,
-                 policy: nn.Cell,
-                 optimizer: nn.Optimizer,
-                 scheduler):
+                 policy: tk.Model,
+                 optimizer: tk.optimizers.Optimizer,
+                 device: str = 'cpu'):
         self.config = config
+        self.render = config.render
         self.comm = MPI.COMM_WORLD
         self.nenvs = envs.num_envs
         self.nsteps = config.nsteps
         self.nminibatch = config.nminibatch
         self.policy_nepoch = config.policy_nepoch
         self.value_nepoch = config.value_nepoch
         self.aux_nepoch = config.aux_nepoch
-        self.render = config.render
 
         self.gamma = config.gamma
         self.lam = config.lam
         self.use_obsnorm = config.use_obsnorm
         self.use_rewnorm = config.use_rewnorm
         self.obsnorm_range = config.obsnorm_range
         self.rewnorm_range = config.rewnorm_range
@@ -38,25 +37,26 @@
                                      self.auxiliary_info_shape,
                                      self.nenvs,
                                      self.nsteps,
                                      self.nminibatch,
                                      self.gamma,
                                      self.lam)
         learner = PPG_Learner(policy,
-                             optimizer,
-                             scheduler,
-                             writer,
-                             config.modeldir,
-                             config.ent_coef,
-                             config.clip_range,
-                             config.kl_beta)
+                              optimizer,
+                              writer,
+                              config.device,
+                              config.modeldir,
+                              config.ent_coef,
+                              config.clip_range,
+                              config.kl_beta)
 
         self.obs_rms = RunningMeanStd(shape=space2shape(self.observation_space), comm=self.comm, use_mpi=False)
         self.ret_rms = RunningMeanStd(shape=(), comm=self.comm, use_mpi=False)
-        super(PPG_Agent, self).__init__(envs, policy, memory, learner, writer, config.logdir, config.modeldir)
+        super(PPG_Agent, self).__init__(envs, policy, memory, learner, writer, device, config.logdir,
+                                        config.modeldir)
 
     def _process_observation(self, observations):
         if self.use_obsnorm:
             if isinstance(self.observation_space, Dict):
                 for key in self.observation_space.spaces.keys():
                     observations[key] = np.clip(
                         (observations[key] - self.obs_rms.mean[key]) / (self.obs_rms.std[key] + EPS),
@@ -70,28 +70,24 @@
     def _process_reward(self, rewards):
         if self.use_rewnorm:
             std = np.clip(self.ret_rms.std, 0.1, 100)
             return np.clip(rewards / std, -self.rewnorm_range, self.rewnorm_range)
         return rewards
 
     def _action(self, obs):
-        states, act_probs, vs, _ = self.policy(ms.Tensor(obs))
-        # acts = self.policy.actor.sample(act_probs).asnumpy()
-        dists = CategoricalDistribution(self.action_space.n)
-        dists.set_param(act_probs)
-        acts = dists.stochastic_sample().asnumpy()
-        vs = vs.asnumpy()
-        if context._get_mode() == 0:
-            return {"state": states[0].asnumpy()}, acts, vs, split_distributions(dists)
-        else:
-            for key in states.keys():
-                states[key] = states[key].asnumpy()
-            return states, acts, vs, split_distributions(dists)
+        states, _, vs, _ = self.policy(obs)
+        dists = self.policy.actor.dist
+        acts = dists.stochastic_sample()
+        for key in states.keys():
+            states[key] = states[key].numpy()
+        vs = vs.numpy()
+        acts = acts.numpy()
+        return states, acts, vs, split_distributions(dists)
 
-    def train(self, train_steps=10000, load_model=None):
+    def train(self, train_steps=10000):
         episodes = np.zeros((self.nenvs,), np.int32)
         scores = np.zeros((self.nenvs,), np.float32)
         returns = np.zeros((self.nenvs,), np.float32)
 
         obs = self.envs.reset()
         for step in tqdm(range(train_steps)):
             self.obs_rms.update(obs)
@@ -99,37 +95,35 @@
             states, acts, rets, dists = self._action(obs)
             next_obs, rewards, dones, infos = self.envs.step(acts)
             if self.render: self.envs.render()
             self.memory.store(obs, acts, self._process_reward(rewards), rets, dones, states, {"old_dist": dists})
             if self.memory.full:
                 _, _, vals, _ = self._action(self._process_observation(next_obs))
                 for i in range(self.nenvs):
-                    self.memory.finish_path(rewards[i], i)
-                
+                    self.memory.finish_path(vals[i], i)
                 # policy update
-                # update_type: 0-policy_update, 1-critic_update, 2-auxiliary_update
                 for _ in range(self.nminibatch * self.policy_nepoch):
                     obs_batch, act_batch, ret_batch, adv_batch, _, aux_batch = self.memory.sample()
-                    self.learner.update(obs_batch, act_batch, ret_batch, adv_batch, aux_batch['old_dist'], 0)
+                    self.learner.update_policy(obs_batch, act_batch, ret_batch, adv_batch, aux_batch['old_dist'])
                 # critic update
                 for _ in range(self.nminibatch * self.value_nepoch):
                     obs_batch, act_batch, ret_batch, adv_batch, _, aux_batch = self.memory.sample()
-                    self.learner.update(obs_batch, act_batch, ret_batch, adv_batch, aux_batch['old_dist'], 1)
-                    
+                    self.learner.update_critic(obs_batch, act_batch, ret_batch, adv_batch, aux_batch['old_dist'])
+
                 # update old_prob
-                buffer_obs = self.memory.observations
+                buffer_obs_shape = self.memory.observations.shape
+                buffer_obs = self.memory.observations.reshape([-1, buffer_obs_shape[-1]])
                 buffer_act = self.memory.actions
-                _,new_dists,_,_ = self.policy(ms.Tensor(buffer_obs))
-                new_dist = CategoricalDistribution(self.action_space.n)
-                new_dist.set_param(new_dists)
+                _, new_logits, _, _ = self.policy(buffer_obs)
+                self.policy.actor.dist.set_param(tf.reshape(new_logits, buffer_obs_shape[0:-1]+(-1, )))
+                new_dist = self.policy.actor.dist
                 self.memory.auxiliary_infos['old_dist'] = split_distributions(new_dist)
                 for _ in range(self.nminibatch * self.aux_nepoch):
                     obs_batch, act_batch, ret_batch, adv_batch, _, aux_batch = self.memory.sample()
-                    self.learner.update(obs_batch, act_batch, ret_batch, adv_batch, aux_batch['old_dist'], 2)
-                
+                    self.learner.update_auxiliary(obs_batch, act_batch, ret_batch, adv_batch, aux_batch['old_dist'])
                 self.memory.clear()
             scores += rewards
             returns = self.gamma * returns + rewards
             obs = next_obs
             for i in range(self.nenvs):
                 if dones[i] == True:
                     self.ret_rms.update(returns[i:i + 1])
@@ -159,10 +153,10 @@
             self.envs.render()
             scores += rewards
             returns = self.gamma * returns + rewards
             obs = next_obs
             for i in range(self.nenvs):
                 if dones[i] == True:
                     scores[i], returns[i] = 0, 0
-    
+
     def evaluate(self):
         pass
```

### Comparing `xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_ms/agents/policy_gradient/ppoclip_agent.py` & `xuanpolicy-0.1.6/xuanpolicy/mindspore/agents/policy_gradient/ppokl_agent.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-from xuanpolicy.xuanpolicy_ms.agents import *
+from xuanpolicy.mindspore.agents import *
 
 
-class PPOCLIP_Agent(Agent):
+class PPOKL_Agent(Agent):
     def __init__(self,
                  config: Namespace,
                  envs: VecEnv,
                  policy: nn.Cell,
                  optimizer: nn.Optimizer,
                  scheduler: Optional[nn.exponential_decay_lr] = None):
         self.config = config
@@ -41,20 +41,20 @@
         learner = PPOCLIP_Learner(policy,
                                   optimizer,
                                   scheduler,
                                   writer,
                                   config.modeldir,
                                   config.vf_coef,
                                   config.ent_coef,
-                                  config.clip_range)
+                                  0.2)
 
         self.obs_rms = RunningMeanStd(shape=space2shape(self.observation_space), comm=self.comm, use_mpi=False)
         self.ret_rms = RunningMeanStd(shape=(), comm=self.comm, use_mpi=False)
-        super(PPOCLIP_Agent, self).__init__(envs, policy, memory, learner, writer, config.logdir,
-                                            config.modeldir)
+        super(PPOKL_Agent, self).__init__(envs, policy, memory, learner, writer, config.logdir,
+                                          config.modeldir)
 
     def _process_observation(self, observations):
         if self.use_obsnorm:
             if isinstance(self.observation_space, Dict):
                 for key in self.observation_space.spaces.keys():
                     observations[key] = np.clip(
                         (observations[key] - self.obs_rms.mean[key]) / (self.obs_rms.std[key] + EPS),
```

### Comparing `xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_ms/agents/policy_gradient/ppokl_agent.py` & `xuanpolicy-0.1.6/xuanpolicy/mindspore/agents/policy_gradient/ppoclip_agent.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-from xuanpolicy.xuanpolicy_ms.agents import *
+from xuanpolicy.mindspore.agents import *
 
 
-class PPOKL_Agent(Agent):
+class PPOCLIP_Agent(Agent):
     def __init__(self,
                  config: Namespace,
                  envs: VecEnv,
                  policy: nn.Cell,
                  optimizer: nn.Optimizer,
                  scheduler: Optional[nn.exponential_decay_lr] = None):
         self.config = config
@@ -41,20 +41,20 @@
         learner = PPOCLIP_Learner(policy,
                                   optimizer,
                                   scheduler,
                                   writer,
                                   config.modeldir,
                                   config.vf_coef,
                                   config.ent_coef,
-                                  0.2)
+                                  config.clip_range)
 
         self.obs_rms = RunningMeanStd(shape=space2shape(self.observation_space), comm=self.comm, use_mpi=False)
         self.ret_rms = RunningMeanStd(shape=(), comm=self.comm, use_mpi=False)
-        super(PPOKL_Agent, self).__init__(envs, policy, memory, learner, writer, config.logdir,
-                                          config.modeldir)
+        super(PPOCLIP_Agent, self).__init__(envs, policy, memory, learner, writer, config.logdir,
+                                            config.modeldir)
 
     def _process_observation(self, observations):
         if self.use_obsnorm:
             if isinstance(self.observation_space, Dict):
                 for key in self.observation_space.spaces.keys():
                     observations[key] = np.clip(
                         (observations[key] - self.obs_rms.mean[key]) / (self.obs_rms.std[key] + EPS),
```

### Comparing `xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_ms/agents/policy_gradient/sac_agent.py` & `xuanpolicy-0.1.6/xuanpolicy/mindspore/agents/policy_gradient/sac_agent.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from xuanpolicy.xuanpolicy_ms.agents import *
+from xuanpolicy.mindspore.agents import *
 
 
 class SAC_Agent(Agent):
     def __init__(self,
                  config: Namespace,
                  envs: VecEnv,
                  policy: nn.Cell,
```

### Comparing `xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_ms/agents/policy_gradient/sacdis_agent.py` & `xuanpolicy-0.1.6/xuanpolicy/mindspore/agents/policy_gradient/sacdis_agent.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-from xuanpolicy.xuanpolicy_ms.agents import *
-from xuanpolicy.xuanpolicy_ms.utils.distributions import CategoricalDistribution
+from xuanpolicy.mindspore.agents import *
+from xuanpolicy.mindspore.utils.distributions import CategoricalDistribution
 
 
 class SACDIS_Agent(Agent):
     def __init__(self,
                  config: Namespace,
                  envs: VecEnv,
                  policy: nn.Cell,
```

### Comparing `xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_ms/agents/policy_gradient/spdqn_agent.py` & `xuanpolicy-0.1.6/xuanpolicy/mindspore/agents/policy_gradient/spdqn_agent.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from xuanpolicy.xuanpolicy_ms.agents import *
+from xuanpolicy.mindspore.agents import *
 import gym
 from gym import spaces
 
 class SPDQN_Agent(Agent):
     def __init__(self,
                  config: Namespace,
                  envs: Toy_Env,
```

### Comparing `xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_ms/agents/policy_gradient/td3_agent.py` & `xuanpolicy-0.1.6/xuanpolicy/mindspore/agents/policy_gradient/td3_agent.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from xuanpolicy.xuanpolicy_ms.agents import *
+from xuanpolicy.mindspore.agents import *
 
 
 class TD3_Agent(Agent):
     def __init__(self,
                  config: Namespace,
                  envs: VecEnv,
                  policy: nn.Cell,
```

### Comparing `xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_ms/agents/qlearning_family/C51_agent.py` & `xuanpolicy-0.1.6/xuanpolicy/mindspore/agents/qlearning_family/C51_agent.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from xuanpolicy.xuanpolicy_ms.agents import *
+from xuanpolicy.mindspore.agents import *
 
 
 class C51_Agent(Agent):
     def __init__(self,
                  config: Namespace,
                  envs: VecEnv,
                  policy: nn.Cell,
```

### Comparing `xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_ms/agents/qlearning_family/cdqn_agent.py` & `xuanpolicy-0.1.6/xuanpolicy/mindspore/agents/qlearning_family/cdqn_agent.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from xuanpolicy.xuanpolicy_ms.agents import *
+from xuanpolicy.mindspore.agents import *
 
 
 class CDQN_Agent(Agent):
     def __init__(self,
                  config: Namespace,
                  envs: VecEnv,
                  policy: nn.Cell,
```

### Comparing `xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_ms/agents/qlearning_family/cldqn_agent.py` & `xuanpolicy-0.1.6/xuanpolicy/mindspore/agents/qlearning_family/cldqn_agent.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from xuanpolicy.xuanpolicy_ms.agents import *
+from xuanpolicy.mindspore.agents import *
 
 
 class CLDQN_Agent(Agent):
     def __init__(self,
                  config: Namespace,
                  envs: VecEnv,
                  policy: nn.Cell,
```

### Comparing `xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_ms/agents/qlearning_family/ddqn_agent.py` & `xuanpolicy-0.1.6/xuanpolicy/mindspore/agents/qlearning_family/ddqn_agent.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from xuanpolicy.xuanpolicy_ms.agents import *
+from xuanpolicy.mindspore.agents import *
 
 
 class DDQN_Agent(Agent):
     def __init__(self,
                  config: Namespace,
                  envs: VecEnv,
                  policy: nn.Cell,
```

### Comparing `xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_ms/agents/qlearning_family/dqn_agent.py` & `xuanpolicy-0.1.6/xuanpolicy/mindspore/agents/qlearning_family/dqn_agent.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from xuanpolicy.xuanpolicy_ms.agents import *
+from xuanpolicy.mindspore.agents import *
 
 
 class DQN_Agent(Agent):
     def __init__(self,
                  config: Namespace,
                  envs: VecEnv,
                  policy: nn.Cell,
```

### Comparing `xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_ms/agents/qlearning_family/dueldqn_agent.py` & `xuanpolicy-0.1.6/xuanpolicy/mindspore/agents/qlearning_family/dueldqn_agent.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from xuanpolicy.xuanpolicy_ms.agents import *
+from xuanpolicy.mindspore.agents import *
 
 
 class DuelDQN_Agent(Agent):
     def __init__(self,
                  config: Namespace,
                  envs: VecEnv,
                  policy: nn.Cell,
```

### Comparing `xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_ms/agents/qlearning_family/ldqn_agent.py` & `xuanpolicy-0.1.6/xuanpolicy/mindspore/agents/qlearning_family/ldqn_agent.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from xuanpolicy.xuanpolicy_ms.agents import *
+from xuanpolicy.mindspore.agents import *
 
 
 class LDQN_Agent(Agent):
     def __init__(self,
                  config: Namespace,
                  envs: VecEnv,
                  policy: nn.Cell,
```

### Comparing `xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_ms/agents/qlearning_family/noisydqn_agent.py` & `xuanpolicy-0.1.6/xuanpolicy/mindspore/agents/qlearning_family/noisydqn_agent.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from xuanpolicy.xuanpolicy_ms.agents import *
+from xuanpolicy.mindspore.agents import *
 
 
 class NoisyDQN_Agent(Agent):
     def __init__(self,
                  config: Namespace,
                  envs: VecEnv,
                  policy: nn.Cell,
```

### Comparing `xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_ms/agents/qlearning_family/perdqn_agent.py` & `xuanpolicy-0.1.6/xuanpolicy/mindspore/agents/qlearning_family/perdqn_agent.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from xuanpolicy.xuanpolicy_ms.agents import *
+from xuanpolicy.mindspore.agents import *
 
 
 class PerDQN_Agent(Agent):
     def __init__(self,
                  config: Namespace,
                  envs: VecEnv,
                  policy: nn.Cell,
```

### Comparing `xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_ms/agents/qlearning_family/qrdqn_agent.py` & `xuanpolicy-0.1.6/xuanpolicy/mindspore/agents/qlearning_family/qrdqn_agent.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from xuanpolicy.xuanpolicy_ms.agents import *
+from xuanpolicy.mindspore.agents import *
 
 
 class QRDQN_Agent(Agent):
     def __init__(self,
                  config: Namespace,
                  envs: VecEnv,
                  policy: nn.Cell,
```

### Comparing `xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_ms/learners/__init__.py` & `xuanpolicy-0.1.6/xuanpolicy/mindspore/learners/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import mindspore as ms
 import mindspore.nn as nn
 import numpy as np
 from typing import Sequence, Optional, Callable, Union
 from gym.spaces import Space, Box, Discrete, Dict
 from torch.utils.tensorboard import SummaryWriter
-from xuanpolicy.xuanpolicy_ms.utils.set_trainer import *
+from xuanpolicy.mindspore.utils.set_trainer import *
 from argparse import Namespace
 from mindspore import Tensor
 from mindspore.ops import OneHot, GatherD
 import mindspore.ops as ops
 
 from .learner import Learner, LearnerMAS
 from .policy_gradient.pg_learner import PG_Learner
```

### Comparing `xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_ms/learners/learner.py` & `xuanpolicy-0.1.6/xuanpolicy/mindspore/learners/learner.py`

 * *Files identical despite different names*

### Comparing `xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_ms/learners/multi_agent_rl/coma_learner.py` & `xuanpolicy-0.1.6/xuanpolicy/mindspore/learners/multi_agent_rl/coma_learner.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
 COMA: Counterfactual Multi-Agent Policy Gradients
 Paper link: https://ojs.aaai.org/index.php/AAAI/article/view/11794
 Implementation: MindSpore
 """
-from xuanpolicy.xuanpolicy_ms.learners import *
+from xuanpolicy.mindspore.learners import *
 
 
 class COMA_Learner(LearnerMAS):
     class ActorNetWithLossCell(nn.Cell):
         def __init__(self, backbone, n_agents):
             super(COMA_Learner.ActorNetWithLossCell, self).__init__()
             self._backbone = backbone
```

### Comparing `xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_ms/learners/multi_agent_rl/dcg_learner.py` & `xuanpolicy-0.1.6/xuanpolicy/mindspore/learners/multi_agent_rl/dcg_learner.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
 DCG: Deep coordination graphs
 Paper link: http://proceedings.mlr.press/v119/boehmer20a/boehmer20a.pdf
 Implementation: MindSpore
 """
-from xuanpolicy.xuanpolicy_ms.learners import *
+from xuanpolicy.mindspore.learners import *
 import torch_scatter
 import torch
 import copy
 
 
 class DCG_Learner(LearnerMAS):
     class PolicyNetWithLossCell(nn.Cell):
```

### Comparing `xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_ms/learners/multi_agent_rl/iddpg_learner.py` & `xuanpolicy-0.1.6/xuanpolicy/mindspore/learners/multi_agent_rl/iddpg_learner.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
 Independent Deep Deterministic Policy Gradient (IDDPG)
 Implementation: MindSpore
 """
-from xuanpolicy.xuanpolicy_ms.learners import *
+from xuanpolicy.mindspore.learners import *
 
 
 class IDDPG_Learner(LearnerMAS):
     class ActorNetWithLossCell(nn.Cell):
         def __init__(self, backbone):
             super(IDDPG_Learner.ActorNetWithLossCell, self).__init__()
             self._backbone = backbone
```

### Comparing `xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_ms/learners/multi_agent_rl/iql_learner.py` & `xuanpolicy-0.1.6/xuanpolicy/mindspore/learners/multi_agent_rl/iql_learner.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
 Independent Q-learning (IQL)
 Implementation: MindSpore
 """
-from xuanpolicy.xuanpolicy_ms.learners import *
+from xuanpolicy.mindspore.learners import *
 
 
 class IQL_Learner(LearnerMAS):
     class PolicyNetWithLossCell(nn.Cell):
         def __init__(self, backbone):
             super(IQL_Learner.PolicyNetWithLossCell, self).__init__(auto_prefix=False)
             self._backbone = backbone
```

### Comparing `xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_ms/learners/multi_agent_rl/isac_learner.py` & `xuanpolicy-0.1.6/xuanpolicy/mindspore/learners/multi_agent_rl/isac_learner.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
 Independent Soft Actor-critic (ISAC)
 Implementation: Pytorch
 Creator: Kun Jiang (kjiang@seu.edu.cn)
 """
-from xuanpolicy.xuanpolicy_ms.learners import *
+from xuanpolicy.mindspore.learners import *
 
 
 class ISAC_Learner(LearnerMAS):
     class ActorNetWithLossCell(nn.Cell):
         def __init__(self, backbone, n_agents, alpha):
             super(ISAC_Learner.ActorNetWithLossCell, self).__init__()
             self._backbone = backbone
```

### Comparing `xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_ms/learners/multi_agent_rl/maddpg_learner.py` & `xuanpolicy-0.1.6/xuanpolicy/mindspore/learners/multi_agent_rl/maddpg_learner.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """
 Multi-Agent Deep Deterministic Policy Gradient
 Paper link:
 https://proceedings.neurips.cc/paper/2017/file/68a9750337a418a86fe06c1991a1d64c-Paper.pdf
 Implementation: MindSpore
 Trick: Parameter sharing for all agents, with agents' one-hot IDs as actor-critic's inputs.
 """
-from xuanpolicy.xuanpolicy_ms.learners import *
+from xuanpolicy.mindspore.learners import *
 
 
 class MADDPG_Learner(LearnerMAS):
     class ActorNetWithLossCell(nn.Cell):
         def __init__(self, backbone, n_agents):
             super(MADDPG_Learner.ActorNetWithLossCell, self).__init__()
             self._backbone = backbone
```

### Comparing `xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_ms/learners/multi_agent_rl/mappoclip_learner.py` & `xuanpolicy-0.1.6/xuanpolicy/mindspore/learners/multi_agent_rl/mappoclip_learner.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """
 Multi-Agent Proximal Policy Optimization (MAPPO)
 Paper link:
 https://arxiv.org/pdf/2103.01955.pdf
 Implementation: MindSpore
 """
-from xuanpolicy.xuanpolicy_ms.learners import *
+from xuanpolicy.mindspore.learners import *
 
 
 class MAPPO_Clip_Learner(LearnerMAS):
     class PolicyNetWithLossCell(nn.Cell):
         def __init__(self, backbone, n_agents, vf_coef, ent_coef, clip_range, use_value_clip, value_clip_range):
             super(MAPPO_Clip_Learner.PolicyNetWithLossCell, self).__init__()
             self._backbone = backbone
```

### Comparing `xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_ms/learners/multi_agent_rl/mappokl_learner.py` & `xuanpolicy-0.1.6/xuanpolicy/mindspore/learners/multi_agent_rl/mappokl_learner.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """
 Multi-Agent Proximal Policy Optimization (MAPPO)
 Paper link:
 https://arxiv.org/pdf/2103.01955.pdf
 Implementation: MindSpore
 """
-from xuanpolicy.xuanpolicy_ms.learners import *
+from xuanpolicy.mindspore.learners import *
 
 
 class MAPPO_KL_Learner(LearnerMAS):
     class PolicyNetWithLossCell(nn.Cell):
         def __init__(self, backbone, n_agents, vf_coef, ent_coef, clip_range, use_value_clip, value_clip_range, target_kl):
             super(MAPPO_KL_Learner.PolicyNetWithLossCell, self).__init__()
             self._backbone = backbone
```

### Comparing `xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_ms/learners/multi_agent_rl/masac_learner.py` & `xuanpolicy-0.1.6/xuanpolicy/mindspore/learners/multi_agent_rl/masac_learner.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
 Multi-agent Soft Actor-critic (MASAC)
 Implementation: Pytorch
 Creator: Kun Jiang (kjiang@seu.edu.cn)
 """
-from xuanpolicy.xuanpolicy_ms.learners import *
+from xuanpolicy.mindspore.learners import *
 
 
 class MASAC_Learner(LearnerMAS):
     class ActorNetWithLossCell(nn.Cell):
         def __init__(self, backbone, n_agents, alpha):
             super(MASAC_Learner.ActorNetWithLossCell, self).__init__()
             self._backbone = backbone
```

### Comparing `xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_ms/learners/multi_agent_rl/matd3_learner.py` & `xuanpolicy-0.1.6/xuanpolicy/mindspore/learners/multi_agent_rl/matd3_learner.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
 Multi-Agent TD3
 
 """
-from xuanpolicy.xuanpolicy_ms.learners import *
+from xuanpolicy.mindspore.learners import *
 
 
 class MATD3_Learner(LearnerMAS):
     class ActorNetWithLossCell(nn.Cell):
         def __init__(self, backbone, n_agents):
             super(MATD3_Learner.ActorNetWithLossCell, self).__init__()
             self._backbone = backbone
```

### Comparing `xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_ms/learners/multi_agent_rl/mfac_learner.py` & `xuanpolicy-0.1.6/xuanpolicy/mindspore/learners/multi_agent_rl/mfac_learner.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """
 MFAC: Mean Field Actor-Critic
 Paper link:
 http://proceedings.mlr.press/v80/yang18d/yang18d.pdf
 Implementation: MindSpore
 """
-from xuanpolicy.xuanpolicy_ms.learners import *
+from xuanpolicy.mindspore.learners import *
 
 
 class MFAC_Learner(LearnerMAS):
     class ActorNetWithLossCell(nn.Cell):
         def __init__(self, backbone, n_agents, dim_act):
             super(MFAC_Learner.ActorNetWithLossCell, self).__init__()
             self._backbone = backbone
```

### Comparing `xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_ms/learners/multi_agent_rl/mfq_learner.py` & `xuanpolicy-0.1.6/xuanpolicy/mindspore/learners/multi_agent_rl/mfq_learner.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """
 MFQ: Mean Field Q-Learning
 Paper link:
 http://proceedings.mlr.press/v80/yang18d/yang18d.pdf
 Implementation: MindSpore
 """
-from xuanpolicy.xuanpolicy_ms.learners import *
+from xuanpolicy.mindspore.learners import *
 
 
 class MFQ_Learner(LearnerMAS):
     class PolicyNetWithLossCell(nn.Cell):
         def __init__(self, backbone, n_agents):
             super(MFQ_Learner.PolicyNetWithLossCell, self).__init__()
             self._backbone = backbone
```

### Comparing `xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_ms/learners/multi_agent_rl/qmix_learner.py` & `xuanpolicy-0.1.6/xuanpolicy/mindspore/learners/multi_agent_rl/qmix_learner.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """
 Qmix: Monotonic value function factorisation for deep multi-agent reinforcement learning
 Paper link:
 http://proceedings.mlr.press/v80/rashid18a/rashid18a.pdf
 Implementation: MindSpore
 """
-from xuanpolicy.xuanpolicy_ms.learners import *
+from xuanpolicy.mindspore.learners import *
 
 
 class QMIX_Learner(LearnerMAS):
     class PolicyNetWithLossCell(nn.Cell):
         def __init__(self, backbone):
             super(QMIX_Learner.PolicyNetWithLossCell, self).__init__(auto_prefix=False)
             self._backbone = backbone
```

### Comparing `xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_ms/learners/multi_agent_rl/qtran_learner.py` & `xuanpolicy-0.1.6/xuanpolicy/mindspore/learners/multi_agent_rl/qtran_learner.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """
 QTRAN: Learning to Factorize with Transformation for Cooperative Multi-Agent Reinforcement Learning
 Paper link:
 http://proceedings.mlr.press/v97/son19a/son19a.pdf
 Implementation: MindSpore
 """
-from xuanpolicy.xuanpolicy_ms.learners import *
+from xuanpolicy.mindspore.learners import *
 
 
 class QTRAN_Learner(LearnerMAS):
     class PolicyNetWithLossCell(nn.Cell):
         def __init__(self, backbone, dim_act, n_agents, agent_name, lambda_opt, lambda_nopt):
             super(QTRAN_Learner.PolicyNetWithLossCell, self).__init__(auto_prefix=False)
             self._backbone = backbone
```

### Comparing `xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_ms/learners/multi_agent_rl/vdac_learner.py` & `xuanpolicy-0.1.6/xuanpolicy/mindspore/learners/multi_agent_rl/vdac_learner.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
 Value Decomposition Actor-Critic (VDAC)
 Paper link: https://ojs.aaai.org/index.php/AAAI/article/view/17353
 Implementation: MindSpore
 """
-from xuanpolicy.xuanpolicy_ms.learners import *
+from xuanpolicy.mindspore.learners import *
 
 
 class VDAC_Learner(LearnerMAS):
     class PolicyNetWithLossCell(nn.Cell):
         def __init__(self, backbone, vf_coef, ent_coef):
             super(VDAC_Learner.PolicyNetWithLossCell, self).__init__()
             self._backbone = backbone
```

### Comparing `xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_ms/learners/multi_agent_rl/vdn_learner.py` & `xuanpolicy-0.1.6/xuanpolicy/mindspore/learners/multi_agent_rl/vdn_learner.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """
 Value Decomposition Networks (VDN)
 Paper link:
 https://arxiv.org/pdf/1706.05296.pdf
 Implementation: MindSpore
 """
-from xuanpolicy.xuanpolicy_ms.learners import *
+from xuanpolicy.mindspore.learners import *
 
 
 class VDN_Learner(LearnerMAS):
     class PolicyNetWithLossCell(nn.Cell):
         def __init__(self, backbone):
             super(VDN_Learner.PolicyNetWithLossCell, self).__init__(auto_prefix=False)
             self._backbone = backbone
```

### Comparing `xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_ms/learners/multi_agent_rl/wqmix_learner.py` & `xuanpolicy-0.1.6/xuanpolicy/mindspore/learners/multi_agent_rl/wqmix_learner.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """
 Weighted QMIX
 Paper link:
 https://proceedings.neurips.cc/paper/2020/file/73a427badebe0e32caa2e1fc7530b7f3-Paper.pdf
 Implementation: MindSpore
 """
-from xuanpolicy.xuanpolicy_ms.learners import *
+from xuanpolicy.mindspore.learners import *
 
 
 class WQMIX_Learner(LearnerMAS):
     class PolicyNetWithLossCell(nn.Cell):
         def __init__(self, backbone, n_agent, agent_name, alpha):
             super(WQMIX_Learner.PolicyNetWithLossCell, self).__init__(auto_prefix=False)
             self.n_agent = n_agent
```

### Comparing `xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_ms/learners/policy_gradient/a2c_learner.py` & `xuanpolicy-0.1.6/xuanpolicy/mindspore/learners/policy_gradient/a2c_learner.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from xuanpolicy.xuanpolicy_ms.learners import *
+from xuanpolicy.mindspore.learners import *
 
 
 class A2C_Learner(Learner):
     class ACNetWithLossCell(nn.Cell):
         def __init__(self, backbone, ent_coef, vf_coef):
             super(A2C_Learner.ACNetWithLossCell, self).__init__()
             self._backbone = backbone
```

### Comparing `xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_ms/learners/policy_gradient/ddpg_learner.py` & `xuanpolicy-0.1.6/xuanpolicy/mindspore/learners/policy_gradient/ddpg_learner.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from xuanpolicy.xuanpolicy_ms.learners import *
+from xuanpolicy.mindspore.learners import *
 
 
 class DDPG_Learner(Learner):
     class ActorNetWithLossCell(nn.Cell):
         def __init__(self, backbone):
             super(DDPG_Learner.ActorNetWithLossCell, self).__init__()
             self._backbone = backbone
```

### Comparing `xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_ms/learners/policy_gradient/mpdqn_learner.py` & `xuanpolicy-0.1.6/xuanpolicy/mindspore/learners/policy_gradient/mpdqn_learner.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from xuanpolicy.xuanpolicy_ms.learners import *
+from xuanpolicy.mindspore.learners import *
 from mindspore.ops import OneHot
 
 
 class MPDQN_Learner(Learner):
     class QNetWithLossCell(nn.Cell):
         def __init__(self, backbone, loss_fn):
             super(MPDQN_Learner.QNetWithLossCell, self).__init__(auto_prefix=False)
```

### Comparing `xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_ms/learners/policy_gradient/pdqn_learner.py` & `xuanpolicy-0.1.6/xuanpolicy/mindspore/learners/policy_gradient/pdqn_learner.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from xuanpolicy.xuanpolicy_ms.learners import *
+from xuanpolicy.mindspore.learners import *
 from mindspore.ops import OneHot
 
 
 class PDQN_Learner(Learner):
     class ConActorNetWithLossCell(nn.Cell):
         def __init__(self, backbone):
             super(PDQN_Learner.ConActorNetWithLossCell, self).__init__(auto_prefix=False)
```

### Comparing `xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_ms/learners/policy_gradient/pg_learner.py` & `xuanpolicy-0.1.6/xuanpolicy/mindspore/learners/policy_gradient/pg_learner.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from xuanpolicy.xuanpolicy_ms.learners import *
+from xuanpolicy.mindspore.learners import *
 
 
 class PG_Learner(Learner):
     class PolicyNetWithLossCell(nn.Cell):
         def __init__(self, backbone, ent_coef):
             super(PG_Learner.PolicyNetWithLossCell, self).__init__(auto_prefix=False)
             self._backbone = backbone
```

### Comparing `xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_ms/learners/policy_gradient/ppg_learner.py` & `xuanpolicy-0.1.6/xuanpolicy/mindspore/learners/policy_gradient/ppg_learner.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-from xuanpolicy.xuanpolicy_ms.learners import *
-from xuanpolicy.xuanpolicy_ms.utils.operations import merge_distributions
+from xuanpolicy.mindspore.learners import *
+from xuanpolicy.mindspore.utils.operations import merge_distributions
 from mindspore.nn.probability.distribution import Categorical
 
 class PPG_Learner(Learner):
     class PolicyNetWithLossCell(nn.Cell):
         def __init__(self, backbone, ent_coef, kl_beta, clip_range, loss_fn):
             super(PPG_Learner.PolicyNetWithLossCell, self).__init__(auto_prefix=False)
             self._backbone = backbone
```

### Comparing `xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_ms/learners/policy_gradient/ppoclip_learner.py` & `xuanpolicy-0.1.6/xuanpolicy/mindspore/learners/policy_gradient/ppoclip_learner.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from xuanpolicy.xuanpolicy_ms.learners import *
+from xuanpolicy.mindspore.learners import *
 
 
 class PPOCLIP_Learner(Learner):
     class PolicyNetWithLossCell(nn.Cell):
         def __init__(self, backbone, ent_coef, vf_coef, clip_range):
             super(PPOCLIP_Learner.PolicyNetWithLossCell, self).__init__()
             self._backbone = backbone
```

### Comparing `xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_ms/learners/policy_gradient/ppokl_learner.py` & `xuanpolicy-0.1.6/xuanpolicy/mindspore/learners/policy_gradient/ppokl_learner.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from xuanpolicy.xuanpolicy_ms.learners import *
+from xuanpolicy.mindspore.learners import *
 
 
 class PPOCLIP_Learner(Learner):
     class PolicyNetWithLossCell(nn.Cell):
         def __init__(self, backbone, ent_coef, vf_coef, clip_range):
             super(PPOCLIP_Learner.PolicyNetWithLossCell, self).__init__()
             self._backbone = backbone
```

### Comparing `xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_ms/learners/policy_gradient/sac_learner.py` & `xuanpolicy-0.1.6/xuanpolicy/mindspore/learners/policy_gradient/sac_learner.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from xuanpolicy.xuanpolicy_ms.learners import *
+from xuanpolicy.mindspore.learners import *
 from mindspore.nn.probability.distribution import Normal
 
 
 class SAC_Learner(Learner):
     class ActorNetWithLossCell(nn.Cell):
         def __init__(self, backbone):
             super(SAC_Learner.ActorNetWithLossCell, self).__init__()
```

### Comparing `xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_ms/learners/policy_gradient/sacdis_learner.py` & `xuanpolicy-0.1.6/xuanpolicy/mindspore/learners/policy_gradient/sacdis_learner.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from xuanpolicy.xuanpolicy_ms.learners import *
+from xuanpolicy.mindspore.learners import *
 
 
 class SACDIS_Learner(Learner):
     class ActorNetWithLossCell(nn.Cell):
         def __init__(self, backbone):
             super(SACDIS_Learner.ActorNetWithLossCell, self).__init__()
             self._backbone = backbone
```

### Comparing `xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_ms/learners/policy_gradient/spdqn_learner.py` & `xuanpolicy-0.1.6/xuanpolicy/mindspore/learners/policy_gradient/spdqn_learner.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from xuanpolicy.xuanpolicy_ms.learners import *
+from xuanpolicy.mindspore.learners import *
 from mindspore.ops import OneHot
 
 
 class SPDQN_Learner(Learner):
     class QNetWithLossCell(nn.Cell):
         def __init__(self, backbone, loss_fn):
             super(SPDQN_Learner.QNetWithLossCell, self).__init__(auto_prefix=False)
```

### Comparing `xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_ms/learners/policy_gradient/td3_learner.py` & `xuanpolicy-0.1.6/xuanpolicy/mindspore/learners/policy_gradient/td3_learner.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # TD3 add three tricks to DDPG:
 # 1. noisy action in target actor
 # 2. double critic network
 # 3. delayed actor update
-from xuanpolicy.xuanpolicy_ms.learners import *
+from xuanpolicy.mindspore.learners import *
 
 
 class TD3_Learner(Learner):
     class ActorNetWithLossCell(nn.Cell):
         def __init__(self, backbone):
             super(TD3_Learner.ActorNetWithLossCell, self).__init__()
             self._backbone = backbone
```

### Comparing `xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_ms/learners/qlearning_family/c51_learner.py` & `xuanpolicy-0.1.6/xuanpolicy/mindspore/learners/qlearning_family/c51_learner.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from xuanpolicy.xuanpolicy_ms.learners import *
+from xuanpolicy.mindspore.learners import *
 from mindspore.ops import OneHot,Log,BatchMatMul,ExpandDims,Squeeze,ReduceSum,Abs,ReduceMean,clip_by_value
 
 
 class C51_Learner(Learner):
     class PolicyNetWithLossCell(nn.Cell):
         def __init__(self, backbone):
             super(C51_Learner.PolicyNetWithLossCell, self).__init__(auto_prefix=False)
```

### Comparing `xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_ms/learners/qlearning_family/cdqn_learner.py` & `xuanpolicy-0.1.6/xuanpolicy/mindspore/learners/qlearning_family/cdqn_learner.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from xuanpolicy.xuanpolicy_ms.learners import *
+from xuanpolicy.mindspore.learners import *
 from mindspore.ops import OneHot
 
 
 class CDQN_Learner(Learner):
     class PolicyNetWithLossCell(nn.Cell):
         def __init__(self, backbone, loss_fn):
             super(CDQN_Learner.PolicyNetWithLossCell, self).__init__(auto_prefix=False)
```

### Comparing `xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_ms/learners/qlearning_family/cldqn_learner.py` & `xuanpolicy-0.1.6/xuanpolicy/mindspore/learners/qlearning_family/cldqn_learner.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from xuanpolicy.xuanpolicy_ms.learners import *
+from xuanpolicy.mindspore.learners import *
 from mindspore.ops import OneHot
 
 
 class CLDQN_Learner(Learner):
     class PolicyNetWithLossCell(nn.Cell):
         def __init__(self, backbone, loss_fn):
             super(CLDQN_Learner.PolicyNetWithLossCell, self).__init__(auto_prefix=False)
```

### Comparing `xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_ms/learners/qlearning_family/ddqn_learner.py` & `xuanpolicy-0.1.6/xuanpolicy/mindspore/learners/qlearning_family/ddqn_learner.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from xuanpolicy.xuanpolicy_ms.learners import *
+from xuanpolicy.mindspore.learners import *
 from mindspore.ops import OneHot
 
 
 class DDQN_Learner(Learner):
     class PolicyNetWithLossCell(nn.Cell):
         def __init__(self, backbone, loss_fn):
             super(DDQN_Learner.PolicyNetWithLossCell, self).__init__(auto_prefix=False)
```

### Comparing `xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_ms/learners/qlearning_family/dqn_learner.py` & `xuanpolicy-0.1.6/xuanpolicy/mindspore/learners/qlearning_family/dqn_learner.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from xuanpolicy.xuanpolicy_ms.learners import *
+from xuanpolicy.mindspore.learners import *
 from mindspore.ops import OneHot
 
 
 class DQN_Learner(Learner):
     class PolicyNetWithLossCell(nn.Cell):
         def __init__(self, backbone, loss_fn):
             super(DQN_Learner.PolicyNetWithLossCell, self).__init__(auto_prefix=False)
```

### Comparing `xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_ms/learners/qlearning_family/dueldqn_learner.py` & `xuanpolicy-0.1.6/xuanpolicy/mindspore/learners/qlearning_family/dueldqn_learner.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from xuanpolicy.xuanpolicy_ms.learners import *
+from xuanpolicy.mindspore.learners import *
 from mindspore.ops import OneHot
 
 
 class DuelDQN_Learner(Learner):
     class PolicyNetWithLossCell(nn.Cell):
         def __init__(self, backbone, loss_fn):
             super(DuelDQN_Learner.PolicyNetWithLossCell, self).__init__(auto_prefix=False)
```

### Comparing `xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_ms/learners/qlearning_family/ldqn_learner.py` & `xuanpolicy-0.1.6/xuanpolicy/mindspore/learners/qlearning_family/ldqn_learner.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from xuanpolicy.xuanpolicy_ms.learners import *
+from xuanpolicy.mindspore.learners import *
 from mindspore.ops import OneHot
 
 
 class LDQN_Learner(Learner):
     class PolicyNetWithLossCell(nn.Cell):
         def __init__(self, backbone, loss_fn):
             super(LDQN_Learner.PolicyNetWithLossCell, self).__init__(auto_prefix=False)
```

### Comparing `xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_ms/learners/qlearning_family/perdqn_learner.py` & `xuanpolicy-0.1.6/xuanpolicy/mindspore/learners/qlearning_family/perdqn_learner.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from xuanpolicy.xuanpolicy_ms.learners import *
+from xuanpolicy.mindspore.learners import *
 from mindspore.ops import OneHot
 
 
 class PerDQN_Learner(Learner):
     class PolicyNetWithLossCell(nn.Cell):
         def __init__(self, backbone, loss_fn):
             super(PerDQN_Learner.PolicyNetWithLossCell, self).__init__(auto_prefix=False)
```

### Comparing `xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_ms/learners/qlearning_family/qrdqn_learner.py` & `xuanpolicy-0.1.6/xuanpolicy/mindspore/learners/qlearning_family/qrdqn_learner.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from xuanpolicy.xuanpolicy_ms.learners import *
+from xuanpolicy.mindspore.learners import *
 from mindspore.ops import OneHot,ExpandDims,ReduceSum
 
 
 class QRDQN_Learner(Learner):
     class PolicyNetWithLossCell(nn.Cell):
         def __init__(self, backbone, loss_fn):
             super(QRDQN_Learner.PolicyNetWithLossCell, self).__init__(auto_prefix=False)
```

### Comparing `xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_ms/policies/__init__.py` & `xuanpolicy-0.1.6/xuanpolicy/mindspore/policies/__init__.py`

 * *Files identical despite different names*

### Comparing `xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_ms/policies/categorical.py` & `xuanpolicy-0.1.6/xuanpolicy/mindspore/policies/categorical.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-from xuanpolicy.xuanpolicy_ms.policies import *
-from xuanpolicy.xuanpolicy_ms.utils import *
+from xuanpolicy.mindspore.policies import *
+from xuanpolicy.mindspore.utils import *
 from mindspore.nn.probability.distribution import Categorical
 import copy
 
 
 class ActorNet(nn.Cell):
     class Sample(nn.Cell):
         def __init__(self):
```

### Comparing `xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_ms/policies/categorical_marl.py` & `xuanpolicy-0.1.6/xuanpolicy/mindspore/policies/categorical_marl.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-from xuanpolicy.xuanpolicy_ms.policies import *
-from xuanpolicy.xuanpolicy_ms.utils import *
-from xuanpolicy.xuanpolicy_ms.representations import Basic_Identical
+from xuanpolicy.mindspore.policies import *
+from xuanpolicy.mindspore.utils import *
+from xuanpolicy.mindspore.representations import Basic_Identical
 from .deterministic_marl import BasicQhead
 from mindspore.nn.probability.distribution import Categorical
 import copy
 
 
 class ActorNet(nn.Cell):
     class Sample(nn.Cell):
```

### Comparing `xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_ms/policies/deterministic.py` & `xuanpolicy-0.1.6/xuanpolicy/mindspore/policies/deterministic.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-from xuanpolicy.xuanpolicy_ms.policies import *
-from xuanpolicy.xuanpolicy_ms.utils import *
+from xuanpolicy.mindspore.policies import *
+from xuanpolicy.mindspore.utils import *
 import copy
 from gym.spaces import Space, Box, Discrete, Dict
 
 class BasicQhead(nn.Cell):
     def __init__(self,
                  state_dim: int,
                  action_dim: int,
```

### Comparing `xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_ms/policies/deterministic_marl.py` & `xuanpolicy-0.1.6/xuanpolicy/mindspore/policies/deterministic_marl.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import markdown.extensions.smarty
 
-from xuanpolicy.xuanpolicy_ms.policies import *
-from xuanpolicy.xuanpolicy_ms.utils import *
+from xuanpolicy.mindspore.policies import *
+from xuanpolicy.mindspore.utils import *
 import copy
-from xuanpolicy.xuanpolicy_ms.representations import Basic_Identical
+from xuanpolicy.mindspore.representations import Basic_Identical
 from mindspore.nn.probability.distribution import Categorical
 
 
 class BasicQhead(nn.Cell):
     def __init__(self,
                  state_dim: int,
                  action_dim: int,
```

### Comparing `xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_ms/policies/gaussian.py` & `xuanpolicy-0.1.6/xuanpolicy/mindspore/policies/gaussian.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-from xuanpolicy.xuanpolicy_ms.policies import *
-from xuanpolicy.xuanpolicy_ms.utils import *
+from xuanpolicy.mindspore.policies import *
+from xuanpolicy.mindspore.utils import *
 from mindspore.nn.probability.distribution import Normal
 import copy
 
 class ActorNet(nn.Cell):
     class Sample(nn.Cell):
         def __init__(self, log_std):
             super(ActorNet.Sample, self).__init__()
```

### Comparing `xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_ms/policies/gaussian_marl.py` & `xuanpolicy-0.1.6/xuanpolicy/mindspore/policies/gaussian_marl.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-from xuanpolicy.xuanpolicy_ms.policies import *
-from xuanpolicy.xuanpolicy_ms.utils import *
-from xuanpolicy.xuanpolicy_ms.representations import Basic_Identical
+from xuanpolicy.mindspore.policies import *
+from xuanpolicy.mindspore.utils import *
+from xuanpolicy.mindspore.representations import Basic_Identical
 from mindspore.nn.probability.distribution import Normal
 import copy
 
 
 class BasicQhead(nn.Cell):
     def __init__(self,
                  state_dim: int,
```

### Comparing `xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_ms/policies/mixers.py` & `xuanpolicy-0.1.6/xuanpolicy/mindspore/policies/mixers.py`

 * *Files identical despite different names*

### Comparing `xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_ms/representations/__init__.py` & `xuanpolicy-0.1.6/xuanpolicy/mindspore/representations/__init__.py`

 * *Files identical despite different names*

### Comparing `xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_ms/representations/networks.py` & `xuanpolicy-0.1.6/xuanpolicy/mindspore/representations/networks.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import mindspore as ms
 import mindspore.nn as nn
 from typing import Sequence, Optional, Union, Callable
 import numpy as np
-from xuanpolicy.xuanpolicy_ms.utils.layers import ModuleType, mlp_block, cnn_block, gru_block
+from xuanpolicy.mindspore.utils.layers import ModuleType, mlp_block, cnn_block, gru_block
 
 
 # directly returns the original observation
 class Basic_Identical(nn.Cell):
     def __init__(self,
                  input_shape: Sequence[int]):
         super(Basic_Identical, self).__init__()
```

### Comparing `xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_ms/runners/runner_basic.py` & `xuanpolicy-0.1.6/xuanpolicy/torch/runners/runner_basic.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,28 +1,38 @@
+import time
+
 from xuanpolicy.environment import make_envs
 
 
 class Runner_Base(object):
     def __init__(self, args):
         # build environments
-        self.envs = make_envs(args.env_name, args.env_id, args.seed, args.vectorize, args.parallels)
+        if hasattr(args, 'continuous_action'):
+            self.envs = make_envs(args.env_name, args.env_id, args.seed, args.vectorize, args.parallels,
+                                  args.continuous_action, args.render_mode)
+        else:
+            self.envs = make_envs(args.env_name, args.env_id, args.seed, args.vectorize, args.parallels,
+                                  args.render_mode)
+
         if args.vectorize != 'NOREQUIRED':
             self.n_envs = self.envs.num_envs
 
         self.train_at_step = args.train_at_step
 
     def run(self):
         pass
 
     def tb_load(self, data):
         return
 
 
 class Runner_Base_MARL(Runner_Base):
     def __init__(self, args):
+        if args.test_mode:
+            args.render_mode = 'human'
         super(Runner_Base_MARL, self).__init__(args)
         # build environments
         self.n_handles = len(self.envs.handles)
         self.loss = [[0.0] for _ in range(self.n_handles)]
 
         self.agent_keys = self.envs.agent_keys
         self.agent_ids = self.envs.agent_ids
@@ -85,7 +95,9 @@
         for h, arg in enumerate(args):
             agent_name = self.envs.agent_keys[h][0][0:-2]
             if arg.n_agents == 1:
                 infos.append(agent_name + ": {} agent".format(arg.n_agents) + ", {}".format(arg.agent))
             else:
                 infos.append(agent_name + ": {} agents".format(arg.n_agents) + ", {}".format(arg.agent))
         print(infos)
+        time.sleep(0.01)
+
```

### Comparing `xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_ms/runners/runner_drl.py` & `xuanpolicy-0.1.6/xuanpolicy/mindspore/runners/runner_drl.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from .runner_basic import *
-from xuanpolicy.xuanpolicy_ms.agents import get_total_iters
-from xuanpolicy.xuanpolicy_ms.representations import REGISTRY as REGISTRY_Representation
-from xuanpolicy.xuanpolicy_ms.agents import REGISTRY as REGISTRY_Agent
-from xuanpolicy.xuanpolicy_ms.policies import REGISTRY as REGISTRY_Policy
-from xuanpolicy.xuanpolicy_ms.utils.input_reformat import get_repre_in, get_policy_in
+from xuanpolicy.mindspore.agents import get_total_iters
+from xuanpolicy.mindspore.representations import REGISTRY as REGISTRY_Representation
+from xuanpolicy.mindspore.agents import REGISTRY as REGISTRY_Agent
+from xuanpolicy.mindspore.policies import REGISTRY as REGISTRY_Policy
+from xuanpolicy.mindspore.utils.input_reformat import get_repre_in, get_policy_in
 import itertools
 from mindspore.nn import Adam
 from mindspore.nn.learning_rate_schedule import ExponentialDecayLR as lr_decay_model
 import gym.spaces
 import numpy as np
 
 
@@ -70,8 +70,9 @@
                                           decay_rate=0.5,
                                           decay_steps=get_total_iters(self.agent_name, self.args)
                                           )
             optimizer = Adam(policy.trainable_params(), lr_scheduler, eps=1e-5)
             self.agent = REGISTRY_Agent[self.agent_name](self.args, self.envs, policy, optimizer, lr_scheduler)
 
     def run(self):
-        self.agent.test() if self.args.test_mode else self.agent.train(self.args.training_steps)
+        self.agent.test(self.args.test_steps) if self.args.test_mode else self.agent.train(self.args.training_steps)
+        self.envs.close()
```

### Comparing `xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_ms/runners/runner_marl.py` & `xuanpolicy-0.1.6/xuanpolicy/tensorflow/runners/runner_marl.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from .runner_basic import *
-from xuanpolicy.xuanpolicy_ms.agents import REGISTRY as REGISTRY_Agent
+from xuanpolicy.tensorflow.agents import REGISTRY as REGISTRY_Agent
 from gym.spaces import Box
 from tqdm import tqdm
 import numpy as np
 from copy import deepcopy
+import time
 
 
 class Runner(Runner_Base_MARL):
     def __init__(self, args):
         self.args = args if type(args) == list else [args]
         super(Runner, self).__init__(self.args[0])
 
@@ -23,15 +24,15 @@
             else:
                 arg.dim_act = self.envs.action_space[self.agent_keys[h][0]].n
                 arg.act_shape = (arg.n_agents,)
             arg.action_space = self.envs.action_space
             arg.dim_obs = self.envs.observation_space[self.agent_keys[h][0]].shape
             arg.obs_shape = (arg.n_agents,) + arg.dim_obs
             arg.rew_shape, arg.done_shape, arg.act_prob_shape = (arg.n_agents, 1), (arg.n_agents,), (arg.dim_act,)
-            self.marl_agents.append(REGISTRY_Agent[arg.agent](arg, self.envs))
+            self.marl_agents.append(REGISTRY_Agent[arg.agent](arg, self.envs, arg.device))
             self.marl_names.append(arg.agent)
             if arg.test_mode:
                 self.marl_agents[h].load_model(arg.modeldir)
 
         self.print_infos(self.args)
 
     def run_episode(self, episode, test_mode=False):
@@ -44,15 +45,16 @@
 
         while True:
             actions_dict = self.get_actions(obs_n, episode, test_mode, act_mean_last, agent_mask, state)
             actions_execute = self.combine_env_actions(actions_dict['actions_n'])
             next_obs_n, rew_n, done_n, dones, info = self.envs.step(actions_execute)
             next_state, agent_mask = self.envs.global_state(), self.envs.agent_mask()
 
-            if self.render or self.test_mode: self.envs.render(self.render_delay)
+            if self.render or self.test_mode:
+                time.sleep(self.render_delay)
             if test_mode:
                 for h in range(self.n_handles):
                     scores[h] += (1-done_envs) * np.mean(rew_n[h] * agent_mask[h][:, :, np.newaxis], axis=1)
             else:
                 self.store_data(obs_n, next_obs_n, actions_dict, state, next_state, agent_mask, rew_n, done_n, self.envs)
                 for h, mas_group in enumerate(self.marl_agents):
                     if self.args[h].train_at_step: self.marl_agents[h].train(episode)
@@ -92,30 +94,30 @@
                 for i_test in range(self.n_tests):
                     r_episode = self.run_episode(i_episode, test_mode=True)
                     reward += r_episode
                 reward = reward / self.n_tests
                 for h, mas_group in enumerate(self.marl_agents):
                     for i in range(self.n_envs):
                         self.marl_agents[h].writer.add_scalars("reward_mean", {"env-%d" % i: reward[h, i]}, i_episode)
-                    if i_episode % 5000 == 0 or i_episode == self.n_episodes - 1:
-                        mas_group.save_model()
+        for h, mas_group in enumerate(self.marl_agents):
+            mas_group.save_model()
 
         self.envs.close()
 
     def store_data(self, obs_n, next_obs_n, actions_dict, state, next_state, agent_mask, rew_n, done_n, env):
         for h, mas_group in enumerate(self.marl_agents):
             data_step = {'obs': obs_n[h], 'obs_next': next_obs_n[h], 'actions': actions_dict['actions_n'][h],
                          'state': state, 'state_next': next_state, 'rewards': rew_n[h],
                          'agent_mask': agent_mask[h], 'terminals': done_n[h]}
             if self.marl_names[h] in ["CID_Simple", "CID_Rainbow"]:
                 rew_n_assign = mas_group.reward_shaping(state, obs_n[h], actions_dict['actions_n'][h], rew_n[h], env)
                 data_step.update({'rewards_assign': rew_n_assign})
             elif self.marl_names[h] in ["MAPPO_KL", "MAPPO_Clip", "VDAC"]:
                 if self.marl_names[h] == "MAPPO_KL":
-                    data_step.update({'values': actions_dict['values'][h], 'act_prob_old': actions_dict['log_pi'][h]})
+                    data_step.update({'values': actions_dict['values'][h], 'pi_dist_old': actions_dict['log_pi'][h]})
                 else:
                     data_step.update({'values': actions_dict['values'][h], 'log_pi_old': actions_dict['log_pi'][h]})
             elif self.marl_names[h] in ["COMA"]:
                 data_step.update({'actions_onehot': actions_dict['act_n_onehot'][h]})
             elif self.marl_names[h] in ["MFQ", "MFAC"]:
                 data_step.update({'act_mean': actions_dict['act_mean'][h]})
             else:
```

### Comparing `xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_ms/utils/distributions.py` & `xuanpolicy-0.1.6/xuanpolicy/mindspore/utils/distributions.py`

 * *Files identical despite different names*

### Comparing `xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_ms/utils/input_reformat.py` & `xuanpolicy-0.1.6/xuanpolicy/mindspore/utils/input_reformat.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from xuanpolicy.common import space2shape
 from copy import deepcopy
-from xuanpolicy.xuanpolicy_ms.policies import Policy_Inputs, Policy_Inputs_All
-from xuanpolicy.xuanpolicy_ms.representations import Representation_Inputs, Representation_Inputs_All
+from xuanpolicy.mindspore.policies import Policy_Inputs, Policy_Inputs_All
+from xuanpolicy.mindspore.representations import Representation_Inputs, Representation_Inputs_All
 from operator import itemgetter
 import mindspore.nn as nn
 from mindspore.common.initializer import TruncatedNormal
 
 
 def get_repre_in(args):
     representation_name = args.representation
```

### Comparing `xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_ms/utils/layers.py` & `xuanpolicy-0.1.6/xuanpolicy/mindspore/utils/layers.py`

 * *Files identical despite different names*

### Comparing `xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_ms/utils/operations.py` & `xuanpolicy-0.1.6/xuanpolicy/mindspore/utils/operations.py`

 * *Files identical despite different names*

### Comparing `xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_ms/utils/set_trainer.py` & `xuanpolicy-0.1.6/xuanpolicy/mindspore/utils/set_trainer.py`

 * *Files identical despite different names*

### Comparing `xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_tf/agents/__init__.py` & `xuanpolicy-0.1.6/xuanpolicy/tensorflow/agents/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,21 +6,21 @@
 from torch.utils.tensorboard import SummaryWriter
 
 import tensorflow as tf
 import tensorflow.keras as tk
 
 from xuanpolicy.environment import *
 from xuanpolicy.common import *
-from xuanpolicy.xuanpolicy_tf.learners import *
-from xuanpolicy.xuanpolicy_tf.policies import *
-from xuanpolicy.xuanpolicy_tf.utils import *
-from xuanpolicy.xuanpolicy_tf.policies import REGISTRY as REGISTRY_Policy
-from xuanpolicy.xuanpolicy_tf.utils.input_reformat import get_repre_in, get_policy_in_marl
-from xuanpolicy.xuanpolicy_tf.representations import REGISTRY as REGISTRY_Representation
-from xuanpolicy.xuanpolicy_tf.runners.runner_basic import MyLinearLR
+from xuanpolicy.tensorflow.learners import *
+from xuanpolicy.tensorflow.policies import *
+from xuanpolicy.tensorflow.utils import *
+from xuanpolicy.tensorflow.policies import REGISTRY as REGISTRY_Policy
+from xuanpolicy.tensorflow.utils.input_reformat import get_repre_in, get_policy_in_marl
+from xuanpolicy.tensorflow.representations import REGISTRY as REGISTRY_Representation
+from xuanpolicy.tensorflow.runners.runner_basic import MyLinearLR
 
 from .agent import Agent
 from .agents_marl import MARLAgents, RandomAgents, get_total_iters
 from .agent import get_total_iters
 
 '''
 Single-Agent DRL Algorithms
```

### Comparing `xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_tf/agents/agent.py` & `xuanpolicy-0.1.6/xuanpolicy/tensorflow/agents/agent.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from xuanpolicy.xuanpolicy_tf.agents import *
+from xuanpolicy.tensorflow.agents import *
 
 class Agent(ABC):
     def __init__(self,
                  envs: VecEnv,
                  policy: tk.Model,
                  memory: Buffer,
                  learner: Learner,
```

### Comparing `xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_tf/agents/agents_marl.py` & `xuanpolicy-0.1.6/xuanpolicy/tensorflow/agents/agents_marl.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from xuanpolicy.xuanpolicy_tf.agents import *
+from xuanpolicy.tensorflow.agents import *
 
 
 class MARLAgents(object):
     def __init__(self,
                  config: Namespace,
                  envs: DummyVecEnv_MAS,
                  policy: tk.Model,
```

### Comparing `xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_tf/agents/multi_agent_rl/coma_agents.py` & `xuanpolicy-0.1.6/xuanpolicy/tensorflow/agents/multi_agent_rl/coma_agents.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-from xuanpolicy.xuanpolicy_tf.agents import *
-from xuanpolicy.xuanpolicy_tf.agents.agents_marl import linear_decay_or_increase
+from xuanpolicy.tensorflow.agents import *
+from xuanpolicy.tensorflow.agents.agents_marl import linear_decay_or_increase
 
 
 class COMA_Agents(MARLAgents):
     def __init__(self,
                  config: Namespace,
                  envs: DummyVecEnv_MAS,
                  device: str = "cpu:0"):
```

### Comparing `xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_tf/agents/multi_agent_rl/dcg_agents.py` & `xuanpolicy-0.1.6/xuanpolicy/tensorflow/agents/multi_agent_rl/dcg_agents.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-from xuanpolicy.xuanpolicy_tf.agents import *
-from xuanpolicy.xuanpolicy_tf.agents.agents_marl import linear_decay_or_increase
+from xuanpolicy.tensorflow.agents import *
+from xuanpolicy.tensorflow.agents.agents_marl import linear_decay_or_increase
 
 
 class DCG_Agents(MARLAgents):
     def __init__(self,
                  config: Namespace,
                  envs: DummyVecEnv_MAS,
                  device: str = "cpu:0"):
```

### Comparing `xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_tf/agents/multi_agent_rl/iddpg_agents.py` & `xuanpolicy-0.1.6/xuanpolicy/tensorflow/agents/multi_agent_rl/mappokl_agents.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,59 +1,57 @@
-from xuanpolicy.xuanpolicy_tf.agents import *
+from xuanpolicy.tensorflow.agents import *
 
 
-class IDDPG_Agents(MARLAgents):
+class MAPPO_KL_Agents(MARLAgents):
     def __init__(self,
                  config: Namespace,
                  envs: DummyVecEnv_MAS,
                  device: str = "cpu:0"):
         self.comm = MPI.COMM_WORLD
 
         self.gamma = config.gamma
         self.use_obsnorm = config.use_obsnorm
         self.use_rewnorm = config.use_rewnorm
         self.obsnorm_range = config.obsnorm_range
         self.rewnorm_range = config.rewnorm_range
 
+        if config.state_space is not None:
+            config.dim_state, state_shape = config.state_space.shape, config.state_space.shape
+        else:
+            config.dim_state, state_shape = None, None
+
         input_representation = get_repre_in(config)
         representation = REGISTRY_Representation[config.representation](*input_representation)
+
         input_policy = get_policy_in_marl(config, representation, config.agent_keys)
         policy = REGISTRY_Policy[config.policy](*input_policy)
-        lr_scheduler = [MyLinearLR(config.lr_a, start_factor=1.0, end_factor=0.5,
-                                   total_iters=get_total_iters(config.agent_name, config)),
-                        MyLinearLR(config.lr_c, start_factor=1.0, end_factor=0.5,
-                                   total_iters=get_total_iters(config.agent_name, config))]
-        optimizer = [tk.optimizers.Adam(lr_scheduler[0]),
-                     tk.optimizers.Adam(lr_scheduler[1])]
+        lr_scheduler = MyLinearLR(config.learning_rate, start_factor=1.0, end_factor=0.5,
+                                  total_iters=get_total_iters(config.agent_name, config))
+        optimizer = tk.optimizers.Adam(lr_scheduler)
         self.observation_space = envs.observation_space
         self.action_space = envs.action_space
         self.representation_info_shape = policy.representation.output_shapes
         self.auxiliary_info_shape = {}
 
         writer = SummaryWriter(config.logdir)
         if config.state_space is not None:
             config.dim_state, state_shape = config.state_space.shape, config.state_space.shape
         else:
             config.dim_state, state_shape = None, None
-        memory = MARL_OffPolicyBuffer(state_shape,
-                                      config.obs_shape,
-                                      config.act_shape,
-                                      config.rew_shape,
-                                      config.done_shape,
-                                      envs.num_envs,
-                                      config.buffer_size,
-                                      config.batch_size)
-        learner = IDDPG_Learner(config, policy, optimizer, writer,
-                                config.device, config.modeldir, config.gamma)
+        memory = MARL_OnPolicyBuffer(state_shape, config.obs_shape, config.act_shape, config.rew_shape,
+                                     config.done_shape, envs.num_envs, config.nsteps, config.nminibatch,
+                                     config.use_gae, config.use_advnorm, config.gamma, config.lam)
+        learner = MAPPO_KL_Learner(config, policy, optimizer, writer,
+                                   config.device, config.modeldir, config.gamma)
 
         self.obs_rms = RunningMeanStd(shape=space2shape(self.observation_space[config.agent_keys[0]]),
                                       comm=self.comm, use_mpi=False)
         self.ret_rms = RunningMeanStd(shape=(), comm=self.comm, use_mpi=False)
-        super(IDDPG_Agents, self).__init__(config, envs, policy, memory, learner, writer, device,
-                                           config.logdir, config.modeldir)
+        super(MAPPO_KL_Agents, self).__init__(config, envs, policy, memory, learner, writer, device,
+                                              config.logdir, config.modeldir)
 
     def _process_observation(self, observations):
         if self.use_obsnorm:
             if isinstance(self.observation_space, Dict):
                 for key in self.observation_space.spaces.keys():
                     observations[key] = np.clip(
                         (observations[key] - self.obs_rms.mean[key]) / (self.obs_rms.std[key] + EPS),
@@ -66,22 +64,35 @@
 
     def _process_reward(self, rewards):
         if self.use_rewnorm:
             std = np.clip(self.ret_rms.std, 0.1, 100)
             return np.clip(rewards / std, -self.rewnorm_range, self.rewnorm_range)
         return rewards
 
-    def act(self, obs_n, episode, test_mode, noise=False):
+    def act(self, obs_n, episode, test_mode, state=None, noise=False):
         batch_size = len(obs_n)
         with tf.device(self.device):
             agents_id = tf.tile(tf.expand_dims(tf.eye(self.n_agents), axis=0), multiples=(batch_size, 1, 1))
             inputs_policy = {"obs": tf.convert_to_tensor(obs_n), "ids": agents_id}
-            _, actions = self.policy(inputs_policy)
-        actions = actions.numpy()
-        if noise:
-            actions += np.random.normal(0, self.args.sigma, size=actions.shape)
-        return actions
+            _, dists = self.policy(inputs_policy)
+            acts = dists.stochastic_sample()
+            state = tf.convert_to_tensor(state)
+            state_expand = tf.tile(tf.expand_dims(state, axis=-2), (1, self.n_agents, 1))
+            vs = self.policy.values(state_expand, agents_id)
+        return acts.numpy(), split_distributions(dists), vs.numpy()
+
+    def value(self, obs, state):
+        batch_size = len(state)
+        agents_id = tf.tile(tf.expand_dims(tf.eye(self.n_agents), axis=0), multiples=(batch_size, 1, 1))
+        repre_out = self.policy.representation(obs)
+        critic_input = tf.concat([torch.Tensor(repre_out['state']), agents_id], axis=-1)
+        values_n = self.policy.critic(critic_input)
+        values = self.policy.value_tot(values_n, global_state=state)
+        values = tf.expand_dims(tf.tile(tf.reshape(values, (-1, 1)), (1, self.n_agents)), axis=-1)
+        return values.numpy()
 
     def train(self, i_episode):
-        if self.memory.can_sample(self.args.batch_size):
-            sample = self.memory.sample()
-            self.learner.update(sample)
+        if self.memory.full:
+            for _ in range(self.args.nminibatch * self.args.nepoch):
+                sample = self.memory.sample()
+                self.learner.update(sample)
+            self.memory.clear()
```

### Comparing `xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_tf/agents/multi_agent_rl/iql_agents.py` & `xuanpolicy-0.1.6/xuanpolicy/tensorflow/agents/multi_agent_rl/vdn_agents.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-from xuanpolicy.xuanpolicy_tf.agents import *
-from xuanpolicy.xuanpolicy_tf.agents.agents_marl import linear_decay_or_increase
+from xuanpolicy.tensorflow.agents import *
+from xuanpolicy.tensorflow.agents.agents_marl import linear_decay_or_increase
 
 
-class IQL_Agents(MARLAgents):
+class VDN_Agents(MARLAgents):
     def __init__(self,
                  config: Namespace,
                  envs: DummyVecEnv_MAS,
                  device: str = "cpu:0"):
         self.comm = MPI.COMM_WORLD
 
         self.gamma = config.gamma
@@ -17,15 +17,16 @@
 
         self.start_greedy = config.start_greedy
         self.end_greedy = config.end_greedy
         self.egreedy = config.start_greedy
 
         input_representation = get_repre_in(config)
         representation = REGISTRY_Representation[config.representation](*input_representation)
-        input_policy = get_policy_in_marl(config, representation, config.agent_keys)
+        mixer = VDN_mixer()
+        input_policy = get_policy_in_marl(config, representation, config.agent_keys, mixer)
         policy = REGISTRY_Policy[config.policy](*input_policy)
         # lr_scheduler = tk.optimizers.schedules.ExponentialDecay(config.learning_rate, decay_steps=1000,
         #                                                         decay_rate=0.9)
         lr_scheduler = MyLinearLR(config.learning_rate, start_factor=1.0, end_factor=0.5,
                                   total_iters=get_total_iters(config.agent_name, config))
         optimizer = tk.optimizers.Adam(lr_scheduler)
         self.observation_space = envs.observation_space
@@ -42,23 +43,24 @@
                                       config.obs_shape,
                                       config.act_shape,
                                       config.rew_shape,
                                       config.done_shape,
                                       envs.num_envs,
                                       config.buffer_size,
                                       config.batch_size)
-        learner = IQL_Learner(config, policy, optimizer, writer,
-                              config.device, config.modeldir, config.gamma, config.sync_frequency)
+        learner = VDN_Learner(config, policy, optimizer, writer,
+                              config.device, config.modeldir, config.gamma,
+                              config.sync_frequency)
 
         self.obs_rms = RunningMeanStd(shape=space2shape(self.observation_space[config.agent_keys[0]]),
                                       comm=self.comm, use_mpi=False)
         self.ret_rms = RunningMeanStd(shape=(), comm=self.comm, use_mpi=False)
         self.epsilon_decay = linear_decay_or_increase(config.start_greedy, config.end_greedy,
                                                       config.greedy_update_steps)
-        super(IQL_Agents, self).__init__(config, envs, policy, memory, learner, writer, device,
+        super(VDN_Agents, self).__init__(config, envs, policy, memory, learner, writer, device,
                                          config.logdir, config.modeldir)
 
     def _process_observation(self, observations):
         if self.use_obsnorm:
             if isinstance(self.observation_space, Dict):
                 for key in self.observation_space.spaces.keys():
                     observations[key] = np.clip(
```

### Comparing `xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_tf/agents/multi_agent_rl/isac_agents.py` & `xuanpolicy-0.1.6/xuanpolicy/torch/agents/multi_agent_rl/iql_agents.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,33 +1,35 @@
-from xuanpolicy.xuanpolicy_tf.agents import *
+from xuanpolicy.torch.agents import *
+from xuanpolicy.torch.agents.agents_marl import linear_decay_or_increase
 
 
-class ISAC_Agents(MARLAgents):
+class IQL_Agents(MARLAgents):
     def __init__(self,
                  config: Namespace,
                  envs: DummyVecEnv_MAS,
-                 device: str = "cpu:0"):
+                 device: Optional[Union[int, str, torch.device]] = None):
         self.comm = MPI.COMM_WORLD
 
         self.gamma = config.gamma
         self.use_obsnorm = config.use_obsnorm
         self.use_rewnorm = config.use_rewnorm
         self.obsnorm_range = config.obsnorm_range
         self.rewnorm_range = config.rewnorm_range
 
+        self.start_greedy = config.start_greedy
+        self.end_greedy = config.end_greedy
+        self.egreedy = config.start_greedy
+
         input_representation = get_repre_in(config)
         representation = REGISTRY_Representation[config.representation](*input_representation)
         input_policy = get_policy_in_marl(config, representation, config.agent_keys)
         policy = REGISTRY_Policy[config.policy](*input_policy)
-        lr_scheduler = [MyLinearLR(config.lr_a, start_factor=1.0, end_factor=0.5,
-                                   total_iters=get_total_iters(config.agent_name, config)),
-                        MyLinearLR(config.lr_c, start_factor=1.0, end_factor=0.5,
-                                   total_iters=get_total_iters(config.agent_name, config))]
-        optimizer = [tk.optimizers.Adam(lr_scheduler[0]),
-                     tk.optimizers.Adam(lr_scheduler[1])]
+        optimizer = torch.optim.Adam(policy.parameters(), config.learning_rate, eps=1e-5)
+        scheduler = torch.optim.lr_scheduler.LinearLR(optimizer, start_factor=1.0, end_factor=0.5,
+                                                      total_iters=get_total_iters(config.agent_name, config))
         self.observation_space = envs.observation_space
         self.action_space = envs.action_space
         self.representation_info_shape = policy.representation.output_shapes
         self.auxiliary_info_shape = {}
 
         writer = SummaryWriter(config.logdir)
         if config.state_space is not None:
@@ -38,21 +40,25 @@
                                       config.obs_shape,
                                       config.act_shape,
                                       config.rew_shape,
                                       config.done_shape,
                                       envs.num_envs,
                                       config.buffer_size,
                                       config.batch_size)
-        learner = ISAC_Learner(config, policy, optimizer, writer, config.device, config.modeldir, config.gamma)
+        learner = IQL_Learner(config, policy, optimizer, scheduler, writer,
+                              config.device, config.modeldir, config.gamma,
+                              config.sync_frequency)
 
         self.obs_rms = RunningMeanStd(shape=space2shape(self.observation_space[config.agent_keys[0]]),
                                       comm=self.comm, use_mpi=False)
         self.ret_rms = RunningMeanStd(shape=(), comm=self.comm, use_mpi=False)
-        super(ISAC_Agents, self).__init__(config, envs, policy, memory, learner, writer, device,
-                                          config.logdir, config.modeldir)
+        self.epsilon_decay = linear_decay_or_increase(config.start_greedy, config.end_greedy,
+                                                      config.greedy_update_steps)
+        super(IQL_Agents, self).__init__(config, envs, policy, memory, learner, writer, device,
+                                         config.logdir, config.modeldir)
 
     def _process_observation(self, observations):
         if self.use_obsnorm:
             if isinstance(self.observation_space, Dict):
                 for key in self.observation_space.spaces.keys():
                     observations[key] = np.clip(
                         (observations[key] - self.obs_rms.mean[key]) / (self.obs_rms.std[key] + EPS),
@@ -65,21 +71,14 @@
 
     def _process_reward(self, rewards):
         if self.use_rewnorm:
             std = np.clip(self.ret_rms.std, 0.1, 100)
             return np.clip(rewards / std, -self.rewnorm_range, self.rewnorm_range)
         return rewards
 
-    def act(self, obs_n, episode, test_mode, state=None, noise=False):
-        batch_size = len(obs_n)
-        with tf.device(self.device):
-            agents_id = tf.tile(tf.expand_dims(tf.eye(self.n_agents), axis=0), multiples=(batch_size, 1, 1))
-            inputs_policy = {"obs": tf.convert_to_tensor(obs_n), "ids": agents_id}
-            _, dists = self.policy(inputs_policy)
-            acts = dists.sample()
-        actions = acts.numpy()
-        return actions
-
     def train(self, i_episode):
+        self.epsilon_decay.update()
+        for i in range(self.nenvs):
+            self.writer.add_scalars("epsilon", {"env-%d" % i: self.epsilon_decay.epsilon}, i_episode)
         if self.memory.can_sample(self.args.batch_size):
             sample = self.memory.sample()
             self.learner.update(sample)
```

### Comparing `xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_tf/agents/multi_agent_rl/maddpg_agents.py` & `xuanpolicy-0.1.6/xuanpolicy/torch/agents/multi_agent_rl/mappoclip_agents.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,59 +1,57 @@
-from xuanpolicy.xuanpolicy_tf.agents import *
+from xuanpolicy.torch.agents import *
 
 
-class MADDPG_Agents(MARLAgents):
+class MAPPO_Clip_Agents(MARLAgents):
     def __init__(self,
                  config: Namespace,
                  envs: DummyVecEnv_MAS,
-                 device: str = "cpu:0"):
+                 device: Optional[Union[int, str, torch.device]] = None):
         self.comm = MPI.COMM_WORLD
 
         self.gamma = config.gamma
         self.use_obsnorm = config.use_obsnorm
         self.use_rewnorm = config.use_rewnorm
         self.obsnorm_range = config.obsnorm_range
         self.rewnorm_range = config.rewnorm_range
 
+        if config.state_space is not None:
+            config.dim_state, state_shape = config.state_space.shape, config.state_space.shape
+        else:
+            config.dim_state, state_shape = None, None
+
         input_representation = get_repre_in(config)
         representation = REGISTRY_Representation[config.representation](*input_representation)
+
         input_policy = get_policy_in_marl(config, representation, config.agent_keys)
         policy = REGISTRY_Policy[config.policy](*input_policy)
-        lr_scheduler = [MyLinearLR(config.lr_a, start_factor=1.0, end_factor=0.5,
-                                   total_iters=get_total_iters(config.agent_name, config)),
-                        MyLinearLR(config.lr_c, start_factor=1.0, end_factor=0.5,
-                                   total_iters=get_total_iters(config.agent_name, config))]
-        optimizer = [tk.optimizers.Adam(lr_scheduler[0]),
-                     tk.optimizers.Adam(lr_scheduler[1])]
+        optimizer = torch.optim.Adam(policy.parameters(), config.learning_rate, eps=1e-5)
+        scheduler = torch.optim.lr_scheduler.LinearLR(optimizer, start_factor=1.0, end_factor=0.5,
+                                                      total_iters=get_total_iters(config.agent_name, config))
         self.observation_space = envs.observation_space
         self.action_space = envs.action_space
         self.representation_info_shape = policy.representation.output_shapes
         self.auxiliary_info_shape = {}
 
         writer = SummaryWriter(config.logdir)
         if config.state_space is not None:
             config.dim_state, state_shape = config.state_space.shape, config.state_space.shape
         else:
             config.dim_state, state_shape = None, None
-        memory = MARL_OffPolicyBuffer(state_shape,
-                                      config.obs_shape,
-                                      config.act_shape,
-                                      config.rew_shape,
-                                      config.done_shape,
-                                      envs.num_envs,
-                                      config.buffer_size,
-                                      config.batch_size)
-        learner = MADDPG_Learner(config, policy, optimizer, writer,
-                                 config.device, config.modeldir, config.gamma)
+        memory = MARL_OnPolicyBuffer(state_shape, config.obs_shape, config.act_shape, config.rew_shape,
+                                     config.done_shape, envs.num_envs, config.nsteps, config.nminibatch,
+                                     config.use_gae, config.use_advnorm, config.gamma, config.lam)
+        learner = MAPPO_Clip_Learner(config, policy, optimizer, scheduler, writer,
+                                     config.device, config.modeldir, config.gamma)
 
         self.obs_rms = RunningMeanStd(shape=space2shape(self.observation_space[config.agent_keys[0]]),
                                       comm=self.comm, use_mpi=False)
         self.ret_rms = RunningMeanStd(shape=(), comm=self.comm, use_mpi=False)
-        super(MADDPG_Agents, self).__init__(config, envs, policy, memory, learner, writer, device,
-                                            config.logdir, config.modeldir)
+        super(MAPPO_Clip_Agents, self).__init__(config, envs, policy, memory, learner, writer, device,
+                                                config.logdir, config.modeldir)
 
     def _process_observation(self, observations):
         if self.use_obsnorm:
             if isinstance(self.observation_space, Dict):
                 for key in self.observation_space.spaces.keys():
                     observations[key] = np.clip(
                         (observations[key] - self.obs_rms.mean[key]) / (self.obs_rms.std[key] + EPS),
@@ -66,22 +64,32 @@
 
     def _process_reward(self, rewards):
         if self.use_rewnorm:
             std = np.clip(self.ret_rms.std, 0.1, 100)
             return np.clip(rewards / std, -self.rewnorm_range, self.rewnorm_range)
         return rewards
 
-    def act(self, obs_n, episode, test_mode, noise=False):
+    def act(self, obs_n, episode, test_mode, state=None, noise=False):
         batch_size = len(obs_n)
-        with tf.device(self.device):
-            agents_id = tf.tile(tf.expand_dims(tf.eye(self.n_agents), axis=0), multiples=(batch_size, 1, 1))
-            inputs_policy = {"obs": tf.convert_to_tensor(obs_n), "ids": agents_id}
-            _, actions = self.policy(inputs_policy)
-        actions = actions.numpy()
-        if noise:
-            actions += np.random.normal(0, self.args.sigma, size=actions.shape)
-        return actions
+        agents_id = torch.eye(self.n_agents).unsqueeze(0).expand(batch_size, -1, -1).to(self.device)
+        _, dists = self.policy(obs_n, agents_id)
+        acts = dists.stochastic_sample()
+        log_pi_a = dists.log_prob(acts)
+        state_expand = torch.Tensor(state).unsqueeze(-2).expand(-1, self.n_agents, -1).to(self.device)
+        vs = self.policy.values(state_expand, agents_id)
+        return acts.detach().cpu().numpy(), log_pi_a.detach().cpu().numpy(), vs.detach().cpu().numpy()
+
+    def value(self, obs, state):
+        batch_size = len(state)
+        agents_id = torch.eye(self.n_agents).unsqueeze(0).expand(batch_size, -1, -1).to(self.device)
+        repre_out = self.policy.representation(obs)
+        critic_input = torch.concat([torch.Tensor(repre_out['state']), agents_id], dim=-1)
+        values_n = self.policy.critic(critic_input)
+        values = self.policy.value_tot(values_n, global_state=state).view(-1, 1).repeat(1, self.n_agents).unsqueeze(-1)
+        return values.detach().cpu().numpy()
 
     def train(self, i_episode):
-        if self.memory.can_sample(self.args.batch_size):
-            sample = self.memory.sample()
-            self.learner.update(sample)
+        if self.memory.full:
+            for _ in range(self.args.nminibatch * self.args.nepoch):
+                sample = self.memory.sample()
+                self.learner.update(sample)
+            self.memory.clear()
```

### Comparing `xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_tf/agents/multi_agent_rl/mappoclip_agents.py` & `xuanpolicy-0.1.6/xuanpolicy/tensorflow/agents/multi_agent_rl/mfac_agents.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-from xuanpolicy.xuanpolicy_tf.agents import *
+from xuanpolicy.tensorflow.agents import *
 
 
-class MAPPO_Clip_Agents(MARLAgents):
+class MFAC_Agents(MARLAgents):
     def __init__(self,
                  config: Namespace,
                  envs: DummyVecEnv_MAS,
                  device: str = "cpu:0"):
         self.comm = MPI.COMM_WORLD
 
         self.gamma = config.gamma
@@ -17,41 +17,46 @@
         if config.state_space is not None:
             config.dim_state, state_shape = config.state_space.shape, config.state_space.shape
         else:
             config.dim_state, state_shape = None, None
 
         input_representation = get_repre_in(config)
         representation = REGISTRY_Representation[config.representation](*input_representation)
-
         input_policy = get_policy_in_marl(config, representation, config.agent_keys)
         policy = REGISTRY_Policy[config.policy](*input_policy)
-        lr_scheduler = MyLinearLR(config.learning_rate, start_factor=1.0, end_factor=0.5,
-                                  total_iters=get_total_iters(config.agent_name, config))
-        optimizer = tk.optimizers.Adam(lr_scheduler)
+        lr_scheduler = [MyLinearLR(config.lr_a, start_factor=1.0, end_factor=0.5, total_iters=get_total_iters(config.agent_name, config)),
+                        MyLinearLR(config.lr_c, start_factor=1.0, end_factor=0.5, total_iters=get_total_iters(config.agent_name, config))]
+        optimizer = [tk.optimizers.Adam(lr_scheduler[0]), tk.optimizers.Adam(lr_scheduler[1])]
         self.observation_space = envs.observation_space
         self.action_space = envs.action_space
         self.representation_info_shape = policy.representation.output_shapes
         self.auxiliary_info_shape = {}
 
         writer = SummaryWriter(config.logdir)
         if config.state_space is not None:
             config.dim_state, state_shape = config.state_space.shape, config.state_space.shape
         else:
             config.dim_state, state_shape = None, None
-        memory = MARL_OnPolicyBuffer(state_shape, config.obs_shape, config.act_shape, config.rew_shape,
-                                     config.done_shape, envs.num_envs, config.nsteps, config.nminibatch,
-                                     config.use_gae, config.use_advnorm, config.gamma, config.lam)
-        learner = MAPPO_Clip_Learner(config, policy, optimizer, writer,
-                                     config.device, config.modeldir, config.gamma)
+        memory = MeanField_OnPolicyBuffer(state_shape,
+                                          config.obs_shape,
+                                          config.act_shape,
+                                          config.act_prob_shape,
+                                          config.rew_shape,
+                                          config.done_shape,
+                                          envs.num_envs,
+                                          config.nsteps,
+                                          config.nminibatch,
+                                          config.use_gae, config.use_advnorm, config.gamma, config.lam)
+        learner = MFAC_Learner(config, policy, optimizer, writer, config.device, config.modeldir, config.gamma)
 
         self.obs_rms = RunningMeanStd(shape=space2shape(self.observation_space[config.agent_keys[0]]),
                                       comm=self.comm, use_mpi=False)
         self.ret_rms = RunningMeanStd(shape=(), comm=self.comm, use_mpi=False)
-        super(MAPPO_Clip_Agents, self).__init__(config, envs, policy, memory, learner, writer, device,
-                                                config.logdir, config.modeldir)
+        super(MFAC_Agents, self).__init__(config, envs, policy, memory, learner, writer, device,
+                                          config.logdir, config.modeldir)
 
     def _process_observation(self, observations):
         if self.use_obsnorm:
             if isinstance(self.observation_space, Dict):
                 for key in self.observation_space.spaces.keys():
                     observations[key] = np.clip(
                         (observations[key] - self.obs_rms.mean[key]) / (self.obs_rms.std[key] + EPS),
@@ -64,35 +69,36 @@
 
     def _process_reward(self, rewards):
         if self.use_rewnorm:
             std = np.clip(self.ret_rms.std, 0.1, 100)
             return np.clip(rewards / std, -self.rewnorm_range, self.rewnorm_range)
         return rewards
 
-    def act(self, obs_n, episode, test_mode, state=None, noise=False):
+    def act(self, obs_n, episode, test_mode, act_mean=None, agent_mask=None, noise=False):
         batch_size = len(obs_n)
-        with tf.device(self.device):
-            agents_id = tf.tile(tf.expand_dims(tf.eye(self.n_agents), axis=0), multiples=(batch_size, 1, 1))
-            inputs_policy = {"obs": tf.convert_to_tensor(obs_n), "ids": agents_id}
-            _, dists = self.policy(inputs_policy)
-            acts = dists.stochastic_sample()
-            log_pi_a = dists.log_prob(acts)
-            state = tf.convert_to_tensor(state)
-            state_expand = tf.tile(tf.expand_dims(state, axis=-2), (1, self.n_agents, 1))
-            vs = self.policy.values(state_expand, agents_id)
-        return acts.numpy(), log_pi_a.numpy(), vs.numpy()
+        inputs = {"obs": obs_n,
+                  "ids": np.tile(np.expand_dims(np.eye(self.n_agents), 0), (batch_size, 1, 1))}
+        _, dists = self.policy(inputs)
+        acts = dists.stochastic_sample()
+
+        n_alive = np.expand_dims(np.sum(agent_mask, axis=-1), axis=-1).repeat(self.dim_act, axis=1)
+        action_n_mask = np.expand_dims(agent_mask, axis=-1).repeat(self.dim_act, axis=-1)
+        act_neighbor_onehot = self.learner.onehot_action(acts, self.dim_act).numpy() * action_n_mask
+        act_mean_current = np.sum(act_neighbor_onehot, axis=1) / n_alive
+
+        return acts.numpy(), act_mean_current
 
     def value(self, obs, state):
         batch_size = len(state)
-        agents_id = tf.tile(tf.expand_dims(tf.eye(self.n_agents), axis=0), multiples=(batch_size, 1, 1))
+        agents_id = np.tile(np.expand_dims(np.eye(self.n_agents), 0), (batch_size, 1, 1))
         repre_out = self.policy.representation(obs)
-        critic_input = tf.concat([torch.Tensor(repre_out['state']), agents_id], axis=-1)
+        critic_input = tf.concat([repre_out['state'], agents_id], axis=-1)
         values_n = self.policy.critic(critic_input)
-        values = self.policy.value_tot(values_n, global_state=state)
-        values = tf.expand_dims(tf.tile(tf.reshape(values, (-1, 1)), (1, self.n_agents)), axis=-1)
+
+        values = tf.expand_dims(tf.tile(tf.reshape(self.policy.value_tot(values_n, global_state=state), [-1, 1]), (1, self.n_agents)), axis=-1)
         return values.numpy()
 
     def train(self, i_episode):
         if self.memory.full:
             for _ in range(self.args.nminibatch * self.args.nepoch):
                 sample = self.memory.sample()
                 self.learner.update(sample)
```

### Comparing `xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_tf/agents/multi_agent_rl/mappokl_agents.py` & `xuanpolicy-0.1.6/xuanpolicy/torch/agents/multi_agent_rl/vdn_agents.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,57 +1,65 @@
-from xuanpolicy.xuanpolicy_tf.agents import *
+from xuanpolicy.torch.agents import *
+from xuanpolicy.torch.agents.agents_marl import linear_decay_or_increase
 
 
-class MAPPO_KL_Agents(MARLAgents):
+class VDN_Agents(MARLAgents):
     def __init__(self,
                  config: Namespace,
                  envs: DummyVecEnv_MAS,
-                 device: str = "cpu:0"):
+                 device: Optional[Union[int, str, torch.device]] = None):
         self.comm = MPI.COMM_WORLD
 
         self.gamma = config.gamma
         self.use_obsnorm = config.use_obsnorm
         self.use_rewnorm = config.use_rewnorm
         self.obsnorm_range = config.obsnorm_range
         self.rewnorm_range = config.rewnorm_range
 
-        if config.state_space is not None:
-            config.dim_state, state_shape = config.state_space.shape, config.state_space.shape
-        else:
-            config.dim_state, state_shape = None, None
+        self.start_greedy = config.start_greedy
+        self.end_greedy = config.end_greedy
+        self.egreedy = config.start_greedy
 
         input_representation = get_repre_in(config)
         representation = REGISTRY_Representation[config.representation](*input_representation)
-
-        input_policy = get_policy_in_marl(config, representation, config.agent_keys)
+        mixer = VDN_mixer()
+        input_policy = get_policy_in_marl(config, representation, config.agent_keys, mixer)
         policy = REGISTRY_Policy[config.policy](*input_policy)
-        lr_scheduler = MyLinearLR(config.learning_rate, start_factor=1.0, end_factor=0.5,
-                                  total_iters=get_total_iters(config.agent_name, config))
-        optimizer = tk.optimizers.Adam(lr_scheduler)
+        optimizer = torch.optim.Adam(policy.parameters(), config.learning_rate, eps=1e-5)
+        scheduler = torch.optim.lr_scheduler.LinearLR(optimizer, start_factor=1.0, end_factor=0.5,
+                                                      total_iters=get_total_iters(config.agent_name, config))
         self.observation_space = envs.observation_space
         self.action_space = envs.action_space
         self.representation_info_shape = policy.representation.output_shapes
         self.auxiliary_info_shape = {}
 
         writer = SummaryWriter(config.logdir)
         if config.state_space is not None:
             config.dim_state, state_shape = config.state_space.shape, config.state_space.shape
         else:
             config.dim_state, state_shape = None, None
-        memory = MARL_OnPolicyBuffer(state_shape, config.obs_shape, config.act_shape, config.rew_shape,
-                                     config.done_shape, envs.num_envs, config.nsteps, config.nminibatch,
-                                     config.use_gae, config.use_advnorm, config.gamma, config.lam)
-        learner = MAPPO_KL_Learner(config, policy, optimizer, writer,
-                                   config.device, config.modeldir, config.gamma)
+        memory = MARL_OffPolicyBuffer(state_shape,
+                                      config.obs_shape,
+                                      config.act_shape,
+                                      config.rew_shape,
+                                      config.done_shape,
+                                      envs.num_envs,
+                                      config.buffer_size,
+                                      config.batch_size)
+        learner = VDN_Learner(config, policy, optimizer, scheduler, writer,
+                              config.device, config.modeldir, config.gamma,
+                              config.sync_frequency)
 
         self.obs_rms = RunningMeanStd(shape=space2shape(self.observation_space[config.agent_keys[0]]),
                                       comm=self.comm, use_mpi=False)
         self.ret_rms = RunningMeanStd(shape=(), comm=self.comm, use_mpi=False)
-        super(MAPPO_KL_Agents, self).__init__(config, envs, policy, memory, learner, writer, device,
-                                              config.logdir, config.modeldir)
+        self.epsilon_decay = linear_decay_or_increase(config.start_greedy, config.end_greedy,
+                                                      config.greedy_update_steps)
+        super(VDN_Agents, self).__init__(config, envs, policy, memory, learner, writer, device,
+                                         config.logdir, config.modeldir)
 
     def _process_observation(self, observations):
         if self.use_obsnorm:
             if isinstance(self.observation_space, Dict):
                 for key in self.observation_space.spaces.keys():
                     observations[key] = np.clip(
                         (observations[key] - self.obs_rms.mean[key]) / (self.obs_rms.std[key] + EPS),
@@ -64,35 +72,14 @@
 
     def _process_reward(self, rewards):
         if self.use_rewnorm:
             std = np.clip(self.ret_rms.std, 0.1, 100)
             return np.clip(rewards / std, -self.rewnorm_range, self.rewnorm_range)
         return rewards
 
-    def act(self, obs_n, episode, test_mode, state=None, noise=False):
-        batch_size = len(obs_n)
-        with tf.device(self.device):
-            agents_id = tf.tile(tf.expand_dims(tf.eye(self.n_agents), axis=0), multiples=(batch_size, 1, 1))
-            inputs_policy = {"obs": tf.convert_to_tensor(obs_n), "ids": agents_id}
-            _, dists = self.policy(inputs_policy)
-            acts = dists.stochastic_sample()
-            state = tf.convert_to_tensor(state)
-            state_expand = tf.tile(tf.expand_dims(state, axis=-2), (1, self.n_agents, 1))
-            vs = self.policy.values(state_expand, agents_id)
-        return acts.numpy(), split_distributions(dists), vs.numpy()
-
-    def value(self, obs, state):
-        batch_size = len(state)
-        agents_id = tf.tile(tf.expand_dims(tf.eye(self.n_agents), axis=0), multiples=(batch_size, 1, 1))
-        repre_out = self.policy.representation(obs)
-        critic_input = tf.concat([torch.Tensor(repre_out['state']), agents_id], axis=-1)
-        values_n = self.policy.critic(critic_input)
-        values = self.policy.value_tot(values_n, global_state=state)
-        values = tf.expand_dims(tf.tile(tf.reshape(values, (-1, 1)), (1, self.n_agents)), axis=-1)
-        return values.numpy()
-
     def train(self, i_episode):
-        if self.memory.full:
-            for _ in range(self.args.nminibatch * self.args.nepoch):
-                sample = self.memory.sample()
-                self.learner.update(sample)
-            self.memory.clear()
+        self.epsilon_decay.update()
+        for i in range(self.nenvs):
+            self.writer.add_scalars("epsilon", {"env-%d" % i: self.epsilon_decay.epsilon}, i_episode)
+        if self.memory.can_sample(self.args.batch_size):
+            sample = self.memory.sample()
+            self.learner.update(sample)
```

### Comparing `xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_tf/agents/multi_agent_rl/masac_agents.py` & `xuanpolicy-0.1.6/xuanpolicy/torch/agents/multi_agent_rl/wqmix_agents.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,57 +1,67 @@
-from xuanpolicy.xuanpolicy_tf.agents import *
+from xuanpolicy.torch.agents import *
+from xuanpolicy.torch.agents.agents_marl import linear_decay_or_increase
 
 
-class MASAC_Agents(MARLAgents):
+class WQMIX_Agents(MARLAgents):
     def __init__(self,
                  config: Namespace,
                  envs: DummyVecEnv_MAS,
-                 device: str = "cpu:0"):
+                 device: Optional[Union[int, str, torch.device]] = None):
         self.comm = MPI.COMM_WORLD
 
+        self.alpha = config.alpha
         self.gamma = config.gamma
         self.use_obsnorm = config.use_obsnorm
         self.use_rewnorm = config.use_rewnorm
         self.obsnorm_range = config.obsnorm_range
         self.rewnorm_range = config.rewnorm_range
 
+        self.start_greedy = config.start_greedy
+        self.end_greedy = config.end_greedy
+        self.egreedy = config.start_greedy
+        if config.state_space is not None:
+            config.dim_state, state_shape = config.state_space.shape, config.state_space.shape
+        else:
+            config.dim_state, state_shape = None, None
+
         input_representation = get_repre_in(config)
         representation = REGISTRY_Representation[config.representation](*input_representation)
-        input_policy = get_policy_in_marl(config, representation, config.agent_keys)
+        mixer = QMIX_mixer(config.dim_state[0], config.hidden_dim_mixing_net, config.hidden_dim_hyper_net,
+                           config.n_agents, device)
+        ff_mixer = QMIX_FF_mixer(config.dim_state[0], config.hidden_dim_mixing_net, config.n_agents, device)
+        input_policy = get_policy_in_marl(config, representation, config.agent_keys, mixer, ff_mixer)
         policy = REGISTRY_Policy[config.policy](*input_policy)
-        lr_scheduler = [MyLinearLR(config.lr_a, start_factor=1.0, end_factor=0.5,
-                                   total_iters=get_total_iters(config.agent_name, config)),
-                        MyLinearLR(config.lr_c, start_factor=1.0, end_factor=0.5,
-                                   total_iters=get_total_iters(config.agent_name, config))]
-        optimizer = [tk.optimizers.Adam(lr_scheduler[0]),
-                     tk.optimizers.Adam(lr_scheduler[1])]
+        optimizer = torch.optim.Adam(policy.parameters(), config.learning_rate, eps=1e-5)
+        scheduler = torch.optim.lr_scheduler.LinearLR(optimizer, start_factor=1.0, end_factor=0.5,
+                                                      total_iters=get_total_iters(config.agent_name, config))
         self.observation_space = envs.observation_space
         self.action_space = envs.action_space
         self.representation_info_shape = policy.representation.output_shapes
         self.auxiliary_info_shape = {}
 
         writer = SummaryWriter(config.logdir)
-        if config.state_space is not None:
-            config.dim_state, state_shape = config.state_space.shape, config.state_space.shape
-        else:
-            config.dim_state, state_shape = None, None
         memory = MARL_OffPolicyBuffer(state_shape,
                                       config.obs_shape,
                                       config.act_shape,
                                       config.rew_shape,
                                       config.done_shape,
                                       envs.num_envs,
                                       config.buffer_size,
                                       config.batch_size)
-        learner = MASAC_Learner(config, policy, optimizer, writer, config.device, config.modeldir, config.gamma)
+        learner = WQMIX_Learner(config, policy, optimizer, scheduler, writer,
+                                config.device, config.modeldir, config.gamma,
+                                config.sync_frequency)
 
         self.obs_rms = RunningMeanStd(shape=space2shape(self.observation_space[config.agent_keys[0]]),
                                       comm=self.comm, use_mpi=False)
         self.ret_rms = RunningMeanStd(shape=(), comm=self.comm, use_mpi=False)
-        super(MASAC_Agents, self).__init__(config, envs, policy, memory, learner, writer, device,
+        self.epsilon_decay = linear_decay_or_increase(config.start_greedy, config.end_greedy,
+                                                      config.greedy_update_steps)
+        super(WQMIX_Agents, self).__init__(config, envs, policy, memory, learner, writer, device,
                                            config.logdir, config.modeldir)
 
     def _process_observation(self, observations):
         if self.use_obsnorm:
             if isinstance(self.observation_space, Dict):
                 for key in self.observation_space.spaces.keys():
                     observations[key] = np.clip(
@@ -65,21 +75,14 @@
 
     def _process_reward(self, rewards):
         if self.use_rewnorm:
             std = np.clip(self.ret_rms.std, 0.1, 100)
             return np.clip(rewards / std, -self.rewnorm_range, self.rewnorm_range)
         return rewards
 
-    def act(self, obs_n, episode, test_mode, state=None, noise=False):
-        batch_size = len(obs_n)
-        with tf.device(self.device):
-            agents_id = tf.tile(tf.expand_dims(tf.eye(self.n_agents), axis=0), multiples=(batch_size, 1, 1))
-            inputs_policy = {"obs": tf.convert_to_tensor(obs_n), "ids": agents_id}
-            _, dists = self.policy(inputs_policy)
-            acts = dists.sample()
-        actions = acts.numpy()
-        return actions
-
     def train(self, i_episode):
+        self.epsilon_decay.update()
+        for i in range(self.nenvs):
+            self.writer.add_scalars("epsilon", {"env-%d" % i: self.epsilon_decay.epsilon}, i_episode)
         if self.memory.can_sample(self.args.batch_size):
             sample = self.memory.sample()
             self.learner.update(sample)
```

### Comparing `xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_tf/agents/multi_agent_rl/matd3_agents.py` & `xuanpolicy-0.1.6/xuanpolicy/torch/agents/multi_agent_rl/mappokl_agents.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,59 +1,57 @@
-from xuanpolicy.xuanpolicy_tf.agents import *
+from xuanpolicy.torch.agents import *
 
 
-class MATD3_Agents(MARLAgents):
+class MAPPO_KL_Agents(MARLAgents):
     def __init__(self,
                  config: Namespace,
                  envs: DummyVecEnv_MAS,
-                 device: str = "cpu:0"):
+                 device: Optional[Union[int, str, torch.device]] = None):
         self.comm = MPI.COMM_WORLD
 
         self.gamma = config.gamma
         self.use_obsnorm = config.use_obsnorm
         self.use_rewnorm = config.use_rewnorm
         self.obsnorm_range = config.obsnorm_range
         self.rewnorm_range = config.rewnorm_range
 
+        if config.state_space is not None:
+            config.dim_state, state_shape = config.state_space.shape, config.state_space.shape
+        else:
+            config.dim_state, state_shape = None, None
+
         input_representation = get_repre_in(config)
         representation = REGISTRY_Representation[config.representation](*input_representation)
+
         input_policy = get_policy_in_marl(config, representation, config.agent_keys)
         policy = REGISTRY_Policy[config.policy](*input_policy)
-        lr_scheduler = [MyLinearLR(config.lr_a, start_factor=1.0, end_factor=0.5,
-                                   total_iters=get_total_iters(config.agent_name, config)),
-                        MyLinearLR(config.lr_c, start_factor=1.0, end_factor=0.5,
-                                   total_iters=get_total_iters(config.agent_name, config))]
-        optimizer = [tk.optimizers.Adam(lr_scheduler[0]),
-                     tk.optimizers.Adam(lr_scheduler[1])]
+        optimizer = torch.optim.Adam(policy.parameters(), config.learning_rate, eps=1e-5)
+        scheduler = torch.optim.lr_scheduler.LinearLR(optimizer, start_factor=1.0, end_factor=0.5,
+                                                      total_iters=get_total_iters(config.agent_name, config))
         self.observation_space = envs.observation_space
         self.action_space = envs.action_space
         self.representation_info_shape = policy.representation.output_shapes
         self.auxiliary_info_shape = {}
 
         writer = SummaryWriter(config.logdir)
         if config.state_space is not None:
             config.dim_state, state_shape = config.state_space.shape, config.state_space.shape
         else:
             config.dim_state, state_shape = None, None
-        memory = MARL_OffPolicyBuffer(state_shape,
-                                      config.obs_shape,
-                                      config.act_shape,
-                                      config.rew_shape,
-                                      config.done_shape,
-                                      envs.num_envs,
-                                      config.buffer_size,
-                                      config.batch_size)
-        learner = MATD3_Learner(config, policy, optimizer, writer,
-                                 config.device, config.modeldir, config.gamma)
+        memory = MARL_OnPolicyBuffer(state_shape, config.obs_shape, config.act_shape, config.rew_shape,
+                                     config.done_shape, envs.num_envs, config.nsteps, config.nminibatch,
+                                     config.use_gae, config.use_advnorm, config.gamma, config.lam)
+        learner = MAPPO_KL_Learner(config, policy, optimizer, scheduler, writer,
+                                   config.device, config.modeldir, config.gamma)
 
         self.obs_rms = RunningMeanStd(shape=space2shape(self.observation_space[config.agent_keys[0]]),
                                       comm=self.comm, use_mpi=False)
         self.ret_rms = RunningMeanStd(shape=(), comm=self.comm, use_mpi=False)
-        super(MATD3_Agents, self).__init__(config, envs, policy, memory, learner, writer, device,
-                                            config.logdir, config.modeldir)
+        super(MAPPO_KL_Agents, self).__init__(config, envs, policy, memory, learner, writer, device,
+                                              config.logdir, config.modeldir)
 
     def _process_observation(self, observations):
         if self.use_obsnorm:
             if isinstance(self.observation_space, Dict):
                 for key in self.observation_space.spaces.keys():
                     observations[key] = np.clip(
                         (observations[key] - self.obs_rms.mean[key]) / (self.obs_rms.std[key] + EPS),
@@ -66,22 +64,31 @@
 
     def _process_reward(self, rewards):
         if self.use_rewnorm:
             std = np.clip(self.ret_rms.std, 0.1, 100)
             return np.clip(rewards / std, -self.rewnorm_range, self.rewnorm_range)
         return rewards
 
-    def act(self, obs_n, episode, test_mode, noise=False):
+    def act(self, obs_n, episode, test_mode, state=None, noise=False):
         batch_size = len(obs_n)
-        with tf.device(self.device):
-            agents_id = tf.tile(tf.expand_dims(tf.eye(self.n_agents), axis=0), multiples=(batch_size, 1, 1))
-            inputs_policy = {"obs": tf.convert_to_tensor(obs_n), "ids": agents_id}
-            _, actions = self.policy(inputs_policy)
-        actions = actions.numpy()
-        if noise:
-            actions += np.random.normal(0, self.args.sigma, size=actions.shape)
-        return actions
+        agents_id = torch.eye(self.n_agents).unsqueeze(0).expand(batch_size, -1, -1).to(self.device)
+        _, dists = self.policy(obs_n, agents_id)
+        acts = dists.stochastic_sample()
+        state_expand = torch.Tensor(state).unsqueeze(-2).expand(-1, self.n_agents, -1).to(self.device)
+        vs = self.policy.values(state_expand, agents_id)
+        return acts.detach().cpu().numpy(), split_distributions(dists), vs.detach().cpu().numpy()
+
+    def value(self, obs, state):
+        batch_size = len(state)
+        agents_id = torch.eye(self.n_agents).unsqueeze(0).expand(batch_size, -1, -1).to(self.device)
+        repre_out = self.policy.representation(obs)
+        critic_input = torch.concat([torch.Tensor(repre_out['state']), agents_id], dim=-1)
+        values_n = self.policy.critic(critic_input)
+        values = self.policy.value_tot(values_n, global_state=state).view(-1, 1).repeat(1, self.n_agents).unsqueeze(-1)
+        return values.detach().cpu().numpy()
 
     def train(self, i_episode):
-        if self.memory.can_sample(self.args.batch_size):
-            sample = self.memory.sample()
-            self.learner.update(sample)
+        if self.memory.full:
+            for _ in range(self.args.nminibatch * self.args.nepoch):
+                sample = self.memory.sample()
+                self.learner.update(sample)
+            self.memory.clear()
```

### Comparing `xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_tf/agents/multi_agent_rl/mfac_agents.py` & `xuanpolicy-0.1.6/xuanpolicy/torch/agents/multi_agent_rl/coma_agents.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,61 +1,63 @@
-from xuanpolicy.xuanpolicy_tf.agents import *
+from xuanpolicy.torch.agents import *
+from xuanpolicy.torch.agents.agents_marl import linear_decay_or_increase
 
 
-class MFAC_Agents(MARLAgents):
+class COMA_Agents(MARLAgents):
     def __init__(self,
                  config: Namespace,
                  envs: DummyVecEnv_MAS,
-                 device: str = "cpu:0"):
+                 device: Optional[Union[int, str, torch.device]] = None):
         self.comm = MPI.COMM_WORLD
+        config.batch_size = config.batch_size * envs.num_envs
 
         self.gamma = config.gamma
         self.use_obsnorm = config.use_obsnorm
         self.use_rewnorm = config.use_rewnorm
         self.obsnorm_range = config.obsnorm_range
         self.rewnorm_range = config.rewnorm_range
 
         if config.state_space is not None:
             config.dim_state, state_shape = config.state_space.shape, config.state_space.shape
         else:
             config.dim_state, state_shape = None, None
 
         input_representation = get_repre_in(config)
         representation = REGISTRY_Representation[config.representation](*input_representation)
-        input_policy = get_policy_in_marl(config, representation, config.agent_keys)
+        input_policy = get_policy_in_marl(config, representation, config.agent_keys, None)
         policy = REGISTRY_Policy[config.policy](*input_policy)
-        lr_scheduler = [MyLinearLR(config.lr_a, start_factor=1.0, end_factor=0.5, total_iters=get_total_iters(config.agent_name, config)),
-                        MyLinearLR(config.lr_c, start_factor=1.0, end_factor=0.5, total_iters=get_total_iters(config.agent_name, config))]
-        optimizer = [tk.optimizers.Adam(lr_scheduler[0]), tk.optimizers.Adam(lr_scheduler[1])]
+        optimizer = [torch.optim.Adam(policy.parameters_actor, config.learning_rate_actor, eps=1e-5),
+                     torch.optim.Adam(policy.parameters_critic, config.learning_rate_critic, eps=1e-5)]
+        scheduler = [torch.optim.lr_scheduler.LinearLR(optimizer[0], start_factor=1.0, end_factor=0.5,
+                                                       total_iters=get_total_iters(config.agent_name, config)),
+                     torch.optim.lr_scheduler.LinearLR(optimizer[1], start_factor=1.0, end_factor=0.5,
+                                                       total_iters=get_total_iters(config.agent_name, config))]
         self.observation_space = envs.observation_space
         self.action_space = envs.action_space
         self.representation_info_shape = policy.representation.output_shapes
         self.auxiliary_info_shape = {}
 
         writer = SummaryWriter(config.logdir)
         if config.state_space is not None:
             config.dim_state, state_shape = config.state_space.shape, config.state_space.shape
         else:
             config.dim_state, state_shape = None, None
-        memory = MeanField_OnPolicyBuffer(state_shape,
-                                          config.obs_shape,
-                                          config.act_shape,
-                                          config.act_prob_shape,
-                                          config.rew_shape,
-                                          config.done_shape,
-                                          envs.num_envs,
-                                          config.nsteps,
-                                          config.nminibatch,
-                                          config.use_gae, config.use_advnorm, config.gamma, config.lam)
-        learner = MFAC_Learner(config, policy, optimizer, writer, config.device, config.modeldir, config.gamma)
+        config.act_onehot_shape = config.act_shape + tuple([config.dim_act])
+        memory = COMA_Buffer(state_shape, config.obs_shape, config.act_shape, config.act_onehot_shape,
+                             config.rew_shape, config.done_shape, envs.num_envs,
+                             config.buffer_size, config.batch_size, envs.envs[0].max_cycles)
+        learner = COMA_Learner(config, policy, optimizer, scheduler, writer,
+                               config.device, config.modeldir, config.gamma, config.sync_frequency)
 
         self.obs_rms = RunningMeanStd(shape=space2shape(self.observation_space[config.agent_keys[0]]),
                                       comm=self.comm, use_mpi=False)
         self.ret_rms = RunningMeanStd(shape=(), comm=self.comm, use_mpi=False)
-        super(MFAC_Agents, self).__init__(config, envs, policy, memory, learner, writer, device,
+        self.epsilon_decay = linear_decay_or_increase(config.start_greedy, config.end_greedy,
+                                                      config.greedy_update_steps)
+        super(COMA_Agents, self).__init__(config, envs, policy, memory, learner, writer, device,
                                           config.logdir, config.modeldir)
 
     def _process_observation(self, observations):
         if self.use_obsnorm:
             if isinstance(self.observation_space, Dict):
                 for key in self.observation_space.spaces.keys():
                     observations[key] = np.clip(
@@ -69,37 +71,33 @@
 
     def _process_reward(self, rewards):
         if self.use_rewnorm:
             std = np.clip(self.ret_rms.std, 0.1, 100)
             return np.clip(rewards / std, -self.rewnorm_range, self.rewnorm_range)
         return rewards
 
-    def act(self, obs_n, episode, test_mode, act_mean=None, agent_mask=None, noise=False):
+    def act(self, obs_n, episode, test_mode, noise=False):
         batch_size = len(obs_n)
-        inputs = {"obs": obs_n,
-                  "ids": np.tile(np.expand_dims(np.eye(self.n_agents), 0), (batch_size, 1, 1))}
-        _, dists = self.policy(inputs)
-        acts = dists.stochastic_sample()
-
-        n_alive = np.expand_dims(np.sum(agent_mask, axis=-1), axis=-1).repeat(self.dim_act, axis=1)
-        action_n_mask = np.expand_dims(agent_mask, axis=-1).repeat(self.dim_act, axis=-1)
-        act_neighbor_onehot = self.learner.onehot_action(acts, self.dim_act).numpy() * action_n_mask
-        act_mean_current = np.sum(act_neighbor_onehot, axis=1) / n_alive
-
-        return acts.numpy(), act_mean_current
-
-    def value(self, obs, state):
-        batch_size = len(state)
-        agents_id = np.tile(np.expand_dims(np.eye(self.n_agents), 0), (batch_size, 1, 1))
-        repre_out = self.policy.representation(obs)
-        critic_input = tf.concat([repre_out['state'], agents_id], axis=-1)
-        values_n = self.policy.critic(critic_input)
-
-        values = tf.expand_dims(tf.tile(tf.reshape(self.policy.value_tot(values_n, global_state=state), [-1, 1]), (1, self.n_agents)), axis=-1)
-        return values.numpy()
+        agents_id = torch.eye(self.n_agents).unsqueeze(0).expand(batch_size, -1, -1).to(self.device)
+        states, dists = self.policy(obs_n, agents_id)
+        # acts = dists.stochastic_sample()  # stochastic policy
+        epsilon = 1.0 if test_mode else self.epsilon_decay.epsilon
+        greedy_actions = dists.logits.argmax(dim=-1, keepdims=False)
+        if noise:
+            random_variable = np.random.random(greedy_actions.shape)
+            action_pick = np.int32((random_variable < epsilon))
+            random_actions = np.array([[self.args.action_space[agent].sample() for agent in self.agent_keys]])
+            actions_select = action_pick * greedy_actions.cpu().numpy() + (1 - action_pick) * random_actions
+            actions_onehot = self.learner.onehot_action(torch.Tensor(actions_select), self.dim_act)
+            return actions_select, actions_onehot.detach().cpu().numpy()
+        else:
+            actions_onehot = self.learner.onehot_action(greedy_actions, self.dim_act)
+            return greedy_actions.detach().cpu().numpy(), actions_onehot.detach().cpu().numpy()
 
     def train(self, i_episode):
+        self.epsilon_decay.update()
+        for i in range(self.nenvs):
+            self.writer.add_scalars("epsilon", {"env-%d" % i: self.epsilon_decay.epsilon}, i_episode)
         if self.memory.full:
-            for _ in range(self.args.nminibatch * self.args.nepoch):
-                sample = self.memory.sample()
-                self.learner.update(sample)
-            self.memory.clear()
+            sample = self.memory.sample()
+            self.learner.update(sample)
+        # self.memory.clear()
```

### Comparing `xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_tf/agents/multi_agent_rl/mfq_agents.py` & `xuanpolicy-0.1.6/xuanpolicy/tensorflow/agents/multi_agent_rl/mfq_agents.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-from xuanpolicy.xuanpolicy_tf.agents import *
-from xuanpolicy.xuanpolicy_tf.agents.agents_marl import linear_decay_or_increase
+from xuanpolicy.tensorflow.agents import *
+from xuanpolicy.tensorflow.agents.agents_marl import linear_decay_or_increase
 
 
 class MFQ_Agents(MARLAgents):
     def __init__(self,
                  config: Namespace,
                  envs: DummyVecEnv_MAS,
                  device: str = "cpu:0"):
```

### Comparing `xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_tf/agents/multi_agent_rl/qmix_agents.py` & `xuanpolicy-0.1.6/xuanpolicy/tensorflow/agents/multi_agent_rl/wqmix_agents.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,19 @@
-from xuanpolicy.xuanpolicy_tf.agents import *
-from xuanpolicy.xuanpolicy_tf.agents.agents_marl import linear_decay_or_increase
+from xuanpolicy.tensorflow.agents import *
+from xuanpolicy.tensorflow.agents.agents_marl import linear_decay_or_increase
 
 
-class QMIX_Agents(MARLAgents):
+class WQMIX_Agents(MARLAgents):
     def __init__(self,
                  config: Namespace,
                  envs: DummyVecEnv_MAS,
                  device: str = "cpu:0"):
         self.comm = MPI.COMM_WORLD
 
+        self.alpha = config.alpha
         self.gamma = config.gamma
         self.use_obsnorm = config.use_obsnorm
         self.use_rewnorm = config.use_rewnorm
         self.obsnorm_range = config.obsnorm_range
         self.rewnorm_range = config.rewnorm_range
 
         self.start_greedy = config.start_greedy
@@ -23,15 +24,16 @@
         else:
             config.dim_state, state_shape = None, None
 
         input_representation = get_repre_in(config)
         representation = REGISTRY_Representation[config.representation](*input_representation)
         mixer = QMIX_mixer(config.dim_state[0], config.hidden_dim_mixing_net, config.hidden_dim_hyper_net,
                            config.n_agents)
-        input_policy = get_policy_in_marl(config, representation, config.agent_keys, mixer)
+        ff_mixer = QMIX_FF_mixer(config.dim_state[0], config.hidden_dim_mixing_net, config.n_agents)
+        input_policy = get_policy_in_marl(config, representation, config.agent_keys, mixer, ff_mixer)
         policy = REGISTRY_Policy[config.policy](*input_policy)
         # lr_scheduler = tk.optimizers.schedules.ExponentialDecay(config.learning_rate, decay_steps=1000,
         #                                                         decay_rate=0.9)
         lr_scheduler = MyLinearLR(config.learning_rate, start_factor=1.0, end_factor=0.5,
                                   total_iters=get_total_iters(config.agent_name, config))
         optimizer = tk.optimizers.Adam(lr_scheduler)
         self.observation_space = envs.observation_space
@@ -44,25 +46,25 @@
                                       config.obs_shape,
                                       config.act_shape,
                                       config.rew_shape,
                                       config.done_shape,
                                       envs.num_envs,
                                       config.buffer_size,
                                       config.batch_size)
-        learner = QMIX_Learner(config, policy, optimizer, writer,
-                               config.device, config.modeldir, config.gamma,
-                               config.sync_frequency)
+        learner = WQMIX_Learner(config, policy, optimizer, writer,
+                                config.device, config.modeldir, config.gamma,
+                                config.sync_frequency)
 
         self.obs_rms = RunningMeanStd(shape=space2shape(self.observation_space[config.agent_keys[0]]),
                                       comm=self.comm, use_mpi=False)
         self.ret_rms = RunningMeanStd(shape=(), comm=self.comm, use_mpi=False)
         self.epsilon_decay = linear_decay_or_increase(config.start_greedy, config.end_greedy,
                                                       config.greedy_update_steps)
-        super(QMIX_Agents, self).__init__(config, envs, policy, memory, learner, writer, device,
-                                          config.logdir, config.modeldir)
+        super(WQMIX_Agents, self).__init__(config, envs, policy, memory, learner, writer, device,
+                                           config.logdir, config.modeldir)
 
     def _process_observation(self, observations):
         if self.use_obsnorm:
             if isinstance(self.observation_space, Dict):
                 for key in self.observation_space.spaces.keys():
                     observations[key] = np.clip(
                         (observations[key] - self.obs_rms.mean[key]) / (self.obs_rms.std[key] + EPS),
```

### Comparing `xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_tf/agents/multi_agent_rl/qtran_agents.py` & `xuanpolicy-0.1.6/xuanpolicy/tensorflow/agents/multi_agent_rl/qtran_agents.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-from xuanpolicy.xuanpolicy_tf.agents import *
-from xuanpolicy.xuanpolicy_tf.agents.agents_marl import linear_decay_or_increase
+from xuanpolicy.tensorflow.agents import *
+from xuanpolicy.tensorflow.agents.agents_marl import linear_decay_or_increase
 
 
 class QTRAN_Agents(MARLAgents):
     def __init__(self,
                  config: Namespace,
                  envs: DummyVecEnv_MAS,
                  device: str = "cpu:0"):
```

### Comparing `xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_tf/agents/multi_agent_rl/vdac_agents.py` & `xuanpolicy-0.1.6/xuanpolicy/tensorflow/agents/multi_agent_rl/vdac_agents.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from xuanpolicy.xuanpolicy_tf.agents import *
+from xuanpolicy.tensorflow.agents import *
 
 
 class VDAC_Agents(MARLAgents):
     def __init__(self,
                  config: Namespace,
                  envs: DummyVecEnv_MAS,
                  device: str = "cpu:0"):
```

### Comparing `xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_tf/agents/multi_agent_rl/vdn_agents.py` & `xuanpolicy-0.1.6/xuanpolicy/mindspore/agents/multi_agent_rl/maddpg_agents.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,40 +1,39 @@
-from xuanpolicy.xuanpolicy_tf.agents import *
-from xuanpolicy.xuanpolicy_tf.agents.agents_marl import linear_decay_or_increase
+from xuanpolicy.mindspore.agents import *
 
 
-class VDN_Agents(MARLAgents):
+class MADDPG_Agents(MARLAgents):
     def __init__(self,
                  config: Namespace,
-                 envs: DummyVecEnv_MAS,
-                 device: str = "cpu:0"):
+                 envs: DummyVecEnv_MAS):
         self.comm = MPI.COMM_WORLD
 
         self.gamma = config.gamma
         self.use_obsnorm = config.use_obsnorm
         self.use_rewnorm = config.use_rewnorm
         self.obsnorm_range = config.obsnorm_range
         self.rewnorm_range = config.rewnorm_range
 
-        self.start_greedy = config.start_greedy
-        self.end_greedy = config.end_greedy
-        self.egreedy = config.start_greedy
-
         input_representation = get_repre_in(config)
         representation = REGISTRY_Representation[config.representation](*input_representation)
-        mixer = VDN_mixer()
-        input_policy = get_policy_in_marl(config, representation, config.agent_keys, mixer)
+        input_policy = get_policy_in_marl(config, representation, config.agent_keys)
         policy = REGISTRY_Policy[config.policy](*input_policy)
-        # lr_scheduler = tk.optimizers.schedules.ExponentialDecay(config.learning_rate, decay_steps=1000,
-        #                                                         decay_rate=0.9)
-        lr_scheduler = MyLinearLR(config.learning_rate, start_factor=1.0, end_factor=0.5,
-                                  total_iters=get_total_iters(config.agent_name, config))
-        optimizer = tk.optimizers.Adam(lr_scheduler)
+        scheduler = [lr_decay_model(learning_rate=config.lr_a, decay_rate=0.5,
+                                    decay_steps=get_total_iters(config.agent_name, config)),
+                     lr_decay_model(learning_rate=config.lr_c, decay_rate=0.5,
+                                    decay_steps=get_total_iters(config.agent_name, config))]
+        optimizer = [Adam(policy.parameters_actor, scheduler[0], eps=1e-5),
+                     Adam(policy.parameters_critic, scheduler[1], eps=1e-5)]
         self.observation_space = envs.observation_space
         self.action_space = envs.action_space
+        self.actions_high, self.actions_low = [], []
+        for k in config.agent_keys:
+            self.actions_high.append(self.action_space[k].high)
+            self.actions_low.append(self.action_space[k].low)
+        self.actions_high, self.actions_low = np.array(self.actions_high), np.array(self.actions_low)
         self.representation_info_shape = policy.representation.output_shapes
         self.auxiliary_info_shape = {}
 
         writer = SummaryWriter(config.logdir)
         if config.state_space is not None:
             config.dim_state, state_shape = config.state_space.shape, config.state_space.shape
         else:
@@ -43,25 +42,21 @@
                                       config.obs_shape,
                                       config.act_shape,
                                       config.rew_shape,
                                       config.done_shape,
                                       envs.num_envs,
                                       config.buffer_size,
                                       config.batch_size)
-        learner = VDN_Learner(config, policy, optimizer, writer,
-                              config.device, config.modeldir, config.gamma,
-                              config.sync_frequency)
+        learner = MADDPG_Learner(config, policy, optimizer, scheduler, writer, config.modeldir, config.gamma)
 
         self.obs_rms = RunningMeanStd(shape=space2shape(self.observation_space[config.agent_keys[0]]),
                                       comm=self.comm, use_mpi=False)
         self.ret_rms = RunningMeanStd(shape=(), comm=self.comm, use_mpi=False)
-        self.epsilon_decay = linear_decay_or_increase(config.start_greedy, config.end_greedy,
-                                                      config.greedy_update_steps)
-        super(VDN_Agents, self).__init__(config, envs, policy, memory, learner, writer, device,
-                                         config.logdir, config.modeldir)
+        super(MADDPG_Agents, self).__init__(config, envs, policy, memory, learner, writer,
+                                            config.logdir, config.modeldir)
 
     def _process_observation(self, observations):
         if self.use_obsnorm:
             if isinstance(self.observation_space, Dict):
                 for key in self.observation_space.spaces.keys():
                     observations[key] = np.clip(
                         (observations[key] - self.obs_rms.mean[key]) / (self.obs_rms.std[key] + EPS),
@@ -74,14 +69,22 @@
 
     def _process_reward(self, rewards):
         if self.use_rewnorm:
             std = np.clip(self.ret_rms.std, 0.1, 100)
             return np.clip(rewards / std, -self.rewnorm_range, self.rewnorm_range)
         return rewards
 
+    def act(self, obs_n, episode, test_mode, noise=False):
+        batch_size = len(obs_n)
+        agents_id = ops.broadcast_to(self.expand_dims(self.eye(self.n_agents, self.n_agents, ms.float32), 0),
+                                     (batch_size, -1, -1))
+        _, actions = self.policy(Tensor(obs_n), agents_id)
+        actions = actions.asnumpy()
+        if noise:
+            actions += np.random.normal(0, self.args.sigma, size=actions.shape)
+            actions = np.clip(actions, self.actions_low, self.actions_high)
+        return actions
+
     def train(self, i_episode):
-        self.epsilon_decay.update()
-        for i in range(self.nenvs):
-            self.writer.add_scalars("epsilon", {"env-%d" % i: self.epsilon_decay.epsilon}, i_episode)
         if self.memory.can_sample(self.args.batch_size):
             sample = self.memory.sample()
             self.learner.update(sample)
```

### Comparing `xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_tf/agents/multi_agent_rl/wqmix_agents.py` & `xuanpolicy-0.1.6/xuanpolicy/tensorflow/agents/multi_agent_rl/iddpg_agents.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,69 +1,62 @@
-from xuanpolicy.xuanpolicy_tf.agents import *
-from xuanpolicy.xuanpolicy_tf.agents.agents_marl import linear_decay_or_increase
+from xuanpolicy.tensorflow.agents import *
 
 
-class WQMIX_Agents(MARLAgents):
+class IDDPG_Agents(MARLAgents):
     def __init__(self,
                  config: Namespace,
                  envs: DummyVecEnv_MAS,
                  device: str = "cpu:0"):
         self.comm = MPI.COMM_WORLD
 
-        self.alpha = config.alpha
         self.gamma = config.gamma
         self.use_obsnorm = config.use_obsnorm
         self.use_rewnorm = config.use_rewnorm
         self.obsnorm_range = config.obsnorm_range
         self.rewnorm_range = config.rewnorm_range
 
-        self.start_greedy = config.start_greedy
-        self.end_greedy = config.end_greedy
-        self.egreedy = config.start_greedy
-        if config.state_space is not None:
-            config.dim_state, state_shape = config.state_space.shape, config.state_space.shape
-        else:
-            config.dim_state, state_shape = None, None
-
         input_representation = get_repre_in(config)
         representation = REGISTRY_Representation[config.representation](*input_representation)
-        mixer = QMIX_mixer(config.dim_state[0], config.hidden_dim_mixing_net, config.hidden_dim_hyper_net,
-                           config.n_agents)
-        ff_mixer = QMIX_FF_mixer(config.dim_state[0], config.hidden_dim_mixing_net, config.n_agents)
-        input_policy = get_policy_in_marl(config, representation, config.agent_keys, mixer, ff_mixer)
+        input_policy = get_policy_in_marl(config, representation, config.agent_keys)
         policy = REGISTRY_Policy[config.policy](*input_policy)
-        # lr_scheduler = tk.optimizers.schedules.ExponentialDecay(config.learning_rate, decay_steps=1000,
-        #                                                         decay_rate=0.9)
-        lr_scheduler = MyLinearLR(config.learning_rate, start_factor=1.0, end_factor=0.5,
-                                  total_iters=get_total_iters(config.agent_name, config))
-        optimizer = tk.optimizers.Adam(lr_scheduler)
+        lr_scheduler = [MyLinearLR(config.lr_a, start_factor=1.0, end_factor=0.5,
+                                   total_iters=get_total_iters(config.agent_name, config)),
+                        MyLinearLR(config.lr_c, start_factor=1.0, end_factor=0.5,
+                                   total_iters=get_total_iters(config.agent_name, config))]
+        optimizer = [tk.optimizers.Adam(lr_scheduler[0]),
+                     tk.optimizers.Adam(lr_scheduler[1])]
         self.observation_space = envs.observation_space
         self.action_space = envs.action_space
+        self.actions_high, self.actions_low = [], []
+        for k in config.agent_keys:
+            self.actions_high.append(self.action_space[k].high)
+            self.actions_low.append(self.action_space[k].low)
         self.representation_info_shape = policy.representation.output_shapes
         self.auxiliary_info_shape = {}
 
         writer = SummaryWriter(config.logdir)
+        if config.state_space is not None:
+            config.dim_state, state_shape = config.state_space.shape, config.state_space.shape
+        else:
+            config.dim_state, state_shape = None, None
         memory = MARL_OffPolicyBuffer(state_shape,
                                       config.obs_shape,
                                       config.act_shape,
                                       config.rew_shape,
                                       config.done_shape,
                                       envs.num_envs,
                                       config.buffer_size,
                                       config.batch_size)
-        learner = WQMIX_Learner(config, policy, optimizer, writer,
-                                config.device, config.modeldir, config.gamma,
-                                config.sync_frequency)
+        learner = IDDPG_Learner(config, policy, optimizer, writer,
+                                config.device, config.modeldir, config.gamma)
 
         self.obs_rms = RunningMeanStd(shape=space2shape(self.observation_space[config.agent_keys[0]]),
                                       comm=self.comm, use_mpi=False)
         self.ret_rms = RunningMeanStd(shape=(), comm=self.comm, use_mpi=False)
-        self.epsilon_decay = linear_decay_or_increase(config.start_greedy, config.end_greedy,
-                                                      config.greedy_update_steps)
-        super(WQMIX_Agents, self).__init__(config, envs, policy, memory, learner, writer, device,
+        super(IDDPG_Agents, self).__init__(config, envs, policy, memory, learner, writer, device,
                                            config.logdir, config.modeldir)
 
     def _process_observation(self, observations):
         if self.use_obsnorm:
             if isinstance(self.observation_space, Dict):
                 for key in self.observation_space.spaces.keys():
                     observations[key] = np.clip(
@@ -77,14 +70,23 @@
 
     def _process_reward(self, rewards):
         if self.use_rewnorm:
             std = np.clip(self.ret_rms.std, 0.1, 100)
             return np.clip(rewards / std, -self.rewnorm_range, self.rewnorm_range)
         return rewards
 
+    def act(self, obs_n, episode, test_mode, noise=False):
+        batch_size = len(obs_n)
+        with tf.device(self.device):
+            agents_id = tf.tile(tf.expand_dims(tf.eye(self.n_agents), axis=0), multiples=(batch_size, 1, 1))
+            inputs_policy = {"obs": tf.convert_to_tensor(obs_n), "ids": agents_id}
+            _, actions = self.policy(inputs_policy)
+        actions = actions.numpy()
+        if noise:
+            actions += np.random.normal(0, self.args.sigma, size=actions.shape)
+            actions = np.clip(actions, self.actions_low, self.actions_high)
+        return actions
+
     def train(self, i_episode):
-        self.epsilon_decay.update()
-        for i in range(self.nenvs):
-            self.writer.add_scalars("epsilon", {"env-%d" % i: self.epsilon_decay.epsilon}, i_episode)
         if self.memory.can_sample(self.args.batch_size):
             sample = self.memory.sample()
             self.learner.update(sample)
```

### Comparing `xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_tf/agents/policy_gradient/a2c_agent.py` & `xuanpolicy-0.1.6/xuanpolicy/tensorflow/agents/policy_gradient/a2c_agent.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from xuanpolicy.xuanpolicy_tf.agents import *
+from xuanpolicy.tensorflow.agents import *
 
 
 class A2C_Agent(Agent):
     def __init__(self,
                  config: Namespace,
                  envs: VecEnv,
                  policy: tk.Model,
```

### Comparing `xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_tf/agents/policy_gradient/ddpg_agent.py` & `xuanpolicy-0.1.6/xuanpolicy/tensorflow/agents/policy_gradient/ddpg_agent.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from xuanpolicy.xuanpolicy_tf.agents import *
+from xuanpolicy.tensorflow.agents import *
 
 
 class DDPG_Agent(Agent):
     def __init__(self,
                  config: Namespace,
                  envs: VecEnv,
                  policy: tk.Model,
```

### Comparing `xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_tf/agents/policy_gradient/mpdqn_agent.py` & `xuanpolicy-0.1.6/xuanpolicy/tensorflow/agents/policy_gradient/mpdqn_agent.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from xuanpolicy.xuanpolicy_tf.agents import *
+from xuanpolicy.tensorflow.agents import *
 import gym
 from gym import spaces
 
 
 class MPDQN_Agent(Agent):
     def __init__(self,
                  config: Namespace,
```

### Comparing `xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_tf/agents/policy_gradient/pdqn_agent.py` & `xuanpolicy-0.1.6/xuanpolicy/tensorflow/agents/policy_gradient/pdqn_agent.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from xuanpolicy.xuanpolicy_tf.agents import *
+from xuanpolicy.tensorflow.agents import *
 import gym
 from gym import spaces
 
 
 class PDQN_Agent(Agent):
     def __init__(self,
                  config: Namespace,
```

### Comparing `xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_tf/agents/policy_gradient/pg_agent.py` & `xuanpolicy-0.1.6/xuanpolicy/tensorflow/agents/policy_gradient/pg_agent.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from xuanpolicy.xuanpolicy_tf.agents import *
+from xuanpolicy.tensorflow.agents import *
 
 
 class PG_Agent(Agent):
     def __init__(self,
                  config: Namespace,
                  envs: VecEnv,
                  policy: tk.Model,
```

### Comparing `xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_tf/agents/policy_gradient/ppg_agent.py` & `xuanpolicy-0.1.6/xuanpolicy/torch/agents/policy_gradient/ppg_agent.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,27 +1,27 @@
-from xuanpolicy.xuanpolicy_tf.agents import *
+from xuanpolicy.torch.agents import *
 
 
 class PPG_Agent(Agent):
     def __init__(self,
                  config: Namespace,
                  envs: VecEnv,
-                 policy: tk.Model,
-                 optimizer: tk.optimizers.Optimizer,
-                 device: str = 'cpu'):
-        self.config = config
+                 policy: nn.Module,
+                 optimizer: torch.optim.Optimizer,
+                 scheduler: Optional[torch.optim.lr_scheduler._LRScheduler] = None,
+                 device: Optional[Union[int, str, torch.device]] = None):
         self.render = config.render
         self.comm = MPI.COMM_WORLD
         self.nenvs = envs.num_envs
         self.nsteps = config.nsteps
         self.nminibatch = config.nminibatch
         self.policy_nepoch = config.policy_nepoch
         self.value_nepoch = config.value_nepoch
         self.aux_nepoch = config.aux_nepoch
-
+        
         self.gamma = config.gamma
         self.lam = config.lam
         self.use_obsnorm = config.use_obsnorm
         self.use_rewnorm = config.use_rewnorm
         self.obsnorm_range = config.obsnorm_range
         self.rewnorm_range = config.rewnorm_range
 
@@ -38,25 +38,26 @@
                                      self.nenvs,
                                      self.nsteps,
                                      self.nminibatch,
                                      self.gamma,
                                      self.lam)
         learner = PPG_Learner(policy,
                               optimizer,
+                              scheduler,
                               writer,
                               config.device,
                               config.modeldir,
                               config.ent_coef,
                               config.clip_range,
                               config.kl_beta)
 
         self.obs_rms = RunningMeanStd(shape=space2shape(self.observation_space), comm=self.comm, use_mpi=False)
         self.ret_rms = RunningMeanStd(shape=(), comm=self.comm, use_mpi=False)
         super(PPG_Agent, self).__init__(envs, policy, memory, learner, writer, device, config.logdir,
-                                        config.modeldir)
+                                            config.modeldir)
 
     def _process_observation(self, observations):
         if self.use_obsnorm:
             if isinstance(self.observation_space, Dict):
                 for key in self.observation_space.spaces.keys():
                     observations[key] = np.clip(
                         (observations[key] - self.obs_rms.mean[key]) / (self.obs_rms.std[key] + EPS),
@@ -70,21 +71,20 @@
     def _process_reward(self, rewards):
         if self.use_rewnorm:
             std = np.clip(self.ret_rms.std, 0.1, 100)
             return np.clip(rewards / std, -self.rewnorm_range, self.rewnorm_range)
         return rewards
 
     def _action(self, obs):
-        states, _, vs, _ = self.policy(obs)
-        dists = self.policy.actor.dist
+        states, dists, vs, _ = self.policy(obs)
         acts = dists.stochastic_sample()
         for key in states.keys():
-            states[key] = states[key].numpy()
-        vs = vs.numpy()
-        acts = acts.numpy()
+            states[key] = states[key].detach().cpu().numpy()
+        vs = vs.detach().cpu().numpy()
+        acts = acts.detach().cpu().numpy()
         return states, acts, vs, split_distributions(dists)
 
     def train(self, train_steps=10000):
         episodes = np.zeros((self.nenvs,), np.int32)
         scores = np.zeros((self.nenvs,), np.float32)
         returns = np.zeros((self.nenvs,), np.float32)
 
@@ -104,22 +104,19 @@
                 for _ in range(self.nminibatch * self.policy_nepoch):
                     obs_batch, act_batch, ret_batch, adv_batch, _, aux_batch = self.memory.sample()
                     self.learner.update_policy(obs_batch, act_batch, ret_batch, adv_batch, aux_batch['old_dist'])
                 # critic update
                 for _ in range(self.nminibatch * self.value_nepoch):
                     obs_batch, act_batch, ret_batch, adv_batch, _, aux_batch = self.memory.sample()
                     self.learner.update_critic(obs_batch, act_batch, ret_batch, adv_batch, aux_batch['old_dist'])
-
+                    
                 # update old_prob
-                buffer_obs_shape = self.memory.observations.shape
-                buffer_obs = self.memory.observations.reshape([-1, buffer_obs_shape[-1]])
+                buffer_obs = self.memory.observations
                 buffer_act = self.memory.actions
-                _, new_logits, _, _ = self.policy(buffer_obs)
-                self.policy.actor.dist.set_param(tf.reshape(new_logits, buffer_obs_shape[0:-1]+(-1, )))
-                new_dist = self.policy.actor.dist
+                _,new_dist,_,_ = self.policy(buffer_obs)
                 self.memory.auxiliary_infos['old_dist'] = split_distributions(new_dist)
                 for _ in range(self.nminibatch * self.aux_nepoch):
                     obs_batch, act_batch, ret_batch, adv_batch, _, aux_batch = self.memory.sample()
                     self.learner.update_auxiliary(obs_batch, act_batch, ret_batch, adv_batch, aux_batch['old_dist'])
                 self.memory.clear()
             scores += rewards
             returns = self.gamma * returns + rewards
```

### Comparing `xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_tf/agents/policy_gradient/ppoclip_agent.py` & `xuanpolicy-0.1.6/xuanpolicy/tensorflow/agents/policy_gradient/ppoclip_agent.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from xuanpolicy.xuanpolicy_tf.agents import *
+from xuanpolicy.tensorflow.agents import *
 
 
 class PPOCLIP_Agent(Agent):
     def __init__(self,
                  config: Namespace,
                  envs: VecEnv,
                  policy: tk.Model,
```

### Comparing `xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_tf/agents/policy_gradient/ppokl_agent.py` & `xuanpolicy-0.1.6/xuanpolicy/tensorflow/agents/policy_gradient/ppokl_agent.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from xuanpolicy.xuanpolicy_tf.agents import *
+from xuanpolicy.tensorflow.agents import *
 
 
 class PPOKL_Agent(Agent):
     def __init__(self,
                  config: Namespace,
                  envs: VecEnv,
                  policy: tk.Model,
```

### Comparing `xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_tf/agents/policy_gradient/sac_agent.py` & `xuanpolicy-0.1.6/xuanpolicy/tensorflow/agents/policy_gradient/sac_agent.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from xuanpolicy.xuanpolicy_tf.agents import *
+from xuanpolicy.tensorflow.agents import *
 
 
 class SAC_Agent(Agent):
     def __init__(self,
                  config: Namespace,
                  envs: VecEnv,
                  policy: tk.Model,
```

### Comparing `xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_tf/agents/policy_gradient/sacdis_agent.py` & `xuanpolicy-0.1.6/xuanpolicy/tensorflow/agents/policy_gradient/sacdis_agent.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from xuanpolicy.xuanpolicy_tf.agents import *
+from xuanpolicy.tensorflow.agents import *
 
 
 class SACDIS_Agent(Agent):
     def __init__(self,
                  config: Namespace,
                  envs: VecEnv,
                  policy: tk.Model,
```

### Comparing `xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_tf/agents/policy_gradient/spdqn_agent.py` & `xuanpolicy-0.1.6/xuanpolicy/tensorflow/agents/policy_gradient/spdqn_agent.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from xuanpolicy.xuanpolicy_tf.agents import *
+from xuanpolicy.tensorflow.agents import *
 import gym
 from gym import spaces
 
 
 class SPDQN_Agent(Agent):
     def __init__(self,
                  config: Namespace,
```

### Comparing `xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_tf/agents/policy_gradient/td3_agent.py` & `xuanpolicy-0.1.6/xuanpolicy/tensorflow/agents/policy_gradient/td3_agent.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from xuanpolicy.xuanpolicy_tf.agents import *
+from xuanpolicy.tensorflow.agents import *
 
 
 class TD3_Agent(Agent):
     def __init__(self,
                  config: Namespace,
                  envs: VecEnv,
                  policy: tk.Model,
```

### Comparing `xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_tf/agents/qlearning_family/c51_agent.py` & `xuanpolicy-0.1.6/xuanpolicy/tensorflow/agents/qlearning_family/c51_agent.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from xuanpolicy.xuanpolicy_tf.agents import *
+from xuanpolicy.tensorflow.agents import *
 
 
 class C51_Agent(Agent):
     def __init__(self,
                  config: Namespace,
                  envs: VecEnv,
                  policy: tk.Model,
```

### Comparing `xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_tf/agents/qlearning_family/cdqn_agent.py` & `xuanpolicy-0.1.6/xuanpolicy/tensorflow/agents/qlearning_family/cdqn_agent.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from xuanpolicy.xuanpolicy_tf.agents import *
+from xuanpolicy.tensorflow.agents import *
 
 
 class CDQN_Agent(Agent):
     def __init__(self,
                  config: Namespace,
                  envs: VecEnv,
                  policy: tk.Model,
```

### Comparing `xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_tf/agents/qlearning_family/cldqn_agent.py` & `xuanpolicy-0.1.6/xuanpolicy/tensorflow/agents/qlearning_family/dqn_agent.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,18 @@
-from xuanpolicy.xuanpolicy_tf.agents import *
+from xuanpolicy.tensorflow.agents import *
 
 
-class CLDQN_Agent(Agent):
+class DQN_Agent(Agent):
     def __init__(self,
                  config: Namespace,
                  envs: VecEnv,
                  policy: tk.Model,
                  optimizer: tk.optimizers.Optimizer,
                  device: str = 'cpu'):
+        self.config = config
         self.render = config.render
         self.comm = MPI.COMM_WORLD
         self.nenvs = envs.num_envs
 
         self.gamma = config.gamma
         self.use_obsnorm = config.use_obsnorm
         self.use_rewnorm = config.use_rewnorm
@@ -43,15 +44,15 @@
                               config.device,
                               config.modeldir,
                               config.gamma,
                               config.sync_frequency)
 
         self.obs_rms = RunningMeanStd(shape=space2shape(self.observation_space), comm=self.comm, use_mpi=False)
         self.ret_rms = RunningMeanStd(shape=(), comm=self.comm, use_mpi=False)
-        super(CLDQN_Agent, self).__init__(envs, policy, memory, learner, writer, device, config.logdir, config.modeldir)
+        super(DQN_Agent, self).__init__(envs, policy, memory, learner, writer, device, config.logdir, config.modeldir)
 
     def _process_observation(self, observations):
         if self.use_obsnorm:
             if isinstance(self.observation_space, Dict):
                 for key in self.observation_space.spaces.keys():
                     observations[key] = np.clip(
                         (observations[key] - self.obs_rms.mean[key]) / (self.obs_rms.std[key] + EPS),
@@ -112,25 +113,26 @@
                     returns[i] = 0
                     episodes[i] += 1
             if step % 50000 == 0 or step == train_steps - 1:
                 self.save_model()
                 np.save(self.modeldir + "/obs_rms.npy",
                         {'mean': self.obs_rms.mean, 'std': self.obs_rms.std, 'count': self.obs_rms.count})
 
-    def test(self, test_steps=10000, episode=0):
+    def test(self, test_steps=10000):
         self.load_model(self.modeldir)
         scores = np.zeros((self.nenvs,), np.float32)
         returns = np.zeros((self.nenvs,), np.float32)
         obs = self.envs.reset()
         for _ in tqdm(range(test_steps)):
             self.obs_rms.update(obs)
             obs = self._process_observation(obs)
             states, acts = self._action(obs, egreedy=0.0)
             next_obs, rewards, dones, infos = self.envs.step(acts)
             self.envs.render()
+            time.sleep(self.config.render_delay)
 
             scores += rewards
             returns = self.gamma * returns + rewards
             obs = next_obs
 
             for i in range(self.nenvs):
                 if dones[i] == True:
```

### Comparing `xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_tf/agents/qlearning_family/ddqn_agent.py` & `xuanpolicy-0.1.6/xuanpolicy/tensorflow/agents/qlearning_family/ddqn_agent.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from xuanpolicy.xuanpolicy_tf.agents import *
+from xuanpolicy.tensorflow.agents import *
 
 
 class DDQN_Agent(Agent):
     def __init__(self,
                  config: Namespace,
                  envs: VecEnv,
                  policy: tk.Model,
```

### Comparing `xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_tf/agents/qlearning_family/dqn_agent.py` & `xuanpolicy-0.1.6/xuanpolicy/tensorflow/agents/qlearning_family/cldqn_agent.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,17 @@
-from xuanpolicy.xuanpolicy_tf.agents import *
+from xuanpolicy.tensorflow.agents import *
 
 
-class DQN_Agent(Agent):
+class CLDQN_Agent(Agent):
     def __init__(self,
                  config: Namespace,
                  envs: VecEnv,
                  policy: tk.Model,
                  optimizer: tk.optimizers.Optimizer,
                  device: str = 'cpu'):
-        self.config = config
         self.render = config.render
         self.comm = MPI.COMM_WORLD
         self.nenvs = envs.num_envs
 
         self.gamma = config.gamma
         self.use_obsnorm = config.use_obsnorm
         self.use_rewnorm = config.use_rewnorm
@@ -44,15 +43,15 @@
                               config.device,
                               config.modeldir,
                               config.gamma,
                               config.sync_frequency)
 
         self.obs_rms = RunningMeanStd(shape=space2shape(self.observation_space), comm=self.comm, use_mpi=False)
         self.ret_rms = RunningMeanStd(shape=(), comm=self.comm, use_mpi=False)
-        super(DQN_Agent, self).__init__(envs, policy, memory, learner, writer, device, config.logdir, config.modeldir)
+        super(CLDQN_Agent, self).__init__(envs, policy, memory, learner, writer, device, config.logdir, config.modeldir)
 
     def _process_observation(self, observations):
         if self.use_obsnorm:
             if isinstance(self.observation_space, Dict):
                 for key in self.observation_space.spaces.keys():
                     observations[key] = np.clip(
                         (observations[key] - self.obs_rms.mean[key]) / (self.obs_rms.std[key] + EPS),
@@ -113,26 +112,25 @@
                     returns[i] = 0
                     episodes[i] += 1
             if step % 50000 == 0 or step == train_steps - 1:
                 self.save_model()
                 np.save(self.modeldir + "/obs_rms.npy",
                         {'mean': self.obs_rms.mean, 'std': self.obs_rms.std, 'count': self.obs_rms.count})
 
-    def test(self, test_steps=10000):
+    def test(self, test_steps=10000, episode=0):
         self.load_model(self.modeldir)
         scores = np.zeros((self.nenvs,), np.float32)
         returns = np.zeros((self.nenvs,), np.float32)
         obs = self.envs.reset()
         for _ in tqdm(range(test_steps)):
             self.obs_rms.update(obs)
             obs = self._process_observation(obs)
             states, acts = self._action(obs, egreedy=0.0)
             next_obs, rewards, dones, infos = self.envs.step(acts)
             self.envs.render()
-            time.sleep(self.config.render_delay)
 
             scores += rewards
             returns = self.gamma * returns + rewards
             obs = next_obs
 
             for i in range(self.nenvs):
                 if dones[i] == True:
```

### Comparing `xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_tf/agents/qlearning_family/dueldqn_agent.py` & `xuanpolicy-0.1.6/xuanpolicy/tensorflow/agents/qlearning_family/dueldqn_agent.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from xuanpolicy.xuanpolicy_tf.agents import *
+from xuanpolicy.tensorflow.agents import *
 
 
 class DuelDQN_Agent(Agent):
     def __init__(self,
                  config: Namespace,
                  envs: VecEnv,
                  policy: tk.Model,
```

### Comparing `xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_tf/agents/qlearning_family/ldqn_agent.py` & `xuanpolicy-0.1.6/xuanpolicy/tensorflow/agents/qlearning_family/qrdqn_agent.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-from xuanpolicy.xuanpolicy_tf.agents import *
+from xuanpolicy.tensorflow.agents import *
 
 
-class LDQN_Agent(Agent):
+class QRDQN_Agent(Agent):
     def __init__(self,
                  config: Namespace,
                  envs: VecEnv,
                  policy: tk.Model,
                  optimizer: tk.optimizers.Optimizer,
                  device: str = 'cpu'):
         self.config = config
@@ -34,25 +34,25 @@
         memory = DummyOffPolicyBuffer(self.observation_space,
                                       self.action_space,
                                       self.representation_info_shape,
                                       self.auxiliary_info_shape,
                                       self.nenvs,
                                       config.nsize,
                                       config.batchsize)
-        learner = DQN_Learner(policy,
-                              optimizer,
-                              writer,
-                              config.device,
-                              config.modeldir,
-                              config.gamma,
-                              config.sync_frequency)
+        learner = QRDQN_Learner(policy,
+                                optimizer,
+                                writer,
+                                config.device,
+                                config.modeldir,
+                                config.gamma,
+                                config.sync_frequency)
 
         self.obs_rms = RunningMeanStd(shape=space2shape(self.observation_space), comm=self.comm, use_mpi=False)
         self.ret_rms = RunningMeanStd(shape=(), comm=self.comm, use_mpi=False)
-        super(LDQN_Agent, self).__init__(envs, policy, memory, learner, writer, device, config.logdir, config.modeldir)
+        super(QRDQN_Agent, self).__init__(envs, policy, memory, learner, writer, device, config.logdir, config.modeldir)
 
     def _process_observation(self, observations):
         if self.use_obsnorm:
             if isinstance(self.observation_space, Dict):
                 for key in self.observation_space.spaces.keys():
                     observations[key] = np.clip(
                         (observations[key] - self.obs_rms.mean[key]) / (self.obs_rms.std[key] + EPS),
```

### Comparing `xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_tf/agents/qlearning_family/noisydqn_agent.py` & `xuanpolicy-0.1.6/xuanpolicy/tensorflow/agents/qlearning_family/noisydqn_agent.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from xuanpolicy.xuanpolicy_tf.agents import *
+from xuanpolicy.tensorflow.agents import *
 
 
 class NoisyDQN_Agent(Agent):
     def __init__(self,
                  config: Namespace,
                  envs: VecEnv,
                  policy: tk.Model,
```

### Comparing `xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_tf/agents/qlearning_family/perdqn_agent.py` & `xuanpolicy-0.1.6/xuanpolicy/tensorflow/agents/qlearning_family/perdqn_agent.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from xuanpolicy.xuanpolicy_tf.agents import *
+from xuanpolicy.tensorflow.agents import *
 
 
 class PerDQN_Agent(Agent):
     def __init__(self,
                  config: Namespace,
                  envs: VecEnv,
                  policy: tk.Model,
```

### Comparing `xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_tf/agents/qlearning_family/qrdqn_agent.py` & `xuanpolicy-0.1.6/xuanpolicy/tensorflow/agents/qlearning_family/ldqn_agent.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-from xuanpolicy.xuanpolicy_tf.agents import *
+from xuanpolicy.tensorflow.agents import *
 
 
-class QRDQN_Agent(Agent):
+class LDQN_Agent(Agent):
     def __init__(self,
                  config: Namespace,
                  envs: VecEnv,
                  policy: tk.Model,
                  optimizer: tk.optimizers.Optimizer,
                  device: str = 'cpu'):
         self.config = config
@@ -34,25 +34,25 @@
         memory = DummyOffPolicyBuffer(self.observation_space,
                                       self.action_space,
                                       self.representation_info_shape,
                                       self.auxiliary_info_shape,
                                       self.nenvs,
                                       config.nsize,
                                       config.batchsize)
-        learner = QRDQN_Learner(policy,
-                                optimizer,
-                                writer,
-                                config.device,
-                                config.modeldir,
-                                config.gamma,
-                                config.sync_frequency)
+        learner = DQN_Learner(policy,
+                              optimizer,
+                              writer,
+                              config.device,
+                              config.modeldir,
+                              config.gamma,
+                              config.sync_frequency)
 
         self.obs_rms = RunningMeanStd(shape=space2shape(self.observation_space), comm=self.comm, use_mpi=False)
         self.ret_rms = RunningMeanStd(shape=(), comm=self.comm, use_mpi=False)
-        super(QRDQN_Agent, self).__init__(envs, policy, memory, learner, writer, device, config.logdir, config.modeldir)
+        super(LDQN_Agent, self).__init__(envs, policy, memory, learner, writer, device, config.logdir, config.modeldir)
 
     def _process_observation(self, observations):
         if self.use_obsnorm:
             if isinstance(self.observation_space, Dict):
                 for key in self.observation_space.spaces.keys():
                     observations[key] = np.clip(
                         (observations[key] - self.obs_rms.mean[key]) / (self.obs_rms.std[key] + EPS),
```

### Comparing `xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_tf/learners/__init__.py` & `xuanpolicy-0.1.6/xuanpolicy/tensorflow/learners/__init__.py`

 * *Files identical despite different names*

### Comparing `xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_tf/learners/learner.py` & `xuanpolicy-0.1.6/xuanpolicy/tensorflow/learners/learner.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from xuanpolicy.xuanpolicy_tf.learners import *
+from xuanpolicy.tensorflow.learners import *
 from argparse import Namespace
 
 
 class Learner(ABC):
     def __init__(self,
                  policy: tk.Model,
                  optimizer: Union[tk.optimizers.Optimizer, Sequence[tk.optimizers.Optimizer]],
```

### Comparing `xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_tf/learners/multi_agent_rl/coma_learner.py` & `xuanpolicy-0.1.6/xuanpolicy/tensorflow/learners/multi_agent_rl/coma_learner.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
 COMA: Counterfactual Multi-Agent Policy Gradients
 Paper link: https://ojs.aaai.org/index.php/AAAI/article/view/11794
 Implementation: TensorFlow 2.X
 """
-from xuanpolicy.xuanpolicy_tf.learners import *
+from xuanpolicy.tensorflow.learners import *
 
 
 class COMA_Learner(LearnerMAS):
     def __init__(self,
                  config: Namespace,
                  policy: tk.Model,
                  optimizer: Sequence[tk.optimizers.Optimizer],
```

### Comparing `xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_tf/learners/multi_agent_rl/dcg_learner.py` & `xuanpolicy-0.1.6/xuanpolicy/tensorflow/learners/multi_agent_rl/dcg_learner.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 DCG: Deep coordination graphs
 Paper link: http://proceedings.mlr.press/v119/boehmer20a/boehmer20a.pdf
 Implementation: TensorFlow 2.X
 """
 import numpy as np
 import torch
 
-from xuanpolicy.xuanpolicy_tf.learners import *
+from xuanpolicy.tensorflow.learners import *
 import torch_scatter
 
 
 class DCG_Learner(LearnerMAS):
     def __init__(self,
                  config: Namespace,
                  policy: tk.Model,
```

### Comparing `xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_tf/learners/multi_agent_rl/iddpg_learner.py` & `xuanpolicy-0.1.6/xuanpolicy/tensorflow/learners/multi_agent_rl/iddpg_learner.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
 Independent Deep Deterministic Policy Gradient (IDDPG)
 Implementation: TensorFlow 2.X
 """
-from xuanpolicy.xuanpolicy_tf.learners import *
+from xuanpolicy.tensorflow.learners import *
 
 
 class IDDPG_Learner(LearnerMAS):
     def __init__(self,
                  config: Namespace,
                  policy: tk.Model,
                  optimizer: Sequence[tk.optimizers.Optimizer],
```

### Comparing `xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_tf/learners/multi_agent_rl/iql_learner.py` & `xuanpolicy-0.1.6/xuanpolicy/tensorflow/learners/multi_agent_rl/iql_learner.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
 Independent Q-learning (IQL)
 Implementation: TensorFlow 2.X
 """
-from xuanpolicy.xuanpolicy_tf.learners import *
+from xuanpolicy.tensorflow.learners import *
 
 
 class IQL_Learner(LearnerMAS):
     def __init__(self,
                  config: Namespace,
                  policy: tk.Model,
                  optimizer: tk.optimizers.Optimizer,
```

### Comparing `xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_tf/learners/multi_agent_rl/isac_learner.py` & `xuanpolicy-0.1.6/xuanpolicy/tensorflow/learners/multi_agent_rl/isac_learner.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
 Independent Soft Actor-critic (ISAC)
 Implementation: TensorFlow 2.X
 """
-from xuanpolicy.xuanpolicy_tf.learners import *
+from xuanpolicy.tensorflow.learners import *
 
 
 class ISAC_Learner(LearnerMAS):
     def __init__(self,
                  config: Namespace,
                  policy: tk.Model,
                  optimizer: Sequence[tk.optimizers.Optimizer],
```

### Comparing `xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_tf/learners/multi_agent_rl/maac_learner.py` & `xuanpolicy-0.1.6/xuanpolicy/torch/learners/multi_agent_rl/maddpg_learner.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 """
 Multi-Agent Deep Deterministic Policy Gradient
 Paper link:
 https://proceedings.neurips.cc/paper/2017/file/68a9750337a418a86fe06c1991a1d64c-Paper.pdf
-Implementation: TensorFlow 2.X
+Implementation: Pytorch
 Trick: Parameter sharing for all agents, with agents' one-hot IDs as actor-critic's inputs.
 """
-from xuanpolicy.xuanpolicy_torch.learners import *
+from xuanpolicy.torch.learners import *
 
 
-class MAAC_Learner(LearnerMAS):
+class MADDPG_Learner(LearnerMAS):
     def __init__(self,
                  config: Namespace,
                  policy: nn.Module,
                  optimizer: Sequence[torch.optim.Optimizer],
                  scheduler: Sequence[torch.optim.lr_scheduler._LRScheduler] = None,
                  summary_writer: Optional[SummaryWriter] = None,
                  device: Optional[Union[int, str, torch.device]] = None,
@@ -20,15 +20,15 @@
                  gamma: float = 0.99,
                  sync_frequency: int = 100
                  ):
         self.gamma = gamma
         self.tau = config.tau
         self.sync_frequency = sync_frequency
         self.mse_loss = nn.MSELoss()
-        super(MAAC_Learner, self).__init__(config, policy, optimizer, scheduler, summary_writer, device, modeldir)
+        super(MADDPG_Learner, self).__init__(config, policy, optimizer, scheduler, summary_writer, device, modeldir)
         self.optimizer = {
             'actor': optimizer[0],
             'critic': optimizer[1]
         }
         self.scheduler = {
             'actor': scheduler[0],
             'critic': scheduler[1]
```

### Comparing `xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_tf/learners/multi_agent_rl/maddpg_learner.py` & `xuanpolicy-0.1.6/xuanpolicy/tensorflow/learners/multi_agent_rl/maddpg_learner.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """
 Multi-Agent Deep Deterministic Policy Gradient
 Paper link:
 https://proceedings.neurips.cc/paper/2017/file/68a9750337a418a86fe06c1991a1d64c-Paper.pdf
 Implementation: TensorFlow 2.X
 Trick: Parameter sharing for all agents, with agents' one-hot IDs as actor-critic's inputs.
 """
-from xuanpolicy.xuanpolicy_tf.learners import *
+from xuanpolicy.tensorflow.learners import *
 
 
 class MADDPG_Learner(LearnerMAS):
     def __init__(self,
                  config: Namespace,
                  policy: tk.Model,
                  optimizer: Sequence[tk.optimizers.Optimizer],
```

### Comparing `xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_tf/learners/multi_agent_rl/madqn_learner.py` & `xuanpolicy-0.1.6/xuanpolicy/tensorflow/learners/multi_agent_rl/madqn_learner.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """
 Multi-Agent Deep Q Network
 Code link: github.com/opendilab/DI-engine/blob/main/ding/policy/madqn.py
 Implementation: TensorFlow 2.X
 Trick: Parameter sharing for all agents, with agents' one-hot IDs as actor-critic's inputs.
 """
-from xuanpolicy.xuanpolicy_torch.learners import *
+from xuanpolicy.torch.learners import *
 
 
 class MADQN_Learner(LearnerMAS):
     def __init__(self,
                  config: Namespace,
                  policy: nn.Module,
                  optimizer: torch.optim.Optimizer,
```

### Comparing `xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_tf/learners/multi_agent_rl/mappoclip_learner.py` & `xuanpolicy-0.1.6/xuanpolicy/tensorflow/learners/multi_agent_rl/mappoclip_learner.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """
 Multi-Agent Proximal Policy Optimization (MAPPO)
 Paper link:
 https://arxiv.org/pdf/2103.01955.pdf
 Implementation: TensorFlow 2.X
 """
-from xuanpolicy.xuanpolicy_tf.learners import *
+from xuanpolicy.tensorflow.learners import *
 
 
 class MAPPO_Clip_Learner(LearnerMAS):
     def __init__(self,
                  config: Namespace,
                  policy: tk.Model,
                  optimizer: tk.optimizers.Optimizer,
```

### Comparing `xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_tf/learners/multi_agent_rl/mappokl_learner.py` & `xuanpolicy-0.1.6/xuanpolicy/tensorflow/learners/multi_agent_rl/mappokl_learner.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """
 Multi-Agent Proximal Policy Optimization (MAPPO)
 Paper link:
 https://arxiv.org/pdf/2103.01955.pdf
 Implementation: TensorFlow 2.X
 """
-from xuanpolicy.xuanpolicy_tf.learners import *
-from xuanpolicy.xuanpolicy_tf.utils.operations import merge_distributions
+from xuanpolicy.tensorflow.learners import *
+from xuanpolicy.tensorflow.utils.operations import merge_distributions
 
 
 class MAPPO_KL_Learner(LearnerMAS):
     def __init__(self,
                  config: Namespace,
                  policy: tk.Model,
                  optimizer: tk.optimizers.Optimizer,
```

### Comparing `xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_tf/learners/multi_agent_rl/masac_learner.py` & `xuanpolicy-0.1.6/xuanpolicy/tensorflow/learners/multi_agent_rl/masac_learner.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
 Multi-agent Soft Actor-critic (MASAC)
 Implementation: TensorFlow 2.X
 """
-from xuanpolicy.xuanpolicy_tf.learners import *
+from xuanpolicy.tensorflow.learners import *
 
 
 class MASAC_Learner(LearnerMAS):
     def __init__(self,
                  config: Namespace,
                  policy: tk.Model,
                  optimizer: Sequence[tk.optimizers.Optimizer],
```

### Comparing `xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_tf/learners/multi_agent_rl/matd3_learner.py` & `xuanpolicy-0.1.6/xuanpolicy/tensorflow/learners/multi_agent_rl/matd3_learner.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
 Multi-Agent TD3
 
 """
-from xuanpolicy.xuanpolicy_tf.learners import *
+from xuanpolicy.tensorflow.learners import *
 
 
 class MATD3_Learner(LearnerMAS):
     def __init__(self,
                  config: Namespace,
                  policy: tk.Model,
                  optimizer: Sequence[tk.optimizers.Optimizer],
```

### Comparing `xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_tf/learners/multi_agent_rl/mfac_learner.py` & `xuanpolicy-0.1.6/xuanpolicy/tensorflow/learners/multi_agent_rl/mfac_learner.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """
 MFAC: Mean Field Actor-Critic
 Paper link:
 http://proceedings.mlr.press/v80/yang18d/yang18d.pdf
 Implementation: TensorFlow 2.X
 """
-from xuanpolicy.xuanpolicy_tf.learners import *
+from xuanpolicy.tensorflow.learners import *
 
 
 class MFAC_Learner(LearnerMAS):
     def __init__(self,
                  config: Namespace,
                  policy: tk.Model,
                  optimizer: Sequence[tk.optimizers.Optimizer],
```

### Comparing `xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_tf/learners/multi_agent_rl/mfq_learner.py` & `xuanpolicy-0.1.6/xuanpolicy/tensorflow/learners/multi_agent_rl/mfq_learner.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """
 MFQ: Mean Field Q-Learning
 Paper link:
 http://proceedings.mlr.press/v80/yang18d/yang18d.pdf
 Implementation: TensorFlow 2.X
 """
-from xuanpolicy.xuanpolicy_tf.learners import *
+from xuanpolicy.tensorflow.learners import *
 
 
 class MFQ_Learner(LearnerMAS):
     def __init__(self,
                  config: Namespace,
                  policy: tk.Model,
                  optimizer: tk.optimizers.Optimizer,
```

### Comparing `xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_tf/learners/multi_agent_rl/qmix_learner.py` & `xuanpolicy-0.1.6/xuanpolicy/tensorflow/learners/multi_agent_rl/qmix_learner.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """
 Qmix: Monotonic value function factorisation for deep multi-agent reinforcement learning
 Paper link:
 http://proceedings.mlr.press/v80/rashid18a/rashid18a.pdf
 Implementation: TensorFlow 2.X
 """
-from xuanpolicy.xuanpolicy_tf.learners import *
+from xuanpolicy.tensorflow.learners import *
 
 
 class QMIX_Learner(LearnerMAS):
     def __init__(self,
                  config: Namespace,
                  policy: tk.Model,
                  optimizer: tk.optimizers.Optimizer,
```

### Comparing `xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_tf/learners/multi_agent_rl/qtran_learner.py` & `xuanpolicy-0.1.6/xuanpolicy/tensorflow/learners/multi_agent_rl/qtran_learner.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """
 QTRAN: Learning to Factorize with Transformation for Cooperative Multi-Agent Reinforcement Learning
 Paper link:
 http://proceedings.mlr.press/v97/son19a/son19a.pdf
 Implementation: TensorFlow 2.X
 """
-from xuanpolicy.xuanpolicy_tf.learners import *
+from xuanpolicy.tensorflow.learners import *
 
 
 class QTRAN_Learner(LearnerMAS):
     def __init__(self,
                  config: Namespace,
                  policy: tk.Model,
                  optimizer: tk.optimizers.Optimizer,
```

### Comparing `xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_tf/learners/multi_agent_rl/vdac_learner.py` & `xuanpolicy-0.1.6/xuanpolicy/tensorflow/learners/multi_agent_rl/vdac_learner.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
 Value Decomposition Actor-Critic (VDAC)
 Paper link: https://ojs.aaai.org/index.php/AAAI/article/view/17353
 Implementation: Pytorch
 """
-from xuanpolicy.xuanpolicy_tf.learners import *
+from xuanpolicy.tensorflow.learners import *
 
 
 class VDAC_Learner(LearnerMAS):
     def __init__(self,
                  config: Namespace,
                  policy: tk.Model,
                  optimizer: tk.optimizers.Optimizer,
```

### Comparing `xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_tf/learners/multi_agent_rl/vdn_learner.py` & `xuanpolicy-0.1.6/xuanpolicy/tensorflow/learners/multi_agent_rl/vdn_learner.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """
 Value Decomposition Networks (VDN)
 Paper link:
 https://arxiv.org/pdf/1706.05296.pdf
 Implementation: TensorFlow 2.X
 """
-from xuanpolicy.xuanpolicy_tf.learners import *
+from xuanpolicy.tensorflow.learners import *
 
 
 class VDN_Learner(LearnerMAS):
     def __init__(self,
                  config: Namespace,
                  policy: tk.Model,
                  optimizer: tk.optimizers.Optimizer,
```

### Comparing `xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_tf/learners/multi_agent_rl/wqmix_learner.py` & `xuanpolicy-0.1.6/xuanpolicy/tensorflow/learners/multi_agent_rl/wqmix_learner.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """
 Weighted QMIX
 Paper link:
 https://proceedings.neurips.cc/paper/2020/file/73a427badebe0e32caa2e1fc7530b7f3-Paper.pdf
 Implementation: TensorFlow 2.X
 """
-from xuanpolicy.xuanpolicy_tf.learners import *
+from xuanpolicy.tensorflow.learners import *
 
 
 class WQMIX_Learner(LearnerMAS):
     def __init__(self,
                  config: Namespace,
                  policy: tk.Model,
                  optimizer: tk.optimizers.Optimizer,
```

### Comparing `xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_tf/learners/policy_gradient/a2c_learner.py` & `xuanpolicy-0.1.6/xuanpolicy/tensorflow/learners/policy_gradient/a2c_learner.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from xuanpolicy.xuanpolicy_tf.learners import *
+from xuanpolicy.tensorflow.learners import *
 
 
 class A2C_Learner(Learner):
     def __init__(self,
                  policy: tk.Model,
                  optimizer: tk.optimizers.Optimizer,
                  summary_writer: Optional[SummaryWriter] = None,
```

### Comparing `xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_tf/learners/policy_gradient/ddpg_learner.py` & `xuanpolicy-0.1.6/xuanpolicy/tensorflow/learners/policy_gradient/ddpg_learner.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from xuanpolicy.xuanpolicy_tf.learners import *
+from xuanpolicy.tensorflow.learners import *
 
 
 class DDPG_Learner(Learner):
     def __init__(self,
                  policy: tk.Model,
                  optimizers: Sequence[tk.optimizers.Optimizer],
                  summary_writer: Optional[SummaryWriter] = None,
```

### Comparing `xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_tf/learners/policy_gradient/mpdqn_learner.py` & `xuanpolicy-0.1.6/xuanpolicy/tensorflow/learners/policy_gradient/mpdqn_learner.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from xuanpolicy.xuanpolicy_tf.learners import *
+from xuanpolicy.tensorflow.learners import *
 
 class MPDQN_Learner(Learner):
     def __init__(self,
                  policy: tk.Model,
                  optimizers: Sequence[tk.optimizers.Optimizer],
                  summary_writer: Optional[SummaryWriter] = None,
                  device: str = "cpu:0",
```

### Comparing `xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_tf/learners/policy_gradient/pdqn_learner.py` & `xuanpolicy-0.1.6/xuanpolicy/tensorflow/learners/policy_gradient/pdqn_learner.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from xuanpolicy.xuanpolicy_tf.learners import *
+from xuanpolicy.tensorflow.learners import *
 
 class PDQN_Learner(Learner):
     def __init__(self,
                  policy: tk.Model,
                  optimizers: Sequence[tk.optimizers.Optimizer],
                  summary_writer: Optional[SummaryWriter] = None,
                  device: str = "cpu:0",
```

### Comparing `xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_tf/learners/policy_gradient/pg_learner.py` & `xuanpolicy-0.1.6/xuanpolicy/tensorflow/learners/policy_gradient/pg_learner.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from xuanpolicy.xuanpolicy_tf.learners import *
+from xuanpolicy.tensorflow.learners import *
 
 
 class PG_Learner(Learner):
     def __init__(self,
                  policy: tk.Model,
                  optimizer: tk.optimizers.Optimizer,
                  summary_writer: Optional[SummaryWriter] = None,
```

### Comparing `xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_tf/learners/policy_gradient/ppg_learner.py` & `xuanpolicy-0.1.6/xuanpolicy/tensorflow/learners/policy_gradient/ppg_learner.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from argparse import Action
 
-from xuanpolicy.xuanpolicy_tf.learners import *
-from xuanpolicy.xuanpolicy_tf.utils.operations import merge_distributions
+from xuanpolicy.tensorflow.learners import *
+from xuanpolicy.tensorflow.utils.operations import merge_distributions
 
 
 class PPG_Learner(Learner):
     def __init__(self,
                  policy: tk.Model,
                  optimizer: tk.optimizers.Optimizer,
                  summary_writer: Optional[SummaryWriter] = None,
```

### Comparing `xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_tf/learners/policy_gradient/ppoclip_learner.py` & `xuanpolicy-0.1.6/xuanpolicy/tensorflow/learners/policy_gradient/ppoclip_learner.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from xuanpolicy.xuanpolicy_tf.learners import *
+from xuanpolicy.tensorflow.learners import *
 
 
 class PPOCLIP_Learner(Learner):
     def __init__(self,
                  policy: tk.Model,
                  optimizer: tk.optimizers.Optimizer,
                  summary_writer: Optional[SummaryWriter] = None,
```

### Comparing `xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_tf/learners/policy_gradient/ppokl_learner.py` & `xuanpolicy-0.1.6/xuanpolicy/tensorflow/learners/policy_gradient/ppokl_learner.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from torch import kl_div
-from xuanpolicy.xuanpolicy_tf.learners import *
-from xuanpolicy.xuanpolicy_tf.utils.operations import merge_distributions
+from xuanpolicy.tensorflow.learners import *
+from xuanpolicy.tensorflow.utils.operations import merge_distributions
 
 
 class PPOKL_Learner(Learner):
     def __init__(self,
                  policy: tk.Model,
                  optimizer: tk.optimizers.Optimizer,
                  summary_writer: Optional[SummaryWriter] = None,
```

### Comparing `xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_tf/learners/policy_gradient/sac_learner.py` & `xuanpolicy-0.1.6/xuanpolicy/tensorflow/learners/policy_gradient/sac_learner.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from xuanpolicy.xuanpolicy_tf.learners import *
+from xuanpolicy.tensorflow.learners import *
 
 
 class SAC_Learner(Learner):
     def __init__(self,
                  policy: tk.Model,
                  optimizers: Sequence[tk.optimizers.Optimizer],
                  summary_writer: Optional[SummaryWriter] = None,
```

### Comparing `xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_tf/learners/policy_gradient/sacdis_learner.py` & `xuanpolicy-0.1.6/xuanpolicy/tensorflow/learners/policy_gradient/sacdis_learner.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from xuanpolicy.xuanpolicy_tf.learners import *
+from xuanpolicy.tensorflow.learners import *
 
 
 class SACDIS_Learner(Learner):
     def __init__(self,
                  policy: tk.Model,
                  optimizers: Sequence[tk.optimizers.Optimizer],
                  summary_writer: Optional[SummaryWriter] = None,
```

### Comparing `xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_tf/learners/policy_gradient/spdqn_learner.py` & `xuanpolicy-0.1.6/xuanpolicy/tensorflow/learners/policy_gradient/spdqn_learner.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from xuanpolicy.xuanpolicy_tf.learners import *
+from xuanpolicy.tensorflow.learners import *
 
 class SPDQN_Learner(Learner):
     def __init__(self,
                  policy: tk.Model,
                  optimizers: Sequence[tk.optimizers.Optimizer],
                  summary_writer: Optional[SummaryWriter] = None,
                  device: str = "cpu:0",
```

### Comparing `xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_tf/learners/policy_gradient/td3_learner.py` & `xuanpolicy-0.1.6/xuanpolicy/tensorflow/learners/policy_gradient/td3_learner.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # TD3 add three tricks to DDPG:
 # 1. noisy action in target actor
 # 2. double critic network
 # 3. delayed actor update
-from xuanpolicy.xuanpolicy_tf.learners import *
+from xuanpolicy.tensorflow.learners import *
 import itertools
 
 
 class TD3_Learner(Learner):
     def __init__(self,
                  policy: tk.Model,
                  optimizers: Sequence[tk.optimizers.Optimizer],
```

### Comparing `xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_tf/learners/qlearning_family/c51_learner.py` & `xuanpolicy-0.1.6/xuanpolicy/tensorflow/learners/qlearning_family/c51_learner.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from xuanpolicy.xuanpolicy_tf.learners import *
+from xuanpolicy.tensorflow.learners import *
 
 
 class C51_Learner(Learner):
     def __init__(self,
                  policy: tk.Model,
                  optimizer: tk.optimizers.Optimizer,
                  summary_writer: Optional[SummaryWriter] = None,
```

### Comparing `xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_tf/learners/qlearning_family/cdqn_learner.py` & `xuanpolicy-0.1.6/xuanpolicy/tensorflow/learners/qlearning_family/cdqn_learner.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from xuanpolicy.xuanpolicy_tf.learners import *
+from xuanpolicy.tensorflow.learners import *
 
 
 class CDQN_Learner(Learner):
     def __init__(self,
                  policy: tk.Model,
                  optimizer: tk.optimizers.Optimizer,
                  summary_writer: Optional[SummaryWriter] = None,
```

### Comparing `xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_tf/learners/qlearning_family/cldqn_learner.py` & `xuanpolicy-0.1.6/xuanpolicy/tensorflow/learners/qlearning_family/ldqn_learner.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,24 +1,22 @@
-import tkinter
+from xuanpolicy.tensorflow.learners import *
 
-from xuanpolicy.xuanpolicy_tf.learners import *
 
-
-class CLDQN_Learner(Learner):
+class LDQN_Learner(Learner):
     def __init__(self,
                  policy: tk.Model,
                  optimizer: tk.optimizers.Optimizer,
                  summary_writer: Optional[SummaryWriter] = None,
                  device: str = "cpu:0",
                  modeldir: str = "./",
                  gamma: float = 0.99,
                  sync_frequency: int = 100):
         self.gamma = gamma
         self.sync_frequency = sync_frequency
-        super(CLDQN_Learner, self).__init__(policy, optimizer, summary_writer, device, modeldir)
+        super(LDQN_Learner, self).__init__(policy, optimizer, summary_writer, device, modeldir)
 
     def update(self, obs_batch, act_batch, rew_batch, next_batch, terminal_batch):
         self.iterations += 1
         with tf.device(self.device):
             act_batch = tf.convert_to_tensor(act_batch, dtype=tf.int32)
             rew_batch = tf.convert_to_tensor(rew_batch)
             ter_batch = tf.convert_to_tensor(terminal_batch)
@@ -26,14 +24,15 @@
             with tf.GradientTape() as tape:
                 _, _, evalQ, _ = self.policy(obs_batch)
                 _, _, _, targetQ = self.policy(next_batch)
                 targetQ = targetQ.max(dim=-1).values
                 targetQ = rew_batch + self.gamma * (1 - ter_batch) * targetQ
                 targetQ = tf.stop_gradient(targetQ)
                 predictQ = tf.math.reduce_sum(evalQ * tf.one_hot(act_batch, evalQ.shape[1]), axis=-1)
+
                 loss = tk.losses.mean_squared_error(targetQ, predictQ)
                 gradients = tape.gradient(loss, self.policy.trainable_variables)
                 self.optimizer.apply_gradients([
                     (grad, var)
                     for (grad, var) in zip(gradients, self.policy.trainable_variables)
                     if grad is not None
                 ])
```

### Comparing `xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_tf/learners/qlearning_family/ddqn_learner.py` & `xuanpolicy-0.1.6/xuanpolicy/tensorflow/learners/qlearning_family/ddqn_learner.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from xuanpolicy.xuanpolicy_tf.learners import *
+from xuanpolicy.tensorflow.learners import *
 
 
 class DDQN_Learner(Learner):
     def __init__(self,
                  policy: tk.Model,
                  optimizer: tk.optimizers.Optimizer,
                  summary_writer: Optional[SummaryWriter] = None,
```

### Comparing `xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_tf/learners/qlearning_family/dqn_learner.py` & `xuanpolicy-0.1.6/xuanpolicy/tensorflow/learners/qlearning_family/dqn_learner.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from xuanpolicy.xuanpolicy_tf.learners import *
+from xuanpolicy.tensorflow.learners import *
 
 
 class DQN_Learner(Learner):
     def __init__(self,
                  policy: tk.Model,
                  optimizer: tk.optimizers.Optimizer,
                  summary_writer: Optional[SummaryWriter] = None,
```

### Comparing `xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_tf/learners/qlearning_family/dueldqn_learner.py` & `xuanpolicy-0.1.6/xuanpolicy/tensorflow/learners/qlearning_family/dueldqn_learner.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from xuanpolicy.xuanpolicy_tf.learners import *
+from xuanpolicy.tensorflow.learners import *
 
 
 class DuelDQN_Learner(Learner):
     def __init__(self,
                  policy: tk.Model,
                  optimizer: tk.optimizers.Optimizer,
                  summary_writer: Optional[SummaryWriter] = None,
```

### Comparing `xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_tf/learners/qlearning_family/ldqn_learner.py` & `xuanpolicy-0.1.6/xuanpolicy/tensorflow/learners/qlearning_family/perdqn_learner.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,38 +1,39 @@
-from xuanpolicy.xuanpolicy_tf.learners import *
+from xuanpolicy.tensorflow.learners import *
 
 
-class LDQN_Learner(Learner):
+class PerDQN_Learner(Learner):
     def __init__(self,
                  policy: tk.Model,
                  optimizer: tk.optimizers.Optimizer,
                  summary_writer: Optional[SummaryWriter] = None,
                  device: str = "cpu:0",
                  modeldir: str = "./",
                  gamma: float = 0.99,
                  sync_frequency: int = 100):
         self.gamma = gamma
         self.sync_frequency = sync_frequency
-        super(LDQN_Learner, self).__init__(policy, optimizer, summary_writer, device, modeldir)
+        super(PerDQN_Learner, self).__init__(policy, optimizer, summary_writer, device, modeldir)
 
     def update(self, obs_batch, act_batch, rew_batch, next_batch, terminal_batch):
         self.iterations += 1
         with tf.device(self.device):
             act_batch = tf.convert_to_tensor(act_batch, dtype=tf.int32)
             rew_batch = tf.convert_to_tensor(rew_batch)
             ter_batch = tf.convert_to_tensor(terminal_batch)
 
             with tf.GradientTape() as tape:
                 _, _, evalQ, _ = self.policy(obs_batch)
                 _, _, _, targetQ = self.policy(next_batch)
-                targetQ = targetQ.max(dim=-1).values
+                targetQ = tf.math.reduce_max(targetQ, axis=-1)
                 targetQ = rew_batch + self.gamma * (1 - ter_batch) * targetQ
                 targetQ = tf.stop_gradient(targetQ)
                 predictQ = tf.math.reduce_sum(evalQ * tf.one_hot(act_batch, evalQ.shape[1]), axis=-1)
 
+                td_error = targetQ - predictQ
                 loss = tk.losses.mean_squared_error(targetQ, predictQ)
                 gradients = tape.gradient(loss, self.policy.trainable_variables)
                 self.optimizer.apply_gradients([
                     (grad, var)
                     for (grad, var) in zip(gradients, self.policy.trainable_variables)
                     if grad is not None
                 ])
@@ -41,7 +42,9 @@
             if self.iterations % self.sync_frequency == 0:
                 self.policy.copy_target()
 
             lr = self.optimizer._decayed_lr(tf.float32)
             self.writer.add_scalar("Qloss", loss.numpy(), self.iterations)
             self.writer.add_scalar("predictQ", tf.math.reduce_mean(predictQ).numpy(), self.iterations)
             self.writer.add_scalar("lr", lr.numpy(), self.iterations)
+
+            return np.abs(td_error.numpy())
```

### Comparing `xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_tf/learners/qlearning_family/perdqn_learner.py` & `xuanpolicy-0.1.6/xuanpolicy/tensorflow/learners/qlearning_family/cldqn_learner.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,39 +1,39 @@
-from xuanpolicy.xuanpolicy_tf.learners import *
+import tkinter
 
+from xuanpolicy.tensorflow.learners import *
 
-class PerDQN_Learner(Learner):
+
+class CLDQN_Learner(Learner):
     def __init__(self,
                  policy: tk.Model,
                  optimizer: tk.optimizers.Optimizer,
                  summary_writer: Optional[SummaryWriter] = None,
                  device: str = "cpu:0",
                  modeldir: str = "./",
                  gamma: float = 0.99,
                  sync_frequency: int = 100):
         self.gamma = gamma
         self.sync_frequency = sync_frequency
-        super(PerDQN_Learner, self).__init__(policy, optimizer, summary_writer, device, modeldir)
+        super(CLDQN_Learner, self).__init__(policy, optimizer, summary_writer, device, modeldir)
 
     def update(self, obs_batch, act_batch, rew_batch, next_batch, terminal_batch):
         self.iterations += 1
         with tf.device(self.device):
             act_batch = tf.convert_to_tensor(act_batch, dtype=tf.int32)
             rew_batch = tf.convert_to_tensor(rew_batch)
             ter_batch = tf.convert_to_tensor(terminal_batch)
 
             with tf.GradientTape() as tape:
                 _, _, evalQ, _ = self.policy(obs_batch)
                 _, _, _, targetQ = self.policy(next_batch)
-                targetQ = tf.math.reduce_max(targetQ, axis=-1)
+                targetQ = targetQ.max(dim=-1).values
                 targetQ = rew_batch + self.gamma * (1 - ter_batch) * targetQ
                 targetQ = tf.stop_gradient(targetQ)
                 predictQ = tf.math.reduce_sum(evalQ * tf.one_hot(act_batch, evalQ.shape[1]), axis=-1)
-
-                td_error = targetQ - predictQ
                 loss = tk.losses.mean_squared_error(targetQ, predictQ)
                 gradients = tape.gradient(loss, self.policy.trainable_variables)
                 self.optimizer.apply_gradients([
                     (grad, var)
                     for (grad, var) in zip(gradients, self.policy.trainable_variables)
                     if grad is not None
                 ])
@@ -42,9 +42,7 @@
             if self.iterations % self.sync_frequency == 0:
                 self.policy.copy_target()
 
             lr = self.optimizer._decayed_lr(tf.float32)
             self.writer.add_scalar("Qloss", loss.numpy(), self.iterations)
             self.writer.add_scalar("predictQ", tf.math.reduce_mean(predictQ).numpy(), self.iterations)
             self.writer.add_scalar("lr", lr.numpy(), self.iterations)
-
-            return np.abs(td_error.numpy())
```

### Comparing `xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_tf/learners/qlearning_family/qrdqn_learner.py` & `xuanpolicy-0.1.6/xuanpolicy/tensorflow/learners/qlearning_family/qrdqn_learner.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from xuanpolicy.xuanpolicy_tf.learners import *
+from xuanpolicy.tensorflow.learners import *
 
 
 class QRDQN_Learner(Learner):
     def __init__(self,
                  policy: tk.Model,
                  optimizer: tk.optimizers.Optimizer,
                  summary_writer: Optional[SummaryWriter] = None,
```

### Comparing `xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_tf/policies/__init__.py` & `xuanpolicy-0.1.6/xuanpolicy/tensorflow/policies/__init__.py`

 * *Files identical despite different names*

### Comparing `xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_tf/policies/categorical.py` & `xuanpolicy-0.1.6/xuanpolicy/tensorflow/policies/categorical.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-from xuanpolicy.xuanpolicy_tf.policies import *
-from xuanpolicy.xuanpolicy_tf.utils import *
+from xuanpolicy.tensorflow.policies import *
+from xuanpolicy.tensorflow.utils import *
 
 
 class ActorNet(tk.Model):
     def __init__(self,
                  state_dim: int,
                  action_dim: int,
                  hidden_sizes: Sequence[int],
```

### Comparing `xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_tf/policies/categorical_marl.py` & `xuanpolicy-0.1.6/xuanpolicy/tensorflow/policies/categorical_marl.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-from xuanpolicy.xuanpolicy_tf.policies import *
-from xuanpolicy.xuanpolicy_tf.utils import *
-from xuanpolicy.xuanpolicy_tf.representations import Basic_Identical
+from xuanpolicy.tensorflow.policies import *
+from xuanpolicy.tensorflow.utils import *
+from xuanpolicy.tensorflow.representations import Basic_Identical
 from .deterministic_marl import BasicQhead
 
 
 class ActorNet(tk.Model):
     def __init__(self,
                  state_dim: int,
                  action_dim: int,
```

### Comparing `xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_tf/policies/deterministic.py` & `xuanpolicy-0.1.6/xuanpolicy/tensorflow/policies/deterministic.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-from xuanpolicy.xuanpolicy_tf.policies import *
-from xuanpolicy.xuanpolicy_tf.utils import *
-from xuanpolicy.xuanpolicy_tf.representations import Basic_Identical
-from xuanpolicy.xuanpolicy_tf.representations import C_DQN, L_DQN, CL_DQN
+from xuanpolicy.tensorflow.policies import *
+from xuanpolicy.tensorflow.utils import *
+from xuanpolicy.tensorflow.representations import Basic_Identical
+from xuanpolicy.tensorflow.representations import C_DQN, L_DQN, CL_DQN
 
 
 class BasicQhead(tk.Model):
     def __init__(self,
                  state_dim: int,
                  action_dim: int,
                  hidden_sizes: Sequence[int],
```

### Comparing `xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_tf/policies/deterministic_marl.py` & `xuanpolicy-0.1.6/xuanpolicy/tensorflow/policies/deterministic_marl.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-from xuanpolicy.xuanpolicy_tf.policies import *
-from xuanpolicy.xuanpolicy_tf.utils import *
-from xuanpolicy.xuanpolicy_tf.representations import Basic_Identical
+from xuanpolicy.tensorflow.policies import *
+from xuanpolicy.tensorflow.utils import *
+from xuanpolicy.tensorflow.representations import Basic_Identical
 
 from itertools import chain
 
 
 class BasicQhead(tk.Model):
     def __init__(self,
                  state_dim: int,
```

### Comparing `xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_tf/policies/gaussian.py` & `xuanpolicy-0.1.6/xuanpolicy/tensorflow/policies/gaussian.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-from xuanpolicy.xuanpolicy_tf.policies import *
-from xuanpolicy.xuanpolicy_tf.utils import *
-from xuanpolicy.xuanpolicy_tf.representations import Basic_Identical
+from xuanpolicy.tensorflow.policies import *
+from xuanpolicy.tensorflow.utils import *
+from xuanpolicy.tensorflow.representations import Basic_Identical
 import tensorflow_probability as tfp
 
 tfd = tfp.distributions
 
 
 class ActorNet(tk.Model):
     def __init__(self,
```

### Comparing `xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_tf/policies/gaussian_marl.py` & `xuanpolicy-0.1.6/xuanpolicy/tensorflow/policies/gaussian_marl.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-from xuanpolicy.xuanpolicy_tf.policies import *
-from xuanpolicy.xuanpolicy_tf.utils import *
-from xuanpolicy.xuanpolicy_tf.representations import Basic_Identical
+from xuanpolicy.tensorflow.policies import *
+from xuanpolicy.tensorflow.utils import *
+from xuanpolicy.tensorflow.representations import Basic_Identical
 import tensorflow_probability as tfp
 
 tfd = tfp.distributions
 
 
 class BasicQhead(tk.Model):
     def __init__(self,
```

### Comparing `xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_tf/policies/mixers.py` & `xuanpolicy-0.1.6/xuanpolicy/tensorflow/policies/mixers.py`

 * *Files identical despite different names*

### Comparing `xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_tf/representations/__init__.py` & `xuanpolicy-0.1.6/xuanpolicy/tensorflow/representations/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import tensorflow as tf
 import numpy as np
 from typing import Sequence, Union, Optional, Callable
-from xuanpolicy.xuanpolicy_tf.utils.layers import *
+from xuanpolicy.tensorflow.utils.layers import *
 
 from .networks import Basic_Identical, Basic_MLP, Basic_CNN
 from .networks import CoG_MLP, CoG_RNN, CoG_CNN
 from .networks import C_DQN, L_DQN, CL_DQN
 
 REGISTRY = {
     "Basic_MLP": Basic_MLP,
```

### Comparing `xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_tf/representations/networks.py` & `xuanpolicy-0.1.6/xuanpolicy/tensorflow/representations/networks.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from xuanpolicy.xuanpolicy_tf.representations import *
+from xuanpolicy.tensorflow.representations import *
 
 
 class Basic_Identical(tk.Model):
     def __init__(self,
                  input_shape: Sequence[int],
                  device: str = "cpu"):
         super(Basic_Identical, self).__init__()
```

### Comparing `xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_tf/runners/runner_basic.py` & `xuanpolicy-0.1.6/xuanpolicy/tensorflow/runners/runner_basic.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,30 +1,38 @@
+import time
 from xuanpolicy.environment import make_envs
-import tensorflow as tf
 import tensorflow.keras as tk
 
 
 class Runner_Base(object):
     def __init__(self, args):
         # build environments
-        self.envs = make_envs(args.env_name, args.env_id, args.seed, args.vectorize, args.parallels)
+        if hasattr(args, 'continuous_action'):
+            self.envs = make_envs(args.env_name, args.env_id, args.seed, args.vectorize, args.parallels,
+                                  args.continuous_action, args.render_mode)
+        else:
+            self.envs = make_envs(args.env_name, args.env_id, args.seed, args.vectorize, args.parallels,
+                                  args.render_mode)
+
         if args.vectorize != 'NOREQUIRED':
             self.n_envs = self.envs.num_envs
 
         self.train_at_step = args.train_at_step
 
     def run(self):
         pass
 
     def tb_load(self, data):
         return
 
 
 class Runner_Base_MARL(Runner_Base):
     def __init__(self, args):
+        if args.test_mode:
+            args.render_mode = 'human'
         super(Runner_Base_MARL, self).__init__(args)
         # build environments
         self.n_handles = len(self.envs.handles)
         self.loss = [[0.0] for _ in range(self.n_handles)]
 
         self.agent_keys = self.envs.agent_keys
         self.agent_ids = self.envs.agent_ids
@@ -87,14 +95,15 @@
         for h, arg in enumerate(args):
             agent_name = self.envs.agent_keys[h][0][0:-2]
             if arg.n_agents == 1:
                 infos.append(agent_name + ": {} agent".format(arg.n_agents) + ", {}".format(arg.agent))
             else:
                 infos.append(agent_name + ": {} agents".format(arg.n_agents) + ", {}".format(arg.agent))
         print(infos)
+        time.sleep(0.01)
 
 
 class MyLinearLR(tk.optimizers.schedules.LearningRateSchedule):
     def __init__(self, initial_learning_rate, start_factor, end_factor, total_iters):
         self.initial_learning_rate = initial_learning_rate
         self.start_factor = start_factor
         self.end_factor = end_factor
```

### Comparing `xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_tf/runners/runner_drl.py` & `xuanpolicy-0.1.6/xuanpolicy/tensorflow/runners/runner_drl.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from .runner_basic import *
-from xuanpolicy.xuanpolicy_tf.agents import get_total_iters
-from xuanpolicy.xuanpolicy_tf.representations import REGISTRY as REGISTRY_Representation
-from xuanpolicy.xuanpolicy_tf.agents import REGISTRY as REGISTRY_Agent
-from xuanpolicy.xuanpolicy_tf.policies import REGISTRY as REGISTRY_Policy
-from xuanpolicy.xuanpolicy_tf.utils.input_reformat import get_repre_in, get_policy_in
+from xuanpolicy.tensorflow.agents import get_total_iters
+from xuanpolicy.tensorflow.representations import REGISTRY as REGISTRY_Representation
+from xuanpolicy.tensorflow.agents import REGISTRY as REGISTRY_Agent
+from xuanpolicy.tensorflow.policies import REGISTRY as REGISTRY_Policy
+from xuanpolicy.tensorflow.utils.input_reformat import get_repre_in, get_policy_in
 import tensorflow.keras as tk
 import gym.spaces
 import numpy as np
 
 
 class Runner_DRL(Runner_Base):
     def __init__(self, args):
@@ -62,8 +62,9 @@
             #                           total_iters=get_total_iters(self.agent_name, self.args))
             lr_scheduler = tk.optimizers.schedules.ExponentialDecay(self.args.learning_rate, decay_steps=1000,
                                                                     decay_rate=0.9)
             optimizer = tk.optimizers.Adam(lr_scheduler)
             self.agent = REGISTRY_Agent[self.agent_name](self.args, self.envs, policy, optimizer, self.args.device)
 
     def run(self):
-        self.agent.test() if self.args.test_mode else self.agent.train(self.args.training_steps)
+        self.agent.test(self.args.test_steps) if self.args.test_mode else self.agent.train(self.args.training_steps)
+        self.envs.close()
```

### Comparing `xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_tf/runners/runner_marl.py` & `xuanpolicy-0.1.6/xuanpolicy/torch/runners/runner_marl.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,22 +1,26 @@
+import time
+
 from .runner_basic import *
-from xuanpolicy.xuanpolicy_tf.agents import REGISTRY as REGISTRY_Agent
-from gym.spaces import Box
+from xuanpolicy.torch.agents import REGISTRY as REGISTRY_Agent
+from gymnasium.spaces.box import Box
 from tqdm import tqdm
 import numpy as np
 from copy import deepcopy
 
 
 class Runner(Runner_Base_MARL):
     def __init__(self, args):
         self.args = args if type(args) == list else [args]
         super(Runner, self).__init__(self.args[0])
 
         # environment details, representations, policies, optimizers, and agents.
         for h, arg in enumerate(self.args):
+            if self.n_handles > 1 and arg.agent != "RANDOM":
+                arg.modeldir += "side_{}/".format(h)
             arg.handle, arg.n_agents = h, self.envs.n_agents[h]
             arg.agent_keys, arg.agent_ids = self.agent_keys[h], self.agent_ids[h]
             arg.state_space = self.envs.state_space
             arg.observation_space = self.envs.observation_space
             if isinstance(self.envs.action_space[self.agent_keys[h][0]], Box):
                 arg.dim_act = self.envs.action_space[self.agent_keys[h][0]].shape[0]
                 arg.act_shape = (arg.n_agents,) + (arg.dim_act,)
@@ -44,15 +48,16 @@
 
         while True:
             actions_dict = self.get_actions(obs_n, episode, test_mode, act_mean_last, agent_mask, state)
             actions_execute = self.combine_env_actions(actions_dict['actions_n'])
             next_obs_n, rew_n, done_n, dones, info = self.envs.step(actions_execute)
             next_state, agent_mask = self.envs.global_state(), self.envs.agent_mask()
 
-            if self.render or self.test_mode: self.envs.render(self.render_delay)
+            if self.render or self.test_mode:
+                time.sleep(self.render_delay)
             if test_mode:
                 for h in range(self.n_handles):
                     scores[h] += (1-done_envs) * np.mean(rew_n[h] * agent_mask[h][:, :, np.newaxis], axis=1)
             else:
                 self.store_data(obs_n, next_obs_n, actions_dict, state, next_state, agent_mask, rew_n, done_n, self.envs)
                 for h, mas_group in enumerate(self.marl_agents):
                     if self.args[h].train_at_step: self.marl_agents[h].train(episode)
@@ -61,26 +66,31 @@
 
             for e, d in enumerate(dones):
                 if d:  # if done, then reset this environment
                     done_envs[e], obs_reset = d, self.envs.reset_one_env(e)
                     state[e] = self.envs.global_state_one_env(e)
                     if not test_mode:
                         for h, mas_group in enumerate(self.marl_agents):
+                            if mas_group.args.agent_name == "random":
+                                continue
                             obs_n[h][e], act_mean_last[h][e] = obs_reset[h], np.zeros([self.args[h].dim_act])
                             if (self.marl_names[h] in ["MAPPO", "CID_Simple", "VDAC"]) and (not self.args[h].consider_terminal_states):
                                 value_next_e = mas_group.value(next_obs_n[h], next_state)[e]
                             else:
                                 value_next_e = np.zeros([mas_group.n_agents, 1])
                             mas_group.memory.finish_ac_path(value_next_e, e)
 
-            if all(done_envs): break
+            if all(done_envs):
+                break
 
         # train the model
         if not test_mode:
             for h, mas_group in enumerate(self.marl_agents):
+                if mas_group.args.agent_name == "random":
+                    continue
                 if not self.args[h].train_at_step:
                     mas_group.train(episode)
 
         return scores
 
     def run(self):
         for i_episode in tqdm(range(self.n_episodes)):
@@ -90,23 +100,27 @@
             if (i_episode % self.test_period == 0) and (not self.test_mode):
                 reward = np.zeros([self.n_handles, self.n_envs, 1])
                 for i_test in range(self.n_tests):
                     r_episode = self.run_episode(i_episode, test_mode=True)
                     reward += r_episode
                 reward = reward / self.n_tests
                 for h, mas_group in enumerate(self.marl_agents):
+                    if mas_group.args.agent_name == "random":
+                        continue
                     for i in range(self.n_envs):
                         self.marl_agents[h].writer.add_scalars("reward_mean", {"env-%d" % i: reward[h, i]}, i_episode)
-        for h, mas_group in enumerate(self.marl_agents):
-            mas_group.save_model()
+                    if i_episode % 5000 == 0 or i_episode == self.n_episodes - 1:
+                        mas_group.save_model()
 
         self.envs.close()
 
     def store_data(self, obs_n, next_obs_n, actions_dict, state, next_state, agent_mask, rew_n, done_n, env):
         for h, mas_group in enumerate(self.marl_agents):
+            if mas_group.args.agent_name == "random":
+                continue
             data_step = {'obs': obs_n[h], 'obs_next': next_obs_n[h], 'actions': actions_dict['actions_n'][h],
                          'state': state, 'state_next': next_state, 'rewards': rew_n[h],
                          'agent_mask': agent_mask[h], 'terminals': done_n[h]}
             if self.marl_names[h] in ["CID_Simple", "CID_Rainbow"]:
                 rew_n_assign = mas_group.reward_shaping(state, obs_n[h], actions_dict['actions_n'][h], rew_n[h], env)
                 data_step.update({'rewards_assign': rew_n_assign})
             elif self.marl_names[h] in ["MAPPO_KL", "MAPPO_Clip", "VDAC"]:
```

### Comparing `xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_tf/utils/distributions.py` & `xuanpolicy-0.1.6/xuanpolicy/tensorflow/utils/distributions.py`

 * *Files identical despite different names*

### Comparing `xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_tf/utils/input_reformat.py` & `xuanpolicy-0.1.6/xuanpolicy/tensorflow/utils/input_reformat.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from xuanpolicy.common import space2shape
 from copy import deepcopy
-from xuanpolicy.xuanpolicy_tf.policies import Policy_Inputs, Policy_Inputs_All
-from xuanpolicy.xuanpolicy_tf.representations import Representation_Inputs, Representation_Inputs_All
+from xuanpolicy.tensorflow.policies import Policy_Inputs, Policy_Inputs_All
+from xuanpolicy.tensorflow.representations import Representation_Inputs, Representation_Inputs_All
 from operator import itemgetter
 import tensorflow.keras as tk
 
 
 def get_repre_in(args):
     representation_name = args.representation
     input_dict = deepcopy(Representation_Inputs_All)
```

### Comparing `xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_tf/utils/layers.py` & `xuanpolicy-0.1.6/xuanpolicy/tensorflow/utils/layers.py`

 * *Files identical despite different names*

### Comparing `xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_tf/utils/operations.py` & `xuanpolicy-0.1.6/xuanpolicy/tensorflow/utils/operations.py`

 * *Files identical despite different names*

### Comparing `xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_torch/agents/__init__.py` & `xuanpolicy-0.1.6/xuanpolicy/torch/agents/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,20 +5,20 @@
 from tqdm import tqdm
 from torch.utils.tensorboard import SummaryWriter
 import torch
 import torch.nn as nn
 import torch.nn.functional as F
 from xuanpolicy.environment import *
 from xuanpolicy.common import *
-from xuanpolicy.xuanpolicy_torch.learners import *
-from xuanpolicy.xuanpolicy_torch.policies import *
-from xuanpolicy.xuanpolicy_torch.utils import *
-from xuanpolicy.xuanpolicy_torch.policies import REGISTRY as REGISTRY_Policy
-from xuanpolicy.xuanpolicy_torch.utils.input_reformat import get_repre_in, get_policy_in_marl
-from xuanpolicy.xuanpolicy_torch.representations import REGISTRY as REGISTRY_Representation
+from xuanpolicy.torch.learners import *
+from xuanpolicy.torch.policies import *
+from xuanpolicy.torch.utils import *
+from xuanpolicy.torch.policies import REGISTRY as REGISTRY_Policy
+from xuanpolicy.torch.utils.input_reformat import get_repre_in, get_policy_in_marl
+from xuanpolicy.torch.representations import REGISTRY as REGISTRY_Representation
 
 from .agent import Agent
 from .agents_marl import MARLAgents, RandomAgents, get_total_iters
 
 '''
 Single-Agent DRL algorithms
 '''
```

### Comparing `xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_torch/agents/agent.py` & `xuanpolicy-0.1.6/xuanpolicy/mindspore/agents/agent.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,27 +1,25 @@
-from xuanpolicy.xuanpolicy_torch.agents import *
+from xuanpolicy.mindspore.agents import *
 
 
 class Agent(ABC):
     def __init__(self,
                  envs: VecEnv,
-                 policy: nn.Module,
+                 policy: nn.Cell,
                  memory: Buffer,
                  learner: Learner,
                  writer: SummaryWriter,
-                 device: Optional[Union[str, int, torch.device]] = None,
                  logdir: str = "./logs/",
                  modeldir: str = "./models/",
                  ):
         self.envs = envs
         self.policy = policy
         self.memory = memory
         self.learner = learner
         self.writer = writer
-        self.device = device
         self.logdir = logdir
         self.modeldir = modeldir
         create_directory(logdir)
         create_directory(modeldir)
 
     def save_model(self):
         self.learner.save_model()
```

### Comparing `xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_torch/agents/agents_marl.py` & `xuanpolicy-0.1.6/xuanpolicy/torch/agents/agents_marl.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from xuanpolicy.xuanpolicy_torch.agents import *
+from xuanpolicy.torch.agents import *
 
 
 class MARLAgents(object):
     def __init__(self,
                  config: Namespace,
                  envs: DummyVecEnv_MAS,
                  policy: nn.Module,
@@ -89,14 +89,19 @@
 def get_total_iters(agent_name, args):
     if agent_name in ["A2C", "A3C", "PG", "PPO_Clip","PPO_KL","PPG","VDAC", "COMA", "MFAC", "MAPPO_Clip", "MAPPO_KL"]:
         return int(args.training_steps * args.nepoch * args.nminibatch / args.nsteps)
     else:
         return int(args.training_steps / args.training_frequency)
 
 
-class RandomAgents(MARLAgents):
-    def __init__(self, args):
-        super(RandomAgents, self).__init__(args)
+class RandomAgents(object):
+    def __init__(self, args, envs, device=None):
+        self.args = args
+        self.n_agents = self.args.n_agents
+        self.agent_keys = args.agent_keys
+        self.action_space = self.args.action_space
+        self.nenvs = envs.num_envs
 
     def act(self, obs_n, episode, test_mode, noise=False):
-        random_actions = np.array([[self.args.action_space[agent].sample() for agent in self.agent_keys]])
+        rand_a = [[self.action_space[agent].sample() for agent in self.agent_keys] for e in range(self.nenvs)]
+        random_actions = np.array(rand_a)
         return random_actions
```

### Comparing `xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_torch/agents/multi_agent_rl/coma_agents.py` & `xuanpolicy-0.1.6/xuanpolicy/torch/agents/multi_agent_rl/matd3_agents.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,64 +1,67 @@
-from xuanpolicy.xuanpolicy_torch.agents import *
-from xuanpolicy.xuanpolicy_torch.agents.agents_marl import linear_decay_or_increase
+from xuanpolicy.torch.agents import *
 
 
-class COMA_Agents(MARLAgents):
+class MATD3_Agents(MARLAgents):
     def __init__(self,
                  config: Namespace,
                  envs: DummyVecEnv_MAS,
                  device: Optional[Union[int, str, torch.device]] = None):
         self.comm = MPI.COMM_WORLD
-        config.batch_size = config.batch_size * envs.num_envs
 
         self.gamma = config.gamma
         self.use_obsnorm = config.use_obsnorm
         self.use_rewnorm = config.use_rewnorm
         self.obsnorm_range = config.obsnorm_range
         self.rewnorm_range = config.rewnorm_range
 
-        if config.state_space is not None:
-            config.dim_state, state_shape = config.state_space.shape, config.state_space.shape
-        else:
-            config.dim_state, state_shape = None, None
-
         input_representation = get_repre_in(config)
         representation = REGISTRY_Representation[config.representation](*input_representation)
-        input_policy = get_policy_in_marl(config, representation, config.agent_keys, None)
+        input_policy = get_policy_in_marl(config, representation, config.agent_keys)
         policy = REGISTRY_Policy[config.policy](*input_policy)
-        optimizer = [torch.optim.Adam(policy.parameters_actor, config.learning_rate_actor, eps=1e-5),
-                     torch.optim.Adam(policy.parameters_critic, config.learning_rate_critic, eps=1e-5)]
+        optimizer = [torch.optim.Adam(policy.parameters_actor, config.lr_a, eps=1e-5),
+                     torch.optim.Adam(policy.critic_net_A.parameters(), config.lr_c, eps=1e-5),
+                     torch.optim.Adam(policy.critic_net_B.parameters(), config.lr_c, eps=1e-5)]
         scheduler = [torch.optim.lr_scheduler.LinearLR(optimizer[0], start_factor=1.0, end_factor=0.5,
                                                        total_iters=get_total_iters(config.agent_name, config)),
                      torch.optim.lr_scheduler.LinearLR(optimizer[1], start_factor=1.0, end_factor=0.5,
+                                                       total_iters=get_total_iters(config.agent_name, config)),
+                     torch.optim.lr_scheduler.LinearLR(optimizer[2], start_factor=1.0, end_factor=0.5,
                                                        total_iters=get_total_iters(config.agent_name, config))]
         self.observation_space = envs.observation_space
         self.action_space = envs.action_space
+        self.actions_high, self.actions_low = [], []
+        for k in config.agent_keys:
+            self.actions_high.append(self.action_space[k].high)
+            self.actions_low.append(self.action_space[k].low)
+        self.actions_high, self.actions_low = np.array(self.actions_high), np.array(self.actions_low)
         self.representation_info_shape = policy.representation.output_shapes
         self.auxiliary_info_shape = {}
 
         writer = SummaryWriter(config.logdir)
         if config.state_space is not None:
             config.dim_state, state_shape = config.state_space.shape, config.state_space.shape
         else:
             config.dim_state, state_shape = None, None
-        config.act_onehot_shape = config.act_shape + tuple([config.dim_act])
-        memory = COMA_Buffer(state_shape, config.obs_shape, config.act_shape, config.act_onehot_shape,
-                             config.rew_shape, config.done_shape, envs.num_envs,
-                             config.buffer_size, config.batch_size, envs.envs[0].max_cycles)
-        learner = COMA_Learner(config, policy, optimizer, scheduler, writer,
-                               config.device, config.modeldir, config.gamma, config.sync_frequency)
+        memory = MARL_OffPolicyBuffer(state_shape,
+                                      config.obs_shape,
+                                      config.act_shape,
+                                      config.rew_shape,
+                                      config.done_shape,
+                                      envs.num_envs,
+                                      config.buffer_size,
+                                      config.batch_size)
+        learner = MATD3_Learner(config, policy, optimizer, scheduler, writer,
+                                 config.device, config.modeldir, config.gamma)
 
         self.obs_rms = RunningMeanStd(shape=space2shape(self.observation_space[config.agent_keys[0]]),
                                       comm=self.comm, use_mpi=False)
         self.ret_rms = RunningMeanStd(shape=(), comm=self.comm, use_mpi=False)
-        self.epsilon_decay = linear_decay_or_increase(config.start_greedy, config.end_greedy,
-                                                      config.greedy_update_steps)
-        super(COMA_Agents, self).__init__(config, envs, policy, memory, learner, writer, device,
-                                          config.logdir, config.modeldir)
+        super(MATD3_Agents, self).__init__(config, envs, policy, memory, learner, writer, device,
+                                            config.logdir, config.modeldir)
 
     def _process_observation(self, observations):
         if self.use_obsnorm:
             if isinstance(self.observation_space, Dict):
                 for key in self.observation_space.spaces.keys():
                     observations[key] = np.clip(
                         (observations[key] - self.obs_rms.mean[key]) / (self.obs_rms.std[key] + EPS),
@@ -74,30 +77,18 @@
             std = np.clip(self.ret_rms.std, 0.1, 100)
             return np.clip(rewards / std, -self.rewnorm_range, self.rewnorm_range)
         return rewards
 
     def act(self, obs_n, episode, test_mode, noise=False):
         batch_size = len(obs_n)
         agents_id = torch.eye(self.n_agents).unsqueeze(0).expand(batch_size, -1, -1).to(self.device)
-        states, dists = self.policy(obs_n, agents_id)
-        # acts = dists.stochastic_sample()  # stochastic policy
-        epsilon = 1.0 if test_mode else self.epsilon_decay.epsilon
-        greedy_actions = dists.logits.argmax(dim=-1, keepdims=False)
+        _, actions = self.policy(torch.Tensor(obs_n), agents_id)
+        actions = actions.cpu().detach().numpy()
         if noise:
-            random_variable = np.random.random(greedy_actions.shape)
-            action_pick = np.int32((random_variable < epsilon))
-            random_actions = np.array([[self.args.action_space[agent].sample() for agent in self.agent_keys]])
-            actions_select = action_pick * greedy_actions.cpu().numpy() + (1 - action_pick) * random_actions
-            actions_onehot = self.learner.onehot_action(torch.Tensor(actions_select), self.dim_act)
-            return actions_select, actions_onehot.detach().cpu().numpy()
-        else:
-            actions_onehot = self.learner.onehot_action(greedy_actions, self.dim_act)
-            return greedy_actions.detach().cpu().numpy(), actions_onehot.detach().cpu().numpy()
+            actions += np.random.normal(0, self.args.sigma, size=actions.shape)
+            actions = np.clip(actions, self.actions_low, self.actions_high)
+        return actions
 
     def train(self, i_episode):
-        self.epsilon_decay.update()
-        for i in range(self.nenvs):
-            self.writer.add_scalars("epsilon", {"env-%d" % i: self.epsilon_decay.epsilon}, i_episode)
-        if self.memory.full:
+        if self.memory.can_sample(self.args.batch_size):
             sample = self.memory.sample()
             self.learner.update(sample)
-        # self.memory.clear()
```

### Comparing `xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_torch/agents/multi_agent_rl/dcg_agents.py` & `xuanpolicy-0.1.6/xuanpolicy/torch/agents/multi_agent_rl/dcg_agents.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import torch.nn
 
-from xuanpolicy.xuanpolicy_torch.agents import *
-from xuanpolicy.xuanpolicy_torch.agents.agents_marl import linear_decay_or_increase
+from xuanpolicy.torch.agents import *
+from xuanpolicy.torch.agents.agents_marl import linear_decay_or_increase
 
 
 class DCG_Agents(MARLAgents):
     def __init__(self,
                  config: Namespace,
                  envs: DummyVecEnv_MAS,
                  device: Optional[Union[int, str, torch.device]] = None):
@@ -20,15 +20,15 @@
         self.start_greedy = config.start_greedy
         self.end_greedy = config.end_greedy
         self.egreedy = config.start_greedy
 
         input_representation = get_repre_in(config)
         representation = REGISTRY_Representation[config.representation](*input_representation)
         repre_state_dim = config.representation_hidden_size[-1]
-        from xuanpolicy.xuanpolicy_torch.policies.coordination_graph import DCG_utility, DCG_payoff, Coordination_Graph
+        from xuanpolicy.torch.policies.coordination_graph import DCG_utility, DCG_payoff, Coordination_Graph
         utility = DCG_utility(repre_state_dim, config.hidden_utility_dim, config.dim_act).to(device)
         payoffs = DCG_payoff(repre_state_dim * 2, config.hidden_payoff_dim, config.dim_act, config).to(device)
         dcgraph = Coordination_Graph(config.n_agents, config.graph_type)
         dcgraph.set_coordination_graph(device)
         if config.agent == "DCG_S":
             policy = REGISTRY_Policy[config.policy](config.action_space[config.agent_keys[0]],
                                                     config.state_space.shape[0], representation,
@@ -56,15 +56,15 @@
                                       config.obs_shape,
                                       config.act_shape,
                                       config.rew_shape,
                                       config.done_shape,
                                       envs.num_envs,
                                       config.buffer_size,
                                       config.batch_size)
-        from xuanpolicy.xuanpolicy_torch.learners.multi_agent_rl.dcg_learner import DCG_Learner
+        from xuanpolicy.torch.learners.multi_agent_rl.dcg_learner import DCG_Learner
         learner = DCG_Learner(config, policy, optimizer, scheduler, writer,
                               config.device, config.modeldir, config.gamma,
                               config.sync_frequency)
 
         self.obs_rms = RunningMeanStd(shape=space2shape(self.observation_space[config.agent_keys[0]]),
                                       comm=self.comm, use_mpi=False)
         self.ret_rms = RunningMeanStd(shape=(), comm=self.comm, use_mpi=False)
```

### Comparing `xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_torch/agents/multi_agent_rl/iddpg_agents.py` & `xuanpolicy-0.1.6/xuanpolicy/torch/agents/multi_agent_rl/qmix_agents.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,59 +1,66 @@
-from xuanpolicy.xuanpolicy_torch.agents import *
+from xuanpolicy.torch.agents import *
+from xuanpolicy.torch.agents.agents_marl import linear_decay_or_increase
 
 
-class IDDPG_Agents(MARLAgents):
+class QMIX_Agents(MARLAgents):
     def __init__(self,
                  config: Namespace,
                  envs: DummyVecEnv_MAS,
                  device: Optional[Union[int, str, torch.device]] = None):
         self.comm = MPI.COMM_WORLD
 
         self.gamma = config.gamma
         self.use_obsnorm = config.use_obsnorm
         self.use_rewnorm = config.use_rewnorm
         self.obsnorm_range = config.obsnorm_range
         self.rewnorm_range = config.rewnorm_range
 
+        self.start_greedy = config.start_greedy
+        self.end_greedy = config.end_greedy
+        self.egreedy = config.start_greedy
+        if config.state_space is not None:
+            config.dim_state, state_shape = config.state_space.shape, config.state_space.shape
+        else:
+            config.dim_state, state_shape = None, None
+
         input_representation = get_repre_in(config)
         representation = REGISTRY_Representation[config.representation](*input_representation)
-        input_policy = get_policy_in_marl(config, representation, config.agent_keys)
+        mixer = QMIX_mixer(config.dim_state[0], config.hidden_dim_mixing_net, config.hidden_dim_hyper_net,
+                           config.n_agents, device)
+        input_policy = get_policy_in_marl(config, representation, config.agent_keys, mixer)
         policy = REGISTRY_Policy[config.policy](*input_policy)
-        optimizer = [torch.optim.Adam(policy.parameters_actor, config.lr_a, eps=1e-5),
-                     torch.optim.Adam(policy.parameters_critic, config.lr_c, eps=1e-5)]
-        scheduler = [torch.optim.lr_scheduler.LinearLR(optimizer[0], start_factor=1.0, end_factor=0.5,
-                                                       total_iters=get_total_iters(config.agent_name, config)),
-                     torch.optim.lr_scheduler.LinearLR(optimizer[1], start_factor=1.0, end_factor=0.5,
-                                                       total_iters=get_total_iters(config.agent_name, config))]
+        optimizer = torch.optim.Adam(policy.parameters(), config.learning_rate, eps=1e-5)
+        scheduler = torch.optim.lr_scheduler.LinearLR(optimizer, start_factor=1.0, end_factor=0.5,
+                                                      total_iters=get_total_iters(config.agent_name, config))
         self.observation_space = envs.observation_space
         self.action_space = envs.action_space
         self.representation_info_shape = policy.representation.output_shapes
         self.auxiliary_info_shape = {}
 
         writer = SummaryWriter(config.logdir)
-        if config.state_space is not None:
-            config.dim_state, state_shape = config.state_space.shape, config.state_space.shape
-        else:
-            config.dim_state, state_shape = None, None
         memory = MARL_OffPolicyBuffer(state_shape,
                                       config.obs_shape,
                                       config.act_shape,
                                       config.rew_shape,
                                       config.done_shape,
                                       envs.num_envs,
                                       config.buffer_size,
                                       config.batch_size)
-        learner = IDDPG_Learner(config, policy, optimizer, scheduler, writer,
-                                config.device, config.modeldir, config.gamma)
+        learner = QMIX_Learner(config, policy, optimizer, scheduler, writer,
+                               config.device, config.modeldir, config.gamma,
+                               config.sync_frequency)
 
         self.obs_rms = RunningMeanStd(shape=space2shape(self.observation_space[config.agent_keys[0]]),
                                       comm=self.comm, use_mpi=False)
         self.ret_rms = RunningMeanStd(shape=(), comm=self.comm, use_mpi=False)
-        super(IDDPG_Agents, self).__init__(config, envs, policy, memory, learner, writer, device,
-                                           config.logdir, config.modeldir)
+        self.epsilon_decay = linear_decay_or_increase(config.start_greedy, config.end_greedy,
+                                                      config.greedy_update_steps)
+        super(QMIX_Agents, self).__init__(config, envs, policy, memory, learner, writer, device,
+                                          config.logdir, config.modeldir)
 
     def _process_observation(self, observations):
         if self.use_obsnorm:
             if isinstance(self.observation_space, Dict):
                 for key in self.observation_space.spaces.keys():
                     observations[key] = np.clip(
                         (observations[key] - self.obs_rms.mean[key]) / (self.obs_rms.std[key] + EPS),
@@ -66,20 +73,14 @@
 
     def _process_reward(self, rewards):
         if self.use_rewnorm:
             std = np.clip(self.ret_rms.std, 0.1, 100)
             return np.clip(rewards / std, -self.rewnorm_range, self.rewnorm_range)
         return rewards
 
-    def act(self, obs_n, episode, test_mode, noise=False):
-        batch_size = len(obs_n)
-        agents_id = torch.eye(self.n_agents).unsqueeze(0).expand(batch_size, -1, -1).to(self.device)
-        _, actions = self.policy(torch.Tensor(obs_n), agents_id)
-        actions = actions.cpu().detach().numpy()
-        if noise:
-            actions += np.random.normal(0, self.args.sigma, size=actions.shape)
-        return actions
-
     def train(self, i_episode):
+        self.epsilon_decay.update()
+        for i in range(self.nenvs):
+            self.writer.add_scalars("epsilon", {"env-%d" % i: self.epsilon_decay.epsilon}, i_episode)
         if self.memory.can_sample(self.args.batch_size):
             sample = self.memory.sample()
             self.learner.update(sample)
```

### Comparing `xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_torch/agents/multi_agent_rl/iql_agents.py` & `xuanpolicy-0.1.6/xuanpolicy/torch/agents/multi_agent_rl/qtran_agents.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-from xuanpolicy.xuanpolicy_torch.agents import *
-from xuanpolicy.xuanpolicy_torch.agents.agents_marl import linear_decay_or_increase
+from xuanpolicy.torch.agents import *
+from xuanpolicy.torch.agents.agents_marl import linear_decay_or_increase
 
 
-class IQL_Agents(MARLAgents):
+class QTRAN_Agents(MARLAgents):
     def __init__(self,
                  config: Namespace,
                  envs: DummyVecEnv_MAS,
                  device: Optional[Union[int, str, torch.device]] = None):
         self.comm = MPI.COMM_WORLD
 
         self.gamma = config.gamma
@@ -14,51 +14,61 @@
         self.use_rewnorm = config.use_rewnorm
         self.obsnorm_range = config.obsnorm_range
         self.rewnorm_range = config.rewnorm_range
 
         self.start_greedy = config.start_greedy
         self.end_greedy = config.end_greedy
         self.egreedy = config.start_greedy
+        if config.state_space is not None:
+            config.dim_state, state_shape = config.state_space.shape, config.state_space.shape
+        else:
+            config.dim_state, state_shape = None, None
 
         input_representation = get_repre_in(config)
         representation = REGISTRY_Representation[config.representation](*input_representation)
-        input_policy = get_policy_in_marl(config, representation, config.agent_keys)
+        mixer = VDN_mixer()
+        if config.agent == "QTRAN_base":
+            qtran_net = QTRAN_base(config.dim_state[0], config.dim_act, config.qtran_net_hidden_dim,
+                                   config.n_agents, config.q_hidden_size[0]).to(device)
+        elif config.agent == "QTRAN_alt":
+            qtran_net = QTRAN_alt(config.dim_state[0], config.dim_act, config.qtran_net_hidden_dim,
+                                  config.n_agents, config.q_hidden_size[0]).to(device)
+        else:
+            raise ValueError("Mixer {} not recognised.".format(config.agent))
+
+        input_policy = get_policy_in_marl(config, representation, config.agent_keys, mixer, qtran_mixer=qtran_net)
         policy = REGISTRY_Policy[config.policy](*input_policy)
         optimizer = torch.optim.Adam(policy.parameters(), config.learning_rate, eps=1e-5)
         scheduler = torch.optim.lr_scheduler.LinearLR(optimizer, start_factor=1.0, end_factor=0.5,
                                                       total_iters=get_total_iters(config.agent_name, config))
         self.observation_space = envs.observation_space
         self.action_space = envs.action_space
         self.representation_info_shape = policy.representation.output_shapes
         self.auxiliary_info_shape = {}
 
         writer = SummaryWriter(config.logdir)
-        if config.state_space is not None:
-            config.dim_state, state_shape = config.state_space.shape, config.state_space.shape
-        else:
-            config.dim_state, state_shape = None, None
         memory = MARL_OffPolicyBuffer(state_shape,
                                       config.obs_shape,
                                       config.act_shape,
                                       config.rew_shape,
                                       config.done_shape,
                                       envs.num_envs,
                                       config.buffer_size,
                                       config.batch_size)
-        learner = IQL_Learner(config, policy, optimizer, scheduler, writer,
-                              config.device, config.modeldir, config.gamma,
-                              config.sync_frequency)
+        learner = QTRAN_Learner(config, policy, optimizer, scheduler, writer,
+                                config.device, config.modeldir, config.gamma,
+                                config.sync_frequency)
 
         self.obs_rms = RunningMeanStd(shape=space2shape(self.observation_space[config.agent_keys[0]]),
                                       comm=self.comm, use_mpi=False)
         self.ret_rms = RunningMeanStd(shape=(), comm=self.comm, use_mpi=False)
         self.epsilon_decay = linear_decay_or_increase(config.start_greedy, config.end_greedy,
                                                       config.greedy_update_steps)
-        super(IQL_Agents, self).__init__(config, envs, policy, memory, learner, writer, device,
-                                         config.logdir, config.modeldir)
+        super(QTRAN_Agents, self).__init__(config, envs, policy, memory, learner, writer, device,
+                                           config.logdir, config.modeldir)
 
     def _process_observation(self, observations):
         if self.use_obsnorm:
             if isinstance(self.observation_space, Dict):
                 for key in self.observation_space.spaces.keys():
                     observations[key] = np.clip(
                         (observations[key] - self.obs_rms.mean[key]) / (self.obs_rms.std[key] + EPS),
```

### Comparing `xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_torch/agents/multi_agent_rl/isac_agents.py` & `xuanpolicy-0.1.6/xuanpolicy/torch/agents/multi_agent_rl/isac_agents.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from xuanpolicy.xuanpolicy_torch.agents import *
+from xuanpolicy.torch.agents import *
 
 
 class ISAC_Agents(MARLAgents):
     def __init__(self,
                  config: Namespace,
                  envs: DummyVecEnv_MAS,
                  device: Optional[Union[int, str, torch.device]] = None):
@@ -22,14 +22,19 @@
                      torch.optim.Adam(policy.parameters_critic, config.lr_c, eps=1e-5)]
         scheduler = [torch.optim.lr_scheduler.LinearLR(optimizer[0], start_factor=1.0, end_factor=0.5,
                                                        total_iters=get_total_iters(config.agent_name, config)),
                      torch.optim.lr_scheduler.LinearLR(optimizer[1], start_factor=1.0, end_factor=0.5,
                                                        total_iters=get_total_iters(config.agent_name, config))]
         self.observation_space = envs.observation_space
         self.action_space = envs.action_space
+        self.actions_high, self.actions_low = [], []
+        for k in config.agent_keys:
+            self.actions_high.append(self.action_space[k].high)
+            self.actions_low.append(self.action_space[k].low)
+        self.actions_high, self.actions_low = np.array(self.actions_high), np.array(self.actions_low)
         self.representation_info_shape = policy.representation.output_shapes
         self.auxiliary_info_shape = {}
 
         writer = SummaryWriter(config.logdir)
         if config.state_space is not None:
             config.dim_state, state_shape = config.state_space.shape, config.state_space.shape
         else:
@@ -72,13 +77,14 @@
 
     def act(self, obs_n, episode, test_mode, state=None, noise=False):
         batch_size = len(obs_n)
         agents_id = torch.eye(self.n_agents).unsqueeze(0).expand(batch_size, -1, -1).to(self.device)
         _, dists = self.policy(obs_n, agents_id)
         acts = dists.rsample()
         actions = acts.cpu().detach().numpy()
+        actions = np.clip(actions, self.actions_low, self.actions_high)
         return actions
 
     def train(self, i_episode):
         if self.memory.can_sample(self.args.batch_size):
             sample = self.memory.sample()
             self.learner.update(sample)
```

### Comparing `xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_torch/agents/multi_agent_rl/maddpg_agents.py` & `xuanpolicy-0.1.6/xuanpolicy/torch/agents/multi_agent_rl/masac_agents.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-from xuanpolicy.xuanpolicy_torch.agents import *
+from xuanpolicy.torch.agents import *
 
 
-class MADDPG_Agents(MARLAgents):
+class MASAC_Agents(MARLAgents):
     def __init__(self,
                  config: Namespace,
                  envs: DummyVecEnv_MAS,
                  device: Optional[Union[int, str, torch.device]] = None):
         self.comm = MPI.COMM_WORLD
 
         self.gamma = config.gamma
@@ -22,14 +22,19 @@
                      torch.optim.Adam(policy.parameters_critic, config.lr_c, eps=1e-5)]
         scheduler = [torch.optim.lr_scheduler.LinearLR(optimizer[0], start_factor=1.0, end_factor=0.5,
                                                        total_iters=get_total_iters(config.agent_name, config)),
                      torch.optim.lr_scheduler.LinearLR(optimizer[1], start_factor=1.0, end_factor=0.5,
                                                        total_iters=get_total_iters(config.agent_name, config))]
         self.observation_space = envs.observation_space
         self.action_space = envs.action_space
+        self.actions_high, self.actions_low = [], []
+        for k in config.agent_keys:
+            self.actions_high.append(self.action_space[k].high)
+            self.actions_low.append(self.action_space[k].low)
+        self.actions_high, self.actions_low = np.array(self.actions_high), np.array(self.actions_low)
         self.representation_info_shape = policy.representation.output_shapes
         self.auxiliary_info_shape = {}
 
         writer = SummaryWriter(config.logdir)
         if config.state_space is not None:
             config.dim_state, state_shape = config.state_space.shape, config.state_space.shape
         else:
@@ -38,22 +43,22 @@
                                       config.obs_shape,
                                       config.act_shape,
                                       config.rew_shape,
                                       config.done_shape,
                                       envs.num_envs,
                                       config.buffer_size,
                                       config.batch_size)
-        learner = MADDPG_Learner(config, policy, optimizer, scheduler, writer,
-                                 config.device, config.modeldir, config.gamma)
+        learner = MASAC_Learner(config, policy, optimizer, scheduler, writer,
+                                config.device, config.modeldir, config.gamma)
 
         self.obs_rms = RunningMeanStd(shape=space2shape(self.observation_space[config.agent_keys[0]]),
                                       comm=self.comm, use_mpi=False)
         self.ret_rms = RunningMeanStd(shape=(), comm=self.comm, use_mpi=False)
-        super(MADDPG_Agents, self).__init__(config, envs, policy, memory, learner, writer, device,
-                                            config.logdir, config.modeldir)
+        super(MASAC_Agents, self).__init__(config, envs, policy, memory, learner, writer, device,
+                                           config.logdir, config.modeldir)
 
     def _process_observation(self, observations):
         if self.use_obsnorm:
             if isinstance(self.observation_space, Dict):
                 for key in self.observation_space.spaces.keys():
                     observations[key] = np.clip(
                         (observations[key] - self.obs_rms.mean[key]) / (self.obs_rms.std[key] + EPS),
@@ -66,20 +71,20 @@
 
     def _process_reward(self, rewards):
         if self.use_rewnorm:
             std = np.clip(self.ret_rms.std, 0.1, 100)
             return np.clip(rewards / std, -self.rewnorm_range, self.rewnorm_range)
         return rewards
 
-    def act(self, obs_n, episode, test_mode, noise=False):
+    def act(self, obs_n, episode, test_mode, state=None, noise=False):
         batch_size = len(obs_n)
         agents_id = torch.eye(self.n_agents).unsqueeze(0).expand(batch_size, -1, -1).to(self.device)
-        _, actions = self.policy(torch.Tensor(obs_n), agents_id)
-        actions = actions.cpu().detach().numpy()
-        if noise:
-            actions += np.random.normal(0, self.args.sigma, size=actions.shape)
+        _, dists = self.policy(obs_n, agents_id)
+        acts = dists.rsample()
+        actions = acts.cpu().detach().numpy()
+        actions = np.clip(actions, self.actions_low, self.actions_high)
         return actions
 
     def train(self, i_episode):
         if self.memory.can_sample(self.args.batch_size):
             sample = self.memory.sample()
             self.learner.update(sample)
```

### Comparing `xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_torch/agents/multi_agent_rl/madqn_agents.py` & `xuanpolicy-0.1.6/xuanpolicy/torch/agents/multi_agent_rl/madqn_agents.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from xuanpolicy.xuanpolicy_torch.agents import *
+from xuanpolicy.torch.agents import *
 
 
 class MADQN_Agents(MARLAgents):
     def __init__(self,
                  config: Namespace,
                  envs: DummyVecEnv_MAS,
                  device: Optional[Union[int, str, torch.device]] = None):
```

### Comparing `xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_torch/agents/multi_agent_rl/mappoclip_agents.py` & `xuanpolicy-0.1.6/xuanpolicy/torch/agents/multi_agent_rl/vdac_agents.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,32 +1,40 @@
-from xuanpolicy.xuanpolicy_torch.agents import *
+from xuanpolicy.torch.agents import *
 
 
-class MAPPO_Clip_Agents(MARLAgents):
+class VDAC_Agents(MARLAgents):
     def __init__(self,
                  config: Namespace,
                  envs: DummyVecEnv_MAS,
                  device: Optional[Union[int, str, torch.device]] = None):
         self.comm = MPI.COMM_WORLD
+        self.device = torch.device("cuda" if (torch.cuda.is_available() and config.device in ["gpu", "cuda:0"]) else "cpu")
 
         self.gamma = config.gamma
         self.use_obsnorm = config.use_obsnorm
         self.use_rewnorm = config.use_rewnorm
         self.obsnorm_range = config.obsnorm_range
         self.rewnorm_range = config.rewnorm_range
 
         if config.state_space is not None:
             config.dim_state, state_shape = config.state_space.shape, config.state_space.shape
         else:
             config.dim_state, state_shape = None, None
 
         input_representation = get_repre_in(config)
         representation = REGISTRY_Representation[config.representation](*input_representation)
+        if config.mixer == "VDN":
+            mixer = VDN_mixer()
+        elif config.mixer == "QMIX":
+            mixer = QMIX_mixer(config.dim_state[0], config.hidden_dim_mixing_net, config.hidden_dim_hyper_net,
+                               config.n_agents, self.device)
+        else:
+            mixer = None
 
-        input_policy = get_policy_in_marl(config, representation, config.agent_keys)
+        input_policy = get_policy_in_marl(config, representation, config.agent_keys, mixer)
         policy = REGISTRY_Policy[config.policy](*input_policy)
         optimizer = torch.optim.Adam(policy.parameters(), config.learning_rate, eps=1e-5)
         scheduler = torch.optim.lr_scheduler.LinearLR(optimizer, start_factor=1.0, end_factor=0.5,
                                                       total_iters=get_total_iters(config.agent_name, config))
         self.observation_space = envs.observation_space
         self.action_space = envs.action_space
         self.representation_info_shape = policy.representation.output_shapes
@@ -36,22 +44,22 @@
         if config.state_space is not None:
             config.dim_state, state_shape = config.state_space.shape, config.state_space.shape
         else:
             config.dim_state, state_shape = None, None
         memory = MARL_OnPolicyBuffer(state_shape, config.obs_shape, config.act_shape, config.rew_shape,
                                      config.done_shape, envs.num_envs, config.nsteps, config.nminibatch,
                                      config.use_gae, config.use_advnorm, config.gamma, config.lam)
-        learner = MAPPO_Clip_Learner(config, policy, optimizer, scheduler, writer,
-                                     config.device, config.modeldir, config.gamma)
+        learner = VDAC_Learner(config, policy, optimizer, scheduler, writer,
+                               config.device, config.modeldir, config.gamma)
 
         self.obs_rms = RunningMeanStd(shape=space2shape(self.observation_space[config.agent_keys[0]]),
                                       comm=self.comm, use_mpi=False)
         self.ret_rms = RunningMeanStd(shape=(), comm=self.comm, use_mpi=False)
-        super(MAPPO_Clip_Agents, self).__init__(config, envs, policy, memory, learner, writer, device,
-                                                config.logdir, config.modeldir)
+        super(VDAC_Agents, self).__init__(config, envs, policy, memory, learner, writer, device,
+                                          config.logdir, config.modeldir)
 
     def _process_observation(self, observations):
         if self.use_obsnorm:
             if isinstance(self.observation_space, Dict):
                 for key in self.observation_space.spaces.keys():
                     observations[key] = np.clip(
                         (observations[key] - self.obs_rms.mean[key]) / (self.obs_rms.std[key] + EPS),
@@ -67,20 +75,21 @@
             std = np.clip(self.ret_rms.std, 0.1, 100)
             return np.clip(rewards / std, -self.rewnorm_range, self.rewnorm_range)
         return rewards
 
     def act(self, obs_n, episode, test_mode, state=None, noise=False):
         batch_size = len(obs_n)
         agents_id = torch.eye(self.n_agents).unsqueeze(0).expand(batch_size, -1, -1).to(self.device)
-        _, dists = self.policy(obs_n, agents_id)
+        states, dists, vs = self.policy(obs_n, agents_id)
+        if self.args.mixer == "VDN":
+            vs_tot = self.policy.value_tot(vs).repeat(1, self.n_agents).unsqueeze(-1)
+        else:
+            vs_tot = self.policy.value_tot(vs, state).repeat(1, self.n_agents).unsqueeze(-1)
         acts = dists.stochastic_sample()
-        log_pi_a = dists.log_prob(acts)
-        state_expand = torch.Tensor(state).unsqueeze(-2).expand(-1, self.n_agents, -1).to(self.device)
-        vs = self.policy.values(state_expand, agents_id)
-        return acts.detach().cpu().numpy(), log_pi_a.detach().cpu().numpy(), vs.detach().cpu().numpy()
+        return acts.detach().cpu().numpy(), vs_tot.detach().cpu().numpy()
 
     def value(self, obs, state):
         batch_size = len(state)
         agents_id = torch.eye(self.n_agents).unsqueeze(0).expand(batch_size, -1, -1).to(self.device)
         repre_out = self.policy.representation(obs)
         critic_input = torch.concat([torch.Tensor(repre_out['state']), agents_id], dim=-1)
         values_n = self.policy.critic(critic_input)
```

### Comparing `xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_torch/agents/multi_agent_rl/mappokl_agents.py` & `xuanpolicy-0.1.6/xuanpolicy/torch/agents/multi_agent_rl/iddpg_agents.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,57 +1,64 @@
-from xuanpolicy.xuanpolicy_torch.agents import *
+from xuanpolicy.torch.agents import *
 
 
-class MAPPO_KL_Agents(MARLAgents):
+class IDDPG_Agents(MARLAgents):
     def __init__(self,
                  config: Namespace,
                  envs: DummyVecEnv_MAS,
                  device: Optional[Union[int, str, torch.device]] = None):
         self.comm = MPI.COMM_WORLD
 
         self.gamma = config.gamma
         self.use_obsnorm = config.use_obsnorm
         self.use_rewnorm = config.use_rewnorm
         self.obsnorm_range = config.obsnorm_range
         self.rewnorm_range = config.rewnorm_range
 
-        if config.state_space is not None:
-            config.dim_state, state_shape = config.state_space.shape, config.state_space.shape
-        else:
-            config.dim_state, state_shape = None, None
-
         input_representation = get_repre_in(config)
         representation = REGISTRY_Representation[config.representation](*input_representation)
-
         input_policy = get_policy_in_marl(config, representation, config.agent_keys)
         policy = REGISTRY_Policy[config.policy](*input_policy)
-        optimizer = torch.optim.Adam(policy.parameters(), config.learning_rate, eps=1e-5)
-        scheduler = torch.optim.lr_scheduler.LinearLR(optimizer, start_factor=1.0, end_factor=0.5,
-                                                      total_iters=get_total_iters(config.agent_name, config))
+        optimizer = [torch.optim.Adam(policy.parameters_actor, config.lr_a, eps=1e-5),
+                     torch.optim.Adam(policy.parameters_critic, config.lr_c, eps=1e-5)]
+        scheduler = [torch.optim.lr_scheduler.LinearLR(optimizer[0], start_factor=1.0, end_factor=0.5,
+                                                       total_iters=get_total_iters(config.agent_name, config)),
+                     torch.optim.lr_scheduler.LinearLR(optimizer[1], start_factor=1.0, end_factor=0.5,
+                                                       total_iters=get_total_iters(config.agent_name, config))]
         self.observation_space = envs.observation_space
         self.action_space = envs.action_space
+        self.actions_high, self.actions_low = [], []
+        for k in config.agent_keys:
+            self.actions_high.append(self.action_space[k].high)
+            self.actions_low.append(self.action_space[k].low)
+        self.actions_high, self.actions_low = np.array(self.actions_high), np.array(self.actions_low)
         self.representation_info_shape = policy.representation.output_shapes
         self.auxiliary_info_shape = {}
 
         writer = SummaryWriter(config.logdir)
         if config.state_space is not None:
             config.dim_state, state_shape = config.state_space.shape, config.state_space.shape
         else:
             config.dim_state, state_shape = None, None
-        memory = MARL_OnPolicyBuffer(state_shape, config.obs_shape, config.act_shape, config.rew_shape,
-                                     config.done_shape, envs.num_envs, config.nsteps, config.nminibatch,
-                                     config.use_gae, config.use_advnorm, config.gamma, config.lam)
-        learner = MAPPO_KL_Learner(config, policy, optimizer, scheduler, writer,
-                                   config.device, config.modeldir, config.gamma)
+        memory = MARL_OffPolicyBuffer(state_shape,
+                                      config.obs_shape,
+                                      config.act_shape,
+                                      config.rew_shape,
+                                      config.done_shape,
+                                      envs.num_envs,
+                                      config.buffer_size,
+                                      config.batch_size)
+        learner = IDDPG_Learner(config, policy, optimizer, scheduler, writer,
+                                config.device, config.modeldir, config.gamma)
 
         self.obs_rms = RunningMeanStd(shape=space2shape(self.observation_space[config.agent_keys[0]]),
                                       comm=self.comm, use_mpi=False)
         self.ret_rms = RunningMeanStd(shape=(), comm=self.comm, use_mpi=False)
-        super(MAPPO_KL_Agents, self).__init__(config, envs, policy, memory, learner, writer, device,
-                                              config.logdir, config.modeldir)
+        super(IDDPG_Agents, self).__init__(config, envs, policy, memory, learner, writer, device,
+                                           config.logdir, config.modeldir)
 
     def _process_observation(self, observations):
         if self.use_obsnorm:
             if isinstance(self.observation_space, Dict):
                 for key in self.observation_space.spaces.keys():
                     observations[key] = np.clip(
                         (observations[key] - self.obs_rms.mean[key]) / (self.obs_rms.std[key] + EPS),
@@ -64,31 +71,21 @@
 
     def _process_reward(self, rewards):
         if self.use_rewnorm:
             std = np.clip(self.ret_rms.std, 0.1, 100)
             return np.clip(rewards / std, -self.rewnorm_range, self.rewnorm_range)
         return rewards
 
-    def act(self, obs_n, episode, test_mode, state=None, noise=False):
+    def act(self, obs_n, episode, test_mode, noise=False):
         batch_size = len(obs_n)
         agents_id = torch.eye(self.n_agents).unsqueeze(0).expand(batch_size, -1, -1).to(self.device)
-        _, dists = self.policy(obs_n, agents_id)
-        acts = dists.stochastic_sample()
-        state_expand = torch.Tensor(state).unsqueeze(-2).expand(-1, self.n_agents, -1).to(self.device)
-        vs = self.policy.values(state_expand, agents_id)
-        return acts.detach().cpu().numpy(), split_distributions(dists), vs.detach().cpu().numpy()
-
-    def value(self, obs, state):
-        batch_size = len(state)
-        agents_id = torch.eye(self.n_agents).unsqueeze(0).expand(batch_size, -1, -1).to(self.device)
-        repre_out = self.policy.representation(obs)
-        critic_input = torch.concat([torch.Tensor(repre_out['state']), agents_id], dim=-1)
-        values_n = self.policy.critic(critic_input)
-        values = self.policy.value_tot(values_n, global_state=state).view(-1, 1).repeat(1, self.n_agents).unsqueeze(-1)
-        return values.detach().cpu().numpy()
+        _, actions = self.policy(torch.Tensor(obs_n), agents_id)
+        actions = actions.cpu().detach().numpy()
+        if noise:
+            actions += np.random.normal(0, self.args.sigma, size=actions.shape)
+            actions = np.clip(actions, self.actions_low, self.actions_high)
+        return actions
 
     def train(self, i_episode):
-        if self.memory.full:
-            for _ in range(self.args.nminibatch * self.args.nepoch):
-                sample = self.memory.sample()
-                self.learner.update(sample)
-            self.memory.clear()
+        if self.memory.can_sample(self.args.batch_size):
+            sample = self.memory.sample()
+            self.learner.update(sample)
```

### Comparing `xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_torch/agents/multi_agent_rl/masac_agents.py` & `xuanpolicy-0.1.6/xuanpolicy/torch/agents/multi_agent_rl/maddpg_agents.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-from xuanpolicy.xuanpolicy_torch.agents import *
+from xuanpolicy.torch.agents import *
 
 
-class MASAC_Agents(MARLAgents):
+class MADDPG_Agents(MARLAgents):
     def __init__(self,
                  config: Namespace,
                  envs: DummyVecEnv_MAS,
                  device: Optional[Union[int, str, torch.device]] = None):
         self.comm = MPI.COMM_WORLD
 
         self.gamma = config.gamma
@@ -22,14 +22,19 @@
                      torch.optim.Adam(policy.parameters_critic, config.lr_c, eps=1e-5)]
         scheduler = [torch.optim.lr_scheduler.LinearLR(optimizer[0], start_factor=1.0, end_factor=0.5,
                                                        total_iters=get_total_iters(config.agent_name, config)),
                      torch.optim.lr_scheduler.LinearLR(optimizer[1], start_factor=1.0, end_factor=0.5,
                                                        total_iters=get_total_iters(config.agent_name, config))]
         self.observation_space = envs.observation_space
         self.action_space = envs.action_space
+        self.actions_high, self.actions_low = [], []
+        for k in config.agent_keys:
+            self.actions_high.append(self.action_space[k].high)
+            self.actions_low.append(self.action_space[k].low)
+        self.actions_high, self.actions_low = np.array(self.actions_high), np.array(self.actions_low)
         self.representation_info_shape = policy.representation.output_shapes
         self.auxiliary_info_shape = {}
 
         writer = SummaryWriter(config.logdir)
         if config.state_space is not None:
             config.dim_state, state_shape = config.state_space.shape, config.state_space.shape
         else:
@@ -38,22 +43,22 @@
                                       config.obs_shape,
                                       config.act_shape,
                                       config.rew_shape,
                                       config.done_shape,
                                       envs.num_envs,
                                       config.buffer_size,
                                       config.batch_size)
-        learner = MASAC_Learner(config, policy, optimizer, scheduler, writer,
-                                config.device, config.modeldir, config.gamma)
+        learner = MADDPG_Learner(config, policy, optimizer, scheduler, writer,
+                                 config.device, config.modeldir, config.gamma)
 
         self.obs_rms = RunningMeanStd(shape=space2shape(self.observation_space[config.agent_keys[0]]),
                                       comm=self.comm, use_mpi=False)
         self.ret_rms = RunningMeanStd(shape=(), comm=self.comm, use_mpi=False)
-        super(MASAC_Agents, self).__init__(config, envs, policy, memory, learner, writer, device,
-                                           config.logdir, config.modeldir)
+        super(MADDPG_Agents, self).__init__(config, envs, policy, memory, learner, writer, device,
+                                            config.logdir, config.modeldir)
 
     def _process_observation(self, observations):
         if self.use_obsnorm:
             if isinstance(self.observation_space, Dict):
                 for key in self.observation_space.spaces.keys():
                     observations[key] = np.clip(
                         (observations[key] - self.obs_rms.mean[key]) / (self.obs_rms.std[key] + EPS),
@@ -66,19 +71,21 @@
 
     def _process_reward(self, rewards):
         if self.use_rewnorm:
             std = np.clip(self.ret_rms.std, 0.1, 100)
             return np.clip(rewards / std, -self.rewnorm_range, self.rewnorm_range)
         return rewards
 
-    def act(self, obs_n, episode, test_mode, state=None, noise=False):
+    def act(self, obs_n, episode, test_mode, noise=False):
         batch_size = len(obs_n)
         agents_id = torch.eye(self.n_agents).unsqueeze(0).expand(batch_size, -1, -1).to(self.device)
-        _, dists = self.policy(obs_n, agents_id)
-        acts = dists.rsample()
-        actions = acts.cpu().detach().numpy()
+        _, actions = self.policy(torch.Tensor(obs_n), agents_id)
+        actions = actions.cpu().detach().numpy()
+        if noise:
+            actions += np.random.normal(0, self.args.sigma, size=actions.shape)
+            actions = np.clip(actions, self.actions_low, self.actions_high)
         return actions
 
     def train(self, i_episode):
         if self.memory.can_sample(self.args.batch_size):
             sample = self.memory.sample()
             self.learner.update(sample)
```

### Comparing `xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_torch/agents/multi_agent_rl/matd3_agents.py` & `xuanpolicy-0.1.6/xuanpolicy/torch/agents/multi_agent_rl/mfac_agents.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,62 +1,66 @@
-from xuanpolicy.xuanpolicy_torch.agents import *
+from xuanpolicy.torch.agents import *
 
 
-class MATD3_Agents(MARLAgents):
+class MFAC_Agents(MARLAgents):
     def __init__(self,
                  config: Namespace,
                  envs: DummyVecEnv_MAS,
                  device: Optional[Union[int, str, torch.device]] = None):
         self.comm = MPI.COMM_WORLD
 
         self.gamma = config.gamma
         self.use_obsnorm = config.use_obsnorm
         self.use_rewnorm = config.use_rewnorm
         self.obsnorm_range = config.obsnorm_range
         self.rewnorm_range = config.rewnorm_range
 
+        if config.state_space is not None:
+            config.dim_state, state_shape = config.state_space.shape, config.state_space.shape
+        else:
+            config.dim_state, state_shape = None, None
+
         input_representation = get_repre_in(config)
         representation = REGISTRY_Representation[config.representation](*input_representation)
         input_policy = get_policy_in_marl(config, representation, config.agent_keys)
         policy = REGISTRY_Policy[config.policy](*input_policy)
         optimizer = [torch.optim.Adam(policy.parameters_actor, config.lr_a, eps=1e-5),
-                     torch.optim.Adam(policy.critic_net_A.parameters(), config.lr_c, eps=1e-5),
-                     torch.optim.Adam(policy.critic_net_B.parameters(), config.lr_c, eps=1e-5)]
+                     torch.optim.Adam(policy.parameters_critic, config.lr_c, eps=1e-5)]
         scheduler = [torch.optim.lr_scheduler.LinearLR(optimizer[0], start_factor=1.0, end_factor=0.5,
                                                        total_iters=get_total_iters(config.agent_name, config)),
                      torch.optim.lr_scheduler.LinearLR(optimizer[1], start_factor=1.0, end_factor=0.5,
-                                                       total_iters=get_total_iters(config.agent_name, config)),
-                     torch.optim.lr_scheduler.LinearLR(optimizer[2], start_factor=1.0, end_factor=0.5,
                                                        total_iters=get_total_iters(config.agent_name, config))]
         self.observation_space = envs.observation_space
         self.action_space = envs.action_space
         self.representation_info_shape = policy.representation.output_shapes
         self.auxiliary_info_shape = {}
 
         writer = SummaryWriter(config.logdir)
         if config.state_space is not None:
             config.dim_state, state_shape = config.state_space.shape, config.state_space.shape
         else:
             config.dim_state, state_shape = None, None
-        memory = MARL_OffPolicyBuffer(state_shape,
-                                      config.obs_shape,
-                                      config.act_shape,
-                                      config.rew_shape,
-                                      config.done_shape,
-                                      envs.num_envs,
-                                      config.buffer_size,
-                                      config.batch_size)
-        learner = MATD3_Learner(config, policy, optimizer, scheduler, writer,
-                                 config.device, config.modeldir, config.gamma)
+        memory = MeanField_OnPolicyBuffer(state_shape,
+                                          config.obs_shape,
+                                          config.act_shape,
+                                          config.act_prob_shape,
+                                          config.rew_shape,
+                                          config.done_shape,
+                                          envs.num_envs,
+                                          config.nsteps,
+                                          config.nminibatch,
+                                          config.use_gae, config.use_advnorm, config.gamma, config.lam)
+        learner = MFAC_Learner(config, policy, optimizer, scheduler, writer,
+                               config.device, config.modeldir, config.gamma)
 
         self.obs_rms = RunningMeanStd(shape=space2shape(self.observation_space[config.agent_keys[0]]),
                                       comm=self.comm, use_mpi=False)
         self.ret_rms = RunningMeanStd(shape=(), comm=self.comm, use_mpi=False)
-        super(MATD3_Agents, self).__init__(config, envs, policy, memory, learner, writer, device,
-                                            config.logdir, config.modeldir)
+        super(MFAC_Agents, self).__init__(config, envs, policy, memory, learner, writer, device,
+                                          config.logdir, config.modeldir)
 
     def _process_observation(self, observations):
         if self.use_obsnorm:
             if isinstance(self.observation_space, Dict):
                 for key in self.observation_space.spaces.keys():
                     observations[key] = np.clip(
                         (observations[key] - self.obs_rms.mean[key]) / (self.obs_rms.std[key] + EPS),
@@ -69,20 +73,38 @@
 
     def _process_reward(self, rewards):
         if self.use_rewnorm:
             std = np.clip(self.ret_rms.std, 0.1, 100)
             return np.clip(rewards / std, -self.rewnorm_range, self.rewnorm_range)
         return rewards
 
-    def act(self, obs_n, episode, test_mode, noise=False):
+    def act(self, obs_n, episode, test_mode, act_mean=None, agent_mask=None, noise=False):
         batch_size = len(obs_n)
         agents_id = torch.eye(self.n_agents).unsqueeze(0).expand(batch_size, -1, -1).to(self.device)
-        _, actions = self.policy(torch.Tensor(obs_n), agents_id)
-        actions = actions.cpu().detach().numpy()
-        if noise:
-            actions += np.random.normal(0, self.args.sigma, size=actions.shape)
-        return actions
+        obs_n = torch.Tensor(obs_n).to(self.device)
+
+        _, dists = self.policy(obs_n, agents_id)
+        acts = dists.stochastic_sample()
+
+        n_alive = torch.Tensor(agent_mask).sum(dim=-1).unsqueeze(-1).repeat(1, self.dim_act).to(self.device)
+        action_n_mask = torch.Tensor(agent_mask).unsqueeze(-1).repeat(1, 1, self.dim_act).to(self.device)
+        act_neighbor_onehot = self.learner.onehot_action(acts, self.dim_act) * action_n_mask
+        act_mean_current = act_neighbor_onehot.float().sum(dim=1) / n_alive
+        act_mean_current = act_mean_current.cpu().detach().numpy()
+
+        return acts.detach().cpu().numpy(), act_mean_current
+
+    def value(self, obs, state):
+        batch_size = len(state)
+        agents_id = torch.eye(self.n_agents).unsqueeze(0).expand(batch_size, -1, -1).to(self.device)
+        repre_out = self.policy.representation(obs)
+        critic_input = torch.concat([torch.Tensor(repre_out['state']), agents_id], dim=-1)
+        values_n = self.policy.critic(critic_input)
+        values = self.policy.value_tot(values_n, global_state=state).view(-1, 1).repeat(1, self.n_agents).unsqueeze(-1)
+        return values.detach().cpu().numpy()
 
     def train(self, i_episode):
-        if self.memory.can_sample(self.args.batch_size):
-            sample = self.memory.sample()
-            self.learner.update(sample)
+        if self.memory.full:
+            for _ in range(self.args.nminibatch * self.args.nepoch):
+                sample = self.memory.sample()
+                self.learner.update(sample)
+            self.memory.clear()
```

### Comparing `xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_torch/agents/multi_agent_rl/mfac_agents.py` & `xuanpolicy-0.1.6/xuanpolicy/torch/agents/multi_agent_rl/mfq_agents.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,66 +1,65 @@
-from xuanpolicy.xuanpolicy_torch.agents import *
+from xuanpolicy.torch.agents import *
+from xuanpolicy.torch.agents.agents_marl import linear_decay_or_increase
 
 
-class MFAC_Agents(MARLAgents):
+class MFQ_Agents(MARLAgents):
     def __init__(self,
                  config: Namespace,
                  envs: DummyVecEnv_MAS,
                  device: Optional[Union[int, str, torch.device]] = None):
         self.comm = MPI.COMM_WORLD
 
         self.gamma = config.gamma
         self.use_obsnorm = config.use_obsnorm
         self.use_rewnorm = config.use_rewnorm
         self.obsnorm_range = config.obsnorm_range
         self.rewnorm_range = config.rewnorm_range
 
-        if config.state_space is not None:
-            config.dim_state, state_shape = config.state_space.shape, config.state_space.shape
-        else:
-            config.dim_state, state_shape = None, None
+        self.start_greedy = config.start_greedy
+        self.end_greedy = config.end_greedy
+        self.egreedy = config.start_greedy
 
         input_representation = get_repre_in(config)
         representation = REGISTRY_Representation[config.representation](*input_representation)
         input_policy = get_policy_in_marl(config, representation, config.agent_keys)
         policy = REGISTRY_Policy[config.policy](*input_policy)
-        optimizer = [torch.optim.Adam(policy.parameters_actor, config.lr_a, eps=1e-5),
-                     torch.optim.Adam(policy.parameters_critic, config.lr_c, eps=1e-5)]
-        scheduler = [torch.optim.lr_scheduler.LinearLR(optimizer[0], start_factor=1.0, end_factor=0.5,
-                                                       total_iters=get_total_iters(config.agent_name, config)),
-                     torch.optim.lr_scheduler.LinearLR(optimizer[1], start_factor=1.0, end_factor=0.5,
-                                                       total_iters=get_total_iters(config.agent_name, config))]
+        optimizer = torch.optim.Adam(policy.parameters(), config.learning_rate, eps=1e-5)
+        scheduler = torch.optim.lr_scheduler.LinearLR(optimizer, start_factor=1.0, end_factor=0.5,
+                                                      total_iters=get_total_iters(config.agent_name, config))
         self.observation_space = envs.observation_space
         self.action_space = envs.action_space
         self.representation_info_shape = policy.representation.output_shapes
         self.auxiliary_info_shape = {}
 
         writer = SummaryWriter(config.logdir)
         if config.state_space is not None:
             config.dim_state, state_shape = config.state_space.shape, config.state_space.shape
         else:
             config.dim_state, state_shape = None, None
-        memory = MeanField_OnPolicyBuffer(state_shape,
-                                          config.obs_shape,
-                                          config.act_shape,
-                                          config.act_prob_shape,
-                                          config.rew_shape,
-                                          config.done_shape,
-                                          envs.num_envs,
-                                          config.nsteps,
-                                          config.nminibatch,
-                                          config.use_gae, config.use_advnorm, config.gamma, config.lam)
-        learner = MFAC_Learner(config, policy, optimizer, scheduler, writer,
-                               config.device, config.modeldir, config.gamma)
+        memory = MeanField_OffPolicyBuffer(state_shape,
+                                           config.obs_shape,
+                                           config.act_shape,
+                                           config.act_prob_shape,
+                                           config.rew_shape,
+                                           config.done_shape,
+                                           envs.num_envs,
+                                           config.buffer_size,
+                                           config.batch_size)
+        learner = MFQ_Learner(config, policy, optimizer, scheduler, writer,
+                              config.device, config.modeldir, config.gamma,
+                              config.sync_frequency)
 
         self.obs_rms = RunningMeanStd(shape=space2shape(self.observation_space[config.agent_keys[0]]),
                                       comm=self.comm, use_mpi=False)
         self.ret_rms = RunningMeanStd(shape=(), comm=self.comm, use_mpi=False)
-        super(MFAC_Agents, self).__init__(config, envs, policy, memory, learner, writer, device,
-                                          config.logdir, config.modeldir)
+        self.epsilon_decay = linear_decay_or_increase(config.start_greedy, config.end_greedy,
+                                                      config.greedy_update_steps)
+        super(MFQ_Agents, self).__init__(config, envs, policy, memory, learner, writer, device,
+                                         config.logdir, config.modeldir)
 
     def _process_observation(self, observations):
         if self.use_obsnorm:
             if isinstance(self.observation_space, Dict):
                 for key in self.observation_space.spaces.keys():
                     observations[key] = np.clip(
                         (observations[key] - self.obs_rms.mean[key]) / (self.obs_rms.std[key] + EPS),
@@ -74,37 +73,39 @@
     def _process_reward(self, rewards):
         if self.use_rewnorm:
             std = np.clip(self.ret_rms.std, 0.1, 100)
             return np.clip(rewards / std, -self.rewnorm_range, self.rewnorm_range)
         return rewards
 
     def act(self, obs_n, episode, test_mode, act_mean=None, agent_mask=None, noise=False):
-        batch_size = len(obs_n)
+        if not test_mode:
+            epsilon = self.epsilon_decay.epsilon
+        else:
+            epsilon = 1.0
+        batch_size = obs_n.shape[0]
         agents_id = torch.eye(self.n_agents).unsqueeze(0).expand(batch_size, -1, -1).to(self.device)
-        obs_n = torch.Tensor(obs_n).to(self.device)
-
-        _, dists = self.policy(obs_n, agents_id)
-        acts = dists.stochastic_sample()
+        obs_in = torch.Tensor(obs_n).to(self.device)
+        act_mean = torch.Tensor(act_mean).unsqueeze(dim=-2).repeat(1, self.n_agents, 1).to(self.device)
 
+        _, greedy_actions, q_output = self.policy(obs_in, act_mean, agents_id)
         n_alive = torch.Tensor(agent_mask).sum(dim=-1).unsqueeze(-1).repeat(1, self.dim_act).to(self.device)
         action_n_mask = torch.Tensor(agent_mask).unsqueeze(-1).repeat(1, 1, self.dim_act).to(self.device)
-        act_neighbor_onehot = self.learner.onehot_action(acts, self.dim_act) * action_n_mask
+        act_neighbor_sample = self.policy.sample_actions(logits=q_output).to(self.device)
+        act_neighbor_onehot = self.learner.onehot_action(act_neighbor_sample, self.dim_act) * action_n_mask
         act_mean_current = act_neighbor_onehot.float().sum(dim=1) / n_alive
         act_mean_current = act_mean_current.cpu().detach().numpy()
-
-        return acts.detach().cpu().numpy(), act_mean_current
-
-    def value(self, obs, state):
-        batch_size = len(state)
-        agents_id = torch.eye(self.n_agents).unsqueeze(0).expand(batch_size, -1, -1).to(self.device)
-        repre_out = self.policy.representation(obs)
-        critic_input = torch.concat([torch.Tensor(repre_out['state']), agents_id], dim=-1)
-        values_n = self.policy.critic(critic_input)
-        values = self.policy.value_tot(values_n, global_state=state).view(-1, 1).repeat(1, self.n_agents).unsqueeze(-1)
-        return values.detach().cpu().numpy()
+        greedy_actions = greedy_actions.cpu().detach().numpy()
+        if noise:
+            random_variable = np.random.rand(batch_size, self.n_agents).reshape(greedy_actions.shape)
+            action_pick = np.int32((random_variable < epsilon))
+            random_actions = np.array([[self.args.action_space[agent].sample() for agent in self.agent_keys]])
+            return action_pick * greedy_actions + (1 - action_pick) * random_actions, act_mean_current
+        else:
+            return greedy_actions, act_mean_current
 
     def train(self, i_episode):
-        if self.memory.full:
-            for _ in range(self.args.nminibatch * self.args.nepoch):
-                sample = self.memory.sample()
-                self.learner.update(sample)
-            self.memory.clear()
+        self.epsilon_decay.update()
+        for i in range(self.nenvs):
+            self.writer.add_scalars("epsilon", {"env-%d" % i: self.epsilon_decay.epsilon}, i_episode)
+        if self.memory.can_sample(self.args.batch_size):
+            sample = self.memory.sample()
+            self.learner.update(sample)
```

### Comparing `xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_torch/agents/multi_agent_rl/qmix_agents.py` & `xuanpolicy-0.1.6/xuanpolicy/tensorflow/agents/multi_agent_rl/masac_agents.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,66 +1,63 @@
-from xuanpolicy.xuanpolicy_torch.agents import *
-from xuanpolicy.xuanpolicy_torch.agents.agents_marl import linear_decay_or_increase
+from xuanpolicy.tensorflow.agents import *
 
 
-class QMIX_Agents(MARLAgents):
+class MASAC_Agents(MARLAgents):
     def __init__(self,
                  config: Namespace,
                  envs: DummyVecEnv_MAS,
-                 device: Optional[Union[int, str, torch.device]] = None):
+                 device: str = "cpu:0"):
         self.comm = MPI.COMM_WORLD
 
         self.gamma = config.gamma
         self.use_obsnorm = config.use_obsnorm
         self.use_rewnorm = config.use_rewnorm
         self.obsnorm_range = config.obsnorm_range
         self.rewnorm_range = config.rewnorm_range
 
-        self.start_greedy = config.start_greedy
-        self.end_greedy = config.end_greedy
-        self.egreedy = config.start_greedy
-        if config.state_space is not None:
-            config.dim_state, state_shape = config.state_space.shape, config.state_space.shape
-        else:
-            config.dim_state, state_shape = None, None
-
         input_representation = get_repre_in(config)
         representation = REGISTRY_Representation[config.representation](*input_representation)
-        mixer = QMIX_mixer(config.dim_state[0], config.hidden_dim_mixing_net, config.hidden_dim_hyper_net,
-                           config.n_agents, device)
-        input_policy = get_policy_in_marl(config, representation, config.agent_keys, mixer)
+        input_policy = get_policy_in_marl(config, representation, config.agent_keys)
         policy = REGISTRY_Policy[config.policy](*input_policy)
-        optimizer = torch.optim.Adam(policy.parameters(), config.learning_rate, eps=1e-5)
-        scheduler = torch.optim.lr_scheduler.LinearLR(optimizer, start_factor=1.0, end_factor=0.5,
-                                                      total_iters=get_total_iters(config.agent_name, config))
+        lr_scheduler = [MyLinearLR(config.lr_a, start_factor=1.0, end_factor=0.5,
+                                   total_iters=get_total_iters(config.agent_name, config)),
+                        MyLinearLR(config.lr_c, start_factor=1.0, end_factor=0.5,
+                                   total_iters=get_total_iters(config.agent_name, config))]
+        optimizer = [tk.optimizers.Adam(lr_scheduler[0]),
+                     tk.optimizers.Adam(lr_scheduler[1])]
         self.observation_space = envs.observation_space
         self.action_space = envs.action_space
+        self.actions_high, self.actions_low = [], []
+        for k in config.agent_keys:
+            self.actions_high.append(self.action_space[k].high)
+            self.actions_low.append(self.action_space[k].low)
+        self.actions_high, self.actions_low = np.array(self.actions_high), np.array(self.actions_low)
         self.representation_info_shape = policy.representation.output_shapes
         self.auxiliary_info_shape = {}
 
         writer = SummaryWriter(config.logdir)
+        if config.state_space is not None:
+            config.dim_state, state_shape = config.state_space.shape, config.state_space.shape
+        else:
+            config.dim_state, state_shape = None, None
         memory = MARL_OffPolicyBuffer(state_shape,
                                       config.obs_shape,
                                       config.act_shape,
                                       config.rew_shape,
                                       config.done_shape,
                                       envs.num_envs,
                                       config.buffer_size,
                                       config.batch_size)
-        learner = QMIX_Learner(config, policy, optimizer, scheduler, writer,
-                               config.device, config.modeldir, config.gamma,
-                               config.sync_frequency)
+        learner = MASAC_Learner(config, policy, optimizer, writer, config.device, config.modeldir, config.gamma)
 
         self.obs_rms = RunningMeanStd(shape=space2shape(self.observation_space[config.agent_keys[0]]),
                                       comm=self.comm, use_mpi=False)
         self.ret_rms = RunningMeanStd(shape=(), comm=self.comm, use_mpi=False)
-        self.epsilon_decay = linear_decay_or_increase(config.start_greedy, config.end_greedy,
-                                                      config.greedy_update_steps)
-        super(QMIX_Agents, self).__init__(config, envs, policy, memory, learner, writer, device,
-                                          config.logdir, config.modeldir)
+        super(MASAC_Agents, self).__init__(config, envs, policy, memory, learner, writer, device,
+                                           config.logdir, config.modeldir)
 
     def _process_observation(self, observations):
         if self.use_obsnorm:
             if isinstance(self.observation_space, Dict):
                 for key in self.observation_space.spaces.keys():
                     observations[key] = np.clip(
                         (observations[key] - self.obs_rms.mean[key]) / (self.obs_rms.std[key] + EPS),
@@ -73,14 +70,22 @@
 
     def _process_reward(self, rewards):
         if self.use_rewnorm:
             std = np.clip(self.ret_rms.std, 0.1, 100)
             return np.clip(rewards / std, -self.rewnorm_range, self.rewnorm_range)
         return rewards
 
+    def act(self, obs_n, episode, test_mode, state=None, noise=False):
+        batch_size = len(obs_n)
+        with tf.device(self.device):
+            agents_id = tf.tile(tf.expand_dims(tf.eye(self.n_agents), axis=0), multiples=(batch_size, 1, 1))
+            inputs_policy = {"obs": tf.convert_to_tensor(obs_n), "ids": agents_id}
+            _, dists = self.policy(inputs_policy)
+            acts = dists.sample()
+        actions = acts.numpy()
+        actions = np.clip(actions, self.actions_low, self.actions_high)
+        return actions
+
     def train(self, i_episode):
-        self.epsilon_decay.update()
-        for i in range(self.nenvs):
-            self.writer.add_scalars("epsilon", {"env-%d" % i: self.epsilon_decay.epsilon}, i_episode)
         if self.memory.can_sample(self.args.batch_size):
             sample = self.memory.sample()
             self.learner.update(sample)
```

### Comparing `xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_torch/agents/multi_agent_rl/qtran_agents.py` & `xuanpolicy-0.1.6/xuanpolicy/tensorflow/agents/multi_agent_rl/isac_agents.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,74 +1,63 @@
-from xuanpolicy.xuanpolicy_torch.agents import *
-from xuanpolicy.xuanpolicy_torch.agents.agents_marl import linear_decay_or_increase
+from xuanpolicy.tensorflow.agents import *
 
 
-class QTRAN_Agents(MARLAgents):
+class ISAC_Agents(MARLAgents):
     def __init__(self,
                  config: Namespace,
                  envs: DummyVecEnv_MAS,
-                 device: Optional[Union[int, str, torch.device]] = None):
+                 device: str = "cpu:0"):
         self.comm = MPI.COMM_WORLD
 
         self.gamma = config.gamma
         self.use_obsnorm = config.use_obsnorm
         self.use_rewnorm = config.use_rewnorm
         self.obsnorm_range = config.obsnorm_range
         self.rewnorm_range = config.rewnorm_range
 
-        self.start_greedy = config.start_greedy
-        self.end_greedy = config.end_greedy
-        self.egreedy = config.start_greedy
-        if config.state_space is not None:
-            config.dim_state, state_shape = config.state_space.shape, config.state_space.shape
-        else:
-            config.dim_state, state_shape = None, None
-
         input_representation = get_repre_in(config)
         representation = REGISTRY_Representation[config.representation](*input_representation)
-        mixer = VDN_mixer()
-        if config.agent == "QTRAN_base":
-            qtran_net = QTRAN_base(config.dim_state[0], config.dim_act, config.qtran_net_hidden_dim,
-                                   config.n_agents, config.q_hidden_size[0]).to(device)
-        elif config.agent == "QTRAN_alt":
-            qtran_net = QTRAN_alt(config.dim_state[0], config.dim_act, config.qtran_net_hidden_dim,
-                                  config.n_agents, config.q_hidden_size[0]).to(device)
-        else:
-            raise ValueError("Mixer {} not recognised.".format(config.agent))
-
-        input_policy = get_policy_in_marl(config, representation, config.agent_keys, mixer, qtran_mixer=qtran_net)
+        input_policy = get_policy_in_marl(config, representation, config.agent_keys)
         policy = REGISTRY_Policy[config.policy](*input_policy)
-        optimizer = torch.optim.Adam(policy.parameters(), config.learning_rate, eps=1e-5)
-        scheduler = torch.optim.lr_scheduler.LinearLR(optimizer, start_factor=1.0, end_factor=0.5,
-                                                      total_iters=get_total_iters(config.agent_name, config))
+        lr_scheduler = [MyLinearLR(config.lr_a, start_factor=1.0, end_factor=0.5,
+                                   total_iters=get_total_iters(config.agent_name, config)),
+                        MyLinearLR(config.lr_c, start_factor=1.0, end_factor=0.5,
+                                   total_iters=get_total_iters(config.agent_name, config))]
+        optimizer = [tk.optimizers.Adam(lr_scheduler[0]),
+                     tk.optimizers.Adam(lr_scheduler[1])]
         self.observation_space = envs.observation_space
         self.action_space = envs.action_space
+        self.actions_high, self.actions_low = [], []
+        for k in config.agent_keys:
+            self.actions_high.append(self.action_space[k].high)
+            self.actions_low.append(self.action_space[k].low)
+        self.actions_high, self.actions_low = np.array(self.actions_high), np.array(self.actions_low)
         self.representation_info_shape = policy.representation.output_shapes
         self.auxiliary_info_shape = {}
 
         writer = SummaryWriter(config.logdir)
+        if config.state_space is not None:
+            config.dim_state, state_shape = config.state_space.shape, config.state_space.shape
+        else:
+            config.dim_state, state_shape = None, None
         memory = MARL_OffPolicyBuffer(state_shape,
                                       config.obs_shape,
                                       config.act_shape,
                                       config.rew_shape,
                                       config.done_shape,
                                       envs.num_envs,
                                       config.buffer_size,
                                       config.batch_size)
-        learner = QTRAN_Learner(config, policy, optimizer, scheduler, writer,
-                                config.device, config.modeldir, config.gamma,
-                                config.sync_frequency)
+        learner = ISAC_Learner(config, policy, optimizer, writer, config.device, config.modeldir, config.gamma)
 
         self.obs_rms = RunningMeanStd(shape=space2shape(self.observation_space[config.agent_keys[0]]),
                                       comm=self.comm, use_mpi=False)
         self.ret_rms = RunningMeanStd(shape=(), comm=self.comm, use_mpi=False)
-        self.epsilon_decay = linear_decay_or_increase(config.start_greedy, config.end_greedy,
-                                                      config.greedy_update_steps)
-        super(QTRAN_Agents, self).__init__(config, envs, policy, memory, learner, writer, device,
-                                           config.logdir, config.modeldir)
+        super(ISAC_Agents, self).__init__(config, envs, policy, memory, learner, writer, device,
+                                          config.logdir, config.modeldir)
 
     def _process_observation(self, observations):
         if self.use_obsnorm:
             if isinstance(self.observation_space, Dict):
                 for key in self.observation_space.spaces.keys():
                     observations[key] = np.clip(
                         (observations[key] - self.obs_rms.mean[key]) / (self.obs_rms.std[key] + EPS),
@@ -81,14 +70,22 @@
 
     def _process_reward(self, rewards):
         if self.use_rewnorm:
             std = np.clip(self.ret_rms.std, 0.1, 100)
             return np.clip(rewards / std, -self.rewnorm_range, self.rewnorm_range)
         return rewards
 
+    def act(self, obs_n, episode, test_mode, state=None, noise=False):
+        batch_size = len(obs_n)
+        with tf.device(self.device):
+            agents_id = tf.tile(tf.expand_dims(tf.eye(self.n_agents), axis=0), multiples=(batch_size, 1, 1))
+            inputs_policy = {"obs": tf.convert_to_tensor(obs_n), "ids": agents_id}
+            _, dists = self.policy(inputs_policy)
+            acts = dists.sample()
+        actions = acts.numpy()
+        actions = np.clip(actions, self.actions_low, self.actions_high)
+        return actions
+
     def train(self, i_episode):
-        self.epsilon_decay.update()
-        for i in range(self.nenvs):
-            self.writer.add_scalars("epsilon", {"env-%d" % i: self.epsilon_decay.epsilon}, i_episode)
         if self.memory.can_sample(self.args.batch_size):
             sample = self.memory.sample()
             self.learner.update(sample)
```

### Comparing `xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_torch/agents/multi_agent_rl/vdn_agents.py` & `xuanpolicy-0.1.6/xuanpolicy/tensorflow/agents/multi_agent_rl/matd3_agents.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,38 +1,40 @@
-from xuanpolicy.xuanpolicy_torch.agents import *
-from xuanpolicy.xuanpolicy_torch.agents.agents_marl import linear_decay_or_increase
+from xuanpolicy.tensorflow.agents import *
 
 
-class VDN_Agents(MARLAgents):
+class MATD3_Agents(MARLAgents):
     def __init__(self,
                  config: Namespace,
                  envs: DummyVecEnv_MAS,
-                 device: Optional[Union[int, str, torch.device]] = None):
+                 device: str = "cpu:0"):
         self.comm = MPI.COMM_WORLD
 
         self.gamma = config.gamma
         self.use_obsnorm = config.use_obsnorm
         self.use_rewnorm = config.use_rewnorm
         self.obsnorm_range = config.obsnorm_range
         self.rewnorm_range = config.rewnorm_range
 
-        self.start_greedy = config.start_greedy
-        self.end_greedy = config.end_greedy
-        self.egreedy = config.start_greedy
-
         input_representation = get_repre_in(config)
         representation = REGISTRY_Representation[config.representation](*input_representation)
-        mixer = VDN_mixer()
-        input_policy = get_policy_in_marl(config, representation, config.agent_keys, mixer)
+        input_policy = get_policy_in_marl(config, representation, config.agent_keys)
         policy = REGISTRY_Policy[config.policy](*input_policy)
-        optimizer = torch.optim.Adam(policy.parameters(), config.learning_rate, eps=1e-5)
-        scheduler = torch.optim.lr_scheduler.LinearLR(optimizer, start_factor=1.0, end_factor=0.5,
-                                                      total_iters=get_total_iters(config.agent_name, config))
+        lr_scheduler = [MyLinearLR(config.lr_a, start_factor=1.0, end_factor=0.5,
+                                   total_iters=get_total_iters(config.agent_name, config)),
+                        MyLinearLR(config.lr_c, start_factor=1.0, end_factor=0.5,
+                                   total_iters=get_total_iters(config.agent_name, config))]
+        optimizer = [tk.optimizers.Adam(lr_scheduler[0]),
+                     tk.optimizers.Adam(lr_scheduler[1])]
         self.observation_space = envs.observation_space
         self.action_space = envs.action_space
+        self.actions_high, self.actions_low = [], []
+        for k in config.agent_keys:
+            self.actions_high.append(self.action_space[k].high)
+            self.actions_low.append(self.action_space[k].low)
+        self.actions_high, self.actions_low = np.array(self.actions_high), np.array(self.actions_low)
         self.representation_info_shape = policy.representation.output_shapes
         self.auxiliary_info_shape = {}
 
         writer = SummaryWriter(config.logdir)
         if config.state_space is not None:
             config.dim_state, state_shape = config.state_space.shape, config.state_space.shape
         else:
@@ -41,25 +43,22 @@
                                       config.obs_shape,
                                       config.act_shape,
                                       config.rew_shape,
                                       config.done_shape,
                                       envs.num_envs,
                                       config.buffer_size,
                                       config.batch_size)
-        learner = VDN_Learner(config, policy, optimizer, scheduler, writer,
-                              config.device, config.modeldir, config.gamma,
-                              config.sync_frequency)
+        learner = MATD3_Learner(config, policy, optimizer, writer,
+                                 config.device, config.modeldir, config.gamma)
 
         self.obs_rms = RunningMeanStd(shape=space2shape(self.observation_space[config.agent_keys[0]]),
                                       comm=self.comm, use_mpi=False)
         self.ret_rms = RunningMeanStd(shape=(), comm=self.comm, use_mpi=False)
-        self.epsilon_decay = linear_decay_or_increase(config.start_greedy, config.end_greedy,
-                                                      config.greedy_update_steps)
-        super(VDN_Agents, self).__init__(config, envs, policy, memory, learner, writer, device,
-                                         config.logdir, config.modeldir)
+        super(MATD3_Agents, self).__init__(config, envs, policy, memory, learner, writer, device,
+                                            config.logdir, config.modeldir)
 
     def _process_observation(self, observations):
         if self.use_obsnorm:
             if isinstance(self.observation_space, Dict):
                 for key in self.observation_space.spaces.keys():
                     observations[key] = np.clip(
                         (observations[key] - self.obs_rms.mean[key]) / (self.obs_rms.std[key] + EPS),
@@ -72,14 +71,23 @@
 
     def _process_reward(self, rewards):
         if self.use_rewnorm:
             std = np.clip(self.ret_rms.std, 0.1, 100)
             return np.clip(rewards / std, -self.rewnorm_range, self.rewnorm_range)
         return rewards
 
+    def act(self, obs_n, episode, test_mode, noise=False):
+        batch_size = len(obs_n)
+        with tf.device(self.device):
+            agents_id = tf.tile(tf.expand_dims(tf.eye(self.n_agents), axis=0), multiples=(batch_size, 1, 1))
+            inputs_policy = {"obs": tf.convert_to_tensor(obs_n), "ids": agents_id}
+            _, actions = self.policy(inputs_policy)
+        actions = actions.numpy()
+        if noise:
+            actions += np.random.normal(0, self.args.sigma, size=actions.shape)
+            actions = np.clip(actions, self.actions_low, self.actions_high)
+        return actions
+
     def train(self, i_episode):
-        self.epsilon_decay.update()
-        for i in range(self.nenvs):
-            self.writer.add_scalars("epsilon", {"env-%d" % i: self.epsilon_decay.epsilon}, i_episode)
         if self.memory.can_sample(self.args.batch_size):
             sample = self.memory.sample()
             self.learner.update(sample)
```

### Comparing `xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_torch/agents/multi_agent_rl/wqmix_agents.py` & `xuanpolicy-0.1.6/xuanpolicy/mindspore/agents/multi_agent_rl/isac_agents.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,68 +1,62 @@
-from xuanpolicy.xuanpolicy_torch.agents import *
-from xuanpolicy.xuanpolicy_torch.agents.agents_marl import linear_decay_or_increase
+from xuanpolicy.mindspore.agents import *
 
 
-class WQMIX_Agents(MARLAgents):
+class ISAC_Agents(MARLAgents):
     def __init__(self,
                  config: Namespace,
-                 envs: DummyVecEnv_MAS,
-                 device: Optional[Union[int, str, torch.device]] = None):
+                 envs: DummyVecEnv_MAS):
         self.comm = MPI.COMM_WORLD
 
-        self.alpha = config.alpha
         self.gamma = config.gamma
         self.use_obsnorm = config.use_obsnorm
         self.use_rewnorm = config.use_rewnorm
         self.obsnorm_range = config.obsnorm_range
         self.rewnorm_range = config.rewnorm_range
 
-        self.start_greedy = config.start_greedy
-        self.end_greedy = config.end_greedy
-        self.egreedy = config.start_greedy
-        if config.state_space is not None:
-            config.dim_state, state_shape = config.state_space.shape, config.state_space.shape
-        else:
-            config.dim_state, state_shape = None, None
-
         input_representation = get_repre_in(config)
         representation = REGISTRY_Representation[config.representation](*input_representation)
-        mixer = QMIX_mixer(config.dim_state[0], config.hidden_dim_mixing_net, config.hidden_dim_hyper_net,
-                           config.n_agents, device)
-        ff_mixer = QMIX_FF_mixer(config.dim_state[0], config.hidden_dim_mixing_net, config.n_agents, device)
-        input_policy = get_policy_in_marl(config, representation, config.agent_keys, mixer, ff_mixer)
+        input_policy = get_policy_in_marl(config, representation, config.agent_keys)
         policy = REGISTRY_Policy[config.policy](*input_policy)
-        optimizer = torch.optim.Adam(policy.parameters(), config.learning_rate, eps=1e-5)
-        scheduler = torch.optim.lr_scheduler.LinearLR(optimizer, start_factor=1.0, end_factor=0.5,
-                                                      total_iters=get_total_iters(config.agent_name, config))
+        scheduler = [lr_decay_model(learning_rate=config.lr_a, decay_rate=0.5,
+                                    decay_steps=get_total_iters(config.agent_name, config)),
+                     lr_decay_model(learning_rate=config.lr_c, decay_rate=0.5,
+                                    decay_steps=get_total_iters(config.agent_name, config))]
+        optimizer = [Adam(policy.parameters_actor, scheduler[0], eps=1e-5),
+                     Adam(policy.parameters_critic, scheduler[1], eps=1e-5)]
         self.observation_space = envs.observation_space
         self.action_space = envs.action_space
+        self.actions_high, self.actions_low = [], []
+        for k in config.agent_keys:
+            self.actions_high.append(self.action_space[k].high)
+            self.actions_low.append(self.action_space[k].low)
+        self.actions_high, self.actions_low = np.array(self.actions_high), np.array(self.actions_low)
         self.representation_info_shape = policy.representation.output_shapes
         self.auxiliary_info_shape = {}
 
         writer = SummaryWriter(config.logdir)
+        if config.state_space is not None:
+            config.dim_state, state_shape = config.state_space.shape, config.state_space.shape
+        else:
+            config.dim_state, state_shape = None, None
         memory = MARL_OffPolicyBuffer(state_shape,
                                       config.obs_shape,
                                       config.act_shape,
                                       config.rew_shape,
                                       config.done_shape,
                                       envs.num_envs,
                                       config.buffer_size,
                                       config.batch_size)
-        learner = WQMIX_Learner(config, policy, optimizer, scheduler, writer,
-                                config.device, config.modeldir, config.gamma,
-                                config.sync_frequency)
+        learner = ISAC_Learner(config, policy, optimizer, scheduler, writer, config.modeldir, config.gamma)
 
         self.obs_rms = RunningMeanStd(shape=space2shape(self.observation_space[config.agent_keys[0]]),
                                       comm=self.comm, use_mpi=False)
         self.ret_rms = RunningMeanStd(shape=(), comm=self.comm, use_mpi=False)
-        self.epsilon_decay = linear_decay_or_increase(config.start_greedy, config.end_greedy,
-                                                      config.greedy_update_steps)
-        super(WQMIX_Agents, self).__init__(config, envs, policy, memory, learner, writer, device,
-                                           config.logdir, config.modeldir)
+        super(ISAC_Agents, self).__init__(config, envs, policy, memory, learner, writer,
+                                          config.logdir, config.modeldir)
 
     def _process_observation(self, observations):
         if self.use_obsnorm:
             if isinstance(self.observation_space, Dict):
                 for key in self.observation_space.spaces.keys():
                     observations[key] = np.clip(
                         (observations[key] - self.obs_rms.mean[key]) / (self.obs_rms.std[key] + EPS),
@@ -75,14 +69,21 @@
 
     def _process_reward(self, rewards):
         if self.use_rewnorm:
             std = np.clip(self.ret_rms.std, 0.1, 100)
             return np.clip(rewards / std, -self.rewnorm_range, self.rewnorm_range)
         return rewards
 
+    def act(self, obs_n, episode, test_mode, state=None, noise=False):
+        batch_size = len(obs_n)
+        agents_id = ops.broadcast_to(self.expand_dims(self.eye(self.n_agents, self.n_agents, ms.float32), 0),
+                                     (batch_size, -1, -1))
+        _, act_mu, act_std = self.policy(Tensor(obs_n), agents_id)
+        acts = self.policy.actor_net.sample(act_mu, act_std)
+        actions = acts.asnumpy()
+        actions = np.clip(actions, self.actions_low, self.actions_high)
+        return actions
+
     def train(self, i_episode):
-        self.epsilon_decay.update()
-        for i in range(self.nenvs):
-            self.writer.add_scalars("epsilon", {"env-%d" % i: self.epsilon_decay.epsilon}, i_episode)
         if self.memory.can_sample(self.args.batch_size):
             sample = self.memory.sample()
             self.learner.update(sample)
```

### Comparing `xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_torch/agents/policy_gradient/a2c_agent.py` & `xuanpolicy-0.1.6/xuanpolicy/torch/agents/policy_gradient/a2c_agent.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from xuanpolicy.xuanpolicy_torch.agents import *
+from xuanpolicy.torch.agents import *
 
 
 class A2C_Agent(Agent):
     def __init__(self,
                  config: Namespace,
                  envs: VecEnv,
                  policy: nn.Module,
```

### Comparing `xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_torch/agents/policy_gradient/ddpg_agent.py` & `xuanpolicy-0.1.6/xuanpolicy/torch/agents/policy_gradient/ddpg_agent.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from xuanpolicy.xuanpolicy_torch.agents import *
+from xuanpolicy.torch.agents import *
 
 
 class DDPG_Agent(Agent):
     def __init__(self,
                  config: Namespace,
                  envs: VecEnv,
                  policy: nn.Module,
```

### Comparing `xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_torch/agents/policy_gradient/mpdqn_agent.py` & `xuanpolicy-0.1.6/xuanpolicy/torch/agents/policy_gradient/mpdqn_agent.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from xuanpolicy.xuanpolicy_torch.agents import *
+from xuanpolicy.torch.agents import *
 import gym
 from gym import spaces
 
 
 class MPDQN_Agent(Agent):
     def __init__(self,
                  config: Namespace,
```

### Comparing `xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_torch/agents/policy_gradient/pdqn_agent.py` & `xuanpolicy-0.1.6/xuanpolicy/torch/agents/policy_gradient/pdqn_agent.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import numpy as np
 
-from xuanpolicy.xuanpolicy_torch.agents import *
+from xuanpolicy.torch.agents import *
 import gym
 from gym import spaces
 
 
 class PDQN_Agent(Agent):
     def __init__(self,
                  config: Namespace,
```

### Comparing `xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_torch/agents/policy_gradient/pg_agent.py` & `xuanpolicy-0.1.6/xuanpolicy/torch/agents/policy_gradient/pg_agent.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from xuanpolicy.xuanpolicy_torch.agents import *
+from xuanpolicy.torch.agents import *
 
 
 class PG_Agent(Agent):
     def __init__(self,
                  config: Namespace,
                  envs: VecEnv,
                  policy: nn.Module,
```

### Comparing `xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_torch/agents/policy_gradient/ppg_agent.py` & `xuanpolicy-0.1.6/xuanpolicy/mindspore/agents/policy_gradient/ppg_agent.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,27 +1,28 @@
-from xuanpolicy.xuanpolicy_torch.agents import *
+from xuanpolicy.mindspore.agents import *
+from xuanpolicy.mindspore.utils.distributions import CategoricalDistribution
 
 
 class PPG_Agent(Agent):
     def __init__(self,
                  config: Namespace,
                  envs: VecEnv,
-                 policy: nn.Module,
-                 optimizer: torch.optim.Optimizer,
-                 scheduler: Optional[torch.optim.lr_scheduler._LRScheduler] = None,
-                 device: Optional[Union[int, str, torch.device]] = None):
-        self.render = config.render
+                 policy: nn.Cell,
+                 optimizer: nn.Optimizer,
+                 scheduler):
+        self.config = config
         self.comm = MPI.COMM_WORLD
         self.nenvs = envs.num_envs
         self.nsteps = config.nsteps
         self.nminibatch = config.nminibatch
         self.policy_nepoch = config.policy_nepoch
         self.value_nepoch = config.value_nepoch
         self.aux_nepoch = config.aux_nepoch
-        
+        self.render = config.render
+
         self.gamma = config.gamma
         self.lam = config.lam
         self.use_obsnorm = config.use_obsnorm
         self.use_rewnorm = config.use_rewnorm
         self.obsnorm_range = config.obsnorm_range
         self.rewnorm_range = config.rewnorm_range
 
@@ -37,27 +38,25 @@
                                      self.auxiliary_info_shape,
                                      self.nenvs,
                                      self.nsteps,
                                      self.nminibatch,
                                      self.gamma,
                                      self.lam)
         learner = PPG_Learner(policy,
-                              optimizer,
-                              scheduler,
-                              writer,
-                              config.device,
-                              config.modeldir,
-                              config.ent_coef,
-                              config.clip_range,
-                              config.kl_beta)
+                             optimizer,
+                             scheduler,
+                             writer,
+                             config.modeldir,
+                             config.ent_coef,
+                             config.clip_range,
+                             config.kl_beta)
 
         self.obs_rms = RunningMeanStd(shape=space2shape(self.observation_space), comm=self.comm, use_mpi=False)
         self.ret_rms = RunningMeanStd(shape=(), comm=self.comm, use_mpi=False)
-        super(PPG_Agent, self).__init__(envs, policy, memory, learner, writer, device, config.logdir,
-                                            config.modeldir)
+        super(PPG_Agent, self).__init__(envs, policy, memory, learner, writer, config.logdir, config.modeldir)
 
     def _process_observation(self, observations):
         if self.use_obsnorm:
             if isinstance(self.observation_space, Dict):
                 for key in self.observation_space.spaces.keys():
                     observations[key] = np.clip(
                         (observations[key] - self.obs_rms.mean[key]) / (self.obs_rms.std[key] + EPS),
@@ -71,23 +70,28 @@
     def _process_reward(self, rewards):
         if self.use_rewnorm:
             std = np.clip(self.ret_rms.std, 0.1, 100)
             return np.clip(rewards / std, -self.rewnorm_range, self.rewnorm_range)
         return rewards
 
     def _action(self, obs):
-        states, dists, vs, _ = self.policy(obs)
-        acts = dists.stochastic_sample()
-        for key in states.keys():
-            states[key] = states[key].detach().cpu().numpy()
-        vs = vs.detach().cpu().numpy()
-        acts = acts.detach().cpu().numpy()
-        return states, acts, vs, split_distributions(dists)
+        states, act_probs, vs, _ = self.policy(ms.Tensor(obs))
+        # acts = self.policy.actor.sample(act_probs).asnumpy()
+        dists = CategoricalDistribution(self.action_space.n)
+        dists.set_param(act_probs)
+        acts = dists.stochastic_sample().asnumpy()
+        vs = vs.asnumpy()
+        if context._get_mode() == 0:
+            return {"state": states[0].asnumpy()}, acts, vs, split_distributions(dists)
+        else:
+            for key in states.keys():
+                states[key] = states[key].asnumpy()
+            return states, acts, vs, split_distributions(dists)
 
-    def train(self, train_steps=10000):
+    def train(self, train_steps=10000, load_model=None):
         episodes = np.zeros((self.nenvs,), np.int32)
         scores = np.zeros((self.nenvs,), np.float32)
         returns = np.zeros((self.nenvs,), np.float32)
 
         obs = self.envs.reset()
         for step in tqdm(range(train_steps)):
             self.obs_rms.update(obs)
@@ -95,32 +99,37 @@
             states, acts, rets, dists = self._action(obs)
             next_obs, rewards, dones, infos = self.envs.step(acts)
             if self.render: self.envs.render()
             self.memory.store(obs, acts, self._process_reward(rewards), rets, dones, states, {"old_dist": dists})
             if self.memory.full:
                 _, _, vals, _ = self._action(self._process_observation(next_obs))
                 for i in range(self.nenvs):
-                    self.memory.finish_path(vals[i], i)
+                    self.memory.finish_path(rewards[i], i)
+                
                 # policy update
+                # update_type: 0-policy_update, 1-critic_update, 2-auxiliary_update
                 for _ in range(self.nminibatch * self.policy_nepoch):
                     obs_batch, act_batch, ret_batch, adv_batch, _, aux_batch = self.memory.sample()
-                    self.learner.update_policy(obs_batch, act_batch, ret_batch, adv_batch, aux_batch['old_dist'])
+                    self.learner.update(obs_batch, act_batch, ret_batch, adv_batch, aux_batch['old_dist'], 0)
                 # critic update
                 for _ in range(self.nminibatch * self.value_nepoch):
                     obs_batch, act_batch, ret_batch, adv_batch, _, aux_batch = self.memory.sample()
-                    self.learner.update_critic(obs_batch, act_batch, ret_batch, adv_batch, aux_batch['old_dist'])
+                    self.learner.update(obs_batch, act_batch, ret_batch, adv_batch, aux_batch['old_dist'], 1)
                     
                 # update old_prob
                 buffer_obs = self.memory.observations
                 buffer_act = self.memory.actions
-                _,new_dist,_,_ = self.policy(buffer_obs)
+                _,new_dists,_,_ = self.policy(ms.Tensor(buffer_obs))
+                new_dist = CategoricalDistribution(self.action_space.n)
+                new_dist.set_param(new_dists)
                 self.memory.auxiliary_infos['old_dist'] = split_distributions(new_dist)
                 for _ in range(self.nminibatch * self.aux_nepoch):
                     obs_batch, act_batch, ret_batch, adv_batch, _, aux_batch = self.memory.sample()
-                    self.learner.update_auxiliary(obs_batch, act_batch, ret_batch, adv_batch, aux_batch['old_dist'])
+                    self.learner.update(obs_batch, act_batch, ret_batch, adv_batch, aux_batch['old_dist'], 2)
+                
                 self.memory.clear()
             scores += rewards
             returns = self.gamma * returns + rewards
             obs = next_obs
             for i in range(self.nenvs):
                 if dones[i] == True:
                     self.ret_rms.update(returns[i:i + 1])
@@ -150,10 +159,10 @@
             self.envs.render()
             scores += rewards
             returns = self.gamma * returns + rewards
             obs = next_obs
             for i in range(self.nenvs):
                 if dones[i] == True:
                     scores[i], returns[i] = 0, 0
-
+    
     def evaluate(self):
         pass
```

### Comparing `xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_torch/agents/policy_gradient/ppoclip_agent.py` & `xuanpolicy-0.1.6/xuanpolicy/torch/agents/policy_gradient/ppoclip_agent.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from xuanpolicy.xuanpolicy_torch.agents import *
+from xuanpolicy.torch.agents import *
 
 
 class PPOCLIP_Agent(Agent):
     def __init__(self,
                  config: Namespace,
                  envs: VecEnv,
                  policy: nn.Module,
```

### Comparing `xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_torch/agents/policy_gradient/ppokl_agent.py` & `xuanpolicy-0.1.6/xuanpolicy/torch/agents/policy_gradient/ppokl_agent.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from xuanpolicy.xuanpolicy_torch.agents import *
+from xuanpolicy.torch.agents import *
 
 
 class PPOKL_Agent(Agent):
     def __init__(self,
                  config: Namespace,
                  envs: VecEnv,
                  policy: nn.Module,
```

### Comparing `xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_torch/agents/policy_gradient/sac_agent.py` & `xuanpolicy-0.1.6/xuanpolicy/torch/agents/policy_gradient/sac_agent.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from xuanpolicy.xuanpolicy_torch.agents import *
+from xuanpolicy.torch.agents import *
 
 
 class SAC_Agent(Agent):
     def __init__(self,
                  config: Namespace,
                  envs: VecEnv,
                  policy: nn.Module,
```

### Comparing `xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_torch/agents/policy_gradient/sacdis_agent.py` & `xuanpolicy-0.1.6/xuanpolicy/torch/agents/policy_gradient/sacdis_agent.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from xuanpolicy.xuanpolicy_torch.agents import *
+from xuanpolicy.torch.agents import *
 
 
 class SACDIS_Agent(Agent):
     def __init__(self,
                  config: Namespace,
                  envs: VecEnv,
                  policy: nn.Module,
```

### Comparing `xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_torch/agents/policy_gradient/spdqn_agent.py` & `xuanpolicy-0.1.6/xuanpolicy/torch/agents/policy_gradient/spdqn_agent.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from xuanpolicy.xuanpolicy_torch.agents import *
+from xuanpolicy.torch.agents import *
 import gym
 from gym import spaces
 
 
 class SPDQN_Agent(Agent):
     def __init__(self,
                  config: Namespace,
```

### Comparing `xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_torch/agents/policy_gradient/td3_agent.py` & `xuanpolicy-0.1.6/xuanpolicy/torch/agents/policy_gradient/td3_agent.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from xuanpolicy.xuanpolicy_torch.agents import *
+from xuanpolicy.torch.agents import *
 
 
 class TD3_Agent(Agent):
     def __init__(self,
                  config: Namespace,
                  envs: VecEnv,
                  policy: nn.Module,
```

### Comparing `xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_torch/agents/qlearning_family/c51_agent.py` & `xuanpolicy-0.1.6/xuanpolicy/torch/agents/qlearning_family/c51_agent.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from xuanpolicy.xuanpolicy_torch.agents import *
+from xuanpolicy.torch.agents import *
 
 
 class C51_Agent(Agent):
     def __init__(self,
                  config: Namespace,
                  envs: VecEnv,
                  policy: nn.Module,
```

### Comparing `xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_torch/agents/qlearning_family/cdqn_agent.py` & `xuanpolicy-0.1.6/xuanpolicy/torch/agents/qlearning_family/cdqn_agent.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from xuanpolicy.xuanpolicy_torch.agents import *
+from xuanpolicy.torch.agents import *
 
 
 class CDQN_Agent(Agent):
     def __init__(self,
                  config: Namespace,
                  envs: VecEnv,
                  policy: nn.Module,
```

### Comparing `xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_torch/agents/qlearning_family/cldqn_agent.py` & `xuanpolicy-0.1.6/xuanpolicy/torch/agents/qlearning_family/cldqn_agent.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from xuanpolicy.xuanpolicy_torch.agents import *
+from xuanpolicy.torch.agents import *
 
 
 class CLDQN_Agent(Agent):
     def __init__(self,
                  config: Namespace,
                  envs: VecEnv,
                  policy: nn.Module,
```

### Comparing `xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_torch/agents/qlearning_family/ddqn_agent.py` & `xuanpolicy-0.1.6/xuanpolicy/torch/agents/qlearning_family/ddqn_agent.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from xuanpolicy.xuanpolicy_torch.agents import *
+from xuanpolicy.torch.agents import *
 
 
 class DDQN_Agent(Agent):
     def __init__(self,
                  config: Namespace,
                  envs: VecEnv,
                  policy: nn.Module,
```

### Comparing `xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_torch/agents/qlearning_family/dqn_agent.py` & `xuanpolicy-0.1.6/xuanpolicy/torch/agents/qlearning_family/dqn_agent.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from xuanpolicy.xuanpolicy_torch.agents import *
+from xuanpolicy.torch.agents import *
 
 
 class DQN_Agent(Agent):
     def __init__(self,
                  config: Namespace,
                  envs: VecEnv,
                  policy: nn.Module,
```

### Comparing `xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_torch/agents/qlearning_family/dueldqn_agent.py` & `xuanpolicy-0.1.6/xuanpolicy/torch/agents/qlearning_family/dueldqn_agent.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from xuanpolicy.xuanpolicy_torch.agents import *
+from xuanpolicy.torch.agents import *
 
 
 class DuelDQN_Agent(Agent):
     def __init__(self,
                  config: Namespace,
                  envs: VecEnv,
                  policy: nn.Module,
```

### Comparing `xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_torch/agents/qlearning_family/ldqn_agent.py` & `xuanpolicy-0.1.6/xuanpolicy/torch/agents/qlearning_family/ldqn_agent.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from xuanpolicy.xuanpolicy_torch.agents import *
+from xuanpolicy.torch.agents import *
 
 
 class LDQN_Agent(Agent):
     def __init__(self,
                  config: Namespace,
                  envs: VecEnv,
                  policy: nn.Module,
```

### Comparing `xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_torch/agents/qlearning_family/noisydqn_agent.py` & `xuanpolicy-0.1.6/xuanpolicy/torch/agents/qlearning_family/noisydqn_agent.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from xuanpolicy.xuanpolicy_torch.agents import *
+from xuanpolicy.torch.agents import *
 
 
 class NoisyDQN_Agent(Agent):
     def __init__(self,
                  config: Namespace,
                  envs: VecEnv,
                  policy: nn.Module,
```

### Comparing `xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_torch/agents/qlearning_family/perdqn_agent.py` & `xuanpolicy-0.1.6/xuanpolicy/torch/agents/qlearning_family/perdqn_agent.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from xuanpolicy.xuanpolicy_torch.agents import *
+from xuanpolicy.torch.agents import *
 
 
 class PerDQN_Agent(Agent):
     def __init__(self,
                  config: Namespace,
                  envs: VecEnv,
                  policy: nn.Module,
```

### Comparing `xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_torch/agents/qlearning_family/qrdqn_agent.py` & `xuanpolicy-0.1.6/xuanpolicy/torch/agents/qlearning_family/qrdqn_agent.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from xuanpolicy.xuanpolicy_torch.agents import *
+from xuanpolicy.torch.agents import *
 
 
 class QRDQN_Agent(Agent):
     def __init__(self,
                  config: Namespace,
                  envs: VecEnv,
                  policy: nn.Module,
```

### Comparing `xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_torch/learners/__init__.py` & `xuanpolicy-0.1.6/xuanpolicy/torch/learners/__init__.py`

 * *Files identical despite different names*

### Comparing `xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_torch/learners/learner.py` & `xuanpolicy-0.1.6/xuanpolicy/torch/learners/learner.py`

 * *Files identical despite different names*

### Comparing `xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_torch/learners/multi_agent_rl/coma_learner.py` & `xuanpolicy-0.1.6/xuanpolicy/torch/learners/multi_agent_rl/coma_learner.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
 COMA: Counterfactual Multi-Agent Policy Gradients
 Paper link: https://ojs.aaai.org/index.php/AAAI/article/view/11794
 Implementation: Pytorch
 """
-from xuanpolicy.xuanpolicy_torch.learners import *
+from xuanpolicy.torch.learners import *
 
 
 class COMA_Learner(LearnerMAS):
     def __init__(self,
                  config: Namespace,
                  policy: nn.Module,
                  optimizer: Sequence[torch.optim.Optimizer],
```

### Comparing `xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_torch/learners/multi_agent_rl/dcg_learner.py` & `xuanpolicy-0.1.6/xuanpolicy/torch/learners/multi_agent_rl/dcg_learner.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
 DCG: Deep coordination graphs
 Paper link: http://proceedings.mlr.press/v119/boehmer20a/boehmer20a.pdf
 Implementation: Pytorch
 """
-from xuanpolicy.xuanpolicy_torch.learners import *
+from xuanpolicy.torch.learners import *
 import torch_scatter
 
 
 class DCG_Learner(LearnerMAS):
     def __init__(self,
                  config: Namespace,
                  policy: nn.Module,
```

### Comparing `xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_torch/learners/multi_agent_rl/iddpg_learner.py` & `xuanpolicy-0.1.6/xuanpolicy/torch/learners/multi_agent_rl/iddpg_learner.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
 Independent Deep Deterministic Policy Gradient (IDDPG)
 Implementation: Pytorch
 """
-from xuanpolicy.xuanpolicy_torch.learners import *
+from xuanpolicy.torch.learners import *
 
 
 class IDDPG_Learner(LearnerMAS):
     def __init__(self,
                  config: Namespace,
                  policy: nn.Module,
                  optimizer: Sequence[torch.optim.Optimizer],
```

### Comparing `xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_torch/learners/multi_agent_rl/iql_learner.py` & `xuanpolicy-0.1.6/xuanpolicy/torch/learners/multi_agent_rl/iql_learner.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
 Independent Q-learning (IQL)
 Implementation: Pytorch
 """
-from xuanpolicy.xuanpolicy_torch.learners import *
+from xuanpolicy.torch.learners import *
 
 
 class IQL_Learner(LearnerMAS):
     def __init__(self,
                  config: Namespace,
                  policy: nn.Module,
                  optimizer: torch.optim.Optimizer,
```

### Comparing `xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_torch/learners/multi_agent_rl/isac_learner.py` & `xuanpolicy-0.1.6/xuanpolicy/torch/learners/multi_agent_rl/isac_learner.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
 Independent Soft Actor-critic (ISAC)
 Implementation: Pytorch
 """
-from xuanpolicy.xuanpolicy_torch.learners import *
+from xuanpolicy.torch.learners import *
 
 
 class ISAC_Learner(LearnerMAS):
     def __init__(self,
                  config: Namespace,
                  policy: nn.Module,
                  optimizer: Sequence[torch.optim.Optimizer],
```

### Comparing `xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_torch/learners/multi_agent_rl/maddpg_learner.py` & `xuanpolicy-0.1.6/xuanpolicy/tensorflow/learners/multi_agent_rl/maac_learner.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 """
 Multi-Agent Deep Deterministic Policy Gradient
 Paper link:
 https://proceedings.neurips.cc/paper/2017/file/68a9750337a418a86fe06c1991a1d64c-Paper.pdf
-Implementation: Pytorch
+Implementation: TensorFlow 2.X
 Trick: Parameter sharing for all agents, with agents' one-hot IDs as actor-critic's inputs.
 """
-from xuanpolicy.xuanpolicy_torch.learners import *
+from xuanpolicy.torch.learners import *
 
 
-class MADDPG_Learner(LearnerMAS):
+class MAAC_Learner(LearnerMAS):
     def __init__(self,
                  config: Namespace,
                  policy: nn.Module,
                  optimizer: Sequence[torch.optim.Optimizer],
                  scheduler: Sequence[torch.optim.lr_scheduler._LRScheduler] = None,
                  summary_writer: Optional[SummaryWriter] = None,
                  device: Optional[Union[int, str, torch.device]] = None,
@@ -20,15 +20,15 @@
                  gamma: float = 0.99,
                  sync_frequency: int = 100
                  ):
         self.gamma = gamma
         self.tau = config.tau
         self.sync_frequency = sync_frequency
         self.mse_loss = nn.MSELoss()
-        super(MADDPG_Learner, self).__init__(config, policy, optimizer, scheduler, summary_writer, device, modeldir)
+        super(MAAC_Learner, self).__init__(config, policy, optimizer, scheduler, summary_writer, device, modeldir)
         self.optimizer = {
             'actor': optimizer[0],
             'critic': optimizer[1]
         }
         self.scheduler = {
             'actor': scheduler[0],
             'critic': scheduler[1]
```

### Comparing `xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_torch/learners/multi_agent_rl/madqn_learner.py` & `xuanpolicy-0.1.6/xuanpolicy/torch/learners/multi_agent_rl/madqn_learner.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """
 Multi-Agent Deep Q Network
 Code link: github.com/opendilab/DI-engine/blob/main/ding/policy/madqn.py
 Implementation: Pytorch
 Creator: Kun Jiang (kjiang@seu.edu.cn)
 Trick: Parameter sharing for all agents, with agents' one-hot IDs as actor-critic's inputs.
 """
-from xuanpolicy.xuanpolicy_torch.learners import *
+from xuanpolicy.torch.learners import *
 
 
 class MADQN_Learner(LearnerMAS):
     def __init__(self,
                  config: Namespace,
                  policy: nn.Module,
                  optimizer: torch.optim.Optimizer,
```

### Comparing `xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_torch/learners/multi_agent_rl/mappoclip_learner.py` & `xuanpolicy-0.1.6/xuanpolicy/torch/learners/multi_agent_rl/mappoclip_learner.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """
 Multi-Agent Proximal Policy Optimization (MAPPO)
 Paper link:
 https://arxiv.org/pdf/2103.01955.pdf
 Implementation: Pytorch
 """
-from xuanpolicy.xuanpolicy_torch.learners import *
+from xuanpolicy.torch.learners import *
 
 
 class MAPPO_Clip_Learner(LearnerMAS):
     def __init__(self,
                  config: Namespace,
                  policy: nn.Module,
                  optimizer: torch.optim.Optimizer,
```

### Comparing `xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_torch/learners/multi_agent_rl/mappokl_learner.py` & `xuanpolicy-0.1.6/xuanpolicy/torch/learners/multi_agent_rl/mappokl_learner.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,16 +2,16 @@
 Multi-Agent Proximal Policy Optimization (MAPPO)
 Paper link:
 https://arxiv.org/pdf/2103.01955.pdf
 Implementation: Pytorch
 """
 import torch
 
-from xuanpolicy.xuanpolicy_torch.learners import *
-from xuanpolicy.xuanpolicy_torch.utils.operations import merge_distributions
+from xuanpolicy.torch.learners import *
+from xuanpolicy.torch.utils.operations import merge_distributions
 
 
 class MAPPO_KL_Learner(LearnerMAS):
     def __init__(self,
                  config: Namespace,
                  policy: nn.Module,
                  optimizer: torch.optim.Optimizer,
```

### Comparing `xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_torch/learners/multi_agent_rl/masac_learner.py` & `xuanpolicy-0.1.6/xuanpolicy/torch/learners/multi_agent_rl/masac_learner.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
 Multi-agent Soft Actor-critic (MASAC)
 Implementation: Pytorch
 """
-from xuanpolicy.xuanpolicy_torch.learners import *
+from xuanpolicy.torch.learners import *
 
 
 class MASAC_Learner(LearnerMAS):
     def __init__(self,
                  config: Namespace,
                  policy: nn.Module,
                  optimizer: Sequence[torch.optim.Optimizer],
```

### Comparing `xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_torch/learners/multi_agent_rl/matd3_learner.py` & `xuanpolicy-0.1.6/xuanpolicy/torch/learners/multi_agent_rl/matd3_learner.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """
 Multi-Agent TD3
 """
-from xuanpolicy.xuanpolicy_torch.learners import *
+from xuanpolicy.torch.learners import *
 
 
 class MATD3_Learner(LearnerMAS):
     def __init__(self,
                  config: Namespace,
                  policy: nn.Module,
                  optimizer: Sequence[torch.optim.Optimizer],
```

### Comparing `xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_torch/learners/multi_agent_rl/mfac_learner.py` & `xuanpolicy-0.1.6/xuanpolicy/torch/learners/multi_agent_rl/mfac_learner.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 MFAC: Mean Field Actor-Critic
 Paper link:
 http://proceedings.mlr.press/v80/yang18d/yang18d.pdf
 Implementation: Pytorch
 """
 import torch
 
-from xuanpolicy.xuanpolicy_torch.learners import *
+from xuanpolicy.torch.learners import *
 
 
 class MFAC_Learner(LearnerMAS):
     def __init__(self,
                  config: Namespace,
                  policy: nn.Module,
                  optimizer: Sequence[torch.optim.Optimizer],
```

### Comparing `xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_torch/learners/multi_agent_rl/mfq_learner.py` & `xuanpolicy-0.1.6/xuanpolicy/torch/learners/multi_agent_rl/mfq_learner.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """
 MFQ: Mean Field Q-Learning
 Paper link:
 http://proceedings.mlr.press/v80/yang18d/yang18d.pdf
 Implementation: Pytorch
 """
-from xuanpolicy.xuanpolicy_torch.learners import *
+from xuanpolicy.torch.learners import *
 
 
 class MFQ_Learner(LearnerMAS):
     def __init__(self,
                  config: Namespace,
                  policy: nn.Module,
                  optimizer: torch.optim.Optimizer,
```

### Comparing `xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_torch/learners/multi_agent_rl/qmix_learner.py` & `xuanpolicy-0.1.6/xuanpolicy/torch/learners/multi_agent_rl/qmix_learner.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """
 Qmix: Monotonic value function factorisation for deep multi-agent reinforcement learning
 Paper link:
 http://proceedings.mlr.press/v80/rashid18a/rashid18a.pdf
 Implementation: Pytorch
 """
-from xuanpolicy.xuanpolicy_torch.learners import *
+from xuanpolicy.torch.learners import *
 
 
 class QMIX_Learner(LearnerMAS):
     def __init__(self,
                  config: Namespace,
                  policy: nn.Module,
                  optimizer: torch.optim.Optimizer,
```

### Comparing `xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_torch/learners/multi_agent_rl/qtran_learner.py` & `xuanpolicy-0.1.6/xuanpolicy/torch/learners/multi_agent_rl/qtran_learner.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """
 QTRAN: Learning to Factorize with Transformation for Cooperative Multi-Agent Reinforcement Learning
 Paper link:
 http://proceedings.mlr.press/v97/son19a/son19a.pdf
 Implementation: Pytorch
 """
-from xuanpolicy.xuanpolicy_torch.learners import *
+from xuanpolicy.torch.learners import *
 
 
 class QTRAN_Learner(LearnerMAS):
     def __init__(self,
                  config: Namespace,
                  policy: nn.Module,
                  optimizer: torch.optim.Optimizer,
```

### Comparing `xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_torch/learners/multi_agent_rl/vdac_learner.py` & `xuanpolicy-0.1.6/xuanpolicy/torch/learners/multi_agent_rl/vdac_learner.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
 Value Decomposition Actor-Critic (VDAC)
 Paper link: https://ojs.aaai.org/index.php/AAAI/article/view/17353
 Implementation: Pytorch
 """
-from xuanpolicy.xuanpolicy_torch.learners import *
+from xuanpolicy.torch.learners import *
 
 
 class VDAC_Learner(LearnerMAS):
     def __init__(self,
                  config: Namespace,
                  policy: nn.Module,
                  optimizer: torch.optim.Optimizer,
```

### Comparing `xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_torch/learners/multi_agent_rl/vdn_learner.py` & `xuanpolicy-0.1.6/xuanpolicy/torch/learners/multi_agent_rl/vdn_learner.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """
 Value Decomposition Networks (VDN)
 Paper link:
 https://arxiv.org/pdf/1706.05296.pdf
 Implementation: Pytorch
 """
-from xuanpolicy.xuanpolicy_torch.learners import *
+from xuanpolicy.torch.learners import *
 
 
 class VDN_Learner(LearnerMAS):
     def __init__(self,
                  config: Namespace,
                  policy: nn.Module,
                  optimizer: torch.optim.Optimizer,
```

### Comparing `xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_torch/learners/multi_agent_rl/wqmix_learner.py` & `xuanpolicy-0.1.6/xuanpolicy/torch/learners/multi_agent_rl/wqmix_learner.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """
 Weighted QMIX
 Paper link:
 https://proceedings.neurips.cc/paper/2020/file/73a427badebe0e32caa2e1fc7530b7f3-Paper.pdf
 Implementation: Pytorch
 """
-from xuanpolicy.xuanpolicy_torch.learners import *
+from xuanpolicy.torch.learners import *
 
 
 class WQMIX_Learner(LearnerMAS):
     def __init__(self,
                  config: Namespace,
                  policy: nn.Module,
                  optimizer: torch.optim.Optimizer,
```

### Comparing `xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_torch/learners/policy_gradient/a2c_learner.py` & `xuanpolicy-0.1.6/xuanpolicy/torch/learners/policy_gradient/a2c_learner.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from xuanpolicy.xuanpolicy_torch.learners import *
+from xuanpolicy.torch.learners import *
 
 
 class A2C_Learner(Learner):
     def __init__(self,
                  policy: nn.Module,
                  optimizer: torch.optim.Optimizer,
                  scheduler: Optional[torch.optim.lr_scheduler._LRScheduler] = None,
```

### Comparing `xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_torch/learners/policy_gradient/ddpg_learner.py` & `xuanpolicy-0.1.6/xuanpolicy/torch/learners/policy_gradient/ddpg_learner.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from xuanpolicy.xuanpolicy_torch.learners import *
+from xuanpolicy.torch.learners import *
 
 
 class DDPG_Learner(Learner):
     def __init__(self,
                  policy: nn.Module,
                  optimizers: Sequence[torch.optim.Optimizer],
                  schedulers: Sequence[torch.optim.lr_scheduler._LRScheduler],
```

### Comparing `xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_torch/learners/policy_gradient/mpdqn_learner.py` & `xuanpolicy-0.1.6/xuanpolicy/torch/learners/policy_gradient/mpdqn_learner.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from xuanpolicy.xuanpolicy_torch.learners import *
+from xuanpolicy.torch.learners import *
 
 
 class MPDQN_Learner(Learner):
     def __init__(self,
                  policy: nn.Module,
                  optimizers: Sequence[torch.optim.Optimizer],
                  schedulers: Sequence[torch.optim.lr_scheduler._LRScheduler],
```

### Comparing `xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_torch/learners/policy_gradient/pdqn_learner.py` & `xuanpolicy-0.1.6/xuanpolicy/torch/learners/policy_gradient/pdqn_learner.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from xuanpolicy.xuanpolicy_torch.learners import *
+from xuanpolicy.torch.learners import *
 
 class PDQN_Learner(Learner):
     def __init__(self,
                  policy: nn.Module,
                  optimizers: Sequence[torch.optim.Optimizer],
                  schedulers: Sequence[torch.optim.lr_scheduler._LRScheduler],
                  summary_writer: Optional[SummaryWriter] = None,
```

### Comparing `xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_torch/learners/policy_gradient/pg_learner.py` & `xuanpolicy-0.1.6/xuanpolicy/torch/learners/policy_gradient/pg_learner.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from xuanpolicy.xuanpolicy_torch.learners import *
+from xuanpolicy.torch.learners import *
 
 
 class PG_Learner(Learner):
     def __init__(self,
                  policy: nn.Module,
                  optimizer: torch.optim.Optimizer,
                  scheduler: Optional[torch.optim.lr_scheduler._LRScheduler] = None,
```

### Comparing `xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_torch/learners/policy_gradient/ppg_learner.py` & `xuanpolicy-0.1.6/xuanpolicy/torch/learners/policy_gradient/ppg_learner.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-from xuanpolicy.xuanpolicy_torch.learners import *
-from xuanpolicy.xuanpolicy_torch.utils.operations import merge_distributions
+from xuanpolicy.torch.learners import *
+from xuanpolicy.torch.utils.operations import merge_distributions
 
 
 class PPG_Learner(Learner):
     def __init__(self,
                  policy: nn.Module,
                  optimizer: torch.optim.Optimizer,
                  scheduler: Optional[torch.optim.lr_scheduler._LRScheduler] = None,
```

### Comparing `xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_torch/learners/policy_gradient/ppoclip_learner.py` & `xuanpolicy-0.1.6/xuanpolicy/torch/learners/policy_gradient/ppoclip_learner.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from xuanpolicy.xuanpolicy_torch.learners import *
+from xuanpolicy.torch.learners import *
 
 
 class PPOCLIP_Learner(Learner):
     def __init__(self,
                  policy: nn.Module,
                  optimizer: torch.optim.Optimizer,
                  scheduler: Optional[torch.optim.lr_scheduler._LRScheduler] = None,
```

### Comparing `xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_torch/learners/policy_gradient/ppokl_learner.py` & `xuanpolicy-0.1.6/xuanpolicy/torch/learners/policy_gradient/ppokl_learner.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-from xuanpolicy.xuanpolicy_torch.learners import *
-from xuanpolicy.xuanpolicy_torch.utils.operations import merge_distributions
+from xuanpolicy.torch.learners import *
+from xuanpolicy.torch.utils.operations import merge_distributions
 
 
 class PPOKL_Learner(Learner):
     def __init__(self,
                  policy: nn.Module,
                  optimizer: torch.optim.Optimizer,
                  scheduler: Optional[torch.optim.lr_scheduler._LRScheduler] = None,
```

### Comparing `xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_torch/learners/policy_gradient/sac_learner.py` & `xuanpolicy-0.1.6/xuanpolicy/torch/learners/policy_gradient/sac_learner.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from xuanpolicy.xuanpolicy_torch.learners import *
+from xuanpolicy.torch.learners import *
 
 
 class SAC_Learner(Learner):
     def __init__(self,
                  policy: nn.Module,
                  optimizers: Sequence[torch.optim.Optimizer],
                  schedulers: Sequence[torch.optim.lr_scheduler._LRScheduler],
```

### Comparing `xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_torch/learners/policy_gradient/sacdis_learner.py` & `xuanpolicy-0.1.6/xuanpolicy/torch/learners/policy_gradient/sacdis_learner.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from xuanpolicy.xuanpolicy_torch.learners import *
+from xuanpolicy.torch.learners import *
 
 
 class SACDIS_Learner(Learner):
     def __init__(self,
                  policy: nn.Module,
                  optimizers: Sequence[torch.optim.Optimizer],
                  schedulers: Sequence[torch.optim.lr_scheduler._LRScheduler],
```

### Comparing `xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_torch/learners/policy_gradient/spdqn_learner.py` & `xuanpolicy-0.1.6/xuanpolicy/torch/learners/policy_gradient/spdqn_learner.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from xuanpolicy.xuanpolicy_torch.learners import *
+from xuanpolicy.torch.learners import *
 
 
 class SPDQN_Learner(Learner):
     def __init__(self,
                  policy: nn.Module,
                  optimizers: Sequence[torch.optim.Optimizer],
                  schedulers: Sequence[torch.optim.lr_scheduler._LRScheduler],
```

### Comparing `xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_torch/learners/policy_gradient/td3_learner.py` & `xuanpolicy-0.1.6/xuanpolicy/torch/learners/policy_gradient/td3_learner.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # TD3 add three tricks to DDPG:
 # 1. noisy action in target actor
 # 2. double critic network
 # 3. delayed actor update
-from xuanpolicy.xuanpolicy_torch.learners import *
+from xuanpolicy.torch.learners import *
 
 
 class TD3_Learner(Learner):
     def __init__(self,
                  policy: nn.Module,
                  optimizers: Sequence[torch.optim.Optimizer],
                  schedulers: Sequence[torch.optim.lr_scheduler._LRScheduler],
```

### Comparing `xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_torch/learners/qlearning_family/c51_learner.py` & `xuanpolicy-0.1.6/xuanpolicy/torch/learners/qlearning_family/c51_learner.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from xuanpolicy.xuanpolicy_torch.learners import *
+from xuanpolicy.torch.learners import *
 
 
 class C51_Learner(Learner):
     def __init__(self,
                  policy: nn.Module,
                  optimizer: torch.optim.Optimizer,
                  scheduler: Optional[torch.optim.lr_scheduler._LRScheduler] = None,
```

### Comparing `xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_torch/learners/qlearning_family/cdqn_learner.py` & `xuanpolicy-0.1.6/xuanpolicy/torch/learners/qlearning_family/cdqn_learner.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from xuanpolicy.xuanpolicy_torch.learners import *
+from xuanpolicy.torch.learners import *
 
 
 class CDQN_Learner(Learner):
     def __init__(self,
                  policy: nn.Module,
                  optimizer: torch.optim.Optimizer,
                  scheduler: Optional[torch.optim.lr_scheduler._LRScheduler] = None,
```

### Comparing `xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_torch/learners/qlearning_family/cldqn_learner.py` & `xuanpolicy-0.1.6/xuanpolicy/torch/learners/qlearning_family/cldqn_learner.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from xuanpolicy.xuanpolicy_torch.learners import *
+from xuanpolicy.torch.learners import *
 
 
 class CLDQN_Learner(Learner):
     def __init__(self,
                  policy: nn.Module,
                  optimizer: torch.optim.Optimizer,
                  scheduler: Optional[torch.optim.lr_scheduler._LRScheduler] = None,
```

### Comparing `xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_torch/learners/qlearning_family/ddqn_learner.py` & `xuanpolicy-0.1.6/xuanpolicy/torch/learners/qlearning_family/ddqn_learner.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from xuanpolicy.xuanpolicy_torch.learners import *
+from xuanpolicy.torch.learners import *
 
 
 class DDQN_Learner(Learner):
     def __init__(self,
                  policy: nn.Module,
                  optimizer: torch.optim.Optimizer,
                  scheduler: Optional[torch.optim.lr_scheduler._LRScheduler] = None,
```

### Comparing `xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_torch/learners/qlearning_family/dqn_learner.py` & `xuanpolicy-0.1.6/xuanpolicy/torch/learners/qlearning_family/dqn_learner.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from xuanpolicy.xuanpolicy_torch.learners import *
+from xuanpolicy.torch.learners import *
 
 
 class DQN_Learner(Learner):
     def __init__(self,
                  policy: nn.Module,
                  optimizer: torch.optim.Optimizer,
                  scheduler: Optional[torch.optim.lr_scheduler._LRScheduler] = None,
```

### Comparing `xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_torch/learners/qlearning_family/dueldqn_learner.py` & `xuanpolicy-0.1.6/xuanpolicy/torch/learners/qlearning_family/dueldqn_learner.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from xuanpolicy.xuanpolicy_torch.learners import *
+from xuanpolicy.torch.learners import *
 
 
 class DuelDQN_Learner(Learner):
     def __init__(self,
                  policy: nn.Module,
                  optimizer: torch.optim.Optimizer,
                  scheduler: Optional[torch.optim.lr_scheduler._LRScheduler] = None,
```

### Comparing `xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_torch/learners/qlearning_family/ldqn_learner.py` & `xuanpolicy-0.1.6/xuanpolicy/torch/learners/qlearning_family/ldqn_learner.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from xuanpolicy.xuanpolicy_torch.learners import *
+from xuanpolicy.torch.learners import *
 
 
 class LDQN_Learner(Learner):
     def __init__(self,
                  policy: nn.Module,
                  optimizer: torch.optim.Optimizer,
                  scheduler: Optional[torch.optim.lr_scheduler._LRScheduler] = None,
```

### Comparing `xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_torch/learners/qlearning_family/perdqn_learner.py` & `xuanpolicy-0.1.6/xuanpolicy/torch/learners/qlearning_family/perdqn_learner.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from xuanpolicy.xuanpolicy_torch.learners import *
+from xuanpolicy.torch.learners import *
 
 
 class PerDQN_Learner(Learner):
     def __init__(self,
                  policy: nn.Module,
                  optimizer: torch.optim.Optimizer,
                  scheduler: Optional[torch.optim.lr_scheduler._LRScheduler] = None,
```

### Comparing `xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_torch/learners/qlearning_family/qrdqn_learner.py` & `xuanpolicy-0.1.6/xuanpolicy/torch/learners/qlearning_family/qrdqn_learner.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from xuanpolicy.xuanpolicy_torch.learners import *
+from xuanpolicy.torch.learners import *
 
 
 class QRDQN_Learner(Learner):
     def __init__(self,
                  policy: nn.Module,
                  optimizer: torch.optim.Optimizer,
                  scheduler: Optional[torch.optim.lr_scheduler._LRScheduler] = None,
```

### Comparing `xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_torch/policies/__init__.py` & `xuanpolicy-0.1.6/xuanpolicy/torch/policies/__init__.py`

 * *Files identical despite different names*

### Comparing `xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_torch/policies/categorical.py` & `xuanpolicy-0.1.6/xuanpolicy/torch/policies/categorical.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import torch.distributions
 
-from xuanpolicy.xuanpolicy_torch.policies import *
-from xuanpolicy.xuanpolicy_torch.utils import *
-from xuanpolicy.xuanpolicy_torch.representations import Basic_Identical
+from xuanpolicy.torch.policies import *
+from xuanpolicy.torch.utils import *
+from xuanpolicy.torch.representations import Basic_Identical
 
 
 class ActorNet(nn.Module):
     def __init__(self,
                  state_dim: int,
                  action_dim: int,
                  hidden_sizes: Sequence[int],
```

### Comparing `xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_torch/policies/categorical_marl.py` & `xuanpolicy-0.1.6/xuanpolicy/torch/policies/categorical_marl.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-from xuanpolicy.xuanpolicy_torch.policies import *
-from xuanpolicy.xuanpolicy_torch.utils import *
-from xuanpolicy.xuanpolicy_torch.representations import Basic_Identical
+from xuanpolicy.torch.policies import *
+from xuanpolicy.torch.utils import *
+from xuanpolicy.torch.representations import Basic_Identical
 from .deterministic_marl import BasicQhead
 
 
 class ActorNet(nn.Module):
     def __init__(self,
                  state_dim: int,
                  action_dim: int,
```

### Comparing `xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_torch/policies/coordination_graph.py` & `xuanpolicy-0.1.6/xuanpolicy/torch/policies/coordination_graph.py`

 * *Files identical despite different names*

### Comparing `xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_torch/policies/deterministic.py` & `xuanpolicy-0.1.6/xuanpolicy/torch/policies/deterministic.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-from xuanpolicy.xuanpolicy_torch.policies import *
-from xuanpolicy.xuanpolicy_torch.utils import *
-from xuanpolicy.xuanpolicy_torch.representations import Basic_Identical
-from xuanpolicy.xuanpolicy_torch.representations import C_DQN, L_DQN, CL_DQN
+from xuanpolicy.torch.policies import *
+from xuanpolicy.torch.utils import *
+from xuanpolicy.torch.representations import Basic_Identical
+from xuanpolicy.torch.representations import C_DQN, L_DQN, CL_DQN
 
 
 class BasicQhead(nn.Module):
     def __init__(self,
                  state_dim: int,
                  action_dim: int,
                  hidden_sizes: Sequence[int],
```

### Comparing `xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_torch/policies/deterministic_marl.py` & `xuanpolicy-0.1.6/xuanpolicy/torch/policies/deterministic_marl.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-from xuanpolicy.xuanpolicy_torch.policies import *
-from xuanpolicy.xuanpolicy_torch.utils import *
-from xuanpolicy.xuanpolicy_torch.representations import Basic_Identical
+from xuanpolicy.torch.policies import *
+from xuanpolicy.torch.utils import *
+from xuanpolicy.torch.representations import Basic_Identical
 from gymnasium.spaces.box import Box as Box_pettingzoo
 from gymnasium import spaces as spaces_pettingzoo
 
 
 class BasicQhead(nn.Module):
     def __init__(self,
                  state_dim: int,
@@ -278,31 +278,32 @@
                 tp.data.copy_(ep)
 
 
 class ActorNet(nn.Module):
     def __init__(self,
                  state_dim: int,
                  n_agents: int,
-                 action_dim: int,
+                 action_space: spaces_pettingzoo,
                  hidden_sizes: Sequence[int],
                  normalize: Optional[ModuleType] = None,
                  initialize: Optional[Callable[..., torch.Tensor]] = None,
                  activation: Optional[ModuleType] = None,
                  device: Optional[Union[str, int, torch.device]] = None):
         super(ActorNet, self).__init__()
         layers = []
         input_shape = (state_dim + n_agents,)
+        action_dim = action_space.shape[0]
         for h in hidden_sizes:
             mlp, input_shape = mlp_block(input_shape[0], h, normalize, activation, initialize, device)
             layers.extend(mlp)
-        layers.extend(mlp_block(input_shape[0], action_dim, None, nn.Tanh, initialize, device)[0])
+        layers.extend(mlp_block(input_shape[0], action_dim, None, nn.Sigmoid, initialize, device)[0])
         self.model = nn.Sequential(*layers)
 
     def forward(self, x: torch.tensor):
-        return torch.sigmoid(self.model(x))
+        return self.model(x)
 
 
 class CriticNet(nn.Module):
     def __init__(self,
                  independent: bool,
                  state_dim: int,
                  n_agents: int,
@@ -344,15 +345,15 @@
         assert isinstance(action_space, Box_pettingzoo)
         super(Basic_DDPG_policy, self).__init__()
         self.action_dim = action_space.shape[0]
         self.n_agents = n_agents
         self.representation = representation
         self.representation_info_shape = self.representation.output_shapes
 
-        self.actor_net = ActorNet(representation.output_shapes['state'][0], n_agents, self.action_dim,
+        self.actor_net = ActorNet(representation.output_shapes['state'][0], n_agents, action_space,
                                   actor_hidden_size, normalize, initialize, activation, device)
         self.critic_net = CriticNet(True, representation.output_shapes['state'][0], n_agents, self.action_dim,
                                     critic_hidden_size, normalize, initialize, activation, device)
         self.target_actor_net = copy.deepcopy(self.actor_net)
         self.target_critic_net = copy.deepcopy(self.critic_net)
         self.parameters_actor = list(self.representation.parameters()) + list(self.actor_net.parameters())
         self.parameters_critic = self.critic_net.parameters()
```

### Comparing `xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_torch/policies/gaussian.py` & `xuanpolicy-0.1.6/xuanpolicy/torch/policies/gaussian.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import torch
 
-from xuanpolicy.xuanpolicy_torch.policies import *
-from xuanpolicy.xuanpolicy_torch.utils import *
-from xuanpolicy.xuanpolicy_torch.representations import Basic_Identical
+from xuanpolicy.torch.policies import *
+from xuanpolicy.torch.utils import *
+from xuanpolicy.torch.representations import Basic_Identical
 
 
 class ActorNet(nn.Module):
     def __init__(self,
                  state_dim: int,
                  action_dim: int,
                  hidden_sizes: Sequence[int],
```

### Comparing `xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_torch/policies/gaussian_marl.py` & `xuanpolicy-0.1.6/xuanpolicy/torch/policies/gaussian_marl.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import torch.distributions
 
-from xuanpolicy.xuanpolicy_torch.policies import *
-from xuanpolicy.xuanpolicy_torch.utils import *
-from xuanpolicy.xuanpolicy_torch.representations import Basic_Identical
+from xuanpolicy.torch.policies import *
+from xuanpolicy.torch.utils import *
+from xuanpolicy.torch.representations import Basic_Identical
+from gymnasium.spaces.box import Box as Box_pettingzoo
 
 
 class BasicQhead(nn.Module):
     def __init__(self,
                  state_dim: int,
                  action_dim: int,
                  n_agents: int,
@@ -137,15 +138,15 @@
                  actor_hidden_size: Sequence[int],
                  critic_hidden_size: Sequence[int],
                  normalize: Optional[ModuleType] = None,
                  initialize: Optional[Callable[..., torch.Tensor]] = None,
                  activation: Optional[ModuleType] = None,
                  device: Optional[Union[str, int, torch.device]] = None
                  ):
-        assert isinstance(action_space, Box)
+        assert isinstance(action_space, Box_pettingzoo)
         super(Basic_ISAC_policy, self).__init__()
         self.action_dim = action_space.shape[0]
         self.n_agents = n_agents
         self.representation = representation
         self.representation_info_shape = self.representation.output_shapes
 
         self.actor_net = ActorNet(representation.output_shapes['state'][0], n_agents, self.action_dim,
@@ -195,15 +196,15 @@
                  actor_hidden_size: Sequence[int],
                  critic_hidden_size: Sequence[int],
                  normalize: Optional[ModuleType] = None,
                  initialize: Optional[Callable[..., torch.Tensor]] = None,
                  activation: Optional[ModuleType] = None,
                  device: Optional[Union[str, int, torch.device]] = None
                  ):
-        assert isinstance(action_space, Box)
+        assert isinstance(action_space, Box_pettingzoo)
         super(MASAC_policy, self).__init__(action_space, n_agents, representation,
                                             actor_hidden_size, critic_hidden_size,
                                             normalize, initialize, activation, device)
         self.critic_net = CriticNet(False, representation.output_shapes['state'][0], n_agents, self.action_dim,
                                     critic_hidden_size, normalize, initialize, activation, device)
         self.target_critic_net = copy.deepcopy(self.critic_net)
         self.parameters_critic = self.critic_net.parameters()
```

### Comparing `xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_torch/policies/mixers.py` & `xuanpolicy-0.1.6/xuanpolicy/torch/policies/mixers.py`

 * *Files identical despite different names*

### Comparing `xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_torch/representations/__init__.py` & `xuanpolicy-0.1.6/xuanpolicy/torch/representations/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import torch
 import torch.nn as nn
 import torch.nn.functional as F
 import numpy as np
 from typing import Sequence, Union, Optional, Callable
-from xuanpolicy.xuanpolicy_torch.utils.layers import *
+from xuanpolicy.torch.utils.layers import *
 
 from .networks import Basic_MLP
 from .networks import Basic_Identical
 from .networks import Basic_CNN
 from .networks import CoG_MLP, CoG_RNN, CoG_CNN
 from .networks import C_DQN,L_DQN,CL_DQN
```

### Comparing `xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_torch/representations/networks.py` & `xuanpolicy-0.1.6/xuanpolicy/torch/representations/networks.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from xuanpolicy.xuanpolicy_torch.representations import *
+from xuanpolicy.torch.representations import *
 
 
 # directly returns the original observation
 class Basic_Identical(nn.Module):
     def __init__(self,
                  input_shape: Sequence[int],
                  device: Optional[Union[str, int, torch.device]] = None):
```

### Comparing `xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_torch/runners/runner_basic.py` & `xuanpolicy-0.1.6/xuanpolicy/mindspore/runners/runner_basic.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+import time
+
 from xuanpolicy.environment import make_envs
 
 
 class Runner_Base(object):
     def __init__(self, args):
         # build environments
         if hasattr(args, 'continuous_action'):
@@ -21,14 +23,16 @@
 
     def tb_load(self, data):
         return
 
 
 class Runner_Base_MARL(Runner_Base):
     def __init__(self, args):
+        if args.test_mode:
+            args.render_mode = 'human'
         super(Runner_Base_MARL, self).__init__(args)
         # build environments
         self.n_handles = len(self.envs.handles)
         self.loss = [[0.0] for _ in range(self.n_handles)]
 
         self.agent_keys = self.envs.agent_keys
         self.agent_ids = self.envs.agent_ids
@@ -91,8 +95,8 @@
         for h, arg in enumerate(args):
             agent_name = self.envs.agent_keys[h][0][0:-2]
             if arg.n_agents == 1:
                 infos.append(agent_name + ": {} agent".format(arg.n_agents) + ", {}".format(arg.agent))
             else:
                 infos.append(agent_name + ": {} agents".format(arg.n_agents) + ", {}".format(arg.agent))
         print(infos)
-
+        time.sleep(0.01)
```

### Comparing `xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_torch/runners/runner_drl.py` & `xuanpolicy-0.1.6/xuanpolicy/torch/runners/runner_drl.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from .runner_basic import *
-from xuanpolicy.xuanpolicy_torch.agents import get_total_iters
-from xuanpolicy.xuanpolicy_torch.representations import REGISTRY as REGISTRY_Representation
-from xuanpolicy.xuanpolicy_torch.agents import REGISTRY as REGISTRY_Agent
-from xuanpolicy.xuanpolicy_torch.policies import REGISTRY as REGISTRY_Policy
-from xuanpolicy.xuanpolicy_torch.utils.input_reformat import get_repre_in, get_policy_in
+from xuanpolicy.torch.agents import get_total_iters
+from xuanpolicy.torch.representations import REGISTRY as REGISTRY_Representation
+from xuanpolicy.torch.agents import REGISTRY as REGISTRY_Agent
+from xuanpolicy.torch.policies import REGISTRY as REGISTRY_Policy
+from xuanpolicy.torch.utils.input_reformat import get_repre_in, get_policy_in
 import itertools
 import torch
 import gym.spaces
 import numpy as np
 
 
 class Runner_DRL(Runner_Base):
@@ -66,8 +66,9 @@
             optimizer = torch.optim.Adam(policy.parameters(), self.args.learning_rate, eps=1e-5)
             lr_scheduler = torch.optim.lr_scheduler.LinearLR(optimizer, start_factor=1.0, end_factor=0.5,
                                                              total_iters=get_total_iters(self.agent_name, self.args))
             self.agent = REGISTRY_Agent[self.agent_name](self.args, self.envs, policy, optimizer, lr_scheduler,
                                                          self.args.device)
 
     def run(self):
-        self.agent.test() if self.args.test_mode else self.agent.train(self.args.training_steps)
+        self.agent.test(self.args.test_steps) if self.args.test_mode else self.agent.train(self.args.training_steps)
+        self.envs.close()
```

### Comparing `xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_torch/runners/runner_marl.py` & `xuanpolicy-0.1.6/xuanpolicy/mindspore/runners/runner_marl.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from .runner_basic import *
-from xuanpolicy.xuanpolicy_torch.agents import REGISTRY as REGISTRY_Agent
-from gymnasium.spaces.box import Box
+from xuanpolicy.mindspore.agents import REGISTRY as REGISTRY_Agent
+from gym.spaces import Box
 from tqdm import tqdm
 import numpy as np
 from copy import deepcopy
+import time
 
 
 class Runner(Runner_Base_MARL):
     def __init__(self, args):
         self.args = args if type(args) == list else [args]
         super(Runner, self).__init__(self.args[0])
 
@@ -23,15 +24,15 @@
             else:
                 arg.dim_act = self.envs.action_space[self.agent_keys[h][0]].n
                 arg.act_shape = (arg.n_agents,)
             arg.action_space = self.envs.action_space
             arg.dim_obs = self.envs.observation_space[self.agent_keys[h][0]].shape
             arg.obs_shape = (arg.n_agents,) + arg.dim_obs
             arg.rew_shape, arg.done_shape, arg.act_prob_shape = (arg.n_agents, 1), (arg.n_agents,), (arg.dim_act,)
-            self.marl_agents.append(REGISTRY_Agent[arg.agent](arg, self.envs, arg.device))
+            self.marl_agents.append(REGISTRY_Agent[arg.agent](arg, self.envs))
             self.marl_names.append(arg.agent)
             if arg.test_mode:
                 self.marl_agents[h].load_model(arg.modeldir)
 
         self.print_infos(self.args)
 
     def run_episode(self, episode, test_mode=False):
@@ -44,15 +45,16 @@
 
         while True:
             actions_dict = self.get_actions(obs_n, episode, test_mode, act_mean_last, agent_mask, state)
             actions_execute = self.combine_env_actions(actions_dict['actions_n'])
             next_obs_n, rew_n, done_n, dones, info = self.envs.step(actions_execute)
             next_state, agent_mask = self.envs.global_state(), self.envs.agent_mask()
 
-            if self.render or self.test_mode: self.envs.render(self.render_delay)
+            if self.render or self.test_mode:
+                time.sleep(self.render_delay)
             if test_mode:
                 for h in range(self.n_handles):
                     scores[h] += (1-done_envs) * np.mean(rew_n[h] * agent_mask[h][:, :, np.newaxis], axis=1)
             else:
                 self.store_data(obs_n, next_obs_n, actions_dict, state, next_state, agent_mask, rew_n, done_n, self.envs)
                 for h, mas_group in enumerate(self.marl_agents):
                     if self.args[h].train_at_step: self.marl_agents[h].train(episode)
@@ -107,15 +109,15 @@
                          'state': state, 'state_next': next_state, 'rewards': rew_n[h],
                          'agent_mask': agent_mask[h], 'terminals': done_n[h]}
             if self.marl_names[h] in ["CID_Simple", "CID_Rainbow"]:
                 rew_n_assign = mas_group.reward_shaping(state, obs_n[h], actions_dict['actions_n'][h], rew_n[h], env)
                 data_step.update({'rewards_assign': rew_n_assign})
             elif self.marl_names[h] in ["MAPPO_KL", "MAPPO_Clip", "VDAC"]:
                 if self.marl_names[h] == "MAPPO_KL":
-                    data_step.update({'values': actions_dict['values'][h], 'pi_dist_old': actions_dict['log_pi'][h]})
+                    data_step.update({'values': actions_dict['values'][h], 'act_prob_old': actions_dict['log_pi'][h]})
                 else:
                     data_step.update({'values': actions_dict['values'][h], 'log_pi_old': actions_dict['log_pi'][h]})
             elif self.marl_names[h] in ["COMA"]:
                 data_step.update({'actions_onehot': actions_dict['act_n_onehot'][h]})
             elif self.marl_names[h] in ["MFQ", "MFAC"]:
                 data_step.update({'act_mean': actions_dict['act_mean'][h]})
             else:
```

### Comparing `xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_torch/utils/distributions.py` & `xuanpolicy-0.1.6/xuanpolicy/torch/utils/distributions.py`

 * *Files identical despite different names*

### Comparing `xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_torch/utils/input_reformat.py` & `xuanpolicy-0.1.6/xuanpolicy/torch/utils/input_reformat.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from xuanpolicy.common import space2shape
 from copy import deepcopy
-from xuanpolicy.xuanpolicy_torch.policies import Policy_Inputs, Policy_Inputs_All
-from xuanpolicy.xuanpolicy_torch.representations import Representation_Inputs, Representation_Inputs_All
+from xuanpolicy.torch.policies import Policy_Inputs, Policy_Inputs_All
+from xuanpolicy.torch.representations import Representation_Inputs, Representation_Inputs_All
 from operator import itemgetter
 import torch
 
 
 def get_repre_in(args):
     representation_name = args.representation
     input_dict = deepcopy(Representation_Inputs_All)
```

### Comparing `xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_torch/utils/layers.py` & `xuanpolicy-0.1.6/xuanpolicy/torch/utils/layers.py`

 * *Files identical despite different names*

### Comparing `xuanpolicy-0.1.5/xuanpolicy/xuanpolicy_torch/utils/operations.py` & `xuanpolicy-0.1.6/xuanpolicy/torch/utils/operations.py`

 * *Files identical despite different names*

### Comparing `xuanpolicy-0.1.5/xuanpolicy.egg-info/PKG-INFO` & `xuanpolicy-0.1.6/xuanpolicy.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xuanpolicy
-Version: 0.1.5
+Version: 0.1.6
 Summary: XuanPolicy: A Comprehensive Deep Reinforcement Learning Library.
 Home-page: 
 Download-URL: 
 Author: Wenzhang Liu, Wenzhe Cai, Kun Jiang, etc.
 Author-email: 
 License: MIT
 Keywords: deep reinforcement learning,software library,platform
```

