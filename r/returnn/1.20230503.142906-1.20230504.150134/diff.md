# Comparing `tmp/returnn-1.20230503.142906.tar.gz` & `tmp/returnn-1.20230504.150134.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/returnn-1.20230503.142906.tar", last modified: Wed May  3 12:54:14 2023, max compression
+gzip compressed data, was "dist/returnn-1.20230504.150134.tar", last modified: Thu May  4 13:26:23 2023, max compression
```

## Comparing `returnn-1.20230503.142906.tar` & `returnn-1.20230504.150134.tar`

### file list

```diff
@@ -1,438 +1,440 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:54:14.000000 returnn-1.20230503.142906/
--rw-r--r--   0 runner    (1001) docker     (123)      198 2023-05-03 12:53:53.000000 returnn-1.20230503.142906/.editorconfig
--rw-r--r--   0 runner    (1001) docker     (123)      526 2023-05-03 12:53:53.000000 returnn-1.20230503.142906/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      828 2023-05-03 12:53:53.000000 returnn-1.20230503.142906/.gitmodules
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-05-03 12:53:53.000000 returnn-1.20230503.142906/.kateconfig
--rw-r--r--   0 runner    (1001) docker     (123)     8556 2023-05-03 12:53:53.000000 returnn-1.20230503.142906/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)      704 2023-05-03 12:53:53.000000 returnn-1.20230503.142906/CODEOWNERS
--rw-r--r--   0 runner    (1001) docker     (123)     4880 2023-05-03 12:53:53.000000 returnn-1.20230503.142906/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)    10244 2023-05-03 12:53:53.000000 returnn-1.20230503.142906/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      579 2023-05-03 12:53:53.000000 returnn-1.20230503.142906/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4718 2023-05-03 12:54:14.000000 returnn-1.20230503.142906/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3573 2023-05-03 12:53:53.000000 returnn-1.20230503.142906/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1171 2023-05-03 12:53:53.000000 returnn-1.20230503.142906/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-05-03 12:54:14.000000 returnn-1.20230503.142906/_setup_info_generated.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:54:14.000000 returnn-1.20230503.142906/demos/
--rw-r--r--   0 runner    (1001) docker     (123)    36006 2023-05-03 12:53:53.000000 returnn-1.20230503.142906/demos/12AX.cluster_map
--rw-r--r--   0 runner    (1001) docker     (123)      476 2023-05-03 12:53:53.000000 returnn-1.20230503.142906/demos/_setup_returnn_env.py
--rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-05-03 12:53:53.000000 returnn-1.20230503.142906/demos/demo-fwd.config
--rw-r--r--   0 runner    (1001) docker     (123)     2703 2023-05-03 12:53:53.000000 returnn-1.20230503.142906/demos/demo-horovod-mpi.py
--rw-r--r--   0 runner    (1001) docker     (123)      520 2023-05-03 12:53:53.000000 returnn-1.20230503.142906/demos/demo-horovod-mpi.py.sh
--rwxr-xr-x   0 runner    (1001) docker     (123)      264 2023-05-03 12:53:53.000000 returnn-1.20230503.142906/demos/demo-horovod-mpi.sh
--rw-r--r--   0 runner    (1001) docker     (123)     1756 2023-05-03 12:53:53.000000 returnn-1.20230503.142906/demos/demo-hyper-param-tuning.config
--rwxr-xr-x   0 runner    (1001) docker     (123)     2396 2023-05-03 12:53:53.000000 returnn-1.20230503.142906/demos/demo-iter-dataset.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3635 2023-05-03 12:53:53.000000 returnn-1.20230503.142906/demos/demo-list-devices.py
--rw-r--r--   0 runner    (1001) docker     (123)     2848 2023-05-03 12:53:53.000000 returnn-1.20230503.142906/demos/demo-lua-torch-layer.config
--rw-r--r--   0 runner    (1001) docker     (123)      487 2023-05-03 12:53:53.000000 returnn-1.20230503.142906/demos/demo-pretrain.config
--rwxr-xr-x   0 runner    (1001) docker     (123)     2331 2023-05-03 12:53:53.000000 returnn-1.20230503.142906/demos/demo-record-and-push-to-webserver.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1950 2023-05-03 12:53:53.000000 returnn-1.20230503.142906/demos/demo-returnn-as-framework.py
--rw-r--r--   0 runner    (1001) docker     (123)     2708 2023-05-03 12:53:53.000000 returnn-1.20230503.142906/demos/demo-rf.config
--rw-r--r--   0 runner    (1001) docker     (123)     2331 2023-05-03 12:53:53.000000 returnn-1.20230503.142906/demos/demo-rhn-enwik8.config
--rwxr-xr-x   0 runner    (1001) docker     (123)     1378 2023-05-03 12:53:53.000000 returnn-1.20230503.142906/demos/demo-sprint-interface.py
--rw-r--r--   0 runner    (1001) docker     (123)     3147 2023-05-03 12:53:53.000000 returnn-1.20230503.142906/demos/demo-tf-att-copy.config
--rw-r--r--   0 runner    (1001) docker     (123)     2428 2023-05-03 12:53:53.000000 returnn-1.20230503.142906/demos/demo-tf-attention.config
--rw-r--r--   0 runner    (1001) docker     (123)     1481 2023-05-03 12:53:53.000000 returnn-1.20230503.142906/demos/demo-tf-chunking-blstm.12ax.config
--rw-r--r--   0 runner    (1001) docker     (123)     1416 2023-05-03 12:53:53.000000 returnn-1.20230503.142906/demos/demo-tf-contribrnn-lstm.12ax.config
--rw-r--r--   0 runner    (1001) docker     (123)     3073 2023-05-03 12:53:53.000000 returnn-1.20230503.142906/demos/demo-tf-enc-dec.config
--rwxr-xr-x   0 runner    (1001) docker     (123)    11615 2023-05-03 12:53:53.000000 returnn-1.20230503.142906/demos/demo-tf-hard-att-copy.config
--rwxr-xr-x   0 runner    (1001) docker     (123)     7287 2023-05-03 12:53:53.000000 returnn-1.20230503.142906/demos/demo-tf-lstm-benchmark.py
--rw-r--r--   0 runner    (1001) docker     (123)     1527 2023-05-03 12:53:53.000000 returnn-1.20230503.142906/demos/demo-tf-maxgradnorm-lstm.12ax.config
--rw-r--r--   0 runner    (1001) docker     (123)     1413 2023-05-03 12:53:53.000000 returnn-1.20230503.142906/demos/demo-tf-native-lstm-lowmem.12ax.config
--rw-r--r--   0 runner    (1001) docker     (123)     1576 2023-05-03 12:53:53.000000 returnn-1.20230503.142906/demos/demo-tf-native-lstm.12ax.config
--rw-r--r--   0 runner    (1001) docker     (123)     1768 2023-05-03 12:53:53.000000 returnn-1.20230503.142906/demos/demo-tf-native-lstm2.12ax.config
--rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-05-03 12:53:53.000000 returnn-1.20230503.142906/demos/demo-tf-native-lstm2.12ax.tuned.config
--rw-r--r--   0 runner    (1001) docker     (123)     1794 2023-05-03 12:53:53.000000 returnn-1.20230503.142906/demos/demo-tf-neural-transducer.12ax.config
--rw-r--r--   0 runner    (1001) docker     (123)     1825 2023-05-03 12:53:53.000000 returnn-1.20230503.142906/demos/demo-tf-rec-explicit-lstm.config
--rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-05-03 12:53:53.000000 returnn-1.20230503.142906/demos/demo-tf-rec-explicit-rnn.config
--rw-r--r--   0 runner    (1001) docker     (123)     2018 2023-05-03 12:53:53.000000 returnn-1.20230503.142906/demos/demo-tf-rec-self-att.config
--rw-r--r--   0 runner    (1001) docker     (123)     5188 2023-05-03 12:53:53.000000 returnn-1.20230503.142906/demos/demo-tf-search-compiled-graph.py
--rw-r--r--   0 runner    (1001) docker     (123)     1430 2023-05-03 12:53:53.000000 returnn-1.20230503.142906/demos/demo-tf-vanilla-lstm.12ax.config
--rw-r--r--   0 runner    (1001) docker     (123)     4818 2023-05-03 12:53:53.000000 returnn-1.20230503.142906/demos/demo-timit-lstm-ctc.config
--rw-r--r--   0 runner    (1001) docker     (123)     2521 2023-05-03 12:53:53.000000 returnn-1.20230503.142906/demos/demo-torch.config
--rw-r--r--   0 runner    (1001) docker     (123)      766 2023-05-03 12:53:53.000000 returnn-1.20230503.142906/demos/demo-upd-mult-model.lstm.12ax.config
--rwxr-xr-x   0 runner    (1001) docker     (123)      651 2023-05-03 12:53:53.000000 returnn-1.20230503.142906/demos/demo.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:54:14.000000 returnn-1.20230503.142906/demos/mdlstm/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:54:14.000000 returnn-1.20230503.142906/demos/mdlstm/IAM/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:54:14.000000 returnn-1.20230503.142906/demos/mdlstm/IAM/IAM_lines/
--rwxr-xr-x   0 runner    (1001) docker     (123)    43239 2023-05-03 12:53:53.000000 returnn-1.20230503.142906/demos/mdlstm/IAM/IAM_lines/a01-000u-00.png
--rwxr-xr-x   0 runner    (1001) docker     (123)    43552 2023-05-03 12:53:53.000000 returnn-1.20230503.142906/demos/mdlstm/IAM/IAM_lines/a01-007-04.png
--rwxr-xr-x   0 runner    (1001) docker     (123)    45111 2023-05-03 12:53:53.000000 returnn-1.20230503.142906/demos/mdlstm/IAM/IAM_lines/a01-007-06.png
--rw-r--r--   0 runner    (1001) docker     (123)     1709 2023-05-03 12:53:53.000000 returnn-1.20230503.142906/demos/mdlstm/IAM/README.txt
--rw-r--r--   0 runner    (1001) docker     (123)      158 2023-05-03 12:53:53.000000 returnn-1.20230503.142906/demos/mdlstm/IAM/chars.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1896 2023-05-03 12:53:53.000000 returnn-1.20230503.142906/demos/mdlstm/IAM/config_demo
--rw-r--r--   0 runner    (1001) docker     (123)     1981 2023-05-03 12:53:53.000000 returnn-1.20230503.142906/demos/mdlstm/IAM/config_fwd
--rw-r--r--   0 runner    (1001) docker     (123)     1983 2023-05-03 12:53:53.000000 returnn-1.20230503.142906/demos/mdlstm/IAM/config_real
--rwxr-xr-x   0 runner    (1001) docker     (123)    10194 2023-05-03 12:53:53.000000 returnn-1.20230503.142906/demos/mdlstm/IAM/create_IAM_dataset.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      749 2023-05-03 12:53:53.000000 returnn-1.20230503.142906/demos/mdlstm/IAM/decode.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:54:14.000000 returnn-1.20230503.142906/demos/mdlstm/IAM/features/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:54:14.000000 returnn-1.20230503.142906/demos/mdlstm/IAM/features/raw/
--rw-r--r--   0 runner    (1001) docker     (123)   248580 2023-05-03 12:53:53.000000 returnn-1.20230503.142906/demos/mdlstm/IAM/features/raw/demo.h5
--rwxr-xr-x   0 runner    (1001) docker     (123)       86 2023-05-03 12:53:53.000000 returnn-1.20230503.142906/demos/mdlstm/IAM/go.sh
--rw-r--r--   0 runner    (1001) docker     (123)      235 2023-05-03 12:53:53.000000 returnn-1.20230503.142906/demos/mdlstm/IAM/lines.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:54:14.000000 returnn-1.20230503.142906/demos/mdlstm/IAM/split/
--rw-r--r--   0 runner    (1001) docker     (123)     2712 2023-05-03 12:53:53.000000 returnn-1.20230503.142906/demos/mdlstm/IAM/split/eval.txt
--rw-r--r--   0 runner    (1001) docker     (123)    69536 2023-05-03 12:53:53.000000 returnn-1.20230503.142906/demos/mdlstm/IAM/split/train.txt
--rw-r--r--   0 runner    (1001) docker     (123)      934 2023-05-03 12:53:53.000000 returnn-1.20230503.142906/demos/mdlstm/IAM/split/valid.txt
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-05-03 12:53:53.000000 returnn-1.20230503.142906/demos/mdlstm/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:54:14.000000 returnn-1.20230503.142906/demos/mdlstm/artificial/
--rwxr-xr-x   0 runner    (1001) docker     (123)     2804 2023-05-03 12:53:53.000000 returnn-1.20230503.142906/demos/mdlstm/artificial/create_test_h5.py
--rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-05-03 12:53:53.000000 returnn-1.20230503.142906/demos/mdlstm/artificial/forwardconfig
--rwxr-xr-x   0 runner    (1001) docker     (123)      105 2023-05-03 12:53:53.000000 returnn-1.20230503.142906/demos/mdlstm/artificial/go.sh
--rw-r--r--   0 runner    (1001) docker     (123)      970 2023-05-03 12:53:53.000000 returnn-1.20230503.142906/demos/mdlstm/artificial/trainconfig
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:54:14.000000 returnn-1.20230503.142906/demos/mdlstm/artificial_rgb/
--rwxr-xr-x   0 runner    (1001) docker     (123)     2966 2023-05-03 12:53:53.000000 returnn-1.20230503.142906/demos/mdlstm/artificial_rgb/create_test_h5.py
--rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-05-03 12:53:53.000000 returnn-1.20230503.142906/demos/mdlstm/artificial_rgb/forwardconfig
--rwxr-xr-x   0 runner    (1001) docker     (123)      105 2023-05-03 12:53:53.000000 returnn-1.20230503.142906/demos/mdlstm/artificial_rgb/go.sh
--rw-r--r--   0 runner    (1001) docker     (123)      970 2023-05-03 12:53:53.000000 returnn-1.20230503.142906/demos/mdlstm/artificial_rgb/trainconfig
--rw-r--r--   0 runner    (1001) docker     (123)      463 2023-05-03 12:53:53.000000 returnn-1.20230503.142906/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-03 12:53:53.000000 returnn-1.20230503.142906/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:54:14.000000 returnn-1.20230503.142906/returnn/
--rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-05-03 12:53:53.000000 returnn-1.20230503.142906/returnn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24324 2023-05-03 12:53:53.000000 returnn-1.20230503.142906/returnn/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6981 2023-05-03 12:53:53.000000 returnn-1.20230503.142906/returnn/__old_mod_loader__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4659 2023-05-03 12:53:53.000000 returnn-1.20230503.142906/returnn/__setup__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24267 2023-05-03 12:53:53.000000 returnn-1.20230503.142906/returnn/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:54:14.000000 returnn-1.20230503.142906/returnn/datasets/
--rw-r--r--   0 runner    (1001) docker     (123)      390 2023-05-03 12:53:53.000000 returnn-1.20230503.142906/returnn/datasets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18032 2023-05-03 12:53:53.000000 returnn-1.20230503.142906/returnn/datasets/audio.py
--rw-r--r--   0 runner    (1001) docker     (123)    62931 2023-05-03 12:53:53.000000 returnn-1.20230503.142906/returnn/datasets/basic.py
--rw-r--r--   0 runner    (1001) docker     (123)     2388 2023-05-03 12:53:53.000000 returnn-1.20230503.142906/returnn/datasets/bundle_file.py
--rw-r--r--   0 runner    (1001) docker     (123)    24892 2023-05-03 12:53:53.000000 returnn-1.20230503.142906/returnn/datasets/cached.py
--rw-r--r--   0 runner    (1001) docker     (123)    11658 2023-05-03 12:53:53.000000 returnn-1.20230503.142906/returnn/datasets/cached2.py
--rw-r--r--   0 runner    (1001) docker     (123)    94213 2023-05-03 12:53:53.000000 returnn-1.20230503.142906/returnn/datasets/generating.py
--rw-r--r--   0 runner    (1001) docker     (123)    65113 2023-05-03 12:53:53.000000 returnn-1.20230503.142906/returnn/datasets/hdf.py
--rw-r--r--   0 runner    (1001) docker     (123)    85120 2023-05-03 12:53:53.000000 returnn-1.20230503.142906/returnn/datasets/lm.py
--rw-r--r--   0 runner    (1001) docker     (123)     9065 2023-05-03 12:53:53.000000 returnn-1.20230503.142906/returnn/datasets/map.py
--rw-r--r--   0 runner    (1001) docker     (123)    75821 2023-05-03 12:53:53.000000 returnn-1.20230503.142906/returnn/datasets/meta.py
--rw-r--r--   0 runner    (1001) docker     (123)    11167 2023-05-03 12:53:53.000000 returnn-1.20230503.142906/returnn/datasets/multi_proc.py
--rw-r--r--   0 runner    (1001) docker     (123)    14596 2023-05-03 12:53:53.000000 returnn-1.20230503.142906/returnn/datasets/normalization_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     5291 2023-05-03 12:53:53.000000 returnn-1.20230503.142906/returnn/datasets/numpy_dump.py
--rw-r--r--   0 runner    (1001) docker     (123)     9127 2023-05-03 12:53:53.000000 returnn-1.20230503.142906/returnn/datasets/raw_wav.py
--rw-r--r--   0 runner    (1001) docker     (123)    56015 2023-05-03 12:53:53.000000 returnn-1.20230503.142906/returnn/datasets/sprint.py
--rw-r--r--   0 runner    (1001) docker     (123)    17608 2023-05-03 12:53:53.000000 returnn-1.20230503.142906/returnn/datasets/stereo.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:54:14.000000 returnn-1.20230503.142906/returnn/datasets/util/
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-03 12:53:53.000000 returnn-1.20230503.142906/returnn/datasets/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23915 2023-05-03 12:53:53.000000 returnn-1.20230503.142906/returnn/datasets/util/feature_extraction.py
--rw-r--r--   0 runner    (1001) docker     (123)    20445 2023-05-03 12:53:53.000000 returnn-1.20230503.142906/returnn/datasets/util/vocabulary.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:54:14.000000 returnn-1.20230503.142906/returnn/engine/
--rw-r--r--   0 runner    (1001) docker     (123)      228 2023-05-03 12:53:53.000000 returnn-1.20230503.142906/returnn/engine/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9325 2023-05-03 12:53:53.000000 returnn-1.20230503.142906/returnn/engine/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     9912 2023-05-03 12:53:53.000000 returnn-1.20230503.142906/returnn/engine/batch.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:54:14.000000 returnn-1.20230503.142906/returnn/extern/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:54:14.000000 returnn-1.20230503.142906/returnn/extern/WarpRna/
--rw-r--r--   0 runner    (1001) docker     (123)     4005 2023-05-03 12:53:53.000000 returnn-1.20230503.142906/returnn/extern/WarpRna/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4024 2023-05-03 12:53:53.000000 returnn-1.20230503.142906/returnn/extern/WarpRna/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:54:14.000000 returnn-1.20230503.142906/returnn/extern/WarpRna/warp-rna/
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-05-03 12:53:54.000000 returnn-1.20230503.142906/returnn/extern/WarpRna/warp-rna/.git
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-03 12:53:57.000000 returnn-1.20230503.142906/returnn/extern/WarpRna/warp-rna/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-05-03 12:53:57.000000 returnn-1.20230503.142906/returnn/extern/WarpRna/warp-rna/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1448 2023-05-03 12:53:57.000000 returnn-1.20230503.142906/returnn/extern/WarpRna/warp-rna/README.md
--rw-r--r--   0 runner    (1001) docker     (123)    13770 2023-05-03 12:53:57.000000 returnn-1.20230503.142906/returnn/extern/WarpRna/warp-rna/aligner.gif
--rw-r--r--   0 runner    (1001) docker     (123)    51077 2023-05-03 12:53:57.000000 returnn-1.20230503.142906/returnn/extern/WarpRna/warp-rna/check.png
--rw-r--r--   0 runner    (1001) docker     (123)    11544 2023-05-03 12:53:57.000000 returnn-1.20230503.142906/returnn/extern/WarpRna/warp-rna/core.cu
--rw-r--r--   0 runner    (1001) docker     (123)      975 2023-05-03 12:53:57.000000 returnn-1.20230503.142906/returnn/extern/WarpRna/warp-rna/core.h
--rw-r--r--   0 runner    (1001) docker     (123)     2512 2023-05-03 12:53:57.000000 returnn-1.20230503.142906/returnn/extern/WarpRna/warp-rna/core_cpu.cpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:54:14.000000 returnn-1.20230503.142906/returnn/extern/WarpRna/warp-rna/pytorch_binding/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-05-03 12:53:57.000000 returnn-1.20230503.142906/returnn/extern/WarpRna/warp-rna/pytorch_binding/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-05-03 12:53:57.000000 returnn-1.20230503.142906/returnn/extern/WarpRna/warp-rna/pytorch_binding/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2089 2023-05-03 12:53:57.000000 returnn-1.20230503.142906/returnn/extern/WarpRna/warp-rna/pytorch_binding/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     3485 2023-05-03 12:53:57.000000 returnn-1.20230503.142906/returnn/extern/WarpRna/warp-rna/pytorch_binding/binding.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    11544 2023-05-03 12:53:57.000000 returnn-1.20230503.142906/returnn/extern/WarpRna/warp-rna/pytorch_binding/core.cu
--rw-r--r--   0 runner    (1001) docker     (123)      975 2023-05-03 12:53:57.000000 returnn-1.20230503.142906/returnn/extern/WarpRna/warp-rna/pytorch_binding/core.h
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-03 12:53:57.000000 returnn-1.20230503.142906/returnn/extern/WarpRna/warp-rna/pytorch_binding/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2079 2023-05-03 12:53:57.000000 returnn-1.20230503.142906/returnn/extern/WarpRna/warp-rna/pytorch_binding/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:54:14.000000 returnn-1.20230503.142906/returnn/extern/WarpRna/warp-rna/pytorch_binding/warp_rna/
--rw-r--r--   0 runner    (1001) docker     (123)     2885 2023-05-03 12:53:57.000000 returnn-1.20230503.142906/returnn/extern/WarpRna/warp-rna/pytorch_binding/warp_rna/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6961 2023-05-03 12:53:57.000000 returnn-1.20230503.142906/returnn/extern/WarpRna/warp-rna/pytorch_binding/warp_rna/test.py
--rw-r--r--   0 runner    (1001) docker     (123)     4141 2023-05-03 12:53:57.000000 returnn-1.20230503.142906/returnn/extern/WarpRna/warp-rna/ref_rna.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:54:14.000000 returnn-1.20230503.142906/returnn/extern/WarpRna/warp-rna/tensorflow_binding/
--rw-r--r--   0 runner    (1001) docker     (123)     6150 2023-05-03 12:53:57.000000 returnn-1.20230503.142906/returnn/extern/WarpRna/warp-rna/tensorflow_binding/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:54:14.000000 returnn-1.20230503.142906/returnn/extern/WarpRna/warp-rna/tensorflow_binding/src/
--rw-r--r--   0 runner    (1001) docker     (123)     1693 2023-05-03 12:53:57.000000 returnn-1.20230503.142906/returnn/extern/WarpRna/warp-rna/tensorflow_binding/src/warp_rna_op.cc
--rw-r--r--   0 runner    (1001) docker     (123)     6030 2023-05-03 12:53:57.000000 returnn-1.20230503.142906/returnn/extern/WarpRna/warp-rna/tensorflow_binding/src/warp_rna_op_kernel_tmpl.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:54:14.000000 returnn-1.20230503.142906/returnn/extern/WarpRna/warp-rna/tensorflow_binding/warp_rna/
--rw-r--r--   0 runner    (1001) docker     (123)     2076 2023-05-03 12:53:57.000000 returnn-1.20230503.142906/returnn/extern/WarpRna/warp-rna/tensorflow_binding/warp_rna/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4252 2023-05-03 12:53:57.000000 returnn-1.20230503.142906/returnn/extern/WarpRna/warp-rna/test.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      135 2023-05-03 12:53:53.000000 returnn-1.20230503.142906/returnn/extern/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:54:14.000000 returnn-1.20230503.142906/returnn/extern/graph_editor/
--rw-r--r--   0 runner    (1001) docker     (123)      257 2023-05-03 12:53:53.000000 returnn-1.20230503.142906/returnn/extern/graph_editor/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1239 2023-05-03 12:53:53.000000 returnn-1.20230503.142906/returnn/extern/graph_editor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8479 2023-05-03 12:53:53.000000 returnn-1.20230503.142906/returnn/extern/graph_editor/edit.py
--rw-r--r--   0 runner    (1001) docker     (123)    19826 2023-05-03 12:53:53.000000 returnn-1.20230503.142906/returnn/extern/graph_editor/reroute.py
--rw-r--r--   0 runner    (1001) docker     (123)    29772 2023-05-03 12:53:53.000000 returnn-1.20230503.142906/returnn/extern/graph_editor/select.py
--rw-r--r--   0 runner    (1001) docker     (123)    26578 2023-05-03 12:53:53.000000 returnn-1.20230503.142906/returnn/extern/graph_editor/subgraph.py
--rw-r--r--   0 runner    (1001) docker     (123)    30380 2023-05-03 12:53:53.000000 returnn-1.20230503.142906/returnn/extern/graph_editor/transform.py
--rw-r--r--   0 runner    (1001) docker     (123)    18727 2023-05-03 12:53:53.000000 returnn-1.20230503.142906/returnn/extern/graph_editor/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:54:14.000000 returnn-1.20230503.142906/returnn/frontend/
--rw-r--r--   0 runner    (1001) docker     (123)     1260 2023-05-03 12:53:53.000000 returnn-1.20230503.142906/returnn/frontend/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    36943 2023-05-03 12:53:53.000000 returnn-1.20230503.142906/returnn/frontend/_backend.py
--rw-r--r--   0 runner    (1001) docker     (123)     5125 2023-05-03 12:53:53.000000 returnn-1.20230503.142906/returnn/frontend/_numpy_backend.py
--rw-r--r--   0 runner    (1001) docker     (123)     5087 2023-05-03 12:53:53.000000 returnn-1.20230503.142906/returnn/frontend/_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    16971 2023-05-03 12:53:53.000000 returnn-1.20230503.142906/returnn/frontend/array_.py
--rw-r--r--   0 runner    (1001) docker     (123)    20833 2023-05-03 12:53:53.000000 returnn-1.20230503.142906/returnn/frontend/attention.py
--rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-05-03 12:53:53.000000 returnn-1.20230503.142906/returnn/frontend/cond.py
--rw-r--r--   0 runner    (1001) docker     (123)     2104 2023-05-03 12:53:53.000000 returnn-1.20230503.142906/returnn/frontend/const.py
--rw-r--r--   0 runner    (1001) docker     (123)     6015 2023-05-03 12:53:53.000000 returnn-1.20230503.142906/returnn/frontend/container.py
--rw-r--r--   0 runner    (1001) docker     (123)      413 2023-05-03 12:53:53.000000 returnn-1.20230503.142906/returnn/frontend/control_flow_ctx.py
--rw-r--r--   0 runner    (1001) docker     (123)    22357 2023-05-03 12:53:53.000000 returnn-1.20230503.142906/returnn/frontend/conv.py
--rw-r--r--   0 runner    (1001) docker     (123)      519 2023-05-03 12:53:53.000000 returnn-1.20230503.142906/returnn/frontend/device.py
--rw-r--r--   0 runner    (1001) docker     (123)     3538 2023-05-03 12:53:53.000000 returnn-1.20230503.142906/returnn/frontend/dims.py
--rw-r--r--   0 runner    (1001) docker     (123)     3334 2023-05-03 12:53:53.000000 returnn-1.20230503.142906/returnn/frontend/dropout.py
--rw-r--r--   0 runner    (1001) docker     (123)      964 2023-05-03 12:53:53.000000 returnn-1.20230503.142906/returnn/frontend/dtype.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:54:14.000000 returnn-1.20230503.142906/returnn/frontend/encoder/
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-03 12:53:53.000000 returnn-1.20230503.142906/returnn/frontend/encoder/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2109 2023-05-03 12:53:53.000000 returnn-1.20230503.142906/returnn/frontend/encoder/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    15428 2023-05-03 12:53:53.000000 returnn-1.20230503.142906/returnn/frontend/encoder/conformer.py
--rw-r--r--   0 runner    (1001) docker     (123)      330 2023-05-03 12:53:53.000000 returnn-1.20230503.142906/returnn/frontend/gradient.py
--rw-r--r--   0 runner    (1001) docker     (123)     5855 2023-05-03 12:53:53.000000 returnn-1.20230503.142906/returnn/frontend/init.py
--rw-r--r--   0 runner    (1001) docker     (123)     2147 2023-05-03 12:53:53.000000 returnn-1.20230503.142906/returnn/frontend/linear.py
--rw-r--r--   0 runner    (1001) docker     (123)      808 2023-05-03 12:53:53.000000 returnn-1.20230503.142906/returnn/frontend/loop.py
--rw-r--r--   0 runner    (1001) docker     (123)     1898 2023-05-03 12:53:53.000000 returnn-1.20230503.142906/returnn/frontend/loss.py
--rw-r--r--   0 runner    (1001) docker     (123)    13010 2023-05-03 12:53:53.000000 returnn-1.20230503.142906/returnn/frontend/math_.py
--rw-r--r--   0 runner    (1001) docker     (123)     1945 2023-05-03 12:53:53.000000 returnn-1.20230503.142906/returnn/frontend/matmul.py
--rw-r--r--   0 runner    (1001) docker     (123)     9877 2023-05-03 12:53:53.000000 returnn-1.20230503.142906/returnn/frontend/module.py
--rw-r--r--   0 runner    (1001) docker     (123)     8114 2023-05-03 12:53:53.000000 returnn-1.20230503.142906/returnn/frontend/normalization.py
--rw-r--r--   0 runner    (1001) docker     (123)     6143 2023-05-03 12:53:53.000000 returnn-1.20230503.142906/returnn/frontend/parameter.py
--rw-r--r--   0 runner    (1001) docker     (123)    10723 2023-05-03 12:53:53.000000 returnn-1.20230503.142906/returnn/frontend/rand.py
--rw-r--r--   0 runner    (1001) docker     (123)     2374 2023-05-03 12:53:53.000000 returnn-1.20230503.142906/returnn/frontend/rec.py
--rw-r--r--   0 runner    (1001) docker     (123)     4750 2023-05-03 12:53:53.000000 returnn-1.20230503.142906/returnn/frontend/reduce.py
--rw-r--r--   0 runner    (1001) docker     (123)    12200 2023-05-03 12:53:53.000000 returnn-1.20230503.142906/returnn/frontend/run_ctx.py
--rw-r--r--   0 runner    (1001) docker     (123)     9385 2023-05-03 12:53:53.000000 returnn-1.20230503.142906/returnn/frontend/signal.py
--rw-r--r--   0 runner    (1001) docker     (123)     2188 2023-05-03 12:53:53.000000 returnn-1.20230503.142906/returnn/frontend/state.py
--rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-05-03 12:53:53.000000 returnn-1.20230503.142906/returnn/frontend/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:54:14.000000 returnn-1.20230503.142906/returnn/import_/
--rw-r--r--   0 runner    (1001) docker     (123)      243 2023-05-03 12:53:53.000000 returnn-1.20230503.142906/returnn/import_/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8148 2023-05-03 12:53:53.000000 returnn-1.20230503.142906/returnn/import_/common.py
--rw-r--r--   0 runner    (1001) docker     (123)    13961 2023-05-03 12:53:53.000000 returnn-1.20230503.142906/returnn/import_/git.py
--rw-r--r--   0 runner    (1001) docker     (123)      798 2023-05-03 12:53:53.000000 returnn-1.20230503.142906/returnn/import_/import_.py
--rw-r--r--   0 runner    (1001) docker     (123)    33063 2023-05-03 12:53:53.000000 returnn-1.20230503.142906/returnn/learning_rate_control.py
--rw-r--r--   0 runner    (1001) docker     (123)    11738 2023-05-03 12:53:53.000000 returnn-1.20230503.142906/returnn/log.py
--rw-r--r--   0 runner    (1001) docker     (123)    35760 2023-05-03 12:53:53.000000 returnn-1.20230503.142906/returnn/native_op.cpp
--rw-r--r--   0 runner    (1001) docker     (123)   244393 2023-05-03 12:53:53.000000 returnn-1.20230503.142906/returnn/native_op.py
--rw-r--r--   0 runner    (1001) docker     (123)    23542 2023-05-03 12:53:53.000000 returnn-1.20230503.142906/returnn/pretrain.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:54:14.000000 returnn-1.20230503.142906/returnn/sprint/
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-05-03 12:53:53.000000 returnn-1.20230503.142906/returnn/sprint/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    31545 2023-05-03 12:53:53.000000 returnn-1.20230503.142906/returnn/sprint/cache.py
--rw-r--r--   0 runner    (1001) docker     (123)    31137 2023-05-03 12:53:53.000000 returnn-1.20230503.142906/returnn/sprint/control.py
--rw-r--r--   0 runner    (1001) docker     (123)    23313 2023-05-03 12:53:53.000000 returnn-1.20230503.142906/returnn/sprint/error_signals.py
--rw-r--r--   0 runner    (1001) docker     (123)    12305 2023-05-03 12:53:53.000000 returnn-1.20230503.142906/returnn/sprint/extern_interface.py
--rw-r--r--   0 runner    (1001) docker     (123)    36475 2023-05-03 12:53:53.000000 returnn-1.20230503.142906/returnn/sprint/interface.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:54:14.000000 returnn-1.20230503.142906/returnn/tensor/
--rw-r--r--   0 runner    (1001) docker     (123)      501 2023-05-03 12:53:53.000000 returnn-1.20230503.142906/returnn/tensor/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-05-03 12:53:53.000000 returnn-1.20230503.142906/returnn/tensor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    99004 2023-05-03 12:53:53.000000 returnn-1.20230503.142906/returnn/tensor/_dim_extra.py
--rw-r--r--   0 runner    (1001) docker     (123)   157144 2023-05-03 12:53:53.000000 returnn-1.20230503.142906/returnn/tensor/_tensor_extra.py
--rw-r--r--   0 runner    (1001) docker     (123)      643 2023-05-03 12:53:53.000000 returnn-1.20230503.142906/returnn/tensor/_tensor_mixin_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4890 2023-05-03 12:53:53.000000 returnn-1.20230503.142906/returnn/tensor/_tensor_op_overloads.py
--rw-r--r--   0 runner    (1001) docker     (123)     5125 2023-05-03 12:53:53.000000 returnn-1.20230503.142906/returnn/tensor/control_flow_ctx.py
--rw-r--r--   0 runner    (1001) docker     (123)     3884 2023-05-03 12:53:53.000000 returnn-1.20230503.142906/returnn/tensor/dim.py
--rw-r--r--   0 runner    (1001) docker     (123)     1884 2023-05-03 12:53:53.000000 returnn-1.20230503.142906/returnn/tensor/marked_dim.py
--rw-r--r--   0 runner    (1001) docker     (123)     7491 2023-05-03 12:53:53.000000 returnn-1.20230503.142906/returnn/tensor/tensor.py
--rw-r--r--   0 runner    (1001) docker     (123)     4187 2023-05-03 12:53:53.000000 returnn-1.20230503.142906/returnn/tensor/tensor_dict.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:54:14.000000 returnn-1.20230503.142906/returnn/tf/
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-05-03 12:53:53.000000 returnn-1.20230503.142906/returnn/tf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1632 2023-05-03 12:53:53.000000 returnn-1.20230503.142906/returnn/tf/compat.py
--rw-r--r--   0 runner    (1001) docker     (123)    36852 2023-05-03 12:53:53.000000 returnn-1.20230503.142906/returnn/tf/data_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (123)    15108 2023-05-03 12:53:53.000000 returnn-1.20230503.142906/returnn/tf/distributed.py
--rw-r--r--   0 runner    (1001) docker     (123)   151440 2023-05-03 12:53:53.000000 returnn-1.20230503.142906/returnn/tf/engine.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:54:14.000000 returnn-1.20230503.142906/returnn/tf/frontend_layers/
--rw-r--r--   0 runner    (1001) docker     (123)      455 2023-05-03 12:53:53.000000 returnn-1.20230503.142906/returnn/tf/frontend_layers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    37396 2023-05-03 12:53:53.000000 returnn-1.20230503.142906/returnn/tf/frontend_layers/_backend.py
--rw-r--r--   0 runner    (1001) docker     (123)     2626 2023-05-03 12:53:53.000000 returnn-1.20230503.142906/returnn/tf/frontend_layers/_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    10163 2023-05-03 12:53:53.000000 returnn-1.20230503.142906/returnn/tf/frontend_layers/cond.py
--rw-r--r--   0 runner    (1001) docker     (123)     4272 2023-05-03 12:53:53.000000 returnn-1.20230503.142906/returnn/tf/frontend_layers/config_entry_points.py
--rw-r--r--   0 runner    (1001) docker     (123)      888 2023-05-03 12:53:53.000000 returnn-1.20230503.142906/returnn/tf/frontend_layers/debug_eager_mode.py
--rw-r--r--   0 runner    (1001) docker     (123)     5712 2023-05-03 12:53:53.000000 returnn-1.20230503.142906/returnn/tf/frontend_layers/dims.py
--rw-r--r--   0 runner    (1001) docker     (123)    70144 2023-05-03 12:53:53.000000 returnn-1.20230503.142906/returnn/tf/frontend_layers/layer.py
--rw-r--r--   0 runner    (1001) docker     (123)    15516 2023-05-03 12:53:53.000000 returnn-1.20230503.142906/returnn/tf/frontend_layers/make_layer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2239 2023-05-03 12:53:53.000000 returnn-1.20230503.142906/returnn/tf/frontend_layers/prev_tensor_ref.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:54:14.000000 returnn-1.20230503.142906/returnn/tf/frontend_low_level/
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-05-03 12:53:53.000000 returnn-1.20230503.142906/returnn/tf/frontend_low_level/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20071 2023-05-03 12:53:53.000000 returnn-1.20230503.142906/returnn/tf/frontend_low_level/_backend.py
--rw-r--r--   0 runner    (1001) docker     (123)     5404 2023-05-03 12:53:53.000000 returnn-1.20230503.142906/returnn/tf/horovod.py
--rw-r--r--   0 runner    (1001) docker     (123)    31611 2023-05-03 12:53:53.000000 returnn-1.20230503.142906/returnn/tf/hyper_param_tuning.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:54:14.000000 returnn-1.20230503.142906/returnn/tf/layers/
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-05-03 12:53:53.000000 returnn-1.20230503.142906/returnn/tf/layers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   149447 2023-05-03 12:53:53.000000 returnn-1.20230503.142906/returnn/tf/layers/base.py
--rw-r--r--   0 runner    (1001) docker     (123)   590816 2023-05-03 12:53:53.000000 returnn-1.20230503.142906/returnn/tf/layers/basic.py
--rw-r--r--   0 runner    (1001) docker     (123)   539812 2023-05-03 12:53:53.000000 returnn-1.20230503.142906/returnn/tf/layers/rec.py
--rw-r--r--   0 runner    (1001) docker     (123)    21515 2023-05-03 12:53:53.000000 returnn-1.20230503.142906/returnn/tf/layers/segmental_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    52409 2023-05-03 12:53:53.000000 returnn-1.20230503.142906/returnn/tf/layers/signal_processing.py
--rw-r--r--   0 runner    (1001) docker     (123)    79733 2023-05-03 12:53:53.000000 returnn-1.20230503.142906/returnn/tf/native_op.py
--rw-r--r--   0 runner    (1001) docker     (123)   222320 2023-05-03 12:53:53.000000 returnn-1.20230503.142906/returnn/tf/network.py
--rw-r--r--   0 runner    (1001) docker     (123)     5471 2023-05-03 12:53:53.000000 returnn-1.20230503.142906/returnn/tf/sprint.py
--rw-r--r--   0 runner    (1001) docker     (123)    71410 2023-05-03 12:53:53.000000 returnn-1.20230503.142906/returnn/tf/updater.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:54:14.000000 returnn-1.20230503.142906/returnn/tf/util/
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-05-03 12:53:53.000000 returnn-1.20230503.142906/returnn/tf/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   293169 2023-05-03 12:53:53.000000 returnn-1.20230503.142906/returnn/tf/util/basic.py
--rw-r--r--   0 runner    (1001) docker     (123)    28839 2023-05-03 12:53:53.000000 returnn-1.20230503.142906/returnn/tf/util/data.py
--rw-r--r--   0 runner    (1001) docker     (123)    17333 2023-05-03 12:53:53.000000 returnn-1.20230503.142906/returnn/tf/util/ken_lm.py
--rw-r--r--   0 runner    (1001) docker     (123)    11277 2023-05-03 12:53:53.000000 returnn-1.20230503.142906/returnn/tf/util/open_fst.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:54:14.000000 returnn-1.20230503.142906/returnn/torch/
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-05-03 12:53:53.000000 returnn-1.20230503.142906/returnn/torch/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-03 12:53:53.000000 returnn-1.20230503.142906/returnn/torch/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:54:14.000000 returnn-1.20230503.142906/returnn/torch/data/
--rw-r--r--   0 runner    (1001) docker     (123)      132 2023-05-03 12:53:53.000000 returnn-1.20230503.142906/returnn/torch/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9483 2023-05-03 12:53:53.000000 returnn-1.20230503.142906/returnn/torch/data/pipeline.py
--rw-r--r--   0 runner    (1001) docker     (123)     5410 2023-05-03 12:53:53.000000 returnn-1.20230503.142906/returnn/torch/data/returnn_dataset_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)      970 2023-05-03 12:53:53.000000 returnn-1.20230503.142906/returnn/torch/data/tensor_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    22317 2023-05-03 12:53:53.000000 returnn-1.20230503.142906/returnn/torch/engine.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:54:14.000000 returnn-1.20230503.142906/returnn/torch/frontend/
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-05-03 12:53:53.000000 returnn-1.20230503.142906/returnn/torch/frontend/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    59306 2023-05-03 12:53:53.000000 returnn-1.20230503.142906/returnn/torch/frontend/_backend.py
--rw-r--r--   0 runner    (1001) docker     (123)     1830 2023-05-03 12:53:53.000000 returnn-1.20230503.142906/returnn/torch/frontend/_rand.py
--rw-r--r--   0 runner    (1001) docker     (123)     2714 2023-05-03 12:53:53.000000 returnn-1.20230503.142906/returnn/torch/frontend/bridge.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:54:14.000000 returnn-1.20230503.142906/returnn/torch/functional/
--rw-r--r--   0 runner    (1001) docker     (123)      193 2023-05-03 12:53:53.000000 returnn-1.20230503.142906/returnn/torch/functional/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-05-03 12:53:53.000000 returnn-1.20230503.142906/returnn/torch/functional/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10645 2023-05-03 12:53:53.000000 returnn-1.20230503.142906/returnn/torch/updater.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:54:14.000000 returnn-1.20230503.142906/returnn/util/
--rw-r--r--   0 runner    (1001) docker     (123)      336 2023-05-03 12:53:53.000000 returnn-1.20230503.142906/returnn/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   144924 2023-05-03 12:53:53.000000 returnn-1.20230503.142906/returnn/util/basic.py
--rw-r--r--   0 runner    (1001) docker     (123)    59572 2023-05-03 12:53:53.000000 returnn-1.20230503.142906/returnn/util/better_exchook.py
--rw-r--r--   0 runner    (1001) docker     (123)    17977 2023-05-03 12:53:53.000000 returnn-1.20230503.142906/returnn/util/bpe.py
--rw-r--r--   0 runner    (1001) docker     (123)    15987 2023-05-03 12:53:53.000000 returnn-1.20230503.142906/returnn/util/debug.py
--rw-r--r--   0 runner    (1001) docker     (123)     2905 2023-05-03 12:53:53.000000 returnn-1.20230503.142906/returnn/util/debug_helpers.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    59177 2023-05-03 12:53:53.000000 returnn-1.20230503.142906/returnn/util/fsa.py
--rw-r--r--   0 runner    (1001) docker     (123)     2009 2023-05-03 12:53:53.000000 returnn-1.20230503.142906/returnn/util/literal_py_to_pickle.py
--rw-r--r--   0 runner    (1001) docker     (123)     8131 2023-05-03 12:53:53.000000 returnn-1.20230503.142906/returnn/util/pprint.py
--rw-r--r--   0 runner    (1001) docker     (123)    14846 2023-05-03 12:53:53.000000 returnn-1.20230503.142906/returnn/util/py-to-pickle.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      277 2023-05-03 12:53:53.000000 returnn-1.20230503.142906/returnn/util/py_compat.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     7273 2023-05-03 12:53:53.000000 returnn-1.20230503.142906/returnn/util/sig_proc.py
--rw-r--r--   0 runner    (1001) docker     (123)    27230 2023-05-03 12:53:53.000000 returnn-1.20230503.142906/returnn/util/task_system.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:54:14.000000 returnn-1.20230503.142906/returnn.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4718 2023-05-03 12:54:14.000000 returnn-1.20230503.142906/returnn.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    12191 2023-05-03 12:54:14.000000 returnn-1.20230503.142906/returnn.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-03 12:54:14.000000 returnn-1.20230503.142906/returnn.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-03 12:54:14.000000 returnn-1.20230503.142906/returnn.egg-info/top_level.txt
--rwxr-xr-x   0 runner    (1001) docker     (123)      461 2023-05-03 12:53:53.000000 returnn-1.20230503.142906/rnn.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-03 12:54:14.000000 returnn-1.20230503.142906/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     4159 2023-05-03 12:53:53.000000 returnn-1.20230503.142906/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:54:14.000000 returnn-1.20230503.142906/tests/
--rwxr-xr-x   0 runner    (1001) docker     (123)     3392 2023-05-03 12:53:53.000000 returnn-1.20230503.142906/tests/DummySprintExec.py
--rw-r--r--   0 runner    (1001) docker     (123)     2671 2023-05-03 12:53:53.000000 returnn-1.20230503.142906/tests/PyCharm-inspection-profile.xml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:54:14.000000 returnn-1.20230503.142906/tests/PyCharm.idea/
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-03 12:53:53.000000 returnn-1.20230503.142906/tests/PyCharm.idea/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-03 12:53:53.000000 returnn-1.20230503.142906/tests/PyCharm.idea/.name
--rw-r--r--   0 runner    (1001) docker     (123)      512 2023-05-03 12:53:53.000000 returnn-1.20230503.142906/tests/PyCharm.idea/codeStyleSettings.xml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:54:14.000000 returnn-1.20230503.142906/tests/PyCharm.idea/codeStyles/
--rw-r--r--   0 runner    (1001) docker     (123)      328 2023-05-03 12:53:53.000000 returnn-1.20230503.142906/tests/PyCharm.idea/codeStyles/Project.xml
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-05-03 12:53:53.000000 returnn-1.20230503.142906/tests/PyCharm.idea/codeStyles/codeStyleConfig.xml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:54:14.000000 returnn-1.20230503.142906/tests/PyCharm.idea/inspectionProfiles/
--rw-r--r--   0 runner    (1001) docker     (123)     2671 2023-05-03 12:53:53.000000 returnn-1.20230503.142906/tests/PyCharm.idea/inspectionProfiles/Project_Default.xml
--rw-r--r--   0 runner    (1001) docker     (123)      181 2023-05-03 12:53:53.000000 returnn-1.20230503.142906/tests/PyCharm.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0 runner    (1001) docker     (123)      318 2023-05-03 12:53:53.000000 returnn-1.20230503.142906/tests/PyCharm.idea/misc.xml
--rw-r--r--   0 runner    (1001) docker     (123)      267 2023-05-03 12:53:53.000000 returnn-1.20230503.142906/tests/PyCharm.idea/modules.xml
--rw-r--r--   0 runner    (1001) docker     (123)      417 2023-05-03 12:53:53.000000 returnn-1.20230503.142906/tests/PyCharm.idea/returnn.iml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:54:14.000000 returnn-1.20230503.142906/tests/PyCharm.idea/scopes/
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-05-03 12:53:53.000000 returnn-1.20230503.142906/tests/PyCharm.idea/scopes/scope_settings.xml
--rw-r--r--   0 runner    (1001) docker     (123)      871 2023-05-03 12:53:53.000000 returnn-1.20230503.142906/tests/_set_num_threads1.py
--rw-r--r--   0 runner    (1001) docker     (123)      476 2023-05-03 12:53:53.000000 returnn-1.20230503.142906/tests/_setup_returnn_env.py
--rw-r--r--   0 runner    (1001) docker     (123)     8833 2023-05-03 12:53:53.000000 returnn-1.20230503.142906/tests/_setup_test_env.py
--rw-r--r--   0 runner    (1001) docker     (123)      794 2023-05-03 12:53:53.000000 returnn-1.20230503.142906/tests/bpe-unicode-demo.codes
--rw-r--r--   0 runner    (1001) docker     (123)     2205 2023-05-03 12:53:53.000000 returnn-1.20230503.142906/tests/bpe-unicode-demo.vocab
--rw-r--r--   0 runner    (1001) docker     (123)      386 2023-05-03 12:53:53.000000 returnn-1.20230503.142906/tests/lexicon_opt.fst
--rw-r--r--   0 runner    (1001) docker     (123)      520 2023-05-03 12:53:53.000000 returnn-1.20230503.142906/tests/lexicon_opt.isyms
--rw-r--r--   0 runner    (1001) docker     (123)    34282 2023-05-03 12:53:53.000000 returnn-1.20230503.142906/tests/lexicon_opt.jpg
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-03 12:53:53.000000 returnn-1.20230503.142906/tests/lexicon_opt.osyms
--rw-r--r--   0 runner    (1001) docker     (123)     6880 2023-05-03 12:53:53.000000 returnn-1.20230503.142906/tests/lint_common.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    29203 2023-05-03 12:53:53.000000 returnn-1.20230503.142906/tests/pycharm-inspect.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2960 2023-05-03 12:53:53.000000 returnn-1.20230503.142906/tests/pylint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2963 2023-05-03 12:53:53.000000 returnn-1.20230503.142906/tests/returnn-as-framework.py
--rw-r--r--   0 runner    (1001) docker     (123)    11010 2023-05-03 12:53:53.000000 returnn-1.20230503.142906/tests/rf_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      617 2023-05-03 12:53:53.000000 returnn-1.20230503.142906/tests/spelling.dic
--rw-r--r--   0 runner    (1001) docker     (123)     7845 2023-05-03 12:53:53.000000 returnn-1.20230503.142906/tests/test_Config.py
--rw-r--r--   0 runner    (1001) docker     (123)    18921 2023-05-03 12:53:53.000000 returnn-1.20230503.142906/tests/test_Dataset.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    13634 2023-05-03 12:53:53.000000 returnn-1.20230503.142906/tests/test_Fsa.py
--rw-r--r--   0 runner    (1001) docker     (123)     8904 2023-05-03 12:53:53.000000 returnn-1.20230503.142906/tests/test_GeneratingDataset.py
--rw-r--r--   0 runner    (1001) docker     (123)    32796 2023-05-03 12:53:53.000000 returnn-1.20230503.142906/tests/test_HDFDataset.py
--rw-r--r--   0 runner    (1001) docker     (123)    10326 2023-05-03 12:53:53.000000 returnn-1.20230503.142906/tests/test_LearningRateControl.py
--rw-r--r--   0 runner    (1001) docker     (123)     7187 2023-05-03 12:53:53.000000 returnn-1.20230503.142906/tests/test_Log.py
--rw-r--r--   0 runner    (1001) docker     (123)     3635 2023-05-03 12:53:53.000000 returnn-1.20230503.142906/tests/test_MultiProcDataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     3333 2023-05-03 12:53:53.000000 returnn-1.20230503.142906/tests/test_PTDataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     2465 2023-05-03 12:53:53.000000 returnn-1.20230503.142906/tests/test_Pretrain.py
--rw-r--r--   0 runner    (1001) docker     (123)    21403 2023-05-03 12:53:53.000000 returnn-1.20230503.142906/tests/test_ResNet.py
--rw-r--r--   0 runner    (1001) docker     (123)     5014 2023-05-03 12:53:53.000000 returnn-1.20230503.142906/tests/test_SprintDataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     3330 2023-05-03 12:53:53.000000 returnn-1.20230503.142906/tests/test_SprintInterface.py
--rw-r--r--   0 runner    (1001) docker     (123)   238053 2023-05-03 12:53:53.000000 returnn-1.20230503.142906/tests/test_TFEngine.py
--rw-r--r--   0 runner    (1001) docker     (123)   135453 2023-05-03 12:53:53.000000 returnn-1.20230503.142906/tests/test_TFNativeOp.py
--rw-r--r--   0 runner    (1001) docker     (123)   551303 2023-05-03 12:53:53.000000 returnn-1.20230503.142906/tests/test_TFNetworkLayer.py
--rw-r--r--   0 runner    (1001) docker     (123)   549696 2023-05-03 12:53:53.000000 returnn-1.20230503.142906/tests/test_TFNetworkRecLayer.py
--rw-r--r--   0 runner    (1001) docker     (123)    14485 2023-05-03 12:53:53.000000 returnn-1.20230503.142906/tests/test_TFNetworkSigProcLayer.py
--rw-r--r--   0 runner    (1001) docker     (123)    20440 2023-05-03 12:53:53.000000 returnn-1.20230503.142906/tests/test_TFUpdater.py
--rw-r--r--   0 runner    (1001) docker     (123)   187644 2023-05-03 12:53:53.000000 returnn-1.20230503.142906/tests/test_TFUtil.py
--rw-r--r--   0 runner    (1001) docker     (123)     3082 2023-05-03 12:53:53.000000 returnn-1.20230503.142906/tests/test_TF_determinism.py
--rw-r--r--   0 runner    (1001) docker     (123)     2156 2023-05-03 12:53:53.000000 returnn-1.20230503.142906/tests/test_TaskSystem.py
--rw-r--r--   0 runner    (1001) docker     (123)     5088 2023-05-03 12:53:53.000000 returnn-1.20230503.142906/tests/test_TaskSystem_SharedMem.py
--rw-r--r--   0 runner    (1001) docker     (123)     9378 2023-05-03 12:53:53.000000 returnn-1.20230503.142906/tests/test_TranslationDataset.py
--rw-r--r--   0 runner    (1001) docker     (123)    14944 2023-05-03 12:53:53.000000 returnn-1.20230503.142906/tests/test_Util.py
--rw-r--r--   0 runner    (1001) docker     (123)    10578 2023-05-03 12:53:53.000000 returnn-1.20230503.142906/tests/test_demos.py
--rw-r--r--   0 runner    (1001) docker     (123)     7375 2023-05-03 12:53:53.000000 returnn-1.20230503.142906/tests/test_fork_exec.py
--rw-r--r--   0 runner    (1001) docker     (123)     2893 2023-05-03 12:53:53.000000 returnn-1.20230503.142906/tests/test_hdf_dump.py
--rw-r--r--   0 runner    (1001) docker     (123)     4725 2023-05-03 12:53:53.000000 returnn-1.20230503.142906/tests/test_rf_array.py
--rw-r--r--   0 runner    (1001) docker     (123)     4491 2023-05-03 12:53:53.000000 returnn-1.20230503.142906/tests/test_rf_attention.py
--rw-r--r--   0 runner    (1001) docker     (123)     6405 2023-05-03 12:53:53.000000 returnn-1.20230503.142906/tests/test_rf_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     5321 2023-05-03 12:53:53.000000 returnn-1.20230503.142906/tests/test_rf_cond.py
--rw-r--r--   0 runner    (1001) docker     (123)     4591 2023-05-03 12:53:53.000000 returnn-1.20230503.142906/tests/test_rf_container.py
--rw-r--r--   0 runner    (1001) docker     (123)    10228 2023-05-03 12:53:53.000000 returnn-1.20230503.142906/tests/test_rf_conv.py
--rw-r--r--   0 runner    (1001) docker     (123)     1963 2023-05-03 12:53:53.000000 returnn-1.20230503.142906/tests/test_rf_encoder_conformer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2312 2023-05-03 12:53:53.000000 returnn-1.20230503.142906/tests/test_rf_math.py
--rw-r--r--   0 runner    (1001) docker     (123)     1127 2023-05-03 12:53:53.000000 returnn-1.20230503.142906/tests/test_rf_normalization.py
--rw-r--r--   0 runner    (1001) docker     (123)     1772 2023-05-03 12:53:53.000000 returnn-1.20230503.142906/tests/test_rf_rec.py
--rw-r--r--   0 runner    (1001) docker     (123)     1052 2023-05-03 12:53:53.000000 returnn-1.20230503.142906/tests/test_rf_signal.py
--rw-r--r--   0 runner    (1001) docker     (123)     1135 2023-05-03 12:53:53.000000 returnn-1.20230503.142906/tests/test_tensor.py
--rw-r--r--   0 runner    (1001) docker     (123)     8435 2023-05-03 12:53:53.000000 returnn-1.20230503.142906/tests/test_tools.py
--rw-r--r--   0 runner    (1001) docker     (123)    15594 2023-05-03 12:53:53.000000 returnn-1.20230503.142906/tests/test_torch_frontend.py
--rw-r--r--   0 runner    (1001) docker     (123)    15534 2023-05-03 12:53:53.000000 returnn-1.20230503.142906/tests/test_torch_internal_frontend.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:54:14.000000 returnn-1.20230503.142906/tools/
--rw-r--r--   0 runner    (1001) docker     (123)      476 2023-05-03 12:53:53.000000 returnn-1.20230503.142906/tools/_setup_returnn_env.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     9650 2023-05-03 12:53:53.000000 returnn-1.20230503.142906/tools/analyze-dataset-batches.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3943 2023-05-03 12:53:53.000000 returnn-1.20230503.142906/tools/bliss-collect-seq-lens.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      780 2023-05-03 12:53:53.000000 returnn-1.20230503.142906/tools/bliss-dump-text.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6608 2023-05-03 12:53:53.000000 returnn-1.20230503.142906/tools/bliss-get-segment-names.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    18221 2023-05-03 12:53:53.000000 returnn-1.20230503.142906/tools/bliss-to-ogg-zip.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5644 2023-05-03 12:53:53.000000 returnn-1.20230503.142906/tools/bpe-create-lexicon.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    10532 2023-05-03 12:53:53.000000 returnn-1.20230503.142906/tools/calculate-word-error-rate.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1759 2023-05-03 12:53:53.000000 returnn-1.20230503.142906/tools/cleanup-old-models.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    10783 2023-05-03 12:53:53.000000 returnn-1.20230503.142906/tools/collect-orth-symbols.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6801 2023-05-03 12:53:53.000000 returnn-1.20230503.142906/tools/collect-words.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4395 2023-05-03 12:53:53.000000 returnn-1.20230503.142906/tools/compile_native_op.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    81620 2023-05-03 12:53:53.000000 returnn-1.20230503.142906/tools/compile_tf_graph.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     8500 2023-05-03 12:53:53.000000 returnn-1.20230503.142906/tools/debug-dump-search-scores.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    47001 2023-05-03 12:53:53.000000 returnn-1.20230503.142906/tools/debug-plot-search-scores.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6048 2023-05-03 12:53:53.000000 returnn-1.20230503.142906/tools/dump-dataset-raw-strings.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    12524 2023-05-03 12:53:53.000000 returnn-1.20230503.142906/tools/dump-dataset.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5770 2023-05-03 12:53:53.000000 returnn-1.20230503.142906/tools/dump-forward-stats.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2576 2023-05-03 12:53:53.000000 returnn-1.20230503.142906/tools/dump-forward.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1596 2023-05-03 12:53:53.000000 returnn-1.20230503.142906/tools/dump-network-json.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      719 2023-05-03 12:53:53.000000 returnn-1.20230503.142906/tools/dump-pickle.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    16425 2023-05-03 12:53:53.000000 returnn-1.20230503.142906/tools/extract_state_tying_from_dataset.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    14986 2023-05-03 12:53:53.000000 returnn-1.20230503.142906/tools/get-attention-weights.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2936 2023-05-03 12:53:53.000000 returnn-1.20230503.142906/tools/get-best-model-epoch.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3900 2023-05-03 12:53:53.000000 returnn-1.20230503.142906/tools/hdf_dump.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    19622 2023-05-03 12:53:53.000000 returnn-1.20230503.142906/tools/hdf_dump_translation_dataset.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    49563 2023-05-03 12:53:53.000000 returnn-1.20230503.142906/tools/import-blocks-mt-model.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    31498 2023-05-03 12:53:53.000000 returnn-1.20230503.142906/tools/import-t2t-mt-model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:54:14.000000 returnn-1.20230503.142906/tools/lattice_rescorer/
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-03 12:53:53.000000 returnn-1.20230503.142906/tools/lattice_rescorer/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     2254 2023-05-03 12:53:53.000000 returnn-1.20230503.142906/tools/lattice_rescorer/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     7825 2023-05-03 12:53:53.000000 returnn-1.20230503.142906/tools/lattice_rescorer/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:54:14.000000 returnn-1.20230503.142906/tools/lattice_rescorer/example/
--rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-05-03 12:53:53.000000 returnn-1.20230503.142906/tools/lattice_rescorer/example/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-05-03 12:53:53.000000 returnn-1.20230503.142906/tools/lattice_rescorer/example/libs_list
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:54:14.000000 returnn-1.20230503.142906/tools/lattice_rescorer/example/network.040/
--rw-r--r--   0 runner    (1001) docker     (123)     5775 2023-05-03 12:53:53.000000 returnn-1.20230503.142906/tools/lattice_rescorer/example/network.040/i600_m600_m600.sgd_b16_lr0_cl2.newbobabs.config
--rw-r--r--   0 runner    (1001) docker     (123)     6110 2023-05-03 12:53:53.000000 returnn-1.20230503.142906/tools/lattice_rescorer/example/network.040/i600_m600_m600.sgd_b16_lr0_cl2.newbobabs.keep_over_epoch.lstm2.config
--rwxr-xr-x   0 runner    (1001) docker     (123)      800 2023-05-03 12:53:53.000000 returnn-1.20230503.142906/tools/lattice_rescorer/example/rescore_lattice.sh
--rw-r--r--   0 runner    (1001) docker     (123)      296 2023-05-03 12:53:53.000000 returnn-1.20230503.142906/tools/lattice_rescorer/example/state_vars_list
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-05-03 12:53:53.000000 returnn-1.20230503.142906/tools/lattice_rescorer/example/tensor_names_list
--rw-r--r--   0 runner    (1001) docker     (123)     1687 2023-05-03 12:53:53.000000 returnn-1.20230503.142906/tools/lattice_rescorer/file.h
--rw-r--r--   0 runner    (1001) docker     (123)    26055 2023-05-03 12:53:53.000000 returnn-1.20230503.142906/tools/lattice_rescorer/htklatticerescorer.cc
--rw-r--r--   0 runner    (1001) docker     (123)    10856 2023-05-03 12:53:53.000000 returnn-1.20230503.142906/tools/lattice_rescorer/htklatticerescorer.h
--rw-r--r--   0 runner    (1001) docker     (123)    12488 2023-05-03 12:53:53.000000 returnn-1.20230503.142906/tools/lattice_rescorer/main.cc
--rw-r--r--   0 runner    (1001) docker     (123)     2184 2023-05-03 12:53:53.000000 returnn-1.20230503.142906/tools/lattice_rescorer/rescorer.h
--rw-r--r--   0 runner    (1001) docker     (123)     5563 2023-05-03 12:53:53.000000 returnn-1.20230503.142906/tools/lattice_rescorer/vocabulary.cc
--rw-r--r--   0 runner    (1001) docker     (123)     3023 2023-05-03 12:53:53.000000 returnn-1.20230503.142906/tools/lattice_rescorer/vocabulary.h
--rwxr-xr-x   0 runner    (1001) docker     (123)     5438 2023-05-03 12:53:53.000000 returnn-1.20230503.142906/tools/tf_avg_checkpoints.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6269 2023-05-03 12:53:53.000000 returnn-1.20230503.142906/tools/tf_inspect_checkpoint.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1288 2023-05-03 12:53:53.000000 returnn-1.20230503.142906/tools/tf_inspect_summary_log.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:26:23.000000 returnn-1.20230504.150134/
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-05-04 13:26:04.000000 returnn-1.20230504.150134/.editorconfig
+-rw-r--r--   0 runner    (1001) docker     (123)      526 2023-05-04 13:26:04.000000 returnn-1.20230504.150134/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      828 2023-05-04 13:26:04.000000 returnn-1.20230504.150134/.gitmodules
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-05-04 13:26:04.000000 returnn-1.20230504.150134/.kateconfig
+-rw-r--r--   0 runner    (1001) docker     (123)     8556 2023-05-04 13:26:04.000000 returnn-1.20230504.150134/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)      704 2023-05-04 13:26:04.000000 returnn-1.20230504.150134/CODEOWNERS
+-rw-r--r--   0 runner    (1001) docker     (123)     4880 2023-05-04 13:26:04.000000 returnn-1.20230504.150134/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)    10244 2023-05-04 13:26:04.000000 returnn-1.20230504.150134/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      579 2023-05-04 13:26:04.000000 returnn-1.20230504.150134/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4718 2023-05-04 13:26:23.000000 returnn-1.20230504.150134/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3573 2023-05-04 13:26:04.000000 returnn-1.20230504.150134/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1171 2023-05-04 13:26:04.000000 returnn-1.20230504.150134/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-05-04 13:26:23.000000 returnn-1.20230504.150134/_setup_info_generated.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:26:23.000000 returnn-1.20230504.150134/demos/
+-rw-r--r--   0 runner    (1001) docker     (123)    36006 2023-05-04 13:26:04.000000 returnn-1.20230504.150134/demos/12AX.cluster_map
+-rw-r--r--   0 runner    (1001) docker     (123)      476 2023-05-04 13:26:04.000000 returnn-1.20230504.150134/demos/_setup_returnn_env.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-05-04 13:26:04.000000 returnn-1.20230504.150134/demos/demo-fwd.config
+-rw-r--r--   0 runner    (1001) docker     (123)     2703 2023-05-04 13:26:04.000000 returnn-1.20230504.150134/demos/demo-horovod-mpi.py
+-rw-r--r--   0 runner    (1001) docker     (123)      520 2023-05-04 13:26:04.000000 returnn-1.20230504.150134/demos/demo-horovod-mpi.py.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)      264 2023-05-04 13:26:04.000000 returnn-1.20230504.150134/demos/demo-horovod-mpi.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     1756 2023-05-04 13:26:04.000000 returnn-1.20230504.150134/demos/demo-hyper-param-tuning.config
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2396 2023-05-04 13:26:04.000000 returnn-1.20230504.150134/demos/demo-iter-dataset.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3635 2023-05-04 13:26:04.000000 returnn-1.20230504.150134/demos/demo-list-devices.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2848 2023-05-04 13:26:04.000000 returnn-1.20230504.150134/demos/demo-lua-torch-layer.config
+-rw-r--r--   0 runner    (1001) docker     (123)      487 2023-05-04 13:26:04.000000 returnn-1.20230504.150134/demos/demo-pretrain.config
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2331 2023-05-04 13:26:04.000000 returnn-1.20230504.150134/demos/demo-record-and-push-to-webserver.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1950 2023-05-04 13:26:04.000000 returnn-1.20230504.150134/demos/demo-returnn-as-framework.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2708 2023-05-04 13:26:04.000000 returnn-1.20230504.150134/demos/demo-rf.config
+-rw-r--r--   0 runner    (1001) docker     (123)     2331 2023-05-04 13:26:04.000000 returnn-1.20230504.150134/demos/demo-rhn-enwik8.config
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1378 2023-05-04 13:26:04.000000 returnn-1.20230504.150134/demos/demo-sprint-interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3147 2023-05-04 13:26:04.000000 returnn-1.20230504.150134/demos/demo-tf-att-copy.config
+-rw-r--r--   0 runner    (1001) docker     (123)     2428 2023-05-04 13:26:04.000000 returnn-1.20230504.150134/demos/demo-tf-attention.config
+-rw-r--r--   0 runner    (1001) docker     (123)     1481 2023-05-04 13:26:04.000000 returnn-1.20230504.150134/demos/demo-tf-chunking-blstm.12ax.config
+-rw-r--r--   0 runner    (1001) docker     (123)     1416 2023-05-04 13:26:04.000000 returnn-1.20230504.150134/demos/demo-tf-contribrnn-lstm.12ax.config
+-rw-r--r--   0 runner    (1001) docker     (123)     3073 2023-05-04 13:26:04.000000 returnn-1.20230504.150134/demos/demo-tf-enc-dec.config
+-rwxr-xr-x   0 runner    (1001) docker     (123)    11615 2023-05-04 13:26:04.000000 returnn-1.20230504.150134/demos/demo-tf-hard-att-copy.config
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7287 2023-05-04 13:26:04.000000 returnn-1.20230504.150134/demos/demo-tf-lstm-benchmark.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1527 2023-05-04 13:26:04.000000 returnn-1.20230504.150134/demos/demo-tf-maxgradnorm-lstm.12ax.config
+-rw-r--r--   0 runner    (1001) docker     (123)     1413 2023-05-04 13:26:04.000000 returnn-1.20230504.150134/demos/demo-tf-native-lstm-lowmem.12ax.config
+-rw-r--r--   0 runner    (1001) docker     (123)     1576 2023-05-04 13:26:04.000000 returnn-1.20230504.150134/demos/demo-tf-native-lstm.12ax.config
+-rw-r--r--   0 runner    (1001) docker     (123)     1768 2023-05-04 13:26:04.000000 returnn-1.20230504.150134/demos/demo-tf-native-lstm2.12ax.config
+-rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-05-04 13:26:04.000000 returnn-1.20230504.150134/demos/demo-tf-native-lstm2.12ax.tuned.config
+-rw-r--r--   0 runner    (1001) docker     (123)     1794 2023-05-04 13:26:04.000000 returnn-1.20230504.150134/demos/demo-tf-neural-transducer.12ax.config
+-rw-r--r--   0 runner    (1001) docker     (123)     1825 2023-05-04 13:26:04.000000 returnn-1.20230504.150134/demos/demo-tf-rec-explicit-lstm.config
+-rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-05-04 13:26:04.000000 returnn-1.20230504.150134/demos/demo-tf-rec-explicit-rnn.config
+-rw-r--r--   0 runner    (1001) docker     (123)     2018 2023-05-04 13:26:04.000000 returnn-1.20230504.150134/demos/demo-tf-rec-self-att.config
+-rw-r--r--   0 runner    (1001) docker     (123)     5188 2023-05-04 13:26:04.000000 returnn-1.20230504.150134/demos/demo-tf-search-compiled-graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1430 2023-05-04 13:26:04.000000 returnn-1.20230504.150134/demos/demo-tf-vanilla-lstm.12ax.config
+-rw-r--r--   0 runner    (1001) docker     (123)     4818 2023-05-04 13:26:04.000000 returnn-1.20230504.150134/demos/demo-timit-lstm-ctc.config
+-rw-r--r--   0 runner    (1001) docker     (123)     2521 2023-05-04 13:26:04.000000 returnn-1.20230504.150134/demos/demo-torch.config
+-rw-r--r--   0 runner    (1001) docker     (123)      766 2023-05-04 13:26:04.000000 returnn-1.20230504.150134/demos/demo-upd-mult-model.lstm.12ax.config
+-rwxr-xr-x   0 runner    (1001) docker     (123)      651 2023-05-04 13:26:04.000000 returnn-1.20230504.150134/demos/demo.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:26:23.000000 returnn-1.20230504.150134/demos/mdlstm/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:26:23.000000 returnn-1.20230504.150134/demos/mdlstm/IAM/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:26:23.000000 returnn-1.20230504.150134/demos/mdlstm/IAM/IAM_lines/
+-rwxr-xr-x   0 runner    (1001) docker     (123)    43239 2023-05-04 13:26:04.000000 returnn-1.20230504.150134/demos/mdlstm/IAM/IAM_lines/a01-000u-00.png
+-rwxr-xr-x   0 runner    (1001) docker     (123)    43552 2023-05-04 13:26:04.000000 returnn-1.20230504.150134/demos/mdlstm/IAM/IAM_lines/a01-007-04.png
+-rwxr-xr-x   0 runner    (1001) docker     (123)    45111 2023-05-04 13:26:04.000000 returnn-1.20230504.150134/demos/mdlstm/IAM/IAM_lines/a01-007-06.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1709 2023-05-04 13:26:04.000000 returnn-1.20230504.150134/demos/mdlstm/IAM/README.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      158 2023-05-04 13:26:04.000000 returnn-1.20230504.150134/demos/mdlstm/IAM/chars.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1896 2023-05-04 13:26:04.000000 returnn-1.20230504.150134/demos/mdlstm/IAM/config_demo
+-rw-r--r--   0 runner    (1001) docker     (123)     1981 2023-05-04 13:26:04.000000 returnn-1.20230504.150134/demos/mdlstm/IAM/config_fwd
+-rw-r--r--   0 runner    (1001) docker     (123)     1983 2023-05-04 13:26:04.000000 returnn-1.20230504.150134/demos/mdlstm/IAM/config_real
+-rwxr-xr-x   0 runner    (1001) docker     (123)    10194 2023-05-04 13:26:04.000000 returnn-1.20230504.150134/demos/mdlstm/IAM/create_IAM_dataset.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      749 2023-05-04 13:26:04.000000 returnn-1.20230504.150134/demos/mdlstm/IAM/decode.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:26:23.000000 returnn-1.20230504.150134/demos/mdlstm/IAM/features/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:26:23.000000 returnn-1.20230504.150134/demos/mdlstm/IAM/features/raw/
+-rw-r--r--   0 runner    (1001) docker     (123)   248580 2023-05-04 13:26:04.000000 returnn-1.20230504.150134/demos/mdlstm/IAM/features/raw/demo.h5
+-rwxr-xr-x   0 runner    (1001) docker     (123)       86 2023-05-04 13:26:04.000000 returnn-1.20230504.150134/demos/mdlstm/IAM/go.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-05-04 13:26:04.000000 returnn-1.20230504.150134/demos/mdlstm/IAM/lines.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:26:23.000000 returnn-1.20230504.150134/demos/mdlstm/IAM/split/
+-rw-r--r--   0 runner    (1001) docker     (123)     2712 2023-05-04 13:26:04.000000 returnn-1.20230504.150134/demos/mdlstm/IAM/split/eval.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    69536 2023-05-04 13:26:04.000000 returnn-1.20230504.150134/demos/mdlstm/IAM/split/train.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      934 2023-05-04 13:26:04.000000 returnn-1.20230504.150134/demos/mdlstm/IAM/split/valid.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-05-04 13:26:04.000000 returnn-1.20230504.150134/demos/mdlstm/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:26:23.000000 returnn-1.20230504.150134/demos/mdlstm/artificial/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2804 2023-05-04 13:26:04.000000 returnn-1.20230504.150134/demos/mdlstm/artificial/create_test_h5.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-05-04 13:26:04.000000 returnn-1.20230504.150134/demos/mdlstm/artificial/forwardconfig
+-rwxr-xr-x   0 runner    (1001) docker     (123)      105 2023-05-04 13:26:04.000000 returnn-1.20230504.150134/demos/mdlstm/artificial/go.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      970 2023-05-04 13:26:04.000000 returnn-1.20230504.150134/demos/mdlstm/artificial/trainconfig
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:26:23.000000 returnn-1.20230504.150134/demos/mdlstm/artificial_rgb/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2966 2023-05-04 13:26:04.000000 returnn-1.20230504.150134/demos/mdlstm/artificial_rgb/create_test_h5.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-05-04 13:26:04.000000 returnn-1.20230504.150134/demos/mdlstm/artificial_rgb/forwardconfig
+-rwxr-xr-x   0 runner    (1001) docker     (123)      105 2023-05-04 13:26:04.000000 returnn-1.20230504.150134/demos/mdlstm/artificial_rgb/go.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      970 2023-05-04 13:26:04.000000 returnn-1.20230504.150134/demos/mdlstm/artificial_rgb/trainconfig
+-rw-r--r--   0 runner    (1001) docker     (123)      463 2023-05-04 13:26:04.000000 returnn-1.20230504.150134/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-04 13:26:04.000000 returnn-1.20230504.150134/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:26:23.000000 returnn-1.20230504.150134/returnn/
+-rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-05-04 13:26:04.000000 returnn-1.20230504.150134/returnn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24324 2023-05-04 13:26:04.000000 returnn-1.20230504.150134/returnn/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6981 2023-05-04 13:26:04.000000 returnn-1.20230504.150134/returnn/__old_mod_loader__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4659 2023-05-04 13:26:04.000000 returnn-1.20230504.150134/returnn/__setup__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24267 2023-05-04 13:26:04.000000 returnn-1.20230504.150134/returnn/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:26:23.000000 returnn-1.20230504.150134/returnn/datasets/
+-rw-r--r--   0 runner    (1001) docker     (123)      390 2023-05-04 13:26:04.000000 returnn-1.20230504.150134/returnn/datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18032 2023-05-04 13:26:04.000000 returnn-1.20230504.150134/returnn/datasets/audio.py
+-rw-r--r--   0 runner    (1001) docker     (123)    62931 2023-05-04 13:26:04.000000 returnn-1.20230504.150134/returnn/datasets/basic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2388 2023-05-04 13:26:04.000000 returnn-1.20230504.150134/returnn/datasets/bundle_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24892 2023-05-04 13:26:04.000000 returnn-1.20230504.150134/returnn/datasets/cached.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11658 2023-05-04 13:26:04.000000 returnn-1.20230504.150134/returnn/datasets/cached2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    94213 2023-05-04 13:26:04.000000 returnn-1.20230504.150134/returnn/datasets/generating.py
+-rw-r--r--   0 runner    (1001) docker     (123)    65113 2023-05-04 13:26:04.000000 returnn-1.20230504.150134/returnn/datasets/hdf.py
+-rw-r--r--   0 runner    (1001) docker     (123)    85120 2023-05-04 13:26:04.000000 returnn-1.20230504.150134/returnn/datasets/lm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9065 2023-05-04 13:26:04.000000 returnn-1.20230504.150134/returnn/datasets/map.py
+-rw-r--r--   0 runner    (1001) docker     (123)    75821 2023-05-04 13:26:04.000000 returnn-1.20230504.150134/returnn/datasets/meta.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11167 2023-05-04 13:26:04.000000 returnn-1.20230504.150134/returnn/datasets/multi_proc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14596 2023-05-04 13:26:04.000000 returnn-1.20230504.150134/returnn/datasets/normalization_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5291 2023-05-04 13:26:04.000000 returnn-1.20230504.150134/returnn/datasets/numpy_dump.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9127 2023-05-04 13:26:04.000000 returnn-1.20230504.150134/returnn/datasets/raw_wav.py
+-rw-r--r--   0 runner    (1001) docker     (123)    56015 2023-05-04 13:26:04.000000 returnn-1.20230504.150134/returnn/datasets/sprint.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17608 2023-05-04 13:26:04.000000 returnn-1.20230504.150134/returnn/datasets/stereo.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:26:23.000000 returnn-1.20230504.150134/returnn/datasets/util/
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-04 13:26:04.000000 returnn-1.20230504.150134/returnn/datasets/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23915 2023-05-04 13:26:04.000000 returnn-1.20230504.150134/returnn/datasets/util/feature_extraction.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20445 2023-05-04 13:26:04.000000 returnn-1.20230504.150134/returnn/datasets/util/vocabulary.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:26:23.000000 returnn-1.20230504.150134/returnn/engine/
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-05-04 13:26:04.000000 returnn-1.20230504.150134/returnn/engine/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9325 2023-05-04 13:26:04.000000 returnn-1.20230504.150134/returnn/engine/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9912 2023-05-04 13:26:04.000000 returnn-1.20230504.150134/returnn/engine/batch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:26:23.000000 returnn-1.20230504.150134/returnn/extern/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:26:23.000000 returnn-1.20230504.150134/returnn/extern/WarpRna/
+-rw-r--r--   0 runner    (1001) docker     (123)     4005 2023-05-04 13:26:04.000000 returnn-1.20230504.150134/returnn/extern/WarpRna/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4024 2023-05-04 13:26:04.000000 returnn-1.20230504.150134/returnn/extern/WarpRna/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:26:23.000000 returnn-1.20230504.150134/returnn/extern/WarpRna/warp-rna/
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-05-04 13:26:06.000000 returnn-1.20230504.150134/returnn/extern/WarpRna/warp-rna/.git
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-04 13:26:08.000000 returnn-1.20230504.150134/returnn/extern/WarpRna/warp-rna/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-05-04 13:26:08.000000 returnn-1.20230504.150134/returnn/extern/WarpRna/warp-rna/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1448 2023-05-04 13:26:08.000000 returnn-1.20230504.150134/returnn/extern/WarpRna/warp-rna/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)    13770 2023-05-04 13:26:08.000000 returnn-1.20230504.150134/returnn/extern/WarpRna/warp-rna/aligner.gif
+-rw-r--r--   0 runner    (1001) docker     (123)    51077 2023-05-04 13:26:08.000000 returnn-1.20230504.150134/returnn/extern/WarpRna/warp-rna/check.png
+-rw-r--r--   0 runner    (1001) docker     (123)    11544 2023-05-04 13:26:08.000000 returnn-1.20230504.150134/returnn/extern/WarpRna/warp-rna/core.cu
+-rw-r--r--   0 runner    (1001) docker     (123)      975 2023-05-04 13:26:08.000000 returnn-1.20230504.150134/returnn/extern/WarpRna/warp-rna/core.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2512 2023-05-04 13:26:08.000000 returnn-1.20230504.150134/returnn/extern/WarpRna/warp-rna/core_cpu.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:26:23.000000 returnn-1.20230504.150134/returnn/extern/WarpRna/warp-rna/pytorch_binding/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-05-04 13:26:08.000000 returnn-1.20230504.150134/returnn/extern/WarpRna/warp-rna/pytorch_binding/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-05-04 13:26:08.000000 returnn-1.20230504.150134/returnn/extern/WarpRna/warp-rna/pytorch_binding/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2089 2023-05-04 13:26:08.000000 returnn-1.20230504.150134/returnn/extern/WarpRna/warp-rna/pytorch_binding/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3485 2023-05-04 13:26:08.000000 returnn-1.20230504.150134/returnn/extern/WarpRna/warp-rna/pytorch_binding/binding.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    11544 2023-05-04 13:26:08.000000 returnn-1.20230504.150134/returnn/extern/WarpRna/warp-rna/pytorch_binding/core.cu
+-rw-r--r--   0 runner    (1001) docker     (123)      975 2023-05-04 13:26:08.000000 returnn-1.20230504.150134/returnn/extern/WarpRna/warp-rna/pytorch_binding/core.h
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-04 13:26:08.000000 returnn-1.20230504.150134/returnn/extern/WarpRna/warp-rna/pytorch_binding/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2079 2023-05-04 13:26:08.000000 returnn-1.20230504.150134/returnn/extern/WarpRna/warp-rna/pytorch_binding/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:26:23.000000 returnn-1.20230504.150134/returnn/extern/WarpRna/warp-rna/pytorch_binding/warp_rna/
+-rw-r--r--   0 runner    (1001) docker     (123)     2885 2023-05-04 13:26:08.000000 returnn-1.20230504.150134/returnn/extern/WarpRna/warp-rna/pytorch_binding/warp_rna/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6961 2023-05-04 13:26:08.000000 returnn-1.20230504.150134/returnn/extern/WarpRna/warp-rna/pytorch_binding/warp_rna/test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4141 2023-05-04 13:26:08.000000 returnn-1.20230504.150134/returnn/extern/WarpRna/warp-rna/ref_rna.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:26:23.000000 returnn-1.20230504.150134/returnn/extern/WarpRna/warp-rna/tensorflow_binding/
+-rw-r--r--   0 runner    (1001) docker     (123)     6150 2023-05-04 13:26:08.000000 returnn-1.20230504.150134/returnn/extern/WarpRna/warp-rna/tensorflow_binding/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:26:23.000000 returnn-1.20230504.150134/returnn/extern/WarpRna/warp-rna/tensorflow_binding/src/
+-rw-r--r--   0 runner    (1001) docker     (123)     1693 2023-05-04 13:26:08.000000 returnn-1.20230504.150134/returnn/extern/WarpRna/warp-rna/tensorflow_binding/src/warp_rna_op.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     6030 2023-05-04 13:26:08.000000 returnn-1.20230504.150134/returnn/extern/WarpRna/warp-rna/tensorflow_binding/src/warp_rna_op_kernel_tmpl.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:26:23.000000 returnn-1.20230504.150134/returnn/extern/WarpRna/warp-rna/tensorflow_binding/warp_rna/
+-rw-r--r--   0 runner    (1001) docker     (123)     2076 2023-05-04 13:26:08.000000 returnn-1.20230504.150134/returnn/extern/WarpRna/warp-rna/tensorflow_binding/warp_rna/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4252 2023-05-04 13:26:08.000000 returnn-1.20230504.150134/returnn/extern/WarpRna/warp-rna/test.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-05-04 13:26:04.000000 returnn-1.20230504.150134/returnn/extern/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:26:23.000000 returnn-1.20230504.150134/returnn/extern/graph_editor/
+-rw-r--r--   0 runner    (1001) docker     (123)      257 2023-05-04 13:26:04.000000 returnn-1.20230504.150134/returnn/extern/graph_editor/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1239 2023-05-04 13:26:04.000000 returnn-1.20230504.150134/returnn/extern/graph_editor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8479 2023-05-04 13:26:04.000000 returnn-1.20230504.150134/returnn/extern/graph_editor/edit.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19826 2023-05-04 13:26:04.000000 returnn-1.20230504.150134/returnn/extern/graph_editor/reroute.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29772 2023-05-04 13:26:04.000000 returnn-1.20230504.150134/returnn/extern/graph_editor/select.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26578 2023-05-04 13:26:04.000000 returnn-1.20230504.150134/returnn/extern/graph_editor/subgraph.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30380 2023-05-04 13:26:04.000000 returnn-1.20230504.150134/returnn/extern/graph_editor/transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18727 2023-05-04 13:26:04.000000 returnn-1.20230504.150134/returnn/extern/graph_editor/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:26:23.000000 returnn-1.20230504.150134/returnn/frontend/
+-rw-r--r--   0 runner    (1001) docker     (123)     1260 2023-05-04 13:26:04.000000 returnn-1.20230504.150134/returnn/frontend/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37648 2023-05-04 13:26:04.000000 returnn-1.20230504.150134/returnn/frontend/_backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5125 2023-05-04 13:26:04.000000 returnn-1.20230504.150134/returnn/frontend/_numpy_backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5087 2023-05-04 13:26:04.000000 returnn-1.20230504.150134/returnn/frontend/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17465 2023-05-04 13:26:04.000000 returnn-1.20230504.150134/returnn/frontend/array_.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20833 2023-05-04 13:26:04.000000 returnn-1.20230504.150134/returnn/frontend/attention.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-05-04 13:26:04.000000 returnn-1.20230504.150134/returnn/frontend/cond.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2104 2023-05-04 13:26:04.000000 returnn-1.20230504.150134/returnn/frontend/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6015 2023-05-04 13:26:04.000000 returnn-1.20230504.150134/returnn/frontend/container.py
+-rw-r--r--   0 runner    (1001) docker     (123)      413 2023-05-04 13:26:04.000000 returnn-1.20230504.150134/returnn/frontend/control_flow_ctx.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22357 2023-05-04 13:26:04.000000 returnn-1.20230504.150134/returnn/frontend/conv.py
+-rw-r--r--   0 runner    (1001) docker     (123)      519 2023-05-04 13:26:04.000000 returnn-1.20230504.150134/returnn/frontend/device.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3538 2023-05-04 13:26:04.000000 returnn-1.20230504.150134/returnn/frontend/dims.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3334 2023-05-04 13:26:04.000000 returnn-1.20230504.150134/returnn/frontend/dropout.py
+-rw-r--r--   0 runner    (1001) docker     (123)      964 2023-05-04 13:26:04.000000 returnn-1.20230504.150134/returnn/frontend/dtype.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:26:23.000000 returnn-1.20230504.150134/returnn/frontend/encoder/
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-04 13:26:04.000000 returnn-1.20230504.150134/returnn/frontend/encoder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2109 2023-05-04 13:26:04.000000 returnn-1.20230504.150134/returnn/frontend/encoder/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15428 2023-05-04 13:26:04.000000 returnn-1.20230504.150134/returnn/frontend/encoder/conformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      330 2023-05-04 13:26:04.000000 returnn-1.20230504.150134/returnn/frontend/gradient.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5855 2023-05-04 13:26:04.000000 returnn-1.20230504.150134/returnn/frontend/init.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2147 2023-05-04 13:26:04.000000 returnn-1.20230504.150134/returnn/frontend/linear.py
+-rw-r--r--   0 runner    (1001) docker     (123)      808 2023-05-04 13:26:04.000000 returnn-1.20230504.150134/returnn/frontend/loop.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1898 2023-05-04 13:26:04.000000 returnn-1.20230504.150134/returnn/frontend/loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13010 2023-05-04 13:26:04.000000 returnn-1.20230504.150134/returnn/frontend/math_.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1945 2023-05-04 13:26:04.000000 returnn-1.20230504.150134/returnn/frontend/matmul.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9877 2023-05-04 13:26:04.000000 returnn-1.20230504.150134/returnn/frontend/module.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8114 2023-05-04 13:26:04.000000 returnn-1.20230504.150134/returnn/frontend/normalization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7158 2023-05-04 13:26:04.000000 returnn-1.20230504.150134/returnn/frontend/parameter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10723 2023-05-04 13:26:04.000000 returnn-1.20230504.150134/returnn/frontend/rand.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2374 2023-05-04 13:26:04.000000 returnn-1.20230504.150134/returnn/frontend/rec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4750 2023-05-04 13:26:04.000000 returnn-1.20230504.150134/returnn/frontend/reduce.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12200 2023-05-04 13:26:04.000000 returnn-1.20230504.150134/returnn/frontend/run_ctx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9385 2023-05-04 13:26:04.000000 returnn-1.20230504.150134/returnn/frontend/signal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2188 2023-05-04 13:26:04.000000 returnn-1.20230504.150134/returnn/frontend/state.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-05-04 13:26:04.000000 returnn-1.20230504.150134/returnn/frontend/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:26:23.000000 returnn-1.20230504.150134/returnn/import_/
+-rw-r--r--   0 runner    (1001) docker     (123)      243 2023-05-04 13:26:04.000000 returnn-1.20230504.150134/returnn/import_/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8148 2023-05-04 13:26:04.000000 returnn-1.20230504.150134/returnn/import_/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13961 2023-05-04 13:26:04.000000 returnn-1.20230504.150134/returnn/import_/git.py
+-rw-r--r--   0 runner    (1001) docker     (123)      798 2023-05-04 13:26:04.000000 returnn-1.20230504.150134/returnn/import_/import_.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33063 2023-05-04 13:26:04.000000 returnn-1.20230504.150134/returnn/learning_rate_control.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11738 2023-05-04 13:26:04.000000 returnn-1.20230504.150134/returnn/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35760 2023-05-04 13:26:04.000000 returnn-1.20230504.150134/returnn/native_op.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)   244393 2023-05-04 13:26:04.000000 returnn-1.20230504.150134/returnn/native_op.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23542 2023-05-04 13:26:04.000000 returnn-1.20230504.150134/returnn/pretrain.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:26:23.000000 returnn-1.20230504.150134/returnn/sprint/
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-05-04 13:26:04.000000 returnn-1.20230504.150134/returnn/sprint/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31545 2023-05-04 13:26:04.000000 returnn-1.20230504.150134/returnn/sprint/cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31137 2023-05-04 13:26:04.000000 returnn-1.20230504.150134/returnn/sprint/control.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23313 2023-05-04 13:26:04.000000 returnn-1.20230504.150134/returnn/sprint/error_signals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12305 2023-05-04 13:26:04.000000 returnn-1.20230504.150134/returnn/sprint/extern_interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36475 2023-05-04 13:26:04.000000 returnn-1.20230504.150134/returnn/sprint/interface.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:26:23.000000 returnn-1.20230504.150134/returnn/tensor/
+-rw-r--r--   0 runner    (1001) docker     (123)      501 2023-05-04 13:26:04.000000 returnn-1.20230504.150134/returnn/tensor/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-05-04 13:26:04.000000 returnn-1.20230504.150134/returnn/tensor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    99004 2023-05-04 13:26:04.000000 returnn-1.20230504.150134/returnn/tensor/_dim_extra.py
+-rw-r--r--   0 runner    (1001) docker     (123)   157144 2023-05-04 13:26:04.000000 returnn-1.20230504.150134/returnn/tensor/_tensor_extra.py
+-rw-r--r--   0 runner    (1001) docker     (123)      643 2023-05-04 13:26:04.000000 returnn-1.20230504.150134/returnn/tensor/_tensor_mixin_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4890 2023-05-04 13:26:04.000000 returnn-1.20230504.150134/returnn/tensor/_tensor_op_overloads.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5125 2023-05-04 13:26:04.000000 returnn-1.20230504.150134/returnn/tensor/control_flow_ctx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3884 2023-05-04 13:26:04.000000 returnn-1.20230504.150134/returnn/tensor/dim.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1884 2023-05-04 13:26:04.000000 returnn-1.20230504.150134/returnn/tensor/marked_dim.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7491 2023-05-04 13:26:04.000000 returnn-1.20230504.150134/returnn/tensor/tensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4187 2023-05-04 13:26:04.000000 returnn-1.20230504.150134/returnn/tensor/tensor_dict.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:26:23.000000 returnn-1.20230504.150134/returnn/tf/
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-05-04 13:26:04.000000 returnn-1.20230504.150134/returnn/tf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1632 2023-05-04 13:26:04.000000 returnn-1.20230504.150134/returnn/tf/compat.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36852 2023-05-04 13:26:04.000000 returnn-1.20230504.150134/returnn/tf/data_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15108 2023-05-04 13:26:04.000000 returnn-1.20230504.150134/returnn/tf/distributed.py
+-rw-r--r--   0 runner    (1001) docker     (123)   151443 2023-05-04 13:26:04.000000 returnn-1.20230504.150134/returnn/tf/engine.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:26:23.000000 returnn-1.20230504.150134/returnn/tf/frontend_layers/
+-rw-r--r--   0 runner    (1001) docker     (123)      452 2023-05-04 13:26:04.000000 returnn-1.20230504.150134/returnn/tf/frontend_layers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37861 2023-05-04 13:26:04.000000 returnn-1.20230504.150134/returnn/tf/frontend_layers/_backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3702 2023-05-04 13:26:04.000000 returnn-1.20230504.150134/returnn/tf/frontend_layers/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14297 2023-05-04 13:26:04.000000 returnn-1.20230504.150134/returnn/tf/frontend_layers/cond.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4304 2023-05-04 13:26:04.000000 returnn-1.20230504.150134/returnn/tf/frontend_layers/config_entry_points.py
+-rw-r--r--   0 runner    (1001) docker     (123)      888 2023-05-04 13:26:04.000000 returnn-1.20230504.150134/returnn/tf/frontend_layers/debug_eager_mode.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5712 2023-05-04 13:26:04.000000 returnn-1.20230504.150134/returnn/tf/frontend_layers/dims.py
+-rw-r--r--   0 runner    (1001) docker     (123)    71987 2023-05-04 13:26:04.000000 returnn-1.20230504.150134/returnn/tf/frontend_layers/layer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15829 2023-05-04 13:26:04.000000 returnn-1.20230504.150134/returnn/tf/frontend_layers/make_layer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5107 2023-05-04 13:26:04.000000 returnn-1.20230504.150134/returnn/tf/frontend_layers/parameter_assign.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2239 2023-05-04 13:26:04.000000 returnn-1.20230504.150134/returnn/tf/frontend_layers/prev_tensor_ref.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:26:23.000000 returnn-1.20230504.150134/returnn/tf/frontend_low_level/
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-05-04 13:26:04.000000 returnn-1.20230504.150134/returnn/tf/frontend_low_level/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20261 2023-05-04 13:26:04.000000 returnn-1.20230504.150134/returnn/tf/frontend_low_level/_backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5404 2023-05-04 13:26:04.000000 returnn-1.20230504.150134/returnn/tf/horovod.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31611 2023-05-04 13:26:04.000000 returnn-1.20230504.150134/returnn/tf/hyper_param_tuning.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:26:23.000000 returnn-1.20230504.150134/returnn/tf/layers/
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-05-04 13:26:04.000000 returnn-1.20230504.150134/returnn/tf/layers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   149447 2023-05-04 13:26:04.000000 returnn-1.20230504.150134/returnn/tf/layers/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)   585273 2023-05-04 13:26:04.000000 returnn-1.20230504.150134/returnn/tf/layers/basic.py
+-rw-r--r--   0 runner    (1001) docker     (123)   539812 2023-05-04 13:26:04.000000 returnn-1.20230504.150134/returnn/tf/layers/rec.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21515 2023-05-04 13:26:04.000000 returnn-1.20230504.150134/returnn/tf/layers/segmental_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    52409 2023-05-04 13:26:04.000000 returnn-1.20230504.150134/returnn/tf/layers/signal_processing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11239 2023-05-04 13:26:04.000000 returnn-1.20230504.150134/returnn/tf/layers/variable.py
+-rw-r--r--   0 runner    (1001) docker     (123)    79733 2023-05-04 13:26:04.000000 returnn-1.20230504.150134/returnn/tf/native_op.py
+-rw-r--r--   0 runner    (1001) docker     (123)   222320 2023-05-04 13:26:04.000000 returnn-1.20230504.150134/returnn/tf/network.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5471 2023-05-04 13:26:04.000000 returnn-1.20230504.150134/returnn/tf/sprint.py
+-rw-r--r--   0 runner    (1001) docker     (123)    71410 2023-05-04 13:26:04.000000 returnn-1.20230504.150134/returnn/tf/updater.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:26:23.000000 returnn-1.20230504.150134/returnn/tf/util/
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-05-04 13:26:04.000000 returnn-1.20230504.150134/returnn/tf/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   296804 2023-05-04 13:26:04.000000 returnn-1.20230504.150134/returnn/tf/util/basic.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28839 2023-05-04 13:26:04.000000 returnn-1.20230504.150134/returnn/tf/util/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17333 2023-05-04 13:26:04.000000 returnn-1.20230504.150134/returnn/tf/util/ken_lm.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11277 2023-05-04 13:26:04.000000 returnn-1.20230504.150134/returnn/tf/util/open_fst.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:26:23.000000 returnn-1.20230504.150134/returnn/torch/
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-05-04 13:26:04.000000 returnn-1.20230504.150134/returnn/torch/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-04 13:26:04.000000 returnn-1.20230504.150134/returnn/torch/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:26:23.000000 returnn-1.20230504.150134/returnn/torch/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-05-04 13:26:04.000000 returnn-1.20230504.150134/returnn/torch/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9483 2023-05-04 13:26:04.000000 returnn-1.20230504.150134/returnn/torch/data/pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5410 2023-05-04 13:26:04.000000 returnn-1.20230504.150134/returnn/torch/data/returnn_dataset_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      970 2023-05-04 13:26:04.000000 returnn-1.20230504.150134/returnn/torch/data/tensor_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22317 2023-05-04 13:26:04.000000 returnn-1.20230504.150134/returnn/torch/engine.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:26:23.000000 returnn-1.20230504.150134/returnn/torch/frontend/
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-05-04 13:26:04.000000 returnn-1.20230504.150134/returnn/torch/frontend/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    60092 2023-05-04 13:26:04.000000 returnn-1.20230504.150134/returnn/torch/frontend/_backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1830 2023-05-04 13:26:04.000000 returnn-1.20230504.150134/returnn/torch/frontend/_rand.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2714 2023-05-04 13:26:04.000000 returnn-1.20230504.150134/returnn/torch/frontend/bridge.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:26:23.000000 returnn-1.20230504.150134/returnn/torch/functional/
+-rw-r--r--   0 runner    (1001) docker     (123)      193 2023-05-04 13:26:04.000000 returnn-1.20230504.150134/returnn/torch/functional/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-05-04 13:26:04.000000 returnn-1.20230504.150134/returnn/torch/functional/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11122 2023-05-04 13:26:04.000000 returnn-1.20230504.150134/returnn/torch/updater.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:26:23.000000 returnn-1.20230504.150134/returnn/util/
+-rw-r--r--   0 runner    (1001) docker     (123)      336 2023-05-04 13:26:04.000000 returnn-1.20230504.150134/returnn/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   144924 2023-05-04 13:26:04.000000 returnn-1.20230504.150134/returnn/util/basic.py
+-rw-r--r--   0 runner    (1001) docker     (123)    59572 2023-05-04 13:26:04.000000 returnn-1.20230504.150134/returnn/util/better_exchook.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17977 2023-05-04 13:26:04.000000 returnn-1.20230504.150134/returnn/util/bpe.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15987 2023-05-04 13:26:04.000000 returnn-1.20230504.150134/returnn/util/debug.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2905 2023-05-04 13:26:04.000000 returnn-1.20230504.150134/returnn/util/debug_helpers.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    59177 2023-05-04 13:26:04.000000 returnn-1.20230504.150134/returnn/util/fsa.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2009 2023-05-04 13:26:04.000000 returnn-1.20230504.150134/returnn/util/literal_py_to_pickle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8131 2023-05-04 13:26:04.000000 returnn-1.20230504.150134/returnn/util/pprint.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14846 2023-05-04 13:26:04.000000 returnn-1.20230504.150134/returnn/util/py-to-pickle.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      277 2023-05-04 13:26:04.000000 returnn-1.20230504.150134/returnn/util/py_compat.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7273 2023-05-04 13:26:04.000000 returnn-1.20230504.150134/returnn/util/sig_proc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27230 2023-05-04 13:26:04.000000 returnn-1.20230504.150134/returnn/util/task_system.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:26:23.000000 returnn-1.20230504.150134/returnn.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4718 2023-05-04 13:26:23.000000 returnn-1.20230504.150134/returnn.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12268 2023-05-04 13:26:23.000000 returnn-1.20230504.150134/returnn.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 13:26:23.000000 returnn-1.20230504.150134/returnn.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-04 13:26:23.000000 returnn-1.20230504.150134/returnn.egg-info/top_level.txt
+-rwxr-xr-x   0 runner    (1001) docker     (123)      461 2023-05-04 13:26:04.000000 returnn-1.20230504.150134/rnn.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-04 13:26:23.000000 returnn-1.20230504.150134/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     4159 2023-05-04 13:26:04.000000 returnn-1.20230504.150134/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:26:23.000000 returnn-1.20230504.150134/tests/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3392 2023-05-04 13:26:04.000000 returnn-1.20230504.150134/tests/DummySprintExec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2671 2023-05-04 13:26:04.000000 returnn-1.20230504.150134/tests/PyCharm-inspection-profile.xml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:26:23.000000 returnn-1.20230504.150134/tests/PyCharm.idea/
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-04 13:26:04.000000 returnn-1.20230504.150134/tests/PyCharm.idea/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-04 13:26:04.000000 returnn-1.20230504.150134/tests/PyCharm.idea/.name
+-rw-r--r--   0 runner    (1001) docker     (123)      512 2023-05-04 13:26:04.000000 returnn-1.20230504.150134/tests/PyCharm.idea/codeStyleSettings.xml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:26:23.000000 returnn-1.20230504.150134/tests/PyCharm.idea/codeStyles/
+-rw-r--r--   0 runner    (1001) docker     (123)      328 2023-05-04 13:26:04.000000 returnn-1.20230504.150134/tests/PyCharm.idea/codeStyles/Project.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-05-04 13:26:04.000000 returnn-1.20230504.150134/tests/PyCharm.idea/codeStyles/codeStyleConfig.xml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:26:23.000000 returnn-1.20230504.150134/tests/PyCharm.idea/inspectionProfiles/
+-rw-r--r--   0 runner    (1001) docker     (123)     2671 2023-05-04 13:26:04.000000 returnn-1.20230504.150134/tests/PyCharm.idea/inspectionProfiles/Project_Default.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      181 2023-05-04 13:26:04.000000 returnn-1.20230504.150134/tests/PyCharm.idea/inspectionProfiles/profiles_settings.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      318 2023-05-04 13:26:04.000000 returnn-1.20230504.150134/tests/PyCharm.idea/misc.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      267 2023-05-04 13:26:04.000000 returnn-1.20230504.150134/tests/PyCharm.idea/modules.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      417 2023-05-04 13:26:04.000000 returnn-1.20230504.150134/tests/PyCharm.idea/returnn.iml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:26:23.000000 returnn-1.20230504.150134/tests/PyCharm.idea/scopes/
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-05-04 13:26:04.000000 returnn-1.20230504.150134/tests/PyCharm.idea/scopes/scope_settings.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      871 2023-05-04 13:26:04.000000 returnn-1.20230504.150134/tests/_set_num_threads1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      476 2023-05-04 13:26:04.000000 returnn-1.20230504.150134/tests/_setup_returnn_env.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8833 2023-05-04 13:26:04.000000 returnn-1.20230504.150134/tests/_setup_test_env.py
+-rw-r--r--   0 runner    (1001) docker     (123)      794 2023-05-04 13:26:04.000000 returnn-1.20230504.150134/tests/bpe-unicode-demo.codes
+-rw-r--r--   0 runner    (1001) docker     (123)     2205 2023-05-04 13:26:04.000000 returnn-1.20230504.150134/tests/bpe-unicode-demo.vocab
+-rw-r--r--   0 runner    (1001) docker     (123)      386 2023-05-04 13:26:04.000000 returnn-1.20230504.150134/tests/lexicon_opt.fst
+-rw-r--r--   0 runner    (1001) docker     (123)      520 2023-05-04 13:26:04.000000 returnn-1.20230504.150134/tests/lexicon_opt.isyms
+-rw-r--r--   0 runner    (1001) docker     (123)    34282 2023-05-04 13:26:04.000000 returnn-1.20230504.150134/tests/lexicon_opt.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-04 13:26:04.000000 returnn-1.20230504.150134/tests/lexicon_opt.osyms
+-rw-r--r--   0 runner    (1001) docker     (123)     6880 2023-05-04 13:26:04.000000 returnn-1.20230504.150134/tests/lint_common.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    29203 2023-05-04 13:26:04.000000 returnn-1.20230504.150134/tests/pycharm-inspect.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2960 2023-05-04 13:26:04.000000 returnn-1.20230504.150134/tests/pylint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2963 2023-05-04 13:26:04.000000 returnn-1.20230504.150134/tests/returnn-as-framework.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11619 2023-05-04 13:26:04.000000 returnn-1.20230504.150134/tests/rf_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      617 2023-05-04 13:26:04.000000 returnn-1.20230504.150134/tests/spelling.dic
+-rw-r--r--   0 runner    (1001) docker     (123)     7845 2023-05-04 13:26:04.000000 returnn-1.20230504.150134/tests/test_Config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18921 2023-05-04 13:26:04.000000 returnn-1.20230504.150134/tests/test_Dataset.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    13634 2023-05-04 13:26:04.000000 returnn-1.20230504.150134/tests/test_Fsa.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8904 2023-05-04 13:26:04.000000 returnn-1.20230504.150134/tests/test_GeneratingDataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32796 2023-05-04 13:26:04.000000 returnn-1.20230504.150134/tests/test_HDFDataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10326 2023-05-04 13:26:04.000000 returnn-1.20230504.150134/tests/test_LearningRateControl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7187 2023-05-04 13:26:04.000000 returnn-1.20230504.150134/tests/test_Log.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3635 2023-05-04 13:26:04.000000 returnn-1.20230504.150134/tests/test_MultiProcDataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3333 2023-05-04 13:26:04.000000 returnn-1.20230504.150134/tests/test_PTDataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2465 2023-05-04 13:26:04.000000 returnn-1.20230504.150134/tests/test_Pretrain.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21403 2023-05-04 13:26:04.000000 returnn-1.20230504.150134/tests/test_ResNet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5014 2023-05-04 13:26:04.000000 returnn-1.20230504.150134/tests/test_SprintDataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3330 2023-05-04 13:26:04.000000 returnn-1.20230504.150134/tests/test_SprintInterface.py
+-rw-r--r--   0 runner    (1001) docker     (123)   238053 2023-05-04 13:26:04.000000 returnn-1.20230504.150134/tests/test_TFEngine.py
+-rw-r--r--   0 runner    (1001) docker     (123)   135453 2023-05-04 13:26:04.000000 returnn-1.20230504.150134/tests/test_TFNativeOp.py
+-rw-r--r--   0 runner    (1001) docker     (123)   551354 2023-05-04 13:26:04.000000 returnn-1.20230504.150134/tests/test_TFNetworkLayer.py
+-rw-r--r--   0 runner    (1001) docker     (123)   549696 2023-05-04 13:26:04.000000 returnn-1.20230504.150134/tests/test_TFNetworkRecLayer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14485 2023-05-04 13:26:04.000000 returnn-1.20230504.150134/tests/test_TFNetworkSigProcLayer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20440 2023-05-04 13:26:04.000000 returnn-1.20230504.150134/tests/test_TFUpdater.py
+-rw-r--r--   0 runner    (1001) docker     (123)   187644 2023-05-04 13:26:04.000000 returnn-1.20230504.150134/tests/test_TFUtil.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3082 2023-05-04 13:26:04.000000 returnn-1.20230504.150134/tests/test_TF_determinism.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2156 2023-05-04 13:26:04.000000 returnn-1.20230504.150134/tests/test_TaskSystem.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5088 2023-05-04 13:26:04.000000 returnn-1.20230504.150134/tests/test_TaskSystem_SharedMem.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9378 2023-05-04 13:26:04.000000 returnn-1.20230504.150134/tests/test_TranslationDataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14944 2023-05-04 13:26:04.000000 returnn-1.20230504.150134/tests/test_Util.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10578 2023-05-04 13:26:04.000000 returnn-1.20230504.150134/tests/test_demos.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7375 2023-05-04 13:26:04.000000 returnn-1.20230504.150134/tests/test_fork_exec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2893 2023-05-04 13:26:04.000000 returnn-1.20230504.150134/tests/test_hdf_dump.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4725 2023-05-04 13:26:04.000000 returnn-1.20230504.150134/tests/test_rf_array.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4491 2023-05-04 13:26:04.000000 returnn-1.20230504.150134/tests/test_rf_attention.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7608 2023-05-04 13:26:04.000000 returnn-1.20230504.150134/tests/test_rf_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9490 2023-05-04 13:26:04.000000 returnn-1.20230504.150134/tests/test_rf_cond.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4591 2023-05-04 13:26:04.000000 returnn-1.20230504.150134/tests/test_rf_container.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10228 2023-05-04 13:26:04.000000 returnn-1.20230504.150134/tests/test_rf_conv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1963 2023-05-04 13:26:04.000000 returnn-1.20230504.150134/tests/test_rf_encoder_conformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2312 2023-05-04 13:26:04.000000 returnn-1.20230504.150134/tests/test_rf_math.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1127 2023-05-04 13:26:04.000000 returnn-1.20230504.150134/tests/test_rf_normalization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1772 2023-05-04 13:26:04.000000 returnn-1.20230504.150134/tests/test_rf_rec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1052 2023-05-04 13:26:04.000000 returnn-1.20230504.150134/tests/test_rf_signal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1135 2023-05-04 13:26:04.000000 returnn-1.20230504.150134/tests/test_tensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8435 2023-05-04 13:26:04.000000 returnn-1.20230504.150134/tests/test_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15594 2023-05-04 13:26:04.000000 returnn-1.20230504.150134/tests/test_torch_frontend.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15534 2023-05-04 13:26:04.000000 returnn-1.20230504.150134/tests/test_torch_internal_frontend.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:26:23.000000 returnn-1.20230504.150134/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)      476 2023-05-04 13:26:04.000000 returnn-1.20230504.150134/tools/_setup_returnn_env.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     9650 2023-05-04 13:26:04.000000 returnn-1.20230504.150134/tools/analyze-dataset-batches.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3943 2023-05-04 13:26:04.000000 returnn-1.20230504.150134/tools/bliss-collect-seq-lens.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      780 2023-05-04 13:26:04.000000 returnn-1.20230504.150134/tools/bliss-dump-text.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6608 2023-05-04 13:26:04.000000 returnn-1.20230504.150134/tools/bliss-get-segment-names.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    18221 2023-05-04 13:26:04.000000 returnn-1.20230504.150134/tools/bliss-to-ogg-zip.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5644 2023-05-04 13:26:04.000000 returnn-1.20230504.150134/tools/bpe-create-lexicon.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    10532 2023-05-04 13:26:04.000000 returnn-1.20230504.150134/tools/calculate-word-error-rate.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1759 2023-05-04 13:26:04.000000 returnn-1.20230504.150134/tools/cleanup-old-models.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    10783 2023-05-04 13:26:04.000000 returnn-1.20230504.150134/tools/collect-orth-symbols.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6801 2023-05-04 13:26:04.000000 returnn-1.20230504.150134/tools/collect-words.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4395 2023-05-04 13:26:04.000000 returnn-1.20230504.150134/tools/compile_native_op.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    81620 2023-05-04 13:26:04.000000 returnn-1.20230504.150134/tools/compile_tf_graph.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8500 2023-05-04 13:26:04.000000 returnn-1.20230504.150134/tools/debug-dump-search-scores.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    47001 2023-05-04 13:26:04.000000 returnn-1.20230504.150134/tools/debug-plot-search-scores.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6048 2023-05-04 13:26:04.000000 returnn-1.20230504.150134/tools/dump-dataset-raw-strings.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    12524 2023-05-04 13:26:04.000000 returnn-1.20230504.150134/tools/dump-dataset.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5770 2023-05-04 13:26:04.000000 returnn-1.20230504.150134/tools/dump-forward-stats.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2576 2023-05-04 13:26:04.000000 returnn-1.20230504.150134/tools/dump-forward.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1596 2023-05-04 13:26:04.000000 returnn-1.20230504.150134/tools/dump-network-json.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      719 2023-05-04 13:26:04.000000 returnn-1.20230504.150134/tools/dump-pickle.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    16425 2023-05-04 13:26:04.000000 returnn-1.20230504.150134/tools/extract_state_tying_from_dataset.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    14986 2023-05-04 13:26:04.000000 returnn-1.20230504.150134/tools/get-attention-weights.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2936 2023-05-04 13:26:04.000000 returnn-1.20230504.150134/tools/get-best-model-epoch.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3900 2023-05-04 13:26:04.000000 returnn-1.20230504.150134/tools/hdf_dump.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    19622 2023-05-04 13:26:04.000000 returnn-1.20230504.150134/tools/hdf_dump_translation_dataset.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    49563 2023-05-04 13:26:04.000000 returnn-1.20230504.150134/tools/import-blocks-mt-model.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    31498 2023-05-04 13:26:04.000000 returnn-1.20230504.150134/tools/import-t2t-mt-model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:26:23.000000 returnn-1.20230504.150134/tools/lattice_rescorer/
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-04 13:26:04.000000 returnn-1.20230504.150134/tools/lattice_rescorer/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     2254 2023-05-04 13:26:04.000000 returnn-1.20230504.150134/tools/lattice_rescorer/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     7825 2023-05-04 13:26:04.000000 returnn-1.20230504.150134/tools/lattice_rescorer/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:26:23.000000 returnn-1.20230504.150134/tools/lattice_rescorer/example/
+-rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-05-04 13:26:04.000000 returnn-1.20230504.150134/tools/lattice_rescorer/example/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-05-04 13:26:04.000000 returnn-1.20230504.150134/tools/lattice_rescorer/example/libs_list
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:26:23.000000 returnn-1.20230504.150134/tools/lattice_rescorer/example/network.040/
+-rw-r--r--   0 runner    (1001) docker     (123)     5775 2023-05-04 13:26:04.000000 returnn-1.20230504.150134/tools/lattice_rescorer/example/network.040/i600_m600_m600.sgd_b16_lr0_cl2.newbobabs.config
+-rw-r--r--   0 runner    (1001) docker     (123)     6110 2023-05-04 13:26:04.000000 returnn-1.20230504.150134/tools/lattice_rescorer/example/network.040/i600_m600_m600.sgd_b16_lr0_cl2.newbobabs.keep_over_epoch.lstm2.config
+-rwxr-xr-x   0 runner    (1001) docker     (123)      800 2023-05-04 13:26:04.000000 returnn-1.20230504.150134/tools/lattice_rescorer/example/rescore_lattice.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      296 2023-05-04 13:26:04.000000 returnn-1.20230504.150134/tools/lattice_rescorer/example/state_vars_list
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-05-04 13:26:04.000000 returnn-1.20230504.150134/tools/lattice_rescorer/example/tensor_names_list
+-rw-r--r--   0 runner    (1001) docker     (123)     1687 2023-05-04 13:26:04.000000 returnn-1.20230504.150134/tools/lattice_rescorer/file.h
+-rw-r--r--   0 runner    (1001) docker     (123)    26055 2023-05-04 13:26:04.000000 returnn-1.20230504.150134/tools/lattice_rescorer/htklatticerescorer.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    10856 2023-05-04 13:26:04.000000 returnn-1.20230504.150134/tools/lattice_rescorer/htklatticerescorer.h
+-rw-r--r--   0 runner    (1001) docker     (123)    12488 2023-05-04 13:26:04.000000 returnn-1.20230504.150134/tools/lattice_rescorer/main.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     2184 2023-05-04 13:26:04.000000 returnn-1.20230504.150134/tools/lattice_rescorer/rescorer.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5563 2023-05-04 13:26:04.000000 returnn-1.20230504.150134/tools/lattice_rescorer/vocabulary.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     3023 2023-05-04 13:26:04.000000 returnn-1.20230504.150134/tools/lattice_rescorer/vocabulary.h
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5438 2023-05-04 13:26:04.000000 returnn-1.20230504.150134/tools/tf_avg_checkpoints.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6269 2023-05-04 13:26:04.000000 returnn-1.20230504.150134/tools/tf_inspect_checkpoint.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1288 2023-05-04 13:26:04.000000 returnn-1.20230504.150134/tools/tf_inspect_summary_log.py
```

### Comparing `returnn-1.20230503.142906/.gitignore` & `returnn-1.20230504.150134/.gitignore`

 * *Files identical despite different names*

### Comparing `returnn-1.20230503.142906/.gitmodules` & `returnn-1.20230504.150134/.gitmodules`

 * *Files identical despite different names*

### Comparing `returnn-1.20230503.142906/CHANGELOG.md` & `returnn-1.20230504.150134/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `returnn-1.20230503.142906/CODEOWNERS` & `returnn-1.20230504.150134/CODEOWNERS`

 * *Files identical despite different names*

### Comparing `returnn-1.20230503.142906/CONTRIBUTING.md` & `returnn-1.20230504.150134/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `returnn-1.20230503.142906/LICENSE` & `returnn-1.20230504.150134/LICENSE`

 * *Files identical despite different names*

### Comparing `returnn-1.20230503.142906/MANIFEST.in` & `returnn-1.20230504.150134/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `returnn-1.20230503.142906/PKG-INFO` & `returnn-1.20230504.150134/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: returnn
-Version: 1.20230503.142906
+Version: 1.20230504.150134
 Summary: The RWTH extensible training framework for universal recurrent neural networks
 Home-page: https://github.com/rwth-i6/returnn/
 Author: Albert Zeyer
 Author-email: albzey@gmail.com
 License: RETURNN license
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
```

### Comparing `returnn-1.20230503.142906/README.rst` & `returnn-1.20230504.150134/README.rst`

 * *Files identical despite different names*

### Comparing `returnn-1.20230503.142906/__init__.py` & `returnn-1.20230504.150134/__init__.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230503.142906/demos/12AX.cluster_map` & `returnn-1.20230504.150134/demos/12AX.cluster_map`

 * *Files identical despite different names*

### Comparing `returnn-1.20230503.142906/demos/demo-fwd.config` & `returnn-1.20230504.150134/demos/demo-fwd.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230503.142906/demos/demo-horovod-mpi.py` & `returnn-1.20230504.150134/demos/demo-horovod-mpi.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230503.142906/demos/demo-horovod-mpi.py.sh` & `returnn-1.20230504.150134/demos/demo-horovod-mpi.py.sh`

 * *Files identical despite different names*

### Comparing `returnn-1.20230503.142906/demos/demo-hyper-param-tuning.config` & `returnn-1.20230504.150134/demos/demo-hyper-param-tuning.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230503.142906/demos/demo-iter-dataset.py` & `returnn-1.20230504.150134/demos/demo-iter-dataset.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230503.142906/demos/demo-list-devices.py` & `returnn-1.20230504.150134/demos/demo-list-devices.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230503.142906/demos/demo-lua-torch-layer.config` & `returnn-1.20230504.150134/demos/demo-lua-torch-layer.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230503.142906/demos/demo-record-and-push-to-webserver.py` & `returnn-1.20230504.150134/demos/demo-record-and-push-to-webserver.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230503.142906/demos/demo-returnn-as-framework.py` & `returnn-1.20230504.150134/demos/demo-returnn-as-framework.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230503.142906/demos/demo-rf.config` & `returnn-1.20230504.150134/demos/demo-rf.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230503.142906/demos/demo-rhn-enwik8.config` & `returnn-1.20230504.150134/demos/demo-rhn-enwik8.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230503.142906/demos/demo-sprint-interface.py` & `returnn-1.20230504.150134/demos/demo-sprint-interface.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230503.142906/demos/demo-tf-att-copy.config` & `returnn-1.20230504.150134/demos/demo-tf-att-copy.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230503.142906/demos/demo-tf-attention.config` & `returnn-1.20230504.150134/demos/demo-tf-attention.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230503.142906/demos/demo-tf-chunking-blstm.12ax.config` & `returnn-1.20230504.150134/demos/demo-tf-chunking-blstm.12ax.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230503.142906/demos/demo-tf-contribrnn-lstm.12ax.config` & `returnn-1.20230504.150134/demos/demo-tf-contribrnn-lstm.12ax.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230503.142906/demos/demo-tf-enc-dec.config` & `returnn-1.20230504.150134/demos/demo-tf-enc-dec.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230503.142906/demos/demo-tf-hard-att-copy.config` & `returnn-1.20230504.150134/demos/demo-tf-hard-att-copy.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230503.142906/demos/demo-tf-lstm-benchmark.py` & `returnn-1.20230504.150134/demos/demo-tf-lstm-benchmark.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230503.142906/demos/demo-tf-maxgradnorm-lstm.12ax.config` & `returnn-1.20230504.150134/demos/demo-tf-maxgradnorm-lstm.12ax.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230503.142906/demos/demo-tf-native-lstm-lowmem.12ax.config` & `returnn-1.20230504.150134/demos/demo-tf-native-lstm-lowmem.12ax.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230503.142906/demos/demo-tf-native-lstm.12ax.config` & `returnn-1.20230504.150134/demos/demo-tf-native-lstm.12ax.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230503.142906/demos/demo-tf-native-lstm2.12ax.config` & `returnn-1.20230504.150134/demos/demo-tf-native-lstm2.12ax.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230503.142906/demos/demo-tf-native-lstm2.12ax.tuned.config` & `returnn-1.20230504.150134/demos/demo-tf-native-lstm2.12ax.tuned.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230503.142906/demos/demo-tf-neural-transducer.12ax.config` & `returnn-1.20230504.150134/demos/demo-tf-neural-transducer.12ax.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230503.142906/demos/demo-tf-rec-explicit-lstm.config` & `returnn-1.20230504.150134/demos/demo-tf-rec-explicit-lstm.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230503.142906/demos/demo-tf-rec-explicit-rnn.config` & `returnn-1.20230504.150134/demos/demo-tf-rec-explicit-rnn.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230503.142906/demos/demo-tf-rec-self-att.config` & `returnn-1.20230504.150134/demos/demo-tf-rec-self-att.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230503.142906/demos/demo-tf-search-compiled-graph.py` & `returnn-1.20230504.150134/demos/demo-tf-search-compiled-graph.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230503.142906/demos/demo-tf-vanilla-lstm.12ax.config` & `returnn-1.20230504.150134/demos/demo-tf-vanilla-lstm.12ax.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230503.142906/demos/demo-timit-lstm-ctc.config` & `returnn-1.20230504.150134/demos/demo-timit-lstm-ctc.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230503.142906/demos/demo-torch.config` & `returnn-1.20230504.150134/demos/demo-torch.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230503.142906/demos/demo-upd-mult-model.lstm.12ax.config` & `returnn-1.20230504.150134/demos/demo-upd-mult-model.lstm.12ax.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230503.142906/demos/demo.sh` & `returnn-1.20230504.150134/demos/demo.sh`

 * *Files identical despite different names*

### Comparing `returnn-1.20230503.142906/demos/mdlstm/IAM/IAM_lines/a01-000u-00.png` & `returnn-1.20230504.150134/demos/mdlstm/IAM/IAM_lines/a01-000u-00.png`

 * *Files identical despite different names*

### Comparing `returnn-1.20230503.142906/demos/mdlstm/IAM/IAM_lines/a01-007-04.png` & `returnn-1.20230504.150134/demos/mdlstm/IAM/IAM_lines/a01-007-04.png`

 * *Files identical despite different names*

### Comparing `returnn-1.20230503.142906/demos/mdlstm/IAM/IAM_lines/a01-007-06.png` & `returnn-1.20230504.150134/demos/mdlstm/IAM/IAM_lines/a01-007-06.png`

 * *Files identical despite different names*

### Comparing `returnn-1.20230503.142906/demos/mdlstm/IAM/README.txt` & `returnn-1.20230504.150134/demos/mdlstm/IAM/README.txt`

 * *Files identical despite different names*

### Comparing `returnn-1.20230503.142906/demos/mdlstm/IAM/config_demo` & `returnn-1.20230504.150134/demos/mdlstm/IAM/config_demo`

 * *Files identical despite different names*

### Comparing `returnn-1.20230503.142906/demos/mdlstm/IAM/config_fwd` & `returnn-1.20230504.150134/demos/mdlstm/IAM/config_fwd`

 * *Files identical despite different names*

### Comparing `returnn-1.20230503.142906/demos/mdlstm/IAM/config_real` & `returnn-1.20230504.150134/demos/mdlstm/IAM/config_real`

 * *Files identical despite different names*

### Comparing `returnn-1.20230503.142906/demos/mdlstm/IAM/create_IAM_dataset.py` & `returnn-1.20230504.150134/demos/mdlstm/IAM/create_IAM_dataset.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230503.142906/demos/mdlstm/IAM/decode.py` & `returnn-1.20230504.150134/demos/mdlstm/IAM/decode.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230503.142906/demos/mdlstm/IAM/features/raw/demo.h5` & `returnn-1.20230504.150134/demos/mdlstm/IAM/features/raw/demo.h5`

 * *Files identical despite different names*

### Comparing `returnn-1.20230503.142906/demos/mdlstm/IAM/split/eval.txt` & `returnn-1.20230504.150134/demos/mdlstm/IAM/split/eval.txt`

 * *Files identical despite different names*

### Comparing `returnn-1.20230503.142906/demos/mdlstm/IAM/split/train.txt` & `returnn-1.20230504.150134/demos/mdlstm/IAM/split/train.txt`

 * *Files identical despite different names*

### Comparing `returnn-1.20230503.142906/demos/mdlstm/IAM/split/valid.txt` & `returnn-1.20230504.150134/demos/mdlstm/IAM/split/valid.txt`

 * *Files identical despite different names*

### Comparing `returnn-1.20230503.142906/demos/mdlstm/artificial/create_test_h5.py` & `returnn-1.20230504.150134/demos/mdlstm/artificial/create_test_h5.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230503.142906/demos/mdlstm/artificial/forwardconfig` & `returnn-1.20230504.150134/demos/mdlstm/artificial/forwardconfig`

 * *Files identical despite different names*

### Comparing `returnn-1.20230503.142906/demos/mdlstm/artificial/trainconfig` & `returnn-1.20230504.150134/demos/mdlstm/artificial/trainconfig`

 * *Files identical despite different names*

### Comparing `returnn-1.20230503.142906/demos/mdlstm/artificial_rgb/create_test_h5.py` & `returnn-1.20230504.150134/demos/mdlstm/artificial_rgb/create_test_h5.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230503.142906/demos/mdlstm/artificial_rgb/forwardconfig` & `returnn-1.20230504.150134/demos/mdlstm/artificial_rgb/forwardconfig`

 * *Files identical despite different names*

### Comparing `returnn-1.20230503.142906/demos/mdlstm/artificial_rgb/trainconfig` & `returnn-1.20230504.150134/demos/mdlstm/artificial_rgb/trainconfig`

 * *Files identical despite different names*

### Comparing `returnn-1.20230503.142906/returnn/__init__.py` & `returnn-1.20230504.150134/returnn/__init__.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230503.142906/returnn/__main__.py` & `returnn-1.20230504.150134/returnn/__main__.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230503.142906/returnn/__old_mod_loader__.py` & `returnn-1.20230504.150134/returnn/__old_mod_loader__.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230503.142906/returnn/__setup__.py` & `returnn-1.20230504.150134/returnn/__setup__.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230503.142906/returnn/config.py` & `returnn-1.20230504.150134/returnn/config.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230503.142906/returnn/datasets/audio.py` & `returnn-1.20230504.150134/returnn/datasets/audio.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230503.142906/returnn/datasets/basic.py` & `returnn-1.20230504.150134/returnn/datasets/basic.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230503.142906/returnn/datasets/bundle_file.py` & `returnn-1.20230504.150134/returnn/datasets/bundle_file.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230503.142906/returnn/datasets/cached.py` & `returnn-1.20230504.150134/returnn/datasets/cached.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230503.142906/returnn/datasets/cached2.py` & `returnn-1.20230504.150134/returnn/datasets/cached2.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230503.142906/returnn/datasets/generating.py` & `returnn-1.20230504.150134/returnn/datasets/generating.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230503.142906/returnn/datasets/hdf.py` & `returnn-1.20230504.150134/returnn/datasets/hdf.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230503.142906/returnn/datasets/lm.py` & `returnn-1.20230504.150134/returnn/datasets/lm.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230503.142906/returnn/datasets/map.py` & `returnn-1.20230504.150134/returnn/datasets/map.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230503.142906/returnn/datasets/meta.py` & `returnn-1.20230504.150134/returnn/datasets/meta.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230503.142906/returnn/datasets/multi_proc.py` & `returnn-1.20230504.150134/returnn/datasets/multi_proc.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230503.142906/returnn/datasets/normalization_data.py` & `returnn-1.20230504.150134/returnn/datasets/normalization_data.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230503.142906/returnn/datasets/numpy_dump.py` & `returnn-1.20230504.150134/returnn/datasets/numpy_dump.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230503.142906/returnn/datasets/raw_wav.py` & `returnn-1.20230504.150134/returnn/datasets/raw_wav.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230503.142906/returnn/datasets/sprint.py` & `returnn-1.20230504.150134/returnn/datasets/sprint.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230503.142906/returnn/datasets/stereo.py` & `returnn-1.20230504.150134/returnn/datasets/stereo.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230503.142906/returnn/datasets/util/feature_extraction.py` & `returnn-1.20230504.150134/returnn/datasets/util/feature_extraction.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230503.142906/returnn/datasets/util/vocabulary.py` & `returnn-1.20230504.150134/returnn/datasets/util/vocabulary.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230503.142906/returnn/engine/base.py` & `returnn-1.20230504.150134/returnn/engine/base.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230503.142906/returnn/engine/batch.py` & `returnn-1.20230504.150134/returnn/engine/batch.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230503.142906/returnn/extern/WarpRna/__init__.py` & `returnn-1.20230504.150134/returnn/extern/WarpRna/__init__.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230503.142906/returnn/extern/WarpRna/__main__.py` & `returnn-1.20230504.150134/returnn/extern/WarpRna/__main__.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230503.142906/returnn/extern/WarpRna/warp-rna/LICENSE` & `returnn-1.20230504.150134/returnn/extern/WarpRna/warp-rna/LICENSE`

 * *Files identical despite different names*

### Comparing `returnn-1.20230503.142906/returnn/extern/WarpRna/warp-rna/README.md` & `returnn-1.20230504.150134/returnn/extern/WarpRna/warp-rna/README.md`

 * *Files identical despite different names*

### Comparing `returnn-1.20230503.142906/returnn/extern/WarpRna/warp-rna/aligner.gif` & `returnn-1.20230504.150134/returnn/extern/WarpRna/warp-rna/aligner.gif`

 * *Files identical despite different names*

### Comparing `returnn-1.20230503.142906/returnn/extern/WarpRna/warp-rna/check.png` & `returnn-1.20230504.150134/returnn/extern/WarpRna/warp-rna/check.png`

 * *Files identical despite different names*

### Comparing `returnn-1.20230503.142906/returnn/extern/WarpRna/warp-rna/core.cu` & `returnn-1.20230504.150134/returnn/extern/WarpRna/warp-rna/core.cu`

 * *Files identical despite different names*

### Comparing `returnn-1.20230503.142906/returnn/extern/WarpRna/warp-rna/core.h` & `returnn-1.20230504.150134/returnn/extern/WarpRna/warp-rna/core.h`

 * *Files identical despite different names*

### Comparing `returnn-1.20230503.142906/returnn/extern/WarpRna/warp-rna/core_cpu.cpp` & `returnn-1.20230504.150134/returnn/extern/WarpRna/warp-rna/core_cpu.cpp`

 * *Files identical despite different names*

### Comparing `returnn-1.20230503.142906/returnn/extern/WarpRna/warp-rna/pytorch_binding/LICENSE` & `returnn-1.20230504.150134/returnn/extern/WarpRna/warp-rna/pytorch_binding/LICENSE`

 * *Files identical despite different names*

### Comparing `returnn-1.20230503.142906/returnn/extern/WarpRna/warp-rna/pytorch_binding/README.md` & `returnn-1.20230504.150134/returnn/extern/WarpRna/warp-rna/pytorch_binding/README.md`

 * *Files identical despite different names*

### Comparing `returnn-1.20230503.142906/returnn/extern/WarpRna/warp-rna/pytorch_binding/binding.cpp` & `returnn-1.20230504.150134/returnn/extern/WarpRna/warp-rna/pytorch_binding/binding.cpp`

 * *Files identical despite different names*

### Comparing `returnn-1.20230503.142906/returnn/extern/WarpRna/warp-rna/pytorch_binding/core.cu` & `returnn-1.20230504.150134/returnn/extern/WarpRna/warp-rna/pytorch_binding/core.cu`

 * *Files identical despite different names*

### Comparing `returnn-1.20230503.142906/returnn/extern/WarpRna/warp-rna/pytorch_binding/core.h` & `returnn-1.20230504.150134/returnn/extern/WarpRna/warp-rna/pytorch_binding/core.h`

 * *Files identical despite different names*

### Comparing `returnn-1.20230503.142906/returnn/extern/WarpRna/warp-rna/pytorch_binding/setup.py` & `returnn-1.20230504.150134/returnn/extern/WarpRna/warp-rna/pytorch_binding/setup.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230503.142906/returnn/extern/WarpRna/warp-rna/pytorch_binding/warp_rna/__init__.py` & `returnn-1.20230504.150134/returnn/extern/WarpRna/warp-rna/pytorch_binding/warp_rna/__init__.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230503.142906/returnn/extern/WarpRna/warp-rna/pytorch_binding/warp_rna/test.py` & `returnn-1.20230504.150134/returnn/extern/WarpRna/warp-rna/pytorch_binding/warp_rna/test.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230503.142906/returnn/extern/WarpRna/warp-rna/ref_rna.py` & `returnn-1.20230504.150134/returnn/extern/WarpRna/warp-rna/ref_rna.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230503.142906/returnn/extern/WarpRna/warp-rna/tensorflow_binding/setup.py` & `returnn-1.20230504.150134/returnn/extern/WarpRna/warp-rna/tensorflow_binding/setup.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230503.142906/returnn/extern/WarpRna/warp-rna/tensorflow_binding/src/warp_rna_op.cc` & `returnn-1.20230504.150134/returnn/extern/WarpRna/warp-rna/tensorflow_binding/src/warp_rna_op.cc`

 * *Files identical despite different names*

### Comparing `returnn-1.20230503.142906/returnn/extern/WarpRna/warp-rna/tensorflow_binding/src/warp_rna_op_kernel_tmpl.h` & `returnn-1.20230504.150134/returnn/extern/WarpRna/warp-rna/tensorflow_binding/src/warp_rna_op_kernel_tmpl.h`

 * *Files identical despite different names*

### Comparing `returnn-1.20230503.142906/returnn/extern/WarpRna/warp-rna/tensorflow_binding/warp_rna/__init__.py` & `returnn-1.20230504.150134/returnn/extern/WarpRna/warp-rna/tensorflow_binding/warp_rna/__init__.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230503.142906/returnn/extern/WarpRna/warp-rna/test.cpp` & `returnn-1.20230504.150134/returnn/extern/WarpRna/warp-rna/test.cpp`

 * *Files identical despite different names*

### Comparing `returnn-1.20230503.142906/returnn/extern/graph_editor/__init__.py` & `returnn-1.20230504.150134/returnn/extern/graph_editor/__init__.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230503.142906/returnn/extern/graph_editor/edit.py` & `returnn-1.20230504.150134/returnn/extern/graph_editor/edit.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230503.142906/returnn/extern/graph_editor/reroute.py` & `returnn-1.20230504.150134/returnn/extern/graph_editor/reroute.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230503.142906/returnn/extern/graph_editor/select.py` & `returnn-1.20230504.150134/returnn/extern/graph_editor/select.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230503.142906/returnn/extern/graph_editor/subgraph.py` & `returnn-1.20230504.150134/returnn/extern/graph_editor/subgraph.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230503.142906/returnn/extern/graph_editor/transform.py` & `returnn-1.20230504.150134/returnn/extern/graph_editor/transform.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230503.142906/returnn/extern/graph_editor/util.py` & `returnn-1.20230504.150134/returnn/extern/graph_editor/util.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230503.142906/returnn/frontend/__init__.py` & `returnn-1.20230504.150134/returnn/frontend/__init__.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230503.142906/returnn/frontend/_backend.py` & `returnn-1.20230504.150134/returnn/frontend/_backend.py`

 * *Files 1% similar despite different names*

```diff
@@ -259,14 +259,19 @@
         :return: shape[axis] expands to dim.
             in PyTorch or other frameworks which support custom strides,
             this is an efficient view and not a copy.
         """
         raise NotImplementedError
 
     @staticmethod
+    def copy(tensor: Tensor) -> Tensor:
+        """copy"""
+        raise NotImplementedError
+
+    @staticmethod
     def cast_raw(raw_tensor: T, dtype: str) -> T:
         """
         :param raw_tensor:
         :param dtype: e.g. "float32"
         :return: raw tensor with dtype casted
         """
         raise NotImplementedError
@@ -595,14 +600,23 @@
         """
         :param param: parameter
         :param trainable: whether the parameter should be trainable
         """
         raise NotImplementedError
 
     @staticmethod
+    def parameter_assign(param: rf.Parameter, value: Tensor, op: str = "assign") -> None:
+        """
+        :param param: parameter
+        :param value: new value
+        :param op: "assign" or "add"
+        """
+        raise NotImplementedError
+
+    @staticmethod
     def runtime_sanity_checks(tensor: Tensor) -> Any:
         """
         Checks whether the tensor.raw_tensor is consistent with the tensor metadata.
 
         In graph-based frameworks (TF graph), we return some operation here.
         In eager frameworks, we would not return anything but instead directly perform the checks.
         """
@@ -1057,49 +1071,55 @@
 
     if not isinstance(tensor_type, type):
         raise TypeError(f"Expected type, got {tensor_type!r} of type {type(tensor_type)}")
     tensor_type: Type[T]
 
     # We don't register all possible subclasses in the dispatch table.
     # Check through the MRO.
-    for type_ in tensor_type.__mro__:
-        if type_ in _dispatch_table:
+    for base_type in tensor_type.__mro__:
+        if base_type in _dispatch_table:
             # Also register it for faster future lookups.
-            register_backend_by_tensor_type(tensor_type, _dispatch_table[type_])
-            return _dispatch_table[type_]
+            register_backend_by_tensor_type(tensor_type, _dispatch_table[base_type])
+            return _dispatch_table[base_type]
 
     # It would be registered if there was any select_engine or select_backend_* call.
     # However, some code might not have done that, so for the common cases,
     # we do it here.
-    if tensor_type.__module__.split(".")[0] == "tensorflow":
-        from returnn.tf.frontend_low_level import TFBackend
+    for base_type in tensor_type.__mro__:
+        if base_type.__module__.split(".")[0] == "tensorflow":
+            from returnn.tf.frontend_low_level import TFBackend
+
+            backend_type = TFBackend
+            tensor_types = _get_tensor_types_tf()
+        elif base_type.__module__.split(".")[0] == "torch":
+            from returnn.torch.frontend import TorchBackend
+
+            backend_type = TorchBackend
+            tensor_types = _get_tensor_types_torch()
+        elif base_type.__module__.startswith("returnn.tf.frontend_layers."):
+            from returnn.tf.frontend_layers import ReturnnLayersBackend, Layer
+
+            backend_type = ReturnnLayersBackend
+            tensor_types = (Layer,)
+        elif issubclass(base_type, numpy.ndarray):
+            from ._numpy_backend import NumpyBackend
+
+            backend_type = NumpyBackend
+            tensor_types = (numpy.ndarray,)
+        else:
+            continue
+
+        assert any(
+            issubclass(base_type, type_) for type_ in tensor_types
+        ), f"tensor type {tensor_type} base_type {base_type} not in {tensor_types}, expected for backend {backend_type}"
+        for base_type_ in tensor_types:
+            register_backend_by_tensor_type(base_type_, backend_type)
+        return backend_type
 
-        backend_type = TFBackend
-        tensor_types = _get_tensor_types_tf()
-    elif tensor_type.__module__.split(".")[0] == "torch":
-        from returnn.torch.frontend import TorchBackend
-
-        backend_type = TorchBackend
-        tensor_types = _get_tensor_types_torch()
-    elif tensor_type.__module__.startswith("returnn.tf.frontend_layers."):
-        from returnn.tf.frontend_layers import ReturnnLayersBackend, Layer
-
-        backend_type = ReturnnLayersBackend
-        tensor_types = (Layer,)
-    elif issubclass(tensor_type, numpy.ndarray):
-        from ._numpy_backend import NumpyBackend
-
-        backend_type = NumpyBackend
-        tensor_types = (numpy.ndarray,)
-    else:
-        raise TypeError(f"unknown tensor type {tensor_type}")
-    assert any(issubclass(tensor_type, type_) for type_ in tensor_types)
-    for type_ in tensor_types:
-        register_backend_by_tensor_type(type_, backend_type)
-    return backend_type
+    raise TypeError(f"unknown tensor type {tensor_type} with mro {tensor_type.__mro__}")
 
 
 def register_backend_by_tensor_type(tensor_type: Type[T], backend: Type[Backend[T]]):
     """
     :param tensor_type:
     :param backend:
     """
```

### Comparing `returnn-1.20230503.142906/returnn/frontend/_numpy_backend.py` & `returnn-1.20230504.150134/returnn/frontend/_numpy_backend.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230503.142906/returnn/frontend/_utils.py` & `returnn-1.20230504.150134/returnn/frontend/_utils.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230503.142906/returnn/frontend/array_.py` & `returnn-1.20230504.150134/returnn/frontend/array_.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 from .types import RawTensorTypes
 
 T = TypeVar("T")
 
 __all__ = [
     "convert_to_tensor",
     "constant",
+    "copy",
     "cast",
     "merge_dims",
     "split_dims",
     "reshape",
     "split",
     "expand_dim",
     "concat",
@@ -94,14 +95,27 @@
             dtype = value_backend.get_dtype_name_raw(value)
     return _backend.convert_to_tensor(value=value, dims=dims, dtype=dtype, sparse_dim=sparse_dim, name=name)
 
 
 constant = convert_to_tensor  # alias for some older code
 
 
+def copy(tensor: Tensor) -> Tensor:
+    """
+    :param tensor:
+    :return: copy of tensor.
+        In eager-based frameworks, it is really a copy.
+        In graph-based frameworks, it might be just a copied reference if it would be immutable.
+        This is really only relevant when operating on tensors which can conceptually be mutated,
+        such as variables (:class:`Parameter`).
+    """
+    # noinspection PyProtectedMember
+    return tensor._raw_backend.copy(tensor)
+
+
 def cast(tensor: Tensor, dtype: str) -> Tensor:
     """
     :param tensor:
     :param dtype:
     :return: tensor with the same data, but with a different dtype
     """
     # noinspection PyProtectedMember
```

### Comparing `returnn-1.20230503.142906/returnn/frontend/attention.py` & `returnn-1.20230504.150134/returnn/frontend/attention.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230503.142906/returnn/frontend/cond.py` & `returnn-1.20230504.150134/returnn/frontend/cond.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230503.142906/returnn/frontend/const.py` & `returnn-1.20230504.150134/returnn/frontend/const.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230503.142906/returnn/frontend/container.py` & `returnn-1.20230504.150134/returnn/frontend/container.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230503.142906/returnn/frontend/conv.py` & `returnn-1.20230504.150134/returnn/frontend/conv.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230503.142906/returnn/frontend/device.py` & `returnn-1.20230504.150134/returnn/frontend/device.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230503.142906/returnn/frontend/dims.py` & `returnn-1.20230504.150134/returnn/frontend/dims.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230503.142906/returnn/frontend/dropout.py` & `returnn-1.20230504.150134/returnn/frontend/dropout.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230503.142906/returnn/frontend/dtype.py` & `returnn-1.20230504.150134/returnn/frontend/dtype.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230503.142906/returnn/frontend/encoder/base.py` & `returnn-1.20230504.150134/returnn/frontend/encoder/base.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230503.142906/returnn/frontend/encoder/conformer.py` & `returnn-1.20230504.150134/returnn/frontend/encoder/conformer.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230503.142906/returnn/frontend/init.py` & `returnn-1.20230504.150134/returnn/frontend/init.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230503.142906/returnn/frontend/linear.py` & `returnn-1.20230504.150134/returnn/frontend/linear.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230503.142906/returnn/frontend/loop.py` & `returnn-1.20230504.150134/returnn/frontend/loop.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230503.142906/returnn/frontend/loss.py` & `returnn-1.20230504.150134/returnn/frontend/loss.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230503.142906/returnn/frontend/math_.py` & `returnn-1.20230504.150134/returnn/frontend/math_.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230503.142906/returnn/frontend/matmul.py` & `returnn-1.20230504.150134/returnn/frontend/matmul.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230503.142906/returnn/frontend/module.py` & `returnn-1.20230504.150134/returnn/frontend/module.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230503.142906/returnn/frontend/normalization.py` & `returnn-1.20230504.150134/returnn/frontend/normalization.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230503.142906/returnn/frontend/parameter.py` & `returnn-1.20230504.150134/returnn/frontend/parameter.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
 Parameter / variable
 """
 
 from __future__ import annotations
-from typing import Optional, TypeVar, Sequence
+from typing import Optional, Union, TypeVar, Sequence
 from returnn.tensor import Tensor, Dim
 import returnn.frontend as rf
 from ._backend import global_backend as _global_backend
 
 
 __all__ = ["Parameter"]
 
@@ -111,14 +111,35 @@
         # https://github.com/rwth-i6/returnn_common/issues/216
         self._initial = value
 
         if isinstance(value, rf.init.ParamInit):
             value = value(dims=self.dims, dtype=self.dtype)
         self._raw_backend.set_parameter_initial_value(self, value)
 
+    def assign(self, value: Union[Tensor, rf.RawTensorTypes]):
+        """
+        Assign new value to this parameter.
+        This will also update the allocated raw tensor inplace.
+
+        For graph-based backends, handling the control flow is up to the backend,
+        e.g.~making sure it is being executed in the right order,
+        in the right control flow context, and at all.
+        There is no op or anything like that returned here which the user needs to take care of.
+        So the user can think of it just as imperative eager-style code.
+        """
+        self._raw_backend.parameter_assign(self, rf.convert_to_tensor(value, _backend=self._raw_backend), op="assign")
+
+    def assign_add(self, value: Union[Tensor, rf.RawTensorTypes]):
+        """
+        Add value to this parameter.
+        This will also update the raw tensor.
+        See :func:`assign`.
+        """
+        self._raw_backend.parameter_assign(self, rf.convert_to_tensor(value, _backend=self._raw_backend), op="add")
+
     @property
     def weight_decay(self) -> float:
         """
         Weight decay, which is equivalent to L2 loss on the parameters for SGD.
         On RETURNN side, whether this is handled separately or is part of the main loss,
         can be controlled via the ``decouple_constraints`` config option.
         https://github.com/rwth-i6/returnn_common/issues/59#issuecomment-1073913421
```

### Comparing `returnn-1.20230503.142906/returnn/frontend/rand.py` & `returnn-1.20230504.150134/returnn/frontend/rand.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230503.142906/returnn/frontend/rec.py` & `returnn-1.20230504.150134/returnn/frontend/rec.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230503.142906/returnn/frontend/reduce.py` & `returnn-1.20230504.150134/returnn/frontend/reduce.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230503.142906/returnn/frontend/run_ctx.py` & `returnn-1.20230504.150134/returnn/frontend/run_ctx.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230503.142906/returnn/frontend/signal.py` & `returnn-1.20230504.150134/returnn/frontend/signal.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230503.142906/returnn/frontend/state.py` & `returnn-1.20230504.150134/returnn/frontend/state.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230503.142906/returnn/frontend/types.py` & `returnn-1.20230504.150134/returnn/frontend/types.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230503.142906/returnn/import_/common.py` & `returnn-1.20230504.150134/returnn/import_/common.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230503.142906/returnn/import_/git.py` & `returnn-1.20230504.150134/returnn/import_/git.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230503.142906/returnn/import_/import_.py` & `returnn-1.20230504.150134/returnn/import_/import_.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230503.142906/returnn/learning_rate_control.py` & `returnn-1.20230504.150134/returnn/learning_rate_control.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230503.142906/returnn/log.py` & `returnn-1.20230504.150134/returnn/log.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230503.142906/returnn/native_op.cpp` & `returnn-1.20230504.150134/returnn/native_op.cpp`

 * *Files identical despite different names*

### Comparing `returnn-1.20230503.142906/returnn/native_op.py` & `returnn-1.20230504.150134/returnn/native_op.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230503.142906/returnn/pretrain.py` & `returnn-1.20230504.150134/returnn/pretrain.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230503.142906/returnn/sprint/cache.py` & `returnn-1.20230504.150134/returnn/sprint/cache.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230503.142906/returnn/sprint/control.py` & `returnn-1.20230504.150134/returnn/sprint/control.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230503.142906/returnn/sprint/error_signals.py` & `returnn-1.20230504.150134/returnn/sprint/error_signals.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230503.142906/returnn/sprint/extern_interface.py` & `returnn-1.20230504.150134/returnn/sprint/extern_interface.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230503.142906/returnn/sprint/interface.py` & `returnn-1.20230504.150134/returnn/sprint/interface.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230503.142906/returnn/tensor/_dim_extra.py` & `returnn-1.20230504.150134/returnn/tensor/_dim_extra.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230503.142906/returnn/tensor/_tensor_extra.py` & `returnn-1.20230504.150134/returnn/tensor/_tensor_extra.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230503.142906/returnn/tensor/_tensor_mixin_base.py` & `returnn-1.20230504.150134/returnn/tensor/_tensor_mixin_base.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230503.142906/returnn/tensor/_tensor_op_overloads.py` & `returnn-1.20230504.150134/returnn/tensor/_tensor_op_overloads.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230503.142906/returnn/tensor/control_flow_ctx.py` & `returnn-1.20230504.150134/returnn/tensor/control_flow_ctx.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230503.142906/returnn/tensor/dim.py` & `returnn-1.20230504.150134/returnn/tensor/dim.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230503.142906/returnn/tensor/marked_dim.py` & `returnn-1.20230504.150134/returnn/tensor/marked_dim.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230503.142906/returnn/tensor/tensor.py` & `returnn-1.20230504.150134/returnn/tensor/tensor.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230503.142906/returnn/tensor/tensor_dict.py` & `returnn-1.20230504.150134/returnn/tensor/tensor_dict.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230503.142906/returnn/tf/compat.py` & `returnn-1.20230504.150134/returnn/tf/compat.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230503.142906/returnn/tf/data_pipeline.py` & `returnn-1.20230504.150134/returnn/tf/data_pipeline.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230503.142906/returnn/tf/distributed.py` & `returnn-1.20230504.150134/returnn/tf/distributed.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230503.142906/returnn/tf/engine.py` & `returnn-1.20230504.150134/returnn/tf/engine.py`

 * *Files 0% similar despite different names*

```diff
@@ -1151,15 +1151,15 @@
         """
         if not config:
             config = self.config
         if self._have_rf_get_model_func:
             assert BackendEngine.get_selected_engine() == BackendEngine.TensorFlowNetDict  # not implemented otherwise
             assert not self.pretrain  # the RF API uses a different pretrain mechanism
             assert epoch is not None and step is not None
-            net_dict = rfl.get_net_dict(epoch=epoch, step=step)
+            net_dict, _ = rfl.get_net_dict(epoch=epoch, step=step)
         elif self.is_pretrain_epoch(epoch=epoch):
             # This would be obsolete if we don't want to load an existing model.
             # In self.init_train_epoch(), we initialize a new model.
             net_dict = self.pretrain.get_network_json_for_epoch(epoch)
         elif self.custom_get_net_dict:
             net_dict = self.custom_get_net_dict(epoch=epoch)
             assert isinstance(net_dict, dict), "%s should return dict but returned %s" % (
```

### Comparing `returnn-1.20230503.142906/returnn/tf/frontend_layers/_backend.py` & `returnn-1.20230504.150134/returnn/tf/frontend_layers/_backend.py`

 * *Files 1% similar despite different names*

```diff
@@ -128,14 +128,19 @@
     @staticmethod
     def transpose(tensor: Tensor, perm: Sequence[Union[Dim, int]], *, allow_int: bool = False) -> Tensor:
         """transpose"""
         assert all(isinstance(d, Dim) for d in perm)  # axis as int not supported
         return rfl.make_layer({"class": "transpose", "from": tensor, "perm": perm}, name="transpose")
 
     @staticmethod
+    def copy(tensor: Tensor) -> Tensor:
+        """copy"""
+        return rfl.make_layer({"class": "identity", "from": tensor}, name="copy")
+
+    @staticmethod
     def cast(tensor: Tensor, dtype: str) -> Tensor:
         """cast"""
         return rfl.make_layer({"class": "cast", "from": tensor, "dtype": dtype}, name="cast")
 
     @staticmethod
     def stop_gradient(tensor: Tensor) -> Tensor:
         """stop grad"""
@@ -351,15 +356,17 @@
             log_probs = rf.log_softmax(logits, axis=axis)
             return -rf.matmul(targets, log_probs, reduce=axis)
 
     @staticmethod
     def create_parameter_raw(tensor: rf.Parameter) -> Layer:
         """create parameter"""
         return rfl.make_layer(
-            {"class": "variable", "shape": tensor.dims, "dtype": tensor.dtype}, name=tensor.name, out=tensor
+            {"class": "variable", "shape": tensor.dims, "dtype": tensor.dtype, "param_name": "param"},
+            name=tensor.name,
+            out=tensor,
         ).raw_tensor
 
     @staticmethod
     def set_parameter_initial_value(param: rf.Parameter[Layer], value: Union[None, Tensor, rf.RawTensorTypes]) -> None:
         """set parameter initial value"""
         if value is None:
             param.raw_tensor.layer_dict.pop("init", None)
@@ -402,14 +409,21 @@
         if trainable:
             # pop it, as it's the default
             param.raw_tensor.layer_dict.pop("trainable", None)
         else:
             param.raw_tensor.layer_dict["trainable"] = False
 
     @staticmethod
+    def parameter_assign(param: rf.Parameter[Layer], value: Tensor, op: str = "assign") -> None:
+        """param assign"""
+        from .parameter_assign import parameter_assign
+
+        parameter_assign(param=param, value=value, op=op)
+
+    @staticmethod
     def convert_to_tensor(
         value: Union[Tensor, Layer, RawTensorTypes],
         *,
         dims: Sequence[Dim],
         dtype: str,
         sparse_dim: Optional[Dim] = None,
         name: Optional[str] = None,
```

### Comparing `returnn-1.20230503.142906/returnn/tf/frontend_layers/_utils.py` & `returnn-1.20230504.150134/returnn/tf/frontend_layers/prev_tensor_ref.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,76 +1,54 @@
 """
-Some utilities for internal use
+prev tensor ref for loop, i.e. RecLayer, specifically "prev:..." layer references
 """
 
 from __future__ import annotations
-from typing import Optional, Union, Iterable, List
-from returnn.util.basic import NotSpecified
-from returnn.tensor import Tensor, Dim
-from returnn.util.basic import RefIdEq
+from returnn.tensor import Tensor
 from .. import frontend_layers as rfl
 
 
-def unique_tensor_list(tensors: Iterable[Tensor]) -> List[Tensor]:
-    """
-    :param list[Tensor] tensors:
-    :return: list with unique tensors
-    :rtype: list[Tensor]
-    """
-    seen = set()  # over ref, not tensor (which is not hashable)
-    out = []
-    for tensor in tensors:
-        if RefIdEq(tensor) not in seen:
-            out.append(tensor)
-            seen.add(RefIdEq(tensor))
-    return out
-
+__all__ = ["PrevTensorRef"]
 
-def copy(tensor: Tensor[rfl.Layer], *, name: Union[rfl.Layer, str]) -> Tensor[rfl.Layer]:
-    """copy"""
-    return rfl.make_layer({"class": "copy", "from": tensor}, name=name)
 
-
-def mark_as_output_in_scope(tensor: Tensor, scope: rfl.Layer) -> Tensor:
-    """
-    Mark this as an output.
+class PrevTensorRef(Tensor):
     """
-    assert tensor.raw_tensor.layer_dict, f"mark_as_output can only be called on a layer, not a layer-ref {tensor}."
-    res = tensor
-    if tensor.raw_tensor is scope.children.get("output"):
-        pass  # not needed
-    elif tensor.raw_tensor.parent is not scope:
-        res = copy(tensor, name=scope.get_new_child(suggested_name=tensor.raw_tensor.get_abs_name(join_str="_")))
-        res.raw_tensor.layer_dict["is_output_layer"] = True
-    else:
-        assert tensor.raw_tensor.parent is scope
-        assert tensor.raw_tensor.layer_dict
-        tensor.raw_tensor.layer_dict["is_output_layer"] = True
-    scope.marked_outputs.append(res)
-    return res
-
-
-def get_last_hidden_state(
-    source: Tensor,
-    *,
-    out_dim: Optional[Dim] = NotSpecified,
-    combine: str = NotSpecified,
-    key: Optional[Union[str, int]] = NotSpecified,
-) -> Tensor:
+    Refers to a layer from the previous loop iteration.
     """
-    Will combine (concat or add or so) all the last hidden states from all sources.
 
-    :param nn.Tensor source:
-    :param nn.Dim|None out_dim:
-    :param str combine: "concat" or "add"
-    :param str|int|None key: for the state, which could be a namedtuple. see :func:`RnnCellLayer.get_state_by_key`
-    :return: layer
-    """
-    if not isinstance(source, Tensor):
-        raise TypeError(f"_get_last_hidden_state: unexpected type for source {source!r}, need tensor")
-    args = {
-        "out_dim": out_dim,
-        "combine": combine,
-        "key": key,
-    }
-    args = {key: value for (key, value) in args.items() if value is not NotSpecified}
-    return rfl.make_layer({"class": "get_last_hidden_state", "from": source, **args}, name="get_last_hidden_state")
+    @classmethod
+    def get_prev_ref(cls, *, cur_layer_name_ctx: rfl.Layer, initial: Tensor) -> PrevTensorRef:
+        """
+        Create prev ref.
+        """
+        parent_name_ctx = cur_layer_name_ctx.parent
+        prev_tensor_name_ctx = parent_name_ctx.get_child(f"prev:{cur_layer_name_ctx.name}")
+        if prev_tensor_name_ctx.tensor:
+            prev_tensor_ref = prev_tensor_name_ctx.tensor
+            assert isinstance(prev_tensor_ref, PrevTensorRef)
+            assert prev_tensor_ref.cur_layer_name_ctx is cur_layer_name_ctx
+        else:
+            prev_tensor_ref = PrevTensorRef(
+                name_ctx=prev_tensor_name_ctx, cur_layer_name_ctx=cur_layer_name_ctx, data=initial
+            )
+            assert prev_tensor_name_ctx.tensor is prev_tensor_ref
+        return prev_tensor_ref
+
+    def __init__(self, *, name_ctx: rfl.Layer, cur_layer_name_ctx: rfl.Layer, data: Tensor):
+        # At the time we instantiate this, cur_layer_name_ctx.tensor probably does not exist yet.
+        super().__init__(**data.get_kwargs())
+        self.raw_tensor = name_ctx
+        self.cur_layer_name_ctx = cur_layer_name_ctx
+        self.raw_tensor.layer_extra_dependencies.append(self.cur_layer_name_ctx)
+
+    def assign_new_cur_tensor_name_ctx(self, cur_tensor_name_ctx: rfl.Layer):
+        """
+        Changes self.name_ctx to new name_ctx.
+        """
+        self.raw_tensor.layer_extra_dependencies.remove(self.cur_layer_name_ctx)
+        prev_layer_name = f"prev:{cur_tensor_name_ctx.name}"
+        assert prev_layer_name not in cur_tensor_name_ctx.parent.children
+        prev_layer_name_ctx = cur_tensor_name_ctx.parent.get_child(prev_layer_name)
+        prev_layer_name_ctx.move_tensor_here(self)
+        assert self.raw_tensor is prev_layer_name_ctx
+        self.cur_layer_name_ctx = cur_tensor_name_ctx
+        self.raw_tensor.layer_extra_dependencies.append(self.cur_layer_name_ctx)
```

### Comparing `returnn-1.20230503.142906/returnn/tf/frontend_layers/cond.py` & `returnn-1.20230504.150134/returnn/tf/frontend_layers/cond.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """
 Conditional logic
 
 https://github.com/rwth-i6/returnn_common/issues/24
 """
 
 from __future__ import annotations
-from typing import List, TypeVar, Generic
+from typing import Any, List, TypeVar, Generic, Callable
 from tensorflow.python.util import nest
 from returnn.tensor import Tensor, ControlFlowContext
 import returnn.frontend as rf
 import returnn.tf.frontend_layers as rfl
 from . import _utils
 
 
@@ -45,15 +45,17 @@
     """
 
     def __init__(self, condition: Tensor, *, name: str = "cond"):
         self.condition = condition
         self._entered = False
         self._entered_state = True
         self._true_value = None
+        self._true_value_set = False
         self._false_value = None
+        self._false_value_set = False
         self._result_value = None
         self.layer_module = CondModule(cond=self)
         self.name_ctx = rfl.Layer(
             module=self.layer_module, suggested_name=name, parent=rfl.Layer.current_ctx(), can_access_children=False
         )
         self.name_ctx.custom_layer_name_scope = ""
         self.true_branch_control_flow_ctx = ControlFlowContext(
@@ -78,14 +80,18 @@
             parent=self.name_ctx,
             virtual=True,
             can_access_children=False,
             new_control_flow_ctx=self.false_branch_control_flow_ctx,
         )
         self.false_branch_name_ctx.is_subnet = True
         self.false_branch_name_ctx.extend_reserved_names({"output"})
+        self._extra_ops_true_branch: List[Tensor] = []
+        self._extra_ops_false_branch: List[Tensor] = []
+        self._false_branch_prehooks: List[Callable[[], Any]] = []
+        self._false_branch_posthooks: List[Callable[[], Any]] = []
 
     def __repr__(self):
         return f"Cond{self.name_ctx}"
 
     def __enter__(self):
         assert not self._entered, f"{self} cannot enter twice"
         self._entered = True
@@ -118,32 +124,48 @@
         """
         Defines the True branch value.
         Enter the False branch.
         Assign self.false afterwards.
         """
         assert self._entered, f"{self} you need to be in the context scope"
         assert self._entered_state is True, f"{self} you cannot enter the else branch twice"
-        assert true_value is not None
-        assert self._true_value is None
+        assert not self._true_value_set
         if isinstance(true_value, Tensor):
             true_value = _utils.copy(true_value, name=self.true_branch_name_ctx.get_child("output"))
         else:
             values_flat = nest.flatten(true_value)  # type: List[Tensor]
             assert values_flat
             for i, v in enumerate(values_flat):
+                if v is None:
+                    # Dummy value.
+                    # Allow this in case the whole output is just None.
+                    # Maybe there were other side effects.
+                    v = rf.zeros((), dtype="int32")
                 assert isinstance(v, Tensor), f"unexpected {true_value!r}, only expects tensors, got {type(v)}"
                 if i == 0:
                     values_flat[i] = _utils.copy(v, name=self.true_branch_name_ctx.get_child("output"))
                 else:
                     values_flat[i] = _utils.mark_as_output_in_scope(v, scope=self.true_branch_name_ctx)
+            if len(values_flat) == 0:
+                # maybe there are just ops with side effects, maybe also only in the other branch
+                # dummy output
+                _utils.copy(rf.zeros((), dtype="int32"), name=self.true_branch_name_ctx.get_child("output"))
             true_value = nest.pack_sequence_as(true_value, values_flat)
+        for op in self._extra_ops_true_branch:
+            _utils.mark_as_output_in_scope(op, scope=self.true_branch_name_ctx)
         self.true_branch_name_ctx.__exit__(None, None, None)
         self.false_branch_name_ctx.__enter__()
+        self.false_branch_name_ctx.extend_reserved_names(
+            {v.raw_tensor.name for v in self.true_branch_name_ctx.marked_outputs}
+        )
         self._true_value = true_value
+        self._true_value_set = True
         self._entered_state = False
+        for hook in self._false_branch_prehooks:
+            hook()
 
     @property
     def false(self) -> T:
         """
         The getter usually would not be used.
         """
         return self._false_value
@@ -154,49 +176,88 @@
         Define the False branch value.
         After this, self.result is available.
         """
         assert self._entered, f"{self} you need to be in the context scope"
         assert (
             self._entered_state is False
         ), f"{self} you need to be in the False branch, have assigned :func:`true` before"
-        assert false_value is not None
-        assert self._false_value is None
+        assert not self._false_value_set
         nest.assert_same_structure(self._true_value, false_value)
         # This needs to match the true() setter logic.
         if isinstance(false_value, Tensor):
             false_value = _utils.copy(false_value, name=self.false_branch_name_ctx.get_child("output"))
         else:
             true_values_flat = nest.flatten(self._true_value)  # type: List[Tensor]
             false_values_flat = nest.flatten(false_value)  # type: List[Tensor]
             assert false_values_flat and len(false_values_flat) == len(true_values_flat)
             for i, (true_v, false_v) in enumerate(zip(true_values_flat, false_values_flat)):
                 assert isinstance(true_v, Tensor)
-                assert isinstance(
-                    false_v, Tensor
-                ), f"unexpected {false_value!r}, only expects tensors, got {type(false_v)}"
+                if false_v is None:  # see above
+                    false_v = rf.zeros((), dtype="int32")  # dummy value
+                else:
+                    assert isinstance(
+                        false_v, Tensor
+                    ), f"unexpected {false_value!r}, only expects tensors, got {type(false_v)}"
                 assert true_v.raw_tensor.parent is self.true_branch_name_ctx
                 name = true_v.raw_tensor.name
+                assert name not in self.false_branch_name_ctx.children
                 false_values_flat[i] = _utils.copy(false_v, name=self.false_branch_name_ctx.get_child(name))
                 if name != "output":
                     false_values_flat[i].raw_tensor.layer_dict["is_output_layer"] = True
+            if len(false_values_flat) == 0:
+                # Same as in true branch, see above.
+                _utils.copy(rf.zeros((), dtype="int32"), name=self.true_branch_name_ctx.get_child("output"))
             false_value = nest.pack_sequence_as(false_value, false_values_flat)
+        for true_out in self.true_branch_name_ctx.marked_outputs:
+            name = true_out.raw_tensor.name
+            if name in self.false_branch_name_ctx.children:
+                continue
+            _utils.zeros_like_as_output_in_scope(true_out, name=self.false_branch_name_ctx.get_child(name))
+        for op in self._extra_ops_false_branch:
+            op = _utils.mark_as_output_in_scope(op, scope=self.false_branch_name_ctx)
+            name = op.raw_tensor.name
+            assert name not in self.true_branch_name_ctx.children
+            _utils.zeros_like_as_output_in_scope(op, name=self.true_branch_name_ctx.get_child(name))
         self.false_branch_name_ctx.__exit__(None, None, None)
         self._false_value = false_value
+        self._false_value_set = True
+        for cb in self._false_branch_posthooks:
+            cb()
         self._result_value = self.layer_module()
 
     @property
     def result(self) -> T:
         """
         :return: the result, after you assigned :func:`true` and :func:`false`.
         """
-        assert self._true_value is not None, f"{self} you need to have defined the true value"
-        assert self._false_value is not None, f"{self} you need to have defined the false value"
-        assert self._result_value is not None
+        assert self._true_value_set, f"{self} you need to have defined the true value"
+        assert self._false_value_set, f"{self} you need to have defined the false value"
         return self._result_value
 
+    def add_op_to_current_branch(self, op: Tensor):
+        """
+        :param op: like an assign_op. the value of the tensor is irrelevant, the underlying op is relevant
+        """
+        assert self._entered, f"{self} you need to be in the context scope"
+        (self._extra_ops_true_branch if self._entered_state else self._extra_ops_false_branch).append(op)
+
+    def add_other_branch_prehook(self, callback: Callable[[], Any]):
+        """add prehook to the other branch"""
+        assert self._entered, f"{self} you need to be in the context scope"
+        if not self._entered_state:
+            return  # already in false branch, will not enter any other branch
+        self._false_branch_prehooks.insert(0, callback)
+
+    def add_other_branch_posthook(self, callback: Callable[[], Any]):
+        """add posthook to the other branch"""
+        assert self._entered, f"{self} you need to be in the context scope"
+        if not self._entered_state:
+            return  # already in false branch, will not enter any other branch
+        self._false_branch_posthooks.append(callback)
+
 
 class CondModule(rf.Module):
     """
     This module is used internally by :class:`Cond` to create the RETURNN :class:`CondLayer` for the conditional code.
     This module would not be directly used by the user.
     """
 
@@ -229,24 +290,42 @@
                 "false_layer": {
                     "class": "subnetwork",
                     "from": [],
                     "subnetwork": self.cond.false_branch_name_ctx.make_net(),
                 },
             },
             name=name_ctx,
-            predefined_out_data=true_values_flat[0].copy_template(),
+            predefined_out_data=true_values_flat[0].copy_template()
+            if true_values_flat
+            else Tensor("dummy", (), "int32"),
         )
 
-        results = []
-        for i, (true_v, false_v) in enumerate(zip(true_values_flat, false_values_flat)):
-            assert isinstance(true_v, Tensor) and isinstance(false_v, Tensor)
-            assert true_v.raw_tensor.parent is self.cond.true_branch_name_ctx
-            name = true_v.raw_tensor.name
-            if i == 0:
-                results.append(res)
-            else:
-                # noinspection PyProtectedMember
-                results.append(rfl._get_sub_layer(res, name, data=true_v.copy_template()))
-            results[-1].raw_tensor.layer_extra_dependencies.extend(
-                (self.cond.condition.raw_tensor, true_v.raw_tensor, false_v.raw_tensor)
-            )
-        return nest.pack_sequence_as(true_value, results)
+        if true_values_flat:
+            results = []
+            for i, (true_v, false_v) in enumerate(zip(true_values_flat, false_values_flat)):
+                assert isinstance(true_v, Tensor) and isinstance(false_v, Tensor)
+                assert true_v.raw_tensor.parent is self.cond.true_branch_name_ctx
+                name = true_v.raw_tensor.name
+                if i == 0:
+                    results.append(res)
+                else:
+                    # noinspection PyProtectedMember
+                    results.append(rfl._get_sub_layer(res, name, data=true_v.copy_template()))
+                results[-1].raw_tensor.layer_extra_dependencies.extend(
+                    (self.cond.condition.raw_tensor, true_v.raw_tensor, false_v.raw_tensor)
+                )
+            res = nest.pack_sequence_as(true_value, results)
+            if not results:
+                results = [res]
+        else:
+            results = [res]
+
+        # noinspection PyProtectedMember
+        if self.cond._extra_ops_true_branch or self.cond._extra_ops_false_branch:
+            # Make sure this is registered as output layer.
+            assert not name_ctx.inner_control_flow()  # not implemented
+            out = results[0]
+            out = _utils.copy(out, name=name_ctx.root.get_new_child(out.name))
+            out.raw_tensor.layer_dict["is_output_layer"] = True
+            name_ctx.root.marked_outputs.append(out)
+
+        return res
```

### Comparing `returnn-1.20230503.142906/returnn/tf/frontend_layers/config_entry_points.py` & `returnn-1.20230504.150134/returnn/tf/frontend_layers/config_entry_points.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 Functions to get the network dict based on the config
 via the API get_model, train_step, forward_step.
 
 https://github.com/rwth-i6/returnn/issues/1120
 """
 
 from __future__ import annotations
-from typing import Any, Dict
+from typing import Any, Dict, Tuple
 from tensorflow.python.util import nest
 from returnn.util.basic import BehaviorVersion
 from returnn.tensor import TensorDict, Tensor, Dim
 from returnn.config import get_global_config
 import returnn.frontend as rf
 from .. import frontend_layers as rfl
 from . import _utils
@@ -19,15 +19,15 @@
 __all__ = ["get_net_dict"]
 
 
 def get_net_dict(
     *,
     epoch: int,
     step: int,
-) -> Dict[str, Any]:
+) -> Tuple[Dict[str, Any], rf.Module]:
     """called from the RETURNN config"""
     BehaviorVersion.set_min_behavior_version(rfl.min_returnn_behavior_version)
     rf.select_backend_returnn_layers_tf()
     rfl.Layer.reset_default_root()
 
     config = get_global_config()
 
@@ -106,8 +106,8 @@
             # but now the TF engine actually wants to have Tensor[tf.Tensor].
             # Reset it now. The TF engine should redefine it again.
             if elem.dyn_size_ext:
                 elem.dyn_size_ext.raw_tensor = None
         return elem
 
     net_dict = nest.map_structure(_cleanup_net_dict_value, net_dict)
-    return net_dict
+    return net_dict, model
```

### Comparing `returnn-1.20230503.142906/returnn/tf/frontend_layers/debug_eager_mode.py` & `returnn-1.20230504.150134/returnn/tf/frontend_layers/debug_eager_mode.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230503.142906/returnn/tf/frontend_layers/dims.py` & `returnn-1.20230504.150134/returnn/tf/frontend_layers/dims.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230503.142906/returnn/tf/frontend_layers/layer.py` & `returnn-1.20230504.150134/returnn/tf/frontend_layers/layer.py`

 * *Files 1% similar despite different names*

```diff
@@ -143,27 +143,28 @@
         Use :func:`NameCtx.new_root` or :func:`scoped`.
         """
         self.module = module
         self.tensor = None  # type: Optional[Tensor]
         self.tensor_remove_unused_cleanup_hooks = []  # type: List[Callable[[Tensor], None]]
         self.layer_dict = None  # type: Optional[LayerDictRaw]
         self.layer_extra_dependencies = []  # type: List[Layer]
+        self.usages = []  # type: List[Layer]
         self.debug_layer = None  # type: Optional[LayerBase]
         self._enter_stack_frames = None  # type: Optional[Set[types.FrameType]]
         self.is_subnet = False  # it says whether it can have children
         self._subnet_main_output = None  # type: Optional[Tensor]  # when this is via SubnetworkLayer
         self.virtual = virtual  # does not consume a layer name in RETURNN. see get_name_in_ctx
         self.can_access_children = can_access_children  # from outside
         self.require_global_access = False  # from outside
         self.new_control_flow_ctx = new_control_flow_ctx
         self.children = {}  # type: Dict[str, Layer]
         self.extern_data = {}  # type: Dict[str, Tensor]  # only for the root name ctx
         self.global_batch = None  # type: Optional[BatchInfo]  # only for the root name ctx
         self.extra_net_dict = {}  # type: Dict[str, Any]  # only for the root name ctx
-        self.marked_outputs = []  # type: List[Tensor]
+        self.marked_outputs = []  # type: List[Tensor[rfl.Layer]]
         self.marked_losses = []  # type: List[Tensor]
         self.parent = parent if parent is not NotSpecified else self.current_ctx()
         self.name = name  # early assign such that debug repr works later
         if not name:
             if suggested_name:
                 name = self._get_unique_name(suggested_name)
             elif self.parent:
@@ -221,32 +222,35 @@
         self.parent._add_child(self)
 
     def move_tensor_here(self: Layer, tensor: Tensor):
         """
         Moves an existing layer ref (with assigned name ctx)
         to another name ctx (without assigned layer or layer ref).
 
-        This assumes that there are no other references to tensor.name_ctx
+        This assumes that there are no other references to tensor.raw_tensor
         because those would become invalid.
         References to tensor itself should be fine.
         """
         assert not self.layer_dict and not self.tensor  # none yet assigned
+        assert tensor.raw_tensor is not None
+        assert isinstance(tensor.raw_tensor, Layer)
 
         # Remove tensor.name_ctx from its parent name ctx.
         if tensor.raw_tensor.parent:
             old_name_ctx = tensor.raw_tensor.parent.children.pop(tensor.raw_tensor.name)
             assert old_name_ctx is tensor.raw_tensor
-        old_name_ctx = tensor.raw_tensor  # type: Layer
+        old_name_ctx: Layer = tensor.raw_tensor
 
         # Now reassign.
         tensor.raw_tensor = self
         self.tensor = tensor
         self.tensor_remove_unused_cleanup_hooks = old_name_ctx.tensor_remove_unused_cleanup_hooks
         self.layer_dict = old_name_ctx.layer_dict
         self.layer_extra_dependencies = old_name_ctx.layer_extra_dependencies
+        self.usages = old_name_ctx.usages
         self.is_subnet = old_name_ctx.is_subnet
         self._subnet_main_output = old_name_ctx._subnet_main_output
         for name, child in old_name_ctx.children.items():
             child.parent = self
             if name not in self.children:
                 self.children[name] = child
             else:
@@ -310,14 +314,15 @@
         """
         # Do not update inplace because we want an own instance on self.
         self._ReservedNames = self._ReservedNames | names
 
     def _assign_param_names(self, root_module: rf.Module):
         root = self.root
         for name, param in root_module.named_parameters(recurse=True):
+            param = _resolve_param_tensor(param)
             param_layer = param.raw_tensor
             assert isinstance(param_layer, Layer), f"param {param} has no layer"
             if not param_layer.parent and param_layer is not root:  # no parent yet?
                 param_layer.assign_parent(root, name)
 
     def _remove_unused_and_handle_subnets(self):
         # Collect all used tensor names.
@@ -412,15 +417,21 @@
                     sub_out.tensor = sub_real_out
                     root_mod_call.tensor = sub_real_out
 
                 # Do not use self.move_tensor_here(root_mod_call.tensor) because we don't want the extra logic.
                 for name, child in list(root_mod_call.children.items()):
                     child.assign_parent(parent=self, suggested_name=name)
 
-        # Check if we can rename some layers.
+        # Check if we can rename some layers
+        # based on the module hierarchy (parameters and module outputs).
+        # The layer names are not really relevant though,
+        # so this is just to make the config nicer.
+        # Only for parameters, we must make sure that the name is correct.
+        # However, this can always be done via the `name_scope` option,
+        # if the name would not match otherwise.
         queue = [self.root]  # type: List[Layer]
         mod_in_layer = {}  # type: Dict[Tuple[Layer, RefIdEq[rf.Module]], Layer]
         while queue:
             ctx = queue.pop(0)
 
             assert not ctx.parent or ctx.parent.children[ctx.name] is ctx
             for child in ctx.children.values():
@@ -636,14 +647,19 @@
         from returnn.util.better_exchook import get_current_frame
 
         frame = get_current_frame()
         self._enter_stack_frames = set()
         while frame:
             self._enter_stack_frames.add(frame)
             frame = frame.f_back
+        # make_layer() uses current_ctx() to get the parent scope.
+        # current_ctx() uses _auto_setup_parent_name_ctx() and this checks the recent layer.
+        # So, to make sure that we get the right parent scope in make_layer(),
+        # we need to set this.
+        self.__class__._recent = self
         return self
 
     def __exit__(self, exc_type, exc_val, exc_tb):
         assert self._stack[-1] is self, f"{self}.__exit__: stack {self._stack} top is not self"
         self._enter_stack_frames = None
         self._stack.pop(-1)
 
@@ -670,15 +686,15 @@
             if path is not None:
                 return ".".join(path)
         # Fallback to the canonical name.
         return self.module.get_default_name()
 
     def _get_unique_name(self, suggested_name: Optional[str] = None) -> str:
         name = suggested_name or self._get_suggested_name()
-        reserved_names = set(self.parent.children.keys()) | self._ReservedNames
+        reserved_names = set(self.parent.children.keys()) | self.parent._ReservedNames
         if self.parent.module:
             # Also reserve all attrib names of the parent module.
             # However, we allow to use the name if it is the attrib itself.
             if self.module and name not in reserved_names and getattr(self.parent.module, name, None) is self.module:
                 return name
             if self.tensor and name not in reserved_names and getattr(self.parent.module, name, None) is self.tensor:
                 return name
@@ -1066,15 +1082,16 @@
                     dim.dyn_size_ext
                 ), f"{sub_name_ctx}: need {dim} to be defined to be able to know about implicit dims"
             dim_tags.extend(data_template.dim_tags_set_implicit_only_wrapped)
             assert len(dim_tags) == len(
                 set((d, d.match_priority if isinstance(d, Dim) else 0) for d in dim_tags)
             ), f"duplicate dims in {sub_name_ctx} {sub_name_ctx.tensor}"
             if len(dim_tags) == len(set(dim_tags)):  # might not be unique without match_priority
-                if layer_dict["class"] not in {"constant", "variable", "random", "subnetwork"}:  # redundant
+                # For some layer classes, the out_shape would be redundant.
+                if layer_dict["class"] not in {"constant", "variable", "random", "subnetwork", "transpose"}:
                     layer_dict["out_shape"] = set(dim_tags)
 
             assert "name_scope" not in layer_dict  # we explicitly want to assign it now (if needed)
             if sub_name_ctx.custom_layer_name_scope is not None:
                 sub_name_scope = sub_name_ctx.custom_layer_name_scope
                 layer_dict["name_scope"] = sub_name_scope
                 assert sub_name_scope == ""  # anything else unexpected currently
@@ -1087,18 +1104,18 @@
                 # Note that parameters could be assigned lazily at some later point.
                 layer_abs_name_scope_parent = _stack.layer_abs_name_scope_effective
                 if layer_abs_name_scope_parent:
                     layer_abs_name_scope_parent += "/"
                 layer_abs_name_scope_default = layer_abs_name_scope_parent + sub_name_ctx.name
 
                 sub_layer_abs_name_scope = self._expected_layer_abs_name_scope(sub_name_ctx)
-                if isinstance(sub_name_ctx.tensor, rf.Parameter):
+                if sub_name_ctx.layer_dict["class"] == "variable":
                     assert (
                         sub_layer_abs_name_scope
-                    ), f"parameter {sub_name_ctx} must have a unique name in {self.root_module}"
+                    ), f"VariableLayer {sub_name_ctx} must have a unique name in {self.root_module}"
                 if sub_layer_abs_name_scope is not None:
                     if (
                         layer_abs_name_scope_default != sub_layer_abs_name_scope
                     ):  # default does not match what we require
                         if sub_layer_abs_name_scope == _stack.layer_abs_name_scope_effective:
                             layer_dict["name_scope"] = ""
                         elif sub_layer_abs_name_scope.startswith(layer_abs_name_scope_parent):  # can use relative
@@ -1485,14 +1502,15 @@
             for name, child in parent.named_children():
                 if RefIdEq(child) not in self.module_to_name_path:
                     self.module_to_name_path[RefIdEq(child)] = self.module_to_name_path[RefIdEq(parent)] + (name,)
                     self.name_path_to_module[self.module_to_name_path[RefIdEq(child)]] = child
                     queue.append(child)
             for name, param in parent.named_parameters(recurse=False):
                 assert isinstance(param.raw_tensor, rfl.Layer)
+                param = _resolve_param_tensor(param)
                 if param.raw_tensor not in self.tensor_to_name_path:
                     self.tensor_to_name_path[param.raw_tensor] = self.module_to_name_path[RefIdEq(parent)] + (name,)
 
     def get_name_path(
         self: _NamePathCache,
         child: Union[rf.Module, Tensor],
         *,
@@ -1514,14 +1532,33 @@
                 return self.module_to_name_path[RefIdEq(child)]
             else:
                 return self.module_to_name_path.get(RefIdEq(child))
         else:
             raise TypeError(f"invalid type {type(child)}")
 
 
+def _resolve_param_tensor(param: rf.Parameter[rfl.Layer]) -> rf.Tensor[rfl.Layer]:
+    """
+    Get the original tensor from a parameter, pointing to the VariableLayer.
+    Via parameter_assign, the current param tensor might be some variable read,
+    not the original VariableLayer.
+
+    :param param:
+    :return: tensor pointing to the VariableLayr
+    """
+    while True:
+        if param.raw_tensor.layer_dict["class"] == "variable":
+            return param
+        if param.raw_tensor.layer_dict["class"] == "variable_read":
+            param = param.raw_tensor.layer_dict["var"]
+            assert isinstance(param, rf.Tensor)
+            continue
+        raise Exception(f"unexpected param tensor {param} {param.raw_tensor} with opts {param.raw_tensor.layer_dict}")
+
+
 _AutoSetupNameCtxPrevTopFrame = None  # type: Optional[types.FrameType]
 _AutoSetupNameCtxCodeBlacklist = set()  # type: Set[types.CodeType]
 
 
 def _auto_setup_parent_name_ctx(*, ignore_top_stack_frames: int = 1) -> Layer:
     """
     Sets up a NameCtx corresponding to the Python call stack trace.
```

### Comparing `returnn-1.20230503.142906/returnn/tf/frontend_layers/make_layer.py` & `returnn-1.20230504.150134/returnn/tf/frontend_layers/make_layer.py`

 * *Files 2% similar despite different names*

```diff
@@ -73,14 +73,15 @@
             out = predefined_out_data.copy_template()
         else:
             out = _tensor_from_layer_dict(layer_dict, layer=layer)
 
         # Do not assign name_ctx.tensor yet because we potentially could raise exceptions later.
         assert layer.tensor is None
         assert layer.layer_dict is None
+        assert not layer.usages
 
         assert layer_dict is not None
 
         out.control_flow_ctx = rfl.Layer.inner_control_flow()
         if out.have_batch_axis() and not out.batch:
             # You could say this is a bug of RETURNN. Or at least RETURNN is just incomplete here.
             # RETURNN usually would fix that later when the layer is actually created,
@@ -91,14 +92,20 @@
                 if dep.tensor is not None and dep.tensor.batch and dep.tensor.batch not in batches:
                     batches.append(dep.tensor.batch)
             if batches:
                 out.batch = BatchInfo.get_common_batch_info(batches)
             elif layer.root.global_batch:
                 out.batch = layer.root.global_batch
 
+        for value in nest.flatten(layer_dict):
+            if isinstance(value, Tensor) and value.raw_tensor is not None:
+                value: Tensor[rfl.Layer]
+                assert isinstance(value.raw_tensor, rfl.Layer)
+                value.raw_tensor.usages.append(layer)
+
         layer.layer_dict = layer_dict
         layer.tensor = out
         out.raw_tensor = layer
 
     except Exception:
         # Just forward the exception.
         # However, if we already created a new name_ctx for it, we can clean this up now.
```

### Comparing `returnn-1.20230503.142906/returnn/tf/frontend_low_level/_backend.py` & `returnn-1.20230504.150134/returnn/tf/frontend_low_level/_backend.py`

 * *Files 1% similar despite different names*

```diff
@@ -191,14 +191,21 @@
         :return: shape[axis] expands to dim
         """
         assert raw_tensor.shape.as_list()[axis] == 1
         with tf_util.same_control_flow_ctx(raw_tensor):
             return tf.tile(raw_tensor, [1] * axis + [dim] + [1] * (raw_tensor.shape.ndims - axis - 1))
 
     @staticmethod
+    def copy(tensor: Tensor) -> Tensor:
+        """copy"""
+        out = tensor.copy_template()
+        out.raw_tensor = tf.identity(tensor.raw_tensor)
+        return out
+
+    @staticmethod
     def cast_raw(raw_tensor: tf.Tensor, dtype: str) -> tf.Tensor:
         """cast"""
         return tf.cast(raw_tensor, dtype)
 
     @staticmethod
     def activation_raw(raw_tensor: tf.Tensor, func: str) -> tf.Tensor:
         """
```

### Comparing `returnn-1.20230503.142906/returnn/tf/horovod.py` & `returnn-1.20230504.150134/returnn/tf/horovod.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230503.142906/returnn/tf/hyper_param_tuning.py` & `returnn-1.20230504.150134/returnn/tf/hyper_param_tuning.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230503.142906/returnn/tf/layers/base.py` & `returnn-1.20230504.150134/returnn/tf/layers/base.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230503.142906/returnn/tf/layers/basic.py` & `returnn-1.20230504.150134/returnn/tf/layers/basic.py`

 * *Files 0% similar despite different names*

```diff
@@ -426,37 +426,39 @@
     The difference to :class:`CopyLayer` is that this creates a new TF op (``tf.identity``),
     which allows for potential control dependencies.
     This is the whole purpose of this layer.
     """
 
     layer_class = "identity"
 
-    def __init__(self, sources: List[LayerBase], control_dependencies: Sequence[LayerBase], **kwargs):
+    def __init__(self, sources: List[LayerBase], control_dependencies: Optional[Sequence[LayerBase]] = None, **kwargs):
         super().__init__(sources=sources, **kwargs)
         assert len(sources) == 1
-        self.control_dependencies = control_dependencies
-        with tf.control_dependencies([src.output.placeholder.op for src in self.control_dependencies]):
+        self.control_dependencies = list(control_dependencies) if control_dependencies else []
+        deps = [src.output.placeholder.op for src in self.control_dependencies]
+        with tf.control_dependencies(deps) if deps else contextlib.nullcontext():
             self.output.placeholder = tf.identity(self.sources[0].output.placeholder)
 
     def get_dep_layers(self) -> List[LayerBase]:
         """deps"""
-        return super().get_dep_layers() + list(self.control_dependencies)
+        return super().get_dep_layers() + self.control_dependencies
 
     @classmethod
     def get_out_data_from_opts(cls, name: str, sources: List[LayerBase], **kwargs):
         """out"""
         assert sources
         return sources[0].output.copy(name="%s_output" % name)
 
     @classmethod
     def transform_config_dict(cls, d, network, get_layer):
         """transform"""
         super().transform_config_dict(d, network=network, get_layer=get_layer)
-        assert isinstance(d.get("control_dependencies"), (list, tuple))
-        d["control_dependencies"] = [get_layer(src_name) for src_name in d["control_dependencies"]]
+        if d.get("control_dependencies") is not None:
+            assert isinstance(d["control_dependencies"], (list, tuple))
+            d["control_dependencies"] = [get_layer(src_name) for src_name in d["control_dependencies"]]
 
 
 class ConcatLayer(LayerBase):
     """
     Concatenates the inputs in specified axes.
     This generalizes :class:`CopyLayer` which concatenates in the feature dim.
     """
@@ -10448,160 +10450,14 @@
             with cl.cls_setup_scope(**layer_desc):
                 d = cl.get_rec_initial_extra_outputs_shape_invariants(rec_layer=rec_layer, **layer_desc)
                 for key, value in d.items():
                     shape_invariants["%s/%s" % (layer_name, key)] = value
         return shape_invariants
 
 
-class VariableLayer(LayerBase):
-    """
-    Represents a variable. Can add batch/time dimension if wanted. Can be trainable.
-    See defaults.
-    """
-
-    layer_class = "variable"
-
-    def __init__(
-        self,
-        shape,
-        dtype="float32",
-        add_batch_axis=False,
-        add_time_axis=False,
-        trainable=True,
-        non_critical_for_restore=False,
-        init=None,
-        init_by_layer=None,
-        param_name=None,
-        **kwargs,
-    ):
-        """
-        :param tuple[int|Dim]|list[int|Dim] shape:
-        :param str dtype:
-        :param bool add_batch_axis:
-        :param bool add_time_axis:
-        :param bool trainable:
-        :param bool non_critical_for_restore:
-        :param str|float|int|None init: see :func:`returnn.tf.util.basic.get_initializer`. 0 by default.
-          Alternatively, you can also use option `init_by_layer`.
-        :param LayerBase|None init_by_layer:
-        :param str|None param_name: self.name (layer name) by default
-        """
-        shape  # noqa  # used in get_out_data_from_opts
-        super(VariableLayer, self).__init__(trainable=trainable, **kwargs)
-        assert not self.sources, "%s: does not expect any sources" % self
-        self.init_by_layer = init_by_layer
-        dim_tags = list(self.output.dim_tags)
-        if add_batch_axis:
-            assert dim_tags[0].is_batch_dim()
-            dim_tags = dim_tags[1:]
-        if add_time_axis:
-            assert dim_tags[0].dimension == 1
-            dim_tags = dim_tags[1:]
-        shape_ = [d.dimension for d in dim_tags]
-        assert all(shape_), self.output  # all static
-        with self.var_creation_scope():
-            if init_by_layer is None:
-                if init is None:
-                    init = 0
-                initializer = tf_util.get_initializer(
-                    init, dtype=dtype, seed=self.network.random.randint(2**31), eval_local_ns={"layer": self}
-                )
-            else:
-                assert init_by_layer is not None
-                out_data_base = Data(name=self.output.name, dim_tags=dim_tags, dtype=dtype)
-                initializer = init_by_layer.output.copy_compatible_to(out_data_base).placeholder
-                shape_ = None  # get_variable requires shape to be not defined when the initializer is another tensor
-            var = self.add_param(
-                tf_compat.v1.get_variable(
-                    name=param_name or self.name,
-                    shape=shape_,
-                    dtype=dtype,
-                    initializer=initializer,
-                    trainable=trainable,
-                ),
-                axes_split_info=[d.axis_split_info() for d in dim_tags],
-                non_critical_for_restore=non_critical_for_restore,
-            )
-            out = var
-            if add_time_axis:
-                out = tf.expand_dims(out, axis=0)
-            if add_batch_axis:
-                # Unbroadcast to not confuse some other layers
-                batch_dim = self.output.get_batch_dim()
-                out = tf_util.expand_dims_unbroadcast(out, axis=0, dim=batch_dim)
-        self.output.placeholder = out
-
-    def get_dep_layers(self):
-        """
-        :rtype: list[LayerBase]
-        """
-        deps = super(VariableLayer, self).get_dep_layers()
-        if self.init_by_layer:
-            deps.append(self.init_by_layer)
-        return deps
-
-    @classmethod
-    def transform_config_dict(cls, d, network, get_layer):
-        """
-        :param dict[str] d: will modify inplace
-        :param returnn.tf.network.TFNetwork network:
-        :param ((str) -> LayerBase) get_layer: function to get or construct another layer
-        """
-        # Overwrite default behavior for default sources.
-        # Here: none by default.
-        d.setdefault("from", [])
-        super(VariableLayer, cls).transform_config_dict(d, network=network, get_layer=get_layer)
-        if d.get("init_by_layer", None):
-            d["init_by_layer"] = get_layer(d["init_by_layer"])
-
-    @classmethod
-    def get_out_data_from_opts(
-        cls, name, network, shape, dtype="float32", add_batch_axis=False, add_time_axis=False, **kwargs
-    ):
-        """
-        :param str name:
-        :param returnn.tf.network.TFNetwork network:
-        :param tuple[int|Dim]|list[int|Dim] shape:
-        :param str dtype:
-        :param bool add_batch_axis:
-        :param bool add_time_axis:
-        :rtype: Data
-        """
-        assert isinstance(shape, (list, tuple))
-        assert len(shape) == 0 or all(shape)
-        dim_tags = []
-        for i, d in enumerate(shape):
-            if isinstance(d, Dim):
-                assert d.dimension is not None, "%r: need static dims but got %r" % (name, d)
-            elif isinstance(d, int):
-                d = Dim(
-                    kind=Dim.Types.Spatial if i < len(shape) - 1 else Dim.Types.Feature,
-                    description="%s:static:%i" % (name, i),
-                    auto_generated=True,
-                    dimension=d,
-                )
-            else:
-                raise TypeError("Layer %r: invalid type %s in shape %r" % (name, type(d), shape))
-            dim_tags.append(d)
-        if add_time_axis:
-            dim_tags.insert(
-                0, Dim(kind=Dim.Types.Time, description="%s:dummy-time" % name, dimension=1, auto_generated=True)
-            )
-        if add_batch_axis:
-            dim_tags.insert(
-                0, Dim(kind=Dim.Types.Batch, description="batch", batch=network.get_global_batch_info(), dimension=None)
-            )
-        return Data(
-            name="%s_output" % name,
-            dim_tags=dim_tags,
-            dtype=dtype,
-            batch=network.get_global_batch_info() if add_batch_axis else None,
-        )
-
-
 class TrainFlagLayer(LayerBase):
     """
     Returns the train flag (bool scalar) of the current network.
     """
 
     layer_class = "train_flag"
 
@@ -13504,27 +13360,29 @@
 
 _LayerClassDictInitialized = False
 _LayerClassDict = {}  # type: typing.Dict[str,typing.Type[LayerBase]]
 
 
 def _init_layer_class_dict():
     global _LayerClassDictInitialized
-    _LayerClassDictInitialized = True
     from . import rec
+    from . import variable
     from . import signal_processing
     from . import segmental_model
 
     auto_register_layer_classes(list(globals().values()))
-    for mod in [rec, signal_processing, segmental_model]:
+    for mod in [rec, variable, signal_processing, segmental_model]:
         auto_register_layer_classes(list(vars(mod).values()))
 
     for alias, v in {"forward": LinearLayer, "hidden": LinearLayer}.items():
         assert alias not in _LayerClassDict
         _LayerClassDict[alias] = v
 
+    _LayerClassDictInitialized = True
+
 
 def auto_register_layer_classes(vars_values):
     """
     Example usage::
 
         from returnn.tf.layers.basic import auto_register_layer_classes
         auto_register_layer_classes('extern_private/your_stuff/CoolThingy.py')
```

### Comparing `returnn-1.20230503.142906/returnn/tf/layers/rec.py` & `returnn-1.20230504.150134/returnn/tf/layers/rec.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230503.142906/returnn/tf/layers/segmental_model.py` & `returnn-1.20230504.150134/returnn/tf/layers/segmental_model.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230503.142906/returnn/tf/layers/signal_processing.py` & `returnn-1.20230504.150134/returnn/tf/layers/signal_processing.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230503.142906/returnn/tf/native_op.py` & `returnn-1.20230504.150134/returnn/tf/native_op.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230503.142906/returnn/tf/network.py` & `returnn-1.20230504.150134/returnn/tf/network.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230503.142906/returnn/tf/sprint.py` & `returnn-1.20230504.150134/returnn/tf/sprint.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230503.142906/returnn/tf/updater.py` & `returnn-1.20230504.150134/returnn/tf/updater.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230503.142906/returnn/tf/util/basic.py` & `returnn-1.20230504.150134/returnn/tf/util/basic.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """
 Lots of random utility functions for TensorFlow.
 """
 
 from __future__ import annotations
 
-from typing import Optional
+from typing import Optional, List
 import typing
 import contextlib
 import os
 import sys
 import threading
 import numpy
 import tensorflow as tf
@@ -22,14 +22,15 @@
 # noinspection PyUnresolvedReferences
 from .data import Data, SearchBeam, Dim, DimensionTag
 
 try:
     from tensorflow.python.ops.control_flow_v2_func_graphs import ControlFlowFuncGraph
 except ImportError:
     ControlFlowFuncGraph = None
+from tensorflow.python.ops.control_flow_ops import ControlFlowContext
 
 
 class CollectionKeys:
     """
     Extension of :class:`tf.compat.v1.GraphKeys`
     """
 
@@ -5855,14 +5856,92 @@
         graph._set_control_flow_context(ctx)
         yield ctx
     finally:
         # noinspection PyProtectedMember
         graph._set_control_flow_context(cur_ctx)
 
 
+def op_in_right_control_flow_context(op: tf.Operation) -> Optional[tf.Operation]:
+    """
+    :param op: op with some control flow.
+    :return: some op in a control flow context which can be accessed from the current control flow context,
+        or None if there is no such op.
+    """
+    import tensorflow.python.ops.control_flow_ops as tf_control_flow_ops
+    import tensorflow.python.ops.control_flow_util as tf_control_flow_util
+
+    # Check that we get the right control flow context.
+    # noinspection PyProtectedMember
+    control_flow_ctx: Optional[tf_control_flow_ops.ControlFlowContext] = op._get_control_flow_context()
+    graph = tf_compat.v1.get_default_graph()
+    if not control_flow_ctx and graph is op.graph:  # Simple case, early exit.
+        return op
+
+    if ControlFlowFuncGraph:
+        if isinstance(op.graph, ControlFlowFuncGraph):
+            raise NotImplementedError(f"not implemented yet for control flow v2, op {op}, graph {op.graph}")
+    assert graph is op.graph  # if this is not the case, maybe control flow V2, or eager. not implemented yet...
+    # noinspection PyProtectedMember
+    cur_control_flow_ctx: Optional[tf_control_flow_ops.ControlFlowContext] = graph._get_control_flow_context()
+    while not tf_control_flow_util.IsContainingContext(cur_control_flow_ctx, control_flow_ctx):
+        assert control_flow_ctx
+        # Get op from outer control flow context.
+        assert isinstance(control_flow_ctx, tf_control_flow_ops.CondContext)  # not implemented otherwise yet...
+        # If the current control flow context is the False branch,
+        # and the op control flow context is from the corresponding True branch,
+        # then we cannot access it.
+        # Also, there would not be any Merge ops, as the cond is not finished yet.
+        if (
+            isinstance(cur_control_flow_ctx, tf_control_flow_ops.CondContext)
+            and cur_control_flow_ctx.pred is control_flow_ctx.pred
+            and control_flow_ctx.branch == 1
+            and cur_control_flow_ctx.branch == 0
+        ):
+            return None
+        merge_ops = _merge_ops_for_control_flow_ctx(control_flow_ctx)
+        assert merge_ops, f"no merge op found for control flow context {control_flow_ctx}, cur {cur_control_flow_ctx}"
+        merge_ops = [op_ for op_ in merge_ops if _output_op_has_path_to_input_op(op_, op)]
+        assert merge_ops, f"no merge op found which has path to op {op}"
+        # Just take the first.
+        op = merge_ops[0]
+        # noinspection PyProtectedMember
+        control_flow_ctx = op._get_control_flow_context()
+    return op
+
+
+def _merge_ops_for_control_flow_ctx(control_flow_ctx: ControlFlowContext) -> List[tf.Operation]:
+    graph = tf_compat.v1.get_default_graph()
+    ops = []
+    for op in graph.get_operations():
+        op: tf.Operation
+        if op.type == "Merge":
+            for in_ in op.inputs:
+                in_: tf.Tensor
+                # noinspection PyProtectedMember
+                in_control_flow_ctx = in_.op._get_control_flow_context()
+                if in_control_flow_ctx is control_flow_ctx:
+                    ops.append(op)
+    return ops
+
+
+def _output_op_has_path_to_input_op(output_op: tf.Operation, input_op: tf.Operation) -> bool:
+    queue = [output_op]
+    visited = set()
+    while queue:
+        op = queue.pop(0)
+        if op in visited:
+            continue
+        visited.add(op)
+        if op is input_op:
+            return True
+        queue.extend([t.op for t in op.inputs])
+        queue.extend(op.control_inputs)
+    return False
+
+
 def get_protobuf_fields(obj):
     """
     :param obj: protobuf object
     :rtype: dict[str]
     """
     return {k.name: v for (k, v) in obj.ListFields()}
```

### Comparing `returnn-1.20230503.142906/returnn/tf/util/data.py` & `returnn-1.20230504.150134/returnn/tf/util/data.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230503.142906/returnn/tf/util/ken_lm.py` & `returnn-1.20230504.150134/returnn/tf/util/ken_lm.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230503.142906/returnn/tf/util/open_fst.py` & `returnn-1.20230504.150134/returnn/tf/util/open_fst.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230503.142906/returnn/torch/data/pipeline.py` & `returnn-1.20230504.150134/returnn/torch/data/pipeline.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230503.142906/returnn/torch/data/returnn_dataset_wrapper.py` & `returnn-1.20230504.150134/returnn/torch/data/returnn_dataset_wrapper.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230503.142906/returnn/torch/data/tensor_utils.py` & `returnn-1.20230504.150134/returnn/torch/data/tensor_utils.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230503.142906/returnn/torch/engine.py` & `returnn-1.20230504.150134/returnn/torch/engine.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230503.142906/returnn/torch/frontend/_backend.py` & `returnn-1.20230504.150134/returnn/torch/frontend/_backend.py`

 * *Files 2% similar despite different names*

```diff
@@ -142,14 +142,21 @@
         :param raw_tensor:
         :param axis: e.g. 1
         :return: raw tensor with new axis
         """
         return raw_tensor.unsqueeze(axis)
 
     @staticmethod
+    def copy(tensor: Tensor[torch.Tensor]) -> Tensor[torch.Tensor]:
+        """copy"""
+        out = tensor.copy_template()
+        out.raw_tensor = tensor.raw_tensor.clone()
+        return out
+
+    @staticmethod
     def cast_raw(raw_tensor: torch.Tensor, dtype: str) -> torch.Tensor:
         """cast"""
         return raw_tensor.to(dtype=TorchBackend.as_dtype_raw(dtype))
 
     @staticmethod
     def stop_gradient(tensor: Tensor) -> Tensor:
         """stop grad"""
@@ -513,14 +520,28 @@
     def set_parameter_trainable(param: rf.Parameter, trainable: bool) -> None:
         """set trainable"""
         raw_param = param.raw_tensor
         assert isinstance(raw_param, torch.nn.Parameter)
         raw_param.requires_grad = trainable
 
     @staticmethod
+    def parameter_assign(param: rf.Parameter, value: Tensor, op: str = "assign") -> None:
+        """param assign"""
+        value_ = value.copy_compatible_to(param)
+        raw_param = param.raw_tensor
+        assert isinstance(raw_param, torch.nn.Parameter)
+        with torch.no_grad():
+            if op == "assign":
+                raw_param.copy_(value_.raw_tensor)
+            elif op == "add":
+                raw_param.add_(value_.raw_tensor)
+            else:
+                raise ValueError(f"Parameter {param} assign: Unsupported op: {op}")
+
+    @staticmethod
     def compare_raw(a: torch.Tensor, kind: str, b: torch.Tensor) -> torch.Tensor:
         """
         :param a:
         :param kind: "equal", "less", "less_equal", "greater", "greater_equal", "not_equal"
         :param b:
         :return: a `kind` b
         """
```

### Comparing `returnn-1.20230503.142906/returnn/torch/frontend/_rand.py` & `returnn-1.20230504.150134/returnn/torch/frontend/_rand.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230503.142906/returnn/torch/frontend/bridge.py` & `returnn-1.20230504.150134/returnn/torch/frontend/bridge.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230503.142906/returnn/torch/updater.py` & `returnn-1.20230504.150134/returnn/torch/updater.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,16 +3,18 @@
 and model param update logic in general.
 """
 
 from __future__ import annotations
 
 import torch
 import typing
+from typing import Set
 
 from returnn.log import log
+from returnn.util.basic import RefIdEq
 
 _OptimizerClassesDictInitialized = False
 _OptimizerClassesDict = {}
 
 
 def _init_optimizer_classes_dict():
     """
@@ -237,16 +239,22 @@
             return [{"params": network_params}]
 
         # Distinguish between parameters with and without weight_decay/L2 regularization.
         # Parameters without weight decay: biases + LayerNorm/Embedding layers.
         wd_params = set()
         no_wd_params = set()
         blacklist_wd_modules = (torch.nn.LayerNorm, torch.nn.Embedding)
+        # Tracker of visited parameters to only add each parameter once, in case two modules share common parameters.
+        # We need the wrapper class RefIdEq because Parameters are compared by value and not by reference.
+        visited_params: Set[RefIdEq[torch.nn.Parameter]] = set()
         for mn, m in self.network.named_modules():
             for pn, p in m.named_parameters():
+                if RefIdEq(p) in visited_params:
+                    continue
+                visited_params.add(RefIdEq(p))
                 fpn = "%s.%s" % (mn, pn) if mn else pn  # Full param name
                 if pn.endswith("bias"):
                     no_wd_params.add(fpn)
                 elif pn.endswith("weight") and isinstance(m, blacklist_wd_modules):
                     no_wd_params.add(fpn)
                 else:
                     wd_params.add(fpn)
```

### Comparing `returnn-1.20230503.142906/returnn/util/basic.py` & `returnn-1.20230504.150134/returnn/util/basic.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230503.142906/returnn/util/better_exchook.py` & `returnn-1.20230504.150134/returnn/util/better_exchook.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230503.142906/returnn/util/bpe.py` & `returnn-1.20230504.150134/returnn/util/bpe.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230503.142906/returnn/util/debug.py` & `returnn-1.20230504.150134/returnn/util/debug.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230503.142906/returnn/util/debug_helpers.py` & `returnn-1.20230504.150134/returnn/util/debug_helpers.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230503.142906/returnn/util/fsa.py` & `returnn-1.20230504.150134/returnn/util/fsa.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230503.142906/returnn/util/literal_py_to_pickle.py` & `returnn-1.20230504.150134/returnn/util/literal_py_to_pickle.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230503.142906/returnn/util/pprint.py` & `returnn-1.20230504.150134/returnn/util/pprint.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230503.142906/returnn/util/py-to-pickle.cpp` & `returnn-1.20230504.150134/returnn/util/py-to-pickle.cpp`

 * *Files identical despite different names*

### Comparing `returnn-1.20230503.142906/returnn/util/sig_proc.py` & `returnn-1.20230504.150134/returnn/util/sig_proc.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230503.142906/returnn/util/task_system.py` & `returnn-1.20230504.150134/returnn/util/task_system.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230503.142906/returnn.egg-info/PKG-INFO` & `returnn-1.20230504.150134/returnn.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: returnn
-Version: 1.20230503.142906
+Version: 1.20230504.150134
 Summary: The RWTH extensible training framework for universal recurrent neural networks
 Home-page: https://github.com/rwth-i6/returnn/
 Author: Albert Zeyer
 Author-email: albzey@gmail.com
 License: RETURNN license
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
```

### Comparing `returnn-1.20230503.142906/returnn.egg-info/SOURCES.txt` & `returnn-1.20230504.150134/returnn.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -222,23 +222,25 @@
 returnn/tf/frontend_layers/_utils.py
 returnn/tf/frontend_layers/cond.py
 returnn/tf/frontend_layers/config_entry_points.py
 returnn/tf/frontend_layers/debug_eager_mode.py
 returnn/tf/frontend_layers/dims.py
 returnn/tf/frontend_layers/layer.py
 returnn/tf/frontend_layers/make_layer.py
+returnn/tf/frontend_layers/parameter_assign.py
 returnn/tf/frontend_layers/prev_tensor_ref.py
 returnn/tf/frontend_low_level/__init__.py
 returnn/tf/frontend_low_level/_backend.py
 returnn/tf/layers/__init__.py
 returnn/tf/layers/base.py
 returnn/tf/layers/basic.py
 returnn/tf/layers/rec.py
 returnn/tf/layers/segmental_model.py
 returnn/tf/layers/signal_processing.py
+returnn/tf/layers/variable.py
 returnn/tf/util/__init__.py
 returnn/tf/util/basic.py
 returnn/tf/util/data.py
 returnn/tf/util/ken_lm.py
 returnn/tf/util/open_fst.py
 returnn/torch/README.md
 returnn/torch/__init__.py
```

### Comparing `returnn-1.20230503.142906/setup.py` & `returnn-1.20230504.150134/setup.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230503.142906/tests/DummySprintExec.py` & `returnn-1.20230504.150134/tests/DummySprintExec.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230503.142906/tests/PyCharm-inspection-profile.xml` & `returnn-1.20230504.150134/tests/PyCharm-inspection-profile.xml`

 * *Files identical despite different names*

### Comparing `returnn-1.20230503.142906/tests/PyCharm.idea/codeStyleSettings.xml` & `returnn-1.20230504.150134/tests/PyCharm.idea/codeStyleSettings.xml`

 * *Files identical despite different names*

### Comparing `returnn-1.20230503.142906/tests/PyCharm.idea/inspectionProfiles/Project_Default.xml` & `returnn-1.20230504.150134/tests/PyCharm.idea/inspectionProfiles/Project_Default.xml`

 * *Files identical despite different names*

### Comparing `returnn-1.20230503.142906/tests/_set_num_threads1.py` & `returnn-1.20230504.150134/tests/_set_num_threads1.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230503.142906/tests/_setup_test_env.py` & `returnn-1.20230504.150134/tests/_setup_test_env.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230503.142906/tests/bpe-unicode-demo.codes` & `returnn-1.20230504.150134/tests/bpe-unicode-demo.codes`

 * *Files identical despite different names*

### Comparing `returnn-1.20230503.142906/tests/bpe-unicode-demo.vocab` & `returnn-1.20230504.150134/tests/bpe-unicode-demo.vocab`

 * *Files identical despite different names*

### Comparing `returnn-1.20230503.142906/tests/lexicon_opt.isyms` & `returnn-1.20230504.150134/tests/lexicon_opt.isyms`

 * *Files identical despite different names*

### Comparing `returnn-1.20230503.142906/tests/lexicon_opt.jpg` & `returnn-1.20230504.150134/tests/lexicon_opt.jpg`

 * *Files identical despite different names*

### Comparing `returnn-1.20230503.142906/tests/lint_common.py` & `returnn-1.20230504.150134/tests/lint_common.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230503.142906/tests/pycharm-inspect.py` & `returnn-1.20230504.150134/tests/pycharm-inspect.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230503.142906/tests/pylint.py` & `returnn-1.20230504.150134/tests/pylint.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230503.142906/tests/returnn-as-framework.py` & `returnn-1.20230504.150134/tests/returnn-as-framework.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230503.142906/tests/rf_utils.py` & `returnn-1.20230504.150134/tests/rf_utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """
 RETURNN frontend (returnn.frontend) utils
 """
 
 from __future__ import annotations
 from typing import Optional, Union, Dict
 import contextlib
+import re
 import numpy
 import numpy.testing
 from tensorflow.python.util import nest
 
 from returnn.config import Config, global_config_ctx
 from returnn.util.pprint import pprint
 import returnn.frontend as rf
@@ -126,22 +127,34 @@
             "get_model": get_model,
             "task": "forward",
             "forward_step": forward_step,
         }
     )
 
     with tf_scope() as session, global_config_ctx(config):
-        net_dict = get_net_dict(epoch=1, step=0)
+        net_dict, model = get_net_dict(epoch=1, step=0)
         print("*** TF net dict:")
         pprint(net_dict)
         outputs_layers = rf.get_run_ctx().outputs
         print("*** outputs:", outputs_layers)
 
         net = TFNetwork(config=config, train_flag=False)
         net.construct_from_dict(net_dict)
+
+        rf_params = {name.replace(".", "/"): p for name, p in model.named_parameters()}
+        tf_params = {re.sub("/param:0$", "", p.name): p for p in net.get_params_list()}
+        rf_params_not_in_tf = set(rf_params.keys()) - set(tf_params.keys())
+        tf_params_not_in_rf = set(tf_params.keys()) - set(rf_params.keys())
+        if rf_params_not_in_tf or tf_params_not_in_rf:
+            raise Exception(
+                "params not equal:\n"
+                f"RF params not in TF: {rf_params_not_in_tf}\n"
+                f"TF params not in RF: {tf_params_not_in_rf}"
+            )
+
         session.run(tf_compat.v1.global_variables_initializer())
 
         outputs_tf = TensorDict()
         for k, v in outputs_layers.data.items():
             v: Tensor[rfl.Layer]
             assert isinstance(v.raw_tensor, rfl.Layer)
             layer_name = v.raw_tensor.get_abs_name()
```

### Comparing `returnn-1.20230503.142906/tests/spelling.dic` & `returnn-1.20230504.150134/tests/spelling.dic`

 * *Files identical despite different names*

### Comparing `returnn-1.20230503.142906/tests/test_Config.py` & `returnn-1.20230504.150134/tests/test_Config.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230503.142906/tests/test_Dataset.py` & `returnn-1.20230504.150134/tests/test_Dataset.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230503.142906/tests/test_Fsa.py` & `returnn-1.20230504.150134/tests/test_Fsa.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230503.142906/tests/test_GeneratingDataset.py` & `returnn-1.20230504.150134/tests/test_GeneratingDataset.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230503.142906/tests/test_HDFDataset.py` & `returnn-1.20230504.150134/tests/test_HDFDataset.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230503.142906/tests/test_LearningRateControl.py` & `returnn-1.20230504.150134/tests/test_LearningRateControl.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230503.142906/tests/test_Log.py` & `returnn-1.20230504.150134/tests/test_Log.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230503.142906/tests/test_MultiProcDataset.py` & `returnn-1.20230504.150134/tests/test_MultiProcDataset.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230503.142906/tests/test_PTDataset.py` & `returnn-1.20230504.150134/tests/test_PTDataset.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230503.142906/tests/test_Pretrain.py` & `returnn-1.20230504.150134/tests/test_Pretrain.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230503.142906/tests/test_ResNet.py` & `returnn-1.20230504.150134/tests/test_ResNet.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230503.142906/tests/test_SprintDataset.py` & `returnn-1.20230504.150134/tests/test_SprintDataset.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230503.142906/tests/test_SprintInterface.py` & `returnn-1.20230504.150134/tests/test_SprintInterface.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230503.142906/tests/test_TFEngine.py` & `returnn-1.20230504.150134/tests/test_TFEngine.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230503.142906/tests/test_TFNativeOp.py` & `returnn-1.20230504.150134/tests/test_TFNativeOp.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230503.142906/tests/test_TFNetworkLayer.py` & `returnn-1.20230504.150134/tests/test_TFNetworkLayer.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 import unittest
 import numpy.testing
 from pprint import pprint
 from returnn.util import better_exchook
 from returnn.config import Config
 from returnn.tf.network import *
 from returnn.tf.layers.basic import *
+from returnn.tf.layers.variable import *
 import returnn.tf.compat as tf_compat
 import returnn.tf.util.basic as tf_util
 from returnn.tf.util.data import Dim, SpatialDim, FeatureDim, BatchInfo
 
 print("TF version:", tf.__version__)
 print("Numpy version:", numpy.__version__)
 
@@ -10933,15 +10934,16 @@
         out_weights = network.get_default_output_layer().params["W"]
         print("out_weights:", out_weights)
         assert isinstance(out_weights, tf.Variable)
         assert out_weights.get_shape().as_list() == [11 + 13, 17]
         # TODO: multiple checks:
         # the split info itself
         # the param init handling...
-        # actually, for param init handling, input dim splits do not matter. they matter just for copying/growing-pretrain.
+        # actually, for param init handling, input dim splits do not matter.
+        # they matter just for copying/growing-pretrain.
         # for param init handling, output dim split do matter.
 
 
 def test_VariableLayer_split_info():
     feat1 = FeatureDim("feature1", 3)
     feat2 = FeatureDim("feature2", 5)
     net_dict = {"output": {"class": "variable", "shape": [2 * feat1 + feat2, 3 * feat1]}}
```

### Comparing `returnn-1.20230503.142906/tests/test_TFNetworkRecLayer.py` & `returnn-1.20230504.150134/tests/test_TFNetworkRecLayer.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230503.142906/tests/test_TFNetworkSigProcLayer.py` & `returnn-1.20230504.150134/tests/test_TFNetworkSigProcLayer.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230503.142906/tests/test_TFUpdater.py` & `returnn-1.20230504.150134/tests/test_TFUpdater.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230503.142906/tests/test_TFUtil.py` & `returnn-1.20230504.150134/tests/test_TFUtil.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230503.142906/tests/test_TF_determinism.py` & `returnn-1.20230504.150134/tests/test_TF_determinism.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230503.142906/tests/test_TaskSystem.py` & `returnn-1.20230504.150134/tests/test_TaskSystem.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230503.142906/tests/test_TaskSystem_SharedMem.py` & `returnn-1.20230504.150134/tests/test_TaskSystem_SharedMem.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230503.142906/tests/test_TranslationDataset.py` & `returnn-1.20230504.150134/tests/test_TranslationDataset.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230503.142906/tests/test_Util.py` & `returnn-1.20230504.150134/tests/test_Util.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230503.142906/tests/test_demos.py` & `returnn-1.20230504.150134/tests/test_demos.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230503.142906/tests/test_fork_exec.py` & `returnn-1.20230504.150134/tests/test_fork_exec.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230503.142906/tests/test_hdf_dump.py` & `returnn-1.20230504.150134/tests/test_hdf_dump.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230503.142906/tests/test_rf_array.py` & `returnn-1.20230504.150134/tests/test_rf_array.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230503.142906/tests/test_rf_attention.py` & `returnn-1.20230504.150134/tests/test_rf_attention.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230503.142906/tests/test_rf_base.py` & `returnn-1.20230504.150134/tests/test_rf_base.py`

 * *Files 15% similar despite different names*

```diff
@@ -182,7 +182,41 @@
 
     # noinspection PyShadowingNames
     def _forward_step(*, model: _Net, extern_data: TensorDict):
         out = model(extern_data["data"])
         out.mark_as_default_output(shape=())
 
     run_model(extern_data, lambda *, epoch, step: _Net(), _forward_step)
+
+
+def test_param_assign():
+    time_dim = Dim(Tensor("time", [batch_dim], dtype="int32"))
+    in_dim = Dim(7, name="in")
+    extern_data = TensorDict(
+        {
+            "data": Tensor("data", [batch_dim, time_dim, in_dim], dtype="float32"),
+        }
+    )
+
+    class _Net(rf.Module):
+        def __init__(self):
+            super().__init__()
+            self.param = rf.Parameter(dims=(), dtype="int32")
+            self.param.initial = 2
+
+        def __call__(self, x: Tensor) -> Tuple[Tensor, Tensor, Tensor]:
+            # No extra care should be needed for graph-based backends.
+            a = rf.copy(self.param)
+            self.param.assign(5)
+            b = rf.copy(self.param)
+            self.param.assign(7)
+            return a, b, self.param
+
+    # noinspection PyShadowingNames
+    def _forward_step(*, model: _Net, extern_data: TensorDict):
+        a, b, c = model(extern_data["data"])
+        a.mark_as_output("a", shape=())
+        b.mark_as_output("b", shape=())
+        c.mark_as_output("c", shape=())
+
+    out = run_model(extern_data, lambda *, epoch, step: _Net(), _forward_step)
+    assert out["a"].raw_tensor == 2 and out["b"].raw_tensor == 5 and out["c"].raw_tensor == 7
```

### Comparing `returnn-1.20230503.142906/tests/test_rf_cond.py` & `returnn-1.20230504.150134/tests/test_rf_cond.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """
 RETURNN frontend (returnn.frontend) tests
 """
 
 from __future__ import annotations
+from typing import Tuple
 import _setup_test_env  # noqa
 import returnn.frontend as rf
 from returnn.tensor import Tensor, Dim, TensorDict, batch_dim
 from rf_utils import run_model
 
 
 def test_cond():
@@ -139,12 +140,120 @@
         out = model(extern_data["data"])
         out.mark_as_default_output(shape=(batch_dim, time_dim, out_dim))
 
     run_model(extern_data, lambda *, epoch, step: _Net(), _forward_step, dyn_dim_max_sizes={time_dim: 5})
     run_model(extern_data, lambda *, epoch, step: _Net(), _forward_step, dyn_dim_max_sizes={time_dim: 6})
 
 
+def test_cond_param_assign():
+    time_dim = Dim(Tensor("time", [batch_dim], dtype="int32"))
+    in_dim = Dim(7, name="in")
+    extern_data = TensorDict(
+        {
+            "data": Tensor("data", [batch_dim, time_dim, in_dim], dtype="float32"),
+        }
+    )
+
+    class _Net(rf.Module):
+        def __init__(self):
+            super().__init__()
+            self.param = rf.Parameter(dims=(), dtype="int32")
+            self.param.initial = 2
+
+        def __call__(self, x: Tensor) -> Tensor:
+            # No extra care should be needed for graph-based backends.
+            rf.cond(
+                pred=time_dim.get_dim_value_tensor() % 2 == 0,
+                true_fn=lambda: self.param.assign_add(3),
+                false_fn=lambda: None,
+            )
+            return self.param
+
+    # noinspection PyShadowingNames
+    def _forward_step(*, model: _Net, extern_data: TensorDict):
+        out = model(extern_data["data"])
+        out.mark_as_default_output(shape=())
+
+    out1 = run_model(extern_data, lambda *, epoch, step: _Net(), _forward_step, dyn_dim_max_sizes={time_dim: 5})
+    out2 = run_model(extern_data, lambda *, epoch, step: _Net(), _forward_step, dyn_dim_max_sizes={time_dim: 6})
+    assert out1["output"].raw_tensor == 2
+    assert out2["output"].raw_tensor == 5
+
+
+def test_cond_param_assign2():
+    time_dim = Dim(Tensor("time", [batch_dim], dtype="int32"))
+    in_dim = Dim(7, name="in")
+    extern_data = TensorDict(
+        {
+            "data": Tensor("data", [batch_dim, time_dim, in_dim], dtype="float32"),
+        }
+    )
+
+    class _Net(rf.Module):
+        def __init__(self):
+            super().__init__()
+            self.param = rf.Parameter(dims=(), dtype="int32")
+            self.param.initial = 2
+
+        def __call__(self, x: Tensor) -> Tensor:
+            # No extra care should be needed for graph-based backends.
+            rf.cond(
+                pred=time_dim.get_dim_value_tensor() % 2 == 0,
+                true_fn=lambda: self.param.assign_add(3),
+                false_fn=lambda: self.param.assign_add(7),
+            )
+            return self.param
+
+    # noinspection PyShadowingNames
+    def _forward_step(*, model: _Net, extern_data: TensorDict):
+        out = model(extern_data["data"])
+        out.mark_as_default_output(shape=())
+
+    out1 = run_model(extern_data, lambda *, epoch, step: _Net(), _forward_step, dyn_dim_max_sizes={time_dim: 5})
+    out2 = run_model(extern_data, lambda *, epoch, step: _Net(), _forward_step, dyn_dim_max_sizes={time_dim: 6})
+    assert out1["output"].raw_tensor == 9
+    assert out2["output"].raw_tensor == 5
+
+
+def test_cond_param_assign3():
+    time_dim = Dim(Tensor("time", [batch_dim], dtype="int32"))
+    in_dim = Dim(7, name="in")
+    extern_data = TensorDict(
+        {
+            "data": Tensor("data", [batch_dim, time_dim, in_dim], dtype="float32"),
+        }
+    )
+
+    class _Net(rf.Module):
+        def __init__(self):
+            super().__init__()
+            self.param = rf.Parameter(dims=(), dtype="int32")
+            self.param.initial = 2
+
+        def __call__(self, x: Tensor) -> Tuple[Tensor, Tensor]:
+            # No extra care should be needed for graph-based backends.
+            return (
+                rf.cond(
+                    pred=time_dim.get_dim_value_tensor() % 2 == 0,
+                    true_fn=lambda: (self.param.assign_add(3), rf.convert_to_tensor(42))[-1],
+                    false_fn=lambda: self.param * 3,
+                ),
+                self.param,
+            )
+
+    # noinspection PyShadowingNames
+    def _forward_step(*, model: _Net, extern_data: TensorDict):
+        out, param = model(extern_data["data"])
+        out.mark_as_default_output(shape=())
+        param.mark_as_output(shape=(), name="param")
+
+    out1 = run_model(extern_data, lambda *, epoch, step: _Net(), _forward_step, dyn_dim_max_sizes={time_dim: 5})
+    out2 = run_model(extern_data, lambda *, epoch, step: _Net(), _forward_step, dyn_dim_max_sizes={time_dim: 6})
+    assert out1["output"].raw_tensor == 6 and out1["param"].raw_tensor == 2
+    assert out2["output"].raw_tensor == 42 and out2["param"].raw_tensor == 5
+
+
 # TODO some more from RETURNN-common, like:
 #  - test_cond_random
 #  - test_cond_new_axis
 #  - test_cond_dim (https://github.com/rwth-i6/returnn/pull/1262)
 #  - test_cond_multiple_outputs
```

### Comparing `returnn-1.20230503.142906/tests/test_rf_container.py` & `returnn-1.20230504.150134/tests/test_rf_container.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230503.142906/tests/test_rf_conv.py` & `returnn-1.20230504.150134/tests/test_rf_conv.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230503.142906/tests/test_rf_encoder_conformer.py` & `returnn-1.20230504.150134/tests/test_rf_encoder_conformer.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230503.142906/tests/test_rf_math.py` & `returnn-1.20230504.150134/tests/test_rf_math.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230503.142906/tests/test_rf_normalization.py` & `returnn-1.20230504.150134/tests/test_rf_normalization.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230503.142906/tests/test_rf_rec.py` & `returnn-1.20230504.150134/tests/test_rf_rec.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230503.142906/tests/test_rf_signal.py` & `returnn-1.20230504.150134/tests/test_rf_signal.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230503.142906/tests/test_tensor.py` & `returnn-1.20230504.150134/tests/test_tensor.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230503.142906/tests/test_tools.py` & `returnn-1.20230504.150134/tests/test_tools.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230503.142906/tests/test_torch_frontend.py` & `returnn-1.20230504.150134/tests/test_torch_frontend.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230503.142906/tests/test_torch_internal_frontend.py` & `returnn-1.20230504.150134/tests/test_torch_internal_frontend.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230503.142906/tools/analyze-dataset-batches.py` & `returnn-1.20230504.150134/tools/analyze-dataset-batches.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230503.142906/tools/bliss-collect-seq-lens.py` & `returnn-1.20230504.150134/tools/bliss-collect-seq-lens.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230503.142906/tools/bliss-dump-text.py` & `returnn-1.20230504.150134/tools/bliss-dump-text.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230503.142906/tools/bliss-get-segment-names.py` & `returnn-1.20230504.150134/tools/bliss-get-segment-names.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230503.142906/tools/bliss-to-ogg-zip.py` & `returnn-1.20230504.150134/tools/bliss-to-ogg-zip.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230503.142906/tools/bpe-create-lexicon.py` & `returnn-1.20230504.150134/tools/bpe-create-lexicon.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230503.142906/tools/calculate-word-error-rate.py` & `returnn-1.20230504.150134/tools/calculate-word-error-rate.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230503.142906/tools/cleanup-old-models.py` & `returnn-1.20230504.150134/tools/cleanup-old-models.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230503.142906/tools/collect-orth-symbols.py` & `returnn-1.20230504.150134/tools/collect-orth-symbols.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230503.142906/tools/collect-words.py` & `returnn-1.20230504.150134/tools/collect-words.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230503.142906/tools/compile_native_op.py` & `returnn-1.20230504.150134/tools/compile_native_op.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230503.142906/tools/compile_tf_graph.py` & `returnn-1.20230504.150134/tools/compile_tf_graph.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230503.142906/tools/debug-dump-search-scores.py` & `returnn-1.20230504.150134/tools/debug-dump-search-scores.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230503.142906/tools/debug-plot-search-scores.py` & `returnn-1.20230504.150134/tools/debug-plot-search-scores.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230503.142906/tools/dump-dataset-raw-strings.py` & `returnn-1.20230504.150134/tools/dump-dataset-raw-strings.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230503.142906/tools/dump-dataset.py` & `returnn-1.20230504.150134/tools/dump-dataset.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230503.142906/tools/dump-forward-stats.py` & `returnn-1.20230504.150134/tools/dump-forward-stats.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230503.142906/tools/dump-forward.py` & `returnn-1.20230504.150134/tools/dump-forward.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230503.142906/tools/dump-network-json.py` & `returnn-1.20230504.150134/tools/dump-network-json.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230503.142906/tools/dump-pickle.py` & `returnn-1.20230504.150134/tools/dump-pickle.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230503.142906/tools/extract_state_tying_from_dataset.py` & `returnn-1.20230504.150134/tools/extract_state_tying_from_dataset.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230503.142906/tools/get-attention-weights.py` & `returnn-1.20230504.150134/tools/get-attention-weights.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230503.142906/tools/get-best-model-epoch.py` & `returnn-1.20230504.150134/tools/get-best-model-epoch.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230503.142906/tools/hdf_dump.py` & `returnn-1.20230504.150134/tools/hdf_dump.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230503.142906/tools/hdf_dump_translation_dataset.py` & `returnn-1.20230504.150134/tools/hdf_dump_translation_dataset.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230503.142906/tools/import-blocks-mt-model.py` & `returnn-1.20230504.150134/tools/import-blocks-mt-model.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230503.142906/tools/import-t2t-mt-model.py` & `returnn-1.20230504.150134/tools/import-t2t-mt-model.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230503.142906/tools/lattice_rescorer/Makefile` & `returnn-1.20230504.150134/tools/lattice_rescorer/Makefile`

 * *Files identical despite different names*

### Comparing `returnn-1.20230503.142906/tools/lattice_rescorer/README.md` & `returnn-1.20230504.150134/tools/lattice_rescorer/README.md`

 * *Files identical despite different names*

### Comparing `returnn-1.20230503.142906/tools/lattice_rescorer/example/README.md` & `returnn-1.20230504.150134/tools/lattice_rescorer/example/README.md`

 * *Files identical despite different names*

### Comparing `returnn-1.20230503.142906/tools/lattice_rescorer/example/network.040/i600_m600_m600.sgd_b16_lr0_cl2.newbobabs.config` & `returnn-1.20230504.150134/tools/lattice_rescorer/example/network.040/i600_m600_m600.sgd_b16_lr0_cl2.newbobabs.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230503.142906/tools/lattice_rescorer/example/network.040/i600_m600_m600.sgd_b16_lr0_cl2.newbobabs.keep_over_epoch.lstm2.config` & `returnn-1.20230504.150134/tools/lattice_rescorer/example/network.040/i600_m600_m600.sgd_b16_lr0_cl2.newbobabs.keep_over_epoch.lstm2.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230503.142906/tools/lattice_rescorer/example/rescore_lattice.sh` & `returnn-1.20230504.150134/tools/lattice_rescorer/example/rescore_lattice.sh`

 * *Files identical despite different names*

### Comparing `returnn-1.20230503.142906/tools/lattice_rescorer/file.h` & `returnn-1.20230504.150134/tools/lattice_rescorer/file.h`

 * *Files identical despite different names*

### Comparing `returnn-1.20230503.142906/tools/lattice_rescorer/htklatticerescorer.cc` & `returnn-1.20230504.150134/tools/lattice_rescorer/htklatticerescorer.cc`

 * *Files identical despite different names*

### Comparing `returnn-1.20230503.142906/tools/lattice_rescorer/htklatticerescorer.h` & `returnn-1.20230504.150134/tools/lattice_rescorer/htklatticerescorer.h`

 * *Files identical despite different names*

### Comparing `returnn-1.20230503.142906/tools/lattice_rescorer/main.cc` & `returnn-1.20230504.150134/tools/lattice_rescorer/main.cc`

 * *Files identical despite different names*

### Comparing `returnn-1.20230503.142906/tools/lattice_rescorer/rescorer.h` & `returnn-1.20230504.150134/tools/lattice_rescorer/rescorer.h`

 * *Files identical despite different names*

### Comparing `returnn-1.20230503.142906/tools/lattice_rescorer/vocabulary.cc` & `returnn-1.20230504.150134/tools/lattice_rescorer/vocabulary.cc`

 * *Files identical despite different names*

### Comparing `returnn-1.20230503.142906/tools/lattice_rescorer/vocabulary.h` & `returnn-1.20230504.150134/tools/lattice_rescorer/vocabulary.h`

 * *Files identical despite different names*

### Comparing `returnn-1.20230503.142906/tools/tf_avg_checkpoints.py` & `returnn-1.20230504.150134/tools/tf_avg_checkpoints.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230503.142906/tools/tf_inspect_checkpoint.py` & `returnn-1.20230504.150134/tools/tf_inspect_checkpoint.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230503.142906/tools/tf_inspect_summary_log.py` & `returnn-1.20230504.150134/tools/tf_inspect_summary_log.py`

 * *Files identical despite different names*

