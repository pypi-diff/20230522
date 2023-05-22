# Comparing `tmp/persyn-0.0.4.tar.gz` & `tmp/persyn-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "persyn-0.0.4.tar", last modified: Thu Mar 30 04:12:57 2023, max compression
+gzip compressed data, was "persyn-0.0.9.tar", last modified: Mon May 22 01:56:22 2023, max compression
```

## Comparing `persyn-0.0.4.tar` & `persyn-0.0.9.tar`

### file list

```diff
@@ -1,132 +1,131 @@
-drwxrwxr-x   0 rob       (1000) rob       (1000)        0 2023-03-30 04:12:57.329997 persyn-0.0.4/
--rw-rw-r--   0 rob       (1000) rob       (1000)     1058 2023-01-09 01:22:11.000000 persyn-0.0.4/LICENSE.txt
--rw-rw-r--   0 rob       (1000) rob       (1000)     3059 2023-03-30 04:12:57.329997 persyn-0.0.4/PKG-INFO
--rw-rw-r--   0 rob       (1000) rob       (1000)     2482 2023-02-25 20:04:24.000000 persyn-0.0.4/README.md
--rw-rw-r--   0 rob       (1000) rob       (1000)     2128 2023-03-30 04:12:43.000000 persyn-0.0.4/pyproject.toml
--rw-rw-r--   0 rob       (1000) rob       (1000)       38 2023-03-30 04:12:57.329997 persyn-0.0.4/setup.cfg
-drwxrwxr-x   0 rob       (1000) rob       (1000)        0 2023-03-30 04:12:57.313997 persyn-0.0.4/src/
--rw-rw-r--   0 rob       (1000) rob       (1000)        0 2023-01-09 01:22:11.000000 persyn-0.0.4/src/__init__.py
-drwxrwxr-x   0 rob       (1000) rob       (1000)        0 2023-03-30 04:12:57.313997 persyn-0.0.4/src/chat/
--rw-rw-r--   0 rob       (1000) rob       (1000)        0 2023-01-09 01:22:11.000000 persyn-0.0.4/src/chat/__init__.py
--rw-rw-r--   0 rob       (1000) rob       (1000)    14686 2023-03-30 04:10:20.000000 persyn-0.0.4/src/chat/common.py
-drwxrwxr-x   0 rob       (1000) rob       (1000)        0 2023-03-30 04:12:57.313997 persyn-0.0.4/src/chat/discord/
--rwxr-xr-x   0 rob       (1000) rob       (1000)     1740 2022-11-07 00:33:58.000000 persyn-0.0.4/src/chat/discord/basic.py
--rwxrwxr-x   0 rob       (1000) rob       (1000)    11030 2023-03-30 04:10:20.000000 persyn-0.0.4/src/chat/discord/bot.py
-drwxrwxr-x   0 rob       (1000) rob       (1000)        0 2023-03-30 04:12:57.313997 persyn-0.0.4/src/chat/mastodon/
--rwxrwxr-x   0 rob       (1000) rob       (1000)    11512 2023-03-30 04:10:20.000000 persyn-0.0.4/src/chat/mastodon/bot.py
--rw-rw-r--   0 rob       (1000) rob       (1000)     2001 2023-01-09 01:22:11.000000 persyn-0.0.4/src/chat/mastodon/login.py
--rwxrwxr-x   0 rob       (1000) rob       (1000)     1208 2023-01-09 01:22:11.000000 persyn-0.0.4/src/chat/mastodon/masto-login.py
--rwxr-xr-x   0 rob       (1000) rob       (1000)     1919 2022-11-20 03:02:40.000000 persyn-0.0.4/src/chat/mastodon/masto-stream.py
--rw-rw-r--   0 rob       (1000) rob       (1000)     3314 2023-02-25 20:04:24.000000 persyn-0.0.4/src/chat/simple.py
-drwxrwxr-x   0 rob       (1000) rob       (1000)        0 2023-03-30 04:12:57.313997 persyn-0.0.4/src/chat/slack/
--rwxrwxr-x   0 rob       (1000) rob       (1000)    18670 2023-03-30 04:10:20.000000 persyn-0.0.4/src/chat/slack/bot.py
-drwxrwxr-x   0 rob       (1000) rob       (1000)        0 2023-03-30 04:12:57.313997 persyn-0.0.4/src/chat/stdio/
--rw-rw-r--   0 rob       (1000) rob       (1000)     1488 2023-02-25 20:04:24.000000 persyn-0.0.4/src/chat/stdio/add_goal.py
--rw-rw-r--   0 rob       (1000) rob       (1000)     1436 2023-02-25 20:04:24.000000 persyn-0.0.4/src/chat/stdio/elaborate.py
--rwxrwxr-x   0 rob       (1000) rob       (1000)     3416 2023-03-30 04:10:20.000000 persyn-0.0.4/src/chat/stdio/import_text.py
--rw-rw-r--   0 rob       (1000) rob       (1000)     1603 2023-02-25 20:04:24.000000 persyn-0.0.4/src/chat/stdio/inject_idea.py
--rw-rw-r--   0 rob       (1000) rob       (1000)     1647 2023-02-25 20:04:24.000000 persyn-0.0.4/src/chat/stdio/opine.py
--rw-rw-r--   0 rob       (1000) rob       (1000)     1606 2023-02-25 20:04:24.000000 persyn-0.0.4/src/chat/stdio/read_rss.py
--rw-rw-r--   0 rob       (1000) rob       (1000)     1760 2023-03-30 04:10:20.000000 persyn-0.0.4/src/chat/stdio/read_url.py
--rw-rw-r--   0 rob       (1000) rob       (1000)     1491 2023-02-25 20:04:24.000000 persyn-0.0.4/src/chat/stdio/send_chat.py
--rw-rw-r--   0 rob       (1000) rob       (1000)     1671 2023-02-25 20:04:24.000000 persyn-0.0.4/src/chat/stdio/summarize.py
-drwxrwxr-x   0 rob       (1000) rob       (1000)        0 2023-03-30 04:12:57.317997 persyn-0.0.4/src/dreams/
--rw-rw-r--   0 rob       (1000) rob       (1000)        0 2023-01-09 01:22:11.000000 persyn-0.0.4/src/dreams/__init__.py
-drwxrwxr-x   0 rob       (1000) rob       (1000)        0 2023-03-30 04:12:57.317997 persyn-0.0.4/src/dreams/clip_interrogator/
--rw-rw-r--   0 rob       (1000) rob       (1000)        0 2023-01-09 01:22:11.000000 persyn-0.0.4/src/dreams/clip_interrogator/__init__.py
--rw-rw-r--   0 rob       (1000) rob       (1000)    10568 2023-01-09 01:22:11.000000 persyn-0.0.4/src/dreams/clip_interrogator/interrogator.py
--rw-rw-r--   0 rob       (1000) rob       (1000)     5864 2023-02-25 20:04:24.000000 persyn-0.0.4/src/dreams/dreams.py
-drwxrwxr-x   0 rob       (1000) rob       (1000)        0 2023-03-30 04:12:57.309997 persyn-0.0.4/src/dreams/env/
-drwxrwxr-x   0 rob       (1000) rob       (1000)        0 2023-03-30 04:12:57.317997 persyn-0.0.4/src/dreams/env/bin/
--rw-rw-r--   0 rob       (1000) rob       (1000)     1199 2023-01-15 02:17:08.000000 persyn-0.0.4/src/dreams/env/bin/activate_this.py
--rwxrwxr-x   0 rob       (1000) rob       (1000)     1721 2023-01-15 03:32:50.000000 persyn-0.0.4/src/dreams/env/bin/jp.py
-drwxrwxr-x   0 rob       (1000) rob       (1000)        0 2023-03-30 04:12:57.317997 persyn-0.0.4/src/dreams/prompt-parrot/
--rw-rw-r--   0 rob       (1000) rob       (1000)     2939 2023-01-09 01:22:11.000000 persyn-0.0.4/src/dreams/prompt-parrot/prompt-parrot.py
--rwxr-xr-x   0 rob       (1000) rob       (1000)      434 2022-11-13 03:35:28.000000 persyn-0.0.4/src/dreams/receive-sqs.py
--rwxr-xr-x   0 rob       (1000) rob       (1000)      898 2022-11-21 01:01:15.000000 persyn-0.0.4/src/dreams/send-sqs.py
--rw-rw-r--   0 rob       (1000) rob       (1000)     6366 2023-02-25 20:04:24.000000 persyn-0.0.4/src/dreams/stable_diffusion.py
-drwxrwxr-x   0 rob       (1000) rob       (1000)        0 2023-03-30 04:12:57.317997 persyn-0.0.4/src/dreams/stylegan2/
--rwxr-xr-x   0 rob       (1000) rob       (1000)    30282 2022-02-21 19:19:05.000000 persyn-0.0.4/src/dreams/stylegan2/dataset_tool.py
-drwxrwxr-x   0 rob       (1000) rob       (1000)        0 2023-03-30 04:12:57.317997 persyn-0.0.4/src/dreams/stylegan2/dnnlib/
--rwxr-xr-x   0 rob       (1000) rob       (1000)      774 2022-02-21 19:19:28.000000 persyn-0.0.4/src/dreams/stylegan2/dnnlib/__init__.py
-drwxrwxr-x   0 rob       (1000) rob       (1000)        0 2023-03-30 04:12:57.317997 persyn-0.0.4/src/dreams/stylegan2/dnnlib/submission/
--rwxr-xr-x   0 rob       (1000) rob       (1000)      274 2022-02-21 19:19:28.000000 persyn-0.0.4/src/dreams/stylegan2/dnnlib/submission/__init__.py
-drwxrwxr-x   0 rob       (1000) rob       (1000)        0 2023-03-30 04:12:57.321997 persyn-0.0.4/src/dreams/stylegan2/dnnlib/submission/internal/
--rwxr-xr-x   0 rob       (1000) rob       (1000)      247 2022-02-21 19:19:28.000000 persyn-0.0.4/src/dreams/stylegan2/dnnlib/submission/internal/__init__.py
--rwxr-xr-x   0 rob       (1000) rob       (1000)      769 2022-02-21 19:19:28.000000 persyn-0.0.4/src/dreams/stylegan2/dnnlib/submission/internal/local.py
--rwxr-xr-x   0 rob       (1000) rob       (1000)     4245 2022-02-21 19:19:28.000000 persyn-0.0.4/src/dreams/stylegan2/dnnlib/submission/run_context.py
--rwxr-xr-x   0 rob       (1000) rob       (1000)    13502 2022-02-21 19:19:28.000000 persyn-0.0.4/src/dreams/stylegan2/dnnlib/submission/submit.py
-drwxrwxr-x   0 rob       (1000) rob       (1000)        0 2023-03-30 04:12:57.321997 persyn-0.0.4/src/dreams/stylegan2/dnnlib/tflib/
--rwxr-xr-x   0 rob       (1000) rob       (1000)      467 2022-02-21 19:19:28.000000 persyn-0.0.4/src/dreams/stylegan2/dnnlib/tflib/__init__.py
--rwxr-xr-x   0 rob       (1000) rob       (1000)     8038 2022-02-21 19:19:28.000000 persyn-0.0.4/src/dreams/stylegan2/dnnlib/tflib/autosummary.py
--rwxr-xr-x   0 rob       (1000) rob       (1000)     7223 2022-02-21 19:19:28.000000 persyn-0.0.4/src/dreams/stylegan2/dnnlib/tflib/custom_ops.py
--rwxr-xr-x   0 rob       (1000) rob       (1000)    29982 2022-02-21 19:19:28.000000 persyn-0.0.4/src/dreams/stylegan2/dnnlib/tflib/network.py
-drwxrwxr-x   0 rob       (1000) rob       (1000)        0 2023-03-30 04:12:57.321997 persyn-0.0.4/src/dreams/stylegan2/dnnlib/tflib/ops/
--rwxr-xr-x   0 rob       (1000) rob       (1000)      235 2022-02-21 19:19:28.000000 persyn-0.0.4/src/dreams/stylegan2/dnnlib/tflib/ops/__init__.py
--rwxr-xr-x   0 rob       (1000) rob       (1000)     8539 2022-02-21 19:19:28.000000 persyn-0.0.4/src/dreams/stylegan2/dnnlib/tflib/ops/fused_bias_act.py
--rwxr-xr-x   0 rob       (1000) rob       (1000)    16588 2022-02-21 19:19:28.000000 persyn-0.0.4/src/dreams/stylegan2/dnnlib/tflib/ops/upfirdn_2d.py
--rwxr-xr-x   0 rob       (1000) rob       (1000)    20298 2022-02-21 19:19:28.000000 persyn-0.0.4/src/dreams/stylegan2/dnnlib/tflib/optimizer.py
--rwxr-xr-x   0 rob       (1000) rob       (1000)     9675 2022-02-21 19:19:28.000000 persyn-0.0.4/src/dreams/stylegan2/dnnlib/tflib/tfutil.py
--rwxr-xr-x   0 rob       (1000) rob       (1000)    13916 2022-02-21 19:19:28.000000 persyn-0.0.4/src/dreams/stylegan2/dnnlib/util.py
-drwxrwxr-x   0 rob       (1000) rob       (1000)        0 2023-03-30 04:12:57.309997 persyn-0.0.4/src/dreams/stylegan2/env/
-drwxrwxr-x   0 rob       (1000) rob       (1000)        0 2023-03-30 04:12:57.321997 persyn-0.0.4/src/dreams/stylegan2/env/bin/
--rw-r--r--   0 rob       (1000) rob       (1000)     1137 2022-02-21 19:19:51.000000 persyn-0.0.4/src/dreams/stylegan2/env/bin/activate_this.py
--rwxr-xr-x   0 rob       (1000) rob       (1000)     2722 2022-02-21 19:19:05.000000 persyn-0.0.4/src/dreams/stylegan2/make_a_face.py
-drwxrwxr-x   0 rob       (1000) rob       (1000)        0 2023-03-30 04:12:57.321997 persyn-0.0.4/src/dreams/stylegan2/metrics/
--rwxr-xr-x   0 rob       (1000) rob       (1000)      235 2022-02-21 19:19:28.000000 persyn-0.0.4/src/dreams/stylegan2/metrics/__init__.py
--rwxr-xr-x   0 rob       (1000) rob       (1000)     3330 2022-02-21 19:19:28.000000 persyn-0.0.4/src/dreams/stylegan2/metrics/frechet_inception_distance.py
--rwxr-xr-x   0 rob       (1000) rob       (1000)     2587 2022-02-21 19:19:28.000000 persyn-0.0.4/src/dreams/stylegan2/metrics/inception_score.py
--rwxr-xr-x   0 rob       (1000) rob       (1000)     9978 2022-02-21 19:19:28.000000 persyn-0.0.4/src/dreams/stylegan2/metrics/linear_separability.py
--rwxr-xr-x   0 rob       (1000) rob       (1000)     7055 2022-02-21 19:19:28.000000 persyn-0.0.4/src/dreams/stylegan2/metrics/metric_base.py
--rwxr-xr-x   0 rob       (1000) rob       (1000)     2311 2022-02-21 19:19:28.000000 persyn-0.0.4/src/dreams/stylegan2/metrics/metric_defaults.py
--rwxr-xr-x   0 rob       (1000) rob       (1000)     5605 2022-02-21 19:19:28.000000 persyn-0.0.4/src/dreams/stylegan2/metrics/perceptual_path_length.py
--rwxr-xr-x   0 rob       (1000) rob       (1000)    11437 2022-02-21 19:19:28.000000 persyn-0.0.4/src/dreams/stylegan2/metrics/precision_recall.py
--rwxr-xr-x   0 rob       (1000) rob       (1000)     7521 2022-02-21 19:19:05.000000 persyn-0.0.4/src/dreams/stylegan2/pretrained_networks.py
--rwxr-xr-x   0 rob       (1000) rob       (1000)     8975 2022-02-21 19:19:05.000000 persyn-0.0.4/src/dreams/stylegan2/projector.py
--rwxr-xr-x   0 rob       (1000) rob       (1000)     8245 2022-02-21 19:19:05.000000 persyn-0.0.4/src/dreams/stylegan2/run_generator.py
--rwxr-xr-x   0 rob       (1000) rob       (1000)     3447 2022-02-21 19:19:05.000000 persyn-0.0.4/src/dreams/stylegan2/run_metrics.py
--rwxr-xr-x   0 rob       (1000) rob       (1000)     6963 2022-02-21 19:19:05.000000 persyn-0.0.4/src/dreams/stylegan2/run_projector.py
--rwxr-xr-x   0 rob       (1000) rob       (1000)     8473 2022-02-21 19:19:05.000000 persyn-0.0.4/src/dreams/stylegan2/run_training.py
-drwxrwxr-x   0 rob       (1000) rob       (1000)        0 2023-03-30 04:12:57.321997 persyn-0.0.4/src/dreams/stylegan2/training/
--rwxr-xr-x   0 rob       (1000) rob       (1000)      235 2022-02-21 19:19:28.000000 persyn-0.0.4/src/dreams/stylegan2/training/__init__.py
--rwxr-xr-x   0 rob       (1000) rob       (1000)     9881 2022-02-21 19:19:28.000000 persyn-0.0.4/src/dreams/stylegan2/training/dataset.py
--rwxr-xr-x   0 rob       (1000) rob       (1000)    10731 2022-02-21 19:19:28.000000 persyn-0.0.4/src/dreams/stylegan2/training/loss.py
--rwxr-xr-x   0 rob       (1000) rob       (1000)     5706 2022-02-21 19:19:28.000000 persyn-0.0.4/src/dreams/stylegan2/training/misc.py
--rwxr-xr-x   0 rob       (1000) rob       (1000)    33273 2022-02-21 19:19:28.000000 persyn-0.0.4/src/dreams/stylegan2/training/networks_stylegan.py
--rwxr-xr-x   0 rob       (1000) rob       (1000)    38074 2022-02-21 19:19:28.000000 persyn-0.0.4/src/dreams/stylegan2/training/networks_stylegan2.py
--rwxr-xr-x   0 rob       (1000) rob       (1000)    19892 2022-02-21 19:19:28.000000 persyn-0.0.4/src/dreams/stylegan2/training/training_loop.py
-drwxrwxr-x   0 rob       (1000) rob       (1000)        0 2023-03-30 04:12:57.325997 persyn-0.0.4/src/interaction/
--rw-rw-r--   0 rob       (1000) rob       (1000)        0 2023-01-09 01:22:11.000000 persyn-0.0.4/src/interaction/__init__.py
--rw-rw-r--   0 rob       (1000) rob       (1000)     1008 2023-01-09 01:22:11.000000 persyn-0.0.4/src/interaction/chrono.py
--rw-rw-r--   0 rob       (1000) rob       (1000)    17184 2023-03-30 04:10:20.000000 persyn-0.0.4/src/interaction/cns.py
--rw-rw-r--   0 rob       (1000) rob       (1000)     2855 2023-03-30 04:10:20.000000 persyn-0.0.4/src/interaction/completion.py
--rw-rw-r--   0 rob       (1000) rob       (1000)    29689 2023-02-25 20:04:24.000000 persyn-0.0.4/src/interaction/feels.py
--rw-rw-r--   0 rob       (1000) rob       (1000)    25880 2023-03-30 04:10:20.000000 persyn-0.0.4/src/interaction/gpt.py
--rwxrwxr-x   0 rob       (1000) rob       (1000)       60 2023-01-09 01:22:11.000000 persyn-0.0.4/src/interaction/install.py
--rw-rw-r--   0 rob       (1000) rob       (1000)    22519 2023-03-30 04:10:20.000000 persyn-0.0.4/src/interaction/interact.py
--rwxrwxr-x   0 rob       (1000) rob       (1000)    12601 2023-03-30 04:10:20.000000 persyn-0.0.4/src/interaction/interact_server.py
--rw-rw-r--   0 rob       (1000) rob       (1000)    37477 2023-03-30 04:10:20.000000 persyn-0.0.4/src/interaction/memory.py
--rw-rw-r--   0 rob       (1000) rob       (1000)     2176 2023-03-30 04:10:20.000000 persyn-0.0.4/src/interaction/messages.py
--rw-rw-r--   0 rob       (1000) rob       (1000)    13814 2023-02-25 20:04:24.000000 persyn-0.0.4/src/interaction/nlp_cloud.py
-drwxrwxr-x   0 rob       (1000) rob       (1000)        0 2023-03-30 04:12:57.313997 persyn-0.0.4/src/interaction/notebooks/
-drwxrwxr-x   0 rob       (1000) rob       (1000)        0 2023-03-30 04:12:57.313997 persyn-0.0.4/src/interaction/notebooks/env/
-drwxrwxr-x   0 rob       (1000) rob       (1000)        0 2023-03-30 04:12:57.325997 persyn-0.0.4/src/interaction/notebooks/env/bin/
--rw-rw-r--   0 rob       (1000) rob       (1000)     1199 2022-10-23 00:31:31.000000 persyn-0.0.4/src/interaction/notebooks/env/bin/activate_this.py
--rwxrwxr-x   0 rob       (1000) rob       (1000)     1732 2022-12-04 20:53:32.000000 persyn-0.0.4/src/interaction/notebooks/env/bin/jp.py
--rw-rw-r--   0 rob       (1000) rob       (1000)    13396 2023-02-25 20:04:24.000000 persyn-0.0.4/src/interaction/relationships.py
--rw-rw-r--   0 rob       (1000) rob       (1000)     2725 2023-01-09 01:22:11.000000 persyn-0.0.4/src/interaction/reminders.py
--rw-rw-r--   0 rob       (1000) rob       (1000)     1248 2023-01-09 01:22:11.000000 persyn-0.0.4/src/interaction/voice.py
--rwxrwxr-x   0 rob       (1000) rob       (1000)      863 2023-01-09 01:22:11.000000 persyn-0.0.4/src/kill_bot.py
--rwxrwxr-x   0 rob       (1000) rob       (1000)     4548 2023-02-25 20:04:24.000000 persyn-0.0.4/src/launch_bot.py
-drwxrwxr-x   0 rob       (1000) rob       (1000)        0 2023-03-30 04:12:57.325997 persyn-0.0.4/src/persyn.egg-info/
--rw-rw-r--   0 rob       (1000) rob       (1000)     3059 2023-03-30 04:12:57.000000 persyn-0.0.4/src/persyn.egg-info/PKG-INFO
--rw-rw-r--   0 rob       (1000) rob       (1000)     3531 2023-03-30 04:12:57.000000 persyn-0.0.4/src/persyn.egg-info/SOURCES.txt
--rw-rw-r--   0 rob       (1000) rob       (1000)        1 2023-03-30 04:12:57.000000 persyn-0.0.4/src/persyn.egg-info/dependency_links.txt
--rw-rw-r--   0 rob       (1000) rob       (1000)      653 2023-03-30 04:12:57.000000 persyn-0.0.4/src/persyn.egg-info/entry_points.txt
--rw-rw-r--   0 rob       (1000) rob       (1000)      514 2023-03-30 04:12:57.000000 persyn-0.0.4/src/persyn.egg-info/requires.txt
--rw-rw-r--   0 rob       (1000) rob       (1000)       59 2023-03-30 04:12:57.000000 persyn-0.0.4/src/persyn.egg-info/top_level.txt
-drwxrwxr-x   0 rob       (1000) rob       (1000)        0 2023-03-30 04:12:57.329997 persyn-0.0.4/src/utils/
--rw-rw-r--   0 rob       (1000) rob       (1000)        0 2023-01-09 01:22:11.000000 persyn-0.0.4/src/utils/__init__.py
--rw-rw-r--   0 rob       (1000) rob       (1000)     5169 2023-01-09 01:22:11.000000 persyn-0.0.4/src/utils/art.py
--rw-rw-r--   0 rob       (1000) rob       (1000)     1623 2023-03-30 04:10:20.000000 persyn-0.0.4/src/utils/color_logging.py
--rw-rw-r--   0 rob       (1000) rob       (1000)     5309 2023-03-30 04:10:20.000000 persyn-0.0.4/src/utils/config.py
+drwxrwxr-x   0 rob       (1000) rob       (1000)        0 2023-05-22 01:56:22.282214 persyn-0.0.9/
+-rw-rw-r--   0 rob       (1000) rob       (1000)     1058 2023-01-09 01:22:11.000000 persyn-0.0.9/LICENSE.txt
+-rw-rw-r--   0 rob       (1000) rob       (1000)     3059 2023-05-22 01:56:22.282214 persyn-0.0.9/PKG-INFO
+-rw-rw-r--   0 rob       (1000) rob       (1000)     2482 2023-05-22 01:51:08.000000 persyn-0.0.9/README.md
+-rw-rw-r--   0 rob       (1000) rob       (1000)     2219 2023-05-22 01:56:10.000000 persyn-0.0.9/pyproject.toml
+-rw-rw-r--   0 rob       (1000) rob       (1000)       38 2023-05-22 01:56:22.282214 persyn-0.0.9/setup.cfg
+drwxrwxr-x   0 rob       (1000) rob       (1000)        0 2023-05-22 01:56:22.270214 persyn-0.0.9/src/
+-rw-rw-r--   0 rob       (1000) rob       (1000)        0 2023-05-22 01:51:08.000000 persyn-0.0.9/src/__init__.py
+drwxrwxr-x   0 rob       (1000) rob       (1000)        0 2023-05-22 01:56:22.270214 persyn-0.0.9/src/chat/
+-rw-rw-r--   0 rob       (1000) rob       (1000)        0 2023-05-22 01:51:08.000000 persyn-0.0.9/src/chat/__init__.py
+-rw-rw-r--   0 rob       (1000) rob       (1000)    14686 2023-05-22 01:51:08.000000 persyn-0.0.9/src/chat/common.py
+drwxrwxr-x   0 rob       (1000) rob       (1000)        0 2023-05-22 01:56:22.270214 persyn-0.0.9/src/chat/discord/
+-rwxrwxr-x   0 rob       (1000) rob       (1000)    11030 2023-05-22 01:51:08.000000 persyn-0.0.9/src/chat/discord/bot.py
+drwxrwxr-x   0 rob       (1000) rob       (1000)        0 2023-05-22 01:56:22.270214 persyn-0.0.9/src/chat/mastodon/
+-rwxrwxr-x   0 rob       (1000) rob       (1000)    11512 2023-05-22 01:51:08.000000 persyn-0.0.9/src/chat/mastodon/bot.py
+-rw-rw-r--   0 rob       (1000) rob       (1000)     2001 2023-05-22 01:51:08.000000 persyn-0.0.9/src/chat/mastodon/login.py
+-rwxrwxr-x   0 rob       (1000) rob       (1000)     1208 2023-05-22 01:51:08.000000 persyn-0.0.9/src/chat/mastodon/masto-login.py
+-rw-rw-r--   0 rob       (1000) rob       (1000)     3314 2023-05-22 01:51:08.000000 persyn-0.0.9/src/chat/simple.py
+drwxrwxr-x   0 rob       (1000) rob       (1000)        0 2023-05-22 01:56:22.270214 persyn-0.0.9/src/chat/slack/
+-rwxrwxr-x   0 rob       (1000) rob       (1000)    18670 2023-05-22 01:51:08.000000 persyn-0.0.9/src/chat/slack/bot.py
+drwxrwxr-x   0 rob       (1000) rob       (1000)        0 2023-05-22 01:56:22.274214 persyn-0.0.9/src/chat/stdio/
+-rw-rw-r--   0 rob       (1000) rob       (1000)     1488 2023-05-22 01:51:08.000000 persyn-0.0.9/src/chat/stdio/add_goal.py
+-rw-rw-r--   0 rob       (1000) rob       (1000)     1436 2023-05-22 01:51:08.000000 persyn-0.0.9/src/chat/stdio/elaborate.py
+-rwxrwxr-x   0 rob       (1000) rob       (1000)     3416 2023-05-22 01:51:08.000000 persyn-0.0.9/src/chat/stdio/import_text.py
+-rw-rw-r--   0 rob       (1000) rob       (1000)     1603 2023-05-22 01:51:08.000000 persyn-0.0.9/src/chat/stdio/inject_idea.py
+-rw-rw-r--   0 rob       (1000) rob       (1000)     1647 2023-05-22 01:51:08.000000 persyn-0.0.9/src/chat/stdio/opine.py
+-rw-rw-r--   0 rob       (1000) rob       (1000)     1606 2023-05-22 01:51:08.000000 persyn-0.0.9/src/chat/stdio/read_rss.py
+-rw-rw-r--   0 rob       (1000) rob       (1000)     1760 2023-05-22 01:51:08.000000 persyn-0.0.9/src/chat/stdio/read_url.py
+-rw-rw-r--   0 rob       (1000) rob       (1000)     1491 2023-05-22 01:51:08.000000 persyn-0.0.9/src/chat/stdio/send_chat.py
+-rw-rw-r--   0 rob       (1000) rob       (1000)     1671 2023-05-22 01:51:08.000000 persyn-0.0.9/src/chat/stdio/summarize.py
+drwxrwxr-x   0 rob       (1000) rob       (1000)        0 2023-05-22 01:56:22.274214 persyn-0.0.9/src/dreams/
+-rw-rw-r--   0 rob       (1000) rob       (1000)        0 2023-05-22 01:51:08.000000 persyn-0.0.9/src/dreams/__init__.py
+drwxrwxr-x   0 rob       (1000) rob       (1000)        0 2023-05-22 01:56:22.274214 persyn-0.0.9/src/dreams/clip_interrogator/
+-rw-rw-r--   0 rob       (1000) rob       (1000)        0 2023-05-22 01:51:08.000000 persyn-0.0.9/src/dreams/clip_interrogator/__init__.py
+-rw-rw-r--   0 rob       (1000) rob       (1000)    10568 2023-05-22 01:51:08.000000 persyn-0.0.9/src/dreams/clip_interrogator/interrogator.py
+-rw-rw-r--   0 rob       (1000) rob       (1000)     5864 2023-05-22 01:51:08.000000 persyn-0.0.9/src/dreams/dreams.py
+drwxrwxr-x   0 rob       (1000) rob       (1000)        0 2023-05-22 01:56:22.274214 persyn-0.0.9/src/dreams/prompt-parrot/
+-rw-rw-r--   0 rob       (1000) rob       (1000)     2939 2023-05-22 01:51:08.000000 persyn-0.0.9/src/dreams/prompt-parrot/prompt-parrot.py
+-rw-rw-r--   0 rob       (1000) rob       (1000)     6366 2023-05-22 01:51:08.000000 persyn-0.0.9/src/dreams/stable_diffusion.py
+drwxrwxr-x   0 rob       (1000) rob       (1000)        0 2023-05-22 01:56:22.274214 persyn-0.0.9/src/interaction/
+-rw-rw-r--   0 rob       (1000) rob       (1000)        0 2023-05-22 01:51:08.000000 persyn-0.0.9/src/interaction/__init__.py
+-rw-rw-r--   0 rob       (1000) rob       (1000)     1008 2023-05-22 01:51:08.000000 persyn-0.0.9/src/interaction/chrono.py
+-rw-rw-r--   0 rob       (1000) rob       (1000)    17184 2023-05-22 01:51:08.000000 persyn-0.0.9/src/interaction/cns.py
+-rw-rw-r--   0 rob       (1000) rob       (1000)     2855 2023-05-22 01:51:08.000000 persyn-0.0.9/src/interaction/completion.py
+-rw-rw-r--   0 rob       (1000) rob       (1000)    29689 2023-05-22 01:51:08.000000 persyn-0.0.9/src/interaction/feels.py
+-rw-rw-r--   0 rob       (1000) rob       (1000)    25880 2023-05-22 01:51:08.000000 persyn-0.0.9/src/interaction/gpt.py
+-rwxrwxr-x   0 rob       (1000) rob       (1000)       60 2023-05-22 01:51:08.000000 persyn-0.0.9/src/interaction/install.py
+-rw-rw-r--   0 rob       (1000) rob       (1000)    22519 2023-05-22 01:51:08.000000 persyn-0.0.9/src/interaction/interact.py
+-rwxrwxr-x   0 rob       (1000) rob       (1000)    12601 2023-05-22 01:51:08.000000 persyn-0.0.9/src/interaction/interact_server.py
+-rw-rw-r--   0 rob       (1000) rob       (1000)    37477 2023-05-22 01:51:08.000000 persyn-0.0.9/src/interaction/memory.py
+-rw-rw-r--   0 rob       (1000) rob       (1000)     2176 2023-05-22 01:51:08.000000 persyn-0.0.9/src/interaction/messages.py
+-rw-rw-r--   0 rob       (1000) rob       (1000)    13814 2023-05-22 01:51:08.000000 persyn-0.0.9/src/interaction/nlp_cloud.py
+-rw-rw-r--   0 rob       (1000) rob       (1000)    13396 2023-05-22 01:51:08.000000 persyn-0.0.9/src/interaction/relationships.py
+-rw-rw-r--   0 rob       (1000) rob       (1000)     2725 2023-05-22 01:51:08.000000 persyn-0.0.9/src/interaction/reminders.py
+-rw-rw-r--   0 rob       (1000) rob       (1000)     1248 2023-05-22 01:51:08.000000 persyn-0.0.9/src/interaction/voice.py
+-rwxrwxr-x   0 rob       (1000) rob       (1000)      863 2023-05-22 01:51:08.000000 persyn-0.0.9/src/kill_bot.py
+-rwxrwxr-x   0 rob       (1000) rob       (1000)     4548 2023-05-22 01:51:08.000000 persyn-0.0.9/src/launch_bot.py
+drwxrwxr-x   0 rob       (1000) rob       (1000)        0 2023-05-22 01:56:22.270214 persyn-0.0.9/src/persyn/
+drwxrwxr-x   0 rob       (1000) rob       (1000)        0 2023-05-22 01:56:22.270214 persyn-0.0.9/src/persyn/dreams/
+drwxrwxr-x   0 rob       (1000) rob       (1000)        0 2023-05-22 01:56:22.270214 persyn-0.0.9/src/persyn/dreams/env/
+drwxrwxr-x   0 rob       (1000) rob       (1000)        0 2023-05-22 01:56:22.278214 persyn-0.0.9/src/persyn/dreams/env/bin/
+-rw-rw-r--   0 rob       (1000) rob       (1000)     1199 2023-01-15 02:17:08.000000 persyn-0.0.9/src/persyn/dreams/env/bin/activate_this.py
+-rwxrwxr-x   0 rob       (1000) rob       (1000)     1721 2023-01-15 03:32:50.000000 persyn-0.0.9/src/persyn/dreams/env/bin/jp.py
+drwxrwxr-x   0 rob       (1000) rob       (1000)        0 2023-05-22 01:56:22.278214 persyn-0.0.9/src/persyn/dreams/stylegan2/
+-rwxr-xr-x   0 rob       (1000) rob       (1000)    30282 2022-02-21 19:19:05.000000 persyn-0.0.9/src/persyn/dreams/stylegan2/dataset_tool.py
+drwxrwxr-x   0 rob       (1000) rob       (1000)        0 2023-05-22 01:56:22.278214 persyn-0.0.9/src/persyn/dreams/stylegan2/dnnlib/
+-rwxr-xr-x   0 rob       (1000) rob       (1000)      774 2022-02-21 19:19:28.000000 persyn-0.0.9/src/persyn/dreams/stylegan2/dnnlib/__init__.py
+drwxrwxr-x   0 rob       (1000) rob       (1000)        0 2023-05-22 01:56:22.278214 persyn-0.0.9/src/persyn/dreams/stylegan2/dnnlib/submission/
+-rwxr-xr-x   0 rob       (1000) rob       (1000)      274 2022-02-21 19:19:28.000000 persyn-0.0.9/src/persyn/dreams/stylegan2/dnnlib/submission/__init__.py
+drwxrwxr-x   0 rob       (1000) rob       (1000)        0 2023-05-22 01:56:22.278214 persyn-0.0.9/src/persyn/dreams/stylegan2/dnnlib/submission/internal/
+-rwxr-xr-x   0 rob       (1000) rob       (1000)      247 2022-02-21 19:19:28.000000 persyn-0.0.9/src/persyn/dreams/stylegan2/dnnlib/submission/internal/__init__.py
+-rwxr-xr-x   0 rob       (1000) rob       (1000)      769 2022-02-21 19:19:28.000000 persyn-0.0.9/src/persyn/dreams/stylegan2/dnnlib/submission/internal/local.py
+-rwxr-xr-x   0 rob       (1000) rob       (1000)     4245 2022-02-21 19:19:28.000000 persyn-0.0.9/src/persyn/dreams/stylegan2/dnnlib/submission/run_context.py
+-rwxr-xr-x   0 rob       (1000) rob       (1000)    13502 2022-02-21 19:19:28.000000 persyn-0.0.9/src/persyn/dreams/stylegan2/dnnlib/submission/submit.py
+drwxrwxr-x   0 rob       (1000) rob       (1000)        0 2023-05-22 01:56:22.278214 persyn-0.0.9/src/persyn/dreams/stylegan2/dnnlib/tflib/
+-rwxr-xr-x   0 rob       (1000) rob       (1000)      467 2022-02-21 19:19:28.000000 persyn-0.0.9/src/persyn/dreams/stylegan2/dnnlib/tflib/__init__.py
+-rwxr-xr-x   0 rob       (1000) rob       (1000)     8038 2022-02-21 19:19:28.000000 persyn-0.0.9/src/persyn/dreams/stylegan2/dnnlib/tflib/autosummary.py
+-rwxr-xr-x   0 rob       (1000) rob       (1000)     7223 2022-02-21 19:19:28.000000 persyn-0.0.9/src/persyn/dreams/stylegan2/dnnlib/tflib/custom_ops.py
+-rwxr-xr-x   0 rob       (1000) rob       (1000)    29982 2022-02-21 19:19:28.000000 persyn-0.0.9/src/persyn/dreams/stylegan2/dnnlib/tflib/network.py
+drwxrwxr-x   0 rob       (1000) rob       (1000)        0 2023-05-22 01:56:22.282214 persyn-0.0.9/src/persyn/dreams/stylegan2/dnnlib/tflib/ops/
+-rwxr-xr-x   0 rob       (1000) rob       (1000)      235 2022-02-21 19:19:28.000000 persyn-0.0.9/src/persyn/dreams/stylegan2/dnnlib/tflib/ops/__init__.py
+-rwxr-xr-x   0 rob       (1000) rob       (1000)     8539 2022-02-21 19:19:28.000000 persyn-0.0.9/src/persyn/dreams/stylegan2/dnnlib/tflib/ops/fused_bias_act.py
+-rwxr-xr-x   0 rob       (1000) rob       (1000)    16588 2022-02-21 19:19:28.000000 persyn-0.0.9/src/persyn/dreams/stylegan2/dnnlib/tflib/ops/upfirdn_2d.py
+-rwxr-xr-x   0 rob       (1000) rob       (1000)    20298 2022-02-21 19:19:28.000000 persyn-0.0.9/src/persyn/dreams/stylegan2/dnnlib/tflib/optimizer.py
+-rwxr-xr-x   0 rob       (1000) rob       (1000)     9675 2022-02-21 19:19:28.000000 persyn-0.0.9/src/persyn/dreams/stylegan2/dnnlib/tflib/tfutil.py
+-rwxr-xr-x   0 rob       (1000) rob       (1000)    13916 2022-02-21 19:19:28.000000 persyn-0.0.9/src/persyn/dreams/stylegan2/dnnlib/util.py
+drwxrwxr-x   0 rob       (1000) rob       (1000)        0 2023-05-22 01:56:22.270214 persyn-0.0.9/src/persyn/dreams/stylegan2/env/
+drwxrwxr-x   0 rob       (1000) rob       (1000)        0 2023-05-22 01:56:22.282214 persyn-0.0.9/src/persyn/dreams/stylegan2/env/bin/
+-rw-r--r--   0 rob       (1000) rob       (1000)     1137 2022-02-21 19:19:51.000000 persyn-0.0.9/src/persyn/dreams/stylegan2/env/bin/activate_this.py
+-rwxr-xr-x   0 rob       (1000) rob       (1000)     2722 2022-02-21 19:19:05.000000 persyn-0.0.9/src/persyn/dreams/stylegan2/make_a_face.py
+drwxrwxr-x   0 rob       (1000) rob       (1000)        0 2023-05-22 01:56:22.282214 persyn-0.0.9/src/persyn/dreams/stylegan2/metrics/
+-rwxr-xr-x   0 rob       (1000) rob       (1000)      235 2022-02-21 19:19:28.000000 persyn-0.0.9/src/persyn/dreams/stylegan2/metrics/__init__.py
+-rwxr-xr-x   0 rob       (1000) rob       (1000)     3330 2022-02-21 19:19:28.000000 persyn-0.0.9/src/persyn/dreams/stylegan2/metrics/frechet_inception_distance.py
+-rwxr-xr-x   0 rob       (1000) rob       (1000)     2587 2022-02-21 19:19:28.000000 persyn-0.0.9/src/persyn/dreams/stylegan2/metrics/inception_score.py
+-rwxr-xr-x   0 rob       (1000) rob       (1000)     9978 2022-02-21 19:19:28.000000 persyn-0.0.9/src/persyn/dreams/stylegan2/metrics/linear_separability.py
+-rwxr-xr-x   0 rob       (1000) rob       (1000)     7055 2022-02-21 19:19:28.000000 persyn-0.0.9/src/persyn/dreams/stylegan2/metrics/metric_base.py
+-rwxr-xr-x   0 rob       (1000) rob       (1000)     2311 2022-02-21 19:19:28.000000 persyn-0.0.9/src/persyn/dreams/stylegan2/metrics/metric_defaults.py
+-rwxr-xr-x   0 rob       (1000) rob       (1000)     5605 2022-02-21 19:19:28.000000 persyn-0.0.9/src/persyn/dreams/stylegan2/metrics/perceptual_path_length.py
+-rwxr-xr-x   0 rob       (1000) rob       (1000)    11437 2022-02-21 19:19:28.000000 persyn-0.0.9/src/persyn/dreams/stylegan2/metrics/precision_recall.py
+-rwxr-xr-x   0 rob       (1000) rob       (1000)     7521 2022-02-21 19:19:05.000000 persyn-0.0.9/src/persyn/dreams/stylegan2/pretrained_networks.py
+-rwxr-xr-x   0 rob       (1000) rob       (1000)     8975 2022-02-21 19:19:05.000000 persyn-0.0.9/src/persyn/dreams/stylegan2/projector.py
+-rwxr-xr-x   0 rob       (1000) rob       (1000)     8245 2022-02-21 19:19:05.000000 persyn-0.0.9/src/persyn/dreams/stylegan2/run_generator.py
+-rwxr-xr-x   0 rob       (1000) rob       (1000)     3447 2022-02-21 19:19:05.000000 persyn-0.0.9/src/persyn/dreams/stylegan2/run_metrics.py
+-rwxr-xr-x   0 rob       (1000) rob       (1000)     6963 2022-02-21 19:19:05.000000 persyn-0.0.9/src/persyn/dreams/stylegan2/run_projector.py
+-rwxr-xr-x   0 rob       (1000) rob       (1000)     8473 2022-02-21 19:19:05.000000 persyn-0.0.9/src/persyn/dreams/stylegan2/run_training.py
+drwxrwxr-x   0 rob       (1000) rob       (1000)        0 2023-05-22 01:56:22.282214 persyn-0.0.9/src/persyn/dreams/stylegan2/training/
+-rwxr-xr-x   0 rob       (1000) rob       (1000)      235 2022-02-21 19:19:28.000000 persyn-0.0.9/src/persyn/dreams/stylegan2/training/__init__.py
+-rwxr-xr-x   0 rob       (1000) rob       (1000)     9881 2022-02-21 19:19:28.000000 persyn-0.0.9/src/persyn/dreams/stylegan2/training/dataset.py
+-rwxr-xr-x   0 rob       (1000) rob       (1000)    10731 2022-02-21 19:19:28.000000 persyn-0.0.9/src/persyn/dreams/stylegan2/training/loss.py
+-rwxr-xr-x   0 rob       (1000) rob       (1000)     5706 2022-02-21 19:19:28.000000 persyn-0.0.9/src/persyn/dreams/stylegan2/training/misc.py
+-rwxr-xr-x   0 rob       (1000) rob       (1000)    33273 2022-02-21 19:19:28.000000 persyn-0.0.9/src/persyn/dreams/stylegan2/training/networks_stylegan.py
+-rwxr-xr-x   0 rob       (1000) rob       (1000)    38074 2022-02-21 19:19:28.000000 persyn-0.0.9/src/persyn/dreams/stylegan2/training/networks_stylegan2.py
+-rwxr-xr-x   0 rob       (1000) rob       (1000)    19892 2022-02-21 19:19:28.000000 persyn-0.0.9/src/persyn/dreams/stylegan2/training/training_loop.py
+drwxrwxr-x   0 rob       (1000) rob       (1000)        0 2023-05-22 01:56:22.270214 persyn-0.0.9/src/persyn/interaction/
+drwxrwxr-x   0 rob       (1000) rob       (1000)        0 2023-05-22 01:56:22.270214 persyn-0.0.9/src/persyn/interaction/notebooks/
+drwxrwxr-x   0 rob       (1000) rob       (1000)        0 2023-05-22 01:56:22.270214 persyn-0.0.9/src/persyn/interaction/notebooks/env/
+drwxrwxr-x   0 rob       (1000) rob       (1000)        0 2023-05-22 01:56:22.282214 persyn-0.0.9/src/persyn/interaction/notebooks/env/bin/
+-rw-rw-r--   0 rob       (1000) rob       (1000)     1199 2022-10-23 00:31:31.000000 persyn-0.0.9/src/persyn/interaction/notebooks/env/bin/activate_this.py
+-rwxrwxr-x   0 rob       (1000) rob       (1000)     1732 2022-12-04 20:53:32.000000 persyn-0.0.9/src/persyn/interaction/notebooks/env/bin/jp.py
+drwxrwxr-x   0 rob       (1000) rob       (1000)        0 2023-05-22 01:56:22.278214 persyn-0.0.9/src/persyn.egg-info/
+-rw-rw-r--   0 rob       (1000) rob       (1000)     3059 2023-05-22 01:56:22.000000 persyn-0.0.9/src/persyn.egg-info/PKG-INFO
+-rw-rw-r--   0 rob       (1000) rob       (1000)     3730 2023-05-22 01:56:22.000000 persyn-0.0.9/src/persyn.egg-info/SOURCES.txt
+-rw-rw-r--   0 rob       (1000) rob       (1000)        1 2023-05-22 01:56:22.000000 persyn-0.0.9/src/persyn.egg-info/dependency_links.txt
+-rw-rw-r--   0 rob       (1000) rob       (1000)      653 2023-05-22 01:56:22.000000 persyn-0.0.9/src/persyn.egg-info/entry_points.txt
+-rw-rw-r--   0 rob       (1000) rob       (1000)      532 2023-05-22 01:56:22.000000 persyn-0.0.9/src/persyn.egg-info/requires.txt
+-rw-rw-r--   0 rob       (1000) rob       (1000)       66 2023-05-22 01:56:22.000000 persyn-0.0.9/src/persyn.egg-info/top_level.txt
+drwxrwxr-x   0 rob       (1000) rob       (1000)        0 2023-05-22 01:56:22.282214 persyn-0.0.9/src/utils/
+-rw-rw-r--   0 rob       (1000) rob       (1000)        0 2023-05-22 01:51:08.000000 persyn-0.0.9/src/utils/__init__.py
+-rw-rw-r--   0 rob       (1000) rob       (1000)     5169 2023-05-22 01:51:08.000000 persyn-0.0.9/src/utils/art.py
+-rw-rw-r--   0 rob       (1000) rob       (1000)     1623 2023-05-22 01:51:08.000000 persyn-0.0.9/src/utils/color_logging.py
+-rw-rw-r--   0 rob       (1000) rob       (1000)     5309 2023-05-22 01:51:08.000000 persyn-0.0.9/src/utils/config.py
```

### Comparing `persyn-0.0.4/LICENSE.txt` & `persyn-0.0.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `persyn-0.0.4/PKG-INFO` & `persyn-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: persyn
-Version: 0.0.4
+Version: 0.0.9
 Summary: Personality Syndrome. Persyn for short.
 Author-email: Rob Flickenger <rob@hackerfriendly.com>
 Project-URL: Homepage, https://persyn.io
 Project-URL: Bug Tracker, https://github.com/hackerfriendly/persyn/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `persyn-0.0.4/README.md` & `persyn-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `persyn-0.0.4/pyproject.toml` & `persyn-0.0.9/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "persyn"
-version = "0.0.4"
+version = "0.0.9"
 authors = [
   { name="Rob Flickenger", email="rob@hackerfriendly.com" },
 ]
 description = "Personality Syndrome. Persyn for short."
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
@@ -41,15 +41,18 @@
   "scipy==1.9.0",
   "shortuuid",
   "slack_bolt",
   "spacy",
   "spacytextblob",
   "uvicorn",
   "wikipedia",
-  "asyncio"
+  "asyncio",
+  "tiktoken",
+  "neomodel",
+  # "autobus @ git+https://github.com/hackerfriendly/autobus"
 ]
 
 [project.scripts]
 launch_bot = "launch_bot:main"
 kill_bot = "kill_bot:main"
 interact = "interaction.interact_server:launch"
 slack = "chat.slack.bot:main"
```

### Comparing `persyn-0.0.4/src/chat/common.py` & `persyn-0.0.9/src/chat/common.py`

 * *Files identical despite different names*

### Comparing `persyn-0.0.4/src/chat/discord/bot.py` & `persyn-0.0.9/src/chat/discord/bot.py`

 * *Files identical despite different names*

### Comparing `persyn-0.0.4/src/chat/mastodon/bot.py` & `persyn-0.0.9/src/chat/mastodon/bot.py`

 * *Files identical despite different names*

### Comparing `persyn-0.0.4/src/chat/mastodon/login.py` & `persyn-0.0.9/src/chat/mastodon/login.py`

 * *Files identical despite different names*

### Comparing `persyn-0.0.4/src/chat/mastodon/masto-login.py` & `persyn-0.0.9/src/chat/mastodon/masto-login.py`

 * *Files identical despite different names*

### Comparing `persyn-0.0.4/src/chat/simple.py` & `persyn-0.0.9/src/chat/simple.py`

 * *Files identical despite different names*

### Comparing `persyn-0.0.4/src/chat/slack/bot.py` & `persyn-0.0.9/src/chat/slack/bot.py`

 * *Files identical despite different names*

### Comparing `persyn-0.0.4/src/chat/stdio/add_goal.py` & `persyn-0.0.9/src/chat/stdio/add_goal.py`

 * *Files identical despite different names*

### Comparing `persyn-0.0.4/src/chat/stdio/elaborate.py` & `persyn-0.0.9/src/chat/stdio/elaborate.py`

 * *Files identical despite different names*

### Comparing `persyn-0.0.4/src/chat/stdio/import_text.py` & `persyn-0.0.9/src/chat/stdio/import_text.py`

 * *Files identical despite different names*

### Comparing `persyn-0.0.4/src/chat/stdio/inject_idea.py` & `persyn-0.0.9/src/chat/stdio/inject_idea.py`

 * *Files identical despite different names*

### Comparing `persyn-0.0.4/src/chat/stdio/opine.py` & `persyn-0.0.9/src/chat/stdio/opine.py`

 * *Files identical despite different names*

### Comparing `persyn-0.0.4/src/chat/stdio/read_rss.py` & `persyn-0.0.9/src/chat/stdio/read_rss.py`

 * *Files identical despite different names*

### Comparing `persyn-0.0.4/src/chat/stdio/read_url.py` & `persyn-0.0.9/src/chat/stdio/read_url.py`

 * *Files identical despite different names*

### Comparing `persyn-0.0.4/src/chat/stdio/send_chat.py` & `persyn-0.0.9/src/chat/stdio/send_chat.py`

 * *Files identical despite different names*

### Comparing `persyn-0.0.4/src/chat/stdio/summarize.py` & `persyn-0.0.9/src/chat/stdio/summarize.py`

 * *Files identical despite different names*

### Comparing `persyn-0.0.4/src/dreams/clip_interrogator/interrogator.py` & `persyn-0.0.9/src/dreams/clip_interrogator/interrogator.py`

 * *Files identical despite different names*

### Comparing `persyn-0.0.4/src/dreams/dreams.py` & `persyn-0.0.9/src/dreams/dreams.py`

 * *Files identical despite different names*

### Comparing `persyn-0.0.4/src/dreams/env/bin/activate_this.py` & `persyn-0.0.9/src/persyn/dreams/env/bin/activate_this.py`

 * *Files identical despite different names*

### Comparing `persyn-0.0.4/src/dreams/env/bin/jp.py` & `persyn-0.0.9/src/persyn/dreams/env/bin/jp.py`

 * *Files identical despite different names*

### Comparing `persyn-0.0.4/src/dreams/prompt-parrot/prompt-parrot.py` & `persyn-0.0.9/src/dreams/prompt-parrot/prompt-parrot.py`

 * *Files identical despite different names*

### Comparing `persyn-0.0.4/src/dreams/stable_diffusion.py` & `persyn-0.0.9/src/dreams/stable_diffusion.py`

 * *Files identical despite different names*

### Comparing `persyn-0.0.4/src/dreams/stylegan2/dataset_tool.py` & `persyn-0.0.9/src/persyn/dreams/stylegan2/dataset_tool.py`

 * *Files identical despite different names*

### Comparing `persyn-0.0.4/src/dreams/stylegan2/dnnlib/__init__.py` & `persyn-0.0.9/src/persyn/dreams/stylegan2/dnnlib/__init__.py`

 * *Files identical despite different names*

### Comparing `persyn-0.0.4/src/dreams/stylegan2/dnnlib/submission/internal/local.py` & `persyn-0.0.9/src/persyn/dreams/stylegan2/dnnlib/submission/internal/local.py`

 * *Files identical despite different names*

### Comparing `persyn-0.0.4/src/dreams/stylegan2/dnnlib/submission/run_context.py` & `persyn-0.0.9/src/persyn/dreams/stylegan2/dnnlib/submission/run_context.py`

 * *Files identical despite different names*

### Comparing `persyn-0.0.4/src/dreams/stylegan2/dnnlib/submission/submit.py` & `persyn-0.0.9/src/persyn/dreams/stylegan2/dnnlib/submission/submit.py`

 * *Files identical despite different names*

### Comparing `persyn-0.0.4/src/dreams/stylegan2/dnnlib/tflib/autosummary.py` & `persyn-0.0.9/src/persyn/dreams/stylegan2/dnnlib/tflib/autosummary.py`

 * *Files identical despite different names*

### Comparing `persyn-0.0.4/src/dreams/stylegan2/dnnlib/tflib/custom_ops.py` & `persyn-0.0.9/src/persyn/dreams/stylegan2/dnnlib/tflib/custom_ops.py`

 * *Files identical despite different names*

### Comparing `persyn-0.0.4/src/dreams/stylegan2/dnnlib/tflib/network.py` & `persyn-0.0.9/src/persyn/dreams/stylegan2/dnnlib/tflib/network.py`

 * *Files identical despite different names*

### Comparing `persyn-0.0.4/src/dreams/stylegan2/dnnlib/tflib/ops/fused_bias_act.py` & `persyn-0.0.9/src/persyn/dreams/stylegan2/dnnlib/tflib/ops/fused_bias_act.py`

 * *Files identical despite different names*

### Comparing `persyn-0.0.4/src/dreams/stylegan2/dnnlib/tflib/ops/upfirdn_2d.py` & `persyn-0.0.9/src/persyn/dreams/stylegan2/dnnlib/tflib/ops/upfirdn_2d.py`

 * *Files identical despite different names*

### Comparing `persyn-0.0.4/src/dreams/stylegan2/dnnlib/tflib/optimizer.py` & `persyn-0.0.9/src/persyn/dreams/stylegan2/dnnlib/tflib/optimizer.py`

 * *Files identical despite different names*

### Comparing `persyn-0.0.4/src/dreams/stylegan2/dnnlib/tflib/tfutil.py` & `persyn-0.0.9/src/persyn/dreams/stylegan2/dnnlib/tflib/tfutil.py`

 * *Files identical despite different names*

### Comparing `persyn-0.0.4/src/dreams/stylegan2/dnnlib/util.py` & `persyn-0.0.9/src/persyn/dreams/stylegan2/dnnlib/util.py`

 * *Files identical despite different names*

### Comparing `persyn-0.0.4/src/dreams/stylegan2/env/bin/activate_this.py` & `persyn-0.0.9/src/persyn/dreams/stylegan2/env/bin/activate_this.py`

 * *Files identical despite different names*

### Comparing `persyn-0.0.4/src/dreams/stylegan2/make_a_face.py` & `persyn-0.0.9/src/persyn/dreams/stylegan2/make_a_face.py`

 * *Files identical despite different names*

### Comparing `persyn-0.0.4/src/dreams/stylegan2/metrics/frechet_inception_distance.py` & `persyn-0.0.9/src/persyn/dreams/stylegan2/metrics/frechet_inception_distance.py`

 * *Files identical despite different names*

### Comparing `persyn-0.0.4/src/dreams/stylegan2/metrics/inception_score.py` & `persyn-0.0.9/src/persyn/dreams/stylegan2/metrics/inception_score.py`

 * *Files identical despite different names*

### Comparing `persyn-0.0.4/src/dreams/stylegan2/metrics/linear_separability.py` & `persyn-0.0.9/src/persyn/dreams/stylegan2/metrics/linear_separability.py`

 * *Files identical despite different names*

### Comparing `persyn-0.0.4/src/dreams/stylegan2/metrics/metric_base.py` & `persyn-0.0.9/src/persyn/dreams/stylegan2/metrics/metric_base.py`

 * *Files identical despite different names*

### Comparing `persyn-0.0.4/src/dreams/stylegan2/metrics/metric_defaults.py` & `persyn-0.0.9/src/persyn/dreams/stylegan2/metrics/metric_defaults.py`

 * *Files identical despite different names*

### Comparing `persyn-0.0.4/src/dreams/stylegan2/metrics/perceptual_path_length.py` & `persyn-0.0.9/src/persyn/dreams/stylegan2/metrics/perceptual_path_length.py`

 * *Files identical despite different names*

### Comparing `persyn-0.0.4/src/dreams/stylegan2/metrics/precision_recall.py` & `persyn-0.0.9/src/persyn/dreams/stylegan2/metrics/precision_recall.py`

 * *Files identical despite different names*

### Comparing `persyn-0.0.4/src/dreams/stylegan2/pretrained_networks.py` & `persyn-0.0.9/src/persyn/dreams/stylegan2/pretrained_networks.py`

 * *Files identical despite different names*

### Comparing `persyn-0.0.4/src/dreams/stylegan2/projector.py` & `persyn-0.0.9/src/persyn/dreams/stylegan2/projector.py`

 * *Files identical despite different names*

### Comparing `persyn-0.0.4/src/dreams/stylegan2/run_generator.py` & `persyn-0.0.9/src/persyn/dreams/stylegan2/run_generator.py`

 * *Files identical despite different names*

### Comparing `persyn-0.0.4/src/dreams/stylegan2/run_metrics.py` & `persyn-0.0.9/src/persyn/dreams/stylegan2/run_metrics.py`

 * *Files identical despite different names*

### Comparing `persyn-0.0.4/src/dreams/stylegan2/run_projector.py` & `persyn-0.0.9/src/persyn/dreams/stylegan2/run_projector.py`

 * *Files identical despite different names*

### Comparing `persyn-0.0.4/src/dreams/stylegan2/run_training.py` & `persyn-0.0.9/src/persyn/dreams/stylegan2/run_training.py`

 * *Files identical despite different names*

### Comparing `persyn-0.0.4/src/dreams/stylegan2/training/dataset.py` & `persyn-0.0.9/src/persyn/dreams/stylegan2/training/dataset.py`

 * *Files identical despite different names*

### Comparing `persyn-0.0.4/src/dreams/stylegan2/training/loss.py` & `persyn-0.0.9/src/persyn/dreams/stylegan2/training/loss.py`

 * *Files identical despite different names*

### Comparing `persyn-0.0.4/src/dreams/stylegan2/training/misc.py` & `persyn-0.0.9/src/persyn/dreams/stylegan2/training/misc.py`

 * *Files identical despite different names*

### Comparing `persyn-0.0.4/src/dreams/stylegan2/training/networks_stylegan.py` & `persyn-0.0.9/src/persyn/dreams/stylegan2/training/networks_stylegan.py`

 * *Files identical despite different names*

### Comparing `persyn-0.0.4/src/dreams/stylegan2/training/networks_stylegan2.py` & `persyn-0.0.9/src/persyn/dreams/stylegan2/training/networks_stylegan2.py`

 * *Files identical despite different names*

### Comparing `persyn-0.0.4/src/dreams/stylegan2/training/training_loop.py` & `persyn-0.0.9/src/persyn/dreams/stylegan2/training/training_loop.py`

 * *Files identical despite different names*

### Comparing `persyn-0.0.4/src/interaction/chrono.py` & `persyn-0.0.9/src/interaction/chrono.py`

 * *Files identical despite different names*

### Comparing `persyn-0.0.4/src/interaction/cns.py` & `persyn-0.0.9/src/interaction/cns.py`

 * *Files identical despite different names*

### Comparing `persyn-0.0.4/src/interaction/completion.py` & `persyn-0.0.9/src/interaction/completion.py`

 * *Files identical despite different names*

### Comparing `persyn-0.0.4/src/interaction/feels.py` & `persyn-0.0.9/src/interaction/feels.py`

 * *Files identical despite different names*

### Comparing `persyn-0.0.4/src/interaction/gpt.py` & `persyn-0.0.9/src/interaction/gpt.py`

 * *Files identical despite different names*

### Comparing `persyn-0.0.4/src/interaction/interact.py` & `persyn-0.0.9/src/interaction/interact.py`

 * *Files identical despite different names*

### Comparing `persyn-0.0.4/src/interaction/interact_server.py` & `persyn-0.0.9/src/interaction/interact_server.py`

 * *Files identical despite different names*

### Comparing `persyn-0.0.4/src/interaction/memory.py` & `persyn-0.0.9/src/interaction/memory.py`

 * *Files identical despite different names*

### Comparing `persyn-0.0.4/src/interaction/messages.py` & `persyn-0.0.9/src/interaction/messages.py`

 * *Files identical despite different names*

### Comparing `persyn-0.0.4/src/interaction/nlp_cloud.py` & `persyn-0.0.9/src/interaction/nlp_cloud.py`

 * *Files identical despite different names*

### Comparing `persyn-0.0.4/src/interaction/notebooks/env/bin/activate_this.py` & `persyn-0.0.9/src/persyn/interaction/notebooks/env/bin/activate_this.py`

 * *Files identical despite different names*

### Comparing `persyn-0.0.4/src/interaction/notebooks/env/bin/jp.py` & `persyn-0.0.9/src/persyn/interaction/notebooks/env/bin/jp.py`

 * *Files identical despite different names*

### Comparing `persyn-0.0.4/src/interaction/relationships.py` & `persyn-0.0.9/src/interaction/relationships.py`

 * *Files identical despite different names*

### Comparing `persyn-0.0.4/src/interaction/reminders.py` & `persyn-0.0.9/src/interaction/reminders.py`

 * *Files identical despite different names*

### Comparing `persyn-0.0.4/src/interaction/voice.py` & `persyn-0.0.9/src/interaction/voice.py`

 * *Files identical despite different names*

### Comparing `persyn-0.0.4/src/kill_bot.py` & `persyn-0.0.9/src/kill_bot.py`

 * *Files identical despite different names*

### Comparing `persyn-0.0.4/src/launch_bot.py` & `persyn-0.0.9/src/launch_bot.py`

 * *Files identical despite different names*

### Comparing `persyn-0.0.4/src/persyn.egg-info/PKG-INFO` & `persyn-0.0.9/src/persyn.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: persyn
-Version: 0.0.4
+Version: 0.0.9
 Summary: Personality Syndrome. Persyn for short.
 Author-email: Rob Flickenger <rob@hackerfriendly.com>
 Project-URL: Homepage, https://persyn.io
 Project-URL: Bug Tracker, https://github.com/hackerfriendly/persyn/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `persyn-0.0.4/src/persyn.egg-info/entry_points.txt` & `persyn-0.0.9/src/persyn.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `persyn-0.0.4/src/persyn.egg-info/requires.txt` & `persyn-0.0.9/src/persyn.egg-info/requires.txt`

 * *Files 22% similar despite different names*

```diff
@@ -23,14 +23,16 @@
 shortuuid
 slack_bolt
 spacy
 spacytextblob
 uvicorn
 wikipedia
 asyncio
+tiktoken
+neomodel
 
 [all]
 accelerate
 diffusers
 safetensors
 scipy
 timm
```

### Comparing `persyn-0.0.4/src/utils/art.py` & `persyn-0.0.9/src/utils/art.py`

 * *Files identical despite different names*

### Comparing `persyn-0.0.4/src/utils/color_logging.py` & `persyn-0.0.9/src/utils/color_logging.py`

 * *Files identical despite different names*

### Comparing `persyn-0.0.4/src/utils/config.py` & `persyn-0.0.9/src/utils/config.py`

 * *Files identical despite different names*

