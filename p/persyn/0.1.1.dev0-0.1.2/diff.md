# Comparing `tmp/persyn-0.1.1.dev0.tar.gz` & `tmp/persyn-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "persyn-0.1.1.dev0.tar", last modified: Mon May 22 03:00:45 2023, max compression
+gzip compressed data, was "persyn-0.1.2.tar", last modified: Mon May 22 03:10:08 2023, max compression
```

## Comparing `persyn-0.1.1.dev0.tar` & `persyn-0.1.2.tar`

### file list

```diff
@@ -1,127 +1,127 @@
-drwxrwxr-x   0 rob       (1000) rob       (1000)        0 2023-05-22 03:00:45.735715 persyn-0.1.1.dev0/
--rw-rw-r--   0 rob       (1000) rob       (1000)     1058 2023-01-09 01:22:11.000000 persyn-0.1.1.dev0/LICENSE.txt
--rw-rw-r--   0 rob       (1000) rob       (1000)     3526 2023-05-22 03:00:45.735715 persyn-0.1.1.dev0/PKG-INFO
--rw-rw-r--   0 rob       (1000) rob       (1000)     2944 2023-05-22 02:29:25.000000 persyn-0.1.1.dev0/README.md
--rw-rw-r--   0 rob       (1000) rob       (1000)     2389 2023-05-22 02:59:43.000000 persyn-0.1.1.dev0/pyproject.toml
--rw-rw-r--   0 rob       (1000) rob       (1000)       38 2023-05-22 03:00:45.735715 persyn-0.1.1.dev0/setup.cfg
-drwxrwxr-x   0 rob       (1000) rob       (1000)        0 2023-05-22 03:00:45.715716 persyn-0.1.1.dev0/src/
-drwxrwxr-x   0 rob       (1000) rob       (1000)        0 2023-05-22 03:00:45.719716 persyn-0.1.1.dev0/src/persyn/
--rw-rw-r--   0 rob       (1000) rob       (1000)        0 2023-05-22 02:29:25.000000 persyn-0.1.1.dev0/src/persyn/__init__.py
-drwxrwxr-x   0 rob       (1000) rob       (1000)        0 2023-05-22 03:00:45.723716 persyn-0.1.1.dev0/src/persyn/chat/
--rw-rw-r--   0 rob       (1000) rob       (1000)        0 2023-05-22 02:29:25.000000 persyn-0.1.1.dev0/src/persyn/chat/__init__.py
--rw-rw-r--   0 rob       (1000) rob       (1000)    14576 2023-05-22 02:29:25.000000 persyn-0.1.1.dev0/src/persyn/chat/common.py
-drwxrwxr-x   0 rob       (1000) rob       (1000)        0 2023-05-22 03:00:45.723716 persyn-0.1.1.dev0/src/persyn/chat/discord/
--rwxrwxr-x   0 rob       (1000) rob       (1000)     1740 2023-05-22 02:29:25.000000 persyn-0.1.1.dev0/src/persyn/chat/discord/basic.py
--rwxrwxr-x   0 rob       (1000) rob       (1000)    11065 2023-05-22 02:29:25.000000 persyn-0.1.1.dev0/src/persyn/chat/discord/bot.py
-drwxrwxr-x   0 rob       (1000) rob       (1000)        0 2023-05-22 03:00:45.723716 persyn-0.1.1.dev0/src/persyn/chat/mastodon/
--rwxrwxr-x   0 rob       (1000) rob       (1000)    11540 2023-05-22 02:29:25.000000 persyn-0.1.1.dev0/src/persyn/chat/mastodon/bot.py
--rw-rw-r--   0 rob       (1000) rob       (1000)     2015 2023-05-22 02:29:25.000000 persyn-0.1.1.dev0/src/persyn/chat/mastodon/login.py
--rwxrwxr-x   0 rob       (1000) rob       (1000)     1208 2023-05-22 02:29:25.000000 persyn-0.1.1.dev0/src/persyn/chat/mastodon/masto-login.py
--rwxrwxr-x   0 rob       (1000) rob       (1000)     1919 2023-05-22 02:29:25.000000 persyn-0.1.1.dev0/src/persyn/chat/mastodon/masto-stream.py
--rw-rw-r--   0 rob       (1000) rob       (1000)     3321 2023-05-22 02:29:25.000000 persyn-0.1.1.dev0/src/persyn/chat/simple.py
-drwxrwxr-x   0 rob       (1000) rob       (1000)        0 2023-05-22 03:00:45.723716 persyn-0.1.1.dev0/src/persyn/chat/slack/
--rwxrwxr-x   0 rob       (1000) rob       (1000)    18640 2023-05-22 02:29:25.000000 persyn-0.1.1.dev0/src/persyn/chat/slack/bot.py
-drwxrwxr-x   0 rob       (1000) rob       (1000)        0 2023-05-22 03:00:45.723716 persyn-0.1.1.dev0/src/persyn/chat/stdio/
--rw-rw-r--   0 rob       (1000) rob       (1000)     1502 2023-05-22 02:29:25.000000 persyn-0.1.1.dev0/src/persyn/chat/stdio/add_goal.py
--rw-rw-r--   0 rob       (1000) rob       (1000)     1450 2023-05-22 02:29:25.000000 persyn-0.1.1.dev0/src/persyn/chat/stdio/elaborate.py
--rwxrwxr-x   0 rob       (1000) rob       (1000)     3284 2023-05-22 02:29:25.000000 persyn-0.1.1.dev0/src/persyn/chat/stdio/import_text.py
--rw-rw-r--   0 rob       (1000) rob       (1000)     1617 2023-05-22 02:29:25.000000 persyn-0.1.1.dev0/src/persyn/chat/stdio/inject_idea.py
--rw-rw-r--   0 rob       (1000) rob       (1000)     1661 2023-05-22 02:29:25.000000 persyn-0.1.1.dev0/src/persyn/chat/stdio/opine.py
--rw-rw-r--   0 rob       (1000) rob       (1000)     1620 2023-05-22 02:29:25.000000 persyn-0.1.1.dev0/src/persyn/chat/stdio/read_rss.py
--rw-rw-r--   0 rob       (1000) rob       (1000)     1774 2023-05-22 02:29:25.000000 persyn-0.1.1.dev0/src/persyn/chat/stdio/read_url.py
--rw-rw-r--   0 rob       (1000) rob       (1000)     1505 2023-05-22 02:29:25.000000 persyn-0.1.1.dev0/src/persyn/chat/stdio/send_chat.py
--rw-rw-r--   0 rob       (1000) rob       (1000)     1685 2023-05-22 02:29:25.000000 persyn-0.1.1.dev0/src/persyn/chat/stdio/summarize.py
-drwxrwxr-x   0 rob       (1000) rob       (1000)        0 2023-05-22 03:00:45.723716 persyn-0.1.1.dev0/src/persyn/dreams/
--rw-rw-r--   0 rob       (1000) rob       (1000)        0 2023-05-22 02:29:25.000000 persyn-0.1.1.dev0/src/persyn/dreams/__init__.py
-drwxrwxr-x   0 rob       (1000) rob       (1000)        0 2023-05-22 03:00:45.723716 persyn-0.1.1.dev0/src/persyn/dreams/clip_interrogator/
--rw-rw-r--   0 rob       (1000) rob       (1000)        0 2023-05-22 02:29:25.000000 persyn-0.1.1.dev0/src/persyn/dreams/clip_interrogator/__init__.py
--rw-rw-r--   0 rob       (1000) rob       (1000)    10568 2023-05-22 02:29:25.000000 persyn-0.1.1.dev0/src/persyn/dreams/clip_interrogator/interrogator.py
--rw-rw-r--   0 rob       (1000) rob       (1000)     5892 2023-05-22 02:57:37.000000 persyn-0.1.1.dev0/src/persyn/dreams/dreams.py
-drwxrwxr-x   0 rob       (1000) rob       (1000)        0 2023-05-22 03:00:45.723716 persyn-0.1.1.dev0/src/persyn/dreams/prompt-parrot/
--rw-rw-r--   0 rob       (1000) rob       (1000)     2939 2023-05-22 02:29:25.000000 persyn-0.1.1.dev0/src/persyn/dreams/prompt-parrot/prompt-parrot.py
--rwxrwxr-x   0 rob       (1000) rob       (1000)      434 2023-05-22 02:29:25.000000 persyn-0.1.1.dev0/src/persyn/dreams/receive-sqs.py
--rwxrwxr-x   0 rob       (1000) rob       (1000)      898 2023-05-22 02:29:25.000000 persyn-0.1.1.dev0/src/persyn/dreams/send-sqs.py
--rw-rw-r--   0 rob       (1000) rob       (1000)     6387 2023-05-22 02:59:43.000000 persyn-0.1.1.dev0/src/persyn/dreams/stable_diffusion.py
-drwxrwxr-x   0 rob       (1000) rob       (1000)        0 2023-05-22 03:00:45.727716 persyn-0.1.1.dev0/src/persyn/dreams/stylegan2/
--rwxr-xr-x   0 rob       (1000) rob       (1000)    30282 2022-02-21 19:19:05.000000 persyn-0.1.1.dev0/src/persyn/dreams/stylegan2/dataset_tool.py
-drwxrwxr-x   0 rob       (1000) rob       (1000)        0 2023-05-22 03:00:45.727716 persyn-0.1.1.dev0/src/persyn/dreams/stylegan2/dnnlib/
--rwxr-xr-x   0 rob       (1000) rob       (1000)      774 2022-02-21 19:19:28.000000 persyn-0.1.1.dev0/src/persyn/dreams/stylegan2/dnnlib/__init__.py
-drwxrwxr-x   0 rob       (1000) rob       (1000)        0 2023-05-22 03:00:45.727716 persyn-0.1.1.dev0/src/persyn/dreams/stylegan2/dnnlib/submission/
--rwxr-xr-x   0 rob       (1000) rob       (1000)      274 2022-02-21 19:19:28.000000 persyn-0.1.1.dev0/src/persyn/dreams/stylegan2/dnnlib/submission/__init__.py
-drwxrwxr-x   0 rob       (1000) rob       (1000)        0 2023-05-22 03:00:45.727716 persyn-0.1.1.dev0/src/persyn/dreams/stylegan2/dnnlib/submission/internal/
--rwxr-xr-x   0 rob       (1000) rob       (1000)      247 2022-02-21 19:19:28.000000 persyn-0.1.1.dev0/src/persyn/dreams/stylegan2/dnnlib/submission/internal/__init__.py
--rwxr-xr-x   0 rob       (1000) rob       (1000)      769 2022-02-21 19:19:28.000000 persyn-0.1.1.dev0/src/persyn/dreams/stylegan2/dnnlib/submission/internal/local.py
--rwxr-xr-x   0 rob       (1000) rob       (1000)     4245 2022-02-21 19:19:28.000000 persyn-0.1.1.dev0/src/persyn/dreams/stylegan2/dnnlib/submission/run_context.py
--rwxr-xr-x   0 rob       (1000) rob       (1000)    13502 2022-02-21 19:19:28.000000 persyn-0.1.1.dev0/src/persyn/dreams/stylegan2/dnnlib/submission/submit.py
-drwxrwxr-x   0 rob       (1000) rob       (1000)        0 2023-05-22 03:00:45.727716 persyn-0.1.1.dev0/src/persyn/dreams/stylegan2/dnnlib/tflib/
--rwxr-xr-x   0 rob       (1000) rob       (1000)      467 2022-02-21 19:19:28.000000 persyn-0.1.1.dev0/src/persyn/dreams/stylegan2/dnnlib/tflib/__init__.py
--rwxr-xr-x   0 rob       (1000) rob       (1000)     8038 2022-02-21 19:19:28.000000 persyn-0.1.1.dev0/src/persyn/dreams/stylegan2/dnnlib/tflib/autosummary.py
--rwxr-xr-x   0 rob       (1000) rob       (1000)     7223 2022-02-21 19:19:28.000000 persyn-0.1.1.dev0/src/persyn/dreams/stylegan2/dnnlib/tflib/custom_ops.py
--rwxr-xr-x   0 rob       (1000) rob       (1000)    29982 2022-02-21 19:19:28.000000 persyn-0.1.1.dev0/src/persyn/dreams/stylegan2/dnnlib/tflib/network.py
-drwxrwxr-x   0 rob       (1000) rob       (1000)        0 2023-05-22 03:00:45.727716 persyn-0.1.1.dev0/src/persyn/dreams/stylegan2/dnnlib/tflib/ops/
--rwxr-xr-x   0 rob       (1000) rob       (1000)      235 2022-02-21 19:19:28.000000 persyn-0.1.1.dev0/src/persyn/dreams/stylegan2/dnnlib/tflib/ops/__init__.py
--rwxr-xr-x   0 rob       (1000) rob       (1000)     8539 2022-02-21 19:19:28.000000 persyn-0.1.1.dev0/src/persyn/dreams/stylegan2/dnnlib/tflib/ops/fused_bias_act.py
--rwxr-xr-x   0 rob       (1000) rob       (1000)    16588 2022-02-21 19:19:28.000000 persyn-0.1.1.dev0/src/persyn/dreams/stylegan2/dnnlib/tflib/ops/upfirdn_2d.py
--rwxr-xr-x   0 rob       (1000) rob       (1000)    20298 2022-02-21 19:19:28.000000 persyn-0.1.1.dev0/src/persyn/dreams/stylegan2/dnnlib/tflib/optimizer.py
--rwxr-xr-x   0 rob       (1000) rob       (1000)     9675 2022-02-21 19:19:28.000000 persyn-0.1.1.dev0/src/persyn/dreams/stylegan2/dnnlib/tflib/tfutil.py
--rwxr-xr-x   0 rob       (1000) rob       (1000)    13916 2022-02-21 19:19:28.000000 persyn-0.1.1.dev0/src/persyn/dreams/stylegan2/dnnlib/util.py
--rwxr-xr-x   0 rob       (1000) rob       (1000)     2722 2022-02-21 19:19:05.000000 persyn-0.1.1.dev0/src/persyn/dreams/stylegan2/make_a_face.py
-drwxrwxr-x   0 rob       (1000) rob       (1000)        0 2023-05-22 03:00:45.727716 persyn-0.1.1.dev0/src/persyn/dreams/stylegan2/metrics/
--rwxr-xr-x   0 rob       (1000) rob       (1000)      235 2022-02-21 19:19:28.000000 persyn-0.1.1.dev0/src/persyn/dreams/stylegan2/metrics/__init__.py
--rwxr-xr-x   0 rob       (1000) rob       (1000)     3330 2022-02-21 19:19:28.000000 persyn-0.1.1.dev0/src/persyn/dreams/stylegan2/metrics/frechet_inception_distance.py
--rwxr-xr-x   0 rob       (1000) rob       (1000)     2587 2022-02-21 19:19:28.000000 persyn-0.1.1.dev0/src/persyn/dreams/stylegan2/metrics/inception_score.py
--rwxr-xr-x   0 rob       (1000) rob       (1000)     9978 2022-02-21 19:19:28.000000 persyn-0.1.1.dev0/src/persyn/dreams/stylegan2/metrics/linear_separability.py
--rwxr-xr-x   0 rob       (1000) rob       (1000)     7055 2022-02-21 19:19:28.000000 persyn-0.1.1.dev0/src/persyn/dreams/stylegan2/metrics/metric_base.py
--rwxr-xr-x   0 rob       (1000) rob       (1000)     2311 2022-02-21 19:19:28.000000 persyn-0.1.1.dev0/src/persyn/dreams/stylegan2/metrics/metric_defaults.py
--rwxr-xr-x   0 rob       (1000) rob       (1000)     5605 2022-02-21 19:19:28.000000 persyn-0.1.1.dev0/src/persyn/dreams/stylegan2/metrics/perceptual_path_length.py
--rwxr-xr-x   0 rob       (1000) rob       (1000)    11437 2022-02-21 19:19:28.000000 persyn-0.1.1.dev0/src/persyn/dreams/stylegan2/metrics/precision_recall.py
--rwxr-xr-x   0 rob       (1000) rob       (1000)     7521 2022-02-21 19:19:05.000000 persyn-0.1.1.dev0/src/persyn/dreams/stylegan2/pretrained_networks.py
--rwxr-xr-x   0 rob       (1000) rob       (1000)     8975 2022-02-21 19:19:05.000000 persyn-0.1.1.dev0/src/persyn/dreams/stylegan2/projector.py
--rwxr-xr-x   0 rob       (1000) rob       (1000)     8245 2022-02-21 19:19:05.000000 persyn-0.1.1.dev0/src/persyn/dreams/stylegan2/run_generator.py
--rwxr-xr-x   0 rob       (1000) rob       (1000)     3447 2022-02-21 19:19:05.000000 persyn-0.1.1.dev0/src/persyn/dreams/stylegan2/run_metrics.py
--rwxr-xr-x   0 rob       (1000) rob       (1000)     6963 2022-02-21 19:19:05.000000 persyn-0.1.1.dev0/src/persyn/dreams/stylegan2/run_projector.py
--rwxr-xr-x   0 rob       (1000) rob       (1000)     8473 2022-02-21 19:19:05.000000 persyn-0.1.1.dev0/src/persyn/dreams/stylegan2/run_training.py
-drwxrwxr-x   0 rob       (1000) rob       (1000)        0 2023-05-22 03:00:45.731716 persyn-0.1.1.dev0/src/persyn/dreams/stylegan2/training/
--rwxr-xr-x   0 rob       (1000) rob       (1000)      235 2022-02-21 19:19:28.000000 persyn-0.1.1.dev0/src/persyn/dreams/stylegan2/training/__init__.py
--rwxr-xr-x   0 rob       (1000) rob       (1000)     9881 2022-02-21 19:19:28.000000 persyn-0.1.1.dev0/src/persyn/dreams/stylegan2/training/dataset.py
--rwxr-xr-x   0 rob       (1000) rob       (1000)    10731 2022-02-21 19:19:28.000000 persyn-0.1.1.dev0/src/persyn/dreams/stylegan2/training/loss.py
--rwxr-xr-x   0 rob       (1000) rob       (1000)     5706 2022-02-21 19:19:28.000000 persyn-0.1.1.dev0/src/persyn/dreams/stylegan2/training/misc.py
--rwxr-xr-x   0 rob       (1000) rob       (1000)    33273 2022-02-21 19:19:28.000000 persyn-0.1.1.dev0/src/persyn/dreams/stylegan2/training/networks_stylegan.py
--rwxr-xr-x   0 rob       (1000) rob       (1000)    38074 2022-02-21 19:19:28.000000 persyn-0.1.1.dev0/src/persyn/dreams/stylegan2/training/networks_stylegan2.py
--rwxr-xr-x   0 rob       (1000) rob       (1000)    19892 2022-02-21 19:19:28.000000 persyn-0.1.1.dev0/src/persyn/dreams/stylegan2/training/training_loop.py
-drwxrwxr-x   0 rob       (1000) rob       (1000)        0 2023-05-22 03:00:45.731716 persyn-0.1.1.dev0/src/persyn/interaction/
--rw-rw-r--   0 rob       (1000) rob       (1000)        0 2023-05-22 02:29:25.000000 persyn-0.1.1.dev0/src/persyn/interaction/__init__.py
--rw-rw-r--   0 rob       (1000) rob       (1000)     1186 2023-05-22 02:29:25.000000 persyn-0.1.1.dev0/src/persyn/interaction/chrono.py
--rw-rw-r--   0 rob       (1000) rob       (1000)    17244 2023-05-22 02:29:25.000000 persyn-0.1.1.dev0/src/persyn/interaction/cns.py
--rw-rw-r--   0 rob       (1000) rob       (1000)     2864 2023-05-22 02:29:25.000000 persyn-0.1.1.dev0/src/persyn/interaction/completion.py
--rw-rw-r--   0 rob       (1000) rob       (1000)    29689 2023-05-22 02:29:25.000000 persyn-0.1.1.dev0/src/persyn/interaction/feels.py
--rw-rw-r--   0 rob       (1000) rob       (1000)    26517 2023-05-22 02:29:25.000000 persyn-0.1.1.dev0/src/persyn/interaction/gpt.py
--rw-rw-r--   0 rob       (1000) rob       (1000)     8333 2023-05-22 02:29:25.000000 persyn-0.1.1.dev0/src/persyn/interaction/graph.py
--rwxrwxr-x   0 rob       (1000) rob       (1000)       60 2023-05-22 02:29:25.000000 persyn-0.1.1.dev0/src/persyn/interaction/install.py
--rw-rw-r--   0 rob       (1000) rob       (1000)    21658 2023-05-22 02:29:25.000000 persyn-0.1.1.dev0/src/persyn/interaction/interact.py
--rwxrwxr-x   0 rob       (1000) rob       (1000)    12617 2023-05-22 02:29:25.000000 persyn-0.1.1.dev0/src/persyn/interaction/interact_server.py
--rw-rw-r--   0 rob       (1000) rob       (1000)    30437 2023-05-22 02:29:25.000000 persyn-0.1.1.dev0/src/persyn/interaction/memory.py
--rw-rw-r--   0 rob       (1000) rob       (1000)     2176 2023-05-22 02:29:25.000000 persyn-0.1.1.dev0/src/persyn/interaction/messages.py
--rw-rw-r--   0 rob       (1000) rob       (1000)    13828 2023-05-22 02:29:25.000000 persyn-0.1.1.dev0/src/persyn/interaction/nlp_cloud.py
-drwxrwxr-x   0 rob       (1000) rob       (1000)        0 2023-05-22 03:00:45.719716 persyn-0.1.1.dev0/src/persyn/interaction/notebooks/
-drwxrwxr-x   0 rob       (1000) rob       (1000)        0 2023-05-22 03:00:45.719716 persyn-0.1.1.dev0/src/persyn/interaction/notebooks/env/
-drwxrwxr-x   0 rob       (1000) rob       (1000)        0 2023-05-22 03:00:45.731716 persyn-0.1.1.dev0/src/persyn/interaction/notebooks/env/bin/
--rw-rw-r--   0 rob       (1000) rob       (1000)     1199 2022-10-23 00:31:31.000000 persyn-0.1.1.dev0/src/persyn/interaction/notebooks/env/bin/activate_this.py
--rwxrwxr-x   0 rob       (1000) rob       (1000)     1732 2022-12-04 20:53:32.000000 persyn-0.1.1.dev0/src/persyn/interaction/notebooks/env/bin/jp.py
--rw-rw-r--   0 rob       (1000) rob       (1000)    13403 2023-05-22 02:29:25.000000 persyn-0.1.1.dev0/src/persyn/interaction/relationships.py
--rw-rw-r--   0 rob       (1000) rob       (1000)     2732 2023-05-22 02:29:25.000000 persyn-0.1.1.dev0/src/persyn/interaction/reminders.py
--rw-rw-r--   0 rob       (1000) rob       (1000)     1248 2023-05-22 02:29:25.000000 persyn-0.1.1.dev0/src/persyn/interaction/voice.py
--rwxrwxr-x   0 rob       (1000) rob       (1000)      870 2023-05-22 02:29:25.000000 persyn-0.1.1.dev0/src/persyn/kill_bot.py
--rwxrwxr-x   0 rob       (1000) rob       (1000)     4562 2023-05-22 02:29:25.000000 persyn-0.1.1.dev0/src/persyn/launch_bot.py
-drwxrwxr-x   0 rob       (1000) rob       (1000)        0 2023-05-22 03:00:45.735715 persyn-0.1.1.dev0/src/persyn/utils/
--rw-rw-r--   0 rob       (1000) rob       (1000)        0 2023-05-22 02:29:25.000000 persyn-0.1.1.dev0/src/persyn/utils/__init__.py
--rw-rw-r--   0 rob       (1000) rob       (1000)     5169 2023-05-22 02:29:25.000000 persyn-0.1.1.dev0/src/persyn/utils/art.py
--rw-rw-r--   0 rob       (1000) rob       (1000)     1623 2023-05-22 02:29:25.000000 persyn-0.1.1.dev0/src/persyn/utils/color_logging.py
--rw-rw-r--   0 rob       (1000) rob       (1000)     4648 2023-05-22 02:29:25.000000 persyn-0.1.1.dev0/src/persyn/utils/config.py
-drwxrwxr-x   0 rob       (1000) rob       (1000)        0 2023-05-22 03:00:45.719716 persyn-0.1.1.dev0/src/persyn.egg-info/
--rw-rw-r--   0 rob       (1000) rob       (1000)     3526 2023-05-22 03:00:45.000000 persyn-0.1.1.dev0/src/persyn.egg-info/PKG-INFO
--rw-rw-r--   0 rob       (1000) rob       (1000)     4086 2023-05-22 03:00:45.000000 persyn-0.1.1.dev0/src/persyn.egg-info/SOURCES.txt
--rw-rw-r--   0 rob       (1000) rob       (1000)        1 2023-05-22 03:00:45.000000 persyn-0.1.1.dev0/src/persyn.egg-info/dependency_links.txt
--rw-rw-r--   0 rob       (1000) rob       (1000)      779 2023-05-22 03:00:45.000000 persyn-0.1.1.dev0/src/persyn.egg-info/entry_points.txt
--rw-rw-r--   0 rob       (1000) rob       (1000)      562 2023-05-22 03:00:45.000000 persyn-0.1.1.dev0/src/persyn.egg-info/requires.txt
--rw-rw-r--   0 rob       (1000) rob       (1000)        7 2023-05-22 03:00:45.000000 persyn-0.1.1.dev0/src/persyn.egg-info/top_level.txt
+drwxrwxr-x   0 rob       (1000) rob       (1000)        0 2023-05-22 03:10:08.067473 persyn-0.1.2/
+-rw-rw-r--   0 rob       (1000) rob       (1000)     1058 2023-01-09 01:22:11.000000 persyn-0.1.2/LICENSE.txt
+-rw-rw-r--   0 rob       (1000) rob       (1000)     3521 2023-05-22 03:10:08.067473 persyn-0.1.2/PKG-INFO
+-rw-rw-r--   0 rob       (1000) rob       (1000)     2944 2023-05-22 02:29:25.000000 persyn-0.1.2/README.md
+-rw-rw-r--   0 rob       (1000) rob       (1000)     2385 2023-05-22 03:09:47.000000 persyn-0.1.2/pyproject.toml
+-rw-rw-r--   0 rob       (1000) rob       (1000)       38 2023-05-22 03:10:08.067473 persyn-0.1.2/setup.cfg
+drwxrwxr-x   0 rob       (1000) rob       (1000)        0 2023-05-22 03:10:08.051473 persyn-0.1.2/src/
+drwxrwxr-x   0 rob       (1000) rob       (1000)        0 2023-05-22 03:10:08.055473 persyn-0.1.2/src/persyn/
+-rw-rw-r--   0 rob       (1000) rob       (1000)        0 2023-05-22 02:29:25.000000 persyn-0.1.2/src/persyn/__init__.py
+drwxrwxr-x   0 rob       (1000) rob       (1000)        0 2023-05-22 03:10:08.055473 persyn-0.1.2/src/persyn/chat/
+-rw-rw-r--   0 rob       (1000) rob       (1000)        0 2023-05-22 02:29:25.000000 persyn-0.1.2/src/persyn/chat/__init__.py
+-rw-rw-r--   0 rob       (1000) rob       (1000)    14576 2023-05-22 02:29:25.000000 persyn-0.1.2/src/persyn/chat/common.py
+drwxrwxr-x   0 rob       (1000) rob       (1000)        0 2023-05-22 03:10:08.055473 persyn-0.1.2/src/persyn/chat/discord/
+-rwxrwxr-x   0 rob       (1000) rob       (1000)     1740 2023-05-22 02:29:25.000000 persyn-0.1.2/src/persyn/chat/discord/basic.py
+-rwxrwxr-x   0 rob       (1000) rob       (1000)    11065 2023-05-22 02:29:25.000000 persyn-0.1.2/src/persyn/chat/discord/bot.py
+drwxrwxr-x   0 rob       (1000) rob       (1000)        0 2023-05-22 03:10:08.055473 persyn-0.1.2/src/persyn/chat/mastodon/
+-rwxrwxr-x   0 rob       (1000) rob       (1000)    11540 2023-05-22 02:29:25.000000 persyn-0.1.2/src/persyn/chat/mastodon/bot.py
+-rw-rw-r--   0 rob       (1000) rob       (1000)     2015 2023-05-22 02:29:25.000000 persyn-0.1.2/src/persyn/chat/mastodon/login.py
+-rwxrwxr-x   0 rob       (1000) rob       (1000)     1208 2023-05-22 02:29:25.000000 persyn-0.1.2/src/persyn/chat/mastodon/masto-login.py
+-rwxrwxr-x   0 rob       (1000) rob       (1000)     1919 2023-05-22 02:29:25.000000 persyn-0.1.2/src/persyn/chat/mastodon/masto-stream.py
+-rw-rw-r--   0 rob       (1000) rob       (1000)     3321 2023-05-22 02:29:25.000000 persyn-0.1.2/src/persyn/chat/simple.py
+drwxrwxr-x   0 rob       (1000) rob       (1000)        0 2023-05-22 03:10:08.055473 persyn-0.1.2/src/persyn/chat/slack/
+-rwxrwxr-x   0 rob       (1000) rob       (1000)    18640 2023-05-22 02:29:25.000000 persyn-0.1.2/src/persyn/chat/slack/bot.py
+drwxrwxr-x   0 rob       (1000) rob       (1000)        0 2023-05-22 03:10:08.059473 persyn-0.1.2/src/persyn/chat/stdio/
+-rw-rw-r--   0 rob       (1000) rob       (1000)     1502 2023-05-22 02:29:25.000000 persyn-0.1.2/src/persyn/chat/stdio/add_goal.py
+-rw-rw-r--   0 rob       (1000) rob       (1000)     1450 2023-05-22 02:29:25.000000 persyn-0.1.2/src/persyn/chat/stdio/elaborate.py
+-rwxrwxr-x   0 rob       (1000) rob       (1000)     3284 2023-05-22 02:29:25.000000 persyn-0.1.2/src/persyn/chat/stdio/import_text.py
+-rw-rw-r--   0 rob       (1000) rob       (1000)     1617 2023-05-22 02:29:25.000000 persyn-0.1.2/src/persyn/chat/stdio/inject_idea.py
+-rw-rw-r--   0 rob       (1000) rob       (1000)     1661 2023-05-22 02:29:25.000000 persyn-0.1.2/src/persyn/chat/stdio/opine.py
+-rw-rw-r--   0 rob       (1000) rob       (1000)     1620 2023-05-22 02:29:25.000000 persyn-0.1.2/src/persyn/chat/stdio/read_rss.py
+-rw-rw-r--   0 rob       (1000) rob       (1000)     1774 2023-05-22 02:29:25.000000 persyn-0.1.2/src/persyn/chat/stdio/read_url.py
+-rw-rw-r--   0 rob       (1000) rob       (1000)     1505 2023-05-22 02:29:25.000000 persyn-0.1.2/src/persyn/chat/stdio/send_chat.py
+-rw-rw-r--   0 rob       (1000) rob       (1000)     1685 2023-05-22 02:29:25.000000 persyn-0.1.2/src/persyn/chat/stdio/summarize.py
+drwxrwxr-x   0 rob       (1000) rob       (1000)        0 2023-05-22 03:10:08.059473 persyn-0.1.2/src/persyn/dreams/
+-rw-rw-r--   0 rob       (1000) rob       (1000)        0 2023-05-22 02:29:25.000000 persyn-0.1.2/src/persyn/dreams/__init__.py
+drwxrwxr-x   0 rob       (1000) rob       (1000)        0 2023-05-22 03:10:08.059473 persyn-0.1.2/src/persyn/dreams/clip_interrogator/
+-rw-rw-r--   0 rob       (1000) rob       (1000)        0 2023-05-22 02:29:25.000000 persyn-0.1.2/src/persyn/dreams/clip_interrogator/__init__.py
+-rw-rw-r--   0 rob       (1000) rob       (1000)    10568 2023-05-22 02:29:25.000000 persyn-0.1.2/src/persyn/dreams/clip_interrogator/interrogator.py
+-rw-rw-r--   0 rob       (1000) rob       (1000)     5892 2023-05-22 02:57:37.000000 persyn-0.1.2/src/persyn/dreams/dreams.py
+drwxrwxr-x   0 rob       (1000) rob       (1000)        0 2023-05-22 03:10:08.059473 persyn-0.1.2/src/persyn/dreams/prompt-parrot/
+-rw-rw-r--   0 rob       (1000) rob       (1000)     2939 2023-05-22 02:29:25.000000 persyn-0.1.2/src/persyn/dreams/prompt-parrot/prompt-parrot.py
+-rwxrwxr-x   0 rob       (1000) rob       (1000)      434 2023-05-22 02:29:25.000000 persyn-0.1.2/src/persyn/dreams/receive-sqs.py
+-rwxrwxr-x   0 rob       (1000) rob       (1000)      898 2023-05-22 02:29:25.000000 persyn-0.1.2/src/persyn/dreams/send-sqs.py
+-rw-rw-r--   0 rob       (1000) rob       (1000)     6387 2023-05-22 02:59:43.000000 persyn-0.1.2/src/persyn/dreams/stable_diffusion.py
+drwxrwxr-x   0 rob       (1000) rob       (1000)        0 2023-05-22 03:10:08.059473 persyn-0.1.2/src/persyn/dreams/stylegan2/
+-rwxr-xr-x   0 rob       (1000) rob       (1000)    30282 2022-02-21 19:19:05.000000 persyn-0.1.2/src/persyn/dreams/stylegan2/dataset_tool.py
+drwxrwxr-x   0 rob       (1000) rob       (1000)        0 2023-05-22 03:10:08.059473 persyn-0.1.2/src/persyn/dreams/stylegan2/dnnlib/
+-rwxr-xr-x   0 rob       (1000) rob       (1000)      774 2022-02-21 19:19:28.000000 persyn-0.1.2/src/persyn/dreams/stylegan2/dnnlib/__init__.py
+drwxrwxr-x   0 rob       (1000) rob       (1000)        0 2023-05-22 03:10:08.059473 persyn-0.1.2/src/persyn/dreams/stylegan2/dnnlib/submission/
+-rwxr-xr-x   0 rob       (1000) rob       (1000)      274 2022-02-21 19:19:28.000000 persyn-0.1.2/src/persyn/dreams/stylegan2/dnnlib/submission/__init__.py
+drwxrwxr-x   0 rob       (1000) rob       (1000)        0 2023-05-22 03:10:08.059473 persyn-0.1.2/src/persyn/dreams/stylegan2/dnnlib/submission/internal/
+-rwxr-xr-x   0 rob       (1000) rob       (1000)      247 2022-02-21 19:19:28.000000 persyn-0.1.2/src/persyn/dreams/stylegan2/dnnlib/submission/internal/__init__.py
+-rwxr-xr-x   0 rob       (1000) rob       (1000)      769 2022-02-21 19:19:28.000000 persyn-0.1.2/src/persyn/dreams/stylegan2/dnnlib/submission/internal/local.py
+-rwxr-xr-x   0 rob       (1000) rob       (1000)     4245 2022-02-21 19:19:28.000000 persyn-0.1.2/src/persyn/dreams/stylegan2/dnnlib/submission/run_context.py
+-rwxr-xr-x   0 rob       (1000) rob       (1000)    13502 2022-02-21 19:19:28.000000 persyn-0.1.2/src/persyn/dreams/stylegan2/dnnlib/submission/submit.py
+drwxrwxr-x   0 rob       (1000) rob       (1000)        0 2023-05-22 03:10:08.063473 persyn-0.1.2/src/persyn/dreams/stylegan2/dnnlib/tflib/
+-rwxr-xr-x   0 rob       (1000) rob       (1000)      467 2022-02-21 19:19:28.000000 persyn-0.1.2/src/persyn/dreams/stylegan2/dnnlib/tflib/__init__.py
+-rwxr-xr-x   0 rob       (1000) rob       (1000)     8038 2022-02-21 19:19:28.000000 persyn-0.1.2/src/persyn/dreams/stylegan2/dnnlib/tflib/autosummary.py
+-rwxr-xr-x   0 rob       (1000) rob       (1000)     7223 2022-02-21 19:19:28.000000 persyn-0.1.2/src/persyn/dreams/stylegan2/dnnlib/tflib/custom_ops.py
+-rwxr-xr-x   0 rob       (1000) rob       (1000)    29982 2022-02-21 19:19:28.000000 persyn-0.1.2/src/persyn/dreams/stylegan2/dnnlib/tflib/network.py
+drwxrwxr-x   0 rob       (1000) rob       (1000)        0 2023-05-22 03:10:08.063473 persyn-0.1.2/src/persyn/dreams/stylegan2/dnnlib/tflib/ops/
+-rwxr-xr-x   0 rob       (1000) rob       (1000)      235 2022-02-21 19:19:28.000000 persyn-0.1.2/src/persyn/dreams/stylegan2/dnnlib/tflib/ops/__init__.py
+-rwxr-xr-x   0 rob       (1000) rob       (1000)     8539 2022-02-21 19:19:28.000000 persyn-0.1.2/src/persyn/dreams/stylegan2/dnnlib/tflib/ops/fused_bias_act.py
+-rwxr-xr-x   0 rob       (1000) rob       (1000)    16588 2022-02-21 19:19:28.000000 persyn-0.1.2/src/persyn/dreams/stylegan2/dnnlib/tflib/ops/upfirdn_2d.py
+-rwxr-xr-x   0 rob       (1000) rob       (1000)    20298 2022-02-21 19:19:28.000000 persyn-0.1.2/src/persyn/dreams/stylegan2/dnnlib/tflib/optimizer.py
+-rwxr-xr-x   0 rob       (1000) rob       (1000)     9675 2022-02-21 19:19:28.000000 persyn-0.1.2/src/persyn/dreams/stylegan2/dnnlib/tflib/tfutil.py
+-rwxr-xr-x   0 rob       (1000) rob       (1000)    13916 2022-02-21 19:19:28.000000 persyn-0.1.2/src/persyn/dreams/stylegan2/dnnlib/util.py
+-rwxr-xr-x   0 rob       (1000) rob       (1000)     2722 2022-02-21 19:19:05.000000 persyn-0.1.2/src/persyn/dreams/stylegan2/make_a_face.py
+drwxrwxr-x   0 rob       (1000) rob       (1000)        0 2023-05-22 03:10:08.063473 persyn-0.1.2/src/persyn/dreams/stylegan2/metrics/
+-rwxr-xr-x   0 rob       (1000) rob       (1000)      235 2022-02-21 19:19:28.000000 persyn-0.1.2/src/persyn/dreams/stylegan2/metrics/__init__.py
+-rwxr-xr-x   0 rob       (1000) rob       (1000)     3330 2022-02-21 19:19:28.000000 persyn-0.1.2/src/persyn/dreams/stylegan2/metrics/frechet_inception_distance.py
+-rwxr-xr-x   0 rob       (1000) rob       (1000)     2587 2022-02-21 19:19:28.000000 persyn-0.1.2/src/persyn/dreams/stylegan2/metrics/inception_score.py
+-rwxr-xr-x   0 rob       (1000) rob       (1000)     9978 2022-02-21 19:19:28.000000 persyn-0.1.2/src/persyn/dreams/stylegan2/metrics/linear_separability.py
+-rwxr-xr-x   0 rob       (1000) rob       (1000)     7055 2022-02-21 19:19:28.000000 persyn-0.1.2/src/persyn/dreams/stylegan2/metrics/metric_base.py
+-rwxr-xr-x   0 rob       (1000) rob       (1000)     2311 2022-02-21 19:19:28.000000 persyn-0.1.2/src/persyn/dreams/stylegan2/metrics/metric_defaults.py
+-rwxr-xr-x   0 rob       (1000) rob       (1000)     5605 2022-02-21 19:19:28.000000 persyn-0.1.2/src/persyn/dreams/stylegan2/metrics/perceptual_path_length.py
+-rwxr-xr-x   0 rob       (1000) rob       (1000)    11437 2022-02-21 19:19:28.000000 persyn-0.1.2/src/persyn/dreams/stylegan2/metrics/precision_recall.py
+-rwxr-xr-x   0 rob       (1000) rob       (1000)     7521 2022-02-21 19:19:05.000000 persyn-0.1.2/src/persyn/dreams/stylegan2/pretrained_networks.py
+-rwxr-xr-x   0 rob       (1000) rob       (1000)     8975 2022-02-21 19:19:05.000000 persyn-0.1.2/src/persyn/dreams/stylegan2/projector.py
+-rwxr-xr-x   0 rob       (1000) rob       (1000)     8245 2022-02-21 19:19:05.000000 persyn-0.1.2/src/persyn/dreams/stylegan2/run_generator.py
+-rwxr-xr-x   0 rob       (1000) rob       (1000)     3447 2022-02-21 19:19:05.000000 persyn-0.1.2/src/persyn/dreams/stylegan2/run_metrics.py
+-rwxr-xr-x   0 rob       (1000) rob       (1000)     6963 2022-02-21 19:19:05.000000 persyn-0.1.2/src/persyn/dreams/stylegan2/run_projector.py
+-rwxr-xr-x   0 rob       (1000) rob       (1000)     8473 2022-02-21 19:19:05.000000 persyn-0.1.2/src/persyn/dreams/stylegan2/run_training.py
+drwxrwxr-x   0 rob       (1000) rob       (1000)        0 2023-05-22 03:10:08.063473 persyn-0.1.2/src/persyn/dreams/stylegan2/training/
+-rwxr-xr-x   0 rob       (1000) rob       (1000)      235 2022-02-21 19:19:28.000000 persyn-0.1.2/src/persyn/dreams/stylegan2/training/__init__.py
+-rwxr-xr-x   0 rob       (1000) rob       (1000)     9881 2022-02-21 19:19:28.000000 persyn-0.1.2/src/persyn/dreams/stylegan2/training/dataset.py
+-rwxr-xr-x   0 rob       (1000) rob       (1000)    10731 2022-02-21 19:19:28.000000 persyn-0.1.2/src/persyn/dreams/stylegan2/training/loss.py
+-rwxr-xr-x   0 rob       (1000) rob       (1000)     5706 2022-02-21 19:19:28.000000 persyn-0.1.2/src/persyn/dreams/stylegan2/training/misc.py
+-rwxr-xr-x   0 rob       (1000) rob       (1000)    33273 2022-02-21 19:19:28.000000 persyn-0.1.2/src/persyn/dreams/stylegan2/training/networks_stylegan.py
+-rwxr-xr-x   0 rob       (1000) rob       (1000)    38074 2022-02-21 19:19:28.000000 persyn-0.1.2/src/persyn/dreams/stylegan2/training/networks_stylegan2.py
+-rwxr-xr-x   0 rob       (1000) rob       (1000)    19892 2022-02-21 19:19:28.000000 persyn-0.1.2/src/persyn/dreams/stylegan2/training/training_loop.py
+drwxrwxr-x   0 rob       (1000) rob       (1000)        0 2023-05-22 03:10:08.067473 persyn-0.1.2/src/persyn/interaction/
+-rw-rw-r--   0 rob       (1000) rob       (1000)        0 2023-05-22 02:29:25.000000 persyn-0.1.2/src/persyn/interaction/__init__.py
+-rw-rw-r--   0 rob       (1000) rob       (1000)     1186 2023-05-22 02:29:25.000000 persyn-0.1.2/src/persyn/interaction/chrono.py
+-rw-rw-r--   0 rob       (1000) rob       (1000)    17244 2023-05-22 02:29:25.000000 persyn-0.1.2/src/persyn/interaction/cns.py
+-rw-rw-r--   0 rob       (1000) rob       (1000)     2864 2023-05-22 02:29:25.000000 persyn-0.1.2/src/persyn/interaction/completion.py
+-rw-rw-r--   0 rob       (1000) rob       (1000)    29689 2023-05-22 02:29:25.000000 persyn-0.1.2/src/persyn/interaction/feels.py
+-rw-rw-r--   0 rob       (1000) rob       (1000)    26517 2023-05-22 02:29:25.000000 persyn-0.1.2/src/persyn/interaction/gpt.py
+-rw-rw-r--   0 rob       (1000) rob       (1000)     8333 2023-05-22 02:29:25.000000 persyn-0.1.2/src/persyn/interaction/graph.py
+-rwxrwxr-x   0 rob       (1000) rob       (1000)       60 2023-05-22 02:29:25.000000 persyn-0.1.2/src/persyn/interaction/install.py
+-rw-rw-r--   0 rob       (1000) rob       (1000)    21658 2023-05-22 02:29:25.000000 persyn-0.1.2/src/persyn/interaction/interact.py
+-rwxrwxr-x   0 rob       (1000) rob       (1000)    12617 2023-05-22 02:29:25.000000 persyn-0.1.2/src/persyn/interaction/interact_server.py
+-rw-rw-r--   0 rob       (1000) rob       (1000)    30437 2023-05-22 02:29:25.000000 persyn-0.1.2/src/persyn/interaction/memory.py
+-rw-rw-r--   0 rob       (1000) rob       (1000)     2176 2023-05-22 02:29:25.000000 persyn-0.1.2/src/persyn/interaction/messages.py
+-rw-rw-r--   0 rob       (1000) rob       (1000)    13828 2023-05-22 02:29:25.000000 persyn-0.1.2/src/persyn/interaction/nlp_cloud.py
+drwxrwxr-x   0 rob       (1000) rob       (1000)        0 2023-05-22 03:10:08.055473 persyn-0.1.2/src/persyn/interaction/notebooks/
+drwxrwxr-x   0 rob       (1000) rob       (1000)        0 2023-05-22 03:10:08.055473 persyn-0.1.2/src/persyn/interaction/notebooks/env/
+drwxrwxr-x   0 rob       (1000) rob       (1000)        0 2023-05-22 03:10:08.067473 persyn-0.1.2/src/persyn/interaction/notebooks/env/bin/
+-rw-rw-r--   0 rob       (1000) rob       (1000)     1199 2022-10-23 00:31:31.000000 persyn-0.1.2/src/persyn/interaction/notebooks/env/bin/activate_this.py
+-rwxrwxr-x   0 rob       (1000) rob       (1000)     1732 2022-12-04 20:53:32.000000 persyn-0.1.2/src/persyn/interaction/notebooks/env/bin/jp.py
+-rw-rw-r--   0 rob       (1000) rob       (1000)    13403 2023-05-22 02:29:25.000000 persyn-0.1.2/src/persyn/interaction/relationships.py
+-rw-rw-r--   0 rob       (1000) rob       (1000)     2732 2023-05-22 02:29:25.000000 persyn-0.1.2/src/persyn/interaction/reminders.py
+-rw-rw-r--   0 rob       (1000) rob       (1000)     1248 2023-05-22 02:29:25.000000 persyn-0.1.2/src/persyn/interaction/voice.py
+-rwxrwxr-x   0 rob       (1000) rob       (1000)      870 2023-05-22 02:29:25.000000 persyn-0.1.2/src/persyn/kill_bot.py
+-rwxrwxr-x   0 rob       (1000) rob       (1000)     4562 2023-05-22 02:29:25.000000 persyn-0.1.2/src/persyn/launch_bot.py
+drwxrwxr-x   0 rob       (1000) rob       (1000)        0 2023-05-22 03:10:08.067473 persyn-0.1.2/src/persyn/utils/
+-rw-rw-r--   0 rob       (1000) rob       (1000)        0 2023-05-22 02:29:25.000000 persyn-0.1.2/src/persyn/utils/__init__.py
+-rw-rw-r--   0 rob       (1000) rob       (1000)     5169 2023-05-22 02:29:25.000000 persyn-0.1.2/src/persyn/utils/art.py
+-rw-rw-r--   0 rob       (1000) rob       (1000)     1623 2023-05-22 02:29:25.000000 persyn-0.1.2/src/persyn/utils/color_logging.py
+-rw-rw-r--   0 rob       (1000) rob       (1000)     4648 2023-05-22 02:29:25.000000 persyn-0.1.2/src/persyn/utils/config.py
+drwxrwxr-x   0 rob       (1000) rob       (1000)        0 2023-05-22 03:10:08.055473 persyn-0.1.2/src/persyn.egg-info/
+-rw-rw-r--   0 rob       (1000) rob       (1000)     3521 2023-05-22 03:10:08.000000 persyn-0.1.2/src/persyn.egg-info/PKG-INFO
+-rw-rw-r--   0 rob       (1000) rob       (1000)     4086 2023-05-22 03:10:08.000000 persyn-0.1.2/src/persyn.egg-info/SOURCES.txt
+-rw-rw-r--   0 rob       (1000) rob       (1000)        1 2023-05-22 03:10:08.000000 persyn-0.1.2/src/persyn.egg-info/dependency_links.txt
+-rw-rw-r--   0 rob       (1000) rob       (1000)      779 2023-05-22 03:10:08.000000 persyn-0.1.2/src/persyn.egg-info/entry_points.txt
+-rw-rw-r--   0 rob       (1000) rob       (1000)      562 2023-05-22 03:10:08.000000 persyn-0.1.2/src/persyn.egg-info/requires.txt
+-rw-rw-r--   0 rob       (1000) rob       (1000)        7 2023-05-22 03:10:08.000000 persyn-0.1.2/src/persyn.egg-info/top_level.txt
```

### Comparing `persyn-0.1.1.dev0/LICENSE.txt` & `persyn-0.1.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `persyn-0.1.1.dev0/PKG-INFO` & `persyn-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: persyn
-Version: 0.1.1.dev0
+Version: 0.1.2
 Summary: Personality Syndrome. Persyn for short.
 Author-email: Rob Flickenger <rob@hackerfriendly.com>
 Project-URL: Homepage, https://persyn.io
 Project-URL: Bug Tracker, https://github.com/hackerfriendly/persyn/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `persyn-0.1.1.dev0/README.md` & `persyn-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `persyn-0.1.1.dev0/pyproject.toml` & `persyn-0.1.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "persyn"
-version = "0.1.1-dev"
+version = "0.1.2"
 authors = [
   { name="Rob Flickenger", email="rob@hackerfriendly.com" },
 ]
 description = "Personality Syndrome. Persyn for short."
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `persyn-0.1.1.dev0/src/persyn/chat/common.py` & `persyn-0.1.2/src/persyn/chat/common.py`

 * *Files identical despite different names*

### Comparing `persyn-0.1.1.dev0/src/persyn/chat/discord/basic.py` & `persyn-0.1.2/src/persyn/chat/discord/basic.py`

 * *Files identical despite different names*

### Comparing `persyn-0.1.1.dev0/src/persyn/chat/discord/bot.py` & `persyn-0.1.2/src/persyn/chat/discord/bot.py`

 * *Files identical despite different names*

### Comparing `persyn-0.1.1.dev0/src/persyn/chat/mastodon/bot.py` & `persyn-0.1.2/src/persyn/chat/mastodon/bot.py`

 * *Files identical despite different names*

### Comparing `persyn-0.1.1.dev0/src/persyn/chat/mastodon/login.py` & `persyn-0.1.2/src/persyn/chat/mastodon/login.py`

 * *Files identical despite different names*

### Comparing `persyn-0.1.1.dev0/src/persyn/chat/mastodon/masto-login.py` & `persyn-0.1.2/src/persyn/chat/mastodon/masto-login.py`

 * *Files identical despite different names*

### Comparing `persyn-0.1.1.dev0/src/persyn/chat/mastodon/masto-stream.py` & `persyn-0.1.2/src/persyn/chat/mastodon/masto-stream.py`

 * *Files identical despite different names*

### Comparing `persyn-0.1.1.dev0/src/persyn/chat/simple.py` & `persyn-0.1.2/src/persyn/chat/simple.py`

 * *Files identical despite different names*

### Comparing `persyn-0.1.1.dev0/src/persyn/chat/slack/bot.py` & `persyn-0.1.2/src/persyn/chat/slack/bot.py`

 * *Files identical despite different names*

### Comparing `persyn-0.1.1.dev0/src/persyn/chat/stdio/add_goal.py` & `persyn-0.1.2/src/persyn/chat/stdio/add_goal.py`

 * *Files identical despite different names*

### Comparing `persyn-0.1.1.dev0/src/persyn/chat/stdio/elaborate.py` & `persyn-0.1.2/src/persyn/chat/stdio/elaborate.py`

 * *Files identical despite different names*

### Comparing `persyn-0.1.1.dev0/src/persyn/chat/stdio/import_text.py` & `persyn-0.1.2/src/persyn/chat/stdio/import_text.py`

 * *Files identical despite different names*

### Comparing `persyn-0.1.1.dev0/src/persyn/chat/stdio/inject_idea.py` & `persyn-0.1.2/src/persyn/chat/stdio/inject_idea.py`

 * *Files identical despite different names*

### Comparing `persyn-0.1.1.dev0/src/persyn/chat/stdio/opine.py` & `persyn-0.1.2/src/persyn/chat/stdio/opine.py`

 * *Files identical despite different names*

### Comparing `persyn-0.1.1.dev0/src/persyn/chat/stdio/read_rss.py` & `persyn-0.1.2/src/persyn/chat/stdio/read_rss.py`

 * *Files identical despite different names*

### Comparing `persyn-0.1.1.dev0/src/persyn/chat/stdio/read_url.py` & `persyn-0.1.2/src/persyn/chat/stdio/read_url.py`

 * *Files identical despite different names*

### Comparing `persyn-0.1.1.dev0/src/persyn/chat/stdio/send_chat.py` & `persyn-0.1.2/src/persyn/chat/stdio/send_chat.py`

 * *Files identical despite different names*

### Comparing `persyn-0.1.1.dev0/src/persyn/chat/stdio/summarize.py` & `persyn-0.1.2/src/persyn/chat/stdio/summarize.py`

 * *Files identical despite different names*

### Comparing `persyn-0.1.1.dev0/src/persyn/dreams/clip_interrogator/interrogator.py` & `persyn-0.1.2/src/persyn/dreams/clip_interrogator/interrogator.py`

 * *Files identical despite different names*

### Comparing `persyn-0.1.1.dev0/src/persyn/dreams/dreams.py` & `persyn-0.1.2/src/persyn/dreams/dreams.py`

 * *Files identical despite different names*

### Comparing `persyn-0.1.1.dev0/src/persyn/dreams/prompt-parrot/prompt-parrot.py` & `persyn-0.1.2/src/persyn/dreams/prompt-parrot/prompt-parrot.py`

 * *Files identical despite different names*

### Comparing `persyn-0.1.1.dev0/src/persyn/dreams/send-sqs.py` & `persyn-0.1.2/src/persyn/dreams/send-sqs.py`

 * *Files identical despite different names*

### Comparing `persyn-0.1.1.dev0/src/persyn/dreams/stable_diffusion.py` & `persyn-0.1.2/src/persyn/dreams/stable_diffusion.py`

 * *Files identical despite different names*

### Comparing `persyn-0.1.1.dev0/src/persyn/dreams/stylegan2/dataset_tool.py` & `persyn-0.1.2/src/persyn/dreams/stylegan2/dataset_tool.py`

 * *Files identical despite different names*

### Comparing `persyn-0.1.1.dev0/src/persyn/dreams/stylegan2/dnnlib/__init__.py` & `persyn-0.1.2/src/persyn/dreams/stylegan2/dnnlib/__init__.py`

 * *Files identical despite different names*

### Comparing `persyn-0.1.1.dev0/src/persyn/dreams/stylegan2/dnnlib/submission/internal/local.py` & `persyn-0.1.2/src/persyn/dreams/stylegan2/dnnlib/submission/internal/local.py`

 * *Files identical despite different names*

### Comparing `persyn-0.1.1.dev0/src/persyn/dreams/stylegan2/dnnlib/submission/run_context.py` & `persyn-0.1.2/src/persyn/dreams/stylegan2/dnnlib/submission/run_context.py`

 * *Files identical despite different names*

### Comparing `persyn-0.1.1.dev0/src/persyn/dreams/stylegan2/dnnlib/submission/submit.py` & `persyn-0.1.2/src/persyn/dreams/stylegan2/dnnlib/submission/submit.py`

 * *Files identical despite different names*

### Comparing `persyn-0.1.1.dev0/src/persyn/dreams/stylegan2/dnnlib/tflib/autosummary.py` & `persyn-0.1.2/src/persyn/dreams/stylegan2/dnnlib/tflib/autosummary.py`

 * *Files identical despite different names*

### Comparing `persyn-0.1.1.dev0/src/persyn/dreams/stylegan2/dnnlib/tflib/custom_ops.py` & `persyn-0.1.2/src/persyn/dreams/stylegan2/dnnlib/tflib/custom_ops.py`

 * *Files identical despite different names*

### Comparing `persyn-0.1.1.dev0/src/persyn/dreams/stylegan2/dnnlib/tflib/network.py` & `persyn-0.1.2/src/persyn/dreams/stylegan2/dnnlib/tflib/network.py`

 * *Files identical despite different names*

### Comparing `persyn-0.1.1.dev0/src/persyn/dreams/stylegan2/dnnlib/tflib/ops/fused_bias_act.py` & `persyn-0.1.2/src/persyn/dreams/stylegan2/dnnlib/tflib/ops/fused_bias_act.py`

 * *Files identical despite different names*

### Comparing `persyn-0.1.1.dev0/src/persyn/dreams/stylegan2/dnnlib/tflib/ops/upfirdn_2d.py` & `persyn-0.1.2/src/persyn/dreams/stylegan2/dnnlib/tflib/ops/upfirdn_2d.py`

 * *Files identical despite different names*

### Comparing `persyn-0.1.1.dev0/src/persyn/dreams/stylegan2/dnnlib/tflib/optimizer.py` & `persyn-0.1.2/src/persyn/dreams/stylegan2/dnnlib/tflib/optimizer.py`

 * *Files identical despite different names*

### Comparing `persyn-0.1.1.dev0/src/persyn/dreams/stylegan2/dnnlib/tflib/tfutil.py` & `persyn-0.1.2/src/persyn/dreams/stylegan2/dnnlib/tflib/tfutil.py`

 * *Files identical despite different names*

### Comparing `persyn-0.1.1.dev0/src/persyn/dreams/stylegan2/dnnlib/util.py` & `persyn-0.1.2/src/persyn/dreams/stylegan2/dnnlib/util.py`

 * *Files identical despite different names*

### Comparing `persyn-0.1.1.dev0/src/persyn/dreams/stylegan2/make_a_face.py` & `persyn-0.1.2/src/persyn/dreams/stylegan2/make_a_face.py`

 * *Files identical despite different names*

### Comparing `persyn-0.1.1.dev0/src/persyn/dreams/stylegan2/metrics/frechet_inception_distance.py` & `persyn-0.1.2/src/persyn/dreams/stylegan2/metrics/frechet_inception_distance.py`

 * *Files identical despite different names*

### Comparing `persyn-0.1.1.dev0/src/persyn/dreams/stylegan2/metrics/inception_score.py` & `persyn-0.1.2/src/persyn/dreams/stylegan2/metrics/inception_score.py`

 * *Files identical despite different names*

### Comparing `persyn-0.1.1.dev0/src/persyn/dreams/stylegan2/metrics/linear_separability.py` & `persyn-0.1.2/src/persyn/dreams/stylegan2/metrics/linear_separability.py`

 * *Files identical despite different names*

### Comparing `persyn-0.1.1.dev0/src/persyn/dreams/stylegan2/metrics/metric_base.py` & `persyn-0.1.2/src/persyn/dreams/stylegan2/metrics/metric_base.py`

 * *Files identical despite different names*

### Comparing `persyn-0.1.1.dev0/src/persyn/dreams/stylegan2/metrics/metric_defaults.py` & `persyn-0.1.2/src/persyn/dreams/stylegan2/metrics/metric_defaults.py`

 * *Files identical despite different names*

### Comparing `persyn-0.1.1.dev0/src/persyn/dreams/stylegan2/metrics/perceptual_path_length.py` & `persyn-0.1.2/src/persyn/dreams/stylegan2/metrics/perceptual_path_length.py`

 * *Files identical despite different names*

### Comparing `persyn-0.1.1.dev0/src/persyn/dreams/stylegan2/metrics/precision_recall.py` & `persyn-0.1.2/src/persyn/dreams/stylegan2/metrics/precision_recall.py`

 * *Files identical despite different names*

### Comparing `persyn-0.1.1.dev0/src/persyn/dreams/stylegan2/pretrained_networks.py` & `persyn-0.1.2/src/persyn/dreams/stylegan2/pretrained_networks.py`

 * *Files identical despite different names*

### Comparing `persyn-0.1.1.dev0/src/persyn/dreams/stylegan2/projector.py` & `persyn-0.1.2/src/persyn/dreams/stylegan2/projector.py`

 * *Files identical despite different names*

### Comparing `persyn-0.1.1.dev0/src/persyn/dreams/stylegan2/run_generator.py` & `persyn-0.1.2/src/persyn/dreams/stylegan2/run_generator.py`

 * *Files identical despite different names*

### Comparing `persyn-0.1.1.dev0/src/persyn/dreams/stylegan2/run_metrics.py` & `persyn-0.1.2/src/persyn/dreams/stylegan2/run_metrics.py`

 * *Files identical despite different names*

### Comparing `persyn-0.1.1.dev0/src/persyn/dreams/stylegan2/run_projector.py` & `persyn-0.1.2/src/persyn/dreams/stylegan2/run_projector.py`

 * *Files identical despite different names*

### Comparing `persyn-0.1.1.dev0/src/persyn/dreams/stylegan2/run_training.py` & `persyn-0.1.2/src/persyn/dreams/stylegan2/run_training.py`

 * *Files identical despite different names*

### Comparing `persyn-0.1.1.dev0/src/persyn/dreams/stylegan2/training/dataset.py` & `persyn-0.1.2/src/persyn/dreams/stylegan2/training/dataset.py`

 * *Files identical despite different names*

### Comparing `persyn-0.1.1.dev0/src/persyn/dreams/stylegan2/training/loss.py` & `persyn-0.1.2/src/persyn/dreams/stylegan2/training/loss.py`

 * *Files identical despite different names*

### Comparing `persyn-0.1.1.dev0/src/persyn/dreams/stylegan2/training/misc.py` & `persyn-0.1.2/src/persyn/dreams/stylegan2/training/misc.py`

 * *Files identical despite different names*

### Comparing `persyn-0.1.1.dev0/src/persyn/dreams/stylegan2/training/networks_stylegan.py` & `persyn-0.1.2/src/persyn/dreams/stylegan2/training/networks_stylegan.py`

 * *Files identical despite different names*

### Comparing `persyn-0.1.1.dev0/src/persyn/dreams/stylegan2/training/networks_stylegan2.py` & `persyn-0.1.2/src/persyn/dreams/stylegan2/training/networks_stylegan2.py`

 * *Files identical despite different names*

### Comparing `persyn-0.1.1.dev0/src/persyn/dreams/stylegan2/training/training_loop.py` & `persyn-0.1.2/src/persyn/dreams/stylegan2/training/training_loop.py`

 * *Files identical despite different names*

### Comparing `persyn-0.1.1.dev0/src/persyn/interaction/chrono.py` & `persyn-0.1.2/src/persyn/interaction/chrono.py`

 * *Files identical despite different names*

### Comparing `persyn-0.1.1.dev0/src/persyn/interaction/cns.py` & `persyn-0.1.2/src/persyn/interaction/cns.py`

 * *Files identical despite different names*

### Comparing `persyn-0.1.1.dev0/src/persyn/interaction/completion.py` & `persyn-0.1.2/src/persyn/interaction/completion.py`

 * *Files identical despite different names*

### Comparing `persyn-0.1.1.dev0/src/persyn/interaction/feels.py` & `persyn-0.1.2/src/persyn/interaction/feels.py`

 * *Files identical despite different names*

### Comparing `persyn-0.1.1.dev0/src/persyn/interaction/gpt.py` & `persyn-0.1.2/src/persyn/interaction/gpt.py`

 * *Files identical despite different names*

### Comparing `persyn-0.1.1.dev0/src/persyn/interaction/graph.py` & `persyn-0.1.2/src/persyn/interaction/graph.py`

 * *Files identical despite different names*

### Comparing `persyn-0.1.1.dev0/src/persyn/interaction/interact.py` & `persyn-0.1.2/src/persyn/interaction/interact.py`

 * *Files identical despite different names*

### Comparing `persyn-0.1.1.dev0/src/persyn/interaction/interact_server.py` & `persyn-0.1.2/src/persyn/interaction/interact_server.py`

 * *Files identical despite different names*

### Comparing `persyn-0.1.1.dev0/src/persyn/interaction/memory.py` & `persyn-0.1.2/src/persyn/interaction/memory.py`

 * *Files identical despite different names*

### Comparing `persyn-0.1.1.dev0/src/persyn/interaction/messages.py` & `persyn-0.1.2/src/persyn/interaction/messages.py`

 * *Files identical despite different names*

### Comparing `persyn-0.1.1.dev0/src/persyn/interaction/nlp_cloud.py` & `persyn-0.1.2/src/persyn/interaction/nlp_cloud.py`

 * *Files identical despite different names*

### Comparing `persyn-0.1.1.dev0/src/persyn/interaction/notebooks/env/bin/activate_this.py` & `persyn-0.1.2/src/persyn/interaction/notebooks/env/bin/activate_this.py`

 * *Files identical despite different names*

### Comparing `persyn-0.1.1.dev0/src/persyn/interaction/notebooks/env/bin/jp.py` & `persyn-0.1.2/src/persyn/interaction/notebooks/env/bin/jp.py`

 * *Files identical despite different names*

### Comparing `persyn-0.1.1.dev0/src/persyn/interaction/relationships.py` & `persyn-0.1.2/src/persyn/interaction/relationships.py`

 * *Files identical despite different names*

### Comparing `persyn-0.1.1.dev0/src/persyn/interaction/reminders.py` & `persyn-0.1.2/src/persyn/interaction/reminders.py`

 * *Files identical despite different names*

### Comparing `persyn-0.1.1.dev0/src/persyn/interaction/voice.py` & `persyn-0.1.2/src/persyn/interaction/voice.py`

 * *Files identical despite different names*

### Comparing `persyn-0.1.1.dev0/src/persyn/kill_bot.py` & `persyn-0.1.2/src/persyn/kill_bot.py`

 * *Files identical despite different names*

### Comparing `persyn-0.1.1.dev0/src/persyn/launch_bot.py` & `persyn-0.1.2/src/persyn/launch_bot.py`

 * *Files identical despite different names*

### Comparing `persyn-0.1.1.dev0/src/persyn/utils/art.py` & `persyn-0.1.2/src/persyn/utils/art.py`

 * *Files identical despite different names*

### Comparing `persyn-0.1.1.dev0/src/persyn/utils/color_logging.py` & `persyn-0.1.2/src/persyn/utils/color_logging.py`

 * *Files identical despite different names*

### Comparing `persyn-0.1.1.dev0/src/persyn/utils/config.py` & `persyn-0.1.2/src/persyn/utils/config.py`

 * *Files identical despite different names*

### Comparing `persyn-0.1.1.dev0/src/persyn.egg-info/PKG-INFO` & `persyn-0.1.2/src/persyn.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: persyn
-Version: 0.1.1.dev0
+Version: 0.1.2
 Summary: Personality Syndrome. Persyn for short.
 Author-email: Rob Flickenger <rob@hackerfriendly.com>
 Project-URL: Homepage, https://persyn.io
 Project-URL: Bug Tracker, https://github.com/hackerfriendly/persyn/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `persyn-0.1.1.dev0/src/persyn.egg-info/SOURCES.txt` & `persyn-0.1.2/src/persyn.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `persyn-0.1.1.dev0/src/persyn.egg-info/entry_points.txt` & `persyn-0.1.2/src/persyn.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `persyn-0.1.1.dev0/src/persyn.egg-info/requires.txt` & `persyn-0.1.2/src/persyn.egg-info/requires.txt`

 * *Files identical despite different names*

