# Comparing `tmp/fmldk-1.2.1.tar.gz` & `tmp/fmldk-1.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fmldk-1.2.1.tar", last modified: Wed May  3 06:13:51 2023, max compression
+gzip compressed data, was "fmldk-1.2.2.tar", last modified: Thu May  4 06:32:59 2023, max compression
```

## Comparing `fmldk-1.2.1.tar` & `fmldk-1.2.2.tar`

### file list

```diff
@@ -1,93 +1,93 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 06:13:51.477582 fmldk-1.2.1/
--rw-r--r--   0 runner    (1001) docker     (123)    30440 2023-05-03 06:13:51.477582 fmldk-1.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    30262 2023-05-03 06:13:40.000000 fmldk-1.2.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 06:13:51.461582 fmldk-1.2.1/ctfr/
--rw-r--r--   0 runner    (1001) docker     (123)      254 2023-05-03 06:13:40.000000 fmldk-1.2.1/ctfr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    55520 2023-05-03 06:13:40.000000 fmldk-1.2.1/ctfr/ctfr_data.py
--rw-r--r--   0 runner    (1001) docker     (123)    13307 2023-05-03 06:13:40.000000 fmldk-1.2.1/ctfr/ctfr_losses.py
--rw-r--r--   0 runner    (1001) docker     (123)    12423 2023-05-03 06:13:40.000000 fmldk-1.2.1/ctfr/ctfr_losses_bkp.py
--rw-r--r--   0 runner    (1001) docker     (123)   113137 2023-05-03 06:13:40.000000 fmldk-1.2.1/ctfr/ctfr_models.py
--rw-r--r--   0 runner    (1001) docker     (123)   105725 2023-05-03 06:13:40.000000 fmldk-1.2.1/ctfr/ctfr_models_v0.1.29.py
--rw-r--r--   0 runner    (1001) docker     (123)   111862 2023-05-03 06:13:40.000000 fmldk-1.2.1/ctfr/ctfr_models_v0.1.31.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 06:13:51.461582 fmldk-1.2.1/ctfrv2/
--rw-r--r--   0 runner    (1001) docker     (123)      307 2023-05-03 06:13:40.000000 fmldk-1.2.1/ctfrv2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    55580 2023-05-03 06:13:40.000000 fmldk-1.2.1/ctfrv2/ctfrv2_data.py
--rw-r--r--   0 runner    (1001) docker     (123)    42022 2023-05-03 06:13:40.000000 fmldk-1.2.1/ctfrv2/ctfrv2_global_scaled_data.py
--rw-r--r--   0 runner    (1001) docker     (123)    13260 2023-05-03 06:13:40.000000 fmldk-1.2.1/ctfrv2/ctfrv2_losses.py
--rw-r--r--   0 runner    (1001) docker     (123)    86435 2023-05-03 06:13:40.000000 fmldk-1.2.1/ctfrv2/ctfrv2_models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 06:13:51.461582 fmldk-1.2.1/ctfrv2_gpu/
--rw-r--r--   0 runner    (1001) docker     (123)      277 2023-05-03 06:13:40.000000 fmldk-1.2.1/ctfrv2_gpu/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    36457 2023-05-03 06:13:40.000000 fmldk-1.2.1/ctfrv2_gpu/ctfrv2_data_gpu.py
--rw-r--r--   0 runner    (1001) docker     (123)    17684 2023-05-03 06:13:40.000000 fmldk-1.2.1/ctfrv2_gpu/ctfrv2_losses_gpu.py
--rw-r--r--   0 runner    (1001) docker     (123)    78757 2023-05-03 06:13:40.000000 fmldk-1.2.1/ctfrv2_gpu/ctfrv2_model_gpu.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 06:13:51.465582 fmldk-1.2.1/eda/
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-03 06:13:40.000000 fmldk-1.2.1/eda/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    38969 2023-05-03 06:13:40.000000 fmldk-1.2.1/eda/eda_lib.py
--rw-r--r--   0 runner    (1001) docker     (123)    21432 2023-05-03 06:13:40.000000 fmldk-1.2.1/eda/eda_lib_v0.1.18.py
--rw-r--r--   0 runner    (1001) docker     (123)    22984 2023-05-03 06:13:40.000000 fmldk-1.2.1/eda/eda_lib_v0.1.19.py
--rw-r--r--   0 runner    (1001) docker     (123)    34650 2023-05-03 06:13:40.000000 fmldk-1.2.1/eda/eda_lib_v0.1.37.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 06:13:51.465582 fmldk-1.2.1/fmldk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    30440 2023-05-03 06:13:51.000000 fmldk-1.2.1/fmldk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1877 2023-05-03 06:13:51.000000 fmldk-1.2.1/fmldk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-03 06:13:51.000000 fmldk-1.2.1/fmldk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-05-03 06:13:51.000000 fmldk-1.2.1/fmldk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-05-03 06:13:51.000000 fmldk-1.2.1/fmldk.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 06:13:51.465582 fmldk-1.2.1/sage/
--rw-r--r--   0 runner    (1001) docker     (123)      222 2023-05-03 06:13:40.000000 fmldk-1.2.1/sage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    46655 2023-05-03 06:13:40.000000 fmldk-1.2.1/sage/sage_data.py
--rw-r--r--   0 runner    (1001) docker     (123)    42404 2023-05-03 06:13:40.000000 fmldk-1.2.1/sage/sage_data_old.py
--rw-r--r--   0 runner    (1001) docker     (123)    42020 2023-05-03 06:13:40.000000 fmldk-1.2.1/sage/sage_global_scaled_data_old.py
--rw-r--r--   0 runner    (1001) docker     (123)    17695 2023-05-03 06:13:40.000000 fmldk-1.2.1/sage/sage_losses.py
--rw-r--r--   0 runner    (1001) docker     (123)    14320 2023-05-03 06:13:40.000000 fmldk-1.2.1/sage/sage_losses_old.py
--rw-r--r--   0 runner    (1001) docker     (123)    86777 2023-05-03 06:13:40.000000 fmldk-1.2.1/sage/sage_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    83909 2023-05-03 06:13:40.000000 fmldk-1.2.1/sage/sage_model_old.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 06:13:51.469582 fmldk-1.2.1/sage_gpu/
--rw-r--r--   0 runner    (1001) docker     (123)      246 2023-05-03 06:13:40.000000 fmldk-1.2.1/sage_gpu/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    36438 2023-05-03 06:13:40.000000 fmldk-1.2.1/sage_gpu/sage_data_gpu.py
--rw-r--r--   0 runner    (1001) docker     (123)    17683 2023-05-03 06:13:40.000000 fmldk-1.2.1/sage_gpu/sage_losses_gpu.py
--rw-r--r--   0 runner    (1001) docker     (123)    87798 2023-05-03 06:13:40.000000 fmldk-1.2.1/sage_gpu/sage_model_gpu.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-03 06:13:51.477582 fmldk-1.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      795 2023-05-03 06:13:40.000000 fmldk-1.2.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 06:13:51.469582 fmldk-1.2.1/stctn/
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-05-03 06:13:40.000000 fmldk-1.2.1/stctn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    55190 2023-05-03 06:13:40.000000 fmldk-1.2.1/stctn/stctn_data.py
--rw-r--r--   0 runner    (1001) docker     (123)    13307 2023-05-03 06:13:40.000000 fmldk-1.2.1/stctn/stctn_losses.py
--rw-r--r--   0 runner    (1001) docker     (123)    12423 2023-05-03 06:13:40.000000 fmldk-1.2.1/stctn/stctn_losses_bkp.py
--rw-r--r--   0 runner    (1001) docker     (123)    53648 2023-05-03 06:13:40.000000 fmldk-1.2.1/stctn/stctn_models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 06:13:51.473582 fmldk-1.2.1/tfr/
--rw-r--r--   0 runner    (1001) docker     (123)      352 2023-05-03 06:13:40.000000 fmldk-1.2.1/tfr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    55577 2023-05-03 06:13:40.000000 fmldk-1.2.1/tfr/tfr_data.py
--rw-r--r--   0 runner    (1001) docker     (123)    23667 2023-05-03 06:13:40.000000 fmldk-1.2.1/tfr/tfr_data_v0.1.11.py
--rw-r--r--   0 runner    (1001) docker     (123)    26192 2023-05-03 06:13:40.000000 fmldk-1.2.1/tfr/tfr_data_v0.1.12.py
--rw-r--r--   0 runner    (1001) docker     (123)    37924 2023-05-03 06:13:40.000000 fmldk-1.2.1/tfr/tfr_data_v0.1.14.py
--rw-r--r--   0 runner    (1001) docker     (123)    40021 2023-05-03 06:13:40.000000 fmldk-1.2.1/tfr/tfr_data_v0.1.15.py
--rw-r--r--   0 runner    (1001) docker     (123)    46425 2023-05-03 06:13:40.000000 fmldk-1.2.1/tfr/tfr_data_v0.1.16.py
--rw-r--r--   0 runner    (1001) docker     (123)    54017 2023-05-03 06:13:40.000000 fmldk-1.2.1/tfr/tfr_data_v0.1.18.py
--rw-r--r--   0 runner    (1001) docker     (123)    55773 2023-05-03 06:13:40.000000 fmldk-1.2.1/tfr/tfr_data_v0.1.21.py
--rw-r--r--   0 runner    (1001) docker     (123)   107319 2023-05-03 06:13:40.000000 fmldk-1.2.1/tfr/tfr_local_block_sparse_attention.py
--rw-r--r--   0 runner    (1001) docker     (123)    93067 2023-05-03 06:13:40.000000 fmldk-1.2.1/tfr/tfr_local_block_sparse_attention_v0.1.10.py
--rw-r--r--   0 runner    (1001) docker     (123)    97067 2023-05-03 06:13:40.000000 fmldk-1.2.1/tfr/tfr_local_block_sparse_attention_v0.1.12.py
--rw-r--r--   0 runner    (1001) docker     (123)    13292 2023-05-03 06:13:40.000000 fmldk-1.2.1/tfr/tfr_losses.py
--rw-r--r--   0 runner    (1001) docker     (123)    12423 2023-05-03 06:13:40.000000 fmldk-1.2.1/tfr/tfr_losses_bkp.py
--rw-r--r--   0 runner    (1001) docker     (123)   113988 2023-05-03 06:13:40.000000 fmldk-1.2.1/tfr/tfr_models.py
--rw-r--r--   0 runner    (1001) docker     (123)    96299 2023-05-03 06:13:40.000000 fmldk-1.2.1/tfr/tfr_models_v0.1.10.py
--rw-r--r--   0 runner    (1001) docker     (123)   100101 2023-05-03 06:13:40.000000 fmldk-1.2.1/tfr/tfr_models_v0.1.11.py
--rw-r--r--   0 runner    (1001) docker     (123)   109483 2023-05-03 06:13:40.000000 fmldk-1.2.1/tfr/tfr_models_v0.1.23.py
--rw-r--r--   0 runner    (1001) docker     (123)   114250 2023-05-03 06:13:40.000000 fmldk-1.2.1/tfr/tfr_models_v0.1.31.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 06:13:51.473582 fmldk-1.2.1/tft/
--rw-r--r--   0 runner    (1001) docker     (123)      282 2023-05-03 06:13:40.000000 fmldk-1.2.1/tft/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    46653 2023-05-03 06:13:40.000000 fmldk-1.2.1/tft/tft_data.py
--rw-r--r--   0 runner    (1001) docker     (123)    42403 2023-05-03 06:13:40.000000 fmldk-1.2.1/tft/tft_data_old.py
--rw-r--r--   0 runner    (1001) docker     (123)    55578 2023-05-03 06:13:40.000000 fmldk-1.2.1/tft/tft_data_v1.1.3.py
--rw-r--r--   0 runner    (1001) docker     (123)    62667 2023-05-03 06:13:40.000000 fmldk-1.2.1/tft/tft_data_v1.1.7.py
--rw-r--r--   0 runner    (1001) docker     (123)    42019 2023-05-03 06:13:40.000000 fmldk-1.2.1/tft/tft_global_scaled_data.py
--rw-r--r--   0 runner    (1001) docker     (123)    17695 2023-05-03 06:13:40.000000 fmldk-1.2.1/tft/tft_losses.py
--rw-r--r--   0 runner    (1001) docker     (123)    84122 2023-05-03 06:13:40.000000 fmldk-1.2.1/tft/tft_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    64043 2023-05-03 06:13:40.000000 fmldk-1.2.1/tft/tft_model_v0.1.26.py
--rw-r--r--   0 runner    (1001) docker     (123)    65090 2023-05-03 06:13:40.000000 fmldk-1.2.1/tft/tft_model_v0.1.31.py
--rw-r--r--   0 runner    (1001) docker     (123)    73433 2023-05-03 06:13:40.000000 fmldk-1.2.1/tft/tft_model_v1.1.3.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 06:13:51.477582 fmldk-1.2.1/tft_gpu/
--rw-r--r--   0 runner    (1001) docker     (123)      251 2023-05-03 06:13:40.000000 fmldk-1.2.1/tft_gpu/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    36454 2023-05-03 06:13:40.000000 fmldk-1.2.1/tft_gpu/tft_data_gpu.py
--rw-r--r--   0 runner    (1001) docker     (123)    17695 2023-05-03 06:13:40.000000 fmldk-1.2.1/tft_gpu/tft_losses_gpu.py
--rw-r--r--   0 runner    (1001) docker     (123)    78604 2023-05-03 06:13:40.000000 fmldk-1.2.1/tft_gpu/tft_model_gpu.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 06:32:59.030654 fmldk-1.2.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    30440 2023-05-04 06:32:59.030654 fmldk-1.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    30262 2023-05-04 06:32:41.000000 fmldk-1.2.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 06:32:59.010654 fmldk-1.2.2/ctfr/
+-rw-r--r--   0 runner    (1001) docker     (123)      254 2023-05-04 06:32:41.000000 fmldk-1.2.2/ctfr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    55520 2023-05-04 06:32:41.000000 fmldk-1.2.2/ctfr/ctfr_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13307 2023-05-04 06:32:41.000000 fmldk-1.2.2/ctfr/ctfr_losses.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12423 2023-05-04 06:32:41.000000 fmldk-1.2.2/ctfr/ctfr_losses_bkp.py
+-rw-r--r--   0 runner    (1001) docker     (123)   113137 2023-05-04 06:32:41.000000 fmldk-1.2.2/ctfr/ctfr_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)   105725 2023-05-04 06:32:41.000000 fmldk-1.2.2/ctfr/ctfr_models_v0.1.29.py
+-rw-r--r--   0 runner    (1001) docker     (123)   111862 2023-05-04 06:32:41.000000 fmldk-1.2.2/ctfr/ctfr_models_v0.1.31.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 06:32:59.010654 fmldk-1.2.2/ctfrv2/
+-rw-r--r--   0 runner    (1001) docker     (123)      307 2023-05-04 06:32:41.000000 fmldk-1.2.2/ctfrv2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    55580 2023-05-04 06:32:41.000000 fmldk-1.2.2/ctfrv2/ctfrv2_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42022 2023-05-04 06:32:41.000000 fmldk-1.2.2/ctfrv2/ctfrv2_global_scaled_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13260 2023-05-04 06:32:41.000000 fmldk-1.2.2/ctfrv2/ctfrv2_losses.py
+-rw-r--r--   0 runner    (1001) docker     (123)    86435 2023-05-04 06:32:41.000000 fmldk-1.2.2/ctfrv2/ctfrv2_models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 06:32:59.014654 fmldk-1.2.2/ctfrv2_gpu/
+-rw-r--r--   0 runner    (1001) docker     (123)      277 2023-05-04 06:32:41.000000 fmldk-1.2.2/ctfrv2_gpu/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36574 2023-05-04 06:32:41.000000 fmldk-1.2.2/ctfrv2_gpu/ctfrv2_data_gpu.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17684 2023-05-04 06:32:41.000000 fmldk-1.2.2/ctfrv2_gpu/ctfrv2_losses_gpu.py
+-rw-r--r--   0 runner    (1001) docker     (123)    78757 2023-05-04 06:32:41.000000 fmldk-1.2.2/ctfrv2_gpu/ctfrv2_model_gpu.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 06:32:59.014654 fmldk-1.2.2/eda/
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-04 06:32:41.000000 fmldk-1.2.2/eda/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38969 2023-05-04 06:32:41.000000 fmldk-1.2.2/eda/eda_lib.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21432 2023-05-04 06:32:41.000000 fmldk-1.2.2/eda/eda_lib_v0.1.18.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22984 2023-05-04 06:32:41.000000 fmldk-1.2.2/eda/eda_lib_v0.1.19.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34650 2023-05-04 06:32:41.000000 fmldk-1.2.2/eda/eda_lib_v0.1.37.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 06:32:59.014654 fmldk-1.2.2/fmldk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    30440 2023-05-04 06:32:58.000000 fmldk-1.2.2/fmldk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1877 2023-05-04 06:32:59.000000 fmldk-1.2.2/fmldk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 06:32:58.000000 fmldk-1.2.2/fmldk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-05-04 06:32:58.000000 fmldk-1.2.2/fmldk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-05-04 06:32:58.000000 fmldk-1.2.2/fmldk.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 06:32:59.018654 fmldk-1.2.2/sage/
+-rw-r--r--   0 runner    (1001) docker     (123)      222 2023-05-04 06:32:41.000000 fmldk-1.2.2/sage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46655 2023-05-04 06:32:41.000000 fmldk-1.2.2/sage/sage_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42404 2023-05-04 06:32:41.000000 fmldk-1.2.2/sage/sage_data_old.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42020 2023-05-04 06:32:41.000000 fmldk-1.2.2/sage/sage_global_scaled_data_old.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17695 2023-05-04 06:32:41.000000 fmldk-1.2.2/sage/sage_losses.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14320 2023-05-04 06:32:41.000000 fmldk-1.2.2/sage/sage_losses_old.py
+-rw-r--r--   0 runner    (1001) docker     (123)    86777 2023-05-04 06:32:41.000000 fmldk-1.2.2/sage/sage_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    83909 2023-05-04 06:32:41.000000 fmldk-1.2.2/sage/sage_model_old.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 06:32:59.018654 fmldk-1.2.2/sage_gpu/
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-05-04 06:32:41.000000 fmldk-1.2.2/sage_gpu/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36555 2023-05-04 06:32:41.000000 fmldk-1.2.2/sage_gpu/sage_data_gpu.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17683 2023-05-04 06:32:41.000000 fmldk-1.2.2/sage_gpu/sage_losses_gpu.py
+-rw-r--r--   0 runner    (1001) docker     (123)    87795 2023-05-04 06:32:41.000000 fmldk-1.2.2/sage_gpu/sage_model_gpu.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-04 06:32:59.034654 fmldk-1.2.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      795 2023-05-04 06:32:41.000000 fmldk-1.2.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 06:32:59.022654 fmldk-1.2.2/stctn/
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-05-04 06:32:41.000000 fmldk-1.2.2/stctn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    55190 2023-05-04 06:32:41.000000 fmldk-1.2.2/stctn/stctn_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13307 2023-05-04 06:32:41.000000 fmldk-1.2.2/stctn/stctn_losses.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12423 2023-05-04 06:32:41.000000 fmldk-1.2.2/stctn/stctn_losses_bkp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    53648 2023-05-04 06:32:41.000000 fmldk-1.2.2/stctn/stctn_models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 06:32:59.026654 fmldk-1.2.2/tfr/
+-rw-r--r--   0 runner    (1001) docker     (123)      352 2023-05-04 06:32:41.000000 fmldk-1.2.2/tfr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    55577 2023-05-04 06:32:41.000000 fmldk-1.2.2/tfr/tfr_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23667 2023-05-04 06:32:41.000000 fmldk-1.2.2/tfr/tfr_data_v0.1.11.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26192 2023-05-04 06:32:41.000000 fmldk-1.2.2/tfr/tfr_data_v0.1.12.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37924 2023-05-04 06:32:41.000000 fmldk-1.2.2/tfr/tfr_data_v0.1.14.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40021 2023-05-04 06:32:41.000000 fmldk-1.2.2/tfr/tfr_data_v0.1.15.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46425 2023-05-04 06:32:41.000000 fmldk-1.2.2/tfr/tfr_data_v0.1.16.py
+-rw-r--r--   0 runner    (1001) docker     (123)    54017 2023-05-04 06:32:41.000000 fmldk-1.2.2/tfr/tfr_data_v0.1.18.py
+-rw-r--r--   0 runner    (1001) docker     (123)    55773 2023-05-04 06:32:41.000000 fmldk-1.2.2/tfr/tfr_data_v0.1.21.py
+-rw-r--r--   0 runner    (1001) docker     (123)   107319 2023-05-04 06:32:41.000000 fmldk-1.2.2/tfr/tfr_local_block_sparse_attention.py
+-rw-r--r--   0 runner    (1001) docker     (123)    93067 2023-05-04 06:32:41.000000 fmldk-1.2.2/tfr/tfr_local_block_sparse_attention_v0.1.10.py
+-rw-r--r--   0 runner    (1001) docker     (123)    97067 2023-05-04 06:32:41.000000 fmldk-1.2.2/tfr/tfr_local_block_sparse_attention_v0.1.12.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13292 2023-05-04 06:32:41.000000 fmldk-1.2.2/tfr/tfr_losses.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12423 2023-05-04 06:32:41.000000 fmldk-1.2.2/tfr/tfr_losses_bkp.py
+-rw-r--r--   0 runner    (1001) docker     (123)   113988 2023-05-04 06:32:41.000000 fmldk-1.2.2/tfr/tfr_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)    96299 2023-05-04 06:32:41.000000 fmldk-1.2.2/tfr/tfr_models_v0.1.10.py
+-rw-r--r--   0 runner    (1001) docker     (123)   100101 2023-05-04 06:32:41.000000 fmldk-1.2.2/tfr/tfr_models_v0.1.11.py
+-rw-r--r--   0 runner    (1001) docker     (123)   109483 2023-05-04 06:32:41.000000 fmldk-1.2.2/tfr/tfr_models_v0.1.23.py
+-rw-r--r--   0 runner    (1001) docker     (123)   114250 2023-05-04 06:32:41.000000 fmldk-1.2.2/tfr/tfr_models_v0.1.31.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 06:32:59.030654 fmldk-1.2.2/tft/
+-rw-r--r--   0 runner    (1001) docker     (123)      282 2023-05-04 06:32:41.000000 fmldk-1.2.2/tft/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46653 2023-05-04 06:32:41.000000 fmldk-1.2.2/tft/tft_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42403 2023-05-04 06:32:41.000000 fmldk-1.2.2/tft/tft_data_old.py
+-rw-r--r--   0 runner    (1001) docker     (123)    55578 2023-05-04 06:32:41.000000 fmldk-1.2.2/tft/tft_data_v1.1.3.py
+-rw-r--r--   0 runner    (1001) docker     (123)    62667 2023-05-04 06:32:41.000000 fmldk-1.2.2/tft/tft_data_v1.1.7.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42019 2023-05-04 06:32:41.000000 fmldk-1.2.2/tft/tft_global_scaled_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17695 2023-05-04 06:32:41.000000 fmldk-1.2.2/tft/tft_losses.py
+-rw-r--r--   0 runner    (1001) docker     (123)    84122 2023-05-04 06:32:41.000000 fmldk-1.2.2/tft/tft_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    64043 2023-05-04 06:32:41.000000 fmldk-1.2.2/tft/tft_model_v0.1.26.py
+-rw-r--r--   0 runner    (1001) docker     (123)    65090 2023-05-04 06:32:41.000000 fmldk-1.2.2/tft/tft_model_v0.1.31.py
+-rw-r--r--   0 runner    (1001) docker     (123)    73433 2023-05-04 06:32:41.000000 fmldk-1.2.2/tft/tft_model_v1.1.3.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 06:32:59.030654 fmldk-1.2.2/tft_gpu/
+-rw-r--r--   0 runner    (1001) docker     (123)      251 2023-05-04 06:32:41.000000 fmldk-1.2.2/tft_gpu/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36571 2023-05-04 06:32:41.000000 fmldk-1.2.2/tft_gpu/tft_data_gpu.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17695 2023-05-04 06:32:41.000000 fmldk-1.2.2/tft_gpu/tft_losses_gpu.py
+-rw-r--r--   0 runner    (1001) docker     (123)    78604 2023-05-04 06:32:41.000000 fmldk-1.2.2/tft_gpu/tft_model_gpu.py
```

### Comparing `fmldk-1.2.1/PKG-INFO` & `fmldk-1.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fmldk
-Version: 1.2.1
+Version: 1.2.2
 Summary: Forecast ML library
 Author: Rahul Sinha
 Author-email: rahul.sinha@unilever.com
 Description-Content-Type: text/markdown
 
 ### A library to easily build & train Transformer models for forecasting.
```

### Comparing `fmldk-1.2.1/README.md` & `fmldk-1.2.2/README.md`

 * *Files identical despite different names*

### Comparing `fmldk-1.2.1/ctfr/ctfr_data.py` & `fmldk-1.2.2/ctfr/ctfr_data.py`

 * *Files identical despite different names*

### Comparing `fmldk-1.2.1/ctfr/ctfr_losses.py` & `fmldk-1.2.2/ctfr/ctfr_losses.py`

 * *Files identical despite different names*

### Comparing `fmldk-1.2.1/ctfr/ctfr_losses_bkp.py` & `fmldk-1.2.2/ctfr/ctfr_losses_bkp.py`

 * *Files identical despite different names*

### Comparing `fmldk-1.2.1/ctfr/ctfr_models.py` & `fmldk-1.2.2/ctfr/ctfr_models.py`

 * *Files identical despite different names*

### Comparing `fmldk-1.2.1/ctfr/ctfr_models_v0.1.29.py` & `fmldk-1.2.2/ctfr/ctfr_models_v0.1.29.py`

 * *Files identical despite different names*

### Comparing `fmldk-1.2.1/ctfr/ctfr_models_v0.1.31.py` & `fmldk-1.2.2/ctfr/ctfr_models_v0.1.31.py`

 * *Files identical despite different names*

### Comparing `fmldk-1.2.1/ctfrv2/ctfrv2_data.py` & `fmldk-1.2.2/ctfrv2/ctfrv2_data.py`

 * *Files identical despite different names*

### Comparing `fmldk-1.2.1/ctfrv2/ctfrv2_global_scaled_data.py` & `fmldk-1.2.2/ctfrv2/ctfrv2_global_scaled_data.py`

 * *Files identical despite different names*

### Comparing `fmldk-1.2.1/ctfrv2/ctfrv2_losses.py` & `fmldk-1.2.2/ctfrv2/ctfrv2_losses.py`

 * *Files identical despite different names*

### Comparing `fmldk-1.2.1/ctfrv2/ctfrv2_models.py` & `fmldk-1.2.2/ctfrv2/ctfrv2_models.py`

 * *Files identical despite different names*

### Comparing `fmldk-1.2.1/ctfrv2_gpu/ctfrv2_data_gpu.py` & `fmldk-1.2.2/ctfrv2_gpu/ctfrv2_data_gpu.py`

 * *Files 0% similar despite different names*

```diff
@@ -244,15 +244,15 @@
             test_len = int(gdf[(gdf[self.time_index_col]>self.train_till) & (gdf[self.time_index_col]<=self.test_till)].groupby(self.id_col)[self.target_col].count().max())
             test_len = test_len + (self.window_len - self.fh) 
             gdf = gdf[gdf[self.time_index_col]<=self.test_till].groupby(self.id_col).apply(lambda x: x[-test_len:]).reset_index(drop=True)
             
         gdf = gdf.reset_index(drop=True)
         delta = len(gdf) - self.window_len
 
-        num_samples = max(1,len(gdf) - self.window_len)
+        num_samples = max(1, delta+1)
 
         if mode == 'train':
           max_samples = num_samples if self.max_key_train_samples == -1 else self.max_key_train_samples
         elif mode == 'test':
           max_samples = num_samples if self.max_key_test_samples == -1 else self.max_key_test_samples
         
         arr_list = []
@@ -278,16 +278,19 @@
             pad_list.append([pad_len])
             scale_list.append(scale)
             known_scale_list.append(known_scale)
             unknown_scale_list.append(unknown_scale)
         else:
             pad_len = 0
             sample_interval = max(1, int(num_samples/max_samples))
-            for i in range(min(max_samples, num_samples)):
-              arr = gdf.loc[i*sample_interval:i*sample_interval + self.window_len - 1, self.col_list].reset_index(drop=True).values
+            # take only the most recent max_samples
+            start_pos = max(0, int(len(gdf) - (sample_interval * (max_samples - 1) + self.window_len)))
+
+            for i in range(start_pos, num_samples, sample_interval):
+              arr = gdf.loc[i:i + self.window_len - 1, self.col_list].reset_index(drop=True).values
               arr_list.append(arr)
               pad_list.append([pad_len])
               scale_list.append(scale)
               known_scale_list.append(known_scale)
               unknown_scale_list.append(unknown_scale)
         
         arr = np.stack(arr_list, axis=0)
```

### Comparing `fmldk-1.2.1/ctfrv2_gpu/ctfrv2_losses_gpu.py` & `fmldk-1.2.2/ctfrv2_gpu/ctfrv2_losses_gpu.py`

 * *Files identical despite different names*

### Comparing `fmldk-1.2.1/ctfrv2_gpu/ctfrv2_model_gpu.py` & `fmldk-1.2.2/ctfrv2_gpu/ctfrv2_model_gpu.py`

 * *Files identical despite different names*

### Comparing `fmldk-1.2.1/eda/eda_lib.py` & `fmldk-1.2.2/eda/eda_lib.py`

 * *Files identical despite different names*

### Comparing `fmldk-1.2.1/eda/eda_lib_v0.1.18.py` & `fmldk-1.2.2/eda/eda_lib_v0.1.18.py`

 * *Files identical despite different names*

### Comparing `fmldk-1.2.1/eda/eda_lib_v0.1.19.py` & `fmldk-1.2.2/eda/eda_lib_v0.1.19.py`

 * *Files identical despite different names*

### Comparing `fmldk-1.2.1/eda/eda_lib_v0.1.37.py` & `fmldk-1.2.2/eda/eda_lib_v0.1.37.py`

 * *Files identical despite different names*

### Comparing `fmldk-1.2.1/fmldk.egg-info/PKG-INFO` & `fmldk-1.2.2/fmldk.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fmldk
-Version: 1.2.1
+Version: 1.2.2
 Summary: Forecast ML library
 Author: Rahul Sinha
 Author-email: rahul.sinha@unilever.com
 Description-Content-Type: text/markdown
 
 ### A library to easily build & train Transformer models for forecasting.
```

### Comparing `fmldk-1.2.1/fmldk.egg-info/SOURCES.txt` & `fmldk-1.2.2/fmldk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fmldk-1.2.1/sage/sage_data.py` & `fmldk-1.2.2/sage/sage_data.py`

 * *Files identical despite different names*

### Comparing `fmldk-1.2.1/sage/sage_data_old.py` & `fmldk-1.2.2/sage/sage_data_old.py`

 * *Files identical despite different names*

### Comparing `fmldk-1.2.1/sage/sage_global_scaled_data_old.py` & `fmldk-1.2.2/sage/sage_global_scaled_data_old.py`

 * *Files identical despite different names*

### Comparing `fmldk-1.2.1/sage/sage_losses.py` & `fmldk-1.2.2/sage/sage_losses.py`

 * *Files identical despite different names*

### Comparing `fmldk-1.2.1/sage/sage_losses_old.py` & `fmldk-1.2.2/sage/sage_losses_old.py`

 * *Files identical despite different names*

### Comparing `fmldk-1.2.1/sage/sage_model.py` & `fmldk-1.2.2/sage/sage_model.py`

 * *Files identical despite different names*

### Comparing `fmldk-1.2.1/sage/sage_model_old.py` & `fmldk-1.2.2/sage/sage_model_old.py`

 * *Files identical despite different names*

### Comparing `fmldk-1.2.1/sage_gpu/sage_data_gpu.py` & `fmldk-1.2.2/sage_gpu/sage_data_gpu.py`

 * *Files 0% similar despite different names*

```diff
@@ -241,15 +241,15 @@
             test_len = int(gdf[(gdf[self.time_index_col]>self.train_till) & (gdf[self.time_index_col]<=self.test_till)].groupby(self.id_col)[self.target_col].count().max())
             test_len = test_len + (self.window_len - self.fh) 
             gdf = gdf[gdf[self.time_index_col]<=self.test_till].groupby(self.id_col).apply(lambda x: x[-test_len:]).reset_index(drop=True)
             
         gdf = gdf.reset_index(drop=True)
         delta = len(gdf) - self.window_len
 
-        num_samples = max(1,len(gdf) - self.window_len)
+        num_samples = max(1, delta+1)
 
         if mode == 'train':
           max_samples = num_samples if self.max_key_train_samples == -1 else self.max_key_train_samples
         elif mode == 'test':
           max_samples = num_samples if self.max_key_test_samples == -1 else self.max_key_test_samples
         
         arr_list = []
@@ -275,16 +275,19 @@
             pad_list.append([pad_len])
             scale_list.append(scale)
             known_scale_list.append(known_scale)
             unknown_scale_list.append(unknown_scale)
         else:
             pad_len = 0
             sample_interval = max(1, int(num_samples/max_samples))
-            for i in range(min(max_samples, num_samples)):
-              arr = gdf.loc[i*sample_interval:i*sample_interval + self.window_len - 1, self.col_list].reset_index(drop=True).values
+            # take only the most recent max_samples
+            start_pos = max(0, int(len(gdf) - (sample_interval * (max_samples - 1) + self.window_len)))
+
+            for i in range(start_pos, num_samples, sample_interval):
+              arr = gdf.loc[i:i + self.window_len - 1, self.col_list].reset_index(drop=True).values
               arr_list.append(arr)
               pad_list.append([pad_len])
               scale_list.append(scale)
               known_scale_list.append(known_scale)
               unknown_scale_list.append(unknown_scale)
         
         arr = np.stack(arr_list, axis=0)
```

### Comparing `fmldk-1.2.1/sage_gpu/sage_losses_gpu.py` & `fmldk-1.2.2/sage_gpu/sage_losses_gpu.py`

 * *Files identical despite different names*

### Comparing `fmldk-1.2.1/sage_gpu/sage_model_gpu.py` & `fmldk-1.2.2/sage_gpu/sage_model_gpu.py`

 * *Files 0% similar despite different names*

```diff
@@ -891,15 +891,15 @@
         self.dropout_rate = dropout_rate
         
         if (len(self.col_index_dict.get('static_num_indices')[0])==0) and (len(self.col_index_dict.get('static_cat_indices')[0])==0):
             self.static_variables = False
         else:
             self.static_variables = True
         
-        self.model = ConvVarTransformer(static_variables = self.static_variables,
+        self.model = SageTransformer(static_variables = self.static_variables,
                                     num_layers = num_layers,
                                     d_model = d_model,
                                     num_heads = num_heads, 
                                     kernel_sizes = kernel_sizes,
                                     dff = d_model,
                                     hist_len = self.hist_len, 
                                     f_len = self.f_len,
```

### Comparing `fmldk-1.2.1/setup.py` & `fmldk-1.2.2/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 # The directory containing this file
 this_directory = Path(__file__).parent
 long_description  = (this_directory / "README.md").read_text()
 
 # This call to setup() does all the work
 setup(
     name="fmldk",
-    version="1.2.1",
+    version="1.2.2",
     description="Forecast ML library",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="Rahul Sinha",
     author_email="rahul.sinha@unilever.com",
     packages=["sage","sage_gpu","tfr","tft","tft_gpu","stctn","ctfr","ctfrv2","ctfrv2_gpu","eda"],
     include_package_data=True,
```

### Comparing `fmldk-1.2.1/stctn/stctn_data.py` & `fmldk-1.2.2/stctn/stctn_data.py`

 * *Files identical despite different names*

### Comparing `fmldk-1.2.1/stctn/stctn_losses.py` & `fmldk-1.2.2/stctn/stctn_losses.py`

 * *Files identical despite different names*

### Comparing `fmldk-1.2.1/stctn/stctn_losses_bkp.py` & `fmldk-1.2.2/stctn/stctn_losses_bkp.py`

 * *Files identical despite different names*

### Comparing `fmldk-1.2.1/stctn/stctn_models.py` & `fmldk-1.2.2/stctn/stctn_models.py`

 * *Files identical despite different names*

### Comparing `fmldk-1.2.1/tfr/tfr_data.py` & `fmldk-1.2.2/tfr/tfr_data.py`

 * *Files identical despite different names*

### Comparing `fmldk-1.2.1/tfr/tfr_data_v0.1.11.py` & `fmldk-1.2.2/tfr/tfr_data_v0.1.11.py`

 * *Files identical despite different names*

### Comparing `fmldk-1.2.1/tfr/tfr_data_v0.1.12.py` & `fmldk-1.2.2/tfr/tfr_data_v0.1.12.py`

 * *Files identical despite different names*

### Comparing `fmldk-1.2.1/tfr/tfr_data_v0.1.14.py` & `fmldk-1.2.2/tfr/tfr_data_v0.1.14.py`

 * *Files identical despite different names*

### Comparing `fmldk-1.2.1/tfr/tfr_data_v0.1.15.py` & `fmldk-1.2.2/tfr/tfr_data_v0.1.15.py`

 * *Files identical despite different names*

### Comparing `fmldk-1.2.1/tfr/tfr_data_v0.1.16.py` & `fmldk-1.2.2/tfr/tfr_data_v0.1.16.py`

 * *Files identical despite different names*

### Comparing `fmldk-1.2.1/tfr/tfr_data_v0.1.18.py` & `fmldk-1.2.2/tfr/tfr_data_v0.1.18.py`

 * *Files identical despite different names*

### Comparing `fmldk-1.2.1/tfr/tfr_data_v0.1.21.py` & `fmldk-1.2.2/tfr/tfr_data_v0.1.21.py`

 * *Files identical despite different names*

### Comparing `fmldk-1.2.1/tfr/tfr_local_block_sparse_attention.py` & `fmldk-1.2.2/tfr/tfr_local_block_sparse_attention.py`

 * *Files identical despite different names*

### Comparing `fmldk-1.2.1/tfr/tfr_local_block_sparse_attention_v0.1.10.py` & `fmldk-1.2.2/tfr/tfr_local_block_sparse_attention_v0.1.10.py`

 * *Files identical despite different names*

### Comparing `fmldk-1.2.1/tfr/tfr_local_block_sparse_attention_v0.1.12.py` & `fmldk-1.2.2/tfr/tfr_local_block_sparse_attention_v0.1.12.py`

 * *Files identical despite different names*

### Comparing `fmldk-1.2.1/tfr/tfr_losses.py` & `fmldk-1.2.2/tfr/tfr_losses.py`

 * *Files identical despite different names*

### Comparing `fmldk-1.2.1/tfr/tfr_losses_bkp.py` & `fmldk-1.2.2/tfr/tfr_losses_bkp.py`

 * *Files identical despite different names*

### Comparing `fmldk-1.2.1/tfr/tfr_models.py` & `fmldk-1.2.2/tfr/tfr_models.py`

 * *Files identical despite different names*

### Comparing `fmldk-1.2.1/tfr/tfr_models_v0.1.10.py` & `fmldk-1.2.2/tfr/tfr_models_v0.1.10.py`

 * *Files identical despite different names*

### Comparing `fmldk-1.2.1/tfr/tfr_models_v0.1.11.py` & `fmldk-1.2.2/tfr/tfr_models_v0.1.11.py`

 * *Files identical despite different names*

### Comparing `fmldk-1.2.1/tfr/tfr_models_v0.1.23.py` & `fmldk-1.2.2/tfr/tfr_models_v0.1.23.py`

 * *Files identical despite different names*

### Comparing `fmldk-1.2.1/tfr/tfr_models_v0.1.31.py` & `fmldk-1.2.2/tfr/tfr_models_v0.1.31.py`

 * *Files identical despite different names*

### Comparing `fmldk-1.2.1/tft/tft_data.py` & `fmldk-1.2.2/tft/tft_data.py`

 * *Files identical despite different names*

### Comparing `fmldk-1.2.1/tft/tft_data_old.py` & `fmldk-1.2.2/tft/tft_data_old.py`

 * *Files identical despite different names*

### Comparing `fmldk-1.2.1/tft/tft_data_v1.1.3.py` & `fmldk-1.2.2/tft/tft_data_v1.1.3.py`

 * *Files identical despite different names*

### Comparing `fmldk-1.2.1/tft/tft_data_v1.1.7.py` & `fmldk-1.2.2/tft/tft_data_v1.1.7.py`

 * *Files identical despite different names*

### Comparing `fmldk-1.2.1/tft/tft_global_scaled_data.py` & `fmldk-1.2.2/tft/tft_global_scaled_data.py`

 * *Files identical despite different names*

### Comparing `fmldk-1.2.1/tft/tft_losses.py` & `fmldk-1.2.2/tft/tft_losses.py`

 * *Files identical despite different names*

### Comparing `fmldk-1.2.1/tft/tft_model.py` & `fmldk-1.2.2/tft/tft_model.py`

 * *Files identical despite different names*

### Comparing `fmldk-1.2.1/tft/tft_model_v0.1.26.py` & `fmldk-1.2.2/tft/tft_model_v0.1.26.py`

 * *Files identical despite different names*

### Comparing `fmldk-1.2.1/tft/tft_model_v0.1.31.py` & `fmldk-1.2.2/tft/tft_model_v0.1.31.py`

 * *Files identical despite different names*

### Comparing `fmldk-1.2.1/tft/tft_model_v1.1.3.py` & `fmldk-1.2.2/tft/tft_model_v1.1.3.py`

 * *Files identical despite different names*

### Comparing `fmldk-1.2.1/tft_gpu/tft_data_gpu.py` & `fmldk-1.2.2/tft_gpu/tft_data_gpu.py`

 * *Files 0% similar despite different names*

```diff
@@ -244,15 +244,15 @@
             test_len = int(gdf[(gdf[self.time_index_col]>self.train_till) & (gdf[self.time_index_col]<=self.test_till)].groupby(self.id_col)[self.target_col].count().max())
             test_len = test_len + (self.window_len - self.fh) 
             gdf = gdf[gdf[self.time_index_col]<=self.test_till].groupby(self.id_col).apply(lambda x: x[-test_len:]).reset_index(drop=True)
             
         gdf = gdf.reset_index(drop=True)
         delta = len(gdf) - self.window_len
 
-        num_samples = max(1,len(gdf) - self.window_len)
+        num_samples = max(1, delta+1)
 
         if mode == 'train':
           max_samples = num_samples if self.max_key_train_samples == -1 else self.max_key_train_samples
         elif mode == 'test':
           max_samples = num_samples if self.max_key_test_samples == -1 else self.max_key_test_samples
         
         arr_list = []
@@ -278,16 +278,19 @@
             pad_list.append([pad_len])
             scale_list.append(scale)
             known_scale_list.append(known_scale)
             unknown_scale_list.append(unknown_scale)
         else:
             pad_len = 0
             sample_interval = max(1, int(num_samples/max_samples))
-            for i in range(min(max_samples, num_samples)):
-              arr = gdf.loc[i*sample_interval:i*sample_interval + self.window_len - 1, self.col_list].reset_index(drop=True).values
+            # take only the most recent max_samples
+            start_pos = max(0, int(len(gdf) - (sample_interval * (max_samples - 1) + self.window_len)))
+
+            for i in range(start_pos, num_samples, sample_interval):
+              arr = gdf.loc[i:i + self.window_len - 1, self.col_list].reset_index(drop=True).values
               arr_list.append(arr)
               pad_list.append([pad_len])
               scale_list.append(scale)
               known_scale_list.append(known_scale)
               unknown_scale_list.append(unknown_scale)
         
         arr = np.stack(arr_list, axis=0)
```

### Comparing `fmldk-1.2.1/tft_gpu/tft_losses_gpu.py` & `fmldk-1.2.2/tft_gpu/tft_losses_gpu.py`

 * *Files identical despite different names*

### Comparing `fmldk-1.2.1/tft_gpu/tft_model_gpu.py` & `fmldk-1.2.2/tft_gpu/tft_model_gpu.py`

 * *Files identical despite different names*

