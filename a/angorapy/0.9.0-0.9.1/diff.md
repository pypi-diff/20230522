# Comparing `tmp/angorapy-0.9.0.tar.gz` & `tmp/angorapy-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "angorapy-0.9.0.tar", last modified: Sat Mar 25 16:32:09 2023, max compression
+gzip compressed data, was "angorapy-0.9.1.tar", last modified: Mon May 22 11:50:38 2023, max compression
```

## Comparing `angorapy-0.9.0.tar` & `angorapy-0.9.1.tar`

### file list

```diff
@@ -1,177 +1,176 @@
-drwxrwxr-x   0 weidler   (1000) weidler   (1000)        0 2023-03-25 16:32:09.620537 angorapy-0.9.0/
--rw-rw-r--   0 weidler   (1000) weidler   (1000)    34502 2020-12-04 16:52:46.000000 angorapy-0.9.0/LICENSE
--rw-rw-r--   0 weidler   (1000) weidler   (1000)     8379 2023-03-25 16:32:09.620537 angorapy-0.9.0/PKG-INFO
--rw-rw-r--   0 weidler   (1000) weidler   (1000)     7579 2023-02-24 12:57:38.000000 angorapy-0.9.0/README.md
-drwxrwxr-x   0 weidler   (1000) weidler   (1000)        0 2023-03-25 16:32:09.608537 angorapy-0.9.0/angorapy/
--rw-rw-r--   0 weidler   (1000) weidler   (1000)      302 2023-03-25 14:31:30.000000 angorapy-0.9.0/angorapy/__init__.py
-drwxrwxr-x   0 weidler   (1000) weidler   (1000)        0 2023-03-25 16:32:09.608537 angorapy-0.9.0/angorapy/agent/
--rw-rw-r--   0 weidler   (1000) weidler   (1000)      125 2022-07-01 11:57:01.000000 angorapy-0.9.0/angorapy/agent/__init__.py
--rw-rw-r--   0 weidler   (1000) weidler   (1000)     4583 2022-07-01 11:57:02.000000 angorapy-0.9.0/angorapy/agent/core.py
--rw-rw-r--   0 weidler   (1000) weidler   (1000)     6243 2023-03-17 08:50:52.000000 angorapy-0.9.0/angorapy/agent/dataio.py
--rw-rw-r--   0 weidler   (1000) weidler   (1000)    15141 2023-03-25 11:16:16.000000 angorapy-0.9.0/angorapy/agent/gather.py
-drwxrwxr-x   0 weidler   (1000) weidler   (1000)        0 2023-03-25 16:32:09.608537 angorapy-0.9.0/angorapy/agent/ppo/
--rw-rw-r--   0 weidler   (1000) weidler   (1000)        0 2022-07-01 11:57:01.000000 angorapy-0.9.0/angorapy/agent/ppo/__init__.py
--rw-rw-r--   0 weidler   (1000) weidler   (1000)     4347 2023-02-24 12:57:38.000000 angorapy-0.9.0/angorapy/agent/ppo/loss.py
--rw-rw-r--   0 weidler   (1000) weidler   (1000)     4637 2023-02-24 12:57:38.000000 angorapy-0.9.0/angorapy/agent/ppo/optim.py
--rw-rw-r--   0 weidler   (1000) weidler   (1000)    57431 2023-03-25 13:59:27.000000 angorapy-0.9.0/angorapy/agent/ppo_agent.py
-drwxrwxr-x   0 weidler   (1000) weidler   (1000)        0 2023-03-25 16:32:09.608537 angorapy-0.9.0/angorapy/analysis/
--rw-rw-r--   0 weidler   (1000) weidler   (1000)       74 2023-03-25 14:32:12.000000 angorapy-0.9.0/angorapy/analysis/__init__.py
--rw-rw-r--   0 weidler   (1000) weidler   (1000)    12821 2022-11-04 09:11:45.000000 angorapy-0.9.0/angorapy/analysis/chiefinvestigation.py
--rw-rw-r--   0 weidler   (1000) weidler   (1000)      817 2023-02-24 12:57:45.000000 angorapy-0.9.0/angorapy/analysis/dynamics.py
--rw-rw-r--   0 weidler   (1000) weidler   (1000)      426 2023-02-24 12:57:38.000000 angorapy-0.9.0/angorapy/analysis/inspect_camera.py
-drwxrwxr-x   0 weidler   (1000) weidler   (1000)        0 2023-03-25 16:32:09.608537 angorapy-0.9.0/angorapy/analysis/investigators/
--rw-rw-r--   0 weidler   (1000) weidler   (1000)      297 2023-03-25 13:11:41.000000 angorapy-0.9.0/angorapy/analysis/investigators/__init__.py
--rw-rw-r--   0 weidler   (1000) weidler   (1000)    11196 2023-03-25 15:23:23.000000 angorapy-0.9.0/angorapy/analysis/investigators/base_investigator.py
--rw-rw-r--   0 weidler   (1000) weidler   (1000)     1398 2023-02-24 12:57:45.000000 angorapy-0.9.0/angorapy/analysis/investigators/correlation.py
--rw-rw-r--   0 weidler   (1000) weidler   (1000)     5217 2023-02-24 12:57:45.000000 angorapy-0.9.0/angorapy/analysis/investigators/dynamics.py
--rw-rw-r--   0 weidler   (1000) weidler   (1000)     6097 2023-03-20 14:10:23.000000 angorapy-0.9.0/angorapy/analysis/investigators/predictability.py
--rw-rw-r--   0 weidler   (1000) weidler   (1000)      738 2023-03-21 07:48:24.000000 angorapy-0.9.0/angorapy/analysis/plot_predictability.py
--rw-rw-r--   0 weidler   (1000) weidler   (1000)     1282 2023-02-24 12:57:45.000000 angorapy-0.9.0/angorapy/analysis/plot_predictability_grouped.py
--rw-rw-r--   0 weidler   (1000) weidler   (1000)     1347 2023-03-21 08:14:54.000000 angorapy-0.9.0/angorapy/analysis/plot_predictability_grouped_with_error_bars.py
--rw-rw-r--   0 weidler   (1000) weidler   (1000)      723 2023-03-21 07:53:15.000000 angorapy-0.9.0/angorapy/analysis/plot_predictability_with_error_bars.py
--rw-rw-r--   0 weidler   (1000) weidler   (1000)     2625 2022-07-01 11:57:02.000000 angorapy-0.9.0/angorapy/analysis/plot_utils.py
-drwxrwxr-x   0 weidler   (1000) weidler   (1000)        0 2023-03-25 16:32:09.612537 angorapy-0.9.0/angorapy/analysis/plotting/
--rw-rw-r--   0 weidler   (1000) weidler   (1000)        0 2022-07-01 11:57:01.000000 angorapy-0.9.0/angorapy/analysis/plotting/__init__.py
--rw-rw-r--   0 weidler   (1000) weidler   (1000)     5798 2023-02-24 12:57:38.000000 angorapy-0.9.0/angorapy/analysis/plotting/autocorrelation_combined_plot.py
--rw-rw-r--   0 weidler   (1000) weidler   (1000)      865 2022-07-01 11:57:02.000000 angorapy-0.9.0/angorapy/analysis/plotting/make_viz_featuremax.py
--rw-rw-r--   0 weidler   (1000) weidler   (1000)     2059 2022-07-01 11:57:02.000000 angorapy-0.9.0/angorapy/analysis/plotting/make_viz_pretraining_fmap.py
--rw-rw-r--   0 weidler   (1000) weidler   (1000)     1452 2022-07-01 11:57:02.000000 angorapy-0.9.0/angorapy/analysis/plotting/make_viz_pretraining_saliency.py
--rw-rw-r--   0 weidler   (1000) weidler   (1000)     2269 2022-07-01 11:57:02.000000 angorapy-0.9.0/angorapy/analysis/plotting/plot_benchmark.py
--rw-rw-r--   0 weidler   (1000) weidler   (1000)     3879 2023-02-24 12:57:38.000000 angorapy-0.9.0/angorapy/analysis/plotting/plot_benchmark_groups.py
--rw-rw-r--   0 weidler   (1000) weidler   (1000)     5484 2023-02-24 12:57:38.000000 angorapy-0.9.0/angorapy/analysis/plotting/plot_benchmark_groups_with_beta.py
--rw-rw-r--   0 weidler   (1000) weidler   (1000)     1316 2023-02-24 12:57:38.000000 angorapy-0.9.0/angorapy/analysis/plotting/plot_distributed_computation_benchmark.py
--rw-rw-r--   0 weidler   (1000) weidler   (1000)      665 2022-07-01 11:57:02.000000 angorapy-0.9.0/angorapy/analysis/plotting/plot_experiment_best_evaluation.py
--rw-rw-r--   0 weidler   (1000) weidler   (1000)     1043 2023-02-24 12:57:38.000000 angorapy-0.9.0/angorapy/analysis/plotting/plot_experiment_comparison.py
--rw-rw-r--   0 weidler   (1000) weidler   (1000)     4765 2023-03-22 16:18:12.000000 angorapy-0.9.0/angorapy/analysis/plotting/plot_experiment_comparison_only_success_multiple_runs.py
--rw-rw-r--   0 weidler   (1000) weidler   (1000)     4796 2023-02-24 12:57:38.000000 angorapy-0.9.0/angorapy/analysis/plotting/plot_experiment_comparison_only_success_multiple_runs_line_scatter.py
--rw-rw-r--   0 weidler   (1000) weidler   (1000)     5109 2023-02-24 12:57:38.000000 angorapy-0.9.0/angorapy/analysis/plotting/plot_experiment_comparison_only_success_multiple_runs_with_zoom.py
--rw-rw-r--   0 weidler   (1000) weidler   (1000)     2601 2023-02-24 12:57:38.000000 angorapy-0.9.0/angorapy/analysis/plotting/plot_experiment_comparison_with_success.py
--rw-rw-r--   0 weidler   (1000) weidler   (1000)     6481 2023-02-24 12:57:38.000000 angorapy-0.9.0/angorapy/analysis/plotting/plot_experiment_comparison_with_success_multiple_runs.py
--rw-rw-r--   0 weidler   (1000) weidler   (1000)     2289 2023-01-18 14:21:44.000000 angorapy-0.9.0/angorapy/analysis/plotting/plot_experiment_progression.py
--rw-rw-r--   0 weidler   (1000) weidler   (1000)     1446 2022-07-01 11:57:02.000000 angorapy-0.9.0/angorapy/analysis/plotting/plot_losses.py
--rw-rw-r--   0 weidler   (1000) weidler   (1000)     3260 2023-03-21 08:19:26.000000 angorapy-0.9.0/angorapy/analysis/predictability.py
-drwxrwxr-x   0 weidler   (1000) weidler   (1000)        0 2023-03-25 16:32:09.612537 angorapy-0.9.0/angorapy/analysis/sindy/
--rw-rw-r--   0 weidler   (1000) weidler   (1000)        0 2023-02-24 12:57:45.000000 angorapy-0.9.0/angorapy/analysis/sindy/__init__.py
--rw-rw-r--   0 weidler   (1000) weidler   (1000)     1910 2023-02-24 12:57:45.000000 angorapy-0.9.0/angorapy/analysis/sindy/autoencoder.py
--rw-rw-r--   0 weidler   (1000) weidler   (1000)      286 2023-02-24 12:57:45.000000 angorapy-0.9.0/angorapy/analysis/sindy/loss.py
-drwxrwxr-x   0 weidler   (1000) weidler   (1000)        0 2023-03-25 16:32:09.612537 angorapy-0.9.0/angorapy/analysis/util/
--rw-rw-r--   0 weidler   (1000) weidler   (1000)        0 2023-02-24 12:57:45.000000 angorapy-0.9.0/angorapy/analysis/util/__init__.py
--rw-rw-r--   0 weidler   (1000) weidler   (1000)     9175 2023-02-24 12:57:45.000000 angorapy-0.9.0/angorapy/analysis/util/sindy.py
--rw-rw-r--   0 weidler   (1000) weidler   (1000)    17221 2022-07-01 11:57:02.000000 angorapy-0.9.0/angorapy/analysis/visualization.py
--rw-rw-r--   0 weidler   (1000) weidler   (1000)     5073 2022-07-01 11:57:02.000000 angorapy-0.9.0/angorapy/benchmark.py
-drwxrwxr-x   0 weidler   (1000) weidler   (1000)        0 2023-03-25 16:32:09.612537 angorapy-0.9.0/angorapy/common/
--rw-rw-r--   0 weidler   (1000) weidler   (1000)        0 2022-07-01 11:57:01.000000 angorapy-0.9.0/angorapy/common/__init__.py
--rw-rw-r--   0 weidler   (1000) weidler   (1000)     2398 2023-02-24 12:57:38.000000 angorapy-0.9.0/angorapy/common/activations.py
--rw-rw-r--   0 weidler   (1000) weidler   (1000)     1369 2023-02-24 12:57:38.000000 angorapy-0.9.0/angorapy/common/const.py
--rw-rw-r--   0 weidler   (1000) weidler   (1000)     8123 2023-02-24 12:57:38.000000 angorapy-0.9.0/angorapy/common/data_buffers.py
--rw-rw-r--   0 weidler   (1000) weidler   (1000)     1610 2023-03-13 17:47:00.000000 angorapy-0.9.0/angorapy/common/layers.py
--rw-rw-r--   0 weidler   (1000) weidler   (1000)     1350 2022-07-01 11:57:02.000000 angorapy-0.9.0/angorapy/common/loss.py
--rw-rw-r--   0 weidler   (1000) weidler   (1000)     3073 2023-03-20 13:15:59.000000 angorapy-0.9.0/angorapy/common/mpi_optim.py
--rw-rw-r--   0 weidler   (1000) weidler   (1000)    25984 2023-03-25 16:05:06.000000 angorapy-0.9.0/angorapy/common/policies.py
--rw-rw-r--   0 weidler   (1000) weidler   (1000)     6261 2023-02-24 12:57:38.000000 angorapy-0.9.0/angorapy/common/reward.py
--rw-rw-r--   0 weidler   (1000) weidler   (1000)     7840 2023-02-24 13:11:30.000000 angorapy-0.9.0/angorapy/common/senses.py
--rw-rw-r--   0 weidler   (1000) weidler   (1000)    11433 2023-03-12 11:30:11.000000 angorapy-0.9.0/angorapy/common/transformers.py
--rw-rw-r--   0 weidler   (1000) weidler   (1000)     6028 2023-03-24 16:47:12.000000 angorapy-0.9.0/angorapy/common/wrappers.py
-drwxrwxr-x   0 weidler   (1000) weidler   (1000)        0 2023-03-25 16:32:09.612537 angorapy-0.9.0/angorapy/configs/
--rw-rw-r--   0 weidler   (1000) weidler   (1000)        0 2022-07-01 11:57:01.000000 angorapy-0.9.0/angorapy/configs/__init__.py
--rw-rw-r--   0 weidler   (1000) weidler   (1000)     8258 2023-02-24 12:57:45.000000 angorapy-0.9.0/angorapy/configs/hp_config.py
--rw-rw-r--   0 weidler   (1000) weidler   (1000)     2251 2022-07-01 11:57:02.000000 angorapy-0.9.0/angorapy/configs/reward_config.py
-drwxrwxr-x   0 weidler   (1000) weidler   (1000)        0 2023-03-25 16:32:09.612537 angorapy-0.9.0/angorapy/environments/
--rw-rw-r--   0 weidler   (1000) weidler   (1000)    11768 2023-03-24 16:48:56.000000 angorapy-0.9.0/angorapy/environments/__init__.py
--rw-rw-r--   0 weidler   (1000) weidler   (1000)     2082 2022-07-01 12:01:11.000000 angorapy-0.9.0/angorapy/environments/adapted.py
--rw-rw-r--   0 weidler   (1000) weidler   (1000)    11094 2023-03-24 16:43:54.000000 angorapy-0.9.0/angorapy/environments/anthrobotics.py
-drwxrwxr-x   0 weidler   (1000) weidler   (1000)        0 2023-03-25 16:32:09.612537 angorapy-0.9.0/angorapy/environments/assets/
--rw-rw-r--   0 weidler   (1000) weidler   (1000)    12706 2022-07-01 12:01:11.000000 angorapy-0.9.0/angorapy/environments/assets/LICENSE.md
-drwxrwxr-x   0 weidler   (1000) weidler   (1000)        0 2023-03-25 16:32:09.612537 angorapy-0.9.0/angorapy/environments/assets/hand/
--rw-rw-r--   0 weidler   (1000) weidler   (1000)     2329 2022-07-01 12:00:59.000000 angorapy-0.9.0/angorapy/environments/assets/hand/manipulate_block.xml
--rw-rw-r--   0 weidler   (1000) weidler   (1000)     2401 2022-07-01 12:00:59.000000 angorapy-0.9.0/angorapy/environments/assets/hand/manipulate_block_touch_sensors.xml
--rw-rw-r--   0 weidler   (1000) weidler   (1000)     2326 2022-07-01 12:00:59.000000 angorapy-0.9.0/angorapy/environments/assets/hand/manipulate_egg.xml
--rw-rw-r--   0 weidler   (1000) weidler   (1000)     2394 2022-07-01 12:00:59.000000 angorapy-0.9.0/angorapy/environments/assets/hand/manipulate_egg_touch_sensors.xml
--rw-rw-r--   0 weidler   (1000) weidler   (1000)     2184 2022-07-01 12:00:59.000000 angorapy-0.9.0/angorapy/environments/assets/hand/manipulate_pen.xml
--rw-rw-r--   0 weidler   (1000) weidler   (1000)     2252 2022-07-01 12:00:59.000000 angorapy-0.9.0/angorapy/environments/assets/hand/manipulate_pen_touch_sensors.xml
--rw-rw-r--   0 weidler   (1000) weidler   (1000)    16788 2022-07-01 12:00:59.000000 angorapy-0.9.0/angorapy/environments/assets/hand/robot.xml
--rw-rw-r--   0 weidler   (1000) weidler   (1000)    32115 2022-07-01 12:00:59.000000 angorapy-0.9.0/angorapy/environments/assets/hand/robot_touch_sensors_92.xml
--rw-rw-r--   0 weidler   (1000) weidler   (1000)     2091 2023-02-24 12:57:38.000000 angorapy-0.9.0/angorapy/environments/assets/hand/shadowhand.xml
--rw-rw-r--   0 weidler   (1000) weidler   (1000)     3389 2022-07-01 12:00:59.000000 angorapy-0.9.0/angorapy/environments/assets/hand/shadowhand_manipulate.xml
--rw-rw-r--   0 weidler   (1000) weidler   (1000)    16537 2022-07-01 12:00:59.000000 angorapy-0.9.0/angorapy/environments/assets/hand/shared.xml
--rw-rw-r--   0 weidler   (1000) weidler   (1000)     2052 2022-07-01 12:00:59.000000 angorapy-0.9.0/angorapy/environments/assets/hand/shared_asset.xml
--rw-rw-r--   0 weidler   (1000) weidler   (1000)     9201 2022-07-01 12:00:59.000000 angorapy-0.9.0/angorapy/environments/assets/hand/shared_touch_sensors_92.xml
--rw-rw-r--   0 weidler   (1000) weidler   (1000)    31885 2022-07-01 12:00:59.000000 angorapy-0.9.0/angorapy/environments/assets/hand/touch_sensors.xml
-drwxrwxr-x   0 weidler   (1000) weidler   (1000)        0 2023-03-25 16:32:09.604537 angorapy-0.9.0/angorapy/environments/assets/stls/
-drwxrwxr-x   0 weidler   (1000) weidler   (1000)        0 2023-03-25 16:32:09.616537 angorapy-0.9.0/angorapy/environments/assets/stls/hand/
--rw-rw-r--   0 weidler   (1000) weidler   (1000)    17084 2022-07-01 12:01:11.000000 angorapy-0.9.0/angorapy/environments/assets/stls/hand/F1.stl
--rw-rw-r--   0 weidler   (1000) weidler   (1000)    22884 2022-07-01 12:01:11.000000 angorapy-0.9.0/angorapy/environments/assets/stls/hand/F2.stl
--rw-rw-r--   0 weidler   (1000) weidler   (1000)    54684 2022-07-01 12:01:11.000000 angorapy-0.9.0/angorapy/environments/assets/stls/hand/F3.stl
--rw-rw-r--   0 weidler   (1000) weidler   (1000)     6334 2022-07-01 12:01:11.000000 angorapy-0.9.0/angorapy/environments/assets/stls/hand/TH1_z.stl
--rw-rw-r--   0 weidler   (1000) weidler   (1000)    63184 2022-07-01 12:01:11.000000 angorapy-0.9.0/angorapy/environments/assets/stls/hand/TH2_z.stl
--rw-rw-r--   0 weidler   (1000) weidler   (1000)    21184 2022-07-01 12:01:11.000000 angorapy-0.9.0/angorapy/environments/assets/stls/hand/TH3_z.stl
--rw-rw-r--   0 weidler   (1000) weidler   (1000)   934534 2022-07-01 12:01:11.000000 angorapy-0.9.0/angorapy/environments/assets/stls/hand/forearm_electric.stl
--rw-rw-r--   0 weidler   (1000) weidler   (1000)    45384 2022-07-01 12:01:11.000000 angorapy-0.9.0/angorapy/environments/assets/stls/hand/forearm_electric_cvx.stl
--rw-rw-r--   0 weidler   (1000) weidler   (1000)    30184 2022-07-01 12:01:11.000000 angorapy-0.9.0/angorapy/environments/assets/stls/hand/knuckle.stl
--rw-rw-r--   0 weidler   (1000) weidler   (1000)    75084 2022-07-01 12:01:11.000000 angorapy-0.9.0/angorapy/environments/assets/stls/hand/lfmetacarpal.stl
--rw-rw-r--   0 weidler   (1000) weidler   (1000)   347784 2022-07-01 12:01:11.000000 angorapy-0.9.0/angorapy/environments/assets/stls/hand/palm.stl
--rw-rw-r--   0 weidler   (1000) weidler   (1000)    92784 2022-07-01 12:01:11.000000 angorapy-0.9.0/angorapy/environments/assets/stls/hand/wrist.stl
-drwxrwxr-x   0 weidler   (1000) weidler   (1000)        0 2023-03-25 16:32:09.616537 angorapy-0.9.0/angorapy/environments/assets/textures/
--rw-rw-r--   0 weidler   (1000) weidler   (1000)    15879 2022-07-01 12:01:11.000000 angorapy-0.9.0/angorapy/environments/assets/textures/block.png
--rw-rw-r--   0 weidler   (1000) weidler   (1000)    40953 2022-07-01 12:01:11.000000 angorapy-0.9.0/angorapy/environments/assets/textures/block_hidden.png
-drwxrwxr-x   0 weidler   (1000) weidler   (1000)        0 2023-03-25 16:32:09.616537 angorapy-0.9.0/angorapy/environments/hand/
--rw-rw-r--   0 weidler   (1000) weidler   (1000)        0 2023-02-24 12:57:38.000000 angorapy-0.9.0/angorapy/environments/hand/__init__.py
--rw-rw-r--   0 weidler   (1000) weidler   (1000)    24334 2023-03-24 16:43:54.000000 angorapy-0.9.0/angorapy/environments/hand/manipulate.py
--rw-rw-r--   0 weidler   (1000) weidler   (1000)    17277 2023-02-24 12:57:45.000000 angorapy-0.9.0/angorapy/environments/hand/reach.py
--rw-rw-r--   0 weidler   (1000) weidler   (1000)    13121 2023-03-22 14:16:51.000000 angorapy-0.9.0/angorapy/environments/hand/shadowhand.py
--rw-rw-r--   0 weidler   (1000) weidler   (1000)      330 2022-09-14 11:48:13.000000 angorapy-0.9.0/angorapy/environments/hand/test.py
--rw-rw-r--   0 weidler   (1000) weidler   (1000)     6574 2023-02-24 12:57:38.000000 angorapy-0.9.0/angorapy/environments/hanoi.py
--rw-rw-r--   0 weidler   (1000) weidler   (1000)    13272 2023-02-24 12:57:45.000000 angorapy-0.9.0/angorapy/environments/rotations.py
--rw-rw-r--   0 weidler   (1000) weidler   (1000)      478 2022-07-01 12:01:11.000000 angorapy-0.9.0/angorapy/environments/test.py
--rw-rw-r--   0 weidler   (1000) weidler   (1000)     1043 2022-07-01 11:57:02.000000 angorapy-0.9.0/angorapy/environments/utils.py
--rw-rw-r--   0 weidler   (1000) weidler   (1000)     3285 2023-03-25 13:55:04.000000 angorapy-0.9.0/angorapy/evaluate.py
-drwxrwxr-x   0 weidler   (1000) weidler   (1000)        0 2023-03-25 16:32:09.616537 angorapy-0.9.0/angorapy/models/
--rw-rw-r--   0 weidler   (1000) weidler   (1000)     1196 2023-03-16 13:21:33.000000 angorapy-0.9.0/angorapy/models/__init__.py
--rw-rw-r--   0 weidler   (1000) weidler   (1000)     1265 2023-02-24 12:57:38.000000 angorapy-0.9.0/angorapy/models/components.py
--rw-rw-r--   0 weidler   (1000) weidler   (1000)    11391 2023-03-24 15:56:01.000000 angorapy-0.9.0/angorapy/models/convolutional.py
--rw-rw-r--   0 weidler   (1000) weidler   (1000)     2213 2023-03-16 13:23:20.000000 angorapy-0.9.0/angorapy/models/mighty_maker.py
--rw-rw-r--   0 weidler   (1000) weidler   (1000)    11241 2023-03-25 16:08:18.000000 angorapy-0.9.0/angorapy/models/shadow.py
--rw-rw-r--   0 weidler   (1000) weidler   (1000)    11358 2023-03-25 13:17:09.000000 angorapy-0.9.0/angorapy/models/shadow_v2.py
--rw-rw-r--   0 weidler   (1000) weidler   (1000)    11833 2023-02-24 12:57:38.000000 angorapy-0.9.0/angorapy/models/simple.py
-drwxrwxr-x   0 weidler   (1000) weidler   (1000)        0 2023-03-25 16:32:09.616537 angorapy-0.9.0/angorapy/monitor/
--rw-rw-r--   0 weidler   (1000) weidler   (1000)      130 2022-11-04 09:11:45.000000 angorapy-0.9.0/angorapy/monitor/__init__.py
--rw-rw-r--   0 weidler   (1000) weidler   (1000)    23641 2023-03-20 09:21:51.000000 angorapy-0.9.0/angorapy/monitor/app.py
--rw-rw-r--   0 weidler   (1000) weidler   (1000)     3668 2023-03-22 11:38:39.000000 angorapy-0.9.0/angorapy/observe.py
--rw-rw-r--   0 weidler   (1000) weidler   (1000)     5873 2023-03-24 18:10:40.000000 angorapy-0.9.0/angorapy/pretrain.py
--rw-rw-r--   0 weidler   (1000) weidler   (1000)    13693 2023-03-20 13:17:31.000000 angorapy-0.9.0/angorapy/train.py
-drwxrwxr-x   0 weidler   (1000) weidler   (1000)        0 2023-03-25 16:32:09.620537 angorapy-0.9.0/angorapy/utilities/
--rw-rw-r--   0 weidler   (1000) weidler   (1000)        0 2022-07-01 11:57:02.000000 angorapy-0.9.0/angorapy/utilities/__init__.py
--rw-rw-r--   0 weidler   (1000) weidler   (1000)     6579 2023-03-24 15:39:11.000000 angorapy-0.9.0/angorapy/utilities/data_generation.py
--rw-rw-r--   0 weidler   (1000) weidler   (1000)     2032 2023-02-24 12:57:38.000000 angorapy-0.9.0/angorapy/utilities/datatypes.py
--rw-rw-r--   0 weidler   (1000) weidler   (1000)      653 2022-07-01 11:57:02.000000 angorapy-0.9.0/angorapy/utilities/defaults.py
--rw-rw-r--   0 weidler   (1000) weidler   (1000)      169 2023-02-24 12:57:38.000000 angorapy-0.9.0/angorapy/utilities/dtypes.py
--rw-rw-r--   0 weidler   (1000) weidler   (1000)      445 2023-02-24 12:57:38.000000 angorapy-0.9.0/angorapy/utilities/error.py
--rw-rw-r--   0 weidler   (1000) weidler   (1000)     1303 2023-02-24 12:57:45.000000 angorapy-0.9.0/angorapy/utilities/hooks.py
--rw-rw-r--   0 weidler   (1000) weidler   (1000)     8897 2023-03-25 13:21:31.000000 angorapy-0.9.0/angorapy/utilities/model_utils.py
-drwxrwxr-x   0 weidler   (1000) weidler   (1000)        0 2023-03-25 16:32:09.620537 angorapy-0.9.0/angorapy/utilities/monitor/
--rw-rw-r--   0 weidler   (1000) weidler   (1000)        0 2022-07-01 11:57:02.000000 angorapy-0.9.0/angorapy/utilities/monitor/__init__.py
--rw-rw-r--   0 weidler   (1000) weidler   (1000)      968 2022-07-01 11:57:02.000000 angorapy-0.9.0/angorapy/utilities/monitor/plotting_base.py
--rw-rw-r--   0 weidler   (1000) weidler   (1000)     3371 2023-02-24 12:57:38.000000 angorapy-0.9.0/angorapy/utilities/monitor/statistical_plots.py
--rw-rw-r--   0 weidler   (1000) weidler   (1000)    20509 2023-02-24 12:57:38.000000 angorapy-0.9.0/angorapy/utilities/monitor/training_plots.py
--rw-rw-r--   0 weidler   (1000) weidler   (1000)     9504 2023-02-24 12:57:38.000000 angorapy-0.9.0/angorapy/utilities/monitoring.py
--rw-rw-r--   0 weidler   (1000) weidler   (1000)     4052 2022-07-01 11:57:02.000000 angorapy-0.9.0/angorapy/utilities/plotting.py
--rw-rw-r--   0 weidler   (1000) weidler   (1000)     1592 2022-07-01 11:57:02.000000 angorapy-0.9.0/angorapy/utilities/statistics.py
--rw-rw-r--   0 weidler   (1000) weidler   (1000)     9298 2023-03-25 11:08:17.000000 angorapy-0.9.0/angorapy/utilities/util.py
-drwxrwxr-x   0 weidler   (1000) weidler   (1000)        0 2023-03-25 16:32:09.608537 angorapy-0.9.0/angorapy.egg-info/
--rw-rw-r--   0 weidler   (1000) weidler   (1000)     8379 2023-03-25 16:32:09.000000 angorapy-0.9.0/angorapy.egg-info/PKG-INFO
--rw-rw-r--   0 weidler   (1000) weidler   (1000)     5928 2023-03-25 16:32:09.000000 angorapy-0.9.0/angorapy.egg-info/SOURCES.txt
--rw-rw-r--   0 weidler   (1000) weidler   (1000)        1 2023-03-25 16:32:09.000000 angorapy-0.9.0/angorapy.egg-info/dependency_links.txt
--rw-rw-r--   0 weidler   (1000) weidler   (1000)      387 2023-03-25 16:32:09.000000 angorapy-0.9.0/angorapy.egg-info/requires.txt
--rw-rw-r--   0 weidler   (1000) weidler   (1000)       15 2023-03-25 16:32:09.000000 angorapy-0.9.0/angorapy.egg-info/top_level.txt
--rw-rw-r--   0 weidler   (1000) weidler   (1000)       38 2023-03-25 16:32:09.620537 angorapy-0.9.0/setup.cfg
--rw-rw-r--   0 weidler   (1000) weidler   (1000)     1962 2023-03-25 16:28:06.000000 angorapy-0.9.0/setup.py
-drwxrwxr-x   0 weidler   (1000) weidler   (1000)        0 2023-03-25 16:32:09.620537 angorapy-0.9.0/tests/
--rw-rw-r--   0 weidler   (1000) weidler   (1000)        0 2020-12-04 16:52:46.000000 angorapy-0.9.0/tests/__init__.py
--rw-rw-r--   0 weidler   (1000) weidler   (1000)     1614 2023-03-20 13:31:40.000000 angorapy-0.9.0/tests/mpimemory.py
--rw-rw-r--   0 weidler   (1000) weidler   (1000)      437 2023-03-20 13:24:28.000000 angorapy-0.9.0/tests/numpy_optim.py
--rw-rw-r--   0 weidler   (1000) weidler   (1000)     4789 2023-02-24 12:57:45.000000 angorapy-0.9.0/tests/test_agent.py
--rw-rw-r--   0 weidler   (1000) weidler   (1000)     5351 2023-02-24 12:57:38.000000 angorapy-0.9.0/tests/test_distributions.py
--rw-rw-r--   0 weidler   (1000) weidler   (1000)     5204 2023-02-24 12:57:38.000000 angorapy-0.9.0/tests/test_environments.py
--rw-rw-r--   0 weidler   (1000) weidler   (1000)     2208 2023-02-24 12:57:38.000000 angorapy-0.9.0/tests/test_model_utils.py
--rw-rw-r--   0 weidler   (1000) weidler   (1000)      741 2022-07-01 11:57:02.000000 angorapy-0.9.0/tests/test_statistics.py
--rw-rw-r--   0 weidler   (1000) weidler   (1000)     1915 2023-02-24 12:57:45.000000 angorapy-0.9.0/tests/tete.py
+drwxrwxr-x   0 weidler   (1000) weidler   (1000)        0 2023-05-22 11:50:38.070226 angorapy-0.9.1/
+-rw-rw-r--   0 weidler   (1000) weidler   (1000)    34502 2020-12-04 16:52:46.000000 angorapy-0.9.1/LICENSE
+-rw-rw-r--   0 weidler   (1000) weidler   (1000)     9590 2023-05-22 11:50:38.070226 angorapy-0.9.1/PKG-INFO
+-rw-rw-r--   0 weidler   (1000) weidler   (1000)     8790 2023-05-22 11:50:16.000000 angorapy-0.9.1/README.md
+drwxrwxr-x   0 weidler   (1000) weidler   (1000)        0 2023-05-22 11:50:38.058226 angorapy-0.9.1/angorapy/
+-rw-rw-r--   0 weidler   (1000) weidler   (1000)      398 2023-05-22 11:24:36.000000 angorapy-0.9.1/angorapy/__init__.py
+drwxrwxr-x   0 weidler   (1000) weidler   (1000)        0 2023-05-22 11:50:38.058226 angorapy-0.9.1/angorapy/agent/
+-rw-rw-r--   0 weidler   (1000) weidler   (1000)      125 2022-07-01 11:57:01.000000 angorapy-0.9.1/angorapy/agent/__init__.py
+-rw-rw-r--   0 weidler   (1000) weidler   (1000)     4583 2022-07-01 11:57:02.000000 angorapy-0.9.1/angorapy/agent/core.py
+-rw-rw-r--   0 weidler   (1000) weidler   (1000)     6243 2023-03-25 16:33:57.000000 angorapy-0.9.1/angorapy/agent/dataio.py
+-rw-rw-r--   0 weidler   (1000) weidler   (1000)    15141 2023-03-25 16:33:57.000000 angorapy-0.9.1/angorapy/agent/gather.py
+drwxrwxr-x   0 weidler   (1000) weidler   (1000)        0 2023-05-22 11:50:38.058226 angorapy-0.9.1/angorapy/agent/ppo/
+-rw-rw-r--   0 weidler   (1000) weidler   (1000)        0 2022-07-01 11:57:01.000000 angorapy-0.9.1/angorapy/agent/ppo/__init__.py
+-rw-rw-r--   0 weidler   (1000) weidler   (1000)     4347 2023-03-25 16:33:57.000000 angorapy-0.9.1/angorapy/agent/ppo/loss.py
+-rw-rw-r--   0 weidler   (1000) weidler   (1000)     4637 2023-03-25 16:33:57.000000 angorapy-0.9.1/angorapy/agent/ppo/optim.py
+-rw-rw-r--   0 weidler   (1000) weidler   (1000)    57556 2023-05-22 11:24:36.000000 angorapy-0.9.1/angorapy/agent/ppo_agent.py
+drwxrwxr-x   0 weidler   (1000) weidler   (1000)        0 2023-05-22 11:50:38.058226 angorapy-0.9.1/angorapy/analysis/
+-rw-rw-r--   0 weidler   (1000) weidler   (1000)       74 2023-03-25 16:33:57.000000 angorapy-0.9.1/angorapy/analysis/__init__.py
+-rw-rw-r--   0 weidler   (1000) weidler   (1000)    12821 2022-11-04 09:11:45.000000 angorapy-0.9.1/angorapy/analysis/chiefinvestigation.py
+-rw-rw-r--   0 weidler   (1000) weidler   (1000)      817 2023-03-25 16:33:57.000000 angorapy-0.9.1/angorapy/analysis/dynamics.py
+-rw-rw-r--   0 weidler   (1000) weidler   (1000)      426 2023-03-25 16:33:57.000000 angorapy-0.9.1/angorapy/analysis/inspect_camera.py
+drwxrwxr-x   0 weidler   (1000) weidler   (1000)        0 2023-05-22 11:50:38.058226 angorapy-0.9.1/angorapy/analysis/investigators/
+-rw-rw-r--   0 weidler   (1000) weidler   (1000)      297 2023-03-25 16:33:57.000000 angorapy-0.9.1/angorapy/analysis/investigators/__init__.py
+-rw-rw-r--   0 weidler   (1000) weidler   (1000)    11196 2023-03-25 16:33:57.000000 angorapy-0.9.1/angorapy/analysis/investigators/base_investigator.py
+-rw-rw-r--   0 weidler   (1000) weidler   (1000)     1398 2023-03-25 16:33:57.000000 angorapy-0.9.1/angorapy/analysis/investigators/correlation.py
+-rw-rw-r--   0 weidler   (1000) weidler   (1000)     5217 2023-03-25 16:33:57.000000 angorapy-0.9.1/angorapy/analysis/investigators/dynamics.py
+-rw-rw-r--   0 weidler   (1000) weidler   (1000)     7134 2023-05-22 11:24:36.000000 angorapy-0.9.1/angorapy/analysis/investigators/predictability.py
+-rw-rw-r--   0 weidler   (1000) weidler   (1000)      738 2023-03-25 16:33:57.000000 angorapy-0.9.1/angorapy/analysis/plot_predictability.py
+-rw-rw-r--   0 weidler   (1000) weidler   (1000)     1282 2023-03-25 16:33:57.000000 angorapy-0.9.1/angorapy/analysis/plot_predictability_grouped.py
+-rw-rw-r--   0 weidler   (1000) weidler   (1000)     1596 2023-05-22 11:24:36.000000 angorapy-0.9.1/angorapy/analysis/plot_predictability_grouped_with_error_bars.py
+-rw-rw-r--   0 weidler   (1000) weidler   (1000)     1608 2023-05-22 11:24:36.000000 angorapy-0.9.1/angorapy/analysis/plot_predictability_with_error_bars.py
+-rw-rw-r--   0 weidler   (1000) weidler   (1000)     1973 2023-05-22 11:24:36.000000 angorapy-0.9.1/angorapy/analysis/plot_predictability_with_error_bars_single_figure.py
+-rw-rw-r--   0 weidler   (1000) weidler   (1000)     2625 2022-07-01 11:57:02.000000 angorapy-0.9.1/angorapy/analysis/plot_utils.py
+drwxrwxr-x   0 weidler   (1000) weidler   (1000)        0 2023-05-22 11:50:38.058226 angorapy-0.9.1/angorapy/analysis/plotting/
+-rw-rw-r--   0 weidler   (1000) weidler   (1000)        0 2022-07-01 11:57:01.000000 angorapy-0.9.1/angorapy/analysis/plotting/__init__.py
+-rw-rw-r--   0 weidler   (1000) weidler   (1000)     5798 2023-03-25 16:33:57.000000 angorapy-0.9.1/angorapy/analysis/plotting/autocorrelation_combined_plot.py
+-rw-rw-r--   0 weidler   (1000) weidler   (1000)      865 2022-07-01 11:57:02.000000 angorapy-0.9.1/angorapy/analysis/plotting/make_viz_featuremax.py
+-rw-rw-r--   0 weidler   (1000) weidler   (1000)     2059 2022-07-01 11:57:02.000000 angorapy-0.9.1/angorapy/analysis/plotting/make_viz_pretraining_fmap.py
+-rw-rw-r--   0 weidler   (1000) weidler   (1000)     1452 2022-07-01 11:57:02.000000 angorapy-0.9.1/angorapy/analysis/plotting/make_viz_pretraining_saliency.py
+-rw-rw-r--   0 weidler   (1000) weidler   (1000)     2269 2022-07-01 11:57:02.000000 angorapy-0.9.1/angorapy/analysis/plotting/plot_benchmark.py
+-rw-rw-r--   0 weidler   (1000) weidler   (1000)     3879 2023-02-24 12:57:38.000000 angorapy-0.9.1/angorapy/analysis/plotting/plot_benchmark_groups.py
+-rw-rw-r--   0 weidler   (1000) weidler   (1000)     5484 2023-05-18 12:29:38.000000 angorapy-0.9.1/angorapy/analysis/plotting/plot_benchmark_groups_with_beta.py
+-rw-rw-r--   0 weidler   (1000) weidler   (1000)     1316 2023-03-25 16:33:57.000000 angorapy-0.9.1/angorapy/analysis/plotting/plot_distributed_computation_benchmark.py
+-rw-rw-r--   0 weidler   (1000) weidler   (1000)      665 2022-07-01 11:57:02.000000 angorapy-0.9.1/angorapy/analysis/plotting/plot_experiment_best_evaluation.py
+-rw-rw-r--   0 weidler   (1000) weidler   (1000)     1043 2023-03-25 16:33:57.000000 angorapy-0.9.1/angorapy/analysis/plotting/plot_experiment_comparison.py
+-rw-rw-r--   0 weidler   (1000) weidler   (1000)     5791 2023-05-22 11:24:36.000000 angorapy-0.9.1/angorapy/analysis/plotting/plot_experiment_comparison_only_success_multiple_runs.py
+-rw-rw-r--   0 weidler   (1000) weidler   (1000)     4796 2023-05-18 12:29:38.000000 angorapy-0.9.1/angorapy/analysis/plotting/plot_experiment_comparison_only_success_multiple_runs_line_scatter.py
+-rw-rw-r--   0 weidler   (1000) weidler   (1000)     5109 2023-03-25 16:33:57.000000 angorapy-0.9.1/angorapy/analysis/plotting/plot_experiment_comparison_only_success_multiple_runs_with_zoom.py
+-rw-rw-r--   0 weidler   (1000) weidler   (1000)     2601 2023-03-25 16:33:57.000000 angorapy-0.9.1/angorapy/analysis/plotting/plot_experiment_comparison_with_success.py
+-rw-rw-r--   0 weidler   (1000) weidler   (1000)     6481 2023-05-18 12:29:38.000000 angorapy-0.9.1/angorapy/analysis/plotting/plot_experiment_comparison_with_success_multiple_runs.py
+-rw-rw-r--   0 weidler   (1000) weidler   (1000)     2289 2023-01-18 14:21:44.000000 angorapy-0.9.1/angorapy/analysis/plotting/plot_experiment_progression.py
+-rw-rw-r--   0 weidler   (1000) weidler   (1000)     1446 2022-07-01 11:57:02.000000 angorapy-0.9.1/angorapy/analysis/plotting/plot_losses.py
+-rw-rw-r--   0 weidler   (1000) weidler   (1000)     4331 2023-05-22 11:24:36.000000 angorapy-0.9.1/angorapy/analysis/predictability.py
+drwxrwxr-x   0 weidler   (1000) weidler   (1000)        0 2023-05-22 11:50:38.062226 angorapy-0.9.1/angorapy/analysis/sindy/
+-rw-rw-r--   0 weidler   (1000) weidler   (1000)        0 2023-03-25 16:33:57.000000 angorapy-0.9.1/angorapy/analysis/sindy/__init__.py
+-rw-rw-r--   0 weidler   (1000) weidler   (1000)     1910 2023-03-25 16:33:57.000000 angorapy-0.9.1/angorapy/analysis/sindy/autoencoder.py
+-rw-rw-r--   0 weidler   (1000) weidler   (1000)      286 2023-03-25 16:33:57.000000 angorapy-0.9.1/angorapy/analysis/sindy/loss.py
+drwxrwxr-x   0 weidler   (1000) weidler   (1000)        0 2023-05-22 11:50:38.062226 angorapy-0.9.1/angorapy/analysis/util/
+-rw-rw-r--   0 weidler   (1000) weidler   (1000)        0 2023-03-25 16:33:57.000000 angorapy-0.9.1/angorapy/analysis/util/__init__.py
+-rw-rw-r--   0 weidler   (1000) weidler   (1000)     9175 2023-03-25 16:33:57.000000 angorapy-0.9.1/angorapy/analysis/util/sindy.py
+-rw-rw-r--   0 weidler   (1000) weidler   (1000)    17221 2022-07-01 11:57:02.000000 angorapy-0.9.1/angorapy/analysis/visualization.py
+-rw-rw-r--   0 weidler   (1000) weidler   (1000)     5073 2022-07-01 11:57:02.000000 angorapy-0.9.1/angorapy/benchmark.py
+drwxrwxr-x   0 weidler   (1000) weidler   (1000)        0 2023-05-22 11:50:38.062226 angorapy-0.9.1/angorapy/common/
+-rw-rw-r--   0 weidler   (1000) weidler   (1000)        0 2022-07-01 11:57:01.000000 angorapy-0.9.1/angorapy/common/__init__.py
+-rw-rw-r--   0 weidler   (1000) weidler   (1000)     2398 2023-03-25 16:33:57.000000 angorapy-0.9.1/angorapy/common/activations.py
+-rw-rw-r--   0 weidler   (1000) weidler   (1000)     1369 2023-03-25 16:33:57.000000 angorapy-0.9.1/angorapy/common/const.py
+-rw-rw-r--   0 weidler   (1000) weidler   (1000)     8123 2023-03-25 16:33:57.000000 angorapy-0.9.1/angorapy/common/data_buffers.py
+-rw-rw-r--   0 weidler   (1000) weidler   (1000)     1610 2023-03-13 17:47:00.000000 angorapy-0.9.1/angorapy/common/layers.py
+-rw-rw-r--   0 weidler   (1000) weidler   (1000)     1350 2022-07-01 11:57:02.000000 angorapy-0.9.1/angorapy/common/loss.py
+-rw-rw-r--   0 weidler   (1000) weidler   (1000)     3073 2023-03-25 16:33:57.000000 angorapy-0.9.1/angorapy/common/mpi_optim.py
+-rw-rw-r--   0 weidler   (1000) weidler   (1000)    25984 2023-03-25 16:33:57.000000 angorapy-0.9.1/angorapy/common/policies.py
+-rw-rw-r--   0 weidler   (1000) weidler   (1000)     6261 2023-02-24 12:57:38.000000 angorapy-0.9.1/angorapy/common/reward.py
+-rw-rw-r--   0 weidler   (1000) weidler   (1000)     7840 2023-03-25 16:33:57.000000 angorapy-0.9.1/angorapy/common/senses.py
+-rw-rw-r--   0 weidler   (1000) weidler   (1000)    11433 2023-03-25 16:33:57.000000 angorapy-0.9.1/angorapy/common/transformers.py
+-rw-rw-r--   0 weidler   (1000) weidler   (1000)     6028 2023-03-25 16:33:57.000000 angorapy-0.9.1/angorapy/common/wrappers.py
+drwxrwxr-x   0 weidler   (1000) weidler   (1000)        0 2023-05-22 11:50:38.062226 angorapy-0.9.1/angorapy/configs/
+-rw-rw-r--   0 weidler   (1000) weidler   (1000)        0 2022-07-01 11:57:01.000000 angorapy-0.9.1/angorapy/configs/__init__.py
+-rw-rw-r--   0 weidler   (1000) weidler   (1000)     8258 2023-03-25 16:33:57.000000 angorapy-0.9.1/angorapy/configs/hp_config.py
+-rw-rw-r--   0 weidler   (1000) weidler   (1000)     2251 2022-07-01 11:57:02.000000 angorapy-0.9.1/angorapy/configs/reward_config.py
+drwxrwxr-x   0 weidler   (1000) weidler   (1000)        0 2023-05-22 11:50:38.062226 angorapy-0.9.1/angorapy/environments/
+-rw-rw-r--   0 weidler   (1000) weidler   (1000)    11768 2023-03-25 16:33:57.000000 angorapy-0.9.1/angorapy/environments/__init__.py
+-rw-rw-r--   0 weidler   (1000) weidler   (1000)     2082 2022-07-01 12:01:11.000000 angorapy-0.9.1/angorapy/environments/adapted.py
+-rw-rw-r--   0 weidler   (1000) weidler   (1000)    11177 2023-05-22 11:24:36.000000 angorapy-0.9.1/angorapy/environments/anthrobotics.py
+drwxrwxr-x   0 weidler   (1000) weidler   (1000)        0 2023-05-22 11:50:38.062226 angorapy-0.9.1/angorapy/environments/assets/
+-rw-rw-r--   0 weidler   (1000) weidler   (1000)    12706 2022-07-01 12:01:11.000000 angorapy-0.9.1/angorapy/environments/assets/LICENSE.md
+drwxrwxr-x   0 weidler   (1000) weidler   (1000)        0 2023-05-22 11:50:38.062226 angorapy-0.9.1/angorapy/environments/assets/hand/
+-rw-rw-r--   0 weidler   (1000) weidler   (1000)     2329 2022-07-01 12:00:59.000000 angorapy-0.9.1/angorapy/environments/assets/hand/manipulate_block.xml
+-rw-rw-r--   0 weidler   (1000) weidler   (1000)     2401 2022-07-01 12:00:59.000000 angorapy-0.9.1/angorapy/environments/assets/hand/manipulate_block_touch_sensors.xml
+-rw-rw-r--   0 weidler   (1000) weidler   (1000)     2326 2022-07-01 12:00:59.000000 angorapy-0.9.1/angorapy/environments/assets/hand/manipulate_egg.xml
+-rw-rw-r--   0 weidler   (1000) weidler   (1000)     2394 2022-07-01 12:00:59.000000 angorapy-0.9.1/angorapy/environments/assets/hand/manipulate_egg_touch_sensors.xml
+-rw-rw-r--   0 weidler   (1000) weidler   (1000)     2184 2022-07-01 12:00:59.000000 angorapy-0.9.1/angorapy/environments/assets/hand/manipulate_pen.xml
+-rw-rw-r--   0 weidler   (1000) weidler   (1000)     2252 2022-07-01 12:00:59.000000 angorapy-0.9.1/angorapy/environments/assets/hand/manipulate_pen_touch_sensors.xml
+-rw-rw-r--   0 weidler   (1000) weidler   (1000)    16788 2022-07-01 12:00:59.000000 angorapy-0.9.1/angorapy/environments/assets/hand/robot.xml
+-rw-rw-r--   0 weidler   (1000) weidler   (1000)    32115 2022-07-01 12:00:59.000000 angorapy-0.9.1/angorapy/environments/assets/hand/robot_touch_sensors_92.xml
+-rw-rw-r--   0 weidler   (1000) weidler   (1000)     2091 2023-02-24 12:57:38.000000 angorapy-0.9.1/angorapy/environments/assets/hand/shadowhand.xml
+-rw-rw-r--   0 weidler   (1000) weidler   (1000)     3389 2022-07-01 12:00:59.000000 angorapy-0.9.1/angorapy/environments/assets/hand/shadowhand_manipulate.xml
+-rw-rw-r--   0 weidler   (1000) weidler   (1000)    16537 2022-07-01 12:00:59.000000 angorapy-0.9.1/angorapy/environments/assets/hand/shared.xml
+-rw-rw-r--   0 weidler   (1000) weidler   (1000)     2052 2022-07-01 12:00:59.000000 angorapy-0.9.1/angorapy/environments/assets/hand/shared_asset.xml
+-rw-rw-r--   0 weidler   (1000) weidler   (1000)     9201 2022-07-01 12:00:59.000000 angorapy-0.9.1/angorapy/environments/assets/hand/shared_touch_sensors_92.xml
+-rw-rw-r--   0 weidler   (1000) weidler   (1000)    31885 2022-07-01 12:00:59.000000 angorapy-0.9.1/angorapy/environments/assets/hand/touch_sensors.xml
+drwxrwxr-x   0 weidler   (1000) weidler   (1000)        0 2023-05-22 11:50:38.054226 angorapy-0.9.1/angorapy/environments/assets/stls/
+drwxrwxr-x   0 weidler   (1000) weidler   (1000)        0 2023-05-22 11:50:38.066226 angorapy-0.9.1/angorapy/environments/assets/stls/hand/
+-rw-rw-r--   0 weidler   (1000) weidler   (1000)    17084 2022-07-01 12:01:11.000000 angorapy-0.9.1/angorapy/environments/assets/stls/hand/F1.stl
+-rw-rw-r--   0 weidler   (1000) weidler   (1000)    22884 2022-07-01 12:01:11.000000 angorapy-0.9.1/angorapy/environments/assets/stls/hand/F2.stl
+-rw-rw-r--   0 weidler   (1000) weidler   (1000)    54684 2022-07-01 12:01:11.000000 angorapy-0.9.1/angorapy/environments/assets/stls/hand/F3.stl
+-rw-rw-r--   0 weidler   (1000) weidler   (1000)     6334 2022-07-01 12:01:11.000000 angorapy-0.9.1/angorapy/environments/assets/stls/hand/TH1_z.stl
+-rw-rw-r--   0 weidler   (1000) weidler   (1000)    63184 2022-07-01 12:01:11.000000 angorapy-0.9.1/angorapy/environments/assets/stls/hand/TH2_z.stl
+-rw-rw-r--   0 weidler   (1000) weidler   (1000)    21184 2022-07-01 12:01:11.000000 angorapy-0.9.1/angorapy/environments/assets/stls/hand/TH3_z.stl
+-rw-rw-r--   0 weidler   (1000) weidler   (1000)   934534 2022-07-01 12:01:11.000000 angorapy-0.9.1/angorapy/environments/assets/stls/hand/forearm_electric.stl
+-rw-rw-r--   0 weidler   (1000) weidler   (1000)    45384 2022-07-01 12:01:11.000000 angorapy-0.9.1/angorapy/environments/assets/stls/hand/forearm_electric_cvx.stl
+-rw-rw-r--   0 weidler   (1000) weidler   (1000)    30184 2022-07-01 12:01:11.000000 angorapy-0.9.1/angorapy/environments/assets/stls/hand/knuckle.stl
+-rw-rw-r--   0 weidler   (1000) weidler   (1000)    75084 2022-07-01 12:01:11.000000 angorapy-0.9.1/angorapy/environments/assets/stls/hand/lfmetacarpal.stl
+-rw-rw-r--   0 weidler   (1000) weidler   (1000)   347784 2022-07-01 12:01:11.000000 angorapy-0.9.1/angorapy/environments/assets/stls/hand/palm.stl
+-rw-rw-r--   0 weidler   (1000) weidler   (1000)    92784 2022-07-01 12:01:11.000000 angorapy-0.9.1/angorapy/environments/assets/stls/hand/wrist.stl
+drwxrwxr-x   0 weidler   (1000) weidler   (1000)        0 2023-05-22 11:50:38.066226 angorapy-0.9.1/angorapy/environments/assets/textures/
+-rw-rw-r--   0 weidler   (1000) weidler   (1000)    15879 2022-07-01 12:01:11.000000 angorapy-0.9.1/angorapy/environments/assets/textures/block.png
+-rw-rw-r--   0 weidler   (1000) weidler   (1000)    40953 2022-07-01 12:01:11.000000 angorapy-0.9.1/angorapy/environments/assets/textures/block_hidden.png
+drwxrwxr-x   0 weidler   (1000) weidler   (1000)        0 2023-05-22 11:50:38.066226 angorapy-0.9.1/angorapy/environments/hand/
+-rw-rw-r--   0 weidler   (1000) weidler   (1000)        0 2023-02-24 12:57:38.000000 angorapy-0.9.1/angorapy/environments/hand/__init__.py
+-rw-rw-r--   0 weidler   (1000) weidler   (1000)    24334 2023-03-25 16:33:57.000000 angorapy-0.9.1/angorapy/environments/hand/manipulate.py
+-rw-rw-r--   0 weidler   (1000) weidler   (1000)    17277 2023-03-25 16:33:57.000000 angorapy-0.9.1/angorapy/environments/hand/reach.py
+-rw-rw-r--   0 weidler   (1000) weidler   (1000)    13384 2023-05-22 11:24:36.000000 angorapy-0.9.1/angorapy/environments/hand/shadowhand.py
+-rw-rw-r--   0 weidler   (1000) weidler   (1000)      330 2022-09-14 11:48:13.000000 angorapy-0.9.1/angorapy/environments/hand/test.py
+-rw-rw-r--   0 weidler   (1000) weidler   (1000)     6574 2023-02-24 12:57:38.000000 angorapy-0.9.1/angorapy/environments/hanoi.py
+-rw-rw-r--   0 weidler   (1000) weidler   (1000)    13272 2023-03-25 16:33:57.000000 angorapy-0.9.1/angorapy/environments/rotations.py
+-rw-rw-r--   0 weidler   (1000) weidler   (1000)      478 2022-07-01 12:01:11.000000 angorapy-0.9.1/angorapy/environments/test.py
+-rw-rw-r--   0 weidler   (1000) weidler   (1000)     1043 2022-07-01 11:57:02.000000 angorapy-0.9.1/angorapy/environments/utils.py
+-rw-rw-r--   0 weidler   (1000) weidler   (1000)     3285 2023-05-18 12:29:38.000000 angorapy-0.9.1/angorapy/evaluate.py
+drwxrwxr-x   0 weidler   (1000) weidler   (1000)        0 2023-05-22 11:50:38.066226 angorapy-0.9.1/angorapy/models/
+-rw-rw-r--   0 weidler   (1000) weidler   (1000)     1338 2023-05-22 11:24:36.000000 angorapy-0.9.1/angorapy/models/__init__.py
+-rw-rw-r--   0 weidler   (1000) weidler   (1000)     1265 2023-02-24 12:57:38.000000 angorapy-0.9.1/angorapy/models/components.py
+-rw-rw-r--   0 weidler   (1000) weidler   (1000)    11391 2023-05-05 13:13:24.000000 angorapy-0.9.1/angorapy/models/convolutional.py
+-rw-rw-r--   0 weidler   (1000) weidler   (1000)     2213 2023-03-25 16:33:57.000000 angorapy-0.9.1/angorapy/models/mighty_maker.py
+-rw-rw-r--   0 weidler   (1000) weidler   (1000)    11241 2023-03-25 16:33:57.000000 angorapy-0.9.1/angorapy/models/shadow.py
+-rw-rw-r--   0 weidler   (1000) weidler   (1000)    11360 2023-05-22 11:24:36.000000 angorapy-0.9.1/angorapy/models/shadow_v2.py
+-rw-rw-r--   0 weidler   (1000) weidler   (1000)    11469 2023-05-22 11:24:36.000000 angorapy-0.9.1/angorapy/models/simple.py
+drwxrwxr-x   0 weidler   (1000) weidler   (1000)        0 2023-05-22 11:50:38.066226 angorapy-0.9.1/angorapy/monitor/
+-rw-rw-r--   0 weidler   (1000) weidler   (1000)      130 2022-11-04 09:11:45.000000 angorapy-0.9.1/angorapy/monitor/__init__.py
+-rw-rw-r--   0 weidler   (1000) weidler   (1000)    23668 2023-05-22 11:24:36.000000 angorapy-0.9.1/angorapy/monitor/app.py
+-rw-rw-r--   0 weidler   (1000) weidler   (1000)     3668 2023-03-25 16:33:57.000000 angorapy-0.9.1/angorapy/observe.py
+-rw-rw-r--   0 weidler   (1000) weidler   (1000)     5873 2023-05-18 12:29:38.000000 angorapy-0.9.1/angorapy/pretrain.py
+-rw-rw-r--   0 weidler   (1000) weidler   (1000)    13743 2023-05-22 11:24:36.000000 angorapy-0.9.1/angorapy/train.py
+drwxrwxr-x   0 weidler   (1000) weidler   (1000)        0 2023-05-22 11:50:38.070226 angorapy-0.9.1/angorapy/utilities/
+-rw-rw-r--   0 weidler   (1000) weidler   (1000)        0 2022-07-01 11:57:02.000000 angorapy-0.9.1/angorapy/utilities/__init__.py
+-rw-rw-r--   0 weidler   (1000) weidler   (1000)     6579 2023-05-18 12:29:38.000000 angorapy-0.9.1/angorapy/utilities/data_generation.py
+-rw-rw-r--   0 weidler   (1000) weidler   (1000)     2032 2023-03-25 16:33:57.000000 angorapy-0.9.1/angorapy/utilities/datatypes.py
+-rw-rw-r--   0 weidler   (1000) weidler   (1000)      653 2022-07-01 11:57:02.000000 angorapy-0.9.1/angorapy/utilities/defaults.py
+-rw-rw-r--   0 weidler   (1000) weidler   (1000)      169 2023-03-25 16:33:57.000000 angorapy-0.9.1/angorapy/utilities/dtypes.py
+-rw-rw-r--   0 weidler   (1000) weidler   (1000)      445 2023-03-25 16:33:57.000000 angorapy-0.9.1/angorapy/utilities/error.py
+-rw-rw-r--   0 weidler   (1000) weidler   (1000)     1303 2023-03-25 16:33:57.000000 angorapy-0.9.1/angorapy/utilities/hooks.py
+-rw-rw-r--   0 weidler   (1000) weidler   (1000)     9527 2023-05-22 11:24:36.000000 angorapy-0.9.1/angorapy/utilities/model_utils.py
+drwxrwxr-x   0 weidler   (1000) weidler   (1000)        0 2023-05-22 11:50:38.070226 angorapy-0.9.1/angorapy/utilities/monitor/
+-rw-rw-r--   0 weidler   (1000) weidler   (1000)        0 2022-07-01 11:57:02.000000 angorapy-0.9.1/angorapy/utilities/monitor/__init__.py
+-rw-rw-r--   0 weidler   (1000) weidler   (1000)      968 2022-07-01 11:57:02.000000 angorapy-0.9.1/angorapy/utilities/monitor/plotting_base.py
+-rw-rw-r--   0 weidler   (1000) weidler   (1000)     3371 2023-02-24 12:57:38.000000 angorapy-0.9.1/angorapy/utilities/monitor/statistical_plots.py
+-rw-rw-r--   0 weidler   (1000) weidler   (1000)    20509 2023-03-25 16:33:57.000000 angorapy-0.9.1/angorapy/utilities/monitor/training_plots.py
+-rw-rw-r--   0 weidler   (1000) weidler   (1000)     9504 2023-03-25 16:33:57.000000 angorapy-0.9.1/angorapy/utilities/monitoring.py
+-rw-rw-r--   0 weidler   (1000) weidler   (1000)     4052 2022-07-01 11:57:02.000000 angorapy-0.9.1/angorapy/utilities/plotting.py
+-rw-rw-r--   0 weidler   (1000) weidler   (1000)     1592 2022-07-01 11:57:02.000000 angorapy-0.9.1/angorapy/utilities/statistics.py
+-rw-rw-r--   0 weidler   (1000) weidler   (1000)     9298 2023-03-25 16:33:57.000000 angorapy-0.9.1/angorapy/utilities/util.py
+drwxrwxr-x   0 weidler   (1000) weidler   (1000)        0 2023-05-22 11:50:38.058226 angorapy-0.9.1/angorapy.egg-info/
+-rw-rw-r--   0 weidler   (1000) weidler   (1000)     9590 2023-05-22 11:50:38.000000 angorapy-0.9.1/angorapy.egg-info/PKG-INFO
+-rw-rw-r--   0 weidler   (1000) weidler   (1000)     5974 2023-05-22 11:50:38.000000 angorapy-0.9.1/angorapy.egg-info/SOURCES.txt
+-rw-rw-r--   0 weidler   (1000) weidler   (1000)        1 2023-05-22 11:50:38.000000 angorapy-0.9.1/angorapy.egg-info/dependency_links.txt
+-rw-rw-r--   0 weidler   (1000) weidler   (1000)      455 2023-05-22 11:50:38.000000 angorapy-0.9.1/angorapy.egg-info/requires.txt
+-rw-rw-r--   0 weidler   (1000) weidler   (1000)       15 2023-05-22 11:50:38.000000 angorapy-0.9.1/angorapy.egg-info/top_level.txt
+-rw-rw-r--   0 weidler   (1000) weidler   (1000)       38 2023-05-22 11:50:38.070226 angorapy-0.9.1/setup.cfg
+-rw-rw-r--   0 weidler   (1000) weidler   (1000)     2052 2023-05-22 11:24:36.000000 angorapy-0.9.1/setup.py
+drwxrwxr-x   0 weidler   (1000) weidler   (1000)        0 2023-05-22 11:50:38.070226 angorapy-0.9.1/tests/
+-rw-rw-r--   0 weidler   (1000) weidler   (1000)        0 2020-12-04 16:52:46.000000 angorapy-0.9.1/tests/__init__.py
+-rw-rw-r--   0 weidler   (1000) weidler   (1000)     4789 2023-03-25 16:33:57.000000 angorapy-0.9.1/tests/test_agent.py
+-rw-rw-r--   0 weidler   (1000) weidler   (1000)     2432 2023-05-22 11:24:36.000000 angorapy-0.9.1/tests/test_builtin_models.py
+-rw-rw-r--   0 weidler   (1000) weidler   (1000)     5351 2023-02-24 12:57:38.000000 angorapy-0.9.1/tests/test_distributions.py
+-rw-rw-r--   0 weidler   (1000) weidler   (1000)     5204 2023-03-25 16:33:57.000000 angorapy-0.9.1/tests/test_environments.py
+-rw-rw-r--   0 weidler   (1000) weidler   (1000)     2208 2023-02-24 12:57:38.000000 angorapy-0.9.1/tests/test_model_utils.py
+-rw-rw-r--   0 weidler   (1000) weidler   (1000)      741 2022-07-01 11:57:02.000000 angorapy-0.9.1/tests/test_statistics.py
```

### Comparing `angorapy-0.9.0/LICENSE` & `angorapy-0.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `angorapy-0.9.0/PKG-INFO` & `angorapy-0.9.1/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,27 +1,7 @@
-Metadata-Version: 2.1
-Name: angorapy
-Version: 0.9.0
-Summary: ANthropomorphic Goal-ORiented Modeling, Learning and Analysis for Neuroscience
-Home-page: https://github.com/ccnmaastricht/angorapy
-Author: Tonio Weidler
-Author-email: research@tonioweidler.de
-License: GPL-3.0
-Classifier: Development Status :: 3 - Alpha
-Classifier: Intended Audience :: Science/Research
-Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
-Classifier: Operating System :: POSIX :: Linux
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 ![](https://img.shields.io/pypi/pyversions/angorapy)
 ![](https://img.shields.io/pypi/v/angorapy)
 ![](https://img.shields.io/github/license/ccnmaastricht/angorapy)
 ![](https://img.shields.io/github/stars/ccnmaastricht/angorapy)
 
 
 <br />
@@ -38,28 +18,60 @@
 
 This library is developed as part of the [Human Brain Project](https://www.humanbrainproject.eu/) at [CCN Maastricht](https://www.ccnmaastricht.com/). It is an effort to build software by neuroscientists, for neuroscientists. If you have suggestions, requests or questions, feel free to [open an issue](https://github.com/ccnmaastricht/angorapy/issues/new/choose).
 
 ![Manipulation Gif](docs/gifs/manipulate_best.gif)
 
 ## 📥 Installation
 
-AngoraPy is available on PyPI. 
+### Prerequisites
+AngoraPy requires Python 3.6 or higher. It is recommended to use a virtual environment to install AngoraPy and its dependencies. Additionally, some prerequisites are required. 
 
-```bash
-pip install angorapy
-```
+On Ubuntu, these can be installed by running
 
-### From source
-Alternatively, you can download this repository or the source code of any previous release or branch and install from source, using pip.
+    sudo apt-get install swig
 
-```bash
-pip install -e .
-```
+Additionally, to run AngoraPy with its native distribution, you need MPI installed. On Ubuntu, this can be done by running
+
+    sudo apt-get install libopenmpi-dev
+
+However, any other MPI implementation should work as well.
+
+### Installing AngoraPy
+
+#### Binaries
+AngoraPy is available as a binary package on PyPI. To install it, run 
+
+    pip install angorapy
+
+in your terminal.
+
+If you would like to install a specific version, you can specify it by appending `==<version>` to the command above. For example, to install version 0.9.0, run 
 
-This way, if you make changes to the source code, these will be recognized in the installation (without the need to reinstall).
+    pip install angorapy==0.9.0
+
+#### Source Installation
+To install AngoraPy from source, clone the repository and run `pip install -e .` in the root directory.
+
+### Post-Installation
+
+#### MuJoCo
+Gym installs both MuJoCo's new native Python bindings and the old mujoco-py bindings. You will not need the latter for AngoraPy, so you may uninstall it by running
+
+    pip uninstall mujoco-py
+
+#### Test Your Installation
+You can test your installation by running the following command in your terminal:
+
+    python -m angorapy.train CartPole-v1
+
+To test your MPI installation, run
+
+    mpirun -np <numthreads> --use-hwthread-cpus python -m angorapy.train LunarLanderContinuous-v2
+
+where `<numthreads>` is the number of threads you want to (and can) use.
 
 ### Docker
 Alternatively, you can install AngoraPy and all its dependencies in a docker container using the Dockerfile provided in this repository (/docker/Dockerfile). To this end, download the repository and build the docker image from the /docker directory:
 
 ```bash
 sudo docker build -t angorapy:master https://github.com/ccnmaastricht/angorapy.git#master -f - < Dockerfile
 ```
@@ -96,32 +108,24 @@
 To train agents with custom models, environments, etc. you write your own script. The following is a minimal example:
 
 ```python
 from angorapy.common.wrappers import make_env
 from angorapy.models import get_model_builder
 from angorapy.agent.ppo_agent import PPOAgent
 
-env = make_env("LunarLanderContinuous-v2")
-model_builder = get_model_builder("simple", "ffn")
-agent = PPOAgent(model_builder, env)
-agent.drill(100, 10, 512)
+env = make_env("ReachAbsolute-v0")
+model_builder = get_model_builder("shadow", "lstm")
+agent = PPOAgent(model_builder, env, workers=24)
+agent.drill(n=100, epochs=10, batch_size=512)
 ```
 
 For more details, consult the [examples](examples).
 
 ## 🎓 Documentation
-Detailed documentation of AngoraPy is provided in the READMEs of most subpackages. Additionally, we provide [examples and tutorials](examples) that get you started with writing your own scripts using AngoraPy. For further readings on specific modules, consult the following READMEs: 
-
- - [Agent](angorapy/agent) [WIP]
- - [Environments](angorapy/environments)
- - [Models](angorapy/models)
- - [Analysis](angorapy/analysis)
- - [Monitoring](angorapy/monitoring)
-
-If you are missing a documentation for a specific part of AngoraPy, feel free to open an issue and we will do our best to add it.
+We provide [examples](examples) that get you started with writing your own scripts using AngoraPy. Additionally there is a growing list of [tutorials](https://github.com/weidler/angorapy-tutorials). If you are missing a documentation for a specific part of AngoraPy, feel free to open an issue and we will do our best to add it.
 
 ## 🔀 Distributed Computation
 PPO is an asynchronous algorithm, allowing multiple parallel workers to generate experience independently. 
 We allow parallel gathering and optimization through MPI. Agents will automatically distribute their workers evenly on 
 the available CPU cores, while optimization is distributed over all available GPUs. If no GPUs are available, all CPUs 
 share the task of optimizing.
 
@@ -170,17 +174,21 @@
 The number of parallel workers will equal the number of nodes times the number of CPUs per node 
 (32 x 12 = 384 in the template above).
 
 ## 🔗 Citing AngoraPy
 
 If you use AngoraPy for your research, please cite us as follows
 
-    Weidler, T., & Senden, M. (2020). AngoraPy: Anthropomorphic Goal-Oriented Robotic Control for Neuroscientific Modeling [Computer software]
+    Weidler, Tonio, & Senden, Mario. (2023). AngoraPy - Anthropomorphic Goal-Oriented Robotic Control for Neuroscientific Modeling (0.9.0). Zenodo. https://doi.org/10.5281/zenodo.7770180
 
 Or using bibtex
 
-    @software{angorapy2020,
-        author = {Weidler, Tonio and Senden, Mario},
-        month = {3},
-        title = {{AngoraPy: Anthropomorphic Goal-Oriented Robotic Control for Neuroscientific Modeling}},
-        year = {2020}
-    }
+    @software{weidler_angorapy_2023,
+        author       = {Weidler, Tonio and Senden, Mario},
+        title        = {{AngoraPy - Anthropomorphic Goal-Oriented Robotic 
+                         Control for Neuroscientific Modeling}},
+        year         = 2023,
+        publisher    = {Zenodo},
+        version      = {0.9.0},
+        doi          = {10.5281/zenodo.6636482},
+        url          = {https://doi.org/10.5281/zenodo.6636482}
+   }
```

### Comparing `angorapy-0.9.0/README.md` & `angorapy-0.9.1/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,474 +1,600 @@
-00000000: 215b 5d28 6874 7470 733a 2f2f 696d 672e  ![](https://img.
-00000010: 7368 6965 6c64 732e 696f 2f70 7970 692f  shields.io/pypi/
-00000020: 7079 7665 7273 696f 6e73 2f61 6e67 6f72  pyversions/angor
-00000030: 6170 7929 0a21 5b5d 2868 7474 7073 3a2f  apy).![](https:/
-00000040: 2f69 6d67 2e73 6869 656c 6473 2e69 6f2f  /img.shields.io/
-00000050: 7079 7069 2f76 2f61 6e67 6f72 6170 7929  pypi/v/angorapy)
-00000060: 0a21 5b5d 2868 7474 7073 3a2f 2f69 6d67  .![](https://img
-00000070: 2e73 6869 656c 6473 2e69 6f2f 6769 7468  .shields.io/gith
-00000080: 7562 2f6c 6963 656e 7365 2f63 636e 6d61  ub/license/ccnma
-00000090: 6173 7472 6963 6874 2f61 6e67 6f72 6170  astricht/angorap
-000000a0: 7929 0a21 5b5d 2868 7474 7073 3a2f 2f69  y).![](https://i
-000000b0: 6d67 2e73 6869 656c 6473 2e69 6f2f 6769  mg.shields.io/gi
-000000c0: 7468 7562 2f73 7461 7273 2f63 636e 6d61  thub/stars/ccnma
-000000d0: 6173 7472 6963 6874 2f61 6e67 6f72 6170  astricht/angorap
-000000e0: 7929 0a0a 0a3c 6272 202f 3e0a 3c62 7220  y)...<br />.<br 
-000000f0: 2f3e 0a0a 3c70 2061 6c69 676e 3d22 6365  />..<p align="ce
-00000100: 6e74 6572 223e 3c69 6d67 2073 7263 3d22  nter"><img src="
-00000110: 646f 6373 2f69 6d67 2f61 6e67 6f72 6170  docs/img/angorap
-00000120: 792e 7376 6722 2077 6964 7468 3d32 3525  y.svg" width=25%
-00000130: 2061 6c69 676e 3d22 6365 6e74 6572 2220   align="center" 
-00000140: 2f3e 3c2f 703e 0a3c 6833 3e20 3c70 2061  /></p>.<h3> <p a
-00000150: 6c69 676e 3d22 6365 6e74 6572 223e 2041  lign="center"> A
-00000160: 6e74 6872 6f70 6f6d 6f72 7068 6963 2047  nthropomorphic G
-00000170: 6f61 6c2d 4f72 6965 6e74 6564 2052 6f62  oal-Oriented Rob
-00000180: 6f74 6963 2043 6f6e 7472 6f6c 2066 6f72  otic Control for
-00000190: 204e 6575 726f 7363 6965 6e74 6966 6963   Neuroscientific
-000001a0: 204d 6f64 656c 696e 6720 3c2f 703e 203c   Modeling </p> <
-000001b0: 2f68 333e 0a0a 3c62 7220 2f3e 0a20 2020  /h3>..<br />.   
-000001c0: 0a2a 2a41 6e67 6f72 6150 792a 2a20 6973  .**AngoraPy** is
-000001d0: 2061 6e20 6f70 656e 2073 6f75 7263 6520   an open source 
-000001e0: 6d6f 6465 6c69 6e67 206c 6962 7261 7279  modeling library
-000001f0: 2066 6f72 205b 676f 616c 2d6f 7269 656e   for [goal-orien
-00000200: 7465 6420 7265 7365 6172 6368 5d28 6874  ted research](ht
-00000210: 7470 733a 2f2f 7075 626d 6564 2e6e 6362  tps://pubmed.ncb
-00000220: 692e 6e6c 6d2e 6e69 682e 676f 762f 3236  i.nlm.nih.gov/26
-00000230: 3930 3635 3032 2f29 2069 6e20 2a2a 6e65  906502/) in **ne
-00000240: 7572 6f73 6369 656e 6365 2a2a 2e20 4974  uroscience**. It
-00000250: 2070 726f 7669 6465 7320 6120 7369 6d70   provides a simp
-00000260: 6c65 2069 6e74 6572 6661 6365 2074 6f20  le interface to 
-00000270: 7472 6169 6e20 6465 6570 206e 6575 7261  train deep neura
-00000280: 6c20 6e65 7477 6f72 6b20 6d6f 6465 6c73  l network models
-00000290: 206f 6620 7468 6520 6875 6d61 6e20 6272   of the human br
-000002a0: 6169 6e20 6f6e 2076 6172 696f 7573 2c20  ain on various, 
-000002b0: 6375 7374 6f6d 697a 6162 6c65 2c20 7365  customizable, se
-000002c0: 6e73 6f72 696d 6f74 6f72 2074 6173 6b73  nsorimotor tasks
-000002d0: 2c20 7573 696e 6720 7265 696e 666f 7263  , using reinforc
-000002e0: 656d 656e 7420 6c65 6172 6e69 6e67 2e20  ement learning. 
-000002f0: 4974 2074 6865 7265 6279 2065 6d70 6f77  It thereby empow
-00000300: 6572 7320 676f 616c 2d64 7269 7665 6e20  ers goal-driven 
-00000310: 6d6f 6465 6c69 6e67 2074 6f20 7375 7270  modeling to surp
-00000320: 6173 7320 7468 6520 7365 6e73 6f72 7920  ass the sensory 
-00000330: 646f 6d61 696e 2061 6e64 2065 6e74 6572  domain and enter
-00000340: 2074 6861 7420 6f66 2073 656e 736f 7269   that of sensori
-00000350: 5f6d 6f74 6f72 5f20 636f 6e74 726f 6c2c  _motor_ control,
-00000360: 2063 6c6f 7369 6e67 2074 6865 2070 6572   closing the per
-00000370: 6365 7074 696f 6e2d 6163 7469 6f6e 206c  ception-action l
-00000380: 6f6f 702e 200a 0a2a 2a41 6e67 6f72 6150  oop. ..**AngoraP
-00000390: 792a 2a20 6973 2064 6573 6967 6e65 6420  y** is designed 
-000003a0: 746f 2072 6571 7569 7265 206e 6f20 6465  to require no de
-000003b0: 6570 6572 2075 6e64 6572 7374 616e 6469  eper understandi
-000003c0: 6e67 206f 6620 7265 696e 666f 7263 656d  ng of reinforcem
-000003d0: 656e 7420 6c65 6172 6e69 6e67 2e20 4974  ent learning. It
-000003e0: 2065 6d70 6c6f 7973 2073 7461 7465 2d6f   employs state-o
-000003f0: 662d 7468 652d 6172 7420 6d61 6368 696e  f-the-art machin
-00000400: 6520 6c65 6172 6e69 6e67 2074 6563 686e  e learning techn
-00000410: 6971 7565 732c 206f 7074 696d 697a 6564  iques, optimized
-00000420: 2066 6f72 2064 6973 7472 6962 7574 6564   for distributed
-00000430: 2063 6f6d 7075 7461 7469 6f6e 2073 6361   computation sca
-00000440: 6c69 6e67 2066 726f 6d20 6c6f 6361 6c20  ling from local 
-00000450: 776f 726b 7374 6174 696f 6e73 2074 6f20  workstations to 
-00000460: 6869 6768 2d70 6572 666f 726d 616e 6365  high-performance
-00000470: 2063 6f6d 7075 7469 6e67 2063 6c75 7374   computing clust
-00000480: 6572 732e 2057 6520 6169 6d20 746f 2068  ers. We aim to h
-00000490: 6964 6520 6173 206d 7563 6820 6f66 2074  ide as much of t
-000004a0: 6869 7320 756e 6465 7220 7468 6520 686f  his under the ho
-000004b0: 6f64 206f 6620 616e 2069 6e74 7569 7469  od of an intuiti
-000004c0: 7665 2c20 6869 6768 2d6c 6576 656c 2041  ve, high-level A
-000004d0: 5049 2062 7574 2070 7265 7365 7276 6520  PI but preserve 
-000004e0: 7468 6520 6f70 7469 6f6e 2066 6f72 2063  the option for c
-000004f0: 7573 746f 6d69 7a69 6e67 206d 6f73 7420  ustomizing most 
-00000500: 6173 7065 6374 7320 6f66 2074 6865 2070  aspects of the p
-00000510: 6970 656c 696e 652e 0a0a 5468 6973 206c  ipeline...This l
-00000520: 6962 7261 7279 2069 7320 6465 7665 6c6f  ibrary is develo
-00000530: 7065 6420 6173 2070 6172 7420 6f66 2074  ped as part of t
-00000540: 6865 205b 4875 6d61 6e20 4272 6169 6e20  he [Human Brain 
-00000550: 5072 6f6a 6563 745d 2868 7474 7073 3a2f  Project](https:/
-00000560: 2f77 7777 2e68 756d 616e 6272 6169 6e70  /www.humanbrainp
-00000570: 726f 6a65 6374 2e65 752f 2920 6174 205b  roject.eu/) at [
-00000580: 4343 4e20 4d61 6173 7472 6963 6874 5d28  CCN Maastricht](
-00000590: 6874 7470 733a 2f2f 7777 772e 6363 6e6d  https://www.ccnm
-000005a0: 6161 7374 7269 6368 742e 636f 6d2f 292e  aastricht.com/).
-000005b0: 2049 7420 6973 2061 6e20 6566 666f 7274   It is an effort
-000005c0: 2074 6f20 6275 696c 6420 736f 6674 7761   to build softwa
-000005d0: 7265 2062 7920 6e65 7572 6f73 6369 656e  re by neuroscien
-000005e0: 7469 7374 732c 2066 6f72 206e 6575 726f  tists, for neuro
-000005f0: 7363 6965 6e74 6973 7473 2e20 4966 2079  scientists. If y
-00000600: 6f75 2068 6176 6520 7375 6767 6573 7469  ou have suggesti
-00000610: 6f6e 732c 2072 6571 7565 7374 7320 6f72  ons, requests or
-00000620: 2071 7565 7374 696f 6e73 2c20 6665 656c   questions, feel
-00000630: 2066 7265 6520 746f 205b 6f70 656e 2061   free to [open a
-00000640: 6e20 6973 7375 655d 2868 7474 7073 3a2f  n issue](https:/
-00000650: 2f67 6974 6875 622e 636f 6d2f 6363 6e6d  /github.com/ccnm
-00000660: 6161 7374 7269 6368 742f 616e 676f 7261  aastricht/angora
-00000670: 7079 2f69 7373 7565 732f 6e65 772f 6368  py/issues/new/ch
-00000680: 6f6f 7365 292e 0a0a 215b 4d61 6e69 7075  oose)...![Manipu
-00000690: 6c61 7469 6f6e 2047 6966 5d28 646f 6373  lation Gif](docs
-000006a0: 2f67 6966 732f 6d61 6e69 7075 6c61 7465  /gifs/manipulate
-000006b0: 5f62 6573 742e 6769 6629 0a0a 2323 20f0  _best.gif)..## .
-000006c0: 9f93 a520 496e 7374 616c 6c61 7469 6f6e  ... Installation
-000006d0: 0a0a 416e 676f 7261 5079 2069 7320 6176  ..AngoraPy is av
-000006e0: 6169 6c61 626c 6520 6f6e 2050 7950 492e  ailable on PyPI.
-000006f0: 200a 0a60 6060 6261 7368 0a70 6970 2069   ..```bash.pip i
-00000700: 6e73 7461 6c6c 2061 6e67 6f72 6170 790a  nstall angorapy.
-00000710: 6060 600a 0a23 2323 2046 726f 6d20 736f  ```..### From so
-00000720: 7572 6365 0a41 6c74 6572 6e61 7469 7665  urce.Alternative
-00000730: 6c79 2c20 796f 7520 6361 6e20 646f 776e  ly, you can down
-00000740: 6c6f 6164 2074 6869 7320 7265 706f 7369  load this reposi
-00000750: 746f 7279 206f 7220 7468 6520 736f 7572  tory or the sour
-00000760: 6365 2063 6f64 6520 6f66 2061 6e79 2070  ce code of any p
-00000770: 7265 7669 6f75 7320 7265 6c65 6173 6520  revious release 
-00000780: 6f72 2062 7261 6e63 6820 616e 6420 696e  or branch and in
-00000790: 7374 616c 6c20 6672 6f6d 2073 6f75 7263  stall from sourc
-000007a0: 652c 2075 7369 6e67 2070 6970 2e0a 0a60  e, using pip...`
-000007b0: 6060 6261 7368 0a70 6970 2069 6e73 7461  ``bash.pip insta
-000007c0: 6c6c 202d 6520 2e0a 6060 600a 0a54 6869  ll -e ..```..Thi
-000007d0: 7320 7761 792c 2069 6620 796f 7520 6d61  s way, if you ma
-000007e0: 6b65 2063 6861 6e67 6573 2074 6f20 7468  ke changes to th
-000007f0: 6520 736f 7572 6365 2063 6f64 652c 2074  e source code, t
-00000800: 6865 7365 2077 696c 6c20 6265 2072 6563  hese will be rec
-00000810: 6f67 6e69 7a65 6420 696e 2074 6865 2069  ognized in the i
-00000820: 6e73 7461 6c6c 6174 696f 6e20 2877 6974  nstallation (wit
-00000830: 686f 7574 2074 6865 206e 6565 6420 746f  hout the need to
-00000840: 2072 6569 6e73 7461 6c6c 292e 0a0a 2323   reinstall)...##
-00000850: 2320 446f 636b 6572 0a41 6c74 6572 6e61  # Docker.Alterna
-00000860: 7469 7665 6c79 2c20 796f 7520 6361 6e20  tively, you can 
-00000870: 696e 7374 616c 6c20 416e 676f 7261 5079  install AngoraPy
-00000880: 2061 6e64 2061 6c6c 2069 7473 2064 6570   and all its dep
-00000890: 656e 6465 6e63 6965 7320 696e 2061 2064  endencies in a d
-000008a0: 6f63 6b65 7220 636f 6e74 6169 6e65 7220  ocker container 
-000008b0: 7573 696e 6720 7468 6520 446f 636b 6572  using the Docker
-000008c0: 6669 6c65 2070 726f 7669 6465 6420 696e  file provided in
-000008d0: 2074 6869 7320 7265 706f 7369 746f 7279   this repository
-000008e0: 2028 2f64 6f63 6b65 722f 446f 636b 6572   (/docker/Docker
-000008f0: 6669 6c65 292e 2054 6f20 7468 6973 2065  file). To this e
-00000900: 6e64 2c20 646f 776e 6c6f 6164 2074 6865  nd, download the
-00000910: 2072 6570 6f73 6974 6f72 7920 616e 6420   repository and 
-00000920: 6275 696c 6420 7468 6520 646f 636b 6572  build the docker
-00000930: 2069 6d61 6765 2066 726f 6d20 7468 6520   image from the 
-00000940: 2f64 6f63 6b65 7220 6469 7265 6374 6f72  /docker director
-00000950: 793a 0a0a 6060 6062 6173 680a 7375 646f  y:..```bash.sudo
-00000960: 2064 6f63 6b65 7220 6275 696c 6420 2d74   docker build -t
-00000970: 2061 6e67 6f72 6170 793a 6d61 7374 6572   angorapy:master
-00000980: 2068 7474 7073 3a2f 2f67 6974 6875 622e   https://github.
-00000990: 636f 6d2f 6363 6e6d 6161 7374 7269 6368  com/ccnmaastrich
-000009a0: 742f 616e 676f 7261 7079 2e67 6974 236d  t/angorapy.git#m
-000009b0: 6173 7465 7220 2d66 202d 203c 2044 6f63  aster -f - < Doc
-000009c0: 6b65 7266 696c 650a 6060 600a 0a54 6f20  kerfile.```..To 
-000009d0: 696e 7374 616c 6c20 6469 6666 6572 656e  install differen
-000009e0: 7420 7665 7273 696f 6e73 2c20 7265 706c  t versions, repl
-000009f0: 6163 6520 6023 6d61 7374 6572 6020 696e  ace `#master` in
-00000a00: 2074 6865 2073 6f75 7263 6520 6279 2074   the source by t
-00000a10: 6865 2074 6167 2f62 7261 6e63 6820 6f66  he tag/branch of
-00000a20: 2074 6865 2072 6573 7065 6374 6976 6520   the respective 
-00000a30: 7665 7273 696f 6e20 796f 7520 7761 6e74  version you want
-00000a40: 2074 6f20 696e 7374 616c 6c2e 0a0a 2323   to install...##
-00000a50: 20f0 9f9a 8020 4765 7474 696e 6720 5374   .... Getting St
-00000a60: 6172 7465 640a 5468 6520 7363 7269 7074  arted.The script
-00000a70: 7320 6074 7261 696e 2e70 7960 2c20 6065  s `train.py`, `e
-00000a80: 7661 6c75 6174 652e 7079 6020 616e 6420  valuate.py` and 
-00000a90: 606f 6273 6572 7665 2e70 7960 2070 726f  `observe.py` pro
-00000aa0: 7669 6465 2072 6561 6479 2d6d 6164 6520  vide ready-made 
-00000ab0: 7363 7269 7074 7320 666f 7220 7472 6169  scripts for trai
-00000ac0: 6e69 6e67 2061 6e64 2065 7661 6c75 6174  ning and evaluat
-00000ad0: 696e 6720 616e 2061 6765 6e74 2069 6e20  ing an agent in 
-00000ae0: 616e 7920 656e 7669 726f 6e6d 656e 742e  any environment.
-00000af0: 2057 6974 6820 6070 7265 7472 6169 6e2e   With `pretrain.
-00000b00: 7079 602c 2069 7420 6973 2070 6f73 7369  py`, it is possi
-00000b10: 626c 6520 746f 2070 7265 7472 6169 6e20  ble to pretrain 
-00000b20: 7468 6520 7669 7375 616c 2063 6f6d 706f  the visual compo
-00000b30: 6e65 6e74 2e20 6062 656e 6368 6d61 726b  nent. `benchmark
-00000b40: 2e70 7960 2070 726f 7669 6465 7320 6675  .py` provides fu
-00000b50: 6e63 7469 6f6e 616c 6974 7920 666f 7220  nctionality for 
-00000b60: 7472 6169 6e69 6e67 2061 2062 6174 6368  training a batch
-00000b70: 206f 6620 6167 656e 7473 2070 6f73 7369   of agents possi
-00000b80: 626c 7920 7573 696e 6720 6469 6666 6572  bly using differ
-00000b90: 656e 7420 636f 6e66 6967 7320 666f 7220  ent configs for 
-00000ba0: 636f 6d70 6172 6973 6f6e 206f 6620 7374  comparison of st
-00000bb0: 7261 7465 6769 6573 2e0a 0a23 2323 2054  rategies...### T
-00000bc0: 7261 696e 696e 6720 616e 2041 6765 6e74  raining an Agent
-00000bd0: 0a54 6865 2060 7472 6169 6e2e 7079 6020  .The `train.py` 
-00000be0: 636f 6d6d 616e 646c 696e 6520 696e 7465  commandline inte
-00000bf0: 7266 6163 6520 7072 6f76 6964 6573 2061  rface provides a
-00000c00: 2063 6f6e 7665 6e69 656e 7420 656e 7472   convenient entr
-00000c10: 792d 706f 696e 7420 666f 7220 7275 6e6e  y-point for runn
-00000c20: 696e 6720 616c 6c20 736f 7274 7320 6f66  ing all sorts of
-00000c30: 2065 7870 6572 696d 656e 7473 2075 7369   experiments usi
-00000c40: 6e67 2074 6865 2062 7569 6c74 696e 206d  ng the builtin m
-00000c50: 6f64 656c 7320 616e 6420 656e 7669 726f  odels and enviro
-00000c60: 6e6d 656e 7473 2069 6e20 616e 676f 7261  nments in angora
-00000c70: 7079 2e20 596f 7520 6361 6e20 7472 6169  py. You can trai
-00000c80: 6e20 616e 2061 6765 6e74 206f 6e20 616e  n an agent on an
-00000c90: 7920 656e 7669 726f 6e6d 656e 7420 7769  y environment wi
-00000ca0: 7468 206f 7074 696f 6e61 6c20 6879 7065  th optional hype
-00000cb0: 7270 6172 616d 6574 6572 732e 2041 6464  rparameters. Add
-00000cc0: 6974 696f 6e61 6c6c 792c 2061 206d 6f6e  itionally, a mon
-00000cd0: 6974 6f72 2077 696c 6c20 6265 2061 7574  itor will be aut
-00000ce0: 6f6d 6174 6963 616c 6c79 206c 696e 6b65  omatically linke
-00000cf0: 6420 746f 2074 6865 2074 7261 696e 696e  d to the trainin
-00000d00: 6720 6f66 2074 6865 2061 6765 6e74 2e20  g of the agent. 
-00000d10: 466f 7220 6d6f 7265 2064 6574 6169 6c20  For more detail 
-00000d20: 636f 6e73 756c 7420 7468 6520 3c61 2068  consult the <a h
-00000d30: 7265 663d 226d 6f6e 6974 6f72 2f52 4541  ref="monitor/REA
-00000d40: 444d 452e 6d64 223e 5245 4144 4d45 206f  DME.md">README o
-00000d50: 6e20 6d6f 6e69 746f 7269 6e67 3c2f 613e  n monitoring</a>
-00000d60: 2e0a 0a42 6173 6520 7573 6167 6520 6f66  ...Base usage of
-00000d70: 2060 7472 6169 6e2e 7079 6020 6973 2061   `train.py` is a
-00000d80: 7320 666f 6c6c 6f77 733a 0a0a 2020 2020  s follows:..    
-00000d90: 7079 7468 6f6e 2074 7261 696e 2e70 7920  python train.py 
-00000da0: 454e 5620 2d2d 6172 6368 6974 6563 7475  ENV --architectu
-00000db0: 7265 204d 4f44 454c 0a20 2020 200a 466f  re MODEL.    .Fo
-00000dc0: 7220 696e 7374 616e 6365 2c20 7472 6169  r instance, trai
-00000dd0: 6e69 6e67 2060 4c75 6e61 724c 616e 6465  ning `LunarLande
-00000de0: 7243 6f6e 7469 6e75 6f75 732d 7632 6020  rContinuous-v2` 
-00000df0: 7573 696e 6720 7468 6520 6064 6565 7065  using the `deepe
-00000e00: 7260 2061 7263 6869 7465 6374 7572 6520  r` architecture 
-00000e10: 6973 2070 6f73 7369 626c 6520 6279 2072  is possible by r
-00000e20: 756e 6e69 6e67 3a0a 0a20 2020 2070 7974  unning:..    pyt
-00000e30: 686f 6e20 7472 6169 6e2e 7079 204c 756e  hon train.py Lun
-00000e40: 6172 4c61 6e64 6572 436f 6e74 696e 756f  arLanderContinuo
-00000e50: 7573 2d76 3220 2d2d 6172 6368 6974 6563  us-v2 --architec
-00000e60: 7475 7265 2064 6565 7065 720a 2020 2020  ture deeper.    
-00000e70: 0a46 6f72 206d 6f72 6520 6164 7661 6e63  .For more advanc
-00000e80: 6564 206f 7074 696f 6e73 206c 696b 6520  ed options like 
-00000e90: 6375 7374 6f6d 2068 7970 6572 7061 7261  custom hyperpara
-00000ea0: 6d65 7465 7273 2c20 636f 6e73 756c 740a  meters, consult.
-00000eb0: 0a20 2020 2070 7974 686f 6e20 7472 6169  .    python trai
-00000ec0: 6e2e 7079 202d 680a 0a0a 2323 2320 4576  n.py -h...### Ev
-00000ed0: 616c 7561 7469 6e67 2061 6e64 204f 6273  aluating and Obs
-00000ee0: 6572 7669 6e67 2061 6e20 4167 656e 740a  erving an Agent.
-00000ef0: 5468 6572 6520 6172 6520 7477 6f20 6d6f  There are two mo
-00000f00: 7265 2065 6e74 7279 2070 6f69 6e74 7320  re entry points 
-00000f10: 666f 7220 6576 616c 7561 7469 6e67 2061  for evaluating a
-00000f20: 6e64 206f 6273 6572 7669 6e67 2061 6e20  nd observing an 
-00000f30: 6167 656e 743a 2060 6576 616c 7561 7465  agent: `evaluate
-00000f40: 2e70 7960 2061 6e64 2060 6f62 7365 7276  .py` and `observ
-00000f50: 652e 7079 602e 2047 656e 6572 616c 2075  e.py`. General u
-00000f60: 7361 6765 2069 7320 6173 2066 6f6c 6c6f  sage is as follo
-00000f70: 7773 0a0a 2020 2020 7079 7468 6f6e 2065  ws..    python e
-00000f80: 7661 6c75 6174 652e 7079 2049 440a 0a57  valuate.py ID..W
-00000f90: 6865 7265 2049 4420 6973 2074 6865 2061  here ID is the a
-00000fa0: 6765 6e74 2773 2049 4420 6769 7665 6e20  gent's ID given 
-00000fb0: 7768 656e 2069 7473 2063 7265 6174 6564  when its created
-00000fc0: 2028 6074 7261 696e 2e70 7960 2070 7269   (`train.py` pri
-00000fd0: 6e74 7320 7468 6973 206f 7574 742c 2069  nts this outt, i
-00000fe0: 6e20 6375 7374 6f6d 2073 6372 6970 7473  n custom scripts
-00000ff0: 2067 6574 2069 7420 7769 7468 2060 6167   get it with `ag
-00001000: 656e 742e 6167 656e 745f 6964 6029 2e0a  ent.agent_id`)..
-00001010: 0a23 2323 2057 7269 7469 6e67 2061 2054  .### Writing a T
-00001020: 7261 696e 696e 6720 5363 7269 7074 0a54  raining Script.T
-00001030: 6f20 7472 6169 6e20 6167 656e 7473 2077  o train agents w
-00001040: 6974 6820 6375 7374 6f6d 206d 6f64 656c  ith custom model
-00001050: 732c 2065 6e76 6972 6f6e 6d65 6e74 732c  s, environments,
-00001060: 2065 7463 2e20 796f 7520 7772 6974 6520   etc. you write 
-00001070: 796f 7572 206f 776e 2073 6372 6970 742e  your own script.
-00001080: 2054 6865 2066 6f6c 6c6f 7769 6e67 2069   The following i
-00001090: 7320 6120 6d69 6e69 6d61 6c20 6578 616d  s a minimal exam
-000010a0: 706c 653a 0a0a 6060 6070 7974 686f 6e0a  ple:..```python.
-000010b0: 6672 6f6d 2061 6e67 6f72 6170 792e 636f  from angorapy.co
-000010c0: 6d6d 6f6e 2e77 7261 7070 6572 7320 696d  mmon.wrappers im
-000010d0: 706f 7274 206d 616b 655f 656e 760a 6672  port make_env.fr
-000010e0: 6f6d 2061 6e67 6f72 6170 792e 6d6f 6465  om angorapy.mode
-000010f0: 6c73 2069 6d70 6f72 7420 6765 745f 6d6f  ls import get_mo
-00001100: 6465 6c5f 6275 696c 6465 720a 6672 6f6d  del_builder.from
-00001110: 2061 6e67 6f72 6170 792e 6167 656e 742e   angorapy.agent.
-00001120: 7070 6f5f 6167 656e 7420 696d 706f 7274  ppo_agent import
-00001130: 2050 504f 4167 656e 740a 0a65 6e76 203d   PPOAgent..env =
-00001140: 206d 616b 655f 656e 7628 224c 756e 6172   make_env("Lunar
-00001150: 4c61 6e64 6572 436f 6e74 696e 756f 7573  LanderContinuous
-00001160: 2d76 3222 290a 6d6f 6465 6c5f 6275 696c  -v2").model_buil
-00001170: 6465 7220 3d20 6765 745f 6d6f 6465 6c5f  der = get_model_
-00001180: 6275 696c 6465 7228 2273 696d 706c 6522  builder("simple"
-00001190: 2c20 2266 666e 2229 0a61 6765 6e74 203d  , "ffn").agent =
-000011a0: 2050 504f 4167 656e 7428 6d6f 6465 6c5f   PPOAgent(model_
-000011b0: 6275 696c 6465 722c 2065 6e76 290a 6167  builder, env).ag
-000011c0: 656e 742e 6472 696c 6c28 3130 302c 2031  ent.drill(100, 1
-000011d0: 302c 2035 3132 290a 6060 600a 0a46 6f72  0, 512).```..For
-000011e0: 206d 6f72 6520 6465 7461 696c 732c 2063   more details, c
-000011f0: 6f6e 7375 6c74 2074 6865 205b 6578 616d  onsult the [exam
-00001200: 706c 6573 5d28 6578 616d 706c 6573 292e  ples](examples).
-00001210: 0a0a 2323 20f0 9f8e 9320 446f 6375 6d65  ..## .... Docume
-00001220: 6e74 6174 696f 6e0a 4465 7461 696c 6564  ntation.Detailed
-00001230: 2064 6f63 756d 656e 7461 7469 6f6e 206f   documentation o
-00001240: 6620 416e 676f 7261 5079 2069 7320 7072  f AngoraPy is pr
-00001250: 6f76 6964 6564 2069 6e20 7468 6520 5245  ovided in the RE
-00001260: 4144 4d45 7320 6f66 206d 6f73 7420 7375  ADMEs of most su
-00001270: 6270 6163 6b61 6765 732e 2041 6464 6974  bpackages. Addit
-00001280: 696f 6e61 6c6c 792c 2077 6520 7072 6f76  ionally, we prov
-00001290: 6964 6520 5b65 7861 6d70 6c65 7320 616e  ide [examples an
-000012a0: 6420 7475 746f 7269 616c 735d 2865 7861  d tutorials](exa
-000012b0: 6d70 6c65 7329 2074 6861 7420 6765 7420  mples) that get 
-000012c0: 796f 7520 7374 6172 7465 6420 7769 7468  you started with
-000012d0: 2077 7269 7469 6e67 2079 6f75 7220 6f77   writing your ow
-000012e0: 6e20 7363 7269 7074 7320 7573 696e 6720  n scripts using 
-000012f0: 416e 676f 7261 5079 2e20 466f 7220 6675  AngoraPy. For fu
-00001300: 7274 6865 7220 7265 6164 696e 6773 206f  rther readings o
-00001310: 6e20 7370 6563 6966 6963 206d 6f64 756c  n specific modul
-00001320: 6573 2c20 636f 6e73 756c 7420 7468 6520  es, consult the 
-00001330: 666f 6c6c 6f77 696e 6720 5245 4144 4d45  following README
-00001340: 733a 200a 0a20 2d20 5b41 6765 6e74 5d28  s: .. - [Agent](
-00001350: 616e 676f 7261 7079 2f61 6765 6e74 2920  angorapy/agent) 
-00001360: 5b57 4950 5d0a 202d 205b 456e 7669 726f  [WIP]. - [Enviro
-00001370: 6e6d 656e 7473 5d28 616e 676f 7261 7079  nments](angorapy
-00001380: 2f65 6e76 6972 6f6e 6d65 6e74 7329 0a20  /environments). 
-00001390: 2d20 5b4d 6f64 656c 735d 2861 6e67 6f72  - [Models](angor
-000013a0: 6170 792f 6d6f 6465 6c73 290a 202d 205b  apy/models). - [
-000013b0: 416e 616c 7973 6973 5d28 616e 676f 7261  Analysis](angora
-000013c0: 7079 2f61 6e61 6c79 7369 7329 0a20 2d20  py/analysis). - 
-000013d0: 5b4d 6f6e 6974 6f72 696e 675d 2861 6e67  [Monitoring](ang
-000013e0: 6f72 6170 792f 6d6f 6e69 746f 7269 6e67  orapy/monitoring
-000013f0: 290a 0a49 6620 796f 7520 6172 6520 6d69  )..If you are mi
-00001400: 7373 696e 6720 6120 646f 6375 6d65 6e74  ssing a document
-00001410: 6174 696f 6e20 666f 7220 6120 7370 6563  ation for a spec
-00001420: 6966 6963 2070 6172 7420 6f66 2041 6e67  ific part of Ang
-00001430: 6f72 6150 792c 2066 6565 6c20 6672 6565  oraPy, feel free
-00001440: 2074 6f20 6f70 656e 2061 6e20 6973 7375   to open an issu
-00001450: 6520 616e 6420 7765 2077 696c 6c20 646f  e and we will do
-00001460: 206f 7572 2062 6573 7420 746f 2061 6464   our best to add
-00001470: 2069 742e 0a0a 2323 20f0 9f94 8020 4469   it...## .... Di
-00001480: 7374 7269 6275 7465 6420 436f 6d70 7574  stributed Comput
-00001490: 6174 696f 6e0a 5050 4f20 6973 2061 6e20  ation.PPO is an 
-000014a0: 6173 796e 6368 726f 6e6f 7573 2061 6c67  asynchronous alg
-000014b0: 6f72 6974 686d 2c20 616c 6c6f 7769 6e67  orithm, allowing
-000014c0: 206d 756c 7469 706c 6520 7061 7261 6c6c   multiple parall
-000014d0: 656c 2077 6f72 6b65 7273 2074 6f20 6765  el workers to ge
-000014e0: 6e65 7261 7465 2065 7870 6572 6965 6e63  nerate experienc
-000014f0: 6520 696e 6465 7065 6e64 656e 746c 792e  e independently.
-00001500: 200a 5765 2061 6c6c 6f77 2070 6172 616c   .We allow paral
-00001510: 6c65 6c20 6761 7468 6572 696e 6720 616e  lel gathering an
-00001520: 6420 6f70 7469 6d69 7a61 7469 6f6e 2074  d optimization t
-00001530: 6872 6f75 6768 204d 5049 2e20 4167 656e  hrough MPI. Agen
-00001540: 7473 2077 696c 6c20 6175 746f 6d61 7469  ts will automati
-00001550: 6361 6c6c 7920 6469 7374 7269 6275 7465  cally distribute
-00001560: 2074 6865 6972 2077 6f72 6b65 7273 2065   their workers e
-00001570: 7665 6e6c 7920 6f6e 200a 7468 6520 6176  venly on .the av
-00001580: 6169 6c61 626c 6520 4350 5520 636f 7265  ailable CPU core
-00001590: 732c 2077 6869 6c65 206f 7074 696d 697a  s, while optimiz
-000015a0: 6174 696f 6e20 6973 2064 6973 7472 6962  ation is distrib
-000015b0: 7574 6564 206f 7665 7220 616c 6c20 6176  uted over all av
-000015c0: 6169 6c61 626c 6520 4750 5573 2e20 4966  ailable GPUs. If
-000015d0: 206e 6f20 4750 5573 2061 7265 2061 7661   no GPUs are ava
-000015e0: 696c 6162 6c65 2c20 616c 6c20 4350 5573  ilable, all CPUs
-000015f0: 200a 7368 6172 6520 7468 6520 7461 736b   .share the task
-00001600: 206f 6620 6f70 7469 6d69 7a69 6e67 2e0a   of optimizing..
-00001610: 0a44 6973 7472 6962 7574 696f 6e20 6973  .Distribution is
-00001620: 2070 6f73 7369 626c 6520 6c6f 6361 6c6c   possible locall
-00001630: 7920 6f6e 2079 6f75 7220 776f 726b 7374  y on your workst
-00001640: 6174 696f 6e20 616e 6420 6f6e 2048 5043  ation and on HPC
-00001650: 2073 6974 6573 2e20 0a0a 2323 2320 f09f   sites. ..### ..
-00001660: 92bb 204c 6f63 616c 2044 6973 7472 6962  .. Local Distrib
-00001670: 7574 6564 2043 6f6d 7075 7469 6e67 2077  uted Computing w
-00001680: 6974 6820 4d50 490a 546f 2075 7365 204d  ith MPI.To use M
-00001690: 5049 206c 6f63 616c 6c79 2c20 796f 7520  PI locally, you 
-000016a0: 6e65 6564 2074 6f20 6861 7665 2061 2072  need to have a r
-000016b0: 756e 6e69 6e67 204d 5049 2069 6d70 6c65  unning MPI imple
-000016c0: 6d65 6e74 6174 696f 6e2c 2065 2e67 2e20  mentation, e.g. 
-000016d0: 4f70 656e 204d 5049 2034 206f 6e20 5562  Open MPI 4 on Ub
-000016e0: 756e 7475 2e0a 546f 2065 7865 6375 7465  untu..To execute
-000016f0: 2060 7472 6169 6e2e 7079 6020 7669 6120   `train.py` via 
-00001700: 4d50 492c 2072 756e 0a0a 6060 6062 6173  MPI, run..```bas
-00001710: 680a 6d70 6972 756e 202d 6e70 2031 3220  h.mpirun -np 12 
-00001720: 2d2d 7573 652d 6877 7468 7265 6164 2d63  --use-hwthread-c
-00001730: 7075 7320 7079 7468 6f6e 3320 7472 6169  pus python3 trai
-00001740: 6e2e 7079 202e 2e2e 0a60 6060 0a0a 7768  n.py ....```..wh
-00001750: 6572 652c 2069 6e20 7468 6973 2065 7861  ere, in this exa
-00001760: 6d70 6c65 2c20 3132 2069 7320 7468 6520  mple, 12 is the 
-00001770: 6e75 6d62 6572 206f 6620 6c6f 6361 6c6c  number of locall
-00001780: 7920 6176 6169 6c61 626c 6520 4350 5520  y available CPU 
-00001790: 7468 7265 6164 7320 616e 6420 602d 2d75  threads and `--u
-000017a0: 7365 2d68 7774 6872 6561 642d 6370 7573  se-hwthread-cpus
-000017b0: 600a 6d61 6b65 7320 6176 6169 6c61 626c  `.makes availabl
-000017c0: 6520 7468 7265 6164 7320 2861 7320 6f70  e threads (as op
-000017d0: 706f 7365 6420 746f 206f 6e6c 7920 636f  posed to only co
-000017e0: 7265 7329 2e20 5573 6167 6520 6f66 2060  res). Usage of `
-000017f0: 7472 6169 6e2e 7079 6020 6973 2061 7320  train.py` is as 
-00001800: 6465 7363 7269 6265 6420 7072 6576 696f  described previo
-00001810: 7573 6c79 2e0a 0a23 2323 203a 636c 6f75  usly...### :clou
-00001820: 643a 2044 6973 7472 6962 7574 6564 2054  d: Distributed T
-00001830: 7261 696e 696e 6720 6f6e 2053 4c55 524d  raining on SLURM
-00001840: 2d62 6173 6564 2048 5043 2063 6c75 7374  -based HPC clust
-00001850: 6572 730a 2a50 6c65 6173 6520 6e6f 7465  ers.*Please note
-00001860: 2074 6861 7420 7468 6520 666f 6c6c 6f77   that the follow
-00001870: 696e 6720 6973 206f 7074 696d 697a 6564  ing is optimized
-00001880: 2061 6e64 2074 6573 7465 6420 6f6e 2074   and tested on t
-00001890: 6865 2073 7065 6369 6669 6320 636c 7573  he specific clus
-000018a0: 7465 7220 7765 2075 7365 2c20 6275 7420  ter we use, but 
-000018b0: 7368 6f75 6c64 2065 7874 656e 6420 746f  should extend to
-000018c0: 2061 7420 6c65 6173 7420 0a61 6e79 2053   at least .any S
-000018d0: 4c55 524d 2062 6173 6564 2073 6574 7570  LURM based setup
-000018e0: 2e2a 0a0a 4f6e 2061 6e79 2053 4c55 524d  .*..On any SLURM
-000018f0: 2d62 6173 6564 2048 5043 2063 6c75 7374  -based HPC clust
-00001900: 6572 2079 6f75 206d 6179 2073 7562 6d69  er you may submi
-00001910: 7420 796f 7572 206a 6f62 2077 6974 6820  t your job with 
-00001920: 7362 6174 6368 2075 7369 7369 6e67 2074  sbatch usising t
-00001930: 6865 2066 6f6c 6c6f 7769 6e67 2073 6372  he following scr
-00001940: 6970 7420 7465 6d70 6c61 7465 3a0a 0a60  ipt template:..`
-00001950: 6060 6261 7368 0a23 212f 6269 6e2f 6261  ``bash.#!/bin/ba
-00001960: 7368 202d 6c0a 2353 4241 5443 4820 2d2d  sh -l.#SBATCH --
-00001970: 6a6f 622d 6e61 6d65 3d22 616e 676f 7261  job-name="angora
-00001980: 7079 220a 2353 4241 5443 4820 2d2d 6163  py".#SBATCH --ac
-00001990: 636f 756e 743d 7878 780a 2353 4241 5443  count=xxx.#SBATC
-000019a0: 4820 2d2d 7469 6d65 3d32 343a 3030 3a30  H --time=24:00:0
-000019b0: 300a 2353 4241 5443 4820 2d2d 6e6f 6465  0.#SBATCH --node
-000019c0: 733d 3332 0a23 5342 4154 4348 202d 2d6e  s=32.#SBATCH --n
-000019d0: 7461 736b 732d 7065 722d 636f 7265 3d31  tasks-per-core=1
-000019e0: 0a23 5342 4154 4348 202d 2d6e 7461 736b  .#SBATCH --ntask
-000019f0: 732d 7065 722d 6e6f 6465 3d31 320a 2353  s-per-node=12.#S
-00001a00: 4241 5443 4820 2d2d 6370 7573 2d70 6572  BATCH --cpus-per
-00001a10: 2d74 6173 6b3d 310a 2353 4241 5443 4820  -task=1.#SBATCH 
-00001a20: 2d2d 7061 7274 6974 696f 6e3d 6e6f 726d  --partition=norm
-00001a30: 616c 0a23 5342 4154 4348 202d 2d63 6f6e  al.#SBATCH --con
-00001a40: 7374 7261 696e 743d 6770 7526 7374 6172  straint=gpu&star
-00001a50: 7478 0a23 5342 4154 4348 202d 2d68 696e  tx.#SBATCH --hin
-00001a60: 743d 6e6f 6d75 6c74 6974 6872 6561 640a  t=nomultithread.
-00001a70: 0a65 7870 6f72 7420 4f4d 505f 4e55 4d5f  .export OMP_NUM_
-00001a80: 5448 5245 4144 533d 2453 4c55 524d 5f43  THREADS=$SLURM_C
-00001a90: 5055 535f 5045 525f 5441 534b 0a65 7870  PUS_PER_TASK.exp
-00001aa0: 6f72 7420 4352 4159 5f43 5544 415f 4d50  ort CRAY_CUDA_MP
-00001ab0: 533d 310a 0a23 206c 6f61 6420 7669 7274  S=1..# load virt
-00001ac0: 7561 6c20 656e 7669 726f 6e6d 656e 740a  ual environment.
-00001ad0: 736f 7572 6365 2024 7b48 4f4d 457d 2f72  source ${HOME}/r
-00001ae0: 6f62 6f76 656e 762f 6269 6e2f 6163 7469  obovenv/bin/acti
-00001af0: 7661 7465 0a0a 6578 706f 7274 2044 4953  vate..export DIS
-00001b00: 504c 4159 3d3a 300a 7372 756e 2070 7974  PLAY=:0.srun pyt
-00001b10: 686f 6e33 202d 7520 7472 6169 6e2e 7079  hon3 -u train.py
-00001b20: 202e 2e2e 0a60 6060 0a0a 5468 6520 6e75   ....```..The nu
-00001b30: 6d62 6572 206f 6620 7061 7261 6c6c 656c  mber of parallel
-00001b40: 2077 6f72 6b65 7273 2077 696c 6c20 6571   workers will eq
-00001b50: 7561 6c20 7468 6520 6e75 6d62 6572 206f  ual the number o
-00001b60: 6620 6e6f 6465 7320 7469 6d65 7320 7468  f nodes times th
-00001b70: 6520 6e75 6d62 6572 206f 6620 4350 5573  e number of CPUs
-00001b80: 2070 6572 206e 6f64 6520 0a28 3332 2078   per node .(32 x
-00001b90: 2031 3220 3d20 3338 3420 696e 2074 6865   12 = 384 in the
-00001ba0: 2074 656d 706c 6174 6520 6162 6f76 6529   template above)
-00001bb0: 2e0a 0a23 2320 f09f 9497 2043 6974 696e  ...## .... Citin
-00001bc0: 6720 416e 676f 7261 5079 0a0a 4966 2079  g AngoraPy..If y
-00001bd0: 6f75 2075 7365 2041 6e67 6f72 6150 7920  ou use AngoraPy 
-00001be0: 666f 7220 796f 7572 2072 6573 6561 7263  for your researc
-00001bf0: 682c 2070 6c65 6173 6520 6369 7465 2075  h, please cite u
-00001c00: 7320 6173 2066 6f6c 6c6f 7773 0a0a 2020  s as follows..  
-00001c10: 2020 5765 6964 6c65 722c 2054 2e2c 2026    Weidler, T., &
-00001c20: 2053 656e 6465 6e2c 204d 2e20 2832 3032   Senden, M. (202
-00001c30: 3029 2e20 416e 676f 7261 5079 3a20 416e  0). AngoraPy: An
-00001c40: 7468 726f 706f 6d6f 7270 6869 6320 476f  thropomorphic Go
-00001c50: 616c 2d4f 7269 656e 7465 6420 526f 626f  al-Oriented Robo
-00001c60: 7469 6320 436f 6e74 726f 6c20 666f 7220  tic Control for 
-00001c70: 4e65 7572 6f73 6369 656e 7469 6669 6320  Neuroscientific 
-00001c80: 4d6f 6465 6c69 6e67 205b 436f 6d70 7574  Modeling [Comput
-00001c90: 6572 2073 6f66 7477 6172 655d 0a0a 4f72  er software]..Or
-00001ca0: 2075 7369 6e67 2062 6962 7465 780a 0a20   using bibtex.. 
-00001cb0: 2020 2040 736f 6674 7761 7265 7b61 6e67     @software{ang
-00001cc0: 6f72 6170 7932 3032 302c 0a20 2020 2020  orapy2020,.     
-00001cd0: 2020 2061 7574 686f 7220 3d20 7b57 6569     author = {Wei
-00001ce0: 646c 6572 2c20 546f 6e69 6f20 616e 6420  dler, Tonio and 
-00001cf0: 5365 6e64 656e 2c20 4d61 7269 6f7d 2c0a  Senden, Mario},.
-00001d00: 2020 2020 2020 2020 6d6f 6e74 6820 3d20          month = 
-00001d10: 7b33 7d2c 0a20 2020 2020 2020 2074 6974  {3},.        tit
-00001d20: 6c65 203d 207b 7b41 6e67 6f72 6150 793a  le = {{AngoraPy:
-00001d30: 2041 6e74 6872 6f70 6f6d 6f72 7068 6963   Anthropomorphic
-00001d40: 2047 6f61 6c2d 4f72 6965 6e74 6564 2052   Goal-Oriented R
-00001d50: 6f62 6f74 6963 2043 6f6e 7472 6f6c 2066  obotic Control f
-00001d60: 6f72 204e 6575 726f 7363 6965 6e74 6966  or Neuroscientif
-00001d70: 6963 204d 6f64 656c 696e 677d 7d2c 0a20  ic Modeling}},. 
-00001d80: 2020 2020 2020 2079 6561 7220 3d20 7b32         year = {2
-00001d90: 3032 307d 0a20 2020 207d 0a              020}.    }.
+00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
+00000010: 3a20 322e 310a 4e61 6d65 3a20 616e 676f  : 2.1.Name: ango
+00000020: 7261 7079 0a56 6572 7369 6f6e 3a20 302e  rapy.Version: 0.
+00000030: 392e 310a 5375 6d6d 6172 793a 2041 4e74  9.1.Summary: ANt
+00000040: 6872 6f70 6f6d 6f72 7068 6963 2047 6f61  hropomorphic Goa
+00000050: 6c2d 4f52 6965 6e74 6564 204d 6f64 656c  l-ORiented Model
+00000060: 696e 672c 204c 6561 726e 696e 6720 616e  ing, Learning an
+00000070: 6420 416e 616c 7973 6973 2066 6f72 204e  d Analysis for N
+00000080: 6575 726f 7363 6965 6e63 650a 486f 6d65  euroscience.Home
+00000090: 2d70 6167 653a 2068 7474 7073 3a2f 2f67  -page: https://g
+000000a0: 6974 6875 622e 636f 6d2f 6363 6e6d 6161  ithub.com/ccnmaa
+000000b0: 7374 7269 6368 742f 616e 676f 7261 7079  stricht/angorapy
+000000c0: 0a41 7574 686f 723a 2054 6f6e 696f 2057  .Author: Tonio W
+000000d0: 6569 646c 6572 0a41 7574 686f 722d 656d  eidler.Author-em
+000000e0: 6169 6c3a 2072 6573 6561 7263 6840 746f  ail: research@to
+000000f0: 6e69 6f77 6569 646c 6572 2e64 650a 4c69  nioweidler.de.Li
+00000100: 6365 6e73 653a 2047 504c 2d33 2e30 0a43  cense: GPL-3.0.C
+00000110: 6c61 7373 6966 6965 723a 2044 6576 656c  lassifier: Devel
+00000120: 6f70 6d65 6e74 2053 7461 7475 7320 3a3a  opment Status ::
+00000130: 2033 202d 2041 6c70 6861 0a43 6c61 7373   3 - Alpha.Class
+00000140: 6966 6965 723a 2049 6e74 656e 6465 6420  ifier: Intended 
+00000150: 4175 6469 656e 6365 203a 3a20 5363 6965  Audience :: Scie
+00000160: 6e63 652f 5265 7365 6172 6368 0a43 6c61  nce/Research.Cla
+00000170: 7373 6966 6965 723a 204c 6963 656e 7365  ssifier: License
+00000180: 203a 3a20 4f53 4920 4170 7072 6f76 6564   :: OSI Approved
+00000190: 203a 3a20 474e 5520 4765 6e65 7261 6c20   :: GNU General 
+000001a0: 5075 626c 6963 204c 6963 656e 7365 2076  Public License v
+000001b0: 3320 2847 504c 7633 290a 436c 6173 7369  3 (GPLv3).Classi
+000001c0: 6669 6572 3a20 4f70 6572 6174 696e 6720  fier: Operating 
+000001d0: 5379 7374 656d 203a 3a20 504f 5349 5820  System :: POSIX 
+000001e0: 3a3a 204c 696e 7578 0a43 6c61 7373 6966  :: Linux.Classif
+000001f0: 6965 723a 2050 726f 6772 616d 6d69 6e67  ier: Programming
+00000200: 204c 616e 6775 6167 6520 3a3a 2050 7974   Language :: Pyt
+00000210: 686f 6e20 3a3a 2033 0a43 6c61 7373 6966  hon :: 3.Classif
+00000220: 6965 723a 2050 726f 6772 616d 6d69 6e67  ier: Programming
+00000230: 204c 616e 6775 6167 6520 3a3a 2050 7974   Language :: Pyt
+00000240: 686f 6e20 3a3a 2033 2e35 0a43 6c61 7373  hon :: 3.5.Class
+00000250: 6966 6965 723a 2050 726f 6772 616d 6d69  ifier: Programmi
+00000260: 6e67 204c 616e 6775 6167 6520 3a3a 2050  ng Language :: P
+00000270: 7974 686f 6e20 3a3a 2033 2e36 0a43 6c61  ython :: 3.6.Cla
+00000280: 7373 6966 6965 723a 2050 726f 6772 616d  ssifier: Program
+00000290: 6d69 6e67 204c 616e 6775 6167 6520 3a3a  ming Language ::
+000002a0: 2050 7974 686f 6e20 3a3a 2033 2e37 0a43   Python :: 3.7.C
+000002b0: 6c61 7373 6966 6965 723a 2050 726f 6772  lassifier: Progr
+000002c0: 616d 6d69 6e67 204c 616e 6775 6167 6520  amming Language 
+000002d0: 3a3a 2050 7974 686f 6e20 3a3a 2033 2e38  :: Python :: 3.8
+000002e0: 0a44 6573 6372 6970 7469 6f6e 2d43 6f6e  .Description-Con
+000002f0: 7465 6e74 2d54 7970 653a 2074 6578 742f  tent-Type: text/
+00000300: 6d61 726b 646f 776e 0a4c 6963 656e 7365  markdown.License
+00000310: 2d46 696c 653a 204c 4943 454e 5345 0a0a  -File: LICENSE..
+00000320: 215b 5d28 6874 7470 733a 2f2f 696d 672e  ![](https://img.
+00000330: 7368 6965 6c64 732e 696f 2f70 7970 692f  shields.io/pypi/
+00000340: 7079 7665 7273 696f 6e73 2f61 6e67 6f72  pyversions/angor
+00000350: 6170 7929 0a21 5b5d 2868 7474 7073 3a2f  apy).![](https:/
+00000360: 2f69 6d67 2e73 6869 656c 6473 2e69 6f2f  /img.shields.io/
+00000370: 7079 7069 2f76 2f61 6e67 6f72 6170 7929  pypi/v/angorapy)
+00000380: 0a21 5b5d 2868 7474 7073 3a2f 2f69 6d67  .![](https://img
+00000390: 2e73 6869 656c 6473 2e69 6f2f 6769 7468  .shields.io/gith
+000003a0: 7562 2f6c 6963 656e 7365 2f63 636e 6d61  ub/license/ccnma
+000003b0: 6173 7472 6963 6874 2f61 6e67 6f72 6170  astricht/angorap
+000003c0: 7929 0a21 5b5d 2868 7474 7073 3a2f 2f69  y).![](https://i
+000003d0: 6d67 2e73 6869 656c 6473 2e69 6f2f 6769  mg.shields.io/gi
+000003e0: 7468 7562 2f73 7461 7273 2f63 636e 6d61  thub/stars/ccnma
+000003f0: 6173 7472 6963 6874 2f61 6e67 6f72 6170  astricht/angorap
+00000400: 7929 0a0a 0a3c 6272 202f 3e0a 3c62 7220  y)...<br />.<br 
+00000410: 2f3e 0a0a 3c70 2061 6c69 676e 3d22 6365  />..<p align="ce
+00000420: 6e74 6572 223e 3c69 6d67 2073 7263 3d22  nter"><img src="
+00000430: 646f 6373 2f69 6d67 2f61 6e67 6f72 6170  docs/img/angorap
+00000440: 792e 7376 6722 2077 6964 7468 3d32 3525  y.svg" width=25%
+00000450: 2061 6c69 676e 3d22 6365 6e74 6572 2220   align="center" 
+00000460: 2f3e 3c2f 703e 0a3c 6833 3e20 3c70 2061  /></p>.<h3> <p a
+00000470: 6c69 676e 3d22 6365 6e74 6572 223e 2041  lign="center"> A
+00000480: 6e74 6872 6f70 6f6d 6f72 7068 6963 2047  nthropomorphic G
+00000490: 6f61 6c2d 4f72 6965 6e74 6564 2052 6f62  oal-Oriented Rob
+000004a0: 6f74 6963 2043 6f6e 7472 6f6c 2066 6f72  otic Control for
+000004b0: 204e 6575 726f 7363 6965 6e74 6966 6963   Neuroscientific
+000004c0: 204d 6f64 656c 696e 6720 3c2f 703e 203c   Modeling </p> <
+000004d0: 2f68 333e 0a0a 3c62 7220 2f3e 0a20 2020  /h3>..<br />.   
+000004e0: 0a2a 2a41 6e67 6f72 6150 792a 2a20 6973  .**AngoraPy** is
+000004f0: 2061 6e20 6f70 656e 2073 6f75 7263 6520   an open source 
+00000500: 6d6f 6465 6c69 6e67 206c 6962 7261 7279  modeling library
+00000510: 2066 6f72 205b 676f 616c 2d6f 7269 656e   for [goal-orien
+00000520: 7465 6420 7265 7365 6172 6368 5d28 6874  ted research](ht
+00000530: 7470 733a 2f2f 7075 626d 6564 2e6e 6362  tps://pubmed.ncb
+00000540: 692e 6e6c 6d2e 6e69 682e 676f 762f 3236  i.nlm.nih.gov/26
+00000550: 3930 3635 3032 2f29 2069 6e20 2a2a 6e65  906502/) in **ne
+00000560: 7572 6f73 6369 656e 6365 2a2a 2e20 4974  uroscience**. It
+00000570: 2070 726f 7669 6465 7320 6120 7369 6d70   provides a simp
+00000580: 6c65 2069 6e74 6572 6661 6365 2074 6f20  le interface to 
+00000590: 7472 6169 6e20 6465 6570 206e 6575 7261  train deep neura
+000005a0: 6c20 6e65 7477 6f72 6b20 6d6f 6465 6c73  l network models
+000005b0: 206f 6620 7468 6520 6875 6d61 6e20 6272   of the human br
+000005c0: 6169 6e20 6f6e 2076 6172 696f 7573 2c20  ain on various, 
+000005d0: 6375 7374 6f6d 697a 6162 6c65 2c20 7365  customizable, se
+000005e0: 6e73 6f72 696d 6f74 6f72 2074 6173 6b73  nsorimotor tasks
+000005f0: 2c20 7573 696e 6720 7265 696e 666f 7263  , using reinforc
+00000600: 656d 656e 7420 6c65 6172 6e69 6e67 2e20  ement learning. 
+00000610: 4974 2074 6865 7265 6279 2065 6d70 6f77  It thereby empow
+00000620: 6572 7320 676f 616c 2d64 7269 7665 6e20  ers goal-driven 
+00000630: 6d6f 6465 6c69 6e67 2074 6f20 7375 7270  modeling to surp
+00000640: 6173 7320 7468 6520 7365 6e73 6f72 7920  ass the sensory 
+00000650: 646f 6d61 696e 2061 6e64 2065 6e74 6572  domain and enter
+00000660: 2074 6861 7420 6f66 2073 656e 736f 7269   that of sensori
+00000670: 5f6d 6f74 6f72 5f20 636f 6e74 726f 6c2c  _motor_ control,
+00000680: 2063 6c6f 7369 6e67 2074 6865 2070 6572   closing the per
+00000690: 6365 7074 696f 6e2d 6163 7469 6f6e 206c  ception-action l
+000006a0: 6f6f 702e 200a 0a2a 2a41 6e67 6f72 6150  oop. ..**AngoraP
+000006b0: 792a 2a20 6973 2064 6573 6967 6e65 6420  y** is designed 
+000006c0: 746f 2072 6571 7569 7265 206e 6f20 6465  to require no de
+000006d0: 6570 6572 2075 6e64 6572 7374 616e 6469  eper understandi
+000006e0: 6e67 206f 6620 7265 696e 666f 7263 656d  ng of reinforcem
+000006f0: 656e 7420 6c65 6172 6e69 6e67 2e20 4974  ent learning. It
+00000700: 2065 6d70 6c6f 7973 2073 7461 7465 2d6f   employs state-o
+00000710: 662d 7468 652d 6172 7420 6d61 6368 696e  f-the-art machin
+00000720: 6520 6c65 6172 6e69 6e67 2074 6563 686e  e learning techn
+00000730: 6971 7565 732c 206f 7074 696d 697a 6564  iques, optimized
+00000740: 2066 6f72 2064 6973 7472 6962 7574 6564   for distributed
+00000750: 2063 6f6d 7075 7461 7469 6f6e 2073 6361   computation sca
+00000760: 6c69 6e67 2066 726f 6d20 6c6f 6361 6c20  ling from local 
+00000770: 776f 726b 7374 6174 696f 6e73 2074 6f20  workstations to 
+00000780: 6869 6768 2d70 6572 666f 726d 616e 6365  high-performance
+00000790: 2063 6f6d 7075 7469 6e67 2063 6c75 7374   computing clust
+000007a0: 6572 732e 2057 6520 6169 6d20 746f 2068  ers. We aim to h
+000007b0: 6964 6520 6173 206d 7563 6820 6f66 2074  ide as much of t
+000007c0: 6869 7320 756e 6465 7220 7468 6520 686f  his under the ho
+000007d0: 6f64 206f 6620 616e 2069 6e74 7569 7469  od of an intuiti
+000007e0: 7665 2c20 6869 6768 2d6c 6576 656c 2041  ve, high-level A
+000007f0: 5049 2062 7574 2070 7265 7365 7276 6520  PI but preserve 
+00000800: 7468 6520 6f70 7469 6f6e 2066 6f72 2063  the option for c
+00000810: 7573 746f 6d69 7a69 6e67 206d 6f73 7420  ustomizing most 
+00000820: 6173 7065 6374 7320 6f66 2074 6865 2070  aspects of the p
+00000830: 6970 656c 696e 652e 0a0a 5468 6973 206c  ipeline...This l
+00000840: 6962 7261 7279 2069 7320 6465 7665 6c6f  ibrary is develo
+00000850: 7065 6420 6173 2070 6172 7420 6f66 2074  ped as part of t
+00000860: 6865 205b 4875 6d61 6e20 4272 6169 6e20  he [Human Brain 
+00000870: 5072 6f6a 6563 745d 2868 7474 7073 3a2f  Project](https:/
+00000880: 2f77 7777 2e68 756d 616e 6272 6169 6e70  /www.humanbrainp
+00000890: 726f 6a65 6374 2e65 752f 2920 6174 205b  roject.eu/) at [
+000008a0: 4343 4e20 4d61 6173 7472 6963 6874 5d28  CCN Maastricht](
+000008b0: 6874 7470 733a 2f2f 7777 772e 6363 6e6d  https://www.ccnm
+000008c0: 6161 7374 7269 6368 742e 636f 6d2f 292e  aastricht.com/).
+000008d0: 2049 7420 6973 2061 6e20 6566 666f 7274   It is an effort
+000008e0: 2074 6f20 6275 696c 6420 736f 6674 7761   to build softwa
+000008f0: 7265 2062 7920 6e65 7572 6f73 6369 656e  re by neuroscien
+00000900: 7469 7374 732c 2066 6f72 206e 6575 726f  tists, for neuro
+00000910: 7363 6965 6e74 6973 7473 2e20 4966 2079  scientists. If y
+00000920: 6f75 2068 6176 6520 7375 6767 6573 7469  ou have suggesti
+00000930: 6f6e 732c 2072 6571 7565 7374 7320 6f72  ons, requests or
+00000940: 2071 7565 7374 696f 6e73 2c20 6665 656c   questions, feel
+00000950: 2066 7265 6520 746f 205b 6f70 656e 2061   free to [open a
+00000960: 6e20 6973 7375 655d 2868 7474 7073 3a2f  n issue](https:/
+00000970: 2f67 6974 6875 622e 636f 6d2f 6363 6e6d  /github.com/ccnm
+00000980: 6161 7374 7269 6368 742f 616e 676f 7261  aastricht/angora
+00000990: 7079 2f69 7373 7565 732f 6e65 772f 6368  py/issues/new/ch
+000009a0: 6f6f 7365 292e 0a0a 215b 4d61 6e69 7075  oose)...![Manipu
+000009b0: 6c61 7469 6f6e 2047 6966 5d28 646f 6373  lation Gif](docs
+000009c0: 2f67 6966 732f 6d61 6e69 7075 6c61 7465  /gifs/manipulate
+000009d0: 5f62 6573 742e 6769 6629 0a0a 2323 20f0  _best.gif)..## .
+000009e0: 9f93 a520 496e 7374 616c 6c61 7469 6f6e  ... Installation
+000009f0: 0a0a 2323 2320 5072 6572 6571 7569 7369  ..### Prerequisi
+00000a00: 7465 730a 416e 676f 7261 5079 2072 6571  tes.AngoraPy req
+00000a10: 7569 7265 7320 5079 7468 6f6e 2033 2e36  uires Python 3.6
+00000a20: 206f 7220 6869 6768 6572 2e20 4974 2069   or higher. It i
+00000a30: 7320 7265 636f 6d6d 656e 6465 6420 746f  s recommended to
+00000a40: 2075 7365 2061 2076 6972 7475 616c 2065   use a virtual e
+00000a50: 6e76 6972 6f6e 6d65 6e74 2074 6f20 696e  nvironment to in
+00000a60: 7374 616c 6c20 416e 676f 7261 5079 2061  stall AngoraPy a
+00000a70: 6e64 2069 7473 2064 6570 656e 6465 6e63  nd its dependenc
+00000a80: 6965 732e 2041 6464 6974 696f 6e61 6c6c  ies. Additionall
+00000a90: 792c 2073 6f6d 6520 7072 6572 6571 7569  y, some prerequi
+00000aa0: 7369 7465 7320 6172 6520 7265 7175 6972  sites are requir
+00000ab0: 6564 2e20 0a0a 4f6e 2055 6275 6e74 752c  ed. ..On Ubuntu,
+00000ac0: 2074 6865 7365 2063 616e 2062 6520 696e   these can be in
+00000ad0: 7374 616c 6c65 6420 6279 2072 756e 6e69  stalled by runni
+00000ae0: 6e67 0a0a 2020 2020 7375 646f 2061 7074  ng..    sudo apt
+00000af0: 2d67 6574 2069 6e73 7461 6c6c 2073 7769  -get install swi
+00000b00: 670a 0a41 6464 6974 696f 6e61 6c6c 792c  g..Additionally,
+00000b10: 2074 6f20 7275 6e20 416e 676f 7261 5079   to run AngoraPy
+00000b20: 2077 6974 6820 6974 7320 6e61 7469 7665   with its native
+00000b30: 2064 6973 7472 6962 7574 696f 6e2c 2079   distribution, y
+00000b40: 6f75 206e 6565 6420 4d50 4920 696e 7374  ou need MPI inst
+00000b50: 616c 6c65 642e 204f 6e20 5562 756e 7475  alled. On Ubuntu
+00000b60: 2c20 7468 6973 2063 616e 2062 6520 646f  , this can be do
+00000b70: 6e65 2062 7920 7275 6e6e 696e 670a 0a20  ne by running.. 
+00000b80: 2020 2073 7564 6f20 6170 742d 6765 7420     sudo apt-get 
+00000b90: 696e 7374 616c 6c20 6c69 626f 7065 6e6d  install libopenm
+00000ba0: 7069 2d64 6576 0a0a 486f 7765 7665 722c  pi-dev..However,
+00000bb0: 2061 6e79 206f 7468 6572 204d 5049 2069   any other MPI i
+00000bc0: 6d70 6c65 6d65 6e74 6174 696f 6e20 7368  mplementation sh
+00000bd0: 6f75 6c64 2077 6f72 6b20 6173 2077 656c  ould work as wel
+00000be0: 6c2e 0a0a 2323 2320 496e 7374 616c 6c69  l...### Installi
+00000bf0: 6e67 2041 6e67 6f72 6150 790a 0a23 2323  ng AngoraPy..###
+00000c00: 2320 4269 6e61 7269 6573 0a41 6e67 6f72  # Binaries.Angor
+00000c10: 6150 7920 6973 2061 7661 696c 6162 6c65  aPy is available
+00000c20: 2061 7320 6120 6269 6e61 7279 2070 6163   as a binary pac
+00000c30: 6b61 6765 206f 6e20 5079 5049 2e20 546f  kage on PyPI. To
+00000c40: 2069 6e73 7461 6c6c 2069 742c 2072 756e   install it, run
+00000c50: 200a 0a20 2020 2070 6970 2069 6e73 7461   ..    pip insta
+00000c60: 6c6c 2061 6e67 6f72 6170 790a 0a69 6e20  ll angorapy..in 
+00000c70: 796f 7572 2074 6572 6d69 6e61 6c2e 0a0a  your terminal...
+00000c80: 4966 2079 6f75 2077 6f75 6c64 206c 696b  If you would lik
+00000c90: 6520 746f 2069 6e73 7461 6c6c 2061 2073  e to install a s
+00000ca0: 7065 6369 6669 6320 7665 7273 696f 6e2c  pecific version,
+00000cb0: 2079 6f75 2063 616e 2073 7065 6369 6679   you can specify
+00000cc0: 2069 7420 6279 2061 7070 656e 6469 6e67   it by appending
+00000cd0: 2060 3d3d 3c76 6572 7369 6f6e 3e60 2074   `==<version>` t
+00000ce0: 6f20 7468 6520 636f 6d6d 616e 6420 6162  o the command ab
+00000cf0: 6f76 652e 2046 6f72 2065 7861 6d70 6c65  ove. For example
+00000d00: 2c20 746f 2069 6e73 7461 6c6c 2076 6572  , to install ver
+00000d10: 7369 6f6e 2030 2e39 2e30 2c20 7275 6e20  sion 0.9.0, run 
+00000d20: 0a0a 2020 2020 7069 7020 696e 7374 616c  ..    pip instal
+00000d30: 6c20 616e 676f 7261 7079 3d3d 302e 392e  l angorapy==0.9.
+00000d40: 300a 0a23 2323 2320 536f 7572 6365 2049  0..#### Source I
+00000d50: 6e73 7461 6c6c 6174 696f 6e0a 546f 2069  nstallation.To i
+00000d60: 6e73 7461 6c6c 2041 6e67 6f72 6150 7920  nstall AngoraPy 
+00000d70: 6672 6f6d 2073 6f75 7263 652c 2063 6c6f  from source, clo
+00000d80: 6e65 2074 6865 2072 6570 6f73 6974 6f72  ne the repositor
+00000d90: 7920 616e 6420 7275 6e20 6070 6970 2069  y and run `pip i
+00000da0: 6e73 7461 6c6c 202d 6520 2e60 2069 6e20  nstall -e .` in 
+00000db0: 7468 6520 726f 6f74 2064 6972 6563 746f  the root directo
+00000dc0: 7279 2e0a 0a23 2323 2050 6f73 742d 496e  ry...### Post-In
+00000dd0: 7374 616c 6c61 7469 6f6e 0a0a 2323 2323  stallation..####
+00000de0: 204d 754a 6f43 6f0a 4779 6d20 696e 7374   MuJoCo.Gym inst
+00000df0: 616c 6c73 2062 6f74 6820 4d75 4a6f 436f  alls both MuJoCo
+00000e00: 2773 206e 6577 206e 6174 6976 6520 5079  's new native Py
+00000e10: 7468 6f6e 2062 696e 6469 6e67 7320 616e  thon bindings an
+00000e20: 6420 7468 6520 6f6c 6420 6d75 6a6f 636f  d the old mujoco
+00000e30: 2d70 7920 6269 6e64 696e 6773 2e20 596f  -py bindings. Yo
+00000e40: 7520 7769 6c6c 206e 6f74 206e 6565 6420  u will not need 
+00000e50: 7468 6520 6c61 7474 6572 2066 6f72 2041  the latter for A
+00000e60: 6e67 6f72 6150 792c 2073 6f20 796f 7520  ngoraPy, so you 
+00000e70: 6d61 7920 756e 696e 7374 616c 6c20 6974  may uninstall it
+00000e80: 2062 7920 7275 6e6e 696e 670a 0a20 2020   by running..   
+00000e90: 2070 6970 2075 6e69 6e73 7461 6c6c 206d   pip uninstall m
+00000ea0: 756a 6f63 6f2d 7079 0a0a 2323 2323 2054  ujoco-py..#### T
+00000eb0: 6573 7420 596f 7572 2049 6e73 7461 6c6c  est Your Install
+00000ec0: 6174 696f 6e0a 596f 7520 6361 6e20 7465  ation.You can te
+00000ed0: 7374 2079 6f75 7220 696e 7374 616c 6c61  st your installa
+00000ee0: 7469 6f6e 2062 7920 7275 6e6e 696e 6720  tion by running 
+00000ef0: 7468 6520 666f 6c6c 6f77 696e 6720 636f  the following co
+00000f00: 6d6d 616e 6420 696e 2079 6f75 7220 7465  mmand in your te
+00000f10: 726d 696e 616c 3a0a 0a20 2020 2070 7974  rminal:..    pyt
+00000f20: 686f 6e20 2d6d 2061 6e67 6f72 6170 792e  hon -m angorapy.
+00000f30: 7472 6169 6e20 4361 7274 506f 6c65 2d76  train CartPole-v
+00000f40: 310a 0a54 6f20 7465 7374 2079 6f75 7220  1..To test your 
+00000f50: 4d50 4920 696e 7374 616c 6c61 7469 6f6e  MPI installation
+00000f60: 2c20 7275 6e0a 0a20 2020 206d 7069 7275  , run..    mpiru
+00000f70: 6e20 2d6e 7020 3c6e 756d 7468 7265 6164  n -np <numthread
+00000f80: 733e 202d 2d75 7365 2d68 7774 6872 6561  s> --use-hwthrea
+00000f90: 642d 6370 7573 2070 7974 686f 6e20 2d6d  d-cpus python -m
+00000fa0: 2061 6e67 6f72 6170 792e 7472 6169 6e20   angorapy.train 
+00000fb0: 4c75 6e61 724c 616e 6465 7243 6f6e 7469  LunarLanderConti
+00000fc0: 6e75 6f75 732d 7632 0a0a 7768 6572 6520  nuous-v2..where 
+00000fd0: 603c 6e75 6d74 6872 6561 6473 3e60 2069  `<numthreads>` i
+00000fe0: 7320 7468 6520 6e75 6d62 6572 206f 6620  s the number of 
+00000ff0: 7468 7265 6164 7320 796f 7520 7761 6e74  threads you want
+00001000: 2074 6f20 2861 6e64 2063 616e 2920 7573   to (and can) us
+00001010: 652e 0a0a 2323 2320 446f 636b 6572 0a41  e...### Docker.A
+00001020: 6c74 6572 6e61 7469 7665 6c79 2c20 796f  lternatively, yo
+00001030: 7520 6361 6e20 696e 7374 616c 6c20 416e  u can install An
+00001040: 676f 7261 5079 2061 6e64 2061 6c6c 2069  goraPy and all i
+00001050: 7473 2064 6570 656e 6465 6e63 6965 7320  ts dependencies 
+00001060: 696e 2061 2064 6f63 6b65 7220 636f 6e74  in a docker cont
+00001070: 6169 6e65 7220 7573 696e 6720 7468 6520  ainer using the 
+00001080: 446f 636b 6572 6669 6c65 2070 726f 7669  Dockerfile provi
+00001090: 6465 6420 696e 2074 6869 7320 7265 706f  ded in this repo
+000010a0: 7369 746f 7279 2028 2f64 6f63 6b65 722f  sitory (/docker/
+000010b0: 446f 636b 6572 6669 6c65 292e 2054 6f20  Dockerfile). To 
+000010c0: 7468 6973 2065 6e64 2c20 646f 776e 6c6f  this end, downlo
+000010d0: 6164 2074 6865 2072 6570 6f73 6974 6f72  ad the repositor
+000010e0: 7920 616e 6420 6275 696c 6420 7468 6520  y and build the 
+000010f0: 646f 636b 6572 2069 6d61 6765 2066 726f  docker image fro
+00001100: 6d20 7468 6520 2f64 6f63 6b65 7220 6469  m the /docker di
+00001110: 7265 6374 6f72 793a 0a0a 6060 6062 6173  rectory:..```bas
+00001120: 680a 7375 646f 2064 6f63 6b65 7220 6275  h.sudo docker bu
+00001130: 696c 6420 2d74 2061 6e67 6f72 6170 793a  ild -t angorapy:
+00001140: 6d61 7374 6572 2068 7474 7073 3a2f 2f67  master https://g
+00001150: 6974 6875 622e 636f 6d2f 6363 6e6d 6161  ithub.com/ccnmaa
+00001160: 7374 7269 6368 742f 616e 676f 7261 7079  stricht/angorapy
+00001170: 2e67 6974 236d 6173 7465 7220 2d66 202d  .git#master -f -
+00001180: 203c 2044 6f63 6b65 7266 696c 650a 6060   < Dockerfile.``
+00001190: 600a 0a54 6f20 696e 7374 616c 6c20 6469  `..To install di
+000011a0: 6666 6572 656e 7420 7665 7273 696f 6e73  fferent versions
+000011b0: 2c20 7265 706c 6163 6520 6023 6d61 7374  , replace `#mast
+000011c0: 6572 6020 696e 2074 6865 2073 6f75 7263  er` in the sourc
+000011d0: 6520 6279 2074 6865 2074 6167 2f62 7261  e by the tag/bra
+000011e0: 6e63 6820 6f66 2074 6865 2072 6573 7065  nch of the respe
+000011f0: 6374 6976 6520 7665 7273 696f 6e20 796f  ctive version yo
+00001200: 7520 7761 6e74 2074 6f20 696e 7374 616c  u want to instal
+00001210: 6c2e 0a0a 2323 20f0 9f9a 8020 4765 7474  l...## .... Gett
+00001220: 696e 6720 5374 6172 7465 640a 5468 6520  ing Started.The 
+00001230: 7363 7269 7074 7320 6074 7261 696e 2e70  scripts `train.p
+00001240: 7960 2c20 6065 7661 6c75 6174 652e 7079  y`, `evaluate.py
+00001250: 6020 616e 6420 606f 6273 6572 7665 2e70  ` and `observe.p
+00001260: 7960 2070 726f 7669 6465 2072 6561 6479  y` provide ready
+00001270: 2d6d 6164 6520 7363 7269 7074 7320 666f  -made scripts fo
+00001280: 7220 7472 6169 6e69 6e67 2061 6e64 2065  r training and e
+00001290: 7661 6c75 6174 696e 6720 616e 2061 6765  valuating an age
+000012a0: 6e74 2069 6e20 616e 7920 656e 7669 726f  nt in any enviro
+000012b0: 6e6d 656e 742e 2057 6974 6820 6070 7265  nment. With `pre
+000012c0: 7472 6169 6e2e 7079 602c 2069 7420 6973  train.py`, it is
+000012d0: 2070 6f73 7369 626c 6520 746f 2070 7265   possible to pre
+000012e0: 7472 6169 6e20 7468 6520 7669 7375 616c  train the visual
+000012f0: 2063 6f6d 706f 6e65 6e74 2e20 6062 656e   component. `ben
+00001300: 6368 6d61 726b 2e70 7960 2070 726f 7669  chmark.py` provi
+00001310: 6465 7320 6675 6e63 7469 6f6e 616c 6974  des functionalit
+00001320: 7920 666f 7220 7472 6169 6e69 6e67 2061  y for training a
+00001330: 2062 6174 6368 206f 6620 6167 656e 7473   batch of agents
+00001340: 2070 6f73 7369 626c 7920 7573 696e 6720   possibly using 
+00001350: 6469 6666 6572 656e 7420 636f 6e66 6967  different config
+00001360: 7320 666f 7220 636f 6d70 6172 6973 6f6e  s for comparison
+00001370: 206f 6620 7374 7261 7465 6769 6573 2e0a   of strategies..
+00001380: 0a23 2323 2054 7261 696e 696e 6720 616e  .### Training an
+00001390: 2041 6765 6e74 0a54 6865 2060 7472 6169   Agent.The `trai
+000013a0: 6e2e 7079 6020 636f 6d6d 616e 646c 696e  n.py` commandlin
+000013b0: 6520 696e 7465 7266 6163 6520 7072 6f76  e interface prov
+000013c0: 6964 6573 2061 2063 6f6e 7665 6e69 656e  ides a convenien
+000013d0: 7420 656e 7472 792d 706f 696e 7420 666f  t entry-point fo
+000013e0: 7220 7275 6e6e 696e 6720 616c 6c20 736f  r running all so
+000013f0: 7274 7320 6f66 2065 7870 6572 696d 656e  rts of experimen
+00001400: 7473 2075 7369 6e67 2074 6865 2062 7569  ts using the bui
+00001410: 6c74 696e 206d 6f64 656c 7320 616e 6420  ltin models and 
+00001420: 656e 7669 726f 6e6d 656e 7473 2069 6e20  environments in 
+00001430: 616e 676f 7261 7079 2e20 596f 7520 6361  angorapy. You ca
+00001440: 6e20 7472 6169 6e20 616e 2061 6765 6e74  n train an agent
+00001450: 206f 6e20 616e 7920 656e 7669 726f 6e6d   on any environm
+00001460: 656e 7420 7769 7468 206f 7074 696f 6e61  ent with optiona
+00001470: 6c20 6879 7065 7270 6172 616d 6574 6572  l hyperparameter
+00001480: 732e 2041 6464 6974 696f 6e61 6c6c 792c  s. Additionally,
+00001490: 2061 206d 6f6e 6974 6f72 2077 696c 6c20   a monitor will 
+000014a0: 6265 2061 7574 6f6d 6174 6963 616c 6c79  be automatically
+000014b0: 206c 696e 6b65 6420 746f 2074 6865 2074   linked to the t
+000014c0: 7261 696e 696e 6720 6f66 2074 6865 2061  raining of the a
+000014d0: 6765 6e74 2e20 466f 7220 6d6f 7265 2064  gent. For more d
+000014e0: 6574 6169 6c20 636f 6e73 756c 7420 7468  etail consult th
+000014f0: 6520 3c61 2068 7265 663d 226d 6f6e 6974  e <a href="monit
+00001500: 6f72 2f52 4541 444d 452e 6d64 223e 5245  or/README.md">RE
+00001510: 4144 4d45 206f 6e20 6d6f 6e69 746f 7269  ADME on monitori
+00001520: 6e67 3c2f 613e 2e0a 0a42 6173 6520 7573  ng</a>...Base us
+00001530: 6167 6520 6f66 2060 7472 6169 6e2e 7079  age of `train.py
+00001540: 6020 6973 2061 7320 666f 6c6c 6f77 733a  ` is as follows:
+00001550: 0a0a 2020 2020 7079 7468 6f6e 2074 7261  ..    python tra
+00001560: 696e 2e70 7920 454e 5620 2d2d 6172 6368  in.py ENV --arch
+00001570: 6974 6563 7475 7265 204d 4f44 454c 0a20  itecture MODEL. 
+00001580: 2020 200a 466f 7220 696e 7374 616e 6365     .For instance
+00001590: 2c20 7472 6169 6e69 6e67 2060 4c75 6e61  , training `Luna
+000015a0: 724c 616e 6465 7243 6f6e 7469 6e75 6f75  rLanderContinuou
+000015b0: 732d 7632 6020 7573 696e 6720 7468 6520  s-v2` using the 
+000015c0: 6064 6565 7065 7260 2061 7263 6869 7465  `deeper` archite
+000015d0: 6374 7572 6520 6973 2070 6f73 7369 626c  cture is possibl
+000015e0: 6520 6279 2072 756e 6e69 6e67 3a0a 0a20  e by running:.. 
+000015f0: 2020 2070 7974 686f 6e20 7472 6169 6e2e     python train.
+00001600: 7079 204c 756e 6172 4c61 6e64 6572 436f  py LunarLanderCo
+00001610: 6e74 696e 756f 7573 2d76 3220 2d2d 6172  ntinuous-v2 --ar
+00001620: 6368 6974 6563 7475 7265 2064 6565 7065  chitecture deepe
+00001630: 720a 2020 2020 0a46 6f72 206d 6f72 6520  r.    .For more 
+00001640: 6164 7661 6e63 6564 206f 7074 696f 6e73  advanced options
+00001650: 206c 696b 6520 6375 7374 6f6d 2068 7970   like custom hyp
+00001660: 6572 7061 7261 6d65 7465 7273 2c20 636f  erparameters, co
+00001670: 6e73 756c 740a 0a20 2020 2070 7974 686f  nsult..    pytho
+00001680: 6e20 7472 6169 6e2e 7079 202d 680a 0a0a  n train.py -h...
+00001690: 2323 2320 4576 616c 7561 7469 6e67 2061  ### Evaluating a
+000016a0: 6e64 204f 6273 6572 7669 6e67 2061 6e20  nd Observing an 
+000016b0: 4167 656e 740a 5468 6572 6520 6172 6520  Agent.There are 
+000016c0: 7477 6f20 6d6f 7265 2065 6e74 7279 2070  two more entry p
+000016d0: 6f69 6e74 7320 666f 7220 6576 616c 7561  oints for evalua
+000016e0: 7469 6e67 2061 6e64 206f 6273 6572 7669  ting and observi
+000016f0: 6e67 2061 6e20 6167 656e 743a 2060 6576  ng an agent: `ev
+00001700: 616c 7561 7465 2e70 7960 2061 6e64 2060  aluate.py` and `
+00001710: 6f62 7365 7276 652e 7079 602e 2047 656e  observe.py`. Gen
+00001720: 6572 616c 2075 7361 6765 2069 7320 6173  eral usage is as
+00001730: 2066 6f6c 6c6f 7773 0a0a 2020 2020 7079   follows..    py
+00001740: 7468 6f6e 2065 7661 6c75 6174 652e 7079  thon evaluate.py
+00001750: 2049 440a 0a57 6865 7265 2049 4420 6973   ID..Where ID is
+00001760: 2074 6865 2061 6765 6e74 2773 2049 4420   the agent's ID 
+00001770: 6769 7665 6e20 7768 656e 2069 7473 2063  given when its c
+00001780: 7265 6174 6564 2028 6074 7261 696e 2e70  reated (`train.p
+00001790: 7960 2070 7269 6e74 7320 7468 6973 206f  y` prints this o
+000017a0: 7574 742c 2069 6e20 6375 7374 6f6d 2073  utt, in custom s
+000017b0: 6372 6970 7473 2067 6574 2069 7420 7769  cripts get it wi
+000017c0: 7468 2060 6167 656e 742e 6167 656e 745f  th `agent.agent_
+000017d0: 6964 6029 2e0a 0a23 2323 2057 7269 7469  id`)...### Writi
+000017e0: 6e67 2061 2054 7261 696e 696e 6720 5363  ng a Training Sc
+000017f0: 7269 7074 0a54 6f20 7472 6169 6e20 6167  ript.To train ag
+00001800: 656e 7473 2077 6974 6820 6375 7374 6f6d  ents with custom
+00001810: 206d 6f64 656c 732c 2065 6e76 6972 6f6e   models, environ
+00001820: 6d65 6e74 732c 2065 7463 2e20 796f 7520  ments, etc. you 
+00001830: 7772 6974 6520 796f 7572 206f 776e 2073  write your own s
+00001840: 6372 6970 742e 2054 6865 2066 6f6c 6c6f  cript. The follo
+00001850: 7769 6e67 2069 7320 6120 6d69 6e69 6d61  wing is a minima
+00001860: 6c20 6578 616d 706c 653a 0a0a 6060 6070  l example:..```p
+00001870: 7974 686f 6e0a 6672 6f6d 2061 6e67 6f72  ython.from angor
+00001880: 6170 792e 636f 6d6d 6f6e 2e77 7261 7070  apy.common.wrapp
+00001890: 6572 7320 696d 706f 7274 206d 616b 655f  ers import make_
+000018a0: 656e 760a 6672 6f6d 2061 6e67 6f72 6170  env.from angorap
+000018b0: 792e 6d6f 6465 6c73 2069 6d70 6f72 7420  y.models import 
+000018c0: 6765 745f 6d6f 6465 6c5f 6275 696c 6465  get_model_builde
+000018d0: 720a 6672 6f6d 2061 6e67 6f72 6170 792e  r.from angorapy.
+000018e0: 6167 656e 742e 7070 6f5f 6167 656e 7420  agent.ppo_agent 
+000018f0: 696d 706f 7274 2050 504f 4167 656e 740a  import PPOAgent.
+00001900: 0a65 6e76 203d 206d 616b 655f 656e 7628  .env = make_env(
+00001910: 2252 6561 6368 4162 736f 6c75 7465 2d76  "ReachAbsolute-v
+00001920: 3022 290a 6d6f 6465 6c5f 6275 696c 6465  0").model_builde
+00001930: 7220 3d20 6765 745f 6d6f 6465 6c5f 6275  r = get_model_bu
+00001940: 696c 6465 7228 2273 6861 646f 7722 2c20  ilder("shadow", 
+00001950: 226c 7374 6d22 290a 6167 656e 7420 3d20  "lstm").agent = 
+00001960: 5050 4f41 6765 6e74 286d 6f64 656c 5f62  PPOAgent(model_b
+00001970: 7569 6c64 6572 2c20 656e 762c 2077 6f72  uilder, env, wor
+00001980: 6b65 7273 3d32 3429 0a61 6765 6e74 2e64  kers=24).agent.d
+00001990: 7269 6c6c 286e 3d31 3030 2c20 6570 6f63  rill(n=100, epoc
+000019a0: 6873 3d31 302c 2062 6174 6368 5f73 697a  hs=10, batch_siz
+000019b0: 653d 3531 3229 0a60 6060 0a0a 466f 7220  e=512).```..For 
+000019c0: 6d6f 7265 2064 6574 6169 6c73 2c20 636f  more details, co
+000019d0: 6e73 756c 7420 7468 6520 5b65 7861 6d70  nsult the [examp
+000019e0: 6c65 735d 2865 7861 6d70 6c65 7329 2e0a  les](examples)..
+000019f0: 0a23 2320 f09f 8e93 2044 6f63 756d 656e  .## .... Documen
+00001a00: 7461 7469 6f6e 0a57 6520 7072 6f76 6964  tation.We provid
+00001a10: 6520 5b65 7861 6d70 6c65 735d 2865 7861  e [examples](exa
+00001a20: 6d70 6c65 7329 2074 6861 7420 6765 7420  mples) that get 
+00001a30: 796f 7520 7374 6172 7465 6420 7769 7468  you started with
+00001a40: 2077 7269 7469 6e67 2079 6f75 7220 6f77   writing your ow
+00001a50: 6e20 7363 7269 7074 7320 7573 696e 6720  n scripts using 
+00001a60: 416e 676f 7261 5079 2e20 4164 6469 7469  AngoraPy. Additi
+00001a70: 6f6e 616c 6c79 2074 6865 7265 2069 7320  onally there is 
+00001a80: 6120 6772 6f77 696e 6720 6c69 7374 206f  a growing list o
+00001a90: 6620 5b74 7574 6f72 6961 6c73 5d28 6874  f [tutorials](ht
+00001aa0: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
+00001ab0: 2f77 6569 646c 6572 2f61 6e67 6f72 6170  /weidler/angorap
+00001ac0: 792d 7475 746f 7269 616c 7329 2e20 4966  y-tutorials). If
+00001ad0: 2079 6f75 2061 7265 206d 6973 7369 6e67   you are missing
+00001ae0: 2061 2064 6f63 756d 656e 7461 7469 6f6e   a documentation
+00001af0: 2066 6f72 2061 2073 7065 6369 6669 6320   for a specific 
+00001b00: 7061 7274 206f 6620 416e 676f 7261 5079  part of AngoraPy
+00001b10: 2c20 6665 656c 2066 7265 6520 746f 206f  , feel free to o
+00001b20: 7065 6e20 616e 2069 7373 7565 2061 6e64  pen an issue and
+00001b30: 2077 6520 7769 6c6c 2064 6f20 6f75 7220   we will do our 
+00001b40: 6265 7374 2074 6f20 6164 6420 6974 2e0a  best to add it..
+00001b50: 0a23 2320 f09f 9480 2044 6973 7472 6962  .## .... Distrib
+00001b60: 7574 6564 2043 6f6d 7075 7461 7469 6f6e  uted Computation
+00001b70: 0a50 504f 2069 7320 616e 2061 7379 6e63  .PPO is an async
+00001b80: 6872 6f6e 6f75 7320 616c 676f 7269 7468  hronous algorith
+00001b90: 6d2c 2061 6c6c 6f77 696e 6720 6d75 6c74  m, allowing mult
+00001ba0: 6970 6c65 2070 6172 616c 6c65 6c20 776f  iple parallel wo
+00001bb0: 726b 6572 7320 746f 2067 656e 6572 6174  rkers to generat
+00001bc0: 6520 6578 7065 7269 656e 6365 2069 6e64  e experience ind
+00001bd0: 6570 656e 6465 6e74 6c79 2e20 0a57 6520  ependently. .We 
+00001be0: 616c 6c6f 7720 7061 7261 6c6c 656c 2067  allow parallel g
+00001bf0: 6174 6865 7269 6e67 2061 6e64 206f 7074  athering and opt
+00001c00: 696d 697a 6174 696f 6e20 7468 726f 7567  imization throug
+00001c10: 6820 4d50 492e 2041 6765 6e74 7320 7769  h MPI. Agents wi
+00001c20: 6c6c 2061 7574 6f6d 6174 6963 616c 6c79  ll automatically
+00001c30: 2064 6973 7472 6962 7574 6520 7468 6569   distribute thei
+00001c40: 7220 776f 726b 6572 7320 6576 656e 6c79  r workers evenly
+00001c50: 206f 6e20 0a74 6865 2061 7661 696c 6162   on .the availab
+00001c60: 6c65 2043 5055 2063 6f72 6573 2c20 7768  le CPU cores, wh
+00001c70: 696c 6520 6f70 7469 6d69 7a61 7469 6f6e  ile optimization
+00001c80: 2069 7320 6469 7374 7269 6275 7465 6420   is distributed 
+00001c90: 6f76 6572 2061 6c6c 2061 7661 696c 6162  over all availab
+00001ca0: 6c65 2047 5055 732e 2049 6620 6e6f 2047  le GPUs. If no G
+00001cb0: 5055 7320 6172 6520 6176 6169 6c61 626c  PUs are availabl
+00001cc0: 652c 2061 6c6c 2043 5055 7320 0a73 6861  e, all CPUs .sha
+00001cd0: 7265 2074 6865 2074 6173 6b20 6f66 206f  re the task of o
+00001ce0: 7074 696d 697a 696e 672e 0a0a 4469 7374  ptimizing...Dist
+00001cf0: 7269 6275 7469 6f6e 2069 7320 706f 7373  ribution is poss
+00001d00: 6962 6c65 206c 6f63 616c 6c79 206f 6e20  ible locally on 
+00001d10: 796f 7572 2077 6f72 6b73 7461 7469 6f6e  your workstation
+00001d20: 2061 6e64 206f 6e20 4850 4320 7369 7465   and on HPC site
+00001d30: 732e 200a 0a23 2323 20f0 9f92 bb20 4c6f  s. ..### .... Lo
+00001d40: 6361 6c20 4469 7374 7269 6275 7465 6420  cal Distributed 
+00001d50: 436f 6d70 7574 696e 6720 7769 7468 204d  Computing with M
+00001d60: 5049 0a54 6f20 7573 6520 4d50 4920 6c6f  PI.To use MPI lo
+00001d70: 6361 6c6c 792c 2079 6f75 206e 6565 6420  cally, you need 
+00001d80: 746f 2068 6176 6520 6120 7275 6e6e 696e  to have a runnin
+00001d90: 6720 4d50 4920 696d 706c 656d 656e 7461  g MPI implementa
+00001da0: 7469 6f6e 2c20 652e 672e 204f 7065 6e20  tion, e.g. Open 
+00001db0: 4d50 4920 3420 6f6e 2055 6275 6e74 752e  MPI 4 on Ubuntu.
+00001dc0: 0a54 6f20 6578 6563 7574 6520 6074 7261  .To execute `tra
+00001dd0: 696e 2e70 7960 2076 6961 204d 5049 2c20  in.py` via MPI, 
+00001de0: 7275 6e0a 0a60 6060 6261 7368 0a6d 7069  run..```bash.mpi
+00001df0: 7275 6e20 2d6e 7020 3132 202d 2d75 7365  run -np 12 --use
+00001e00: 2d68 7774 6872 6561 642d 6370 7573 2070  -hwthread-cpus p
+00001e10: 7974 686f 6e33 2074 7261 696e 2e70 7920  ython3 train.py 
+00001e20: 2e2e 2e0a 6060 600a 0a77 6865 7265 2c20  ....```..where, 
+00001e30: 696e 2074 6869 7320 6578 616d 706c 652c  in this example,
+00001e40: 2031 3220 6973 2074 6865 206e 756d 6265   12 is the numbe
+00001e50: 7220 6f66 206c 6f63 616c 6c79 2061 7661  r of locally ava
+00001e60: 696c 6162 6c65 2043 5055 2074 6872 6561  ilable CPU threa
+00001e70: 6473 2061 6e64 2060 2d2d 7573 652d 6877  ds and `--use-hw
+00001e80: 7468 7265 6164 2d63 7075 7360 0a6d 616b  thread-cpus`.mak
+00001e90: 6573 2061 7661 696c 6162 6c65 2074 6872  es available thr
+00001ea0: 6561 6473 2028 6173 206f 7070 6f73 6564  eads (as opposed
+00001eb0: 2074 6f20 6f6e 6c79 2063 6f72 6573 292e   to only cores).
+00001ec0: 2055 7361 6765 206f 6620 6074 7261 696e   Usage of `train
+00001ed0: 2e70 7960 2069 7320 6173 2064 6573 6372  .py` is as descr
+00001ee0: 6962 6564 2070 7265 7669 6f75 736c 792e  ibed previously.
+00001ef0: 0a0a 2323 2320 3a63 6c6f 7564 3a20 4469  ..### :cloud: Di
+00001f00: 7374 7269 6275 7465 6420 5472 6169 6e69  stributed Traini
+00001f10: 6e67 206f 6e20 534c 5552 4d2d 6261 7365  ng on SLURM-base
+00001f20: 6420 4850 4320 636c 7573 7465 7273 0a2a  d HPC clusters.*
+00001f30: 506c 6561 7365 206e 6f74 6520 7468 6174  Please note that
+00001f40: 2074 6865 2066 6f6c 6c6f 7769 6e67 2069   the following i
+00001f50: 7320 6f70 7469 6d69 7a65 6420 616e 6420  s optimized and 
+00001f60: 7465 7374 6564 206f 6e20 7468 6520 7370  tested on the sp
+00001f70: 6563 6966 6963 2063 6c75 7374 6572 2077  ecific cluster w
+00001f80: 6520 7573 652c 2062 7574 2073 686f 756c  e use, but shoul
+00001f90: 6420 6578 7465 6e64 2074 6f20 6174 206c  d extend to at l
+00001fa0: 6561 7374 200a 616e 7920 534c 5552 4d20  east .any SLURM 
+00001fb0: 6261 7365 6420 7365 7475 702e 2a0a 0a4f  based setup.*..O
+00001fc0: 6e20 616e 7920 534c 5552 4d2d 6261 7365  n any SLURM-base
+00001fd0: 6420 4850 4320 636c 7573 7465 7220 796f  d HPC cluster yo
+00001fe0: 7520 6d61 7920 7375 626d 6974 2079 6f75  u may submit you
+00001ff0: 7220 6a6f 6220 7769 7468 2073 6261 7463  r job with sbatc
+00002000: 6820 7573 6973 696e 6720 7468 6520 666f  h usising the fo
+00002010: 6c6c 6f77 696e 6720 7363 7269 7074 2074  llowing script t
+00002020: 656d 706c 6174 653a 0a0a 6060 6062 6173  emplate:..```bas
+00002030: 680a 2321 2f62 696e 2f62 6173 6820 2d6c  h.#!/bin/bash -l
+00002040: 0a23 5342 4154 4348 202d 2d6a 6f62 2d6e  .#SBATCH --job-n
+00002050: 616d 653d 2261 6e67 6f72 6170 7922 0a23  ame="angorapy".#
+00002060: 5342 4154 4348 202d 2d61 6363 6f75 6e74  SBATCH --account
+00002070: 3d78 7878 0a23 5342 4154 4348 202d 2d74  =xxx.#SBATCH --t
+00002080: 696d 653d 3234 3a30 303a 3030 0a23 5342  ime=24:00:00.#SB
+00002090: 4154 4348 202d 2d6e 6f64 6573 3d33 320a  ATCH --nodes=32.
+000020a0: 2353 4241 5443 4820 2d2d 6e74 6173 6b73  #SBATCH --ntasks
+000020b0: 2d70 6572 2d63 6f72 653d 310a 2353 4241  -per-core=1.#SBA
+000020c0: 5443 4820 2d2d 6e74 6173 6b73 2d70 6572  TCH --ntasks-per
+000020d0: 2d6e 6f64 653d 3132 0a23 5342 4154 4348  -node=12.#SBATCH
+000020e0: 202d 2d63 7075 732d 7065 722d 7461 736b   --cpus-per-task
+000020f0: 3d31 0a23 5342 4154 4348 202d 2d70 6172  =1.#SBATCH --par
+00002100: 7469 7469 6f6e 3d6e 6f72 6d61 6c0a 2353  tition=normal.#S
+00002110: 4241 5443 4820 2d2d 636f 6e73 7472 6169  BATCH --constrai
+00002120: 6e74 3d67 7075 2673 7461 7274 780a 2353  nt=gpu&startx.#S
+00002130: 4241 5443 4820 2d2d 6869 6e74 3d6e 6f6d  BATCH --hint=nom
+00002140: 756c 7469 7468 7265 6164 0a0a 6578 706f  ultithread..expo
+00002150: 7274 204f 4d50 5f4e 554d 5f54 4852 4541  rt OMP_NUM_THREA
+00002160: 4453 3d24 534c 5552 4d5f 4350 5553 5f50  DS=$SLURM_CPUS_P
+00002170: 4552 5f54 4153 4b0a 6578 706f 7274 2043  ER_TASK.export C
+00002180: 5241 595f 4355 4441 5f4d 5053 3d31 0a0a  RAY_CUDA_MPS=1..
+00002190: 2320 6c6f 6164 2076 6972 7475 616c 2065  # load virtual e
+000021a0: 6e76 6972 6f6e 6d65 6e74 0a73 6f75 7263  nvironment.sourc
+000021b0: 6520 247b 484f 4d45 7d2f 726f 626f 7665  e ${HOME}/robove
+000021c0: 6e76 2f62 696e 2f61 6374 6976 6174 650a  nv/bin/activate.
+000021d0: 0a65 7870 6f72 7420 4449 5350 4c41 593d  .export DISPLAY=
+000021e0: 3a30 0a73 7275 6e20 7079 7468 6f6e 3320  :0.srun python3 
+000021f0: 2d75 2074 7261 696e 2e70 7920 2e2e 2e0a  -u train.py ....
+00002200: 6060 600a 0a54 6865 206e 756d 6265 7220  ```..The number 
+00002210: 6f66 2070 6172 616c 6c65 6c20 776f 726b  of parallel work
+00002220: 6572 7320 7769 6c6c 2065 7175 616c 2074  ers will equal t
+00002230: 6865 206e 756d 6265 7220 6f66 206e 6f64  he number of nod
+00002240: 6573 2074 696d 6573 2074 6865 206e 756d  es times the num
+00002250: 6265 7220 6f66 2043 5055 7320 7065 7220  ber of CPUs per 
+00002260: 6e6f 6465 200a 2833 3220 7820 3132 203d  node .(32 x 12 =
+00002270: 2033 3834 2069 6e20 7468 6520 7465 6d70   384 in the temp
+00002280: 6c61 7465 2061 626f 7665 292e 0a0a 2323  late above)...##
+00002290: 20f0 9f94 9720 4369 7469 6e67 2041 6e67   .... Citing Ang
+000022a0: 6f72 6150 790a 0a49 6620 796f 7520 7573  oraPy..If you us
+000022b0: 6520 416e 676f 7261 5079 2066 6f72 2079  e AngoraPy for y
+000022c0: 6f75 7220 7265 7365 6172 6368 2c20 706c  our research, pl
+000022d0: 6561 7365 2063 6974 6520 7573 2061 7320  ease cite us as 
+000022e0: 666f 6c6c 6f77 730a 0a20 2020 2057 6569  follows..    Wei
+000022f0: 646c 6572 2c20 546f 6e69 6f2c 2026 2053  dler, Tonio, & S
+00002300: 656e 6465 6e2c 204d 6172 696f 2e20 2832  enden, Mario. (2
+00002310: 3032 3329 2e20 416e 676f 7261 5079 202d  023). AngoraPy -
+00002320: 2041 6e74 6872 6f70 6f6d 6f72 7068 6963   Anthropomorphic
+00002330: 2047 6f61 6c2d 4f72 6965 6e74 6564 2052   Goal-Oriented R
+00002340: 6f62 6f74 6963 2043 6f6e 7472 6f6c 2066  obotic Control f
+00002350: 6f72 204e 6575 726f 7363 6965 6e74 6966  or Neuroscientif
+00002360: 6963 204d 6f64 656c 696e 6720 2830 2e39  ic Modeling (0.9
+00002370: 2e30 292e 205a 656e 6f64 6f2e 2068 7474  .0). Zenodo. htt
+00002380: 7073 3a2f 2f64 6f69 2e6f 7267 2f31 302e  ps://doi.org/10.
+00002390: 3532 3831 2f7a 656e 6f64 6f2e 3737 3730  5281/zenodo.7770
+000023a0: 3138 300a 0a4f 7220 7573 696e 6720 6269  180..Or using bi
+000023b0: 6274 6578 0a0a 2020 2020 4073 6f66 7477  btex..    @softw
+000023c0: 6172 657b 7765 6964 6c65 725f 616e 676f  are{weidler_ango
+000023d0: 7261 7079 5f32 3032 332c 0a20 2020 2020  rapy_2023,.     
+000023e0: 2020 2061 7574 686f 7220 2020 2020 2020     author       
+000023f0: 3d20 7b57 6569 646c 6572 2c20 546f 6e69  = {Weidler, Toni
+00002400: 6f20 616e 6420 5365 6e64 656e 2c20 4d61  o and Senden, Ma
+00002410: 7269 6f7d 2c0a 2020 2020 2020 2020 7469  rio},.        ti
+00002420: 746c 6520 2020 2020 2020 203d 207b 7b41  tle        = {{A
+00002430: 6e67 6f72 6150 7920 2d20 416e 7468 726f  ngoraPy - Anthro
+00002440: 706f 6d6f 7270 6869 6320 476f 616c 2d4f  pomorphic Goal-O
+00002450: 7269 656e 7465 6420 526f 626f 7469 6320  riented Robotic 
+00002460: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00002470: 2020 2020 2020 2020 2020 436f 6e74 726f            Contro
+00002480: 6c20 666f 7220 4e65 7572 6f73 6369 656e  l for Neuroscien
+00002490: 7469 6669 6320 4d6f 6465 6c69 6e67 7d7d  tific Modeling}}
+000024a0: 2c0a 2020 2020 2020 2020 7965 6172 2020  ,.        year  
+000024b0: 2020 2020 2020 203d 2032 3032 332c 0a20         = 2023,. 
+000024c0: 2020 2020 2020 2070 7562 6c69 7368 6572         publisher
+000024d0: 2020 2020 3d20 7b5a 656e 6f64 6f7d 2c0a      = {Zenodo},.
+000024e0: 2020 2020 2020 2020 7665 7273 696f 6e20          version 
+000024f0: 2020 2020 203d 207b 302e 392e 307d 2c0a       = {0.9.0},.
+00002500: 2020 2020 2020 2020 646f 6920 2020 2020          doi     
+00002510: 2020 2020 203d 207b 3130 2e35 3238 312f       = {10.5281/
+00002520: 7a65 6e6f 646f 2e36 3633 3634 3832 7d2c  zenodo.6636482},
+00002530: 0a20 2020 2020 2020 2075 726c 2020 2020  .        url    
+00002540: 2020 2020 2020 3d20 7b68 7474 7073 3a2f        = {https:/
+00002550: 2f64 6f69 2e6f 7267 2f31 302e 3532 3831  /doi.org/10.5281
+00002560: 2f7a 656e 6f64 6f2e 3636 3336 3438 327d  /zenodo.6636482}
+00002570: 0a20 2020 7d0a                           .   }.
```

### Comparing `angorapy-0.9.0/angorapy/agent/core.py` & `angorapy-0.9.1/angorapy/agent/core.py`

 * *Files identical despite different names*

### Comparing `angorapy-0.9.0/angorapy/agent/dataio.py` & `angorapy-0.9.1/angorapy/agent/dataio.py`

 * *Files identical despite different names*

### Comparing `angorapy-0.9.0/angorapy/agent/gather.py` & `angorapy-0.9.1/angorapy/agent/gather.py`

 * *Files identical despite different names*

### Comparing `angorapy-0.9.0/angorapy/agent/ppo/loss.py` & `angorapy-0.9.1/angorapy/agent/ppo/loss.py`

 * *Files identical despite different names*

### Comparing `angorapy-0.9.0/angorapy/agent/ppo/optim.py` & `angorapy-0.9.1/angorapy/agent/ppo/optim.py`

 * *Files identical despite different names*

### Comparing `angorapy-0.9.0/angorapy/agent/ppo_agent.py` & `angorapy-0.9.1/angorapy/agent/ppo_agent.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,14 +17,16 @@
 import numpy as np
 import nvidia_smi
 import psutil
 import tensorflow as tf
 from gym.spaces import Discrete, Box, MultiDiscrete
 from tensorflow.keras import mixed_precision
 
+from angorapy.common.senses import Sensation
+
 try:
     from mpi4py import MPI
 except:
     MPI = None
 
 from psutil import NoSuchProcess
 from tqdm import tqdm
@@ -318,25 +320,27 @@
         """Set GPU usage mode."""
         self.device = "GPU:0" if activated else "CPU:0"
         pass
 
     def assign_gatherer(self, new_gathering_class: Callable):
         self.gatherer_class = new_gathering_class
 
-    def act(self, state):
+    def act(self, state: Sensation):
         """Sample an action from the agent's policy based on a given state. The sampled action is returned in a format
         that can be directly given to an environment.
 
         This method is mostly useful at inference time and serves as q quick wrapper around the steps required to
         process the raw numpy states of the environment into a state readable by the policy network, followed by
         sampling from the predicted distribution."""
 
         # based on given state, predict action distribution and state value; need flatten due to tf eager bug
+        _, _, joint = self.build_models(self.joint.get_weights(), 1, 1)
+
         prepared_state = state.with_leading_dims(time=self.is_recurrent).dict_as_tf()
-        policy_out = flatten(self.joint(prepared_state, training=False))
+        policy_out = flatten(joint(prepared_state, training=False))
 
         predicted_distribution_parameters, value = policy_out[:-1], policy_out[-1]
         # from the action distribution sample an action and remember both the action and its probability
         action, action_probability = self.distribution.act(*predicted_distribution_parameters)
 
         return action
```

### Comparing `angorapy-0.9.0/angorapy/analysis/chiefinvestigation.py` & `angorapy-0.9.1/angorapy/analysis/chiefinvestigation.py`

 * *Files identical despite different names*

### Comparing `angorapy-0.9.0/angorapy/analysis/dynamics.py` & `angorapy-0.9.1/angorapy/analysis/dynamics.py`

 * *Files identical despite different names*

### Comparing `angorapy-0.9.0/angorapy/analysis/investigators/base_investigator.py` & `angorapy-0.9.1/angorapy/analysis/investigators/base_investigator.py`

 * *Files identical despite different names*

### Comparing `angorapy-0.9.0/angorapy/analysis/investigators/correlation.py` & `angorapy-0.9.1/angorapy/analysis/investigators/correlation.py`

 * *Files identical despite different names*

### Comparing `angorapy-0.9.0/angorapy/analysis/investigators/dynamics.py` & `angorapy-0.9.1/angorapy/analysis/investigators/dynamics.py`

 * *Files identical despite different names*

### Comparing `angorapy-0.9.0/angorapy/analysis/investigators/predictability.py` & `angorapy-0.9.1/angorapy/analysis/investigators/predictability.py`

 * *Files 24% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 
 from angorapy.analysis.investigators import base_investigator
 from angorapy.common.policies import BasePolicyDistribution
 from angorapy.common.senses import stack_sensations
 from angorapy.common.wrappers import BaseWrapper
 from angorapy.environments.rotations import quat2mat, quat2axisangle
 from angorapy.utilities.util import flatten, stack_dicts
+import tensorflow_graphics.geometry.transformation as tfg
 
 
 class Predictability(base_investigator.Investigator):
     """Investigate predictability of information from the activity in different regions of the network."""
 
     def __init__(self, network: tf.keras.Model, distribution: BasePolicyDistribution):
         super().__init__(network, distribution)
@@ -31,14 +32,15 @@
         state, info = env.reset(return_info=True)
 
         state_collection = []
         activation_collection = []
         other_collection = []
         prev_achieved_goals = [info["achieved_goal"]] * 50
         prev_object_quats = [info["achieved_goal"][3:]] * 10
+        need_thump_this_episode = False
         for _ in tqdm.tqdm(range(n_states)):
             state_collection.append(state)
             other = {
                 "reward": info.get("original_reward", 0),
             }
 
             prepared_state = state.with_leading_dims(time=self.is_recurrent).dict()
@@ -47,37 +49,55 @@
 
             probabilities = flatten(activations["output"])
             action, _ = self.distribution.act(*probabilities)
 
             observation, reward, terminated, truncated, info = env.step(action)
             done = terminated or truncated
 
+            # if env.is_thumb_tip_touching():
+            #     need_thump_this_episode = True
+
+            # other["needed_thumb"] = None
             other["fingertip_positions"] = env.unwrapped.get_fingertip_positions()
             other["translation"] = env.unwrapped._goal_distance(info["achieved_goal"], prev_achieved_goals[-1])
             other["translation_to_10"] = env.unwrapped._goal_distance(info["achieved_goal"], prev_achieved_goals[-10])
             other["translation_to_50"] = env.unwrapped._goal_distance(info["achieved_goal"], prev_achieved_goals[-50])
             other["object_orientation"] = env.unwrapped.data.jnt('object:joint').qpos.copy()[3:]
-
-            prev_quat = transform.Rotation.from_quat(prev_object_quats[-1])
-            prev_quat_10 = transform.Rotation.from_quat(prev_object_quats[-10])
-            current_quat = transform.Rotation.from_quat(other["object_orientation"])
-            change_in_orientation = (prev_quat_10 * current_quat.inv()).as_quat()
-
-            other["rotation_matrix"] = quat2mat((prev_quat * current_quat.inv()).as_quat()).flatten()
-            other["rotation_matrix_last_10"] = quat2mat(change_in_orientation).flatten()
-            other["current_rotational_axis"] = quat2axisangle(change_in_orientation)[0]  # todo
+            # other["relative_angle"] = tfg.quaternion.relative_angle(
+            #     tf.cast(env.unwrapped.data.jnt('object:joint').qpos.copy()[3:], dtype=tf.float64),
+            #     tf.cast(state["goal"], dtype=tf.float64)
+            # )
+            # prev_quat = transform.Rotation.from_quat(prev_object_quats[-1])
+            # prev_quat_10 = transform.Rotation.from_quat(prev_object_quats[-10])
+            # current_quat = transform.Rotation.from_quat(other["object_orientation"])
+            # change_in_orientation = (prev_quat_10 * current_quat.inv()).as_quat()
+
+            # other["rotation_matrix"] = quat2mat((prev_quat * current_quat.inv()).as_quat()).flatten()
+            # other["rotation_matrix_last_10"] = quat2mat(change_in_orientation).flatten()
+            # other["current_rotational_axis"] = quat2axisangle(change_in_orientation)[0]  # todo
+            other["goals_achieved_so_far"] = env.consecutive_goals_reached
 
             other_collection.append(other)
 
             if done:
                 state, info = env.reset(return_info=True)
+                prev_achieved_goals = [info["achieved_goal"]] * 50
+
                 self.network.reset_states()
+
+                # for ot in other_collection:
+                #     ot["needed_thumb"] = ot["needed_thumb"] if ot["needed_thumb"] is not None else need_thump_this_episode
+
+                # need_thump_this_episode = False
+
             else:
                 state = observation
                 prev_achieved_goals.append(info["achieved_goal"])
+                # for ot in other_collection:
+                #     ot["needed_thumb"] = ot["needed_thumb"] if ot["needed_thumb"] is not None else need_thump_this_episode
 
                 if len(prev_achieved_goals) > 50:
                     prev_achieved_goals.pop(0)
 
         stacked_other_collection = stack_dicts(other_collection)
         stacked_other_collection["translation"][:-1] = stacked_other_collection["translation"][1:]
         stacked_other_collection["translation_to_10"][:-10] = stacked_other_collection["translation_to_10"][10:]
@@ -111,10 +131,10 @@
             x[source_layer]))).as_numpy_iterator())
         Y_test = list(self.val_data.map(lambda x: (tf.random.normal(base_shape) if source_layer == "noise" else tf.squeeze(
             x[target_information]))).as_numpy_iterator())
 
         predictor.fit(X, Y)
         score = predictor.score(X_test, Y_test)
 
-        print(f"{target_information} from {source_layer} has an R2 of {predictor.score(X_test, Y_test)}.")
+        # print(f"{target_information} from {source_layer} has an R2 of {predictor.score(X_test, Y_test)}.")
 
         return score
```

### Comparing `angorapy-0.9.0/angorapy/analysis/plot_predictability.py` & `angorapy-0.9.1/angorapy/analysis/plot_predictability.py`

 * *Files identical despite different names*

### Comparing `angorapy-0.9.0/angorapy/analysis/plot_predictability_grouped.py` & `angorapy-0.9.1/angorapy/analysis/plot_predictability_grouped.py`

 * *Files identical despite different names*

### Comparing `angorapy-0.9.0/angorapy/analysis/plot_predictability_grouped_with_error_bars.py` & `angorapy-0.9.1/angorapy/analysis/plot_predictability_grouped_with_error_bars.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,43 +1,51 @@
 import json
 import re
 
 import numpy as np
 from matplotlib import pyplot as plt
+import matplotlib
+font = {'family' : 'Times',
+        'weight' : 'normal',
+        'size'   : 12}
 
-with open("results/predictability_repeated_mar20.json", "r") as f:
+matplotlib.rc('font', **font)
+with open("../../storage/predictability_repeated_april08.json", "r") as f:
     results = json.load(f)
 
 included_regions = ["M1_activation", "pmc_recurrent_layer", "goal"]
 included_targets = ["translation", "translation_to_10", "translation_to_50"]
 # included_regions = ["M1_activation", "pmc_recurrent_layer"]
 # included_targets = ["reward", "goal"]
 # included_regions = ["M1_activation", "pmc_recurrent_layer"]
 # included_targets = ['rotation_matrix', 'rotation_matrix_last_10']
 
 
 x = np.arange(len(included_targets))
-width = 0.7 / len(included_regions)
+width = 0.8 / len(included_regions)
 
 rects = []
 fig, ax = plt.subplots()
 
-for i, source in enumerate(included_regions):
-       ax.bar(x - (width / (len(included_regions)) * i),
+for i, source in enumerate(included_regions, start=-1):
+       ax.bar(x + i * width,
               [np.mean(results[source][t]) for t in included_targets],
               width,
               yerr=[np.std(results[source][t]) for t in included_targets],
-              label=source.split("_")[0],
+              label=source.split("_")[0].upper() if "_" in source else source.capitalize(),
               capsize=3)
 
-# ax.set_xticks(x, ["orientation in 8ms", "orientation in 80ms", "orientation in 400ms"])
-ax.set_xticks(x, included_targets)
-ax.legend()
+ax.set_xticks(x, ["Orientation in 8ms", "Orientation in 80ms", "Orientation in 400ms"])
+# ax.set_xticks(x, included_targets)
+ax.legend(ncol=3)
+
 ax.set_ylabel("Predictability (R2)")
 
 ax.set_ylim(0, 1)
 
-plt.show()
+# plt.show()
+
+# set figure size to 8x2 inches
+fig.set_size_inches(8, 2)
 
-# plt.xticks(rotation="vertical")
-# plt.gcf().subplots_adjust(bottom=0.3)
-# plt.savefig("M1vsPMC.svg", format="svg", bbox_inches="tight")
+# save the figure to a pdf file without whitespace around it
+plt.savefig(f"predictability_translation_grouped.pdf", format="pdf", bbox_inches="tight")
```

### Comparing `angorapy-0.9.0/angorapy/analysis/plot_utils.py` & `angorapy-0.9.1/angorapy/analysis/plot_utils.py`

 * *Files identical despite different names*

### Comparing `angorapy-0.9.0/angorapy/analysis/plotting/autocorrelation_combined_plot.py` & `angorapy-0.9.1/angorapy/analysis/plotting/autocorrelation_combined_plot.py`

 * *Files identical despite different names*

### Comparing `angorapy-0.9.0/angorapy/analysis/plotting/make_viz_featuremax.py` & `angorapy-0.9.1/angorapy/analysis/plotting/make_viz_featuremax.py`

 * *Files identical despite different names*

### Comparing `angorapy-0.9.0/angorapy/analysis/plotting/make_viz_pretraining_fmap.py` & `angorapy-0.9.1/angorapy/analysis/plotting/make_viz_pretraining_fmap.py`

 * *Files identical despite different names*

### Comparing `angorapy-0.9.0/angorapy/analysis/plotting/make_viz_pretraining_saliency.py` & `angorapy-0.9.1/angorapy/analysis/plotting/make_viz_pretraining_saliency.py`

 * *Files identical despite different names*

### Comparing `angorapy-0.9.0/angorapy/analysis/plotting/plot_benchmark.py` & `angorapy-0.9.1/angorapy/analysis/plotting/plot_benchmark.py`

 * *Files identical despite different names*

### Comparing `angorapy-0.9.0/angorapy/analysis/plotting/plot_benchmark_groups.py` & `angorapy-0.9.1/angorapy/analysis/plotting/plot_benchmark_groups.py`

 * *Files identical despite different names*

### Comparing `angorapy-0.9.0/angorapy/analysis/plotting/plot_benchmark_groups_with_beta.py` & `angorapy-0.9.1/angorapy/analysis/plotting/plot_benchmark_groups_with_beta.py`

 * *Files identical despite different names*

### Comparing `angorapy-0.9.0/angorapy/analysis/plotting/plot_distributed_computation_benchmark.py` & `angorapy-0.9.1/angorapy/analysis/plotting/plot_distributed_computation_benchmark.py`

 * *Files identical despite different names*

### Comparing `angorapy-0.9.0/angorapy/analysis/plotting/plot_experiment_best_evaluation.py` & `angorapy-0.9.1/angorapy/analysis/plotting/plot_experiment_best_evaluation.py`

 * *Files identical despite different names*

### Comparing `angorapy-0.9.0/angorapy/analysis/plotting/plot_experiment_comparison.py` & `angorapy-0.9.1/angorapy/analysis/plotting/plot_experiment_comparison.py`

 * *Files identical despite different names*

### Comparing `angorapy-0.9.0/angorapy/analysis/plotting/plot_experiment_comparison_only_success_multiple_runs.py` & `angorapy-0.9.1/angorapy/analysis/plotting/plot_experiment_comparison_only_success_multiple_runs_line_scatter.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,89 +1,87 @@
 import itertools
 import json
 import os
 
-
 import numpy as np
 import pandas as pd
 import seaborn as sns
 from matplotlib import pyplot as plt
-import matplotlib
 
 from angorapy.common.const import PATH_TO_EXPERIMENTS, QUALITATIVE_COLOR_PALETTE
 
-
-font = {'family' : 'Times New Roman',
-        'weight' : 'normal',
-        'size'   : 22}
-
-matplotlib.rc('font', **font)
-
-# experiment_ids = [['1675028736765791', '1674983643322591'],
-#                   ['1674985163288377', '1674983177286330'],
-#                   ['1674343261520188', '1674308148646663', '1674074113967956', '1674074113731734', '1673350499432390']]  # compare distributions
-experiment_ids = [['1679142835973298'],
-                  ['1673350499432390']]  # compare distributions
-names = ["brain-inspired architecture", "OpenAI (2018)"]
-
-
+experiment_ids = [['1674975602294059', '1674975602446141', '1671749718306373'],
+                  ['1674343261520188', '1674308148646663', '1674074113967956', '1674074113731734', '1673350499432390']]
+names = ["symmetric", "asymmetric"]
 reward_developments = {}
 reward_bands = {}
 
 cosucc_developments = {}
 cosucc_bands = {}
 
 evaluation_rewards = {}
 evaluation_reward_histograms = {}
 
 for i, group in enumerate(experiment_ids):
     exp_name = names[i]
     reward_developments[exp_name] = []
     cosucc_developments[exp_name] = []
+    cosucc_bands[exp_name] = []
     evaluation_rewards[exp_name] = []
     evaluation_reward_histograms[exp_name] = []
 
     for id in group:
         with open(os.path.join("../../../", PATH_TO_EXPERIMENTS, str(id), "meta.json")) as f:
             meta = json.load(f)
         with open(os.path.join("../../../", PATH_TO_EXPERIMENTS, str(id), "progress.json")) as f:
             progress = json.load(f)
         with open(os.path.join("../../../", PATH_TO_EXPERIMENTS, str(id), "statistics.json")) as f:
             statistics = json.load(f)
-        with open(os.path.join("../../../", PATH_TO_EXPERIMENTS, str(id), "evaluation.json")) as f:
-            evaluation = json.load(f)
 
-        reward_developments[exp_name].append(progress["rewards"]["mean"])
-        cosucc_developments[exp_name].append(statistics["auxiliary_performances"]["consecutive_goals_reached"]["mean"])
-        evaluation_rewards[exp_name] += evaluation["auxiliary_performances"]["consecutive_goals_reached"]
-        evaluation_reward_histograms[exp_name].append(
-            np.histogram(evaluation["auxiliary_performances"]["consecutive_goals_reached"], bins=50))
-
-    evaluation_reward_histograms[exp_name] = np.mean([c for c, b in evaluation_reward_histograms[exp_name]], axis=0), \
-    evaluation_reward_histograms[exp_name][0][1]
-    reward_developments[exp_name] = np.array(
-        [trace[:min(map(len, reward_developments[exp_name]))] for trace in reward_developments[exp_name]])
-    cosucc_developments[exp_name] = np.array(
-        [trace[:min(map(len, cosucc_developments[exp_name]))] for trace in cosucc_developments[exp_name]])
-
-    rd_mean = np.mean(reward_developments[exp_name], axis=0)
-    cd_mean = np.mean(cosucc_developments[exp_name], axis=0)
-    rd_std = np.std(reward_developments[exp_name], axis=0)
-    cd_std = np.std(cosucc_developments[exp_name], axis=0)
-    reward_bands[exp_name] = (rd_mean - rd_std, rd_mean + rd_std)
-    cosucc_bands[exp_name] = (cd_mean - cd_std, cd_mean + cd_std)
-
-ax1 = plt.subplot2grid((1, 3), (0, 0), colspan=3)
-# ax2 = plt.subplot2grid((1, 3), (0, 2), colspan=1)
-
-x_max = len(list(reward_developments.items())[0][1][0])
-for i, (name, rewards) in enumerate(reward_developments.items()):
-    x_max = max(x_max, np.argmax(rewards))
-    ax1.plot(np.mean(cosucc_developments[name], axis=0)[:np.argmax(rewards)], label=name, color=QUALITATIVE_COLOR_PALETTE[i])
-    ax1.fill_between(range(len(cosucc_bands[name][0])), cosucc_bands[name][0], cosucc_bands[name][1], alpha=0.2)
+        try:
+            with open(os.path.join("../../../", PATH_TO_EXPERIMENTS, str(id), "evaluation.json")) as f:
+                evaluation = json.load(f)
+
+            evaluation_rewards[exp_name] += evaluation["auxiliary_performances"]["consecutive_goals_reached"]
+            evaluation_reward_histograms[exp_name].append(
+                np.histogram(evaluation["auxiliary_performances"]["consecutive_goals_reached"], bins=50))
+        except:
+            pass
+
+        window_size_one_sided = 5
+        cosucc_traj = statistics["auxiliary_performances"]["consecutive_goals_reached"]["mean"]
+        cosucc_developments[exp_name].append(np.array([
+            np.mean(np.array(cosucc_traj)[max(i - window_size_one_sided, 0):min(i + window_size_one_sided, len(cosucc_traj))]) for i in
+            range(len(cosucc_traj))
+        ]))
+        cosucc_bands[exp_name].append(np.array([
+            np.std(np.array(cosucc_traj)[
+                    max(i - window_size_one_sided, 0):min(i + window_size_one_sided, len(cosucc_traj))]) for i in
+            range(len(cosucc_traj))
+        ]))
+
+    try:
+        evaluation_reward_histograms[exp_name] = np.mean([c for c, b in evaluation_reward_histograms[exp_name]],
+                                                         axis=0), evaluation_reward_histograms[exp_name][0][1]
+    except:
+        pass
+    # reward_developments[exp_name] = np.array(
+    #     [trace[:min(map(len, reward_developments[exp_name]))] for trace in reward_developments[exp_name]])
+    # cosucc_developments[exp_name] = np.array(
+    #     [trace[:min(map(len, cosucc_developments[exp_name]))] for trace in cosucc_developments[exp_name]])
+
+ax1 = plt.subplot2grid((1, 3), (0, 0), colspan=2)
+ax2 = plt.subplot2grid((1, 3), (0, 2), colspan=1)
+
+for i, (name, rewards) in enumerate(cosucc_developments.items()):
+    for j in range(len(cosucc_developments[name])):
+        ax1.plot(cosucc_developments[name][j], label=name if j == 0 else None, color=QUALITATIVE_COLOR_PALETTE[i])
+        ax1.fill_between(range(len(cosucc_bands[name][j])),
+                         cosucc_developments[name][j] - cosucc_bands[name][j],
+                         cosucc_developments[name][j] + cosucc_bands[name][j], alpha=0.2, color=QUALITATIVE_COLOR_PALETTE[i])
 
     # ax2.hist(
     #     evaluation_reward_histograms[name][1][:-1],
     #     evaluation_reward_histograms[name][1],
     #     weights=evaluation_reward_histograms[name][0],
     #     edgecolor="white", linewidth=0.5, alpha=0.8
     # )
@@ -91,22 +89,22 @@
     # ax2.set_ylabel("Number of Episodes")
 
 df = pd.DataFrame(
     {"group": itertools.chain(*[[name] * len(dp) for name, dp in evaluation_rewards.items()]),
      "Consecutive Goals Reached": np.concatenate([dp for name, dp in evaluation_rewards.items()])}
 )
 
-# sns.boxplot(data=df, x="group", y="Consecutive Goals Reached", medianprops={"color": "red"}, flierprops={"marker": "x"},
-#             fliersize=1, ax=ax2, palette={name: QUALITATIVE_COLOR_PALETTE[i] for i, name in enumerate(names)},
-#             showmeans=True, meanprops={"marker": "o", "markerfacecolor": "white", "markeredgecolor": "black"})
-# ax2.set_xlabel("")
-
+sns.boxplot(data=df, x="group", y="Consecutive Goals Reached", medianprops={"color": "red"}, flierprops={"marker": "x"},
+            fliersize=1, ax=ax2, palette={name: QUALITATIVE_COLOR_PALETTE[i] for i, name in enumerate(names)},
+            showmeans=True, meanprops={"marker": "o", "markerfacecolor": "white", "markeredgecolor": "black"})
+ax2.set_xlabel("")
 
 ax1.set_xlabel("Cycle")
 ax1.set_ylabel("Avg. Consecutive Goals Reached")
-ax1.legend()
+ax1.legend(loc="upper left")
 
-ax1.set_xlim(0, x_max)
+ax1.set_xlim(0)
 
-plt.gcf().set_size_inches(16, 8)
+plt.gcf().set_size_inches(12, 4)
 plt.subplots_adjust(wspace=0.3, right=0.995, left=0.05, top=0.99)
-plt.savefig("../../../docs/figures/brain-vs-openai.svg", format="svg", bbox="tight")
+plt.show()
+# plt.savefig("../../../docs/figures/manipulate-asymmetry-ablation.pdf", format="pdf", bbox="tight")
```

### Comparing `angorapy-0.9.0/angorapy/analysis/plotting/plot_experiment_comparison_only_success_multiple_runs_line_scatter.py` & `angorapy-0.9.1/angorapy/analysis/plotting/plot_experiment_comparison_only_success_multiple_runs_with_zoom.py`

 * *Files 27% similar despite different names*

```diff
@@ -4,107 +4,111 @@
 
 import numpy as np
 import pandas as pd
 import seaborn as sns
 from matplotlib import pyplot as plt
 
 from angorapy.common.const import PATH_TO_EXPERIMENTS, QUALITATIVE_COLOR_PALETTE
+from mpl_toolkits.axes_grid1.inset_locator import zoomed_inset_axes
+from mpl_toolkits.axes_grid1.inset_locator import mark_inset
 
-experiment_ids = [['1674975602294059', '1674975602446141', '1671749718306373'],
-                  ['1674343261520188', '1674308148646663', '1674074113967956', '1674074113731734', '1673350499432390']]
-names = ["symmetric", "asymmetric"]
+
+experiment_ids = [['1675028736765791', '1674983643322591'],
+                  ['1674985163288377', '1674983177286330'],
+                  ['1674343261520188', '1674308148646663', '1674074113967956', '1673350499432390']]  # compare distributions
+names = ["beta", "gaussian", "multicategorical"]
+# names = ["beta", "multicategorical"]
 reward_developments = {}
 reward_bands = {}
 
 cosucc_developments = {}
 cosucc_bands = {}
 
 evaluation_rewards = {}
 evaluation_reward_histograms = {}
 
 for i, group in enumerate(experiment_ids):
     exp_name = names[i]
     reward_developments[exp_name] = []
     cosucc_developments[exp_name] = []
-    cosucc_bands[exp_name] = []
     evaluation_rewards[exp_name] = []
     evaluation_reward_histograms[exp_name] = []
 
     for id in group:
         with open(os.path.join("../../../", PATH_TO_EXPERIMENTS, str(id), "meta.json")) as f:
             meta = json.load(f)
         with open(os.path.join("../../../", PATH_TO_EXPERIMENTS, str(id), "progress.json")) as f:
             progress = json.load(f)
         with open(os.path.join("../../../", PATH_TO_EXPERIMENTS, str(id), "statistics.json")) as f:
             statistics = json.load(f)
+        with open(os.path.join("../../../", PATH_TO_EXPERIMENTS, str(id), "evaluation.json")) as f:
+            evaluation = json.load(f)
 
-        try:
-            with open(os.path.join("../../../", PATH_TO_EXPERIMENTS, str(id), "evaluation.json")) as f:
-                evaluation = json.load(f)
-
-            evaluation_rewards[exp_name] += evaluation["auxiliary_performances"]["consecutive_goals_reached"]
-            evaluation_reward_histograms[exp_name].append(
-                np.histogram(evaluation["auxiliary_performances"]["consecutive_goals_reached"], bins=50))
-        except:
-            pass
-
-        window_size_one_sided = 5
-        cosucc_traj = statistics["auxiliary_performances"]["consecutive_goals_reached"]["mean"]
-        cosucc_developments[exp_name].append(np.array([
-            np.mean(np.array(cosucc_traj)[max(i - window_size_one_sided, 0):min(i + window_size_one_sided, len(cosucc_traj))]) for i in
-            range(len(cosucc_traj))
-        ]))
-        cosucc_bands[exp_name].append(np.array([
-            np.std(np.array(cosucc_traj)[
-                    max(i - window_size_one_sided, 0):min(i + window_size_one_sided, len(cosucc_traj))]) for i in
-            range(len(cosucc_traj))
-        ]))
-
-    try:
-        evaluation_reward_histograms[exp_name] = np.mean([c for c, b in evaluation_reward_histograms[exp_name]],
-                                                         axis=0), evaluation_reward_histograms[exp_name][0][1]
-    except:
-        pass
-    # reward_developments[exp_name] = np.array(
-    #     [trace[:min(map(len, reward_developments[exp_name]))] for trace in reward_developments[exp_name]])
-    # cosucc_developments[exp_name] = np.array(
-    #     [trace[:min(map(len, cosucc_developments[exp_name]))] for trace in cosucc_developments[exp_name]])
+        reward_developments[exp_name].append(progress["rewards"]["mean"])
+        cosucc_developments[exp_name].append(statistics["auxiliary_performances"]["consecutive_goals_reached"]["mean"])
+        evaluation_rewards[exp_name] += evaluation["auxiliary_performances"]["consecutive_goals_reached"]
+        evaluation_reward_histograms[exp_name].append(
+            np.histogram(evaluation["auxiliary_performances"]["consecutive_goals_reached"], bins=50))
+
+    evaluation_reward_histograms[exp_name] = np.mean([c for c, b in evaluation_reward_histograms[exp_name]], axis=0), \
+    evaluation_reward_histograms[exp_name][0][1]
+    reward_developments[exp_name] = np.array(
+        [trace[:min(map(len, reward_developments[exp_name]))] for trace in reward_developments[exp_name]])
+    cosucc_developments[exp_name] = np.array(
+        [trace[:min(map(len, cosucc_developments[exp_name]))] for trace in cosucc_developments[exp_name]])
+
+    rd_mean = np.mean(reward_developments[exp_name], axis=0)
+    cd_mean = np.mean(cosucc_developments[exp_name], axis=0)
+    rd_std = np.std(reward_developments[exp_name], axis=0)
+    cd_std = np.std(cosucc_developments[exp_name], axis=0)
+    reward_bands[exp_name] = (rd_mean - rd_std, rd_mean + rd_std)
+    cosucc_bands[exp_name] = (cd_mean - cd_std, cd_mean + cd_std)
 
 ax1 = plt.subplot2grid((1, 3), (0, 0), colspan=2)
 ax2 = plt.subplot2grid((1, 3), (0, 2), colspan=1)
+axins = zoomed_inset_axes(ax1, 2, loc=1) # zoom = 2
+
+x_max = len(list(reward_developments.items())[0][1][0])
+for i, (name, rewards) in enumerate(reward_developments.items()):
+    x_max = max(x_max, len(rewards[0]))
+    ax1.plot(np.mean(cosucc_developments[name], axis=0), label=name, color=QUALITATIVE_COLOR_PALETTE[i])
+    ax1.fill_between(range(len(cosucc_bands[name][0])), cosucc_bands[name][0], cosucc_bands[name][1], alpha=0.2)
 
-for i, (name, rewards) in enumerate(cosucc_developments.items()):
-    for j in range(len(cosucc_developments[name])):
-        ax1.plot(cosucc_developments[name][j], label=name if j == 0 else None, color=QUALITATIVE_COLOR_PALETTE[i])
-        ax1.fill_between(range(len(cosucc_bands[name][j])),
-                         cosucc_developments[name][j] - cosucc_bands[name][j],
-                         cosucc_developments[name][j] + cosucc_bands[name][j], alpha=0.2, color=QUALITATIVE_COLOR_PALETTE[i])
+    axins.plot(np.mean(cosucc_developments[name], axis=0), label=name, color=QUALITATIVE_COLOR_PALETTE[i])
+    axins.fill_between(range(len(cosucc_bands[name][0])), cosucc_bands[name][0], cosucc_bands[name][1], alpha=0.2)
 
     # ax2.hist(
     #     evaluation_reward_histograms[name][1][:-1],
     #     evaluation_reward_histograms[name][1],
     #     weights=evaluation_reward_histograms[name][0],
     #     edgecolor="white", linewidth=0.5, alpha=0.8
     # )
     # ax2.set_xlabel("Consecutive Goals Reached")
     # ax2.set_ylabel("Number of Episodes")
-
+axins.set_xlim(0, 100.)
+axins.set_ylim(-5., 10.)
+plt.xticks(visible=False)
+plt.yticks(visible=False)
+mark_inset(ax1, axins, loc1=2, loc2=4, fc="none", ec="0.5")
+# plt.draw()
 df = pd.DataFrame(
     {"group": itertools.chain(*[[name] * len(dp) for name, dp in evaluation_rewards.items()]),
      "Consecutive Goals Reached": np.concatenate([dp for name, dp in evaluation_rewards.items()])}
 )
 
 sns.boxplot(data=df, x="group", y="Consecutive Goals Reached", medianprops={"color": "red"}, flierprops={"marker": "x"},
             fliersize=1, ax=ax2, palette={name: QUALITATIVE_COLOR_PALETTE[i] for i, name in enumerate(names)},
             showmeans=True, meanprops={"marker": "o", "markerfacecolor": "white", "markeredgecolor": "black"})
 ax2.set_xlabel("")
 
+
 ax1.set_xlabel("Cycle")
 ax1.set_ylabel("Avg. Consecutive Goals Reached")
-ax1.legend(loc="upper left")
+ax1.legend()
 
-ax1.set_xlim(0)
+ax1.set_xlim(0, x_max)
+ax1.set_ylim(-5)
 
 plt.gcf().set_size_inches(12, 4)
 plt.subplots_adjust(wspace=0.3, right=0.995, left=0.05, top=0.99)
 plt.show()
 # plt.savefig("../../../docs/figures/manipulate-asymmetry-ablation.pdf", format="pdf", bbox="tight")
```

### Comparing `angorapy-0.9.0/angorapy/analysis/plotting/plot_experiment_comparison_only_success_multiple_runs_with_zoom.py` & `angorapy-0.9.1/angorapy/analysis/plotting/plot_experiment_comparison_only_success_multiple_runs.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,114 +1,129 @@
 import itertools
 import json
 import os
 
+
 import numpy as np
 import pandas as pd
 import seaborn as sns
 from matplotlib import pyplot as plt
+import matplotlib
+import statsmodels.stats.api as sms
 
 from angorapy.common.const import PATH_TO_EXPERIMENTS, QUALITATIVE_COLOR_PALETTE
-from mpl_toolkits.axes_grid1.inset_locator import zoomed_inset_axes
-from mpl_toolkits.axes_grid1.inset_locator import mark_inset
 
 
-experiment_ids = [['1675028736765791', '1674983643322591'],
-                  ['1674985163288377', '1674983177286330'],
-                  ['1674343261520188', '1674308148646663', '1674074113967956', '1673350499432390']]  # compare distributions
-names = ["beta", "gaussian", "multicategorical"]
-# names = ["beta", "multicategorical"]
+font = {'family' : 'Times',
+        'weight' : 'normal',
+        'size'   : 15}
+
+matplotlib.rc('font', **font)
+
+# experiment_ids = [['1675028736765791', '1674983643322591'],
+#                   ['1674985163288377', '1674983177286330'],
+#                   ['1674343261520188', '1674308148646663', '1674074113967956', '1674074113731734', '1673350499432390']]  # compare distributions
+experiment_ids = [['1680268307741971', '1680267170902356', '1680266899101867', '1679765936722940', '1679142835973298'],
+                  ['1674343261520188', '1674308148646663', '1674074113967956', '1674074113731734', '1673350499432390']]  # compare distributions
+# experiment_ids = [['1680268307741971', '1680267170902356', '1679765936722940', '1679142835973298'],
+#                   ['1674343261520188', '1674308148646663', '1674074113967956', '1673350499432390']]  # compare distributions
+names = ["FPN model", "OpenAI"]
+
 reward_developments = {}
 reward_bands = {}
 
 cosucc_developments = {}
 cosucc_bands = {}
 
 evaluation_rewards = {}
 evaluation_reward_histograms = {}
 
 for i, group in enumerate(experiment_ids):
     exp_name = names[i]
     reward_developments[exp_name] = []
     cosucc_developments[exp_name] = []
-    evaluation_rewards[exp_name] = []
-    evaluation_reward_histograms[exp_name] = []
+    # evaluation_rewards[exp_name] = []
+    # evaluation_reward_histograms[exp_name] = []
 
     for id in group:
         with open(os.path.join("../../../", PATH_TO_EXPERIMENTS, str(id), "meta.json")) as f:
             meta = json.load(f)
         with open(os.path.join("../../../", PATH_TO_EXPERIMENTS, str(id), "progress.json")) as f:
             progress = json.load(f)
         with open(os.path.join("../../../", PATH_TO_EXPERIMENTS, str(id), "statistics.json")) as f:
             statistics = json.load(f)
-        with open(os.path.join("../../../", PATH_TO_EXPERIMENTS, str(id), "evaluation.json")) as f:
-            evaluation = json.load(f)
+        # with open(os.path.join("../../../", PATH_TO_EXPERIMENTS, str(id), "evaluation.json")) as f:
+        #     evaluation = json.load(f)
 
         reward_developments[exp_name].append(progress["rewards"]["mean"])
         cosucc_developments[exp_name].append(statistics["auxiliary_performances"]["consecutive_goals_reached"]["mean"])
-        evaluation_rewards[exp_name] += evaluation["auxiliary_performances"]["consecutive_goals_reached"]
-        evaluation_reward_histograms[exp_name].append(
-            np.histogram(evaluation["auxiliary_performances"]["consecutive_goals_reached"], bins=50))
+        # evaluation_rewards[exp_name] += evaluation["auxiliary_performances"]["consecutive_goals_reached"]
+        # evaluation_reward_histograms[exp_name].append(
+        #     np.histogram(evaluation["auxiliary_performances"]["consecutive_goals_reached"], bins=50))
 
-    evaluation_reward_histograms[exp_name] = np.mean([c for c, b in evaluation_reward_histograms[exp_name]], axis=0), \
-    evaluation_reward_histograms[exp_name][0][1]
+    # evaluation_reward_histograms[exp_name] = np.mean([c for c, b in evaluation_reward_histograms[exp_name]], axis=0), \
+    # evaluation_reward_histograms[exp_name][0][1]
     reward_developments[exp_name] = np.array(
         [trace[:min(map(len, reward_developments[exp_name]))] for trace in reward_developments[exp_name]])
     cosucc_developments[exp_name] = np.array(
         [trace[:min(map(len, cosucc_developments[exp_name]))] for trace in cosucc_developments[exp_name]])
 
+    descm = sms.DescrStatsW(cosucc_developments[exp_name])
+
     rd_mean = np.mean(reward_developments[exp_name], axis=0)
     cd_mean = np.mean(cosucc_developments[exp_name], axis=0)
     rd_std = np.std(reward_developments[exp_name], axis=0)
-    cd_std = np.std(cosucc_developments[exp_name], axis=0)
     reward_bands[exp_name] = (rd_mean - rd_std, rd_mean + rd_std)
-    cosucc_bands[exp_name] = (cd_mean - cd_std, cd_mean + cd_std)
+    cosucc_bands[exp_name] = descm.tconfint_mean()
 
-ax1 = plt.subplot2grid((1, 3), (0, 0), colspan=2)
-ax2 = plt.subplot2grid((1, 3), (0, 2), colspan=1)
-axins = zoomed_inset_axes(ax1, 2, loc=1) # zoom = 2
+ax1 = plt.subplot2grid((1, 3), (0, 0), colspan=3)
+# ax2 = plt.subplot2grid((1, 3), (0, 2), colspan=1)
 
 x_max = len(list(reward_developments.items())[0][1][0])
 for i, (name, rewards) in enumerate(reward_developments.items()):
-    x_max = max(x_max, len(rewards[0]))
-    ax1.plot(np.mean(cosucc_developments[name], axis=0), label=name, color=QUALITATIVE_COLOR_PALETTE[i])
+    x_max = max(x_max, np.max(np.argmax(rewards, axis=-1)))
+    mean_line = np.mean(cosucc_developments[name], axis=0)[:np.argmax(rewards)]
+    ax1.plot(mean_line, label=name, color=QUALITATIVE_COLOR_PALETTE[i])
     ax1.fill_between(range(len(cosucc_bands[name][0])), cosucc_bands[name][0], cosucc_bands[name][1], alpha=0.2)
 
-    axins.plot(np.mean(cosucc_developments[name], axis=0), label=name, color=QUALITATIVE_COLOR_PALETTE[i])
-    axins.fill_between(range(len(cosucc_bands[name][0])), cosucc_bands[name][0], cosucc_bands[name][1], alpha=0.2)
+    # plot horizontal line indicating max performance with circles as markers
+    ax1.axhline(y=np.max(mean_line), color=QUALITATIVE_COLOR_PALETTE[i], linestyle="--", linewidth=1)
+
+    # plot horizontal line indicating max performance of best agent in group
+    ax1.axhline(y=np.max(np.max(cosucc_developments[name], axis=0)), linestyle=":", color=QUALITATIVE_COLOR_PALETTE[i], linewidth=0.5)
 
     # ax2.hist(
     #     evaluation_reward_histograms[name][1][:-1],
     #     evaluation_reward_histograms[name][1],
     #     weights=evaluation_reward_histograms[name][0],
     #     edgecolor="white", linewidth=0.5, alpha=0.8
     # )
     # ax2.set_xlabel("Consecutive Goals Reached")
     # ax2.set_ylabel("Number of Episodes")
-axins.set_xlim(0, 100.)
-axins.set_ylim(-5., 10.)
-plt.xticks(visible=False)
-plt.yticks(visible=False)
-mark_inset(ax1, axins, loc1=2, loc2=4, fc="none", ec="0.5")
-# plt.draw()
-df = pd.DataFrame(
-    {"group": itertools.chain(*[[name] * len(dp) for name, dp in evaluation_rewards.items()]),
-     "Consecutive Goals Reached": np.concatenate([dp for name, dp in evaluation_rewards.items()])}
-)
-
-sns.boxplot(data=df, x="group", y="Consecutive Goals Reached", medianprops={"color": "red"}, flierprops={"marker": "x"},
-            fliersize=1, ax=ax2, palette={name: QUALITATIVE_COLOR_PALETTE[i] for i, name in enumerate(names)},
-            showmeans=True, meanprops={"marker": "o", "markerfacecolor": "white", "markeredgecolor": "black"})
-ax2.set_xlabel("")
+
+# df = pd.DataFrame(
+#     {"group": itertools.chain(*[[name] * len(dp) for name, dp in evaluation_rewards.items()]),
+#      "Consecutive Goals Reached": np.concatenate([dp for name, dp in evaluation_rewards.items()])}
+# )
+
+# sns.boxplot(data=df, x="group", y="Consecutive Goals Reached", medianprops={"color": "red"}, flierprops={"marker": "x"},
+#             fliersize=1, ax=ax2, palette={name: QUALITATIVE_COLOR_PALETTE[i] for i, name in enumerate(names)},
+#             showmeans=True, meanprops={"marker": "o", "markerfacecolor": "white", "markeredgecolor": "black"})
+# ax2.set_xlabel("")
+
+
 
 
 ax1.set_xlabel("Cycle")
-ax1.set_ylabel("Avg. Consecutive Goals Reached")
-ax1.legend()
+ax1.set_ylabel("Consecutive Goals Reached")
 
-ax1.set_xlim(0, x_max)
-ax1.set_ylim(-5)
+# legend with shorter lines but normal font
+ax1.legend(loc='upper left',  ncol=1, handlelength=.7)
 
-plt.gcf().set_size_inches(12, 4)
-plt.subplots_adjust(wspace=0.3, right=0.995, left=0.05, top=0.99)
-plt.show()
-# plt.savefig("../../../docs/figures/manipulate-asymmetry-ablation.pdf", format="pdf", bbox="tight")
+ax1.set_xlim(0, x_max)
+ax1.set_ylim(0, 50)
+ax1.set_yticks(np.arange(0, 50, 10))
+ax1.set_xticks(np.arange(0, 1200, 200))
+
+plt.gcf().set_size_inches(8, 4)
+plt.subplots_adjust(wspace=0., right=0.999, left=0.1, top=1, bottom=0.15)
+plt.savefig("../../../docs/figures/brain-vs-openai.pdf", format="pdf", bbox="tight")
```

### Comparing `angorapy-0.9.0/angorapy/analysis/plotting/plot_experiment_comparison_with_success.py` & `angorapy-0.9.1/angorapy/analysis/plotting/plot_experiment_comparison_with_success.py`

 * *Files identical despite different names*

### Comparing `angorapy-0.9.0/angorapy/analysis/plotting/plot_experiment_comparison_with_success_multiple_runs.py` & `angorapy-0.9.1/angorapy/analysis/plotting/plot_experiment_comparison_with_success_multiple_runs.py`

 * *Files identical despite different names*

### Comparing `angorapy-0.9.0/angorapy/analysis/plotting/plot_experiment_progression.py` & `angorapy-0.9.1/angorapy/analysis/plotting/plot_experiment_progression.py`

 * *Files identical despite different names*

### Comparing `angorapy-0.9.0/angorapy/analysis/plotting/plot_losses.py` & `angorapy-0.9.1/angorapy/analysis/plotting/plot_losses.py`

 * *Files identical despite different names*

### Comparing `angorapy-0.9.0/angorapy/analysis/sindy/autoencoder.py` & `angorapy-0.9.1/angorapy/analysis/sindy/autoencoder.py`

 * *Files identical despite different names*

### Comparing `angorapy-0.9.0/angorapy/analysis/util/sindy.py` & `angorapy-0.9.1/angorapy/analysis/util/sindy.py`

 * *Files identical despite different names*

### Comparing `angorapy-0.9.0/angorapy/analysis/visualization.py` & `angorapy-0.9.1/angorapy/analysis/visualization.py`

 * *Files identical despite different names*

### Comparing `angorapy-0.9.0/angorapy/benchmark.py` & `angorapy-0.9.1/angorapy/benchmark.py`

 * *Files identical despite different names*

### Comparing `angorapy-0.9.0/angorapy/common/activations.py` & `angorapy-0.9.1/angorapy/common/activations.py`

 * *Files identical despite different names*

### Comparing `angorapy-0.9.0/angorapy/common/const.py` & `angorapy-0.9.1/angorapy/common/const.py`

 * *Files identical despite different names*

### Comparing `angorapy-0.9.0/angorapy/common/data_buffers.py` & `angorapy-0.9.1/angorapy/common/data_buffers.py`

 * *Files identical despite different names*

### Comparing `angorapy-0.9.0/angorapy/common/layers.py` & `angorapy-0.9.1/angorapy/common/layers.py`

 * *Files identical despite different names*

### Comparing `angorapy-0.9.0/angorapy/common/loss.py` & `angorapy-0.9.1/angorapy/common/loss.py`

 * *Files identical despite different names*

### Comparing `angorapy-0.9.0/angorapy/common/mpi_optim.py` & `angorapy-0.9.1/angorapy/common/mpi_optim.py`

 * *Files identical despite different names*

### Comparing `angorapy-0.9.0/angorapy/common/policies.py` & `angorapy-0.9.1/angorapy/common/policies.py`

 * *Files identical despite different names*

### Comparing `angorapy-0.9.0/angorapy/common/reward.py` & `angorapy-0.9.1/angorapy/common/reward.py`

 * *Files identical despite different names*

### Comparing `angorapy-0.9.0/angorapy/common/senses.py` & `angorapy-0.9.1/angorapy/common/senses.py`

 * *Files identical despite different names*

### Comparing `angorapy-0.9.0/angorapy/common/transformers.py` & `angorapy-0.9.1/angorapy/common/transformers.py`

 * *Files identical despite different names*

### Comparing `angorapy-0.9.0/angorapy/common/wrappers.py` & `angorapy-0.9.1/angorapy/common/wrappers.py`

 * *Files identical despite different names*

### Comparing `angorapy-0.9.0/angorapy/configs/hp_config.py` & `angorapy-0.9.1/angorapy/configs/hp_config.py`

 * *Files identical despite different names*

### Comparing `angorapy-0.9.0/angorapy/configs/reward_config.py` & `angorapy-0.9.1/angorapy/configs/reward_config.py`

 * *Files identical despite different names*

### Comparing `angorapy-0.9.0/angorapy/environments/__init__.py` & `angorapy-0.9.1/angorapy/environments/__init__.py`

 * *Files identical despite different names*

### Comparing `angorapy-0.9.0/angorapy/environments/adapted.py` & `angorapy-0.9.1/angorapy/environments/adapted.py`

 * *Files identical despite different names*

### Comparing `angorapy-0.9.0/angorapy/environments/anthrobotics.py` & `angorapy-0.9.1/angorapy/environments/anthrobotics.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import abc
 from abc import ABC
 from collections import OrderedDict
 from os import path
-from typing import Optional, Union, Callable
+from typing import Optional, Union, Callable, Dict, Any
 
 import numpy as np
 import mujoco
 
 import gym
 from gym import error, logger, spaces
 
@@ -34,14 +34,15 @@
         raise NotImplementedError(type(observation), observation)
 
     return space
 
 
 class AnthropomorphicEnv(gym.Env, ABC):
     """Superclass for all environments."""
+    metadata: Dict[str, Any] = {"render_modes": ["human", "rgb_array"]}
 
     def __init__(
             self,
             model_path,
             frame_skip,
             initial_qpos=None,
             vision=False,
```

### Comparing `angorapy-0.9.0/angorapy/environments/assets/LICENSE.md` & `angorapy-0.9.1/angorapy/environments/assets/LICENSE.md`

 * *Files identical despite different names*

### Comparing `angorapy-0.9.0/angorapy/environments/assets/hand/manipulate_block.xml` & `angorapy-0.9.1/angorapy/environments/assets/hand/manipulate_block.xml`

 * *Files identical despite different names*

### Comparing `angorapy-0.9.0/angorapy/environments/assets/hand/manipulate_block_touch_sensors.xml` & `angorapy-0.9.1/angorapy/environments/assets/hand/manipulate_block_touch_sensors.xml`

 * *Files identical despite different names*

### Comparing `angorapy-0.9.0/angorapy/environments/assets/hand/manipulate_egg.xml` & `angorapy-0.9.1/angorapy/environments/assets/hand/manipulate_egg.xml`

 * *Files identical despite different names*

### Comparing `angorapy-0.9.0/angorapy/environments/assets/hand/manipulate_egg_touch_sensors.xml` & `angorapy-0.9.1/angorapy/environments/assets/hand/manipulate_egg_touch_sensors.xml`

 * *Files identical despite different names*

### Comparing `angorapy-0.9.0/angorapy/environments/assets/hand/manipulate_pen.xml` & `angorapy-0.9.1/angorapy/environments/assets/hand/manipulate_pen.xml`

 * *Files identical despite different names*

### Comparing `angorapy-0.9.0/angorapy/environments/assets/hand/manipulate_pen_touch_sensors.xml` & `angorapy-0.9.1/angorapy/environments/assets/hand/manipulate_pen_touch_sensors.xml`

 * *Files identical despite different names*

### Comparing `angorapy-0.9.0/angorapy/environments/assets/hand/robot.xml` & `angorapy-0.9.1/angorapy/environments/assets/hand/robot.xml`

 * *Files identical despite different names*

### Comparing `angorapy-0.9.0/angorapy/environments/assets/hand/robot_touch_sensors_92.xml` & `angorapy-0.9.1/angorapy/environments/assets/hand/robot_touch_sensors_92.xml`

 * *Files identical despite different names*

### Comparing `angorapy-0.9.0/angorapy/environments/assets/hand/shadowhand.xml` & `angorapy-0.9.1/angorapy/environments/assets/hand/shadowhand.xml`

 * *Files identical despite different names*

### Comparing `angorapy-0.9.0/angorapy/environments/assets/hand/shadowhand_manipulate.xml` & `angorapy-0.9.1/angorapy/environments/assets/hand/shadowhand_manipulate.xml`

 * *Files identical despite different names*

### Comparing `angorapy-0.9.0/angorapy/environments/assets/hand/shared.xml` & `angorapy-0.9.1/angorapy/environments/assets/hand/shared.xml`

 * *Files identical despite different names*

### Comparing `angorapy-0.9.0/angorapy/environments/assets/hand/shared_asset.xml` & `angorapy-0.9.1/angorapy/environments/assets/hand/shared_asset.xml`

 * *Files identical despite different names*

### Comparing `angorapy-0.9.0/angorapy/environments/assets/hand/shared_touch_sensors_92.xml` & `angorapy-0.9.1/angorapy/environments/assets/hand/shared_touch_sensors_92.xml`

 * *Files identical despite different names*

### Comparing `angorapy-0.9.0/angorapy/environments/assets/hand/touch_sensors.xml` & `angorapy-0.9.1/angorapy/environments/assets/hand/touch_sensors.xml`

 * *Files identical despite different names*

### Comparing `angorapy-0.9.0/angorapy/environments/assets/stls/hand/F1.stl` & `angorapy-0.9.1/angorapy/environments/assets/stls/hand/F1.stl`

 * *Files identical despite different names*

### Comparing `angorapy-0.9.0/angorapy/environments/assets/stls/hand/F2.stl` & `angorapy-0.9.1/angorapy/environments/assets/stls/hand/F2.stl`

 * *Files identical despite different names*

### Comparing `angorapy-0.9.0/angorapy/environments/assets/stls/hand/F3.stl` & `angorapy-0.9.1/angorapy/environments/assets/stls/hand/F3.stl`

 * *Files identical despite different names*

### Comparing `angorapy-0.9.0/angorapy/environments/assets/stls/hand/TH1_z.stl` & `angorapy-0.9.1/angorapy/environments/assets/stls/hand/TH1_z.stl`

 * *Files identical despite different names*

### Comparing `angorapy-0.9.0/angorapy/environments/assets/stls/hand/TH2_z.stl` & `angorapy-0.9.1/angorapy/environments/assets/stls/hand/TH2_z.stl`

 * *Files identical despite different names*

### Comparing `angorapy-0.9.0/angorapy/environments/assets/stls/hand/TH3_z.stl` & `angorapy-0.9.1/angorapy/environments/assets/stls/hand/TH3_z.stl`

 * *Files identical despite different names*

### Comparing `angorapy-0.9.0/angorapy/environments/assets/stls/hand/forearm_electric.stl` & `angorapy-0.9.1/angorapy/environments/assets/stls/hand/forearm_electric.stl`

 * *Files identical despite different names*

### Comparing `angorapy-0.9.0/angorapy/environments/assets/stls/hand/forearm_electric_cvx.stl` & `angorapy-0.9.1/angorapy/environments/assets/stls/hand/forearm_electric_cvx.stl`

 * *Files identical despite different names*

### Comparing `angorapy-0.9.0/angorapy/environments/assets/stls/hand/knuckle.stl` & `angorapy-0.9.1/angorapy/environments/assets/stls/hand/knuckle.stl`

 * *Files identical despite different names*

### Comparing `angorapy-0.9.0/angorapy/environments/assets/stls/hand/lfmetacarpal.stl` & `angorapy-0.9.1/angorapy/environments/assets/stls/hand/lfmetacarpal.stl`

 * *Files identical despite different names*

### Comparing `angorapy-0.9.0/angorapy/environments/assets/stls/hand/palm.stl` & `angorapy-0.9.1/angorapy/environments/assets/stls/hand/palm.stl`

 * *Files identical despite different names*

### Comparing `angorapy-0.9.0/angorapy/environments/assets/stls/hand/wrist.stl` & `angorapy-0.9.1/angorapy/environments/assets/stls/hand/wrist.stl`

 * *Files identical despite different names*

### Comparing `angorapy-0.9.0/angorapy/environments/assets/textures/block.png` & `angorapy-0.9.1/angorapy/environments/assets/textures/block.png`

 * *Files identical despite different names*

### Comparing `angorapy-0.9.0/angorapy/environments/assets/textures/block_hidden.png` & `angorapy-0.9.1/angorapy/environments/assets/textures/block_hidden.png`

 * *Files identical despite different names*

### Comparing `angorapy-0.9.0/angorapy/environments/hand/manipulate.py` & `angorapy-0.9.1/angorapy/environments/hand/manipulate.py`

 * *Files identical despite different names*

### Comparing `angorapy-0.9.0/angorapy/environments/hand/reach.py` & `angorapy-0.9.1/angorapy/environments/hand/reach.py`

 * *Files identical despite different names*

### Comparing `angorapy-0.9.0/angorapy/environments/hand/shadowhand.py` & `angorapy-0.9.1/angorapy/environments/hand/shadowhand.py`

 * *Files 2% similar despite different names*

```diff
@@ -97,14 +97,15 @@
                  render_mode: Optional[str] = None
                  ):
         gym.utils.EzPickle.__init__(**locals())
 
         self.relative_control = relative_control
         self._touch_sensor_id_site_id = []
         self._touch_sensor_id = []
+        self._thumb_touch_sensor_id = []
         self.distance_threshold = distance_threshold
         self.reward_type = "dense"
         self._freeze_wrist = False
         self.color_scheme = "default"
         self.viewpoint = "topdown"
 
         super(BaseShadowHandEnv, self).__init__(model_path=model, frame_skip=n_substeps, initial_qpos=initial_qpos,
@@ -143,14 +144,18 @@
     # INFORMATION METHODS
     def get_fingertip_positions(self):
         """Get positions of all fingertips in euclidean space. Each position is encoded by three floating point numbers,
         as such the output is a 15-D numpy array."""
         goal = [self.data.site(name).xpos.flatten() for name in FINGERTIP_SITE_NAMES]
         return np.array(goal).flatten()
 
+    def is_thumb_tip_touching(self):
+        if sum(self.data.sensordata[self._touch_sensor_id]) > 0.0:
+            return True
+
     # ENV METHODS
 
     def seed(self, seed=None):
         self.np_random, seed = seeding.np_random(seed)
         return [seed]
 
     def step(self, action: np.ndarray):
@@ -265,14 +270,17 @@
         """Initial configuration of the environment. Can be used to configure initial state
         and extract information from the simulation."""
         for k, v in zip(mj_get_category_names(self.model, "sensor"), self.model.sensor_adr):
             if b'robot0:TS_' in k:
                 # self._touch_sensor_id_site_id.append((v, self.model._site_name2id[k.replace('robot0:TS_', 'robot0:T_')]))
                 self._touch_sensor_id.append(v)
 
+                if b'thtip' in k:
+                    self._thumb_touch_sensor_id.append(v)
+
         if initial_state is not None:
             self.set_state(**initial_state)
 
     @abc.abstractmethod
     def _render_callback(self, render_targets=False):
         """A custom callback that is called before rendering. Can be used to implement custom visualizations."""
         pass
```

### Comparing `angorapy-0.9.0/angorapy/environments/hanoi.py` & `angorapy-0.9.1/angorapy/environments/hanoi.py`

 * *Files identical despite different names*

### Comparing `angorapy-0.9.0/angorapy/environments/rotations.py` & `angorapy-0.9.1/angorapy/environments/rotations.py`

 * *Files identical despite different names*

### Comparing `angorapy-0.9.0/angorapy/environments/utils.py` & `angorapy-0.9.1/angorapy/environments/utils.py`

 * *Files identical despite different names*

### Comparing `angorapy-0.9.0/angorapy/evaluate.py` & `angorapy-0.9.1/angorapy/evaluate.py`

 * *Files identical despite different names*

### Comparing `angorapy-0.9.0/angorapy/models/__init__.py` & `angorapy-0.9.1/angorapy/models/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -5,18 +5,24 @@
 from angorapy.models.convolutional import _build_visual_decoder, _build_openai_encoder
 from angorapy.models.mighty_maker import *
 from angorapy.models.shadow import build_shadow_brain_models, build_shadow_brain_base
 from angorapy.models.shadow_v2 import build_shadow_v2_brain_models, build_shadow_v2_brain_base
 from angorapy.models.simple import build_ffn_models, build_deeper_models, build_rnn_models, _build_encoding_sub_model, \
     build_simple_models
 
+from angorapy.utilities.model_utils import make_input_layers
+
 
 def get_model_builder(model="simple", model_type: str = "ffn", shared: bool = False, blind: bool = True) -> Callable:
     """Get a builder function for a model with the described parameters."""
     # TODO shared seems not to work yet
     params = locals()
     params["shared"] = "shared" if params["shared"] else "distinct"
     params["blind"] = "blind" if params["blind"] else ""
 
     params = [str(val) for key, val in sorted(params.items(), key=lambda x: x[0]) if val != ""]
 
     return globals()[f"build_{'_'.join(params)}_models"]
+
+
+def register_model(builder):
+    globals().update({builder.__name__: builder})
```

### Comparing `angorapy-0.9.0/angorapy/models/components.py` & `angorapy-0.9.1/angorapy/models/components.py`

 * *Files identical despite different names*

### Comparing `angorapy-0.9.0/angorapy/models/convolutional.py` & `angorapy-0.9.1/angorapy/models/convolutional.py`

 * *Files identical despite different names*

### Comparing `angorapy-0.9.0/angorapy/models/mighty_maker.py` & `angorapy-0.9.1/angorapy/models/mighty_maker.py`

 * *Files identical despite different names*

### Comparing `angorapy-0.9.0/angorapy/models/shadow.py` & `angorapy-0.9.1/angorapy/models/shadow.py`

 * *Files identical despite different names*

### Comparing `angorapy-0.9.0/angorapy/models/shadow_v2.py` & `angorapy-0.9.1/angorapy/models/shadow_v2.py`

 * *Files 0% similar despite different names*

```diff
@@ -82,15 +82,16 @@
     pmc, *_ = rnn_class(256,
                         stateful=True,
                         return_sequences=True,
                         batch_size=batch_and_sequence_shape[0],
                         return_state=True,
                         name="pmc_recurrent_layer",
                         recurrent_initializer=OrthogonalMP(),
-                        dtype="float32"
+                        dtype="float32",
+
                         )(pmc_input)
 
     m1_input = tf.keras.layers.concatenate([pmc, ssc_input, spl_input])
 
     m1 = TD(tf.keras.layers.Dense(96, name="m1"), )(m1_input)
     m1 = activation(name="M1_activation")(m1)
```

### Comparing `angorapy-0.9.0/angorapy/models/simple.py` & `angorapy-0.9.1/angorapy/models/simple.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,33 +10,28 @@
 from tensorflow.keras.layers import TimeDistributed
 from tensorflow.python.keras.utils.vis_utils import plot_model
 
 from angorapy.common.policies import BasePolicyDistribution, CategoricalPolicyDistribution, BetaPolicyDistribution, \
     MultiCategoricalPolicyDistribution, RBetaPolicyDistribution, GaussianPolicyDistribution
 from angorapy.common.wrappers import BaseWrapper, make_env
 from angorapy.models.components import _build_encoding_sub_model
+from angorapy.utilities.model_utils import make_input_layers
 from angorapy.utilities.util import env_extract_dims
 
 
 def build_ffn_models(env: BaseWrapper,
                      distribution: BasePolicyDistribution,
                      shared: bool = False,
                      layer_sizes: Tuple = (64, 64)):
     """Build a simple fully connected feed-forward model model."""
 
     # preparation
     state_dimensionality, n_actions = env_extract_dims(env)
 
-    input_list = []
-    for sense_name in state_dimensionality.keys():
-        if sense_name == "asymmetric":
-            continue
-
-        input_node = tf.keras.Input(shape=state_dimensionality[sense_name], name=sense_name)
-        input_list.append(input_node)
+    input_list = make_input_layers(env, None, None)
 
     if len(input_list) > 1:
         inputs = tf.keras.layers.Concatenate(name="flat_inputs")(input_list)
     else:
         inputs = input_list[0]
 
     # policy network
@@ -76,21 +71,15 @@
     Args:
         sequence_length:
     """
     # TODO: remove current workaround: solve issue with stateful masked RNNs by fixing the models sequence length
 
     state_dimensionality, n_actions = env_extract_dims(env)
 
-    input_list = []
-    for sense_name in state_dimensionality.keys():
-        if sense_name == "asymmetric":
-            continue
-
-        input_node = tf.keras.Input(batch_shape=(bs, sequence_length,) + state_dimensionality[sense_name], name=sense_name)
-        input_list.append(input_node)
+    input_list = make_input_layers(env, bs=bs, sequence_length=sequence_length)
 
     if len(input_list) > 1:
         inputs = tf.keras.layers.Concatenate(name="flat_inputs")(input_list)
     else:
         inputs = input_list[0]
 
     if "asymmetric" in state_dimensionality.keys():
```

### Comparing `angorapy-0.9.0/angorapy/monitor/app.py` & `angorapy-0.9.1/angorapy/monitor/app.py`

 * *Files 0% similar despite different names*

```diff
@@ -52,14 +52,15 @@
 
         eid_m = re.match("[0-9]+", str(exp_path.split("/")[-1]))
         if eid_m:
             eid = eid_m.group(0)
             model_path = os.path.join(BASE_SAVE_PATH, eid)
 
             if os.path.isfile(os.path.join(exp_path, "progress.json")):
+                print(eid)
                 with open(os.path.join(exp_path, "progress.json"), "r") as f:
                     progress = json.load(f)
 
                 try:
                     with open(os.path.join(exp_path, "meta.json"), "r") as f:
                         meta = json.load(f)
                 except:
```

### Comparing `angorapy-0.9.0/angorapy/observe.py` & `angorapy-0.9.1/angorapy/observe.py`

 * *Files identical despite different names*

### Comparing `angorapy-0.9.0/angorapy/pretrain.py` & `angorapy-0.9.1/angorapy/pretrain.py`

 * *Files identical despite different names*

### Comparing `angorapy-0.9.0/angorapy/train.py` & `angorapy-0.9.1/angorapy/train.py`

 * *Files 2% similar despite different names*

```diff
@@ -83,16 +83,19 @@
     # choose and make policy distribution
     if settings["distribution"] is None:
         distribution = autoselect_distribution(env)
     else:
         distribution = get_distribution_by_short_name(settings["distribution"])(env)
 
     # setting appropriate model building function
-    blind = not("vision" in list(env.observation_space["observation"].keys())
-                and len(env.observation_space["observation"]["vision"].shape) > 1)
+    try:
+        blind = not("vision" in list(env.observation_space["observation"].keys())
+                    and len(env.observation_space["observation"]["vision"].shape) > 1)
+    except:
+        blind = True
     build_models = get_model_builder(model=settings["architecture"], model_type=settings["model"], shared=settings["shared"],
                                      blind=blind)
 
     # announce experiment
     bc, ec, wn = COLORS["HEADER"], COLORS["ENDC"], COLORS["WARNING"]
     if verbose and is_root:
         env_action_space_type = "continuous" if isinstance(env.action_space, Box) else "discrete"
```

### Comparing `angorapy-0.9.0/angorapy/utilities/data_generation.py` & `angorapy-0.9.1/angorapy/utilities/data_generation.py`

 * *Files identical despite different names*

### Comparing `angorapy-0.9.0/angorapy/utilities/datatypes.py` & `angorapy-0.9.1/angorapy/utilities/datatypes.py`

 * *Files identical despite different names*

### Comparing `angorapy-0.9.0/angorapy/utilities/defaults.py` & `angorapy-0.9.1/angorapy/utilities/defaults.py`

 * *Files identical despite different names*

### Comparing `angorapy-0.9.0/angorapy/utilities/hooks.py` & `angorapy-0.9.1/angorapy/utilities/hooks.py`

 * *Files identical despite different names*

### Comparing `angorapy-0.9.0/angorapy/utilities/model_utils.py` & `angorapy-0.9.1/angorapy/utilities/model_utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 import tensorflow as tf
 from tensorflow.keras.layers import TimeDistributed
 
 import angorapy
 from angorapy.common.policies import BasePolicyDistribution
 from angorapy.common.wrappers import BaseWrapper
 from angorapy.utilities.error import IncompatibleModelException
-from angorapy.utilities.util import flatten
+from angorapy.utilities.util import flatten, env_extract_dims
 
 
 def is_recurrent_model(model: tf.keras.Model):
     """Check if given model is recurrent (i.e. contains a recurrent layer of any sort)"""
     for layer in model.submodules:
         if isinstance(layer, tf.keras.layers.RNN):
             return True
@@ -196,14 +196,34 @@
 
 
 def is_conv(layer):
     """Check if layer is convolutional."""
     return isinstance(layer, CONVOLUTION_BASE_CLASS)
 
 
+# Building helpers
+
+def make_input_layers(env, bs, sequence_length = None):
+    """Build input layers for a model acting on the given environment.
+
+    If the model is not recurrent, provide None for the sequence_length (default)"""
+
+    state_dimensionality, n_actions = env_extract_dims(env)
+    inputs = []
+
+    for modality in state_dimensionality.keys():
+        shape = (bs, )
+        if sequence_length is not None:
+            shape += (sequence_length, )
+        shape += tuple(state_dimensionality[modality])
+        inputs.append(tf.keras.Input(batch_shape=shape, name=modality))
+
+    return inputs
+
+
 # Validators
 
 def validate_model_builder(model_function: Callable, env: BaseWrapper, distribution: BasePolicyDistribution) -> None:
     models = model_function(env, distribution)
 
     # validate model order
     if not models[1].output_shape[-1] == 1:
```

### Comparing `angorapy-0.9.0/angorapy/utilities/monitor/plotting_base.py` & `angorapy-0.9.1/angorapy/utilities/monitor/plotting_base.py`

 * *Files identical despite different names*

### Comparing `angorapy-0.9.0/angorapy/utilities/monitor/statistical_plots.py` & `angorapy-0.9.1/angorapy/utilities/monitor/statistical_plots.py`

 * *Files identical despite different names*

### Comparing `angorapy-0.9.0/angorapy/utilities/monitor/training_plots.py` & `angorapy-0.9.1/angorapy/utilities/monitor/training_plots.py`

 * *Files identical despite different names*

### Comparing `angorapy-0.9.0/angorapy/utilities/monitoring.py` & `angorapy-0.9.1/angorapy/utilities/monitoring.py`

 * *Files identical despite different names*

### Comparing `angorapy-0.9.0/angorapy/utilities/plotting.py` & `angorapy-0.9.1/angorapy/utilities/plotting.py`

 * *Files identical despite different names*

### Comparing `angorapy-0.9.0/angorapy/utilities/statistics.py` & `angorapy-0.9.1/angorapy/utilities/statistics.py`

 * *Files identical despite different names*

### Comparing `angorapy-0.9.0/angorapy/utilities/util.py` & `angorapy-0.9.1/angorapy/utilities/util.py`

 * *Files identical despite different names*

### Comparing `angorapy-0.9.0/angorapy.egg-info/PKG-INFO` & `angorapy-0.9.1/angorapy.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: angorapy
-Version: 0.9.0
+Version: 0.9.1
 Summary: ANthropomorphic Goal-ORiented Modeling, Learning and Analysis for Neuroscience
 Home-page: https://github.com/ccnmaastricht/angorapy
 Author: Tonio Weidler
 Author-email: research@tonioweidler.de
 License: GPL-3.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
@@ -38,28 +38,60 @@
 
 This library is developed as part of the [Human Brain Project](https://www.humanbrainproject.eu/) at [CCN Maastricht](https://www.ccnmaastricht.com/). It is an effort to build software by neuroscientists, for neuroscientists. If you have suggestions, requests or questions, feel free to [open an issue](https://github.com/ccnmaastricht/angorapy/issues/new/choose).
 
 ![Manipulation Gif](docs/gifs/manipulate_best.gif)
 
 ## 📥 Installation
 
-AngoraPy is available on PyPI. 
+### Prerequisites
+AngoraPy requires Python 3.6 or higher. It is recommended to use a virtual environment to install AngoraPy and its dependencies. Additionally, some prerequisites are required. 
 
-```bash
-pip install angorapy
-```
+On Ubuntu, these can be installed by running
 
-### From source
-Alternatively, you can download this repository or the source code of any previous release or branch and install from source, using pip.
+    sudo apt-get install swig
 
-```bash
-pip install -e .
-```
+Additionally, to run AngoraPy with its native distribution, you need MPI installed. On Ubuntu, this can be done by running
+
+    sudo apt-get install libopenmpi-dev
+
+However, any other MPI implementation should work as well.
+
+### Installing AngoraPy
+
+#### Binaries
+AngoraPy is available as a binary package on PyPI. To install it, run 
+
+    pip install angorapy
+
+in your terminal.
+
+If you would like to install a specific version, you can specify it by appending `==<version>` to the command above. For example, to install version 0.9.0, run 
 
-This way, if you make changes to the source code, these will be recognized in the installation (without the need to reinstall).
+    pip install angorapy==0.9.0
+
+#### Source Installation
+To install AngoraPy from source, clone the repository and run `pip install -e .` in the root directory.
+
+### Post-Installation
+
+#### MuJoCo
+Gym installs both MuJoCo's new native Python bindings and the old mujoco-py bindings. You will not need the latter for AngoraPy, so you may uninstall it by running
+
+    pip uninstall mujoco-py
+
+#### Test Your Installation
+You can test your installation by running the following command in your terminal:
+
+    python -m angorapy.train CartPole-v1
+
+To test your MPI installation, run
+
+    mpirun -np <numthreads> --use-hwthread-cpus python -m angorapy.train LunarLanderContinuous-v2
+
+where `<numthreads>` is the number of threads you want to (and can) use.
 
 ### Docker
 Alternatively, you can install AngoraPy and all its dependencies in a docker container using the Dockerfile provided in this repository (/docker/Dockerfile). To this end, download the repository and build the docker image from the /docker directory:
 
 ```bash
 sudo docker build -t angorapy:master https://github.com/ccnmaastricht/angorapy.git#master -f - < Dockerfile
 ```
@@ -96,32 +128,24 @@
 To train agents with custom models, environments, etc. you write your own script. The following is a minimal example:
 
 ```python
 from angorapy.common.wrappers import make_env
 from angorapy.models import get_model_builder
 from angorapy.agent.ppo_agent import PPOAgent
 
-env = make_env("LunarLanderContinuous-v2")
-model_builder = get_model_builder("simple", "ffn")
-agent = PPOAgent(model_builder, env)
-agent.drill(100, 10, 512)
+env = make_env("ReachAbsolute-v0")
+model_builder = get_model_builder("shadow", "lstm")
+agent = PPOAgent(model_builder, env, workers=24)
+agent.drill(n=100, epochs=10, batch_size=512)
 ```
 
 For more details, consult the [examples](examples).
 
 ## 🎓 Documentation
-Detailed documentation of AngoraPy is provided in the READMEs of most subpackages. Additionally, we provide [examples and tutorials](examples) that get you started with writing your own scripts using AngoraPy. For further readings on specific modules, consult the following READMEs: 
-
- - [Agent](angorapy/agent) [WIP]
- - [Environments](angorapy/environments)
- - [Models](angorapy/models)
- - [Analysis](angorapy/analysis)
- - [Monitoring](angorapy/monitoring)
-
-If you are missing a documentation for a specific part of AngoraPy, feel free to open an issue and we will do our best to add it.
+We provide [examples](examples) that get you started with writing your own scripts using AngoraPy. Additionally there is a growing list of [tutorials](https://github.com/weidler/angorapy-tutorials). If you are missing a documentation for a specific part of AngoraPy, feel free to open an issue and we will do our best to add it.
 
 ## 🔀 Distributed Computation
 PPO is an asynchronous algorithm, allowing multiple parallel workers to generate experience independently. 
 We allow parallel gathering and optimization through MPI. Agents will automatically distribute their workers evenly on 
 the available CPU cores, while optimization is distributed over all available GPUs. If no GPUs are available, all CPUs 
 share the task of optimizing.
 
@@ -170,17 +194,21 @@
 The number of parallel workers will equal the number of nodes times the number of CPUs per node 
 (32 x 12 = 384 in the template above).
 
 ## 🔗 Citing AngoraPy
 
 If you use AngoraPy for your research, please cite us as follows
 
-    Weidler, T., & Senden, M. (2020). AngoraPy: Anthropomorphic Goal-Oriented Robotic Control for Neuroscientific Modeling [Computer software]
+    Weidler, Tonio, & Senden, Mario. (2023). AngoraPy - Anthropomorphic Goal-Oriented Robotic Control for Neuroscientific Modeling (0.9.0). Zenodo. https://doi.org/10.5281/zenodo.7770180
 
 Or using bibtex
 
-    @software{angorapy2020,
-        author = {Weidler, Tonio and Senden, Mario},
-        month = {3},
-        title = {{AngoraPy: Anthropomorphic Goal-Oriented Robotic Control for Neuroscientific Modeling}},
-        year = {2020}
-    }
+    @software{weidler_angorapy_2023,
+        author       = {Weidler, Tonio and Senden, Mario},
+        title        = {{AngoraPy - Anthropomorphic Goal-Oriented Robotic 
+                         Control for Neuroscientific Modeling}},
+        year         = 2023,
+        publisher    = {Zenodo},
+        version      = {0.9.0},
+        doi          = {10.5281/zenodo.6636482},
+        url          = {https://doi.org/10.5281/zenodo.6636482}
+   }
```

### Comparing `angorapy-0.9.0/angorapy.egg-info/SOURCES.txt` & `angorapy-0.9.1/angorapy.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -24,14 +24,15 @@
 angorapy/analysis/chiefinvestigation.py
 angorapy/analysis/dynamics.py
 angorapy/analysis/inspect_camera.py
 angorapy/analysis/plot_predictability.py
 angorapy/analysis/plot_predictability_grouped.py
 angorapy/analysis/plot_predictability_grouped_with_error_bars.py
 angorapy/analysis/plot_predictability_with_error_bars.py
+angorapy/analysis/plot_predictability_with_error_bars_single_figure.py
 angorapy/analysis/plot_utils.py
 angorapy/analysis/predictability.py
 angorapy/analysis/visualization.py
 angorapy/analysis/investigators/__init__.py
 angorapy/analysis/investigators/base_investigator.py
 angorapy/analysis/investigators/correlation.py
 angorapy/analysis/investigators/dynamics.py
@@ -137,15 +138,13 @@
 angorapy/utilities/statistics.py
 angorapy/utilities/util.py
 angorapy/utilities/monitor/__init__.py
 angorapy/utilities/monitor/plotting_base.py
 angorapy/utilities/monitor/statistical_plots.py
 angorapy/utilities/monitor/training_plots.py
 tests/__init__.py
-tests/mpimemory.py
-tests/numpy_optim.py
 tests/test_agent.py
+tests/test_builtin_models.py
 tests/test_distributions.py
 tests/test_environments.py
 tests/test_model_utils.py
-tests/test_statistics.py
-tests/tete.py
+tests/test_statistics.py
```

### Comparing `angorapy-0.9.0/setup.py` & `angorapy-0.9.1/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -5,47 +5,49 @@
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 
 setup(
     name='angorapy',
-    version='0.9.0',
+    version='0.9.1',
     description='ANthropomorphic Goal-ORiented Modeling, Learning and Analysis for Neuroscience',
     long_description_content_type='text/markdown',
     long_description=long_description,
     url='https://github.com/ccnmaastricht/angorapy',
     author='Tonio Weidler',
     author_email='research@tonioweidler.de',
     license='GPL-3.0',
     packages=find_packages(),
     include_package_data=True,
     install_requires=[
-        "imageio",
+        "swig==4.1.1",
+        "imageio==2.28.1",
         "numpy==1.19.2",
-        "box2d-py",
-        "gym==0.26.2",
-        "mujoco==2.2.2",
+        "box2d-py==2.3.5",
+        "gym[all]==0.26.2",
+        "mujoco==2.2",
         "tensorflow==2.4.2",
         "tensorflow_probability==0.12.2",
+        "tensorflow_graphics==2021.12.3",
         "mpi4py==3.1.3",
         "tqdm",
         "simplejson",
         "psutil",
         "scipy",
         "scikit-learn",
         "argcomplete",
         "matplotlib",
         "scikit-learn==0.24.1",
         "pandas==1.4.4",
         "nvidia-ml-py3",
         "seaborn",
         "distance",
         "protobuf==3.19.0",
-        "panda_gym",
+        "panda_gym==3.0.6",
         
         "keras_cortex==0.0.7",
 
         # webinterface
         "itsdangerous==2.0.1",
         "werkzeug==2.0.3",
         "Flask~=1.1.2",
```

### Comparing `angorapy-0.9.0/tests/test_agent.py` & `angorapy-0.9.1/tests/test_agent.py`

 * *Files identical despite different names*

### Comparing `angorapy-0.9.0/tests/test_distributions.py` & `angorapy-0.9.1/tests/test_distributions.py`

 * *Files identical despite different names*

### Comparing `angorapy-0.9.0/tests/test_environments.py` & `angorapy-0.9.1/tests/test_environments.py`

 * *Files identical despite different names*

### Comparing `angorapy-0.9.0/tests/test_model_utils.py` & `angorapy-0.9.1/tests/test_model_utils.py`

 * *Files identical despite different names*

### Comparing `angorapy-0.9.0/tests/test_statistics.py` & `angorapy-0.9.1/tests/test_statistics.py`

 * *Files identical despite different names*

