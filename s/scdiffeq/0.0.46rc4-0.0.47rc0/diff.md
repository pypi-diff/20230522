# Comparing `tmp/scdiffeq-0.0.46rc4.tar.gz` & `tmp/scdiffeq-0.0.47rc0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scdiffeq-0.0.46rc4.tar", last modified: Fri May 12 17:29:32 2023, max compression
+gzip compressed data, was "scdiffeq-0.0.47rc0.tar", last modified: Mon May 22 14:23:11 2023, max compression
```

## Comparing `scdiffeq-0.0.46rc4.tar` & `scdiffeq-0.0.47rc0.tar`

### file list

```diff
@@ -1,107 +1,113 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 17:29:32.536421 scdiffeq-0.0.46rc4/
--rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-05-12 17:29:22.000000 scdiffeq-0.0.46rc4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2299 2023-05-12 17:29:32.536421 scdiffeq-0.0.46rc4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1627 2023-05-12 17:29:22.000000 scdiffeq-0.0.46rc4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 17:29:32.528421 scdiffeq-0.0.46rc4/scdiffeq/
--rw-r--r--   0 runner    (1001) docker     (123)      682 2023-05-12 17:29:22.000000 scdiffeq-0.0.46rc4/scdiffeq/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 17:29:32.532421 scdiffeq-0.0.46rc4/scdiffeq/core/
--rw-r--r--   0 runner    (1001) docker     (123)      585 2023-05-12 17:29:22.000000 scdiffeq-0.0.46rc4/scdiffeq/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14467 2023-05-12 17:29:22.000000 scdiffeq-0.0.46rc4/scdiffeq/core/_scdiffeq.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 17:29:32.532421 scdiffeq-0.0.46rc4/scdiffeq/core/callbacks/
--rw-r--r--   0 runner    (1001) docker     (123)      711 2023-05-12 17:29:22.000000 scdiffeq-0.0.46rc4/scdiffeq/core/callbacks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      271 2023-05-12 17:29:22.000000 scdiffeq-0.0.46rc4/scdiffeq/core/callbacks/_gradient_potential_callback.py
--rw-r--r--   0 runner    (1001) docker     (123)      834 2023-05-12 17:29:22.000000 scdiffeq-0.0.46rc4/scdiffeq/core/callbacks/_intermittent_saves.py
--rw-r--r--   0 runner    (1001) docker     (123)     4853 2023-05-12 17:29:22.000000 scdiffeq-0.0.46rc4/scdiffeq/core/callbacks/_loss_accounting.py
--rw-r--r--   0 runner    (1001) docker     (123)      806 2023-05-12 17:29:22.000000 scdiffeq-0.0.46rc4/scdiffeq/core/callbacks/_testing.py
--rw-r--r--   0 runner    (1001) docker     (123)     5319 2023-05-12 17:29:22.000000 scdiffeq-0.0.46rc4/scdiffeq/core/callbacks/_visualize_predictions.py
--rw-r--r--   0 runner    (1001) docker     (123)     8078 2023-05-12 17:29:22.000000 scdiffeq-0.0.46rc4/scdiffeq/core/callbacks/_visualize_tracked_loss.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 17:29:32.532421 scdiffeq-0.0.46rc4/scdiffeq/core/configs/
--rw-r--r--   0 runner    (1001) docker     (123)      488 2023-05-12 17:29:22.000000 scdiffeq-0.0.46rc4/scdiffeq/core/configs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2178 2023-05-12 17:29:22.000000 scdiffeq-0.0.46rc4/scdiffeq/core/configs/_function_credentialling.py
--rw-r--r--   0 runner    (1001) docker     (123)     2183 2023-05-12 17:29:22.000000 scdiffeq-0.0.46rc4/scdiffeq/core/configs/_lightning_callbacks_configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)     2073 2023-05-12 17:29:22.000000 scdiffeq-0.0.46rc4/scdiffeq/core/configs/_lightning_data_configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)     5708 2023-05-12 17:29:22.000000 scdiffeq-0.0.46rc4/scdiffeq/core/configs/_lightning_model_configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)     2140 2023-05-12 17:29:22.000000 scdiffeq-0.0.46rc4/scdiffeq/core/configs/_lightning_model_configuration_v2.py
--rw-r--r--   0 runner    (1001) docker     (123)     6701 2023-05-12 17:29:22.000000 scdiffeq-0.0.46rc4/scdiffeq/core/configs/_lightning_trainer_configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)    10716 2023-05-12 17:29:22.000000 scdiffeq-0.0.46rc4/scdiffeq/core/configs/_time_configuration.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 17:29:32.532421 scdiffeq-0.0.46rc4/scdiffeq/core/lightning_models/
--rw-r--r--   0 runner    (1001) docker     (123)     1229 2023-05-12 17:29:22.000000 scdiffeq-0.0.46rc4/scdiffeq/core/lightning_models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1554 2023-05-12 17:29:22.000000 scdiffeq-0.0.46rc4/scdiffeq/core/lightning_models/_lightning_ode.py
--rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-05-12 17:29:22.000000 scdiffeq-0.0.46rc4/scdiffeq/core/lightning_models/_lightning_ode_fixed_potential.py
--rw-r--r--   0 runner    (1001) docker     (123)     2351 2023-05-12 17:29:22.000000 scdiffeq-0.0.46rc4/scdiffeq/core/lightning_models/_lightning_ode_prior_potential.py
--rw-r--r--   0 runner    (1001) docker     (123)     2456 2023-05-12 17:29:22.000000 scdiffeq-0.0.46rc4/scdiffeq/core/lightning_models/_lightning_ode_vae.py
--rw-r--r--   0 runner    (1001) docker     (123)     2277 2023-05-12 17:29:22.000000 scdiffeq-0.0.46rc4/scdiffeq/core/lightning_models/_lightning_ode_vae_fixed_potential.py
--rw-r--r--   0 runner    (1001) docker     (123)     3052 2023-05-12 17:29:22.000000 scdiffeq-0.0.46rc4/scdiffeq/core/lightning_models/_lightning_ode_vae_prior_potential.py
--rw-r--r--   0 runner    (1001) docker     (123)     1768 2023-05-12 17:29:22.000000 scdiffeq-0.0.46rc4/scdiffeq/core/lightning_models/_lightning_sde.py
--rw-r--r--   0 runner    (1001) docker     (123)     2253 2023-05-12 17:29:22.000000 scdiffeq-0.0.46rc4/scdiffeq/core/lightning_models/_lightning_sde_fate_bias_aware.py
--rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-05-12 17:29:22.000000 scdiffeq-0.0.46rc4/scdiffeq/core/lightning_models/_lightning_sde_fixed_potential.py
--rw-r--r--   0 runner    (1001) docker     (123)     2550 2023-05-12 17:29:22.000000 scdiffeq-0.0.46rc4/scdiffeq/core/lightning_models/_lightning_sde_prior_potential.py
--rw-r--r--   0 runner    (1001) docker     (123)     2837 2023-05-12 17:29:22.000000 scdiffeq-0.0.46rc4/scdiffeq/core/lightning_models/_lightning_sde_vae.py
--rw-r--r--   0 runner    (1001) docker     (123)     3398 2023-05-12 17:29:22.000000 scdiffeq-0.0.46rc4/scdiffeq/core/lightning_models/_lightning_sde_vae_fate_bias_aware.py
--rw-r--r--   0 runner    (1001) docker     (123)     3044 2023-05-12 17:29:22.000000 scdiffeq-0.0.46rc4/scdiffeq/core/lightning_models/_lightning_sde_vae_fixed_potential.py
--rw-r--r--   0 runner    (1001) docker     (123)     2909 2023-05-12 17:29:22.000000 scdiffeq-0.0.46rc4/scdiffeq/core/lightning_models/_lightning_sde_vae_prior_potential.py
--rw-r--r--   0 runner    (1001) docker     (123)     3226 2023-05-12 17:29:22.000000 scdiffeq-0.0.46rc4/scdiffeq/core/lightning_models/_lightning_sde_vae_prior_potential_fate_bias_aware.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 17:29:32.532421 scdiffeq-0.0.46rc4/scdiffeq/core/lightning_models/base/
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-05-12 17:29:22.000000 scdiffeq-0.0.46rc4/scdiffeq/core/lightning_models/base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3808 2023-05-12 17:29:22.000000 scdiffeq-0.0.46rc4/scdiffeq/core/lightning_models/base/_base_lightning_diffeq.py
--rw-r--r--   0 runner    (1001) docker     (123)     2458 2023-05-12 17:29:22.000000 scdiffeq-0.0.46rc4/scdiffeq/core/lightning_models/base/_batch_processor.py
--rw-r--r--   0 runner    (1001) docker     (123)      752 2023-05-12 17:29:22.000000 scdiffeq-0.0.46rc4/scdiffeq/core/lightning_models/base/_sinkhorn_divergence.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 17:29:32.536421 scdiffeq-0.0.46rc4/scdiffeq/core/lightning_models/mix_ins/
--rw-r--r--   0 runner    (1001) docker     (123)      612 2023-05-12 17:29:22.000000 scdiffeq-0.0.46rc4/scdiffeq/core/lightning_models/mix_ins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      625 2023-05-12 17:29:22.000000 scdiffeq-0.0.46rc4/scdiffeq/core/lightning_models/mix_ins/_base_forward_mix_in.py
--rw-r--r--   0 runner    (1001) docker     (123)     2557 2023-05-12 17:29:22.000000 scdiffeq-0.0.46rc4/scdiffeq/core/lightning_models/mix_ins/_drift_prior_mix_in.py
--rw-r--r--   0 runner    (1001) docker     (123)     2583 2023-05-12 17:29:22.000000 scdiffeq-0.0.46rc4/scdiffeq/core/lightning_models/mix_ins/_fate_bias_drift_prior_mix_in.py
--rw-r--r--   0 runner    (1001) docker     (123)     2805 2023-05-12 17:29:22.000000 scdiffeq-0.0.46rc4/scdiffeq/core/lightning_models/mix_ins/_fate_bias_drift_prior_vae_mix_in.py
--rw-r--r--   0 runner    (1001) docker     (123)     2691 2023-05-12 17:29:22.000000 scdiffeq-0.0.46rc4/scdiffeq/core/lightning_models/mix_ins/_fate_bias_mix_in.py
--rw-r--r--   0 runner    (1001) docker     (123)     2822 2023-05-12 17:29:22.000000 scdiffeq-0.0.46rc4/scdiffeq/core/lightning_models/mix_ins/_fate_bias_vae_mix_in.py
--rw-r--r--   0 runner    (1001) docker     (123)      318 2023-05-12 17:29:22.000000 scdiffeq-0.0.46rc4/scdiffeq/core/lightning_models/mix_ins/_potential_mix_in.py
--rw-r--r--   0 runner    (1001) docker     (123)      941 2023-05-12 17:29:22.000000 scdiffeq-0.0.46rc4/scdiffeq/core/lightning_models/mix_ins/_pre_train_mix_in.py
--rw-r--r--   0 runner    (1001) docker     (123)     2264 2023-05-12 17:29:22.000000 scdiffeq-0.0.46rc4/scdiffeq/core/lightning_models/mix_ins/_sde_mix_in.py
--rw-r--r--   0 runner    (1001) docker     (123)     8342 2023-05-12 17:29:22.000000 scdiffeq-0.0.46rc4/scdiffeq/core/lightning_models/mix_ins/_vae_mix_in.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 17:29:32.536421 scdiffeq-0.0.46rc4/scdiffeq/core/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     1302 2023-05-12 17:29:22.000000 scdiffeq-0.0.46rc4/scdiffeq/core/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2018 2023-05-12 17:29:22.000000 scdiffeq-0.0.46rc4/scdiffeq/core/utils/_abc_parse.py
--rw-r--r--   0 runner    (1001) docker     (123)      931 2023-05-12 17:29:22.000000 scdiffeq-0.0.46rc4/scdiffeq/core/utils/_anndata_inspector.py
--rw-r--r--   0 runner    (1001) docker     (123)     2802 2023-05-12 17:29:22.000000 scdiffeq-0.0.46rc4/scdiffeq/core/utils/_autoparse_base_class.py
--rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-05-12 17:29:22.000000 scdiffeq-0.0.46rc4/scdiffeq/core/utils/_default_neural_sde.py
--rw-r--r--   0 runner    (1001) docker     (123)      307 2023-05-12 17:29:22.000000 scdiffeq-0.0.46rc4/scdiffeq/core/utils/_display_tracked_loss.py
--rw-r--r--   0 runner    (1001) docker     (123)     2011 2023-05-12 17:29:22.000000 scdiffeq-0.0.46rc4/scdiffeq/core/utils/_fast_graph.py
--rw-r--r--   0 runner    (1001) docker     (123)      333 2023-05-12 17:29:22.000000 scdiffeq-0.0.46rc4/scdiffeq/core/utils/_fetch_format.py
--rw-r--r--   0 runner    (1001) docker     (123)     2381 2023-05-12 17:29:22.000000 scdiffeq-0.0.46rc4/scdiffeq/core/utils/_filter_df.py
--rw-r--r--   0 runner    (1001) docker     (123)     1652 2023-05-12 17:29:22.000000 scdiffeq-0.0.46rc4/scdiffeq/core/utils/_function_fetch.py
--rw-r--r--   0 runner    (1001) docker     (123)     3402 2023-05-12 17:29:22.000000 scdiffeq-0.0.46rc4/scdiffeq/core/utils/_function_kwargs.py
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-05-12 17:29:22.000000 scdiffeq-0.0.46rc4/scdiffeq/core/utils/_idx_to_int_str.py
--rw-r--r--   0 runner    (1001) docker     (123)      341 2023-05-12 17:29:22.000000 scdiffeq-0.0.46rc4/scdiffeq/core/utils/_info_message.py
--rw-r--r--   0 runner    (1001) docker     (123)     2147 2023-05-12 17:29:22.000000 scdiffeq-0.0.46rc4/scdiffeq/core/utils/_knn_graph_query.py
--rw-r--r--   0 runner    (1001) docker     (123)      892 2023-05-12 17:29:22.000000 scdiffeq-0.0.46rc4/scdiffeq/core/utils/_logging_learnable_hparams.py
--rw-r--r--   0 runner    (1001) docker     (123)     6521 2023-05-12 17:29:22.000000 scdiffeq-0.0.46rc4/scdiffeq/core/utils/_logs.py
--rw-r--r--   0 runner    (1001) docker     (123)      395 2023-05-12 17:29:22.000000 scdiffeq-0.0.46rc4/scdiffeq/core/utils/_normalize_time_to_range.py
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-05-12 17:29:22.000000 scdiffeq-0.0.46rc4/scdiffeq/core/utils/_not_none_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     2339 2023-05-12 17:29:22.000000 scdiffeq-0.0.46rc4/scdiffeq/core/utils/_scdiffeq_logger.py
--rw-r--r--   0 runner    (1001) docker     (123)      346 2023-05-12 17:29:22.000000 scdiffeq-0.0.46rc4/scdiffeq/core/utils/_sum_normalize.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 17:29:32.536421 scdiffeq-0.0.46rc4/scdiffeq/io/
--rw-r--r--   0 runner    (1001) docker     (123)      541 2023-05-12 17:29:22.000000 scdiffeq-0.0.46rc4/scdiffeq/io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      744 2023-05-12 17:29:22.000000 scdiffeq-0.0.46rc4/scdiffeq/io/_pickle_io.py
--rw-r--r--   0 runner    (1001) docker     (123)     1258 2023-05-12 17:29:22.000000 scdiffeq-0.0.46rc4/scdiffeq/io/_read_h5ad.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 17:29:32.536421 scdiffeq-0.0.46rc4/scdiffeq/plotting/
--rw-r--r--   0 runner    (1001) docker     (123)      462 2023-05-12 17:29:22.000000 scdiffeq-0.0.46rc4/scdiffeq/plotting/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 17:29:32.536421 scdiffeq-0.0.46rc4/scdiffeq/tools/
--rw-r--r--   0 runner    (1001) docker     (123)      924 2023-05-12 17:29:22.000000 scdiffeq-0.0.46rc4/scdiffeq/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1482 2023-05-12 17:29:22.000000 scdiffeq-0.0.46rc4/scdiffeq/tools/_annotate_cells.py
--rw-r--r--   0 runner    (1001) docker     (123)     4607 2023-05-12 17:29:22.000000 scdiffeq-0.0.46rc4/scdiffeq/tools/_dimension_reduction.py
--rw-r--r--   0 runner    (1001) docker     (123)     1546 2023-05-12 17:29:22.000000 scdiffeq-0.0.46rc4/scdiffeq/tools/_drift_diffusion_state_characterization.py
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-05-12 17:29:22.000000 scdiffeq-0.0.46rc4/scdiffeq/tools/_fetch.py
--rw-r--r--   0 runner    (1001) docker     (123)     1292 2023-05-12 17:29:22.000000 scdiffeq-0.0.46rc4/scdiffeq/tools/_func_from_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     1019 2023-05-12 17:29:22.000000 scdiffeq-0.0.46rc4/scdiffeq/tools/_hyperparams.py
--rw-r--r--   0 runner    (1001) docker     (123)     5462 2023-05-12 17:29:22.000000 scdiffeq-0.0.46rc4/scdiffeq/tools/_reconstruct_function.py
--rw-r--r--   0 runner    (1001) docker     (123)     1470 2023-05-12 17:29:22.000000 scdiffeq-0.0.46rc4/scdiffeq/tools/_time_free_sampling.py
--rw-r--r--   0 runner    (1001) docker     (123)      853 2023-05-12 17:29:22.000000 scdiffeq-0.0.46rc4/scdiffeq/tools/_umap.py
--rw-r--r--   0 runner    (1001) docker     (123)     1242 2023-05-12 17:29:22.000000 scdiffeq-0.0.46rc4/scdiffeq/tools/_versions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 17:29:32.532421 scdiffeq-0.0.46rc4/scdiffeq.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2299 2023-05-12 17:29:32.000000 scdiffeq-0.0.46rc4/scdiffeq.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4172 2023-05-12 17:29:32.000000 scdiffeq-0.0.46rc4/scdiffeq.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-12 17:29:32.000000 scdiffeq-0.0.46rc4/scdiffeq.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      306 2023-05-12 17:29:32.000000 scdiffeq-0.0.46rc4/scdiffeq.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-12 17:29:32.000000 scdiffeq-0.0.46rc4/scdiffeq.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-12 17:29:32.536421 scdiffeq-0.0.46rc4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1404 2023-05-12 17:29:22.000000 scdiffeq-0.0.46rc4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 14:23:11.498330 scdiffeq-0.0.47rc0/
+-rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-05-22 14:23:00.000000 scdiffeq-0.0.47rc0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2299 2023-05-22 14:23:11.498330 scdiffeq-0.0.47rc0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1627 2023-05-22 14:23:00.000000 scdiffeq-0.0.47rc0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 14:23:11.490330 scdiffeq-0.0.47rc0/scdiffeq/
+-rw-r--r--   0 runner    (1001) docker     (123)      682 2023-05-22 14:23:00.000000 scdiffeq-0.0.47rc0/scdiffeq/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 14:23:11.490330 scdiffeq-0.0.47rc0/scdiffeq/core/
+-rw-r--r--   0 runner    (1001) docker     (123)      584 2023-05-22 14:23:00.000000 scdiffeq-0.0.47rc0/scdiffeq/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15908 2023-05-22 14:23:00.000000 scdiffeq-0.0.47rc0/scdiffeq/core/_scdiffeq.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 14:23:11.490330 scdiffeq-0.0.47rc0/scdiffeq/core/callbacks/
+-rw-r--r--   0 runner    (1001) docker     (123)      725 2023-05-22 14:23:00.000000 scdiffeq-0.0.47rc0/scdiffeq/core/callbacks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      271 2023-05-22 14:23:00.000000 scdiffeq-0.0.47rc0/scdiffeq/core/callbacks/_gradient_potential_callback.py
+-rw-r--r--   0 runner    (1001) docker     (123)      834 2023-05-22 14:23:00.000000 scdiffeq-0.0.47rc0/scdiffeq/core/callbacks/_intermittent_saves.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4853 2023-05-22 14:23:00.000000 scdiffeq-0.0.47rc0/scdiffeq/core/callbacks/_loss_accounting.py
+-rw-r--r--   0 runner    (1001) docker     (123)      806 2023-05-22 14:23:00.000000 scdiffeq-0.0.47rc0/scdiffeq/core/callbacks/_testing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5319 2023-05-22 14:23:00.000000 scdiffeq-0.0.47rc0/scdiffeq/core/callbacks/_visualize_predictions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8233 2023-05-22 14:23:00.000000 scdiffeq-0.0.47rc0/scdiffeq/core/callbacks/_visualize_tracked_loss.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 14:23:11.490330 scdiffeq-0.0.47rc0/scdiffeq/core/configs/
+-rw-r--r--   0 runner    (1001) docker     (123)      488 2023-05-22 14:23:00.000000 scdiffeq-0.0.47rc0/scdiffeq/core/configs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2210 2023-05-22 14:23:00.000000 scdiffeq-0.0.47rc0/scdiffeq/core/configs/_function_credentialling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2210 2023-05-22 14:23:00.000000 scdiffeq-0.0.47rc0/scdiffeq/core/configs/_lightning_callbacks_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2073 2023-05-22 14:23:00.000000 scdiffeq-0.0.47rc0/scdiffeq/core/configs/_lightning_data_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5708 2023-05-22 14:23:00.000000 scdiffeq-0.0.47rc0/scdiffeq/core/configs/_lightning_model_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2140 2023-05-22 14:23:00.000000 scdiffeq-0.0.47rc0/scdiffeq/core/configs/_lightning_model_configuration_v2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6834 2023-05-22 14:23:00.000000 scdiffeq-0.0.47rc0/scdiffeq/core/configs/_lightning_trainer_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10716 2023-05-22 14:23:00.000000 scdiffeq-0.0.47rc0/scdiffeq/core/configs/_time_configuration.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 14:23:11.494330 scdiffeq-0.0.47rc0/scdiffeq/core/lightning_models/
+-rw-r--r--   0 runner    (1001) docker     (123)     1229 2023-05-22 14:23:00.000000 scdiffeq-0.0.47rc0/scdiffeq/core/lightning_models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1605 2023-05-22 14:23:00.000000 scdiffeq-0.0.47rc0/scdiffeq/core/lightning_models/_lightning_ode.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1694 2023-05-22 14:23:00.000000 scdiffeq-0.0.47rc0/scdiffeq/core/lightning_models/_lightning_ode_fixed_potential.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2420 2023-05-22 14:23:00.000000 scdiffeq-0.0.47rc0/scdiffeq/core/lightning_models/_lightning_ode_prior_potential.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2508 2023-05-22 14:23:00.000000 scdiffeq-0.0.47rc0/scdiffeq/core/lightning_models/_lightning_ode_vae.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2337 2023-05-22 14:23:00.000000 scdiffeq-0.0.47rc0/scdiffeq/core/lightning_models/_lightning_ode_vae_fixed_potential.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3121 2023-05-22 14:23:00.000000 scdiffeq-0.0.47rc0/scdiffeq/core/lightning_models/_lightning_ode_vae_prior_potential.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1827 2023-05-22 14:23:00.000000 scdiffeq-0.0.47rc0/scdiffeq/core/lightning_models/_lightning_sde.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2330 2023-05-22 14:23:00.000000 scdiffeq-0.0.47rc0/scdiffeq/core/lightning_models/_lightning_sde_fate_bias_aware.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1732 2023-05-22 14:23:00.000000 scdiffeq-0.0.47rc0/scdiffeq/core/lightning_models/_lightning_sde_fixed_potential.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2677 2023-05-22 14:23:00.000000 scdiffeq-0.0.47rc0/scdiffeq/core/lightning_models/_lightning_sde_prior_potential.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2936 2023-05-22 14:23:00.000000 scdiffeq-0.0.47rc0/scdiffeq/core/lightning_models/_lightning_sde_vae.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3468 2023-05-22 14:23:00.000000 scdiffeq-0.0.47rc0/scdiffeq/core/lightning_models/_lightning_sde_vae_fate_bias_aware.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3113 2023-05-22 14:23:00.000000 scdiffeq-0.0.47rc0/scdiffeq/core/lightning_models/_lightning_sde_vae_fixed_potential.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2977 2023-05-22 14:23:00.000000 scdiffeq-0.0.47rc0/scdiffeq/core/lightning_models/_lightning_sde_vae_prior_potential.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3295 2023-05-22 14:23:00.000000 scdiffeq-0.0.47rc0/scdiffeq/core/lightning_models/_lightning_sde_vae_prior_potential_fate_bias_aware.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 14:23:11.494330 scdiffeq-0.0.47rc0/scdiffeq/core/lightning_models/base/
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-05-22 14:23:00.000000 scdiffeq-0.0.47rc0/scdiffeq/core/lightning_models/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4385 2023-05-22 14:23:00.000000 scdiffeq-0.0.47rc0/scdiffeq/core/lightning_models/base/_base_lightning_diffeq.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2458 2023-05-22 14:23:00.000000 scdiffeq-0.0.47rc0/scdiffeq/core/lightning_models/base/_batch_processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      752 2023-05-22 14:23:00.000000 scdiffeq-0.0.47rc0/scdiffeq/core/lightning_models/base/_sinkhorn_divergence.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 14:23:11.494330 scdiffeq-0.0.47rc0/scdiffeq/core/lightning_models/mix_ins/
+-rw-r--r--   0 runner    (1001) docker     (123)      612 2023-05-22 14:23:00.000000 scdiffeq-0.0.47rc0/scdiffeq/core/lightning_models/mix_ins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      647 2023-05-22 14:23:00.000000 scdiffeq-0.0.47rc0/scdiffeq/core/lightning_models/mix_ins/_base_forward_mix_in.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2535 2023-05-22 14:23:00.000000 scdiffeq-0.0.47rc0/scdiffeq/core/lightning_models/mix_ins/_drift_prior_mix_in.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2583 2023-05-22 14:23:00.000000 scdiffeq-0.0.47rc0/scdiffeq/core/lightning_models/mix_ins/_fate_bias_drift_prior_mix_in.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2805 2023-05-22 14:23:00.000000 scdiffeq-0.0.47rc0/scdiffeq/core/lightning_models/mix_ins/_fate_bias_drift_prior_vae_mix_in.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2691 2023-05-22 14:23:00.000000 scdiffeq-0.0.47rc0/scdiffeq/core/lightning_models/mix_ins/_fate_bias_mix_in.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2822 2023-05-22 14:23:00.000000 scdiffeq-0.0.47rc0/scdiffeq/core/lightning_models/mix_ins/_fate_bias_vae_mix_in.py
+-rw-r--r--   0 runner    (1001) docker     (123)      318 2023-05-22 14:23:00.000000 scdiffeq-0.0.47rc0/scdiffeq/core/lightning_models/mix_ins/_potential_mix_in.py
+-rw-r--r--   0 runner    (1001) docker     (123)      941 2023-05-22 14:23:00.000000 scdiffeq-0.0.47rc0/scdiffeq/core/lightning_models/mix_ins/_pre_train_mix_in.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2264 2023-05-22 14:23:00.000000 scdiffeq-0.0.47rc0/scdiffeq/core/lightning_models/mix_ins/_sde_mix_in.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4898 2023-05-22 14:23:00.000000 scdiffeq-0.0.47rc0/scdiffeq/core/lightning_models/mix_ins/_vae_mix_in.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 14:23:11.498330 scdiffeq-0.0.47rc0/scdiffeq/core/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     1366 2023-05-22 14:23:00.000000 scdiffeq-0.0.47rc0/scdiffeq/core/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2018 2023-05-22 14:23:00.000000 scdiffeq-0.0.47rc0/scdiffeq/core/utils/_abc_parse.py
+-rw-r--r--   0 runner    (1001) docker     (123)      931 2023-05-22 14:23:00.000000 scdiffeq-0.0.47rc0/scdiffeq/core/utils/_anndata_inspector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2802 2023-05-22 14:23:00.000000 scdiffeq-0.0.47rc0/scdiffeq/core/utils/_autoparse_base_class.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-05-22 14:23:00.000000 scdiffeq-0.0.47rc0/scdiffeq/core/utils/_default_neural_sde.py
+-rw-r--r--   0 runner    (1001) docker     (123)      307 2023-05-22 14:23:00.000000 scdiffeq-0.0.47rc0/scdiffeq/core/utils/_display_tracked_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2011 2023-05-22 14:23:00.000000 scdiffeq-0.0.47rc0/scdiffeq/core/utils/_fast_graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)      333 2023-05-22 14:23:00.000000 scdiffeq-0.0.47rc0/scdiffeq/core/utils/_fetch_format.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2381 2023-05-22 14:23:00.000000 scdiffeq-0.0.47rc0/scdiffeq/core/utils/_filter_df.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2738 2023-05-22 14:23:00.000000 scdiffeq-0.0.47rc0/scdiffeq/core/utils/_flexible_component_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1652 2023-05-22 14:23:00.000000 scdiffeq-0.0.47rc0/scdiffeq/core/utils/_function_fetch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3402 2023-05-22 14:23:00.000000 scdiffeq-0.0.47rc0/scdiffeq/core/utils/_function_kwargs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      231 2023-05-22 14:23:00.000000 scdiffeq-0.0.47rc0/scdiffeq/core/utils/_idx_to_int_str.py
+-rw-r--r--   0 runner    (1001) docker     (123)      341 2023-05-22 14:23:00.000000 scdiffeq-0.0.47rc0/scdiffeq/core/utils/_info_message.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2147 2023-05-22 14:23:00.000000 scdiffeq-0.0.47rc0/scdiffeq/core/utils/_knn_graph_query.py
+-rw-r--r--   0 runner    (1001) docker     (123)      892 2023-05-22 14:23:00.000000 scdiffeq-0.0.47rc0/scdiffeq/core/utils/_logging_learnable_hparams.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6934 2023-05-22 14:23:00.000000 scdiffeq-0.0.47rc0/scdiffeq/core/utils/_logs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      395 2023-05-22 14:23:00.000000 scdiffeq-0.0.47rc0/scdiffeq/core/utils/_normalize_time_to_range.py
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-05-22 14:23:00.000000 scdiffeq-0.0.47rc0/scdiffeq/core/utils/_not_none_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2339 2023-05-22 14:23:00.000000 scdiffeq-0.0.47rc0/scdiffeq/core/utils/_scdiffeq_logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)      346 2023-05-22 14:23:00.000000 scdiffeq-0.0.47rc0/scdiffeq/core/utils/_sum_normalize.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 14:23:11.498330 scdiffeq-0.0.47rc0/scdiffeq/io/
+-rw-r--r--   0 runner    (1001) docker     (123)      541 2023-05-22 14:23:00.000000 scdiffeq-0.0.47rc0/scdiffeq/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      744 2023-05-22 14:23:00.000000 scdiffeq-0.0.47rc0/scdiffeq/io/_pickle_io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1258 2023-05-22 14:23:00.000000 scdiffeq-0.0.47rc0/scdiffeq/io/_read_h5ad.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 14:23:11.498330 scdiffeq-0.0.47rc0/scdiffeq/plotting/
+-rw-r--r--   0 runner    (1001) docker     (123)      462 2023-05-22 14:23:00.000000 scdiffeq-0.0.47rc0/scdiffeq/plotting/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 14:23:11.498330 scdiffeq-0.0.47rc0/scdiffeq/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)     1145 2023-05-22 14:23:00.000000 scdiffeq-0.0.47rc0/scdiffeq/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1482 2023-05-22 14:23:00.000000 scdiffeq-0.0.47rc0/scdiffeq/tools/_annotate_cells.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1446 2023-05-22 14:23:00.000000 scdiffeq-0.0.47rc0/scdiffeq/tools/_data_format.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4607 2023-05-22 14:23:00.000000 scdiffeq-0.0.47rc0/scdiffeq/tools/_dimension_reduction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1546 2023-05-22 14:23:00.000000 scdiffeq-0.0.47rc0/scdiffeq/tools/_drift_diffusion_state_characterization.py
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-05-22 14:23:00.000000 scdiffeq-0.0.47rc0/scdiffeq/tools/_fetch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1292 2023-05-22 14:23:00.000000 scdiffeq-0.0.47rc0/scdiffeq/tools/_func_from_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1019 2023-05-22 14:23:00.000000 scdiffeq-0.0.47rc0/scdiffeq/tools/_hyperparams.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3210 2023-05-22 14:23:00.000000 scdiffeq-0.0.47rc0/scdiffeq/tools/_knn.py
+-rw-r--r--   0 runner    (1001) docker     (123)      866 2023-05-22 14:23:00.000000 scdiffeq-0.0.47rc0/scdiffeq/tools/_negative_cross_entropy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5462 2023-05-22 14:23:00.000000 scdiffeq-0.0.47rc0/scdiffeq/tools/_reconstruct_function.py
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-05-22 14:23:00.000000 scdiffeq-0.0.47rc0/scdiffeq/tools/_sum_norm_df.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1470 2023-05-22 14:23:00.000000 scdiffeq-0.0.47rc0/scdiffeq/tools/_time_free_sampling.py
+-rw-r--r--   0 runner    (1001) docker     (123)      853 2023-05-22 14:23:00.000000 scdiffeq-0.0.47rc0/scdiffeq/tools/_umap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1242 2023-05-22 14:23:00.000000 scdiffeq-0.0.47rc0/scdiffeq/tools/_versions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3561 2023-05-22 14:23:00.000000 scdiffeq-0.0.47rc0/scdiffeq/tools/_x_use.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 14:23:11.490330 scdiffeq-0.0.47rc0/scdiffeq.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2299 2023-05-22 14:23:11.000000 scdiffeq-0.0.47rc0/scdiffeq.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4374 2023-05-22 14:23:11.000000 scdiffeq-0.0.47rc0/scdiffeq.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 14:23:11.000000 scdiffeq-0.0.47rc0/scdiffeq.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      306 2023-05-22 14:23:11.000000 scdiffeq-0.0.47rc0/scdiffeq.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-22 14:23:11.000000 scdiffeq-0.0.47rc0/scdiffeq.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-22 14:23:11.498330 scdiffeq-0.0.47rc0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1404 2023-05-22 14:23:00.000000 scdiffeq-0.0.47rc0/setup.py
```

### Comparing `scdiffeq-0.0.46rc4/LICENSE` & `scdiffeq-0.0.47rc0/LICENSE`

 * *Files identical despite different names*

### Comparing `scdiffeq-0.0.46rc4/PKG-INFO` & `scdiffeq-0.0.47rc0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scdiffeq
-Version: 0.0.46rc4
+Version: 0.0.47rc0
 Summary: scDiffEq: modelling single-cell dynamics using neural differential equations.
 Home-page: https://github.com/mvinyard/sc-neural-diffeqs
 Author: Michael E. Vinyard - Harvard University - Massachussetts General Hospital - Broad Institute of MIT and Harvard
 Author-email: mvinyard@broadinstitute.org
 License: MIT
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Programming Language :: Python :: 3.9
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: scdiffeq Version: 0.0.46rc4 Summary: scDiffEq:
+Metadata-Version: 2.1 Name: scdiffeq Version: 0.0.47rc0 Summary: scDiffEq:
 modelling single-cell dynamics using neural differential equations. Home-page:
 https://github.com/mvinyard/sc-neural-diffeqs Author: Michael E. Vinyard -
 Harvard University - Massachussetts General Hospital - Broad Institute of MIT
 and Harvard Author-email: mvinyard@broadinstitute.org License: MIT Classifier:
 Development Status :: 2 - Pre-Alpha Classifier: Programming Language :: Python
 :: 3.9 Classifier: Intended Audience :: Science/Research Classifier: Topic ::
 Scientific/Engineering :: Bio-Informatics Requires-Python: >3.9.0 Description-
```

### Comparing `scdiffeq-0.0.46rc4/README.md` & `scdiffeq-0.0.47rc0/README.md`

 * *Files identical despite different names*

### Comparing `scdiffeq-0.0.46rc4/scdiffeq/__init__.py` & `scdiffeq-0.0.47rc0/scdiffeq/core/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,23 +1,20 @@
 
 __module_name__ = "__init__.py"
-__version__ = __Version__ = "0.0.46rc4"
-__doc__ = """Top-level __init__ for the scdiffeq package."""
+__version__ = "0.0.46rc2"
+__doc__ = """Top-level __init__ for accessing the scDiffEq model."""
 __author__ = ", ".join(["Michael E. Vinyard", "Anders Rasmussen", "Ruitong Li"])
 __email__ = ", ".join(
     [
         "mvinyard@broadinstitute.org",
         "arasmuss@broadinstitute.org",
         "ruitong@broadinstitute.org",
     ]
 )
 
+# -- import models accessed as sdq.models.<MODEL>: ---------------------------------------
+from ._scdiffeq import scDiffEq
 
-# -- import model API: -------------------------------------------------------------------
-from .core._scdiffeq import scDiffEq
-
-
-# -- import sub-packages: ----------------------------------------------------------------
-from . import core
-from . import io
-from . import plotting as pl
-from . import tools as tl
+from . import lightning_models
+from . import utils
+from . import configs
+from . import callbacks
```

### Comparing `scdiffeq-0.0.46rc4/scdiffeq/core/_scdiffeq.py` & `scdiffeq-0.0.47rc0/scdiffeq/core/_scdiffeq.py`

 * *Files 14% similar despite different names*

```diff
@@ -7,34 +7,38 @@
 import pandas as pd
 import torch
 import glob
 import os
 
 
 # -- import local dependencies: ------------------------------------------------
-from . import configs, lightning_models, utils
-from .. import tools
+from . import configs, lightning_models, utils, callbacks
+from .. import tools, __version__
 
 
 # -- type setting: -------------------------------------------------------------
 from typing import Union, List
 NoneType = type(None)
 
+import warnings
+
+warnings.filterwarnings("ignore", ".*Consider increasing the value of the `num_workers` argument*")
 
 class scDiffEq(utils.ABCParse):
     def __init__(
         self,
         
         # -- data params: -------------------------------------------------------
         adata: anndata.AnnData,
         latent_dim: int = 20,
         model_name: str = "scDiffEq_model",
         use_key: str = "X_scaled",
         obs_keys: List[str] = ["W"],
         kNN_key: str = "X_pca_scDiffEq",
+        seed: int = 0,
         
         # -- pretrain params: ---------------------------------------------------
         pretrain_epochs: int = 500,
         pretrain_lr: float = 1e-3,
         pretrain_optimizer=torch.optim.Adam,
         pretrain_step_size: int = 100,
         pretrain_scheduler=torch.optim.lr_scheduler.StepLR,
@@ -50,22 +54,22 @@
         
         train_key: str = "train",
         val_key: str = "val",
         test_key: str = "test",
         predict_key: str = "predict",
         
         # -- general params: ----------------------------------------------------
-        seed: int = 617,
         num_workers: int = os.cpu_count(),
         silent: bool = True,
         scale_input_counts: bool = True,
         reduce_dimensions: bool = True,
         build_kNN: bool = True,
         fate_bias_csv_path: Union[str, NoneType] = None,
         fate_bias_multiplier: float = 1,
+        viz_frequency: int = 1,
         
         # -- time params: -------------------------------------------------------
         time_key: Union[str, NoneType] = None,
         t0_idx: Union[pd.Index, NoneType] = None,
         t_min: float = 0,
         t_max: float = 1,
         dt: float = 0.1,
@@ -110,21 +114,27 @@
         decoder_n_hidden: int = 4,
         decoder_power: float = 2,
         decoder_activation: Union[str, List[str]] = "LeakyReLU",
         decoder_dropout: Union[float, List[float]] = 0.2,
         decoder_bias: bool = True,
         decoder_output_bias: bool = True,
         
+        version: str = __version__,
+        
         *args,
         **kwargs,
     ):
         self.__config__(locals())
 
     def _configure_obs_idx(self):
-        if not self.adata.obs.index[0] == "1":
+        
+        self._PROVIDED_OBS_IDX = self.adata.obs.index
+        self._PROVIDED_VAR_IDX = self.adata.var.index
+        
+        if self.adata.obs.index[0] != "1":
             self.adata = utils.idx_to_int_str(self.adata)
         
         
     def _configure_data(self, kwargs):
 
         """Configure data (including time time)"""
         
@@ -156,35 +166,37 @@
         if self._reduce_dimensions:
             self.reducer.pca()
             self.adata.obsm["X_pca_scDiffEq"] = self.reducer.X_pca
             self.reducer.umap()
             self.adata.obsm["X_umap_scDiffEq"] = self.reducer.X_umap
 
     def _configure_logger(self):
+
         self.DiffEqLogger = utils.scDiffEqLogger(model_name=self._model_name)
         self.DiffEqLogger()
 
     def _configure_trainer_generator(self):
         
         self.TrainerGenerator = configs.LightningTrainerConfiguration(
             self.DiffEqLogger.versioned_model_outdir
         )
         self._PRETRAIN_CONFIG_COUNT = 0
         self._TRAIN_CONFIG_COUNT = 0
 
     def _configure_kNN_graph(self):
+        
+        # -- prep data: ------
         train_adata = self.adata[self.adata.obs[self._train_key]].copy()
         
-        train_adata.obs = train_adata.obs.reset_index(drop=True)
-        train_adata.obs.index = train_adata.obs.index.astype(str)
+        # -- doesn't seem necessary any longer: ------
+#         train_adata.obs = train_adata.obs.reset_index(drop=True)
+#         train_adata.obs.index = train_adata.obs.index.astype(str)
         
         self._INFO(f"Bulding Annoy kNN Graph on adata.obsm['{self._kNN_key}']")
-        self.kNN_Graph = utils.kNNGraphQuery(
-            adata=train_adata, use_key=self._kNN_key,
-        )
+        self.kNN_Graph = tools.kNN(adata = train_adata, use_key = self._kNN_key)
 
     def _configure_model(self, kwargs):
 
         self._LitModelConfig = configs.LightningModelConfiguration(
             data_dim=self._data_dim,
             latent_dim=self._latent_dim,
             DiffEq_type=self._DiffEq_type,
@@ -195,14 +207,15 @@
             kwargs['PCA'] = self.reducer.PCA
         
         if hasattr(self, "kNN_Graph"):
             kwargs['kNN_Graph'] = self.kNN_Graph
 
         self.DiffEq = self._LitModelConfig(kwargs)
         self._INFO(f"Using the specified parameters, {self.DiffEq} has been called.")
+        self._component_loader = utils.FlexibleComponentLoader(self)
     
     def __config__(self, kwargs):
 
         """
         Run on model.__init__()
 
         Step 0: Parse all kwargs
@@ -221,22 +234,59 @@
         self._configure_logger()
         if kwargs["reduce_dimensions"]:
             self._configure_dimension_reduction()
         if kwargs["build_kNN"]:
             self._configure_kNN_graph()
         self._configure_model(kwargs)
         self._configure_trainer_generator()
+        
+        lightning.seed_everything(self._seed)
+        
+    def to(self, device):
+        self.DiffEq.to(device)
 
     def freeze(self):
         """Freeze lightning model"""
         self.DiffEq.freeze()
+               
+    def load_DiffEq_from_ckpt(self, ckpt_path):
+        
+        self._component_loader.load_DiffEq_state(ckpt_path)
+        self._PARAMS[
+            "diffeq_ckpt_path"
+        ] = self._diffeq_ckpt_path = self._component_loader._diffeq_ckpt_path
+        self.DiffEq._update_lit_diffeq_hparams(self._PARAMS)
+        
+                
+    def load_encoder_from_ckpt(self, ckpt_path):
+        
+        self._component_loader.load_encoder_state(ckpt_path)
+        self._PARAMS[
+            "encoder_ckpt_path"
+        ] = self._encoder_ckpt_path = self._component_loader._encoder_ckpt_path
+        self.DiffEq._update_lit_diffeq_hparams(self._PARAMS)
+        
+        
+    def load_decoder_from_ckpt(self, ckpt_path):
+        
+        self._component_loader.load_decoder_state(ckpt_path)
+        self._PARAMS[
+            "decoder_ckpt_path"
+        ] = self._decoder_ckpt_path = self._component_loader._decoder_ckpt_path
+        self.DiffEq._update_lit_diffeq_hparams(self._PARAMS)
+        
+    def load_VAE_from_ckpt(self, ckpt_path):
+        # TODO: add ability to freeze these once loaded
+        
+        self.load_encoder_from_ckpt(ckpt_path)
+        self.load_decoder_from_ckpt(ckpt_path)
 
     def load(self, ckpt_path, freeze=True):
         self.ckpt_path = ckpt_path
-        self.DiffEq.load_from_checkpoint(ckpt_path)
+        self.DiffEq = self.DiffEq.load_from_checkpoint(ckpt_path)
         if freeze:
             self.DiffEq.freeze()
 
     def _stage_log_path(self, stage):
         log_path = glob.glob(self.DiffEqLogger.versioned_model_outdir + f"/{stage}*")[0]
         self._INFO(f"Access logs at: {log_path}")
         
@@ -261,38 +311,31 @@
     def _configure_pretrain_step(self, epochs, callbacks=[]):
         
         STAGE = "pretrain"
         self._INFO(f"Configuring fit step: {STAGE}")
         
         self.DiffEq._update_lit_diffeq_hparams(self._PARAMS)
 
-#         if not isinstance(epochs, NoneType):
-            
-#             if self._PRETRAIN_CONFIG_COUNT > 0:
-#                 epochs = epochs + self._pretrain_epochs
-            
-#             self._pretrain_epochs = epochs
-#             self._PARAMS["pretrain_epochs"] = epochs
-#             self.DiffEq.hparams['pretrain_epochs'] = epochs
-#             self._INFO(f"Pretrain epochs scheduled: {epochs}")
-
         trainer_kwargs = utils.extract_func_kwargs(
             func=self.TrainerGenerator,
             kwargs=self._PARAMS,
+            ignore = ['version'],
         )
         trainer_kwargs.update(
             utils.extract_func_kwargs(
                 func=lightning.Trainer,
                 kwargs=self._PARAMS,
+                ignore = ['version'],
             )
         )
         trainer_kwargs.update(
             utils.extract_func_kwargs(
                 func=lightning.Trainer,
                 kwargs=locals(),
+                ignore = ['version'],
             )
         )
         trainer_kwargs = self._check_disable_validation(trainer_kwargs)
         
         self.pre_trainer = self.TrainerGenerator(
             max_epochs=self._pretrain_epochs,
             stage=STAGE,
@@ -303,52 +346,48 @@
             **trainer_kwargs
         )
         self._stage_log_path(STAGE)
 
     def pretrain(
         self,
         epochs=None,
-        callbacks = [],
+        pretrain_callbacks = [],
     ):
         """If any of the keyword arguments are passed, they will replace the previously-stated arguments from __init__ and re-configure the DiffEq."""
 
-        self._configure_pretrain_step(epochs, callbacks)
+        self._configure_pretrain_step(epochs, pretrain_callbacks)
         self.pre_trainer.fit(self.DiffEq, self.LitDataModule)
 
     def _configure_train_step(self, epochs, kwargs):
                     
         STAGE = "train"
+        
+        kwargs['callbacks'] = kwargs.pop("train_callbacks")
 
         self._INFO(f"Configuring fit step: {STAGE}")
         
         self.DiffEq._update_lit_diffeq_hparams(self._PARAMS)
 
-#         if not isinstance(epochs, NoneType):
-#             if self._TRAIN_CONFIG_COUNT > 0:
-#                 epochs = epochs + self._train_epochs
-                
-#             self._train_epochs = epochs
-#             self._PARAMS["train_epochs"] = epochs
-#             self.DiffEq.hparams['train_epochs'] = epochs
-#             self._INFO(f"Train epochs scheduled: {epochs}")
-
         trainer_kwargs = utils.extract_func_kwargs(
             func=self.TrainerGenerator,
             kwargs=self._PARAMS,
+            ignore = ['version'],
         )
         trainer_kwargs.update(
             utils.extract_func_kwargs(
                 func=lightning.Trainer,
                 kwargs=self._PARAMS,
+                ignore = ['version'],
             )
         )
         trainer_kwargs.update(
             utils.extract_func_kwargs(
                 func=lightning.Trainer,
                 kwargs=kwargs,
+                ignore = ['version'],
             )
         )
         
         trainer_kwargs = self._check_disable_validation(trainer_kwargs)
         
         self.trainer = self.TrainerGenerator(
             max_epochs=self._train_epochs,
@@ -361,15 +400,15 @@
         )
 
         self._stage_log_path(STAGE)
 
     def train(
         self,
         epochs=500,
-        callbacks=[],
+        train_callbacks=[],
         ckpt_frequency: int = 25,
         save_last_ckpt: bool = True,
         keep_ckpts: int = -1,
         monitor=None,
         accelerator=None,
         log_every_n_steps=1,
         reload_dataloaders_every_n_epochs=1,
@@ -383,15 +422,16 @@
         self.trainer.fit(self.DiffEq, self.LitDataModule)
 
     def fit(
         self,
         train_epochs=200,
         pretrain_epochs=500,
         train_lr = None,
-        callbacks: List = [],
+        pretrain_callbacks: List = [],
+        train_callbacks: List = [],
         ckpt_frequency: int = 25,
         save_last_ckpt: bool = True,
         keep_ckpts: int = -1,
         monitor=None,
         accelerator=None,
         log_every_n_steps=1,
         reload_dataloaders_every_n_epochs=1,
@@ -414,13 +454,16 @@
                 epochs=train_epochs, **utils.extract_func_kwargs(self.train, locals())
             )
             
         # TO-DO: eventually replace how this works...
         self._PRETRAIN_CONFIG_COUNT += 1
         self._TRAIN_CONFIG_COUNT += 1
         
-        
+    @property
+    def tracker(self):
+        return callbacks.ModelTracker(version=self._VERSION)
+
+
     @property
     def loss(self):
-        # scDiffEq_fit_loss_tracking.png
         utils.display_tracked_loss(self.DiffEqLogger)
-        
+
```

### Comparing `scdiffeq-0.0.46rc4/scdiffeq/core/callbacks/__init__.py` & `scdiffeq-0.0.47rc0/scdiffeq/core/callbacks/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -14,9 +14,9 @@
 
 # -- import: -----------------------------------------------------------------------------
 # from ._loss_accounting import LossAccounting
 from ._intermittent_saves import IntermittentSaves
 from ._gradient_potential_callback import GradientPotentialTest
 from ._testing import Testing
 
-from ._visualize_tracked_loss import VisualizeTrackedLoss
+from ._visualize_tracked_loss import ModelTracker, VisualizeTrackedLoss
 from ._visualize_predictions import VisualizePredictions
```

### Comparing `scdiffeq-0.0.46rc4/scdiffeq/core/callbacks/_intermittent_saves.py` & `scdiffeq-0.0.47rc0/scdiffeq/core/callbacks/_intermittent_saves.py`

 * *Files identical despite different names*

### Comparing `scdiffeq-0.0.46rc4/scdiffeq/core/callbacks/_loss_accounting.py` & `scdiffeq-0.0.47rc0/scdiffeq/core/callbacks/_loss_accounting.py`

 * *Files identical despite different names*

### Comparing `scdiffeq-0.0.46rc4/scdiffeq/core/callbacks/_testing.py` & `scdiffeq-0.0.47rc0/scdiffeq/core/callbacks/_testing.py`

 * *Files identical despite different names*

### Comparing `scdiffeq-0.0.46rc4/scdiffeq/core/callbacks/_visualize_predictions.py` & `scdiffeq-0.0.47rc0/scdiffeq/core/callbacks/_visualize_predictions.py`

 * *Files identical despite different names*

### Comparing `scdiffeq-0.0.46rc4/scdiffeq/core/callbacks/_visualize_tracked_loss.py` & `scdiffeq-0.0.47rc0/scdiffeq/core/callbacks/_visualize_tracked_loss.py`

 * *Files 5% similar despite different names*

```diff
@@ -32,26 +32,26 @@
     @property
     def _PATH(self):
         return os.path.join(
             self._working_dir, self._model_name, f"version_{self._version}"
         )
 
     def _HAS_STAGE_LOGS(self, stage_key):
-        return stage_key in [
-            os.path.basename(fpath)
-            for fpath in glob.glob(os.path.join(self._PATH, "*"))
-        ]
+        for fpath in glob.glob(os.path.join(self._PATH, "*/version_*/metrics.csv")):
+            if stage_key in fpath:
+                return True
+            
 
     @property
     def _HAS_PRETRAIN(self):
-        return self._HAS_STAGE_LOGS("pretrain_logs")
+        return self._HAS_STAGE_LOGS("/pretrain_logs")
 
     @property
     def _HAS_TRAIN(self):
-        return self._HAS_STAGE_LOGS("train_logs")
+        return self._HAS_STAGE_LOGS("/train_logs")
 
     @property
     def _PRETRAIN(self):
         if self._HAS_PRETRAIN:
             return utils.PretrainLogs(
                 self._PATH, stage="pretrain", version=self._pretrain_version
             )
@@ -195,15 +195,15 @@
         if self._HAS_TRAIN:
             keys+= self._PLOT_INPUTS["train"].keys()
             
         return keys
 
     @property
     def _NPLOTS(self):
-        nplots = 0
+        nplots = 0        
         if self._HAS_TRAIN:
             nplots += len(self._PLOT_INPUTS["train"].keys())
         if self._HAS_PRETRAIN:
             nplots += len(self._PLOT_INPUTS["pretrain"].keys())
 
         return nplots
 
@@ -243,27 +243,29 @@
             self.axes[en].legend(**self._legend_kwargs)
 
 
 class VisualizeTrackedLoss(lightning.Callback):
     def __init__(
         self,
         version,
+        viz_frequency = 1,
         model_name="scDiffEq_model",
         working_dir=os.getcwd(),
         train_version=0,
         pretrain_version=0,
         fname = "scDiffEq_fit_loss_tracking.png",
         *args,
         **kwargs,
     ):
         self.model_tracker = ModelTracker(
             **utils.extract_func_kwargs(func=ModelTracker, kwargs=locals())
         )
         self._INFO = utils.InfoMessage()
         self.fname = fname
+        self.viz_frequency = viz_frequency
         
     @property
     def save_path(self):
         return os.path.join(self.model_tracker._PATH, self.fname)
         
     def _save_plot(self):
         if not os.path.exists(self.save_path):
@@ -271,10 +273,11 @@
         plt.savefig(self.save_path)
         plt.close()
     
     def on_train_epoch_end(self, trianer, pl_module, *args, **kwargs):
 
         epoch = pl_module.current_epoch
         
-        loss_track_viz = LossTrackingVisualization(self.model_tracker)
-        loss_track_viz.__plot__()
-        self._save_plot()
+        if epoch % self.viz_frequency == 0:
+            loss_track_viz = LossTrackingVisualization(self.model_tracker)
+            loss_track_viz.__plot__()
+            self._save_plot()
```

### Comparing `scdiffeq-0.0.46rc4/scdiffeq/core/configs/_function_credentialling.py` & `scdiffeq-0.0.47rc0/scdiffeq/core/configs/_function_credentialling.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 
-import brownian_diffuser
+# import brownian_diffuser  # deprecated
 import neural_diffeqs
-import torchdiffeq
+# import torchdiffeq # deprecated
 import torchsde
 
 
 class Credentials:
     def __init__(self, func, adjoint=False):
         self.func = func
         self._adjoint = adjoint
@@ -66,8 +66,8 @@
     func_type, mu_is_potential, sigma_is_potential = creds()
     
     return {
         "func_type": func_type,
         "mu_is_potential": mu_is_potential,
         "sigma_is_potential": sigma_is_potential,
         "use_adjoint": adjoint,
-    }
+    }
```

### Comparing `scdiffeq-0.0.46rc4/scdiffeq/core/configs/_lightning_callbacks_configuration.py` & `scdiffeq-0.0.47rc0/scdiffeq/core/configs/_lightning_callbacks_configuration.py`

 * *Files 2% similar despite different names*

```diff
@@ -51,14 +51,15 @@
     @property
     def GradientRetainedCallbacks(self):
         return [callbacks.GradientPotentialTest()] + self.cbs
 
     def __call__(
         self,
         version,
+        viz_frequency = 1,
         model_name="scDiffEq_model",
         working_dir=os.getcwd(),
         train_version=0,
         pretrain_version=0,
         callbacks=[],
         ckpt_frequency=10,
         keep_ckpts=-1,
```

### Comparing `scdiffeq-0.0.46rc4/scdiffeq/core/configs/_lightning_data_configuration.py` & `scdiffeq-0.0.47rc0/scdiffeq/core/configs/_lightning_data_configuration.py`

 * *Files identical despite different names*

### Comparing `scdiffeq-0.0.46rc4/scdiffeq/core/configs/_lightning_model_configuration.py` & `scdiffeq-0.0.47rc0/scdiffeq/core/configs/_lightning_model_configuration.py`

 * *Files identical despite different names*

### Comparing `scdiffeq-0.0.46rc4/scdiffeq/core/configs/_lightning_model_configuration_v2.py` & `scdiffeq-0.0.47rc0/scdiffeq/core/configs/_lightning_model_configuration_v2.py`

 * *Files identical despite different names*

### Comparing `scdiffeq-0.0.46rc4/scdiffeq/core/configs/_lightning_trainer_configuration.py` & `scdiffeq-0.0.47rc0/scdiffeq/core/configs/_lightning_trainer_configuration.py`

 * *Files 3% similar despite different names*

```diff
@@ -38,22 +38,27 @@
     # -- kwargs: ---------------------------------------------------------------
     @property
     def _CSVLogger_kwargs(self):
         return utils.extract_func_kwargs(func=loggers.CSVLogger, kwargs=self._PARAMS, ignore=['version'])
 
     @property
     def _Trainer_kwargs(self):
-        return utils.extract_func_kwargs(func=Trainer, kwargs=self._PARAMS, ignore=["accelerator", "callbacks"])
+        return utils.extract_func_kwargs(
+            func=Trainer,
+            kwargs=self._PARAMS,
+            ignore=["accelerator", "callbacks", 'version'],
+        )
 
     @property
     def Callbacks(self):
         callback_config = LightningCallbacksConfiguration()
         
         return callback_config(
             version = self.version,
+            viz_frequency = self.viz_frequency,
             model_name=self.model_name,
             working_dir=self.working_dir,
             train_version=self.train_version,
             pretrain_version=self.pretrain_version,
             callbacks=self._callbacks,
             ckpt_frequency=self.ckpt_frequency,
             keep_ckpts=self.keep_ckpts,
@@ -123,14 +128,15 @@
     def __call__(
         self,
         lr: float = None,
         model_name="scDiffEq_model",
         working_dir=os.getcwd(),
         train_version=0,
         pretrain_version=0,
+        viz_frequency = 1,
         stage=None,
         max_epochs=500,
         monitor=None,
         accelerator=None,
         devices=None,
         prefix: str = "",
         log_every_n_steps=1,
```

### Comparing `scdiffeq-0.0.46rc4/scdiffeq/core/configs/_time_configuration.py` & `scdiffeq-0.0.47rc0/scdiffeq/core/configs/_time_configuration.py`

 * *Files identical despite different names*

### Comparing `scdiffeq-0.0.46rc4/scdiffeq/core/lightning_models/__init__.py` & `scdiffeq-0.0.47rc0/scdiffeq/core/lightning_models/__init__.py`

 * *Files identical despite different names*

### Comparing `scdiffeq-0.0.46rc4/scdiffeq/core/lightning_models/_lightning_ode.py` & `scdiffeq-0.0.47rc0/scdiffeq/core/lightning_models/_lightning_ode.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,14 +5,16 @@
 
 
 # -- import local dependencies: ------------------------------------------------
 from . import base, mix_ins
 
 
 from typing import Union, List
+from ... import __version__
+
 
 # -- lightning model: ----------------------------------------------------------
 class LightningODE(
     mix_ins.BaseForwardMixIn,
     base.BaseLightningDiffEq,
 ):
     def __init__(
@@ -31,15 +33,15 @@
         # -- general params: ---------------------------------------------------
         train_lr=1e-4,
         train_optimizer=torch.optim.RMSprop,
         train_scheduler=torch.optim.lr_scheduler.StepLR,
         train_step_size=10,
         dt=0.1,
         adjoint=False,
-        
+        version = __version__,
         *args,
         **kwargs,
     ):
         super().__init__()
 
         self.save_hyperparameters()
```

### Comparing `scdiffeq-0.0.46rc4/scdiffeq/core/lightning_models/_lightning_ode_prior_potential.py` & `scdiffeq-0.0.47rc0/scdiffeq/core/lightning_models/_lightning_ode_prior_potential.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,14 +3,16 @@
 import torch
 
 from . import base, mix_ins
 
 from .. import utils
 
 from typing import Union, List
+from ... import __version__
+
 
 class LightningODE_PriorPotential(
     base.BaseLightningDiffEq,
     
 ):
     def __init__(
         self,
@@ -31,14 +33,16 @@
         mu_bias: bool = True,
         mu_output_bias: bool = True,
         mu_n_augment: int = 0,
         sde_type='ito',
         noise_type='general',
         brownian_dim=1,
         
+        version = __version__,
+        
         *args,
         **kwargs,
     ):
         super().__init__()
 
         self.save_hyperparameters()        
         self.func = LatentPotentialODE(
```

### Comparing `scdiffeq-0.0.46rc4/scdiffeq/core/lightning_models/_lightning_ode_vae.py` & `scdiffeq-0.0.47rc0/scdiffeq/core/lightning_models/_lightning_ode_vae.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,14 +7,17 @@
 
 # -- import local dependencies: ------------------------------------------------
 from . import mix_ins
 from . import base
 
 
 from typing import Union, List
+from ... import __version__
+
+
 
 # -- lightning model: ----------------------------------------------------------
 class LightningODE_VAE(
     mix_ins.VAEMixIn,
     mix_ins.PreTrainMixIn,
     base.BaseLightningDiffEq,
 ):
@@ -55,15 +58,15 @@
         # -- decoder parameters: -----------------------------------------------
         decoder_n_hidden: int = 4,
         decoder_power: float = 2,
         decoder_activation: Union[str, List[str]] = 'LeakyReLU',
         decoder_dropout: Union[float, List[float]] = 0.2,
         decoder_bias: bool = True,
         decoder_output_bias: bool = True,
-        
+        version = __version__,
         *args,
         **kwargs,
     ):
         super().__init__()
 
         self.save_hyperparameters()
```

### Comparing `scdiffeq-0.0.46rc4/scdiffeq/core/lightning_models/_lightning_ode_vae_fixed_potential.py` & `scdiffeq-0.0.47rc0/scdiffeq/core/lightning_models/_lightning_ode_vae_fixed_potential.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,14 +4,16 @@
 
 from neural_diffeqs import PotentialODE
 import torch_nets
 import torch
 
 
 from typing import Union, List
+from ... import __version__
+
 
 class LightningODE_VAE_FixedPotential(
     mix_ins.BaseForwardMixIn,
     base.BaseLightningDiffEq,
     mix_ins.PreTrainMixIn,
     mix_ins.PotentialMixIn,
 ):
@@ -32,14 +34,15 @@
         train_optimizer=torch.optim.RMSprop,
         pretrain_scheduler=None,
         train_scheduler=torch.optim.lr_scheduler.StepLR,
         pretrain_step_size=None,
         train_step_size=10,
         dt=0.1,
         adjoint=False,
+        version = __version__,
         *args,
         **kwargs,
     ):
         super().__init__()
 
         self.save_hyperparameters()
```

### Comparing `scdiffeq-0.0.46rc4/scdiffeq/core/lightning_models/_lightning_ode_vae_prior_potential.py` & `scdiffeq-0.0.47rc0/scdiffeq/core/lightning_models/_lightning_ode_vae_prior_potential.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,14 +7,16 @@
 
 # -- import local dependencies: ------------------------------------------------
 from . import mix_ins
 from . import base
 
 
 from typing import Union, List
+from ... import __version__
+
 
 # -- lightning model: ----------------------------------------------------------
 class LightningODE_VAE_PriorPotential(
     mix_ins.DriftPriorMixIn,
     mix_ins.PotentialMixIn,
     mix_ins.VAEMixIn,
     mix_ins.PreTrainMixIn,
@@ -48,14 +50,16 @@
         decoder_n_hidden: int = 4,
         decoder_power: float = 2,
         decoder_activation: Union[str, List[str]] = 'LeakyReLU',
         decoder_dropout: Union[float, List[float]] = 0.2,
         decoder_bias: bool = True,
         decoder_output_bias: bool = True,
         
+        version = __version__,
+        
         *args,
         **kwargs,
     ):
         super().__init__()
 
         self.save_hyperparameters()
```

### Comparing `scdiffeq-0.0.46rc4/scdiffeq/core/lightning_models/_lightning_sde.py` & `scdiffeq-0.0.47rc0/scdiffeq/core/lightning_models/_lightning_sde.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 
 
 # -- import local dependencies: ------------------------------------------------
 from . import base, mix_ins
 
 
 from typing import Union, List
+from ... import __version__
 
 
 # -- lightning model: ----------------------------------------------------------
 class LightningSDE(
     mix_ins.BaseForwardMixIn,
     base.BaseLightningDiffEq,
 ):
@@ -38,14 +39,15 @@
         coef_diffusion: float = 1.0,
         train_lr=1e-4,
         train_optimizer=torch.optim.RMSprop,
         train_scheduler=torch.optim.lr_scheduler.StepLR,
         train_step_size=10,
         dt=0.1,
         adjoint=False,
+        version = __version__,
         *args,
         **kwargs,
     ):
         super().__init__()
 
         self.save_hyperparameters()
```

### Comparing `scdiffeq-0.0.46rc4/scdiffeq/core/lightning_models/_lightning_sde_fate_bias_aware.py` & `scdiffeq-0.0.47rc0/scdiffeq/core/lightning_models/_lightning_sde_fate_bias_aware.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 
 # -- import local dependencies: ------------------------------------------------
 from . import base, mix_ins
 # from scdiffeq.core.lightning_models import base, mix_ins
 
 
 from typing import Union, List
+from ... import __version__
 
 # -- lightning model: ----------------------------------------------------------
 class LightningSDE_FateBiasAware(
     mix_ins.FateBiasMixIn,
     mix_ins.BaseForwardMixIn,
     base.BaseLightningDiffEq,
 ):
@@ -43,14 +44,17 @@
         train_step_size=10,
         dt=0.1,
         adjoint=False,
         t0_idx = None,
         kNN_Graph=None,
         fate_bias_csv_path=None,
         fate_bias_multiplier = 1,
+        
+        version = __version__,
+        
         *args,
         **kwargs,
     ):
         super().__init__()
 
         self.save_hyperparameters(ignore=['kNN_Graph'])
```

### Comparing `scdiffeq-0.0.46rc4/scdiffeq/core/lightning_models/_lightning_sde_fixed_potential.py` & `scdiffeq-0.0.47rc0/scdiffeq/core/lightning_models/_lightning_sde_fixed_potential.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,14 +2,16 @@
 from neural_diffeqs import PotentialSDE
 import torch
 
 
 from . import base, mix_ins
 from typing import Union, List
 
+from ... import __version__
+
 
 # -- lightning model: -----------------------------------
 class LightningSDE_FixedPotential(
     mix_ins.PotentialMixIn,
     mix_ins.BaseForwardMixIn,
     base.BaseLightningDiffEq,
 ):
@@ -36,14 +38,17 @@
         
         train_lr=1e-4,
         train_optimizer=torch.optim.RMSprop,
         train_scheduler=torch.optim.lr_scheduler.StepLR,
         train_step_size=10,
         dt=0.1,
         adjoint=False,
+        
+        version = __version__,
+        
         *args,
         **kwargs,
     ):
         super().__init__()
 
         self.save_hyperparameters()
```

### Comparing `scdiffeq-0.0.46rc4/scdiffeq/core/lightning_models/_lightning_sde_prior_potential.py` & `scdiffeq-0.0.47rc0/scdiffeq/core/lightning_models/_lightning_sde_prior_potential.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,17 +4,20 @@
 
 from . import base, mix_ins
 
 from .. import utils
 
 from typing import Union, List
 
+from ... import __version__
+
 class LightningSDE_PriorPotential(
-    base.BaseLightningDiffEq,
     mix_ins.PotentialMixIn,
+    mix_ins.DriftPriorMixIn,
+    base.BaseLightningDiffEq,
 ):
     def __init__(
         self,
         latent_dim,
         train_lr=1e-4,
         train_optimizer=torch.optim.RMSprop,
         train_scheduler=torch.optim.lr_scheduler.StepLR,
@@ -35,46 +38,47 @@
         sigma_n_augment: int = 0,
         sde_type='ito',
         noise_type='general',
         brownian_dim=1,
         coef_drift: float = 1.0,
         coef_diffusion: float = 1.0,
         coef_prior_drift: float = 1.0,
+        version = __version__,
         *args,
         **kwargs,
     ):
         super().__init__()
 
         self.save_hyperparameters()
         
         # -- torch modules: ----------------------------------------------------
         self._configure_torch_modules(func=LatentPotentialSDE, kwargs=locals())
         self._configure_optimizers_schedulers()
 
-    def forward(self, X0, t, **kwargs):
-        """Forward step: (0) integrate in latent space"""
-        Z_hat, KL_div = self.integrate(
-            Z0=X0, t=t, dt=self.hparams["dt"], logqp=True, **kwargs
-        )
-        return Z_hat, KL_div
+#     def forward(self, X0, t, **kwargs):
+#         """Forward step: (0) integrate in latent space"""
+#         Z_hat, KL_div = self.integrate(
+#             Z0=X0, t=t, dt=self.hparams["dt"], logqp=True, **kwargs
+#         )
+#         return Z_hat, KL_div
 
-    def log_computed_loss(self, sinkhorn_loss, t, kl_div_loss, stage):
+#     def log_computed_loss(self, sinkhorn_loss, t, kl_div_loss, stage):
         
-        sinkhorn_loss = self.log_sinkhorn_divergence(sinkhorn_loss).sum()
-        self.log(f"kl_div_{stage}", kl_div_loss.sum())
+#         sinkhorn_loss = self.log_sinkhorn_divergence(sinkhorn_loss).sum()
+#         self.log(f"kl_div_{stage}", kl_div_loss.sum())
 
-        return sinkhorn_loss + kl_div_loss.sum()
+#         return sinkhorn_loss + kl_div_loss.sum()
 
-    def step(self, batch, batch_idx, stage=None):
+#     def step(self, batch, batch_idx, stage=None):
 
-        batch = self.process_batch(batch, batch_idx)
-        X_hat, kl_div_loss = self.forward(batch.X0, batch.t)
-        sinkhorn_loss = self.compute_sinkhorn_divergence(
-            batch.X, X_hat, batch.W, batch.W_hat
-        )
-        return self.log_computed_loss(
-            sinkhorn_loss, t=batch.t, kl_div_loss=kl_div_loss, stage=stage
-        )
+#         batch = self.process_batch(batch, batch_idx)
+#         X_hat, kl_div_loss = self.forward(batch.X0, batch.t)
+#         sinkhorn_loss = self.compute_sinkhorn_divergence(
+#             batch.X, X_hat, batch.W, batch.W_hat
+#         )
+#         return self.log_computed_loss(
+#             sinkhorn_loss, t=batch.t, kl_div_loss=kl_div_loss, stage=stage
+#         )
 
         
     def __repr__(self):
         return "LightningSDE-PriorPotential"
```

### Comparing `scdiffeq-0.0.46rc4/scdiffeq/core/lightning_models/_lightning_sde_vae.py` & `scdiffeq-0.0.47rc0/scdiffeq/core/lightning_models/_lightning_sde_vae.py`

 * *Files 9% similar despite different names*

```diff
@@ -6,18 +6,21 @@
 
 
 # -- import local dependencies: ------------------------------------------------
 from . import mix_ins, base
 
 from typing import Union, List
 
+from ... import __version__
+
 # -- lightning model: ----------------------------------------------------------
 class LightningSDE_VAE(
     mix_ins.VAEMixIn, 
     mix_ins.PreTrainMixIn,
+    mix_ins.BaseForwardMixIn,
     base.BaseLightningDiffEq,
 ):
     def __init__(
         self,
         data_dim,
         latent_dim,
         train_lr=1e-5,
@@ -63,14 +66,16 @@
         decoder_n_hidden: int = 4,
         decoder_power: float = 2,
         decoder_activation: Union[str, List[str]] = 'LeakyReLU',
         decoder_dropout: Union[float, List[float]] = 0.2,
         decoder_bias: bool = True,
         decoder_output_bias: bool = True,
         
+        version = __version__,
+        
         *args,
         **kwargs,
     ):
         super().__init__()
 
         self.save_hyperparameters()
```

### Comparing `scdiffeq-0.0.46rc4/scdiffeq/core/lightning_models/_lightning_sde_vae_fate_bias_aware.py` & `scdiffeq-0.0.47rc0/scdiffeq/core/lightning_models/_lightning_sde_vae_fate_bias_aware.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,14 +6,17 @@
 
 # -- import local dependencies: ------------------------------------------------
 from . import base, mix_ins
 
 
 from typing import Union, List
 
+from ... import __version__
+
+
 # -- lightning model: ----------------------------------------------------------
 class LightningSDE_VAE_FateBiasAware(
     mix_ins.VAEMixIn,
     mix_ins.FateBiasVAEMixIn,
     mix_ins.PotentialMixIn,
     mix_ins.PreTrainMixIn,
     base.BaseLightningDiffEq,
@@ -73,14 +76,16 @@
         t0_idx = None,
         kNN_Graph=None,
         fate_bias_csv_path=None,
         fate_bias_multiplier = 1,
         
         PCA = None,
         
+        version = __version__,
+        
         *args,
         **kwargs,
     ):
         super().__init__()
 
         self.save_hyperparameters(ignore=['kNN_Graph'])
```

### Comparing `scdiffeq-0.0.46rc4/scdiffeq/core/lightning_models/_lightning_sde_vae_fixed_potential.py` & `scdiffeq-0.0.47rc0/scdiffeq/core/lightning_models/_lightning_sde_vae_fixed_potential.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,14 +4,16 @@
 
 from neural_diffeqs import PotentialSDE
 import torch_nets
 import torch
 
 from typing import Union, List
 
+from ... import __version__
+
 class LightningSDE_VAE_FixedPotential(
     mix_ins.PreTrainMixIn,
     mix_ins.PotentialMixIn,
     mix_ins.VAEMixIn,
     base.BaseLightningDiffEq,
 ):
     def __init__(
@@ -61,14 +63,16 @@
         decoder_activation: Union[str, List[str]] = 'LeakyReLU',
         decoder_dropout: Union[float, List[float]] = 0.2,
         decoder_bias: bool = True,
         decoder_output_bias: bool = True,
         
         dt=0.1,
         adjoint=False,
+        version = __version__,
+        
         *args,
         **kwargs,
     ):
         super().__init__()
 
         self.save_hyperparameters()
```

### Comparing `scdiffeq-0.0.46rc4/scdiffeq/core/lightning_models/_lightning_sde_vae_prior_potential.py` & `scdiffeq-0.0.47rc0/scdiffeq/core/lightning_models/_lightning_sde_vae_prior_potential.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 
 # -- import local dependencies: ------------------------------------------------
 from . import mix_ins
 from . import base
 from .. import utils
 
 from typing import Union, List
+from ... import __version__
 
 
 # -- lightning model: ----------------------------------------------------------
 class LightningSDE_VAE_PriorPotential(
     mix_ins.DriftPriorVAEMixIn,
     mix_ins.PotentialMixIn,
     mix_ins.VAEMixIn,
@@ -70,14 +71,16 @@
         decoder_n_hidden: int = 4,
         decoder_power: float = 2,
         decoder_activation: Union[str, List[str]] = 'LeakyReLU',
         decoder_dropout: Union[float, List[float]] = 0.2,
         decoder_bias: bool = True,
         decoder_output_bias: bool = True,
         
+        version = __version__,
+        
         *args,
         **kwargs,
     ):
         super().__init__()
         
         self.save_hyperparameters()
```

### Comparing `scdiffeq-0.0.46rc4/scdiffeq/core/lightning_models/_lightning_sde_vae_prior_potential_fate_bias_aware.py` & `scdiffeq-0.0.47rc0/scdiffeq/core/lightning_models/_lightning_sde_vae_prior_potential_fate_bias_aware.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,14 +6,16 @@
 
 
 # -- import local dependencies: ------------------------------------------------
 from . import mix_ins
 from . import base
 from .. import utils
 
+from ... import __version__
+
 from typing import Union, List
 
 
 # -- lightning model: ----------------------------------------------------------
 class LightningSDE_VAE_PriorPotential_FateBiasAware(
     mix_ins.FateBiasVAEMixIn,
     mix_ins.DriftPriorVAEMixIn,
@@ -73,14 +75,16 @@
         decoder_activation: Union[str, List[str]] = 'LeakyReLU',
         decoder_dropout: Union[float, List[float]] = 0.2,
         decoder_bias: bool = True,
         decoder_output_bias: bool = True,
         
         PCA = None,
         
+        version = __version__,
+        
         *args,
         **kwargs,
     ):
         super().__init__()
         
         self.save_hyperparameters()
```

### Comparing `scdiffeq-0.0.46rc4/scdiffeq/core/lightning_models/base/_base_lightning_diffeq.py` & `scdiffeq-0.0.47rc0/scdiffeq/core/lightning_models/base/_base_lightning_diffeq.py`

 * *Files 19% similar despite different names*

```diff
@@ -27,73 +27,85 @@
             if key in model_params.keys():
                 if val != model_params[key]:
                     self.hparams.update({key: model_params[key]})
         
     # -- setup: ----------------------------------------------------------------
     def _configure_optimizers_schedulers(self):
         """Assumes no pre-train - i.e., a single optimizer, scheduler"""
+        
         optimizer = self.hparams['train_optimizer']
         scheduler = self.hparams['train_scheduler']
 
         self._optimizers = [optimizer(self.parameters(), lr=self.hparams['train_lr'])]
         self._schedulers = [
             scheduler(
                 optimizer=self._optimizers[0],
                 step_size=self.hparams['train_step_size']),
         ]
 
     def _configure_torch_modules(self, func, kwargs):
         
         kwargs['state_size'] = self.hparams['latent_dim']
-        self.func = func(**utils.function_kwargs(func, kwargs))
+        self.DiffEq = func(**utils.function_kwargs(func, kwargs))
         
     @property
     def PRETRAIN(self):
         return False
     
     # -- integrator stuff: -----------------------------------------------------
     @property
     def _INTEGRATOR(self):
         if self.hparams["adjoint"]:
             return torchsde.sdeint_adjoint
         return torchsde.sdeint
 
     def integrate(self, Z0, t, dt, logqp, **kwargs):
         return self._INTEGRATOR(
-            sde=self.func,
+            sde=self.DiffEq,
             y0=Z0,
             ts=t,
             dt=dt,
             logqp=logqp,
             **kwargs,
         )
 
     # -- sinkhorn stuff: -------------------------------------------------------
     def compute_sinkhorn_divergence(self, X, X_hat, W, W_hat):
         return self.sinkhorn_divergence(
             W.contiguous(), X.contiguous(), W_hat.contiguous(), X_hat.contiguous()
-        )
+        ).requires_grad_()
 
     def log_sinkhorn_divergence(self, sinkhorn_loss, t, stage):
         for i in range(len(t)):
             _t = round(t[i].item(), 3)
             msg = f"sinkhorn_{_t}_{stage}"
             val = sinkhorn_loss[i]
             self.log(msg, val)
 
         return sinkhorn_loss.sum()
+    
+    def log_lr(self):
+                
+        if not isinstance(self.optimizers(), list):
+            lr = self.optimizers().optimizer.state_dict()["param_groups"][0]["lr"]
+            self.log("opt_param_group_lr", lr)
+        else:
+            for i, opt in enumerate(self.optimizers()):
+                for j, pg in enumerate(opt.optimizer.state_dict()["param_groups"]):
+                    self.log(f"opt_{i}_param_group_{j}_lr", pg["lr"])
 
     # -- custom steps: -------------------------------------------------------------
     @abstractmethod
     def forward(self, Z0, t, **kwargs):
         """most likely over-written in another class"""
         ...
 
     @abstractmethod
     def step(self, batch, batch_idx, stage=None):
+        print("WARNING: The base (empty) step is being called from `_base_lightning_diffeq.py`")
         ...
 
     # -- LightningModule methods: ----------------------------------------------
     def training_step(self, batch, batch_idx, *args, **kwargs):
         return self.step(batch, batch_idx, stage="training")
 
     def validation_step(self, batch, batch_idx=None, *args, **kwargs):
```

### Comparing `scdiffeq-0.0.46rc4/scdiffeq/core/lightning_models/base/_batch_processor.py` & `scdiffeq-0.0.47rc0/scdiffeq/core/lightning_models/base/_batch_processor.py`

 * *Files identical despite different names*

### Comparing `scdiffeq-0.0.46rc4/scdiffeq/core/lightning_models/base/_sinkhorn_divergence.py` & `scdiffeq-0.0.47rc0/scdiffeq/core/lightning_models/base/_sinkhorn_divergence.py`

 * *Files identical despite different names*

### Comparing `scdiffeq-0.0.46rc4/scdiffeq/core/lightning_models/mix_ins/__init__.py` & `scdiffeq-0.0.47rc0/scdiffeq/core/lightning_models/mix_ins/__init__.py`

 * *Files identical despite different names*

### Comparing `scdiffeq-0.0.46rc4/scdiffeq/core/lightning_models/mix_ins/_base_forward_mix_in.py` & `scdiffeq-0.0.47rc0/scdiffeq/core/lightning_models/mix_ins/_base_forward_mix_in.py`

 * *Files 17% similar despite different names*

```diff
@@ -11,8 +11,9 @@
     def step(self, batch, batch_idx, stage=None):
 
         batch = self.process_batch(batch, batch_idx)
         X_hat = self.forward(batch.X0, batch.t)
         sinkhorn_loss = self.compute_sinkhorn_divergence(
             batch.X, X_hat, batch.W, batch.W_hat
         )
+        self.log_lr()
         return self.log_sinkhorn_divergence(sinkhorn_loss, t=batch.t, stage=stage)
```

### Comparing `scdiffeq-0.0.46rc4/scdiffeq/core/lightning_models/mix_ins/_drift_prior_mix_in.py` & `scdiffeq-0.0.47rc0/scdiffeq/core/lightning_models/mix_ins/_drift_prior_mix_in.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 
 class DriftPriorMixIn(object):
     logqp = True
     def __init__(self, *args, **kwargs):
         super().__init__()
 
-    def forward(self, X0, t, logqp=False, **kwargs):
+    def forward(self, Z0, t, **kwargs):
         """Forward step: (0) integrate in latent space"""
         
         return self.integrate(
-            Z0=self.Encoder(X0),
+            Z0=Z0,
             t=t,
             dt=self.hparams["dt"],
-            logqp=logqp,
+            logqp=self.logqp,
             **kwargs,
         )
             
     def log_computed_loss(self, sinkhorn_loss, t, kl_div_loss, stage):
         
         sinkhorn_loss = self.log_sinkhorn_divergence(
             sinkhorn_loss=sinkhorn_loss,
```

### Comparing `scdiffeq-0.0.46rc4/scdiffeq/core/lightning_models/mix_ins/_fate_bias_drift_prior_mix_in.py` & `scdiffeq-0.0.47rc0/scdiffeq/core/lightning_models/mix_ins/_fate_bias_drift_prior_mix_in.py`

 * *Files identical despite different names*

### Comparing `scdiffeq-0.0.46rc4/scdiffeq/core/lightning_models/mix_ins/_fate_bias_drift_prior_vae_mix_in.py` & `scdiffeq-0.0.47rc0/scdiffeq/core/lightning_models/mix_ins/_fate_bias_drift_prior_vae_mix_in.py`

 * *Files identical despite different names*

### Comparing `scdiffeq-0.0.46rc4/scdiffeq/core/lightning_models/mix_ins/_fate_bias_mix_in.py` & `scdiffeq-0.0.47rc0/scdiffeq/core/lightning_models/mix_ins/_fate_bias_mix_in.py`

 * *Files identical despite different names*

### Comparing `scdiffeq-0.0.46rc4/scdiffeq/core/lightning_models/mix_ins/_fate_bias_vae_mix_in.py` & `scdiffeq-0.0.47rc0/scdiffeq/core/lightning_models/mix_ins/_fate_bias_vae_mix_in.py`

 * *Files identical despite different names*

### Comparing `scdiffeq-0.0.46rc4/scdiffeq/core/lightning_models/mix_ins/_pre_train_mix_in.py` & `scdiffeq-0.0.47rc0/scdiffeq/core/lightning_models/mix_ins/_pre_train_mix_in.py`

 * *Files identical despite different names*

### Comparing `scdiffeq-0.0.46rc4/scdiffeq/core/lightning_models/mix_ins/_sde_mix_in.py` & `scdiffeq-0.0.47rc0/scdiffeq/core/lightning_models/mix_ins/_sde_mix_in.py`

 * *Files identical despite different names*

### Comparing `scdiffeq-0.0.46rc4/scdiffeq/core/utils/__init__.py` & `scdiffeq-0.0.47rc0/scdiffeq/core/utils/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -37,8 +37,9 @@
 
 from ._logs import Logs, PretrainLogs, TrainLogs
 
 from ._filter_df import filter_df
 
 from ._display_tracked_loss import display_tracked_loss
 
-from ._knn_graph_query import kNNGraphQuery
+from ._knn_graph_query import kNNGraphQuery
+from ._flexible_component_loader import FlexibleComponentLoader
```

### Comparing `scdiffeq-0.0.46rc4/scdiffeq/core/utils/_abc_parse.py` & `scdiffeq-0.0.47rc0/scdiffeq/core/utils/_abc_parse.py`

 * *Files identical despite different names*

### Comparing `scdiffeq-0.0.46rc4/scdiffeq/core/utils/_anndata_inspector.py` & `scdiffeq-0.0.47rc0/scdiffeq/core/utils/_anndata_inspector.py`

 * *Files identical despite different names*

### Comparing `scdiffeq-0.0.46rc4/scdiffeq/core/utils/_autoparse_base_class.py` & `scdiffeq-0.0.47rc0/scdiffeq/core/utils/_autoparse_base_class.py`

 * *Files identical despite different names*

### Comparing `scdiffeq-0.0.46rc4/scdiffeq/core/utils/_default_neural_sde.py` & `scdiffeq-0.0.47rc0/scdiffeq/core/utils/_default_neural_sde.py`

 * *Files identical despite different names*

### Comparing `scdiffeq-0.0.46rc4/scdiffeq/core/utils/_fast_graph.py` & `scdiffeq-0.0.47rc0/scdiffeq/core/utils/_fast_graph.py`

 * *Files identical despite different names*

### Comparing `scdiffeq-0.0.46rc4/scdiffeq/core/utils/_filter_df.py` & `scdiffeq-0.0.47rc0/scdiffeq/core/utils/_filter_df.py`

 * *Files identical despite different names*

### Comparing `scdiffeq-0.0.46rc4/scdiffeq/core/utils/_function_fetch.py` & `scdiffeq-0.0.47rc0/scdiffeq/core/utils/_function_fetch.py`

 * *Files identical despite different names*

### Comparing `scdiffeq-0.0.46rc4/scdiffeq/core/utils/_function_kwargs.py` & `scdiffeq-0.0.47rc0/scdiffeq/core/utils/_function_kwargs.py`

 * *Files identical despite different names*

### Comparing `scdiffeq-0.0.46rc4/scdiffeq/core/utils/_knn_graph_query.py` & `scdiffeq-0.0.47rc0/scdiffeq/core/utils/_knn_graph_query.py`

 * *Files identical despite different names*

### Comparing `scdiffeq-0.0.46rc4/scdiffeq/core/utils/_logging_learnable_hparams.py` & `scdiffeq-0.0.47rc0/scdiffeq/core/utils/_logging_learnable_hparams.py`

 * *Files identical despite different names*

### Comparing `scdiffeq-0.0.46rc4/scdiffeq/core/utils/_logs.py` & `scdiffeq-0.0.47rc0/scdiffeq/core/utils/_logs.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,39 +4,48 @@
 
 from .. import utils
 
 
 # -- Base Class: ------
 class Logs(utils.ABCParse):
     def __init__(self, path, stage, version=0):
-        super().__init__()
         self.__parse__(locals(), public=[None])
-        
+
     @property
-    def _BACKUP_BASE_PATH(self):
-        return os.path.join(
-            self._path, f"{self._stage}_logs", f"version_{int(self._version - 1)}"
-        )
+    def _AVAILABLE_VERSIONS(self):
+        versions = glob.glob(f"{self._path}/{self._stage}*/version_*")
+        n_versions = len(versions)
+        return [int(os.path.basename(v).split("_")[-1]) for v in versions]
+
+    @property
+    def _VERSION(self):
+        """Sometimes the passed version isn't found..."""
+        if self._version in self._AVAILABLE_VERSIONS:
+            return self._version
+        elif len(self._AVAILABLE_VERSIONS) > 0:
+            return max(self._AVAILABLE_VERSIONS)
+        else:
+            return "VERSION NOT FOUND"
 
     @property
     def _BASE_PATH(self):
         return os.path.join(
-            self._path, f"{self._stage}_logs", f"version_{self._version}"
+            self._path, f"{self._stage}_logs", f"version_{self._VERSION}"
         )
 
     @property
     def _METRICS_PATH(self):
         _metrics_path = os.path.join(self._BASE_PATH, "metrics.csv")
-        if not os.path.exists(_metrics_path):
-            try:
-                _metrics_path = os.path.join(self._BACKUP_BASE_PATH, "metrics.csv")
-            except:
-                print(f"Cannot find: {_metrics_path}")
-        
-        return _metrics_path
+        if os.path.exists(_metrics_path):
+            return _metrics_path
+#         else:
+#             _metrics_path = os.path.join(self._BACKUP_BASE_PATH, "metrics.csv")
+#             if os.path.exists(_metrics_path):
+#                 return _metrics_path
+#             raise FileNotFoundError(_metrics_path)
 
     @property
     def _HPARAMS_PATH(self):
         return os.path.join(self._BASE_PATH, "hparams.yaml")
 
     @property
     def _CKPTS_PATH(self):
```

### Comparing `scdiffeq-0.0.46rc4/scdiffeq/core/utils/_scdiffeq_logger.py` & `scdiffeq-0.0.47rc0/scdiffeq/core/utils/_scdiffeq_logger.py`

 * *Files identical despite different names*

### Comparing `scdiffeq-0.0.46rc4/scdiffeq/io/__init__.py` & `scdiffeq-0.0.47rc0/scdiffeq/io/__init__.py`

 * *Files identical despite different names*

### Comparing `scdiffeq-0.0.46rc4/scdiffeq/io/_pickle_io.py` & `scdiffeq-0.0.47rc0/scdiffeq/io/_pickle_io.py`

 * *Files identical despite different names*

### Comparing `scdiffeq-0.0.46rc4/scdiffeq/io/_read_h5ad.py` & `scdiffeq-0.0.47rc0/scdiffeq/io/_read_h5ad.py`

 * *Files identical despite different names*

### Comparing `scdiffeq-0.0.46rc4/scdiffeq/tools/__init__.py` & `scdiffeq-0.0.47rc0/scdiffeq/tools/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -19,8 +19,18 @@
 from ._reconstruct_function import reconstruct_function
 from ._versions import Versions, configure_version
 from ._func_from_version import func_from_version
 from ._umap import UMAP
 from ._fetch import fetch
 from ._drift_diffusion_state_characterization import drift, diffusion
 
-from ._dimension_reduction import DimensionReduction
+from ._dimension_reduction import DimensionReduction
+
+
+# -----------
+from ._data_format import DataFormat
+from ._x_use import X_use, fetch_formatted_data
+from ._knn import kNN
+
+from ._negative_cross_entropy import NegativeCrossEntropy
+
+from ._sum_norm_df import sum_norm_df
```

### Comparing `scdiffeq-0.0.46rc4/scdiffeq/tools/_annotate_cells.py` & `scdiffeq-0.0.47rc0/scdiffeq/tools/_annotate_cells.py`

 * *Files identical despite different names*

### Comparing `scdiffeq-0.0.46rc4/scdiffeq/tools/_dimension_reduction.py` & `scdiffeq-0.0.47rc0/scdiffeq/tools/_dimension_reduction.py`

 * *Files identical despite different names*

### Comparing `scdiffeq-0.0.46rc4/scdiffeq/tools/_drift_diffusion_state_characterization.py` & `scdiffeq-0.0.47rc0/scdiffeq/tools/_drift_diffusion_state_characterization.py`

 * *Files identical despite different names*

### Comparing `scdiffeq-0.0.46rc4/scdiffeq/tools/_func_from_version.py` & `scdiffeq-0.0.47rc0/scdiffeq/tools/_func_from_version.py`

 * *Files identical despite different names*

### Comparing `scdiffeq-0.0.46rc4/scdiffeq/tools/_hyperparams.py` & `scdiffeq-0.0.47rc0/scdiffeq/tools/_hyperparams.py`

 * *Files identical despite different names*

### Comparing `scdiffeq-0.0.46rc4/scdiffeq/tools/_reconstruct_function.py` & `scdiffeq-0.0.47rc0/scdiffeq/tools/_reconstruct_function.py`

 * *Files identical despite different names*

### Comparing `scdiffeq-0.0.46rc4/scdiffeq/tools/_time_free_sampling.py` & `scdiffeq-0.0.47rc0/scdiffeq/tools/_time_free_sampling.py`

 * *Files identical despite different names*

### Comparing `scdiffeq-0.0.46rc4/scdiffeq/tools/_umap.py` & `scdiffeq-0.0.47rc0/scdiffeq/tools/_umap.py`

 * *Files identical despite different names*

### Comparing `scdiffeq-0.0.46rc4/scdiffeq/tools/_versions.py` & `scdiffeq-0.0.47rc0/scdiffeq/tools/_versions.py`

 * *Files identical despite different names*

### Comparing `scdiffeq-0.0.46rc4/scdiffeq.egg-info/PKG-INFO` & `scdiffeq-0.0.47rc0/scdiffeq.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scdiffeq
-Version: 0.0.46rc4
+Version: 0.0.47rc0
 Summary: scDiffEq: modelling single-cell dynamics using neural differential equations.
 Home-page: https://github.com/mvinyard/sc-neural-diffeqs
 Author: Michael E. Vinyard - Harvard University - Massachussetts General Hospital - Broad Institute of MIT and Harvard
 Author-email: mvinyard@broadinstitute.org
 License: MIT
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Programming Language :: Python :: 3.9
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: scdiffeq Version: 0.0.46rc4 Summary: scDiffEq:
+Metadata-Version: 2.1 Name: scdiffeq Version: 0.0.47rc0 Summary: scDiffEq:
 modelling single-cell dynamics using neural differential equations. Home-page:
 https://github.com/mvinyard/sc-neural-diffeqs Author: Michael E. Vinyard -
 Harvard University - Massachussetts General Hospital - Broad Institute of MIT
 and Harvard Author-email: mvinyard@broadinstitute.org License: MIT Classifier:
 Development Status :: 2 - Pre-Alpha Classifier: Programming Language :: Python
 :: 3.9 Classifier: Intended Audience :: Science/Research Classifier: Topic ::
 Scientific/Engineering :: Bio-Informatics Requires-Python: >3.9.0 Description-
```

### Comparing `scdiffeq-0.0.46rc4/scdiffeq.egg-info/SOURCES.txt` & `scdiffeq-0.0.47rc0/scdiffeq.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -60,14 +60,15 @@
 scdiffeq/core/utils/_anndata_inspector.py
 scdiffeq/core/utils/_autoparse_base_class.py
 scdiffeq/core/utils/_default_neural_sde.py
 scdiffeq/core/utils/_display_tracked_loss.py
 scdiffeq/core/utils/_fast_graph.py
 scdiffeq/core/utils/_fetch_format.py
 scdiffeq/core/utils/_filter_df.py
+scdiffeq/core/utils/_flexible_component_loader.py
 scdiffeq/core/utils/_function_fetch.py
 scdiffeq/core/utils/_function_kwargs.py
 scdiffeq/core/utils/_idx_to_int_str.py
 scdiffeq/core/utils/_info_message.py
 scdiffeq/core/utils/_knn_graph_query.py
 scdiffeq/core/utils/_logging_learnable_hparams.py
 scdiffeq/core/utils/_logs.py
@@ -77,16 +78,21 @@
 scdiffeq/core/utils/_sum_normalize.py
 scdiffeq/io/__init__.py
 scdiffeq/io/_pickle_io.py
 scdiffeq/io/_read_h5ad.py
 scdiffeq/plotting/__init__.py
 scdiffeq/tools/__init__.py
 scdiffeq/tools/_annotate_cells.py
+scdiffeq/tools/_data_format.py
 scdiffeq/tools/_dimension_reduction.py
 scdiffeq/tools/_drift_diffusion_state_characterization.py
 scdiffeq/tools/_fetch.py
 scdiffeq/tools/_func_from_version.py
 scdiffeq/tools/_hyperparams.py
+scdiffeq/tools/_knn.py
+scdiffeq/tools/_negative_cross_entropy.py
 scdiffeq/tools/_reconstruct_function.py
+scdiffeq/tools/_sum_norm_df.py
 scdiffeq/tools/_time_free_sampling.py
 scdiffeq/tools/_umap.py
-scdiffeq/tools/_versions.py
+scdiffeq/tools/_versions.py
+scdiffeq/tools/_x_use.py
```

### Comparing `scdiffeq-0.0.46rc4/setup.py` & `scdiffeq-0.0.47rc0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 import re
 import os
 import sys
 
 setuptools.setup(
     name="scdiffeq",
-    version="0.0.46rc4",
+    version="0.0.47rc0",
     python_requires=">3.9.0",
     author="Michael E. Vinyard - Harvard University - Massachussetts General Hospital - Broad Institute of MIT and Harvard",
     author_email="mvinyard@broadinstitute.org",
     url="https://github.com/mvinyard/sc-neural-diffeqs",
     long_description=open("README.md", encoding="utf-8").read(),
     long_description_content_type="text/markdown",
     description="scDiffEq: modelling single-cell dynamics using neural differential equations.",
```

