# Comparing `tmp/nkululeko-0.44.1.tar.gz` & `tmp/nkululeko-0.45.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nkululeko-0.44.1.tar", last modified: Thu Apr 27 09:30:21 2023, max compression
+gzip compressed data, was "nkululeko-0.45.0.tar", last modified: Thu May  4 14:48:25 2023, max compression
```

## Comparing `nkululeko-0.44.1.tar` & `nkululeko-0.45.0.tar`

### file list

```diff
@@ -1,69 +1,70 @@
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2023-04-27 09:30:21.173899 nkululeko-0.44.1/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     5501 2023-04-27 09:02:47.000000 nkululeko-0.44.1/CHANGELOG.md
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1076 2021-10-28 13:49:53.000000 nkululeko-0.44.1/LICENSE
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    16530 2023-04-27 09:30:21.173899 nkululeko-0.44.1/PKG-INFO
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    10476 2023-04-21 08:51:24.000000 nkululeko-0.44.1/README.md
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2023-04-27 09:30:21.173899 nkululeko-0.44.1/nkululeko/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)        0 2023-01-20 08:45:34.000000 nkululeko-0.44.1/nkululeko/__init__.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1385 2023-03-07 15:26:22.000000 nkululeko-0.44.1/nkululeko/augment.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2399 2023-03-23 15:05:56.000000 nkululeko-0.44.1/nkululeko/augmenter.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)       12 2023-01-14 20:36:15.000000 nkululeko-0.44.1/nkululeko/balancer.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      955 2023-01-16 11:55:06.000000 nkululeko-0.44.1/nkululeko/cacheddataset.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)       19 2023-04-27 08:44:51.000000 nkululeko-0.44.1/nkululeko/constants.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    21627 2023-03-23 14:59:33.000000 nkululeko-0.44.1/nkululeko/dataset.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1908 2023-04-27 08:57:05.000000 nkululeko-0.44.1/nkululeko/dataset_csv.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      537 2023-01-16 11:56:12.000000 nkululeko-0.44.1/nkululeko/dataset_ravdess.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1789 2023-02-15 16:47:19.000000 nkululeko-0.44.1/nkululeko/demo.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2286 2023-02-15 16:29:45.000000 nkululeko-0.44.1/nkululeko/demo_predictor.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    20413 2023-04-20 16:45:58.000000 nkululeko-0.44.1/nkululeko/experiment.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1873 2023-04-27 09:18:23.000000 nkululeko-0.44.1/nkululeko/explore.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3726 2023-04-18 13:35:09.000000 nkululeko-0.44.1/nkululeko/feats_analyser.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2536 2023-02-20 12:40:05.000000 nkululeko-0.44.1/nkululeko/feats_audmodel.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3117 2023-04-19 15:46:17.000000 nkululeko-0.44.1/nkululeko/feats_clap.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2045 2023-02-09 11:59:30.000000 nkululeko-0.44.1/nkululeko/feats_import.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1949 2023-02-09 11:57:32.000000 nkululeko-0.44.1/nkululeko/feats_mld.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2772 2023-02-09 11:59:54.000000 nkululeko-0.44.1/nkululeko/feats_opensmile.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     4425 2023-02-09 12:00:41.000000 nkululeko-0.44.1/nkululeko/feats_oxbow.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1699 2023-02-15 16:11:36.000000 nkululeko-0.44.1/nkululeko/feats_praat.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2975 2023-04-19 20:26:13.000000 nkululeko-0.44.1/nkululeko/feats_trill.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     4005 2023-02-09 12:01:59.000000 nkululeko-0.44.1/nkululeko/feats_wav2vec2.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3174 2023-04-19 15:22:07.000000 nkululeko-0.44.1/nkululeko/feature_extractor.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1319 2023-02-28 14:54:13.000000 nkululeko-0.44.1/nkululeko/featureset.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    13546 2023-01-16 10:52:58.000000 nkululeko-0.44.1/nkululeko/feinberg_praat.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1821 2023-01-16 12:04:04.000000 nkululeko-0.44.1/nkululeko/filter_data.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      237 2023-01-16 11:49:55.000000 nkululeko-0.44.1/nkululeko/glob_conf.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      939 2023-01-14 20:36:15.000000 nkululeko-0.44.1/nkululeko/loss_ccc.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1329 2023-01-14 20:36:15.000000 nkululeko-0.44.1/nkululeko/loss_softf1loss.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    12074 2023-02-20 12:50:06.000000 nkululeko-0.44.1/nkululeko/model.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      432 2023-03-24 08:08:57.000000 nkululeko-0.44.1/nkululeko/model_bayes.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     5029 2023-03-24 08:09:03.000000 nkululeko-0.44.1/nkululeko/model_cnn.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      603 2023-03-24 08:09:21.000000 nkululeko-0.44.1/nkululeko/model_gmm.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      544 2023-03-24 08:10:02.000000 nkululeko-0.44.1/nkululeko/model_knn.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      551 2023-03-24 08:09:46.000000 nkululeko-0.44.1/nkululeko/model_knn_reg.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     8007 2023-03-24 08:10:19.000000 nkululeko-0.44.1/nkululeko/model_mlp.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     8781 2023-03-24 08:10:12.000000 nkululeko-0.44.1/nkululeko/model_mlp_regression.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      522 2023-03-24 08:10:26.000000 nkululeko-0.44.1/nkululeko/model_svm.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      505 2023-03-24 08:10:49.000000 nkululeko-0.44.1/nkululeko/model_svr.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      382 2023-03-24 08:11:15.000000 nkululeko-0.44.1/nkululeko/model_tree.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      389 2023-03-24 08:10:58.000000 nkululeko-0.44.1/nkululeko/model_tree_reg.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      236 2023-03-24 08:11:22.000000 nkululeko-0.44.1/nkululeko/model_xgb.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      242 2023-03-24 08:11:33.000000 nkululeko-0.44.1/nkululeko/model_xgr.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     5367 2023-03-24 08:13:41.000000 nkululeko-0.44.1/nkululeko/modelrunner.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1514 2023-01-16 11:50:04.000000 nkululeko-0.44.1/nkululeko/nkululeko.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     6450 2023-04-20 15:44:41.000000 nkululeko-0.44.1/nkululeko/plots.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    10170 2023-03-23 13:43:00.000000 nkululeko-0.44.1/nkululeko/reporter.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      406 2023-01-16 11:15:47.000000 nkululeko-0.44.1/nkululeko/result.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     6753 2023-02-20 11:58:56.000000 nkululeko-0.44.1/nkululeko/runmanager.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3013 2023-01-16 11:17:07.000000 nkululeko-0.44.1/nkululeko/scaler.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1340 2023-02-20 12:57:51.000000 nkululeko-0.44.1/nkululeko/test.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2315 2023-01-16 12:10:32.000000 nkululeko-0.44.1/nkululeko/test_predictor.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     7661 2023-02-20 11:54:33.000000 nkululeko-0.44.1/nkululeko/util.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2023-04-27 09:30:21.173899 nkululeko-0.44.1/nkululeko.egg-info/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    16530 2023-04-27 09:30:21.000000 nkululeko-0.44.1/nkululeko.egg-info/PKG-INFO
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1533 2023-04-27 09:30:21.000000 nkululeko-0.44.1/nkululeko.egg-info/SOURCES.txt
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)        1 2023-04-27 09:30:21.000000 nkululeko-0.44.1/nkululeko.egg-info/dependency_links.txt
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      259 2023-04-27 09:30:21.000000 nkululeko-0.44.1/nkululeko.egg-info/requires.txt
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)       10 2023-04-27 09:30:21.000000 nkululeko-0.44.1/nkululeko.egg-info/top_level.txt
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      100 2023-01-16 10:13:10.000000 nkululeko-0.44.1/pyproject.toml
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      938 2023-04-27 09:30:21.173899 nkululeko-0.44.1/setup.cfg
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)       59 2023-01-20 08:48:57.000000 nkululeko-0.44.1/setup.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2023-05-04 14:48:25.434569 nkululeko-0.45.0/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     5665 2023-05-04 14:43:10.000000 nkululeko-0.45.0/CHANGELOG.md
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1076 2021-10-28 13:49:53.000000 nkululeko-0.45.0/LICENSE
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    16694 2023-05-04 14:48:25.438570 nkululeko-0.45.0/PKG-INFO
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    10476 2023-04-21 08:51:24.000000 nkululeko-0.45.0/README.md
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2023-05-04 14:48:25.434569 nkululeko-0.45.0/nkululeko/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)        0 2023-01-20 08:45:34.000000 nkululeko-0.45.0/nkululeko/__init__.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1385 2023-03-07 15:26:22.000000 nkululeko-0.45.0/nkululeko/augment.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2399 2023-03-23 15:05:56.000000 nkululeko-0.45.0/nkululeko/augmenter.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)       12 2023-01-14 20:36:15.000000 nkululeko-0.45.0/nkululeko/balancer.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      955 2023-01-16 11:55:06.000000 nkululeko-0.45.0/nkululeko/cacheddataset.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)       19 2023-05-04 13:46:28.000000 nkululeko-0.45.0/nkululeko/constants.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    21627 2023-03-23 14:59:33.000000 nkululeko-0.45.0/nkululeko/dataset.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1908 2023-04-27 08:57:05.000000 nkululeko-0.45.0/nkululeko/dataset_csv.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      537 2023-01-16 11:56:12.000000 nkululeko-0.45.0/nkululeko/dataset_ravdess.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1789 2023-02-15 16:47:19.000000 nkululeko-0.45.0/nkululeko/demo.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2286 2023-02-15 16:29:45.000000 nkululeko-0.45.0/nkululeko/demo_predictor.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    20413 2023-04-20 16:45:58.000000 nkululeko-0.45.0/nkululeko/experiment.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1873 2023-04-27 09:18:23.000000 nkululeko-0.45.0/nkululeko/explore.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3726 2023-04-18 13:35:09.000000 nkululeko-0.45.0/nkululeko/feats_analyser.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2748 2023-05-04 14:30:28.000000 nkululeko-0.45.0/nkululeko/feats_audmodel.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2739 2023-05-04 14:30:21.000000 nkululeko-0.45.0/nkululeko/feats_audmodel_dim.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3250 2023-05-04 14:30:36.000000 nkululeko-0.45.0/nkululeko/feats_clap.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2045 2023-05-04 14:08:00.000000 nkululeko-0.45.0/nkululeko/feats_import.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1949 2023-02-09 11:57:32.000000 nkululeko-0.45.0/nkululeko/feats_mld.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2772 2023-02-09 11:59:54.000000 nkululeko-0.45.0/nkululeko/feats_opensmile.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     4425 2023-02-09 12:00:41.000000 nkululeko-0.45.0/nkululeko/feats_oxbow.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1832 2023-05-04 14:30:50.000000 nkululeko-0.45.0/nkululeko/feats_praat.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2975 2023-04-19 20:26:13.000000 nkululeko-0.45.0/nkululeko/feats_trill.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     4005 2023-02-09 12:01:59.000000 nkululeko-0.45.0/nkululeko/feats_wav2vec2.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3456 2023-05-04 13:43:15.000000 nkululeko-0.45.0/nkululeko/feature_extractor.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1319 2023-02-28 14:54:13.000000 nkululeko-0.45.0/nkululeko/featureset.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    13546 2023-01-16 10:52:58.000000 nkululeko-0.45.0/nkululeko/feinberg_praat.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1821 2023-01-16 12:04:04.000000 nkululeko-0.45.0/nkululeko/filter_data.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      237 2023-01-16 11:49:55.000000 nkululeko-0.45.0/nkululeko/glob_conf.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      939 2023-01-14 20:36:15.000000 nkululeko-0.45.0/nkululeko/loss_ccc.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1329 2023-01-14 20:36:15.000000 nkululeko-0.45.0/nkululeko/loss_softf1loss.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    12074 2023-02-20 12:50:06.000000 nkululeko-0.45.0/nkululeko/model.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      432 2023-03-24 08:08:57.000000 nkululeko-0.45.0/nkululeko/model_bayes.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     5029 2023-03-24 08:09:03.000000 nkululeko-0.45.0/nkululeko/model_cnn.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      603 2023-03-24 08:09:21.000000 nkululeko-0.45.0/nkululeko/model_gmm.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      544 2023-03-24 08:10:02.000000 nkululeko-0.45.0/nkululeko/model_knn.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      551 2023-03-24 08:09:46.000000 nkululeko-0.45.0/nkululeko/model_knn_reg.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     8007 2023-03-24 08:10:19.000000 nkululeko-0.45.0/nkululeko/model_mlp.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     8781 2023-03-24 08:10:12.000000 nkululeko-0.45.0/nkululeko/model_mlp_regression.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      522 2023-03-24 08:10:26.000000 nkululeko-0.45.0/nkululeko/model_svm.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      505 2023-03-24 08:10:49.000000 nkululeko-0.45.0/nkululeko/model_svr.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      382 2023-03-24 08:11:15.000000 nkululeko-0.45.0/nkululeko/model_tree.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      389 2023-03-24 08:10:58.000000 nkululeko-0.45.0/nkululeko/model_tree_reg.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      236 2023-03-24 08:11:22.000000 nkululeko-0.45.0/nkululeko/model_xgb.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      242 2023-03-24 08:11:33.000000 nkululeko-0.45.0/nkululeko/model_xgr.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     5367 2023-03-24 08:13:41.000000 nkululeko-0.45.0/nkululeko/modelrunner.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1514 2023-01-16 11:50:04.000000 nkululeko-0.45.0/nkululeko/nkululeko.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     6450 2023-04-20 15:44:41.000000 nkululeko-0.45.0/nkululeko/plots.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    10170 2023-03-23 13:43:00.000000 nkululeko-0.45.0/nkululeko/reporter.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      406 2023-01-16 11:15:47.000000 nkululeko-0.45.0/nkululeko/result.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     6753 2023-02-20 11:58:56.000000 nkululeko-0.45.0/nkululeko/runmanager.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3013 2023-01-16 11:17:07.000000 nkululeko-0.45.0/nkululeko/scaler.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1340 2023-02-20 12:57:51.000000 nkululeko-0.45.0/nkululeko/test.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2315 2023-01-16 12:10:32.000000 nkululeko-0.45.0/nkululeko/test_predictor.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     8174 2023-05-04 14:07:02.000000 nkululeko-0.45.0/nkululeko/util.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2023-05-04 14:48:25.434569 nkululeko-0.45.0/nkululeko.egg-info/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    16694 2023-05-04 14:48:25.000000 nkululeko-0.45.0/nkululeko.egg-info/PKG-INFO
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1565 2023-05-04 14:48:25.000000 nkululeko-0.45.0/nkululeko.egg-info/SOURCES.txt
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)        1 2023-05-04 14:48:25.000000 nkululeko-0.45.0/nkululeko.egg-info/dependency_links.txt
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      259 2023-05-04 14:48:25.000000 nkululeko-0.45.0/nkululeko.egg-info/requires.txt
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)       10 2023-05-04 14:48:25.000000 nkululeko-0.45.0/nkululeko.egg-info/top_level.txt
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      100 2023-01-16 10:13:10.000000 nkululeko-0.45.0/pyproject.toml
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      938 2023-05-04 14:48:25.438570 nkululeko-0.45.0/setup.cfg
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)       59 2023-01-20 08:48:57.000000 nkululeko-0.45.0/setup.py
```

### Comparing `nkululeko-0.44.1/CHANGELOG.md` & `nkululeko-0.45.0/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -2,14 +2,25 @@
 =========
 
 Version 0.44.1
 --------------
 * bugfixing: feature importance: https://github.com/felixbur/nkululeko/issues/23
 * bugfixing: loading csv database with filewise index https://github.com/felixbur/nkululeko/issues/24 
 
+
+Version 0.45.0
+--------------
+* added auddim as features
+* added FEATS store_format
+* added device use to feat_audmodel
+
+Version 0.44.1
+--------------
+* bugfixes
+
 Version 0.44.0
 --------------
 * added scatter functions: tsne, pca, umap
 
 Version 0.43.7
 --------------
 * added clap features
```

### Comparing `nkululeko-0.44.1/LICENSE` & `nkululeko-0.45.0/LICENSE`

 * *Files identical despite different names*

### Comparing `nkululeko-0.44.1/PKG-INFO` & `nkululeko-0.45.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nkululeko
-Version: 0.44.1
+Version: 0.45.0
 Summary: Machine learning audio prediction experiments based on templates
 Home-page: https://github.com/felixbur/nkululeko
 Author: Felix Burkhardt
 Author-email: fxburk@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -213,14 +213,25 @@
 =========
 
 Version 0.44.1
 --------------
 * bugfixing: feature importance: https://github.com/felixbur/nkululeko/issues/23
 * bugfixing: loading csv database with filewise index https://github.com/felixbur/nkululeko/issues/24 
 
+
+Version 0.45.0
+--------------
+* added auddim as features
+* added FEATS store_format
+* added device use to feat_audmodel
+
+Version 0.44.1
+--------------
+* bugfixes
+
 Version 0.44.0
 --------------
 * added scatter functions: tsne, pca, umap
 
 Version 0.43.7
 --------------
 * added clap features
```

### Comparing `nkululeko-0.44.1/README.md` & `nkululeko-0.45.0/README.md`

 * *Files identical despite different names*

### Comparing `nkululeko-0.44.1/nkululeko/augment.py` & `nkululeko-0.45.0/nkululeko/augment.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.44.1/nkululeko/augmenter.py` & `nkululeko-0.45.0/nkululeko/augmenter.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.44.1/nkululeko/cacheddataset.py` & `nkululeko-0.45.0/nkululeko/cacheddataset.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.44.1/nkululeko/dataset.py` & `nkululeko-0.45.0/nkululeko/dataset.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.44.1/nkululeko/dataset_csv.py` & `nkululeko-0.45.0/nkululeko/dataset_csv.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.44.1/nkululeko/dataset_ravdess.py` & `nkululeko-0.45.0/nkululeko/dataset_ravdess.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.44.1/nkululeko/demo.py` & `nkululeko-0.45.0/nkululeko/demo.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.44.1/nkululeko/demo_predictor.py` & `nkululeko-0.45.0/nkululeko/demo_predictor.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.44.1/nkululeko/experiment.py` & `nkululeko-0.45.0/nkululeko/experiment.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.44.1/nkululeko/explore.py` & `nkululeko-0.45.0/nkululeko/explore.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.44.1/nkululeko/feats_analyser.py` & `nkululeko-0.45.0/nkululeko/feats_analyser.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.44.1/nkululeko/feats_audmodel.py` & `nkululeko-0.45.0/nkululeko/feats_audmodel_dim.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,61 +1,63 @@
-# feats_audmodel.py
+# feats_audmodel_dim.py
 from nkululeko.featureset import Featureset
 import os
 import pandas as pd
 import audeer
 import nkululeko.glob_conf as glob_conf
 import audonnx
 import numpy as np
 import audinterface
 
-class AudModelSet(Featureset):
+class AudModelDimSet(Featureset):
     """
-        Embeddings from the wav2vec2. based model finetuned on MSPPodcast emotions, described in the paper
+        Emotional dimensions from the wav2vec2. based model finetuned on MSPPodcast emotions, described in the paper
         "Dawn of the transformer era in speech emotion recognition: closing the valence gap"
         https://arxiv.org/abs/2203.07378
     """
     def __init__(self, name, data_df):
         super().__init__(name, data_df)
         model_url = 'https://zenodo.org/record/6221127/files/w2v2-L-robust-12.6bc4a7fd-1.1.0.zip'
         model_root = self.util.config_val('FEATS', 'aud.model', './audmodel/')
         if not os.path.isdir(model_root):
             cache_root = audeer.mkdir('cache')
             model_root = audeer.mkdir(model_root)
             archive_path = audeer.download_url(model_url, cache_root, verbose=True)
             audeer.extract_archive(archive_path, model_root)
-        self.model = audonnx.load(model_root)
+        device = self.util.config_val('MODEL', 'device', 'cpu')
+        self.model = audonnx.load(model_root, device=device)
 
 
     def extract(self):
         """Extract the features based on the initialized dataset or re-open them when found on disk."""
         store = self.util.get_path('store')
-        storage = f'{store}{self.name}.pkl'
+        store_format = self.util.config_val('FEATS', 'store_format', 'pkl')
+        storage = f'{store}{self.name}.{store_format}'
         extract = eval(self.util.config_val('FEATS', 'needs_feature_extraction', 'False'))
         no_reuse = eval(self.util.config_val('FEATS', 'no_reuse', 'False'))
         if no_reuse or extract or not os.path.isfile(storage):
-            self.util.debug('extracting audmodel features, this might take a while...')
-            hidden_states = audinterface.Feature(
-                self.model.labels('hidden_states'),
+            self.util.debug('extracting audmodel dimensions, this might take a while...')
+            logits = audinterface.Feature(
+                self.model.labels('logits'),
                 process_func=self.model,
                 process_func_args={
-                    'outputs': 'hidden_states',
+                    'outputs': 'logits',
                 },
                 sampling_rate=16000,    
                 resample=True,    
                 num_workers=5,
                 verbose=True,
             )
-            self.df = hidden_states.process_index(self.data_df.index)
-            self.df.to_pickle(storage)
+            self.df = logits.process_index(self.data_df.index)
+            self.util.write_store(self.df, storage, store_format)
             try:
                 glob_conf.config['DATA']['needs_feature_extraction'] = 'False'
             except KeyError:
                 pass
         else:
             self.util.debug('reusing extracted audmodel features.')
-            self.df = pd.read_pickle(storage)
+            self.df = self.util.get_store(storage, store_format)
 
 
     def extract_sample(self, signal, sr):
         result = self.model(signal, sr)
         return np.asarray(result['hidden_states'].flatten())
```

### Comparing `nkululeko-0.44.1/nkululeko/feats_clap.py` & `nkululeko-0.45.0/nkululeko/feats_clap.py`

 * *Files 11% similar despite different names*

```diff
@@ -27,15 +27,16 @@
         self.model.load_ckpt() # download the default pretrained checkpoint.
         print(f'loaded clap model')
 
 
     def extract(self):
         """Extract the features or load them from disk if present."""
         store = self.util.get_path('store')
-        storage = f'{store}{self.name}.pkl'
+        store_format = self.util.config_val('FEATS', 'store_format', 'pkl')
+        storage = f'{store}{self.name}.{store_format}'
         extract = self.util.config_val('FEATS', 'needs_feature_extraction', False)
         no_reuse = eval(self.util.config_val('FEATS', 'no_reuse', 'False'))
         if extract or no_reuse or not os.path.isfile(storage):
             if not self.model_initialized:
                 self.init_model()
             self.util.debug('extracting clap embeddings, this might take a while...')
             emb_series = pd.Series(index = self.data_df.index, dtype=object)
@@ -43,22 +44,22 @@
             for idx, (file, start, end) in enumerate(self.data_df.index.to_list()):
                 signal, sampling_rate = audiofile.read(file, offset=start.total_seconds(), duration=(end-start).total_seconds(), always_2d=True)
                 emb = self.get_embeddings(signal, sampling_rate)
                 emb_series[idx] = emb
                 if idx%10==0:
                     self.util.debug(f'Clap: {idx} of {length} done')
             self.df = pd.DataFrame(emb_series.values.tolist(), index=self.data_df.index) 
-            self.df.to_pickle(storage)
+            self.util.write_store(self.df, storage, store_format)
             try:
                 glob_conf.config['DATA']['needs_feature_extraction'] = 'false'
             except KeyError:
                 pass
         else:
             self.util.debug('reusing extracted wav2vec2 embeddings')
-            self.df = pd.read_pickle(storage)
+            self.df = self.util.get_store(storage, store_format)
             if self.df.isnull().values.any():
                 nanrows = self.df.columns[self.df.isna().any()].tolist()
                 print(nanrows)
                 self.util.error(f'got nan: {self.df.shape} {self.df.isnull().sum().sum()}')
 
 
     def get_embeddings(self, signal, sampling_rate):
```

### Comparing `nkululeko-0.44.1/nkululeko/feats_import.py` & `nkululeko-0.45.0/nkululeko/feats_import.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.44.1/nkululeko/feats_mld.py` & `nkululeko-0.45.0/nkululeko/feats_mld.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.44.1/nkululeko/feats_opensmile.py` & `nkululeko-0.45.0/nkululeko/feats_opensmile.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.44.1/nkululeko/feats_oxbow.py` & `nkululeko-0.45.0/nkululeko/feats_oxbow.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.44.1/nkululeko/feats_praat.py` & `nkululeko-0.45.0/nkululeko/feats_praat.py`

 * *Files 12% similar despite different names*

```diff
@@ -14,29 +14,30 @@
     """
     def __init__(self, name, data_df):
         super().__init__(name, data_df)
 
     def extract(self):
         """Extract the features based on the initialized dataset or re-open them when found on disk."""
         store = self.util.get_path('store')
-        storage = f'{store}{self.name}.pkl'
+        store_format = self.util.config_val('FEATS', 'store_format', 'pkl')
+        storage = f'{store}{self.name}.{store_format}'
         extract = self.util.config_val('FEATS', 'needs_feature_extraction', False)
         no_reuse = eval(self.util.config_val('FEATS', 'no_reuse', 'False'))
         if extract or no_reuse or not os.path.isfile(storage):
             self.util.debug('extracting Praat features, this might take a while...')
             self.df = feinberg_praat.compute_features(self.data_df.index)
             self.df = self.df.set_index(self.data_df.index)
-            self.df.to_pickle(storage)
+            self.util.write_store(self.df, storage, store_format)
             try:
                 glob_conf.config['DATA']['needs_feature_extraction'] = 'false'
             except KeyError:
                 pass
         else:
             self.util.debug('reusing extracted Praat features.')
-            self.df = pd.read_pickle(storage)
+            self.df = self.util.get_store(storage, store_format)
         self.util.debug(f'praat feature names: {self.df.columns}')
         self.df = self.df.astype(float)
 
 
 
     def extract_sample(self, signal, sr):
         self.util.error('feats_praat: extracting single samples not implemented yet')
```

### Comparing `nkululeko-0.44.1/nkululeko/feats_trill.py` & `nkululeko-0.45.0/nkululeko/feats_trill.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.44.1/nkululeko/feats_wav2vec2.py` & `nkululeko-0.45.0/nkululeko/feats_wav2vec2.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.44.1/nkululeko/feature_extractor.py` & `nkululeko-0.45.0/nkululeko/feature_extractor.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,13 @@
-# feature_extractor.py
+"""
+feature_extractor.py
+
+Helper class to encapsulate feature extraction methods
+
+"""
 import pandas as pd
 from nkululeko.util import Util 
 from nkululeko.feats_opensmile import Opensmileset
 
 
 class FeatureExtractor:
     df = None # pandas dataframe to store the features (and indexed with the data from the sets)
@@ -30,14 +35,17 @@
                 self.featExtractor = TRILLset(f'{store_name}_{self.feats_designation}', self.data_df)
             elif feats_type=='wav2vec':
                 from nkululeko.feats_wav2vec2 import Wav2vec2
                 self.featExtractor = Wav2vec2(f'{store_name}_{self.feats_designation}', self.data_df)
             elif feats_type=='audmodel':
                 from nkululeko.feats_audmodel import AudModelSet
                 self.featExtractor = AudModelSet(f'{store_name}_{self.feats_designation}', self.data_df)
+            elif feats_type=='auddim':
+                from nkululeko.feats_audmodel_dim import AudModelDimSet
+                self.featExtractor = AudModelDimSet(f'{store_name}_{self.feats_designation}', self.data_df)
             elif feats_type=='clap':
                 from nkululeko.feats_clap import Clap
                 self.featExtractor = Clap(f'{store_name}_{self.feats_designation}', self.data_df)
             elif feats_type=='praat':
                 from nkululeko.feats_praat import Praatset
                 self.featExtractor = Praatset(f'{store_name}_{self.feats_designation}', self.data_df)
             elif feats_type=='mld':
```

### Comparing `nkululeko-0.44.1/nkululeko/featureset.py` & `nkululeko-0.45.0/nkululeko/featureset.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.44.1/nkululeko/feinberg_praat.py` & `nkululeko-0.45.0/nkululeko/feinberg_praat.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.44.1/nkululeko/filter_data.py` & `nkululeko-0.45.0/nkululeko/filter_data.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.44.1/nkululeko/loss_ccc.py` & `nkululeko-0.45.0/nkululeko/loss_ccc.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.44.1/nkululeko/loss_softf1loss.py` & `nkululeko-0.45.0/nkululeko/loss_softf1loss.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.44.1/nkululeko/model.py` & `nkululeko-0.45.0/nkululeko/model.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.44.1/nkululeko/model_cnn.py` & `nkululeko-0.45.0/nkululeko/model_cnn.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.44.1/nkululeko/model_gmm.py` & `nkululeko-0.45.0/nkululeko/model_gmm.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.44.1/nkululeko/model_knn.py` & `nkululeko-0.45.0/nkululeko/model_knn.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.44.1/nkululeko/model_knn_reg.py` & `nkululeko-0.45.0/nkululeko/model_knn_reg.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.44.1/nkululeko/model_mlp.py` & `nkululeko-0.45.0/nkululeko/model_mlp.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.44.1/nkululeko/model_mlp_regression.py` & `nkululeko-0.45.0/nkululeko/model_mlp_regression.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.44.1/nkululeko/model_svm.py` & `nkululeko-0.45.0/nkululeko/model_svm.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.44.1/nkululeko/modelrunner.py` & `nkululeko-0.45.0/nkululeko/modelrunner.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.44.1/nkululeko/nkululeko.py` & `nkululeko-0.45.0/nkululeko/nkululeko.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.44.1/nkululeko/plots.py` & `nkululeko-0.45.0/nkululeko/plots.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.44.1/nkululeko/reporter.py` & `nkululeko-0.45.0/nkululeko/reporter.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.44.1/nkululeko/runmanager.py` & `nkululeko-0.45.0/nkululeko/runmanager.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.44.1/nkululeko/scaler.py` & `nkululeko-0.45.0/nkululeko/scaler.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.44.1/nkululeko/test.py` & `nkululeko-0.45.0/nkululeko/test.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.44.1/nkululeko/test_predictor.py` & `nkululeko-0.45.0/nkululeko/test_predictor.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.44.1/nkululeko/util.py` & `nkululeko-0.45.0/nkululeko/util.py`

 * *Files 8% similar despite different names*

```diff
@@ -207,7 +207,23 @@
         for report in best_reports:
             all += str(report.result.test) + ', '
             vals = np.append(vals, report.result.test)
         file_name = f'{res_dir}{self.get_exp_name()}_runs.txt'
         with open(file_name, "w") as text_file:
             text_file.write(all)
             text_file.write(f'\nmean: {vals.mean():.3f}, max: {vals.max():.3f}, max_index: {vals.argmax()}')
+
+    def write_store(self, df, storage, format):
+        if format == 'pkl':
+            df.to_pickle(storage)
+        elif format == 'csv':
+            df.to_csv(storage)
+        else:
+            self.error(f'unkown store format: {format}')
+            
+    def get_store(self, name, format):
+        if format == 'pkl':
+            return pd.read_pickle(name)
+        elif format == 'csv':
+            return audformat.utils.read_csv(name)
+        else:
+            self.error(f'unkown store format: {format}')
```

### Comparing `nkululeko-0.44.1/nkululeko.egg-info/PKG-INFO` & `nkululeko-0.45.0/nkululeko.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nkululeko
-Version: 0.44.1
+Version: 0.45.0
 Summary: Machine learning audio prediction experiments based on templates
 Home-page: https://github.com/felixbur/nkululeko
 Author: Felix Burkhardt
 Author-email: fxburk@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -213,14 +213,25 @@
 =========
 
 Version 0.44.1
 --------------
 * bugfixing: feature importance: https://github.com/felixbur/nkululeko/issues/23
 * bugfixing: loading csv database with filewise index https://github.com/felixbur/nkululeko/issues/24 
 
+
+Version 0.45.0
+--------------
+* added auddim as features
+* added FEATS store_format
+* added device use to feat_audmodel
+
+Version 0.44.1
+--------------
+* bugfixes
+
 Version 0.44.0
 --------------
 * added scatter functions: tsne, pca, umap
 
 Version 0.43.7
 --------------
 * added clap features
```

### Comparing `nkululeko-0.44.1/nkululeko.egg-info/SOURCES.txt` & `nkululeko-0.45.0/nkululeko.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 nkululeko/dataset_ravdess.py
 nkululeko/demo.py
 nkululeko/demo_predictor.py
 nkululeko/experiment.py
 nkululeko/explore.py
 nkululeko/feats_analyser.py
 nkululeko/feats_audmodel.py
+nkululeko/feats_audmodel_dim.py
 nkululeko/feats_clap.py
 nkululeko/feats_import.py
 nkululeko/feats_mld.py
 nkululeko/feats_opensmile.py
 nkululeko/feats_oxbow.py
 nkululeko/feats_praat.py
 nkululeko/feats_trill.py
```

### Comparing `nkululeko-0.44.1/setup.cfg` & `nkululeko-0.45.0/setup.cfg`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = nkululeko
-version = 0.44.1
+version = 0.45.0
 author = Felix Burkhardt
 author_email = fxburk@gmail.com
 description = Machine learning audio prediction experiments based on templates
 long_description = file: README.md, CHANGELOG.md
 long_description_content_type = text/markdown
 url = https://github.com/felixbur/nkululeko
 classifiers =
```

