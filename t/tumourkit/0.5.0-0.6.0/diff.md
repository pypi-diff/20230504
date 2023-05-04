# Comparing `tmp/tumourkit-0.5.0.tar.gz` & `tmp/tumourkit-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tumourkit-0.5.0.tar", last modified: Sun Apr 30 10:23:39 2023, max compression
+gzip compressed data, was "tumourkit-0.6.0.tar", last modified: Thu May  4 18:22:57 2023, max compression
```

## Comparing `tumourkit-0.5.0.tar` & `tumourkit-0.6.0.tar`

### file list

```diff
@@ -1,155 +1,156 @@
-drwxr-xr-x   0 joseperezcano   (501) staff       (20)        0 2023-04-30 10:23:39.274073 tumourkit-0.5.0/
--rw-r--r--   0 joseperezcano   (501) staff       (20)    34523 2022-12-31 13:00:33.000000 tumourkit-0.5.0/LICENSE
--rw-r--r--   0 joseperezcano   (501) staff       (20)    42041 2023-04-30 10:23:39.273084 tumourkit-0.5.0/PKG-INFO
--rw-r--r--   0 joseperezcano   (501) staff       (20)     1269 2023-03-25 17:22:23.000000 tumourkit-0.5.0/README.md
-drwxr-xr-x   0 joseperezcano   (501) staff       (20)        0 2023-04-30 10:23:39.154916 tumourkit-0.5.0/demo/
--rw-r--r--   0 joseperezcano   (501) staff       (20)      670 2023-04-14 09:43:14.000000 tumourkit-0.5.0/demo/app.py
-drwxr-xr-x   0 joseperezcano   (501) staff       (20)        0 2023-04-30 10:23:39.148006 tumourkit-0.5.0/docs/
-drwxr-xr-x   0 joseperezcano   (501) staff       (20)        0 2023-04-30 10:23:39.147811 tumourkit-0.5.0/docs/buildenv/
-drwxr-xr-x   0 joseperezcano   (501) staff       (20)        0 2023-04-30 10:23:39.165438 tumourkit-0.5.0/docs/buildenv/bin/
--rwxr-xr-x   0 joseperezcano   (501) staff       (20)      675 2023-03-25 16:44:11.000000 tumourkit-0.5.0/docs/buildenv/bin/rst2html.py
--rwxr-xr-x   0 joseperezcano   (501) staff       (20)      795 2023-03-25 16:44:11.000000 tumourkit-0.5.0/docs/buildenv/bin/rst2html4.py
--rwxr-xr-x   0 joseperezcano   (501) staff       (20)     1163 2023-03-25 16:44:11.000000 tumourkit-0.5.0/docs/buildenv/bin/rst2html5.py
--rwxr-xr-x   0 joseperezcano   (501) staff       (20)      872 2023-03-25 16:44:11.000000 tumourkit-0.5.0/docs/buildenv/bin/rst2latex.py
--rwxr-xr-x   0 joseperezcano   (501) staff       (20)      680 2023-03-25 16:44:11.000000 tumourkit-0.5.0/docs/buildenv/bin/rst2man.py
--rwxr-xr-x   0 joseperezcano   (501) staff       (20)      845 2023-03-25 16:44:11.000000 tumourkit-0.5.0/docs/buildenv/bin/rst2odt.py
--rwxr-xr-x   0 joseperezcano   (501) staff       (20)     1807 2023-03-25 16:44:11.000000 tumourkit-0.5.0/docs/buildenv/bin/rst2odt_prepstyles.py
--rwxr-xr-x   0 joseperezcano   (501) staff       (20)      682 2023-03-25 16:44:11.000000 tumourkit-0.5.0/docs/buildenv/bin/rst2pseudoxml.py
--rwxr-xr-x   0 joseperezcano   (501) staff       (20)      718 2023-03-25 16:44:11.000000 tumourkit-0.5.0/docs/buildenv/bin/rst2s5.py
--rwxr-xr-x   0 joseperezcano   (501) staff       (20)      952 2023-03-25 16:44:11.000000 tumourkit-0.5.0/docs/buildenv/bin/rst2xetex.py
--rwxr-xr-x   0 joseperezcano   (501) staff       (20)      683 2023-03-25 16:44:11.000000 tumourkit-0.5.0/docs/buildenv/bin/rst2xml.py
--rwxr-xr-x   0 joseperezcano   (501) staff       (20)      751 2023-03-25 16:44:11.000000 tumourkit-0.5.0/docs/buildenv/bin/rstpep2html.py
-drwxr-xr-x   0 joseperezcano   (501) staff       (20)        0 2023-04-30 10:23:39.166073 tumourkit-0.5.0/docs/source/
--rw-r--r--   0 joseperezcano   (501) staff       (20)     1151 2023-04-11 15:21:40.000000 tumourkit-0.5.0/docs/source/conf.py
--rw-r--r--   0 joseperezcano   (501) staff       (20)     2132 2023-04-30 10:02:08.000000 tumourkit-0.5.0/pyproject.toml
--rw-r--r--   0 joseperezcano   (501) staff       (20)      818 2023-03-23 17:22:35.000000 tumourkit-0.5.0/requirements.txt
--rw-r--r--   0 joseperezcano   (501) staff       (20)       38 2023-04-30 10:23:39.274204 tumourkit-0.5.0/setup.cfg
-drwxr-xr-x   0 joseperezcano   (501) staff       (20)        0 2023-04-30 10:23:39.181707 tumourkit-0.5.0/tests/
--rw-r--r--   0 joseperezcano   (501) staff       (20)     1596 2023-03-20 09:45:58.000000 tumourkit-0.5.0/tests/centroidspng2csv_test.py
--rw-r--r--   0 joseperezcano   (501) staff       (20)     1871 2023-03-06 07:41:04.000000 tumourkit-0.5.0/tests/conf_matrix_sum_test.py
--rw-r--r--   0 joseperezcano   (501) staff       (20)     2043 2023-03-06 07:25:02.000000 tumourkit-0.5.0/tests/cpairs_test.py
--rw-r--r--   0 joseperezcano   (501) staff       (20)      805 2023-03-06 07:25:20.000000 tumourkit-0.5.0/tests/example_test.py
--rw-r--r--   0 joseperezcano   (501) staff       (20)     3927 2022-12-31 13:06:14.000000 tumourkit-0.5.0/tests/generate_centroids.py
--rw-r--r--   0 joseperezcano   (501) staff       (20)     3403 2022-12-31 13:06:04.000000 tumourkit-0.5.0/tests/generate_rswoosh.py
--rw-r--r--   0 joseperezcano   (501) staff       (20)     1517 2023-03-06 07:25:59.000000 tumourkit-0.5.0/tests/get_conn_comp_test.py
--rw-r--r--   0 joseperezcano   (501) staff       (20)     1827 2023-03-28 15:20:41.000000 tumourkit-0.5.0/tests/graph2centroids_test.py
--rw-r--r--   0 joseperezcano   (501) staff       (20)     1707 2023-03-20 10:39:44.000000 tumourkit-0.5.0/tests/graph_idx_test.py
--rw-r--r--   0 joseperezcano   (501) staff       (20)     2199 2023-03-23 19:39:56.000000 tumourkit-0.5.0/tests/hov_prob_pipe_test.py
--rw-r--r--   0 joseperezcano   (501) staff       (20)     2098 2023-03-06 07:27:57.000000 tumourkit-0.5.0/tests/hov_prob_test.py
--rw-r--r--   0 joseperezcano   (501) staff       (20)     2503 2023-03-23 07:08:34.000000 tumourkit-0.5.0/tests/hovernet_patches_test.py
--rw-r--r--   0 joseperezcano   (501) staff       (20)     1844 2023-03-06 07:41:02.000000 tumourkit-0.5.0/tests/metrics_pairs_test.py
--rw-r--r--   0 joseperezcano   (501) staff       (20)     1974 2023-03-06 07:41:00.000000 tumourkit-0.5.0/tests/metrics_test.py
--rw-r--r--   0 joseperezcano   (501) staff       (20)     1898 2023-03-20 10:58:10.000000 tumourkit-0.5.0/tests/png2graph_test.py
--rw-r--r--   0 joseperezcano   (501) staff       (20)     2240 2023-03-06 07:30:23.000000 tumourkit-0.5.0/tests/pngcsv2geojson_test.py
--rw-r--r--   0 joseperezcano   (501) staff       (20)     1829 2023-03-20 10:39:00.000000 tumourkit-0.5.0/tests/pngcsv2graph_test.py
--rw-r--r--   0 joseperezcano   (501) staff       (20)     1978 2023-04-12 10:40:07.000000 tumourkit-0.5.0/tests/read_nodes_test.py
--rw-r--r--   0 joseperezcano   (501) staff       (20)     1374 2023-03-06 07:31:03.000000 tumourkit-0.5.0/tests/remove_idx_test.py
--rw-r--r--   0 joseperezcano   (501) staff       (20)     1577 2023-03-06 07:31:28.000000 tumourkit-0.5.0/tests/rswoosh_test.py
-drwxr-xr-x   0 joseperezcano   (501) staff       (20)        0 2023-04-30 10:23:39.186228 tumourkit-0.5.0/tumourkit/
--rw-r--r--   0 joseperezcano   (501) staff       (20)      154 2023-04-30 10:23:28.000000 tumourkit-0.5.0/tumourkit/__init__.py
-drwxr-xr-x   0 joseperezcano   (501) staff       (20)        0 2023-04-30 10:23:39.194486 tumourkit-0.5.0/tumourkit/classification/
--rw-r--r--   0 joseperezcano   (501) staff       (20)      155 2023-04-11 15:25:33.000000 tumourkit-0.5.0/tumourkit/classification/__init__.py
--rw-r--r--   0 joseperezcano   (501) staff       (20)     1349 2023-04-12 10:40:08.000000 tumourkit-0.5.0/tumourkit/classification/compute_imbalance.py
--rw-r--r--   0 joseperezcano   (501) staff       (20)     6072 2023-04-12 10:38:57.000000 tumourkit-0.5.0/tumourkit/classification/evaluate.py
--rw-r--r--   0 joseperezcano   (501) staff       (20)     5318 2023-04-11 18:31:20.000000 tumourkit-0.5.0/tumourkit/classification/infer.py
-drwxr-xr-x   0 joseperezcano   (501) staff       (20)        0 2023-04-30 10:23:39.198049 tumourkit-0.5.0/tumourkit/classification/models/
--rw-r--r--   0 joseperezcano   (501) staff       (20)        0 2022-11-28 08:50:03.000000 tumourkit-0.5.0/tumourkit/classification/models/__init__.py
--rw-r--r--   0 joseperezcano   (501) staff       (20)     2532 2023-03-23 17:44:30.000000 tumourkit-0.5.0/tumourkit/classification/models/gat.py
--rw-r--r--   0 joseperezcano   (501) staff       (20)     2008 2022-12-31 13:10:31.000000 tumourkit-0.5.0/tumourkit/classification/models/gcn.py
--rw-r--r--   0 joseperezcano   (501) staff       (20)     7769 2022-12-31 13:10:48.000000 tumourkit-0.5.0/tumourkit/classification/models/hgao.py
--rw-r--r--   0 joseperezcano   (501) staff       (20)     2840 2022-12-19 09:14:00.000000 tumourkit-0.5.0/tumourkit/classification/models/norm.py
--rw-r--r--   0 joseperezcano   (501) staff       (20)     7489 2023-04-12 10:40:12.000000 tumourkit-0.5.0/tumourkit/classification/read_graph.py
--rw-r--r--   0 joseperezcano   (501) staff       (20)    20584 2023-04-13 09:56:23.000000 tumourkit-0.5.0/tumourkit/classification/train_graphs.py
--rw-r--r--   0 joseperezcano   (501) staff       (20)    10352 2023-04-12 10:40:17.000000 tumourkit-0.5.0/tumourkit/classification/train_xgboost.py
--rw-r--r--   0 joseperezcano   (501) staff       (20)     5590 2023-04-17 07:53:40.000000 tumourkit-0.5.0/tumourkit/eval_pipe.py
--rw-r--r--   0 joseperezcano   (501) staff       (20)     7511 2023-04-17 15:24:46.000000 tumourkit-0.5.0/tumourkit/infer_pipe.py
--rw-r--r--   0 joseperezcano   (501) staff       (20)     3151 2023-03-20 14:38:24.000000 tumourkit-0.5.0/tumourkit/make_dirs.py
-drwxr-xr-x   0 joseperezcano   (501) staff       (20)        0 2023-04-30 10:23:39.202388 tumourkit-0.5.0/tumourkit/postprocessing/
--rw-r--r--   0 joseperezcano   (501) staff       (20)      127 2023-03-09 07:25:32.000000 tumourkit-0.5.0/tumourkit/postprocessing/__init__.py
--rw-r--r--   0 joseperezcano   (501) staff       (20)     3619 2023-03-09 07:58:38.000000 tumourkit-0.5.0/tumourkit/postprocessing/join_graph_gt.py
--rw-r--r--   0 joseperezcano   (501) staff       (20)     5469 2023-03-22 15:42:53.000000 tumourkit-0.5.0/tumourkit/postprocessing/join_hovprob_graph.py
--rw-r--r--   0 joseperezcano   (501) staff       (20)     5332 2023-04-02 17:54:39.000000 tumourkit-0.5.0/tumourkit/postprocessing/merge_cells.py
--rw-r--r--   0 joseperezcano   (501) staff       (20)     1623 2023-01-14 21:36:24.000000 tumourkit-0.5.0/tumourkit/postprocessing/rswoosh.py
-drwxr-xr-x   0 joseperezcano   (501) staff       (20)        0 2023-04-30 10:23:39.214732 tumourkit-0.5.0/tumourkit/preprocessing/
--rw-r--r--   0 joseperezcano   (501) staff       (20)      616 2023-03-20 11:26:08.000000 tumourkit-0.5.0/tumourkit/preprocessing/__init__.py
--rw-r--r--   0 joseperezcano   (501) staff       (20)     2298 2023-03-23 19:01:53.000000 tumourkit-0.5.0/tumourkit/preprocessing/centroids2png.py
--rw-r--r--   0 joseperezcano   (501) staff       (20)     4659 2023-03-25 16:07:13.000000 tumourkit-0.5.0/tumourkit/preprocessing/centroidspng2csv.py
--rw-r--r--   0 joseperezcano   (501) staff       (20)     3894 2023-04-30 09:54:10.000000 tumourkit-0.5.0/tumourkit/preprocessing/geojson2pngcsv.py
--rw-r--r--   0 joseperezcano   (501) staff       (20)     3288 2023-03-28 09:36:18.000000 tumourkit-0.5.0/tumourkit/preprocessing/graph2centroids.py
--rw-r--r--   0 joseperezcano   (501) staff       (20)     2844 2023-03-23 19:09:28.000000 tumourkit-0.5.0/tumourkit/preprocessing/hovernet2centroids.py
--rw-r--r--   0 joseperezcano   (501) staff       (20)     3723 2023-03-23 19:11:32.000000 tumourkit-0.5.0/tumourkit/preprocessing/hovernet2geojson.py
--rw-r--r--   0 joseperezcano   (501) staff       (20)     4731 2023-03-23 19:32:48.000000 tumourkit-0.5.0/tumourkit/preprocessing/png2graph.py
--rw-r--r--   0 joseperezcano   (501) staff       (20)     2775 2023-03-25 16:11:44.000000 tumourkit-0.5.0/tumourkit/preprocessing/pngcsv2centroids.py
--rw-r--r--   0 joseperezcano   (501) staff       (20)     5043 2023-04-30 09:55:47.000000 tumourkit-0.5.0/tumourkit/preprocessing/pngcsv2geojson.py
--rw-r--r--   0 joseperezcano   (501) staff       (20)     3935 2023-03-23 19:32:30.000000 tumourkit-0.5.0/tumourkit/preprocessing/pngcsv2graph.py
--rw-r--r--   0 joseperezcano   (501) staff       (20)     1075 2023-04-30 10:05:05.000000 tumourkit-0.5.0/tumourkit/preprocessing/remove_uncertain.py
-drwxr-xr-x   0 joseperezcano   (501) staff       (20)        0 2023-04-30 10:23:39.216294 tumourkit-0.5.0/tumourkit/profiling/
--rw-r--r--   0 joseperezcano   (501) staff       (20)     2824 2022-12-31 13:07:35.000000 tumourkit-0.5.0/tumourkit/profiling/cpairs_profile.py
--rw-r--r--   0 joseperezcano   (501) staff       (20)     1946 2022-12-31 13:07:42.000000 tumourkit-0.5.0/tumourkit/profiling/rswoosh_profile.py
--rw-r--r--   0 joseperezcano   (501) staff       (20)    14758 2023-04-26 19:41:21.000000 tumourkit-0.5.0/tumourkit/research_pipe.py
-drwxr-xr-x   0 joseperezcano   (501) staff       (20)        0 2023-04-30 10:23:39.226608 tumourkit-0.5.0/tumourkit/segmentation/
--rw-r--r--   0 joseperezcano   (501) staff       (20)      182 2023-03-08 12:07:32.000000 tumourkit-0.5.0/tumourkit/segmentation/__init__.py
--rw-r--r--   0 joseperezcano   (501) staff       (20)    12265 2023-04-27 10:59:55.000000 tumourkit-0.5.0/tumourkit/segmentation/evaluate.py
-drwxr-xr-x   0 joseperezcano   (501) staff       (20)        0 2023-04-30 10:23:39.233366 tumourkit-0.5.0/tumourkit/segmentation/hovernet/
--rwx------   0 joseperezcano   (501) staff       (20)        0 2023-03-08 08:02:19.000000 tumourkit-0.5.0/tumourkit/segmentation/hovernet/__init__.py
--rwx------   0 joseperezcano   (501) staff       (20)     2380 2023-03-20 14:44:06.000000 tumourkit-0.5.0/tumourkit/segmentation/hovernet/config.py
-drwxr-xr-x   0 joseperezcano   (501) staff       (20)        0 2023-04-30 10:23:39.237814 tumourkit-0.5.0/tumourkit/segmentation/hovernet/dataloader/
--rwx------   0 joseperezcano   (501) staff       (20)        0 2022-09-15 10:27:49.000000 tumourkit-0.5.0/tumourkit/segmentation/hovernet/dataloader/__init__.py
--rwx------   0 joseperezcano   (501) staff       (20)     3322 2023-04-13 06:48:37.000000 tumourkit-0.5.0/tumourkit/segmentation/hovernet/dataloader/augs.py
--rwx------   0 joseperezcano   (501) staff       (20)     3608 2023-01-26 12:04:04.000000 tumourkit-0.5.0/tumourkit/segmentation/hovernet/dataloader/infer_loader.py
--rwxr-xr-x   0 joseperezcano   (501) staff       (20)     6632 2023-03-15 12:03:08.000000 tumourkit-0.5.0/tumourkit/segmentation/hovernet/dataloader/train_loader.py
--rwx------   0 joseperezcano   (501) staff       (20)     8251 2023-03-08 08:12:38.000000 tumourkit-0.5.0/tumourkit/segmentation/hovernet/extract_patches.py
-drwxr-xr-x   0 joseperezcano   (501) staff       (20)        0 2023-04-30 10:23:39.243665 tumourkit-0.5.0/tumourkit/segmentation/hovernet/infer/
--rwx------   0 joseperezcano   (501) staff       (20)        0 2022-09-15 10:27:53.000000 tumourkit-0.5.0/tumourkit/segmentation/hovernet/infer/__init__.py
--rwx------   0 joseperezcano   (501) staff       (20)     3281 2023-03-22 07:18:47.000000 tumourkit-0.5.0/tumourkit/segmentation/hovernet/infer/base.py
--rwx------   0 joseperezcano   (501) staff       (20)    14233 2023-03-08 12:23:40.000000 tumourkit-0.5.0/tumourkit/segmentation/hovernet/infer/tile.py
--rwx------   0 joseperezcano   (501) staff       (20)    30145 2023-03-23 17:33:09.000000 tumourkit-0.5.0/tumourkit/segmentation/hovernet/infer/wsi.py
-drwxr-xr-x   0 joseperezcano   (501) staff       (20)        0 2023-04-30 10:23:39.245970 tumourkit-0.5.0/tumourkit/segmentation/hovernet/metrics/
--rwx------   0 joseperezcano   (501) staff       (20)        0 2022-09-15 10:27:53.000000 tumourkit-0.5.0/tumourkit/segmentation/hovernet/metrics/__init__.py
--rwx------   0 joseperezcano   (501) staff       (20)    16129 2023-01-10 14:25:36.000000 tumourkit-0.5.0/tumourkit/segmentation/hovernet/metrics/stats_utils.py
-drwxr-xr-x   0 joseperezcano   (501) staff       (20)        0 2023-04-30 10:23:39.249838 tumourkit-0.5.0/tumourkit/segmentation/hovernet/misc/
--rwx------   0 joseperezcano   (501) staff       (20)        0 2022-09-15 10:27:53.000000 tumourkit-0.5.0/tumourkit/segmentation/hovernet/misc/__init__.py
--rwx------   0 joseperezcano   (501) staff       (20)     5473 2023-01-10 14:24:57.000000 tumourkit-0.5.0/tumourkit/segmentation/hovernet/misc/patch_extractor.py
--rwx------   0 joseperezcano   (501) staff       (20)     4951 2023-01-10 14:25:05.000000 tumourkit-0.5.0/tumourkit/segmentation/hovernet/misc/utils.py
--rwx------   0 joseperezcano   (501) staff       (20)     5727 2023-01-10 14:25:12.000000 tumourkit-0.5.0/tumourkit/segmentation/hovernet/misc/viz_utils.py
--rwx------   0 joseperezcano   (501) staff       (20)     7419 2023-01-10 14:25:19.000000 tumourkit-0.5.0/tumourkit/segmentation/hovernet/misc/wsi_handler.py
-drwxr-xr-x   0 joseperezcano   (501) staff       (20)        0 2023-04-30 10:23:39.250835 tumourkit-0.5.0/tumourkit/segmentation/hovernet/models/
--rwx------   0 joseperezcano   (501) staff       (20)        0 2022-09-15 10:27:53.000000 tumourkit-0.5.0/tumourkit/segmentation/hovernet/models/__init__.py
-drwxr-xr-x   0 joseperezcano   (501) staff       (20)        0 2023-04-30 10:23:39.256147 tumourkit-0.5.0/tumourkit/segmentation/hovernet/models/hovernet/
--rwx------   0 joseperezcano   (501) staff       (20)        0 2022-09-15 10:27:53.000000 tumourkit-0.5.0/tumourkit/segmentation/hovernet/models/hovernet/__init__.py
--rwx------   0 joseperezcano   (501) staff       (20)     5421 2023-01-10 14:23:15.000000 tumourkit-0.5.0/tumourkit/segmentation/hovernet/models/hovernet/net_desc.py
--rwx------   0 joseperezcano   (501) staff       (20)     9731 2023-01-10 14:23:26.000000 tumourkit-0.5.0/tumourkit/segmentation/hovernet/models/hovernet/net_utils.py
--rwx------   0 joseperezcano   (501) staff       (20)     6130 2023-03-15 07:07:22.000000 tumourkit-0.5.0/tumourkit/segmentation/hovernet/models/hovernet/opt.py
--rwx------   0 joseperezcano   (501) staff       (20)     7784 2023-03-22 08:36:42.000000 tumourkit-0.5.0/tumourkit/segmentation/hovernet/models/hovernet/post_proc.py
--rwx------   0 joseperezcano   (501) staff       (20)    13296 2023-03-13 19:48:31.000000 tumourkit-0.5.0/tumourkit/segmentation/hovernet/models/hovernet/run_desc.py
--rwx------   0 joseperezcano   (501) staff       (20)     5117 2023-04-25 06:50:35.000000 tumourkit-0.5.0/tumourkit/segmentation/hovernet/models/hovernet/targets.py
--rwx------   0 joseperezcano   (501) staff       (20)     4903 2023-01-10 16:18:24.000000 tumourkit-0.5.0/tumourkit/segmentation/hovernet/models/hovernet/utils.py
--rwx------   0 joseperezcano   (501) staff       (20)     8272 2023-03-08 12:23:15.000000 tumourkit-0.5.0/tumourkit/segmentation/hovernet/run_infer.py
-drwxr-xr-x   0 joseperezcano   (501) staff       (20)        0 2023-04-30 10:23:39.258064 tumourkit-0.5.0/tumourkit/segmentation/hovernet/run_utils/
--rwx------   0 joseperezcano   (501) staff       (20)        0 2022-09-15 10:27:54.000000 tumourkit-0.5.0/tumourkit/segmentation/hovernet/run_utils/__init__.py
-drwxr-xr-x   0 joseperezcano   (501) staff       (20)        0 2023-04-30 10:23:39.262961 tumourkit-0.5.0/tumourkit/segmentation/hovernet/run_utils/callbacks/
--rwx------   0 joseperezcano   (501) staff       (20)        0 2022-09-15 10:27:54.000000 tumourkit-0.5.0/tumourkit/segmentation/hovernet/run_utils/callbacks/__init__.py
--rwx------   0 joseperezcano   (501) staff       (20)     6991 2023-01-11 07:50:22.000000 tumourkit-0.5.0/tumourkit/segmentation/hovernet/run_utils/callbacks/base.py
--rwx------   0 joseperezcano   (501) staff       (20)     6145 2022-09-15 10:27:54.000000 tumourkit-0.5.0/tumourkit/segmentation/hovernet/run_utils/callbacks/logging.py
--rwx------   0 joseperezcano   (501) staff       (20)     5955 2023-01-13 16:18:56.000000 tumourkit-0.5.0/tumourkit/segmentation/hovernet/run_utils/callbacks/serialize.py
--rwx------   0 joseperezcano   (501) staff       (20)     7482 2023-04-13 06:55:55.000000 tumourkit-0.5.0/tumourkit/segmentation/hovernet/run_utils/engine.py
--rwx------   0 joseperezcano   (501) staff       (20)     6834 2023-01-10 14:22:13.000000 tumourkit-0.5.0/tumourkit/segmentation/hovernet/run_utils/utils.py
--rwx------   0 joseperezcano   (501) staff       (20)    10663 2023-03-23 18:07:29.000000 tumourkit-0.5.0/tumourkit/segmentation/hovernet/train.py
--rw-r--r--   0 joseperezcano   (501) staff       (20)     9861 2023-04-17 15:13:33.000000 tumourkit-0.5.0/tumourkit/train_pipe.py
-drwxr-xr-x   0 joseperezcano   (501) staff       (20)        0 2023-04-30 10:23:39.271797 tumourkit-0.5.0/tumourkit/utils/
--rw-r--r--   0 joseperezcano   (501) staff       (20)        0 2022-09-26 11:04:45.000000 tumourkit-0.5.0/tumourkit/utils/__init__.py
--rw-r--r--   0 joseperezcano   (501) staff       (20)     5932 2023-03-23 17:37:13.000000 tumourkit-0.5.0/tumourkit/utils/calibration_error.py
--rw-r--r--   0 joseperezcano   (501) staff       (20)     5628 2023-04-12 10:40:15.000000 tumourkit-0.5.0/tumourkit/utils/classification.py
--rw-r--r--   0 joseperezcano   (501) staff       (20)     3606 2023-03-23 18:25:35.000000 tumourkit-0.5.0/tumourkit/utils/folder2txt.py
--rw-r--r--   0 joseperezcano   (501) staff       (20)     5254 2023-03-23 18:29:29.000000 tumourkit-0.5.0/tumourkit/utils/nearest.py
--rw-r--r--   0 joseperezcano   (501) staff       (20)     3094 2023-04-22 10:28:27.000000 tumourkit-0.5.0/tumourkit/utils/pipes.py
--rw-r--r--   0 joseperezcano   (501) staff       (20)     7022 2023-03-23 18:35:15.000000 tumourkit-0.5.0/tumourkit/utils/postprocessing.py
--rw-r--r--   0 joseperezcano   (501) staff       (20)    21866 2023-04-30 10:04:39.000000 tumourkit-0.5.0/tumourkit/utils/preprocessing.py
--rw-r--r--   0 joseperezcano   (501) staff       (20)     5670 2023-04-12 10:40:06.000000 tumourkit-0.5.0/tumourkit/utils/read_nodes.py
-drwxr-xr-x   0 joseperezcano   (501) staff       (20)        0 2023-04-30 10:23:39.189229 tumourkit-0.5.0/tumourkit.egg-info/
--rw-r--r--   0 joseperezcano   (501) staff       (20)    42041 2023-04-30 10:23:39.000000 tumourkit-0.5.0/tumourkit.egg-info/PKG-INFO
--rw-r--r--   0 joseperezcano   (501) staff       (20)     4860 2023-04-30 10:23:39.000000 tumourkit-0.5.0/tumourkit.egg-info/SOURCES.txt
--rw-r--r--   0 joseperezcano   (501) staff       (20)        1 2023-04-30 10:23:39.000000 tumourkit-0.5.0/tumourkit.egg-info/dependency_links.txt
--rw-r--r--   0 joseperezcano   (501) staff       (20)      910 2023-04-30 10:23:39.000000 tumourkit-0.5.0/tumourkit.egg-info/entry_points.txt
--rw-r--r--   0 joseperezcano   (501) staff       (20)      818 2023-04-30 10:23:39.000000 tumourkit-0.5.0/tumourkit.egg-info/requires.txt
--rw-r--r--   0 joseperezcano   (501) staff       (20)       31 2023-04-30 10:23:39.000000 tumourkit-0.5.0/tumourkit.egg-info/top_level.txt
+drwxr-xr-x   0 joseperezcano   (501) staff       (20)        0 2023-05-04 18:22:57.163659 tumourkit-0.6.0/
+-rw-r--r--   0 joseperezcano   (501) staff       (20)    34523 2022-12-31 13:00:33.000000 tumourkit-0.6.0/LICENSE
+-rw-r--r--   0 joseperezcano   (501) staff       (20)    42041 2023-05-04 18:22:57.163143 tumourkit-0.6.0/PKG-INFO
+-rw-r--r--   0 joseperezcano   (501) staff       (20)     1269 2023-03-25 17:22:23.000000 tumourkit-0.6.0/README.md
+drwxr-xr-x   0 joseperezcano   (501) staff       (20)        0 2023-05-04 18:22:57.039022 tumourkit-0.6.0/docs/
+drwxr-xr-x   0 joseperezcano   (501) staff       (20)        0 2023-05-04 18:22:57.038843 tumourkit-0.6.0/docs/buildenv/
+drwxr-xr-x   0 joseperezcano   (501) staff       (20)        0 2023-05-04 18:22:57.053707 tumourkit-0.6.0/docs/buildenv/bin/
+-rwxr-xr-x   0 joseperezcano   (501) staff       (20)      675 2023-03-25 16:44:11.000000 tumourkit-0.6.0/docs/buildenv/bin/rst2html.py
+-rwxr-xr-x   0 joseperezcano   (501) staff       (20)      795 2023-03-25 16:44:11.000000 tumourkit-0.6.0/docs/buildenv/bin/rst2html4.py
+-rwxr-xr-x   0 joseperezcano   (501) staff       (20)     1163 2023-03-25 16:44:11.000000 tumourkit-0.6.0/docs/buildenv/bin/rst2html5.py
+-rwxr-xr-x   0 joseperezcano   (501) staff       (20)      872 2023-03-25 16:44:11.000000 tumourkit-0.6.0/docs/buildenv/bin/rst2latex.py
+-rwxr-xr-x   0 joseperezcano   (501) staff       (20)      680 2023-03-25 16:44:11.000000 tumourkit-0.6.0/docs/buildenv/bin/rst2man.py
+-rwxr-xr-x   0 joseperezcano   (501) staff       (20)      845 2023-03-25 16:44:11.000000 tumourkit-0.6.0/docs/buildenv/bin/rst2odt.py
+-rwxr-xr-x   0 joseperezcano   (501) staff       (20)     1807 2023-03-25 16:44:11.000000 tumourkit-0.6.0/docs/buildenv/bin/rst2odt_prepstyles.py
+-rwxr-xr-x   0 joseperezcano   (501) staff       (20)      682 2023-03-25 16:44:11.000000 tumourkit-0.6.0/docs/buildenv/bin/rst2pseudoxml.py
+-rwxr-xr-x   0 joseperezcano   (501) staff       (20)      718 2023-03-25 16:44:11.000000 tumourkit-0.6.0/docs/buildenv/bin/rst2s5.py
+-rwxr-xr-x   0 joseperezcano   (501) staff       (20)      952 2023-03-25 16:44:11.000000 tumourkit-0.6.0/docs/buildenv/bin/rst2xetex.py
+-rwxr-xr-x   0 joseperezcano   (501) staff       (20)      683 2023-03-25 16:44:11.000000 tumourkit-0.6.0/docs/buildenv/bin/rst2xml.py
+-rwxr-xr-x   0 joseperezcano   (501) staff       (20)      751 2023-03-25 16:44:11.000000 tumourkit-0.6.0/docs/buildenv/bin/rstpep2html.py
+drwxr-xr-x   0 joseperezcano   (501) staff       (20)        0 2023-05-04 18:22:57.054458 tumourkit-0.6.0/docs/source/
+-rw-r--r--   0 joseperezcano   (501) staff       (20)     1151 2023-04-11 15:21:40.000000 tumourkit-0.6.0/docs/source/conf.py
+-rw-r--r--   0 joseperezcano   (501) staff       (20)     2226 2023-05-04 05:50:12.000000 tumourkit-0.6.0/pyproject.toml
+-rw-r--r--   0 joseperezcano   (501) staff       (20)      856 2023-05-04 18:20:19.000000 tumourkit-0.6.0/requirements.txt
+-rw-r--r--   0 joseperezcano   (501) staff       (20)       38 2023-05-04 18:22:57.163807 tumourkit-0.6.0/setup.cfg
+drwxr-xr-x   0 joseperezcano   (501) staff       (20)        0 2023-05-04 18:22:57.075620 tumourkit-0.6.0/tests/
+-rw-r--r--   0 joseperezcano   (501) staff       (20)     1596 2023-03-20 09:45:58.000000 tumourkit-0.6.0/tests/centroidspng2csv_test.py
+-rw-r--r--   0 joseperezcano   (501) staff       (20)     1871 2023-03-06 07:41:04.000000 tumourkit-0.6.0/tests/conf_matrix_sum_test.py
+-rw-r--r--   0 joseperezcano   (501) staff       (20)     2043 2023-03-06 07:25:02.000000 tumourkit-0.6.0/tests/cpairs_test.py
+-rw-r--r--   0 joseperezcano   (501) staff       (20)      805 2023-03-06 07:25:20.000000 tumourkit-0.6.0/tests/example_test.py
+-rw-r--r--   0 joseperezcano   (501) staff       (20)     3927 2022-12-31 13:06:14.000000 tumourkit-0.6.0/tests/generate_centroids.py
+-rw-r--r--   0 joseperezcano   (501) staff       (20)     3403 2022-12-31 13:06:04.000000 tumourkit-0.6.0/tests/generate_rswoosh.py
+-rw-r--r--   0 joseperezcano   (501) staff       (20)     1517 2023-03-06 07:25:59.000000 tumourkit-0.6.0/tests/get_conn_comp_test.py
+-rw-r--r--   0 joseperezcano   (501) staff       (20)     1827 2023-03-28 15:20:41.000000 tumourkit-0.6.0/tests/graph2centroids_test.py
+-rw-r--r--   0 joseperezcano   (501) staff       (20)     1707 2023-03-20 10:39:44.000000 tumourkit-0.6.0/tests/graph_idx_test.py
+-rw-r--r--   0 joseperezcano   (501) staff       (20)     2199 2023-03-23 19:39:56.000000 tumourkit-0.6.0/tests/hov_prob_pipe_test.py
+-rw-r--r--   0 joseperezcano   (501) staff       (20)     2098 2023-03-06 07:27:57.000000 tumourkit-0.6.0/tests/hov_prob_test.py
+-rw-r--r--   0 joseperezcano   (501) staff       (20)     2503 2023-03-23 07:08:34.000000 tumourkit-0.6.0/tests/hovernet_patches_test.py
+-rw-r--r--   0 joseperezcano   (501) staff       (20)     1844 2023-03-06 07:41:02.000000 tumourkit-0.6.0/tests/metrics_pairs_test.py
+-rw-r--r--   0 joseperezcano   (501) staff       (20)     1974 2023-03-06 07:41:00.000000 tumourkit-0.6.0/tests/metrics_test.py
+-rw-r--r--   0 joseperezcano   (501) staff       (20)     1898 2023-03-20 10:58:10.000000 tumourkit-0.6.0/tests/png2graph_test.py
+-rw-r--r--   0 joseperezcano   (501) staff       (20)     2240 2023-03-06 07:30:23.000000 tumourkit-0.6.0/tests/pngcsv2geojson_test.py
+-rw-r--r--   0 joseperezcano   (501) staff       (20)     1829 2023-03-20 10:39:00.000000 tumourkit-0.6.0/tests/pngcsv2graph_test.py
+-rw-r--r--   0 joseperezcano   (501) staff       (20)     1978 2023-04-12 10:40:07.000000 tumourkit-0.6.0/tests/read_nodes_test.py
+-rw-r--r--   0 joseperezcano   (501) staff       (20)     1374 2023-03-06 07:31:03.000000 tumourkit-0.6.0/tests/remove_idx_test.py
+-rw-r--r--   0 joseperezcano   (501) staff       (20)     1577 2023-03-06 07:31:28.000000 tumourkit-0.6.0/tests/rswoosh_test.py
+drwxr-xr-x   0 joseperezcano   (501) staff       (20)        0 2023-05-04 18:22:57.083781 tumourkit-0.6.0/tumourkit/
+-rw-r--r--   0 joseperezcano   (501) staff       (20)      154 2023-04-30 10:24:02.000000 tumourkit-0.6.0/tumourkit/__init__.py
+drwxr-xr-x   0 joseperezcano   (501) staff       (20)        0 2023-05-04 18:22:57.089478 tumourkit-0.6.0/tumourkit/classification/
+-rw-r--r--   0 joseperezcano   (501) staff       (20)      155 2023-04-11 15:25:33.000000 tumourkit-0.6.0/tumourkit/classification/__init__.py
+-rw-r--r--   0 joseperezcano   (501) staff       (20)     1349 2023-04-12 10:40:08.000000 tumourkit-0.6.0/tumourkit/classification/compute_imbalance.py
+-rw-r--r--   0 joseperezcano   (501) staff       (20)     6072 2023-04-12 10:38:57.000000 tumourkit-0.6.0/tumourkit/classification/evaluate.py
+-rw-r--r--   0 joseperezcano   (501) staff       (20)     5318 2023-04-11 18:31:20.000000 tumourkit-0.6.0/tumourkit/classification/infer.py
+drwxr-xr-x   0 joseperezcano   (501) staff       (20)        0 2023-05-04 18:22:57.091791 tumourkit-0.6.0/tumourkit/classification/models/
+-rw-r--r--   0 joseperezcano   (501) staff       (20)        0 2022-11-28 08:50:03.000000 tumourkit-0.6.0/tumourkit/classification/models/__init__.py
+-rw-r--r--   0 joseperezcano   (501) staff       (20)     2532 2023-03-23 17:44:30.000000 tumourkit-0.6.0/tumourkit/classification/models/gat.py
+-rw-r--r--   0 joseperezcano   (501) staff       (20)     2008 2022-12-31 13:10:31.000000 tumourkit-0.6.0/tumourkit/classification/models/gcn.py
+-rw-r--r--   0 joseperezcano   (501) staff       (20)     7769 2022-12-31 13:10:48.000000 tumourkit-0.6.0/tumourkit/classification/models/hgao.py
+-rw-r--r--   0 joseperezcano   (501) staff       (20)     2840 2022-12-19 09:14:00.000000 tumourkit-0.6.0/tumourkit/classification/models/norm.py
+-rw-r--r--   0 joseperezcano   (501) staff       (20)     7489 2023-04-12 10:40:12.000000 tumourkit-0.6.0/tumourkit/classification/read_graph.py
+-rw-r--r--   0 joseperezcano   (501) staff       (20)    20584 2023-05-01 12:03:44.000000 tumourkit-0.6.0/tumourkit/classification/train_graphs.py
+-rw-r--r--   0 joseperezcano   (501) staff       (20)    10352 2023-04-12 10:40:17.000000 tumourkit-0.6.0/tumourkit/classification/train_xgboost.py
+drwxr-xr-x   0 joseperezcano   (501) staff       (20)        0 2023-05-04 18:22:57.092350 tumourkit-0.6.0/tumourkit/demo/
+-rw-r--r--   0 joseperezcano   (501) staff       (20)    12908 2023-05-04 15:31:12.000000 tumourkit-0.6.0/tumourkit/demo/app.py
+-rw-r--r--   0 joseperezcano   (501) staff       (20)     5613 2023-05-01 12:07:14.000000 tumourkit-0.6.0/tumourkit/eval_pipe.py
+-rw-r--r--   0 joseperezcano   (501) staff       (20)     7511 2023-04-17 15:24:46.000000 tumourkit-0.6.0/tumourkit/infer_pipe.py
+-rw-r--r--   0 joseperezcano   (501) staff       (20)     3151 2023-03-20 14:38:24.000000 tumourkit-0.6.0/tumourkit/make_dirs.py
+drwxr-xr-x   0 joseperezcano   (501) staff       (20)        0 2023-05-04 18:22:57.095546 tumourkit-0.6.0/tumourkit/postprocessing/
+-rw-r--r--   0 joseperezcano   (501) staff       (20)      180 2023-05-03 07:48:49.000000 tumourkit-0.6.0/tumourkit/postprocessing/__init__.py
+-rw-r--r--   0 joseperezcano   (501) staff       (20)     2601 2023-05-04 07:23:47.000000 tumourkit-0.6.0/tumourkit/postprocessing/draw_cells.py
+-rw-r--r--   0 joseperezcano   (501) staff       (20)     3619 2023-03-09 07:58:38.000000 tumourkit-0.6.0/tumourkit/postprocessing/join_graph_gt.py
+-rw-r--r--   0 joseperezcano   (501) staff       (20)     5469 2023-03-22 15:42:53.000000 tumourkit-0.6.0/tumourkit/postprocessing/join_hovprob_graph.py
+-rw-r--r--   0 joseperezcano   (501) staff       (20)     5332 2023-04-02 17:54:39.000000 tumourkit-0.6.0/tumourkit/postprocessing/merge_cells.py
+-rw-r--r--   0 joseperezcano   (501) staff       (20)     1623 2023-01-14 21:36:24.000000 tumourkit-0.6.0/tumourkit/postprocessing/rswoosh.py
+drwxr-xr-x   0 joseperezcano   (501) staff       (20)        0 2023-05-04 18:22:57.100141 tumourkit-0.6.0/tumourkit/preprocessing/
+-rw-r--r--   0 joseperezcano   (501) staff       (20)      616 2023-03-20 11:26:08.000000 tumourkit-0.6.0/tumourkit/preprocessing/__init__.py
+-rw-r--r--   0 joseperezcano   (501) staff       (20)     2298 2023-03-23 19:01:53.000000 tumourkit-0.6.0/tumourkit/preprocessing/centroids2png.py
+-rw-r--r--   0 joseperezcano   (501) staff       (20)     4659 2023-03-25 16:07:13.000000 tumourkit-0.6.0/tumourkit/preprocessing/centroidspng2csv.py
+-rw-r--r--   0 joseperezcano   (501) staff       (20)     3894 2023-04-30 09:54:10.000000 tumourkit-0.6.0/tumourkit/preprocessing/geojson2pngcsv.py
+-rw-r--r--   0 joseperezcano   (501) staff       (20)     3288 2023-03-28 09:36:18.000000 tumourkit-0.6.0/tumourkit/preprocessing/graph2centroids.py
+-rw-r--r--   0 joseperezcano   (501) staff       (20)     2844 2023-03-23 19:09:28.000000 tumourkit-0.6.0/tumourkit/preprocessing/hovernet2centroids.py
+-rw-r--r--   0 joseperezcano   (501) staff       (20)     3723 2023-03-23 19:11:32.000000 tumourkit-0.6.0/tumourkit/preprocessing/hovernet2geojson.py
+-rw-r--r--   0 joseperezcano   (501) staff       (20)     4731 2023-03-23 19:32:48.000000 tumourkit-0.6.0/tumourkit/preprocessing/png2graph.py
+-rw-r--r--   0 joseperezcano   (501) staff       (20)     2775 2023-03-25 16:11:44.000000 tumourkit-0.6.0/tumourkit/preprocessing/pngcsv2centroids.py
+-rw-r--r--   0 joseperezcano   (501) staff       (20)     5043 2023-04-30 09:55:47.000000 tumourkit-0.6.0/tumourkit/preprocessing/pngcsv2geojson.py
+-rw-r--r--   0 joseperezcano   (501) staff       (20)     3935 2023-03-23 19:32:30.000000 tumourkit-0.6.0/tumourkit/preprocessing/pngcsv2graph.py
+-rw-r--r--   0 joseperezcano   (501) staff       (20)     1075 2023-04-30 10:05:05.000000 tumourkit-0.6.0/tumourkit/preprocessing/remove_uncertain.py
+drwxr-xr-x   0 joseperezcano   (501) staff       (20)        0 2023-05-04 18:22:57.101134 tumourkit-0.6.0/tumourkit/profiling/
+-rw-r--r--   0 joseperezcano   (501) staff       (20)     2824 2022-12-31 13:07:35.000000 tumourkit-0.6.0/tumourkit/profiling/cpairs_profile.py
+-rw-r--r--   0 joseperezcano   (501) staff       (20)     1946 2022-12-31 13:07:42.000000 tumourkit-0.6.0/tumourkit/profiling/rswoosh_profile.py
+-rw-r--r--   0 joseperezcano   (501) staff       (20)    14757 2023-05-03 12:46:59.000000 tumourkit-0.6.0/tumourkit/research_pipe.py
+drwxr-xr-x   0 joseperezcano   (501) staff       (20)        0 2023-05-04 18:22:57.102479 tumourkit-0.6.0/tumourkit/segmentation/
+-rw-r--r--   0 joseperezcano   (501) staff       (20)      182 2023-03-08 12:07:32.000000 tumourkit-0.6.0/tumourkit/segmentation/__init__.py
+-rw-r--r--   0 joseperezcano   (501) staff       (20)    12265 2023-04-27 10:59:55.000000 tumourkit-0.6.0/tumourkit/segmentation/evaluate.py
+drwxr-xr-x   0 joseperezcano   (501) staff       (20)        0 2023-05-04 18:22:57.105024 tumourkit-0.6.0/tumourkit/segmentation/hovernet/
+-rwx------   0 joseperezcano   (501) staff       (20)        0 2023-03-08 08:02:19.000000 tumourkit-0.6.0/tumourkit/segmentation/hovernet/__init__.py
+-rwx------   0 joseperezcano   (501) staff       (20)     2380 2023-03-20 14:44:06.000000 tumourkit-0.6.0/tumourkit/segmentation/hovernet/config.py
+drwxr-xr-x   0 joseperezcano   (501) staff       (20)        0 2023-05-04 18:22:57.108209 tumourkit-0.6.0/tumourkit/segmentation/hovernet/dataloader/
+-rwx------   0 joseperezcano   (501) staff       (20)        0 2022-09-15 10:27:49.000000 tumourkit-0.6.0/tumourkit/segmentation/hovernet/dataloader/__init__.py
+-rwx------   0 joseperezcano   (501) staff       (20)     3322 2023-04-13 06:48:37.000000 tumourkit-0.6.0/tumourkit/segmentation/hovernet/dataloader/augs.py
+-rwx------   0 joseperezcano   (501) staff       (20)     3608 2023-01-26 12:04:04.000000 tumourkit-0.6.0/tumourkit/segmentation/hovernet/dataloader/infer_loader.py
+-rwxr-xr-x   0 joseperezcano   (501) staff       (20)     6632 2023-03-15 12:03:08.000000 tumourkit-0.6.0/tumourkit/segmentation/hovernet/dataloader/train_loader.py
+-rwx------   0 joseperezcano   (501) staff       (20)     8251 2023-03-08 08:12:38.000000 tumourkit-0.6.0/tumourkit/segmentation/hovernet/extract_patches.py
+drwxr-xr-x   0 joseperezcano   (501) staff       (20)        0 2023-05-04 18:22:57.115379 tumourkit-0.6.0/tumourkit/segmentation/hovernet/infer/
+-rwx------   0 joseperezcano   (501) staff       (20)        0 2022-09-15 10:27:53.000000 tumourkit-0.6.0/tumourkit/segmentation/hovernet/infer/__init__.py
+-rwx------   0 joseperezcano   (501) staff       (20)     3497 2023-05-03 12:16:27.000000 tumourkit-0.6.0/tumourkit/segmentation/hovernet/infer/base.py
+-rwx------   0 joseperezcano   (501) staff       (20)    14233 2023-03-08 12:23:40.000000 tumourkit-0.6.0/tumourkit/segmentation/hovernet/infer/tile.py
+-rwx------   0 joseperezcano   (501) staff       (20)    30145 2023-03-23 17:33:09.000000 tumourkit-0.6.0/tumourkit/segmentation/hovernet/infer/wsi.py
+drwxr-xr-x   0 joseperezcano   (501) staff       (20)        0 2023-05-04 18:22:57.119873 tumourkit-0.6.0/tumourkit/segmentation/hovernet/metrics/
+-rwx------   0 joseperezcano   (501) staff       (20)        0 2022-09-15 10:27:53.000000 tumourkit-0.6.0/tumourkit/segmentation/hovernet/metrics/__init__.py
+-rwx------   0 joseperezcano   (501) staff       (20)    16129 2023-01-10 14:25:36.000000 tumourkit-0.6.0/tumourkit/segmentation/hovernet/metrics/stats_utils.py
+drwxr-xr-x   0 joseperezcano   (501) staff       (20)        0 2023-05-04 18:22:57.131029 tumourkit-0.6.0/tumourkit/segmentation/hovernet/misc/
+-rwx------   0 joseperezcano   (501) staff       (20)        0 2022-09-15 10:27:53.000000 tumourkit-0.6.0/tumourkit/segmentation/hovernet/misc/__init__.py
+-rwx------   0 joseperezcano   (501) staff       (20)     5473 2023-01-10 14:24:57.000000 tumourkit-0.6.0/tumourkit/segmentation/hovernet/misc/patch_extractor.py
+-rwx------   0 joseperezcano   (501) staff       (20)     4951 2023-01-10 14:25:05.000000 tumourkit-0.6.0/tumourkit/segmentation/hovernet/misc/utils.py
+-rwx------   0 joseperezcano   (501) staff       (20)     5727 2023-01-10 14:25:12.000000 tumourkit-0.6.0/tumourkit/segmentation/hovernet/misc/viz_utils.py
+-rwx------   0 joseperezcano   (501) staff       (20)     7419 2023-01-10 14:25:19.000000 tumourkit-0.6.0/tumourkit/segmentation/hovernet/misc/wsi_handler.py
+drwxr-xr-x   0 joseperezcano   (501) staff       (20)        0 2023-05-04 18:22:57.131735 tumourkit-0.6.0/tumourkit/segmentation/hovernet/models/
+-rwx------   0 joseperezcano   (501) staff       (20)        0 2022-09-15 10:27:53.000000 tumourkit-0.6.0/tumourkit/segmentation/hovernet/models/__init__.py
+drwxr-xr-x   0 joseperezcano   (501) staff       (20)        0 2023-05-04 18:22:57.144098 tumourkit-0.6.0/tumourkit/segmentation/hovernet/models/hovernet/
+-rwx------   0 joseperezcano   (501) staff       (20)        0 2022-09-15 10:27:53.000000 tumourkit-0.6.0/tumourkit/segmentation/hovernet/models/hovernet/__init__.py
+-rwx------   0 joseperezcano   (501) staff       (20)     5421 2023-01-10 14:23:15.000000 tumourkit-0.6.0/tumourkit/segmentation/hovernet/models/hovernet/net_desc.py
+-rwx------   0 joseperezcano   (501) staff       (20)     9731 2023-01-10 14:23:26.000000 tumourkit-0.6.0/tumourkit/segmentation/hovernet/models/hovernet/net_utils.py
+-rwx------   0 joseperezcano   (501) staff       (20)     6130 2023-03-15 07:07:22.000000 tumourkit-0.6.0/tumourkit/segmentation/hovernet/models/hovernet/opt.py
+-rwx------   0 joseperezcano   (501) staff       (20)     7784 2023-03-22 08:36:42.000000 tumourkit-0.6.0/tumourkit/segmentation/hovernet/models/hovernet/post_proc.py
+-rwx------   0 joseperezcano   (501) staff       (20)    13296 2023-03-13 19:48:31.000000 tumourkit-0.6.0/tumourkit/segmentation/hovernet/models/hovernet/run_desc.py
+-rwx------   0 joseperezcano   (501) staff       (20)     5117 2023-04-25 06:50:35.000000 tumourkit-0.6.0/tumourkit/segmentation/hovernet/models/hovernet/targets.py
+-rwx------   0 joseperezcano   (501) staff       (20)     4903 2023-01-10 16:18:24.000000 tumourkit-0.6.0/tumourkit/segmentation/hovernet/models/hovernet/utils.py
+-rwx------   0 joseperezcano   (501) staff       (20)     8325 2023-05-03 12:12:19.000000 tumourkit-0.6.0/tumourkit/segmentation/hovernet/run_infer.py
+drwxr-xr-x   0 joseperezcano   (501) staff       (20)        0 2023-05-04 18:22:57.146149 tumourkit-0.6.0/tumourkit/segmentation/hovernet/run_utils/
+-rwx------   0 joseperezcano   (501) staff       (20)        0 2022-09-15 10:27:54.000000 tumourkit-0.6.0/tumourkit/segmentation/hovernet/run_utils/__init__.py
+drwxr-xr-x   0 joseperezcano   (501) staff       (20)        0 2023-05-04 18:22:57.151752 tumourkit-0.6.0/tumourkit/segmentation/hovernet/run_utils/callbacks/
+-rwx------   0 joseperezcano   (501) staff       (20)        0 2022-09-15 10:27:54.000000 tumourkit-0.6.0/tumourkit/segmentation/hovernet/run_utils/callbacks/__init__.py
+-rwx------   0 joseperezcano   (501) staff       (20)     6991 2023-01-11 07:50:22.000000 tumourkit-0.6.0/tumourkit/segmentation/hovernet/run_utils/callbacks/base.py
+-rwx------   0 joseperezcano   (501) staff       (20)     6145 2022-09-15 10:27:54.000000 tumourkit-0.6.0/tumourkit/segmentation/hovernet/run_utils/callbacks/logging.py
+-rwx------   0 joseperezcano   (501) staff       (20)     5955 2023-01-13 16:18:56.000000 tumourkit-0.6.0/tumourkit/segmentation/hovernet/run_utils/callbacks/serialize.py
+-rwx------   0 joseperezcano   (501) staff       (20)     7482 2023-04-13 06:55:55.000000 tumourkit-0.6.0/tumourkit/segmentation/hovernet/run_utils/engine.py
+-rwx------   0 joseperezcano   (501) staff       (20)     6834 2023-01-10 14:22:13.000000 tumourkit-0.6.0/tumourkit/segmentation/hovernet/run_utils/utils.py
+-rwx------   0 joseperezcano   (501) staff       (20)    10663 2023-03-23 18:07:29.000000 tumourkit-0.6.0/tumourkit/segmentation/hovernet/train.py
+-rw-r--r--   0 joseperezcano   (501) staff       (20)     9861 2023-04-17 15:13:33.000000 tumourkit-0.6.0/tumourkit/train_pipe.py
+drwxr-xr-x   0 joseperezcano   (501) staff       (20)        0 2023-05-04 18:22:57.162298 tumourkit-0.6.0/tumourkit/utils/
+-rw-r--r--   0 joseperezcano   (501) staff       (20)        0 2022-09-26 11:04:45.000000 tumourkit-0.6.0/tumourkit/utils/__init__.py
+-rw-r--r--   0 joseperezcano   (501) staff       (20)     5932 2023-03-23 17:37:13.000000 tumourkit-0.6.0/tumourkit/utils/calibration_error.py
+-rw-r--r--   0 joseperezcano   (501) staff       (20)     5649 2023-05-01 12:06:57.000000 tumourkit-0.6.0/tumourkit/utils/classification.py
+-rw-r--r--   0 joseperezcano   (501) staff       (20)     3606 2023-03-23 18:25:35.000000 tumourkit-0.6.0/tumourkit/utils/folder2txt.py
+-rw-r--r--   0 joseperezcano   (501) staff       (20)     5254 2023-03-23 18:29:29.000000 tumourkit-0.6.0/tumourkit/utils/nearest.py
+-rw-r--r--   0 joseperezcano   (501) staff       (20)     3094 2023-04-22 10:28:27.000000 tumourkit-0.6.0/tumourkit/utils/pipes.py
+-rw-r--r--   0 joseperezcano   (501) staff       (20)     7022 2023-03-23 18:35:15.000000 tumourkit-0.6.0/tumourkit/utils/postprocessing.py
+-rw-r--r--   0 joseperezcano   (501) staff       (20)    21866 2023-04-30 10:04:39.000000 tumourkit-0.6.0/tumourkit/utils/preprocessing.py
+-rw-r--r--   0 joseperezcano   (501) staff       (20)     5714 2023-05-04 05:48:41.000000 tumourkit-0.6.0/tumourkit/utils/read_nodes.py
+drwxr-xr-x   0 joseperezcano   (501) staff       (20)        0 2023-05-04 18:22:57.086899 tumourkit-0.6.0/tumourkit.egg-info/
+-rw-r--r--   0 joseperezcano   (501) staff       (20)    42041 2023-05-04 18:22:57.000000 tumourkit-0.6.0/tumourkit.egg-info/PKG-INFO
+-rw-r--r--   0 joseperezcano   (501) staff       (20)     4909 2023-05-04 18:22:57.000000 tumourkit-0.6.0/tumourkit.egg-info/SOURCES.txt
+-rw-r--r--   0 joseperezcano   (501) staff       (20)        1 2023-05-04 18:22:57.000000 tumourkit-0.6.0/tumourkit.egg-info/dependency_links.txt
+-rw-r--r--   0 joseperezcano   (501) staff       (20)     1000 2023-05-04 18:22:57.000000 tumourkit-0.6.0/tumourkit.egg-info/entry_points.txt
+-rw-r--r--   0 joseperezcano   (501) staff       (20)      856 2023-05-04 18:22:57.000000 tumourkit-0.6.0/tumourkit.egg-info/requires.txt
+-rw-r--r--   0 joseperezcano   (501) staff       (20)       34 2023-05-04 18:22:57.000000 tumourkit-0.6.0/tumourkit.egg-info/top_level.txt
```

### Comparing `tumourkit-0.5.0/LICENSE` & `tumourkit-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `tumourkit-0.5.0/PKG-INFO` & `tumourkit-0.6.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tumourkit
-Version: 0.5.0
+Version: 0.6.0
 Summary: A SDK for tumour study
 Author-email: Jose Pérez Cano <joseperez2000@hotmail.es>
 License:                     GNU AFFERO GENERAL PUBLIC LICENSE
                                Version 3, 19 November 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `tumourkit-0.5.0/README.md` & `tumourkit-0.6.0/README.md`

 * *Files identical despite different names*

### Comparing `tumourkit-0.5.0/docs/buildenv/bin/rst2html.py` & `tumourkit-0.6.0/docs/buildenv/bin/rst2html.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.5.0/docs/buildenv/bin/rst2html4.py` & `tumourkit-0.6.0/docs/buildenv/bin/rst2html4.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.5.0/docs/buildenv/bin/rst2html5.py` & `tumourkit-0.6.0/docs/buildenv/bin/rst2html5.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.5.0/docs/buildenv/bin/rst2latex.py` & `tumourkit-0.6.0/docs/buildenv/bin/rst2latex.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.5.0/docs/buildenv/bin/rst2man.py` & `tumourkit-0.6.0/docs/buildenv/bin/rst2man.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.5.0/docs/buildenv/bin/rst2odt.py` & `tumourkit-0.6.0/docs/buildenv/bin/rst2odt.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.5.0/docs/buildenv/bin/rst2odt_prepstyles.py` & `tumourkit-0.6.0/docs/buildenv/bin/rst2odt_prepstyles.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.5.0/docs/buildenv/bin/rst2pseudoxml.py` & `tumourkit-0.6.0/docs/buildenv/bin/rst2pseudoxml.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.5.0/docs/buildenv/bin/rst2s5.py` & `tumourkit-0.6.0/docs/buildenv/bin/rst2s5.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.5.0/docs/buildenv/bin/rst2xetex.py` & `tumourkit-0.6.0/docs/buildenv/bin/rst2xetex.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.5.0/docs/buildenv/bin/rst2xml.py` & `tumourkit-0.6.0/docs/buildenv/bin/rst2xml.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.5.0/docs/buildenv/bin/rstpep2html.py` & `tumourkit-0.6.0/docs/buildenv/bin/rstpep2html.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.5.0/docs/source/conf.py` & `tumourkit-0.6.0/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.5.0/pyproject.toml` & `tumourkit-0.6.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -49,8 +49,10 @@
 centroidspng2csv = "tumourkit.preprocessing.centroidspng2csv:main"
 make_dirs = "tumourkit.make_dirs:main"
 run_training = "tumourkit.train_pipe:main"
 run_inference = "tumourkit.infer_pipe:main"
 run_research = "tumourkit.research_pipe:main"
 run_evaluation = "tumourkit.eval_pipe:main"
 merge_cells = "tumourkit.postprocessing.merge_cells:main"
-remove_uncertain = "tumourkit.preprocessing.remove_uncertain:main"
+remove_uncertain = "tumourkit.preprocessing.remove_uncertain:main"
+draw_cells = "tumourkit.postprocessing.draw_cells:main"
+start_app = "tumourkit.demo.app:main"
```

### Comparing `tumourkit-0.5.0/requirements.txt` & `tumourkit-0.6.0/requirements.txt`

 * *Files 12% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 attrs==22.2.0
+beautifulsoup4==4.12.2
 certifi==2022.12.7
 charset-normalizer==3.0.1
 contourpy==1.0.7
 cycler==0.11.0
 docopt==0.6.2
 exceptiongroup==1.1.0
 flake8==6.0.0
 fonttools==4.38.0
 geojson==2.5.0
+gradio==3.26.0
 idna==3.4
 imageio==2.24.0
 iniconfig==2.0.0
 joblib==1.2.0
 kiwisolver==1.4.4
 matplotlib==3.6.3
 mccabe==0.7.0
```

### Comparing `tumourkit-0.5.0/tests/centroidspng2csv_test.py` & `tumourkit-0.6.0/tests/centroidspng2csv_test.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.5.0/tests/conf_matrix_sum_test.py` & `tumourkit-0.6.0/tests/conf_matrix_sum_test.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.5.0/tests/cpairs_test.py` & `tumourkit-0.6.0/tests/cpairs_test.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.5.0/tests/example_test.py` & `tumourkit-0.6.0/tests/example_test.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.5.0/tests/generate_centroids.py` & `tumourkit-0.6.0/tests/generate_centroids.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.5.0/tests/generate_rswoosh.py` & `tumourkit-0.6.0/tests/generate_rswoosh.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.5.0/tests/get_conn_comp_test.py` & `tumourkit-0.6.0/tests/get_conn_comp_test.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.5.0/tests/graph2centroids_test.py` & `tumourkit-0.6.0/tests/graph2centroids_test.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.5.0/tests/graph_idx_test.py` & `tumourkit-0.6.0/tests/graph_idx_test.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.5.0/tests/hov_prob_pipe_test.py` & `tumourkit-0.6.0/tests/hov_prob_pipe_test.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.5.0/tests/hov_prob_test.py` & `tumourkit-0.6.0/tests/hov_prob_test.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.5.0/tests/hovernet_patches_test.py` & `tumourkit-0.6.0/tests/hovernet_patches_test.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.5.0/tests/metrics_pairs_test.py` & `tumourkit-0.6.0/tests/metrics_pairs_test.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.5.0/tests/metrics_test.py` & `tumourkit-0.6.0/tests/metrics_test.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.5.0/tests/png2graph_test.py` & `tumourkit-0.6.0/tests/png2graph_test.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.5.0/tests/pngcsv2geojson_test.py` & `tumourkit-0.6.0/tests/pngcsv2geojson_test.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.5.0/tests/pngcsv2graph_test.py` & `tumourkit-0.6.0/tests/pngcsv2graph_test.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.5.0/tests/read_nodes_test.py` & `tumourkit-0.6.0/tests/read_nodes_test.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.5.0/tests/remove_idx_test.py` & `tumourkit-0.6.0/tests/remove_idx_test.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.5.0/tests/rswoosh_test.py` & `tumourkit-0.6.0/tests/rswoosh_test.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.5.0/tumourkit/classification/compute_imbalance.py` & `tumourkit-0.6.0/tumourkit/classification/compute_imbalance.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.5.0/tumourkit/classification/evaluate.py` & `tumourkit-0.6.0/tumourkit/classification/evaluate.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.5.0/tumourkit/classification/infer.py` & `tumourkit-0.6.0/tumourkit/classification/infer.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.5.0/tumourkit/classification/models/gat.py` & `tumourkit-0.6.0/tumourkit/classification/models/gat.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.5.0/tumourkit/classification/models/gcn.py` & `tumourkit-0.6.0/tumourkit/classification/models/gcn.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.5.0/tumourkit/classification/models/hgao.py` & `tumourkit-0.6.0/tumourkit/classification/models/hgao.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.5.0/tumourkit/classification/models/norm.py` & `tumourkit-0.6.0/tumourkit/classification/models/norm.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.5.0/tumourkit/classification/read_graph.py` & `tumourkit-0.6.0/tumourkit/classification/read_graph.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.5.0/tumourkit/classification/train_graphs.py` & `tumourkit-0.6.0/tumourkit/classification/train_graphs.py`

 * *Files 0% similar despite different names*

```diff
@@ -83,15 +83,15 @@
         acc, f1, auc, perc_err, ece = metrics_from_predictions(labels, preds, probs, 2)
         # Tensorboard
         if writer is not None:
             assert(log_suffix is not None and epoch is not None)
             writer.add_scalar('Accuracy/' + log_suffix, acc, epoch)
             writer.add_scalar('F1/' + log_suffix, f1, epoch)
             writer.add_scalar('ROC_AUC/' + log_suffix, auc, epoch)
-            writer.add_scalar('Percentage error/' + log_suffix, perc_err, epoch)
+            writer.add_scalar('Percentage Error/' + log_suffix, perc_err, epoch)
             writer.add_scalar('ECE/' + log_suffix, ece, epoch)
         return f1, acc, auc, perc_err, ece
     else:
         micro, macro, weighted, ece = metrics_from_predictions(labels, preds, probs, num_classes)
         # Tensorboard
         if writer is not None:
             writer.add_scalar('Accuracy/' + log_suffix, micro, epoch)
```

### Comparing `tumourkit-0.5.0/tumourkit/classification/train_xgboost.py` & `tumourkit-0.6.0/tumourkit/classification/train_xgboost.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.5.0/tumourkit/eval_pipe.py` & `tumourkit-0.6.0/tumourkit/eval_pipe.py`

 * *Files 1% similar despite different names*

```diff
@@ -58,25 +58,25 @@
         df = pd.read_csv(os.path.join(folder, file))
         _trues = df['class'].to_numpy()-1
         if trues is None:
             trues = _trues.reshape((-1,1))
         else:
             trues = np.vstack((trues, _trues.reshape((-1, 1))))
         if args.num_classes == 2:
-            _probs = df['prob1'].to_numpy()
+            _probs = df['prob1'].to_numpy().reshape((-1, 1))
             _probs = np.hstack((1 - _probs, _probs))
         else:
             cols = ['prob' + str(k) for k in range(1, args.num_classes + 1)]
             _probs = df[cols].to_numpy()
         if probs is None:
             probs = _probs
         else:
             probs = np.vstack((probs, _probs))
     preds = np.argmax(probs, axis=1).reshape((-1, 1))
-    metrics = metrics_from_predictions(trues, preds, probs, args.num_classes)
+    metrics = metrics_from_predictions(trues, preds, probs[:, 1], args.num_classes)
     if args.num_classes == 2:
         acc, f1, auc, perc_error, ece = metrics
         dic_metrics = {
             'F1': [f1], 'Accuracy': [acc], 'ROC_AUC': [auc], 'Perc_err': [perc_error], 'ECE': [ece]
         }
     else:
         micro, macro, weighted, ece = metrics
```

### Comparing `tumourkit-0.5.0/tumourkit/infer_pipe.py` & `tumourkit-0.6.0/tumourkit/infer_pipe.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.5.0/tumourkit/make_dirs.py` & `tumourkit-0.6.0/tumourkit/make_dirs.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.5.0/tumourkit/postprocessing/join_graph_gt.py` & `tumourkit-0.6.0/tumourkit/postprocessing/join_graph_gt.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.5.0/tumourkit/postprocessing/join_hovprob_graph.py` & `tumourkit-0.6.0/tumourkit/postprocessing/join_hovprob_graph.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.5.0/tumourkit/postprocessing/merge_cells.py` & `tumourkit-0.6.0/tumourkit/postprocessing/merge_cells.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.5.0/tumourkit/postprocessing/rswoosh.py` & `tumourkit-0.6.0/tumourkit/postprocessing/rswoosh.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.5.0/tumourkit/preprocessing/__init__.py` & `tumourkit-0.6.0/tumourkit/preprocessing/__init__.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.5.0/tumourkit/preprocessing/centroids2png.py` & `tumourkit-0.6.0/tumourkit/preprocessing/centroids2png.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.5.0/tumourkit/preprocessing/centroidspng2csv.py` & `tumourkit-0.6.0/tumourkit/preprocessing/centroidspng2csv.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.5.0/tumourkit/preprocessing/geojson2pngcsv.py` & `tumourkit-0.6.0/tumourkit/preprocessing/geojson2pngcsv.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.5.0/tumourkit/preprocessing/graph2centroids.py` & `tumourkit-0.6.0/tumourkit/preprocessing/graph2centroids.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.5.0/tumourkit/preprocessing/hovernet2centroids.py` & `tumourkit-0.6.0/tumourkit/preprocessing/hovernet2centroids.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.5.0/tumourkit/preprocessing/hovernet2geojson.py` & `tumourkit-0.6.0/tumourkit/preprocessing/hovernet2geojson.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.5.0/tumourkit/preprocessing/png2graph.py` & `tumourkit-0.6.0/tumourkit/preprocessing/png2graph.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.5.0/tumourkit/preprocessing/pngcsv2centroids.py` & `tumourkit-0.6.0/tumourkit/preprocessing/pngcsv2centroids.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.5.0/tumourkit/preprocessing/pngcsv2geojson.py` & `tumourkit-0.6.0/tumourkit/preprocessing/pngcsv2geojson.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.5.0/tumourkit/preprocessing/pngcsv2graph.py` & `tumourkit-0.6.0/tumourkit/preprocessing/pngcsv2graph.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.5.0/tumourkit/preprocessing/remove_uncertain.py` & `tumourkit-0.6.0/tumourkit/preprocessing/remove_uncertain.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.5.0/tumourkit/profiling/cpairs_profile.py` & `tumourkit-0.6.0/tumourkit/profiling/cpairs_profile.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.5.0/tumourkit/profiling/rswoosh_profile.py` & `tumourkit-0.6.0/tumourkit/profiling/rswoosh_profile.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.5.0/tumourkit/research_pipe.py` & `tumourkit-0.6.0/tumourkit/research_pipe.py`

 * *Files 0% similar despite different names*

```diff
@@ -261,15 +261,15 @@
         num_confs = 32,
         save_dir = os.path.join(args.root_dir, 'weights', 'classification', 'gnn_void'),
         device = 'cpu' if args.gpu == '' else 'cuda',
         num_workers = args.num_workers,
         checkpoint_iters = -1,
         num_classes = args.num_classes,
         disable_prior = True,
-        disable_morph_feats = False,
+        disable_morph_feats = True,
     )
     train_gnn(newargs)
 
 
 def run_cnn(args: Namespace, logger: Logger) -> None:
     raise NotImplementedError
```

### Comparing `tumourkit-0.5.0/tumourkit/segmentation/evaluate.py` & `tumourkit-0.6.0/tumourkit/segmentation/evaluate.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.5.0/tumourkit/segmentation/hovernet/config.py` & `tumourkit-0.6.0/tumourkit/segmentation/hovernet/config.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.5.0/tumourkit/segmentation/hovernet/dataloader/augs.py` & `tumourkit-0.6.0/tumourkit/segmentation/hovernet/dataloader/augs.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.5.0/tumourkit/segmentation/hovernet/dataloader/infer_loader.py` & `tumourkit-0.6.0/tumourkit/segmentation/hovernet/dataloader/infer_loader.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.5.0/tumourkit/segmentation/hovernet/dataloader/train_loader.py` & `tumourkit-0.6.0/tumourkit/segmentation/hovernet/dataloader/train_loader.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.5.0/tumourkit/segmentation/hovernet/extract_patches.py` & `tumourkit-0.6.0/tumourkit/segmentation/hovernet/extract_patches.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.5.0/tumourkit/segmentation/hovernet/infer/base.py` & `tumourkit-0.6.0/tumourkit/segmentation/hovernet/infer/base.py`

 * *Files 4% similar despite different names*

```diff
@@ -46,24 +46,28 @@
         associated run steps to process each data batch.
         
         """
         model_desc = import_module(".segmentation.hovernet.models.hovernet.net_desc", package="tumourkit")
         model_creator = getattr(model_desc, "create_model")
 
         net = model_creator(**self.method["model_args"])
-        saved_state_dict = torch.load(self.method["model_path"])["desc"]
+        if self.nr_gpus > 0:
+            saved_state_dict = torch.load(self.method["model_path"])["desc"]
+        else:
+            saved_state_dict = torch.load(self.method["model_path"], map_location=torch.device('cpu'))["desc"]
         saved_state_dict = convert_pytorch_checkpoint(saved_state_dict)
 
         net.load_state_dict(saved_state_dict, strict=True)
         net = torch.nn.DataParallel(net)
-        net = net.to("cuda")
+        if self.nr_gpus > 0:
+            net = net.to("cuda")
 
         module_lib = import_module(".segmentation.hovernet.models.hovernet.run_desc", package="tumourkit")
         run_step = getattr(module_lib, "infer_step")
-        self.run_step = lambda input_batch: run_step(input_batch, net)
+        self.run_step = lambda input_batch: run_step(input_batch, net, use_cpu=self.nr_gpus==0)
 
         module_lib = import_module(".segmentation.hovernet.models.hovernet.post_proc", package="tumourkit")
         self.post_proc_func = getattr(module_lib, "process")
         return
 
     def __save_json(self, path, old_dict, mag=None):
         new_dict = {}
```

### Comparing `tumourkit-0.5.0/tumourkit/segmentation/hovernet/infer/tile.py` & `tumourkit-0.6.0/tumourkit/segmentation/hovernet/infer/tile.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.5.0/tumourkit/segmentation/hovernet/infer/wsi.py` & `tumourkit-0.6.0/tumourkit/segmentation/hovernet/infer/wsi.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.5.0/tumourkit/segmentation/hovernet/metrics/stats_utils.py` & `tumourkit-0.6.0/tumourkit/segmentation/hovernet/metrics/stats_utils.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.5.0/tumourkit/segmentation/hovernet/misc/patch_extractor.py` & `tumourkit-0.6.0/tumourkit/segmentation/hovernet/misc/patch_extractor.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.5.0/tumourkit/segmentation/hovernet/misc/utils.py` & `tumourkit-0.6.0/tumourkit/segmentation/hovernet/misc/utils.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.5.0/tumourkit/segmentation/hovernet/misc/viz_utils.py` & `tumourkit-0.6.0/tumourkit/segmentation/hovernet/misc/viz_utils.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.5.0/tumourkit/segmentation/hovernet/misc/wsi_handler.py` & `tumourkit-0.6.0/tumourkit/segmentation/hovernet/misc/wsi_handler.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.5.0/tumourkit/segmentation/hovernet/models/hovernet/net_desc.py` & `tumourkit-0.6.0/tumourkit/segmentation/hovernet/models/hovernet/net_desc.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.5.0/tumourkit/segmentation/hovernet/models/hovernet/net_utils.py` & `tumourkit-0.6.0/tumourkit/segmentation/hovernet/models/hovernet/net_utils.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.5.0/tumourkit/segmentation/hovernet/models/hovernet/opt.py` & `tumourkit-0.6.0/tumourkit/segmentation/hovernet/models/hovernet/opt.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.5.0/tumourkit/segmentation/hovernet/models/hovernet/post_proc.py` & `tumourkit-0.6.0/tumourkit/segmentation/hovernet/models/hovernet/post_proc.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.5.0/tumourkit/segmentation/hovernet/models/hovernet/run_desc.py` & `tumourkit-0.6.0/tumourkit/segmentation/hovernet/models/hovernet/run_desc.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.5.0/tumourkit/segmentation/hovernet/models/hovernet/targets.py` & `tumourkit-0.6.0/tumourkit/segmentation/hovernet/models/hovernet/targets.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.5.0/tumourkit/segmentation/hovernet/models/hovernet/utils.py` & `tumourkit-0.6.0/tumourkit/segmentation/hovernet/models/hovernet/utils.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.5.0/tumourkit/segmentation/hovernet/run_infer.py` & `tumourkit-0.6.0/tumourkit/segmentation/hovernet/run_infer.py`

 * *Files 1% similar despite different names*

```diff
@@ -100,36 +100,37 @@
 #-------------------------------------------------------------------------------------------------------
 
 def main_with_args(args: Dict, sub_args: Dict, sub_cmd: str) -> None:
     gpu_list = args['gpu']
     os.environ['CUDA_VISIBLE_DEVICES'] = gpu_list
 
     nr_gpus = torch.cuda.device_count()
-    log_info('Detect #GPUS: %d' % nr_gpus)
+    log_info('Detect #GPUS: %d' % nr_gpus)        
 
     if args['model_path'] == None:
         raise Exception('A model path must be supplied as an argument with --model_path.')
 
     nr_types = int(args['nr_types']) if int(args['nr_types']) > 0 else None
     method_args = {
+        'nr_gpus' : nr_gpus,
         'method' : {
             'model_args' : {
                 'nr_types'   : nr_types,
                 'mode'       : args['model_mode'],
             },
             'model_path' : args['model_path'],
         },
         'type_info_path'  : None if args['type_info_path'] == '' \
                             else args['type_info_path'],
     }
 
     # ***
     run_args = {
-        'batch_size' : int(args['batch_size']) * nr_gpus,
-
+        'batch_size' : int(args['batch_size']) * max(1, nr_gpus),
+        
         'nr_inference_workers' : int(args['nr_inference_workers']),
         'nr_post_proc_workers' : int(args['nr_post_proc_workers']),
     }
 
     if args['model_mode'] == 'fast':
         run_args['patch_input_shape'] = 256
         run_args['patch_output_shape'] = 164
```

### Comparing `tumourkit-0.5.0/tumourkit/segmentation/hovernet/run_utils/callbacks/base.py` & `tumourkit-0.6.0/tumourkit/segmentation/hovernet/run_utils/callbacks/base.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.5.0/tumourkit/segmentation/hovernet/run_utils/callbacks/logging.py` & `tumourkit-0.6.0/tumourkit/segmentation/hovernet/run_utils/callbacks/logging.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.5.0/tumourkit/segmentation/hovernet/run_utils/callbacks/serialize.py` & `tumourkit-0.6.0/tumourkit/segmentation/hovernet/run_utils/callbacks/serialize.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.5.0/tumourkit/segmentation/hovernet/run_utils/engine.py` & `tumourkit-0.6.0/tumourkit/segmentation/hovernet/run_utils/engine.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.5.0/tumourkit/segmentation/hovernet/run_utils/utils.py` & `tumourkit-0.6.0/tumourkit/segmentation/hovernet/run_utils/utils.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.5.0/tumourkit/segmentation/hovernet/train.py` & `tumourkit-0.6.0/tumourkit/segmentation/hovernet/train.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.5.0/tumourkit/train_pipe.py` & `tumourkit-0.6.0/tumourkit/train_pipe.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.5.0/tumourkit/utils/calibration_error.py` & `tumourkit-0.6.0/tumourkit/utils/calibration_error.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.5.0/tumourkit/utils/classification.py` & `tumourkit-0.6.0/tumourkit/utils/classification.py`

 * *Files 2% similar despite different names*

```diff
@@ -98,15 +98,15 @@
     For binary: Accuracy, F1 Score, ROC AUC, %ERR, ECE
     For multiclass: Micro F1, Macro F1, Weighted F1, ECE
 
     :param y_true: The ground truth to compare with, values start at 0. Shape: (N, 1).
     :type y_true: np.ndarray
     :param y_pred: Predictions with values starting at 0. Shape: (N, 1).
     :type y_pred: np.ndarray
-    :param y_prob: Probabilities of the predictions. Shape: (N, num_classes)
+    :param y_prob: Probabilities of the predictions. Shape: (N, num_classes) or (N, 1) if binary.
     :type y_prob: Optional[np.ndarray]
     :param num_classes: Number of classes to consider.
     :type num_classes: Optional[int]
     :return: Several metrics. Either 4 or 5 floats, depending on whether is binary or multiclass.
     :rtype: List[float]
     """
     if num_classes == 2:
```

### Comparing `tumourkit-0.5.0/tumourkit/utils/folder2txt.py` & `tumourkit-0.6.0/tumourkit/utils/folder2txt.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.5.0/tumourkit/utils/nearest.py` & `tumourkit-0.6.0/tumourkit/utils/nearest.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.5.0/tumourkit/utils/pipes.py` & `tumourkit-0.6.0/tumourkit/utils/pipes.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.5.0/tumourkit/utils/postprocessing.py` & `tumourkit-0.6.0/tumourkit/utils/postprocessing.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.5.0/tumourkit/utils/preprocessing.py` & `tumourkit-0.6.0/tumourkit/utils/preprocessing.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.5.0/tumourkit/utils/read_nodes.py` & `tumourkit-0.6.0/tumourkit/utils/read_nodes.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 """
 from typing import List, Optional, Tuple
 import numpy as np
 import pandas as pd
 from sklearn.model_selection import train_test_split
 import random
 import os
-from .preprocessing import *
+from .preprocessing import get_names
 
 
 def read_node_matrix(
         file: str,
         return_coordinates: Optional[bool] = False,
         return_class: Optional[bool] = True,
         remove_prior: Optional[bool] = False,
@@ -56,17 +56,18 @@
         if not return_coordinates:
             return X, y
         else:
             xx = df['X'].to_numpy()
             yy = df['Y'].to_numpy()
             return X, y, xx, yy
     else:
+        remove_vars.remove('class')
         X = df.drop(remove_vars, axis=1).to_numpy()
         if remove_morph and remove_prior:
-            X = np.zeros((len(y), 1))
+            X = np.zeros((len(X), 1))
         if not return_coordinates:
             return X, None
         else:
             xx = df['X'].to_numpy()
             yy = df['Y'].to_numpy()
             return X, None, xx, yy
```

### Comparing `tumourkit-0.5.0/tumourkit.egg-info/PKG-INFO` & `tumourkit-0.6.0/tumourkit.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tumourkit
-Version: 0.5.0
+Version: 0.6.0
 Summary: A SDK for tumour study
 Author-email: Jose Pérez Cano <joseperez2000@hotmail.es>
 License:                     GNU AFFERO GENERAL PUBLIC LICENSE
                                Version 3, 19 November 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `tumourkit-0.5.0/tumourkit.egg-info/SOURCES.txt` & `tumourkit-0.6.0/tumourkit.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 LICENSE
 README.md
 pyproject.toml
 requirements.txt
-demo/app.py
 docs/buildenv/bin/rst2html.py
 docs/buildenv/bin/rst2html4.py
 docs/buildenv/bin/rst2html5.py
 docs/buildenv/bin/rst2latex.py
 docs/buildenv/bin/rst2man.py
 docs/buildenv/bin/rst2odt.py
 docs/buildenv/bin/rst2odt_prepstyles.py
@@ -56,15 +55,17 @@
 tumourkit/classification/train_graphs.py
 tumourkit/classification/train_xgboost.py
 tumourkit/classification/models/__init__.py
 tumourkit/classification/models/gat.py
 tumourkit/classification/models/gcn.py
 tumourkit/classification/models/hgao.py
 tumourkit/classification/models/norm.py
+tumourkit/demo/app.py
 tumourkit/postprocessing/__init__.py
+tumourkit/postprocessing/draw_cells.py
 tumourkit/postprocessing/join_graph_gt.py
 tumourkit/postprocessing/join_hovprob_graph.py
 tumourkit/postprocessing/merge_cells.py
 tumourkit/postprocessing/rswoosh.py
 tumourkit/preprocessing/__init__.py
 tumourkit/preprocessing/centroids2png.py
 tumourkit/preprocessing/centroidspng2csv.py
```

### Comparing `tumourkit-0.5.0/tumourkit.egg-info/entry_points.txt` & `tumourkit-0.6.0/tumourkit.egg-info/entry_points.txt`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 [console_scripts]
 centroids2png = tumourkit.preprocessing.centroids2png:main
 centroidspng2csv = tumourkit.preprocessing.centroidspng2csv:main
+draw_cells = tumourkit.postprocessing.draw_cells:main
 geojson2pngcsv = tumourkit.preprocessing.geojson2pngcsv:main
 graph2centroids = tumourkit.preprocessing.graph2centroids:main
 hovernet2centroids = tumourkit.preprocessing.hovernet2centroids:main
 hovernet2geojson = tumourkit.preprocessing.hovernet2geojson:main
 make_dirs = tumourkit.make_dirs:main
 merge_cells = tumourkit.postprocessing.merge_cells:main
 pngcsv2centroids = tumourkit.preprocessing.pngcsv2centroids:main
 pngcsv2geojson = tumourkit.preprocessing.pngcsv2geojson:main
 pngcsv2graph = tumourkit.preprocessing.pngcsv2graph:main
 remove_uncertain = tumourkit.preprocessing.remove_uncertain:main
 run_evaluation = tumourkit.eval_pipe:main
 run_inference = tumourkit.infer_pipe:main
 run_research = tumourkit.research_pipe:main
 run_training = tumourkit.train_pipe:main
+start_app = tumourkit.demo.app:main
```

### Comparing `tumourkit-0.5.0/tumourkit.egg-info/requires.txt` & `tumourkit-0.6.0/tumourkit.egg-info/requires.txt`

 * *Files 12% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 attrs==22.2.0
+beautifulsoup4==4.12.2
 certifi==2022.12.7
 charset-normalizer==3.0.1
 contourpy==1.0.7
 cycler==0.11.0
 docopt==0.6.2
 exceptiongroup==1.1.0
 flake8==6.0.0
 fonttools==4.38.0
 geojson==2.5.0
+gradio==3.26.0
 idna==3.4
 imageio==2.24.0
 iniconfig==2.0.0
 joblib==1.2.0
 kiwisolver==1.4.4
 matplotlib==3.6.3
 mccabe==0.7.0
```

