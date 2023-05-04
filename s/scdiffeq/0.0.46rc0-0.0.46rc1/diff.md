# Comparing `tmp/scdiffeq-0.0.46rc0.tar.gz` & `tmp/scdiffeq-0.0.46rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scdiffeq-0.0.46rc0.tar", last modified: Thu May  4 21:35:07 2023, max compression
+gzip compressed data, was "scdiffeq-0.0.46rc1.tar", last modified: Thu May  4 21:39:42 2023, max compression
```

## Comparing `scdiffeq-0.0.46rc0.tar` & `scdiffeq-0.0.46rc1.tar`

### file list

```diff
@@ -1,117 +1,117 @@
-drwxr-xr-x   0 mvinyard   (503) staff       (20)        0 2023-05-04 21:35:07.026999 scdiffeq-0.0.46rc0/
--rw-r--r--   0 mvinyard   (503) staff       (20)    34523 2023-05-04 21:33:36.000000 scdiffeq-0.0.46rc0/LICENSE
--rw-r--r--   0 mvinyard   (503) staff       (20)     2299 2023-05-04 21:35:07.026526 scdiffeq-0.0.46rc0/PKG-INFO
--rw-r--r--   0 mvinyard   (503) staff       (20)     1627 2023-05-04 21:33:36.000000 scdiffeq-0.0.46rc0/README.md
-drwxr-xr-x   0 mvinyard   (503) staff       (20)        0 2023-05-04 21:35:06.974057 scdiffeq-0.0.46rc0/scdiffeq/
--rw-r--r--   0 mvinyard   (503) staff       (20)      665 2023-05-04 21:33:36.000000 scdiffeq-0.0.46rc0/scdiffeq/__init__.py
-drwxr-xr-x   0 mvinyard   (503) staff       (20)        0 2023-05-04 21:35:06.975429 scdiffeq-0.0.46rc0/scdiffeq/core/
--rw-r--r--   0 mvinyard   (503) staff       (20)      950 2023-05-04 21:33:36.000000 scdiffeq-0.0.46rc0/scdiffeq/core/__init__.py
-drwxr-xr-x   0 mvinyard   (503) staff       (20)        0 2023-05-04 21:35:06.977453 scdiffeq-0.0.46rc0/scdiffeq/core/_lightning_models/
--rw-r--r--   0 mvinyard   (503) staff       (20)      567 2023-05-04 21:33:36.000000 scdiffeq-0.0.46rc0/scdiffeq/core/_lightning_models/__init__.py
--rw-r--r--   0 mvinyard   (503) staff       (20)     1864 2023-05-04 21:33:36.000000 scdiffeq-0.0.46rc0/scdiffeq/core/_lightning_models/_batch_processor.py
--rw-r--r--   0 mvinyard   (503) staff       (20)     1894 2023-05-04 21:33:36.000000 scdiffeq-0.0.46rc0/scdiffeq/core/_lightning_models/_lightning_drift_net.py
--rw-r--r--   0 mvinyard   (503) staff       (20)     1787 2023-05-04 21:33:36.000000 scdiffeq-0.0.46rc0/scdiffeq/core/_lightning_models/_lightning_ode.py
--rw-r--r--   0 mvinyard   (503) staff       (20)      568 2023-05-04 21:33:36.000000 scdiffeq-0.0.46rc0/scdiffeq/core/_lightning_models/_lightning_potential_sde.py
--rw-r--r--   0 mvinyard   (503) staff       (20)     2340 2023-05-04 21:33:36.000000 scdiffeq-0.0.46rc0/scdiffeq/core/_lightning_models/_lightning_sde.py
--rw-r--r--   0 mvinyard   (503) staff       (20)     3139 2023-05-04 21:33:36.000000 scdiffeq-0.0.46rc0/scdiffeq/core/_lightning_models/_lightning_sde_latent_potential.py
--rw-r--r--   0 mvinyard   (503) staff       (20)     3118 2023-05-04 21:33:36.000000 scdiffeq-0.0.46rc0/scdiffeq/core/_lightning_models/_lightning_vae_sde.py
--rw-r--r--   0 mvinyard   (503) staff       (20)      751 2023-05-04 21:33:36.000000 scdiffeq-0.0.46rc0/scdiffeq/core/_lightning_models/_sinkhorn_divergence.py
-drwxr-xr-x   0 mvinyard   (503) staff       (20)        0 2023-05-04 21:35:06.978632 scdiffeq-0.0.46rc0/scdiffeq/core/_lightning_models/base_models/
--rw-r--r--   0 mvinyard   (503) staff       (20)      267 2023-05-04 21:33:36.000000 scdiffeq-0.0.46rc0/scdiffeq/core/_lightning_models/base_models/__init__.py
--rw-r--r--   0 mvinyard   (503) staff       (20)     1816 2023-05-04 21:33:36.000000 scdiffeq-0.0.46rc0/scdiffeq/core/_lightning_models/base_models/_base_lightning_diffeq.py
--rw-r--r--   0 mvinyard   (503) staff       (20)     1000 2023-05-04 21:33:36.000000 scdiffeq-0.0.46rc0/scdiffeq/core/_lightning_models/base_models/_base_lightning_drift_net.py
--rw-r--r--   0 mvinyard   (503) staff       (20)      606 2023-05-04 21:33:36.000000 scdiffeq-0.0.46rc0/scdiffeq/core/_lightning_models/base_models/_base_lightning_ode.py
--rw-r--r--   0 mvinyard   (503) staff       (20)      675 2023-05-04 21:33:36.000000 scdiffeq-0.0.46rc0/scdiffeq/core/_lightning_models/base_models/_base_lightning_sde.py
--rw-r--r--   0 mvinyard   (503) staff       (20)     1876 2023-05-04 21:33:36.000000 scdiffeq-0.0.46rc0/scdiffeq/core/_lightning_models/base_models/_base_velocity_diffeq.py
-drwxr-xr-x   0 mvinyard   (503) staff       (20)        0 2023-05-04 21:35:06.979880 scdiffeq-0.0.46rc0/scdiffeq/core/_lightning_models/mix_ins/
--rw-r--r--   0 mvinyard   (503) staff       (20)      213 2023-05-04 21:33:36.000000 scdiffeq-0.0.46rc0/scdiffeq/core/_lightning_models/mix_ins/__init__.py
--rw-r--r--   0 mvinyard   (503) staff       (20)      123 2023-05-04 21:33:36.000000 scdiffeq-0.0.46rc0/scdiffeq/core/_lightning_models/mix_ins/_base_mix_in.py
--rw-r--r--   0 mvinyard   (503) staff       (20)      488 2023-05-04 21:33:36.000000 scdiffeq-0.0.46rc0/scdiffeq/core/_lightning_models/mix_ins/_potential_mix_in.py
--rw-r--r--   0 mvinyard   (503) staff       (20)     1282 2023-05-04 21:33:36.000000 scdiffeq-0.0.46rc0/scdiffeq/core/_lightning_models/mix_ins/_pre_train_mix_in.py
--rw-r--r--   0 mvinyard   (503) staff       (20)     1139 2023-05-04 21:33:36.000000 scdiffeq-0.0.46rc0/scdiffeq/core/_lightning_models/mix_ins/_vae_mix_in.py
--rw-r--r--   0 mvinyard   (503) staff       (20)      968 2023-05-04 21:33:36.000000 scdiffeq-0.0.46rc0/scdiffeq/core/_lightning_models/mix_ins/_vae_pre_train_mix_in.py
--rw-r--r--   0 mvinyard   (503) staff       (20)    18660 2023-05-04 21:33:36.000000 scdiffeq-0.0.46rc0/scdiffeq/core/_scdiffeq.py
-drwxr-xr-x   0 mvinyard   (503) staff       (20)        0 2023-05-04 21:35:06.980863 scdiffeq-0.0.46rc0/scdiffeq/core/callbacks/
--rw-r--r--   0 mvinyard   (503) staff       (20)      593 2023-05-04 21:33:36.000000 scdiffeq-0.0.46rc0/scdiffeq/core/callbacks/__init__.py
--rw-r--r--   0 mvinyard   (503) staff       (20)      271 2023-05-04 21:33:36.000000 scdiffeq-0.0.46rc0/scdiffeq/core/callbacks/_gradient_potential_callback.py
--rw-r--r--   0 mvinyard   (503) staff       (20)      834 2023-05-04 21:33:36.000000 scdiffeq-0.0.46rc0/scdiffeq/core/callbacks/_intermittent_saves.py
--rw-r--r--   0 mvinyard   (503) staff       (20)     4853 2023-05-04 21:33:36.000000 scdiffeq-0.0.46rc0/scdiffeq/core/callbacks/_loss_accounting.py
--rw-r--r--   0 mvinyard   (503) staff       (20)      806 2023-05-04 21:33:36.000000 scdiffeq-0.0.46rc0/scdiffeq/core/callbacks/_testing.py
-drwxr-xr-x   0 mvinyard   (503) staff       (20)        0 2023-05-04 21:35:06.982808 scdiffeq-0.0.46rc0/scdiffeq/core/configs/
--rw-r--r--   0 mvinyard   (503) staff       (20)      488 2023-05-04 21:33:36.000000 scdiffeq-0.0.46rc0/scdiffeq/core/configs/__init__.py
--rw-r--r--   0 mvinyard   (503) staff       (20)     2178 2023-05-04 21:33:36.000000 scdiffeq-0.0.46rc0/scdiffeq/core/configs/_function_credentialling.py
--rw-r--r--   0 mvinyard   (503) staff       (20)     1455 2023-05-04 21:33:36.000000 scdiffeq-0.0.46rc0/scdiffeq/core/configs/_lightning_callbacks_configuration.py
--rw-r--r--   0 mvinyard   (503) staff       (20)     1594 2023-05-04 21:33:36.000000 scdiffeq-0.0.46rc0/scdiffeq/core/configs/_lightning_data_configuration.py
--rw-r--r--   0 mvinyard   (503) staff       (20)     5708 2023-05-04 21:33:36.000000 scdiffeq-0.0.46rc0/scdiffeq/core/configs/_lightning_model_configuration.py
--rw-r--r--   0 mvinyard   (503) staff       (20)     1606 2023-05-04 21:33:36.000000 scdiffeq-0.0.46rc0/scdiffeq/core/configs/_lightning_model_configuration_v2.py
--rw-r--r--   0 mvinyard   (503) staff       (20)     5672 2023-05-04 21:33:36.000000 scdiffeq-0.0.46rc0/scdiffeq/core/configs/_lightning_trainer_configuration.py
--rw-r--r--   0 mvinyard   (503) staff       (20)     6074 2023-05-04 21:33:36.000000 scdiffeq-0.0.46rc0/scdiffeq/core/configs/_time_configuration.py
-drwxr-xr-x   0 mvinyard   (503) staff       (20)        0 2023-05-04 21:35:06.985427 scdiffeq-0.0.46rc0/scdiffeq/core/lightning_models/
--rw-r--r--   0 mvinyard   (503) staff       (20)     1079 2023-05-04 21:33:36.000000 scdiffeq-0.0.46rc0/scdiffeq/core/lightning_models/__init__.py
--rw-r--r--   0 mvinyard   (503) staff       (20)     1554 2023-05-04 21:33:36.000000 scdiffeq-0.0.46rc0/scdiffeq/core/lightning_models/_lightning_ode.py
--rw-r--r--   0 mvinyard   (503) staff       (20)     1057 2023-05-04 21:33:36.000000 scdiffeq-0.0.46rc0/scdiffeq/core/lightning_models/_lightning_ode_fixed_potential.py
--rw-r--r--   0 mvinyard   (503) staff       (20)     2351 2023-05-04 21:33:36.000000 scdiffeq-0.0.46rc0/scdiffeq/core/lightning_models/_lightning_ode_prior_potential.py
--rw-r--r--   0 mvinyard   (503) staff       (20)     2456 2023-05-04 21:33:36.000000 scdiffeq-0.0.46rc0/scdiffeq/core/lightning_models/_lightning_ode_vae.py
--rw-r--r--   0 mvinyard   (503) staff       (20)     2277 2023-05-04 21:33:36.000000 scdiffeq-0.0.46rc0/scdiffeq/core/lightning_models/_lightning_ode_vae_fixed_potential.py
--rw-r--r--   0 mvinyard   (503) staff       (20)     3052 2023-05-04 21:33:36.000000 scdiffeq-0.0.46rc0/scdiffeq/core/lightning_models/_lightning_ode_vae_prior_potential.py
--rw-r--r--   0 mvinyard   (503) staff       (20)     1768 2023-05-04 21:33:36.000000 scdiffeq-0.0.46rc0/scdiffeq/core/lightning_models/_lightning_sde.py
--rw-r--r--   0 mvinyard   (503) staff       (20)     1595 2023-05-04 21:33:36.000000 scdiffeq-0.0.46rc0/scdiffeq/core/lightning_models/_lightning_sde_fixed_potential.py
--rw-r--r--   0 mvinyard   (503) staff       (20)     2550 2023-05-04 21:33:36.000000 scdiffeq-0.0.46rc0/scdiffeq/core/lightning_models/_lightning_sde_prior_potential.py
--rw-r--r--   0 mvinyard   (503) staff       (20)     2838 2023-05-04 21:33:36.000000 scdiffeq-0.0.46rc0/scdiffeq/core/lightning_models/_lightning_sde_vae.py
--rw-r--r--   0 mvinyard   (503) staff       (20)     3044 2023-05-04 21:33:36.000000 scdiffeq-0.0.46rc0/scdiffeq/core/lightning_models/_lightning_sde_vae_fixed_potential.py
--rw-r--r--   0 mvinyard   (503) staff       (20)     2909 2023-05-04 21:33:36.000000 scdiffeq-0.0.46rc0/scdiffeq/core/lightning_models/_lightning_sde_vae_prior_potential.py
-drwxr-xr-x   0 mvinyard   (503) staff       (20)        0 2023-05-04 21:35:06.987083 scdiffeq-0.0.46rc0/scdiffeq/core/lightning_models/base/
--rw-r--r--   0 mvinyard   (503) staff       (20)      154 2023-05-04 21:33:36.000000 scdiffeq-0.0.46rc0/scdiffeq/core/lightning_models/base/__init__.py
--rw-r--r--   0 mvinyard   (503) staff       (20)     3415 2023-05-04 21:33:36.000000 scdiffeq-0.0.46rc0/scdiffeq/core/lightning_models/base/_base_lightning_diffeq.py
--rw-r--r--   0 mvinyard   (503) staff       (20)     2458 2023-05-04 21:33:36.000000 scdiffeq-0.0.46rc0/scdiffeq/core/lightning_models/base/_batch_processor.py
--rw-r--r--   0 mvinyard   (503) staff       (20)      752 2023-05-04 21:33:36.000000 scdiffeq-0.0.46rc0/scdiffeq/core/lightning_models/base/_sinkhorn_divergence.py
-drwxr-xr-x   0 mvinyard   (503) staff       (20)        0 2023-05-04 21:35:06.993453 scdiffeq-0.0.46rc0/scdiffeq/core/lightning_models/mix_ins/
--rw-r--r--   0 mvinyard   (503) staff       (20)      282 2023-05-04 21:33:36.000000 scdiffeq-0.0.46rc0/scdiffeq/core/lightning_models/mix_ins/__init__.py
--rw-r--r--   0 mvinyard   (503) staff       (20)      624 2023-05-04 21:33:36.000000 scdiffeq-0.0.46rc0/scdiffeq/core/lightning_models/mix_ins/_base_forward_mix_in.py
--rw-r--r--   0 mvinyard   (503) staff       (20)     2557 2023-05-04 21:33:36.000000 scdiffeq-0.0.46rc0/scdiffeq/core/lightning_models/mix_ins/_drift_prior_mix_in.py
--rw-r--r--   0 mvinyard   (503) staff       (20)      318 2023-05-04 21:33:36.000000 scdiffeq-0.0.46rc0/scdiffeq/core/lightning_models/mix_ins/_potential_mix_in.py
--rw-r--r--   0 mvinyard   (503) staff       (20)      868 2023-05-04 21:33:36.000000 scdiffeq-0.0.46rc0/scdiffeq/core/lightning_models/mix_ins/_pre_train_mix_in.py
--rw-r--r--   0 mvinyard   (503) staff       (20)     2264 2023-05-04 21:33:36.000000 scdiffeq-0.0.46rc0/scdiffeq/core/lightning_models/mix_ins/_sde_mix_in.py
--rw-r--r--   0 mvinyard   (503) staff       (20)     8342 2023-05-04 21:33:36.000000 scdiffeq-0.0.46rc0/scdiffeq/core/lightning_models/mix_ins/_vae_mix_in.py
-drwxr-xr-x   0 mvinyard   (503) staff       (20)        0 2023-05-04 21:35:07.007129 scdiffeq-0.0.46rc0/scdiffeq/core/utils/
--rw-r--r--   0 mvinyard   (503) staff       (20)     1070 2023-05-04 21:33:36.000000 scdiffeq-0.0.46rc0/scdiffeq/core/utils/__init__.py
--rw-r--r--   0 mvinyard   (503) staff       (20)      611 2023-05-04 21:33:36.000000 scdiffeq-0.0.46rc0/scdiffeq/core/utils/_abc_parse.py
--rw-r--r--   0 mvinyard   (503) staff       (20)      931 2023-05-04 21:33:36.000000 scdiffeq-0.0.46rc0/scdiffeq/core/utils/_anndata_inspector.py
--rw-r--r--   0 mvinyard   (503) staff       (20)     2802 2023-05-04 21:33:36.000000 scdiffeq-0.0.46rc0/scdiffeq/core/utils/_autoparse_base_class.py
--rw-r--r--   0 mvinyard   (503) staff       (20)     1040 2023-05-04 21:33:36.000000 scdiffeq-0.0.46rc0/scdiffeq/core/utils/_default_neural_sde.py
--rw-r--r--   0 mvinyard   (503) staff       (20)     1126 2023-05-04 21:33:36.000000 scdiffeq-0.0.46rc0/scdiffeq/core/utils/_fast_graph.py
--rw-r--r--   0 mvinyard   (503) staff       (20)      333 2023-05-04 21:33:36.000000 scdiffeq-0.0.46rc0/scdiffeq/core/utils/_fetch_format.py
--rw-r--r--   0 mvinyard   (503) staff       (20)     1652 2023-05-04 21:33:36.000000 scdiffeq-0.0.46rc0/scdiffeq/core/utils/_function_fetch.py
--rw-r--r--   0 mvinyard   (503) staff       (20)     3402 2023-05-04 21:33:36.000000 scdiffeq-0.0.46rc0/scdiffeq/core/utils/_function_kwargs.py
--rw-r--r--   0 mvinyard   (503) staff       (20)      341 2023-05-04 21:33:36.000000 scdiffeq-0.0.46rc0/scdiffeq/core/utils/_info_message.py
--rw-r--r--   0 mvinyard   (503) staff       (20)      892 2023-05-04 21:33:36.000000 scdiffeq-0.0.46rc0/scdiffeq/core/utils/_logging_learnable_hparams.py
--rw-r--r--   0 mvinyard   (503) staff       (20)      395 2023-05-04 21:33:36.000000 scdiffeq-0.0.46rc0/scdiffeq/core/utils/_normalize_time_to_range.py
--rw-r--r--   0 mvinyard   (503) staff       (20)       83 2023-05-04 21:33:36.000000 scdiffeq-0.0.46rc0/scdiffeq/core/utils/_not_none_type.py
--rw-r--r--   0 mvinyard   (503) staff       (20)     2339 2023-05-04 21:33:36.000000 scdiffeq-0.0.46rc0/scdiffeq/core/utils/_scdiffeq_logger.py
--rw-r--r--   0 mvinyard   (503) staff       (20)      346 2023-05-04 21:33:36.000000 scdiffeq-0.0.46rc0/scdiffeq/core/utils/_sum_normalize.py
-drwxr-xr-x   0 mvinyard   (503) staff       (20)        0 2023-05-04 21:35:07.010165 scdiffeq-0.0.46rc0/scdiffeq/io/
--rw-r--r--   0 mvinyard   (503) staff       (20)      541 2023-05-04 21:33:36.000000 scdiffeq-0.0.46rc0/scdiffeq/io/__init__.py
--rw-r--r--   0 mvinyard   (503) staff       (20)      744 2023-05-04 21:33:36.000000 scdiffeq-0.0.46rc0/scdiffeq/io/_pickle_io.py
--rw-r--r--   0 mvinyard   (503) staff       (20)     1258 2023-05-04 21:33:36.000000 scdiffeq-0.0.46rc0/scdiffeq/io/_read_h5ad.py
-drwxr-xr-x   0 mvinyard   (503) staff       (20)        0 2023-05-04 21:35:07.013449 scdiffeq-0.0.46rc0/scdiffeq/plotting/
--rw-r--r--   0 mvinyard   (503) staff       (20)      462 2023-05-04 21:33:36.000000 scdiffeq-0.0.46rc0/scdiffeq/plotting/__init__.py
-drwxr-xr-x   0 mvinyard   (503) staff       (20)        0 2023-05-04 21:35:07.025435 scdiffeq-0.0.46rc0/scdiffeq/tools/
--rw-r--r--   0 mvinyard   (503) staff       (20)      924 2023-05-04 21:33:36.000000 scdiffeq-0.0.46rc0/scdiffeq/tools/__init__.py
--rw-r--r--   0 mvinyard   (503) staff       (20)     1482 2023-05-04 21:33:36.000000 scdiffeq-0.0.46rc0/scdiffeq/tools/_annotate_cells.py
--rw-r--r--   0 mvinyard   (503) staff       (20)     4607 2023-05-04 21:33:36.000000 scdiffeq-0.0.46rc0/scdiffeq/tools/_dimension_reduction.py
--rw-r--r--   0 mvinyard   (503) staff       (20)     1546 2023-05-04 21:33:36.000000 scdiffeq-0.0.46rc0/scdiffeq/tools/_drift_diffusion_state_characterization.py
--rw-r--r--   0 mvinyard   (503) staff       (20)      202 2023-05-04 21:33:36.000000 scdiffeq-0.0.46rc0/scdiffeq/tools/_fetch.py
--rw-r--r--   0 mvinyard   (503) staff       (20)     1292 2023-05-04 21:33:36.000000 scdiffeq-0.0.46rc0/scdiffeq/tools/_func_from_version.py
--rw-r--r--   0 mvinyard   (503) staff       (20)     1019 2023-05-04 21:33:36.000000 scdiffeq-0.0.46rc0/scdiffeq/tools/_hyperparams.py
--rw-r--r--   0 mvinyard   (503) staff       (20)     5462 2023-05-04 21:33:36.000000 scdiffeq-0.0.46rc0/scdiffeq/tools/_reconstruct_function.py
--rw-r--r--   0 mvinyard   (503) staff       (20)     1470 2023-05-04 21:33:36.000000 scdiffeq-0.0.46rc0/scdiffeq/tools/_time_free_sampling.py
--rw-r--r--   0 mvinyard   (503) staff       (20)      853 2023-05-04 21:33:36.000000 scdiffeq-0.0.46rc0/scdiffeq/tools/_umap.py
--rw-r--r--   0 mvinyard   (503) staff       (20)     1242 2023-05-04 21:33:36.000000 scdiffeq-0.0.46rc0/scdiffeq/tools/_versions.py
-drwxr-xr-x   0 mvinyard   (503) staff       (20)        0 2023-05-04 21:35:06.975003 scdiffeq-0.0.46rc0/scdiffeq.egg-info/
--rw-r--r--   0 mvinyard   (503) staff       (20)     2299 2023-05-04 21:35:06.000000 scdiffeq-0.0.46rc0/scdiffeq.egg-info/PKG-INFO
--rw-r--r--   0 mvinyard   (503) staff       (20)     4634 2023-05-04 21:35:06.000000 scdiffeq-0.0.46rc0/scdiffeq.egg-info/SOURCES.txt
--rw-r--r--   0 mvinyard   (503) staff       (20)        1 2023-05-04 21:35:06.000000 scdiffeq-0.0.46rc0/scdiffeq.egg-info/dependency_links.txt
--rw-r--r--   0 mvinyard   (503) staff       (20)      272 2023-05-04 21:35:06.000000 scdiffeq-0.0.46rc0/scdiffeq.egg-info/requires.txt
--rw-r--r--   0 mvinyard   (503) staff       (20)        9 2023-05-04 21:35:06.000000 scdiffeq-0.0.46rc0/scdiffeq.egg-info/top_level.txt
--rw-r--r--   0 mvinyard   (503) staff       (20)       38 2023-05-04 21:35:07.027209 scdiffeq-0.0.46rc0/setup.cfg
--rw-r--r--   0 mvinyard   (503) staff       (20)     1348 2023-05-04 21:33:36.000000 scdiffeq-0.0.46rc0/setup.py
+drwxr-xr-x   0 mvinyard   (503) staff       (20)        0 2023-05-04 21:39:42.640339 scdiffeq-0.0.46rc1/
+-rw-r--r--   0 mvinyard   (503) staff       (20)    34523 2023-05-04 21:33:36.000000 scdiffeq-0.0.46rc1/LICENSE
+-rw-r--r--   0 mvinyard   (503) staff       (20)     2299 2023-05-04 21:39:42.639987 scdiffeq-0.0.46rc1/PKG-INFO
+-rw-r--r--   0 mvinyard   (503) staff       (20)     1627 2023-05-04 21:33:36.000000 scdiffeq-0.0.46rc1/README.md
+drwxr-xr-x   0 mvinyard   (503) staff       (20)        0 2023-05-04 21:39:42.619005 scdiffeq-0.0.46rc1/scdiffeq/
+-rw-r--r--   0 mvinyard   (503) staff       (20)      665 2023-05-04 21:33:36.000000 scdiffeq-0.0.46rc1/scdiffeq/__init__.py
+drwxr-xr-x   0 mvinyard   (503) staff       (20)        0 2023-05-04 21:39:42.620626 scdiffeq-0.0.46rc1/scdiffeq/core/
+-rw-r--r--   0 mvinyard   (503) staff       (20)      950 2023-05-04 21:33:36.000000 scdiffeq-0.0.46rc1/scdiffeq/core/__init__.py
+drwxr-xr-x   0 mvinyard   (503) staff       (20)        0 2023-05-04 21:39:42.622944 scdiffeq-0.0.46rc1/scdiffeq/core/_lightning_models/
+-rw-r--r--   0 mvinyard   (503) staff       (20)      567 2023-05-04 21:33:36.000000 scdiffeq-0.0.46rc1/scdiffeq/core/_lightning_models/__init__.py
+-rw-r--r--   0 mvinyard   (503) staff       (20)     1864 2023-05-04 21:33:36.000000 scdiffeq-0.0.46rc1/scdiffeq/core/_lightning_models/_batch_processor.py
+-rw-r--r--   0 mvinyard   (503) staff       (20)     1894 2023-05-04 21:33:36.000000 scdiffeq-0.0.46rc1/scdiffeq/core/_lightning_models/_lightning_drift_net.py
+-rw-r--r--   0 mvinyard   (503) staff       (20)     1787 2023-05-04 21:33:36.000000 scdiffeq-0.0.46rc1/scdiffeq/core/_lightning_models/_lightning_ode.py
+-rw-r--r--   0 mvinyard   (503) staff       (20)      568 2023-05-04 21:33:36.000000 scdiffeq-0.0.46rc1/scdiffeq/core/_lightning_models/_lightning_potential_sde.py
+-rw-r--r--   0 mvinyard   (503) staff       (20)     2340 2023-05-04 21:33:36.000000 scdiffeq-0.0.46rc1/scdiffeq/core/_lightning_models/_lightning_sde.py
+-rw-r--r--   0 mvinyard   (503) staff       (20)     3139 2023-05-04 21:33:36.000000 scdiffeq-0.0.46rc1/scdiffeq/core/_lightning_models/_lightning_sde_latent_potential.py
+-rw-r--r--   0 mvinyard   (503) staff       (20)     3118 2023-05-04 21:33:36.000000 scdiffeq-0.0.46rc1/scdiffeq/core/_lightning_models/_lightning_vae_sde.py
+-rw-r--r--   0 mvinyard   (503) staff       (20)      751 2023-05-04 21:33:36.000000 scdiffeq-0.0.46rc1/scdiffeq/core/_lightning_models/_sinkhorn_divergence.py
+drwxr-xr-x   0 mvinyard   (503) staff       (20)        0 2023-05-04 21:39:42.624384 scdiffeq-0.0.46rc1/scdiffeq/core/_lightning_models/base_models/
+-rw-r--r--   0 mvinyard   (503) staff       (20)      267 2023-05-04 21:33:36.000000 scdiffeq-0.0.46rc1/scdiffeq/core/_lightning_models/base_models/__init__.py
+-rw-r--r--   0 mvinyard   (503) staff       (20)     1816 2023-05-04 21:33:36.000000 scdiffeq-0.0.46rc1/scdiffeq/core/_lightning_models/base_models/_base_lightning_diffeq.py
+-rw-r--r--   0 mvinyard   (503) staff       (20)     1000 2023-05-04 21:33:36.000000 scdiffeq-0.0.46rc1/scdiffeq/core/_lightning_models/base_models/_base_lightning_drift_net.py
+-rw-r--r--   0 mvinyard   (503) staff       (20)      606 2023-05-04 21:33:36.000000 scdiffeq-0.0.46rc1/scdiffeq/core/_lightning_models/base_models/_base_lightning_ode.py
+-rw-r--r--   0 mvinyard   (503) staff       (20)      675 2023-05-04 21:33:36.000000 scdiffeq-0.0.46rc1/scdiffeq/core/_lightning_models/base_models/_base_lightning_sde.py
+-rw-r--r--   0 mvinyard   (503) staff       (20)     1876 2023-05-04 21:33:36.000000 scdiffeq-0.0.46rc1/scdiffeq/core/_lightning_models/base_models/_base_velocity_diffeq.py
+drwxr-xr-x   0 mvinyard   (503) staff       (20)        0 2023-05-04 21:39:42.625735 scdiffeq-0.0.46rc1/scdiffeq/core/_lightning_models/mix_ins/
+-rw-r--r--   0 mvinyard   (503) staff       (20)      213 2023-05-04 21:33:36.000000 scdiffeq-0.0.46rc1/scdiffeq/core/_lightning_models/mix_ins/__init__.py
+-rw-r--r--   0 mvinyard   (503) staff       (20)      123 2023-05-04 21:33:36.000000 scdiffeq-0.0.46rc1/scdiffeq/core/_lightning_models/mix_ins/_base_mix_in.py
+-rw-r--r--   0 mvinyard   (503) staff       (20)      488 2023-05-04 21:33:36.000000 scdiffeq-0.0.46rc1/scdiffeq/core/_lightning_models/mix_ins/_potential_mix_in.py
+-rw-r--r--   0 mvinyard   (503) staff       (20)     1282 2023-05-04 21:33:36.000000 scdiffeq-0.0.46rc1/scdiffeq/core/_lightning_models/mix_ins/_pre_train_mix_in.py
+-rw-r--r--   0 mvinyard   (503) staff       (20)     1139 2023-05-04 21:33:36.000000 scdiffeq-0.0.46rc1/scdiffeq/core/_lightning_models/mix_ins/_vae_mix_in.py
+-rw-r--r--   0 mvinyard   (503) staff       (20)      968 2023-05-04 21:33:36.000000 scdiffeq-0.0.46rc1/scdiffeq/core/_lightning_models/mix_ins/_vae_pre_train_mix_in.py
+-rw-r--r--   0 mvinyard   (503) staff       (20)    18660 2023-05-04 21:33:36.000000 scdiffeq-0.0.46rc1/scdiffeq/core/_scdiffeq.py
+drwxr-xr-x   0 mvinyard   (503) staff       (20)        0 2023-05-04 21:39:42.626797 scdiffeq-0.0.46rc1/scdiffeq/core/callbacks/
+-rw-r--r--   0 mvinyard   (503) staff       (20)      593 2023-05-04 21:33:36.000000 scdiffeq-0.0.46rc1/scdiffeq/core/callbacks/__init__.py
+-rw-r--r--   0 mvinyard   (503) staff       (20)      271 2023-05-04 21:33:36.000000 scdiffeq-0.0.46rc1/scdiffeq/core/callbacks/_gradient_potential_callback.py
+-rw-r--r--   0 mvinyard   (503) staff       (20)      834 2023-05-04 21:33:36.000000 scdiffeq-0.0.46rc1/scdiffeq/core/callbacks/_intermittent_saves.py
+-rw-r--r--   0 mvinyard   (503) staff       (20)     4853 2023-05-04 21:33:36.000000 scdiffeq-0.0.46rc1/scdiffeq/core/callbacks/_loss_accounting.py
+-rw-r--r--   0 mvinyard   (503) staff       (20)      806 2023-05-04 21:33:36.000000 scdiffeq-0.0.46rc1/scdiffeq/core/callbacks/_testing.py
+drwxr-xr-x   0 mvinyard   (503) staff       (20)        0 2023-05-04 21:39:42.628134 scdiffeq-0.0.46rc1/scdiffeq/core/configs/
+-rw-r--r--   0 mvinyard   (503) staff       (20)      488 2023-05-04 21:33:36.000000 scdiffeq-0.0.46rc1/scdiffeq/core/configs/__init__.py
+-rw-r--r--   0 mvinyard   (503) staff       (20)     2178 2023-05-04 21:33:36.000000 scdiffeq-0.0.46rc1/scdiffeq/core/configs/_function_credentialling.py
+-rw-r--r--   0 mvinyard   (503) staff       (20)     1455 2023-05-04 21:33:36.000000 scdiffeq-0.0.46rc1/scdiffeq/core/configs/_lightning_callbacks_configuration.py
+-rw-r--r--   0 mvinyard   (503) staff       (20)     1594 2023-05-04 21:33:36.000000 scdiffeq-0.0.46rc1/scdiffeq/core/configs/_lightning_data_configuration.py
+-rw-r--r--   0 mvinyard   (503) staff       (20)     5708 2023-05-04 21:33:36.000000 scdiffeq-0.0.46rc1/scdiffeq/core/configs/_lightning_model_configuration.py
+-rw-r--r--   0 mvinyard   (503) staff       (20)     1606 2023-05-04 21:33:36.000000 scdiffeq-0.0.46rc1/scdiffeq/core/configs/_lightning_model_configuration_v2.py
+-rw-r--r--   0 mvinyard   (503) staff       (20)     5672 2023-05-04 21:33:36.000000 scdiffeq-0.0.46rc1/scdiffeq/core/configs/_lightning_trainer_configuration.py
+-rw-r--r--   0 mvinyard   (503) staff       (20)     6074 2023-05-04 21:33:36.000000 scdiffeq-0.0.46rc1/scdiffeq/core/configs/_time_configuration.py
+drwxr-xr-x   0 mvinyard   (503) staff       (20)        0 2023-05-04 21:39:42.631183 scdiffeq-0.0.46rc1/scdiffeq/core/lightning_models/
+-rw-r--r--   0 mvinyard   (503) staff       (20)     1079 2023-05-04 21:33:36.000000 scdiffeq-0.0.46rc1/scdiffeq/core/lightning_models/__init__.py
+-rw-r--r--   0 mvinyard   (503) staff       (20)     1554 2023-05-04 21:33:36.000000 scdiffeq-0.0.46rc1/scdiffeq/core/lightning_models/_lightning_ode.py
+-rw-r--r--   0 mvinyard   (503) staff       (20)     1057 2023-05-04 21:33:36.000000 scdiffeq-0.0.46rc1/scdiffeq/core/lightning_models/_lightning_ode_fixed_potential.py
+-rw-r--r--   0 mvinyard   (503) staff       (20)     2351 2023-05-04 21:33:36.000000 scdiffeq-0.0.46rc1/scdiffeq/core/lightning_models/_lightning_ode_prior_potential.py
+-rw-r--r--   0 mvinyard   (503) staff       (20)     2456 2023-05-04 21:33:36.000000 scdiffeq-0.0.46rc1/scdiffeq/core/lightning_models/_lightning_ode_vae.py
+-rw-r--r--   0 mvinyard   (503) staff       (20)     2277 2023-05-04 21:33:36.000000 scdiffeq-0.0.46rc1/scdiffeq/core/lightning_models/_lightning_ode_vae_fixed_potential.py
+-rw-r--r--   0 mvinyard   (503) staff       (20)     3052 2023-05-04 21:33:36.000000 scdiffeq-0.0.46rc1/scdiffeq/core/lightning_models/_lightning_ode_vae_prior_potential.py
+-rw-r--r--   0 mvinyard   (503) staff       (20)     1768 2023-05-04 21:33:36.000000 scdiffeq-0.0.46rc1/scdiffeq/core/lightning_models/_lightning_sde.py
+-rw-r--r--   0 mvinyard   (503) staff       (20)     1595 2023-05-04 21:33:36.000000 scdiffeq-0.0.46rc1/scdiffeq/core/lightning_models/_lightning_sde_fixed_potential.py
+-rw-r--r--   0 mvinyard   (503) staff       (20)     2550 2023-05-04 21:33:36.000000 scdiffeq-0.0.46rc1/scdiffeq/core/lightning_models/_lightning_sde_prior_potential.py
+-rw-r--r--   0 mvinyard   (503) staff       (20)     2838 2023-05-04 21:33:36.000000 scdiffeq-0.0.46rc1/scdiffeq/core/lightning_models/_lightning_sde_vae.py
+-rw-r--r--   0 mvinyard   (503) staff       (20)     3044 2023-05-04 21:33:36.000000 scdiffeq-0.0.46rc1/scdiffeq/core/lightning_models/_lightning_sde_vae_fixed_potential.py
+-rw-r--r--   0 mvinyard   (503) staff       (20)     2909 2023-05-04 21:33:36.000000 scdiffeq-0.0.46rc1/scdiffeq/core/lightning_models/_lightning_sde_vae_prior_potential.py
+drwxr-xr-x   0 mvinyard   (503) staff       (20)        0 2023-05-04 21:39:42.631851 scdiffeq-0.0.46rc1/scdiffeq/core/lightning_models/base/
+-rw-r--r--   0 mvinyard   (503) staff       (20)      154 2023-05-04 21:33:36.000000 scdiffeq-0.0.46rc1/scdiffeq/core/lightning_models/base/__init__.py
+-rw-r--r--   0 mvinyard   (503) staff       (20)     3415 2023-05-04 21:33:36.000000 scdiffeq-0.0.46rc1/scdiffeq/core/lightning_models/base/_base_lightning_diffeq.py
+-rw-r--r--   0 mvinyard   (503) staff       (20)     2458 2023-05-04 21:33:36.000000 scdiffeq-0.0.46rc1/scdiffeq/core/lightning_models/base/_batch_processor.py
+-rw-r--r--   0 mvinyard   (503) staff       (20)      752 2023-05-04 21:33:36.000000 scdiffeq-0.0.46rc1/scdiffeq/core/lightning_models/base/_sinkhorn_divergence.py
+drwxr-xr-x   0 mvinyard   (503) staff       (20)        0 2023-05-04 21:39:42.633345 scdiffeq-0.0.46rc1/scdiffeq/core/lightning_models/mix_ins/
+-rw-r--r--   0 mvinyard   (503) staff       (20)      282 2023-05-04 21:33:36.000000 scdiffeq-0.0.46rc1/scdiffeq/core/lightning_models/mix_ins/__init__.py
+-rw-r--r--   0 mvinyard   (503) staff       (20)      624 2023-05-04 21:33:36.000000 scdiffeq-0.0.46rc1/scdiffeq/core/lightning_models/mix_ins/_base_forward_mix_in.py
+-rw-r--r--   0 mvinyard   (503) staff       (20)     2557 2023-05-04 21:33:36.000000 scdiffeq-0.0.46rc1/scdiffeq/core/lightning_models/mix_ins/_drift_prior_mix_in.py
+-rw-r--r--   0 mvinyard   (503) staff       (20)      318 2023-05-04 21:33:36.000000 scdiffeq-0.0.46rc1/scdiffeq/core/lightning_models/mix_ins/_potential_mix_in.py
+-rw-r--r--   0 mvinyard   (503) staff       (20)      868 2023-05-04 21:33:36.000000 scdiffeq-0.0.46rc1/scdiffeq/core/lightning_models/mix_ins/_pre_train_mix_in.py
+-rw-r--r--   0 mvinyard   (503) staff       (20)     2264 2023-05-04 21:33:36.000000 scdiffeq-0.0.46rc1/scdiffeq/core/lightning_models/mix_ins/_sde_mix_in.py
+-rw-r--r--   0 mvinyard   (503) staff       (20)     8342 2023-05-04 21:33:36.000000 scdiffeq-0.0.46rc1/scdiffeq/core/lightning_models/mix_ins/_vae_mix_in.py
+drwxr-xr-x   0 mvinyard   (503) staff       (20)        0 2023-05-04 21:39:42.636524 scdiffeq-0.0.46rc1/scdiffeq/core/utils/
+-rw-r--r--   0 mvinyard   (503) staff       (20)     1070 2023-05-04 21:33:36.000000 scdiffeq-0.0.46rc1/scdiffeq/core/utils/__init__.py
+-rw-r--r--   0 mvinyard   (503) staff       (20)      611 2023-05-04 21:33:36.000000 scdiffeq-0.0.46rc1/scdiffeq/core/utils/_abc_parse.py
+-rw-r--r--   0 mvinyard   (503) staff       (20)      931 2023-05-04 21:33:36.000000 scdiffeq-0.0.46rc1/scdiffeq/core/utils/_anndata_inspector.py
+-rw-r--r--   0 mvinyard   (503) staff       (20)     2802 2023-05-04 21:33:36.000000 scdiffeq-0.0.46rc1/scdiffeq/core/utils/_autoparse_base_class.py
+-rw-r--r--   0 mvinyard   (503) staff       (20)     1040 2023-05-04 21:33:36.000000 scdiffeq-0.0.46rc1/scdiffeq/core/utils/_default_neural_sde.py
+-rw-r--r--   0 mvinyard   (503) staff       (20)     1126 2023-05-04 21:33:36.000000 scdiffeq-0.0.46rc1/scdiffeq/core/utils/_fast_graph.py
+-rw-r--r--   0 mvinyard   (503) staff       (20)      333 2023-05-04 21:33:36.000000 scdiffeq-0.0.46rc1/scdiffeq/core/utils/_fetch_format.py
+-rw-r--r--   0 mvinyard   (503) staff       (20)     1652 2023-05-04 21:33:36.000000 scdiffeq-0.0.46rc1/scdiffeq/core/utils/_function_fetch.py
+-rw-r--r--   0 mvinyard   (503) staff       (20)     3402 2023-05-04 21:33:36.000000 scdiffeq-0.0.46rc1/scdiffeq/core/utils/_function_kwargs.py
+-rw-r--r--   0 mvinyard   (503) staff       (20)      341 2023-05-04 21:33:36.000000 scdiffeq-0.0.46rc1/scdiffeq/core/utils/_info_message.py
+-rw-r--r--   0 mvinyard   (503) staff       (20)      892 2023-05-04 21:33:36.000000 scdiffeq-0.0.46rc1/scdiffeq/core/utils/_logging_learnable_hparams.py
+-rw-r--r--   0 mvinyard   (503) staff       (20)      395 2023-05-04 21:33:36.000000 scdiffeq-0.0.46rc1/scdiffeq/core/utils/_normalize_time_to_range.py
+-rw-r--r--   0 mvinyard   (503) staff       (20)       83 2023-05-04 21:33:36.000000 scdiffeq-0.0.46rc1/scdiffeq/core/utils/_not_none_type.py
+-rw-r--r--   0 mvinyard   (503) staff       (20)     2339 2023-05-04 21:33:36.000000 scdiffeq-0.0.46rc1/scdiffeq/core/utils/_scdiffeq_logger.py
+-rw-r--r--   0 mvinyard   (503) staff       (20)      346 2023-05-04 21:33:36.000000 scdiffeq-0.0.46rc1/scdiffeq/core/utils/_sum_normalize.py
+drwxr-xr-x   0 mvinyard   (503) staff       (20)        0 2023-05-04 21:39:42.637024 scdiffeq-0.0.46rc1/scdiffeq/io/
+-rw-r--r--   0 mvinyard   (503) staff       (20)      541 2023-05-04 21:33:36.000000 scdiffeq-0.0.46rc1/scdiffeq/io/__init__.py
+-rw-r--r--   0 mvinyard   (503) staff       (20)      744 2023-05-04 21:33:36.000000 scdiffeq-0.0.46rc1/scdiffeq/io/_pickle_io.py
+-rw-r--r--   0 mvinyard   (503) staff       (20)     1258 2023-05-04 21:33:36.000000 scdiffeq-0.0.46rc1/scdiffeq/io/_read_h5ad.py
+drwxr-xr-x   0 mvinyard   (503) staff       (20)        0 2023-05-04 21:39:42.637189 scdiffeq-0.0.46rc1/scdiffeq/plotting/
+-rw-r--r--   0 mvinyard   (503) staff       (20)      462 2023-05-04 21:33:36.000000 scdiffeq-0.0.46rc1/scdiffeq/plotting/__init__.py
+drwxr-xr-x   0 mvinyard   (503) staff       (20)        0 2023-05-04 21:39:42.639676 scdiffeq-0.0.46rc1/scdiffeq/tools/
+-rw-r--r--   0 mvinyard   (503) staff       (20)      924 2023-05-04 21:33:36.000000 scdiffeq-0.0.46rc1/scdiffeq/tools/__init__.py
+-rw-r--r--   0 mvinyard   (503) staff       (20)     1482 2023-05-04 21:33:36.000000 scdiffeq-0.0.46rc1/scdiffeq/tools/_annotate_cells.py
+-rw-r--r--   0 mvinyard   (503) staff       (20)     4607 2023-05-04 21:33:36.000000 scdiffeq-0.0.46rc1/scdiffeq/tools/_dimension_reduction.py
+-rw-r--r--   0 mvinyard   (503) staff       (20)     1546 2023-05-04 21:33:36.000000 scdiffeq-0.0.46rc1/scdiffeq/tools/_drift_diffusion_state_characterization.py
+-rw-r--r--   0 mvinyard   (503) staff       (20)      202 2023-05-04 21:33:36.000000 scdiffeq-0.0.46rc1/scdiffeq/tools/_fetch.py
+-rw-r--r--   0 mvinyard   (503) staff       (20)     1292 2023-05-04 21:33:36.000000 scdiffeq-0.0.46rc1/scdiffeq/tools/_func_from_version.py
+-rw-r--r--   0 mvinyard   (503) staff       (20)     1019 2023-05-04 21:33:36.000000 scdiffeq-0.0.46rc1/scdiffeq/tools/_hyperparams.py
+-rw-r--r--   0 mvinyard   (503) staff       (20)     5462 2023-05-04 21:33:36.000000 scdiffeq-0.0.46rc1/scdiffeq/tools/_reconstruct_function.py
+-rw-r--r--   0 mvinyard   (503) staff       (20)     1470 2023-05-04 21:33:36.000000 scdiffeq-0.0.46rc1/scdiffeq/tools/_time_free_sampling.py
+-rw-r--r--   0 mvinyard   (503) staff       (20)      853 2023-05-04 21:33:36.000000 scdiffeq-0.0.46rc1/scdiffeq/tools/_umap.py
+-rw-r--r--   0 mvinyard   (503) staff       (20)     1242 2023-05-04 21:33:36.000000 scdiffeq-0.0.46rc1/scdiffeq/tools/_versions.py
+drwxr-xr-x   0 mvinyard   (503) staff       (20)        0 2023-05-04 21:39:42.620266 scdiffeq-0.0.46rc1/scdiffeq.egg-info/
+-rw-r--r--   0 mvinyard   (503) staff       (20)     2299 2023-05-04 21:39:42.000000 scdiffeq-0.0.46rc1/scdiffeq.egg-info/PKG-INFO
+-rw-r--r--   0 mvinyard   (503) staff       (20)     4634 2023-05-04 21:39:42.000000 scdiffeq-0.0.46rc1/scdiffeq.egg-info/SOURCES.txt
+-rw-r--r--   0 mvinyard   (503) staff       (20)        1 2023-05-04 21:39:42.000000 scdiffeq-0.0.46rc1/scdiffeq.egg-info/dependency_links.txt
+-rw-r--r--   0 mvinyard   (503) staff       (20)      272 2023-05-04 21:39:42.000000 scdiffeq-0.0.46rc1/scdiffeq.egg-info/requires.txt
+-rw-r--r--   0 mvinyard   (503) staff       (20)        9 2023-05-04 21:39:42.000000 scdiffeq-0.0.46rc1/scdiffeq.egg-info/top_level.txt
+-rw-r--r--   0 mvinyard   (503) staff       (20)       38 2023-05-04 21:39:42.640426 scdiffeq-0.0.46rc1/setup.cfg
+-rw-r--r--   0 mvinyard   (503) staff       (20)     1348 2023-05-04 21:39:40.000000 scdiffeq-0.0.46rc1/setup.py
```

### Comparing `scdiffeq-0.0.46rc0/LICENSE` & `scdiffeq-0.0.46rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `scdiffeq-0.0.46rc0/PKG-INFO` & `scdiffeq-0.0.46rc1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scdiffeq
-Version: 0.0.46rc0
+Version: 0.0.46rc1
 Summary: scDiffEq: modelling single-cell dynamics using neural differential equations.
 Home-page: https://github.com/mvinyard/sc-neural-diffeqs
 Author: Michael E. Vinyard - Harvard University - Massachussetts General Hospital - Broad Institute of MIT and Harvard
 Author-email: mvinyard@broadinstitute.org
 License: MIT
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Programming Language :: Python :: 3.7
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: scdiffeq Version: 0.0.46rc0 Summary: scDiffEq:
+Metadata-Version: 2.1 Name: scdiffeq Version: 0.0.46rc1 Summary: scDiffEq:
 modelling single-cell dynamics using neural differential equations. Home-page:
 https://github.com/mvinyard/sc-neural-diffeqs Author: Michael E. Vinyard -
 Harvard University - Massachussetts General Hospital - Broad Institute of MIT
 and Harvard Author-email: mvinyard@broadinstitute.org License: MIT Classifier:
 Development Status :: 2 - Pre-Alpha Classifier: Programming Language :: Python
 :: 3.7 Classifier: Intended Audience :: Science/Research Classifier: Topic ::
 Scientific/Engineering :: Bio-Informatics Requires-Python: >3.9.0 Description-
```

### Comparing `scdiffeq-0.0.46rc0/README.md` & `scdiffeq-0.0.46rc1/README.md`

 * *Files identical despite different names*

### Comparing `scdiffeq-0.0.46rc0/scdiffeq/__init__.py` & `scdiffeq-0.0.46rc1/scdiffeq/__init__.py`

 * *Files identical despite different names*

### Comparing `scdiffeq-0.0.46rc0/scdiffeq/core/__init__.py` & `scdiffeq-0.0.46rc1/scdiffeq/core/__init__.py`

 * *Files identical despite different names*

### Comparing `scdiffeq-0.0.46rc0/scdiffeq/core/_lightning_models/__init__.py` & `scdiffeq-0.0.46rc1/scdiffeq/core/_lightning_models/__init__.py`

 * *Files identical despite different names*

### Comparing `scdiffeq-0.0.46rc0/scdiffeq/core/_lightning_models/_batch_processor.py` & `scdiffeq-0.0.46rc1/scdiffeq/core/_lightning_models/_batch_processor.py`

 * *Files identical despite different names*

### Comparing `scdiffeq-0.0.46rc0/scdiffeq/core/_lightning_models/_lightning_drift_net.py` & `scdiffeq-0.0.46rc1/scdiffeq/core/_lightning_models/_lightning_drift_net.py`

 * *Files identical despite different names*

### Comparing `scdiffeq-0.0.46rc0/scdiffeq/core/_lightning_models/_lightning_ode.py` & `scdiffeq-0.0.46rc1/scdiffeq/core/_lightning_models/_lightning_ode.py`

 * *Files identical despite different names*

### Comparing `scdiffeq-0.0.46rc0/scdiffeq/core/_lightning_models/_lightning_potential_sde.py` & `scdiffeq-0.0.46rc1/scdiffeq/core/_lightning_models/_lightning_potential_sde.py`

 * *Files identical despite different names*

### Comparing `scdiffeq-0.0.46rc0/scdiffeq/core/_lightning_models/_lightning_sde.py` & `scdiffeq-0.0.46rc1/scdiffeq/core/_lightning_models/_lightning_sde.py`

 * *Files identical despite different names*

### Comparing `scdiffeq-0.0.46rc0/scdiffeq/core/_lightning_models/_lightning_sde_latent_potential.py` & `scdiffeq-0.0.46rc1/scdiffeq/core/_lightning_models/_lightning_sde_latent_potential.py`

 * *Files identical despite different names*

### Comparing `scdiffeq-0.0.46rc0/scdiffeq/core/_lightning_models/_lightning_vae_sde.py` & `scdiffeq-0.0.46rc1/scdiffeq/core/_lightning_models/_lightning_vae_sde.py`

 * *Files identical despite different names*

### Comparing `scdiffeq-0.0.46rc0/scdiffeq/core/_lightning_models/_sinkhorn_divergence.py` & `scdiffeq-0.0.46rc1/scdiffeq/core/_lightning_models/_sinkhorn_divergence.py`

 * *Files identical despite different names*

### Comparing `scdiffeq-0.0.46rc0/scdiffeq/core/_lightning_models/base_models/_base_lightning_diffeq.py` & `scdiffeq-0.0.46rc1/scdiffeq/core/_lightning_models/base_models/_base_lightning_diffeq.py`

 * *Files identical despite different names*

### Comparing `scdiffeq-0.0.46rc0/scdiffeq/core/_lightning_models/base_models/_base_lightning_drift_net.py` & `scdiffeq-0.0.46rc1/scdiffeq/core/_lightning_models/base_models/_base_lightning_drift_net.py`

 * *Files identical despite different names*

### Comparing `scdiffeq-0.0.46rc0/scdiffeq/core/_lightning_models/base_models/_base_lightning_ode.py` & `scdiffeq-0.0.46rc1/scdiffeq/core/_lightning_models/base_models/_base_lightning_ode.py`

 * *Files identical despite different names*

### Comparing `scdiffeq-0.0.46rc0/scdiffeq/core/_lightning_models/base_models/_base_lightning_sde.py` & `scdiffeq-0.0.46rc1/scdiffeq/core/_lightning_models/base_models/_base_lightning_sde.py`

 * *Files identical despite different names*

### Comparing `scdiffeq-0.0.46rc0/scdiffeq/core/_lightning_models/base_models/_base_velocity_diffeq.py` & `scdiffeq-0.0.46rc1/scdiffeq/core/_lightning_models/base_models/_base_velocity_diffeq.py`

 * *Files identical despite different names*

### Comparing `scdiffeq-0.0.46rc0/scdiffeq/core/_lightning_models/mix_ins/_pre_train_mix_in.py` & `scdiffeq-0.0.46rc1/scdiffeq/core/_lightning_models/mix_ins/_pre_train_mix_in.py`

 * *Files identical despite different names*

### Comparing `scdiffeq-0.0.46rc0/scdiffeq/core/_lightning_models/mix_ins/_vae_mix_in.py` & `scdiffeq-0.0.46rc1/scdiffeq/core/_lightning_models/mix_ins/_vae_mix_in.py`

 * *Files identical despite different names*

### Comparing `scdiffeq-0.0.46rc0/scdiffeq/core/_lightning_models/mix_ins/_vae_pre_train_mix_in.py` & `scdiffeq-0.0.46rc1/scdiffeq/core/_lightning_models/mix_ins/_vae_pre_train_mix_in.py`

 * *Files identical despite different names*

### Comparing `scdiffeq-0.0.46rc0/scdiffeq/core/_scdiffeq.py` & `scdiffeq-0.0.46rc1/scdiffeq/core/_scdiffeq.py`

 * *Files identical despite different names*

### Comparing `scdiffeq-0.0.46rc0/scdiffeq/core/callbacks/__init__.py` & `scdiffeq-0.0.46rc1/scdiffeq/core/callbacks/__init__.py`

 * *Files identical despite different names*

### Comparing `scdiffeq-0.0.46rc0/scdiffeq/core/callbacks/_intermittent_saves.py` & `scdiffeq-0.0.46rc1/scdiffeq/core/callbacks/_intermittent_saves.py`

 * *Files identical despite different names*

### Comparing `scdiffeq-0.0.46rc0/scdiffeq/core/callbacks/_loss_accounting.py` & `scdiffeq-0.0.46rc1/scdiffeq/core/callbacks/_loss_accounting.py`

 * *Files identical despite different names*

### Comparing `scdiffeq-0.0.46rc0/scdiffeq/core/callbacks/_testing.py` & `scdiffeq-0.0.46rc1/scdiffeq/core/callbacks/_testing.py`

 * *Files identical despite different names*

### Comparing `scdiffeq-0.0.46rc0/scdiffeq/core/configs/_function_credentialling.py` & `scdiffeq-0.0.46rc1/scdiffeq/core/configs/_function_credentialling.py`

 * *Files identical despite different names*

### Comparing `scdiffeq-0.0.46rc0/scdiffeq/core/configs/_lightning_callbacks_configuration.py` & `scdiffeq-0.0.46rc1/scdiffeq/core/configs/_lightning_callbacks_configuration.py`

 * *Files identical despite different names*

### Comparing `scdiffeq-0.0.46rc0/scdiffeq/core/configs/_lightning_data_configuration.py` & `scdiffeq-0.0.46rc1/scdiffeq/core/configs/_lightning_data_configuration.py`

 * *Files identical despite different names*

### Comparing `scdiffeq-0.0.46rc0/scdiffeq/core/configs/_lightning_model_configuration.py` & `scdiffeq-0.0.46rc1/scdiffeq/core/configs/_lightning_model_configuration.py`

 * *Files identical despite different names*

### Comparing `scdiffeq-0.0.46rc0/scdiffeq/core/configs/_lightning_model_configuration_v2.py` & `scdiffeq-0.0.46rc1/scdiffeq/core/configs/_lightning_model_configuration_v2.py`

 * *Files identical despite different names*

### Comparing `scdiffeq-0.0.46rc0/scdiffeq/core/configs/_lightning_trainer_configuration.py` & `scdiffeq-0.0.46rc1/scdiffeq/core/configs/_lightning_trainer_configuration.py`

 * *Files identical despite different names*

### Comparing `scdiffeq-0.0.46rc0/scdiffeq/core/configs/_time_configuration.py` & `scdiffeq-0.0.46rc1/scdiffeq/core/configs/_time_configuration.py`

 * *Files identical despite different names*

### Comparing `scdiffeq-0.0.46rc0/scdiffeq/core/lightning_models/__init__.py` & `scdiffeq-0.0.46rc1/scdiffeq/core/lightning_models/__init__.py`

 * *Files identical despite different names*

### Comparing `scdiffeq-0.0.46rc0/scdiffeq/core/lightning_models/_lightning_ode.py` & `scdiffeq-0.0.46rc1/scdiffeq/core/lightning_models/_lightning_ode.py`

 * *Files identical despite different names*

### Comparing `scdiffeq-0.0.46rc0/scdiffeq/core/lightning_models/_lightning_ode_fixed_potential.py` & `scdiffeq-0.0.46rc1/scdiffeq/core/lightning_models/_lightning_ode_fixed_potential.py`

 * *Files identical despite different names*

### Comparing `scdiffeq-0.0.46rc0/scdiffeq/core/lightning_models/_lightning_ode_prior_potential.py` & `scdiffeq-0.0.46rc1/scdiffeq/core/lightning_models/_lightning_ode_prior_potential.py`

 * *Files identical despite different names*

### Comparing `scdiffeq-0.0.46rc0/scdiffeq/core/lightning_models/_lightning_ode_vae.py` & `scdiffeq-0.0.46rc1/scdiffeq/core/lightning_models/_lightning_ode_vae.py`

 * *Files identical despite different names*

### Comparing `scdiffeq-0.0.46rc0/scdiffeq/core/lightning_models/_lightning_ode_vae_fixed_potential.py` & `scdiffeq-0.0.46rc1/scdiffeq/core/lightning_models/_lightning_ode_vae_fixed_potential.py`

 * *Files identical despite different names*

### Comparing `scdiffeq-0.0.46rc0/scdiffeq/core/lightning_models/_lightning_ode_vae_prior_potential.py` & `scdiffeq-0.0.46rc1/scdiffeq/core/lightning_models/_lightning_ode_vae_prior_potential.py`

 * *Files identical despite different names*

### Comparing `scdiffeq-0.0.46rc0/scdiffeq/core/lightning_models/_lightning_sde.py` & `scdiffeq-0.0.46rc1/scdiffeq/core/lightning_models/_lightning_sde.py`

 * *Files identical despite different names*

### Comparing `scdiffeq-0.0.46rc0/scdiffeq/core/lightning_models/_lightning_sde_fixed_potential.py` & `scdiffeq-0.0.46rc1/scdiffeq/core/lightning_models/_lightning_sde_fixed_potential.py`

 * *Files identical despite different names*

### Comparing `scdiffeq-0.0.46rc0/scdiffeq/core/lightning_models/_lightning_sde_prior_potential.py` & `scdiffeq-0.0.46rc1/scdiffeq/core/lightning_models/_lightning_sde_prior_potential.py`

 * *Files identical despite different names*

### Comparing `scdiffeq-0.0.46rc0/scdiffeq/core/lightning_models/_lightning_sde_vae.py` & `scdiffeq-0.0.46rc1/scdiffeq/core/lightning_models/_lightning_sde_vae.py`

 * *Files identical despite different names*

### Comparing `scdiffeq-0.0.46rc0/scdiffeq/core/lightning_models/_lightning_sde_vae_fixed_potential.py` & `scdiffeq-0.0.46rc1/scdiffeq/core/lightning_models/_lightning_sde_vae_fixed_potential.py`

 * *Files identical despite different names*

### Comparing `scdiffeq-0.0.46rc0/scdiffeq/core/lightning_models/_lightning_sde_vae_prior_potential.py` & `scdiffeq-0.0.46rc1/scdiffeq/core/lightning_models/_lightning_sde_vae_prior_potential.py`

 * *Files identical despite different names*

### Comparing `scdiffeq-0.0.46rc0/scdiffeq/core/lightning_models/base/_base_lightning_diffeq.py` & `scdiffeq-0.0.46rc1/scdiffeq/core/lightning_models/base/_base_lightning_diffeq.py`

 * *Files identical despite different names*

### Comparing `scdiffeq-0.0.46rc0/scdiffeq/core/lightning_models/base/_batch_processor.py` & `scdiffeq-0.0.46rc1/scdiffeq/core/lightning_models/base/_batch_processor.py`

 * *Files identical despite different names*

### Comparing `scdiffeq-0.0.46rc0/scdiffeq/core/lightning_models/base/_sinkhorn_divergence.py` & `scdiffeq-0.0.46rc1/scdiffeq/core/lightning_models/base/_sinkhorn_divergence.py`

 * *Files identical despite different names*

### Comparing `scdiffeq-0.0.46rc0/scdiffeq/core/lightning_models/mix_ins/_base_forward_mix_in.py` & `scdiffeq-0.0.46rc1/scdiffeq/core/lightning_models/mix_ins/_base_forward_mix_in.py`

 * *Files identical despite different names*

### Comparing `scdiffeq-0.0.46rc0/scdiffeq/core/lightning_models/mix_ins/_drift_prior_mix_in.py` & `scdiffeq-0.0.46rc1/scdiffeq/core/lightning_models/mix_ins/_drift_prior_mix_in.py`

 * *Files identical despite different names*

### Comparing `scdiffeq-0.0.46rc0/scdiffeq/core/lightning_models/mix_ins/_pre_train_mix_in.py` & `scdiffeq-0.0.46rc1/scdiffeq/core/lightning_models/mix_ins/_pre_train_mix_in.py`

 * *Files identical despite different names*

### Comparing `scdiffeq-0.0.46rc0/scdiffeq/core/lightning_models/mix_ins/_sde_mix_in.py` & `scdiffeq-0.0.46rc1/scdiffeq/core/lightning_models/mix_ins/_sde_mix_in.py`

 * *Files identical despite different names*

### Comparing `scdiffeq-0.0.46rc0/scdiffeq/core/lightning_models/mix_ins/_vae_mix_in.py` & `scdiffeq-0.0.46rc1/scdiffeq/core/lightning_models/mix_ins/_vae_mix_in.py`

 * *Files identical despite different names*

### Comparing `scdiffeq-0.0.46rc0/scdiffeq/core/utils/__init__.py` & `scdiffeq-0.0.46rc1/scdiffeq/core/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `scdiffeq-0.0.46rc0/scdiffeq/core/utils/_abc_parse.py` & `scdiffeq-0.0.46rc1/scdiffeq/core/utils/_abc_parse.py`

 * *Files identical despite different names*

### Comparing `scdiffeq-0.0.46rc0/scdiffeq/core/utils/_anndata_inspector.py` & `scdiffeq-0.0.46rc1/scdiffeq/core/utils/_anndata_inspector.py`

 * *Files identical despite different names*

### Comparing `scdiffeq-0.0.46rc0/scdiffeq/core/utils/_autoparse_base_class.py` & `scdiffeq-0.0.46rc1/scdiffeq/core/utils/_autoparse_base_class.py`

 * *Files identical despite different names*

### Comparing `scdiffeq-0.0.46rc0/scdiffeq/core/utils/_default_neural_sde.py` & `scdiffeq-0.0.46rc1/scdiffeq/core/utils/_default_neural_sde.py`

 * *Files identical despite different names*

### Comparing `scdiffeq-0.0.46rc0/scdiffeq/core/utils/_fast_graph.py` & `scdiffeq-0.0.46rc1/scdiffeq/core/utils/_fast_graph.py`

 * *Files identical despite different names*

### Comparing `scdiffeq-0.0.46rc0/scdiffeq/core/utils/_function_fetch.py` & `scdiffeq-0.0.46rc1/scdiffeq/core/utils/_function_fetch.py`

 * *Files identical despite different names*

### Comparing `scdiffeq-0.0.46rc0/scdiffeq/core/utils/_function_kwargs.py` & `scdiffeq-0.0.46rc1/scdiffeq/core/utils/_function_kwargs.py`

 * *Files identical despite different names*

### Comparing `scdiffeq-0.0.46rc0/scdiffeq/core/utils/_logging_learnable_hparams.py` & `scdiffeq-0.0.46rc1/scdiffeq/core/utils/_logging_learnable_hparams.py`

 * *Files identical despite different names*

### Comparing `scdiffeq-0.0.46rc0/scdiffeq/core/utils/_scdiffeq_logger.py` & `scdiffeq-0.0.46rc1/scdiffeq/core/utils/_scdiffeq_logger.py`

 * *Files identical despite different names*

### Comparing `scdiffeq-0.0.46rc0/scdiffeq/io/__init__.py` & `scdiffeq-0.0.46rc1/scdiffeq/io/__init__.py`

 * *Files identical despite different names*

### Comparing `scdiffeq-0.0.46rc0/scdiffeq/io/_pickle_io.py` & `scdiffeq-0.0.46rc1/scdiffeq/io/_pickle_io.py`

 * *Files identical despite different names*

### Comparing `scdiffeq-0.0.46rc0/scdiffeq/io/_read_h5ad.py` & `scdiffeq-0.0.46rc1/scdiffeq/io/_read_h5ad.py`

 * *Files identical despite different names*

### Comparing `scdiffeq-0.0.46rc0/scdiffeq/tools/__init__.py` & `scdiffeq-0.0.46rc1/scdiffeq/tools/__init__.py`

 * *Files identical despite different names*

### Comparing `scdiffeq-0.0.46rc0/scdiffeq/tools/_annotate_cells.py` & `scdiffeq-0.0.46rc1/scdiffeq/tools/_annotate_cells.py`

 * *Files identical despite different names*

### Comparing `scdiffeq-0.0.46rc0/scdiffeq/tools/_dimension_reduction.py` & `scdiffeq-0.0.46rc1/scdiffeq/tools/_dimension_reduction.py`

 * *Files identical despite different names*

### Comparing `scdiffeq-0.0.46rc0/scdiffeq/tools/_drift_diffusion_state_characterization.py` & `scdiffeq-0.0.46rc1/scdiffeq/tools/_drift_diffusion_state_characterization.py`

 * *Files identical despite different names*

### Comparing `scdiffeq-0.0.46rc0/scdiffeq/tools/_func_from_version.py` & `scdiffeq-0.0.46rc1/scdiffeq/tools/_func_from_version.py`

 * *Files identical despite different names*

### Comparing `scdiffeq-0.0.46rc0/scdiffeq/tools/_hyperparams.py` & `scdiffeq-0.0.46rc1/scdiffeq/tools/_hyperparams.py`

 * *Files identical despite different names*

### Comparing `scdiffeq-0.0.46rc0/scdiffeq/tools/_reconstruct_function.py` & `scdiffeq-0.0.46rc1/scdiffeq/tools/_reconstruct_function.py`

 * *Files identical despite different names*

### Comparing `scdiffeq-0.0.46rc0/scdiffeq/tools/_time_free_sampling.py` & `scdiffeq-0.0.46rc1/scdiffeq/tools/_time_free_sampling.py`

 * *Files identical despite different names*

### Comparing `scdiffeq-0.0.46rc0/scdiffeq/tools/_umap.py` & `scdiffeq-0.0.46rc1/scdiffeq/tools/_umap.py`

 * *Files identical despite different names*

### Comparing `scdiffeq-0.0.46rc0/scdiffeq/tools/_versions.py` & `scdiffeq-0.0.46rc1/scdiffeq/tools/_versions.py`

 * *Files identical despite different names*

### Comparing `scdiffeq-0.0.46rc0/scdiffeq.egg-info/PKG-INFO` & `scdiffeq-0.0.46rc1/scdiffeq.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scdiffeq
-Version: 0.0.46rc0
+Version: 0.0.46rc1
 Summary: scDiffEq: modelling single-cell dynamics using neural differential equations.
 Home-page: https://github.com/mvinyard/sc-neural-diffeqs
 Author: Michael E. Vinyard - Harvard University - Massachussetts General Hospital - Broad Institute of MIT and Harvard
 Author-email: mvinyard@broadinstitute.org
 License: MIT
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Programming Language :: Python :: 3.7
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: scdiffeq Version: 0.0.46rc0 Summary: scDiffEq:
+Metadata-Version: 2.1 Name: scdiffeq Version: 0.0.46rc1 Summary: scDiffEq:
 modelling single-cell dynamics using neural differential equations. Home-page:
 https://github.com/mvinyard/sc-neural-diffeqs Author: Michael E. Vinyard -
 Harvard University - Massachussetts General Hospital - Broad Institute of MIT
 and Harvard Author-email: mvinyard@broadinstitute.org License: MIT Classifier:
 Development Status :: 2 - Pre-Alpha Classifier: Programming Language :: Python
 :: 3.7 Classifier: Intended Audience :: Science/Research Classifier: Topic ::
 Scientific/Engineering :: Bio-Informatics Requires-Python: >3.9.0 Description-
```

### Comparing `scdiffeq-0.0.46rc0/scdiffeq.egg-info/SOURCES.txt` & `scdiffeq-0.0.46rc1/scdiffeq.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `scdiffeq-0.0.46rc0/setup.py` & `scdiffeq-0.0.46rc1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 import re
 import os
 import sys
 
 setuptools.setup(
     name="scdiffeq",
-    version="0.0.46rc0",
+    version="0.0.46rc1",
     python_requires=">3.9.0",
     author="Michael E. Vinyard - Harvard University - Massachussetts General Hospital - Broad Institute of MIT and Harvard",
     author_email="mvinyard@broadinstitute.org",
     url="https://github.com/mvinyard/sc-neural-diffeqs",
     long_description=open("README.md", encoding="utf-8").read(),
     long_description_content_type="text/markdown",
     description="scDiffEq: modelling single-cell dynamics using neural differential equations.",
@@ -25,15 +25,15 @@
         "umap-learn>=0.5.3",
         "lightning>=2.0.1",
         "neural-diffeqs==0.3.1rc0",
         "torch-nets>=0.0.4",
         "torch-adata>=0.0.20",
         "autodevice>=0.0.2",
         "brownian-diffuser>=0.0.2",
-        "vinplots>=0.0.76",
+        "vinplots>=0.0.75",
     ],
     classifiers=[
         "Development Status :: 2 - Pre-Alpha",
         "Programming Language :: Python :: 3.7",
         "Intended Audience :: Science/Research",
         "Topic :: Scientific/Engineering :: Bio-Informatics",
     ],
```

