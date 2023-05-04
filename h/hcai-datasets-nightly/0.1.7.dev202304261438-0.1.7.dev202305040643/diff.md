# Comparing `tmp/hcai-datasets-nightly-0.1.7.dev202304261438.tar.gz` & `tmp/hcai-datasets-nightly-0.1.7.dev202305040643.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hcai-datasets-nightly-0.1.7.dev202304261438.tar", last modified: Wed Apr 26 14:38:05 2023, max compression
+gzip compressed data, was "hcai-datasets-nightly-0.1.7.dev202305040643.tar", last modified: Thu May  4 06:43:54 2023, max compression
```

## Comparing `hcai-datasets-nightly-0.1.7.dev202304261438.tar` & `hcai-datasets-nightly-0.1.7.dev202305040643.tar`

### file list

```diff
@@ -1,72 +1,72 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-26 14:38:05.117537 hcai-datasets-nightly-0.1.7.dev202304261438/
--rw-r--r--   0 runner    (1001) docker     (122)      297 2023-04-26 14:37:48.000000 hcai-datasets-nightly-0.1.7.dev202304261438/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)     9089 2023-04-26 14:38:05.117537 hcai-datasets-nightly-0.1.7.dev202304261438/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     8154 2023-04-26 14:37:48.000000 hcai-datasets-nightly-0.1.7.dev202304261438/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-26 14:38:05.113537 hcai-datasets-nightly-0.1.7.dev202304261438/hcai_dataset_utils/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-26 14:37:48.000000 hcai-datasets-nightly-0.1.7.dev202304261438/hcai_dataset_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1094 2023-04-26 14:37:48.000000 hcai-datasets-nightly-0.1.7.dev202304261438/hcai_dataset_utils/bridge_pytorch.py
--rw-r--r--   0 runner    (1001) docker     (122)      928 2023-04-26 14:37:48.000000 hcai-datasets-nightly-0.1.7.dev202304261438/hcai_dataset_utils/bridge_tf.py
--rw-r--r--   0 runner    (1001) docker     (122)      365 2023-04-26 14:37:48.000000 hcai-datasets-nightly-0.1.7.dev202304261438/hcai_dataset_utils/dataset_indexed.py
--rw-r--r--   0 runner    (1001) docker     (122)      735 2023-04-26 14:37:48.000000 hcai-datasets-nightly-0.1.7.dev202304261438/hcai_dataset_utils/import_validator.py
--rw-r--r--   0 runner    (1001) docker     (122)     3028 2023-04-26 14:37:48.000000 hcai-datasets-nightly-0.1.7.dev202304261438/hcai_dataset_utils/pytorch_dataset_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (122)     2770 2023-04-26 14:37:48.000000 hcai-datasets-nightly-0.1.7.dev202304261438/hcai_dataset_utils/statistics.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-26 14:38:05.113537 hcai-datasets-nightly-0.1.7.dev202304261438/hcai_datasets/
--rw-r--r--   0 runner    (1001) docker     (122)     1063 2023-04-26 14:37:48.000000 hcai-datasets-nightly-0.1.7.dev202304261438/hcai_datasets/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-26 14:38:05.113537 hcai-datasets-nightly-0.1.7.dev202304261438/hcai_datasets/examples/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-26 14:37:48.000000 hcai-datasets-nightly-0.1.7.dev202304261438/hcai_datasets/examples/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      607 2023-04-26 14:37:48.000000 hcai-datasets-nightly-0.1.7.dev202304261438/hcai_datasets/examples/example_affectnet_pytorch.py
--rw-r--r--   0 runner    (1001) docker     (122)     1460 2023-04-26 14:37:48.000000 hcai-datasets-nightly-0.1.7.dev202304261438/hcai_datasets/examples/example_affectnet_tensorflow_native.py
--rw-r--r--   0 runner    (1001) docker     (122)      957 2023-04-26 14:37:48.000000 hcai-datasets-nightly-0.1.7.dev202304261438/hcai_datasets/examples/example_affectnet_tfds.py
--rw-r--r--   0 runner    (1001) docker     (122)     1435 2023-04-26 14:37:48.000000 hcai-datasets-nightly-0.1.7.dev202304261438/hcai_datasets/examples/example_ckplus_tensorflow_native.py
--rw-r--r--   0 runner    (1001) docker     (122)      946 2023-04-26 14:37:48.000000 hcai-datasets-nightly-0.1.7.dev202304261438/hcai_datasets/examples/example_ckplus_tfds.py
--rw-r--r--   0 runner    (1001) docker     (122)     1435 2023-04-26 14:37:48.000000 hcai-datasets-nightly-0.1.7.dev202304261438/hcai_datasets/examples/example_faces_tensorflow_native.py
--rw-r--r--   0 runner    (1001) docker     (122)      947 2023-04-26 14:37:48.000000 hcai-datasets-nightly-0.1.7.dev202304261438/hcai_datasets/examples/example_faces_tfds.py
--rw-r--r--   0 runner    (1001) docker     (122)     1977 2023-04-26 14:37:48.000000 hcai-datasets-nightly-0.1.7.dev202304261438/hcai_datasets/examples/example_nova_tensorflow_native.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-26 14:38:05.113537 hcai-datasets-nightly-0.1.7.dev202304261438/hcai_datasets/hcai_affectnet/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-26 14:38:05.113537 hcai-datasets-nightly-0.1.7.dev202304261438/hcai_datasets/hcai_affectnet/Ignore_Lists/
--rw-r--r--   0 runner    (1001) docker     (122)  2377285 2023-04-26 14:37:48.000000 hcai-datasets-nightly-0.1.7.dev202304261438/hcai_datasets/hcai_affectnet/Ignore_Lists/affect_net_ignore_list_duplicates.json
--rw-r--r--   0 runner    (1001) docker     (122)     6234 2023-04-26 14:37:48.000000 hcai-datasets-nightly-0.1.7.dev202304261438/hcai_datasets/hcai_affectnet/Ignore_Lists/affect_net_ignore_list_wrong_format.json
--rw-r--r--   0 runner    (1001) docker     (122)       72 2023-04-26 14:37:49.000000 hcai-datasets-nightly-0.1.7.dev202304261438/hcai_datasets/hcai_affectnet/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     6829 2023-04-26 14:37:49.000000 hcai-datasets-nightly-0.1.7.dev202304261438/hcai_datasets/hcai_affectnet/hcai_affectnet.py
--rw-r--r--   0 runner    (1001) docker     (122)     5916 2023-04-26 14:37:49.000000 hcai-datasets-nightly-0.1.7.dev202304261438/hcai_datasets/hcai_affectnet/hcai_affectnet_iterable.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-26 14:38:05.113537 hcai-datasets-nightly-0.1.7.dev202304261438/hcai_datasets/hcai_audioset/
--rw-r--r--   0 runner    (1001) docker     (122)       66 2023-04-26 14:37:49.000000 hcai-datasets-nightly-0.1.7.dev202304261438/hcai_datasets/hcai_audioset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2412 2023-04-26 14:37:49.000000 hcai-datasets-nightly-0.1.7.dev202304261438/hcai_datasets/hcai_audioset/hcai_audioset.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-26 14:38:05.117537 hcai-datasets-nightly-0.1.7.dev202304261438/hcai_datasets/hcai_ckplus/
--rw-r--r--   0 runner    (1001) docker     (122)       60 2023-04-26 14:37:49.000000 hcai-datasets-nightly-0.1.7.dev202304261438/hcai_datasets/hcai_ckplus/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3017 2023-04-26 14:37:49.000000 hcai-datasets-nightly-0.1.7.dev202304261438/hcai_datasets/hcai_ckplus/hcai_ckplus.py
--rw-r--r--   0 runner    (1001) docker     (122)     1940 2023-04-26 14:37:49.000000 hcai-datasets-nightly-0.1.7.dev202304261438/hcai_datasets/hcai_ckplus/hcai_ckplus_iterable.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-26 14:38:05.117537 hcai-datasets-nightly-0.1.7.dev202304261438/hcai_datasets/hcai_faces/
--rw-r--r--   0 runner    (1001) docker     (122)       57 2023-04-26 14:37:49.000000 hcai-datasets-nightly-0.1.7.dev202304261438/hcai_datasets/hcai_faces/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3303 2023-04-26 14:37:49.000000 hcai-datasets-nightly-0.1.7.dev202304261438/hcai_datasets/hcai_faces/hcai_faces.py
--rw-r--r--   0 runner    (1001) docker     (122)     2051 2023-04-26 14:37:49.000000 hcai-datasets-nightly-0.1.7.dev202304261438/hcai_datasets/hcai_faces/hcai_faces_iterable.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-26 14:38:05.117537 hcai-datasets-nightly-0.1.7.dev202304261438/hcai_datasets/hcai_is2021_ess/
--rw-r--r--   0 runner    (1001) docker     (122)       71 2023-04-26 14:37:49.000000 hcai-datasets-nightly-0.1.7.dev202304261438/hcai_datasets/hcai_is2021_ess/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2756 2023-04-26 14:37:49.000000 hcai-datasets-nightly-0.1.7.dev202304261438/hcai_datasets/hcai_is2021_ess/hcai_is2021_ess.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-26 14:38:05.117537 hcai-datasets-nightly-0.1.7.dev202304261438/hcai_datasets/hcai_librispeech/
--rw-r--r--   0 runner    (1001) docker     (122)       75 2023-04-26 14:37:49.000000 hcai-datasets-nightly-0.1.7.dev202304261438/hcai_datasets/hcai_librispeech/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     4323 2023-04-26 14:37:49.000000 hcai-datasets-nightly-0.1.7.dev202304261438/hcai_datasets/hcai_librispeech/hcai_librispeech.py
--rw-r--r--   0 runner    (1001) docker     (122)      711 2023-04-26 14:37:49.000000 hcai-datasets-nightly-0.1.7.dev202304261438/hcai_datasets/hcai_librispeech/preprocessing.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-26 14:38:05.117537 hcai-datasets-nightly-0.1.7.dev202304261438/hcai_datasets/hcai_nova_dynamic/
--rw-r--r--   0 runner    (1001) docker     (122)       83 2023-04-26 14:37:49.000000 hcai-datasets-nightly-0.1.7.dev202304261438/hcai_datasets/hcai_nova_dynamic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    20593 2023-04-26 14:37:49.000000 hcai-datasets-nightly-0.1.7.dev202304261438/hcai_datasets/hcai_nova_dynamic/hcai_nova_dynamic_iterable.py
--rw-r--r--   0 runner    (1001) docker     (122)     7686 2023-04-26 14:37:49.000000 hcai-datasets-nightly-0.1.7.dev202304261438/hcai_datasets/hcai_nova_dynamic/hcai_nova_dynamic_tfds.py
--rw-r--r--   0 runner    (1001) docker     (122)    24935 2023-04-26 14:37:49.000000 hcai-datasets-nightly-0.1.7.dev202304261438/hcai_datasets/hcai_nova_dynamic/nova_db_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-26 14:38:05.117537 hcai-datasets-nightly-0.1.7.dev202304261438/hcai_datasets/hcai_nova_dynamic/utils/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-26 14:37:49.000000 hcai-datasets-nightly-0.1.7.dev202304261438/hcai_datasets/hcai_nova_dynamic/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    12651 2023-04-26 14:37:49.000000 hcai-datasets-nightly-0.1.7.dev202304261438/hcai_datasets/hcai_nova_dynamic/utils/nova_anno_utils.py
--rw-r--r--   0 runner    (1001) docker     (122)    13914 2023-04-26 14:37:49.000000 hcai-datasets-nightly-0.1.7.dev202304261438/hcai_datasets/hcai_nova_dynamic/utils/nova_data_utils.py
--rw-r--r--   0 runner    (1001) docker     (122)      216 2023-04-26 14:37:49.000000 hcai-datasets-nightly-0.1.7.dev202304261438/hcai_datasets/hcai_nova_dynamic/utils/nova_string_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-26 14:38:05.117537 hcai-datasets-nightly-0.1.7.dev202304261438/hcai_datasets/tests/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-26 14:37:49.000000 hcai-datasets-nightly-0.1.7.dev202304261438/hcai_datasets/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1198 2023-04-26 14:37:49.000000 hcai-datasets-nightly-0.1.7.dev202304261438/hcai_datasets/tests/dummy_set.py
--rw-r--r--   0 runner    (1001) docker     (122)      600 2023-04-26 14:37:49.000000 hcai-datasets-nightly-0.1.7.dev202304261438/hcai_datasets/tests/test_bridge_pytorch.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-26 14:38:05.117537 hcai-datasets-nightly-0.1.7.dev202304261438/hcai_datasets_nightly.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     9089 2023-04-26 14:38:05.000000 hcai-datasets-nightly-0.1.7.dev202304261438/hcai_datasets_nightly.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     2439 2023-04-26 14:38:05.000000 hcai-datasets-nightly-0.1.7.dev202304261438/hcai_datasets_nightly.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-26 14:38:05.000000 hcai-datasets-nightly-0.1.7.dev202304261438/hcai_datasets_nightly.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)      135 2023-04-26 14:38:05.000000 hcai-datasets-nightly-0.1.7.dev202304261438/hcai_datasets_nightly.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       33 2023-04-26 14:38:05.000000 hcai-datasets-nightly-0.1.7.dev202304261438/hcai_datasets_nightly.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)      103 2023-04-26 14:37:49.000000 hcai-datasets-nightly-0.1.7.dev202304261438/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-04-26 14:38:05.117537 hcai-datasets-nightly-0.1.7.dev202304261438/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     2181 2023-04-26 14:37:49.000000 hcai-datasets-nightly-0.1.7.dev202304261438/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-04 06:43:54.831663 hcai-datasets-nightly-0.1.7.dev202305040643/
+-rw-r--r--   0 runner    (1001) docker     (122)      297 2023-05-04 06:43:39.000000 hcai-datasets-nightly-0.1.7.dev202305040643/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)     9089 2023-05-04 06:43:54.831663 hcai-datasets-nightly-0.1.7.dev202305040643/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     8154 2023-05-04 06:43:39.000000 hcai-datasets-nightly-0.1.7.dev202305040643/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-04 06:43:54.823663 hcai-datasets-nightly-0.1.7.dev202305040643/hcai_dataset_utils/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-04 06:43:39.000000 hcai-datasets-nightly-0.1.7.dev202305040643/hcai_dataset_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1094 2023-05-04 06:43:39.000000 hcai-datasets-nightly-0.1.7.dev202305040643/hcai_dataset_utils/bridge_pytorch.py
+-rw-r--r--   0 runner    (1001) docker     (122)      928 2023-05-04 06:43:39.000000 hcai-datasets-nightly-0.1.7.dev202305040643/hcai_dataset_utils/bridge_tf.py
+-rw-r--r--   0 runner    (1001) docker     (122)      365 2023-05-04 06:43:39.000000 hcai-datasets-nightly-0.1.7.dev202305040643/hcai_dataset_utils/dataset_indexed.py
+-rw-r--r--   0 runner    (1001) docker     (122)      735 2023-05-04 06:43:39.000000 hcai-datasets-nightly-0.1.7.dev202305040643/hcai_dataset_utils/import_validator.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3028 2023-05-04 06:43:39.000000 hcai-datasets-nightly-0.1.7.dev202305040643/hcai_dataset_utils/pytorch_dataset_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2770 2023-05-04 06:43:39.000000 hcai-datasets-nightly-0.1.7.dev202305040643/hcai_dataset_utils/statistics.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-04 06:43:54.823663 hcai-datasets-nightly-0.1.7.dev202305040643/hcai_datasets/
+-rw-r--r--   0 runner    (1001) docker     (122)     1063 2023-05-04 06:43:39.000000 hcai-datasets-nightly-0.1.7.dev202305040643/hcai_datasets/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-04 06:43:54.823663 hcai-datasets-nightly-0.1.7.dev202305040643/hcai_datasets/examples/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-04 06:43:39.000000 hcai-datasets-nightly-0.1.7.dev202305040643/hcai_datasets/examples/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      607 2023-05-04 06:43:39.000000 hcai-datasets-nightly-0.1.7.dev202305040643/hcai_datasets/examples/example_affectnet_pytorch.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1460 2023-05-04 06:43:39.000000 hcai-datasets-nightly-0.1.7.dev202305040643/hcai_datasets/examples/example_affectnet_tensorflow_native.py
+-rw-r--r--   0 runner    (1001) docker     (122)      957 2023-05-04 06:43:39.000000 hcai-datasets-nightly-0.1.7.dev202305040643/hcai_datasets/examples/example_affectnet_tfds.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1435 2023-05-04 06:43:39.000000 hcai-datasets-nightly-0.1.7.dev202305040643/hcai_datasets/examples/example_ckplus_tensorflow_native.py
+-rw-r--r--   0 runner    (1001) docker     (122)      946 2023-05-04 06:43:39.000000 hcai-datasets-nightly-0.1.7.dev202305040643/hcai_datasets/examples/example_ckplus_tfds.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1435 2023-05-04 06:43:39.000000 hcai-datasets-nightly-0.1.7.dev202305040643/hcai_datasets/examples/example_faces_tensorflow_native.py
+-rw-r--r--   0 runner    (1001) docker     (122)      947 2023-05-04 06:43:39.000000 hcai-datasets-nightly-0.1.7.dev202305040643/hcai_datasets/examples/example_faces_tfds.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1977 2023-05-04 06:43:39.000000 hcai-datasets-nightly-0.1.7.dev202305040643/hcai_datasets/examples/example_nova_tensorflow_native.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-04 06:43:54.827663 hcai-datasets-nightly-0.1.7.dev202305040643/hcai_datasets/hcai_affectnet/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-04 06:43:54.827663 hcai-datasets-nightly-0.1.7.dev202305040643/hcai_datasets/hcai_affectnet/Ignore_Lists/
+-rw-r--r--   0 runner    (1001) docker     (122)  2377285 2023-05-04 06:43:39.000000 hcai-datasets-nightly-0.1.7.dev202305040643/hcai_datasets/hcai_affectnet/Ignore_Lists/affect_net_ignore_list_duplicates.json
+-rw-r--r--   0 runner    (1001) docker     (122)     6234 2023-05-04 06:43:39.000000 hcai-datasets-nightly-0.1.7.dev202305040643/hcai_datasets/hcai_affectnet/Ignore_Lists/affect_net_ignore_list_wrong_format.json
+-rw-r--r--   0 runner    (1001) docker     (122)       72 2023-05-04 06:43:39.000000 hcai-datasets-nightly-0.1.7.dev202305040643/hcai_datasets/hcai_affectnet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6829 2023-05-04 06:43:39.000000 hcai-datasets-nightly-0.1.7.dev202305040643/hcai_datasets/hcai_affectnet/hcai_affectnet.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5916 2023-05-04 06:43:39.000000 hcai-datasets-nightly-0.1.7.dev202305040643/hcai_datasets/hcai_affectnet/hcai_affectnet_iterable.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-04 06:43:54.827663 hcai-datasets-nightly-0.1.7.dev202305040643/hcai_datasets/hcai_audioset/
+-rw-r--r--   0 runner    (1001) docker     (122)       66 2023-05-04 06:43:39.000000 hcai-datasets-nightly-0.1.7.dev202305040643/hcai_datasets/hcai_audioset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2412 2023-05-04 06:43:39.000000 hcai-datasets-nightly-0.1.7.dev202305040643/hcai_datasets/hcai_audioset/hcai_audioset.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-04 06:43:54.827663 hcai-datasets-nightly-0.1.7.dev202305040643/hcai_datasets/hcai_ckplus/
+-rw-r--r--   0 runner    (1001) docker     (122)       60 2023-05-04 06:43:39.000000 hcai-datasets-nightly-0.1.7.dev202305040643/hcai_datasets/hcai_ckplus/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3017 2023-05-04 06:43:39.000000 hcai-datasets-nightly-0.1.7.dev202305040643/hcai_datasets/hcai_ckplus/hcai_ckplus.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1940 2023-05-04 06:43:39.000000 hcai-datasets-nightly-0.1.7.dev202305040643/hcai_datasets/hcai_ckplus/hcai_ckplus_iterable.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-04 06:43:54.827663 hcai-datasets-nightly-0.1.7.dev202305040643/hcai_datasets/hcai_faces/
+-rw-r--r--   0 runner    (1001) docker     (122)       57 2023-05-04 06:43:39.000000 hcai-datasets-nightly-0.1.7.dev202305040643/hcai_datasets/hcai_faces/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3303 2023-05-04 06:43:39.000000 hcai-datasets-nightly-0.1.7.dev202305040643/hcai_datasets/hcai_faces/hcai_faces.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2051 2023-05-04 06:43:39.000000 hcai-datasets-nightly-0.1.7.dev202305040643/hcai_datasets/hcai_faces/hcai_faces_iterable.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-04 06:43:54.831663 hcai-datasets-nightly-0.1.7.dev202305040643/hcai_datasets/hcai_is2021_ess/
+-rw-r--r--   0 runner    (1001) docker     (122)       71 2023-05-04 06:43:39.000000 hcai-datasets-nightly-0.1.7.dev202305040643/hcai_datasets/hcai_is2021_ess/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2756 2023-05-04 06:43:39.000000 hcai-datasets-nightly-0.1.7.dev202305040643/hcai_datasets/hcai_is2021_ess/hcai_is2021_ess.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-04 06:43:54.831663 hcai-datasets-nightly-0.1.7.dev202305040643/hcai_datasets/hcai_librispeech/
+-rw-r--r--   0 runner    (1001) docker     (122)       75 2023-05-04 06:43:39.000000 hcai-datasets-nightly-0.1.7.dev202305040643/hcai_datasets/hcai_librispeech/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4323 2023-05-04 06:43:39.000000 hcai-datasets-nightly-0.1.7.dev202305040643/hcai_datasets/hcai_librispeech/hcai_librispeech.py
+-rw-r--r--   0 runner    (1001) docker     (122)      711 2023-05-04 06:43:39.000000 hcai-datasets-nightly-0.1.7.dev202305040643/hcai_datasets/hcai_librispeech/preprocessing.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-04 06:43:54.831663 hcai-datasets-nightly-0.1.7.dev202305040643/hcai_datasets/hcai_nova_dynamic/
+-rw-r--r--   0 runner    (1001) docker     (122)       83 2023-05-04 06:43:39.000000 hcai-datasets-nightly-0.1.7.dev202305040643/hcai_datasets/hcai_nova_dynamic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    20593 2023-05-04 06:43:39.000000 hcai-datasets-nightly-0.1.7.dev202305040643/hcai_datasets/hcai_nova_dynamic/hcai_nova_dynamic_iterable.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7686 2023-05-04 06:43:39.000000 hcai-datasets-nightly-0.1.7.dev202305040643/hcai_datasets/hcai_nova_dynamic/hcai_nova_dynamic_tfds.py
+-rw-r--r--   0 runner    (1001) docker     (122)    24935 2023-05-04 06:43:39.000000 hcai-datasets-nightly-0.1.7.dev202305040643/hcai_datasets/hcai_nova_dynamic/nova_db_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-04 06:43:54.831663 hcai-datasets-nightly-0.1.7.dev202305040643/hcai_datasets/hcai_nova_dynamic/utils/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-04 06:43:39.000000 hcai-datasets-nightly-0.1.7.dev202305040643/hcai_datasets/hcai_nova_dynamic/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12645 2023-05-04 06:43:39.000000 hcai-datasets-nightly-0.1.7.dev202305040643/hcai_datasets/hcai_nova_dynamic/utils/nova_anno_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13914 2023-05-04 06:43:39.000000 hcai-datasets-nightly-0.1.7.dev202305040643/hcai_datasets/hcai_nova_dynamic/utils/nova_data_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)      216 2023-05-04 06:43:39.000000 hcai-datasets-nightly-0.1.7.dev202305040643/hcai_datasets/hcai_nova_dynamic/utils/nova_string_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-04 06:43:54.831663 hcai-datasets-nightly-0.1.7.dev202305040643/hcai_datasets/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-04 06:43:39.000000 hcai-datasets-nightly-0.1.7.dev202305040643/hcai_datasets/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1198 2023-05-04 06:43:39.000000 hcai-datasets-nightly-0.1.7.dev202305040643/hcai_datasets/tests/dummy_set.py
+-rw-r--r--   0 runner    (1001) docker     (122)      600 2023-05-04 06:43:39.000000 hcai-datasets-nightly-0.1.7.dev202305040643/hcai_datasets/tests/test_bridge_pytorch.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-04 06:43:54.831663 hcai-datasets-nightly-0.1.7.dev202305040643/hcai_datasets_nightly.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     9089 2023-05-04 06:43:54.000000 hcai-datasets-nightly-0.1.7.dev202305040643/hcai_datasets_nightly.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     2439 2023-05-04 06:43:54.000000 hcai-datasets-nightly-0.1.7.dev202305040643/hcai_datasets_nightly.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-04 06:43:54.000000 hcai-datasets-nightly-0.1.7.dev202305040643/hcai_datasets_nightly.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      135 2023-05-04 06:43:54.000000 hcai-datasets-nightly-0.1.7.dev202305040643/hcai_datasets_nightly.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       33 2023-05-04 06:43:54.000000 hcai-datasets-nightly-0.1.7.dev202305040643/hcai_datasets_nightly.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      103 2023-05-04 06:43:39.000000 hcai-datasets-nightly-0.1.7.dev202305040643/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-05-04 06:43:54.831663 hcai-datasets-nightly-0.1.7.dev202305040643/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     2181 2023-05-04 06:43:39.000000 hcai-datasets-nightly-0.1.7.dev202305040643/setup.py
```

### Comparing `hcai-datasets-nightly-0.1.7.dev202304261438/PKG-INFO` & `hcai-datasets-nightly-0.1.7.dev202305040643/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hcai-datasets-nightly
-Version: 0.1.7.dev202304261438
+Version: 0.1.7.dev202305040643
 Summary: !Alpha Version! - This repository contains the backend server for the nova annotation ui (https://github.com/hcmlab/nova)
 Home-page: https://github.com/hcmlab/nova-server
 Author: Dominik Schiller
 Author-email: dominik.schiller@uni-a.de
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
```

### Comparing `hcai-datasets-nightly-0.1.7.dev202304261438/README.md` & `hcai-datasets-nightly-0.1.7.dev202305040643/README.md`

 * *Files identical despite different names*

### Comparing `hcai-datasets-nightly-0.1.7.dev202304261438/hcai_dataset_utils/bridge_pytorch.py` & `hcai-datasets-nightly-0.1.7.dev202305040643/hcai_dataset_utils/bridge_pytorch.py`

 * *Files identical despite different names*

### Comparing `hcai-datasets-nightly-0.1.7.dev202304261438/hcai_dataset_utils/bridge_tf.py` & `hcai-datasets-nightly-0.1.7.dev202305040643/hcai_dataset_utils/bridge_tf.py`

 * *Files identical despite different names*

### Comparing `hcai-datasets-nightly-0.1.7.dev202304261438/hcai_dataset_utils/import_validator.py` & `hcai-datasets-nightly-0.1.7.dev202305040643/hcai_dataset_utils/import_validator.py`

 * *Files identical despite different names*

### Comparing `hcai-datasets-nightly-0.1.7.dev202304261438/hcai_dataset_utils/pytorch_dataset_wrapper.py` & `hcai-datasets-nightly-0.1.7.dev202305040643/hcai_dataset_utils/pytorch_dataset_wrapper.py`

 * *Files identical despite different names*

### Comparing `hcai-datasets-nightly-0.1.7.dev202304261438/hcai_dataset_utils/statistics.py` & `hcai-datasets-nightly-0.1.7.dev202305040643/hcai_dataset_utils/statistics.py`

 * *Files identical despite different names*

### Comparing `hcai-datasets-nightly-0.1.7.dev202304261438/hcai_datasets/__init__.py` & `hcai-datasets-nightly-0.1.7.dev202305040643/hcai_datasets/__init__.py`

 * *Files identical despite different names*

### Comparing `hcai-datasets-nightly-0.1.7.dev202304261438/hcai_datasets/examples/example_affectnet_pytorch.py` & `hcai-datasets-nightly-0.1.7.dev202305040643/hcai_datasets/examples/example_affectnet_pytorch.py`

 * *Files identical despite different names*

### Comparing `hcai-datasets-nightly-0.1.7.dev202304261438/hcai_datasets/examples/example_affectnet_tensorflow_native.py` & `hcai-datasets-nightly-0.1.7.dev202305040643/hcai_datasets/examples/example_affectnet_tensorflow_native.py`

 * *Files identical despite different names*

### Comparing `hcai-datasets-nightly-0.1.7.dev202304261438/hcai_datasets/examples/example_affectnet_tfds.py` & `hcai-datasets-nightly-0.1.7.dev202305040643/hcai_datasets/examples/example_affectnet_tfds.py`

 * *Files identical despite different names*

### Comparing `hcai-datasets-nightly-0.1.7.dev202304261438/hcai_datasets/examples/example_ckplus_tensorflow_native.py` & `hcai-datasets-nightly-0.1.7.dev202305040643/hcai_datasets/examples/example_ckplus_tensorflow_native.py`

 * *Files identical despite different names*

### Comparing `hcai-datasets-nightly-0.1.7.dev202304261438/hcai_datasets/examples/example_ckplus_tfds.py` & `hcai-datasets-nightly-0.1.7.dev202305040643/hcai_datasets/examples/example_ckplus_tfds.py`

 * *Files identical despite different names*

### Comparing `hcai-datasets-nightly-0.1.7.dev202304261438/hcai_datasets/examples/example_faces_tensorflow_native.py` & `hcai-datasets-nightly-0.1.7.dev202305040643/hcai_datasets/examples/example_faces_tensorflow_native.py`

 * *Files identical despite different names*

### Comparing `hcai-datasets-nightly-0.1.7.dev202304261438/hcai_datasets/examples/example_faces_tfds.py` & `hcai-datasets-nightly-0.1.7.dev202305040643/hcai_datasets/examples/example_faces_tfds.py`

 * *Files identical despite different names*

### Comparing `hcai-datasets-nightly-0.1.7.dev202304261438/hcai_datasets/examples/example_nova_tensorflow_native.py` & `hcai-datasets-nightly-0.1.7.dev202305040643/hcai_datasets/examples/example_nova_tensorflow_native.py`

 * *Files identical despite different names*

### Comparing `hcai-datasets-nightly-0.1.7.dev202304261438/hcai_datasets/hcai_affectnet/Ignore_Lists/affect_net_ignore_list_duplicates.json` & `hcai-datasets-nightly-0.1.7.dev202305040643/hcai_datasets/hcai_affectnet/Ignore_Lists/affect_net_ignore_list_duplicates.json`

 * *Files identical despite different names*

### Comparing `hcai-datasets-nightly-0.1.7.dev202304261438/hcai_datasets/hcai_affectnet/Ignore_Lists/affect_net_ignore_list_wrong_format.json` & `hcai-datasets-nightly-0.1.7.dev202305040643/hcai_datasets/hcai_affectnet/Ignore_Lists/affect_net_ignore_list_wrong_format.json`

 * *Files identical despite different names*

### Comparing `hcai-datasets-nightly-0.1.7.dev202304261438/hcai_datasets/hcai_affectnet/hcai_affectnet.py` & `hcai-datasets-nightly-0.1.7.dev202305040643/hcai_datasets/hcai_affectnet/hcai_affectnet.py`

 * *Files identical despite different names*

### Comparing `hcai-datasets-nightly-0.1.7.dev202304261438/hcai_datasets/hcai_affectnet/hcai_affectnet_iterable.py` & `hcai-datasets-nightly-0.1.7.dev202305040643/hcai_datasets/hcai_affectnet/hcai_affectnet_iterable.py`

 * *Files identical despite different names*

### Comparing `hcai-datasets-nightly-0.1.7.dev202304261438/hcai_datasets/hcai_audioset/hcai_audioset.py` & `hcai-datasets-nightly-0.1.7.dev202305040643/hcai_datasets/hcai_audioset/hcai_audioset.py`

 * *Files identical despite different names*

### Comparing `hcai-datasets-nightly-0.1.7.dev202304261438/hcai_datasets/hcai_ckplus/hcai_ckplus.py` & `hcai-datasets-nightly-0.1.7.dev202305040643/hcai_datasets/hcai_ckplus/hcai_ckplus.py`

 * *Files identical despite different names*

### Comparing `hcai-datasets-nightly-0.1.7.dev202304261438/hcai_datasets/hcai_ckplus/hcai_ckplus_iterable.py` & `hcai-datasets-nightly-0.1.7.dev202305040643/hcai_datasets/hcai_ckplus/hcai_ckplus_iterable.py`

 * *Files identical despite different names*

### Comparing `hcai-datasets-nightly-0.1.7.dev202304261438/hcai_datasets/hcai_faces/hcai_faces.py` & `hcai-datasets-nightly-0.1.7.dev202305040643/hcai_datasets/hcai_faces/hcai_faces.py`

 * *Files identical despite different names*

### Comparing `hcai-datasets-nightly-0.1.7.dev202304261438/hcai_datasets/hcai_faces/hcai_faces_iterable.py` & `hcai-datasets-nightly-0.1.7.dev202305040643/hcai_datasets/hcai_faces/hcai_faces_iterable.py`

 * *Files identical despite different names*

### Comparing `hcai-datasets-nightly-0.1.7.dev202304261438/hcai_datasets/hcai_is2021_ess/hcai_is2021_ess.py` & `hcai-datasets-nightly-0.1.7.dev202305040643/hcai_datasets/hcai_is2021_ess/hcai_is2021_ess.py`

 * *Files identical despite different names*

### Comparing `hcai-datasets-nightly-0.1.7.dev202304261438/hcai_datasets/hcai_librispeech/hcai_librispeech.py` & `hcai-datasets-nightly-0.1.7.dev202305040643/hcai_datasets/hcai_librispeech/hcai_librispeech.py`

 * *Files identical despite different names*

### Comparing `hcai-datasets-nightly-0.1.7.dev202304261438/hcai_datasets/hcai_librispeech/preprocessing.py` & `hcai-datasets-nightly-0.1.7.dev202305040643/hcai_datasets/hcai_librispeech/preprocessing.py`

 * *Files identical despite different names*

### Comparing `hcai-datasets-nightly-0.1.7.dev202304261438/hcai_datasets/hcai_nova_dynamic/hcai_nova_dynamic_iterable.py` & `hcai-datasets-nightly-0.1.7.dev202305040643/hcai_datasets/hcai_nova_dynamic/hcai_nova_dynamic_iterable.py`

 * *Files identical despite different names*

### Comparing `hcai-datasets-nightly-0.1.7.dev202304261438/hcai_datasets/hcai_nova_dynamic/hcai_nova_dynamic_tfds.py` & `hcai-datasets-nightly-0.1.7.dev202305040643/hcai_datasets/hcai_nova_dynamic/hcai_nova_dynamic_tfds.py`

 * *Files identical despite different names*

### Comparing `hcai-datasets-nightly-0.1.7.dev202304261438/hcai_datasets/hcai_nova_dynamic/nova_db_handler.py` & `hcai-datasets-nightly-0.1.7.dev202305040643/hcai_datasets/hcai_nova_dynamic/nova_db_handler.py`

 * *Files identical despite different names*

### Comparing `hcai-datasets-nightly-0.1.7.dev202304261438/hcai_datasets/hcai_nova_dynamic/utils/nova_anno_utils.py` & `hcai-datasets-nightly-0.1.7.dev202305040643/hcai_datasets/hcai_nova_dynamic/utils/nova_anno_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -144,15 +144,15 @@
         # Create
         if self.dataframe.empty:
             self.data_interval = np.empty((0, 2), int)
             self.data_values = np.empty((0, 2), int)
         else:
             # Creating numpy array of annotations for fast access
             # Splitting the annotations into interval and data array
-            self.data_interval = self.dataframe[["from", "to"]].values.astype(np.int)
+            self.data_interval = self.dataframe[["from", "to"]].values.astype(int)
             self.data_values = self.dataframe[["id", "conf"]].values
 
     def get_label_for_frame_legacy(self, start, end):
 
         # If we don't have any data we return the garbage label
         if self.data == -1:
             return -1
@@ -247,15 +247,15 @@
         # Create
         if self.dataframe.empty:
             self.data_interval = np.empty((0, 2), int)
             self.data_values = np.empty((0, 2), int)
         else:
             # Creating numpy array of annotations for fast access
             # Splitting the annotations into interval and data array
-            self.data_interval = self.dataframe[["from", "to"]].values.astype(np.int)
+            self.data_interval = self.dataframe[["from", "to"]].values.astype(int)
             self.data_values = self.dataframe[["name", "conf"]].values
 
     def get_label_for_frame_legacy(self, start, end):
 
         # If we don't have any data we return the garbage label
         if self.data == -1:
             return -1
```

### Comparing `hcai-datasets-nightly-0.1.7.dev202304261438/hcai_datasets/hcai_nova_dynamic/utils/nova_data_utils.py` & `hcai-datasets-nightly-0.1.7.dev202305040643/hcai_datasets/hcai_nova_dynamic/utils/nova_data_utils.py`

 * *Files identical despite different names*

### Comparing `hcai-datasets-nightly-0.1.7.dev202304261438/hcai_datasets/tests/dummy_set.py` & `hcai-datasets-nightly-0.1.7.dev202305040643/hcai_datasets/tests/dummy_set.py`

 * *Files identical despite different names*

### Comparing `hcai-datasets-nightly-0.1.7.dev202304261438/hcai_datasets/tests/test_bridge_pytorch.py` & `hcai-datasets-nightly-0.1.7.dev202305040643/hcai_datasets/tests/test_bridge_pytorch.py`

 * *Files identical despite different names*

### Comparing `hcai-datasets-nightly-0.1.7.dev202304261438/hcai_datasets_nightly.egg-info/PKG-INFO` & `hcai-datasets-nightly-0.1.7.dev202305040643/hcai_datasets_nightly.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hcai-datasets-nightly
-Version: 0.1.7.dev202304261438
+Version: 0.1.7.dev202305040643
 Summary: !Alpha Version! - This repository contains the backend server for the nova annotation ui (https://github.com/hcmlab/nova)
 Home-page: https://github.com/hcmlab/nova-server
 Author: Dominik Schiller
 Author-email: dominik.schiller@uni-a.de
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
```

### Comparing `hcai-datasets-nightly-0.1.7.dev202304261438/hcai_datasets_nightly.egg-info/SOURCES.txt` & `hcai-datasets-nightly-0.1.7.dev202305040643/hcai_datasets_nightly.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hcai-datasets-nightly-0.1.7.dev202304261438/setup.py` & `hcai-datasets-nightly-0.1.7.dev202305040643/setup.py`

 * *Files identical despite different names*

