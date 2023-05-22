# Comparing `tmp/scdiffeq-0.0.47rc0.tar.gz` & `tmp/scdiffeq-0.0.47rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scdiffeq-0.0.47rc0.tar", last modified: Mon May 22 14:23:11 2023, max compression
+gzip compressed data, was "scdiffeq-0.0.47rc1.tar", last modified: Mon May 22 14:44:18 2023, max compression
```

## Comparing `scdiffeq-0.0.47rc0.tar` & `scdiffeq-0.0.47rc1.tar`

### file list

```diff
@@ -1,113 +1,112 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 14:23:11.498330 scdiffeq-0.0.47rc0/
--rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-05-22 14:23:00.000000 scdiffeq-0.0.47rc0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2299 2023-05-22 14:23:11.498330 scdiffeq-0.0.47rc0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1627 2023-05-22 14:23:00.000000 scdiffeq-0.0.47rc0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 14:23:11.490330 scdiffeq-0.0.47rc0/scdiffeq/
--rw-r--r--   0 runner    (1001) docker     (123)      682 2023-05-22 14:23:00.000000 scdiffeq-0.0.47rc0/scdiffeq/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 14:23:11.490330 scdiffeq-0.0.47rc0/scdiffeq/core/
--rw-r--r--   0 runner    (1001) docker     (123)      584 2023-05-22 14:23:00.000000 scdiffeq-0.0.47rc0/scdiffeq/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15908 2023-05-22 14:23:00.000000 scdiffeq-0.0.47rc0/scdiffeq/core/_scdiffeq.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 14:23:11.490330 scdiffeq-0.0.47rc0/scdiffeq/core/callbacks/
--rw-r--r--   0 runner    (1001) docker     (123)      725 2023-05-22 14:23:00.000000 scdiffeq-0.0.47rc0/scdiffeq/core/callbacks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      271 2023-05-22 14:23:00.000000 scdiffeq-0.0.47rc0/scdiffeq/core/callbacks/_gradient_potential_callback.py
--rw-r--r--   0 runner    (1001) docker     (123)      834 2023-05-22 14:23:00.000000 scdiffeq-0.0.47rc0/scdiffeq/core/callbacks/_intermittent_saves.py
--rw-r--r--   0 runner    (1001) docker     (123)     4853 2023-05-22 14:23:00.000000 scdiffeq-0.0.47rc0/scdiffeq/core/callbacks/_loss_accounting.py
--rw-r--r--   0 runner    (1001) docker     (123)      806 2023-05-22 14:23:00.000000 scdiffeq-0.0.47rc0/scdiffeq/core/callbacks/_testing.py
--rw-r--r--   0 runner    (1001) docker     (123)     5319 2023-05-22 14:23:00.000000 scdiffeq-0.0.47rc0/scdiffeq/core/callbacks/_visualize_predictions.py
--rw-r--r--   0 runner    (1001) docker     (123)     8233 2023-05-22 14:23:00.000000 scdiffeq-0.0.47rc0/scdiffeq/core/callbacks/_visualize_tracked_loss.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 14:23:11.490330 scdiffeq-0.0.47rc0/scdiffeq/core/configs/
--rw-r--r--   0 runner    (1001) docker     (123)      488 2023-05-22 14:23:00.000000 scdiffeq-0.0.47rc0/scdiffeq/core/configs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2210 2023-05-22 14:23:00.000000 scdiffeq-0.0.47rc0/scdiffeq/core/configs/_function_credentialling.py
--rw-r--r--   0 runner    (1001) docker     (123)     2210 2023-05-22 14:23:00.000000 scdiffeq-0.0.47rc0/scdiffeq/core/configs/_lightning_callbacks_configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)     2073 2023-05-22 14:23:00.000000 scdiffeq-0.0.47rc0/scdiffeq/core/configs/_lightning_data_configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)     5708 2023-05-22 14:23:00.000000 scdiffeq-0.0.47rc0/scdiffeq/core/configs/_lightning_model_configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)     2140 2023-05-22 14:23:00.000000 scdiffeq-0.0.47rc0/scdiffeq/core/configs/_lightning_model_configuration_v2.py
--rw-r--r--   0 runner    (1001) docker     (123)     6834 2023-05-22 14:23:00.000000 scdiffeq-0.0.47rc0/scdiffeq/core/configs/_lightning_trainer_configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)    10716 2023-05-22 14:23:00.000000 scdiffeq-0.0.47rc0/scdiffeq/core/configs/_time_configuration.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 14:23:11.494330 scdiffeq-0.0.47rc0/scdiffeq/core/lightning_models/
--rw-r--r--   0 runner    (1001) docker     (123)     1229 2023-05-22 14:23:00.000000 scdiffeq-0.0.47rc0/scdiffeq/core/lightning_models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1605 2023-05-22 14:23:00.000000 scdiffeq-0.0.47rc0/scdiffeq/core/lightning_models/_lightning_ode.py
--rw-r--r--   0 runner    (1001) docker     (123)     1694 2023-05-22 14:23:00.000000 scdiffeq-0.0.47rc0/scdiffeq/core/lightning_models/_lightning_ode_fixed_potential.py
--rw-r--r--   0 runner    (1001) docker     (123)     2420 2023-05-22 14:23:00.000000 scdiffeq-0.0.47rc0/scdiffeq/core/lightning_models/_lightning_ode_prior_potential.py
--rw-r--r--   0 runner    (1001) docker     (123)     2508 2023-05-22 14:23:00.000000 scdiffeq-0.0.47rc0/scdiffeq/core/lightning_models/_lightning_ode_vae.py
--rw-r--r--   0 runner    (1001) docker     (123)     2337 2023-05-22 14:23:00.000000 scdiffeq-0.0.47rc0/scdiffeq/core/lightning_models/_lightning_ode_vae_fixed_potential.py
--rw-r--r--   0 runner    (1001) docker     (123)     3121 2023-05-22 14:23:00.000000 scdiffeq-0.0.47rc0/scdiffeq/core/lightning_models/_lightning_ode_vae_prior_potential.py
--rw-r--r--   0 runner    (1001) docker     (123)     1827 2023-05-22 14:23:00.000000 scdiffeq-0.0.47rc0/scdiffeq/core/lightning_models/_lightning_sde.py
--rw-r--r--   0 runner    (1001) docker     (123)     2330 2023-05-22 14:23:00.000000 scdiffeq-0.0.47rc0/scdiffeq/core/lightning_models/_lightning_sde_fate_bias_aware.py
--rw-r--r--   0 runner    (1001) docker     (123)     1732 2023-05-22 14:23:00.000000 scdiffeq-0.0.47rc0/scdiffeq/core/lightning_models/_lightning_sde_fixed_potential.py
--rw-r--r--   0 runner    (1001) docker     (123)     2677 2023-05-22 14:23:00.000000 scdiffeq-0.0.47rc0/scdiffeq/core/lightning_models/_lightning_sde_prior_potential.py
--rw-r--r--   0 runner    (1001) docker     (123)     2936 2023-05-22 14:23:00.000000 scdiffeq-0.0.47rc0/scdiffeq/core/lightning_models/_lightning_sde_vae.py
--rw-r--r--   0 runner    (1001) docker     (123)     3468 2023-05-22 14:23:00.000000 scdiffeq-0.0.47rc0/scdiffeq/core/lightning_models/_lightning_sde_vae_fate_bias_aware.py
--rw-r--r--   0 runner    (1001) docker     (123)     3113 2023-05-22 14:23:00.000000 scdiffeq-0.0.47rc0/scdiffeq/core/lightning_models/_lightning_sde_vae_fixed_potential.py
--rw-r--r--   0 runner    (1001) docker     (123)     2977 2023-05-22 14:23:00.000000 scdiffeq-0.0.47rc0/scdiffeq/core/lightning_models/_lightning_sde_vae_prior_potential.py
--rw-r--r--   0 runner    (1001) docker     (123)     3295 2023-05-22 14:23:00.000000 scdiffeq-0.0.47rc0/scdiffeq/core/lightning_models/_lightning_sde_vae_prior_potential_fate_bias_aware.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 14:23:11.494330 scdiffeq-0.0.47rc0/scdiffeq/core/lightning_models/base/
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-05-22 14:23:00.000000 scdiffeq-0.0.47rc0/scdiffeq/core/lightning_models/base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4385 2023-05-22 14:23:00.000000 scdiffeq-0.0.47rc0/scdiffeq/core/lightning_models/base/_base_lightning_diffeq.py
--rw-r--r--   0 runner    (1001) docker     (123)     2458 2023-05-22 14:23:00.000000 scdiffeq-0.0.47rc0/scdiffeq/core/lightning_models/base/_batch_processor.py
--rw-r--r--   0 runner    (1001) docker     (123)      752 2023-05-22 14:23:00.000000 scdiffeq-0.0.47rc0/scdiffeq/core/lightning_models/base/_sinkhorn_divergence.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 14:23:11.494330 scdiffeq-0.0.47rc0/scdiffeq/core/lightning_models/mix_ins/
--rw-r--r--   0 runner    (1001) docker     (123)      612 2023-05-22 14:23:00.000000 scdiffeq-0.0.47rc0/scdiffeq/core/lightning_models/mix_ins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      647 2023-05-22 14:23:00.000000 scdiffeq-0.0.47rc0/scdiffeq/core/lightning_models/mix_ins/_base_forward_mix_in.py
--rw-r--r--   0 runner    (1001) docker     (123)     2535 2023-05-22 14:23:00.000000 scdiffeq-0.0.47rc0/scdiffeq/core/lightning_models/mix_ins/_drift_prior_mix_in.py
--rw-r--r--   0 runner    (1001) docker     (123)     2583 2023-05-22 14:23:00.000000 scdiffeq-0.0.47rc0/scdiffeq/core/lightning_models/mix_ins/_fate_bias_drift_prior_mix_in.py
--rw-r--r--   0 runner    (1001) docker     (123)     2805 2023-05-22 14:23:00.000000 scdiffeq-0.0.47rc0/scdiffeq/core/lightning_models/mix_ins/_fate_bias_drift_prior_vae_mix_in.py
--rw-r--r--   0 runner    (1001) docker     (123)     2691 2023-05-22 14:23:00.000000 scdiffeq-0.0.47rc0/scdiffeq/core/lightning_models/mix_ins/_fate_bias_mix_in.py
--rw-r--r--   0 runner    (1001) docker     (123)     2822 2023-05-22 14:23:00.000000 scdiffeq-0.0.47rc0/scdiffeq/core/lightning_models/mix_ins/_fate_bias_vae_mix_in.py
--rw-r--r--   0 runner    (1001) docker     (123)      318 2023-05-22 14:23:00.000000 scdiffeq-0.0.47rc0/scdiffeq/core/lightning_models/mix_ins/_potential_mix_in.py
--rw-r--r--   0 runner    (1001) docker     (123)      941 2023-05-22 14:23:00.000000 scdiffeq-0.0.47rc0/scdiffeq/core/lightning_models/mix_ins/_pre_train_mix_in.py
--rw-r--r--   0 runner    (1001) docker     (123)     2264 2023-05-22 14:23:00.000000 scdiffeq-0.0.47rc0/scdiffeq/core/lightning_models/mix_ins/_sde_mix_in.py
--rw-r--r--   0 runner    (1001) docker     (123)     4898 2023-05-22 14:23:00.000000 scdiffeq-0.0.47rc0/scdiffeq/core/lightning_models/mix_ins/_vae_mix_in.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 14:23:11.498330 scdiffeq-0.0.47rc0/scdiffeq/core/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     1366 2023-05-22 14:23:00.000000 scdiffeq-0.0.47rc0/scdiffeq/core/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2018 2023-05-22 14:23:00.000000 scdiffeq-0.0.47rc0/scdiffeq/core/utils/_abc_parse.py
--rw-r--r--   0 runner    (1001) docker     (123)      931 2023-05-22 14:23:00.000000 scdiffeq-0.0.47rc0/scdiffeq/core/utils/_anndata_inspector.py
--rw-r--r--   0 runner    (1001) docker     (123)     2802 2023-05-22 14:23:00.000000 scdiffeq-0.0.47rc0/scdiffeq/core/utils/_autoparse_base_class.py
--rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-05-22 14:23:00.000000 scdiffeq-0.0.47rc0/scdiffeq/core/utils/_default_neural_sde.py
--rw-r--r--   0 runner    (1001) docker     (123)      307 2023-05-22 14:23:00.000000 scdiffeq-0.0.47rc0/scdiffeq/core/utils/_display_tracked_loss.py
--rw-r--r--   0 runner    (1001) docker     (123)     2011 2023-05-22 14:23:00.000000 scdiffeq-0.0.47rc0/scdiffeq/core/utils/_fast_graph.py
--rw-r--r--   0 runner    (1001) docker     (123)      333 2023-05-22 14:23:00.000000 scdiffeq-0.0.47rc0/scdiffeq/core/utils/_fetch_format.py
--rw-r--r--   0 runner    (1001) docker     (123)     2381 2023-05-22 14:23:00.000000 scdiffeq-0.0.47rc0/scdiffeq/core/utils/_filter_df.py
--rw-r--r--   0 runner    (1001) docker     (123)     2738 2023-05-22 14:23:00.000000 scdiffeq-0.0.47rc0/scdiffeq/core/utils/_flexible_component_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)     1652 2023-05-22 14:23:00.000000 scdiffeq-0.0.47rc0/scdiffeq/core/utils/_function_fetch.py
--rw-r--r--   0 runner    (1001) docker     (123)     3402 2023-05-22 14:23:00.000000 scdiffeq-0.0.47rc0/scdiffeq/core/utils/_function_kwargs.py
--rw-r--r--   0 runner    (1001) docker     (123)      231 2023-05-22 14:23:00.000000 scdiffeq-0.0.47rc0/scdiffeq/core/utils/_idx_to_int_str.py
--rw-r--r--   0 runner    (1001) docker     (123)      341 2023-05-22 14:23:00.000000 scdiffeq-0.0.47rc0/scdiffeq/core/utils/_info_message.py
--rw-r--r--   0 runner    (1001) docker     (123)     2147 2023-05-22 14:23:00.000000 scdiffeq-0.0.47rc0/scdiffeq/core/utils/_knn_graph_query.py
--rw-r--r--   0 runner    (1001) docker     (123)      892 2023-05-22 14:23:00.000000 scdiffeq-0.0.47rc0/scdiffeq/core/utils/_logging_learnable_hparams.py
--rw-r--r--   0 runner    (1001) docker     (123)     6934 2023-05-22 14:23:00.000000 scdiffeq-0.0.47rc0/scdiffeq/core/utils/_logs.py
--rw-r--r--   0 runner    (1001) docker     (123)      395 2023-05-22 14:23:00.000000 scdiffeq-0.0.47rc0/scdiffeq/core/utils/_normalize_time_to_range.py
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-05-22 14:23:00.000000 scdiffeq-0.0.47rc0/scdiffeq/core/utils/_not_none_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     2339 2023-05-22 14:23:00.000000 scdiffeq-0.0.47rc0/scdiffeq/core/utils/_scdiffeq_logger.py
--rw-r--r--   0 runner    (1001) docker     (123)      346 2023-05-22 14:23:00.000000 scdiffeq-0.0.47rc0/scdiffeq/core/utils/_sum_normalize.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 14:23:11.498330 scdiffeq-0.0.47rc0/scdiffeq/io/
--rw-r--r--   0 runner    (1001) docker     (123)      541 2023-05-22 14:23:00.000000 scdiffeq-0.0.47rc0/scdiffeq/io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      744 2023-05-22 14:23:00.000000 scdiffeq-0.0.47rc0/scdiffeq/io/_pickle_io.py
--rw-r--r--   0 runner    (1001) docker     (123)     1258 2023-05-22 14:23:00.000000 scdiffeq-0.0.47rc0/scdiffeq/io/_read_h5ad.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 14:23:11.498330 scdiffeq-0.0.47rc0/scdiffeq/plotting/
--rw-r--r--   0 runner    (1001) docker     (123)      462 2023-05-22 14:23:00.000000 scdiffeq-0.0.47rc0/scdiffeq/plotting/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 14:23:11.498330 scdiffeq-0.0.47rc0/scdiffeq/tools/
--rw-r--r--   0 runner    (1001) docker     (123)     1145 2023-05-22 14:23:00.000000 scdiffeq-0.0.47rc0/scdiffeq/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1482 2023-05-22 14:23:00.000000 scdiffeq-0.0.47rc0/scdiffeq/tools/_annotate_cells.py
--rw-r--r--   0 runner    (1001) docker     (123)     1446 2023-05-22 14:23:00.000000 scdiffeq-0.0.47rc0/scdiffeq/tools/_data_format.py
--rw-r--r--   0 runner    (1001) docker     (123)     4607 2023-05-22 14:23:00.000000 scdiffeq-0.0.47rc0/scdiffeq/tools/_dimension_reduction.py
--rw-r--r--   0 runner    (1001) docker     (123)     1546 2023-05-22 14:23:00.000000 scdiffeq-0.0.47rc0/scdiffeq/tools/_drift_diffusion_state_characterization.py
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-05-22 14:23:00.000000 scdiffeq-0.0.47rc0/scdiffeq/tools/_fetch.py
--rw-r--r--   0 runner    (1001) docker     (123)     1292 2023-05-22 14:23:00.000000 scdiffeq-0.0.47rc0/scdiffeq/tools/_func_from_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     1019 2023-05-22 14:23:00.000000 scdiffeq-0.0.47rc0/scdiffeq/tools/_hyperparams.py
--rw-r--r--   0 runner    (1001) docker     (123)     3210 2023-05-22 14:23:00.000000 scdiffeq-0.0.47rc0/scdiffeq/tools/_knn.py
--rw-r--r--   0 runner    (1001) docker     (123)      866 2023-05-22 14:23:00.000000 scdiffeq-0.0.47rc0/scdiffeq/tools/_negative_cross_entropy.py
--rw-r--r--   0 runner    (1001) docker     (123)     5462 2023-05-22 14:23:00.000000 scdiffeq-0.0.47rc0/scdiffeq/tools/_reconstruct_function.py
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-05-22 14:23:00.000000 scdiffeq-0.0.47rc0/scdiffeq/tools/_sum_norm_df.py
--rw-r--r--   0 runner    (1001) docker     (123)     1470 2023-05-22 14:23:00.000000 scdiffeq-0.0.47rc0/scdiffeq/tools/_time_free_sampling.py
--rw-r--r--   0 runner    (1001) docker     (123)      853 2023-05-22 14:23:00.000000 scdiffeq-0.0.47rc0/scdiffeq/tools/_umap.py
--rw-r--r--   0 runner    (1001) docker     (123)     1242 2023-05-22 14:23:00.000000 scdiffeq-0.0.47rc0/scdiffeq/tools/_versions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3561 2023-05-22 14:23:00.000000 scdiffeq-0.0.47rc0/scdiffeq/tools/_x_use.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 14:23:11.490330 scdiffeq-0.0.47rc0/scdiffeq.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2299 2023-05-22 14:23:11.000000 scdiffeq-0.0.47rc0/scdiffeq.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4374 2023-05-22 14:23:11.000000 scdiffeq-0.0.47rc0/scdiffeq.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 14:23:11.000000 scdiffeq-0.0.47rc0/scdiffeq.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      306 2023-05-22 14:23:11.000000 scdiffeq-0.0.47rc0/scdiffeq.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-22 14:23:11.000000 scdiffeq-0.0.47rc0/scdiffeq.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-22 14:23:11.498330 scdiffeq-0.0.47rc0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1404 2023-05-22 14:23:00.000000 scdiffeq-0.0.47rc0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 14:44:18.613166 scdiffeq-0.0.47rc1/
+-rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-05-22 14:44:07.000000 scdiffeq-0.0.47rc1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2299 2023-05-22 14:44:18.613166 scdiffeq-0.0.47rc1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1627 2023-05-22 14:44:07.000000 scdiffeq-0.0.47rc1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 14:44:18.593166 scdiffeq-0.0.47rc1/scdiffeq/
+-rw-r--r--   0 runner    (1001) docker     (123)      571 2023-05-22 14:44:07.000000 scdiffeq-0.0.47rc1/scdiffeq/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 14:44:18.597166 scdiffeq-0.0.47rc1/scdiffeq/core/
+-rw-r--r--   0 runner    (1001) docker     (123)      584 2023-05-22 14:44:07.000000 scdiffeq-0.0.47rc1/scdiffeq/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15908 2023-05-22 14:44:07.000000 scdiffeq-0.0.47rc1/scdiffeq/core/_scdiffeq.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 14:44:18.597166 scdiffeq-0.0.47rc1/scdiffeq/core/callbacks/
+-rw-r--r--   0 runner    (1001) docker     (123)      725 2023-05-22 14:44:07.000000 scdiffeq-0.0.47rc1/scdiffeq/core/callbacks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      271 2023-05-22 14:44:07.000000 scdiffeq-0.0.47rc1/scdiffeq/core/callbacks/_gradient_potential_callback.py
+-rw-r--r--   0 runner    (1001) docker     (123)      834 2023-05-22 14:44:07.000000 scdiffeq-0.0.47rc1/scdiffeq/core/callbacks/_intermittent_saves.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4853 2023-05-22 14:44:07.000000 scdiffeq-0.0.47rc1/scdiffeq/core/callbacks/_loss_accounting.py
+-rw-r--r--   0 runner    (1001) docker     (123)      806 2023-05-22 14:44:07.000000 scdiffeq-0.0.47rc1/scdiffeq/core/callbacks/_testing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5319 2023-05-22 14:44:07.000000 scdiffeq-0.0.47rc1/scdiffeq/core/callbacks/_visualize_predictions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8233 2023-05-22 14:44:07.000000 scdiffeq-0.0.47rc1/scdiffeq/core/callbacks/_visualize_tracked_loss.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 14:44:18.601166 scdiffeq-0.0.47rc1/scdiffeq/core/configs/
+-rw-r--r--   0 runner    (1001) docker     (123)      413 2023-05-22 14:44:07.000000 scdiffeq-0.0.47rc1/scdiffeq/core/configs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2135 2023-05-22 14:44:07.000000 scdiffeq-0.0.47rc1/scdiffeq/core/configs/_function_credentialling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2210 2023-05-22 14:44:07.000000 scdiffeq-0.0.47rc1/scdiffeq/core/configs/_lightning_callbacks_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2073 2023-05-22 14:44:07.000000 scdiffeq-0.0.47rc1/scdiffeq/core/configs/_lightning_data_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2140 2023-05-22 14:44:07.000000 scdiffeq-0.0.47rc1/scdiffeq/core/configs/_lightning_model_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6662 2023-05-22 14:44:07.000000 scdiffeq-0.0.47rc1/scdiffeq/core/configs/_lightning_trainer_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10716 2023-05-22 14:44:07.000000 scdiffeq-0.0.47rc1/scdiffeq/core/configs/_time_configuration.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 14:44:18.605166 scdiffeq-0.0.47rc1/scdiffeq/core/lightning_models/
+-rw-r--r--   0 runner    (1001) docker     (123)     1229 2023-05-22 14:44:07.000000 scdiffeq-0.0.47rc1/scdiffeq/core/lightning_models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1605 2023-05-22 14:44:07.000000 scdiffeq-0.0.47rc1/scdiffeq/core/lightning_models/_lightning_ode.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1694 2023-05-22 14:44:07.000000 scdiffeq-0.0.47rc1/scdiffeq/core/lightning_models/_lightning_ode_fixed_potential.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2420 2023-05-22 14:44:07.000000 scdiffeq-0.0.47rc1/scdiffeq/core/lightning_models/_lightning_ode_prior_potential.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2508 2023-05-22 14:44:07.000000 scdiffeq-0.0.47rc1/scdiffeq/core/lightning_models/_lightning_ode_vae.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2337 2023-05-22 14:44:07.000000 scdiffeq-0.0.47rc1/scdiffeq/core/lightning_models/_lightning_ode_vae_fixed_potential.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3121 2023-05-22 14:44:07.000000 scdiffeq-0.0.47rc1/scdiffeq/core/lightning_models/_lightning_ode_vae_prior_potential.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1827 2023-05-22 14:44:07.000000 scdiffeq-0.0.47rc1/scdiffeq/core/lightning_models/_lightning_sde.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2330 2023-05-22 14:44:07.000000 scdiffeq-0.0.47rc1/scdiffeq/core/lightning_models/_lightning_sde_fate_bias_aware.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1732 2023-05-22 14:44:07.000000 scdiffeq-0.0.47rc1/scdiffeq/core/lightning_models/_lightning_sde_fixed_potential.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2677 2023-05-22 14:44:07.000000 scdiffeq-0.0.47rc1/scdiffeq/core/lightning_models/_lightning_sde_prior_potential.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2936 2023-05-22 14:44:07.000000 scdiffeq-0.0.47rc1/scdiffeq/core/lightning_models/_lightning_sde_vae.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3468 2023-05-22 14:44:07.000000 scdiffeq-0.0.47rc1/scdiffeq/core/lightning_models/_lightning_sde_vae_fate_bias_aware.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3113 2023-05-22 14:44:07.000000 scdiffeq-0.0.47rc1/scdiffeq/core/lightning_models/_lightning_sde_vae_fixed_potential.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2977 2023-05-22 14:44:07.000000 scdiffeq-0.0.47rc1/scdiffeq/core/lightning_models/_lightning_sde_vae_prior_potential.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3295 2023-05-22 14:44:07.000000 scdiffeq-0.0.47rc1/scdiffeq/core/lightning_models/_lightning_sde_vae_prior_potential_fate_bias_aware.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 14:44:18.605166 scdiffeq-0.0.47rc1/scdiffeq/core/lightning_models/base/
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-05-22 14:44:07.000000 scdiffeq-0.0.47rc1/scdiffeq/core/lightning_models/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4385 2023-05-22 14:44:07.000000 scdiffeq-0.0.47rc1/scdiffeq/core/lightning_models/base/_base_lightning_diffeq.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2458 2023-05-22 14:44:07.000000 scdiffeq-0.0.47rc1/scdiffeq/core/lightning_models/base/_batch_processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      752 2023-05-22 14:44:07.000000 scdiffeq-0.0.47rc1/scdiffeq/core/lightning_models/base/_sinkhorn_divergence.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 14:44:18.609166 scdiffeq-0.0.47rc1/scdiffeq/core/lightning_models/mix_ins/
+-rw-r--r--   0 runner    (1001) docker     (123)      612 2023-05-22 14:44:07.000000 scdiffeq-0.0.47rc1/scdiffeq/core/lightning_models/mix_ins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      647 2023-05-22 14:44:07.000000 scdiffeq-0.0.47rc1/scdiffeq/core/lightning_models/mix_ins/_base_forward_mix_in.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2535 2023-05-22 14:44:07.000000 scdiffeq-0.0.47rc1/scdiffeq/core/lightning_models/mix_ins/_drift_prior_mix_in.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2583 2023-05-22 14:44:07.000000 scdiffeq-0.0.47rc1/scdiffeq/core/lightning_models/mix_ins/_fate_bias_drift_prior_mix_in.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2805 2023-05-22 14:44:07.000000 scdiffeq-0.0.47rc1/scdiffeq/core/lightning_models/mix_ins/_fate_bias_drift_prior_vae_mix_in.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2691 2023-05-22 14:44:07.000000 scdiffeq-0.0.47rc1/scdiffeq/core/lightning_models/mix_ins/_fate_bias_mix_in.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2822 2023-05-22 14:44:07.000000 scdiffeq-0.0.47rc1/scdiffeq/core/lightning_models/mix_ins/_fate_bias_vae_mix_in.py
+-rw-r--r--   0 runner    (1001) docker     (123)      318 2023-05-22 14:44:07.000000 scdiffeq-0.0.47rc1/scdiffeq/core/lightning_models/mix_ins/_potential_mix_in.py
+-rw-r--r--   0 runner    (1001) docker     (123)      941 2023-05-22 14:44:07.000000 scdiffeq-0.0.47rc1/scdiffeq/core/lightning_models/mix_ins/_pre_train_mix_in.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2264 2023-05-22 14:44:07.000000 scdiffeq-0.0.47rc1/scdiffeq/core/lightning_models/mix_ins/_sde_mix_in.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4898 2023-05-22 14:44:07.000000 scdiffeq-0.0.47rc1/scdiffeq/core/lightning_models/mix_ins/_vae_mix_in.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 14:44:18.609166 scdiffeq-0.0.47rc1/scdiffeq/core/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     1366 2023-05-22 14:44:07.000000 scdiffeq-0.0.47rc1/scdiffeq/core/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2018 2023-05-22 14:44:07.000000 scdiffeq-0.0.47rc1/scdiffeq/core/utils/_abc_parse.py
+-rw-r--r--   0 runner    (1001) docker     (123)      931 2023-05-22 14:44:07.000000 scdiffeq-0.0.47rc1/scdiffeq/core/utils/_anndata_inspector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2802 2023-05-22 14:44:07.000000 scdiffeq-0.0.47rc1/scdiffeq/core/utils/_autoparse_base_class.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-05-22 14:44:07.000000 scdiffeq-0.0.47rc1/scdiffeq/core/utils/_default_neural_sde.py
+-rw-r--r--   0 runner    (1001) docker     (123)      307 2023-05-22 14:44:07.000000 scdiffeq-0.0.47rc1/scdiffeq/core/utils/_display_tracked_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2011 2023-05-22 14:44:07.000000 scdiffeq-0.0.47rc1/scdiffeq/core/utils/_fast_graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)      333 2023-05-22 14:44:07.000000 scdiffeq-0.0.47rc1/scdiffeq/core/utils/_fetch_format.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2381 2023-05-22 14:44:07.000000 scdiffeq-0.0.47rc1/scdiffeq/core/utils/_filter_df.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2738 2023-05-22 14:44:07.000000 scdiffeq-0.0.47rc1/scdiffeq/core/utils/_flexible_component_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1652 2023-05-22 14:44:07.000000 scdiffeq-0.0.47rc1/scdiffeq/core/utils/_function_fetch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3402 2023-05-22 14:44:07.000000 scdiffeq-0.0.47rc1/scdiffeq/core/utils/_function_kwargs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      231 2023-05-22 14:44:07.000000 scdiffeq-0.0.47rc1/scdiffeq/core/utils/_idx_to_int_str.py
+-rw-r--r--   0 runner    (1001) docker     (123)      341 2023-05-22 14:44:07.000000 scdiffeq-0.0.47rc1/scdiffeq/core/utils/_info_message.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2147 2023-05-22 14:44:07.000000 scdiffeq-0.0.47rc1/scdiffeq/core/utils/_knn_graph_query.py
+-rw-r--r--   0 runner    (1001) docker     (123)      892 2023-05-22 14:44:07.000000 scdiffeq-0.0.47rc1/scdiffeq/core/utils/_logging_learnable_hparams.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6934 2023-05-22 14:44:07.000000 scdiffeq-0.0.47rc1/scdiffeq/core/utils/_logs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      395 2023-05-22 14:44:07.000000 scdiffeq-0.0.47rc1/scdiffeq/core/utils/_normalize_time_to_range.py
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-05-22 14:44:07.000000 scdiffeq-0.0.47rc1/scdiffeq/core/utils/_not_none_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2339 2023-05-22 14:44:07.000000 scdiffeq-0.0.47rc1/scdiffeq/core/utils/_scdiffeq_logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)      346 2023-05-22 14:44:07.000000 scdiffeq-0.0.47rc1/scdiffeq/core/utils/_sum_normalize.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 14:44:18.609166 scdiffeq-0.0.47rc1/scdiffeq/io/
+-rw-r--r--   0 runner    (1001) docker     (123)      541 2023-05-22 14:44:07.000000 scdiffeq-0.0.47rc1/scdiffeq/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      744 2023-05-22 14:44:07.000000 scdiffeq-0.0.47rc1/scdiffeq/io/_pickle_io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1258 2023-05-22 14:44:07.000000 scdiffeq-0.0.47rc1/scdiffeq/io/_read_h5ad.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 14:44:18.609166 scdiffeq-0.0.47rc1/scdiffeq/plotting/
+-rw-r--r--   0 runner    (1001) docker     (123)      462 2023-05-22 14:44:07.000000 scdiffeq-0.0.47rc1/scdiffeq/plotting/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 14:44:18.613166 scdiffeq-0.0.47rc1/scdiffeq/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)     1145 2023-05-22 14:44:07.000000 scdiffeq-0.0.47rc1/scdiffeq/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1482 2023-05-22 14:44:07.000000 scdiffeq-0.0.47rc1/scdiffeq/tools/_annotate_cells.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1446 2023-05-22 14:44:07.000000 scdiffeq-0.0.47rc1/scdiffeq/tools/_data_format.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4607 2023-05-22 14:44:07.000000 scdiffeq-0.0.47rc1/scdiffeq/tools/_dimension_reduction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1546 2023-05-22 14:44:07.000000 scdiffeq-0.0.47rc1/scdiffeq/tools/_drift_diffusion_state_characterization.py
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-05-22 14:44:07.000000 scdiffeq-0.0.47rc1/scdiffeq/tools/_fetch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1292 2023-05-22 14:44:07.000000 scdiffeq-0.0.47rc1/scdiffeq/tools/_func_from_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1019 2023-05-22 14:44:07.000000 scdiffeq-0.0.47rc1/scdiffeq/tools/_hyperparams.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3210 2023-05-22 14:44:07.000000 scdiffeq-0.0.47rc1/scdiffeq/tools/_knn.py
+-rw-r--r--   0 runner    (1001) docker     (123)      866 2023-05-22 14:44:07.000000 scdiffeq-0.0.47rc1/scdiffeq/tools/_negative_cross_entropy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5462 2023-05-22 14:44:07.000000 scdiffeq-0.0.47rc1/scdiffeq/tools/_reconstruct_function.py
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-05-22 14:44:07.000000 scdiffeq-0.0.47rc1/scdiffeq/tools/_sum_norm_df.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1470 2023-05-22 14:44:07.000000 scdiffeq-0.0.47rc1/scdiffeq/tools/_time_free_sampling.py
+-rw-r--r--   0 runner    (1001) docker     (123)      853 2023-05-22 14:44:07.000000 scdiffeq-0.0.47rc1/scdiffeq/tools/_umap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1242 2023-05-22 14:44:07.000000 scdiffeq-0.0.47rc1/scdiffeq/tools/_versions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3561 2023-05-22 14:44:07.000000 scdiffeq-0.0.47rc1/scdiffeq/tools/_x_use.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 14:44:18.593166 scdiffeq-0.0.47rc1/scdiffeq.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2299 2023-05-22 14:44:18.000000 scdiffeq-0.0.47rc1/scdiffeq.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4315 2023-05-22 14:44:18.000000 scdiffeq-0.0.47rc1/scdiffeq.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 14:44:18.000000 scdiffeq-0.0.47rc1/scdiffeq.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      331 2023-05-22 14:44:18.000000 scdiffeq-0.0.47rc1/scdiffeq.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-22 14:44:18.000000 scdiffeq-0.0.47rc1/scdiffeq.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-22 14:44:18.613166 scdiffeq-0.0.47rc1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1440 2023-05-22 14:44:07.000000 scdiffeq-0.0.47rc1/setup.py
```

### Comparing `scdiffeq-0.0.47rc0/LICENSE` & `scdiffeq-0.0.47rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `scdiffeq-0.0.47rc0/PKG-INFO` & `scdiffeq-0.0.47rc1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scdiffeq
-Version: 0.0.47rc0
+Version: 0.0.47rc1
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
-Metadata-Version: 2.1 Name: scdiffeq Version: 0.0.47rc0 Summary: scDiffEq:
+Metadata-Version: 2.1 Name: scdiffeq Version: 0.0.47rc1 Summary: scDiffEq:
 modelling single-cell dynamics using neural differential equations. Home-page:
 https://github.com/mvinyard/sc-neural-diffeqs Author: Michael E. Vinyard -
 Harvard University - Massachussetts General Hospital - Broad Institute of MIT
 and Harvard Author-email: mvinyard@broadinstitute.org License: MIT Classifier:
 Development Status :: 2 - Pre-Alpha Classifier: Programming Language :: Python
 :: 3.9 Classifier: Intended Audience :: Science/Research Classifier: Topic ::
 Scientific/Engineering :: Bio-Informatics Requires-Python: >3.9.0 Description-
```

### Comparing `scdiffeq-0.0.47rc0/README.md` & `scdiffeq-0.0.47rc1/README.md`

 * *Files identical despite different names*

### Comparing `scdiffeq-0.0.47rc0/scdiffeq/core/__init__.py` & `scdiffeq-0.0.47rc1/scdiffeq/core/__init__.py`

 * *Files identical despite different names*

### Comparing `scdiffeq-0.0.47rc0/scdiffeq/core/_scdiffeq.py` & `scdiffeq-0.0.47rc1/scdiffeq/core/_scdiffeq.py`

 * *Files identical despite different names*

### Comparing `scdiffeq-0.0.47rc0/scdiffeq/core/callbacks/__init__.py` & `scdiffeq-0.0.47rc1/scdiffeq/core/callbacks/__init__.py`

 * *Files identical despite different names*

### Comparing `scdiffeq-0.0.47rc0/scdiffeq/core/callbacks/_intermittent_saves.py` & `scdiffeq-0.0.47rc1/scdiffeq/core/callbacks/_intermittent_saves.py`

 * *Files identical despite different names*

### Comparing `scdiffeq-0.0.47rc0/scdiffeq/core/callbacks/_loss_accounting.py` & `scdiffeq-0.0.47rc1/scdiffeq/core/callbacks/_loss_accounting.py`

 * *Files identical despite different names*

### Comparing `scdiffeq-0.0.47rc0/scdiffeq/core/callbacks/_testing.py` & `scdiffeq-0.0.47rc1/scdiffeq/core/callbacks/_testing.py`

 * *Files identical despite different names*

### Comparing `scdiffeq-0.0.47rc0/scdiffeq/core/callbacks/_visualize_predictions.py` & `scdiffeq-0.0.47rc1/scdiffeq/core/callbacks/_visualize_predictions.py`

 * *Files identical despite different names*

### Comparing `scdiffeq-0.0.47rc0/scdiffeq/core/callbacks/_visualize_tracked_loss.py` & `scdiffeq-0.0.47rc1/scdiffeq/core/callbacks/_visualize_tracked_loss.py`

 * *Files identical despite different names*

### Comparing `scdiffeq-0.0.47rc0/scdiffeq/core/configs/_function_credentialling.py` & `scdiffeq-0.0.47rc1/scdiffeq/core/configs/_function_credentialling.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 
-# import brownian_diffuser  # deprecated
 import neural_diffeqs
-# import torchdiffeq # deprecated
 import torchsde
 
 
 class Credentials:
     def __init__(self, func, adjoint=False):
         self.func = func
         self._adjoint = adjoint
```

### Comparing `scdiffeq-0.0.47rc0/scdiffeq/core/configs/_lightning_callbacks_configuration.py` & `scdiffeq-0.0.47rc1/scdiffeq/core/configs/_lightning_callbacks_configuration.py`

 * *Files identical despite different names*

### Comparing `scdiffeq-0.0.47rc0/scdiffeq/core/configs/_lightning_data_configuration.py` & `scdiffeq-0.0.47rc1/scdiffeq/core/configs/_lightning_data_configuration.py`

 * *Files identical despite different names*

### Comparing `scdiffeq-0.0.47rc0/scdiffeq/core/configs/_lightning_model_configuration_v2.py` & `scdiffeq-0.0.47rc1/scdiffeq/core/configs/_lightning_model_configuration.py`

 * *Files identical despite different names*

### Comparing `scdiffeq-0.0.47rc0/scdiffeq/core/configs/_lightning_trainer_configuration.py` & `scdiffeq-0.0.47rc1/scdiffeq/core/configs/_lightning_trainer_configuration.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,16 @@
 
 # -- import packages: ----------------------------------------------------------
-# from pytorch_lightning import Trainer, loggers
+
 from lightning import Trainer
 from lightning.pytorch import loggers
 import torch
 import os
 
 
-# from licorice_font import font_format
-
-# debug_fmt = font_format("DEBUG", ['YELLOW'])
-# debug_msg = f"- {debug_fmt} | "
-
-
 # -- import local dependencies: ------------------------------------------------
 from ._lightning_callbacks_configuration import LightningCallbacksConfiguration
 from .. import utils, callbacks
 
 
 # -- define typing: ------------------------------------------------------------
 from typing import Union, Dict, List
```

### Comparing `scdiffeq-0.0.47rc0/scdiffeq/core/configs/_time_configuration.py` & `scdiffeq-0.0.47rc1/scdiffeq/core/configs/_time_configuration.py`

 * *Files identical despite different names*

### Comparing `scdiffeq-0.0.47rc0/scdiffeq/core/lightning_models/__init__.py` & `scdiffeq-0.0.47rc1/scdiffeq/core/lightning_models/__init__.py`

 * *Files identical despite different names*

### Comparing `scdiffeq-0.0.47rc0/scdiffeq/core/lightning_models/_lightning_ode.py` & `scdiffeq-0.0.47rc1/scdiffeq/core/lightning_models/_lightning_ode.py`

 * *Files identical despite different names*

### Comparing `scdiffeq-0.0.47rc0/scdiffeq/core/lightning_models/_lightning_ode_fixed_potential.py` & `scdiffeq-0.0.47rc1/scdiffeq/core/lightning_models/_lightning_ode_fixed_potential.py`

 * *Files identical despite different names*

### Comparing `scdiffeq-0.0.47rc0/scdiffeq/core/lightning_models/_lightning_ode_prior_potential.py` & `scdiffeq-0.0.47rc1/scdiffeq/core/lightning_models/_lightning_ode_prior_potential.py`

 * *Files identical despite different names*

### Comparing `scdiffeq-0.0.47rc0/scdiffeq/core/lightning_models/_lightning_ode_vae.py` & `scdiffeq-0.0.47rc1/scdiffeq/core/lightning_models/_lightning_ode_vae.py`

 * *Files identical despite different names*

### Comparing `scdiffeq-0.0.47rc0/scdiffeq/core/lightning_models/_lightning_ode_vae_fixed_potential.py` & `scdiffeq-0.0.47rc1/scdiffeq/core/lightning_models/_lightning_ode_vae_fixed_potential.py`

 * *Files identical despite different names*

### Comparing `scdiffeq-0.0.47rc0/scdiffeq/core/lightning_models/_lightning_ode_vae_prior_potential.py` & `scdiffeq-0.0.47rc1/scdiffeq/core/lightning_models/_lightning_ode_vae_prior_potential.py`

 * *Files identical despite different names*

### Comparing `scdiffeq-0.0.47rc0/scdiffeq/core/lightning_models/_lightning_sde.py` & `scdiffeq-0.0.47rc1/scdiffeq/core/lightning_models/_lightning_sde.py`

 * *Files identical despite different names*

### Comparing `scdiffeq-0.0.47rc0/scdiffeq/core/lightning_models/_lightning_sde_fate_bias_aware.py` & `scdiffeq-0.0.47rc1/scdiffeq/core/lightning_models/_lightning_sde_fate_bias_aware.py`

 * *Files identical despite different names*

### Comparing `scdiffeq-0.0.47rc0/scdiffeq/core/lightning_models/_lightning_sde_fixed_potential.py` & `scdiffeq-0.0.47rc1/scdiffeq/core/lightning_models/_lightning_sde_fixed_potential.py`

 * *Files identical despite different names*

### Comparing `scdiffeq-0.0.47rc0/scdiffeq/core/lightning_models/_lightning_sde_prior_potential.py` & `scdiffeq-0.0.47rc1/scdiffeq/core/lightning_models/_lightning_sde_prior_potential.py`

 * *Files identical despite different names*

### Comparing `scdiffeq-0.0.47rc0/scdiffeq/core/lightning_models/_lightning_sde_vae.py` & `scdiffeq-0.0.47rc1/scdiffeq/core/lightning_models/_lightning_sde_vae.py`

 * *Files identical despite different names*

### Comparing `scdiffeq-0.0.47rc0/scdiffeq/core/lightning_models/_lightning_sde_vae_fate_bias_aware.py` & `scdiffeq-0.0.47rc1/scdiffeq/core/lightning_models/_lightning_sde_vae_fate_bias_aware.py`

 * *Files identical despite different names*

### Comparing `scdiffeq-0.0.47rc0/scdiffeq/core/lightning_models/_lightning_sde_vae_fixed_potential.py` & `scdiffeq-0.0.47rc1/scdiffeq/core/lightning_models/_lightning_sde_vae_fixed_potential.py`

 * *Files identical despite different names*

### Comparing `scdiffeq-0.0.47rc0/scdiffeq/core/lightning_models/_lightning_sde_vae_prior_potential.py` & `scdiffeq-0.0.47rc1/scdiffeq/core/lightning_models/_lightning_sde_vae_prior_potential.py`

 * *Files identical despite different names*

### Comparing `scdiffeq-0.0.47rc0/scdiffeq/core/lightning_models/_lightning_sde_vae_prior_potential_fate_bias_aware.py` & `scdiffeq-0.0.47rc1/scdiffeq/core/lightning_models/_lightning_sde_vae_prior_potential_fate_bias_aware.py`

 * *Files identical despite different names*

### Comparing `scdiffeq-0.0.47rc0/scdiffeq/core/lightning_models/base/_base_lightning_diffeq.py` & `scdiffeq-0.0.47rc1/scdiffeq/core/lightning_models/base/_base_lightning_diffeq.py`

 * *Files identical despite different names*

### Comparing `scdiffeq-0.0.47rc0/scdiffeq/core/lightning_models/base/_batch_processor.py` & `scdiffeq-0.0.47rc1/scdiffeq/core/lightning_models/base/_batch_processor.py`

 * *Files identical despite different names*

### Comparing `scdiffeq-0.0.47rc0/scdiffeq/core/lightning_models/base/_sinkhorn_divergence.py` & `scdiffeq-0.0.47rc1/scdiffeq/core/lightning_models/base/_sinkhorn_divergence.py`

 * *Files identical despite different names*

### Comparing `scdiffeq-0.0.47rc0/scdiffeq/core/lightning_models/mix_ins/__init__.py` & `scdiffeq-0.0.47rc1/scdiffeq/core/lightning_models/mix_ins/__init__.py`

 * *Files identical despite different names*

### Comparing `scdiffeq-0.0.47rc0/scdiffeq/core/lightning_models/mix_ins/_base_forward_mix_in.py` & `scdiffeq-0.0.47rc1/scdiffeq/core/lightning_models/mix_ins/_base_forward_mix_in.py`

 * *Files identical despite different names*

### Comparing `scdiffeq-0.0.47rc0/scdiffeq/core/lightning_models/mix_ins/_drift_prior_mix_in.py` & `scdiffeq-0.0.47rc1/scdiffeq/core/lightning_models/mix_ins/_drift_prior_mix_in.py`

 * *Files identical despite different names*

### Comparing `scdiffeq-0.0.47rc0/scdiffeq/core/lightning_models/mix_ins/_fate_bias_drift_prior_mix_in.py` & `scdiffeq-0.0.47rc1/scdiffeq/core/lightning_models/mix_ins/_fate_bias_drift_prior_mix_in.py`

 * *Files identical despite different names*

### Comparing `scdiffeq-0.0.47rc0/scdiffeq/core/lightning_models/mix_ins/_fate_bias_drift_prior_vae_mix_in.py` & `scdiffeq-0.0.47rc1/scdiffeq/core/lightning_models/mix_ins/_fate_bias_drift_prior_vae_mix_in.py`

 * *Files identical despite different names*

### Comparing `scdiffeq-0.0.47rc0/scdiffeq/core/lightning_models/mix_ins/_fate_bias_mix_in.py` & `scdiffeq-0.0.47rc1/scdiffeq/core/lightning_models/mix_ins/_fate_bias_mix_in.py`

 * *Files identical despite different names*

### Comparing `scdiffeq-0.0.47rc0/scdiffeq/core/lightning_models/mix_ins/_fate_bias_vae_mix_in.py` & `scdiffeq-0.0.47rc1/scdiffeq/core/lightning_models/mix_ins/_fate_bias_vae_mix_in.py`

 * *Files identical despite different names*

### Comparing `scdiffeq-0.0.47rc0/scdiffeq/core/lightning_models/mix_ins/_pre_train_mix_in.py` & `scdiffeq-0.0.47rc1/scdiffeq/core/lightning_models/mix_ins/_pre_train_mix_in.py`

 * *Files identical despite different names*

### Comparing `scdiffeq-0.0.47rc0/scdiffeq/core/lightning_models/mix_ins/_sde_mix_in.py` & `scdiffeq-0.0.47rc1/scdiffeq/core/lightning_models/mix_ins/_sde_mix_in.py`

 * *Files identical despite different names*

### Comparing `scdiffeq-0.0.47rc0/scdiffeq/core/lightning_models/mix_ins/_vae_mix_in.py` & `scdiffeq-0.0.47rc1/scdiffeq/core/lightning_models/mix_ins/_vae_mix_in.py`

 * *Files identical despite different names*

### Comparing `scdiffeq-0.0.47rc0/scdiffeq/core/utils/__init__.py` & `scdiffeq-0.0.47rc1/scdiffeq/core/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `scdiffeq-0.0.47rc0/scdiffeq/core/utils/_abc_parse.py` & `scdiffeq-0.0.47rc1/scdiffeq/core/utils/_abc_parse.py`

 * *Files identical despite different names*

### Comparing `scdiffeq-0.0.47rc0/scdiffeq/core/utils/_anndata_inspector.py` & `scdiffeq-0.0.47rc1/scdiffeq/core/utils/_anndata_inspector.py`

 * *Files identical despite different names*

### Comparing `scdiffeq-0.0.47rc0/scdiffeq/core/utils/_autoparse_base_class.py` & `scdiffeq-0.0.47rc1/scdiffeq/core/utils/_autoparse_base_class.py`

 * *Files identical despite different names*

### Comparing `scdiffeq-0.0.47rc0/scdiffeq/core/utils/_default_neural_sde.py` & `scdiffeq-0.0.47rc1/scdiffeq/core/utils/_default_neural_sde.py`

 * *Files identical despite different names*

### Comparing `scdiffeq-0.0.47rc0/scdiffeq/core/utils/_fast_graph.py` & `scdiffeq-0.0.47rc1/scdiffeq/core/utils/_fast_graph.py`

 * *Files identical despite different names*

### Comparing `scdiffeq-0.0.47rc0/scdiffeq/core/utils/_filter_df.py` & `scdiffeq-0.0.47rc1/scdiffeq/core/utils/_filter_df.py`

 * *Files identical despite different names*

### Comparing `scdiffeq-0.0.47rc0/scdiffeq/core/utils/_flexible_component_loader.py` & `scdiffeq-0.0.47rc1/scdiffeq/core/utils/_flexible_component_loader.py`

 * *Files identical despite different names*

### Comparing `scdiffeq-0.0.47rc0/scdiffeq/core/utils/_function_fetch.py` & `scdiffeq-0.0.47rc1/scdiffeq/core/utils/_function_fetch.py`

 * *Files identical despite different names*

### Comparing `scdiffeq-0.0.47rc0/scdiffeq/core/utils/_function_kwargs.py` & `scdiffeq-0.0.47rc1/scdiffeq/core/utils/_function_kwargs.py`

 * *Files identical despite different names*

### Comparing `scdiffeq-0.0.47rc0/scdiffeq/core/utils/_knn_graph_query.py` & `scdiffeq-0.0.47rc1/scdiffeq/core/utils/_knn_graph_query.py`

 * *Files identical despite different names*

### Comparing `scdiffeq-0.0.47rc0/scdiffeq/core/utils/_logging_learnable_hparams.py` & `scdiffeq-0.0.47rc1/scdiffeq/core/utils/_logging_learnable_hparams.py`

 * *Files identical despite different names*

### Comparing `scdiffeq-0.0.47rc0/scdiffeq/core/utils/_logs.py` & `scdiffeq-0.0.47rc1/scdiffeq/core/utils/_logs.py`

 * *Files identical despite different names*

### Comparing `scdiffeq-0.0.47rc0/scdiffeq/core/utils/_scdiffeq_logger.py` & `scdiffeq-0.0.47rc1/scdiffeq/core/utils/_scdiffeq_logger.py`

 * *Files identical despite different names*

### Comparing `scdiffeq-0.0.47rc0/scdiffeq/io/__init__.py` & `scdiffeq-0.0.47rc1/scdiffeq/io/__init__.py`

 * *Files identical despite different names*

### Comparing `scdiffeq-0.0.47rc0/scdiffeq/io/_pickle_io.py` & `scdiffeq-0.0.47rc1/scdiffeq/io/_pickle_io.py`

 * *Files identical despite different names*

### Comparing `scdiffeq-0.0.47rc0/scdiffeq/io/_read_h5ad.py` & `scdiffeq-0.0.47rc1/scdiffeq/io/_read_h5ad.py`

 * *Files identical despite different names*

### Comparing `scdiffeq-0.0.47rc0/scdiffeq/tools/__init__.py` & `scdiffeq-0.0.47rc1/scdiffeq/tools/__init__.py`

 * *Files identical despite different names*

### Comparing `scdiffeq-0.0.47rc0/scdiffeq/tools/_annotate_cells.py` & `scdiffeq-0.0.47rc1/scdiffeq/tools/_annotate_cells.py`

 * *Files identical despite different names*

### Comparing `scdiffeq-0.0.47rc0/scdiffeq/tools/_data_format.py` & `scdiffeq-0.0.47rc1/scdiffeq/tools/_data_format.py`

 * *Files identical despite different names*

### Comparing `scdiffeq-0.0.47rc0/scdiffeq/tools/_dimension_reduction.py` & `scdiffeq-0.0.47rc1/scdiffeq/tools/_dimension_reduction.py`

 * *Files identical despite different names*

### Comparing `scdiffeq-0.0.47rc0/scdiffeq/tools/_drift_diffusion_state_characterization.py` & `scdiffeq-0.0.47rc1/scdiffeq/tools/_drift_diffusion_state_characterization.py`

 * *Files identical despite different names*

### Comparing `scdiffeq-0.0.47rc0/scdiffeq/tools/_func_from_version.py` & `scdiffeq-0.0.47rc1/scdiffeq/tools/_func_from_version.py`

 * *Files identical despite different names*

### Comparing `scdiffeq-0.0.47rc0/scdiffeq/tools/_hyperparams.py` & `scdiffeq-0.0.47rc1/scdiffeq/tools/_hyperparams.py`

 * *Files identical despite different names*

### Comparing `scdiffeq-0.0.47rc0/scdiffeq/tools/_knn.py` & `scdiffeq-0.0.47rc1/scdiffeq/tools/_knn.py`

 * *Files identical despite different names*

### Comparing `scdiffeq-0.0.47rc0/scdiffeq/tools/_negative_cross_entropy.py` & `scdiffeq-0.0.47rc1/scdiffeq/tools/_negative_cross_entropy.py`

 * *Files identical despite different names*

### Comparing `scdiffeq-0.0.47rc0/scdiffeq/tools/_reconstruct_function.py` & `scdiffeq-0.0.47rc1/scdiffeq/tools/_reconstruct_function.py`

 * *Files identical despite different names*

### Comparing `scdiffeq-0.0.47rc0/scdiffeq/tools/_time_free_sampling.py` & `scdiffeq-0.0.47rc1/scdiffeq/tools/_time_free_sampling.py`

 * *Files identical despite different names*

### Comparing `scdiffeq-0.0.47rc0/scdiffeq/tools/_umap.py` & `scdiffeq-0.0.47rc1/scdiffeq/tools/_umap.py`

 * *Files identical despite different names*

### Comparing `scdiffeq-0.0.47rc0/scdiffeq/tools/_versions.py` & `scdiffeq-0.0.47rc1/scdiffeq/tools/_versions.py`

 * *Files identical despite different names*

### Comparing `scdiffeq-0.0.47rc0/scdiffeq/tools/_x_use.py` & `scdiffeq-0.0.47rc1/scdiffeq/tools/_x_use.py`

 * *Files identical despite different names*

### Comparing `scdiffeq-0.0.47rc0/scdiffeq.egg-info/PKG-INFO` & `scdiffeq-0.0.47rc1/scdiffeq.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scdiffeq
-Version: 0.0.47rc0
+Version: 0.0.47rc1
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
-Metadata-Version: 2.1 Name: scdiffeq Version: 0.0.47rc0 Summary: scDiffEq:
+Metadata-Version: 2.1 Name: scdiffeq Version: 0.0.47rc1 Summary: scDiffEq:
 modelling single-cell dynamics using neural differential equations. Home-page:
 https://github.com/mvinyard/sc-neural-diffeqs Author: Michael E. Vinyard -
 Harvard University - Massachussetts General Hospital - Broad Institute of MIT
 and Harvard Author-email: mvinyard@broadinstitute.org License: MIT Classifier:
 Development Status :: 2 - Pre-Alpha Classifier: Programming Language :: Python
 :: 3.9 Classifier: Intended Audience :: Science/Research Classifier: Topic ::
 Scientific/Engineering :: Bio-Informatics Requires-Python: >3.9.0 Description-
```

### Comparing `scdiffeq-0.0.47rc0/scdiffeq.egg-info/SOURCES.txt` & `scdiffeq-0.0.47rc1/scdiffeq.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,14 @@
 scdiffeq/core/callbacks/_visualize_predictions.py
 scdiffeq/core/callbacks/_visualize_tracked_loss.py
 scdiffeq/core/configs/__init__.py
 scdiffeq/core/configs/_function_credentialling.py
 scdiffeq/core/configs/_lightning_callbacks_configuration.py
 scdiffeq/core/configs/_lightning_data_configuration.py
 scdiffeq/core/configs/_lightning_model_configuration.py
-scdiffeq/core/configs/_lightning_model_configuration_v2.py
 scdiffeq/core/configs/_lightning_trainer_configuration.py
 scdiffeq/core/configs/_time_configuration.py
 scdiffeq/core/lightning_models/__init__.py
 scdiffeq/core/lightning_models/_lightning_ode.py
 scdiffeq/core/lightning_models/_lightning_ode_fixed_potential.py
 scdiffeq/core/lightning_models/_lightning_ode_prior_potential.py
 scdiffeq/core/lightning_models/_lightning_ode_vae.py
```

### Comparing `scdiffeq-0.0.47rc0/setup.py` & `scdiffeq-0.0.47rc1/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 import re
 import os
 import sys
 
 setuptools.setup(
     name="scdiffeq",
-    version="0.0.47rc0",
+    version="0.0.47rc1",
     python_requires=">3.9.0",
     author="Michael E. Vinyard - Harvard University - Massachussetts General Hospital - Broad Institute of MIT and Harvard",
     author_email="mvinyard@broadinstitute.org",
     url="https://github.com/mvinyard/sc-neural-diffeqs",
     long_description=open("README.md", encoding="utf-8").read(),
     long_description_content_type="text/markdown",
     description="scDiffEq: modelling single-cell dynamics using neural differential equations.",
@@ -28,14 +28,15 @@
         "torch-nets>=0.0.4",
         "torch-adata>=0.0.23",
         "autodevice>=0.0.2",
         "brownian-diffuser>=0.0.2",
         "vinplots>=0.0.75",
         "annoyance==0.0.18",
         "ABCParse==0.0.3",
+        "scdiffeq-plots==0.0.1rc2",
     ],
     classifiers=[
         "Development Status :: 2 - Pre-Alpha",
         "Programming Language :: Python :: 3.9",
         "Intended Audience :: Science/Research",
         "Topic :: Scientific/Engineering :: Bio-Informatics",
     ],
```

