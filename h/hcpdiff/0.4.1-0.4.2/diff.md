# Comparing `tmp/hcpdiff-0.4.1.tar.gz` & `tmp/hcpdiff-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hcpdiff-0.4.1.tar", last modified: Fri May 12 02:13:55 2023, max compression
+gzip compressed data, was "hcpdiff-0.4.2.tar", last modified: Mon May 22 06:07:04 2023, max compression
```

## Comparing `hcpdiff-0.4.1.tar` & `hcpdiff-0.4.2.tar`

### file list

```diff
@@ -1,110 +1,110 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 02:13:55.566715 hcpdiff-0.4.1/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-12 02:13:42.000000 hcpdiff-0.4.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5767 2023-05-12 02:13:55.566715 hcpdiff-0.4.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5050 2023-05-12 02:13:42.000000 hcpdiff-0.4.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 02:13:55.546715 hcpdiff-0.4.1/cfgs/
--rw-r--r--   0 runner    (1001) docker     (123)      777 2023-05-12 02:13:42.000000 hcpdiff-0.4.1/cfgs/deepspeed.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 02:13:55.550715 hcpdiff-0.4.1/cfgs/infer/
--rw-r--r--   0 runner    (1001) docker     (123)      174 2023-05-12 02:13:42.000000 hcpdiff-0.4.1/cfgs/infer/change_vae.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      646 2023-05-12 02:13:42.000000 hcpdiff-0.4.1/cfgs/infer/euler_a.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1608 2023-05-12 02:13:42.000000 hcpdiff-0.4.1/cfgs/infer/img2img.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      960 2023-05-12 02:13:42.000000 hcpdiff-0.4.1/cfgs/infer/img2img_controlnet.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1216 2023-05-12 02:13:42.000000 hcpdiff-0.4.1/cfgs/infer/text2img.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1542 2023-05-12 02:13:42.000000 hcpdiff-0.4.1/cfgs/infer/text2img_DA++.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1330 2023-05-12 02:13:42.000000 hcpdiff-0.4.1/cfgs/infer/webui_model_infer.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 02:13:55.550715 hcpdiff-0.4.1/cfgs/plugins/
--rw-r--r--   0 runner    (1001) docker     (123)      426 2023-05-12 02:13:42.000000 hcpdiff-0.4.1/cfgs/plugins/plugin_controlnet.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     9778 2023-05-12 02:13:42.000000 hcpdiff-0.4.1/cfgs/te_struct.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 02:13:55.550715 hcpdiff-0.4.1/cfgs/train/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 02:13:55.550715 hcpdiff-0.4.1/cfgs/train/examples/
--rw-r--r--   0 runner    (1001) docker     (123)     2412 2023-05-12 02:13:42.000000 hcpdiff-0.4.1/cfgs/train/examples/CustomDiffusion.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     3667 2023-05-12 02:13:42.000000 hcpdiff-0.4.1/cfgs/train/examples/DreamArtist++.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1431 2023-05-12 02:13:42.000000 hcpdiff-0.4.1/cfgs/train/examples/DreamArtist.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2219 2023-05-12 02:13:42.000000 hcpdiff-0.4.1/cfgs/train/examples/DreamBooth.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      361 2023-05-12 02:13:42.000000 hcpdiff-0.4.1/cfgs/train/examples/Lion_optimizer.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1224 2023-05-12 02:13:42.000000 hcpdiff-0.4.1/cfgs/train/examples/TextualInversion.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-05-12 02:13:42.000000 hcpdiff-0.4.1/cfgs/train/examples/controlnet.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1263 2023-05-12 02:13:42.000000 hcpdiff-0.4.1/cfgs/train/examples/fine-tuning.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1463 2023-05-12 02:13:42.000000 hcpdiff-0.4.1/cfgs/train/examples/locon.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1302 2023-05-12 02:13:42.000000 hcpdiff-0.4.1/cfgs/train/examples/lora_conventional.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      149 2023-05-12 02:13:42.000000 hcpdiff-0.4.1/cfgs/train/examples/min_snr.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2959 2023-05-12 02:13:42.000000 hcpdiff-0.4.1/cfgs/train/train_base.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      984 2023-05-12 02:13:42.000000 hcpdiff-0.4.1/cfgs/train/tuning_base.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    45190 2023-05-12 02:13:42.000000 hcpdiff-0.4.1/cfgs/unet_struct.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 02:13:55.554715 hcpdiff-0.4.1/hcpdiff/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 02:13:42.000000 hcpdiff-0.4.1/hcpdiff/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 02:13:55.554715 hcpdiff-0.4.1/hcpdiff/ckpt_manager/
--rw-r--r--   0 runner    (1001) docker     (123)      200 2023-05-12 02:13:42.000000 hcpdiff-0.4.1/hcpdiff/ckpt_manager/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4173 2023-05-12 02:13:42.000000 hcpdiff-0.4.1/hcpdiff/ckpt_manager/ckpt_pkl.py
--rw-r--r--   0 runner    (1001) docker     (123)     1835 2023-05-12 02:13:42.000000 hcpdiff-0.4.1/hcpdiff/ckpt_manager/ckpt_safetensor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 02:13:55.558715 hcpdiff-0.4.1/hcpdiff/data/
--rw-r--r--   0 runner    (1001) docker     (123)      795 2023-05-12 02:13:42.000000 hcpdiff-0.4.1/hcpdiff/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8566 2023-05-12 02:13:42.000000 hcpdiff-0.4.1/hcpdiff/data/bucket.py
--rw-r--r--   0 runner    (1001) docker     (123)     2214 2023-05-12 02:13:42.000000 hcpdiff-0.4.1/hcpdiff/data/cond_pair_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     6104 2023-05-12 02:13:42.000000 hcpdiff-0.4.1/hcpdiff/data/pair_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     2827 2023-05-12 02:13:42.000000 hcpdiff-0.4.1/hcpdiff/data/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 02:13:55.558715 hcpdiff-0.4.1/hcpdiff/loggers/
--rw-r--r--   0 runner    (1001) docker     (123)      275 2023-05-12 02:13:42.000000 hcpdiff-0.4.1/hcpdiff/loggers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1845 2023-05-12 02:13:42.000000 hcpdiff-0.4.1/hcpdiff/loggers/base_logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     1276 2023-05-12 02:13:42.000000 hcpdiff-0.4.1/hcpdiff/loggers/cli_logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     1034 2023-05-12 02:13:42.000000 hcpdiff-0.4.1/hcpdiff/loggers/tensorboard_logger.py
--rw-r--r--   0 runner    (1001) docker     (123)      803 2023-05-12 02:13:42.000000 hcpdiff-0.4.1/hcpdiff/loggers/wandb_logger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 02:13:55.558715 hcpdiff-0.4.1/hcpdiff/loss/
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-05-12 02:13:42.000000 hcpdiff-0.4.1/hcpdiff/loss/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1011 2023-05-12 02:13:42.000000 hcpdiff-0.4.1/hcpdiff/loss/min_snr_loss.py
--rw-r--r--   0 runner    (1001) docker     (123)      378 2023-05-12 02:13:42.000000 hcpdiff-0.4.1/hcpdiff/loss/mse_loss.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 02:13:55.558715 hcpdiff-0.4.1/hcpdiff/models/
--rw-r--r--   0 runner    (1001) docker     (123)      290 2023-05-12 02:13:42.000000 hcpdiff-0.4.1/hcpdiff/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1384 2023-05-12 02:13:42.000000 hcpdiff-0.4.1/hcpdiff/models/cfg_context.py
--rw-r--r--   0 runner    (1001) docker     (123)     7744 2023-05-12 02:13:42.000000 hcpdiff-0.4.1/hcpdiff/models/controlnet.py
--rw-r--r--   0 runner    (1001) docker     (123)     2991 2023-05-12 02:13:42.000000 hcpdiff-0.4.1/hcpdiff/models/layers.py
--rw-r--r--   0 runner    (1001) docker     (123)     6675 2023-05-12 02:13:42.000000 hcpdiff-0.4.1/hcpdiff/models/lora_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     7832 2023-05-12 02:13:42.000000 hcpdiff-0.4.1/hcpdiff/models/lora_layers.py
--rw-r--r--   0 runner    (1001) docker     (123)     8754 2023-05-12 02:13:42.000000 hcpdiff-0.4.1/hcpdiff/models/plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)     3831 2023-05-12 02:13:42.000000 hcpdiff-0.4.1/hcpdiff/models/text_emb_ex.py
--rw-r--r--   0 runner    (1001) docker     (123)     5674 2023-05-12 02:13:42.000000 hcpdiff-0.4.1/hcpdiff/models/textencoder_ex.py
--rw-r--r--   0 runner    (1001) docker     (123)     2365 2023-05-12 02:13:42.000000 hcpdiff-0.4.1/hcpdiff/models/tokenizer_ex.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 02:13:55.562715 hcpdiff-0.4.1/hcpdiff/noise/
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-05-12 02:13:42.000000 hcpdiff-0.4.1/hcpdiff/noise/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      388 2023-05-12 02:13:42.000000 hcpdiff-0.4.1/hcpdiff/noise/noise_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1766 2023-05-12 02:13:42.000000 hcpdiff-0.4.1/hcpdiff/noise/pyramid_noise.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 02:13:55.562715 hcpdiff-0.4.1/hcpdiff/tools/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 02:13:42.000000 hcpdiff-0.4.1/hcpdiff/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      955 2023-05-12 02:13:42.000000 hcpdiff-0.4.1/hcpdiff/tools/convert_caption_txt2json.py
--rw-r--r--   0 runner    (1001) docker     (123)     1870 2023-05-12 02:13:42.000000 hcpdiff-0.4.1/hcpdiff/tools/create_embedding.py
--rw-r--r--   0 runner    (1001) docker     (123)     1691 2023-05-12 02:13:42.000000 hcpdiff-0.4.1/hcpdiff/tools/gen_from_ptlist.py
--rw-r--r--   0 runner    (1001) docker     (123)      756 2023-05-12 02:13:42.000000 hcpdiff-0.4.1/hcpdiff/tools/init_proj.py
--rw-r--r--   0 runner    (1001) docker     (123)     4234 2023-05-12 02:13:42.000000 hcpdiff-0.4.1/hcpdiff/tools/lora_convert.py
--rw-r--r--   0 runner    (1001) docker     (123)    15204 2023-05-12 02:13:42.000000 hcpdiff-0.4.1/hcpdiff/tools/sd2diffusers.py
--rw-r--r--   0 runner    (1001) docker     (123)    27934 2023-05-12 02:13:42.000000 hcpdiff-0.4.1/hcpdiff/train_ac.py
--rw-r--r--   0 runner    (1001) docker     (123)     4547 2023-05-12 02:13:42.000000 hcpdiff-0.4.1/hcpdiff/train_ac_single.py
--rw-r--r--   0 runner    (1001) docker     (123)     9319 2023-05-12 02:13:42.000000 hcpdiff-0.4.1/hcpdiff/train_colo.py
--rw-r--r--   0 runner    (1001) docker     (123)     3804 2023-05-12 02:13:42.000000 hcpdiff-0.4.1/hcpdiff/train_deepspeed.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 02:13:55.566715 hcpdiff-0.4.1/hcpdiff/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 02:13:42.000000 hcpdiff-0.4.1/hcpdiff/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2778 2023-05-12 02:13:42.000000 hcpdiff-0.4.1/hcpdiff/utils/caption_tools.py
--rw-r--r--   0 runner    (1001) docker     (123)    12964 2023-05-12 02:13:42.000000 hcpdiff-0.4.1/hcpdiff/utils/cfg_net_tools.py
--rw-r--r--   0 runner    (1001) docker     (123)      837 2023-05-12 02:13:42.000000 hcpdiff-0.4.1/hcpdiff/utils/colo_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2993 2023-05-12 02:13:42.000000 hcpdiff-0.4.1/hcpdiff/utils/ema.py
--rw-r--r--   0 runner    (1001) docker     (123)     8433 2023-05-12 02:13:42.000000 hcpdiff-0.4.1/hcpdiff/utils/img_size_tool.py
--rw-r--r--   0 runner    (1001) docker     (123)     7029 2023-05-12 02:13:42.000000 hcpdiff-0.4.1/hcpdiff/utils/net_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2804 2023-05-12 02:13:42.000000 hcpdiff-0.4.1/hcpdiff/utils/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     7548 2023-05-12 02:13:42.000000 hcpdiff-0.4.1/hcpdiff/visualizer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 02:13:55.554715 hcpdiff-0.4.1/hcpdiff.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5767 2023-05-12 02:13:55.000000 hcpdiff-0.4.1/hcpdiff.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2708 2023-05-12 02:13:55.000000 hcpdiff-0.4.1/hcpdiff.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-12 02:13:55.000000 hcpdiff-0.4.1/hcpdiff.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-05-12 02:13:55.000000 hcpdiff-0.4.1/hcpdiff.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      225 2023-05-12 02:13:55.000000 hcpdiff-0.4.1/hcpdiff.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-12 02:13:55.000000 hcpdiff-0.4.1/hcpdiff.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 02:13:55.566715 hcpdiff-0.4.1/prompt_tuning_template/
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-12 02:13:42.000000 hcpdiff-0.4.1/prompt_tuning_template/caption.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-12 02:13:42.000000 hcpdiff-0.4.1/prompt_tuning_template/name.txt
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-12 02:13:42.000000 hcpdiff-0.4.1/prompt_tuning_template/name_2pt_caption.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-12 02:13:42.000000 hcpdiff-0.4.1/prompt_tuning_template/name_caption.txt
--rw-r--r--   0 runner    (1001) docker     (123)      889 2023-05-12 02:13:42.000000 hcpdiff-0.4.1/prompt_tuning_template/object.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1186 2023-05-12 02:13:42.000000 hcpdiff-0.4.1/prompt_tuning_template/object_caption.txt
--rw-r--r--   0 runner    (1001) docker     (123)      872 2023-05-12 02:13:42.000000 hcpdiff-0.4.1/prompt_tuning_template/style.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-05-12 02:13:42.000000 hcpdiff-0.4.1/prompt_tuning_template/style_caption.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-12 02:13:55.566715 hcpdiff-0.4.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1775 2023-05-12 02:13:42.000000 hcpdiff-0.4.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 06:07:04.677458 hcpdiff-0.4.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-22 06:06:40.000000 hcpdiff-0.4.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5767 2023-05-22 06:07:04.677458 hcpdiff-0.4.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5050 2023-05-22 06:06:40.000000 hcpdiff-0.4.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 06:07:04.665458 hcpdiff-0.4.2/cfgs/
+-rw-r--r--   0 runner    (1001) docker     (123)      777 2023-05-22 06:06:40.000000 hcpdiff-0.4.2/cfgs/deepspeed.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 06:07:04.669458 hcpdiff-0.4.2/cfgs/infer/
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-05-22 06:06:40.000000 hcpdiff-0.4.2/cfgs/infer/change_vae.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      216 2023-05-22 06:06:40.000000 hcpdiff-0.4.2/cfgs/infer/euler_a.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-05-22 06:06:40.000000 hcpdiff-0.4.2/cfgs/infer/img2img.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      369 2023-05-22 06:06:40.000000 hcpdiff-0.4.2/cfgs/infer/img2img_controlnet.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-05-22 06:06:40.000000 hcpdiff-0.4.2/cfgs/infer/offload_2GB.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      759 2023-05-22 06:06:40.000000 hcpdiff-0.4.2/cfgs/infer/text2img.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      900 2023-05-22 06:06:40.000000 hcpdiff-0.4.2/cfgs/infer/text2img_DA++.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 06:07:04.669458 hcpdiff-0.4.2/cfgs/plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)      426 2023-05-22 06:06:40.000000 hcpdiff-0.4.2/cfgs/plugins/plugin_controlnet.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     9778 2023-05-22 06:06:40.000000 hcpdiff-0.4.2/cfgs/te_struct.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 06:07:04.669458 hcpdiff-0.4.2/cfgs/train/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 06:07:04.669458 hcpdiff-0.4.2/cfgs/train/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)     2412 2023-05-22 06:06:40.000000 hcpdiff-0.4.2/cfgs/train/examples/CustomDiffusion.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3667 2023-05-22 06:06:40.000000 hcpdiff-0.4.2/cfgs/train/examples/DreamArtist++.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1431 2023-05-22 06:06:40.000000 hcpdiff-0.4.2/cfgs/train/examples/DreamArtist.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2219 2023-05-22 06:06:40.000000 hcpdiff-0.4.2/cfgs/train/examples/DreamBooth.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      361 2023-05-22 06:06:40.000000 hcpdiff-0.4.2/cfgs/train/examples/Lion_optimizer.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1224 2023-05-22 06:06:40.000000 hcpdiff-0.4.2/cfgs/train/examples/TextualInversion.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-05-22 06:06:40.000000 hcpdiff-0.4.2/cfgs/train/examples/controlnet.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1263 2023-05-22 06:06:40.000000 hcpdiff-0.4.2/cfgs/train/examples/fine-tuning.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1463 2023-05-22 06:06:40.000000 hcpdiff-0.4.2/cfgs/train/examples/locon.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1302 2023-05-22 06:06:40.000000 hcpdiff-0.4.2/cfgs/train/examples/lora_conventional.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-05-22 06:06:40.000000 hcpdiff-0.4.2/cfgs/train/examples/min_snr.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2959 2023-05-22 06:06:40.000000 hcpdiff-0.4.2/cfgs/train/train_base.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      984 2023-05-22 06:06:40.000000 hcpdiff-0.4.2/cfgs/train/tuning_base.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    45190 2023-05-22 06:06:40.000000 hcpdiff-0.4.2/cfgs/unet_struct.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 06:07:04.669458 hcpdiff-0.4.2/hcpdiff/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 06:06:40.000000 hcpdiff-0.4.2/hcpdiff/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 06:07:04.673458 hcpdiff-0.4.2/hcpdiff/ckpt_manager/
+-rw-r--r--   0 runner    (1001) docker     (123)      200 2023-05-22 06:06:40.000000 hcpdiff-0.4.2/hcpdiff/ckpt_manager/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4173 2023-05-22 06:06:40.000000 hcpdiff-0.4.2/hcpdiff/ckpt_manager/ckpt_pkl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1835 2023-05-22 06:06:40.000000 hcpdiff-0.4.2/hcpdiff/ckpt_manager/ckpt_safetensor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 06:07:04.673458 hcpdiff-0.4.2/hcpdiff/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      780 2023-05-22 06:06:40.000000 hcpdiff-0.4.2/hcpdiff/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8761 2023-05-22 06:06:40.000000 hcpdiff-0.4.2/hcpdiff/data/bucket.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2024 2023-05-22 06:06:40.000000 hcpdiff-0.4.2/hcpdiff/data/cond_pair_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7132 2023-05-22 06:06:40.000000 hcpdiff-0.4.2/hcpdiff/data/pair_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2018 2023-05-22 06:06:40.000000 hcpdiff-0.4.2/hcpdiff/data/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 06:07:04.673458 hcpdiff-0.4.2/hcpdiff/loggers/
+-rw-r--r--   0 runner    (1001) docker     (123)      275 2023-05-22 06:06:40.000000 hcpdiff-0.4.2/hcpdiff/loggers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1845 2023-05-22 06:06:40.000000 hcpdiff-0.4.2/hcpdiff/loggers/base_logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1276 2023-05-22 06:06:40.000000 hcpdiff-0.4.2/hcpdiff/loggers/cli_logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1034 2023-05-22 06:06:40.000000 hcpdiff-0.4.2/hcpdiff/loggers/tensorboard_logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)      803 2023-05-22 06:06:40.000000 hcpdiff-0.4.2/hcpdiff/loggers/wandb_logger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 06:07:04.673458 hcpdiff-0.4.2/hcpdiff/loss/
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-05-22 06:06:40.000000 hcpdiff-0.4.2/hcpdiff/loss/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1011 2023-05-22 06:06:40.000000 hcpdiff-0.4.2/hcpdiff/loss/min_snr_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)      378 2023-05-22 06:06:40.000000 hcpdiff-0.4.2/hcpdiff/loss/mse_loss.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 06:07:04.673458 hcpdiff-0.4.2/hcpdiff/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      307 2023-05-22 06:06:40.000000 hcpdiff-0.4.2/hcpdiff/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1384 2023-05-22 06:06:40.000000 hcpdiff-0.4.2/hcpdiff/models/cfg_context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7744 2023-05-22 06:06:40.000000 hcpdiff-0.4.2/hcpdiff/models/controlnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2991 2023-05-22 06:06:40.000000 hcpdiff-0.4.2/hcpdiff/models/layers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6697 2023-05-22 06:06:40.000000 hcpdiff-0.4.2/hcpdiff/models/lora_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7854 2023-05-22 06:06:40.000000 hcpdiff-0.4.2/hcpdiff/models/lora_layers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9923 2023-05-22 06:06:40.000000 hcpdiff-0.4.2/hcpdiff/models/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3831 2023-05-22 06:06:40.000000 hcpdiff-0.4.2/hcpdiff/models/text_emb_ex.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5701 2023-05-22 06:06:40.000000 hcpdiff-0.4.2/hcpdiff/models/textencoder_ex.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2365 2023-05-22 06:06:40.000000 hcpdiff-0.4.2/hcpdiff/models/tokenizer_ex.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 06:07:04.673458 hcpdiff-0.4.2/hcpdiff/noise/
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-05-22 06:06:40.000000 hcpdiff-0.4.2/hcpdiff/noise/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      574 2023-05-22 06:06:40.000000 hcpdiff-0.4.2/hcpdiff/noise/noise_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1751 2023-05-22 06:06:40.000000 hcpdiff-0.4.2/hcpdiff/noise/pyramid_noise.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 06:07:04.677458 hcpdiff-0.4.2/hcpdiff/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 06:06:40.000000 hcpdiff-0.4.2/hcpdiff/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      955 2023-05-22 06:06:40.000000 hcpdiff-0.4.2/hcpdiff/tools/convert_caption_txt2json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1870 2023-05-22 06:06:40.000000 hcpdiff-0.4.2/hcpdiff/tools/create_embedding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1928 2023-05-22 06:06:40.000000 hcpdiff-0.4.2/hcpdiff/tools/gen_from_ptlist.py
+-rw-r--r--   0 runner    (1001) docker     (123)      756 2023-05-22 06:06:40.000000 hcpdiff-0.4.2/hcpdiff/tools/init_proj.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4484 2023-05-22 06:06:40.000000 hcpdiff-0.4.2/hcpdiff/tools/lora_convert.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15204 2023-05-22 06:06:40.000000 hcpdiff-0.4.2/hcpdiff/tools/sd2diffusers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28412 2023-05-22 06:06:40.000000 hcpdiff-0.4.2/hcpdiff/train_ac.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4558 2023-05-22 06:06:40.000000 hcpdiff-0.4.2/hcpdiff/train_ac_single.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9319 2023-05-22 06:06:40.000000 hcpdiff-0.4.2/hcpdiff/train_colo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3712 2023-05-22 06:06:40.000000 hcpdiff-0.4.2/hcpdiff/train_deepspeed.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 06:07:04.677458 hcpdiff-0.4.2/hcpdiff/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 06:06:40.000000 hcpdiff-0.4.2/hcpdiff/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2778 2023-05-22 06:06:40.000000 hcpdiff-0.4.2/hcpdiff/utils/caption_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13777 2023-05-22 06:06:40.000000 hcpdiff-0.4.2/hcpdiff/utils/cfg_net_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)      837 2023-05-22 06:06:40.000000 hcpdiff-0.4.2/hcpdiff/utils/colo_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2993 2023-05-22 06:06:40.000000 hcpdiff-0.4.2/hcpdiff/utils/ema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8433 2023-05-22 06:06:40.000000 hcpdiff-0.4.2/hcpdiff/utils/img_size_tool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7303 2023-05-22 06:06:40.000000 hcpdiff-0.4.2/hcpdiff/utils/net_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3086 2023-05-22 06:06:40.000000 hcpdiff-0.4.2/hcpdiff/utils/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10570 2023-05-22 06:06:40.000000 hcpdiff-0.4.2/hcpdiff/visualizer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 06:07:04.673458 hcpdiff-0.4.2/hcpdiff.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5767 2023-05-22 06:07:04.000000 hcpdiff-0.4.2/hcpdiff.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2702 2023-05-22 06:07:04.000000 hcpdiff-0.4.2/hcpdiff.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 06:07:04.000000 hcpdiff-0.4.2/hcpdiff.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-05-22 06:07:04.000000 hcpdiff-0.4.2/hcpdiff.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      259 2023-05-22 06:07:04.000000 hcpdiff-0.4.2/hcpdiff.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-22 06:07:04.000000 hcpdiff-0.4.2/hcpdiff.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 06:07:04.677458 hcpdiff-0.4.2/prompt_tuning_template/
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-22 06:06:40.000000 hcpdiff-0.4.2/prompt_tuning_template/caption.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-22 06:06:40.000000 hcpdiff-0.4.2/prompt_tuning_template/name.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-22 06:06:40.000000 hcpdiff-0.4.2/prompt_tuning_template/name_2pt_caption.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-22 06:06:40.000000 hcpdiff-0.4.2/prompt_tuning_template/name_caption.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      889 2023-05-22 06:06:40.000000 hcpdiff-0.4.2/prompt_tuning_template/object.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1186 2023-05-22 06:06:40.000000 hcpdiff-0.4.2/prompt_tuning_template/object_caption.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      872 2023-05-22 06:06:40.000000 hcpdiff-0.4.2/prompt_tuning_template/style.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-05-22 06:06:40.000000 hcpdiff-0.4.2/prompt_tuning_template/style_caption.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-22 06:07:04.677458 hcpdiff-0.4.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1775 2023-05-22 06:06:40.000000 hcpdiff-0.4.2/setup.py
```

### Comparing `hcpdiff-0.4.1/LICENSE` & `hcpdiff-0.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `hcpdiff-0.4.1/PKG-INFO` & `hcpdiff-0.4.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hcpdiff
-Version: 0.4.1
+Version: 0.4.2
 Summary: A universal Stable-Diffusion toolbox
 Home-page: https://github.com/7eu7d7/HCP-Diffusion
 Author: Ziyi Dong
 Author-email: dzy7eu7d7@gmail.com
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
```

### Comparing `hcpdiff-0.4.1/README.md` & `hcpdiff-0.4.2/README.md`

 * *Files identical despite different names*

### Comparing `hcpdiff-0.4.1/cfgs/deepspeed.json` & `hcpdiff-0.4.2/cfgs/deepspeed.json`

 * *Files identical despite different names*

### Comparing `hcpdiff-0.4.1/cfgs/te_struct.txt` & `hcpdiff-0.4.2/cfgs/te_struct.txt`

 * *Files identical despite different names*

### Comparing `hcpdiff-0.4.1/cfgs/train/examples/CustomDiffusion.yaml` & `hcpdiff-0.4.2/cfgs/train/examples/CustomDiffusion.yaml`

 * *Files identical despite different names*

### Comparing `hcpdiff-0.4.1/cfgs/train/examples/DreamArtist++.yaml` & `hcpdiff-0.4.2/cfgs/train/examples/DreamArtist++.yaml`

 * *Files identical despite different names*

### Comparing `hcpdiff-0.4.1/cfgs/train/examples/DreamArtist.yaml` & `hcpdiff-0.4.2/cfgs/train/examples/DreamArtist.yaml`

 * *Files identical despite different names*

### Comparing `hcpdiff-0.4.1/cfgs/train/examples/DreamBooth.yaml` & `hcpdiff-0.4.2/cfgs/train/examples/DreamBooth.yaml`

 * *Files identical despite different names*

### Comparing `hcpdiff-0.4.1/cfgs/train/examples/TextualInversion.yaml` & `hcpdiff-0.4.2/cfgs/train/examples/TextualInversion.yaml`

 * *Files identical despite different names*

### Comparing `hcpdiff-0.4.1/cfgs/train/examples/controlnet.yaml` & `hcpdiff-0.4.2/cfgs/train/examples/controlnet.yaml`

 * *Files identical despite different names*

### Comparing `hcpdiff-0.4.1/cfgs/train/examples/fine-tuning.yaml` & `hcpdiff-0.4.2/cfgs/train/examples/fine-tuning.yaml`

 * *Files identical despite different names*

### Comparing `hcpdiff-0.4.1/cfgs/train/examples/locon.yaml` & `hcpdiff-0.4.2/cfgs/train/examples/locon.yaml`

 * *Files identical despite different names*

### Comparing `hcpdiff-0.4.1/cfgs/train/examples/lora_conventional.yaml` & `hcpdiff-0.4.2/cfgs/train/examples/lora_conventional.yaml`

 * *Files identical despite different names*

### Comparing `hcpdiff-0.4.1/cfgs/train/train_base.yaml` & `hcpdiff-0.4.2/cfgs/train/train_base.yaml`

 * *Files identical despite different names*

### Comparing `hcpdiff-0.4.1/cfgs/train/tuning_base.yaml` & `hcpdiff-0.4.2/cfgs/train/tuning_base.yaml`

 * *Files identical despite different names*

### Comparing `hcpdiff-0.4.1/cfgs/unet_struct.txt` & `hcpdiff-0.4.2/cfgs/unet_struct.txt`

 * *Files identical despite different names*

### Comparing `hcpdiff-0.4.1/hcpdiff/ckpt_manager/ckpt_pkl.py` & `hcpdiff-0.4.2/hcpdiff/ckpt_manager/ckpt_pkl.py`

 * *Files identical despite different names*

### Comparing `hcpdiff-0.4.1/hcpdiff/ckpt_manager/ckpt_safetensor.py` & `hcpdiff-0.4.2/hcpdiff/ckpt_manager/ckpt_safetensor.py`

 * *Files identical despite different names*

### Comparing `hcpdiff-0.4.1/hcpdiff/data/__init__.py` & `hcpdiff-0.4.2/hcpdiff/data/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from .pair_dataset import TextImagePairDataset
 from .cond_pair_dataset import TextImageCondPairDataset
 from .bucket import BaseBucket, FixedBucket, RatioBucket
-from .utils import collate_fn_ft, CycleData
+from .utils import CycleData
 
 
 class DataGroup:
     def __init__(self, loader_list, loss_weights):
         self.loader_list = loader_list
         self.loss_weights = loss_weights
```

### Comparing `hcpdiff-0.4.1/hcpdiff/data/bucket.py` & `hcpdiff-0.4.2/hcpdiff/data/bucket.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,222 +4,223 @@
     :Name:        aspect ratio bucket with k-means
     :Author:      Dong Ziyi
     :Affiliation: HCP Lab, SYSU
     :Created:     10/03/2023
     :Licence:     Apache-2.0
 """
 
-from typing import List, Tuple, Union
+import math
 import os.path
 import pickle
+from typing import List, Tuple, Union
 
+import cv2
 import numpy as np
-import math
+from loguru import logger
 from sklearn.cluster import KMeans
+
 from hcpdiff.utils.img_size_tool import types_support, get_image_size
-from .utils import resize_crop_fix
 from hcpdiff.utils.utils import get_file_ext
-
-from loguru import logger
+from .utils import resize_crop_fix
 
 class BaseBucket:
     def __getitem__(self, idx):
         '''
         :return: (file name of image), (target image size)
         '''
         raise NotImplementedError()
 
     def __len__(self):
         raise NotImplementedError()
 
-    def build(self, bs:int, img_root_list:List[str]):
+    def build(self, bs: int, img_root_list: List[str]):
         raise NotImplementedError()
 
     def rest(self, epoch):
         pass
 
-    def crop_resize(self, image, size):
+    def crop_resize(self, image, size, mask_interp=cv2.INTER_CUBIC):
         return image
 
 class FixedBucket(BaseBucket):
-    def __init__(self, target_size:Union[Tuple[int,int], int]=512):
-        self.target_size=(target_size, target_size) if isinstance(target_size, int) else target_size
+    def __init__(self, target_size: Union[Tuple[int, int], int] = 512):
+        self.target_size = (target_size, target_size) if isinstance(target_size, int) else target_size
 
-    def build(self, bs:int, img_root_list:List[str]):
+    def build(self, bs: int, img_root_list: List[str]):
         self.img_root_list = img_root_list
-        self.file_names=[os.path.join(img_root, x) for img_root in img_root_list for x in os.listdir(img_root) if get_file_ext(x) in types_support]
+        self.file_names = [os.path.join(img_root, x) for img_root in img_root_list for x in os.listdir(img_root) if get_file_ext(x) in types_support]
 
-    def crop_resize(self, image, size):
-        return resize_crop_fix(image, size)
+    def crop_resize(self, image, size, mask_interp=cv2.INTER_CUBIC):
+        return resize_crop_fix(image, size, mask_interp=mask_interp)
 
     def __getitem__(self, idx) -> Tuple[str, Tuple[int, int]]:
         return self.file_names[idx], self.target_size
 
     def __len__(self):
         return len(self.file_names)
 
 class RatioBucket(BaseBucket):
-    def __init__(self, taget_area:int=640*640, step_size:int=8, num_bucket:int=10, pre_build_arb:str=None):
-        self.taget_area=taget_area
-        self.step_size=step_size
-        self.num_bucket=num_bucket
-        self.pre_build_arb=pre_build_arb
+    def __init__(self, taget_area: int = 640*640, step_size: int = 8, num_bucket: int = 10, pre_build_arb: str = None):
+        self.taget_area = taget_area
+        self.step_size = step_size
+        self.num_bucket = num_bucket
+        self.pre_build_arb = pre_build_arb
 
     def load_arb(self, path):
         with open(path, 'rb') as f:
             data = pickle.load(f)
-        self.buckets=data['buckets']
-        self.size_buckets=data['size_buckets']
-        self.file_names=data['file_names']
-        self.idx_bucket_map=data['idx_bucket_map']
+        self.buckets = data['buckets']
+        self.size_buckets = data['size_buckets']
+        self.file_names = data['file_names']
+        self.idx_bucket_map = data['idx_bucket_map']
         self.data_len = data['data_len']
 
     def save_arb(self, path):
         with open(path, 'wb') as f:
             pickle.dump({
-                'buckets': self.buckets,
-                'size_buckets': self.size_buckets,
-                'idx_bucket_map': self.idx_bucket_map,
-                'file_names': self.file_names,
-                'data_len': self.data_len,
+                'buckets':self.buckets,
+                'size_buckets':self.size_buckets,
+                'idx_bucket_map':self.idx_bucket_map,
+                'file_names':self.file_names,
+                'data_len':self.data_len,
             }, f)
 
     def build_buckets_from_ratios(self):
         logger.info('build buckets from ratios')
-        size_low = int(math.sqrt(self.taget_area / self.ratio_max))
+        size_low = int(math.sqrt(self.taget_area/self.ratio_max))
         size_high = int(self.ratio_max*size_low)
 
         # SD需要边长是8的倍数
         size_low = (size_low//self.step_size)*self.step_size
         size_high = (size_high//self.step_size)*self.step_size
 
         data = []
-        for w in range(size_low, size_high + 1, self.step_size):
-            for h in range(size_low, size_high + 1, self.step_size):
-                data.append([w * h, np.log2(w / h), w, h]) #对比例取对数，更符合人感知，宽高相反的可以对称分布。
+        for w in range(size_low, size_high+1, self.step_size):
+            for h in range(size_low, size_high+1, self.step_size):
+                data.append([w*h, np.log2(w/h), w, h])  # 对比例取对数，更符合人感知，宽高相反的可以对称分布。
         data = np.array(data)
 
-        error_area = np.abs(data[:, 0] - self.taget_area)
-        data_use = data[np.argsort(error_area)[:self.num_bucket*3], :] #取最小的num_bucket*3个
+        error_area = np.abs(data[:, 0]-self.taget_area)
+        data_use = data[np.argsort(error_area)[:self.num_bucket*3], :]  # 取最小的num_bucket*3个
 
-        #聚类，选出指定个数的bucket
+        # 聚类，选出指定个数的bucket
         kmeans = KMeans(n_clusters=self.num_bucket, random_state=0).fit(data_use[:, 1].reshape(-1, 1))
         labels = kmeans.labels_
-        self.buckets = [] # [bucket_id:[file_idx,...]]
+        self.buckets = []  # [bucket_id:[file_idx,...]]
         self.ratios_log = []
         self.size_buckets = []
         for i in range(self.num_bucket):
             map_idx = np.where(labels == i)[0]
-            m_idx = map_idx[np.argmin(np.abs(data_use[labels == i, 1] - np.median(data_use[labels == i, 1])))]
-            #self.buckets[wh_hash(*data_use[m_idx, 2:])]=[]
+            m_idx = map_idx[np.argmin(np.abs(data_use[labels == i, 1]-np.median(data_use[labels == i, 1])))]
+            # self.buckets[wh_hash(*data_use[m_idx, 2:])]=[]
             self.buckets.append([])
             self.ratios_log.append(data_use[m_idx, 1])
             self.size_buckets.append(data_use[m_idx, 2:].astype(int))
-        self.ratios_log=np.array(self.ratios_log)
-        self.size_buckets=np.array(self.size_buckets)
+        self.ratios_log = np.array(self.ratios_log)
+        self.size_buckets = np.array(self.size_buckets)
 
         # fill buckets with images w,h
-        self.idx_bucket_map=np.empty(len(self.file_names), dtype=int)
+        self.idx_bucket_map = np.empty(len(self.file_names), dtype=int)
         for i, file in enumerate(self.file_names):
             w, h = get_image_size(file)
-            bucket_id = np.abs(self.ratios_log-np.log2(w / h)).argmin()
+            bucket_id = np.abs(self.ratios_log-np.log2(w/h)).argmin()
             self.buckets[bucket_id].append(i)
-            self.idx_bucket_map[i]=bucket_id
-        logger.info('buckets info: ' + ', '.join(f'size:{self.size_buckets[i]}, num:{len(b)}' for i, b in enumerate(self.buckets)))
+            self.idx_bucket_map[i] = bucket_id
+        logger.info('buckets info: '+', '.join(f'size:{self.size_buckets[i]}, num:{len(b)}' for i, b in enumerate(self.buckets)))
 
     def build_buckets_from_images(self):
         logger.info('build buckets from images')
         ratio_list = []
         for i, file in enumerate(self.file_names):
             w, h = get_image_size(file)
-            ratio = np.log2(w / h)
+            ratio = np.log2(w/h)
             ratio_list.append(ratio)
-        ratio_list=np.array(ratio_list)
+        ratio_list = np.array(ratio_list)
 
         # 聚类，选出指定个数的bucket
         kmeans = KMeans(n_clusters=self.num_bucket, random_state=0).fit(ratio_list.reshape(-1, 1))
         labels = kmeans.labels_
         self.ratios_log = kmeans.cluster_centers_.reshape(-1)
 
-        ratios=2**self.ratios_log
-        h_all=np.sqrt(self.taget_area/ratios)
-        w_all=h_all*ratios
+        ratios = 2**self.ratios_log
+        h_all = np.sqrt(self.taget_area/ratios)
+        w_all = h_all*ratios
 
         # SD需要边长是8的倍数
-        h_all=(np.round(h_all / self.step_size) * self.step_size).astype(int)
-        w_all=(np.round(w_all / self.step_size) * self.step_size).astype(int)
+        h_all = (np.round(h_all/self.step_size)*self.step_size).astype(int)
+        w_all = (np.round(w_all/self.step_size)*self.step_size).astype(int)
         self.size_buckets = list(zip(w_all, h_all))
         self.size_buckets = np.array(self.size_buckets)
 
         self.buckets = []  # [bucket_id:[file_idx,...]]
         self.idx_bucket_map = np.empty(len(self.file_names), dtype=int)
         for bidx in range(self.num_bucket):
             bnow = labels == bidx
             self.buckets.append(np.where(bnow)[0].tolist())
-            self.idx_bucket_map[bnow]=bidx
+            self.idx_bucket_map[bnow] = bidx
         logger.info('buckets info: '+', '.join(f'size:{self.size_buckets[i]}, num:{len(b)}' for i, b in enumerate(self.buckets)))
 
-    def build(self, bs:int, img_root_list:List[str]):
+    def build(self, bs: int, img_root_list: List[str]):
         '''
         :param bs: batch_size * n_gpus * accumulation_step
         :param pre_build_arb:
         '''
         self.img_root_list = img_root_list
         if self.pre_build_arb and os.path.exists(self.pre_build_arb):
             self.load_arb(self.pre_build_arb)
             return
         else:
             self.file_names = [os.path.join(img_root, x) for img_root in img_root_list for x in os.listdir(img_root)
-                               if get_file_ext(x) in types_support]
+                if get_file_ext(x) in types_support]
         self._build()
 
         self.bs = bs
         rs = np.random.RandomState(42)
         # make len(bucket)%bs==0
         self.data_len = 0
         for bidx, bucket in enumerate(self.buckets):
-            rest = len(bucket) % bs
-            if rest > 0:
-                bucket.extend(rs.choice(bucket, bs - rest))
+            rest = len(bucket)%bs
+            if rest>0:
+                bucket.extend(rs.choice(bucket, bs-rest))
             self.data_len += len(bucket)
-            self.buckets[bidx]=np.array(bucket)
+            self.buckets[bidx] = np.array(bucket)
 
         if self.pre_build_arb:
             self.save_arb(self.pre_build_arb)
 
     def rest(self, epoch):
-        rs = np.random.RandomState(42 + epoch)
+        rs = np.random.RandomState(42+epoch)
         bucket_list = [x.copy() for x in self.buckets]
         # shuffle inter bucket
         for x in bucket_list:
             rs.shuffle(x)
 
         # shuffle of batches
         bucket_list = np.hstack(bucket_list).reshape(-1, self.bs).astype(int)
         rs.shuffle(bucket_list)
 
         self.idx_arb = bucket_list.reshape(-1)
 
-    def crop_resize(self, image, size):
-        return resize_crop_fix(image, size)
+    def crop_resize(self, image, size, mask_interp=cv2.INTER_CUBIC):
+        return resize_crop_fix(image, size, mask_interp=mask_interp)
 
     def __getitem__(self, idx):
         fidx = self.idx_arb[idx]
-        bidx=self.idx_bucket_map[fidx]
+        bidx = self.idx_bucket_map[fidx]
         return self.file_names[fidx], self.size_buckets[bidx]
 
     def __len__(self):
         return self.data_len
 
     @classmethod
-    def from_ratios(cls, target_area:int=640*640, step_size:int=8, num_bucket:int=10, ratio_max:float=4,
-                    pre_build_arb:str=None):
+    def from_ratios(cls, target_area: int = 640*640, step_size: int = 8, num_bucket: int = 10, ratio_max: float = 4,
+                    pre_build_arb: str = None):
         arb = cls(target_area, step_size, num_bucket, pre_build_arb=pre_build_arb)
         arb.ratio_max = ratio_max
         arb._build = arb.build_buckets_from_ratios
         return arb
 
     @classmethod
-    def from_files(cls, target_area:int=640*640, step_size:int=8, num_bucket:int=10, pre_build_arb:str=None):
+    def from_files(cls, target_area: int = 640*640, step_size: int = 8, num_bucket: int = 10, pre_build_arb: str = None):
         arb = RatioBucket(target_area, step_size, num_bucket, pre_build_arb=pre_build_arb)
         arb._build = arb.build_buckets_from_images
-        return arb
+        return arb
```

### Comparing `hcpdiff-0.4.1/hcpdiff/data/cond_pair_dataset.py` & `hcpdiff-0.4.2/hcpdiff/data/cond_pair_dataset.py`

 * *Files 14% similar despite different names*

```diff
@@ -20,17 +20,16 @@
 
 class TextImageCondPairDataset(TextImagePairDataset):
     """
     A dataset to prepare the instance and class images with the prompts for fine-tuning the model.
     It pre-processes the images and the tokenizes prompts.
     """
 
-    def __init__(self, tokenizer, tokenizer_repeats: int = 1, att_mask_encode: bool = False,
-                 bucket: BaseBucket = None, source: Dict = None, return_path: bool = False, **kwargs):
-        super().__init__(tokenizer, tokenizer_repeats, att_mask_encode, bucket, source, return_path)
+    def load_source(self, source: Dict):
+        super(TextImageCondPairDataset, self).load_source(source)
         for data_source in source.values():
             self.source_dict[data_source.img_root].cond_dir = data_source.cond_dir
         self.cond_transform = transforms.ToTensor()
 
     def load_data(self, path, size):
         img_root, img_name = os.path.split(path)
         image = self.load_image(path)
```

### Comparing `hcpdiff-0.4.1/hcpdiff/data/pair_dataset.py` & `hcpdiff-0.4.2/hcpdiff/data/pair_dataset.py`

 * *Files 15% similar despite different names*

```diff
@@ -33,34 +33,34 @@
 
     def __init__(self, tokenizer, tokenizer_repeats: int = 1, att_mask_encode: bool = False,
                  bucket: BaseBucket = None, source: Dict = None, return_path: bool = False, **kwargs):
         self.return_path = return_path
 
         self.tokenizer = tokenizer
         self.tokenizer_repeats = tokenizer_repeats
-
         self.bucket: BaseBucket = bucket
         self.att_mask_encode = att_mask_encode
+        self.load_source(source)
+        self.latents = None  # Cache latents for faster training. Works only without image argumentations.
 
+    def load_source(self, source: Dict):
         self.source_dict = {}
         for data_source in source.values():
             source_metas = Namespace()
             source_metas.caption_dict = self.load_captions(data_source.caption_file)
             source_metas.att_mask_path = {} if data_source.att_mask is None else \
-                {get_file_name(file): os.path.join(data_source.att_mask, file)
-                 for file in os.listdir(data_source.att_mask) if get_file_ext(file) in types_support}
+                {get_file_name(file):os.path.join(data_source.att_mask, file)
+                    for file in os.listdir(data_source.att_mask) if get_file_ext(file) in types_support}
             source_metas.prompt_template = self.load_template(data_source.prompt_template)
             source_metas.image_transforms = data_source.image_transforms
             source_metas.tag_transforms = data_source.tag_transforms
             source_metas.bg_color = tuple(data_source.bg_color)
 
             self.source_dict[os.path.dirname(data_source.img_root+'/')] = source_metas
 
-        self.latents = None  # Cache latents for faster training. Works only without image argumentations.
-
     def load_image(self, path):
         image = Image.open(path)
         if image.mode == 'RGBA':
             img_root = os.path.dirname(path)
             x, y = image.size
             canvas = Image.new('RGBA', image.size, self.source_dict[img_root].bg_color)
             canvas.paste(image, (0, 0, x, y), image)
@@ -144,7 +144,39 @@
 
         data['prompt'] = prompt_ids
 
         if self.return_path:
             return data, path
         else:
             return data
+
+    @staticmethod
+    def collate_fn(batch):
+        datas, sn_list, sp_list = {'img':[]}, [], []
+
+        data0 = batch[0]
+        if 'mask' in data0:
+            datas['mask'] = []
+        if 'cond' in data0:
+            datas['cond'] = []
+
+        for data in batch:
+            datas['img'].append(data['img'])
+            datas['mask'].append(data['mask'])
+            if 'cond' in data:
+                datas['cond'].append(data['cond'])
+
+            target = data['prompt']
+            if len(target.shape) == 2:
+                sn_list.append(target[0])
+                sp_list.append(target[1])
+            else:
+                sp_list.append(target)
+        sn_list += sp_list
+
+        datas['img'] = torch.stack(datas['img'])
+        datas['mask'] = torch.stack(datas['mask']).unsqueeze(1)
+        if 'cond' in data0:
+            datas['cond'] = torch.stack(datas['cond'])
+        datas['prompt'] = torch.stack(sn_list)
+
+        return datas
```

### Comparing `hcpdiff-0.4.1/hcpdiff/data/utils.py` & `hcpdiff-0.4.2/hcpdiff/data/utils.py`

 * *Files 12% similar despite different names*

```diff
@@ -22,65 +22,34 @@
 
     @staticmethod
     def crop(img: np.ndarray, top: int, left: int, height: int, width: int) -> np.ndarray:
         right = left + width
         bottom = top + height
         return img[..., top:bottom, left:right]
 
-def resize_crop_fix(img, target_size):
+def resize_crop_fix(img, target_size, mask_interp=cv2.INTER_CUBIC):
     w,h=img['img'].size
     if w==target_size[0] and h==target_size[1]:
         return img
 
     ratio_img=w/h
     if ratio_img > target_size[0]/target_size[1]:
         new_size = (int(ratio_img*target_size[1]), target_size[1])
         interp_type = Image.ANTIALIAS if h>target_size[1] else Image.BICUBIC
     else:
         new_size = (target_size[0], int(target_size[0]/ratio_img))
         interp_type = Image.ANTIALIAS if w>target_size[0] else Image.BICUBIC
     img['img'] = img['img'].resize(new_size, interp_type)
     if "mask" in img:
-        img['mask'] = cv2.resize(img['mask'], new_size, interpolation=cv2.INTER_CUBIC)
+        img['mask'] = cv2.resize(img['mask'], new_size, interpolation=mask_interp)
     if "cond" in img:
         img['cond'] = img['cond'].resize(new_size, interp_type)
 
     return DualRandomCrop(target_size[::-1])(img)
 
-def collate_fn_ft(batch):
-    datas, sn_list, sp_list = {'img':[]}, [], []
-
-    data0 = batch[0]
-    if 'mask' in data0:
-        datas['mask']=[]
-    if 'cond' in data0:
-        datas['cond']=[]
-
-    for data in batch:
-        datas['img'].append(data['img'])
-        datas['mask'].append(data['mask'])
-        if 'cond' in data:
-            datas['cond'].append(data['cond'])
-
-        target = data['prompt']
-        if len(target.shape)==2:
-            sn_list.append(target[0])
-            sp_list.append(target[1])
-        else:
-            sp_list.append(target)
-    sn_list += sp_list
-
-    datas['img'] = torch.stack(datas['img'])
-    datas['mask'] = torch.stack(datas['mask']).unsqueeze(1)
-    if 'cond' in data0:
-        datas['cond'] = torch.stack(datas['cond'])
-    datas['prompt'] = torch.stack(sn_list)
-
-    return datas
-
 class CycleData():
     def __init__(self, data_loader):
         self.data_loader = data_loader
 
     def __iter__(self):
         self.epoch = 0
         def cycle():
```

### Comparing `hcpdiff-0.4.1/hcpdiff/loggers/base_logger.py` & `hcpdiff-0.4.2/hcpdiff/loggers/base_logger.py`

 * *Files identical despite different names*

### Comparing `hcpdiff-0.4.1/hcpdiff/loggers/cli_logger.py` & `hcpdiff-0.4.2/hcpdiff/loggers/cli_logger.py`

 * *Files identical despite different names*

### Comparing `hcpdiff-0.4.1/hcpdiff/loggers/tensorboard_logger.py` & `hcpdiff-0.4.2/hcpdiff/loggers/tensorboard_logger.py`

 * *Files identical despite different names*

### Comparing `hcpdiff-0.4.1/hcpdiff/loggers/wandb_logger.py` & `hcpdiff-0.4.2/hcpdiff/loggers/wandb_logger.py`

 * *Files identical despite different names*

### Comparing `hcpdiff-0.4.1/hcpdiff/loss/min_snr_loss.py` & `hcpdiff-0.4.2/hcpdiff/loss/min_snr_loss.py`

 * *Files identical despite different names*

### Comparing `hcpdiff-0.4.1/hcpdiff/models/cfg_context.py` & `hcpdiff-0.4.2/hcpdiff/models/cfg_context.py`

 * *Files identical despite different names*

### Comparing `hcpdiff-0.4.1/hcpdiff/models/controlnet.py` & `hcpdiff-0.4.2/hcpdiff/models/controlnet.py`

 * *Files identical despite different names*

### Comparing `hcpdiff-0.4.1/hcpdiff/models/layers.py` & `hcpdiff-0.4.2/hcpdiff/models/layers.py`

 * *Files identical despite different names*

### Comparing `hcpdiff-0.4.1/hcpdiff/models/lora_base.py` & `hcpdiff-0.4.2/hcpdiff/models/lora_base.py`

 * *Files 2% similar despite different names*

```diff
@@ -61,25 +61,25 @@
                 fea_out[batch_mask, ...] = fea_out[batch_mask, ...] + self.layer(fea_in[0][batch_mask, ...]) * self.alpha
                 return fea_out
             else: # colossal-AI dose not support inplace+view
                 new_out = fea_out.clone()
                 new_out[batch_mask, ...] = fea_out[batch_mask, ...] + self.layer(fea_in[0][batch_mask, ...]) * self.alpha
                 return new_out
 
-    def collapse_to_host(self, alpha=None, base_alpha=1.0):
+    def reparameterization_to_host(self, alpha=None, base_alpha=1.0):
         if alpha is None:
             alpha = self.alpha
 
         host = self.host()
-        re_w, re_b = self.get_collapsed_param()
+        re_w, re_b = self.layer.get_collapsed_param()
         host.weight = nn.Parameter(
             host.weight.data * base_alpha + alpha * re_w.to(host.weight.device, dtype=host.weight.dtype)
         )
 
-        if self.lora_up.bias is not None:
+        if self.layer.lora_up.bias is not None:
             if host.bias is None:
                 host.bias = nn.Parameter(re_b.to(host.weight.device, dtype=host.weight.dtype))
             else:
                 host.bias = nn.Parameter(
                     host.bias.data * base_alpha + alpha * re_b.to(host.weight.device, dtype=host.weight.dtype))
 
     class LinearLayer(nn.Module):
```

### Comparing `hcpdiff-0.4.1/hcpdiff/models/lora_layers.py` & `hcpdiff-0.4.2/hcpdiff/models/lora_layers.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 
 import torch
 from einops import repeat, rearrange, einsum
 from torch import nn
 
 from .lora_base import LoraBlock
 from .layers import GroupLinear
+import warnings
 
 class LoraLayer(LoraBlock):
     def __init__(self, lora_id:int, host, rank=1, dropout=0.1, alpha=1.0, bias=False, inplace=True, alpha_auto_scale=True, **kwargs):
         super().__init__(lora_id, host, rank, dropout, alpha, bias, inplace, alpha_auto_scale=alpha_auto_scale)
 
     class LinearLayer(LoraBlock.LinearLayer):
         def __init__(self, host, rank, bias, dropout, block):
@@ -46,16 +47,17 @@
             return w, b
 
 class LoraLayerGroup(LoraBlock):
     def __init__(self, lora_id:int, host, rank=1, dropout=0.1, alpha=1.0, bias=False, inplace=True, rank_groups=1, alpha_auto_scale=True, **kwargs):
         self.rank_groups_raw = rank_groups
         super().__init__(lora_id, host, rank, dropout, alpha, bias, inplace, alpha_auto_scale=alpha_auto_scale)
 
-    def collapse_to_host(self, alpha=None, base_alpha=1.0):
-        raise NotImplementedError('LoraLayerGroup not support reparameterization.')
+    def reparameterization_to_host(self, alpha=None, base_alpha=1.0):
+        warnings.warn('LoraLayerGroup cannot reparameterization.')
+        pass
 
     class LinearLayer(LoraBlock.LinearLayer):
         def __init__(self, host, rank, bias, dropout, block):
             super().__init__(host, rank, bias, dropout, block)
             self.register_buffer('rank_groups', torch.tensor(block.rank_groups_raw, dtype=torch.int))
             self.lora_down = GroupLinear(host.in_features*self.rank_groups, self.rank, groups=self.rank_groups, bias=False)
             self.lora_up = GroupLinear(self.rank, host.out_features*self.rank_groups, groups=self.rank_groups, bias=bias)
```

### Comparing `hcpdiff-0.4.1/hcpdiff/models/plugin.py` & `hcpdiff-0.4.2/hcpdiff/models/plugin.py`

 * *Files 16% similar despite different names*

```diff
@@ -37,18 +37,19 @@
 
     def set_hyper_params(self, **kwargs):
         for k,v in kwargs.items():
             setattr(self, k, v)
 
     @staticmethod
     def extract_state_without_plugin(model: nn.Module, trainable=False):
+        trainable_keys = {k for k, v in model.named_parameters() if v.requires_grad}
         plugin_names = {k for k,v in model.named_modules() if isinstance(v, BasePluginBlock)}
         model_sd = {}
         for k, v in model.state_dict().items():
-            if (not trainable) or v.requires_grad:
+            if (not trainable) or k in trainable_keys:
                 for name in plugin_names:
                     if k.startswith(name):
                         break
                 else:
                     model_sd[k]=v
         return model_sd
 
@@ -183,14 +184,44 @@
         host_model = self.host_model()
         delattr(host_model, self.name)
         for handle_from in self.hook_handle_from:
             handle_from.remove()
         for handle_to in self.hook_handle_to:
             handle_to.remove()
 
+
+class WrapPluginBlock(BasePluginBlock):
+    def __init__(self, name:str, host:nn.Module, host_model=None, parent_block:nn.Module=None, host_name:str=None):
+        super().__init__(name)
+        self.host = weakref.ref(host)
+        self.parent_block = weakref.ref(parent_block)
+        self.host_name = host_name
+
+        delattr(parent_block, host_name)
+        setattr(parent_block, f'{host_name}_origin_block', host)
+        setattr(parent_block, host_name, self)
+
+    def forward(self, *args, **kwargs):
+        args, kwargs = self.pre_forward(*args, **kwargs)
+        output = self.host()(*args, **kwargs)
+        output = self.post_forward(output, *args, **kwargs)
+        return output
+
+    def pre_forward(self, *args, **kwargs):
+        return args, kwargs
+
+    def post_forward(self, output, *args, **kwargs):
+        return output
+
+    def remove(self):
+        parent_block = self.parent_block()
+        delattr(parent_block, self.host_name)
+        delattr(parent_block, f'{self.host_name}_origin_block')
+        setattr(parent_block, self.host_name, self.host())
+
 class PluginGroup:
     def __init__(self, plugin_dict:Dict[str, BasePluginBlock]):
         self.plugin_dict = plugin_dict # {host_model_path: plugin_object}
 
     def __setitem__(self, k, v):
         self.plugin_dict[k]=v
```

### Comparing `hcpdiff-0.4.1/hcpdiff/models/text_emb_ex.py` & `hcpdiff-0.4.2/hcpdiff/models/text_emb_ex.py`

 * *Files identical despite different names*

### Comparing `hcpdiff-0.4.1/hcpdiff/models/textencoder_ex.py` & `hcpdiff-0.4.2/hcpdiff/models/textencoder_ex.py`

 * *Files 1% similar despite different names*

```diff
@@ -55,15 +55,16 @@
         feat_re = rearrange(feat_in[0], 'b (r w) -> (b r) w', r=self.N_repeats) # 使Attention mask的尺寸为N_word+2
         return (feat_re,) if len(feat_in)==1 else (feat_re, *feat_in[1:])
 
     def forward_hook(self, host, feat_in:Tuple[torch.Tensor], feat_out):
         if self.clip_skip>0:
             encoder_hidden_states = feat_out['hidden_states'][-self.clip_skip-1]
             encoder_hidden_states = self.text_enc.text_model.final_layer_norm(encoder_hidden_states)
-            encoder_hidden_states = encoder_hidden_states + 0*feat_out['last_hidden_state'] # avoid unused parameters, make gradient checkpointing happy
+            if self.text_enc.training:
+                encoder_hidden_states = encoder_hidden_states + 0*feat_out['last_hidden_state'] # avoid unused parameters, make gradient checkpointing happy
         else:
             encoder_hidden_states = feat_out['last_hidden_state']  # Get the text embedding for conditioning
 
         encoder_hidden_states = rearrange(encoder_hidden_states, '(b r) ... -> b r ...', r=self.N_repeats)  # [B, N_repeat, N_word+2, N_emb]
         BOS, EOS = encoder_hidden_states[:, 0, :1, :], encoder_hidden_states[:, -1, -1:, :]
         encoder_hidden_states = torch.cat([BOS, encoder_hidden_states[:, :, 1:-1, :].flatten(1, 2), EOS], dim=1)  # [B, N_repeat*N_word+2, N_emb]
 
@@ -127,8 +128,8 @@
             attn_output = layer.out_proj(attn_output)
 
             return attn_output, None
         layer.forward = forward
 
     @classmethod
     def hook_pipe(cls, pipe, N_repeats=3, clip_skip=0):
-        return cls(pipe.text_encoder, pipe.tokenizer, N_repeats=N_repeats, device=pipe._execution_device, clip_skip=clip_skip)
+        return cls(pipe.text_encoder, pipe.tokenizer, N_repeats=N_repeats, device='cuda', clip_skip=clip_skip)
```

### Comparing `hcpdiff-0.4.1/hcpdiff/models/tokenizer_ex.py` & `hcpdiff-0.4.2/hcpdiff/models/tokenizer_ex.py`

 * *Files identical despite different names*

### Comparing `hcpdiff-0.4.1/hcpdiff/noise/pyramid_noise.py` & `hcpdiff-0.4.2/hcpdiff/noise/pyramid_noise.py`

 * *Files 5% similar despite different names*

```diff
@@ -19,19 +19,19 @@
             timesteps: torch.IntTensor,
     ) -> torch.FloatTensor:
         with torch.no_grad():
             b, c, h, w = noise.shape
             for i in range(1, self.level):
                 r = random.random() * 2 + self.step
                 wn, hn = max(1, int(w / (r ** i))), max(1, int(h / (r ** i)))
-                noise += F.interpolate(torch.randn(b, c, hn, wn).to(noise), (w, h), None, self.mode) * (self.discount ** i)
+                noise += F.interpolate(torch.randn(b, c, hn, wn).to(noise), (h, w), None, self.mode) * (self.discount ** i)
                 if wn == 1 or hn == 1:
                     break
             noise = noise / noise.std()
-        return super(PyramidNoiseScheduler, self).add_noise(original_samples, noise, timesteps)
+        return self.base_scheduler.add_noise(original_samples, noise, timesteps)
 
 # if __name__ == '__main__':
 #     noise = torch.randn(1,3,512,512)
 #     level=10
 #     discount=0.6
 #     b, c, h, w = noise.shape
 #     for i in range(level):
```

### Comparing `hcpdiff-0.4.1/hcpdiff/tools/convert_caption_txt2json.py` & `hcpdiff-0.4.2/hcpdiff/tools/convert_caption_txt2json.py`

 * *Files identical despite different names*

### Comparing `hcpdiff-0.4.1/hcpdiff/tools/create_embedding.py` & `hcpdiff-0.4.2/hcpdiff/tools/create_embedding.py`

 * *Files identical despite different names*

### Comparing `hcpdiff-0.4.1/hcpdiff/tools/gen_from_ptlist.py` & `hcpdiff-0.4.2/hcpdiff/tools/gen_from_ptlist.py`

 * *Files 14% similar despite different names*

```diff
@@ -8,21 +8,22 @@
 import json
 from tqdm.auto import tqdm
 
 parser = argparse.ArgumentParser(description='Stable Diffusion Training')
 parser.add_argument('--prompt_file', type=str, default='')
 parser.add_argument('--model', type=str, default='runwayml/stable-diffusion-v1-5')
 parser.add_argument('--out_dir', type=str, default=r'./prompt_ds')
-parser.add_argument('--negative_prompt', type=str, default='')
+parser.add_argument('--negative_prompt', type=str, default='lowres, bad anatomy, bad hands, text, error, missing fingers, extra digit, fewer digits, cropped, worst quality, low quality, normal quality, jpeg artifacts, signature, watermark, username, blurry')
 parser.add_argument('--num', type=int, default=200)
 parser.add_argument('--bs', type=int, default=4)
 args = parser.parse_args()
 
 torch.backends.cudnn.benchmark = True
 
+os.makedirs(args.out_dir, exist_ok=True)
 
 def split_batch(data, bs):
     return [data[i:i + bs] for i in range(0, len(data), bs)]
 
 
 data = pq.read_table(args.prompt_file).to_batches(args.bs)
 pipeline = StableDiffusionPipeline.from_pretrained(args.model, torch_dtype=torch.float16)
```

### Comparing `hcpdiff-0.4.1/hcpdiff/tools/init_proj.py` & `hcpdiff-0.4.2/hcpdiff/tools/init_proj.py`

 * *Files identical despite different names*

### Comparing `hcpdiff-0.4.1/hcpdiff/tools/lora_convert.py` & `hcpdiff-0.4.2/hcpdiff/tools/lora_convert.py`

 * *Files 6% similar despite different names*

```diff
@@ -68,14 +68,17 @@
     print('convert lora model')
     ckpt_manager = auto_manager(args.lora_path)()
 
     if args.from_webui:
         state = ckpt_manager.load_ckpt(args.lora_path)
         # convert the weight name
         sd_TE, sd_unet = converter.convert_from_webui(state)
+        if args.auto_scale_alpha:
+            sd_TE['lora'] = {k:(v/v.shape[1] if 'lora_up' in k else v) for k, v in sd_TE['lora'].items()}
+            sd_unet['lora'] = {k:(v/v.shape[1] if 'lora_up' in k else v) for k, v in sd_unet['lora'].items()}
         # wegiht save
         os.makedirs(args.dump_path, exist_ok=True)
         TE_path = os.path.join(args.dump_path, 'TE-'+lora_name)
         unet_path = os.path.join(args.dump_path, 'unet-'+lora_name)
         ckpt_manager._save_ckpt(sd_TE, save_path=TE_path)
         ckpt_manager._save_ckpt(sd_unet, save_path=unet_path)
         print('save text encoder lora to:', TE_path)
```

### Comparing `hcpdiff-0.4.1/hcpdiff/tools/sd2diffusers.py` & `hcpdiff-0.4.2/hcpdiff/tools/sd2diffusers.py`

 * *Files identical despite different names*

### Comparing `hcpdiff-0.4.1/hcpdiff/train_ac.py` & `hcpdiff-0.4.2/hcpdiff/train_ac.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 from diffusers import AutoencoderKL, UNet2DConditionModel
 from diffusers.utils.import_utils import is_xformers_available
 from omegaconf import OmegaConf
 from transformers import AutoTokenizer
 from functools import partial
 
 from hcpdiff.ckpt_manager import CkptManagerPKL, CkptManagerSafe
-from hcpdiff.data import RatioBucket, DataGroup, collate_fn_ft
+from hcpdiff.data import RatioBucket, DataGroup
 from hcpdiff.loggers import LoggerGroup
 from hcpdiff.models import EmbeddingPTHook, TEEXHook, CFGContext, DreamArtistPTContext
 from hcpdiff.utils.cfg_net_tools import make_hcpdiff, make_plugin
 from hcpdiff.utils.ema import ModelEMA
 from hcpdiff.utils.net_utils import get_scheduler, import_text_encoder_class, TEUnetWrapper, load_emb
 from hcpdiff.utils.utils import load_config_with_cli, get_cfg_range, mgcd
 from hcpdiff.visualizer import Visualizer
@@ -306,16 +306,16 @@
         if cache_latents:
             self.cache_latents = True
             train_dataset.cache_latents(self.vae, self.weight_dtype, self.device, show_prog=self.is_local_main_process)
 
         # Pytorch Data loader
         train_sampler = torch.utils.data.distributed.DistributedSampler(train_dataset, num_replicas=self.world_size,
                                                                         rank=self.local_rank, shuffle=not arb)
-        train_loader = torch.utils.data.DataLoader(train_dataset, batch_size=batch_size,
-                                                   num_workers=self.cfgs.train.workers, sampler=train_sampler, collate_fn=collate_fn_ft)
+        train_loader = torch.utils.data.DataLoader(train_dataset, batch_size=batch_size, num_workers=self.cfgs.train.workers,
+                                                   sampler=train_sampler, collate_fn=train_dataset.collate_fn)
         return train_loader
 
     def get_param_group_train(self):
         # make miniFT and warp with lora
         self.DA_lora = False
         train_params_unet, self.lora_unet = make_hcpdiff(self.unet, self.cfgs.unet, self.cfgs.lora_unet)
         if isinstance(self.lora_unet, tuple):  # creat negative lora
@@ -489,15 +489,15 @@
             raise ValueError(f"Unknown loss type {self.cfgs.train.loss.type}")
         return model_pred, target, timesteps
 
     def train_one_step(self, data_list):
         with self.accelerator.accumulate(self.unet):
             for idx, data in enumerate(data_list):
                 image = data.pop('img').to(self.device, dtype=self.weight_dtype)
-                att_mask = data.pop('mask').to(self.device)
+                att_mask = data.pop('mask').to(self.device) if 'mask' in data else None
                 prompt_ids = data.pop('prompt').to(self.device)
                 other_datas = {k:v.to(self.device, dtype=self.weight_dtype) for k, v in data.items()}
 
                 latents = self.get_latents(image, self.train_loader_group.get_dataset(idx))
                 model_pred, target, timesteps = self.forward(latents, prompt_ids, **other_datas)
                 loss = self.get_loss(model_pred, target, timesteps, att_mask) * self.train_loader_group.get_loss_weights(idx)
                 self.accelerator.backward(loss)
@@ -518,19 +518,26 @@
                 self.lr_scheduler_pt.step()
                 self.optimizer_pt.zero_grad(set_to_none=self.cfgs.train.set_grads_to_none)
 
             self.update_ema()
         return loss.item()
 
     def get_loss(self, model_pred, target, timesteps, att_mask):
-        if len(self.embedding_hook.emb_train)>0:
-            return (self.criterion(model_pred.float(), target.float(), timesteps)*att_mask).mean() \
-                   +0*sum(self.embedding_hook.emb_train).mean()  # avoid unused parameters, make gradient checkpointing happy
+        if att_mask is None:
+            if len(self.embedding_hook.emb_train)>0:
+                return (self.criterion(model_pred.float(), target.float(), timesteps)).mean() \
+                       +0*sum(self.embedding_hook.emb_train).mean()  # avoid unused parameters, make gradient checkpointing happy
+            else:
+                return (self.criterion(model_pred.float(), target.float(), timesteps)).mean()
         else:
-            return (self.criterion(model_pred.float(), target.float(), timesteps)*att_mask).mean()
+            if len(self.embedding_hook.emb_train)>0:
+                return (self.criterion(model_pred.float(), target.float(), timesteps)*att_mask).mean() \
+                       +0*sum(self.embedding_hook.emb_train).mean()  # avoid unused parameters, make gradient checkpointing happy
+            else:
+                return (self.criterion(model_pred.float(), target.float(), timesteps)*att_mask).mean()
 
     def update_ema(self):
         if hasattr(self, 'ema_unet'):
             self.ema_unet.step(self.unet_raw.named_parameters())
         if hasattr(self, 'ema_text_encoder'):
             self.ema_text_encoder.step(self.text_encoder_raw.named_parameters())
```

### Comparing `hcpdiff-0.4.1/hcpdiff/train_ac_single.py` & `hcpdiff-0.4.2/hcpdiff/train_ac_single.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 import argparse
 import sys
-import torch
-from loguru import logger
 from functools import partial
 
+import torch
 from accelerate import Accelerator
+from loguru import logger
+
 from hcpdiff.train_ac import Trainer, RatioBucket, load_config_with_cli, set_seed
-from hcpdiff.data import collate_fn_ft
 
 class TrainerSingleCard(Trainer):
     def init_context(self, cfgs_raw):
         self.accelerator = Accelerator(
             gradient_accumulation_steps=self.cfgs.train.gradient_accumulation_steps,
             mixed_precision=self.cfgs.mixed_precision,
             step_scheduler_with_optimizer=False,
         )
 
         self.local_rank = 0
         self.world_size = self.accelerator.num_processes
 
-        set_seed(self.cfgs.seed + self.local_rank)
+        set_seed(self.cfgs.seed+self.local_rank)
 
     def prepare(self):
         # Prepare everything with accelerator.
         prepare_obj_list = [self.unet]
         prepare_name_list = ['unet']
         if hasattr(self, 'optimizer'):
             prepare_obj_list.extend([self.optimizer, self.lr_scheduler])
@@ -41,32 +41,32 @@
         ds_num = len(self.train_loader_group.loader_list)
         self.train_loader_group.loader_list = list(prepared_obj[-ds_num:])
         prepared_obj = prepared_obj[:-ds_num]
 
         for name, obj in zip(prepare_name_list, prepared_obj):
             setattr(self, name, obj)
 
-    def build_data(self, data_builder:partial) -> torch.utils.data.DataLoader:
+    def build_data(self, data_builder: partial) -> torch.utils.data.DataLoader:
         batch_size = data_builder.keywords.pop('batch_size')
         cache_latents = data_builder.keywords.pop('cache_latents')
         self.batch_size_list.append(batch_size)
 
         train_dataset = data_builder(tokenizer=self.tokenizer, tokenizer_repeats=self.cfgs.model.tokenizer_repeats)
-        train_dataset.bucket.build(batch_size * self.world_size,
+        train_dataset.bucket.build(batch_size*self.world_size,
                                    img_root_list=[source.img_root for source in data_builder.keywords['source'].values()])
         arb = isinstance(train_dataset.bucket, RatioBucket)
         logger.info(f"len(train_dataset): {len(train_dataset)}")
 
         if cache_latents:
             self.cache_latents = True
             train_dataset.cache_latents(self.vae, self.weight_dtype, self.device, show_prog=self.is_local_main_process)
 
         # Pytorch Data loader
         train_loader = torch.utils.data.DataLoader(train_dataset, batch_size=batch_size,
-            num_workers=self.cfgs.train.workers, shuffle=not arb, collate_fn=collate_fn_ft)
+                                                   num_workers=self.cfgs.train.workers, shuffle=not arb, collate_fn=train_dataset.collate_fn)
         return train_loader
 
     def encode_decode(self, prompt_ids, noisy_latents, timesteps, **kwargs):
         input_all = dict(prompt_ids=prompt_ids, noisy_latents=noisy_latents, timesteps=timesteps, **kwargs)
         if hasattr(self.text_encoder, 'input_feeder'):
             for feeder in self.text_encoder.input_feeder:
                 feeder(input_all)
@@ -75,15 +75,15 @@
                 feeder(input_all)
 
         encoder_hidden_states = self.text_encoder(prompt_ids, output_hidden_states=True)  # Get the text embedding for conditioning
         model_pred = self.unet(noisy_latents, timesteps, encoder_hidden_states).sample  # Predict the noise residual
         return model_pred
 
     def get_loss(self, model_pred, target, timesteps, att_mask):
-        return (self.criterion(model_pred.float(), target.float(), timesteps) * att_mask).mean()
+        return (self.criterion(model_pred.float(), target.float(), timesteps)*att_mask).mean()
 
     def update_ema(self):
         if hasattr(self, 'ema_unet'):
             self.ema_unet.step(self.unet.named_parameters())
         if hasattr(self, 'ema_text_encoder'):
             self.ema_text_encoder.step(self.text_encoder.named_parameters())
 
@@ -96,10 +96,10 @@
         return self.text_encoder
 
 if __name__ == '__main__':
     parser = argparse.ArgumentParser(description='Stable Diffusion Training')
     parser.add_argument('--cfg', type=str, default='cfg/train/demo.yaml')
     args, _ = parser.parse_known_args()
 
-    conf = load_config_with_cli(args.cfg, args_list=sys.argv[3:]) # skip --cfg
-    trainer=TrainerSingleCard(conf)
-    trainer.train()
+    conf = load_config_with_cli(args.cfg, args_list=sys.argv[3:])  # skip --cfg
+    trainer = TrainerSingleCard(conf)
+    trainer.train()
```

### Comparing `hcpdiff-0.4.1/hcpdiff/train_colo.py` & `hcpdiff-0.4.2/hcpdiff/train_colo.py`

 * *Files identical despite different names*

### Comparing `hcpdiff-0.4.1/hcpdiff/train_deepspeed.py` & `hcpdiff-0.4.2/hcpdiff/train_deepspeed.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,19 @@
 import argparse
-import sys
-import torch
-from torch import nn
 import os
-import itertools
-from functools import partial
+import sys
 import warnings
+from functools import partial
+
+import torch
 
-from accelerate import Accelerator
-from hcpdiff.train_ac import Trainer, RatioBucket, load_config_with_cli, set_seed
 from hcpdiff.ckpt_manager import CkptManagerPKL, CkptManagerSafe
+from hcpdiff.train_ac import Trainer, load_config_with_cli
 from hcpdiff.utils.net_utils import get_scheduler
 
-
 class TrainerDeepSpeed(Trainer):
 
     def build_ckpt_manager(self):
         if self.cfgs.ckpt_type == 'torch':
             self.ckpt_manager = CkptManagerPKL(plugin_from_raw=True)
         elif self.cfgs.ckpt_type == 'safetensors':
             self.ckpt_manager = CkptManagerSafe(plugin_from_raw=True)
@@ -77,10 +74,10 @@
                 self.lr_scheduler = get_scheduler(optimizer=self.optimizer, **self.cfgs.train.scheduler)
 
 if __name__ == '__main__':
     parser = argparse.ArgumentParser(description='Stable Diffusion Training')
     parser.add_argument('--cfg', type=str, default='cfg/train/demo.yaml')
     args, _ = parser.parse_known_args()
 
-    conf = load_config_with_cli(args.cfg, args_list=sys.argv[3:]) # skip --cfg
-    trainer=TrainerDeepSpeed(conf)
-    trainer.train()
+    conf = load_config_with_cli(args.cfg, args_list=sys.argv[3:])  # skip --cfg
+    trainer = TrainerDeepSpeed(conf)
+    trainer.train()
```

### Comparing `hcpdiff-0.4.1/hcpdiff/utils/caption_tools.py` & `hcpdiff-0.4.2/hcpdiff/utils/caption_tools.py`

 * *Files identical despite different names*

### Comparing `hcpdiff-0.4.1/hcpdiff/utils/cfg_net_tools.py` & `hcpdiff-0.4.2/hcpdiff/utils/cfg_net_tools.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 import re
 import torch
 from torch import nn
 
 from .utils import net_path_join
 from hcpdiff.models.lora_base import LoraBlock, LoraGroup
 from hcpdiff.models import lora_layers
-from hcpdiff.models.plugin import SinglePluginBlock, MultiPluginBlock, PluginBlock, PluginGroup
+from hcpdiff.models.plugin import SinglePluginBlock, MultiPluginBlock, PluginBlock, PluginGroup, WrapPluginBlock
 from hcpdiff.ckpt_manager import CkptManagerPKL, CkptManagerSafe
 
 def get_class_match_layer(class_name, block:nn.Module):
     if type(block).__name__==class_name:
         return ['']
     else:
         return ['.'+name for name, layer in block.named_modules() if type(layer).__name__==class_name]
@@ -92,28 +92,30 @@
 
     train_params=[]
     all_lora_blocks={}
     all_lora_blocks_neg={}
 
     if cfg_model is not None:
         for item in cfg_model:
+            params_group = []
             for layer_name in get_match_layers(item.layers, named_modules):
                 layer = named_modules[layer_name]
                 layer.requires_grad_(True)
                 layer.train()
-                train_params.append({'params':list(LoraBlock.extract_param_without_lora(layer).values()), 'lr':getattr(item, 'lr', default_lr)})
+                params_group.extend(list(LoraBlock.extract_param_without_lora(layer).values()))
+            train_params.append({'params':list(set(params_group)), 'lr':getattr(item, 'lr', default_lr)})
 
     if cfg_lora is not None:
         for lora_id, item in enumerate(cfg_lora):
+            params_group = []
             for layer_name in get_match_layers(item.layers, named_modules):
                 layer = named_modules[layer_name]
                 arg_dict = {k:v for k,v in item.items() if k!='layers'}
                 lora_block_dict = lora_layers.layer_map[getattr(arg_dict, 'type', 'lora')].wrap_model(lora_id, layer, **arg_dict)
 
-                params_group = []
                 block_branch = getattr(item, 'branch', None) # for DreamArtist-lora
                 for k,v in lora_block_dict.items():
                     block_path = net_path_join(layer_name, k)
                     if block_branch is None:
                         all_lora_blocks[block_path] = v
                     elif block_branch=='p':
                         all_lora_blocks[block_path] = v
@@ -123,15 +125,15 @@
                         v.set_mask((0, 0.5))
                     else:
                         raise NotImplementedError(f'Unsupported branch "{block_branch}"')
                     v.requires_grad_(True)
                     v.train()
                     params_group.extend(v.parameters())
 
-                train_params.append({'params': params_group, 'lr':getattr(item, 'lr', default_lr)})
+            train_params.append({'params': params_group, 'lr':getattr(item, 'lr', default_lr)})
 
     if len(all_lora_blocks_neg)>0:
         return train_params, (LoraGroup(all_lora_blocks), LoraGroup(all_lora_blocks_neg))
     else:
         return train_params, LoraGroup(all_lora_blocks)
 
 def make_plugin(model, cfg_plugin, default_lr=1e-5) -> Tuple[List, Dict[str, PluginGroup]]:
@@ -147,65 +149,79 @@
     for plugin_name, builder in cfg_plugin.items():
         all_plugin_blocks={}
 
         lr = builder.keywords.pop('lr') if 'lr' in builder.keywords else default_lr
         train_plugin = builder.keywords.pop('train') if 'train' in builder.keywords else True
         plugin_class = getattr(builder.func, '__self__', builder.func) # support static or class method
 
+        params_group = []
         if issubclass(plugin_class, MultiPluginBlock):
             from_layers = [{**item, 'layer':named_modules[item['layer']]} for item in get_match_layers(builder.keywords.pop('from_layers'), named_modules, return_metas=True)]
             to_layers = [{**item, 'layer':named_modules[item['layer']]} for item in get_match_layers(builder.keywords.pop('to_layers'), named_modules, return_metas=True)]
 
             layer = builder(name=plugin_name, host_model=model, from_layers=from_layers, to_layers=to_layers)
             if train_plugin:
                 layer.requires_grad_(True)
                 layer.train()
-                train_params.append({'params': layer.parameters(), 'lr': lr})
+                params_group.extend(layer.parameters())
             else:
                 layer.requires_grad_(False)
                 layer.eval()
             all_plugin_blocks[''] = layer
         elif issubclass(plugin_class, SinglePluginBlock):
             layers_name = builder.keywords.pop('layers')
             for layer_name in get_match_layers(layers_name, named_modules):
                 blocks = builder(name=plugin_name, host_model=model, host=named_modules[layer_name])
                 if not isinstance(blocks, dict):
                     blocks={'':blocks}
 
-                params_group = []
                 for k,v in blocks.items():
                     all_plugin_blocks[net_path_join(layer_name, k)] = v
                     if train_plugin:
                         v.requires_grad_(True)
                         v.train()
                         params_group.extend(v.parameters())
                     else:
                         v.requires_grad_(False)
                         v.eval()
-                if train_plugin:
-                    train_params.append({'params': params_group, 'lr': lr})
         elif issubclass(plugin_class, PluginBlock):
             from_layer = get_match_layers(builder.keywords.pop('from_layer'), named_modules, return_metas=True)
             to_layer = get_match_layers(builder.keywords.pop('to_layer'), named_modules, return_metas=True)
 
             for from_layer_meta, to_layer_meta in zip(from_layer, to_layer):
                 from_layer_name=from_layer_meta['layer']
                 from_layer_meta['layer']=named_modules[from_layer_name]
                 to_layer_meta['layer']=named_modules[to_layer_meta['layer']]
                 layer = builder(name=plugin_name, host_model=model, from_layer=from_layer_meta, to_layer=to_layer_meta)
                 if train_plugin:
                     layer.requires_grad_(True)
                     layer.train()
-                    train_params.append({'params': layer.parameters(), 'lr': lr})
+                    params_group.extend(layer.parameters())
+                else:
+                    layer.requires_grad_(False)
+                    layer.eval()
+                all_plugin_blocks[from_layer_name] = layer
+        elif issubclass(plugin_class, WrapPluginBlock):
+            layers_name = builder.keywords.pop('layers')
+            for layer_name in get_match_layers(layers_name, named_modules):
+                parent_name, host_name = layers_name.rsplit('.', 1)
+                layer = builder(name=plugin_name, host_model=model, host=named_modules[layer_name],
+                                parent_block=named_modules[parent_name], host_name=host_name)
+                if train_plugin:
+                    layer.requires_grad_(True)
+                    layer.train()
+                    params_group.extend(layer.parameters())
                 else:
                     layer.requires_grad_(False)
                     layer.eval()
                 all_plugin_blocks[from_layer_name] = layer
         else:
             raise NotImplementedError(f'Unknown plugin {plugin_class}')
+        if train_plugin:
+            train_params.append({'params':params_group, 'lr':lr})
         all_plugin_group[plugin_name] = PluginGroup(all_plugin_blocks)
     return train_params, all_plugin_group
 
 @torch.no_grad()
 def load_hcpdiff(model:nn.Module, cfg_merge):
     named_modules = {k: v for k, v in model.named_modules()}
     named_params = {k: v for k, v in model.named_parameters()}
```

### Comparing `hcpdiff-0.4.1/hcpdiff/utils/colo_utils.py` & `hcpdiff-0.4.2/hcpdiff/utils/colo_utils.py`

 * *Files identical despite different names*

### Comparing `hcpdiff-0.4.1/hcpdiff/utils/ema.py` & `hcpdiff-0.4.2/hcpdiff/utils/ema.py`

 * *Files identical despite different names*

### Comparing `hcpdiff-0.4.1/hcpdiff/utils/img_size_tool.py` & `hcpdiff-0.4.2/hcpdiff/utils/img_size_tool.py`

 * *Files identical despite different names*

### Comparing `hcpdiff-0.4.1/hcpdiff/utils/net_utils.py` & `hcpdiff-0.4.2/hcpdiff/utils/net_utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import os
+import time
 from typing import Optional, Union
 
 import torch
 from diffusers.optimization import SchedulerType, TYPE_TO_SCHEDULER_FUNCTION, Optimizer
 from torch import nn
 from torch.optim import lr_scheduler
 from transformers import PretrainedConfig
@@ -163,7 +164,19 @@
                             result = (result,)
                     else:
                         result = args
                     return old_forward(*result, **kwargs)
 
                 block.forward = new_forward
     remove_all_hooks(model)
+
+def _convert_cpu(t):
+    return t.to('cpu') if t.device.type == 'cuda' else t
+
+def _convert_cuda(t):
+    return t.to('cuda') if t.device.type == 'cpu' else t
+
+def to_cpu(model):
+    model._apply(_convert_cpu)
+
+def to_cuda(model):
+    model._apply(_convert_cuda)
```

### Comparing `hcpdiff-0.4.1/hcpdiff/utils/utils.py` & `hcpdiff-0.4.2/hcpdiff/utils/utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 from typing import Tuple
 
 import re
 import torch
 import math
 from omegaconf import OmegaConf
 
+size_mul = {'K': 1<<10, 'M':1<<20, 'G':1<<30, 'T':1<<40}
+size_key = 'TGMK'
+
 def str2bool(v):
     return v.lower() in ("yes", "true", "t", "1")
 
 def low_rank_approximate(weight, rank, clamp_quantile=0.99):
     if len(weight.shape)==4: # conv
         weight=weight.flatten(1)
         out_ch, in_ch, k1, k2 = weight.shape
@@ -98,8 +101,16 @@
 def net_path_join(*args):
     return '.'.join(args).strip('.').replace('..', '.')
 
 def mgcd(*args):
     g = args[0]
     for s in args[1:]:
         g = math.gcd(g, s)
-    return g
+    return g
+
+def size_to_int(size):
+    return int(size[:-3]) * size_mul[size[-3]]
+
+def int_to_size(size):
+    for i,k in zip(range(40, 0, -10), size_key):
+        if size >= 1<<i:
+            return f'{size>>i}{k}iB'
```

### Comparing `hcpdiff-0.4.1/hcpdiff/visualizer.py` & `hcpdiff-0.4.2/hcpdiff/visualizer.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,73 +1,146 @@
 import argparse
 import os
 import sys
+import time
 
 import hydra
+import numpy as np
 import torch
+from PIL import Image
+from accelerate import infer_auto_device_map, dispatch_model
 from diffusers import StableDiffusionPipeline, StableDiffusionImg2ImgPipeline, UNet2DConditionModel
-from diffusers.utils.import_utils import is_xformers_available
 from diffusers.utils import PIL_INTERPOLATION
+from diffusers.utils.import_utils import is_xformers_available
 from matplotlib import pyplot as plt
 from omegaconf import OmegaConf
+from torch.cuda.amp import autocast
 
-from hcpdiff.models import EmbeddingPTHook, TEEXHook, TokenizerHook
+from hcpdiff.models import EmbeddingPTHook, TEEXHook, TokenizerHook, LoraBlock
 from hcpdiff.utils.cfg_net_tools import load_hcpdiff, make_plugin
-from hcpdiff.utils.utils import to_validate_file, load_config_with_cli, load_config
 from hcpdiff.utils.img_size_tool import types_support
-from torch.cuda.amp import autocast
-from PIL import Image
-import numpy as np
+from hcpdiff.utils.net_utils import to_cpu, to_cuda
+from hcpdiff.utils.utils import to_validate_file, load_config_with_cli, load_config, size_to_int, int_to_size
 
-class UnetHook(): # for controlnet
+class UnetHook():  # for controlnet
     def __init__(self, unet):
         self.unet = unet
         self.call_raw = UNet2DConditionModel.__call__
         UNet2DConditionModel.__call__ = self.unet_call
 
     def unet_call(self, sample, timestep, encoder_hidden_states, **kwargs):
         return self.call_raw(self.unet, sample, timestep, encoder_hidden_states)
 
 class Visualizer:
+    dtype_dict = {'fp32':torch.float32, 'amp':torch.float32, 'fp16':torch.float16}
+
     def __init__(self, cfgs):
         self.cfgs_raw = cfgs
         self.cfgs = hydra.utils.instantiate(self.cfgs_raw)
         self.cfg_merge = self.cfgs.merge
+        self.offload = 'offload' in self.cfgs and self.cfgs.offload is not None
+
+        self.dtype = self.dtype_dict[self.cfgs.dtype]
 
         pipeline = self.get_pipeline()
-        comp = pipeline.from_pretrained(self.cfgs.pretrained_model, safety_checker=None, requires_safety_checker=False).components
+        comp = pipeline.from_pretrained(self.cfgs.pretrained_model, safety_checker=None, requires_safety_checker=False,
+                                        torch_dtype=self.dtype).components
         comp.update(self.cfgs.new_components)
         self.pipe = pipeline(**comp)
 
         if self.cfg_merge:
             self.merge_model()
 
-        self.pipe = self.pipe.to("cuda")
+        self.pipe = self.pipe.to(torch_dtype=self.dtype)
+
+        if 'save_model' in self.cfgs and self.cfgs.save_model is not None:
+            self.save_model(self.cfgs.save_model)
+            os._exit(0)
+
+        if self.offload:
+            self.build_offload(self.cfgs.offload)
+        else:
+            self.pipe.unet.to('cuda')
+
+            def decode_latents_offload(latents, decode_latents_raw=self.pipe.decode_latents):
+                to_cpu(self.pipe.unet)
+
+                self.pipe.vae.to('cuda')
+                res = decode_latents_raw(latents)
+                to_cpu(self.pipe.vae)
+
+                self.pipe.unet.to('cuda')
+                return res
+
+            self.pipe.decode_latents = decode_latents_offload
+
         emb, _ = EmbeddingPTHook.hook_from_dir(self.cfgs.emb_dir, self.pipe.tokenizer, self.pipe.text_encoder, N_repeats=self.cfgs.N_repeats)
         self.te_hook = TEEXHook.hook_pipe(self.pipe, N_repeats=self.cfgs.N_repeats, clip_skip=self.cfgs.clip_skip)
         self.token_ex = TokenizerHook(self.pipe.tokenizer)
         UnetHook(self.pipe.unet)
 
         if is_xformers_available():
             self.pipe.unet.enable_xformers_memory_efficient_attention()
             # self.te_hook.enable_xformers()
 
+    def save_model(self, save_cfg):
+        for k,v in self.pipe.unet.named_modules():
+            if isinstance(v, LoraBlock):
+                v.reparameterization_to_host()
+                v.remove()
+        for k,v in self.pipe.text_encoder.named_modules():
+            if isinstance(v, LoraBlock):
+                v.reparameterization_to_host()
+                v.remove()
+
+        self.pipe.save_pretrained(save_cfg.path, safe_serialization=save_cfg.to_safetensors)
+
     def get_pipeline(self):
         if self.cfgs.condition is None:
-            return StableDiffusionPipeline
+            pipe_cls = StableDiffusionPipeline
         else:
-            if self.cfgs.condition.type=='i2i':
-                return StableDiffusionImg2ImgPipeline
-            elif self.cfgs.condition.type=='controlnet':
-                return StableDiffusionPipeline
+            if self.cfgs.condition.type == 'i2i':
+                pipe_cls = StableDiffusionImg2ImgPipeline
+            elif self.cfgs.condition.type == 'controlnet':
+                pipe_cls = StableDiffusionPipeline
             else:
                 raise NotImplementedError(f'No condition type named {self.cfgs.condition.type}')
 
+        class CUDAPipe(pipe_cls):
+            @property
+            def _execution_device(self):
+                return torch.device('cuda')
+        return CUDAPipe
+
+    def build_offload(self, offload_cfg):
+        vram = size_to_int(offload_cfg.max_VRAM)
+        device_map = infer_auto_device_map(self.pipe.unet, max_memory={0:int_to_size(vram >> 1), "cpu":offload_cfg.max_RAM}, dtype=self.dtype)
+        self.pipe.unet = dispatch_model(self.pipe.unet, device_map)
+        if not offload_cfg.vae_cpu:
+            device_map = infer_auto_device_map(self.pipe.vae, max_memory={0:int_to_size(vram >> 5), "cpu":offload_cfg.max_RAM}, dtype=self.dtype)
+            self.pipe.vae = dispatch_model(self.pipe.vae, device_map)
+
+        def decode_latents_offload(latents, decode_latents_raw=self.pipe.decode_latents):
+            to_cpu(self.pipe.unet)
+
+            if offload_cfg.vae_cpu:
+                self.pipe.vae.to(dtype=torch.float32)
+                res = decode_latents_raw(latents.cpu().to(dtype=torch.float32))
+            else:
+                to_cuda(self.pipe.vae)
+                res = decode_latents_raw(latents)
+
+            to_cpu(self.pipe.vae)
+            to_cuda(self.pipe.unet)
+            return res
+
+        self.pipe.decode_latents = decode_latents_offload
+
     def merge_model(self):
-        if 'plugin_cfg' in self.cfg_merge: # Build plugins
+        if 'plugin_cfg' in self.cfg_merge:  # Build plugins
             plugin_cfg = hydra.utils.instantiate(load_config(self.cfg_merge.plugin_cfg))
             make_plugin(self.pipe.unet, plugin_cfg.plugin_unet)
             make_plugin(self.pipe.text_encoder, plugin_cfg.plugin_TE)
 
         for cfg_group in self.cfg_merge.values():
             if hasattr(cfg_group, 'type'):
                 if cfg_group.type == 'unet':
@@ -84,15 +157,15 @@
                 image = [image]
 
             if isinstance(image[0], Image.Image):
                 image = [
                     np.array(i.resize((width, height), resample=PIL_INTERPOLATION["lanczos"]))[None, :] for i in image
                 ]
                 image = np.concatenate(image, axis=0)
-                image = np.array(image).astype(np.float32) / 255.0
+                image = np.array(image).astype(np.float32)/255.0
                 image = image.transpose(0, 3, 1, 2)
                 image = torch.from_numpy(image)
             elif isinstance(image[0], torch.Tensor):
                 image = torch.cat(image, dim=0)
 
         image = image.repeat_interleave(batch_size, dim=0)
         image = image.to(device=device)
@@ -106,58 +179,62 @@
             ex_input_dict['cond'] = self.prepare_cond_image(img, self.cfgs.infer_args.width, self.cfgs.infer_args.height, self.cfgs.bs*2, 'cuda')
         return ex_input_dict
 
     @torch.no_grad()
     def vis_images(self, prompt, negative_prompt='', **kwargs):
         ex_input_dict = self.get_ex_input()
 
+        to_cuda(self.pipe.text_encoder)
+
         mult_p, clean_text_p = self.token_ex.parse_attn_mult(prompt)
         mult_n, clean_text_n = self.token_ex.parse_attn_mult(negative_prompt)
-        with autocast(enabled=self.cfgs.fp16):
+        with autocast(enabled=self.cfgs.dtype == 'amp'):
             emb_n, emb_p = self.te_hook.encode_prompt_to_emb(clean_text_n+clean_text_p).chunk(2)
             emb_p = self.te_hook.mult_attn(emb_p, mult_p)
             emb_n = self.te_hook.mult_attn(emb_n, mult_n)
 
+            to_cpu(self.pipe.text_encoder)
+            to_cuda(self.pipe.unet)
+
             if hasattr(self.pipe.unet, 'input_feeder'):
                 for feeder in self.pipe.unet.input_feeder:
                     feeder(ex_input_dict)
 
             images = self.pipe(prompt_embeds=emb_p, negative_prompt_embeds=emb_n, **kwargs).images
         return images
 
     def save_images(self, images, root, prompt, negative_prompt='', save_cfg=True):
         os.makedirs(root, exist_ok=True)
-        num_img_exist = max([0]+[int(x.split('-', 1)[0]) for x in os.listdir(root) if x.rsplit('.', 1)[-1] in types_support]) + 1
+        num_img_exist = max([0]+[int(x.split('-', 1)[0]) for x in os.listdir(root) if x.rsplit('.', 1)[-1] in types_support])+1
 
         for p, pn, img in zip(prompt, negative_prompt, images):
             img.save(os.path.join(root, f"{num_img_exist}-{to_validate_file(prompt[0])}.{self.cfgs.save.image_type}"), quality=self.cfgs.save.quality)
 
             if save_cfg:
                 with open(os.path.join(root, f"{num_img_exist}-info.yaml"), 'w', encoding='utf-8') as f:
                     f.write(OmegaConf.to_yaml(self.cfgs_raw))
             num_img_exist += 1
 
     def vis_to_dir(self, root, prompt, negative_prompt='', save_cfg=True, **kwargs):
         images = self.vis_images(prompt, negative_prompt, **kwargs)
         self.save_images(images, root, prompt, negative_prompt, save_cfg=save_cfg)
 
     def show_latent(self, prompt, negative_prompt='', **kwargs):
-        emb_n, emb_p = self.te_hook.encode_prompt_to_emb(negative_prompt + prompt).chunk(2)
+        emb_n, emb_p = self.te_hook.encode_prompt_to_emb(negative_prompt+prompt).chunk(2)
         emb_p = self.te_hook.mult_attn(emb_p, self.token_ex.parse_attn_mult(prompt))
         emb_n = self.te_hook.mult_attn(emb_n, self.token_ex.parse_attn_mult(negative_prompt))
         images = self.pipe(prompt_embeds=emb_p, negative_prompt_embeds=emb_n, output_type='latent', **kwargs).images
 
         for img in images:
             plt.figure()
             for i, feat in enumerate(img):
-                plt.subplot(221 + i)
+                plt.subplot(221+i)
                 plt.imshow(feat)
             plt.show()
 
-
 if __name__ == '__main__':
     parser = argparse.ArgumentParser(description='Stable Diffusion Training')
     parser.add_argument('--cfg', type=str, default='')
     args, _ = parser.parse_known_args()
     cfgs = load_config_with_cli(args.cfg, args_list=sys.argv[3:])  # skip --cfg
 
     os.makedirs(cfgs.out_dir, exist_ok=True)
@@ -165,9 +242,9 @@
         G = torch.Generator()
         G.manual_seed(cfgs.seed)
     else:
         G = None
 
     viser = Visualizer(cfgs)
     for i in range(cfgs.num):
-        viser.vis_to_dir(cfgs.out_dir, prompt=[cfgs.prompt] * cfgs.bs, negative_prompt=[cfgs.neg_prompt] * cfgs.bs,
+        viser.vis_to_dir(cfgs.out_dir, prompt=[cfgs.prompt]*cfgs.bs, negative_prompt=[cfgs.neg_prompt]*cfgs.bs,
                          generator=G, save_cfg=cfgs.save.save_cfg, **cfgs.infer_args)
```

### Comparing `hcpdiff-0.4.1/hcpdiff.egg-info/PKG-INFO` & `hcpdiff-0.4.2/hcpdiff.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hcpdiff
-Version: 0.4.1
+Version: 0.4.2
 Summary: A universal Stable-Diffusion toolbox
 Home-page: https://github.com/7eu7d7/HCP-Diffusion
 Author: Ziyi Dong
 Author-email: dzy7eu7d7@gmail.com
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
```

### Comparing `hcpdiff-0.4.1/hcpdiff.egg-info/SOURCES.txt` & `hcpdiff-0.4.2/hcpdiff.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -4,17 +4,17 @@
 cfgs/deepspeed.json
 cfgs/te_struct.txt
 cfgs/unet_struct.txt
 cfgs/infer/change_vae.yaml
 cfgs/infer/euler_a.yaml
 cfgs/infer/img2img.yaml
 cfgs/infer/img2img_controlnet.yaml
+cfgs/infer/offload_2GB.yaml
 cfgs/infer/text2img.yaml
 cfgs/infer/text2img_DA++.yaml
-cfgs/infer/webui_model_infer.yaml
 cfgs/plugins/plugin_controlnet.yaml
 cfgs/train/train_base.yaml
 cfgs/train/tuning_base.yaml
 cfgs/train/examples/CustomDiffusion.yaml
 cfgs/train/examples/DreamArtist++.yaml
 cfgs/train/examples/DreamArtist.yaml
 cfgs/train/examples/DreamBooth.yaml
```

### Comparing `hcpdiff-0.4.1/prompt_tuning_template/object.txt` & `hcpdiff-0.4.2/prompt_tuning_template/object.txt`

 * *Files identical despite different names*

### Comparing `hcpdiff-0.4.1/prompt_tuning_template/object_caption.txt` & `hcpdiff-0.4.2/prompt_tuning_template/object_caption.txt`

 * *Files identical despite different names*

### Comparing `hcpdiff-0.4.1/prompt_tuning_template/style.txt` & `hcpdiff-0.4.2/prompt_tuning_template/style.txt`

 * *Files identical despite different names*

### Comparing `hcpdiff-0.4.1/prompt_tuning_template/style_caption.txt` & `hcpdiff-0.4.2/prompt_tuning_template/style_caption.txt`

 * *Files identical despite different names*

### Comparing `hcpdiff-0.4.1/setup.py` & `hcpdiff-0.4.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
             file_dict[prefix+root].append(os.path.join(root, name))
     return [(k, v) for k, v in file_dict.items()]
 
 
 setuptools.setup(
     name="hcpdiff",
     py_modules=["hcpdiff"],
-    version="0.4.1",
+    version="0.4.2",
     author="Ziyi Dong",
     author_email="dzy7eu7d7@gmail.com",
     description="A universal Stable-Diffusion toolbox",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/7eu7d7/HCP-Diffusion",
     packages=setuptools.find_packages(),
```

