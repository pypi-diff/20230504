# Comparing `tmp/zoobot-1.0.2.tar.gz` & `tmp/zoobot-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zoobot-1.0.2.tar", last modified: Wed Mar 29 09:07:06 2023, max compression
+gzip compressed data, was "zoobot-1.0.3.tar", last modified: Thu May  4 12:35:23 2023, max compression
```

## Comparing `zoobot-1.0.2.tar` & `zoobot-1.0.3.tar`

### file list

```diff
@@ -1,72 +1,72 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 09:07:06.750750 zoobot-1.0.2/
--rwxr-xr-x   0 runner    (1001) docker     (123)    35149 2023-03-29 09:06:57.000000 zoobot-1.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    12099 2023-03-29 09:07:06.750750 zoobot-1.0.2/PKG-INFO
--rwxr-xr-x   0 runner    (1001) docker     (123)    11373 2023-03-29 09:06:57.000000 zoobot-1.0.2/README.md
--rwxr-xr-x   0 runner    (1001) docker     (123)      103 2023-03-29 09:06:57.000000 zoobot-1.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-29 09:07:06.750750 zoobot-1.0.2/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     4072 2023-03-29 09:06:57.000000 zoobot-1.0.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 09:07:06.742751 zoobot-1.0.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2635 2023-03-29 09:06:57.000000 zoobot-1.0.2/tests/test_loss_equivalence.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 09:07:06.742751 zoobot-1.0.2/zoobot/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-29 09:06:57.000000 zoobot-1.0.2/zoobot/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 09:07:06.746750 zoobot-1.0.2/zoobot/pytorch/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-29 09:06:57.000000 zoobot-1.0.2/zoobot/pytorch/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 09:07:06.746750 zoobot-1.0.2/zoobot/pytorch/estimators/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-29 09:06:57.000000 zoobot-1.0.2/zoobot/pytorch/estimators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-03-29 09:06:57.000000 zoobot-1.0.2/zoobot/pytorch/estimators/cuda_check.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1604 2023-03-29 09:06:57.000000 zoobot-1.0.2/zoobot/pytorch/estimators/custom_layers.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    16013 2023-03-29 09:06:57.000000 zoobot-1.0.2/zoobot/pytorch/estimators/define_model.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3188 2023-03-29 09:06:57.000000 zoobot-1.0.2/zoobot/pytorch/estimators/efficientnet_custom.py
--rw-r--r--   0 runner    (1001) docker     (123)     1466 2023-03-29 09:06:57.000000 zoobot-1.0.2/zoobot/pytorch/manchester.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 09:07:06.746750 zoobot-1.0.2/zoobot/pytorch/predictions/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-29 09:06:57.000000 zoobot-1.0.2/zoobot/pytorch/predictions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3895 2023-03-29 09:06:57.000000 zoobot-1.0.2/zoobot/pytorch/predictions/predict_on_catalog.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 09:07:06.746750 zoobot-1.0.2/zoobot/pytorch/training/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-29 09:06:57.000000 zoobot-1.0.2/zoobot/pytorch/training/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20318 2023-03-29 09:06:57.000000 zoobot-1.0.2/zoobot/pytorch/training/finetune.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5860 2023-03-29 09:06:57.000000 zoobot-1.0.2/zoobot/pytorch/training/losses.py
--rw-r--r--   0 runner    (1001) docker     (123)      603 2023-03-29 09:06:57.000000 zoobot-1.0.2/zoobot/pytorch/training/representations.py
--rw-r--r--   0 runner    (1001) docker     (123)     6597 2023-03-29 09:06:57.000000 zoobot-1.0.2/zoobot/pytorch/training/tensorboard_writers.py
--rw-r--r--   0 runner    (1001) docker     (123)    16300 2023-03-29 09:06:57.000000 zoobot-1.0.2/zoobot/pytorch/training/train_with_pytorch_lightning.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 09:07:06.746750 zoobot-1.0.2/zoobot/shared/
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 09:06:57.000000 zoobot-1.0.2/zoobot/shared/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2006 2023-03-29 09:06:57.000000 zoobot-1.0.2/zoobot/shared/benchmark_datasets.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4437 2023-03-29 09:06:57.000000 zoobot-1.0.2/zoobot/shared/compress_representations.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2071 2023-03-29 09:06:57.000000 zoobot-1.0.2/zoobot/shared/label_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)    10528 2023-03-29 09:06:57.000000 zoobot-1.0.2/zoobot/shared/load_predictions.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2844 2023-03-29 09:06:57.000000 zoobot-1.0.2/zoobot/shared/save_predictions.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    11898 2023-03-29 09:06:57.000000 zoobot-1.0.2/zoobot/shared/schemas.py
--rw-r--r--   0 runner    (1001) docker     (123)    12964 2023-03-29 09:06:57.000000 zoobot-1.0.2/zoobot/shared/stats.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 09:07:06.746750 zoobot-1.0.2/zoobot/tensorflow/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-29 09:06:57.000000 zoobot-1.0.2/zoobot/tensorflow/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 09:07:06.750750 zoobot-1.0.2/zoobot/tensorflow/estimators/
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 09:06:57.000000 zoobot-1.0.2/zoobot/tensorflow/estimators/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2508 2023-03-29 09:06:57.000000 zoobot-1.0.2/zoobot/tensorflow/estimators/alexnet_baseline.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1795 2023-03-29 09:06:57.000000 zoobot-1.0.2/zoobot/tensorflow/estimators/custom_callbacks.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1370 2023-03-29 09:06:57.000000 zoobot-1.0.2/zoobot/tensorflow/estimators/custom_layers.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     7227 2023-03-29 09:06:57.000000 zoobot-1.0.2/zoobot/tensorflow/estimators/define_model.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2300 2023-03-29 09:06:57.000000 zoobot-1.0.2/zoobot/tensorflow/estimators/efficientnet_custom.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    84167 2023-03-29 09:06:57.000000 zoobot-1.0.2/zoobot/tensorflow/estimators/efficientnet_standard.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1134 2023-03-29 09:06:57.000000 zoobot-1.0.2/zoobot/tensorflow/estimators/small_cnn_baseline.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 09:07:06.750750 zoobot-1.0.2/zoobot/tensorflow/predictions/
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 09:06:57.000000 zoobot-1.0.2/zoobot/tensorflow/predictions/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3417 2023-03-29 09:06:57.000000 zoobot-1.0.2/zoobot/tensorflow/predictions/predict_on_dataset.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5239 2023-03-29 09:06:57.000000 zoobot-1.0.2/zoobot/tensorflow/predictions/visualize_dirichlet_predictions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 09:07:06.750750 zoobot-1.0.2/zoobot/tensorflow/stats/
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 09:06:57.000000 zoobot-1.0.2/zoobot/tensorflow/stats/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5223 2023-03-29 09:06:57.000000 zoobot-1.0.2/zoobot/tensorflow/stats/coverage.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    14433 2023-03-29 09:06:57.000000 zoobot-1.0.2/zoobot/tensorflow/stats/dirichlet_stats.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3526 2023-03-29 09:06:57.000000 zoobot-1.0.2/zoobot/tensorflow/stats/mixture_stats.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 09:07:06.750750 zoobot-1.0.2/zoobot/tensorflow/training/
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 09:06:57.000000 zoobot-1.0.2/zoobot/tensorflow/training/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1947 2023-03-29 09:06:57.000000 zoobot-1.0.2/zoobot/tensorflow/training/custom_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     7392 2023-03-29 09:06:57.000000 zoobot-1.0.2/zoobot/tensorflow/training/finetune.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6772 2023-03-29 09:06:57.000000 zoobot-1.0.2/zoobot/tensorflow/training/losses.py
--rw-r--r--   0 runner    (1001) docker     (123)    11959 2023-03-29 09:06:57.000000 zoobot-1.0.2/zoobot/tensorflow/training/train_with_keras.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6505 2023-03-29 09:06:57.000000 zoobot-1.0.2/zoobot/tensorflow/training/training_config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 09:07:06.746750 zoobot-1.0.2/zoobot.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    12099 2023-03-29 09:07:06.000000 zoobot-1.0.2/zoobot.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2085 2023-03-29 09:07:06.000000 zoobot-1.0.2/zoobot.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-29 09:07:06.000000 zoobot-1.0.2/zoobot.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      972 2023-03-29 09:07:06.000000 zoobot-1.0.2/zoobot.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-03-29 09:07:06.000000 zoobot-1.0.2/zoobot.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 12:35:23.754416 zoobot-1.0.3/
+-rwxr-xr-x   0 runner    (1001) docker     (123)    35149 2023-05-04 12:35:10.000000 zoobot-1.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    12426 2023-05-04 12:35:23.754416 zoobot-1.0.3/PKG-INFO
+-rwxr-xr-x   0 runner    (1001) docker     (123)    11701 2023-05-04 12:35:10.000000 zoobot-1.0.3/README.md
+-rwxr-xr-x   0 runner    (1001) docker     (123)      103 2023-05-04 12:35:10.000000 zoobot-1.0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-04 12:35:23.754416 zoobot-1.0.3/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4072 2023-05-04 12:35:10.000000 zoobot-1.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 12:35:23.738416 zoobot-1.0.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2635 2023-05-04 12:35:10.000000 zoobot-1.0.3/tests/test_loss_equivalence.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 12:35:23.738416 zoobot-1.0.3/zoobot/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 12:35:10.000000 zoobot-1.0.3/zoobot/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 12:35:23.742416 zoobot-1.0.3/zoobot/pytorch/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 12:35:10.000000 zoobot-1.0.3/zoobot/pytorch/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 12:35:23.742416 zoobot-1.0.3/zoobot/pytorch/estimators/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 12:35:10.000000 zoobot-1.0.3/zoobot/pytorch/estimators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-05-04 12:35:10.000000 zoobot-1.0.3/zoobot/pytorch/estimators/cuda_check.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1604 2023-05-04 12:35:10.000000 zoobot-1.0.3/zoobot/pytorch/estimators/custom_layers.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    16013 2023-05-04 12:35:10.000000 zoobot-1.0.3/zoobot/pytorch/estimators/define_model.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3188 2023-05-04 12:35:10.000000 zoobot-1.0.3/zoobot/pytorch/estimators/efficientnet_custom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1466 2023-05-04 12:35:10.000000 zoobot-1.0.3/zoobot/pytorch/manchester.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 12:35:23.742416 zoobot-1.0.3/zoobot/pytorch/predictions/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 12:35:10.000000 zoobot-1.0.3/zoobot/pytorch/predictions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3895 2023-05-04 12:35:10.000000 zoobot-1.0.3/zoobot/pytorch/predictions/predict_on_catalog.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 12:35:23.746416 zoobot-1.0.3/zoobot/pytorch/training/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 12:35:10.000000 zoobot-1.0.3/zoobot/pytorch/training/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20318 2023-05-04 12:35:10.000000 zoobot-1.0.3/zoobot/pytorch/training/finetune.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5860 2023-05-04 12:35:10.000000 zoobot-1.0.3/zoobot/pytorch/training/losses.py
+-rw-r--r--   0 runner    (1001) docker     (123)      603 2023-05-04 12:35:10.000000 zoobot-1.0.3/zoobot/pytorch/training/representations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6597 2023-05-04 12:35:10.000000 zoobot-1.0.3/zoobot/pytorch/training/tensorboard_writers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16300 2023-05-04 12:35:10.000000 zoobot-1.0.3/zoobot/pytorch/training/train_with_pytorch_lightning.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 12:35:23.746416 zoobot-1.0.3/zoobot/shared/
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 12:35:10.000000 zoobot-1.0.3/zoobot/shared/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2006 2023-05-04 12:35:10.000000 zoobot-1.0.3/zoobot/shared/benchmark_datasets.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4437 2023-05-04 12:35:10.000000 zoobot-1.0.3/zoobot/shared/compress_representations.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2071 2023-05-04 12:35:10.000000 zoobot-1.0.3/zoobot/shared/label_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10528 2023-05-04 12:35:10.000000 zoobot-1.0.3/zoobot/shared/load_predictions.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2844 2023-05-04 12:35:10.000000 zoobot-1.0.3/zoobot/shared/save_predictions.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    11898 2023-05-04 12:35:10.000000 zoobot-1.0.3/zoobot/shared/schemas.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12964 2023-05-04 12:35:10.000000 zoobot-1.0.3/zoobot/shared/stats.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 12:35:23.750416 zoobot-1.0.3/zoobot/tensorflow/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 12:35:10.000000 zoobot-1.0.3/zoobot/tensorflow/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 12:35:23.750416 zoobot-1.0.3/zoobot/tensorflow/estimators/
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 12:35:10.000000 zoobot-1.0.3/zoobot/tensorflow/estimators/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2508 2023-05-04 12:35:10.000000 zoobot-1.0.3/zoobot/tensorflow/estimators/alexnet_baseline.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1795 2023-05-04 12:35:10.000000 zoobot-1.0.3/zoobot/tensorflow/estimators/custom_callbacks.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1370 2023-05-04 12:35:10.000000 zoobot-1.0.3/zoobot/tensorflow/estimators/custom_layers.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7227 2023-05-04 12:35:10.000000 zoobot-1.0.3/zoobot/tensorflow/estimators/define_model.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2300 2023-05-04 12:35:10.000000 zoobot-1.0.3/zoobot/tensorflow/estimators/efficientnet_custom.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    84167 2023-05-04 12:35:10.000000 zoobot-1.0.3/zoobot/tensorflow/estimators/efficientnet_standard.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1134 2023-05-04 12:35:10.000000 zoobot-1.0.3/zoobot/tensorflow/estimators/small_cnn_baseline.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 12:35:23.750416 zoobot-1.0.3/zoobot/tensorflow/predictions/
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 12:35:10.000000 zoobot-1.0.3/zoobot/tensorflow/predictions/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3417 2023-05-04 12:35:10.000000 zoobot-1.0.3/zoobot/tensorflow/predictions/predict_on_dataset.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5239 2023-05-04 12:35:10.000000 zoobot-1.0.3/zoobot/tensorflow/predictions/visualize_dirichlet_predictions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 12:35:23.754416 zoobot-1.0.3/zoobot/tensorflow/stats/
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 12:35:10.000000 zoobot-1.0.3/zoobot/tensorflow/stats/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5223 2023-05-04 12:35:10.000000 zoobot-1.0.3/zoobot/tensorflow/stats/coverage.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    14433 2023-05-04 12:35:10.000000 zoobot-1.0.3/zoobot/tensorflow/stats/dirichlet_stats.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3526 2023-05-04 12:35:10.000000 zoobot-1.0.3/zoobot/tensorflow/stats/mixture_stats.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 12:35:23.754416 zoobot-1.0.3/zoobot/tensorflow/training/
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 12:35:10.000000 zoobot-1.0.3/zoobot/tensorflow/training/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1947 2023-05-04 12:35:10.000000 zoobot-1.0.3/zoobot/tensorflow/training/custom_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7392 2023-05-04 12:35:10.000000 zoobot-1.0.3/zoobot/tensorflow/training/finetune.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6772 2023-05-04 12:35:10.000000 zoobot-1.0.3/zoobot/tensorflow/training/losses.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11959 2023-05-04 12:35:10.000000 zoobot-1.0.3/zoobot/tensorflow/training/train_with_keras.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6505 2023-05-04 12:35:10.000000 zoobot-1.0.3/zoobot/tensorflow/training/training_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 12:35:23.738416 zoobot-1.0.3/zoobot.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    12426 2023-05-04 12:35:23.000000 zoobot-1.0.3/zoobot.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2085 2023-05-04 12:35:23.000000 zoobot-1.0.3/zoobot.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 12:35:23.000000 zoobot-1.0.3/zoobot.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      972 2023-05-04 12:35:23.000000 zoobot-1.0.3/zoobot.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-04 12:35:23.000000 zoobot-1.0.3/zoobot.egg-info/top_level.txt
```

### Comparing `zoobot-1.0.2/LICENSE` & `zoobot-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `zoobot-1.0.2/PKG-INFO` & `zoobot-1.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zoobot
-Version: 1.0.2
+Version: 1.0.3
 Summary: Galaxy morphology classifiers
 Home-page: https://github.com/mwalmsley/zoobot
 Author: Mike Walmsley
 Author-email: walmsleymk1@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License (GPL)
 Classifier: Operating System :: OS Independent
@@ -70,14 +70,16 @@
 
 To use a GPU, you must *already* have CUDA installed and matching the versions above.
 I share my install steps [here](#install_cuda). GPUs are optional - Zoobot will run retrain fine on CPU, just slower.
 
 ## Quickstart
 <a name="quickstart"></a>
 
+The [Colab notebook](https://colab.research.google.com/drive/17bb_KbA2J6yrIm4p4Ue_lEBHMNC1I9Jd?usp=sharing) is the quickest way to get started. Alternatively, the minimal example below illustrates how Zoobot works.
+
 Let's say you want to find ringed galaxies and you have a small labelled dataset of 500 ringed or not-ringed galaxies. You can retrain Zoobot to find rings like so:
 
 ```python
 
     import pandas as pd
     from galaxy_datasets.pytorch.galaxy_datamodule import GalaxyDataModule
     from zoobot.pytorch.training import finetune
@@ -116,15 +118,15 @@
 ```
 
 Zoobot includes many guides and working examples - see the [Getting Started](#getting-started) section below.
 
 ## Getting Started
 <a name="getting_started"></a>
 
-I suggest starting with the worked examples below, which you can copy and adapt.
+I suggest starting with the [Colab notebook](https://colab.research.google.com/drive/17bb_KbA2J6yrIm4p4Ue_lEBHMNC1I9Jd?usp=sharing) or the worked examples below, which you can copy and adapt.
 
 For context and explanation, see the [documentation](https://zoobot.readthedocs.io/).
 
 For pretrained model weights, precalculated representations, catalogues, and so forth, see the [data notes](https://zoobot.readthedocs.io/data_notes.html) in particular.
 
 ### Worked Examples
 <a name="worked_examples"></a>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: zoobot Version: 1.0.2 Summary: Galaxy morphology
+Metadata-Version: 2.1 Name: zoobot Version: 1.0.3 Summary: Galaxy morphology
 classifiers Home-page: https://github.com/mwalmsley/zoobot Author: Mike
 Walmsley Author-email: walmsleymk1@gmail.com Classifier: Programming Language
 :: Python :: 3 Classifier: License :: OSI Approved :: GNU General Public
 License (GPL) Classifier: Operating System :: OS Independent Classifier:
 Development Status :: 4 - Beta Classifier: Environment :: GPU :: NVIDIA CUDA
 Requires-Python: >=3.8 Description-Content-Type: text/markdown Provides-Extra:
 pytorch_cpu Provides-Extra: pytorch_m1 Provides-Extra: pytorch_cu113 Provides-
@@ -38,33 +38,38 @@
 [editable mode](https://pip.pypa.io/en/stable/topics/local-project-installs/
 #editable-installs) so you can easily change the code locally. Zoobot is also
 available directly from pip (`pip install zoobot[option]`). Only use this if
 you are sure you won't be making changes to Zoobot itself. For Google Colab,
 use `pip install zoobot[pytorch_colab]` To use a GPU, you must *already* have
 CUDA installed and matching the versions above. I share my install steps [here]
 (#install_cuda). GPUs are optional - Zoobot will run retrain fine on CPU, just
-slower. ## Quickstart  Let's say you want to find ringed galaxies and you have
-a small labelled dataset of 500 ringed or not-ringed galaxies. You can retrain
-Zoobot to find rings like so: ```python import pandas as pd from
+slower. ## Quickstart  The [Colab notebook](https://colab.research.google.com/
+drive/17bb_KbA2J6yrIm4p4Ue_lEBHMNC1I9Jd?usp=sharing) is the quickest way to get
+started. Alternatively, the minimal example below illustrates how Zoobot works.
+Let's say you want to find ringed galaxies and you have a small labelled
+dataset of 500 ringed or not-ringed galaxies. You can retrain Zoobot to find
+rings like so: ```python import pandas as pd from
 galaxy_datasets.pytorch.galaxy_datamodule import GalaxyDataModule from
 zoobot.pytorch.training import finetune # csv with 'ring' column (0 or 1) and
 'file_loc' column (path to image) labelled_df = pd.read_csv('/your/path/
 some_labelled_galaxies.csv') datamodule = GalaxyDataModule( label_cols=
 ['ring'], catalog=labelled_df, batch_size=32 ) # load trained Zoobot model
 model = finetune.FinetuneableZoobotClassifier(checkpoint_loc, num_classes=2) #
 retrain to find rings trainer = finetune.get_trainer(save_dir) trainer.fit
 (model, datamodule) ``` Then you can make predict if new galaxies have rings:
 ```python from zoobot.pytorch.predictions import predict_on_catalog # csv with
 'file_loc' column (path to image). Zoobot will predict the labels.
 unlabelled_df = pd.read_csv('/your/path/some_unlabelled_galaxies.csv')
 predict_on_catalog.predict( unlabelled_df, model, label_cols=['ring'], # only
 used for save_loc='/your/path/finetuned_predictions.csv' ) ``` Zoobot includes
 many guides and working examples - see the [Getting Started](#getting-started)
-section below. ## Getting Started  I suggest starting with the worked examples
-below, which you can copy and adapt. For context and explanation, see the
+section below. ## Getting Started  I suggest starting with the [Colab notebook]
+(https://colab.research.google.com/drive/
+17bb_KbA2J6yrIm4p4Ue_lEBHMNC1I9Jd?usp=sharing) or the worked examples below,
+which you can copy and adapt. For context and explanation, see the
 [documentation](https://zoobot.readthedocs.io/). For pretrained model weights,
 precalculated representations, catalogues, and so forth, see the [data notes]
 (https://zoobot.readthedocs.io/data_notes.html) in particular. ### Worked
 Examples  PyTorch (recommended): - [pytorch/examples/finetuning/
 finetune_binary_classification.py](https://github.com/mwalmsley/zoobot/blob/
 main/zoobot/pytorch/examples/finetuning/finetune_binary_classification.py) -
 [pytorch/examples/finetuning/finetune_counts_full_tree.py](https://github.com/
```

### Comparing `zoobot-1.0.2/README.md` & `zoobot-1.0.3/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -47,14 +47,16 @@
 
 To use a GPU, you must *already* have CUDA installed and matching the versions above.
 I share my install steps [here](#install_cuda). GPUs are optional - Zoobot will run retrain fine on CPU, just slower.
 
 ## Quickstart
 <a name="quickstart"></a>
 
+The [Colab notebook](https://colab.research.google.com/drive/17bb_KbA2J6yrIm4p4Ue_lEBHMNC1I9Jd?usp=sharing) is the quickest way to get started. Alternatively, the minimal example below illustrates how Zoobot works.
+
 Let's say you want to find ringed galaxies and you have a small labelled dataset of 500 ringed or not-ringed galaxies. You can retrain Zoobot to find rings like so:
 
 ```python
 
     import pandas as pd
     from galaxy_datasets.pytorch.galaxy_datamodule import GalaxyDataModule
     from zoobot.pytorch.training import finetune
@@ -93,15 +95,15 @@
 ```
 
 Zoobot includes many guides and working examples - see the [Getting Started](#getting-started) section below.
 
 ## Getting Started
 <a name="getting_started"></a>
 
-I suggest starting with the worked examples below, which you can copy and adapt.
+I suggest starting with the [Colab notebook](https://colab.research.google.com/drive/17bb_KbA2J6yrIm4p4Ue_lEBHMNC1I9Jd?usp=sharing) or the worked examples below, which you can copy and adapt.
 
 For context and explanation, see the [documentation](https://zoobot.readthedocs.io/).
 
 For pretrained model weights, precalculated representations, catalogues, and so forth, see the [data notes](https://zoobot.readthedocs.io/data_notes.html) in particular.
 
 ### Worked Examples
 <a name="worked_examples"></a>
@@ -188,8 +190,8 @@
 
 - [Galaxy Zoo DECaLS](https://arxiv.org/abs/2102.08414) (first use at Galaxy Zoo)
 - [A Comparison of Deep Learning Architectures for Optical Galaxy Morphology Classification](https://arxiv.org/abs/2111.04353)
 - [Practical Galaxy Morphology Tools from Deep Supervised Representation Learning](https://arxiv.org/abs/2110.12735)
 - [Towards Foundation Models for Galaxy Morphology](https://arxiv.org/abs/2206.11927) (adding contrastive learning)
 - [Harnessing the Hubble Space Telescope Archives: A Catalogue of 21,926 Interacting Galaxies](https://arxiv.org/abs/2303.00366)
 
-Many other works use Zoobot indirectly via the [Galaxy Zoo DECaLS](https://arxiv.org/abs/2102.08414) catalog.
+Many other works use Zoobot indirectly via the [Galaxy Zoo DECaLS](https://arxiv.org/abs/2102.08414) catalog.
```

#### html2text {}

```diff
@@ -29,33 +29,38 @@
 [editable mode](https://pip.pypa.io/en/stable/topics/local-project-installs/
 #editable-installs) so you can easily change the code locally. Zoobot is also
 available directly from pip (`pip install zoobot[option]`). Only use this if
 you are sure you won't be making changes to Zoobot itself. For Google Colab,
 use `pip install zoobot[pytorch_colab]` To use a GPU, you must *already* have
 CUDA installed and matching the versions above. I share my install steps [here]
 (#install_cuda). GPUs are optional - Zoobot will run retrain fine on CPU, just
-slower. ## Quickstart  Let's say you want to find ringed galaxies and you have
-a small labelled dataset of 500 ringed or not-ringed galaxies. You can retrain
-Zoobot to find rings like so: ```python import pandas as pd from
+slower. ## Quickstart  The [Colab notebook](https://colab.research.google.com/
+drive/17bb_KbA2J6yrIm4p4Ue_lEBHMNC1I9Jd?usp=sharing) is the quickest way to get
+started. Alternatively, the minimal example below illustrates how Zoobot works.
+Let's say you want to find ringed galaxies and you have a small labelled
+dataset of 500 ringed or not-ringed galaxies. You can retrain Zoobot to find
+rings like so: ```python import pandas as pd from
 galaxy_datasets.pytorch.galaxy_datamodule import GalaxyDataModule from
 zoobot.pytorch.training import finetune # csv with 'ring' column (0 or 1) and
 'file_loc' column (path to image) labelled_df = pd.read_csv('/your/path/
 some_labelled_galaxies.csv') datamodule = GalaxyDataModule( label_cols=
 ['ring'], catalog=labelled_df, batch_size=32 ) # load trained Zoobot model
 model = finetune.FinetuneableZoobotClassifier(checkpoint_loc, num_classes=2) #
 retrain to find rings trainer = finetune.get_trainer(save_dir) trainer.fit
 (model, datamodule) ``` Then you can make predict if new galaxies have rings:
 ```python from zoobot.pytorch.predictions import predict_on_catalog # csv with
 'file_loc' column (path to image). Zoobot will predict the labels.
 unlabelled_df = pd.read_csv('/your/path/some_unlabelled_galaxies.csv')
 predict_on_catalog.predict( unlabelled_df, model, label_cols=['ring'], # only
 used for save_loc='/your/path/finetuned_predictions.csv' ) ``` Zoobot includes
 many guides and working examples - see the [Getting Started](#getting-started)
-section below. ## Getting Started  I suggest starting with the worked examples
-below, which you can copy and adapt. For context and explanation, see the
+section below. ## Getting Started  I suggest starting with the [Colab notebook]
+(https://colab.research.google.com/drive/
+17bb_KbA2J6yrIm4p4Ue_lEBHMNC1I9Jd?usp=sharing) or the worked examples below,
+which you can copy and adapt. For context and explanation, see the
 [documentation](https://zoobot.readthedocs.io/). For pretrained model weights,
 precalculated representations, catalogues, and so forth, see the [data notes]
 (https://zoobot.readthedocs.io/data_notes.html) in particular. ### Worked
 Examples  PyTorch (recommended): - [pytorch/examples/finetuning/
 finetune_binary_classification.py](https://github.com/mwalmsley/zoobot/blob/
 main/zoobot/pytorch/examples/finetuning/finetune_binary_classification.py) -
 [pytorch/examples/finetuning/finetune_counts_full_tree.py](https://github.com/
```

### Comparing `zoobot-1.0.2/setup.py` & `zoobot-1.0.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="zoobot",
-    version="1.0.2",
+    version="1.0.3",
     author="Mike Walmsley",
     author_email="walmsleymk1@gmail.com",
     description="Galaxy morphology classifiers",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/mwalmsley/zoobot",
     classifiers=[
```

### Comparing `zoobot-1.0.2/tests/test_loss_equivalence.py` & `zoobot-1.0.3/tests/test_loss_equivalence.py`

 * *Files identical despite different names*

### Comparing `zoobot-1.0.2/zoobot/pytorch/estimators/custom_layers.py` & `zoobot-1.0.3/zoobot/pytorch/estimators/custom_layers.py`

 * *Files identical despite different names*

### Comparing `zoobot-1.0.2/zoobot/pytorch/estimators/define_model.py` & `zoobot-1.0.3/zoobot/pytorch/estimators/define_model.py`

 * *Files identical despite different names*

### Comparing `zoobot-1.0.2/zoobot/pytorch/estimators/efficientnet_custom.py` & `zoobot-1.0.3/zoobot/pytorch/estimators/efficientnet_custom.py`

 * *Files identical despite different names*

### Comparing `zoobot-1.0.2/zoobot/pytorch/manchester.py` & `zoobot-1.0.3/zoobot/pytorch/manchester.py`

 * *Files identical despite different names*

### Comparing `zoobot-1.0.2/zoobot/pytorch/predictions/predict_on_catalog.py` & `zoobot-1.0.3/zoobot/pytorch/predictions/predict_on_catalog.py`

 * *Files identical despite different names*

### Comparing `zoobot-1.0.2/zoobot/pytorch/training/finetune.py` & `zoobot-1.0.3/zoobot/pytorch/training/finetune.py`

 * *Files identical despite different names*

### Comparing `zoobot-1.0.2/zoobot/pytorch/training/losses.py` & `zoobot-1.0.3/zoobot/pytorch/training/losses.py`

 * *Files identical despite different names*

### Comparing `zoobot-1.0.2/zoobot/pytorch/training/representations.py` & `zoobot-1.0.3/zoobot/pytorch/training/representations.py`

 * *Files identical despite different names*

### Comparing `zoobot-1.0.2/zoobot/pytorch/training/tensorboard_writers.py` & `zoobot-1.0.3/zoobot/pytorch/training/tensorboard_writers.py`

 * *Files identical despite different names*

### Comparing `zoobot-1.0.2/zoobot/pytorch/training/train_with_pytorch_lightning.py` & `zoobot-1.0.3/zoobot/pytorch/training/train_with_pytorch_lightning.py`

 * *Files identical despite different names*

### Comparing `zoobot-1.0.2/zoobot/shared/benchmark_datasets.py` & `zoobot-1.0.3/zoobot/shared/benchmark_datasets.py`

 * *Files identical despite different names*

### Comparing `zoobot-1.0.2/zoobot/shared/compress_representations.py` & `zoobot-1.0.3/zoobot/shared/compress_representations.py`

 * *Files identical despite different names*

### Comparing `zoobot-1.0.2/zoobot/shared/label_metadata.py` & `zoobot-1.0.3/zoobot/shared/label_metadata.py`

 * *Files identical despite different names*

### Comparing `zoobot-1.0.2/zoobot/shared/load_predictions.py` & `zoobot-1.0.3/zoobot/shared/load_predictions.py`

 * *Files identical despite different names*

### Comparing `zoobot-1.0.2/zoobot/shared/save_predictions.py` & `zoobot-1.0.3/zoobot/shared/save_predictions.py`

 * *Files identical despite different names*

### Comparing `zoobot-1.0.2/zoobot/shared/schemas.py` & `zoobot-1.0.3/zoobot/shared/schemas.py`

 * *Files identical despite different names*

### Comparing `zoobot-1.0.2/zoobot/shared/stats.py` & `zoobot-1.0.3/zoobot/shared/stats.py`

 * *Files identical despite different names*

### Comparing `zoobot-1.0.2/zoobot/tensorflow/estimators/alexnet_baseline.py` & `zoobot-1.0.3/zoobot/tensorflow/estimators/alexnet_baseline.py`

 * *Files identical despite different names*

### Comparing `zoobot-1.0.2/zoobot/tensorflow/estimators/custom_callbacks.py` & `zoobot-1.0.3/zoobot/tensorflow/estimators/custom_callbacks.py`

 * *Files identical despite different names*

### Comparing `zoobot-1.0.2/zoobot/tensorflow/estimators/custom_layers.py` & `zoobot-1.0.3/zoobot/tensorflow/estimators/custom_layers.py`

 * *Files identical despite different names*

### Comparing `zoobot-1.0.2/zoobot/tensorflow/estimators/define_model.py` & `zoobot-1.0.3/zoobot/tensorflow/estimators/define_model.py`

 * *Files identical despite different names*

### Comparing `zoobot-1.0.2/zoobot/tensorflow/estimators/efficientnet_custom.py` & `zoobot-1.0.3/zoobot/tensorflow/estimators/efficientnet_custom.py`

 * *Files identical despite different names*

### Comparing `zoobot-1.0.2/zoobot/tensorflow/estimators/efficientnet_standard.py` & `zoobot-1.0.3/zoobot/tensorflow/estimators/efficientnet_standard.py`

 * *Files identical despite different names*

### Comparing `zoobot-1.0.2/zoobot/tensorflow/estimators/small_cnn_baseline.py` & `zoobot-1.0.3/zoobot/tensorflow/estimators/small_cnn_baseline.py`

 * *Files identical despite different names*

### Comparing `zoobot-1.0.2/zoobot/tensorflow/predictions/predict_on_dataset.py` & `zoobot-1.0.3/zoobot/tensorflow/predictions/predict_on_dataset.py`

 * *Files identical despite different names*

### Comparing `zoobot-1.0.2/zoobot/tensorflow/predictions/visualize_dirichlet_predictions.py` & `zoobot-1.0.3/zoobot/tensorflow/predictions/visualize_dirichlet_predictions.py`

 * *Files identical despite different names*

### Comparing `zoobot-1.0.2/zoobot/tensorflow/stats/coverage.py` & `zoobot-1.0.3/zoobot/tensorflow/stats/coverage.py`

 * *Files identical despite different names*

### Comparing `zoobot-1.0.2/zoobot/tensorflow/stats/dirichlet_stats.py` & `zoobot-1.0.3/zoobot/tensorflow/stats/dirichlet_stats.py`

 * *Files identical despite different names*

### Comparing `zoobot-1.0.2/zoobot/tensorflow/stats/mixture_stats.py` & `zoobot-1.0.3/zoobot/tensorflow/stats/mixture_stats.py`

 * *Files identical despite different names*

### Comparing `zoobot-1.0.2/zoobot/tensorflow/training/custom_metrics.py` & `zoobot-1.0.3/zoobot/tensorflow/training/custom_metrics.py`

 * *Files identical despite different names*

### Comparing `zoobot-1.0.2/zoobot/tensorflow/training/finetune.py` & `zoobot-1.0.3/zoobot/tensorflow/training/finetune.py`

 * *Files identical despite different names*

### Comparing `zoobot-1.0.2/zoobot/tensorflow/training/losses.py` & `zoobot-1.0.3/zoobot/tensorflow/training/losses.py`

 * *Files identical despite different names*

### Comparing `zoobot-1.0.2/zoobot/tensorflow/training/train_with_keras.py` & `zoobot-1.0.3/zoobot/tensorflow/training/train_with_keras.py`

 * *Files identical despite different names*

### Comparing `zoobot-1.0.2/zoobot/tensorflow/training/training_config.py` & `zoobot-1.0.3/zoobot/tensorflow/training/training_config.py`

 * *Files identical despite different names*

### Comparing `zoobot-1.0.2/zoobot.egg-info/PKG-INFO` & `zoobot-1.0.3/zoobot.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zoobot
-Version: 1.0.2
+Version: 1.0.3
 Summary: Galaxy morphology classifiers
 Home-page: https://github.com/mwalmsley/zoobot
 Author: Mike Walmsley
 Author-email: walmsleymk1@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License (GPL)
 Classifier: Operating System :: OS Independent
@@ -70,14 +70,16 @@
 
 To use a GPU, you must *already* have CUDA installed and matching the versions above.
 I share my install steps [here](#install_cuda). GPUs are optional - Zoobot will run retrain fine on CPU, just slower.
 
 ## Quickstart
 <a name="quickstart"></a>
 
+The [Colab notebook](https://colab.research.google.com/drive/17bb_KbA2J6yrIm4p4Ue_lEBHMNC1I9Jd?usp=sharing) is the quickest way to get started. Alternatively, the minimal example below illustrates how Zoobot works.
+
 Let's say you want to find ringed galaxies and you have a small labelled dataset of 500 ringed or not-ringed galaxies. You can retrain Zoobot to find rings like so:
 
 ```python
 
     import pandas as pd
     from galaxy_datasets.pytorch.galaxy_datamodule import GalaxyDataModule
     from zoobot.pytorch.training import finetune
@@ -116,15 +118,15 @@
 ```
 
 Zoobot includes many guides and working examples - see the [Getting Started](#getting-started) section below.
 
 ## Getting Started
 <a name="getting_started"></a>
 
-I suggest starting with the worked examples below, which you can copy and adapt.
+I suggest starting with the [Colab notebook](https://colab.research.google.com/drive/17bb_KbA2J6yrIm4p4Ue_lEBHMNC1I9Jd?usp=sharing) or the worked examples below, which you can copy and adapt.
 
 For context and explanation, see the [documentation](https://zoobot.readthedocs.io/).
 
 For pretrained model weights, precalculated representations, catalogues, and so forth, see the [data notes](https://zoobot.readthedocs.io/data_notes.html) in particular.
 
 ### Worked Examples
 <a name="worked_examples"></a>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: zoobot Version: 1.0.2 Summary: Galaxy morphology
+Metadata-Version: 2.1 Name: zoobot Version: 1.0.3 Summary: Galaxy morphology
 classifiers Home-page: https://github.com/mwalmsley/zoobot Author: Mike
 Walmsley Author-email: walmsleymk1@gmail.com Classifier: Programming Language
 :: Python :: 3 Classifier: License :: OSI Approved :: GNU General Public
 License (GPL) Classifier: Operating System :: OS Independent Classifier:
 Development Status :: 4 - Beta Classifier: Environment :: GPU :: NVIDIA CUDA
 Requires-Python: >=3.8 Description-Content-Type: text/markdown Provides-Extra:
 pytorch_cpu Provides-Extra: pytorch_m1 Provides-Extra: pytorch_cu113 Provides-
@@ -38,33 +38,38 @@
 [editable mode](https://pip.pypa.io/en/stable/topics/local-project-installs/
 #editable-installs) so you can easily change the code locally. Zoobot is also
 available directly from pip (`pip install zoobot[option]`). Only use this if
 you are sure you won't be making changes to Zoobot itself. For Google Colab,
 use `pip install zoobot[pytorch_colab]` To use a GPU, you must *already* have
 CUDA installed and matching the versions above. I share my install steps [here]
 (#install_cuda). GPUs are optional - Zoobot will run retrain fine on CPU, just
-slower. ## Quickstart  Let's say you want to find ringed galaxies and you have
-a small labelled dataset of 500 ringed or not-ringed galaxies. You can retrain
-Zoobot to find rings like so: ```python import pandas as pd from
+slower. ## Quickstart  The [Colab notebook](https://colab.research.google.com/
+drive/17bb_KbA2J6yrIm4p4Ue_lEBHMNC1I9Jd?usp=sharing) is the quickest way to get
+started. Alternatively, the minimal example below illustrates how Zoobot works.
+Let's say you want to find ringed galaxies and you have a small labelled
+dataset of 500 ringed or not-ringed galaxies. You can retrain Zoobot to find
+rings like so: ```python import pandas as pd from
 galaxy_datasets.pytorch.galaxy_datamodule import GalaxyDataModule from
 zoobot.pytorch.training import finetune # csv with 'ring' column (0 or 1) and
 'file_loc' column (path to image) labelled_df = pd.read_csv('/your/path/
 some_labelled_galaxies.csv') datamodule = GalaxyDataModule( label_cols=
 ['ring'], catalog=labelled_df, batch_size=32 ) # load trained Zoobot model
 model = finetune.FinetuneableZoobotClassifier(checkpoint_loc, num_classes=2) #
 retrain to find rings trainer = finetune.get_trainer(save_dir) trainer.fit
 (model, datamodule) ``` Then you can make predict if new galaxies have rings:
 ```python from zoobot.pytorch.predictions import predict_on_catalog # csv with
 'file_loc' column (path to image). Zoobot will predict the labels.
 unlabelled_df = pd.read_csv('/your/path/some_unlabelled_galaxies.csv')
 predict_on_catalog.predict( unlabelled_df, model, label_cols=['ring'], # only
 used for save_loc='/your/path/finetuned_predictions.csv' ) ``` Zoobot includes
 many guides and working examples - see the [Getting Started](#getting-started)
-section below. ## Getting Started  I suggest starting with the worked examples
-below, which you can copy and adapt. For context and explanation, see the
+section below. ## Getting Started  I suggest starting with the [Colab notebook]
+(https://colab.research.google.com/drive/
+17bb_KbA2J6yrIm4p4Ue_lEBHMNC1I9Jd?usp=sharing) or the worked examples below,
+which you can copy and adapt. For context and explanation, see the
 [documentation](https://zoobot.readthedocs.io/). For pretrained model weights,
 precalculated representations, catalogues, and so forth, see the [data notes]
 (https://zoobot.readthedocs.io/data_notes.html) in particular. ### Worked
 Examples  PyTorch (recommended): - [pytorch/examples/finetuning/
 finetune_binary_classification.py](https://github.com/mwalmsley/zoobot/blob/
 main/zoobot/pytorch/examples/finetuning/finetune_binary_classification.py) -
 [pytorch/examples/finetuning/finetune_counts_full_tree.py](https://github.com/
```

### Comparing `zoobot-1.0.2/zoobot.egg-info/SOURCES.txt` & `zoobot-1.0.3/zoobot.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `zoobot-1.0.2/zoobot.egg-info/requires.txt` & `zoobot-1.0.3/zoobot.egg-info/requires.txt`

 * *Files identical despite different names*

