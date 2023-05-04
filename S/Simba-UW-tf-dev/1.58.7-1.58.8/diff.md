# Comparing `tmp/Simba-UW-tf-dev-1.58.7.tar.gz` & `tmp/Simba-UW-tf-dev-1.58.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/Simba-UW-tf-dev-1.58.7.tar", last modified: Wed May  3 21:14:48 2023, max compression
+gzip compressed data, was "dist/Simba-UW-tf-dev-1.58.8.tar", last modified: Thu May  4 20:00:38 2023, max compression
```

## Comparing `Simba-UW-tf-dev-1.58.7.tar` & `Simba-UW-tf-dev-1.58.8.tar`

### file list

```diff
@@ -1,482 +1,482 @@
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-03 21:14:48.000000 Simba-UW-tf-dev-1.58.7/
--rw-r--r--   0 simon      (501) staff       (20)      579 2023-05-03 21:14:48.000000 Simba-UW-tf-dev-1.58.7/PKG-INFO
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-03 21:14:48.000000 Simba-UW-tf-dev-1.58.7/simba/
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-03 21:14:48.000000 Simba-UW-tf-dev-1.58.7/simba/ui/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-05-03 18:36:16.000000 Simba-UW-tf-dev-1.58.7/simba/ui/.DS_Store
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-03 21:14:48.000000 Simba-UW-tf-dev-1.58.7/simba/ui/pop_ups/
--rw-r--r--   0 simon      (501) staff       (20)     3477 2023-05-03 16:54:51.000000 Simba-UW-tf-dev-1.58.7/simba/ui/pop_ups/movement_analysis_time_bins_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     1431 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.58.7/simba/ui/pop_ups/csv_2_parquet_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     2310 2023-04-29 15:00:50.000000 Simba-UW-tf-dev-1.58.7/simba/ui/pop_ups/quick_path_plot_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     2332 2023-04-29 18:13:54.000000 Simba-UW-tf-dev-1.58.7/simba/ui/pop_ups/batch_preprocess_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     8366 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.58.7/simba/ui/pop_ups/heatmap_location_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     9311 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.58.7/simba/ui/pop_ups/clf_probability_plot_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-04-29 16:41:16.000000 Simba-UW-tf-dev-1.58.7/simba/ui/pop_ups/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)     3143 2023-05-03 16:24:11.000000 Simba-UW-tf-dev-1.58.7/simba/ui/pop_ups/movement_analysis_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     3657 2023-04-29 19:37:54.000000 Simba-UW-tf-dev-1.58.7/simba/ui/pop_ups/set_machine_model_parameters_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     9494 2023-04-29 15:00:50.000000 Simba-UW-tf-dev-1.58.7/simba/ui/pop_ups/clf_plot_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)    15044 2023-05-03 21:12:42.000000 Simba-UW-tf-dev-1.58.7/simba/ui/pop_ups/path_plot_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     3024 2023-04-29 16:24:52.000000 Simba-UW-tf-dev-1.58.7/simba/ui/pop_ups/smoothing_interpolation_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     4798 2023-04-29 18:54:24.000000 Simba-UW-tf-dev-1.58.7/simba/ui/pop_ups/visualize_pose_in_dir_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     3551 2023-05-03 16:20:49.000000 Simba-UW-tf-dev-1.58.7/simba/ui/pop_ups/roi_analysis_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     5873 2023-04-29 16:24:52.000000 Simba-UW-tf-dev-1.58.7/simba/ui/pop_ups/outlier_settings_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     8296 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.58.7/simba/ui/pop_ups/gantt_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     5726 2023-05-01 12:04:35.000000 Simba-UW-tf-dev-1.58.7/simba/ui/pop_ups/clf_validation_plot_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     3301 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.58.7/simba/ui/pop_ups/severity_analysis_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     2779 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.58.7/simba/ui/pop_ups/fsttc_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     4066 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.58.7/simba/ui/pop_ups/kleinberg_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     7288 2023-04-29 15:00:50.000000 Simba-UW-tf-dev-1.58.7/simba/ui/pop_ups/directing_other_animals_plot_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     5463 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.58.7/simba/ui/pop_ups/pose_reorganizer_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     2411 2023-05-03 16:35:10.000000 Simba-UW-tf-dev-1.58.7/simba/ui/pop_ups/append_roi_features_animals_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     3251 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.58.7/simba/ui/pop_ups/clf_by_timebins_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     8697 2023-04-29 15:00:50.000000 Simba-UW-tf-dev-1.58.7/simba/ui/pop_ups/heatmap_clf_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     7688 2023-04-29 15:00:50.000000 Simba-UW-tf-dev-1.58.7/simba/ui/pop_ups/data_plot_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     7928 2023-04-29 15:00:50.000000 Simba-UW-tf-dev-1.58.7/simba/ui/pop_ups/roi_features_plot_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     8363 2023-04-29 19:49:16.000000 Simba-UW-tf-dev-1.58.7/simba/ui/pop_ups/pup_retrieval_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)      579 2023-04-29 18:12:37.000000 Simba-UW-tf-dev-1.58.7/simba/ui/pop_ups/about_simba_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     2544 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.58.7/simba/ui/pop_ups/clf_descriptive_statistics_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     6409 2023-04-29 15:00:50.000000 Simba-UW-tf-dev-1.58.7/simba/ui/pop_ups/roi_tracking_plot_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     1468 2023-04-29 16:24:52.000000 Simba-UW-tf-dev-1.58.7/simba/ui/pop_ups/append_roi_features_bodypart_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     5318 2023-04-29 19:01:32.000000 Simba-UW-tf-dev-1.58.7/simba/ui/pop_ups/clf_add_remove_print_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)    42478 2023-04-29 18:56:08.000000 Simba-UW-tf-dev-1.58.7/simba/ui/pop_ups/video_processing_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     7536 2023-04-29 15:00:50.000000 Simba-UW-tf-dev-1.58.7/simba/ui/pop_ups/validation_plot_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     5064 2023-04-29 19:45:45.000000 Simba-UW-tf-dev-1.58.7/simba/ui/pop_ups/clf_by_roi_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     2840 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.58.7/simba/ui/pop_ups/make_path_plot_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     5406 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.58.7/simba/ui/pop_ups/create_user_defined_pose_configuration_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     1065 2023-04-29 16:24:52.000000 Simba-UW-tf-dev-1.58.7/simba/ui/pop_ups/archive_files_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     4098 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.58.7/simba/ui/pop_ups/pose_bp_drop_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)    10712 2023-04-29 15:00:50.000000 Simba-UW-tf-dev-1.58.7/simba/ui/pop_ups/distance_plot_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     2567 2023-04-29 16:24:52.000000 Simba-UW-tf-dev-1.58.7/simba/ui/pop_ups/subset_feature_extractor_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     3114 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.58.7/simba/ui/pop_ups/third_party_annotator_appender_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     2797 2023-05-03 19:08:52.000000 Simba-UW-tf-dev-1.58.7/simba/ui/pop_ups/roi_analysis_time_bins_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)    12632 2023-05-03 20:43:49.000000 Simba-UW-tf-dev-1.58.7/simba/ui/video_info_ui.py
--rw-r--r--   0 simon      (501) staff       (20)     5996 2023-04-28 23:45:44.000000 Simba-UW-tf-dev-1.58.7/simba/ui/user_defined_pose_creator.py
--rw-r--r--   0 simon      (501) staff       (20)    12788 2023-05-01 23:51:03.000000 Simba-UW-tf-dev-1.58.7/simba/ui/create_project_ui.py
--rw-r--r--   0 simon      (501) staff       (20)    10867 2023-04-28 19:59:05.000000 Simba-UW-tf-dev-1.58.7/simba/ui/tkinter_functions.py
--rw-r--r--   0 simon      (501) staff       (20)    33818 2023-04-29 19:43:53.000000 Simba-UW-tf-dev-1.58.7/simba/ui/machine_model_settings_ui.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-03 21:14:48.000000 Simba-UW-tf-dev-1.58.7/simba/blob_storage/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-21 20:39:46.000000 Simba-UW-tf-dev-1.58.7/simba/blob_storage/.DS_Store
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-03 21:14:48.000000 Simba-UW-tf-dev-1.58.7/simba/labelling/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-04-28 20:24:21.000000 Simba-UW-tf-dev-1.58.7/simba/labelling/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)    20637 2023-05-02 00:47:44.000000 Simba-UW-tf-dev-1.58.7/simba/labelling/labelling_interface.py
--rw-r--r--   0 simon      (501) staff       (20)     3419 2023-04-28 19:59:05.000000 Simba-UW-tf-dev-1.58.7/simba/labelling/extract_labelled_frames.py
--rw-r--r--   0 simon      (501) staff       (20)    26652 2023-04-29 19:43:53.000000 Simba-UW-tf-dev-1.58.7/simba/labelling/labelling_advanced_interface.py
--rw-r--r--   0 simon      (501) staff       (20)     6543 2023-04-27 19:42:17.000000 Simba-UW-tf-dev-1.58.7/simba/labelling/play_annotation_video.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-03 21:14:48.000000 Simba-UW-tf-dev-1.58.7/simba/unsupervised/
--rw-r--r--   0 simon      (501) staff       (20)    11932 2023-04-27 20:23:35.000000 Simba-UW-tf-dev-1.58.7/simba/unsupervised/dbcv_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)     3375 2023-05-02 18:14:28.000000 Simba-UW-tf-dev-1.58.7/simba/unsupervised/enums.py
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-04-23 19:55:32.000000 Simba-UW-tf-dev-1.58.7/simba/unsupervised/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)     8187 2023-04-28 13:09:30.000000 Simba-UW-tf-dev-1.58.7/simba/unsupervised/dataset_creator.py
--rw-r--r--   0 simon      (501) staff       (20)     5693 2023-04-28 13:09:30.000000 Simba-UW-tf-dev-1.58.7/simba/unsupervised/grid_search_visualizers.py
--rw-r--r--   0 simon      (501) staff       (20)     7268 2023-04-28 12:30:12.000000 Simba-UW-tf-dev-1.58.7/simba/unsupervised/data_extractor.py
--rw-r--r--   0 simon      (501) staff       (20)     9910 2023-05-02 18:14:28.000000 Simba-UW-tf-dev-1.58.7/simba/unsupervised/ui.py
--rw-r--r--   0 simon      (501) staff       (20)     9915 2023-04-28 13:09:30.000000 Simba-UW-tf-dev-1.58.7/simba/unsupervised/umap_embedder.py
--rw-r--r--   0 simon      (501) staff       (20)    41323 2023-05-02 18:14:28.000000 Simba-UW-tf-dev-1.58.7/simba/unsupervised/pop_up_classes.py
--rw-r--r--   0 simon      (501) staff       (20)     2347 2023-04-28 12:22:34.000000 Simba-UW-tf-dev-1.58.7/simba/unsupervised/bout_aggregator.py
--rw-r--r--   0 simon      (501) staff       (20)    20886 2023-04-28 19:59:05.000000 Simba-UW-tf-dev-1.58.7/simba/unsupervised/cluster_statistics.py
--rw-r--r--   0 simon      (501) staff       (20)     2188 2023-04-18 23:25:29.000000 Simba-UW-tf-dev-1.58.7/simba/unsupervised/data_map.yaml
--rw-r--r--   0 simon      (501) staff       (20)    10289 2023-04-28 13:09:30.000000 Simba-UW-tf-dev-1.58.7/simba/unsupervised/hdbscan_clusterer.py
--rw-r--r--   0 simon      (501) staff       (20)     3937 2023-04-28 19:59:05.000000 Simba-UW-tf-dev-1.58.7/simba/unsupervised/tsne.py
--rw-r--r--   0 simon      (501) staff       (20)     6698 2023-04-28 19:59:05.000000 Simba-UW-tf-dev-1.58.7/simba/unsupervised/cluster_visualizer.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-03 21:14:48.000000 Simba-UW-tf-dev-1.58.7/simba/bounding_box_tools/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.7/simba/bounding_box_tools/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)     6790 2023-04-28 00:15:19.000000 Simba-UW-tf-dev-1.58.7/simba/bounding_box_tools/agg_boundary_stats.py
--rw-r--r--   0 simon      (501) staff       (20)    23590 2023-04-28 20:48:50.000000 Simba-UW-tf-dev-1.58.7/simba/bounding_box_tools/boundary_menus.py
--rw-r--r--   0 simon      (501) staff       (20)     8521 2023-04-28 19:59:05.000000 Simba-UW-tf-dev-1.58.7/simba/bounding_box_tools/boundary_statistics.py
--rw-r--r--   0 simon      (501) staff       (20)     6067 2023-04-27 20:23:35.000000 Simba-UW-tf-dev-1.58.7/simba/bounding_box_tools/find_boundaries.py
--rw-r--r--   0 simon      (501) staff       (20)    11228 2023-04-28 00:28:29.000000 Simba-UW-tf-dev-1.58.7/simba/bounding_box_tools/visualize_boundaries.py
--rw-r--r--   0 simon      (501) staff       (20)    43012 2023-05-03 18:35:59.000000 Simba-UW-tf-dev-1.58.7/simba/.DS_Store
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-03 21:14:48.000000 Simba-UW-tf-dev-1.58.7/simba/feature_extractors/
--rw-r--r--   0 simon      (501) staff       (20)    42323 2023-04-28 19:59:05.000000 Simba-UW-tf-dev-1.58.7/simba/feature_extractors/feature_extractor_14bp.py
--rw-r--r--   0 simon      (501) staff       (20)    21427 2023-04-28 15:16:26.000000 Simba-UW-tf-dev-1.58.7/simba/feature_extractors/feature_extractor_7bp.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-03 21:14:48.000000 Simba-UW-tf-dev-1.58.7/simba/feature_extractors/misc/
--rw-r--r--   0 simon      (501) staff       (20)     1685 2023-04-14 17:52:01.000000 Simba-UW-tf-dev-1.58.7/simba/feature_extractors/misc/doctests.py
--rw-r--r--   0 simon      (501) staff       (20)    23850 2023-04-17 18:48:40.000000 Simba-UW-tf-dev-1.58.7/simba/feature_extractors/misc/fish_feature_extractor_2023_version_3.py
--rw-r--r--   0 simon      (501) staff       (20)     2732 2023-04-04 19:46:36.000000 Simba-UW-tf-dev-1.58.7/simba/feature_extractors/misc/read_in_mp.py
--rw-r--r--   0 simon      (501) staff       (20)     2460 2023-04-22 18:02:29.000000 Simba-UW-tf-dev-1.58.7/simba/feature_extractors/misc/peaks.py
--rw-r--r--   0 simon      (501) staff       (20)    14141 2023-03-15 17:20:08.000000 Simba-UW-tf-dev-1.58.7/simba/feature_extractors/misc/fish_feature_extractor_2022.py
--rw-r--r--   0 simon      (501) staff       (20)     2053 2023-04-04 03:00:41.000000 Simba-UW-tf-dev-1.58.7/simba/feature_extractors/misc/convex_hull_3_scratch_3.py
--rw-r--r--   0 simon      (501) staff       (20)     5762 2023-04-04 01:54:33.000000 Simba-UW-tf-dev-1.58.7/simba/feature_extractors/misc/convex_hull_scratch_1.py
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-14 19:36:02.000000 Simba-UW-tf-dev-1.58.7/simba/feature_extractors/misc/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)    21398 2023-04-16 17:03:37.000000 Simba-UW-tf-dev-1.58.7/simba/feature_extractors/misc/fish_feature_extractor_2023_version_2.py
--rw-r--r--   0 simon      (501) staff       (20)     7127 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.7/simba/feature_extractors/misc/egocentrical_aligner.py
--rw-r--r--   0 simon      (501) staff       (20)     1213 2023-04-11 20:12:47.000000 Simba-UW-tf-dev-1.58.7/simba/feature_extractors/misc/count_values_in_range.py
--rw-r--r--   0 simon      (501) staff       (20)     4708 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.7/simba/feature_extractors/misc/graph_creator.py
--rw-r--r--   0 simon      (501) staff       (20)     3954 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.7/simba/feature_extractors/misc/termite_rois.csv
--rw-r--r--   0 simon      (501) staff       (20)      732 2023-03-20 12:13:51.000000 Simba-UW-tf-dev-1.58.7/simba/feature_extractors/misc/mutual_exclusive.py
--rw-r--r--   0 simon      (501) staff       (20)     2841 2023-04-14 15:16:23.000000 Simba-UW-tf-dev-1.58.7/simba/feature_extractors/misc/video_color.py
--rw-r--r--   0 simon      (501) staff       (20)     1862 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.7/simba/feature_extractors/misc/graph_3d_plotter.py
--rw-r--r--   0 simon      (501) staff       (20)     5232 2023-04-13 14:05:29.000000 Simba-UW-tf-dev-1.58.7/simba/feature_extractors/misc/video_rotator.py
--rw-r--r--   0 simon      (501) staff       (20)     2692 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.7/simba/feature_extractors/misc/add_probability_cnt_features.py
--rw-r--r--   0 simon      (501) staff       (20)     1619 2023-04-08 20:02:08.000000 Simba-UW-tf-dev-1.58.7/simba/feature_extractors/misc/make_splash.py
--rw-r--r--   0 simon      (501) staff       (20)     1658 2023-04-22 19:16:28.000000 Simba-UW-tf-dev-1.58.7/simba/feature_extractors/misc/time_stamp_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)     5232 2023-04-15 19:24:18.000000 Simba-UW-tf-dev-1.58.7/simba/feature_extractors/misc/video_rotator_mp.py
--rw-r--r--   0 simon      (501) staff       (20)    30677 2023-04-27 01:57:28.000000 Simba-UW-tf-dev-1.58.7/simba/feature_extractors/misc/fish_feature_extractor_2023_version_4.py
--rw-r--r--   0 simon      (501) staff       (20)     2058 2023-04-03 23:51:37.000000 Simba-UW-tf-dev-1.58.7/simba/feature_extractors/misc/convex_hull_scratch_2.py
--rw-r--r--   0 simon      (501) staff       (20)    27783 2023-04-28 19:59:05.000000 Simba-UW-tf-dev-1.58.7/simba/feature_extractors/feature_extractor_8bps_2_animals.py
--rw-r--r--   0 simon      (501) staff       (20)    10244 2023-04-25 21:03:39.000000 Simba-UW-tf-dev-1.58.7/simba/feature_extractors/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)     3491 2023-05-03 13:59:23.000000 Simba-UW-tf-dev-1.58.7/simba/feature_extractors/perimeter_jit.py
--rw-r--r--   0 simon      (501) staff       (20)    13322 2023-04-28 19:59:05.000000 Simba-UW-tf-dev-1.58.7/simba/feature_extractors/feature_subsets.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.7/simba/feature_extractors/__init__.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-03 21:14:48.000000 Simba-UW-tf-dev-1.58.7/simba/feature_extractors/__pycache__/
--rw-r--r--   0 simon      (501) staff       (20)      905 2023-04-04 11:31:57.000000 Simba-UW-tf-dev-1.58.7/simba/feature_extractors/__pycache__/perimeter_jit.quickhull_2d-16.py36m.nbi
--rw-r--r--   0 simon      (501) staff       (20)   238196 2023-04-04 11:31:57.000000 Simba-UW-tf-dev-1.58.7/simba/feature_extractors/__pycache__/perimeter_jit.quickhull_2d-16.py36m.1.nbc
--rw-r--r--   0 simon      (501) staff       (20)    69038 2023-04-04 11:32:25.000000 Simba-UW-tf-dev-1.58.7/simba/feature_extractors/__pycache__/perimeter_jit.process-7.py36m.1.nbc
--rw-r--r--   0 simon      (501) staff       (20)   238298 2023-04-04 11:32:29.000000 Simba-UW-tf-dev-1.58.7/simba/feature_extractors/__pycache__/perimeter_jit.convex_hull_perimeter_2d-16.py36m.1.nbc
--rw-r--r--   0 simon      (501) staff       (20)    69338 2023-04-04 11:32:26.000000 Simba-UW-tf-dev-1.58.7/simba/feature_extractors/__pycache__/perimeter_jit.process-7.py36m.2.nbc
--rw-r--r--   0 simon      (501) staff       (20)      917 2023-04-04 11:32:29.000000 Simba-UW-tf-dev-1.58.7/simba/feature_extractors/__pycache__/perimeter_jit.convex_hull_perimeter_2d-16.py36m.nbi
--rw-r--r--   0 simon      (501) staff       (20)     2179 2023-04-04 11:32:26.000000 Simba-UW-tf-dev-1.58.7/simba/feature_extractors/__pycache__/perimeter_jit.process-7.py36m.nbi
--rw-r--r--   0 simon      (501) staff       (20)     8282 2023-04-27 20:23:35.000000 Simba-UW-tf-dev-1.58.7/simba/feature_extractors/feature_extractor_user_defined.py
--rw-r--r--   0 simon      (501) staff       (20)    46269 2023-04-28 19:59:05.000000 Simba-UW-tf-dev-1.58.7/simba/feature_extractors/feature_extractor_16bp.py
--rw-r--r--   0 simon      (501) staff       (20)    28134 2023-04-28 18:40:57.000000 Simba-UW-tf-dev-1.58.7/simba/feature_extractors/feature_extractor_9bp.py
--rw-r--r--   0 simon      (501) staff       (20)    23897 2023-04-28 19:59:05.000000 Simba-UW-tf-dev-1.58.7/simba/feature_extractors/feature_extractor_8bp.py
--rw-r--r--   0 simon      (501) staff       (20)    16825 2023-04-27 20:23:35.000000 Simba-UW-tf-dev-1.58.7/simba/feature_extractors/feature_extractor_4bp.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-03 21:14:48.000000 Simba-UW-tf-dev-1.58.7/simba/feature_extractors/.idea/
--rw-r--r--   0 simon      (501) staff       (20)      617 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.7/simba/feature_extractors/.idea/features_scripts.iml
--rw-r--r--   0 simon      (501) staff       (20)      138 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.7/simba/feature_extractors/.idea/encodings.xml
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-03 21:14:48.000000 Simba-UW-tf-dev-1.58.7/simba/feature_extractors/.idea/inspectionProfiles/
--rw-r--r--   0 simon      (501) staff       (20)      822 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.7/simba/feature_extractors/.idea/inspectionProfiles/Project_Default.xml
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-03 21:14:48.000000 Simba-UW-tf-dev-1.58.7/simba/feature_extractors/.idea/libraries/
--rw-r--r--   0 simon      (501) staff       (20)      128 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.7/simba/feature_extractors/.idea/libraries/R_User_Library.xml
--rw-r--r--   0 simon      (501) staff       (20)      273 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.7/simba/feature_extractors/.idea/.gitignore
--rw-r--r--   0 simon      (501) staff       (20)     8081 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.7/simba/feature_extractors/.idea/workspace.xml
--rw-r--r--   0 simon      (501) staff       (20)      291 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.7/simba/feature_extractors/.idea/modules.xml
--rw-r--r--   0 simon      (501) staff       (20)       23 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.7/simba/feature_extractors/.idea/.name
--rw-r--r--   0 simon      (501) staff       (20)      294 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.7/simba/feature_extractors/.idea/misc.xml
--rw-r--r--   0 simon      (501) staff       (20)    15449 2023-04-30 14:02:53.000000 Simba-UW-tf-dev-1.58.7/simba/requirements.txt
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-03 21:14:48.000000 Simba-UW-tf-dev-1.58.7/simba/mixins/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-15 17:26:03.000000 Simba-UW-tf-dev-1.58.7/simba/mixins/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)    41772 2023-05-03 16:41:23.000000 Simba-UW-tf-dev-1.58.7/simba/mixins/pop_up_mixin.py
--rw-r--r--   0 simon      (501) staff       (20)    29306 2023-04-29 19:43:53.000000 Simba-UW-tf-dev-1.58.7/simba/mixins/config_reader.py
--rw-r--r--   0 simon      (501) staff       (20)    17367 2023-05-01 18:54:03.000000 Simba-UW-tf-dev-1.58.7/simba/mixins/pose_importer_mixin.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-03 21:14:48.000000 Simba-UW-tf-dev-1.58.7/simba/mixins/__pycache__/
--rw-r--r--   0 simon      (501) staff       (20)     1223 2023-04-25 20:46:51.000000 Simba-UW-tf-dev-1.58.7/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-182.py36m.nbi
--rw-r--r--   0 simon      (501) staff       (20)    49894 2023-04-24 19:51:34.000000 Simba-UW-tf-dev-1.58.7/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-183.py36m.1.nbc
--rw-r--r--   0 simon      (501) staff       (20)     1223 2023-04-29 19:21:39.000000 Simba-UW-tf-dev-1.58.7/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-190.py36m.nbi
--rw-r--r--   0 simon      (501) staff       (20)    49963 2023-04-29 19:21:39.000000 Simba-UW-tf-dev-1.58.7/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-190.py36m.1.nbc
--rw-r--r--   0 simon      (501) staff       (20)     1223 2023-04-24 19:51:34.000000 Simba-UW-tf-dev-1.58.7/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-183.py36m.nbi
--rw-r--r--   0 simon      (501) staff       (20)    49894 2023-04-25 20:46:51.000000 Simba-UW-tf-dev-1.58.7/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-182.py36m.1.nbc
--rw-r--r--   0 simon      (501) staff       (20)    49894 2023-04-24 19:06:57.000000 Simba-UW-tf-dev-1.58.7/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-181.py36m.1.nbc
--rw-r--r--   0 simon      (501) staff       (20)     1223 2023-04-24 19:06:57.000000 Simba-UW-tf-dev-1.58.7/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-181.py36m.nbi
--rw-r--r--   0 simon      (501) staff       (20)    23305 2023-05-03 14:22:51.000000 Simba-UW-tf-dev-1.58.7/simba/mixins/feature_extraction_mixin.py
--rw-r--r--   0 simon      (501) staff       (20)    60449 2023-05-03 18:46:32.000000 Simba-UW-tf-dev-1.58.7/simba/mixins/plotting_mixin.py
--rw-r--r--   0 simon      (501) staff       (20)     6175 2023-05-02 18:14:28.000000 Simba-UW-tf-dev-1.58.7/simba/mixins/unsupervised_mixin.py
--rw-r--r--   0 simon      (501) staff       (20)    55362 2023-05-01 20:52:34.000000 Simba-UW-tf-dev-1.58.7/simba/mixins/train_model_mixin.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-03 21:14:48.000000 Simba-UW-tf-dev-1.58.7/simba/third_party_label_appenders/
--rw-r--r--   0 simon      (501) staff       (20)     6228 2023-04-26 18:27:58.000000 Simba-UW-tf-dev-1.58.7/simba/third_party_label_appenders/deepethogram_importer.py
--rw-r--r--   0 simon      (501) staff       (20)     9945 2023-04-25 01:50:43.000000 Simba-UW-tf-dev-1.58.7/simba/third_party_label_appenders/BORIS_appender.py
--rw-r--r--   0 simon      (501) staff       (20)     9063 2023-04-25 01:50:43.000000 Simba-UW-tf-dev-1.58.7/simba/third_party_label_appenders/observer_importer.py
--rw-r--r--   0 simon      (501) staff       (20)    16894 2023-04-28 19:59:05.000000 Simba-UW-tf-dev-1.58.7/simba/third_party_label_appenders/tools.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-04-01 14:10:06.000000 Simba-UW-tf-dev-1.58.7/simba/third_party_label_appenders/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)    18248 2023-04-28 19:59:05.000000 Simba-UW-tf-dev-1.58.7/simba/third_party_label_appenders/third_party_appender.py
--rw-r--r--   0 simon      (501) staff       (20)     8173 2023-04-27 19:42:17.000000 Simba-UW-tf-dev-1.58.7/simba/third_party_label_appenders/ethovision_import.py
--rw-r--r--   0 simon      (501) staff       (20)     6859 2023-04-25 01:50:43.000000 Simba-UW-tf-dev-1.58.7/simba/third_party_label_appenders/BENTO_appender.py
--rw-r--r--   0 simon      (501) staff       (20)     5331 2023-04-25 01:50:43.000000 Simba-UW-tf-dev-1.58.7/simba/third_party_label_appenders/solomon_importer.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-03 21:14:48.000000 Simba-UW-tf-dev-1.58.7/simba/cue_light_tools/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-15 17:25:58.000000 Simba-UW-tf-dev-1.58.7/simba/cue_light_tools/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)     7594 2023-05-01 19:38:38.000000 Simba-UW-tf-dev-1.58.7/simba/cue_light_tools/cue_light_clf_statistics.py
--rw-r--r--   0 simon      (501) staff       (20)    12198 2023-05-01 19:31:25.000000 Simba-UW-tf-dev-1.58.7/simba/cue_light_tools/cue_light_analyzer.py
--rw-r--r--   0 simon      (501) staff       (20)    16737 2023-05-01 19:58:28.000000 Simba-UW-tf-dev-1.58.7/simba/cue_light_tools/cue_light_menues.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.7/simba/cue_light_tools/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)     1690 2023-04-27 20:23:35.000000 Simba-UW-tf-dev-1.58.7/simba/cue_light_tools/cue_light_tools.py
--rw-r--r--   0 simon      (501) staff       (20)    15289 2023-05-01 19:38:38.000000 Simba-UW-tf-dev-1.58.7/simba/cue_light_tools/cue_light_visualizer.py
--rw-r--r--   0 simon      (501) staff       (20)    12615 2023-05-01 19:51:32.000000 Simba-UW-tf-dev-1.58.7/simba/cue_light_tools/cue_light_movement_statistics.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.7/simba/__init__.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-03 21:14:48.000000 Simba-UW-tf-dev-1.58.7/simba/utils/
--rw-r--r--   0 simon      (501) staff       (20)    11588 2023-04-29 19:01:32.000000 Simba-UW-tf-dev-1.58.7/simba/utils/config_creator.py
--rw-r--r--   0 simon      (501) staff       (20)    20258 2023-05-03 16:24:11.000000 Simba-UW-tf-dev-1.58.7/simba/utils/enums.py
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-14 20:15:03.000000 Simba-UW-tf-dev-1.58.7/simba/utils/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)     7365 2023-04-27 20:23:35.000000 Simba-UW-tf-dev-1.58.7/simba/utils/warnings.py
--rw-r--r--   0 simon      (501) staff       (20)     5592 2023-04-27 20:23:35.000000 Simba-UW-tf-dev-1.58.7/simba/utils/checks.py
--rw-r--r--   0 simon      (501) staff       (20)    33901 2023-05-03 20:38:40.000000 Simba-UW-tf-dev-1.58.7/simba/utils/read_write.py
--rw-r--r--   0 simon      (501) staff       (20)     7034 2023-04-28 19:59:05.000000 Simba-UW-tf-dev-1.58.7/simba/utils/lookups.py
--rw-r--r--   0 simon      (501) staff       (20)    14666 2023-04-28 19:59:06.000000 Simba-UW-tf-dev-1.58.7/simba/utils/errors.py
--rw-r--r--   0 simon      (501) staff       (20)    14068 2023-04-29 19:01:32.000000 Simba-UW-tf-dev-1.58.7/simba/utils/data.py
--rw-r--r--   0 simon      (501) staff       (20)     1573 2023-04-29 19:08:53.000000 Simba-UW-tf-dev-1.58.7/simba/utils/printing.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-03 21:14:48.000000 Simba-UW-tf-dev-1.58.7/simba/pose_processors/
--rw-r--r--   0 simon      (501) staff       (20)     8347 2023-04-28 19:59:05.000000 Simba-UW-tf-dev-1.58.7/simba/pose_processors/reorganize_keypoint.py
--rw-r--r--   0 simon      (501) staff       (20)     5223 2023-04-27 20:23:35.000000 Simba-UW-tf-dev-1.58.7/simba/pose_processors/remove_keypoints.py
--rw-r--r--   0 simon      (501) staff       (20)     2613 2023-04-25 15:16:24.000000 Simba-UW-tf-dev-1.58.7/simba/pose_processors/pose_reset.py
--rw-r--r--   0 simon      (501) staff       (20)     5617 2023-04-27 19:42:17.000000 Simba-UW-tf-dev-1.58.7/simba/pose_processors/reverse_pose.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-03 21:14:48.000000 Simba-UW-tf-dev-1.58.7/simba/plotting/
--rw-r--r--   0 simon      (501) staff       (20)     9092 2023-04-29 19:43:53.000000 Simba-UW-tf-dev-1.58.7/simba/plotting/gantt_creator.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-03 21:14:48.000000 Simba-UW-tf-dev-1.58.7/simba/plotting/tools/
--rw-r--r--   0 simon      (501) staff       (20)     5388 2023-04-27 20:23:35.000000 Simba-UW-tf-dev-1.58.7/simba/plotting/tools/tkinter_tools.py
--rw-r--r--   0 simon      (501) staff       (20)    13238 2023-04-30 15:54:10.000000 Simba-UW-tf-dev-1.58.7/simba/plotting/ROI_plotter_mp.py
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-04-25 23:35:57.000000 Simba-UW-tf-dev-1.58.7/simba/plotting/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)    14636 2023-04-28 19:59:05.000000 Simba-UW-tf-dev-1.58.7/simba/plotting/shap_agg_stats_visualizer.py
--rw-r--r--   0 simon      (501) staff       (20)    10173 2023-04-28 19:59:05.000000 Simba-UW-tf-dev-1.58.7/simba/plotting/gantt_creator_mp.py
--rw-r--r--   0 simon      (501) staff       (20)    15981 2023-04-28 19:59:05.000000 Simba-UW-tf-dev-1.58.7/simba/plotting/heat_mapper_clf_mp.py
--rw-r--r--   0 simon      (501) staff       (20)     8563 2023-04-28 19:59:05.000000 Simba-UW-tf-dev-1.58.7/simba/plotting/probability_plot_creator.py
--rw-r--r--   0 simon      (501) staff       (20)    12304 2023-04-29 19:01:32.000000 Simba-UW-tf-dev-1.58.7/simba/plotting/plot_clf_results.py
--rw-r--r--   0 simon      (501) staff       (20)    15119 2023-05-03 19:00:40.000000 Simba-UW-tf-dev-1.58.7/simba/plotting/plot_clf_results_mp.py
--rw-r--r--   0 simon      (501) staff       (20)    15891 2023-04-28 19:59:05.000000 Simba-UW-tf-dev-1.58.7/simba/plotting/ROI_feature_visualizer.py
--rw-r--r--   0 simon      (501) staff       (20)    12739 2023-04-28 19:59:05.000000 Simba-UW-tf-dev-1.58.7/simba/plotting/heat_mapper_location.py
--rw-r--r--   0 simon      (501) staff       (20)    10168 2023-04-30 15:51:37.000000 Simba-UW-tf-dev-1.58.7/simba/plotting/probability_plot_creator_mp.py
--rw-r--r--   0 simon      (501) staff       (20)     5232 2023-04-28 19:59:05.000000 Simba-UW-tf-dev-1.58.7/simba/plotting/interactive_probability_grapher.py
--rw-r--r--   0 simon      (501) staff       (20)     5754 2023-04-28 19:59:05.000000 Simba-UW-tf-dev-1.58.7/simba/plotting/plot_pose_in_dir.py
--rw-r--r--   0 simon      (501) staff       (20)    12771 2023-04-26 14:16:42.000000 Simba-UW-tf-dev-1.58.7/simba/plotting/single_run_model_validation_video.py
--rw-r--r--   0 simon      (501) staff       (20)    12242 2023-04-28 19:59:05.000000 Simba-UW-tf-dev-1.58.7/simba/plotting/frame_mergerer_ffmpeg.py
--rw-r--r--   0 simon      (501) staff       (20)     7917 2023-04-28 19:59:05.000000 Simba-UW-tf-dev-1.58.7/simba/plotting/Directing_animals_visualizer_mp.py
--rw-r--r--   0 simon      (501) staff       (20)    11210 2023-04-28 19:59:05.000000 Simba-UW-tf-dev-1.58.7/simba/plotting/clf_validator.py
--rw-r--r--   0 simon      (501) staff       (20)    15146 2023-05-03 21:12:42.000000 Simba-UW-tf-dev-1.58.7/simba/plotting/path_plotter_mp.py
--rw-r--r--   0 simon      (501) staff       (20)    11330 2023-04-28 19:59:05.000000 Simba-UW-tf-dev-1.58.7/simba/plotting/ROI_feature_visualizer_mp.py
--rw-r--r--   0 simon      (501) staff       (20)     9467 2023-05-03 00:36:49.000000 Simba-UW-tf-dev-1.58.7/simba/plotting/data_plotter.py
--rw-r--r--   0 simon      (501) staff       (20)    13232 2023-05-03 18:58:48.000000 Simba-UW-tf-dev-1.58.7/simba/plotting/path_plotter.py
--rw-r--r--   0 simon      (501) staff       (20)     8493 2023-04-27 19:42:17.000000 Simba-UW-tf-dev-1.58.7/simba/plotting/ez_lineplot.py
--rw-r--r--   0 simon      (501) staff       (20)    11482 2023-04-27 19:42:17.000000 Simba-UW-tf-dev-1.58.7/simba/plotting/distance_plotter_mp.py
--rw-r--r--   0 simon      (501) staff       (20)    15610 2023-04-28 19:59:06.000000 Simba-UW-tf-dev-1.58.7/simba/plotting/ROI_plotter.py
--rw-r--r--   0 simon      (501) staff       (20)    13133 2023-04-28 19:59:05.000000 Simba-UW-tf-dev-1.58.7/simba/plotting/heat_mapper_clf.py
--rw-r--r--   0 simon      (501) staff       (20)     8979 2023-04-28 19:59:05.000000 Simba-UW-tf-dev-1.58.7/simba/plotting/distance_plotter.py
--rw-r--r--   0 simon      (501) staff       (20)     8267 2023-04-30 15:54:10.000000 Simba-UW-tf-dev-1.58.7/simba/plotting/single_run_model_validation_video_mp.py
--rw-r--r--   0 simon      (501) staff       (20)     9761 2023-04-28 19:59:05.000000 Simba-UW-tf-dev-1.58.7/simba/plotting/Directing_animals_visualizer.py
--rw-r--r--   0 simon      (501) staff       (20)    16321 2023-04-28 19:59:05.000000 Simba-UW-tf-dev-1.58.7/simba/plotting/heat_mapper_location_mp.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-03 21:14:48.000000 Simba-UW-tf-dev-1.58.7/simba/dash_app/
--rw-r--r--   0 simon      (501) staff       (20)    49699 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.7/simba/dash_app/SimBA_dash_app.py
--rw-r--r--   0 simon      (501) staff       (20)     5029 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.7/simba/dash_app/run_dash_tkinter.py
--rw-r--r--   0 simon      (501) staff       (20)    24474 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.7/simba/dash_app/dash_app.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-03 21:14:48.000000 Simba-UW-tf-dev-1.58.7/simba/data_processors/
--rw-r--r--   0 simon      (501) staff       (20)     6329 2023-04-28 18:51:08.000000 Simba-UW-tf-dev-1.58.7/simba/data_processors/agg_clf_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)    11575 2023-04-28 19:59:05.000000 Simba-UW-tf-dev-1.58.7/simba/data_processors/interpolation_smoothing.py
--rw-r--r--   0 simon      (501) staff       (20)     7407 2023-04-28 19:12:39.000000 Simba-UW-tf-dev-1.58.7/simba/data_processors/timebins_clf_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)    12822 2023-05-01 13:08:33.000000 Simba-UW-tf-dev-1.58.7/simba/data_processors/fsttc_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)     6317 2023-04-25 18:03:32.000000 Simba-UW-tf-dev-1.58.7/simba/data_processors/interpolate_pose.py
--rw-r--r--   0 simon      (501) staff       (20)     9646 2023-04-28 19:20:42.000000 Simba-UW-tf-dev-1.58.7/simba/data_processors/directing_other_animals_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)     9366 2023-04-29 19:01:32.000000 Simba-UW-tf-dev-1.58.7/simba/data_processors/timebins_movement_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)     4821 2023-04-28 19:59:05.000000 Simba-UW-tf-dev-1.58.7/simba/data_processors/severity_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)    16794 2023-04-29 19:01:32.000000 Simba-UW-tf-dev-1.58.7/simba/data_processors/pup_retrieval_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)     2904 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.7/simba/data_processors/pybursts_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)     9551 2023-04-28 19:59:05.000000 Simba-UW-tf-dev-1.58.7/simba/data_processors/kleinberg_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)     7698 2023-05-03 14:34:44.000000 Simba-UW-tf-dev-1.58.7/simba/data_processors/movement_calculator.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-03 21:14:48.000000 Simba-UW-tf-dev-1.58.7/simba/pose_configurations_archive/
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-03 21:14:48.000000 Simba-UW-tf-dev-1.58.7/simba/pose_configurations_archive/pose_configurations_archive_1/
--rw-r--r--   0 simon      (501) staff       (20)    14340 2023-03-30 11:05:37.000000 Simba-UW-tf-dev-1.58.7/simba/pose_configurations_archive/pose_configurations_archive_1/.DS_Store
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-03 21:14:48.000000 Simba-UW-tf-dev-1.58.7/simba/pose_configurations_archive/pose_configurations_archive_1/bp_names/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-16 13:26:00.000000 Simba-UW-tf-dev-1.58.7/simba/pose_configurations_archive/pose_configurations_archive_1/bp_names/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)     1334 2023-04-28 23:45:27.000000 Simba-UW-tf-dev-1.58.7/simba/pose_configurations_archive/pose_configurations_archive_1/bp_names/bp_names.csv
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-03 21:14:48.000000 Simba-UW-tf-dev-1.58.7/simba/pose_configurations_archive/pose_configurations_archive_1/no_animals/
--rw-r--r--   0 simon      (501) staff       (20)       26 2023-04-28 23:45:27.000000 Simba-UW-tf-dev-1.58.7/simba/pose_configurations_archive/pose_configurations_archive_1/no_animals/no_animals.csv
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-16 13:26:19.000000 Simba-UW-tf-dev-1.58.7/simba/pose_configurations_archive/pose_configurations_archive_1/no_animals/.DS_Store
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-03 21:14:48.000000 Simba-UW-tf-dev-1.58.7/simba/pose_configurations_archive/pose_configurations_archive_1/configuration_names/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-16 13:26:14.000000 Simba-UW-tf-dev-1.58.7/simba/pose_configurations_archive/pose_configurations_archive_1/configuration_names/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)      282 2023-04-28 23:45:27.000000 Simba-UW-tf-dev-1.58.7/simba/pose_configurations_archive/pose_configurations_archive_1/configuration_names/pose_config_names.csv
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-03 21:14:48.000000 Simba-UW-tf-dev-1.58.7/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/
--rw-r--r--   0 simon      (501) staff       (20)     8196 2023-03-30 10:45:10.000000 Simba-UW-tf-dev-1.58.7/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)    39805 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.7/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/8.png
--rw-r--r--   0 simon      (501) staff       (20)    62501 2023-03-30 10:39:05.000000 Simba-UW-tf-dev-1.58.7/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/9.png
--rw-r--r--   0 simon      (501) staff       (20)     6172 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.7/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/12.png
--rw-r--r--   0 simon      (501) staff       (20)    11376 2023-04-28 23:45:27.000000 Simba-UW-tf-dev-1.58.7/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/13.png
--rw-r--r--   0 simon      (501) staff       (20)    69501 2023-03-30 10:44:04.000000 Simba-UW-tf-dev-1.58.7/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/11.png
--rw-r--r--   0 simon      (501) staff       (20)    69410 2023-03-30 10:40:01.000000 Simba-UW-tf-dev-1.58.7/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/10.png
--rw-r--r--   0 simon      (501) staff       (20)    16000 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.7/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/4.png
--rw-r--r--   0 simon      (501) staff       (20)    28150 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.7/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/5.png
--rw-r--r--   0 simon      (501) staff       (20)    31140 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.7/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/7.png
--rw-r--r--   0 simon      (501) staff       (20)    30634 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.7/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/6.png
--rw-r--r--   0 simon      (501) staff       (20)    15417 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.7/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/2.png
--rw-r--r--   0 simon      (501) staff       (20)    15786 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.7/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/3.png
--rw-r--r--   0 simon      (501) staff       (20)    18939 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.7/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/1.png
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-03 21:14:48.000000 Simba-UW-tf-dev-1.58.7/simba/model/
--rw-r--r--   0 simon      (501) staff       (20)    19187 2023-04-29 19:01:32.000000 Simba-UW-tf-dev-1.58.7/simba/model/train_rf.py
--rw-r--r--   0 simon      (501) staff       (20)     3542 2023-04-28 20:13:23.000000 Simba-UW-tf-dev-1.58.7/simba/model/inference_batch.py
--rw-r--r--   0 simon      (501) staff       (20)    18624 2023-05-01 20:34:07.000000 Simba-UW-tf-dev-1.58.7/simba/model/grid_search_rf.py
--rw-r--r--   0 simon      (501) staff       (20)     3170 2023-04-28 20:11:10.000000 Simba-UW-tf-dev-1.58.7/simba/model/inference_validation.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-03 21:14:48.000000 Simba-UW-tf-dev-1.58.7/simba/roi_tools/
--rw-r--r--   0 simon      (501) staff       (20)     6487 2023-05-03 18:24:03.000000 Simba-UW-tf-dev-1.58.7/simba/roi_tools/ROI_time_bin_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)     1753 2023-04-27 19:42:17.000000 Simba-UW-tf-dev-1.58.7/simba/roi_tools/ROI_movement_analyzer.py
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-20 12:47:56.000000 Simba-UW-tf-dev-1.58.7/simba/roi_tools/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)    43131 2023-04-28 20:51:11.000000 Simba-UW-tf-dev-1.58.7/simba/roi_tools/ROI_define.py
--rw-r--r--   0 simon      (501) staff       (20)     3403 2023-04-29 19:01:32.000000 Simba-UW-tf-dev-1.58.7/simba/roi_tools/ROI_reset.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.7/simba/roi_tools/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)    19758 2023-05-03 16:31:29.000000 Simba-UW-tf-dev-1.58.7/simba/roi_tools/ROI_analyzer.py
--rw-r--r--   0 simon      (501) staff       (20)    11332 2023-04-26 21:13:20.000000 Simba-UW-tf-dev-1.58.7/simba/roi_tools/ROI_feature_analyzer.py
--rw-r--r--   0 simon      (501) staff       (20)     3654 2023-04-29 19:01:32.000000 Simba-UW-tf-dev-1.58.7/simba/roi_tools/ROI_multiply.py
--rw-r--r--   0 simon      (501) staff       (20)      961 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.7/simba/roi_tools/ROI_size_calculations.py
--rw-r--r--   0 simon      (501) staff       (20)     3505 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.7/simba/roi_tools/ROI_zoom.py
--rw-r--r--   0 simon      (501) staff       (20)    11384 2023-04-27 19:42:17.000000 Simba-UW-tf-dev-1.58.7/simba/roi_tools/ROI_directing_analyzer.py
--rw-r--r--   0 simon      (501) staff       (20)    10128 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.7/simba/roi_tools/ROI_move_shape.py
--rw-r--r--   0 simon      (501) staff       (20)     5079 2023-04-29 19:01:32.000000 Simba-UW-tf-dev-1.58.7/simba/roi_tools/ROI_menus.py
--rw-r--r--   0 simon      (501) staff       (20)    13793 2023-04-26 14:59:42.000000 Simba-UW-tf-dev-1.58.7/simba/roi_tools/ROI_clf_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)    22688 2023-04-29 19:01:32.000000 Simba-UW-tf-dev-1.58.7/simba/roi_tools/ROI_image.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-03 21:14:48.000000 Simba-UW-tf-dev-1.58.7/simba/pose_importers/
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-03 21:14:48.000000 Simba-UW-tf-dev-1.58.7/simba/pose_importers/misc/
--rw-r--r--   0 simon      (501) staff       (20)     7349 2023-05-01 00:05:15.000000 Simba-UW-tf-dev-1.58.7/simba/pose_importers/misc/sleap_csv_importer.py
--rw-r--r--   0 simon      (501) staff       (20)     9719 2023-05-01 00:05:15.000000 Simba-UW-tf-dev-1.58.7/simba/pose_importers/misc/sleap_h5_importer.py
--rw-r--r--   0 simon      (501) staff       (20)     6451 2023-05-01 17:30:49.000000 Simba-UW-tf-dev-1.58.7/simba/pose_importers/misc/madlc_importer.py
--rw-r--r--   0 simon      (501) staff       (20)     7943 2023-05-01 19:07:14.000000 Simba-UW-tf-dev-1.58.7/simba/pose_importers/misc/apt_trk_importer.py
--rw-r--r--   0 simon      (501) staff       (20)    10945 2023-05-01 17:21:29.000000 Simba-UW-tf-dev-1.58.7/simba/pose_importers/misc/sleap_slp_importer.py
--rw-r--r--   0 simon      (501) staff       (20)     2464 2023-04-27 19:42:17.000000 Simba-UW-tf-dev-1.58.7/simba/pose_importers/read_DANNCE_mat.py
--rw-r--r--   0 simon      (501) staff       (20)    22015 2023-04-29 19:01:32.000000 Simba-UW-tf-dev-1.58.7/simba/pose_importers/sleap_importer_slp.py
--rw-r--r--   0 simon      (501) staff       (20)    23524 2023-04-30 23:21:29.000000 Simba-UW-tf-dev-1.58.7/simba/pose_importers/sleap_importer_h5.py
--rw-r--r--   0 simon      (501) staff       (20)    23603 2023-04-29 19:01:32.000000 Simba-UW-tf-dev-1.58.7/simba/pose_importers/dlc_multi_animal_importer.py
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-04-25 16:49:14.000000 Simba-UW-tf-dev-1.58.7/simba/pose_importers/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)    21021 2023-04-30 23:23:03.000000 Simba-UW-tf-dev-1.58.7/simba/pose_importers/sleap_importer_csv.py
--rw-r--r--   0 simon      (501) staff       (20)     7783 2023-04-28 20:16:23.000000 Simba-UW-tf-dev-1.58.7/simba/pose_importers/import_mars.py
--rw-r--r--   0 simon      (501) staff       (20)     6949 2023-04-28 20:19:13.000000 Simba-UW-tf-dev-1.58.7/simba/pose_importers/dlc_importer_csv.py
--rw-r--r--   0 simon      (501) staff       (20)     8060 2023-04-28 19:20:42.000000 Simba-UW-tf-dev-1.58.7/simba/pose_importers/trk_importer.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-03 21:14:48.000000 Simba-UW-tf-dev-1.58.7/simba/pose_configurations/
--rw-r--r--   0 simon      (501) staff       (20)    14340 2023-03-30 11:05:37.000000 Simba-UW-tf-dev-1.58.7/simba/pose_configurations/.DS_Store
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-03 21:14:48.000000 Simba-UW-tf-dev-1.58.7/simba/pose_configurations/bp_names/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-16 13:26:00.000000 Simba-UW-tf-dev-1.58.7/simba/pose_configurations/bp_names/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)     1316 2023-04-29 18:20:02.000000 Simba-UW-tf-dev-1.58.7/simba/pose_configurations/bp_names/bp_names.csv
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-03 21:14:48.000000 Simba-UW-tf-dev-1.58.7/simba/pose_configurations/no_animals/
--rw-r--r--   0 simon      (501) staff       (20)       24 2023-04-29 18:20:02.000000 Simba-UW-tf-dev-1.58.7/simba/pose_configurations/no_animals/no_animals.csv
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-16 13:26:19.000000 Simba-UW-tf-dev-1.58.7/simba/pose_configurations/no_animals/.DS_Store
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-03 21:14:48.000000 Simba-UW-tf-dev-1.58.7/simba/pose_configurations/configuration_names/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-16 13:26:14.000000 Simba-UW-tf-dev-1.58.7/simba/pose_configurations/configuration_names/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)      267 2023-04-29 18:20:02.000000 Simba-UW-tf-dev-1.58.7/simba/pose_configurations/configuration_names/pose_config_names.csv
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-03 21:14:48.000000 Simba-UW-tf-dev-1.58.7/simba/pose_configurations/schematics/
--rw-r--r--   0 simon      (501) staff       (20)    39805 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.7/simba/pose_configurations/schematics/8.png
--rw-r--r--   0 simon      (501) staff       (20)    62501 2023-03-30 10:39:05.000000 Simba-UW-tf-dev-1.58.7/simba/pose_configurations/schematics/9.png
--rw-r--r--   0 simon      (501) staff       (20)     6172 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.7/simba/pose_configurations/schematics/12.png
--rw-r--r--   0 simon      (501) staff       (20)    69501 2023-03-30 10:44:04.000000 Simba-UW-tf-dev-1.58.7/simba/pose_configurations/schematics/11.png
--rw-r--r--   0 simon      (501) staff       (20)    69410 2023-03-30 10:40:01.000000 Simba-UW-tf-dev-1.58.7/simba/pose_configurations/schematics/10.png
--rw-r--r--   0 simon      (501) staff       (20)    16000 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.7/simba/pose_configurations/schematics/4.png
--rw-r--r--   0 simon      (501) staff       (20)    28150 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.7/simba/pose_configurations/schematics/5.png
--rw-r--r--   0 simon      (501) staff       (20)    31140 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.7/simba/pose_configurations/schematics/7.png
--rw-r--r--   0 simon      (501) staff       (20)    30634 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.7/simba/pose_configurations/schematics/6.png
--rw-r--r--   0 simon      (501) staff       (20)    15417 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.7/simba/pose_configurations/schematics/2.png
--rw-r--r--   0 simon      (501) staff       (20)    15786 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.7/simba/pose_configurations/schematics/3.png
--rw-r--r--   0 simon      (501) staff       (20)    18939 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.7/simba/pose_configurations/schematics/1.png
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-03 21:14:48.000000 Simba-UW-tf-dev-1.58.7/simba/video_processors/
--rw-r--r--   0 simon      (501) staff       (20)    41580 2023-04-29 19:01:32.000000 Simba-UW-tf-dev-1.58.7/simba/video_processors/video_processing.py
--rw-r--r--   0 simon      (501) staff       (20)     8196 2023-03-17 14:43:38.000000 Simba-UW-tf-dev-1.58.7/simba/video_processors/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)     7171 2023-04-27 19:42:17.000000 Simba-UW-tf-dev-1.58.7/simba/video_processors/px_to_mm.py
--rw-r--r--   0 simon      (501) staff       (20)    24645 2023-04-28 20:51:11.000000 Simba-UW-tf-dev-1.58.7/simba/video_processors/batch_process_menus.py
--rw-r--r--   0 simon      (501) staff       (20)     7174 2023-04-28 19:59:05.000000 Simba-UW-tf-dev-1.58.7/simba/video_processors/multi_cropper.py
--rw-r--r--   0 simon      (501) staff       (20)     2833 2023-04-27 20:23:35.000000 Simba-UW-tf-dev-1.58.7/simba/video_processors/extract_frames.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.7/simba/video_processors/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)     8214 2023-04-28 19:26:14.000000 Simba-UW-tf-dev-1.58.7/simba/video_processors/calculate_px_dist.py
--rw-r--r--   0 simon      (501) staff       (20)     4695 2023-04-26 18:17:53.000000 Simba-UW-tf-dev-1.58.7/simba/video_processors/extract_seqframes.py
--rw-r--r--   0 simon      (501) staff       (20)    11106 2023-04-25 13:26:59.000000 Simba-UW-tf-dev-1.58.7/simba/video_processors/batch_process_create_ffmpeg_commands.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-03 21:14:48.000000 Simba-UW-tf-dev-1.58.7/simba/outlier_tools/
--rw-r--r--   0 simon      (501) staff       (20)     7377 2023-04-29 19:01:32.000000 Simba-UW-tf-dev-1.58.7/simba/outlier_tools/outlier_corrector_movement.py
--rw-r--r--   0 simon      (501) staff       (20)     8196 2023-03-15 17:05:05.000000 Simba-UW-tf-dev-1.58.7/simba/outlier_tools/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.7/simba/outlier_tools/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)     8190 2023-04-29 19:01:32.000000 Simba-UW-tf-dev-1.58.7/simba/outlier_tools/outlier_corrector_location.py
--rw-r--r--   0 simon      (501) staff       (20)     2913 2023-04-28 17:39:56.000000 Simba-UW-tf-dev-1.58.7/simba/outlier_tools/skip_outlier_correction.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-03 21:14:48.000000 Simba-UW-tf-dev-1.58.7/simba/outlier_tools/.idea/
--rw-r--r--   0 simon      (501) staff       (20)      617 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.7/simba/outlier_tools/.idea/outlier_scripts.iml
--rw-r--r--   0 simon      (501) staff       (20)      138 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.7/simba/outlier_tools/.idea/encodings.xml
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-03 21:14:48.000000 Simba-UW-tf-dev-1.58.7/simba/outlier_tools/.idea/inspectionProfiles/
--rw-r--r--   0 simon      (501) staff       (20)      668 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.7/simba/outlier_tools/.idea/inspectionProfiles/Project_Default.xml
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-03 21:14:48.000000 Simba-UW-tf-dev-1.58.7/simba/outlier_tools/.idea/libraries/
--rw-r--r--   0 simon      (501) staff       (20)      128 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.7/simba/outlier_tools/.idea/libraries/R_User_Library.xml
--rw-r--r--   0 simon      (501) staff       (20)     8102 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.7/simba/outlier_tools/.idea/workspace.xml
--rw-r--r--   0 simon      (501) staff       (20)      289 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.7/simba/outlier_tools/.idea/modules.xml
--rw-r--r--   0 simon      (501) staff       (20)      294 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.7/simba/outlier_tools/.idea/misc.xml
--rw-r--r--   0 simon      (501) staff       (20)    64875 2023-05-03 18:36:47.000000 Simba-UW-tf-dev-1.58.7/simba/SimBA.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-03 21:14:48.000000 Simba-UW-tf-dev-1.58.7/simba/assets/
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-03 21:14:48.000000 Simba-UW-tf-dev-1.58.7/simba/assets/unsupervised/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.7/simba/assets/unsupervised/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)   109483 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.7/simba/assets/unsupervised/model_names.parquet
--rw-r--r--   0 simon      (501) staff       (20)    14175 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.7/simba/assets/unsupervised/features.csv
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-03 21:14:48.000000 Simba-UW-tf-dev-1.58.7/simba/assets/shap/
--rw-r--r--   0 simon      (501) staff       (20)     1177 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.7/simba/assets/shap/down_arrow.jpg
--rw-r--r--   0 simon      (501) staff       (20)     1733 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.7/simba/assets/shap/intruder_shape.jpg
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-03 21:14:48.000000 Simba-UW-tf-dev-1.58.7/simba/assets/shap/feature_categories/
--rw-r--r--   0 simon      (501) staff       (20)      109 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.7/simba/assets/shap/feature_categories/.~lock.shap_feature_categories.csv#
--rw-r--r--   0 simon      (501) staff       (20)    17420 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.7/simba/assets/shap/feature_categories/shap_feature_categories.csv
--rw-r--r--   0 simon      (501) staff       (20)     8196 2023-04-10 20:37:13.000000 Simba-UW-tf-dev-1.58.7/simba/assets/shap/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)     1665 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.7/simba/assets/shap/resident_shape.jpg
--rw-r--r--   0 simon      (501) staff       (20)     2415 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.7/simba/assets/shap/resident_intruder_shape.jpg
--rw-r--r--   0 simon      (501) staff       (20)     2012 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.7/simba/assets/shap/animal_distances.jpg
--rw-r--r--   0 simon      (501) staff       (20)     4422 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.7/simba/assets/shap/baseline_scale.jpg
--rw-r--r--   0 simon      (501) staff       (20)   353824 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.7/simba/assets/shap/ubuntu.regular.ttf
--rw-r--r--   0 simon      (501) staff       (20)     6672 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.7/simba/assets/shap/side_scale.jpg
--rw-r--r--   0 simon      (501) staff       (20)   189004 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.7/simba/assets/shap/UbuntuMono-Regular.ttf
--rw-r--r--   0 simon      (501) staff       (20)     2737 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.7/simba/assets/shap/side_scale_5.jpg
--rw-r--r--   0 simon      (501) staff       (20)     1785 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.7/simba/assets/shap/intruder_movement.jpg
--rw-r--r--   0 simon      (501) staff       (20)     1435 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.7/simba/assets/shap/resident_movement.jpg
--rw-r--r--   0 simon      (501) staff       (20)     3134 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.7/simba/assets/shap/color_bar.jpg
--rw-r--r--   0 simon      (501) staff       (20)     2120 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.7/simba/assets/shap/resident_intruder_movement.jpg
--rw-r--r--   0 simon      (501) staff       (20)    16388 2023-04-25 19:14:34.000000 Simba-UW-tf-dev-1.58.7/simba/assets/.DS_Store
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-03 21:14:48.000000 Simba-UW-tf-dev-1.58.7/simba/assets/lookups/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.7/simba/assets/lookups/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)   270783 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.7/simba/assets/lookups/model_names.parquet
--rw-r--r--   0 simon      (501) staff       (20)     2987 2023-04-25 20:39:03.000000 Simba-UW-tf-dev-1.58.7/simba/assets/lookups/feature_extraction_headers.csv
--rw-r--r--   0 simon      (501) staff       (20)    14175 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.7/simba/assets/lookups/features.csv
--rw-r--r--   0 simon      (501) staff       (20)    14175 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.7/simba/assets/lookups/unsupervised_example_x.csv
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-03 21:14:48.000000 Simba-UW-tf-dev-1.58.7/simba/assets/stl/
--rw-r--r--   0 simon      (501) staff       (20)   551576 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.7/simba/assets/stl/operant_tray.stl
--rw-r--r--   0 simon      (501) staff       (20)    67647 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.7/simba/assets/stl/operant_lever.stl
--rw-r--r--   0 simon      (501) staff       (20)    92896 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.7/simba/assets/stl/operant_walls.stl
--rw-r--r--   0 simon      (501) staff       (20)  4759984 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.7/simba/assets/stl/grid_floor.stl
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-03 21:14:48.000000 Simba-UW-tf-dev-1.58.7/simba/assets/img/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-04-10 23:20:37.000000 Simba-UW-tf-dev-1.58.7/simba/assets/img/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)   399272 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.7/simba/assets/img/about_me.png
--rw-r--r--   0 simon      (501) staff       (20)   117108 2023-04-10 23:06:31.000000 Simba-UW-tf-dev-1.58.7/simba/assets/img/splash.mp4
--rw-r--r--   0 simon      (501) staff       (20)   322242 2023-04-06 16:38:51.000000 Simba-UW-tf-dev-1.58.7/simba/assets/img/bg_2.png
--rw-r--r--   0 simon      (501) staff       (20)    69267 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.7/simba/assets/img/splash.pptx
--rw-r--r--   0 simon      (501) staff       (20)   204362 2023-04-06 15:01:45.000000 Simba-UW-tf-dev-1.58.7/simba/assets/img/bg.png
--rw-r--r--   0 simon      (501) staff       (20)   189004 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.7/simba/assets/UbuntuMono-Regular.ttf
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-03 21:14:48.000000 Simba-UW-tf-dev-1.58.7/simba/assets/icons/
--rw-r--r--   0 simon      (501) staff       (20)     1350 2023-03-17 17:59:27.000000 Simba-UW-tf-dev-1.58.7/simba/assets/icons/factory.png
--rw-r--r--   0 simon      (501) staff       (20)     1413 2023-03-21 13:03:06.000000 Simba-UW-tf-dev-1.58.7/simba/assets/icons/cluster.png
--rw-r--r--   0 simon      (501) staff       (20)     1340 2023-03-17 16:51:08.000000 Simba-UW-tf-dev-1.58.7/simba/assets/icons/load.png
--rw-r--r--   0 simon      (501) staff       (20)     4507 2023-03-20 14:13:48.000000 Simba-UW-tf-dev-1.58.7/simba/assets/icons/gif.png
--rw-rw-r--   0 simon      (501) staff       (20)     4566 2023-03-18 18:12:27.000000 Simba-UW-tf-dev-1.58.7/simba/assets/icons/pose.png
--rw-rw-r--   0 simon      (501) staff       (20)     1943 2023-03-18 18:14:10.000000 Simba-UW-tf-dev-1.58.7/simba/assets/icons/features.png
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-04-05 17:25:36.000000 Simba-UW-tf-dev-1.58.7/simba/assets/icons/.DS_Store
--rw-rw-r--   0 simon      (501) staff       (20)     4896 2023-03-17 19:17:29.000000 Simba-UW-tf-dev-1.58.7/simba/assets/icons/settings.png
--rw-r--r--   0 simon      (501) staff       (20)     2090 2023-04-22 15:14:17.000000 Simba-UW-tf-dev-1.58.7/simba/assets/icons/stopwatch.png
--rw-r--r--   0 simon      (501) staff       (20)     1252 2023-03-19 16:48:40.000000 Simba-UW-tf-dev-1.58.7/simba/assets/icons/link.png
--rw-r--r--   0 simon      (501) staff       (20)    14250 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.7/simba/assets/icons/dash_simba.css
--rw-r--r--   0 simon      (501) staff       (20)      917 2023-04-05 16:43:13.000000 Simba-UW-tf-dev-1.58.7/simba/assets/icons/documentation.png
--rw-r--r--   0 simon      (501) staff       (20)     4503 2023-03-20 14:08:00.000000 Simba-UW-tf-dev-1.58.7/simba/assets/icons/fps.png
--rw-r--r--   0 simon      (501) staff       (20)     1299 2023-03-21 13:02:07.000000 Simba-UW-tf-dev-1.58.7/simba/assets/icons/dimensionality_reduction.png
--rw-rw-r--   0 simon      (501) staff       (20)     4823 2023-03-17 19:03:29.000000 Simba-UW-tf-dev-1.58.7/simba/assets/icons/roi.png
--rw-r--r--   0 simon      (501) staff       (20)      920 2023-03-20 14:25:03.000000 Simba-UW-tf-dev-1.58.7/simba/assets/icons/superimpose.png
--rw-r--r--   0 simon      (501) staff       (20)     1136 2023-03-18 20:25:31.000000 Simba-UW-tf-dev-1.58.7/simba/assets/icons/label.png
--rw-r--r--   0 simon      (501) staff       (20)     1016 2023-03-20 14:28:47.000000 Simba-UW-tf-dev-1.58.7/simba/assets/icons/change.png
--rw-r--r--   0 simon      (501) staff       (20)     1124 2023-03-17 18:05:26.000000 Simba-UW-tf-dev-1.58.7/simba/assets/icons/crop.png
--rw-r--r--   0 simon      (501) staff       (20)     2146 2023-04-13 14:09:23.000000 Simba-UW-tf-dev-1.58.7/simba/assets/icons/rotate.png
--rw-r--r--   0 simon      (501) staff       (20)     1057 2023-03-20 14:03:42.000000 Simba-UW-tf-dev-1.58.7/simba/assets/icons/path.png
--rw-r--r--   0 simon      (501) staff       (20)      950 2023-03-17 18:07:33.000000 Simba-UW-tf-dev-1.58.7/simba/assets/icons/clip.png
--rw-r--r--   0 simon      (501) staff       (20)     2121 2023-04-04 14:37:43.000000 Simba-UW-tf-dev-1.58.7/simba/assets/icons/restart.png
--rw-rw-r--   0 simon      (501) staff       (20)     4653 2023-03-17 18:11:59.000000 Simba-UW-tf-dev-1.58.7/simba/assets/icons/calipher.png
--rw-r--r--   0 simon      (501) staff       (20)     1291 2023-03-21 20:16:55.000000 Simba-UW-tf-dev-1.58.7/simba/assets/icons/add_on.png
--rw-rw-r--   0 simon      (501) staff       (20)     4695 2023-03-17 17:57:16.000000 Simba-UW-tf-dev-1.58.7/simba/assets/icons/create.png
--rw-r--r--   0 simon      (501) staff       (20)    78182 2023-03-20 16:35:36.000000 Simba-UW-tf-dev-1.58.7/simba/assets/icons/SimBA_logo.ico
--rw-r--r--   0 simon      (501) staff       (20)     1067 2023-03-20 14:22:44.000000 Simba-UW-tf-dev-1.58.7/simba/assets/icons/print.png
--rw-rw-r--   0 simon      (501) staff       (20)     4653 2023-03-18 20:27:58.000000 Simba-UW-tf-dev-1.58.7/simba/assets/icons/clf.png
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-03 21:14:48.000000 Simba-UW-tf-dev-1.58.7/simba/assets/icons/concat_icons/
--rw-r--r--   0 simon      (501) staff       (20)     6027 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.7/simba/assets/icons/concat_icons/mosaic.png
--rw-r--r--   0 simon      (501) staff       (20)     5654 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.7/simba/assets/icons/concat_icons/vertical.png
--rw-r--r--   0 simon      (501) staff       (20)     5542 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.7/simba/assets/icons/concat_icons/horizontal.png
--rw-r--r--   0 simon      (501) staff       (20)     5939 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.7/simba/assets/icons/concat_icons/mixed_mosaic.png
--rw-r--r--   0 simon      (501) staff       (20)     2060 2023-03-20 14:26:12.000000 Simba-UW-tf-dev-1.58.7/simba/assets/icons/merge.png
--rw-r--r--   0 simon      (501) staff       (20)     1252 2023-04-07 11:25:59.000000 Simba-UW-tf-dev-1.58.7/simba/assets/icons/clean.png
--rw-------   0 simon      (501) staff       (20)     4725 2023-03-18 20:27:47.000000 Simba-UW-tf-dev-1.58.7/simba/assets/icons/clf_2.png
--rw-rw-r--   0 simon      (501) staff       (20)     4795 2023-03-17 18:10:10.000000 Simba-UW-tf-dev-1.58.7/simba/assets/icons/visualize.png
--rw-r--r--   0 simon      (501) staff       (20)     2142 2023-03-20 14:10:28.000000 Simba-UW-tf-dev-1.58.7/simba/assets/icons/concat.png
--rw-r--r--   0 simon      (501) staff       (20)     1474 2023-03-17 19:20:24.000000 Simba-UW-tf-dev-1.58.7/simba/assets/icons/boris.png
--rw-rw-r--   0 simon      (501) staff       (20)     4804 2023-03-19 16:43:01.000000 Simba-UW-tf-dev-1.58.7/simba/assets/icons/frames.png
--rw-r--r--   0 simon      (501) staff       (20)     2425 2023-03-19 16:44:55.000000 Simba-UW-tf-dev-1.58.7/simba/assets/icons/video.png
--rw-r--r--   0 simon      (501) staff       (20)     2089 2023-03-20 14:05:58.000000 Simba-UW-tf-dev-1.58.7/simba/assets/icons/sample.png
--rw-r--r--   0 simon      (501) staff       (20)     1471 2023-03-21 13:04:02.000000 Simba-UW-tf-dev-1.58.7/simba/assets/icons/metrics.png
--rw-r--r--   0 simon      (501) staff       (20)     4555 2023-03-20 14:21:02.000000 Simba-UW-tf-dev-1.58.7/simba/assets/icons/grey.png
--rw-r--r--   0 simon      (501) staff       (20)      930 2023-03-18 18:07:29.000000 Simba-UW-tf-dev-1.58.7/simba/assets/icons/exit.png
--rw-r--r--   0 simon      (501) staff       (20)     4751 2023-03-18 20:31:58.000000 Simba-UW-tf-dev-1.58.7/simba/assets/icons/outlier.png
--rw-r--r--   0 simon      (501) staff       (20)     4392 2023-03-20 14:16:15.000000 Simba-UW-tf-dev-1.58.7/simba/assets/icons/clahe.png
--rw-rw-r--   0 simon      (501) staff       (20)     4637 2023-03-17 19:03:55.000000 Simba-UW-tf-dev-1.58.7/simba/assets/icons/trash.png
--rw-r--r--   0 simon      (501) staff       (20)     1239 2023-03-19 16:51:21.000000 Simba-UW-tf-dev-1.58.7/simba/assets/icons/about.png
--rw-rw-r--   0 simon      (501) staff       (20)     4666 2023-03-17 18:01:21.000000 Simba-UW-tf-dev-1.58.7/simba/assets/icons/convert.png
--rw-r--r--   0 simon      (501) staff       (20)    93229 2023-03-20 16:01:42.000000 Simba-UW-tf-dev-1.58.7/simba/assets/icons/SimBA_logo.icns
--rw-r--r--   0 simon      (501) staff       (20)      991 2023-03-20 19:02:33.000000 Simba-UW-tf-dev-1.58.7/simba/assets/icons/reorganize.png
--rw-rw-r--   0 simon      (501) staff       (20)     4784 2023-03-17 18:50:35.000000 Simba-UW-tf-dev-1.58.7/simba/assets/icons/browse.png
--rw-r--r--   0 simon      (501) staff       (20)    30707 2023-03-20 16:33:38.000000 Simba-UW-tf-dev-1.58.7/simba/assets/icons/SimBA_logo.png
--rw-r--r--   0 simon      (501) staff       (20)     2293 2023-03-17 19:24:38.000000 Simba-UW-tf-dev-1.58.7/simba/assets/icons/ethovision.png
--rw-r--r--   0 simon      (501) staff       (20)     1018 2023-04-05 15:24:49.000000 Simba-UW-tf-dev-1.58.7/simba/assets/icons/close.png
--rw-r--r--   0 simon      (501) staff       (20)    13672 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.7/simba/assets/dash_simba_base.css
--rw-r--r--   0 simon      (501) staff       (20)    31812 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.7/simba/assets/TheGoldenLab.PNG
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-03 21:14:48.000000 Simba-UW-tf-dev-1.58.7/Simba_UW_tf_dev.egg-info/
--rw-rw-r--   0 simon      (501) staff       (20)      579 2023-05-03 21:14:47.000000 Simba-UW-tf-dev-1.58.7/Simba_UW_tf_dev.egg-info/PKG-INFO
--rw-rw-r--   0 simon      (501) staff       (20)    18464 2023-05-03 21:14:48.000000 Simba-UW-tf-dev-1.58.7/Simba_UW_tf_dev.egg-info/SOURCES.txt
--rw-rw-r--   0 simon      (501) staff       (20)       44 2023-05-03 21:14:47.000000 Simba-UW-tf-dev-1.58.7/Simba_UW_tf_dev.egg-info/entry_points.txt
--rw-rw-r--   0 simon      (501) staff       (20)      639 2023-05-03 21:14:47.000000 Simba-UW-tf-dev-1.58.7/Simba_UW_tf_dev.egg-info/requires.txt
--rw-rw-r--   0 simon      (501) staff       (20)        6 2023-05-03 21:14:47.000000 Simba-UW-tf-dev-1.58.7/Simba_UW_tf_dev.egg-info/top_level.txt
--rw-rw-r--   0 simon      (501) staff       (20)        1 2023-05-03 21:14:47.000000 Simba-UW-tf-dev-1.58.7/Simba_UW_tf_dev.egg-info/dependency_links.txt
--rw-rw-r--   0 simon      (501) staff       (20)     7652 2020-05-13 13:27:38.000000 Simba-UW-tf-dev-1.58.7/LICENSE.md
--rw-rw-r--   0 simon      (501) staff       (20)      136 2021-04-10 10:44:06.000000 Simba-UW-tf-dev-1.58.7/MANIFEST.in
--rw-rw-r--   0 simon      (501) staff       (20)     9598 2020-05-13 13:27:40.000000 Simba-UW-tf-dev-1.58.7/README.md
--rw-rw-r--   0 simon      (501) staff       (20)     1897 2023-05-03 21:12:42.000000 Simba-UW-tf-dev-1.58.7/setup.py
--rw-r--r--   0 simon      (501) staff       (20)       38 2023-05-03 21:14:48.000000 Simba-UW-tf-dev-1.58.7/setup.cfg
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-04 20:00:38.000000 Simba-UW-tf-dev-1.58.8/
+-rw-r--r--   0 simon      (501) staff       (20)      579 2023-05-04 20:00:38.000000 Simba-UW-tf-dev-1.58.8/PKG-INFO
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-04 20:00:38.000000 Simba-UW-tf-dev-1.58.8/simba/
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-04 20:00:38.000000 Simba-UW-tf-dev-1.58.8/simba/ui/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-05-03 18:36:16.000000 Simba-UW-tf-dev-1.58.8/simba/ui/.DS_Store
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-04 20:00:38.000000 Simba-UW-tf-dev-1.58.8/simba/ui/pop_ups/
+-rw-r--r--   0 simon      (501) staff       (20)     3463 2023-05-04 17:49:06.000000 Simba-UW-tf-dev-1.58.8/simba/ui/pop_ups/movement_analysis_time_bins_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     1431 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.58.8/simba/ui/pop_ups/csv_2_parquet_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     2310 2023-04-29 15:00:50.000000 Simba-UW-tf-dev-1.58.8/simba/ui/pop_ups/quick_path_plot_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     2332 2023-04-29 18:13:54.000000 Simba-UW-tf-dev-1.58.8/simba/ui/pop_ups/batch_preprocess_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     8366 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.58.8/simba/ui/pop_ups/heatmap_location_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     9302 2023-05-04 15:16:51.000000 Simba-UW-tf-dev-1.58.8/simba/ui/pop_ups/clf_probability_plot_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-04-29 16:41:16.000000 Simba-UW-tf-dev-1.58.8/simba/ui/pop_ups/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)     3143 2023-05-03 16:24:11.000000 Simba-UW-tf-dev-1.58.8/simba/ui/pop_ups/movement_analysis_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     3657 2023-04-29 19:37:54.000000 Simba-UW-tf-dev-1.58.8/simba/ui/pop_ups/set_machine_model_parameters_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     9494 2023-04-29 15:00:50.000000 Simba-UW-tf-dev-1.58.8/simba/ui/pop_ups/clf_plot_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)    15044 2023-05-03 21:12:42.000000 Simba-UW-tf-dev-1.58.8/simba/ui/pop_ups/path_plot_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     3024 2023-04-29 16:24:52.000000 Simba-UW-tf-dev-1.58.8/simba/ui/pop_ups/smoothing_interpolation_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     4798 2023-04-29 18:54:24.000000 Simba-UW-tf-dev-1.58.8/simba/ui/pop_ups/visualize_pose_in_dir_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     3551 2023-05-03 16:20:49.000000 Simba-UW-tf-dev-1.58.8/simba/ui/pop_ups/roi_analysis_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     5873 2023-04-29 16:24:52.000000 Simba-UW-tf-dev-1.58.8/simba/ui/pop_ups/outlier_settings_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     8296 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.58.8/simba/ui/pop_ups/gantt_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     5726 2023-05-01 12:04:35.000000 Simba-UW-tf-dev-1.58.8/simba/ui/pop_ups/clf_validation_plot_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     3301 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.58.8/simba/ui/pop_ups/severity_analysis_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     2779 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.58.8/simba/ui/pop_ups/fsttc_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     4066 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.58.8/simba/ui/pop_ups/kleinberg_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     7288 2023-04-29 15:00:50.000000 Simba-UW-tf-dev-1.58.8/simba/ui/pop_ups/directing_other_animals_plot_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     5463 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.58.8/simba/ui/pop_ups/pose_reorganizer_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     2411 2023-05-03 16:35:10.000000 Simba-UW-tf-dev-1.58.8/simba/ui/pop_ups/append_roi_features_animals_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     3251 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.58.8/simba/ui/pop_ups/clf_by_timebins_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     8697 2023-04-29 15:00:50.000000 Simba-UW-tf-dev-1.58.8/simba/ui/pop_ups/heatmap_clf_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     7688 2023-04-29 15:00:50.000000 Simba-UW-tf-dev-1.58.8/simba/ui/pop_ups/data_plot_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     7928 2023-04-29 15:00:50.000000 Simba-UW-tf-dev-1.58.8/simba/ui/pop_ups/roi_features_plot_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     8363 2023-04-29 19:49:16.000000 Simba-UW-tf-dev-1.58.8/simba/ui/pop_ups/pup_retrieval_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)      579 2023-04-29 18:12:37.000000 Simba-UW-tf-dev-1.58.8/simba/ui/pop_ups/about_simba_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     2544 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.58.8/simba/ui/pop_ups/clf_descriptive_statistics_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     6409 2023-04-29 15:00:50.000000 Simba-UW-tf-dev-1.58.8/simba/ui/pop_ups/roi_tracking_plot_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     1468 2023-04-29 16:24:52.000000 Simba-UW-tf-dev-1.58.8/simba/ui/pop_ups/append_roi_features_bodypart_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     5318 2023-04-29 19:01:32.000000 Simba-UW-tf-dev-1.58.8/simba/ui/pop_ups/clf_add_remove_print_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)    42478 2023-04-29 18:56:08.000000 Simba-UW-tf-dev-1.58.8/simba/ui/pop_ups/video_processing_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     7536 2023-04-29 15:00:50.000000 Simba-UW-tf-dev-1.58.8/simba/ui/pop_ups/validation_plot_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     5255 2023-05-04 18:22:44.000000 Simba-UW-tf-dev-1.58.8/simba/ui/pop_ups/clf_by_roi_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     2840 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.58.8/simba/ui/pop_ups/make_path_plot_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     5406 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.58.8/simba/ui/pop_ups/create_user_defined_pose_configuration_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     1065 2023-04-29 16:24:52.000000 Simba-UW-tf-dev-1.58.8/simba/ui/pop_ups/archive_files_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     4098 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.58.8/simba/ui/pop_ups/pose_bp_drop_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)    10712 2023-04-29 15:00:50.000000 Simba-UW-tf-dev-1.58.8/simba/ui/pop_ups/distance_plot_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     2567 2023-04-29 16:24:52.000000 Simba-UW-tf-dev-1.58.8/simba/ui/pop_ups/subset_feature_extractor_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     3114 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.58.8/simba/ui/pop_ups/third_party_annotator_appender_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     3193 2023-05-04 18:50:54.000000 Simba-UW-tf-dev-1.58.8/simba/ui/pop_ups/roi_analysis_time_bins_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)    12626 2023-05-04 14:03:25.000000 Simba-UW-tf-dev-1.58.8/simba/ui/video_info_ui.py
+-rw-r--r--   0 simon      (501) staff       (20)     6032 2023-05-04 14:03:25.000000 Simba-UW-tf-dev-1.58.8/simba/ui/user_defined_pose_creator.py
+-rw-r--r--   0 simon      (501) staff       (20)    12788 2023-05-01 23:51:03.000000 Simba-UW-tf-dev-1.58.8/simba/ui/create_project_ui.py
+-rw-r--r--   0 simon      (501) staff       (20)    10957 2023-05-04 14:03:25.000000 Simba-UW-tf-dev-1.58.8/simba/ui/tkinter_functions.py
+-rw-r--r--   0 simon      (501) staff       (20)    33955 2023-05-04 19:55:21.000000 Simba-UW-tf-dev-1.58.8/simba/ui/machine_model_settings_ui.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-04 20:00:38.000000 Simba-UW-tf-dev-1.58.8/simba/blob_storage/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-21 20:39:46.000000 Simba-UW-tf-dev-1.58.8/simba/blob_storage/.DS_Store
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-04 20:00:38.000000 Simba-UW-tf-dev-1.58.8/simba/labelling/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-04-28 20:24:21.000000 Simba-UW-tf-dev-1.58.8/simba/labelling/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)    20790 2023-05-04 17:45:45.000000 Simba-UW-tf-dev-1.58.8/simba/labelling/labelling_interface.py
+-rw-r--r--   0 simon      (501) staff       (20)     3466 2023-05-04 14:03:25.000000 Simba-UW-tf-dev-1.58.8/simba/labelling/extract_labelled_frames.py
+-rw-r--r--   0 simon      (501) staff       (20)    26652 2023-04-29 19:43:53.000000 Simba-UW-tf-dev-1.58.8/simba/labelling/labelling_advanced_interface.py
+-rw-r--r--   0 simon      (501) staff       (20)     6543 2023-04-27 19:42:17.000000 Simba-UW-tf-dev-1.58.8/simba/labelling/play_annotation_video.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-04 20:00:38.000000 Simba-UW-tf-dev-1.58.8/simba/unsupervised/
+-rw-r--r--   0 simon      (501) staff       (20)    11932 2023-04-27 20:23:35.000000 Simba-UW-tf-dev-1.58.8/simba/unsupervised/dbcv_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)     3375 2023-05-02 18:14:28.000000 Simba-UW-tf-dev-1.58.8/simba/unsupervised/enums.py
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-04-23 19:55:32.000000 Simba-UW-tf-dev-1.58.8/simba/unsupervised/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)     8187 2023-04-28 13:09:30.000000 Simba-UW-tf-dev-1.58.8/simba/unsupervised/dataset_creator.py
+-rw-r--r--   0 simon      (501) staff       (20)     5693 2023-04-28 13:09:30.000000 Simba-UW-tf-dev-1.58.8/simba/unsupervised/grid_search_visualizers.py
+-rw-r--r--   0 simon      (501) staff       (20)     7268 2023-04-28 12:30:12.000000 Simba-UW-tf-dev-1.58.8/simba/unsupervised/data_extractor.py
+-rw-r--r--   0 simon      (501) staff       (20)     9910 2023-05-02 18:14:28.000000 Simba-UW-tf-dev-1.58.8/simba/unsupervised/ui.py
+-rw-r--r--   0 simon      (501) staff       (20)     9915 2023-04-28 13:09:30.000000 Simba-UW-tf-dev-1.58.8/simba/unsupervised/umap_embedder.py
+-rw-r--r--   0 simon      (501) staff       (20)    41323 2023-05-02 18:14:28.000000 Simba-UW-tf-dev-1.58.8/simba/unsupervised/pop_up_classes.py
+-rw-r--r--   0 simon      (501) staff       (20)     2347 2023-04-28 12:22:34.000000 Simba-UW-tf-dev-1.58.8/simba/unsupervised/bout_aggregator.py
+-rw-r--r--   0 simon      (501) staff       (20)    20886 2023-04-28 19:59:05.000000 Simba-UW-tf-dev-1.58.8/simba/unsupervised/cluster_statistics.py
+-rw-r--r--   0 simon      (501) staff       (20)     2188 2023-04-18 23:25:29.000000 Simba-UW-tf-dev-1.58.8/simba/unsupervised/data_map.yaml
+-rw-r--r--   0 simon      (501) staff       (20)    10289 2023-04-28 13:09:30.000000 Simba-UW-tf-dev-1.58.8/simba/unsupervised/hdbscan_clusterer.py
+-rw-r--r--   0 simon      (501) staff       (20)     3937 2023-04-28 19:59:05.000000 Simba-UW-tf-dev-1.58.8/simba/unsupervised/tsne.py
+-rw-r--r--   0 simon      (501) staff       (20)     6698 2023-04-28 19:59:05.000000 Simba-UW-tf-dev-1.58.8/simba/unsupervised/cluster_visualizer.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-04 20:00:38.000000 Simba-UW-tf-dev-1.58.8/simba/bounding_box_tools/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.8/simba/bounding_box_tools/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)     6791 2023-05-04 15:16:51.000000 Simba-UW-tf-dev-1.58.8/simba/bounding_box_tools/agg_boundary_stats.py
+-rw-r--r--   0 simon      (501) staff       (20)    23590 2023-04-28 20:48:50.000000 Simba-UW-tf-dev-1.58.8/simba/bounding_box_tools/boundary_menus.py
+-rw-r--r--   0 simon      (501) staff       (20)     8521 2023-04-28 19:59:05.000000 Simba-UW-tf-dev-1.58.8/simba/bounding_box_tools/boundary_statistics.py
+-rw-r--r--   0 simon      (501) staff       (20)     6067 2023-04-27 20:23:35.000000 Simba-UW-tf-dev-1.58.8/simba/bounding_box_tools/find_boundaries.py
+-rw-r--r--   0 simon      (501) staff       (20)    11228 2023-04-28 00:28:29.000000 Simba-UW-tf-dev-1.58.8/simba/bounding_box_tools/visualize_boundaries.py
+-rw-r--r--   0 simon      (501) staff       (20)    43012 2023-05-03 18:35:59.000000 Simba-UW-tf-dev-1.58.8/simba/.DS_Store
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-04 20:00:38.000000 Simba-UW-tf-dev-1.58.8/simba/feature_extractors/
+-rw-r--r--   0 simon      (501) staff       (20)    42323 2023-04-28 19:59:05.000000 Simba-UW-tf-dev-1.58.8/simba/feature_extractors/feature_extractor_14bp.py
+-rw-r--r--   0 simon      (501) staff       (20)    21427 2023-04-28 15:16:26.000000 Simba-UW-tf-dev-1.58.8/simba/feature_extractors/feature_extractor_7bp.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-04 20:00:38.000000 Simba-UW-tf-dev-1.58.8/simba/feature_extractors/misc/
+-rw-r--r--   0 simon      (501) staff       (20)     1685 2023-04-14 17:52:01.000000 Simba-UW-tf-dev-1.58.8/simba/feature_extractors/misc/doctests.py
+-rw-r--r--   0 simon      (501) staff       (20)    23850 2023-04-17 18:48:40.000000 Simba-UW-tf-dev-1.58.8/simba/feature_extractors/misc/fish_feature_extractor_2023_version_3.py
+-rw-r--r--   0 simon      (501) staff       (20)     2732 2023-04-04 19:46:36.000000 Simba-UW-tf-dev-1.58.8/simba/feature_extractors/misc/read_in_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)     2460 2023-04-22 18:02:29.000000 Simba-UW-tf-dev-1.58.8/simba/feature_extractors/misc/peaks.py
+-rw-r--r--   0 simon      (501) staff       (20)    14141 2023-03-15 17:20:08.000000 Simba-UW-tf-dev-1.58.8/simba/feature_extractors/misc/fish_feature_extractor_2022.py
+-rw-r--r--   0 simon      (501) staff       (20)     2053 2023-04-04 03:00:41.000000 Simba-UW-tf-dev-1.58.8/simba/feature_extractors/misc/convex_hull_3_scratch_3.py
+-rw-r--r--   0 simon      (501) staff       (20)     5762 2023-04-04 01:54:33.000000 Simba-UW-tf-dev-1.58.8/simba/feature_extractors/misc/convex_hull_scratch_1.py
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-14 19:36:02.000000 Simba-UW-tf-dev-1.58.8/simba/feature_extractors/misc/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)    21398 2023-04-16 17:03:37.000000 Simba-UW-tf-dev-1.58.8/simba/feature_extractors/misc/fish_feature_extractor_2023_version_2.py
+-rw-r--r--   0 simon      (501) staff       (20)     7127 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.8/simba/feature_extractors/misc/egocentrical_aligner.py
+-rw-r--r--   0 simon      (501) staff       (20)     1213 2023-04-11 20:12:47.000000 Simba-UW-tf-dev-1.58.8/simba/feature_extractors/misc/count_values_in_range.py
+-rw-r--r--   0 simon      (501) staff       (20)     4708 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.8/simba/feature_extractors/misc/graph_creator.py
+-rw-r--r--   0 simon      (501) staff       (20)     3954 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.8/simba/feature_extractors/misc/termite_rois.csv
+-rw-r--r--   0 simon      (501) staff       (20)      732 2023-03-20 12:13:51.000000 Simba-UW-tf-dev-1.58.8/simba/feature_extractors/misc/mutual_exclusive.py
+-rw-r--r--   0 simon      (501) staff       (20)     2841 2023-04-14 15:16:23.000000 Simba-UW-tf-dev-1.58.8/simba/feature_extractors/misc/video_color.py
+-rw-r--r--   0 simon      (501) staff       (20)     1862 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.8/simba/feature_extractors/misc/graph_3d_plotter.py
+-rw-r--r--   0 simon      (501) staff       (20)     5232 2023-04-13 14:05:29.000000 Simba-UW-tf-dev-1.58.8/simba/feature_extractors/misc/video_rotator.py
+-rw-r--r--   0 simon      (501) staff       (20)     2692 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.8/simba/feature_extractors/misc/add_probability_cnt_features.py
+-rw-r--r--   0 simon      (501) staff       (20)     1619 2023-04-08 20:02:08.000000 Simba-UW-tf-dev-1.58.8/simba/feature_extractors/misc/make_splash.py
+-rw-r--r--   0 simon      (501) staff       (20)     1658 2023-04-22 19:16:28.000000 Simba-UW-tf-dev-1.58.8/simba/feature_extractors/misc/time_stamp_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)     5232 2023-04-15 19:24:18.000000 Simba-UW-tf-dev-1.58.8/simba/feature_extractors/misc/video_rotator_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)    30677 2023-04-27 01:57:28.000000 Simba-UW-tf-dev-1.58.8/simba/feature_extractors/misc/fish_feature_extractor_2023_version_4.py
+-rw-r--r--   0 simon      (501) staff       (20)     2058 2023-04-03 23:51:37.000000 Simba-UW-tf-dev-1.58.8/simba/feature_extractors/misc/convex_hull_scratch_2.py
+-rw-r--r--   0 simon      (501) staff       (20)    27783 2023-04-28 19:59:05.000000 Simba-UW-tf-dev-1.58.8/simba/feature_extractors/feature_extractor_8bps_2_animals.py
+-rw-r--r--   0 simon      (501) staff       (20)    10244 2023-04-25 21:03:39.000000 Simba-UW-tf-dev-1.58.8/simba/feature_extractors/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)     3491 2023-05-03 13:59:23.000000 Simba-UW-tf-dev-1.58.8/simba/feature_extractors/perimeter_jit.py
+-rw-r--r--   0 simon      (501) staff       (20)    13322 2023-04-28 19:59:05.000000 Simba-UW-tf-dev-1.58.8/simba/feature_extractors/feature_subsets.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.8/simba/feature_extractors/__init__.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-04 20:00:38.000000 Simba-UW-tf-dev-1.58.8/simba/feature_extractors/__pycache__/
+-rw-r--r--   0 simon      (501) staff       (20)      905 2023-04-04 11:31:57.000000 Simba-UW-tf-dev-1.58.8/simba/feature_extractors/__pycache__/perimeter_jit.quickhull_2d-16.py36m.nbi
+-rw-r--r--   0 simon      (501) staff       (20)   238196 2023-04-04 11:31:57.000000 Simba-UW-tf-dev-1.58.8/simba/feature_extractors/__pycache__/perimeter_jit.quickhull_2d-16.py36m.1.nbc
+-rw-r--r--   0 simon      (501) staff       (20)    69038 2023-04-04 11:32:25.000000 Simba-UW-tf-dev-1.58.8/simba/feature_extractors/__pycache__/perimeter_jit.process-7.py36m.1.nbc
+-rw-r--r--   0 simon      (501) staff       (20)   238298 2023-04-04 11:32:29.000000 Simba-UW-tf-dev-1.58.8/simba/feature_extractors/__pycache__/perimeter_jit.convex_hull_perimeter_2d-16.py36m.1.nbc
+-rw-r--r--   0 simon      (501) staff       (20)    69338 2023-04-04 11:32:26.000000 Simba-UW-tf-dev-1.58.8/simba/feature_extractors/__pycache__/perimeter_jit.process-7.py36m.2.nbc
+-rw-r--r--   0 simon      (501) staff       (20)      917 2023-04-04 11:32:29.000000 Simba-UW-tf-dev-1.58.8/simba/feature_extractors/__pycache__/perimeter_jit.convex_hull_perimeter_2d-16.py36m.nbi
+-rw-r--r--   0 simon      (501) staff       (20)     2179 2023-04-04 11:32:26.000000 Simba-UW-tf-dev-1.58.8/simba/feature_extractors/__pycache__/perimeter_jit.process-7.py36m.nbi
+-rw-r--r--   0 simon      (501) staff       (20)     8282 2023-04-27 20:23:35.000000 Simba-UW-tf-dev-1.58.8/simba/feature_extractors/feature_extractor_user_defined.py
+-rw-r--r--   0 simon      (501) staff       (20)    46269 2023-04-28 19:59:05.000000 Simba-UW-tf-dev-1.58.8/simba/feature_extractors/feature_extractor_16bp.py
+-rw-r--r--   0 simon      (501) staff       (20)    28134 2023-04-28 18:40:57.000000 Simba-UW-tf-dev-1.58.8/simba/feature_extractors/feature_extractor_9bp.py
+-rw-r--r--   0 simon      (501) staff       (20)    23897 2023-04-28 19:59:05.000000 Simba-UW-tf-dev-1.58.8/simba/feature_extractors/feature_extractor_8bp.py
+-rw-r--r--   0 simon      (501) staff       (20)    16825 2023-04-27 20:23:35.000000 Simba-UW-tf-dev-1.58.8/simba/feature_extractors/feature_extractor_4bp.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-04 20:00:38.000000 Simba-UW-tf-dev-1.58.8/simba/feature_extractors/.idea/
+-rw-r--r--   0 simon      (501) staff       (20)      617 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.8/simba/feature_extractors/.idea/features_scripts.iml
+-rw-r--r--   0 simon      (501) staff       (20)      138 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.8/simba/feature_extractors/.idea/encodings.xml
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-04 20:00:38.000000 Simba-UW-tf-dev-1.58.8/simba/feature_extractors/.idea/inspectionProfiles/
+-rw-r--r--   0 simon      (501) staff       (20)      822 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.8/simba/feature_extractors/.idea/inspectionProfiles/Project_Default.xml
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-04 20:00:38.000000 Simba-UW-tf-dev-1.58.8/simba/feature_extractors/.idea/libraries/
+-rw-r--r--   0 simon      (501) staff       (20)      128 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.8/simba/feature_extractors/.idea/libraries/R_User_Library.xml
+-rw-r--r--   0 simon      (501) staff       (20)      273 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.8/simba/feature_extractors/.idea/.gitignore
+-rw-r--r--   0 simon      (501) staff       (20)     8081 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.8/simba/feature_extractors/.idea/workspace.xml
+-rw-r--r--   0 simon      (501) staff       (20)      291 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.8/simba/feature_extractors/.idea/modules.xml
+-rw-r--r--   0 simon      (501) staff       (20)       23 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.8/simba/feature_extractors/.idea/.name
+-rw-r--r--   0 simon      (501) staff       (20)      294 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.8/simba/feature_extractors/.idea/misc.xml
+-rw-r--r--   0 simon      (501) staff       (20)    15449 2023-04-30 14:02:53.000000 Simba-UW-tf-dev-1.58.8/simba/requirements.txt
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-04 20:00:38.000000 Simba-UW-tf-dev-1.58.8/simba/mixins/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-15 17:26:03.000000 Simba-UW-tf-dev-1.58.8/simba/mixins/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)    41772 2023-05-03 16:41:23.000000 Simba-UW-tf-dev-1.58.8/simba/mixins/pop_up_mixin.py
+-rw-r--r--   0 simon      (501) staff       (20)    29306 2023-04-29 19:43:53.000000 Simba-UW-tf-dev-1.58.8/simba/mixins/config_reader.py
+-rw-r--r--   0 simon      (501) staff       (20)    17367 2023-05-01 18:54:03.000000 Simba-UW-tf-dev-1.58.8/simba/mixins/pose_importer_mixin.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-04 20:00:38.000000 Simba-UW-tf-dev-1.58.8/simba/mixins/__pycache__/
+-rw-r--r--   0 simon      (501) staff       (20)     1223 2023-04-25 20:46:51.000000 Simba-UW-tf-dev-1.58.8/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-182.py36m.nbi
+-rw-r--r--   0 simon      (501) staff       (20)    49894 2023-04-24 19:51:34.000000 Simba-UW-tf-dev-1.58.8/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-183.py36m.1.nbc
+-rw-r--r--   0 simon      (501) staff       (20)     1223 2023-04-29 19:21:39.000000 Simba-UW-tf-dev-1.58.8/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-190.py36m.nbi
+-rw-r--r--   0 simon      (501) staff       (20)    49963 2023-04-29 19:21:39.000000 Simba-UW-tf-dev-1.58.8/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-190.py36m.1.nbc
+-rw-r--r--   0 simon      (501) staff       (20)     1223 2023-04-24 19:51:34.000000 Simba-UW-tf-dev-1.58.8/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-183.py36m.nbi
+-rw-r--r--   0 simon      (501) staff       (20)    49894 2023-04-25 20:46:51.000000 Simba-UW-tf-dev-1.58.8/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-182.py36m.1.nbc
+-rw-r--r--   0 simon      (501) staff       (20)    49894 2023-04-24 19:06:57.000000 Simba-UW-tf-dev-1.58.8/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-181.py36m.1.nbc
+-rw-r--r--   0 simon      (501) staff       (20)     1223 2023-04-24 19:06:57.000000 Simba-UW-tf-dev-1.58.8/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-181.py36m.nbi
+-rw-r--r--   0 simon      (501) staff       (20)    23591 2023-05-04 16:32:32.000000 Simba-UW-tf-dev-1.58.8/simba/mixins/feature_extraction_mixin.py
+-rw-r--r--   0 simon      (501) staff       (20)    60449 2023-05-03 18:46:32.000000 Simba-UW-tf-dev-1.58.8/simba/mixins/plotting_mixin.py
+-rw-r--r--   0 simon      (501) staff       (20)     6175 2023-05-02 18:14:28.000000 Simba-UW-tf-dev-1.58.8/simba/mixins/unsupervised_mixin.py
+-rw-r--r--   0 simon      (501) staff       (20)    55362 2023-05-01 20:52:34.000000 Simba-UW-tf-dev-1.58.8/simba/mixins/train_model_mixin.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-04 20:00:38.000000 Simba-UW-tf-dev-1.58.8/simba/third_party_label_appenders/
+-rw-r--r--   0 simon      (501) staff       (20)     6228 2023-04-26 18:27:58.000000 Simba-UW-tf-dev-1.58.8/simba/third_party_label_appenders/deepethogram_importer.py
+-rw-r--r--   0 simon      (501) staff       (20)     9945 2023-04-25 01:50:43.000000 Simba-UW-tf-dev-1.58.8/simba/third_party_label_appenders/BORIS_appender.py
+-rw-r--r--   0 simon      (501) staff       (20)     9063 2023-04-25 01:50:43.000000 Simba-UW-tf-dev-1.58.8/simba/third_party_label_appenders/observer_importer.py
+-rw-r--r--   0 simon      (501) staff       (20)    17166 2023-05-04 17:44:05.000000 Simba-UW-tf-dev-1.58.8/simba/third_party_label_appenders/tools.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-04-01 14:10:06.000000 Simba-UW-tf-dev-1.58.8/simba/third_party_label_appenders/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)    18248 2023-04-28 19:59:05.000000 Simba-UW-tf-dev-1.58.8/simba/third_party_label_appenders/third_party_appender.py
+-rw-r--r--   0 simon      (501) staff       (20)     8173 2023-04-27 19:42:17.000000 Simba-UW-tf-dev-1.58.8/simba/third_party_label_appenders/ethovision_import.py
+-rw-r--r--   0 simon      (501) staff       (20)     6858 2023-05-04 15:35:50.000000 Simba-UW-tf-dev-1.58.8/simba/third_party_label_appenders/BENTO_appender.py
+-rw-r--r--   0 simon      (501) staff       (20)     5331 2023-04-25 01:50:43.000000 Simba-UW-tf-dev-1.58.8/simba/third_party_label_appenders/solomon_importer.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-04 20:00:38.000000 Simba-UW-tf-dev-1.58.8/simba/cue_light_tools/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-15 17:25:58.000000 Simba-UW-tf-dev-1.58.8/simba/cue_light_tools/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)     7594 2023-05-01 19:38:38.000000 Simba-UW-tf-dev-1.58.8/simba/cue_light_tools/cue_light_clf_statistics.py
+-rw-r--r--   0 simon      (501) staff       (20)    12195 2023-05-04 14:18:28.000000 Simba-UW-tf-dev-1.58.8/simba/cue_light_tools/cue_light_analyzer.py
+-rw-r--r--   0 simon      (501) staff       (20)    16737 2023-05-01 19:58:28.000000 Simba-UW-tf-dev-1.58.8/simba/cue_light_tools/cue_light_menues.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.8/simba/cue_light_tools/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)     1690 2023-04-27 20:23:35.000000 Simba-UW-tf-dev-1.58.8/simba/cue_light_tools/cue_light_tools.py
+-rw-r--r--   0 simon      (501) staff       (20)    15289 2023-05-01 19:38:38.000000 Simba-UW-tf-dev-1.58.8/simba/cue_light_tools/cue_light_visualizer.py
+-rw-r--r--   0 simon      (501) staff       (20)    12615 2023-05-01 19:51:32.000000 Simba-UW-tf-dev-1.58.8/simba/cue_light_tools/cue_light_movement_statistics.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.8/simba/__init__.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-04 20:00:38.000000 Simba-UW-tf-dev-1.58.8/simba/utils/
+-rw-r--r--   0 simon      (501) staff       (20)    11617 2023-05-04 13:26:06.000000 Simba-UW-tf-dev-1.58.8/simba/utils/config_creator.py
+-rw-r--r--   0 simon      (501) staff       (20)    20258 2023-05-03 16:24:11.000000 Simba-UW-tf-dev-1.58.8/simba/utils/enums.py
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-14 20:15:03.000000 Simba-UW-tf-dev-1.58.8/simba/utils/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)     7365 2023-04-27 20:23:35.000000 Simba-UW-tf-dev-1.58.8/simba/utils/warnings.py
+-rw-r--r--   0 simon      (501) staff       (20)     5837 2023-05-04 15:35:50.000000 Simba-UW-tf-dev-1.58.8/simba/utils/checks.py
+-rw-r--r--   0 simon      (501) staff       (20)    34295 2023-05-04 19:36:13.000000 Simba-UW-tf-dev-1.58.8/simba/utils/read_write.py
+-rw-r--r--   0 simon      (501) staff       (20)     7034 2023-04-28 19:59:05.000000 Simba-UW-tf-dev-1.58.8/simba/utils/lookups.py
+-rw-r--r--   0 simon      (501) staff       (20)    14666 2023-04-28 19:59:06.000000 Simba-UW-tf-dev-1.58.8/simba/utils/errors.py
+-rw-r--r--   0 simon      (501) staff       (20)    14109 2023-05-04 13:26:06.000000 Simba-UW-tf-dev-1.58.8/simba/utils/data.py
+-rw-r--r--   0 simon      (501) staff       (20)     1573 2023-04-29 19:08:53.000000 Simba-UW-tf-dev-1.58.8/simba/utils/printing.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-04 20:00:38.000000 Simba-UW-tf-dev-1.58.8/simba/pose_processors/
+-rw-r--r--   0 simon      (501) staff       (20)     8385 2023-05-04 15:35:50.000000 Simba-UW-tf-dev-1.58.8/simba/pose_processors/reorganize_keypoint.py
+-rw-r--r--   0 simon      (501) staff       (20)     5223 2023-04-27 20:23:35.000000 Simba-UW-tf-dev-1.58.8/simba/pose_processors/remove_keypoints.py
+-rw-r--r--   0 simon      (501) staff       (20)     2641 2023-05-04 14:03:25.000000 Simba-UW-tf-dev-1.58.8/simba/pose_processors/pose_reset.py
+-rw-r--r--   0 simon      (501) staff       (20)     5614 2023-05-04 15:35:50.000000 Simba-UW-tf-dev-1.58.8/simba/pose_processors/reverse_pose.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-04 20:00:38.000000 Simba-UW-tf-dev-1.58.8/simba/plotting/
+-rw-r--r--   0 simon      (501) staff       (20)     9140 2023-05-04 15:02:11.000000 Simba-UW-tf-dev-1.58.8/simba/plotting/gantt_creator.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-04 20:00:38.000000 Simba-UW-tf-dev-1.58.8/simba/plotting/tools/
+-rw-r--r--   0 simon      (501) staff       (20)     5388 2023-04-27 20:23:35.000000 Simba-UW-tf-dev-1.58.8/simba/plotting/tools/tkinter_tools.py
+-rw-r--r--   0 simon      (501) staff       (20)    13238 2023-04-30 15:54:10.000000 Simba-UW-tf-dev-1.58.8/simba/plotting/ROI_plotter_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-04-25 23:35:57.000000 Simba-UW-tf-dev-1.58.8/simba/plotting/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)    14636 2023-04-28 19:59:05.000000 Simba-UW-tf-dev-1.58.8/simba/plotting/shap_agg_stats_visualizer.py
+-rw-r--r--   0 simon      (501) staff       (20)    10199 2023-05-04 15:02:11.000000 Simba-UW-tf-dev-1.58.8/simba/plotting/gantt_creator_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)    15981 2023-04-28 19:59:05.000000 Simba-UW-tf-dev-1.58.8/simba/plotting/heat_mapper_clf_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)     8571 2023-05-04 15:16:51.000000 Simba-UW-tf-dev-1.58.8/simba/plotting/probability_plot_creator.py
+-rw-r--r--   0 simon      (501) staff       (20)    12404 2023-05-04 15:35:50.000000 Simba-UW-tf-dev-1.58.8/simba/plotting/plot_clf_results.py
+-rw-r--r--   0 simon      (501) staff       (20)    15216 2023-05-04 15:35:50.000000 Simba-UW-tf-dev-1.58.8/simba/plotting/plot_clf_results_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)    15872 2023-05-04 15:16:51.000000 Simba-UW-tf-dev-1.58.8/simba/plotting/ROI_feature_visualizer.py
+-rw-r--r--   0 simon      (501) staff       (20)    12739 2023-04-28 19:59:05.000000 Simba-UW-tf-dev-1.58.8/simba/plotting/heat_mapper_location.py
+-rw-r--r--   0 simon      (501) staff       (20)    10168 2023-05-04 15:16:51.000000 Simba-UW-tf-dev-1.58.8/simba/plotting/probability_plot_creator_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)     5232 2023-04-28 19:59:05.000000 Simba-UW-tf-dev-1.58.8/simba/plotting/interactive_probability_grapher.py
+-rw-r--r--   0 simon      (501) staff       (20)     5834 2023-05-04 15:35:50.000000 Simba-UW-tf-dev-1.58.8/simba/plotting/plot_pose_in_dir.py
+-rw-r--r--   0 simon      (501) staff       (20)    12806 2023-05-04 15:16:51.000000 Simba-UW-tf-dev-1.58.8/simba/plotting/single_run_model_validation_video.py
+-rw-r--r--   0 simon      (501) staff       (20)    12434 2023-05-04 17:45:23.000000 Simba-UW-tf-dev-1.58.8/simba/plotting/frame_mergerer_ffmpeg.py
+-rw-r--r--   0 simon      (501) staff       (20)     7917 2023-04-28 19:59:05.000000 Simba-UW-tf-dev-1.58.8/simba/plotting/Directing_animals_visualizer_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)    11263 2023-05-04 15:02:11.000000 Simba-UW-tf-dev-1.58.8/simba/plotting/clf_validator.py
+-rw-r--r--   0 simon      (501) staff       (20)    15234 2023-05-04 15:35:50.000000 Simba-UW-tf-dev-1.58.8/simba/plotting/path_plotter_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)    11330 2023-04-28 19:59:05.000000 Simba-UW-tf-dev-1.58.8/simba/plotting/ROI_feature_visualizer_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)     9514 2023-05-04 15:02:11.000000 Simba-UW-tf-dev-1.58.8/simba/plotting/data_plotter.py
+-rw-r--r--   0 simon      (501) staff       (20)    13232 2023-05-03 18:58:48.000000 Simba-UW-tf-dev-1.58.8/simba/plotting/path_plotter.py
+-rw-r--r--   0 simon      (501) staff       (20)     8493 2023-04-27 19:42:17.000000 Simba-UW-tf-dev-1.58.8/simba/plotting/ez_lineplot.py
+-rw-r--r--   0 simon      (501) staff       (20)    11539 2023-05-04 15:02:11.000000 Simba-UW-tf-dev-1.58.8/simba/plotting/distance_plotter_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)    15610 2023-04-28 19:59:06.000000 Simba-UW-tf-dev-1.58.8/simba/plotting/ROI_plotter.py
+-rw-r--r--   0 simon      (501) staff       (20)    13164 2023-05-04 15:02:11.000000 Simba-UW-tf-dev-1.58.8/simba/plotting/heat_mapper_clf.py
+-rw-r--r--   0 simon      (501) staff       (20)     9036 2023-05-04 15:02:11.000000 Simba-UW-tf-dev-1.58.8/simba/plotting/distance_plotter.py
+-rw-r--r--   0 simon      (501) staff       (20)     8302 2023-05-04 15:16:51.000000 Simba-UW-tf-dev-1.58.8/simba/plotting/single_run_model_validation_video_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)     9761 2023-04-28 19:59:05.000000 Simba-UW-tf-dev-1.58.8/simba/plotting/Directing_animals_visualizer.py
+-rw-r--r--   0 simon      (501) staff       (20)    16321 2023-04-28 19:59:05.000000 Simba-UW-tf-dev-1.58.8/simba/plotting/heat_mapper_location_mp.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-04 20:00:38.000000 Simba-UW-tf-dev-1.58.8/simba/dash_app/
+-rw-r--r--   0 simon      (501) staff       (20)    49699 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.8/simba/dash_app/SimBA_dash_app.py
+-rw-r--r--   0 simon      (501) staff       (20)     5029 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.8/simba/dash_app/run_dash_tkinter.py
+-rw-r--r--   0 simon      (501) staff       (20)    24474 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.8/simba/dash_app/dash_app.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-04 20:00:38.000000 Simba-UW-tf-dev-1.58.8/simba/data_processors/
+-rw-r--r--   0 simon      (501) staff       (20)     6366 2023-05-04 14:18:28.000000 Simba-UW-tf-dev-1.58.8/simba/data_processors/agg_clf_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)    11575 2023-04-28 19:59:05.000000 Simba-UW-tf-dev-1.58.8/simba/data_processors/interpolation_smoothing.py
+-rw-r--r--   0 simon      (501) staff       (20)     7444 2023-05-04 14:18:28.000000 Simba-UW-tf-dev-1.58.8/simba/data_processors/timebins_clf_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)    12854 2023-05-04 14:18:28.000000 Simba-UW-tf-dev-1.58.8/simba/data_processors/fsttc_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)     6317 2023-04-25 18:03:32.000000 Simba-UW-tf-dev-1.58.8/simba/data_processors/interpolate_pose.py
+-rw-r--r--   0 simon      (501) staff       (20)     9646 2023-04-28 19:20:42.000000 Simba-UW-tf-dev-1.58.8/simba/data_processors/directing_other_animals_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)     8258 2023-05-04 17:41:51.000000 Simba-UW-tf-dev-1.58.8/simba/data_processors/timebins_movement_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)     4800 2023-05-04 14:18:28.000000 Simba-UW-tf-dev-1.58.8/simba/data_processors/severity_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)    16856 2023-05-04 14:18:28.000000 Simba-UW-tf-dev-1.58.8/simba/data_processors/pup_retrieval_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)     2945 2023-05-04 14:18:28.000000 Simba-UW-tf-dev-1.58.8/simba/data_processors/pybursts_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)     9608 2023-05-04 14:18:28.000000 Simba-UW-tf-dev-1.58.8/simba/data_processors/kleinberg_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)     7755 2023-05-04 15:35:50.000000 Simba-UW-tf-dev-1.58.8/simba/data_processors/movement_calculator.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-04 20:00:38.000000 Simba-UW-tf-dev-1.58.8/simba/pose_configurations_archive/
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-04 20:00:38.000000 Simba-UW-tf-dev-1.58.8/simba/pose_configurations_archive/pose_configurations_archive_1/
+-rw-r--r--   0 simon      (501) staff       (20)    14340 2023-03-30 11:05:37.000000 Simba-UW-tf-dev-1.58.8/simba/pose_configurations_archive/pose_configurations_archive_1/.DS_Store
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-04 20:00:38.000000 Simba-UW-tf-dev-1.58.8/simba/pose_configurations_archive/pose_configurations_archive_1/bp_names/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-16 13:26:00.000000 Simba-UW-tf-dev-1.58.8/simba/pose_configurations_archive/pose_configurations_archive_1/bp_names/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)     1334 2023-04-28 23:45:27.000000 Simba-UW-tf-dev-1.58.8/simba/pose_configurations_archive/pose_configurations_archive_1/bp_names/bp_names.csv
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-04 20:00:38.000000 Simba-UW-tf-dev-1.58.8/simba/pose_configurations_archive/pose_configurations_archive_1/no_animals/
+-rw-r--r--   0 simon      (501) staff       (20)       26 2023-04-28 23:45:27.000000 Simba-UW-tf-dev-1.58.8/simba/pose_configurations_archive/pose_configurations_archive_1/no_animals/no_animals.csv
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-16 13:26:19.000000 Simba-UW-tf-dev-1.58.8/simba/pose_configurations_archive/pose_configurations_archive_1/no_animals/.DS_Store
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-04 20:00:38.000000 Simba-UW-tf-dev-1.58.8/simba/pose_configurations_archive/pose_configurations_archive_1/configuration_names/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-16 13:26:14.000000 Simba-UW-tf-dev-1.58.8/simba/pose_configurations_archive/pose_configurations_archive_1/configuration_names/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)      282 2023-04-28 23:45:27.000000 Simba-UW-tf-dev-1.58.8/simba/pose_configurations_archive/pose_configurations_archive_1/configuration_names/pose_config_names.csv
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-04 20:00:38.000000 Simba-UW-tf-dev-1.58.8/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/
+-rw-r--r--   0 simon      (501) staff       (20)     8196 2023-03-30 10:45:10.000000 Simba-UW-tf-dev-1.58.8/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)    39805 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.8/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/8.png
+-rw-r--r--   0 simon      (501) staff       (20)    62501 2023-03-30 10:39:05.000000 Simba-UW-tf-dev-1.58.8/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/9.png
+-rw-r--r--   0 simon      (501) staff       (20)     6172 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.8/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/12.png
+-rw-r--r--   0 simon      (501) staff       (20)    11376 2023-04-28 23:45:27.000000 Simba-UW-tf-dev-1.58.8/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/13.png
+-rw-r--r--   0 simon      (501) staff       (20)    69501 2023-03-30 10:44:04.000000 Simba-UW-tf-dev-1.58.8/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/11.png
+-rw-r--r--   0 simon      (501) staff       (20)    69410 2023-03-30 10:40:01.000000 Simba-UW-tf-dev-1.58.8/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/10.png
+-rw-r--r--   0 simon      (501) staff       (20)    16000 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.8/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/4.png
+-rw-r--r--   0 simon      (501) staff       (20)    28150 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.8/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/5.png
+-rw-r--r--   0 simon      (501) staff       (20)    31140 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.8/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/7.png
+-rw-r--r--   0 simon      (501) staff       (20)    30634 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.8/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/6.png
+-rw-r--r--   0 simon      (501) staff       (20)    15417 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.8/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/2.png
+-rw-r--r--   0 simon      (501) staff       (20)    15786 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.8/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/3.png
+-rw-r--r--   0 simon      (501) staff       (20)    18939 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.8/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/1.png
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-04 20:00:38.000000 Simba-UW-tf-dev-1.58.8/simba/model/
+-rw-r--r--   0 simon      (501) staff       (20)    19187 2023-04-29 19:01:32.000000 Simba-UW-tf-dev-1.58.8/simba/model/train_rf.py
+-rw-r--r--   0 simon      (501) staff       (20)     3542 2023-04-28 20:13:23.000000 Simba-UW-tf-dev-1.58.8/simba/model/inference_batch.py
+-rw-r--r--   0 simon      (501) staff       (20)    18698 2023-05-04 19:56:21.000000 Simba-UW-tf-dev-1.58.8/simba/model/grid_search_rf.py
+-rw-r--r--   0 simon      (501) staff       (20)     3170 2023-04-28 20:11:10.000000 Simba-UW-tf-dev-1.58.8/simba/model/inference_validation.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-04 20:00:38.000000 Simba-UW-tf-dev-1.58.8/simba/roi_tools/
+-rw-r--r--   0 simon      (501) staff       (20)     5917 2023-05-04 19:36:28.000000 Simba-UW-tf-dev-1.58.8/simba/roi_tools/ROI_time_bin_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)     1753 2023-04-27 19:42:17.000000 Simba-UW-tf-dev-1.58.8/simba/roi_tools/ROI_movement_analyzer.py
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-20 12:47:56.000000 Simba-UW-tf-dev-1.58.8/simba/roi_tools/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)    43131 2023-04-28 20:51:11.000000 Simba-UW-tf-dev-1.58.8/simba/roi_tools/ROI_define.py
+-rw-r--r--   0 simon      (501) staff       (20)     3403 2023-04-29 19:01:32.000000 Simba-UW-tf-dev-1.58.8/simba/roi_tools/ROI_reset.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.8/simba/roi_tools/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)    19806 2023-05-04 15:35:50.000000 Simba-UW-tf-dev-1.58.8/simba/roi_tools/ROI_analyzer.py
+-rw-r--r--   0 simon      (501) staff       (20)    11373 2023-05-04 15:35:50.000000 Simba-UW-tf-dev-1.58.8/simba/roi_tools/ROI_feature_analyzer.py
+-rw-r--r--   0 simon      (501) staff       (20)     3654 2023-04-29 19:01:32.000000 Simba-UW-tf-dev-1.58.8/simba/roi_tools/ROI_multiply.py
+-rw-r--r--   0 simon      (501) staff       (20)      961 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.8/simba/roi_tools/ROI_size_calculations.py
+-rw-r--r--   0 simon      (501) staff       (20)     3505 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.8/simba/roi_tools/ROI_zoom.py
+-rw-r--r--   0 simon      (501) staff       (20)    11432 2023-05-04 15:35:50.000000 Simba-UW-tf-dev-1.58.8/simba/roi_tools/ROI_directing_analyzer.py
+-rw-r--r--   0 simon      (501) staff       (20)    10128 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.8/simba/roi_tools/ROI_move_shape.py
+-rw-r--r--   0 simon      (501) staff       (20)     5079 2023-04-29 19:01:32.000000 Simba-UW-tf-dev-1.58.8/simba/roi_tools/ROI_menus.py
+-rw-r--r--   0 simon      (501) staff       (20)    13793 2023-04-26 14:59:42.000000 Simba-UW-tf-dev-1.58.8/simba/roi_tools/ROI_clf_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)    22688 2023-04-29 19:01:32.000000 Simba-UW-tf-dev-1.58.8/simba/roi_tools/ROI_image.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-04 20:00:38.000000 Simba-UW-tf-dev-1.58.8/simba/pose_importers/
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-04 20:00:38.000000 Simba-UW-tf-dev-1.58.8/simba/pose_importers/misc/
+-rw-r--r--   0 simon      (501) staff       (20)     7349 2023-05-01 00:05:15.000000 Simba-UW-tf-dev-1.58.8/simba/pose_importers/misc/sleap_csv_importer.py
+-rw-r--r--   0 simon      (501) staff       (20)     9719 2023-05-01 00:05:15.000000 Simba-UW-tf-dev-1.58.8/simba/pose_importers/misc/sleap_h5_importer.py
+-rw-r--r--   0 simon      (501) staff       (20)     6451 2023-05-01 17:30:49.000000 Simba-UW-tf-dev-1.58.8/simba/pose_importers/misc/madlc_importer.py
+-rw-r--r--   0 simon      (501) staff       (20)     7943 2023-05-01 19:07:14.000000 Simba-UW-tf-dev-1.58.8/simba/pose_importers/misc/apt_trk_importer.py
+-rw-r--r--   0 simon      (501) staff       (20)    10945 2023-05-01 17:21:29.000000 Simba-UW-tf-dev-1.58.8/simba/pose_importers/misc/sleap_slp_importer.py
+-rw-r--r--   0 simon      (501) staff       (20)     2464 2023-04-27 19:42:17.000000 Simba-UW-tf-dev-1.58.8/simba/pose_importers/read_DANNCE_mat.py
+-rw-r--r--   0 simon      (501) staff       (20)    22015 2023-04-29 19:01:32.000000 Simba-UW-tf-dev-1.58.8/simba/pose_importers/sleap_importer_slp.py
+-rw-r--r--   0 simon      (501) staff       (20)    23524 2023-04-30 23:21:29.000000 Simba-UW-tf-dev-1.58.8/simba/pose_importers/sleap_importer_h5.py
+-rw-r--r--   0 simon      (501) staff       (20)    23603 2023-04-29 19:01:32.000000 Simba-UW-tf-dev-1.58.8/simba/pose_importers/dlc_multi_animal_importer.py
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-04-25 16:49:14.000000 Simba-UW-tf-dev-1.58.8/simba/pose_importers/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)    21021 2023-04-30 23:23:03.000000 Simba-UW-tf-dev-1.58.8/simba/pose_importers/sleap_importer_csv.py
+-rw-r--r--   0 simon      (501) staff       (20)     7783 2023-04-28 20:16:23.000000 Simba-UW-tf-dev-1.58.8/simba/pose_importers/import_mars.py
+-rw-r--r--   0 simon      (501) staff       (20)     6949 2023-04-28 20:19:13.000000 Simba-UW-tf-dev-1.58.8/simba/pose_importers/dlc_importer_csv.py
+-rw-r--r--   0 simon      (501) staff       (20)     8060 2023-04-28 19:20:42.000000 Simba-UW-tf-dev-1.58.8/simba/pose_importers/trk_importer.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-04 20:00:38.000000 Simba-UW-tf-dev-1.58.8/simba/pose_configurations/
+-rw-r--r--   0 simon      (501) staff       (20)    14340 2023-03-30 11:05:37.000000 Simba-UW-tf-dev-1.58.8/simba/pose_configurations/.DS_Store
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-04 20:00:38.000000 Simba-UW-tf-dev-1.58.8/simba/pose_configurations/bp_names/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-16 13:26:00.000000 Simba-UW-tf-dev-1.58.8/simba/pose_configurations/bp_names/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)     1316 2023-04-29 18:20:02.000000 Simba-UW-tf-dev-1.58.8/simba/pose_configurations/bp_names/bp_names.csv
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-04 20:00:38.000000 Simba-UW-tf-dev-1.58.8/simba/pose_configurations/no_animals/
+-rw-r--r--   0 simon      (501) staff       (20)       24 2023-04-29 18:20:02.000000 Simba-UW-tf-dev-1.58.8/simba/pose_configurations/no_animals/no_animals.csv
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-16 13:26:19.000000 Simba-UW-tf-dev-1.58.8/simba/pose_configurations/no_animals/.DS_Store
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-04 20:00:38.000000 Simba-UW-tf-dev-1.58.8/simba/pose_configurations/configuration_names/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-16 13:26:14.000000 Simba-UW-tf-dev-1.58.8/simba/pose_configurations/configuration_names/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)      267 2023-04-29 18:20:02.000000 Simba-UW-tf-dev-1.58.8/simba/pose_configurations/configuration_names/pose_config_names.csv
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-04 20:00:38.000000 Simba-UW-tf-dev-1.58.8/simba/pose_configurations/schematics/
+-rw-r--r--   0 simon      (501) staff       (20)    39805 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.8/simba/pose_configurations/schematics/8.png
+-rw-r--r--   0 simon      (501) staff       (20)    62501 2023-03-30 10:39:05.000000 Simba-UW-tf-dev-1.58.8/simba/pose_configurations/schematics/9.png
+-rw-r--r--   0 simon      (501) staff       (20)     6172 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.8/simba/pose_configurations/schematics/12.png
+-rw-r--r--   0 simon      (501) staff       (20)    69501 2023-03-30 10:44:04.000000 Simba-UW-tf-dev-1.58.8/simba/pose_configurations/schematics/11.png
+-rw-r--r--   0 simon      (501) staff       (20)    69410 2023-03-30 10:40:01.000000 Simba-UW-tf-dev-1.58.8/simba/pose_configurations/schematics/10.png
+-rw-r--r--   0 simon      (501) staff       (20)    16000 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.8/simba/pose_configurations/schematics/4.png
+-rw-r--r--   0 simon      (501) staff       (20)    28150 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.8/simba/pose_configurations/schematics/5.png
+-rw-r--r--   0 simon      (501) staff       (20)    31140 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.8/simba/pose_configurations/schematics/7.png
+-rw-r--r--   0 simon      (501) staff       (20)    30634 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.8/simba/pose_configurations/schematics/6.png
+-rw-r--r--   0 simon      (501) staff       (20)    15417 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.8/simba/pose_configurations/schematics/2.png
+-rw-r--r--   0 simon      (501) staff       (20)    15786 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.8/simba/pose_configurations/schematics/3.png
+-rw-r--r--   0 simon      (501) staff       (20)    18939 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.8/simba/pose_configurations/schematics/1.png
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-04 20:00:38.000000 Simba-UW-tf-dev-1.58.8/simba/video_processors/
+-rw-r--r--   0 simon      (501) staff       (20)    41779 2023-05-04 14:03:25.000000 Simba-UW-tf-dev-1.58.8/simba/video_processors/video_processing.py
+-rw-r--r--   0 simon      (501) staff       (20)     8196 2023-03-17 14:43:38.000000 Simba-UW-tf-dev-1.58.8/simba/video_processors/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)     7171 2023-04-27 19:42:17.000000 Simba-UW-tf-dev-1.58.8/simba/video_processors/px_to_mm.py
+-rw-r--r--   0 simon      (501) staff       (20)    24645 2023-04-28 20:51:11.000000 Simba-UW-tf-dev-1.58.8/simba/video_processors/batch_process_menus.py
+-rw-r--r--   0 simon      (501) staff       (20)     7174 2023-04-28 19:59:05.000000 Simba-UW-tf-dev-1.58.8/simba/video_processors/multi_cropper.py
+-rw-r--r--   0 simon      (501) staff       (20)     2833 2023-04-27 20:23:35.000000 Simba-UW-tf-dev-1.58.8/simba/video_processors/extract_frames.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.8/simba/video_processors/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)     8214 2023-04-28 19:26:14.000000 Simba-UW-tf-dev-1.58.8/simba/video_processors/calculate_px_dist.py
+-rw-r--r--   0 simon      (501) staff       (20)     4695 2023-04-26 18:17:53.000000 Simba-UW-tf-dev-1.58.8/simba/video_processors/extract_seqframes.py
+-rw-r--r--   0 simon      (501) staff       (20)    11106 2023-04-25 13:26:59.000000 Simba-UW-tf-dev-1.58.8/simba/video_processors/batch_process_create_ffmpeg_commands.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-04 20:00:38.000000 Simba-UW-tf-dev-1.58.8/simba/outlier_tools/
+-rw-r--r--   0 simon      (501) staff       (20)     7377 2023-04-29 19:01:32.000000 Simba-UW-tf-dev-1.58.8/simba/outlier_tools/outlier_corrector_movement.py
+-rw-r--r--   0 simon      (501) staff       (20)     8196 2023-03-15 17:05:05.000000 Simba-UW-tf-dev-1.58.8/simba/outlier_tools/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.8/simba/outlier_tools/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)     8190 2023-04-29 19:01:32.000000 Simba-UW-tf-dev-1.58.8/simba/outlier_tools/outlier_corrector_location.py
+-rw-r--r--   0 simon      (501) staff       (20)     2913 2023-04-28 17:39:56.000000 Simba-UW-tf-dev-1.58.8/simba/outlier_tools/skip_outlier_correction.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-04 20:00:38.000000 Simba-UW-tf-dev-1.58.8/simba/outlier_tools/.idea/
+-rw-r--r--   0 simon      (501) staff       (20)      617 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.8/simba/outlier_tools/.idea/outlier_scripts.iml
+-rw-r--r--   0 simon      (501) staff       (20)      138 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.8/simba/outlier_tools/.idea/encodings.xml
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-04 20:00:38.000000 Simba-UW-tf-dev-1.58.8/simba/outlier_tools/.idea/inspectionProfiles/
+-rw-r--r--   0 simon      (501) staff       (20)      668 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.8/simba/outlier_tools/.idea/inspectionProfiles/Project_Default.xml
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-04 20:00:38.000000 Simba-UW-tf-dev-1.58.8/simba/outlier_tools/.idea/libraries/
+-rw-r--r--   0 simon      (501) staff       (20)      128 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.8/simba/outlier_tools/.idea/libraries/R_User_Library.xml
+-rw-r--r--   0 simon      (501) staff       (20)     8102 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.8/simba/outlier_tools/.idea/workspace.xml
+-rw-r--r--   0 simon      (501) staff       (20)      289 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.8/simba/outlier_tools/.idea/modules.xml
+-rw-r--r--   0 simon      (501) staff       (20)      294 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.8/simba/outlier_tools/.idea/misc.xml
+-rw-r--r--   0 simon      (501) staff       (20)    64875 2023-05-03 18:36:47.000000 Simba-UW-tf-dev-1.58.8/simba/SimBA.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-04 20:00:38.000000 Simba-UW-tf-dev-1.58.8/simba/assets/
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-04 20:00:38.000000 Simba-UW-tf-dev-1.58.8/simba/assets/unsupervised/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.8/simba/assets/unsupervised/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)   109483 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.8/simba/assets/unsupervised/model_names.parquet
+-rw-r--r--   0 simon      (501) staff       (20)    14175 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.8/simba/assets/unsupervised/features.csv
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-04 20:00:38.000000 Simba-UW-tf-dev-1.58.8/simba/assets/shap/
+-rw-r--r--   0 simon      (501) staff       (20)     1177 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.8/simba/assets/shap/down_arrow.jpg
+-rw-r--r--   0 simon      (501) staff       (20)     1733 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.8/simba/assets/shap/intruder_shape.jpg
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-04 20:00:38.000000 Simba-UW-tf-dev-1.58.8/simba/assets/shap/feature_categories/
+-rw-r--r--   0 simon      (501) staff       (20)      109 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.8/simba/assets/shap/feature_categories/.~lock.shap_feature_categories.csv#
+-rw-r--r--   0 simon      (501) staff       (20)    17420 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.8/simba/assets/shap/feature_categories/shap_feature_categories.csv
+-rw-r--r--   0 simon      (501) staff       (20)     8196 2023-04-10 20:37:13.000000 Simba-UW-tf-dev-1.58.8/simba/assets/shap/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)     1665 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.8/simba/assets/shap/resident_shape.jpg
+-rw-r--r--   0 simon      (501) staff       (20)     2415 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.8/simba/assets/shap/resident_intruder_shape.jpg
+-rw-r--r--   0 simon      (501) staff       (20)     2012 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.8/simba/assets/shap/animal_distances.jpg
+-rw-r--r--   0 simon      (501) staff       (20)     4422 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.8/simba/assets/shap/baseline_scale.jpg
+-rw-r--r--   0 simon      (501) staff       (20)   353824 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.8/simba/assets/shap/ubuntu.regular.ttf
+-rw-r--r--   0 simon      (501) staff       (20)     6672 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.8/simba/assets/shap/side_scale.jpg
+-rw-r--r--   0 simon      (501) staff       (20)   189004 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.8/simba/assets/shap/UbuntuMono-Regular.ttf
+-rw-r--r--   0 simon      (501) staff       (20)     2737 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.8/simba/assets/shap/side_scale_5.jpg
+-rw-r--r--   0 simon      (501) staff       (20)     1785 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.8/simba/assets/shap/intruder_movement.jpg
+-rw-r--r--   0 simon      (501) staff       (20)     1435 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.8/simba/assets/shap/resident_movement.jpg
+-rw-r--r--   0 simon      (501) staff       (20)     3134 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.8/simba/assets/shap/color_bar.jpg
+-rw-r--r--   0 simon      (501) staff       (20)     2120 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.8/simba/assets/shap/resident_intruder_movement.jpg
+-rw-r--r--   0 simon      (501) staff       (20)    16388 2023-04-25 19:14:34.000000 Simba-UW-tf-dev-1.58.8/simba/assets/.DS_Store
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-04 20:00:38.000000 Simba-UW-tf-dev-1.58.8/simba/assets/lookups/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.8/simba/assets/lookups/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)   270783 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.8/simba/assets/lookups/model_names.parquet
+-rw-r--r--   0 simon      (501) staff       (20)     2987 2023-04-25 20:39:03.000000 Simba-UW-tf-dev-1.58.8/simba/assets/lookups/feature_extraction_headers.csv
+-rw-r--r--   0 simon      (501) staff       (20)    14175 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.8/simba/assets/lookups/features.csv
+-rw-r--r--   0 simon      (501) staff       (20)    14175 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.8/simba/assets/lookups/unsupervised_example_x.csv
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-04 20:00:38.000000 Simba-UW-tf-dev-1.58.8/simba/assets/stl/
+-rw-r--r--   0 simon      (501) staff       (20)   551576 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.8/simba/assets/stl/operant_tray.stl
+-rw-r--r--   0 simon      (501) staff       (20)    67647 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.8/simba/assets/stl/operant_lever.stl
+-rw-r--r--   0 simon      (501) staff       (20)    92896 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.8/simba/assets/stl/operant_walls.stl
+-rw-r--r--   0 simon      (501) staff       (20)  4759984 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.8/simba/assets/stl/grid_floor.stl
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-04 20:00:38.000000 Simba-UW-tf-dev-1.58.8/simba/assets/img/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-04-10 23:20:37.000000 Simba-UW-tf-dev-1.58.8/simba/assets/img/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)   399272 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.8/simba/assets/img/about_me.png
+-rw-r--r--   0 simon      (501) staff       (20)   117108 2023-04-10 23:06:31.000000 Simba-UW-tf-dev-1.58.8/simba/assets/img/splash.mp4
+-rw-r--r--   0 simon      (501) staff       (20)   322242 2023-04-06 16:38:51.000000 Simba-UW-tf-dev-1.58.8/simba/assets/img/bg_2.png
+-rw-r--r--   0 simon      (501) staff       (20)    69267 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.8/simba/assets/img/splash.pptx
+-rw-r--r--   0 simon      (501) staff       (20)   204362 2023-04-06 15:01:45.000000 Simba-UW-tf-dev-1.58.8/simba/assets/img/bg.png
+-rw-r--r--   0 simon      (501) staff       (20)   189004 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.8/simba/assets/UbuntuMono-Regular.ttf
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-04 20:00:38.000000 Simba-UW-tf-dev-1.58.8/simba/assets/icons/
+-rw-r--r--   0 simon      (501) staff       (20)     1350 2023-03-17 17:59:27.000000 Simba-UW-tf-dev-1.58.8/simba/assets/icons/factory.png
+-rw-r--r--   0 simon      (501) staff       (20)     1413 2023-03-21 13:03:06.000000 Simba-UW-tf-dev-1.58.8/simba/assets/icons/cluster.png
+-rw-r--r--   0 simon      (501) staff       (20)     1340 2023-03-17 16:51:08.000000 Simba-UW-tf-dev-1.58.8/simba/assets/icons/load.png
+-rw-r--r--   0 simon      (501) staff       (20)     4507 2023-03-20 14:13:48.000000 Simba-UW-tf-dev-1.58.8/simba/assets/icons/gif.png
+-rw-rw-r--   0 simon      (501) staff       (20)     4566 2023-03-18 18:12:27.000000 Simba-UW-tf-dev-1.58.8/simba/assets/icons/pose.png
+-rw-rw-r--   0 simon      (501) staff       (20)     1943 2023-03-18 18:14:10.000000 Simba-UW-tf-dev-1.58.8/simba/assets/icons/features.png
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-04-05 17:25:36.000000 Simba-UW-tf-dev-1.58.8/simba/assets/icons/.DS_Store
+-rw-rw-r--   0 simon      (501) staff       (20)     4896 2023-03-17 19:17:29.000000 Simba-UW-tf-dev-1.58.8/simba/assets/icons/settings.png
+-rw-r--r--   0 simon      (501) staff       (20)     2090 2023-04-22 15:14:17.000000 Simba-UW-tf-dev-1.58.8/simba/assets/icons/stopwatch.png
+-rw-r--r--   0 simon      (501) staff       (20)     1252 2023-03-19 16:48:40.000000 Simba-UW-tf-dev-1.58.8/simba/assets/icons/link.png
+-rw-r--r--   0 simon      (501) staff       (20)    14250 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.8/simba/assets/icons/dash_simba.css
+-rw-r--r--   0 simon      (501) staff       (20)      917 2023-04-05 16:43:13.000000 Simba-UW-tf-dev-1.58.8/simba/assets/icons/documentation.png
+-rw-r--r--   0 simon      (501) staff       (20)     4503 2023-03-20 14:08:00.000000 Simba-UW-tf-dev-1.58.8/simba/assets/icons/fps.png
+-rw-r--r--   0 simon      (501) staff       (20)     1299 2023-03-21 13:02:07.000000 Simba-UW-tf-dev-1.58.8/simba/assets/icons/dimensionality_reduction.png
+-rw-rw-r--   0 simon      (501) staff       (20)     4823 2023-03-17 19:03:29.000000 Simba-UW-tf-dev-1.58.8/simba/assets/icons/roi.png
+-rw-r--r--   0 simon      (501) staff       (20)      920 2023-03-20 14:25:03.000000 Simba-UW-tf-dev-1.58.8/simba/assets/icons/superimpose.png
+-rw-r--r--   0 simon      (501) staff       (20)     1136 2023-03-18 20:25:31.000000 Simba-UW-tf-dev-1.58.8/simba/assets/icons/label.png
+-rw-r--r--   0 simon      (501) staff       (20)     1016 2023-03-20 14:28:47.000000 Simba-UW-tf-dev-1.58.8/simba/assets/icons/change.png
+-rw-r--r--   0 simon      (501) staff       (20)     1124 2023-03-17 18:05:26.000000 Simba-UW-tf-dev-1.58.8/simba/assets/icons/crop.png
+-rw-r--r--   0 simon      (501) staff       (20)     2146 2023-04-13 14:09:23.000000 Simba-UW-tf-dev-1.58.8/simba/assets/icons/rotate.png
+-rw-r--r--   0 simon      (501) staff       (20)     1057 2023-03-20 14:03:42.000000 Simba-UW-tf-dev-1.58.8/simba/assets/icons/path.png
+-rw-r--r--   0 simon      (501) staff       (20)      950 2023-03-17 18:07:33.000000 Simba-UW-tf-dev-1.58.8/simba/assets/icons/clip.png
+-rw-r--r--   0 simon      (501) staff       (20)     2121 2023-04-04 14:37:43.000000 Simba-UW-tf-dev-1.58.8/simba/assets/icons/restart.png
+-rw-rw-r--   0 simon      (501) staff       (20)     4653 2023-03-17 18:11:59.000000 Simba-UW-tf-dev-1.58.8/simba/assets/icons/calipher.png
+-rw-r--r--   0 simon      (501) staff       (20)     1291 2023-03-21 20:16:55.000000 Simba-UW-tf-dev-1.58.8/simba/assets/icons/add_on.png
+-rw-rw-r--   0 simon      (501) staff       (20)     4695 2023-03-17 17:57:16.000000 Simba-UW-tf-dev-1.58.8/simba/assets/icons/create.png
+-rw-r--r--   0 simon      (501) staff       (20)    78182 2023-03-20 16:35:36.000000 Simba-UW-tf-dev-1.58.8/simba/assets/icons/SimBA_logo.ico
+-rw-r--r--   0 simon      (501) staff       (20)     1067 2023-03-20 14:22:44.000000 Simba-UW-tf-dev-1.58.8/simba/assets/icons/print.png
+-rw-rw-r--   0 simon      (501) staff       (20)     4653 2023-03-18 20:27:58.000000 Simba-UW-tf-dev-1.58.8/simba/assets/icons/clf.png
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-04 20:00:38.000000 Simba-UW-tf-dev-1.58.8/simba/assets/icons/concat_icons/
+-rw-r--r--   0 simon      (501) staff       (20)     6027 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.8/simba/assets/icons/concat_icons/mosaic.png
+-rw-r--r--   0 simon      (501) staff       (20)     5654 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.8/simba/assets/icons/concat_icons/vertical.png
+-rw-r--r--   0 simon      (501) staff       (20)     5542 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.8/simba/assets/icons/concat_icons/horizontal.png
+-rw-r--r--   0 simon      (501) staff       (20)     5939 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.8/simba/assets/icons/concat_icons/mixed_mosaic.png
+-rw-r--r--   0 simon      (501) staff       (20)     2060 2023-03-20 14:26:12.000000 Simba-UW-tf-dev-1.58.8/simba/assets/icons/merge.png
+-rw-r--r--   0 simon      (501) staff       (20)     1252 2023-04-07 11:25:59.000000 Simba-UW-tf-dev-1.58.8/simba/assets/icons/clean.png
+-rw-------   0 simon      (501) staff       (20)     4725 2023-03-18 20:27:47.000000 Simba-UW-tf-dev-1.58.8/simba/assets/icons/clf_2.png
+-rw-rw-r--   0 simon      (501) staff       (20)     4795 2023-03-17 18:10:10.000000 Simba-UW-tf-dev-1.58.8/simba/assets/icons/visualize.png
+-rw-r--r--   0 simon      (501) staff       (20)     2142 2023-03-20 14:10:28.000000 Simba-UW-tf-dev-1.58.8/simba/assets/icons/concat.png
+-rw-r--r--   0 simon      (501) staff       (20)     1474 2023-03-17 19:20:24.000000 Simba-UW-tf-dev-1.58.8/simba/assets/icons/boris.png
+-rw-rw-r--   0 simon      (501) staff       (20)     4804 2023-03-19 16:43:01.000000 Simba-UW-tf-dev-1.58.8/simba/assets/icons/frames.png
+-rw-r--r--   0 simon      (501) staff       (20)     2425 2023-03-19 16:44:55.000000 Simba-UW-tf-dev-1.58.8/simba/assets/icons/video.png
+-rw-r--r--   0 simon      (501) staff       (20)     2089 2023-03-20 14:05:58.000000 Simba-UW-tf-dev-1.58.8/simba/assets/icons/sample.png
+-rw-r--r--   0 simon      (501) staff       (20)     1471 2023-03-21 13:04:02.000000 Simba-UW-tf-dev-1.58.8/simba/assets/icons/metrics.png
+-rw-r--r--   0 simon      (501) staff       (20)     4555 2023-03-20 14:21:02.000000 Simba-UW-tf-dev-1.58.8/simba/assets/icons/grey.png
+-rw-r--r--   0 simon      (501) staff       (20)      930 2023-03-18 18:07:29.000000 Simba-UW-tf-dev-1.58.8/simba/assets/icons/exit.png
+-rw-r--r--   0 simon      (501) staff       (20)     4751 2023-03-18 20:31:58.000000 Simba-UW-tf-dev-1.58.8/simba/assets/icons/outlier.png
+-rw-r--r--   0 simon      (501) staff       (20)     4392 2023-03-20 14:16:15.000000 Simba-UW-tf-dev-1.58.8/simba/assets/icons/clahe.png
+-rw-rw-r--   0 simon      (501) staff       (20)     4637 2023-03-17 19:03:55.000000 Simba-UW-tf-dev-1.58.8/simba/assets/icons/trash.png
+-rw-r--r--   0 simon      (501) staff       (20)     1239 2023-03-19 16:51:21.000000 Simba-UW-tf-dev-1.58.8/simba/assets/icons/about.png
+-rw-rw-r--   0 simon      (501) staff       (20)     4666 2023-03-17 18:01:21.000000 Simba-UW-tf-dev-1.58.8/simba/assets/icons/convert.png
+-rw-r--r--   0 simon      (501) staff       (20)    93229 2023-03-20 16:01:42.000000 Simba-UW-tf-dev-1.58.8/simba/assets/icons/SimBA_logo.icns
+-rw-r--r--   0 simon      (501) staff       (20)      991 2023-03-20 19:02:33.000000 Simba-UW-tf-dev-1.58.8/simba/assets/icons/reorganize.png
+-rw-rw-r--   0 simon      (501) staff       (20)     4784 2023-03-17 18:50:35.000000 Simba-UW-tf-dev-1.58.8/simba/assets/icons/browse.png
+-rw-r--r--   0 simon      (501) staff       (20)    30707 2023-03-20 16:33:38.000000 Simba-UW-tf-dev-1.58.8/simba/assets/icons/SimBA_logo.png
+-rw-r--r--   0 simon      (501) staff       (20)     2293 2023-03-17 19:24:38.000000 Simba-UW-tf-dev-1.58.8/simba/assets/icons/ethovision.png
+-rw-r--r--   0 simon      (501) staff       (20)     1018 2023-04-05 15:24:49.000000 Simba-UW-tf-dev-1.58.8/simba/assets/icons/close.png
+-rw-r--r--   0 simon      (501) staff       (20)    13672 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.8/simba/assets/dash_simba_base.css
+-rw-r--r--   0 simon      (501) staff       (20)    31812 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.8/simba/assets/TheGoldenLab.PNG
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-04 20:00:38.000000 Simba-UW-tf-dev-1.58.8/Simba_UW_tf_dev.egg-info/
+-rw-rw-r--   0 simon      (501) staff       (20)      579 2023-05-04 20:00:38.000000 Simba-UW-tf-dev-1.58.8/Simba_UW_tf_dev.egg-info/PKG-INFO
+-rw-rw-r--   0 simon      (501) staff       (20)    18464 2023-05-04 20:00:38.000000 Simba-UW-tf-dev-1.58.8/Simba_UW_tf_dev.egg-info/SOURCES.txt
+-rw-rw-r--   0 simon      (501) staff       (20)       44 2023-05-04 20:00:38.000000 Simba-UW-tf-dev-1.58.8/Simba_UW_tf_dev.egg-info/entry_points.txt
+-rw-rw-r--   0 simon      (501) staff       (20)      639 2023-05-04 20:00:38.000000 Simba-UW-tf-dev-1.58.8/Simba_UW_tf_dev.egg-info/requires.txt
+-rw-rw-r--   0 simon      (501) staff       (20)        6 2023-05-04 20:00:38.000000 Simba-UW-tf-dev-1.58.8/Simba_UW_tf_dev.egg-info/top_level.txt
+-rw-rw-r--   0 simon      (501) staff       (20)        1 2023-05-04 20:00:38.000000 Simba-UW-tf-dev-1.58.8/Simba_UW_tf_dev.egg-info/dependency_links.txt
+-rw-rw-r--   0 simon      (501) staff       (20)     7652 2020-05-13 13:27:38.000000 Simba-UW-tf-dev-1.58.8/LICENSE.md
+-rw-rw-r--   0 simon      (501) staff       (20)      136 2021-04-10 10:44:06.000000 Simba-UW-tf-dev-1.58.8/MANIFEST.in
+-rw-rw-r--   0 simon      (501) staff       (20)     9598 2020-05-13 13:27:40.000000 Simba-UW-tf-dev-1.58.8/README.md
+-rw-rw-r--   0 simon      (501) staff       (20)     1897 2023-05-04 20:00:28.000000 Simba-UW-tf-dev-1.58.8/setup.py
+-rw-r--r--   0 simon      (501) staff       (20)       38 2023-05-04 20:00:38.000000 Simba-UW-tf-dev-1.58.8/setup.cfg
```

### Comparing `Simba-UW-tf-dev-1.58.7/PKG-INFO` & `Simba-UW-tf-dev-1.58.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Simba-UW-tf-dev
-Version: 1.58.7
+Version: 1.58.8
 Summary: Toolkit for computer classification of complex social behaviors in experimental animals
 Home-page: https://github.com/sgoldenlab/simba
 Author: Simon Nilsson, Jia Jie Choong, Sophia Hwang
 Author-email: sronilsson@gmail.com
 License: GNU Lesser General Public License v3 (LGPLv3)
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `Simba-UW-tf-dev-1.58.7/simba/ui/.DS_Store` & `Simba-UW-tf-dev-1.58.8/simba/ui/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.7/simba/ui/pop_ups/movement_analysis_time_bins_pop_up.py` & `Simba-UW-tf-dev-1.58.8/simba/ui/pop_ups/movement_analysis_time_bins_pop_up.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,47 +15,47 @@
 
         ConfigReader.__init__(self, config_path=config_path)
         PopUpMixin.__init__(self, title='TIME BINS: DISTANCE/VELOCITY', size=(400, 400))
         self.animal_cnt_frm = CreateLabelFrameWithIcon(parent=self.main_frm, header='SELECT NUMBER OF ANIMALS', icon_name=Keys.DOCUMENTATION.value, icon_link=Links.DATA_ANALYSIS.value)
         self.animal_cnt_dropdown = DropDownMenu(self.animal_cnt_frm, '# of animals', list(range(1, self.animal_cnt+1)), labelwidth=20)
         self.animal_cnt_dropdown.setChoices(1)
         self.animal_cnt_confirm_btn = Button(self.animal_cnt_frm, text="Confirm", command=lambda: self.create_settings_frm())
-        self.body_part_options = deepcopy(self.body_parts_lst)
-        for i in self.multi_animal_id_list:
-            self.body_part_options.append(i + ' CENTER OF GRAVITY')
         self.animal_cnt_frm.grid(row=0, column=0, sticky=NW)
         self.animal_cnt_dropdown.grid(row=0, column=0, sticky=NW)
         self.animal_cnt_confirm_btn.grid(row=0, column=1, sticky=NW)
         self.main_frm.mainloop()
 
     def create_settings_frm(self):
         if hasattr(self, 'setting_frm'):
             self.setting_frm.destroy()
             self.body_part_frm.destroy()
 
         self.setting_frm = LabelFrame(self.main_frm, text="SETTINGS", font=Formats.LABELFRAME_HEADER_FORMAT.value)
-        self.choose_bp_frm(parent=self.setting_frm, bp_options=self.body_part_options)
+        self.choose_bp_frm(parent=self.setting_frm, bp_options=self.body_parts_lst)
         self.plots_frm = LabelFrame(self.setting_frm, text="Plots", font=Formats.LABELFRAME_HEADER_FORMAT.value)
         self.plots_var = BooleanVar()
         self.plots_cb = Checkbutton(self.plots_frm, text='Create plots', variable=self.plots_var)
         self.plots_frm.grid(row=self.frame_children(frame=self.setting_frm), column=0, sticky=NW)
         self.plots_cb.grid(row=0, column=0, sticky=NW)
         self.setting_frm.grid(row=1, column=0, sticky=NW)
         self.create_time_bin_entry()
         self.create_run_frm(run_function=self.run)
 
     def run(self):
         check_int(name='Time bin', value=str(self.time_bin_entrybox.entry_get), min_value=1)
         self.config.set(ConfigKey.PROCESS_MOVEMENT_SETTINGS.value, ConfigKey.ROI_ANIMAL_CNT.value, str(self.animal_cnt_dropdown.getChoices()))
+        body_parts = []
         for cnt, dropdown in self.body_parts_dropdowns.items():
             self.config.set(ConfigKey.PROCESS_MOVEMENT_SETTINGS.value, 'animal_{}_bp'.format(str(cnt + 1)), str(dropdown.getChoices()))
+            body_parts.append(dropdown.getChoices())
         self.update_config()
         time_bin_movement_analyzer = TimeBinsMovementCalculator(config_path=self.config_path,
                                                                 bin_length=int(self.time_bin_entrybox.entry_get),
-                                                                plots=self.plots_var.get())
+                                                                plots=self.plots_var.get(),
+                                                                body_parts=body_parts)
         time_bin_movement_analyzer.run()
 
 
 
 #MovementAnalysisTimeBinsPopUp(config_path='/Users/simon/Desktop/envs/troubleshooting/locomotion/project_folder/project_config.ini')
```

### Comparing `Simba-UW-tf-dev-1.58.7/simba/ui/pop_ups/csv_2_parquet_pop_up.py` & `Simba-UW-tf-dev-1.58.8/simba/ui/pop_ups/csv_2_parquet_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.7/simba/ui/pop_ups/quick_path_plot_pop_up.py` & `Simba-UW-tf-dev-1.58.8/simba/ui/pop_ups/quick_path_plot_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.7/simba/ui/pop_ups/batch_preprocess_pop_up.py` & `Simba-UW-tf-dev-1.58.8/simba/ui/pop_ups/batch_preprocess_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.7/simba/ui/pop_ups/heatmap_location_pop_up.py` & `Simba-UW-tf-dev-1.58.8/simba/ui/pop_ups/heatmap_location_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.7/simba/ui/pop_ups/clf_probability_plot_pop_up.py` & `Simba-UW-tf-dev-1.58.8/simba/ui/pop_ups/clf_probability_plot_pop_up.py`

 * *Files 1% similar despite different names*

```diff
@@ -128,10 +128,10 @@
                                                                        frame_setting=self.probability_frames_var.get(),
                                                                        video_setting=self.probability_videos_var.get(),
                                                                        last_frame=self.probability_last_frm_var.get(),
                                                                        files_found=data_paths,
                                                                        clf_name=self.clf_dropdown.getChoices(),
                                                                        cores=int(self.multiprocess_dropdown.getChoices()),
                                                                        style_attr=style_attr)
-        probability_plot_creator.create_plots()
+        probability_plot_creator.run()
 
 #_ = VisualizeClassificationProbabilityPopUp(config_path='/Users/simon/Desktop/envs/troubleshooting/Two_animals_16bps/project_folder/project_config.ini')
```

### Comparing `Simba-UW-tf-dev-1.58.7/simba/ui/pop_ups/.DS_Store` & `Simba-UW-tf-dev-1.58.8/simba/ui/pop_ups/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.7/simba/ui/pop_ups/movement_analysis_pop_up.py` & `Simba-UW-tf-dev-1.58.8/simba/ui/pop_ups/movement_analysis_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.7/simba/ui/pop_ups/set_machine_model_parameters_pop_up.py` & `Simba-UW-tf-dev-1.58.8/simba/ui/pop_ups/set_machine_model_parameters_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.7/simba/ui/pop_ups/clf_plot_pop_up.py` & `Simba-UW-tf-dev-1.58.8/simba/ui/pop_ups/clf_plot_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.7/simba/ui/pop_ups/path_plot_pop_up.py` & `Simba-UW-tf-dev-1.58.8/simba/ui/pop_ups/path_plot_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.7/simba/ui/pop_ups/smoothing_interpolation_pop_up.py` & `Simba-UW-tf-dev-1.58.8/simba/ui/pop_ups/smoothing_interpolation_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.7/simba/ui/pop_ups/visualize_pose_in_dir_pop_up.py` & `Simba-UW-tf-dev-1.58.8/simba/ui/pop_ups/visualize_pose_in_dir_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.7/simba/ui/pop_ups/roi_analysis_pop_up.py` & `Simba-UW-tf-dev-1.58.8/simba/ui/pop_ups/roi_analysis_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.7/simba/ui/pop_ups/outlier_settings_pop_up.py` & `Simba-UW-tf-dev-1.58.8/simba/ui/pop_ups/outlier_settings_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.7/simba/ui/pop_ups/gantt_pop_up.py` & `Simba-UW-tf-dev-1.58.8/simba/ui/pop_ups/gantt_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.7/simba/ui/pop_ups/clf_validation_plot_pop_up.py` & `Simba-UW-tf-dev-1.58.8/simba/ui/pop_ups/clf_validation_plot_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.7/simba/ui/pop_ups/severity_analysis_pop_up.py` & `Simba-UW-tf-dev-1.58.8/simba/ui/pop_ups/severity_analysis_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.7/simba/ui/pop_ups/fsttc_pop_up.py` & `Simba-UW-tf-dev-1.58.8/simba/ui/pop_ups/fsttc_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.7/simba/ui/pop_ups/kleinberg_pop_up.py` & `Simba-UW-tf-dev-1.58.8/simba/ui/pop_ups/kleinberg_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.7/simba/ui/pop_ups/directing_other_animals_plot_pop_up.py` & `Simba-UW-tf-dev-1.58.8/simba/ui/pop_ups/directing_other_animals_plot_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.7/simba/ui/pop_ups/pose_reorganizer_pop_up.py` & `Simba-UW-tf-dev-1.58.8/simba/ui/pop_ups/pose_reorganizer_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.7/simba/ui/pop_ups/append_roi_features_animals_pop_up.py` & `Simba-UW-tf-dev-1.58.8/simba/ui/pop_ups/append_roi_features_animals_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.7/simba/ui/pop_ups/clf_by_timebins_pop_up.py` & `Simba-UW-tf-dev-1.58.8/simba/ui/pop_ups/clf_by_timebins_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.7/simba/ui/pop_ups/heatmap_clf_pop_up.py` & `Simba-UW-tf-dev-1.58.8/simba/ui/pop_ups/heatmap_clf_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.7/simba/ui/pop_ups/data_plot_pop_up.py` & `Simba-UW-tf-dev-1.58.8/simba/ui/pop_ups/data_plot_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.7/simba/ui/pop_ups/roi_features_plot_pop_up.py` & `Simba-UW-tf-dev-1.58.8/simba/ui/pop_ups/roi_features_plot_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.7/simba/ui/pop_ups/pup_retrieval_pop_up.py` & `Simba-UW-tf-dev-1.58.8/simba/ui/pop_ups/pup_retrieval_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.7/simba/ui/pop_ups/about_simba_pop_up.py` & `Simba-UW-tf-dev-1.58.8/simba/ui/pop_ups/about_simba_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.7/simba/ui/pop_ups/clf_descriptive_statistics_pop_up.py` & `Simba-UW-tf-dev-1.58.8/simba/ui/pop_ups/clf_descriptive_statistics_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.7/simba/ui/pop_ups/roi_tracking_plot_pop_up.py` & `Simba-UW-tf-dev-1.58.8/simba/ui/pop_ups/roi_tracking_plot_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.7/simba/ui/pop_ups/append_roi_features_bodypart_pop_up.py` & `Simba-UW-tf-dev-1.58.8/simba/ui/pop_ups/append_roi_features_bodypart_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.7/simba/ui/pop_ups/clf_add_remove_print_pop_up.py` & `Simba-UW-tf-dev-1.58.8/simba/ui/pop_ups/clf_add_remove_print_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.7/simba/ui/pop_ups/video_processing_pop_up.py` & `Simba-UW-tf-dev-1.58.8/simba/ui/pop_ups/video_processing_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.7/simba/ui/pop_ups/validation_plot_pop_up.py` & `Simba-UW-tf-dev-1.58.8/simba/ui/pop_ups/validation_plot_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.7/simba/ui/pop_ups/clf_by_roi_pop_up.py` & `Simba-UW-tf-dev-1.58.8/simba/ui/pop_ups/clf_by_roi_pop_up.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,24 +1,29 @@
 __author__ = "Simon Nilsson"
 
 from tkinter import *
 from collections import defaultdict
+import os
+
+
 from simba.roi_tools.ROI_clf_calculator import ROIClfCalculator
 from simba.mixins.pop_up_mixin import PopUpMixin
 from simba.mixins.config_reader import ConfigReader
 from simba.ui.tkinter_functions import CreateLabelFrameWithIcon, DropDownMenu
 from simba.utils.enums import Keys, Links
-from simba.utils.errors import NoChoosenROIError, NoChoosenClassifierError, NoChoosenMeasurementError
+from simba.utils.errors import NoChoosenROIError, NoChoosenClassifierError, NoChoosenMeasurementError, ROICoordinatesNotFoundError
 
 class ClfByROIPopUp(PopUpMixin, ConfigReader):
     def __init__(self,
                  config_path: str):
 
-        PopUpMixin.__init__(self, title='CLASSIFICATIONS BY ROI')
         ConfigReader.__init__(self, config_path=config_path)
+        if not os.path.isfile(self.roi_coordinates_path):
+            raise ROICoordinatesNotFoundError(expected_file_path=self.roi_coordinates_path)
+        PopUpMixin.__init__(self, title='CLASSIFICATIONS BY ROI')
         self.read_roi_data()
         body_part_menu = CreateLabelFrameWithIcon(parent=self.main_frm, header='Select body part', icon_name=Keys.DOCUMENTATION.value, icon_link=Links.ANALYZE_ML_RESULTS.value)
         ROI_menu = LabelFrame(self.main_frm, text='Select ROI(s)', padx=5, pady=5)
         classifier_menu = LabelFrame(self.main_frm, text='Select classifier(s)', padx=5, pady=5)
         measurements_menu = LabelFrame(self.main_frm, text='Select measurements', padx=5, pady=5)
         self.total_time_var = BooleanVar()
         self.start_bouts_var = BooleanVar()
```

### Comparing `Simba-UW-tf-dev-1.58.7/simba/ui/pop_ups/make_path_plot_pop_up.py` & `Simba-UW-tf-dev-1.58.8/simba/ui/pop_ups/make_path_plot_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.7/simba/ui/pop_ups/create_user_defined_pose_configuration_pop_up.py` & `Simba-UW-tf-dev-1.58.8/simba/ui/pop_ups/create_user_defined_pose_configuration_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.7/simba/ui/pop_ups/archive_files_pop_up.py` & `Simba-UW-tf-dev-1.58.8/simba/ui/pop_ups/archive_files_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.7/simba/ui/pop_ups/pose_bp_drop_pop_up.py` & `Simba-UW-tf-dev-1.58.8/simba/ui/pop_ups/pose_bp_drop_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.7/simba/ui/pop_ups/distance_plot_pop_up.py` & `Simba-UW-tf-dev-1.58.8/simba/ui/pop_ups/distance_plot_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.7/simba/ui/pop_ups/subset_feature_extractor_pop_up.py` & `Simba-UW-tf-dev-1.58.8/simba/ui/pop_ups/subset_feature_extractor_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.7/simba/ui/pop_ups/third_party_annotator_appender_pop_up.py` & `Simba-UW-tf-dev-1.58.8/simba/ui/pop_ups/third_party_annotator_appender_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.7/simba/ui/pop_ups/roi_analysis_time_bins_pop_up.py` & `Simba-UW-tf-dev-1.58.8/simba/ui/pop_ups/roi_analysis_time_bins_pop_up.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from tkinter import *
 
 from simba.mixins.config_reader import ConfigReader
 from simba.mixins.pop_up_mixin import PopUpMixin
 from simba.ui.tkinter_functions import CreateLabelFrameWithIcon, DropDownMenu
 from simba.utils.enums import Keys, Links, Formats, ConfigKey
-from simba.utils.checks import check_int
+from simba.utils.checks import check_int, check_float
 from simba.roi_tools.ROI_time_bin_calculator import ROITimebinCalculator
 
 class ROIAnalysisTimeBinsPopUp(ConfigReader, PopUpMixin):
 
     def __init__(self,
                  config_path: str):
 
@@ -32,18 +32,23 @@
         self.choose_bp_threshold_frm(parent=self.setting_frm)
         self.setting_frm.grid(row=1, column=0, sticky=NW)
         self.create_time_bin_entry()
         self.create_run_frm(run_function=self.run)
 
     def run(self):
         check_int(name='Time bin', value=self.time_bin_entrybox.entry_get, min_value=1)
+        check_float(name='Probability threshold', value=self.probability_entry.entry_get, min_value=0.00, max_value=1.00)
         self.config.set(ConfigKey.ROI_SETTINGS.value, ConfigKey.ROI_ANIMAL_CNT.value, str(self.animal_cnt_dropdown.getChoices()))
+        body_parts = []
         for cnt, dropdown in self.body_parts_dropdowns.items():
             self.config.set(ConfigKey.PROCESS_MOVEMENT_SETTINGS.value, 'animal_{}_bp'.format(str(cnt + 1)), str(dropdown.getChoices()))
+            body_parts.append(dropdown.getChoices())
         self.update_config()
         roi_time_bin_calculator = ROITimebinCalculator(config_path=self.config_path,
-                                                       bin_length=int(self.time_bin_entrybox.entry_get))
+                                                       bin_length=int(self.time_bin_entrybox.entry_get),
+                                                       threshold=float(self.probability_entry.entry_get),
+                                                       body_parts=body_parts)
         roi_time_bin_calculator.run()
         roi_time_bin_calculator.save()
 
 
 #ROIAnalysisTimeBinsPopUp(config_path='/Users/simon/Desktop/envs/troubleshooting/locomotion/project_folder/project_config.ini')
```

### Comparing `Simba-UW-tf-dev-1.58.7/simba/ui/video_info_ui.py` & `Simba-UW-tf-dev-1.58.8/simba/ui/video_info_ui.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 __author__ = "Simon Nilsson"
 
 from tkinter import *
-import os, glob
+import os
 import pandas as pd
 import collections
 
 from simba.utils.read_write import get_fn_ext, get_video_meta_data, read_config_entry, find_all_videos_in_project
 from simba.utils.enums import Paths, ConfigKey, Dtypes, Keys, Links, Formats
 from simba.video_processors.px_to_mm import get_coordinates_nilsson
 from simba.ui.tkinter_functions import hxtScrollbar, CreateLabelFrameWithIcon
```

### Comparing `Simba-UW-tf-dev-1.58.7/simba/ui/user_defined_pose_creator.py` & `Simba-UW-tf-dev-1.58.8/simba/ui/user_defined_pose_creator.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 __author__ = "Simon Nilsson"
 
 import cv2
 import numpy as np
 import imutils
 import simba
 import os, glob
+from typing import List
+
+
 from simba.utils.enums import Paths
 from simba.utils.data import create_color_palettes
 from simba.utils.errors import InvalidFileTypeError
 from simba.utils.checks import check_file_exist_and_readable
 from simba.mixins.plotting_mixin import PlottingMixin
 
 class PoseConfigCreator(PlottingMixin):
@@ -39,16 +42,16 @@
     >>> pose_config_creator.launch()
     """
 
     def __init__(self,
                  pose_name: str,
                  no_animals: int,
                  img_path: str,
-                 bp_list: list,
-                 animal_id_int_list: list):
+                 bp_list: List[str],
+                 animal_id_int_list: List[str]):
 
         PlottingMixin.__init__(self)
         self.pose_name, self.img_path = pose_name, img_path
         self.bp_list, self.animal_id_int_list = bp_list, animal_id_int_list
         check_file_exist_and_readable(img_path)
         self.no_animals, self.font = no_animals, cv2.FONT_HERSHEY_SIMPLEX
         self.img = cv2.imread(img_path)
```

### Comparing `Simba-UW-tf-dev-1.58.7/simba/ui/create_project_ui.py` & `Simba-UW-tf-dev-1.58.8/simba/ui/create_project_ui.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.7/simba/ui/tkinter_functions.py` & `Simba-UW-tf-dev-1.58.8/simba/ui/tkinter_functions.py`

 * *Files 2% similar despite different names*

```diff
@@ -69,15 +69,20 @@
     if acttyp == '1':  # insert
         if not inStr.isdigit():
             return False
     return True
 
 
 class DropDownMenu(Frame):
-    def __init__(self, parent=None, dropdownLabel='', choice_dict=None, labelwidth='', com=None, **kw):
+    def __init__(self,
+                 parent=None,
+                 dropdownLabel='',
+                 choice_dict=None,
+                 labelwidth='',
+                 com=None, **kw):
         Frame.__init__(self, master=parent, **kw)
         self.dropdownvar = StringVar()
         self.lblName = Label(self, text=dropdownLabel, width=labelwidth, anchor=W)
         self.lblName.grid(row=0, column=0)
         self.choices = choice_dict
         self.popupMenu = OptionMenu(self, self.dropdownvar, *self.choices, command=com)
         self.popupMenu.grid(row=0, column=1)
```

### Comparing `Simba-UW-tf-dev-1.58.7/simba/ui/machine_model_settings_ui.py` & `Simba-UW-tf-dev-1.58.8/simba/ui/machine_model_settings_ui.py`

 * *Files 0% similar despite different names*

```diff
@@ -448,14 +448,16 @@
             self.shap_save_it_dropdown.setChoices(self.meta['shap_save_iteration'])
         if 'partial_dependency' in self.meta.keys():
             if self.meta['partial_dependency'] in Options.RUN_OPTIONS_FLAGS.value:
                 self.partial_dependency_var.set(value=True)
         else:
             self.shap_save_it_dropdown.setChoices('None')
         if 'class_weights' in self.meta.keys():
+            if self.meta['class_weights'] not in Options.CLASS_WEIGHT_OPTIONS.value:
+                self.meta['class_weights'] = 'None'
             self.class_weights_dropdown.setChoices(self.meta['class_weights'])
             if self.meta['class_weights'] == 'custom':
                 self.create_class_weight_table()
                 weights = ast.literal_eval(self.meta['class_custom_weights'])
 
                 self.weight_present.setChoices(weights[1])
                 self.weight_absent.setChoices(weights[0])
```

### Comparing `Simba-UW-tf-dev-1.58.7/simba/blob_storage/.DS_Store` & `Simba-UW-tf-dev-1.58.8/simba/blob_storage/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.7/simba/labelling/.DS_Store` & `Simba-UW-tf-dev-1.58.8/simba/labelling/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.7/simba/labelling/labelling_interface.py` & `Simba-UW-tf-dev-1.58.8/simba/labelling/labelling_interface.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,14 +4,21 @@
 import pandas as pd
 from tkinter import *
 from tkinter import filedialog
 from PIL import Image, ImageTk
 from subprocess import Popen, PIPE
 import os
 from tabulate import tabulate
+from typing import Dict, Optional
+try:
+    from typing import Literal
+except ImportError:
+    from typing_extensions import Literal
+
+
 from simba.utils.errors import FrameRangeError
 from simba.mixins.config_reader import ConfigReader
 from simba.utils.read_write import read_config_entry, read_df, write_df, get_fn_ext, get_video_meta_data, get_all_clf_names
 from simba.utils.checks import check_file_exist_and_readable, check_int, check_float
 from simba.utils.printing import stdout_success
 import simba
 
@@ -40,18 +47,18 @@
 
     Examples
     ----------
     >>> select_labelling_video(config_path='MyConfigPath', threshold_dict={'Attack': 0.4}, file_path='MyVideoFilePath', setting='pseudo', continuing=False)
     """
 
     def __init__(self,
-                 config_path: str=None,
-                 file_path: str=None,
-                 setting: str = 'pseudo',  # from_scratch, #pseudo
-                 threshold_dict: dict=None,
+                 config_path: str,
+                 file_path: str,
+                 threshold_dict: Optional[Dict[str, float]] = None,
+                 setting: Literal['from_scratch', 'pseudo'] = 'pseudo',
                  continuing: bool=False):
 
         ConfigReader.__init__(self, config_path=config_path)
         self.padding, self.file_path = 5, file_path
         self.frm_no, self.threshold_dict = 0, threshold_dict
         self.setting = setting
         self.play_video_script_path = os.path.join(os.path.dirname(simba.__file__), 'play_annotation_video.py')
```

### Comparing `Simba-UW-tf-dev-1.58.7/simba/labelling/extract_labelled_frames.py` & `Simba-UW-tf-dev-1.58.8/simba/labelling/extract_labelled_frames.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 __author__ = "Simon Nilsson"
 
 import os.path
 import cv2
+from typing import List, Dict
+
 from simba.mixins.config_reader import ConfigReader
 from simba.utils.read_write import read_df, find_video_of_file, get_fn_ext, get_video_meta_data
 from simba.utils.printing import stdout_success
 from simba.utils.enums import Dtypes
 from simba.utils.errors import FrameRangeError
 from simba.utils.checks import check_that_column_exist
 
 
 class AnnotationFrameExtractor(ConfigReader):
     def __init__(self,
-                 clfs: list,
-                 settings: dict,
-                 config_path=str):
+                 clfs: List[int],
+                 settings: Dict[str, int],
+                 config_path: str):
         """
         Extracts all human annotated frames where behavior is annotated as present into .pngs within a SimBA project
 
         :param clfs: Names of classifiers to extract behavior-present images from.
         :param settings: User-defined settings. E.g., how much to downsample the png images.
         :param config_path: path to SimBA configparser.ConfigParser project_config.ini
```

### Comparing `Simba-UW-tf-dev-1.58.7/simba/labelling/labelling_advanced_interface.py` & `Simba-UW-tf-dev-1.58.8/simba/labelling/labelling_advanced_interface.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.7/simba/labelling/play_annotation_video.py` & `Simba-UW-tf-dev-1.58.8/simba/labelling/play_annotation_video.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.7/simba/unsupervised/dbcv_calculator.py` & `Simba-UW-tf-dev-1.58.8/simba/unsupervised/dbcv_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.7/simba/unsupervised/enums.py` & `Simba-UW-tf-dev-1.58.8/simba/unsupervised/enums.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.7/simba/unsupervised/.DS_Store` & `Simba-UW-tf-dev-1.58.8/simba/unsupervised/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.7/simba/unsupervised/dataset_creator.py` & `Simba-UW-tf-dev-1.58.8/simba/unsupervised/dataset_creator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.7/simba/unsupervised/grid_search_visualizers.py` & `Simba-UW-tf-dev-1.58.8/simba/unsupervised/grid_search_visualizers.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.7/simba/unsupervised/data_extractor.py` & `Simba-UW-tf-dev-1.58.8/simba/unsupervised/data_extractor.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.7/simba/unsupervised/ui.py` & `Simba-UW-tf-dev-1.58.8/simba/unsupervised/ui.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.7/simba/unsupervised/umap_embedder.py` & `Simba-UW-tf-dev-1.58.8/simba/unsupervised/umap_embedder.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.7/simba/unsupervised/pop_up_classes.py` & `Simba-UW-tf-dev-1.58.8/simba/unsupervised/pop_up_classes.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.7/simba/unsupervised/bout_aggregator.py` & `Simba-UW-tf-dev-1.58.8/simba/unsupervised/bout_aggregator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.7/simba/unsupervised/cluster_statistics.py` & `Simba-UW-tf-dev-1.58.8/simba/unsupervised/cluster_statistics.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.7/simba/unsupervised/data_map.yaml` & `Simba-UW-tf-dev-1.58.8/simba/unsupervised/data_map.yaml`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.7/simba/unsupervised/hdbscan_clusterer.py` & `Simba-UW-tf-dev-1.58.8/simba/unsupervised/hdbscan_clusterer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.7/simba/unsupervised/tsne.py` & `Simba-UW-tf-dev-1.58.8/simba/unsupervised/tsne.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.7/simba/unsupervised/cluster_visualizer.py` & `Simba-UW-tf-dev-1.58.8/simba/unsupervised/cluster_visualizer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.7/simba/bounding_box_tools/.DS_Store` & `Simba-UW-tf-dev-1.58.8/simba/bounding_box_tools/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.7/simba/bounding_box_tools/agg_boundary_stats.py` & `Simba-UW-tf-dev-1.58.8/simba/bounding_box_tools/agg_boundary_stats.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,15 +33,15 @@
     >>> boundary_stats_calculator.save()
     """
 
 
     def __init__(self,
                  config_path: str,
                  measures: list,
-                 shortest_allowed_interaction=int):
+                 shortest_allowed_interaction: int):
 
         ConfigReader.__init__(self, config_path=config_path)
         self.measures, self.shortest_allowed_interaction_ms = measures, shortest_allowed_interaction
         self.anchored_roi_path = os.path.join(self.project_path, 'logs', 'anchored_rois.pickle')
         self.data_path = os.path.join(self.project_path, 'csv', 'anchored_roi_data')
         if not os.path.isdir(self.data_path):
             raise NotDirectoryError(msg=f'SIMBA ERROR: No anchored roi statistics found in {self.data_path}. Create data before analyzing aggregate statistics')
```

### Comparing `Simba-UW-tf-dev-1.58.7/simba/bounding_box_tools/boundary_menus.py` & `Simba-UW-tf-dev-1.58.8/simba/bounding_box_tools/boundary_menus.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.7/simba/bounding_box_tools/boundary_statistics.py` & `Simba-UW-tf-dev-1.58.8/simba/bounding_box_tools/boundary_statistics.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.7/simba/bounding_box_tools/find_boundaries.py` & `Simba-UW-tf-dev-1.58.8/simba/bounding_box_tools/find_boundaries.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.7/simba/bounding_box_tools/visualize_boundaries.py` & `Simba-UW-tf-dev-1.58.8/simba/bounding_box_tools/visualize_boundaries.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.7/simba/.DS_Store` & `Simba-UW-tf-dev-1.58.8/simba/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.7/simba/feature_extractors/feature_extractor_14bp.py` & `Simba-UW-tf-dev-1.58.8/simba/feature_extractors/feature_extractor_14bp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.7/simba/feature_extractors/feature_extractor_7bp.py` & `Simba-UW-tf-dev-1.58.8/simba/feature_extractors/feature_extractor_7bp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.7/simba/feature_extractors/misc/doctests.py` & `Simba-UW-tf-dev-1.58.8/simba/feature_extractors/misc/doctests.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.7/simba/feature_extractors/misc/fish_feature_extractor_2023_version_3.py` & `Simba-UW-tf-dev-1.58.8/simba/feature_extractors/misc/fish_feature_extractor_2023_version_3.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.7/simba/feature_extractors/misc/read_in_mp.py` & `Simba-UW-tf-dev-1.58.8/simba/feature_extractors/misc/read_in_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.7/simba/feature_extractors/misc/peaks.py` & `Simba-UW-tf-dev-1.58.8/simba/feature_extractors/misc/peaks.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.7/simba/feature_extractors/misc/fish_feature_extractor_2022.py` & `Simba-UW-tf-dev-1.58.8/simba/feature_extractors/misc/fish_feature_extractor_2022.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.7/simba/feature_extractors/misc/convex_hull_3_scratch_3.py` & `Simba-UW-tf-dev-1.58.8/simba/feature_extractors/misc/convex_hull_3_scratch_3.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.7/simba/feature_extractors/misc/convex_hull_scratch_1.py` & `Simba-UW-tf-dev-1.58.8/simba/feature_extractors/misc/convex_hull_scratch_1.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.7/simba/feature_extractors/misc/.DS_Store` & `Simba-UW-tf-dev-1.58.8/simba/feature_extractors/misc/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.7/simba/feature_extractors/misc/fish_feature_extractor_2023_version_2.py` & `Simba-UW-tf-dev-1.58.8/simba/feature_extractors/misc/fish_feature_extractor_2023_version_2.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.7/simba/feature_extractors/misc/egocentrical_aligner.py` & `Simba-UW-tf-dev-1.58.8/simba/feature_extractors/misc/egocentrical_aligner.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.7/simba/feature_extractors/misc/count_values_in_range.py` & `Simba-UW-tf-dev-1.58.8/simba/feature_extractors/misc/count_values_in_range.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.7/simba/feature_extractors/misc/graph_creator.py` & `Simba-UW-tf-dev-1.58.8/simba/feature_extractors/misc/graph_creator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.7/simba/feature_extractors/misc/termite_rois.csv` & `Simba-UW-tf-dev-1.58.8/simba/feature_extractors/misc/termite_rois.csv`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.7/simba/feature_extractors/misc/mutual_exclusive.py` & `Simba-UW-tf-dev-1.58.8/simba/feature_extractors/misc/mutual_exclusive.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.7/simba/feature_extractors/misc/video_color.py` & `Simba-UW-tf-dev-1.58.8/simba/feature_extractors/misc/video_color.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.7/simba/feature_extractors/misc/graph_3d_plotter.py` & `Simba-UW-tf-dev-1.58.8/simba/feature_extractors/misc/graph_3d_plotter.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.7/simba/feature_extractors/misc/video_rotator.py` & `Simba-UW-tf-dev-1.58.8/simba/feature_extractors/misc/video_rotator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.7/simba/feature_extractors/misc/add_probability_cnt_features.py` & `Simba-UW-tf-dev-1.58.8/simba/feature_extractors/misc/add_probability_cnt_features.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.7/simba/feature_extractors/misc/make_splash.py` & `Simba-UW-tf-dev-1.58.8/simba/feature_extractors/misc/make_splash.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.7/simba/feature_extractors/misc/time_stamp_calculator.py` & `Simba-UW-tf-dev-1.58.8/simba/feature_extractors/misc/time_stamp_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.7/simba/feature_extractors/misc/video_rotator_mp.py` & `Simba-UW-tf-dev-1.58.8/simba/feature_extractors/misc/video_rotator_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.7/simba/feature_extractors/misc/fish_feature_extractor_2023_version_4.py` & `Simba-UW-tf-dev-1.58.8/simba/feature_extractors/misc/fish_feature_extractor_2023_version_4.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.7/simba/feature_extractors/misc/convex_hull_scratch_2.py` & `Simba-UW-tf-dev-1.58.8/simba/feature_extractors/misc/convex_hull_scratch_2.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.7/simba/feature_extractors/feature_extractor_8bps_2_animals.py` & `Simba-UW-tf-dev-1.58.8/simba/feature_extractors/feature_extractor_8bps_2_animals.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.7/simba/feature_extractors/.DS_Store` & `Simba-UW-tf-dev-1.58.8/simba/feature_extractors/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.7/simba/feature_extractors/perimeter_jit.py` & `Simba-UW-tf-dev-1.58.8/simba/feature_extractors/perimeter_jit.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.7/simba/feature_extractors/feature_subsets.py` & `Simba-UW-tf-dev-1.58.8/simba/feature_extractors/feature_subsets.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.7/simba/feature_extractors/__pycache__/perimeter_jit.quickhull_2d-16.py36m.nbi` & `Simba-UW-tf-dev-1.58.8/simba/feature_extractors/__pycache__/perimeter_jit.quickhull_2d-16.py36m.nbi`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.7/simba/feature_extractors/__pycache__/perimeter_jit.quickhull_2d-16.py36m.1.nbc` & `Simba-UW-tf-dev-1.58.8/simba/feature_extractors/__pycache__/perimeter_jit.quickhull_2d-16.py36m.1.nbc`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.7/simba/feature_extractors/__pycache__/perimeter_jit.process-7.py36m.1.nbc` & `Simba-UW-tf-dev-1.58.8/simba/feature_extractors/__pycache__/perimeter_jit.process-7.py36m.1.nbc`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.7/simba/feature_extractors/__pycache__/perimeter_jit.convex_hull_perimeter_2d-16.py36m.1.nbc` & `Simba-UW-tf-dev-1.58.8/simba/feature_extractors/__pycache__/perimeter_jit.convex_hull_perimeter_2d-16.py36m.1.nbc`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.7/simba/feature_extractors/__pycache__/perimeter_jit.process-7.py36m.2.nbc` & `Simba-UW-tf-dev-1.58.8/simba/feature_extractors/__pycache__/perimeter_jit.process-7.py36m.2.nbc`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.7/simba/feature_extractors/__pycache__/perimeter_jit.convex_hull_perimeter_2d-16.py36m.nbi` & `Simba-UW-tf-dev-1.58.8/simba/feature_extractors/__pycache__/perimeter_jit.convex_hull_perimeter_2d-16.py36m.nbi`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.7/simba/feature_extractors/__pycache__/perimeter_jit.process-7.py36m.nbi` & `Simba-UW-tf-dev-1.58.8/simba/feature_extractors/__pycache__/perimeter_jit.process-7.py36m.nbi`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.7/simba/feature_extractors/feature_extractor_user_defined.py` & `Simba-UW-tf-dev-1.58.8/simba/feature_extractors/feature_extractor_user_defined.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.7/simba/feature_extractors/feature_extractor_16bp.py` & `Simba-UW-tf-dev-1.58.8/simba/feature_extractors/feature_extractor_16bp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.7/simba/feature_extractors/feature_extractor_9bp.py` & `Simba-UW-tf-dev-1.58.8/simba/feature_extractors/feature_extractor_9bp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.7/simba/feature_extractors/feature_extractor_8bp.py` & `Simba-UW-tf-dev-1.58.8/simba/feature_extractors/feature_extractor_8bp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.7/simba/feature_extractors/feature_extractor_4bp.py` & `Simba-UW-tf-dev-1.58.8/simba/feature_extractors/feature_extractor_4bp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.7/simba/feature_extractors/.idea/features_scripts.iml` & `Simba-UW-tf-dev-1.58.8/simba/feature_extractors/.idea/features_scripts.iml`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.7/simba/feature_extractors/.idea/inspectionProfiles/Project_Default.xml` & `Simba-UW-tf-dev-1.58.8/simba/feature_extractors/.idea/inspectionProfiles/Project_Default.xml`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.7/simba/feature_extractors/.idea/workspace.xml` & `Simba-UW-tf-dev-1.58.8/simba/feature_extractors/.idea/workspace.xml`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.7/simba/requirements.txt` & `Simba-UW-tf-dev-1.58.8/simba/requirements.txt`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.7/simba/mixins/.DS_Store` & `Simba-UW-tf-dev-1.58.8/simba/mixins/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.7/simba/mixins/pop_up_mixin.py` & `Simba-UW-tf-dev-1.58.8/simba/mixins/pop_up_mixin.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.7/simba/mixins/config_reader.py` & `Simba-UW-tf-dev-1.58.8/simba/mixins/config_reader.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.7/simba/mixins/pose_importer_mixin.py` & `Simba-UW-tf-dev-1.58.8/simba/mixins/pose_importer_mixin.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.7/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-182.py36m.nbi` & `Simba-UW-tf-dev-1.58.8/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-182.py36m.nbi`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.7/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-183.py36m.1.nbc` & `Simba-UW-tf-dev-1.58.8/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-183.py36m.1.nbc`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.7/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-190.py36m.nbi` & `Simba-UW-tf-dev-1.58.8/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-190.py36m.nbi`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.7/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-190.py36m.1.nbc` & `Simba-UW-tf-dev-1.58.8/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-190.py36m.1.nbc`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.7/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-183.py36m.nbi` & `Simba-UW-tf-dev-1.58.8/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-183.py36m.nbi`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.7/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-182.py36m.1.nbc` & `Simba-UW-tf-dev-1.58.8/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-182.py36m.1.nbc`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.7/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-181.py36m.1.nbc` & `Simba-UW-tf-dev-1.58.8/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-181.py36m.1.nbc`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.7/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-181.py36m.nbi` & `Simba-UW-tf-dev-1.58.8/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-181.py36m.nbi`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.7/simba/mixins/feature_extraction_mixin.py` & `Simba-UW-tf-dev-1.58.8/simba/mixins/feature_extraction_mixin.py`

 * *Files 2% similar despite different names*

```diff
@@ -193,14 +193,20 @@
     def cdist(array_1: np.array, array_2: np.array):
         results = np.full((array_1.shape[0], array_2.shape[0]), np.nan)
         for i in prange(array_1.shape[0]):
             for j in prange(array_2.shape[0]):
                 results[i][j] = np.linalg.norm(array_1[i] - array_2[j])
         return results
 
+    @staticmethod
+    def create_shifted_df(df: pd.DataFrame):
+        data_df_shifted = df.shift(periods=1)
+        data_df_shifted = data_df_shifted.combine_first(df).add_suffix('_shifted')
+        return pd.concat([df, data_df_shifted], axis=1, join='inner').reset_index(drop=True)
+
     def check_directionality_viable(self):
         """
         Helper to check if it is possible to calculate ``directionality`` statistics (i.e., nose, and ear coordinates from
         pose estimation has to be present)
 
         Parameters
         ----------
```

### Comparing `Simba-UW-tf-dev-1.58.7/simba/mixins/plotting_mixin.py` & `Simba-UW-tf-dev-1.58.8/simba/mixins/plotting_mixin.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.7/simba/mixins/unsupervised_mixin.py` & `Simba-UW-tf-dev-1.58.8/simba/mixins/unsupervised_mixin.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.7/simba/mixins/train_model_mixin.py` & `Simba-UW-tf-dev-1.58.8/simba/mixins/train_model_mixin.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.7/simba/third_party_label_appenders/deepethogram_importer.py` & `Simba-UW-tf-dev-1.58.8/simba/third_party_label_appenders/deepethogram_importer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.7/simba/third_party_label_appenders/BORIS_appender.py` & `Simba-UW-tf-dev-1.58.8/simba/third_party_label_appenders/BORIS_appender.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.7/simba/third_party_label_appenders/observer_importer.py` & `Simba-UW-tf-dev-1.58.8/simba/third_party_label_appenders/observer_importer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.7/simba/third_party_label_appenders/tools.py` & `Simba-UW-tf-dev-1.58.8/simba/third_party_label_appenders/tools.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,31 +1,33 @@
 import pandas as pd
 import numpy as np
+from typing import List, Dict
+
 from simba.utils.data import detect_bouts
 from simba.utils.read_write import get_fn_ext, read_video_info
 from simba.utils.enums import Methods
 from simba.utils.warnings import ThirdPartyAnnotationsInvalidFileFormatWarning
 from simba.utils.errors import (InvalidFileTypeError, ColumnNotFoundError)
 
-def observer_timestamp_corrector(timestamps=list):
+def observer_timestamp_corrector(timestamps: List[str]) -> List[str]:
     corrected_ts = []
     for timestamp in timestamps:
         h, m, s = timestamp.split(':', 3)
         missing_fractions = 9 - len(s)
         if missing_fractions == 0:
             corrected_ts.append(timestamp)
         else:
             corrected_ts.append(f'{h}:{m}:{s}.{"0" * missing_fractions}')
     return corrected_ts
 
 
-def read_boris_annotation_files(data_paths: list,
+def read_boris_annotation_files(data_paths: List[str],
                                 error_setting: str,
                                 video_info_df: pd.DataFrame,
-                                log_setting: bool=False):
+                                log_setting: bool=False) -> Dict[str, pd.DataFrame]:
 
     MEDIA_FILE_PATH = 'Media file path'
     OBSERVATION_ID = 'Observation id'
     TIME = 'Time'
     BEHAVIOR = 'Behavior'
     STATUS = 'Status'
     EXPECTED_HEADERS = [TIME, MEDIA_FILE_PATH, BEHAVIOR, STATUS]
@@ -63,18 +65,18 @@
 #
 # df = read_boris_annotation_files(data_paths=['/Users/simon/Downloads/FIXED/c_oxt27_190816_122013_s_trimmcropped.csv'],
 #                                 error_setting='WARNING',
 #                                  log_setting=False,
 #                                  video_info_df=video_info_df)
 
 
-def read_ethovision_files(data_paths: list,
+def read_ethovision_files(data_paths: List[str],
                           error_setting: str,
                           video_info_df: pd.DataFrame,
-                          log_setting: bool=False):
+                          log_setting: bool=False) -> Dict[str, pd.DataFrame]:
 
     VIDEO_FILE = 'Video file'
     HEADER_LINES = 'Number of header lines:'
     RECORDING_TIME = 'Recording time'
     BEHAVIOR = 'Behavior'
     EVENT = 'Event'
     POINT_EVENT = 'point event'
@@ -125,18 +127,18 @@
 # df = read_ethovision_files(data_paths=['/Users/simon/Desktop/envs/simba_dev/tests/test_data/import_tests/ethovision_data/correct.xlsx'],
 #                                 error_setting='WARNING',
 #                                  log_setting=False,
 #                                  video_info_df=video_info_df)
 #
 
 
-def read_observer_files(data_paths: list,
+def read_observer_files(data_paths: List[str],
                         error_setting: str,
                         video_info_df: pd.DataFrame,
-                        log_setting: bool=False):
+                        log_setting: bool=False) -> Dict[str, pd.DataFrame]:
 
     TIME_FIELD = 'Time_Relative_hmsf'
     VIDEO_NAME_FIELD = 'Observation'
     BEHAVIOR_FIELD = 'Behavior'
     EVENT_TYPE_FIELD = 'Event_Type'
     POINT_EVENT = 'Point'
     START = 'State start'
@@ -183,18 +185,18 @@
 #
 # df = read_observer_files(data_paths=['/Users/simon/Desktop/envs/troubleshooting/Gosia/source/behaviours/Exp_38/03+11WT_20171010-120856_4_no_dupl_no_audio_fps4_grey-simba_crop_frame_n.xlsx'],
 #                          error_setting='WARNING',
 #                          log_setting=False,
 #                         video_info_df=video_info_df)
 
 
-def read_solomon_files(data_paths: list,
+def read_solomon_files(data_paths: List[str],
                         error_setting: str,
                         video_info_df: pd.DataFrame,
-                        log_setting: bool=False):
+                        log_setting: bool=False) -> Dict[str, pd.DataFrame]:
 
     BEHAVIOR = 'Behaviour'
     TIME = 'Time'
     EXPECTED_COLUMNS = [TIME, BEHAVIOR]
 
     dfs = {}
     for file_cnt, file_path in enumerate(data_paths):
@@ -233,18 +235,19 @@
 # df = read_solomon_files(data_paths=['/Users/simon/Desktop/envs/simba_dev/tests/test_data/solomon_import/solomon_import/Together_1.csv'],
 #                          error_setting='WARNING',
 #                          log_setting=False,
 #                          video_info_df=video_info_df)
 
 
 
-def read_bento_files(data_paths: list,
+def read_bento_files(data_paths: List[str],
                      error_setting: str,
                      video_info_df: pd.DataFrame,
-                     log_setting: bool=False):
+                     log_setting: bool=False) -> Dict[str, pd.DataFrame]:
+
     BENTO = 'Bento'
     CHANNEL = 'Ch1----------'
 
     dfs = {}
     for file_cnt, file_path in enumerate(data_paths):
         _, video_name, ext = get_fn_ext(filepath=file_path)
         _, _, fps = read_video_info(vid_info_df=video_info_df, video_name=video_name)
@@ -286,17 +289,17 @@
 #                          log_setting=False,
 #                          video_info_df=video_info_df)
 
 
 
 
 
-def read_deepethogram_files(data_paths: list,
+def read_deepethogram_files(data_paths: List[str],
                              error_setting: str,
-                             log_setting: bool=False):
+                             log_setting: bool=False) -> Dict[str, pd.DataFrame]:
 
     BACKGROUND = 'background'
     dfs = {}
     for file_cnt, file_path in enumerate(data_paths):
         _, video_name, _ = get_fn_ext(file_path)
         try:
             data_df = pd.read_csv(file_path, index_col=0)
@@ -316,18 +319,18 @@
                 raise InvalidFileTypeError(msg=f'{file_path} is not a valid BORIS file. See the docs for expected file format.')
             else:
                 pass
 
 
     return dfs
 
-def fix_uneven_start_stop_count(data: pd.DataFrame):
+def fix_uneven_start_stop_count(data: pd.DataFrame) -> pd.DataFrame:
+
     starts = data['FRAME'][data['EVENT'] == 'START'].values
     stops = data['FRAME'][data['EVENT'] == 'STOP'].values
-
     if starts.shape[0] < stops.shape[0]:
         sorted_stops = np.sort(stops)
         for start in starts:
             stop_idx = np.argwhere(sorted_stops>start)[0][0]
             sorted_stops = np.delete(sorted_stops, stop_idx)
         for remove_val in sorted_stops:
             remove_idx = np.argwhere(stops==remove_val)[0][0]
@@ -341,13 +344,13 @@
         for remove_val in sorted_starts:
             remove_idx = np.argwhere(starts==remove_val)[0][0]
             starts = np.delete(starts, remove_idx)
 
 
     return pd.DataFrame({'START': starts, 'STOP': stops})
 
-def check_stop_events_prior_to_start_events(df: pd.DataFrame):
+def check_stop_events_prior_to_start_events(df: pd.DataFrame) -> List[int]:
     overlaps_idx = []
     for obs_cnt, obs in enumerate(df.values):
         if obs[0] > obs[1]:
             overlaps_idx.append(obs_cnt)
     return overlaps_idx
```

### Comparing `Simba-UW-tf-dev-1.58.7/simba/third_party_label_appenders/third_party_appender.py` & `Simba-UW-tf-dev-1.58.8/simba/third_party_label_appenders/third_party_appender.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.7/simba/third_party_label_appenders/ethovision_import.py` & `Simba-UW-tf-dev-1.58.8/simba/third_party_label_appenders/ethovision_import.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.7/simba/third_party_label_appenders/BENTO_appender.py` & `Simba-UW-tf-dev-1.58.8/simba/third_party_label_appenders/BENTO_appender.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 __author__ = "Simon Nilsson"
 
-
 import os, glob
 import pandas as pd
 from copy import deepcopy
 from simba.mixins.config_reader import ConfigReader
 from simba.utils.checks import check_if_filepath_list_is_empty
 from simba.utils.read_write import get_fn_ext, read_df, write_df
 from simba.utils.printing import stdout_success
```

### Comparing `Simba-UW-tf-dev-1.58.7/simba/third_party_label_appenders/solomon_importer.py` & `Simba-UW-tf-dev-1.58.8/simba/third_party_label_appenders/solomon_importer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.7/simba/cue_light_tools/.DS_Store` & `Simba-UW-tf-dev-1.58.8/simba/cue_light_tools/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.7/simba/cue_light_tools/cue_light_clf_statistics.py` & `Simba-UW-tf-dev-1.58.8/simba/cue_light_tools/cue_light_clf_statistics.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.7/simba/cue_light_tools/cue_light_analyzer.py` & `Simba-UW-tf-dev-1.58.8/simba/cue_light_tools/cue_light_analyzer.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 __author__ = "Simon Nilsson"
 
-
 from sklearn.cluster import KMeans
 import os, glob
 import itertools
 import pandas as pd
 import cv2
 import numpy as np
 import multiprocessing
@@ -15,16 +14,14 @@
 from simba.utils.data import detect_bouts
 from simba.utils.printing import stdout_success
 from simba.utils.errors import NoFilesFoundError, CountError, NoROIDataError
 from simba.mixins.config_reader import ConfigReader
 from simba.utils.warnings import NoDataFoundWarning
 
 
-
-
 def get_intensity_scores_in_rois(frm_list: list=None,
                                  video_path: str = None,
                                  rectangles_df: pd.DataFrame = None,
                                  polygon_df: pd.DataFrame = None,
                                  circles_df: pd.DataFrame = None):
     cap = cv2.VideoCapture(video_path)
     start, end = frm_list[0], frm_list[-1]
```

### Comparing `Simba-UW-tf-dev-1.58.7/simba/cue_light_tools/cue_light_menues.py` & `Simba-UW-tf-dev-1.58.8/simba/cue_light_tools/cue_light_menues.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.7/simba/cue_light_tools/cue_light_tools.py` & `Simba-UW-tf-dev-1.58.8/simba/cue_light_tools/cue_light_tools.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.7/simba/cue_light_tools/cue_light_visualizer.py` & `Simba-UW-tf-dev-1.58.8/simba/cue_light_tools/cue_light_visualizer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.7/simba/cue_light_tools/cue_light_movement_statistics.py` & `Simba-UW-tf-dev-1.58.8/simba/cue_light_tools/cue_light_movement_statistics.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.7/simba/utils/config_creator.py` & `Simba-UW-tf-dev-1.58.8/simba/utils/config_creator.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 __author__ = "Simon Nilsson"
 
 import os
 import platform
 from configparser import ConfigParser
 import csv
+from typing import List
 
 import simba
 from simba.utils.printing import stdout_success, SimbaTimer
 from simba.utils.errors import DirectoryExistError
 from simba.utils.enums import (DirNames,
                                ConfigKey,
                                Dtypes,
@@ -45,15 +46,15 @@
     >>> _ = ProjectConfigCreator(project_path = 'project/path', project_name='project_name', target_list=['Attack'], pose_estimation_bp_cnt='16', body_part_config_idx=9, animal_cnt=2, file_type='csv')
 
     """
 
     def __init__(self,
                  project_path: str,
                  project_name: str,
-                 target_list: list,
+                 target_list: List[str],
                  pose_estimation_bp_cnt: str,
                  body_part_config_idx: int,
                  animal_cnt: int,
                  file_type: str = 'csv'):
 
         self.simba_dir = os.path.dirname(simba.__file__)
         self.animal_cnt = animal_cnt
```

### Comparing `Simba-UW-tf-dev-1.58.7/simba/utils/enums.py` & `Simba-UW-tf-dev-1.58.8/simba/utils/enums.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.7/simba/utils/.DS_Store` & `Simba-UW-tf-dev-1.58.8/simba/utils/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.7/simba/utils/warnings.py` & `Simba-UW-tf-dev-1.58.8/simba/utils/warnings.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.7/simba/utils/checks.py` & `Simba-UW-tf-dev-1.58.8/simba/utils/checks.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,36 +1,40 @@
 __author__ = "Simon Nilsson"
 
 import os
 import trafaret as t
 import pandas as pd
+from typing import Any, Optional, Tuple, List
+
 from simba.utils.errors import (NoFilesFoundError,
                                 CorruptedFileError,
                                 IntegerError,
                                 FloatError,
                                 StringError,
                                 NotDirectoryError,
                                 ColumnNotFoundError,
                                 InvalidInputError)
 
-def check_file_exist_and_readable(file_path: str):
+
+def check_file_exist_and_readable(file_path: str) -> None:
     """ Checks if a path points to a readable file"""
     if not os.path.isfile(file_path):
         raise NoFilesFoundError(msg=f'{file_path} is not a valid file path')
     elif not os.access(file_path, os.R_OK):
         raise CorruptedFileError(msg=f'{file_path} is not readable')
     else:
         pass
 
 
 def check_int(name: str,
-              value: None,
-              max_value=None,
-              min_value=None,
-              raise_error: bool=True):
+              value: Any,
+              max_value: Optional[int] = None,
+              min_value: Optional[int] = None,
+              raise_error: bool=True) -> (bool, str):
+
     msg = ''
     try:
         t.Int().check(value)
     except t.DataError as e:
         msg=f'{name} should be an integer number in SimBA, but is set to {str(value)}'
         if raise_error:
             raise IntegerError(msg=msg)
@@ -50,18 +54,18 @@
                 raise IntegerError(msg=msg)
             else:
                 return False, msg
     return True, msg
 
 
 def check_str(name: str,
-              value: None,
-              options=(),
-              allow_blank=False,
-              raise_error: bool = True):
+              value: Any,
+              options: Tuple[str, ...] = (),
+              allow_blank: bool = False,
+              raise_error: bool = True) -> (bool, str):
     msg = ''
     try:
         t.String(allow_blank=allow_blank).check(value)
     except t.DataError as e:
         msg = f'{name} should be an string in SimBA, but is set to {str(value)}'
         if raise_error:
             raise StringError(msg=msg)
@@ -77,18 +81,18 @@
         else:
             return True, msg
     else:
         return True, msg
 
 
 def check_float(name: str,
-                value=None,
-                max_value=None,
-                min_value=None,
-                raise_error: bool=True):
+                value: Any,
+                max_value: Optional[float] = None,
+                min_value: Optional[float] = None,
+                raise_error: bool = True) -> (bool, str):
     msg = ''
     try:
         t.Float().check(value)
     except t.DataError as e:
         msg = f'{name} should be a float number in SimBA, but is set to {str(value)}'
         if raise_error:
             raise FloatError(msg=msg)
@@ -107,37 +111,38 @@
             if raise_error:
                 raise FloatError(msg=msg)
             else:
                 return False, msg
     return True, msg
 
 
-def check_if_filepath_list_is_empty(filepaths: list,
-                                    error_msg: str):
+def check_if_filepath_list_is_empty(filepaths: List[str],
+                                    error_msg: str) -> None:
     if len(filepaths) == 0:
         raise NoFilesFoundError(msg=error_msg)
     else:
         pass
 
 
 def check_if_dir_exists(in_dir: str):
     if not os.path.isdir(in_dir):
         raise NotDirectoryError(msg=f'{in_dir} is not a valid directory')
 
 
 def check_that_column_exist(df: pd.DataFrame,
                             column_name: str,
-                            file_name: str):
+                            file_name: str) -> None:
+
     if column_name not in df.columns:
         raise ColumnNotFoundError(column_name=column_name, file_name=file_name)
 
 def check_if_valid_input(name: str,
                          input: str,
-                         options: list,
-                         raise_error: bool=True):
+                         options: List[str],
+                         raise_error: bool = True) -> (bool, str):
     msg = ''
     if input not in options:
         msg = f'{name} is set to {str(input)}, which is an invalid setting. OPTIONS {options}'
         if raise_error:
             raise InvalidInputError(msg=msg)
         else:
             return False, msg
```

### Comparing `Simba-UW-tf-dev-1.58.7/simba/utils/read_write.py` & `Simba-UW-tf-dev-1.58.8/simba/utils/read_write.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,14 +11,17 @@
 import numpy as np
 import pickle
 import cv2
 from pyarrow import csv
 import os
 from pathlib import Path
 import multiprocessing
+from typing import List, Optional, Any, Union, Tuple, Dict
+
+
 from simba.utils.printing import SimbaTimer
 
 
 from simba.utils.errors import (InvalidFileTypeError,
                                 MissingProjectConfigEntryError,
                                 NotDirectoryError,
                                 InvalidInputError,
@@ -38,29 +41,27 @@
 
 
 PARSE_OPTIONS = csv.ParseOptions(delimiter=',')
 READ_OPTIONS = csv.ReadOptions(encoding='utf8')
 
 def read_df(file_path: str,
             file_type: str,
-            remove_columns: list or None = None,
-            usecols: list or None = None,
-            check_multiindex: bool = False):
+            remove_columns: Optional[List[str]] = None,
+            usecols: Optional[List[str]] = None,
+            check_multiindex: bool = False) -> pd.DataFrame:
 
     """
     Helper function to read single data file into memory.
 
     Parameters
     ----------
     file_path: str
         Path to data file.
     file_type: str
         Type of data. OPTIONS: 'parquet' or 'csv'.
-    idx: int,
-        Index column location. Default: 0.
     remove_columns: list or None,
         If list, then remove columns
     usecols: list or None,
         If list, keep columns
 
     Returns
     -------
@@ -101,15 +102,15 @@
         raise InvalidFileTypeError(msg=f'{file_type} is not a valid filetype OPTIONS: [pickle, csv, parquet]')
 
     return df
 
 def write_df(df: pd.DataFrame,
              file_type: str,
              save_path: str,
-             multi_idx_header: bool = False):
+             multi_idx_header: bool = False) -> None:
 
     """
     Helper function to save single dataframe from memory.
 
     Parameters
     ----------
     df: pd.DataFrame
@@ -146,15 +147,15 @@
                 pickle.dump(df, f, protocol=pickle.HIGHEST_PROTOCOL)
         except Exception as e:
             print(e.args[0])
             raise InvalidFileTypeError(msg='Data could not be saved as a pickle.')
     else:
         raise InvalidFileTypeError(msg=f'{file_type} is not a valid filetype OPTIONS: [csv, pickle, parquet]')
 
-def get_fn_ext(filepath: str):
+def get_fn_ext(filepath: str) -> (str, str, str):
     """
     Helper to split file path into three components: (i) directory, (ii) file name, and (iii) file extension.
     Parameters
     ----------
     filepath: str
         Path to file.
 
@@ -172,16 +173,16 @@
     dir_name = os.path.dirname(filepath)
     return dir_name, file_name, file_extension
 
 def read_config_entry(config: configparser.ConfigParser,
                       section: str,
                       option: str,
                       data_type: str,
-                      default_value=None,
-                      options=None):
+                      default_value: Optional[Any] = None,
+                      options: Optional[List] = None) -> Union[float, int, str]:
     try:
         if config.has_option(section, option):
             if data_type == Dtypes.FLOAT.value:
                 value = config.getfloat(section, option)
             elif data_type == Dtypes.INT.value:
                 value = config.getint(section, option)
             elif data_type == Dtypes.STR.value:
@@ -192,40 +193,41 @@
                     raise NotDirectoryError(msg=f'The SimBA config file includes paths to a folder ({value}) that does not exist.')
             if options != None:
                 if value not in options:
                     raise InvalidInputError(msg=f'{option} is set to {str(value)} in SimBA, but this is not among the valid options: ({options})')
                 else:
                     return value
             return value
+
         elif default_value != None:
             return default_value
         else:
             raise MissingProjectConfigEntryError(msg=f'SimBA could not find an entry for option {option} under section {section} in the project_config.ini. Please specify the settings in the settings menu.')
     except ValueError:
         if default_value != None:
             return default_value
         else:
             raise MissingProjectConfigEntryError(msg=f'SimBA could not find an entry for option {option} under section {section} in the project_config.ini. Please specify the settings in the settings menu.')
 
 
-def read_project_path_and_file_type(config: configparser.ConfigParser):
+def read_project_path_and_file_type(config: configparser.ConfigParser) -> (str, str):
     project_path = read_config_entry(config=config,
                                      section=ConfigKey.GENERAL_SETTINGS.value,
                                      option=ConfigKey.PROJECT_PATH.value,
                                      data_type=ConfigKey.FOLDER_PATH.value)
     file_type = read_config_entry(config=config,
                                   section=ConfigKey.GENERAL_SETTINGS.value,
                                   option=ConfigKey.FILE_TYPE.value,
                                   data_type=Dtypes.STR.value,
                                   default_value=Formats.CSV.value)
 
     return project_path, file_type
 
 
-def read_video_info_csv(file_path: str):
+def read_video_info_csv(file_path: str) -> pd.DataFrame:
 
     """
     Helper to read the project_folder/logs/video_info.csv of the SimBA project in as a pd.DataFrame
     Parameters
     ----------
     file_path: str
     Returns
@@ -251,19 +253,19 @@
 def read_config_file(config_path: str):
     """ Helper to read project_config.ini file"""
     config = ConfigParser()
     try:
         config.read(config_path)
     except Exception as e:
         print(e.args)
-        raise MissingProjectConfigEntryError(msg=f'{self.config_path} is not a valid project_config file. Please check the project_config.ini path.')
+        raise MissingProjectConfigEntryError(msg=f'{config_path} is not a valid project_config file. Please check the project_config.ini path.')
     return config
 
 
-def get_video_meta_data(video_path: str):
+def get_video_meta_data(video_path: str) -> dict:
     """
     Helper to read video metadata (fps, resolution, frame cnt etc.) from video file.
 
     Parameters
     ----------
     video_path: str
         Path to video file.
@@ -292,15 +294,15 @@
     for k, v in video_data.items():
         if v == 0:
             raise InvalidVideoFileError(msg=f'SIMBA WARNING: Video {video_data["video_name"]} has {k} of {str(v)} (full error video path: {video_path}).')
     video_data['resolution_str'] = str(f'{video_data["width"]} x {video_data["height"]}')
     video_data['video_length_s'] = int(video_data['frame_count'] / video_data['fps'])
     return video_data
 
-def remove_a_folder(folder_dir: str):
+def remove_a_folder(folder_dir: str) -> None:
     """Helper to remove a directory"""
     shutil.rmtree(folder_dir, ignore_errors=True)
 
 def concatenate_videos_in_folder(in_folder: str,
                                  save_path: str,
                                  video_format: str = 'mp4',
                                  remove_splits: bool = True) -> None:
@@ -347,17 +349,17 @@
     bp_headers = []
     for bp in body_parts_lst:
         c1, c2, c3 = (f'{bp}_x', f'{bp}_y', f'{bp}_p')
         bp_headers.extend((c1, c2, c3))
     return bp_headers
 
 def read_video_info(vid_info_df: pd.DataFrame,
-                    video_name: str):
+                    video_name: str) -> (pd.DataFrame, float, float):
     """
-    Helper to read the meta data (pixels per mm, resolution, fps etc) from the video_info.csv for a single input file
+    Helper to read the metadata (pixels per mm, resolution, fps etc) from the video_info.csv for a single input file
 
     Parameters
     ----------
     vid_info_df: pd.DataFrame
         Pandas dataframe representing the content of the project_folder/logs/video_info.csv of the SimBA project.
     video_name: str
         The name of the video without extension to get the meta data for.
@@ -381,15 +383,15 @@
             return video_settings, px_per_mm, fps
         except TypeError:
             raise ParametersFileError(msg=f'Make sure the videos that are going to be analyzed are represented with APPROPRIATE VALUES inside the project_folder/logs/video_info.csv file in your SimBA project. Could not interpret the fps, pixels per millimeter and/or fps as numerical values for video {video_name}')
 
 
 def find_all_videos_in_directory(directory: str,
                                  as_dict: bool = False,
-                                 video_formats: tuple = ('.avi', '.mp4', '.mov', '.flv', '.m4v')):
+                                 video_formats: Tuple[str] = ('.avi', '.mp4', '.mov', '.flv', '.m4v')) -> Union[dict, list]:
     """
     Helper to return list of all video file paths in a directory
 
     Parameters
     ----------
     directory: str
         Directory to search.
@@ -419,15 +421,15 @@
             video_dict[name] = video_path
         return video_dict
 
     return video_lst
 
 
 def find_video_of_file(video_dir: str,
-                       filename: str):
+                       filename: str) -> str:
     """
     Helper to find the video file that represents a data file.
 
     Parameters
     ----------
     video_dir: str
         Directory holding putative video file
@@ -453,15 +455,15 @@
     if return_path is None:
         NoFileFoundWarning(f'SimBA could not find a video file representing {filename} in the project video directory')
     return return_path
 
 
 def find_files_of_filetypes_in_directory(directory: str,
                                          extensions: list,
-                                         raise_warning: bool = True):
+                                         raise_warning: bool = True) -> list:
     """
     Helper to find all files in a folder with specified extensions
 
     Parameters
     ----------
     directory: str
         Directory holding files
@@ -484,15 +486,15 @@
         if ext.lower() in extensions:
             accepted_file_paths.append(file_path)
     if not accepted_file_paths and raise_warning:
         raise NoFileFoundWarning(msg=f'SimBA could not find any files with accepted extensions {extensions} in the {str(directory)} directory')
     return accepted_file_paths
 
 
-def convert_parquet_to_csv(directory: str):
+def convert_parquet_to_csv(directory: str) -> None:
     """
     Helper to convert all parquet files in a folder to csv format.
 
     Parameters
     ----------
     directory: str
         Path to directory holding parquet files
@@ -510,15 +512,15 @@
         if 'scorer' in df.columns:
             df = df.set_index('scorer')
         df.to_csv(new_file_path)
         print('Saved {}...'.format(new_file_path))
     stdout_success(msg=f'{str(len(files_found))} parquet files in {directory} converted to csv')
 
 
-def convert_csv_to_parquet(directory: str):
+def convert_csv_to_parquet(directory: str) -> None:
     """
     Helper to convert all csv files in a folder to parquet format.
 
     Parameters
     ----------
     directory: str
         Path to directory holding csv files
@@ -539,15 +541,15 @@
         new_file_path = os.path.join(directory, os.path.basename(file_path).replace('.csv', '.parquet'))
         df.to_parquet(new_file_path)
         print('Saved {}...'.format(new_file_path))
     stdout_success(msg=f'{str(len(files_found))} csv files in {directory} converted to parquet')
 
 
 def get_file_name_info_in_directory(directory: str,
-                                    file_type: str):
+                                    file_type: str) -> Dict[str, str]:
     """
     Helper to return dict of all file path with extension as values as basenames as keys.
     E.g., ['Video_1:, 'C:\project_folder\csv\machine_results\Video_1, ...]
 
     Parameters
     ----------
     directory: str
@@ -566,15 +568,15 @@
         _, file_name, ext = get_fn_ext(file_path)
         results[file_name] = file_path
 
     return results
 
 
 def archive_processed_files(config_path: str,
-                            archive_name: str):
+                            archive_name: str) -> None:
     """
     Helper to archive files within a SimBA project.
 
     Parameters
     ----------
     config_path: str
         Path to SimBA project ``project_config.ini``.
@@ -624,20 +626,20 @@
     video_archive_path = os.path.join(videos_dir, archive_name)
     if not os.path.exists(video_archive_path): os.mkdir(video_archive_path)
     for video_file in videos_file_paths:
         save_video_path = os.path.join(video_archive_path, os.path.basename(video_file))
         shutil.move(video_file, save_video_path)
     stdout_success(msg='Archiving completed')
 
-def str_2_bool(input_str: str):
+def str_2_bool(input_str: str) -> bool:
   return input_str.lower() in ("yes", "true", "1")
 
 
 
-def tabulate_clf_info(clf_path: str):
+def tabulate_clf_info(clf_path: str) -> None:
     """
     Helper to print the hyper-parameters and creation date of a pickled classifier.
 
     Parameters
     ----------
     clf_path: str
         Path to classifier
@@ -682,15 +684,15 @@
             ['NUMBER OF FEATURES', 'NUMBER OF TREES', 'CLASSIFIER CRITERION', 'CLASSIFIER_MIN_SAMPLE_LEAF',
              'CLASSIFIER_N_JOBS', 'CLASSIFIER VERBOSE SETTING', 'CLASSIFIER PATH', 'CLASSIFIER CREATION TIME'],
             [clf_features_no, clf_estimators, clf_criterion, clf_min_samples_leaf,
              clf_n_jobs, clf_verbose, clf_path, str(creation_time)]):
         print(name + ': ' + str(val))
 
 def get_all_clf_names(config: configparser.ConfigParser,
-                      target_cnt: int):
+                      target_cnt: int) -> List[str]:
     """
     Helper to get all classifier names in a SimBA project.
 
     Parameters
     ----------
     config:  configparser.ConfigParser
         Parsed SimBA project_config.ini
@@ -704,66 +706,66 @@
 
     model_names = []
     for i in range(target_cnt):
         entry_name = 'target_name_{}'.format(str(i+1))
         model_names.append(read_config_entry(config, ConfigKey.SML_SETTINGS.value, entry_name, data_type=Dtypes.STR.value))
     return model_names
 
-def read_meta_file(meta_file_path):
+def read_meta_file(meta_file_path) -> pd.DataFrame:
     return pd.read_csv(meta_file_path, index_col=False).to_dict(orient='records')[0]
 
 
-def read_simba_meta_files(folder_path: str):
+def read_simba_meta_files(folder_path: str) -> List[str]:
     file_paths = find_files_of_filetypes_in_directory(directory=folder_path, extensions=['.csv'])
     meta_file_lst = []
     for i in file_paths:
         if i.__contains__("meta"):
             meta_file_lst.append(os.path.join(folder_path, i))
     if len(meta_file_lst) == 0:
         NoFileFoundWarning(msg=f'The training meta-files folder in your project ({folder_path}) does not have any meta files inside it (no files in this folder has the "meta" substring in the filename)')
     return meta_file_lst
 
 
-def find_core_cnt():
+def find_core_cnt() -> (int, int):
     """
     Helper to find the local cpu count and half of the cpu counts.
 
     Returns
     -------
     cpu_cnt: int
     cpu_cnt_to_use: int
     """
     cpu_cnt = multiprocessing.cpu_count()
     cpu_cnt_to_use = int(cpu_cnt / 4)
     if cpu_cnt_to_use < 1:
         cpu_cnt_to_use = 1
     return cpu_cnt, cpu_cnt_to_use
 
-def get_number_of_header_columns_in_df(df: pd.DataFrame):
+def get_number_of_header_columns_in_df(df: pd.DataFrame) -> int:
     """ Returns the number of non-numerical header rows in dataframe """
     for i in range(len(df)):
         try:
             temp = df.iloc[i:].apply(pd.to_numeric).reset_index(drop=True)
             return i
         except ValueError:
             pass
     raise DataHeaderError(msg='Could find the count of header columns in dataframe')
 
-def get_memory_usage_of_df(df: pd.DataFrame) -> dict:
+def get_memory_usage_of_df(df: pd.DataFrame) -> Dict[str, float]:
     results = {}
     results['bytes'] = df.memory_usage(index=True).sum()
     results['megabytes'] = round(results['bytes'] / 1000000, 6)
     results['gigabytes'] = round(results['bytes'] / 1000000000, 6)
     return results
 
 
 
 def copy_single_video_to_project(simba_ini_path: str,
                                  source_path: str,
-                                 allowed_video_formats: tuple = ('avi', 'mp4')) -> None:
+                                 allowed_video_formats: Tuple[str] = ('avi', 'mp4')) -> None:
     """ Helper to import single video file to SimBA project
 
     Parameters
     ----------
     simba_ini_path: str
         path to SimBA project config file in Configparser format
     source_path: str
@@ -788,15 +790,15 @@
         stdout_success(msg=f'Video {file_name} imported to SimBA project (project_folder/videos directory', elapsed_time=timer.elapsed_time_str)
 
 
 
 def copy_multiple_videos_to_project(config_path: str,
                                     source: str,
                                     file_type: str,
-                                    allowed_video_formats: tuple = ('avi', 'mp4')) -> None:
+                                    allowed_video_formats: Tuple[str] = ('avi', 'mp4')) -> None:
     """ Helper to import directory of videos to SimBA project
 
     Parameters
     ----------
     config_path: str
         path to SimBA project config file in Configparser format
     source_path: str
@@ -829,15 +831,15 @@
             timer.stop_timer()
             print('{} copied to project (Video {}/{}, elapsed timer {}s)...'.format(filebasename, str(file_cnt + 1),
                                                                                     str(len(video_path_lst)),
                                                                                     timer.elapsed_time_str))
     stdout_success(msg=f'{str(len(video_path_lst))} videos copied to project.')
 
 def find_all_videos_in_project(videos_dir: str,
-                               basename: bool=False):
+                               basename: bool = False) -> List[str]:
     """ Returns filenames of .avi and .mp4 files in a directory"""
     video_paths = []
     file_paths_in_folder = [f for f in next(os.walk(videos_dir))[2] if not f[0] == '.']
     file_paths_in_folder = [os.path.join(videos_dir, f) for f in file_paths_in_folder]
     for file_cnt, file_path in enumerate(file_paths_in_folder):
         try:
             _, file_name, file_ext = get_fn_ext(file_path)
```

### Comparing `Simba-UW-tf-dev-1.58.7/simba/utils/lookups.py` & `Simba-UW-tf-dev-1.58.8/simba/utils/lookups.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.7/simba/utils/errors.py` & `Simba-UW-tf-dev-1.58.8/simba/utils/errors.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.7/simba/utils/data.py` & `Simba-UW-tf-dev-1.58.8/simba/utils/data.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 __author__ = "Simon Nilsson"
 
 import pandas as pd
 from copy import deepcopy
 import configparser
 from pathlib import Path
-import ast, os
+import ast
 from scipy.signal import savgol_filter
 from pylab import *
+from typing import List
+
 from simba.utils.read_write import (get_fn_ext,
                                     read_project_path_and_file_type,
                                     find_video_of_file,
                                     read_df,
                                     write_df,
                                     read_config_entry,
                                     get_video_meta_data)
@@ -19,16 +21,16 @@
 from simba.utils.printing import stdout_warning
 from simba.utils.enums import ConfigKey, Dtypes
 
 
 
 
 def detect_bouts(data_df: pd.DataFrame,
-                 target_lst: list,
-                 fps: int):
+                 target_lst: List[str],
+                 fps: int) -> pd.DataFrame:
     """
     Helper to detect all behavior bouts for a list of classifiers, or e.g., bouts of being within ROIs.
 
     Parameters
     ----------
     data_df: pd.DataFrame
         Pandas Dataframe with classifier prediction data.
@@ -68,15 +70,15 @@
     return pd.DataFrame(list(zip(nameList, startTimeList, endTimeList, startFrameLst, endFrameList, boutsList)),
                         columns=['Event', 'Start_time', 'End Time', 'Start_frame', 'End_frame', 'Bout_time'])
 
 
 def plug_holes_shortest_bout(data_df: pd.DataFrame,
                              clf_name: str,
                              fps: int,
-                             shortest_bout: int):
+                             shortest_bout: int) -> pd.DataFrame:
     """
 
     Parameters
     ----------
     data_df: pd.DataFrame
         Pandas Dataframe with classifier prediction data.
     clf_name: str
@@ -133,15 +135,15 @@
         data_df.loc[data_df['rolling_match'] == True, clf_name] = 0
         data_df = data_df.drop(['rolling_match'], axis=1)
 
     return data_df
 
 
 def create_color_palettes(no_animals: int,
-                          map_size: int):
+                          map_size: int) -> List[List[int]]:
     """
     Helper to return a list of lists of bgr colors. Each list is pulled from a different palette
     matplotlib color map.
 
     Parameters
     ----------
     no_animals: int
@@ -155,15 +157,15 @@
         Bgr colors
 
     Notes
     -----
 
     Examples
     -----
-    >>> colorListofList = createColorListofList(no_animals=2, map_size=8)
+    >>> clr_lst_of_lst = create_color_palettes(no_animals=2, map_size=8)
     """
 
     colorListofList = []
     cmaps = ['spring',
             'summer',
             'autumn',
             'cool',
@@ -186,15 +188,15 @@
     return colorListofList
 
 
 
 def create_color_palette(pallete_name: str,
                          increments: int,
                          as_rgb_ratio: bool = False,
-                         as_hex: bool = False):
+                         as_hex: bool = False) -> list:
     """
     Helper to create a color palette of bgr colors in a list.
 
     Parameters
     ----------
     pallete_name: str
         Palette name (e.g., 'jet')
@@ -220,15 +222,15 @@
         color_lst.append(rgb)
     return color_lst
 
 
 
 def smooth_data_savitzky_golay(config: configparser.ConfigParser,
                                file_path: str,
-                               time_window_parameter=int):
+                               time_window_parameter: int) -> None:
     """
     Helper to perform Savitzky-Golay smoothing of pose-estimation data. Overwrites the input data with smoothened data.
 
     Parameters
     ----------
     config: configparser.ConfigParser
         Parsed SimBA project_config.ini file
@@ -240,16 +242,16 @@
     Returns
     -------
     None
 
     Example
     ----------
 
-    >>> config = read_config_file(ini_path='/Users/simon/Desktop/envs/troubleshooting/Tests_022023/project_folder/project_config.ini')
-    >>> smooth_data_savitzky_golay(config=config, file_path='/Users/simon/Desktop/envs/troubleshooting/Tests_022023/project_folder/csv/input_csv/Together_1.csv', time_window_parameter=500)
+    >>> config = read_config_file(ini_path='Tests_022023/project_folder/project_config.ini')
+    >>> smooth_data_savitzky_golay(config=config, file_path='Tests_022023/project_folder/csv/input_csv/Together_1.csv', time_window_parameter=500)
     """
 
     check_int(name='Savitzky-Golay time window', value=time_window_parameter)
     check_file_exist_and_readable(file_path)
     _, filename, _ = get_fn_ext(file_path)
     project_dir, file_format = read_project_path_and_file_type(config=config)
     video_dir = os.path.join(project_dir, 'videos')
@@ -272,15 +274,15 @@
         new_df[c] = new_df[c].abs()
     write_df(df=new_df, file_type=file_format, save_path=file_path)
     print(f'Savitzky-Golay smoothing complete for {filename}...')
 
 
 def smooth_data_gaussian(config: configparser.ConfigParser,
                          file_path: str,
-                         time_window_parameter: int):
+                         time_window_parameter: int) -> None:
     """
     Helper to perform Gaussian smoothing of pose-estimation data. Overwrites the input data with smoothened data.
 
     Parameters
     ----------
     config: configparser.ConfigParser
         Parsed SimBA project_config.ini file
@@ -315,15 +317,15 @@
 
     for c in new_df:
         new_df[c] = new_df[c].rolling(window=int(frames_in_time_window), win_type='gaussian', center=True).mean(std=5).fillna(new_df[c]).abs()
     write_df(df=new_df, file_type=file_format, save_path=file_path)
     print(f'Gaussian smoothing complete for file {filename}...')
 
 
-def add_missing_ROI_cols(shape_df: pd.DataFrame):
+def add_missing_ROI_cols(shape_df: pd.DataFrame) -> pd.DataFrame:
     """
     Helper to add missing ROI definitions in ROI info dataframes created by the first version of the SimBA ROI
     user-interface but analyzed using newer versions of SimBA.
 
     Parameters
     ----------
     shape_df: pd.DataFrame
@@ -341,15 +343,15 @@
     if not 'Color name' in shape_df.columns:
         shape_df['Color name'] = 'White'
 
     return shape_df
 
 
 def run_user_defined_feature_extraction_class(file_path: str,
-                                              config_path: str):
+                                              config_path: str) -> None:
     """
     Parameters
     ----------
     file_path: str
         Path to .py file holding user-defined feature extraction class
     config_path: str
         Path to SimBA project config file
```

### Comparing `Simba-UW-tf-dev-1.58.7/simba/utils/printing.py` & `Simba-UW-tf-dev-1.58.8/simba/utils/printing.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.7/simba/pose_processors/reorganize_keypoint.py` & `Simba-UW-tf-dev-1.58.8/simba/pose_processors/reorganize_keypoint.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 __author__ = "Simon Nilsson"
 
 import glob, os
 import pandas as pd
 from collections import OrderedDict
 from datetime import datetime
+from typing import Optional
+
 from simba.utils.checks import check_if_filepath_list_is_empty, check_if_dir_exists
 from simba.utils.printing import stdout_success
 from simba.utils.enums import Formats
 
 
 class KeypointReorganizer(object):
     """
@@ -34,15 +36,15 @@
     >>> keypoint_reorganizer = KeypointReorganizer(data_folder="test_data/misc_test_files", pose_tool='DLC', file_format='csv')
     >>> keypoint_reorganizer.perform_reorganization(bp_lst=['Ear_left_1', 'Ear_right_1', 'Nose_1', 'Center_1', 'Lateral_left_1', 'Lateral_right_1', 'Tail_base_1', 'Ear_left_2', 'Ear_right_2', 'Nose_2', 'Center_2', 'Lateral_left_2', 'Lateral_right_2', 'Tail_base_2'], animal_list=None)
     """
 
     def __init__(self,
                  data_folder: str,
                  pose_tool: str,
-                 file_format: str or None):
+                 file_format: Optional[str] = None):
 
 
         check_if_dir_exists(in_dir=data_folder)
         self.data_folder, self.pose_tool = data_folder, pose_tool
         self.file_format = file_format
         self.files_found = glob.glob(self.data_folder + '/*.' + file_format)
         check_if_filepath_list_is_empty(self.files_found,
```

### Comparing `Simba-UW-tf-dev-1.58.7/simba/pose_processors/remove_keypoints.py` & `Simba-UW-tf-dev-1.58.8/simba/pose_processors/remove_keypoints.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.7/simba/pose_processors/pose_reset.py` & `Simba-UW-tf-dev-1.58.8/simba/pose_processors/pose_reset.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 __author__ = "Simon Nilsson"
 
 import os
 import simba
 import shutil
 import pandas as pd
+from tkinter import *
+
 from simba.utils.printing import stdout_trash
 from simba.utils.lookups import get_bp_config_codes
 from simba.utils.checks import check_file_exist_and_readable
 
 
 class PoseResetter(object):
     """
@@ -24,15 +26,15 @@
 
     Examples
     ----------
     >>> _ = PoseResetter(master=None)
     """
 
     def __init__(self,
-                 master=None):
+                 master: Toplevel):
 
         self.default_pose_configs_cnt = len(get_bp_config_codes().keys())
         self.simba_dir = os.path.dirname(simba.__file__)
         self.pose_configs_dir = os.path.join(self.simba_dir, 'pose_configurations')
         self.archive_dir = os.path.join(self.simba_dir, 'pose_configurations_archive')
         if not os.path.exists(self.archive_dir): os.makedirs(self.archive_dir)
         self.archive_folders_cnt = len(os.listdir(self.archive_dir))
```

### Comparing `Simba-UW-tf-dev-1.58.7/simba/pose_processors/reverse_pose.py` & `Simba-UW-tf-dev-1.58.8/simba/pose_processors/reverse_pose.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import pandas as pd
 import shutil
 import os, glob
 from datetime import datetime
 
 from simba.feature_extractors.feature_extractor_16bp import ExtractFeaturesFrom16bps
 from simba.feature_extractors.feature_extractor_14bp import ExtractFeaturesFrom14bps
-from simba.feature_extractors.extract_features_9bp import extract_features_wotarget_9
+from simba.feature_extractors.feature_extractor_9bp import ExtractFeaturesFrom9bps
 from simba.feature_extractors.feature_extractor_8bp import ExtractFeaturesFrom8bps
 from simba.feature_extractors.feature_extractor_7bp import ExtractFeaturesFrom7bps
 from simba.feature_extractors.feature_extractor_4bp import ExtractFeaturesFrom4bps
 from simba.feature_extractors.feature_extractor_user_defined import UserDefinedFeatureExtractor
 from simba.mixins.config_reader import ConfigReader
 from simba.utils.read_write import read_config_entry, read_df, write_df, get_fn_ext, get_all_clf_names
 from simba.utils.checks import check_that_column_exist, check_file_exist_and_readable
```

### Comparing `Simba-UW-tf-dev-1.58.7/simba/plotting/gantt_creator.py` & `Simba-UW-tf-dev-1.58.8/simba/plotting/gantt_creator.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,14 +2,16 @@
 
 import os
 import numpy as np
 import matplotlib.pyplot as plt
 import io
 import cv2
 import PIL
+from typing import Dict, List
+
 from simba.utils.errors import NoSpecifiedOutputError
 from simba.utils.printing import stdout_success
 from simba.utils.lookups import get_named_colors
 from simba.utils.data import detect_bouts
 from simba.utils.enums import Formats
 from simba.mixins.config_reader import ConfigReader
 from simba.mixins.plotting_mixin import PlottingMixin
@@ -49,16 +51,16 @@
     """
 
     def __init__(self,
                  config_path: str,
                  frame_setting: bool,
                  video_setting: bool,
                  last_frm_setting: bool,
-                 files_found: list,
-                 style_attr: dict):
+                 files_found: List[str],
+                 style_attr: Dict[str, int]):
 
         ConfigReader.__init__(self, config_path=config_path)
         PlottingMixin.__init__(self)
         self.frame_setting, self.video_setting, self.style_attr, self.last_frm_setting = frame_setting, video_setting, style_attr, last_frm_setting
         self.files_found = files_found
         if (self.frame_setting != True) and (self.video_setting != True) and (self.last_frm_setting != True):
             raise NoSpecifiedOutputError(msg='SIMBA ERROR: Please select gantt videos, frames, and/or last frame.')
```

### Comparing `Simba-UW-tf-dev-1.58.7/simba/plotting/tools/tkinter_tools.py` & `Simba-UW-tf-dev-1.58.8/simba/plotting/tools/tkinter_tools.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.7/simba/plotting/ROI_plotter_mp.py` & `Simba-UW-tf-dev-1.58.8/simba/plotting/ROI_plotter_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.7/simba/plotting/.DS_Store` & `Simba-UW-tf-dev-1.58.8/simba/plotting/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.7/simba/plotting/shap_agg_stats_visualizer.py` & `Simba-UW-tf-dev-1.58.8/simba/plotting/shap_agg_stats_visualizer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.7/simba/plotting/gantt_creator_mp.py` & `Simba-UW-tf-dev-1.58.8/simba/plotting/gantt_creator_mp.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 __author__ = "Simon Nilsson"
 
 import warnings
 warnings.simplefilter(action='ignore', category=FutureWarning)
-import pandas as pd
 import os
 import numpy as np
 import cv2
 import multiprocessing
 import functools
 import shutil
 import platform
+from typing import List, Dict
+
 from simba.utils.errors import NoSpecifiedOutputError
 from simba.utils.printing import stdout_success, SimbaTimer
 from simba.utils.lookups import get_named_colors
 from simba.utils.read_write import concatenate_videos_in_folder, get_fn_ext, read_df
 from simba.utils.checks import check_if_filepath_list_is_empty
 from simba.utils.data import detect_bouts
 from simba.utils.enums import Formats
@@ -53,17 +54,17 @@
 
     """
 
     def __init__(self,
                  config_path: str,
                  frame_setting: bool,
                  video_setting: bool,
-                 files_found: list,
+                 files_found: List[str],
                  cores: int,
-                 style_attr: dict,
+                 style_attr: Dict[str, int],
                  last_frm_setting: bool):
 
         if platform.system() == "Darwin":
             multiprocessing.set_start_method('spawn', force=True)
 
         ConfigReader.__init__(self, config_path=config_path)
         PlottingMixin.__init__(self)
```

### Comparing `Simba-UW-tf-dev-1.58.7/simba/plotting/heat_mapper_clf_mp.py` & `Simba-UW-tf-dev-1.58.8/simba/plotting/heat_mapper_clf_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.7/simba/plotting/probability_plot_creator.py` & `Simba-UW-tf-dev-1.58.8/simba/plotting/probability_plot_creator.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 import matplotlib.pyplot as plt
 import cv2
 import PIL
 import io
 import numpy as np
 import os
+from typing import List, Dict
 
 from simba.utils.enums import Formats
 from simba.mixins.config_reader import ConfigReader
 from simba.mixins.plotting_mixin import PlottingMixin
 from simba.utils.errors import NoSpecifiedOutputError
 from simba.utils.read_write import read_df, get_fn_ext
 from simba.utils.printing import stdout_success, SimbaTimer
@@ -47,16 +48,16 @@
 
     def __init__(self,
                  config_path: str,
                  clf_name: str,
                  frame_setting: bool,
                  video_setting: bool,
                  last_image: bool,
-                 style_attr: dict,
-                 files_found: list):
+                 style_attr: Dict[str, int],
+                 files_found: List[str]):
 
         ConfigReader.__init__(self, config_path=config_path)
         PlottingMixin.__init__(self)
         self.frame_setting, self.video_setting, self.style_attr, self.last_image = frame_setting, video_setting, style_attr, last_image
         if (not self.frame_setting) and (not self.video_setting) and (not self.last_image):
             raise NoSpecifiedOutputError(msg='Please choose to either probability videos, probability frames, or both probability frames and videos.')
 
@@ -68,18 +69,17 @@
         if not os.path.exists(self.probability_plot_dir):
             os.makedirs(self.probability_plot_dir)
         print('Processing {} video(s)...'.format(str(len(self.files_found))))
         self.timer = SimbaTimer()
         self.timer.start_timer()
 
 
-    def create_plots(self):
+    def run(self):
         for file_cnt, file_path in enumerate(self.files_found):
-            video_timer = SimbaTimer()
-            video_timer.start_timer()
+            video_timer = SimbaTimer(start=True)
             _, self.video_name, _ = get_fn_ext(file_path)
             video_info, self.px_per_mm, fps = self.read_video_info(video_name=self.video_name)
             data_df = read_df(file_path, self.file_type)
             check_that_column_exist(df=data_df, column_name=self.clf_name, file_name=self.video_name)
             if self.frame_setting:
                 self.save_frame_folder_dir = os.path.join(self.probability_plot_dir, self.video_name + '_' + self.orginal_clf_name)
                 if not os.path.exists(self.save_frame_folder_dir): os.makedirs(self.save_frame_folder_dir)
```

### Comparing `Simba-UW-tf-dev-1.58.7/simba/plotting/plot_clf_results.py` & `Simba-UW-tf-dev-1.58.8/simba/plotting/plot_clf_results.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,14 +2,16 @@
 
 
 import os, glob
 from copy import deepcopy
 import cv2
 import numpy as np
 from PIL import Image
+from typing import Union, Dict, Optional, List
+
 from simba.mixins.config_reader import ConfigReader
 from simba.mixins.train_model_mixin import TrainModelMixin
 from simba.mixins.plotting_mixin import PlottingMixin
 from simba.utils.errors import NoSpecifiedOutputError
 from simba.utils.printing import stdout_success
 from simba.utils.enums import ConfigKey, Formats, Dtypes
 from simba.utils.read_write import get_fn_ext, read_df, get_video_meta_data, read_config_entry
@@ -44,18 +46,18 @@
     >>> clf_plotter.initialize_visualizations()
     """
 
     def __init__(self,
                  config_path: str,
                  video_setting: bool,
                  frame_setting: bool,
-                 text_settings: dict or bool,
-                 rotate: False,
-                 video_file_path=None,
-                 print_timers=True):
+                 text_settings: Union[Dict[str, float], bool],
+                 video_file_path: Optional[List] = None,
+                 rotate: bool = False,
+                 print_timers: bool = True):
 
         ConfigReader.__init__(self, config_path=config_path)
         TrainModelMixin.__init__(self)
         PlottingMixin.__init__(self)
 
         if (not video_setting) and (not frame_setting):
             raise NoSpecifiedOutputError(msg='Please choose to create a video and/or frames. SimBA found that you ticked neither video and/or frames')
```

### Comparing `Simba-UW-tf-dev-1.58.7/simba/plotting/plot_clf_results_mp.py` & `Simba-UW-tf-dev-1.58.8/simba/plotting/plot_clf_results_mp.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,14 +3,16 @@
 import os
 from copy import deepcopy
 import multiprocessing
 import cv2
 import numpy as np
 import functools
 import platform
+from typing import Optional, Dict, List, Union
+
 from simba.utils.errors import NoSpecifiedOutputError
 from simba.utils.printing import stdout_success, SimbaTimer
 from simba.utils.enums import ConfigKey, Formats, Dtypes
 from simba.utils.read_write import read_df, get_video_meta_data, concatenate_videos_in_folder, get_fn_ext, read_config_entry
 from simba.utils.checks import check_file_exist_and_readable, check_float, check_int
 from simba.utils.data import create_color_palette
 from simba.mixins.config_reader import ConfigReader
@@ -122,19 +124,19 @@
     >>> clf_plotter.initialize_visualizations()
     """
 
     def __init__(self,
                  config_path: str,
                  video_setting: bool,
                  frame_setting: bool,
-                 text_settings: dict or bool,
+                 text_settings: Union[Dict[str, float], bool],
                  cores: int,
-                 rotate: False,
-                 video_file_path=None,
-                 print_timers=True):
+                 video_file_path: Optional[str] = None,
+                 rotate: bool = False,
+                 print_timers: bool = True):
 
         ConfigReader.__init__(self, config_path=config_path)
         TrainModelMixin.__init__(self)
         PlottingMixin.__init__(self)
         if platform.system() == "Darwin":
             multiprocessing.set_start_method('spawn', force=True)
```

### Comparing `Simba-UW-tf-dev-1.58.7/simba/plotting/ROI_feature_visualizer.py` & `Simba-UW-tf-dev-1.58.8/simba/plotting/ROI_feature_visualizer.py`

 * *Files 0% similar despite different names*

```diff
@@ -34,16 +34,15 @@
     >>> roi_feature_visualizer = ROIfeatureVisualizer(config_path='MyProjectConfig', video_name='MyVideo.mp4')
     >>> roi_feature_visualizer.create_visualization()
     """
 
     def __init__(self,
                  config_path: str,
                  video_name: str,
-                 style_attr: dict
-                 ):
+                 style_attr: dict):
 
         super().__init__(config_path=config_path)
         _, self.video_name, _ = get_fn_ext(video_name)
         self.save_path = os.path.join(self.roi_features_save_dir, self.video_name + '.mp4')
         if not os.path.exists(self.roi_features_save_dir): os.makedirs(self.roi_features_save_dir)
         c_map_size, self.style_attr = int(len(self.x_cols) + 1), style_attr
         self.roi_feature_creator = ROIFeatureCreator(config_path=config_path)
```

### Comparing `Simba-UW-tf-dev-1.58.7/simba/plotting/heat_mapper_location.py` & `Simba-UW-tf-dev-1.58.8/simba/plotting/heat_mapper_location.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.7/simba/plotting/probability_plot_creator_mp.py` & `Simba-UW-tf-dev-1.58.8/simba/plotting/probability_plot_creator_mp.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 import pandas as pd
 import os
 import cv2
 import numpy as np
 import shutil
 import multiprocessing
 import platform
+from typing import List, Dict
 
 from simba.utils.printing import stdout_success, SimbaTimer
 from simba.utils.read_write import concatenate_videos_in_folder, read_df, get_fn_ext
 from simba.utils.errors import NoSpecifiedOutputError, ColumnNotFoundError
 from simba.utils.checks import check_that_column_exist
 from simba.utils.enums import Formats
 from simba.mixins.config_reader import ConfigReader
@@ -43,27 +44,27 @@
     ----------
     `Visualization tutorials <https://github.com/sgoldenlab/simba/blob/master/docs/tutorial.md#step-11-visualizations>`__.
 
 
     Examples
     ----------
     >>> plot_creator = TresholdPlotCreatorMultiprocess(config_path='/Users/simon/Desktop/troubleshooting/train_model_project/project_folder/project_config.ini', frame_setting=True, video_setting=True, clf_name='Attack', style_attr={'width': 640, 'height': 480, 'font size': 10, 'line width': 6, 'color': 'magneta', 'circle size': 20}, cores=5)
-    >>> plot_creator.create_plot()
+    >>> plot_creator.run()
     """
 
 
     def __init__(self,
                  config_path: str,
                  clf_name: str,
                  frame_setting: bool,
                  video_setting: bool,
                  last_frame: bool,
                  cores: int,
-                 style_attr: dict,
-                 files_found: list):
+                 style_attr: Dict[str, int],
+                 files_found: List[str]):
 
         ConfigReader.__init__(self,config_path=config_path)
         PlottingMixin.__init__(self)
         if platform.system() == "Darwin":
             multiprocessing.set_start_method('spawn', force=True)
         self.frame_setting, self.video_setting, self.cores, self.style_attr, self.last_frame = frame_setting, video_setting, cores, style_attr, last_frame
         if (not self.frame_setting) and (not self.video_setting) and (not self.last_frame):
@@ -72,18 +73,17 @@
         self.probability_col = 'Probability_' + self.clf_name
         self.fontsize = self.style_attr['font size']
         self.out_width, self.out_height = self.style_attr['width'], self.style_attr['height']
         self.fourcc = cv2.VideoWriter_fourcc(*Formats.MP4_CODEC.value)
         if not os.path.exists(self.probability_plot_dir): os.makedirs(self.probability_plot_dir)
         print(f'Processing {str(len(self.files_found))} video(s)...')
 
-    def create_plots(self):
+    def run(self):
         for file_cnt, file_path in enumerate(self.files_found):
-            video_timer = SimbaTimer()
-            video_timer.start_timer()
+            video_timer = SimbaTimer(start=True)
             _, self.video_name, _ = get_fn_ext(file_path)
             video_info, self.px_per_mm, self.fps = self.read_video_info(video_name=self.video_name)
             data_df = read_df(file_path, self.file_type)
             if self.probability_col not in data_df.columns:
                 raise ColumnNotFoundError(column_name=self.probability_col, file_name=file_path)
             check_that_column_exist(df=data_df, column_name=self.clf_name, file_name=self.video_name)
             self.save_frame_folder_dir = os.path.join(self.probability_plot_dir, self.video_name + '_' + self.clf_name)
```

### Comparing `Simba-UW-tf-dev-1.58.7/simba/plotting/interactive_probability_grapher.py` & `Simba-UW-tf-dev-1.58.8/simba/plotting/interactive_probability_grapher.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.7/simba/plotting/plot_pose_in_dir.py` & `Simba-UW-tf-dev-1.58.8/simba/plotting/plot_pose_in_dir.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,30 @@
 __author__ = "Simon Nilsson"
 
 import pandas as pd
 import cv2
 import os, glob
 from pathlib import Path
+from typing import Dict, Optional, Tuple
+
 from simba.utils.lookups import get_color_dict
 from simba.utils.printing import stdout_success, SimbaTimer
 from simba.utils.enums import Formats
 from simba.utils.errors import InvalidInputError
 from simba.utils.read_write import read_df, get_video_meta_data, get_fn_ext, find_video_of_file
 from simba.utils.checks import check_if_filepath_list_is_empty
 from simba.utils.data import create_color_palette
 
 
 ACCEPTED_DIRECTORIES = ['input_csv', 'outlier_corrected_movement', 'outlier_corrected_movement_location']
 
 def create_video_from_dir(in_directory: str,
                           out_directory: str,
                           circle_size: int,
-                          clr_attr: dict or None):
+                          clr_attr: Optional[Dict[str, Tuple[int, int, int]]] = None):
     """
     Class for creating pose-estimation visualizations from data within a SimBA project folder.
 
     Parameters
     ----------
     in_directory: str
         Path to SimBA project directory containing pose-estimation data in parquet or CSV format.
```

### Comparing `Simba-UW-tf-dev-1.58.7/simba/plotting/single_run_model_validation_video.py` & `Simba-UW-tf-dev-1.58.8/simba/plotting/single_run_model_validation_video.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,14 +4,16 @@
 warnings.filterwarnings('ignore',category=FutureWarning)
 warnings.filterwarnings('ignore',category=DeprecationWarning)
 import cv2
 import os
 import numpy as np
 import warnings
 import matplotlib.pyplot as plt
+from typing import Dict, Any
+
 from simba.utils.data import plug_holes_shortest_bout
 from simba.utils.printing import stdout_success
 from simba.utils.read_write import read_df, write_df, get_fn_ext, get_video_meta_data
 from simba.mixins.config_reader import ConfigReader
 from simba.mixins.plotting_mixin import PlottingMixin
 
 plt.interactive(True)
@@ -47,15 +49,15 @@
     def __init__(self,
                  config_path: str,
                  feature_file_path: str,
                  model_path: str,
                  discrimination_threshold: float,
                  shortest_bout: int,
                  create_gantt: str,
-                 settings: None=None):
+                 settings: Dict[str, Any]):
 
         ConfigReader.__init__(self, config_path=config_path)
         PlottingMixin.__init__(self)
         _, self.feature_filename, ext = get_fn_ext(feature_file_path)
         self.discrimination_threshold, self.shortest_bout, self.create_gantt, self.settings = float(discrimination_threshold), shortest_bout, create_gantt, settings
         if not os.path.exists(self.single_validation_video_save_dir): os.makedirs(self.single_validation_video_save_dir)
         _, _, self.fps = self.read_video_info(video_name=self.feature_filename)
```

### Comparing `Simba-UW-tf-dev-1.58.7/simba/plotting/frame_mergerer_ffmpeg.py` & `Simba-UW-tf-dev-1.58.8/simba/plotting/frame_mergerer_ffmpeg.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,18 @@
 __author__ = "Simon Nilsson"
 
 import os
 import subprocess, shutil
 from datetime import datetime
+from typing import Dict, Optional
+try:
+    from typing import Literal
+except ImportError:
+    from typing_extensions import Literal
+
 from simba.utils.read_write import get_fn_ext, remove_a_folder, get_video_meta_data, read_config_file, read_config_entry
 from simba.utils.printing import stdout_success, SimbaTimer
 from simba.utils.enums import Paths
 from simba.mixins.config_reader import ConfigReader
 
 
 class FrameMergererFFmpeg(ConfigReader):
@@ -29,19 +35,19 @@
     -----
     `GitHub tutorial <https://github.com/sgoldenlab/simba/blob/master/docs/tutorial.md#step-12-merge-frames>`__.
 
 
     """
 
     def __init__(self,
-                 config_path: str or None,
-                 concat_type: str,
-                 frame_types: dict,
-                 video_height: int or None,
-                 video_width: int or None):
+                 concat_type: Literal['horizontal', 'vertical', 'mosaic', 'mixed_mosaic'],
+                 frame_types: Dict[str, str],
+                 video_height: int,
+                 video_width: int,
+                 config_path: Optional[str] = None):
 
         self.timer = SimbaTimer(start=True)
         self.datetime = datetime.now().strftime('%Y%m%d%H%M%S')
         if config_path is not None:
             ConfigReader.__init__(self, config_path=config_path)
             self.output_dir = os.path.join(self.project_path, Paths.CONCAT_VIDEOS_DIR.value)
             self.temp_dir = os.path.join(self.project_path, Paths.CONCAT_VIDEOS_DIR.value, 'temp')
```

### Comparing `Simba-UW-tf-dev-1.58.7/simba/plotting/Directing_animals_visualizer_mp.py` & `Simba-UW-tf-dev-1.58.8/simba/plotting/Directing_animals_visualizer_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.7/simba/plotting/clf_validator.py` & `Simba-UW-tf-dev-1.58.8/simba/plotting/clf_validator.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,16 @@
 __author__ = "Simon Nilsson"
 
 import numpy as np
 from copy import deepcopy
 import os
 import cv2
+from typing import Tuple, List
+
+
 from simba.utils.enums import Formats
 from simba.mixins.config_reader import ConfigReader
 from simba.utils.errors import NoSpecifiedOutputError, NoFilesFoundError
 from simba.utils.warnings import NoDataFoundWarning
 from simba.utils.printing import stdout_success, SimbaTimer
 from simba.utils.checks import check_int, check_that_column_exist , check_if_filepath_list_is_empty
 from simba.utils.read_write import get_video_meta_data, get_fn_ext, read_df
@@ -47,18 +50,18 @@
     """
 
     def __init__(self,
                  config_path: str,
                  window: int,
                  clf_name: str,
                  clips: bool,
-                 text_clr: tuple,
+                 text_clr: Tuple[int, int, int],
                  concat_video: bool,
                  video_speed: float,
-                 data_paths: list,
+                 data_paths: List[str],
                  highlight_clr: None or tuple = None):
 
         super().__init__(config_path=config_path)
         if (not clips) and (not concat_video):
             raise NoSpecifiedOutputError(msg='Please select to create clips and/or a concatenated video')
 
         check_int(name='Time window', value=window)
```

### Comparing `Simba-UW-tf-dev-1.58.7/simba/plotting/path_plotter_mp.py` & `Simba-UW-tf-dev-1.58.8/simba/plotting/path_plotter_mp.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 from collections import deque
 from numba import jit, prange
 import numpy as np
 import os
 import functools
 import multiprocessing
 import platform
+from typing import Optional, Dict, List
 
 from simba.mixins.config_reader import ConfigReader
 from simba.mixins.plotting_mixin import PlottingMixin
 from simba.utils.errors import NoSpecifiedOutputError
 from simba.utils.read_write import get_fn_ext, remove_a_folder, concatenate_videos_in_folder, read_df
 from simba.utils.printing import stdout_success, SimbaTimer
 from simba.utils.checks import check_if_filepath_list_is_empty
@@ -46,27 +47,27 @@
 
     Examples
     ----------
     >>> input_style_attr = {'width': 'As input', 'height': 'As input', 'line width': 5, 'font size': 5, 'font thickness': 2, 'circle size': 5, 'bg color': 'White', 'max lines': 100}
     >>> animal_attr = {0: ['Ear_right_1', 'Red']}
     >>> input_clf_attr = {0: ['Attack', 'Black', 'Size: 30'], 1: ['Sniffing', 'Red', 'Size: 30']}
     >>> path_plotter = PathPlotterMulticore(config_path=r'MyConfigPath', frame_setting=False, video_setting=True, style_attr=style_attr, animal_attr=animal_attr, files_found=['project_folder/csv/machine_results/MyVideo.csv'], cores=5, clf_attr=clf_attr)
-    >>> path_plotter.create_path_plots()
+    >>> path_plotter.run()
     """
 
     def __init__(self,
                  config_path: str,
                  frame_setting: bool,
                  video_setting: bool,
                  last_frame: bool,
-                 files_found: list,
-                 input_style_attr: dict or None,
-                 animal_attr: dict,
-                 input_clf_attr: dict or None,
-                 cores: int):
+                 files_found: List[str],
+                 cores: int,
+                 input_style_attr: Optional[Dict] = None,
+                 animal_attr: Dict[int, List[str]] = None,
+                 input_clf_attr: Optional[Dict[int, List[str]]] = None):
 
         if platform.system() == "Darwin":
             multiprocessing.set_start_method('spawn', force=True)
 
 
         if (not frame_setting) and (not video_setting) and (not last_frame):
             raise NoSpecifiedOutputError(msg='SIMBA ERROR: Please choice to create path frames and/or video path plots')
```

### Comparing `Simba-UW-tf-dev-1.58.7/simba/plotting/ROI_feature_visualizer_mp.py` & `Simba-UW-tf-dev-1.58.8/simba/plotting/ROI_feature_visualizer_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.7/simba/plotting/data_plotter.py` & `Simba-UW-tf-dev-1.58.8/simba/plotting/data_plotter.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 __author__ = "Simon Nilsson"
 
 import pandas as pd
 from joblib import Parallel, delayed
 import os
 import numpy as np
 import cv2
+from typing import List, Dict
+
 from simba.utils.enums import Formats
 from simba.data_processors.movement_calculator import MovementCalculator
 from simba.mixins.config_reader import ConfigReader
 from simba.utils.errors import NoSpecifiedOutputError
 from simba.utils.lookups import get_color_dict
 from simba.utils.printing import stdout_success, SimbaTimer
 from simba.utils.read_write import get_fn_ext
@@ -32,17 +34,17 @@
     >>> data_plotter = DataPlotter(config_path='MyConfigPath')
     >>> data_plotter.process_movement()
     >>> data_plotter.create_data_plots()
     """
 
     def __init__(self,
                  config_path: str,
-                 style_attr: dict,
-                 body_part_attr: list,
-                 data_paths: list,
+                 style_attr: Dict,
+                 body_part_attr: List[List[str]],
+                 data_paths: List[str],
                  video_setting: bool,
                  frame_setting: bool,
                  ):
 
         super().__init__(config_path=config_path)
         if (not video_setting) and (not frame_setting):
             raise NoSpecifiedOutputError(msg='SIMBA ERROR: Please choose to create video and/or frames data plots. SimBA found that you ticked neither video and/or frames')
```

### Comparing `Simba-UW-tf-dev-1.58.7/simba/plotting/path_plotter.py` & `Simba-UW-tf-dev-1.58.8/simba/plotting/path_plotter.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.7/simba/plotting/ez_lineplot.py` & `Simba-UW-tf-dev-1.58.8/simba/plotting/ez_lineplot.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.7/simba/plotting/distance_plotter_mp.py` & `Simba-UW-tf-dev-1.58.8/simba/plotting/distance_plotter_mp.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,14 +2,16 @@
 
 import numpy as np
 import multiprocessing
 import functools
 from numba import jit
 import os
 import platform
+from typing import Dict, List
+
 from simba.utils.errors import NoSpecifiedOutputError
 from simba.utils.printing import stdout_success, SimbaTimer
 from simba.mixins.config_reader import ConfigReader
 from simba.mixins.plotting_mixin import PlottingMixin
 from simba.utils.checks import check_if_filepath_list_is_empty
 from simba.utils.read_write import read_df, get_fn_ext, concatenate_videos_in_folder
 
@@ -48,17 +50,17 @@
     """
 
     def __init__(self,
                  config_path: str,
                  frame_setting: bool,
                  video_setting: bool,
                  final_img: bool,
-                 files_found: list,
-                 style_attr: dict,
-                 line_attr: dict,
+                 files_found: List[str],
+                 style_attr: Dict[str, int],
+                 line_attr: Dict[int, list],
                  core_cnt: int):
 
         ConfigReader.__init__(self, config_path=config_path)
         PlottingMixin.__init__(self)
 
         if platform.system() == "Darwin":
             multiprocessing.set_start_method('spawn', force=True)
```

### Comparing `Simba-UW-tf-dev-1.58.7/simba/plotting/ROI_plotter.py` & `Simba-UW-tf-dev-1.58.8/simba/plotting/ROI_plotter.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.7/simba/plotting/heat_mapper_clf.py` & `Simba-UW-tf-dev-1.58.8/simba/plotting/heat_mapper_clf.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,14 +3,17 @@
 import pandas as pd
 import numpy as np
 import os
 import cv2
 from numba import jit, prange
 import matplotlib.pyplot as plt
 from matplotlib.backends.backend_agg import FigureCanvasAgg as FigureCanvas
+from typing import List
+
+
 from simba.utils.enums import Formats
 from simba.utils.printing import stdout_success, SimbaTimer
 from simba.mixins.config_reader import ConfigReader
 from simba.mixins.plotting_mixin import PlottingMixin
 from simba.utils.read_write import get_fn_ext, read_df
 from simba.utils.errors import NoSpecifiedOutputError
 
@@ -57,15 +60,15 @@
     def __init__(self,
                  config_path: str,
                  final_img_setting: bool,
                  video_setting: bool,
                  frame_setting: bool,
                  bodypart: str,
                  clf_name: str,
-                 files_found: list,
+                 files_found: List[str],
                  style_attr: dict
                  ):
 
         ConfigReader.__init__(self, config_path=config_path)
         PlottingMixin.__init__(self)
 
         if (not frame_setting) and (not video_setting) and (not final_img_setting):
```

### Comparing `Simba-UW-tf-dev-1.58.7/simba/plotting/distance_plotter.py` & `Simba-UW-tf-dev-1.58.8/simba/plotting/distance_plotter.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,14 +2,16 @@
 
 import PIL
 import io
 import cv2
 import os
 import numpy as np
 import matplotlib.pyplot as plt
+from typing import Dict, List
+
 from simba.mixins.config_reader import ConfigReader
 from simba.mixins.plotting_mixin import PlottingMixin
 from simba.utils.errors import NoSpecifiedOutputError
 from simba.utils.lookups import get_color_dict
 from simba.utils.printing import stdout_success, SimbaTimer
 from simba.utils.checks import check_if_filepath_list_is_empty
 from simba.utils.enums import Formats
@@ -41,17 +43,17 @@
     """
 
     def __init__(self,
                  config_path: str,
                  frame_setting: bool,
                  video_setting: bool,
                  final_img: bool,
-                 files_found: list,
-                 style_attr: dict,
-                 line_attr: dict):
+                 files_found: List[str],
+                 style_attr: Dict[str, int],
+                 line_attr: Dict[int, list]):
 
         ConfigReader.__init__(self, config_path=config_path)
         PlottingMixin.__init__(self)
         self.video_setting, self.frame_setting, self.files_found, self.style_attr, self.line_attr, self.final_img = video_setting, frame_setting, files_found, style_attr, line_attr, final_img
         if (not frame_setting) and (not video_setting) and (not self.final_img):
             raise NoSpecifiedOutputError('Please choice to create frames and/or video distance plots')
         self.colors_dict = get_color_dict()
```

### Comparing `Simba-UW-tf-dev-1.58.7/simba/plotting/single_run_model_validation_video_mp.py` & `Simba-UW-tf-dev-1.58.8/simba/plotting/single_run_model_validation_video_mp.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 import numpy as np
 import cv2
 import os
 import platform
 import functools
 import multiprocessing
 import matplotlib
+from typing import Dict, Any
 
 from simba.mixins.config_reader import ConfigReader
 from simba.mixins.plotting_mixin import PlottingMixin
 from simba.utils.data import plug_holes_shortest_bout
 from simba.utils.read_write import get_fn_ext, read_df, write_df, get_video_meta_data, concatenate_videos_in_folder
 from simba.utils.printing import stdout_success
 
@@ -47,17 +48,17 @@
 
     def __init__(self,
                  config_path: str,
                  feature_file_path: str,
                  model_path: str,
                  discrimination_threshold: float,
                  shortest_bout: int,
-                 cores:int,
+                 cores: int,
                  create_gantt: str,
-                 settings: None=None):
+                 settings: Dict[str, Any]):
 
         ConfigReader.__init__(self, config_path=config_path)
         PlottingMixin.__init__(self)
         if platform.system() == "Darwin":
             multiprocessing.set_start_method('spawn', force=True)
 
         _, self.feature_filename, ext = get_fn_ext(feature_file_path)
```

### Comparing `Simba-UW-tf-dev-1.58.7/simba/plotting/Directing_animals_visualizer.py` & `Simba-UW-tf-dev-1.58.8/simba/plotting/Directing_animals_visualizer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.7/simba/plotting/heat_mapper_location_mp.py` & `Simba-UW-tf-dev-1.58.8/simba/plotting/heat_mapper_location_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.7/simba/dash_app/SimBA_dash_app.py` & `Simba-UW-tf-dev-1.58.8/simba/dash_app/SimBA_dash_app.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.7/simba/dash_app/run_dash_tkinter.py` & `Simba-UW-tf-dev-1.58.8/simba/dash_app/run_dash_tkinter.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.7/simba/dash_app/dash_app.py` & `Simba-UW-tf-dev-1.58.8/simba/dash_app/dash_app.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.7/simba/data_processors/agg_clf_calculator.py` & `Simba-UW-tf-dev-1.58.8/simba/data_processors/agg_clf_calculator.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 __author__ = "Simon Nilsson"
 
 import pandas as pd
 import os
+from typing import List
+
 from simba.utils.checks import check_file_exist_and_readable, check_if_filepath_list_is_empty
 from simba.mixins.config_reader import ConfigReader
 from simba.utils.data import detect_bouts
 from simba.utils.printing import stdout_success
 from simba.utils.read_write import get_fn_ext, read_df
 
 class AggregateClfCalculator(ConfigReader):
@@ -32,16 +34,16 @@
     >>> clf_log_creator = AggregateClfCalculator(config_path="MyConfigPath", data_measures=['Bout count', 'Total event duration'], classifiers=['Attack', 'Sniffing'])
     >>> clf_log_creator.run()
     >>> clf_log_creator.save()
     """
 
     def __init__(self,
                  config_path: str,
-                 data_measures: list,
-                 classifiers: list):
+                 data_measures: List[str],
+                 classifiers: List[str]):
 
         super().__init__(config_path=config_path)
         self.chosen_measures, self.classifiers = data_measures, classifiers
         self.file_save_name = os.path.join(self.project_path, 'logs', 'data_summary_' + str(self.datetime) + '.csv')
         check_if_filepath_list_is_empty(filepaths=self.machine_results_paths,
                                         error_msg='SIMBA ERROR: No data files found in the project_folder/csv/machine_results directory. Run classifiers before analysing results.')
         print(f'Analyzing {str(len(self.machine_results_paths))} file(s) for {str(len(self.clf_names))} classifiers...')
```

### Comparing `Simba-UW-tf-dev-1.58.7/simba/data_processors/interpolation_smoothing.py` & `Simba-UW-tf-dev-1.58.8/simba/data_processors/interpolation_smoothing.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.7/simba/data_processors/timebins_clf_calculator.py` & `Simba-UW-tf-dev-1.58.8/simba/data_processors/timebins_clf_calculator.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 __author__ = "Simon Nilsson"
 
 import pandas as pd
 import os, glob
 from collections import defaultdict
+from typing import List
+
 from simba.utils.checks import check_int, check_if_filepath_list_is_empty
 from simba.utils.data import detect_bouts
 from simba.utils.printing import stdout_success
 from simba.utils.read_write import get_fn_ext, read_df
 from simba.mixins.config_reader import ConfigReader
 from simba.utils.errors import NoChoosenMeasurementError
 
@@ -36,16 +38,16 @@
     >>> timebin_clf_analyzer.run()
 
     """
 
     def __init__(self,
                  config_path: str,
                  bin_length: int,
-                 measurements: list,
-                 classifiers: list):
+                 measurements: List[str],
+                 classifiers: List[str]):
 
         super().__init__(config_path=config_path)
         if len(measurements) == 0:
             raise NoChoosenMeasurementError()
         check_int(name='Bin length', value=bin_length, min_value=1)
         self.bin_length, self.measurements, self.classifiers = int(bin_length), measurements, classifiers
         self.files_found = glob.glob(self.machine_results_dir + '/*.' + self.file_type)
```

### Comparing `Simba-UW-tf-dev-1.58.7/simba/data_processors/fsttc_calculator.py` & `Simba-UW-tf-dev-1.58.8/simba/data_processors/fsttc_calculator.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 __author__ = "Simon Nilsson"
 
 import os
 import pandas as pd
 import itertools
 import seaborn as sns
+from typing import List
+
 from simba.utils.data import detect_bouts
 from simba.utils.printing import stdout_success
 from simba.utils.read_write import get_fn_ext, read_df
 from simba.utils.checks import check_if_filepath_list_is_empty
 from simba.utils.errors import CountError
 from simba.mixins.config_reader import ConfigReader
 
@@ -48,15 +50,15 @@
            Application to the Study of Retinal Waves, `J Neurosci`, 2014.
     """
 
 
     def __init__(self,
                  config_path: str,
                  time_window: int,
-                 behavior_lst: list,
+                 behavior_lst: List[str],
                  create_graphs: bool):
 
         super().__init__(config_path=config_path)
 
         self.time_delta = int(time_window)
         self.behavior_lst = behavior_lst
         if len(self.behavior_lst) < 2:
```

### Comparing `Simba-UW-tf-dev-1.58.7/simba/data_processors/interpolate_pose.py` & `Simba-UW-tf-dev-1.58.8/simba/data_processors/interpolate_pose.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.7/simba/data_processors/directing_other_animals_calculator.py` & `Simba-UW-tf-dev-1.58.8/simba/data_processors/directing_other_animals_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.7/simba/data_processors/timebins_movement_calculator.py` & `Simba-UW-tf-dev-1.58.8/simba/data_processors/timebins_movement_calculator.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 __author__ = "Simon Nilsson"
 
 import pandas as pd
 import seaborn as sns
 import matplotlib.pyplot as plt
 import itertools
-import os, glob
+import os
+from typing import List
+
 from simba.utils.printing import stdout_success, SimbaTimer
 from simba.utils.enums import ConfigKey, Dtypes
 from simba.utils.checks import check_that_column_exist, check_if_filepath_list_is_empty, check_int
 from simba.utils.read_write import get_fn_ext, read_df, read_config_entry
 from simba.mixins.config_reader import ConfigReader
 from simba.mixins.feature_extraction_mixin import FeatureExtractionMixin
 
@@ -22,133 +24,124 @@
         path to SimBA project config file in Configparser format
     bin_length: int
         Integer representing the time bin size in seconds
 
     Example
     ----------
 
-    >>> timebin_movement_analyzer = TimeBinsMovementCalculator(config_path='MyConfigPath', bin_length=15)
-    >>> timebin_movement_analyzer.analyze_movement()
+    >>> timebin_movement_analyzer = TimeBinsMovementCalculator(config_path='MyConfigPath', bin_length=15, )
+    >>> timebin_movement_analyzer.run()
 
     """
 
     def __init__(self,
                  config_path: str,
                  bin_length: int,
+                 body_parts: List[str],
                  plots: bool):
 
         ConfigReader.__init__(self, config_path=config_path)
         self.bin_length, self.plots = bin_length, plots
         check_int(name='TIME BIN', value=bin_length, min_value=1)
-        self.col_headers = []
-        for animal_no in range(self.animal_cnt):
-            animal_bp = read_config_entry(self.config, ConfigKey.PROCESS_MOVEMENT_SETTINGS.value, 'animal_{}_bp'.format(str(animal_no + 1)), Dtypes.STR.value)
-            self.col_headers.extend((animal_bp + '_x', animal_bp + '_y'))
-
+        self.col_headers, self.bp_dict = [], {}
+        for bp_cnt, bp in enumerate(body_parts):
+            self.col_headers.extend((f'{bp}_x', f'{bp}_y'))
+            animal_name = self.find_animal_name_from_body_part_name(bp_name=bp, bp_dict=self.animal_bp_dict)
+            self.bp_dict[bp_cnt] = {animal_name: [f'{bp}_x', f'{bp}_y']}
         check_if_filepath_list_is_empty(filepaths=self.outlier_corrected_paths,
                                         error_msg=f'SIMBA ERROR: Cannot analyze movement in time-bins, data directory {self.outlier_corrected_dir} is empty.')
         self.animal_combinations = list(itertools.combinations(self.animal_bp_dict, 2))
         print('Processing {} video(s)...'.format(str(len(self.outlier_corrected_paths))))
 
     def __create_plots(self):
+        timer = SimbaTimer(start=True)
         print('Creating time-bin movement plots...')
         sns.set_style("whitegrid", {'grid.linestyle': '--'})
-        self.video_df['Time bin #'] = self.video_df['Time bin #'].astype(str)
         plots_dir = os.path.join(self.project_path, 'logs', f'time_bin_movement_plots_{self.datetime}')
         if not os.path.exists(plots_dir): os.makedirs(plots_dir)
-        for video_name in self.video_df.index.unique():
-            video_df = self.video_df[self.video_df.index == video_name].reset_index(drop=True)
-            video_movement_df = video_df[video_df['Measurement'].isin(list(self.movement_cols))]
-            line_plot = sns.lineplot(data=video_movement_df, x="Time bin #", y="Value", hue='Measurement')
-            line_plot.figure.savefig(os.path.join(plots_dir, f'{video_name}.png'))
-            plt.close()
-        stdout_success(msg='Time bin movement plots saved in {plots_dir}...')
+        for video_name in self.results['VIDEO'].unique():
+            video_df = self.results.loc[(self.results['VIDEO'] == video_name) & (self.results['MEASUREMENT'] == 'Movement (cm)')]
+            for body_part in video_df['BODY-PART'].unique():
+                body_part_df = video_df[video_df['BODY-PART'] == body_part].reset_index(drop=True).sort_values(by=['Time bin #'])
+                body_part_df['Time bin #'] = body_part_df['Time bin #'].astype(str)
+                line_plot = sns.lineplot(data=body_part_df, x="Time bin #", y="VALUE")
+                plt.ylabel("Distance (cm)")
+                line_plot.figure.savefig(os.path.join(plots_dir, f'{video_name}_{body_part}.png'))
+                plt.close()
+        timer.stop_timer()
+        stdout_success(msg=f'Time bin movement plots saved in {plots_dir}', elapsed_time=timer.elapsed_time_str)
+
+
+
+
+        # self.video_df['Time bin #'] = self.video_df['Time bin #'].astype(str)
+
+        # for video_name in self.video_df.index.unique():
+        #     video_df = self.video_df[self.video_df.index == video_name].reset_index(drop=True)
+        #     video_movement_df = video_df[video_df['Measurement'].isin(list(self.movement_cols))]
+        #     line_plot = sns.lineplot(data=video_movement_df, x="Time bin #", y="Value", hue='Measurement')
+        #     line_plot.figure.savefig(os.path.join(plots_dir, f'{video_name}.png'))
+        #     plt.close()
+        # stdout_success(msg=f'Time bin movement plots saved in {plots_dir}...')
 
     def run(self):
         """
         Method for running the movement time-bin analysis. Results are stored in the ``project_folder/logs`` directory
         of the SimBA project.
 
         Returns
         ----------
         None
         """
-        video_dict, self.out_df_lst = {}, []
+        video_dict, out_df_lst = {}, []
+        save_path = os.path.join(self.project_path, 'logs', 'Time_bins_movement_results_' + self.datetime + '.csv')
         for file_cnt, file_path in enumerate(self.outlier_corrected_paths):
             video_timer = SimbaTimer(start=True)
             _, video_name, _ = get_fn_ext(file_path)
             print(f'Processing time-bin movements for video {video_name} ({str(file_cnt+1)}/{str(len(self.outlier_corrected_paths))})...')
-            result_df = pd.DataFrame()
             video_dict[video_name] = {}
             video_settings, px_per_mm, fps = self.read_video_info(video_name=video_name)
             fps, self.movement_cols, self.velocity_cols = int(fps), set(), set()
             bin_length_frames = int(fps * self.bin_length)
-            data_df = read_df(file_path, self.file_type)
-            data_df_sliced = pd.DataFrame()
-            for animal, data in self.animal_bp_dict.items():
-                check_that_column_exist(df=data_df, column_name=data['X_bps'][0], file_name=file_path)
-                check_that_column_exist(df=data_df, column_name=data['Y_bps'][0], file_name=file_path)
-                data_df_sliced[data['X_bps'][0]] = data_df[data['X_bps'][0]]
-                data_df_sliced[data['Y_bps'][0]] = data_df[data['Y_bps'][0]]
-            data_df_shifted = data_df.shift(periods=1).add_suffix('_shifted').fillna(0)
-            data_df = pd.concat([data_df_sliced, data_df_shifted], axis=1, join='inner').fillna(0).reset_index(drop=True)
-            for animal, data in self.animal_bp_dict.items():
-                movement_col_name = 'Movement {}'.format(animal)
-                x_col, y_col = data['X_bps'][0], data['Y_bps'][0]
-                bp_time_1 = data_df[[x_col, y_col]].values
-                bp_time_2 = data_df[[x_col + '_shifted', y_col + '_shifted']].values
-                result_df[movement_col_name] = pd.Series(self.framewise_euclidean_distance(location_1=bp_time_1, location_2=bp_time_2, px_per_mm=px_per_mm, centimeter=True))
-                result_df.loc[0, movement_col_name] = 0
-            for animal_c in self.animal_combinations:
-                distance_col_name = 'Distance {} {}'.format(animal_c[0], animal_c[1])
-                bp_1_x, bp_1_y = self.animal_bp_dict[animal_c[0]]['X_bps'][0], self.animal_bp_dict[animal_c[0]]['Y_bps'][0]
-                bp_2_x, bp_2_y = self.animal_bp_dict[animal_c[0]]['X_bps'][0], self.animal_bp_dict[animal_c[1]]['Y_bps'][0]
-                bp_1 = data_df[[bp_1_x, bp_1_y]].values.astype(float)
-                bp_2 = data_df[[bp_2_x, bp_2_y]].values.astype(float)
-                result_df[distance_col_name] = pd.Series(self.framewise_euclidean_distance(location_1=bp_1, location_2=bp_2, px_per_mm=px_per_mm))
-            results_df_lists = [result_df[i:i + bin_length_frames] for i in range(0, result_df.shape[0], bin_length_frames)]
-            indexed_df_lst = []
-            for bin, results in enumerate(results_df_lists):
-                time_bin_per_s = [results[i:i + fps] for i in range(0, results.shape[0], fps)]
-                for second, df in enumerate(time_bin_per_s):
-                    df['Time bin #'], df['Second'] = bin, second
-                    indexed_df_lst.append(df)
-            indexed_df = pd.concat(indexed_df_lst, axis=0)
-            movement_cols = [x for x in indexed_df.columns if x.startswith('Movement ')]
-            distance_cols = [x for x in indexed_df.columns if x.startswith('Distance ')]
-            for movement_col in movement_cols:
-                movement_sum = indexed_df.groupby(['Time bin #'])[movement_col].sum().reset_index()
-                movement_velocity = indexed_df.groupby(['Time bin #', 'Second'])[movement_col].sum().reset_index()
-                movement_velocity = movement_velocity.groupby(['Time bin #'])[movement_col].mean().reset_index()
-                video_dict[video_name][movement_col + ' (cm)'] = movement_sum
-                self.movement_cols.add(movement_col + ' (cm)')
-                video_dict[video_name][movement_col + ' velocity (cm/s)'] = movement_velocity
-                self.velocity_cols.add(movement_col + ' velocity (cm/s)')
-            for distance_col in distance_cols:
-                video_dict[video_name][distance_col + ' (cm)'] = indexed_df.groupby(['Time bin #'])[distance_col].mean().reset_index()
+            data_df = read_df(file_path, self.file_type, usecols=self.col_headers)
+            data_df = self.create_shifted_df(df=data_df)
+            for animal_data in self.bp_dict.values():
+                name, bps = list(animal_data.keys())[0], list(animal_data.values())[0]
+                bp_time_1, bp_time_2 = data_df[bps].values, data_df[[f'{bps[0]}_shifted', f'{bps[1]}_shifted']].values
+                movement_data = pd.DataFrame(self.framewise_euclidean_distance(location_1=bp_time_1, location_2=bp_time_2, px_per_mm=px_per_mm, centimeter=True), columns=['VALUE'])
+                results_df_lists = [movement_data[i:i + bin_length_frames] for i in range(0, movement_data.shape[0], bin_length_frames)]
+                indexed_df = []
+                for bin, results in enumerate(results_df_lists):
+                    time_bin_per_s = [results[i:i + fps] for i in range(0, results.shape[0], fps)]
+                    for second, df in enumerate(time_bin_per_s):
+                        df['Time bin #'] = bin
+                        df['Second'] = second
+                        indexed_df.append(df)
+                indexed_df = pd.concat(indexed_df, axis=0)
+                velocity_df = indexed_df.groupby(['Time bin #', 'Second'])['VALUE'].sum().reset_index()
+                velocity_df = velocity_df.groupby(['Time bin #'])['VALUE'].mean().reset_index()
+                velocity_df['ANIMAL'] = list(animal_data.keys())[0]
+                velocity_df['BODY-PART'] = bps[0][:-2]
+                velocity_df['MEASUREMENT'] = 'Velocity (cm/s)'
+                movement_df = indexed_df.groupby(['Time bin #'])['VALUE'].sum().reset_index()
+                movement_df['ANIMAL'] = list(animal_data.keys())[0]
+                movement_df['BODY-PART'] = bps[0][:-2]
+                movement_df['MEASUREMENT'] = 'Movement (cm)'
+                results = pd.concat([movement_df, velocity_df], axis=0)
+                results['VIDEO'] = video_name
+                out_df_lst.append(results)
             video_timer.stop_timer()
             print(f'Video {video_name} complete (elapsed time: {video_timer.elapsed_time_str}s)...')
-
-        for video_name, video_info in video_dict.items():
-            for measurement, bin_data in video_info.items():
-                data_df = pd.DataFrame.from_dict(bin_data).reset_index(drop=True)
-                data_df.columns = ['Time bin #', measurement]
-                data_df = pd.melt(data_df, id_vars=['Time bin #']).drop('variable', axis=1).rename(columns={'value': 'Value'})
-                data_df.insert(loc=0, column='Measurement', value=measurement)
-                data_df.insert(loc=0, column='Video', value=video_name)
-                self.out_df_lst.append(data_df)
-        self.video_df = pd.concat(self.out_df_lst, axis= 0).sort_values(by=['Video', 'Time bin #']).set_index('Video')
-        if self.plots:
-            self.__create_plots()
-
-        save_path = os.path.join(self.project_path, 'logs', 'Time_bins_movement_results_' + self.datetime + '.csv')
-        self.video_df.to_csv(save_path)
+        self.results = pd.concat(out_df_lst, axis=0).sort_values(by=['VIDEO', 'Time bin #', 'MEASUREMENT', 'ANIMAL'])[['VIDEO', 'Time bin #', 'ANIMAL', 'BODY-PART', 'MEASUREMENT', 'VALUE']]
+        self.results.to_csv(save_path)
         self.timer.stop_timer()
         stdout_success(msg=f'Movement time-bins results saved at {save_path}', elapsed_time=self.timer.elapsed_time_str)
+        if self.plots:
+            self.__create_plots()
 
-# test = TimeBinsMovementAnalyzer(config_path='/Users/simon/Desktop/envs/troubleshooting/naresh/project_folder/project_config.ini',
-#                                 bin_length=60, plots=True)
-# test.analyze_movement()
+# test = TimeBinsMovementCalculator(config_path='/Users/simon/Desktop/envs/troubleshooting/naresh/project_folder/project_config.ini',
+#                                   bin_length=60, plots=True, body_parts=['midpoint', 'mouth'])
+# test.run()
 
-# test = TimeBinsMovementAnalyzer(config_path='/Users/simon/Desktop/envs/troubleshooting/Two_animals_16bps/project_folder/project_config.ini',
+# test = TimeBinsMovementCalculator(config_path='/Users/simon/Desktop/envs/troubleshooting/Two_animals_16bps/project_folder/project_config.ini',
 #                                 bin_length=1, plots=True)
 # test.analyze_movement()
```

### Comparing `Simba-UW-tf-dev-1.58.7/simba/data_processors/severity_calculator.py` & `Simba-UW-tf-dev-1.58.8/simba/data_processors/severity_calculator.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 __author__ = "Simon Nilsson"
 
 import numpy as np
-import glob, os
+import os
 import pandas as pd
 from datetime import datetime
 from numba import jit
-from simba.utils.read_write import read_video_info_csv, get_fn_ext, read_df
+from typing import Dict, Optional, Union
+
+from simba.utils.read_write import get_fn_ext, read_df
 from simba.utils.checks import check_if_filepath_list_is_empty
-from simba.utils.enums import Paths
 from simba.utils.printing import stdout_success
 from simba.utils.warnings import NoDataFoundWarning
 from simba.mixins.config_reader import ConfigReader
 
 
 class SeverityCalculator(ConfigReader):
     """
@@ -35,15 +36,15 @@
     >>> processor = SeverityProcessor(config_path='project_folder/project_config.ini', settings=settings)
     >>> processor.run()
     >>> processor.save()
     """
 
     def __init__(self,
                  config_path: str,
-                 settings: dict):
+                 settings: Dict):
 
         ConfigReader.__init__(self, config_path=config_path)
         self.settings = settings
         check_if_filepath_list_is_empty(filepaths=self.machine_results_paths,
                                         error_msg=f'SIMBA ERROR: Cannot process severity. {self.machine_results_dir} directory is empty')
         save_name = os.path.join(f'severity_{datetime.now().strftime("%Y%m%d%H%M%S")}.csv')
         self.save_path = os.path.join(self.logs_path, save_name)
```

### Comparing `Simba-UW-tf-dev-1.58.7/simba/data_processors/pup_retrieval_calculator.py` & `Simba-UW-tf-dev-1.58.8/simba/data_processors/pup_retrieval_calculator.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,29 +2,31 @@
 
 import pandas as pd
 
 
 import os, glob
 from datetime import datetime
 import seaborn as sns
+from typing import Dict, Union
+
 from simba.mixins.config_reader import ConfigReader
 from simba.utils.read_write import (read_config_file,
                                     read_config_entry,
                                     read_project_path_and_file_type,
                                     read_video_info_csv,
                                     get_fn_ext,
                                     read_df)
 from simba.utils.checks import check_if_filepath_list_is_empty
 from simba.utils.data import detect_bouts
 from simba.utils.enums import Paths, ConfigKey, Dtypes
 
 class PupRetrieverCalculator(ConfigReader):
     def __init__(self,
                  config_path: str,
-                 settings: dict):
+                 settings: Dict[str, Union[float, str, bool]]):
         """
         Pup retreival calculator used in Winters
 
         :param config_path: path to SimBA configparser.ConfigParser project_config.ini
         :param settings: user-defined setting for pup retrieval
 
         :Example:
```

### Comparing `Simba-UW-tf-dev-1.58.7/simba/data_processors/pybursts_calculator.py` & `Simba-UW-tf-dev-1.58.8/simba/data_processors/pybursts_calculator.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 ### CODE MODIFID FROM PYBURST PACKAGE  https://pypi.org/project/pybursts/
 import numpy as np
 import math
 
-def kleinberg_burst_detection(offsets=None,
-              s=None,
-              gamma=None):
+def kleinberg_burst_detection(offsets: np.array,
+                              s: float,
+                              gamma: float):
 
     offsets = np.array(offsets, dtype=object)
 
     if offsets.size == 1:
         bursts = np.array([0, offsets[0], offsets[0]], ndmin=2, dtype=object)
         return bursts
```

### Comparing `Simba-UW-tf-dev-1.58.7/simba/data_processors/kleinberg_calculator.py` & `Simba-UW-tf-dev-1.58.8/simba/data_processors/kleinberg_calculator.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,16 @@
 __author__ = "Simon Nilsson"
 
 import pandas as pd
 import numpy as np
 import shutil, os
 from copy import deepcopy
+from typing import List
+
+
 from simba.utils.checks import (check_that_column_exist,
                                 check_int,
                                 check_float,
                                 check_if_filepath_list_is_empty)
 from simba.utils.read_write import write_df, read_df, get_fn_ext
 from simba.utils.printing import stdout_success
 from simba.mixins.config_reader import ConfigReader
@@ -53,19 +56,19 @@
            2019.
     .. [3] Bordes et al., Automatically annotated motion tracking identifies a distinct social behavioral profile
            following chronic social defeat stress, `bioRxiv`, 2022.
     '''
 
     def __init__(self,
                  config_path: str,
-                 classifier_names: list,
-                 sigma=2,
-                 gamma=0.3,
-                 hierarchy=1,
-                 hierarchical_search=False):
+                 classifier_names: List[str],
+                 sigma: int=2,
+                 gamma: float=0.3,
+                 hierarchy: int=1,
+                 hierarchical_search: bool=False):
 
         super().__init__(config_path=config_path)
         self.hierarchical_search, sigma, gamma, hierarchy = hierarchical_search, float(sigma), float(gamma), int(hierarchy)
         check_float(value=sigma, name='sigma', min_value=1.01)
         check_float(value=gamma, name='gamma', min_value=0)
         check_int(value=hierarchy, name='hierarchy')
         self.sigma, self.gamma, self.hierarchy = float(sigma), float(gamma), float(hierarchy)
```

### Comparing `Simba-UW-tf-dev-1.58.7/simba/data_processors/movement_calculator.py` & `Simba-UW-tf-dev-1.58.8/simba/data_processors/movement_calculator.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 __author__ = "Simon Nilsson"
 
 import pandas as pd
 import os
 import numpy as np
+from typing import List, Optional
+
 from statistics import mean
 from simba.utils.printing import stdout_success
 from simba.utils.read_write import read_df, get_fn_ext
 from simba.utils.checks import check_if_filepath_list_is_empty
 from simba.mixins.config_reader import ConfigReader
 from simba.mixins.feature_extraction_mixin import FeatureExtractionMixin
 from simba.feature_extractors.perimeter_jit import jitted_centroid
@@ -30,17 +32,17 @@
     >>> movement_processor.run()
     >>> movement_processor.save()
 
     """
 
     def __init__(self,
                  config_path: str,
-                 body_parts: dict,
+                 body_parts: List[str],
                  threshold: float,
-                 file_paths: list=None):
+                 file_paths: Optional[List[str]] = None):
 
         ConfigReader.__init__(self, config_path=config_path)
         FeatureExtractionMixin.__init__(self)
         self.save_path = os.path.join(self.logs_path, 'Movement_log_{}.csv'.format(self.datetime))
         self.file_paths, self.body_parts, self.threshold = file_paths, body_parts, threshold
         if not self.file_paths:
             check_if_filepath_list_is_empty(filepaths=self.outlier_corrected_paths,
```

### Comparing `Simba-UW-tf-dev-1.58.7/simba/pose_configurations_archive/pose_configurations_archive_1/.DS_Store` & `Simba-UW-tf-dev-1.58.8/simba/pose_configurations_archive/pose_configurations_archive_1/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.7/simba/pose_configurations_archive/pose_configurations_archive_1/bp_names/.DS_Store` & `Simba-UW-tf-dev-1.58.8/simba/pose_configurations_archive/pose_configurations_archive_1/bp_names/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.7/simba/pose_configurations_archive/pose_configurations_archive_1/bp_names/bp_names.csv` & `Simba-UW-tf-dev-1.58.8/simba/pose_configurations_archive/pose_configurations_archive_1/bp_names/bp_names.csv`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.7/simba/pose_configurations_archive/pose_configurations_archive_1/no_animals/.DS_Store` & `Simba-UW-tf-dev-1.58.8/simba/pose_configurations_archive/pose_configurations_archive_1/no_animals/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.7/simba/pose_configurations_archive/pose_configurations_archive_1/configuration_names/.DS_Store` & `Simba-UW-tf-dev-1.58.8/simba/pose_configurations_archive/pose_configurations_archive_1/configuration_names/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.7/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/.DS_Store` & `Simba-UW-tf-dev-1.58.8/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.7/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/8.png` & `Simba-UW-tf-dev-1.58.8/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/8.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.7/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/9.png` & `Simba-UW-tf-dev-1.58.8/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/9.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.7/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/12.png` & `Simba-UW-tf-dev-1.58.8/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/12.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.7/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/13.png` & `Simba-UW-tf-dev-1.58.8/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/13.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.7/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/11.png` & `Simba-UW-tf-dev-1.58.8/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/11.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.7/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/10.png` & `Simba-UW-tf-dev-1.58.8/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/10.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.7/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/4.png` & `Simba-UW-tf-dev-1.58.8/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/4.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.7/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/5.png` & `Simba-UW-tf-dev-1.58.8/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/5.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.7/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/7.png` & `Simba-UW-tf-dev-1.58.8/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/7.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.7/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/6.png` & `Simba-UW-tf-dev-1.58.8/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/6.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.7/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/2.png` & `Simba-UW-tf-dev-1.58.8/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/2.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.7/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/3.png` & `Simba-UW-tf-dev-1.58.8/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/3.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.7/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/1.png` & `Simba-UW-tf-dev-1.58.8/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/1.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.7/simba/model/train_rf.py` & `Simba-UW-tf-dev-1.58.8/simba/model/train_rf.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.7/simba/model/inference_batch.py` & `Simba-UW-tf-dev-1.58.8/simba/model/inference_batch.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.7/simba/model/grid_search_rf.py` & `Simba-UW-tf-dev-1.58.8/simba/model/grid_search_rf.py`

 * *Files 1% similar despite different names*

```diff
@@ -65,14 +65,15 @@
             self.x_train, self.y_train = self.smote_oversampler(self.x_train, self.y_train, meta_dict[ConfigKey.OVERSAMPLE_RATIO.value])
 
     def __check_validity_of_meta_files(self, meta_file_paths: list):
         meta_dicts, errors = {}, []
         for config_cnt, path in enumerate(meta_file_paths):
             _, meta_file_name, _ = get_fn_ext(path)
             meta_dict = read_meta_file(path)
+
             meta_dict = {k.lower(): v for k, v in meta_dict.items()}
             errors.append(check_str(name=meta_dict[MetaKeys.CLF_NAME.value], value=meta_dict[MetaKeys.CLF_NAME.value], raise_error=False)[1])
             errors.append(check_str(name=MetaKeys.CRITERION.value, value=meta_dict[MetaKeys.CRITERION.value], options=Options.CLF_CRITERION.value, raise_error=False)[1])
             errors.append(check_str(name=MetaKeys.RF_MAX_FEATURES.value, value=meta_dict[MetaKeys.RF_MAX_FEATURES.value], options=Options.CLF_MAX_FEATURES.value, raise_error=False)[1])
             errors.append(check_str(ConfigKey.UNDERSAMPLE_SETTING.value, meta_dict[ConfigKey.UNDERSAMPLE_SETTING.value].lower(), options=[x.lower() for x in Options.UNDERSAMPLE_OPTIONS.value], raise_error=False)[1])
             errors.append(check_str(ConfigKey.OVERSAMPLE_SETTING.value, meta_dict[ConfigKey.OVERSAMPLE_SETTING.value].lower(), options=[x.lower() for x in Options.OVERSAMPLE_OPTIONS.value], raise_error=False)[1])
             if MetaKeys.TRAIN_TEST_SPLIT_TYPE.value in meta_dict.keys():
@@ -115,15 +116,16 @@
             if MetaKeys.PARTIAL_DEPENDENCY.value in meta_dict.keys():
                 errors.append(check_if_valid_input(MetaKeys.PARTIAL_DEPENDENCY.value, input=meta_dict[MetaKeys.PARTIAL_DEPENDENCY.value],options=Options.RUN_OPTIONS_FLAGS.value, raise_error=False)[1])
 
             if meta_dict[MetaKeys.RF_MAX_FEATURES.value] == Dtypes.NONE.value: meta_dict[MetaKeys.RF_MAX_FEATURES.value] = None
             if MetaKeys.TRAIN_TEST_SPLIT_TYPE.value not in meta_dict.keys(): meta_dict[MetaKeys.TRAIN_TEST_SPLIT_TYPE.value] = Methods.SPLIT_TYPE_FRAMES.value
 
             if ConfigKey.CLASS_WEIGHTS.value in meta_dict.keys():
-                meta_dict[ConfigKey.CLASS_WEIGHTS.value] = meta_dict[ConfigKey.CLASS_WEIGHTS.value]
+                if meta_dict[ConfigKey.CLASS_WEIGHTS.value] not in Options.CLASS_WEIGHT_OPTIONS.value:
+                    meta_dict[ConfigKey.CLASS_WEIGHTS.value] = None
                 if meta_dict[ConfigKey.CLASS_WEIGHTS.value] == 'custom':
                     meta_dict[ConfigKey.CLASS_WEIGHTS.value] = literal_eval(meta_dict['class_custom_weights'])
                     for k, v in meta_dict[ConfigKey.CLASS_WEIGHTS.value].items():
                         meta_dict[ConfigKey.CLASS_WEIGHTS.value][k] = int(v)
                 if meta_dict[ConfigKey.CLASS_WEIGHTS.value] == Dtypes.NONE.value:
                     meta_dict[ConfigKey.CLASS_WEIGHTS.value] = None
             else:
```

### Comparing `Simba-UW-tf-dev-1.58.7/simba/model/inference_validation.py` & `Simba-UW-tf-dev-1.58.8/simba/model/inference_validation.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.7/simba/roi_tools/ROI_time_bin_calculator.py` & `Simba-UW-tf-dev-1.58.8/simba/roi_tools/ROI_time_bin_calculator.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,15 +1,18 @@
 import os
 import pandas as pd
 import itertools
+from typing import List
+
 from simba.roi_tools.ROI_analyzer import ROIAnalyzer
-from simba.utils.printing import stdout_success
-from simba.utils.enums import ConfigKey, DirNames, Dtypes
+from simba.utils.printing import stdout_success, SimbaTimer
+from simba.utils.enums import DirNames
 from simba.mixins.config_reader import ConfigReader
-from simba.utils.read_write import get_fn_ext, read_config_entry, read_df
+from simba.utils.read_write import get_fn_ext, read_df, write_df
+from simba.utils.errors import ROICoordinatesNotFoundError
 
 class ROITimebinCalculator(ConfigReader):
     """
     Class for calulating how much time and how many entries animals are making into user-defined ROIs
     in user-defined time bins. Results are stored in the `project_folder/logs` directory of the SimBA project.
 
     Parameters
@@ -20,85 +23,79 @@
         length of time bins in seconds.
 
     Notes
     ----------
 
     Examples
     ----------
-    >>> roi_time_bin_calculator = ROITimebinCalculator(config_path='MySimBaConfigPath', bin_length=15)
+    >>> roi_time_bin_calculator = ROITimebinCalculator(config_path='MySimBaConfigPath', bin_length=15, body_parts=['Nose_1'], threshold=0.00)
     >>> roi_time_bin_calculator.run()
     >>> roi_time_bin_calculator.save()
     """
 
     def __init__(self,
                  config_path: str,
-                 bin_length: int):
+                 bin_length: int,
+                 body_parts: List[str],
+                 threshold: float):
 
         ConfigReader.__init__(self, config_path=config_path)
-        self.bin_length = bin_length
-        self.roi_animal_cnt = read_config_entry(config=self.config, section=ConfigKey.ROI_SETTINGS.value, option=ConfigKey.ROI_ANIMAL_CNT.value, data_type=Dtypes.INT.value)
-        self.probability_threshold = read_config_entry(config=self.config, section=ConfigKey.ROI_SETTINGS.value, option=ConfigKey.PROBABILITY_THRESHOLD.value, data_type=Dtypes.FLOAT.value, default_value=0.00)
-        self.save_path_time = os.path.join(self.logs_path, 'ROI_time_bins_{}s_time_data_{}.csv'.format(str(bin_length), self.datetime))
-        self.save_path_entries = os.path.join(self.logs_path, 'ROI_time_bins_{}s_entry_data_{}.csv'.format(str(bin_length), self.datetime))
-        self.roi_analyzer = ROIAnalyzer(ini_path=self.config_path, data_path=DirNames.OUTLIER_MOVEMENT_LOCATION.value, calculate_distances=False)
+        if not os.path.isfile(self.roi_coordinates_path):
+            raise ROICoordinatesNotFoundError(expected_file_path=self.roi_coordinates_path)
+        self.read_roi_data()
+        self.bin_length, self.body_parts, self.threshold = bin_length, body_parts, threshold
+        self.save_path_time = os.path.join(self.logs_path, f'ROI_time_bins_{bin_length}s_time_data_{self.datetime}.csv')
+        self.save_path_entries = os.path.join(self.logs_path, f'ROI_time_bins_{bin_length}s_entry_data_{self.datetime}.csv')
+        settings = {'threshold': threshold, 'body_parts': {}}
+        for i in body_parts:
+            animal_name = self.find_animal_name_from_body_part_name(bp_name=i, bp_dict=self.animal_bp_dict)
+            settings['body_parts'][animal_name] = i
+        self.roi_analyzer = ROIAnalyzer(ini_path=self.config_path,
+                                        data_path=DirNames.OUTLIER_MOVEMENT_LOCATION.value,
+                                        calculate_distances=False,
+                                        settings=settings)
+
         self.roi_analyzer.run()
-        self.shape_names = self.roi_analyzer.shape_names
         self.animal_names = list(self.roi_analyzer.bp_dict.keys())
         self.entries_exits_df = self.roi_analyzer.detailed_df
-
+    #
     def run(self):
-        self.files_found = self.roi_analyzer.files_found
-        self.out_dict_time, self.out_dict_entries = {}, {}
-        print('Analyzing time-bin data for {} videos...'.format(str(len(self.files_found))))
-        for file_cnt, file_path in enumerate(self.files_found):
+        self.out_time_lst, self.out_entries_lst = [], []
+        print(f'Analyzing time-bin data for {len(self.outlier_corrected_paths)} video(s)...')
+        for file_cnt, file_path in enumerate(self.outlier_corrected_paths):
+            video_timer = SimbaTimer(start=True)
             _, self.video_name, _ = get_fn_ext(filepath=file_path)
-            self.out_dict_time[self.video_name], self.out_dict_entries[self.video_name] = {}, {}
             _, _, fps = self.read_video_info(video_name=self.video_name)
             frames_per_bin = int(fps * self.bin_length)
             video_frms = list(range(0, len(read_df(file_path=file_path, file_type=self.file_type))))
             frame_bins = [video_frms[i * frames_per_bin:(i + 1) * frames_per_bin] for i in range((len(video_frms) + frames_per_bin - 1) // frames_per_bin )]
             self.video_data = self.entries_exits_df[self.entries_exits_df['VIDEO'] == self.video_name]
             for animal_name, shape_name in list(itertools.product(self.animal_names, self.shape_names)):
-                self.results_time, self.results_entries = {}, {}
-                self.results_time[shape_name], self.results_entries[shape_name] = {}, {}
-                self.results_time[shape_name][animal_name], self.results_entries[shape_name][animal_name] = {}, {}
+                results_entries = pd.DataFrame(columns=['VIDEO', 'SHAPE', 'ANIMAL', 'TIME BIN', 'ENTRY COUNT'])
+                results_time = pd.DataFrame(columns=['VIDEO', 'SHAPE', 'ANIMAL', 'TIME BIN', 'TIME INSIDE SHAPE (S)'])
                 data_df = self.video_data.loc[(self.video_data['SHAPE'] == shape_name) & (self.video_data['ANIMAL'] == animal_name)]
                 entry_frms = list(data_df['ENTRY FRAMES'])
                 inside_shape_frms = [list(range(x, y)) for x, y in zip(list(data_df['ENTRY FRAMES'].astype(int)), list(data_df['EXIT FRAMES'].astype(int) + 1))]
                 inside_shape_frms = [i for s in inside_shape_frms for i in s]
                 for bin_cnt, bin_frms in enumerate(frame_bins):
                     frms_inside_roi_in_timebin = [x for x in inside_shape_frms if x in bin_frms]
                     entry_roi_in_timebin = [x for x in entry_frms if x in bin_frms]
-                    self.results_time[shape_name][animal_name][bin_cnt] = len(frms_inside_roi_in_timebin) / fps
-                    self.results_entries[shape_name][animal_name][bin_cnt] = len(entry_roi_in_timebin)
-                self.out_dict_time[self.video_name].update(self.results_time)
-                self.out_dict_entries[self.video_name].update(self.results_entries)
+                    results_time.loc[len(results_time)] = [self.video_name, shape_name, animal_name, bin_cnt, len(frms_inside_roi_in_timebin) / fps]
+                    results_entries.loc[len(results_entries)] = [self.video_name, shape_name, animal_name, bin_cnt, len(entry_roi_in_timebin)]
+                self.out_time_lst.append(results_time)
+                self.out_entries_lst.append(results_entries)
+            video_timer.stop_timer()
+            print(f'Video {self.video_name} complete (elapsed time {video_timer.elapsed_time_str}s)')
+        self.out_time = pd.concat(self.out_time_lst, axis=0).sort_values(by=['VIDEO', 'SHAPE', 'ANIMAL', 'TIME BIN'])
+        self.out_entries = pd.concat(self.out_entries_lst, axis=0).sort_values(by=['VIDEO', 'SHAPE', 'ANIMAL', 'TIME BIN'])
 
     def save(self):
-        results_time_df = pd.DataFrame(columns=['VIDEO', 'SHAPE', 'ANIMAL', 'TIME BIN', 'TIME INSIDE SHAPE (S)'])
-        results_entries_df = pd.DataFrame(columns=['VIDEO', 'SHAPE', 'ANIMAL', 'TIME BIN', 'ENTRY COUNT'])
-        for video_name, video_data in self.out_dict_time.items():
-            for shape_name, shape_data in video_data.items():
-                for animal_name, animal_data in shape_data.items():
-                    for bin_name, bin_data in animal_data.items():
-                        results_time_df.loc[len(results_time_df)] = [video_name, shape_name, animal_name, bin_name, bin_data]
-        results_time_df['TIME INSIDE SHAPE (S)'] = results_time_df['TIME INSIDE SHAPE (S)'].round(6)
-        results_time_df.to_csv(self.save_path_time)
-        stdout_success(msg=f'ROI time bin time data saved at {self.save_path_time}')
-        for video_name, video_data in self.out_dict_entries.items():
-            for shape_name, shape_data in video_data.items():
-                for animal_name, animal_data in shape_data.items():
-                    for bin_name, bin_data in animal_data.items():
-                        results_entries_df.loc[len(results_entries_df)] = [video_name, shape_name, animal_name, bin_name, bin_data]
-        results_entries_df.to_csv(self.save_path_entries)
+        self.out_entries.to_csv(self.save_path_entries)
+        self.out_time.to_csv(self.save_path_time)
         self.timer.stop_timer()
         stdout_success(msg=f'ROI time bin entry data saved at {self.save_path_entries}', elapsed_time=self.timer.elapsed_time_str)
+        stdout_success(msg=f'ROI time bin time data saved at {self.save_path_time}', elapsed_time=self.timer.elapsed_time_str)
 
-
-# test = ROITimebinCalculator(config_path='/Users/simon/Desktop/troubleshooting/train_model_project/project_folder/project_config.ini',bin_length=5)
-# test.analyze_time_bins()
-# test.save_results()
-
-
-# test = ROITimebinCalculator(config_path=r"/Users/simon/Desktop/envs/troubleshooting/two_black_animals_14bp/project_folder/project_config.ini",bin_length=5)
+# test = ROITimebinCalculator(config_path=r"/Users/simon/Desktop/envs/troubleshooting/sleap_5_animals/project_folder/project_config.ini",
+#                             bin_length=5, body_parts=['Simon_Nose_1_1', 'JJ_Nose_1_2'], threshold=0.00)
 # test.run()
-# test.save_results()
+# test.save()
```

### Comparing `Simba-UW-tf-dev-1.58.7/simba/roi_tools/ROI_movement_analyzer.py` & `Simba-UW-tf-dev-1.58.8/simba/roi_tools/ROI_movement_analyzer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.7/simba/roi_tools/.DS_Store` & `Simba-UW-tf-dev-1.58.8/simba/roi_tools/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.7/simba/roi_tools/ROI_define.py` & `Simba-UW-tf-dev-1.58.8/simba/roi_tools/ROI_define.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.7/simba/roi_tools/ROI_reset.py` & `Simba-UW-tf-dev-1.58.8/simba/roi_tools/ROI_reset.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.7/simba/roi_tools/ROI_analyzer.py` & `Simba-UW-tf-dev-1.58.8/simba/roi_tools/ROI_analyzer.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 __author__ = "Simon Nilsson"
 
 import os, glob, itertools
 import numpy as np
 from shapely.geometry import Point, Polygon
 import pandas as pd
+from typing import Dict, Optional
+
 from simba.utils.printing import stdout_success
 from simba.utils.enums import ConfigKey, Dtypes
 from simba.mixins.config_reader import ConfigReader
 from simba.utils.errors import NoFilesFoundError, BodypartColumnNotFoundError
 from simba.utils.warnings import NoDataFoundWarning
 from simba.utils.read_write import get_fn_ext, read_df, read_config_entry
 
@@ -40,16 +42,16 @@
     >>> roi_analyzer = ROIAnalyzer(ini_path='MyProjectConfig', data_path='outlier_corrected_movement_location', settings=settings, calculate_distances=True)
     >>> roi_analyzer.run()
     >>> roi_analyzer.save()
     """
 
     def __init__(self,
                  ini_path: str,
-                 data_path: str or None,
-                 settings: dict or None = None,
+                 data_path: Optional[str] = None,
+                 settings: Optional[dict] = None,
                  calculate_distances: bool = False):
 
         ConfigReader.__init__(self, config_path=ini_path)
         self.calculate_distances, self.settings = calculate_distances, settings
         if not os.path.exists(self.detailed_roi_data_dir): os.makedirs(self.detailed_roi_data_dir)
         if data_path != None:
             self.input_folder = os.path.join(self.project_path, 'csv', data_path)
```

### Comparing `Simba-UW-tf-dev-1.58.7/simba/roi_tools/ROI_feature_analyzer.py` & `Simba-UW-tf-dev-1.58.8/simba/roi_tools/ROI_feature_analyzer.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 __author__ = "Simon Nilsson"
 
 import numpy as np
 import os, glob
 import itertools
 from copy import deepcopy
+from typing import Optional, Dict
+
 from simba.utils.printing import stdout_success
 from simba.roi_tools.ROI_analyzer import ROIAnalyzer
 from simba.roi_tools.ROI_directing_analyzer import DirectingROIAnalyzer
 from simba.mixins.config_reader import ConfigReader
 from simba.mixins.feature_extraction_mixin import FeatureExtractionMixin
 from simba.utils.errors import NoFilesFoundError, NoROIDataError
 from simba.utils.warnings import NoFileFoundWarning
@@ -34,15 +36,15 @@
     >>> roi_featurizer.run()
     >>> roi_featurizer.save()
 
     """
 
     def __init__(self,
                  config_path: str,
-                 settings: dict or None=None):
+                 settings: Optional[Dict] = None):
 
         ConfigReader.__init__(self, config_path=config_path)
         FeatureExtractionMixin.__init__(self, config_path=config_path)
         self.roi_directing_viable = self.check_directionality_viable()[0]
         self.settings = settings
         if self.roi_directing_viable:
             print('Directionality calculations are VIABLE.')
```

### Comparing `Simba-UW-tf-dev-1.58.7/simba/roi_tools/ROI_multiply.py` & `Simba-UW-tf-dev-1.58.8/simba/roi_tools/ROI_multiply.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.7/simba/roi_tools/ROI_size_calculations.py` & `Simba-UW-tf-dev-1.58.8/simba/roi_tools/ROI_size_calculations.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.7/simba/roi_tools/ROI_zoom.py` & `Simba-UW-tf-dev-1.58.8/simba/roi_tools/ROI_zoom.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.7/simba/roi_tools/ROI_directing_analyzer.py` & `Simba-UW-tf-dev-1.58.8/simba/roi_tools/ROI_directing_analyzer.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 __author__ = "Simon Nilsson"
 
 from simba.roi_tools.ROI_analyzer import ROIAnalyzer
 import pandas as pd
 from numba import jit, prange
 from copy import deepcopy
 import numpy as np
+from typing import Optional, Dict
+
 from simba.mixins.config_reader import ConfigReader
 from simba.mixins.feature_extraction_mixin import FeatureExtractionMixin
 from simba.utils.read_write import get_fn_ext
 
 class DirectingROIAnalyzer(ConfigReader, FeatureExtractionMixin):
     """
     Class for computing aggregate statistics for animals are directing towards ROIs.
@@ -26,17 +28,17 @@
     ----------
     >>> roi_directing_calculator = DirectingROIAnalyzer(config_path='MyProjectConfig')
     >>> roi_directing_calculator.calc_directing_to_ROIs()
 
     """
 
     def __init__(self,
-                 config_path: str=None,
-                 data_path: str=None,
-                 settings: dict or None=None):
+                 config_path: str,
+                 data_path: Optional[str] = None,
+                 settings: Optional[dict] = None):
 
         ConfigReader.__init__(self, config_path=config_path)
         FeatureExtractionMixin.__init__(self, config_path=config_path)
         self.roi_analyzer = ROIAnalyzer(ini_path=config_path, data_path=self.outlier_corrected_dir, settings=settings)
         self.files_found = deepcopy(self.roi_analyzer.files_found)
         self.direct_bp_dict = self.check_directionality_cords()
```

### Comparing `Simba-UW-tf-dev-1.58.7/simba/roi_tools/ROI_move_shape.py` & `Simba-UW-tf-dev-1.58.8/simba/roi_tools/ROI_move_shape.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.7/simba/roi_tools/ROI_menus.py` & `Simba-UW-tf-dev-1.58.8/simba/roi_tools/ROI_menus.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.7/simba/roi_tools/ROI_clf_calculator.py` & `Simba-UW-tf-dev-1.58.8/simba/roi_tools/ROI_clf_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.7/simba/roi_tools/ROI_image.py` & `Simba-UW-tf-dev-1.58.8/simba/roi_tools/ROI_image.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.7/simba/pose_importers/misc/sleap_csv_importer.py` & `Simba-UW-tf-dev-1.58.8/simba/pose_importers/misc/sleap_csv_importer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.7/simba/pose_importers/misc/sleap_h5_importer.py` & `Simba-UW-tf-dev-1.58.8/simba/pose_importers/misc/sleap_h5_importer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.7/simba/pose_importers/misc/madlc_importer.py` & `Simba-UW-tf-dev-1.58.8/simba/pose_importers/misc/madlc_importer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.7/simba/pose_importers/misc/apt_trk_importer.py` & `Simba-UW-tf-dev-1.58.8/simba/pose_importers/misc/apt_trk_importer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.7/simba/pose_importers/misc/sleap_slp_importer.py` & `Simba-UW-tf-dev-1.58.8/simba/pose_importers/misc/sleap_slp_importer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.7/simba/pose_importers/read_DANNCE_mat.py` & `Simba-UW-tf-dev-1.58.8/simba/pose_importers/read_DANNCE_mat.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.7/simba/pose_importers/sleap_importer_slp.py` & `Simba-UW-tf-dev-1.58.8/simba/pose_importers/sleap_importer_slp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.7/simba/pose_importers/sleap_importer_h5.py` & `Simba-UW-tf-dev-1.58.8/simba/pose_importers/sleap_importer_h5.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.7/simba/pose_importers/dlc_multi_animal_importer.py` & `Simba-UW-tf-dev-1.58.8/simba/pose_importers/dlc_multi_animal_importer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.7/simba/pose_importers/.DS_Store` & `Simba-UW-tf-dev-1.58.8/simba/pose_importers/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.7/simba/pose_importers/sleap_importer_csv.py` & `Simba-UW-tf-dev-1.58.8/simba/pose_importers/sleap_importer_csv.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.7/simba/pose_importers/import_mars.py` & `Simba-UW-tf-dev-1.58.8/simba/pose_importers/import_mars.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.7/simba/pose_importers/dlc_importer_csv.py` & `Simba-UW-tf-dev-1.58.8/simba/pose_importers/dlc_importer_csv.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.7/simba/pose_importers/trk_importer.py` & `Simba-UW-tf-dev-1.58.8/simba/pose_importers/trk_importer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.7/simba/pose_configurations/.DS_Store` & `Simba-UW-tf-dev-1.58.8/simba/pose_configurations/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.7/simba/pose_configurations/bp_names/.DS_Store` & `Simba-UW-tf-dev-1.58.8/simba/pose_configurations/bp_names/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.7/simba/pose_configurations/bp_names/bp_names.csv` & `Simba-UW-tf-dev-1.58.8/simba/pose_configurations/bp_names/bp_names.csv`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.7/simba/pose_configurations/no_animals/.DS_Store` & `Simba-UW-tf-dev-1.58.8/simba/pose_configurations/no_animals/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.7/simba/pose_configurations/configuration_names/.DS_Store` & `Simba-UW-tf-dev-1.58.8/simba/pose_configurations/configuration_names/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.7/simba/pose_configurations/schematics/8.png` & `Simba-UW-tf-dev-1.58.8/simba/pose_configurations/schematics/8.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.7/simba/pose_configurations/schematics/9.png` & `Simba-UW-tf-dev-1.58.8/simba/pose_configurations/schematics/9.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.7/simba/pose_configurations/schematics/12.png` & `Simba-UW-tf-dev-1.58.8/simba/pose_configurations/schematics/12.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.7/simba/pose_configurations/schematics/11.png` & `Simba-UW-tf-dev-1.58.8/simba/pose_configurations/schematics/11.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.7/simba/pose_configurations/schematics/10.png` & `Simba-UW-tf-dev-1.58.8/simba/pose_configurations/schematics/10.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.7/simba/pose_configurations/schematics/4.png` & `Simba-UW-tf-dev-1.58.8/simba/pose_configurations/schematics/4.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.7/simba/pose_configurations/schematics/5.png` & `Simba-UW-tf-dev-1.58.8/simba/pose_configurations/schematics/5.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.7/simba/pose_configurations/schematics/7.png` & `Simba-UW-tf-dev-1.58.8/simba/pose_configurations/schematics/7.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.7/simba/pose_configurations/schematics/6.png` & `Simba-UW-tf-dev-1.58.8/simba/pose_configurations/schematics/6.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.7/simba/pose_configurations/schematics/2.png` & `Simba-UW-tf-dev-1.58.8/simba/pose_configurations/schematics/2.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.7/simba/pose_configurations/schematics/3.png` & `Simba-UW-tf-dev-1.58.8/simba/pose_configurations/schematics/3.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.7/simba/pose_configurations/schematics/1.png` & `Simba-UW-tf-dev-1.58.8/simba/pose_configurations/schematics/1.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.7/simba/video_processors/video_processing.py` & `Simba-UW-tf-dev-1.58.8/simba/video_processors/video_processing.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 import simba
 from simba.mixins.config_reader import ConfigReader
 from tkinter import *
 from datetime import datetime
 import time
 from PIL import Image, ImageTk
 import multiprocessing
+from typing import List, Union
 
 from simba.utils.checks import (check_file_exist_and_readable, check_int, check_if_filepath_list_is_empty)
 from simba.utils.read_write import (get_fn_ext,
                                     get_video_meta_data,
                                     find_all_videos_in_directory,
                                     find_core_cnt,
                                     read_config_entry,
@@ -36,15 +37,15 @@
                                   FileExistWarning)
 
 
 MAX_FRM_SIZE = 1080, 650
 
 def change_img_format(directory: str,
                       file_type_in: str,
-                      file_type_out: str):
+                      file_type_out: str) -> None:
     """
     Helper to convert file type of all image files in a folder.
 
     Parameters
     ----------
     directory: str
         Path to directory holding image files
@@ -72,15 +73,15 @@
         im = Image.open(file_path)
         save_name = file_path.replace('.' + str(file_type_in), '.' + str(file_type_out))
         im.save(save_name)
         os.remove(file_path)
     stdout_success(msg=f'SIMBA COMPLETE: Files in {directory} directory converted to {file_type_out}')
 
 
-def clahe_enhance_video(file_path: str):
+def clahe_enhance_video(file_path: str) -> None:
     """
     Helper to convert a single video file to clahe-enhanced greyscale .avi file. The result is saved with prefix
     ``CLAHE_`` in the same directory as in the input file.
 
     Parameters
     ----------
     file_path: str
@@ -122,15 +123,15 @@
 
 
 
 
 
 def extract_frame_range(file_path: str,
                         start_frame: int,
-                        end_frame: int):
+                        end_frame: int) -> None:
     """
     Helper to extract a user-defined range of frames from a video file and save those in png format. Images
     are saved in a folder with the suffix `_frames` within the same directory as the video file.
 
     Parameters
     ----------
     file_path: str
@@ -160,15 +161,15 @@
         frm_save_path = os.path.join(save_dir, '{}.{}'.format(str(frm_number), 'png'))
         cv2.imwrite(frm_save_path,frame)
         print('Frame {} saved (Frame {}/{})'.format(str(frm_number), str(frm_cnt), str(len(frame_range))))
     stdout_success(msg=f'{str(len(frame_range))} frames extracted for video {file_name}')
 
 
 def change_single_video_fps(file_path: str,
-                            fps: int):
+                            fps: int) -> None:
     """
     Helper to change the fps of a single video file. Results are stored in the same directory as in the input file with
     the suffix ``_fps_new_fps``.
 
     Parameters
     ----------
     file_path: str
@@ -187,15 +188,15 @@
     if os.path.isfile(save_path):
         FileExistWarning(msg=f'Overwriting existing file at {save_path}')
     command = str('ffmpeg -i ') + '"' + str(file_path) + '"' + ' -filter:v fps=fps=' + str(fps) + ' ' + '"' + save_path + '"'
     subprocess.call(command, shell=True)
     stdout_success(msg=f'SIMBA COMPLETE: FPS of video {file_name} changed from {str(video_meta_data["fps"])} to {str(fps)} and saved in directory {save_path}')
 
 def change_fps_of_multiple_videos(directory: str,
-                                  fps: int):
+                                  fps: int) -> None:
     """
     Helper to change the fps of video files in a folder. Results are stored in the same directory as in the input files with
     the suffix ``_fps_new_fps``.
 
     Parameters
     ----------
     directory: str
@@ -220,15 +221,15 @@
         print('Converting FPS for {}...'.format(file_name))
         save_path = os.path.join(dir_name, file_name + '_fps_{}{}'.format(str(fps), str(ext)))
         command = str('ffmpeg -i ') + str(file_path) + ' -filter:v fps=fps=' + str(fps) + ' ' + '"' + save_path + '"'
         subprocess.call(command, shell=True)
         print('Video {} complete...'.format(file_name))
     stdout_success(msg=f'SIMBA COMPLETE: FPS of {str(len(video_paths))} videos changed to { str(fps)}')
 
-def convert_video_powerpoint_compatible_format(file_path: str):
+def convert_video_powerpoint_compatible_format(file_path: str) -> None:
     """
     Helper to make a powerpoint compatible copy of a video file. The results is stored in the same directory as the
     input file with the ``_powerpointready`` suffix.
 
     Parameters
     ----------
     file_path: str
@@ -243,15 +244,15 @@
     if os.path.isfile(save_name):
         raise FileExistError(msg='SIMBA ERROR: The outfile file already exist: {}.'.format(save_name))
     command = (str('ffmpeg -i ') + '"' + str(file_path) + '"' + ' -c:v libx264 -preset slow  -profile:v high -level:v 4.0 -pix_fmt yuv420p -crf 22 -codec:a aac ' + '"' + save_name + '"')
     print('Creating video in powerpoint compatible format... ')
     subprocess.call(command, shell=True, stdout=subprocess.PIPE)
     stdout_success(msg=f'SIMBA COMPLETE: Video converted! {save_name} generated!')
 
-def convert_to_mp4(file_path: str):
+def convert_to_mp4(file_path: str) -> None:
     """
     Helper to convert a video file to mp4 format. The results is stored in the same directory as the
     input file with the ``_converted.mp4`` suffix.
 
     Parameters
     ----------
     file_path: str
@@ -266,15 +267,15 @@
         raise FileExistError(msg='SIMBA ERROR: The outfile file already exist: {}.'.format(save_name))
     command = (str('ffmpeg -i ') + '"' + str(file_path) + '"' + ' ' + '"' + save_name + '"')
     print('Converting to mp4... ')
     subprocess.call(command, shell=True, stdout=subprocess.PIPE)
     stdout_success(msg=f'SIMBA COMPLETE: Video converted! {save_name} generated!')
 
 
-def video_to_greyscale(file_path: str):
+def video_to_greyscale(file_path: str) -> None:
     """
     Helper to convert a video file to greyscale mp4 format. The results is stored in the same directory as the
     input file with the ``_grayscale.mp4`` suffix.
 
     Parameters
     ----------
     file_path: str
@@ -289,15 +290,15 @@
         raise FileExistError(msg='SIMBA ERROR: The outfile file already exist: {}.'.format(save_name))
     command = (str('ffmpeg -i ') + '"' + str(file_path) + '"' + ' -vf format=gray ' + '"' + save_name + '"')
     print('Converting to greyscale... ')
     subprocess.call(command, shell=True, stdout=subprocess.PIPE)
     stdout_success(msg=f'SIMBA COMPLETE: Video converted! {save_name} generated!')
 
 
-def superimpose_frame_count(file_path: str):
+def superimpose_frame_count(file_path: str) -> None:
     """
     Helper to superimpose frame count on a video file. The results is stored in the same directory as the
     input file with the ``_frame_no.mp4`` suffix.
 
     Parameters
     ----------
     file_path: str
@@ -318,15 +319,15 @@
         simba_cw = os.path.dirname(simba.__file__)
         simba_font_path = Path(simba_cw, 'assets', 'UbuntuMono-Regular.ttf')
         command = 'ffmpeg -y -i ' + file_path + ' -vf "drawtext=fontfile={}:'.format(simba_font_path) + "text='%{frame_num}': start_number=1: x=(w-tw)/2: y=h-(2*lh): fontcolor=black: fontsize=20: box=1: boxcolor=white: boxborderw=5" + '" ' + "-c:a copy " + save_name
         subprocess.call(command, shell=True, stdout=subprocess.PIPE)
     stdout_success(msg=f'SIMBA COMPLETE: Video converted! {save_name} generated!')
 
 def remove_beginning_of_video(file_path: str,
-                              time: int):
+                              time: int) -> None:
     """
     Helper to remove N seconds from the beginning of a video file. The results is stored in the same directory as the
     input file with the ``_shorten.mp4`` suffix.
 
     Parameters
     ----------
     file_path: str
@@ -343,15 +344,15 @@
     print('Shortening video... ')
     subprocess.call(command, shell=True, stdout=subprocess.PIPE)
     stdout_success(msg=f'SIMBA COMPLETE: Video converted! {save_name} generated!')
 
 
 def clip_video_in_range(file_path: str,
                         start_time: str,
-                        end_time: str):
+                        end_time: str) -> None:
     """
     Helper to clip video in a specific range. The results is stored in the same directory as the
     input file with the ``_clipped.mp4`` suffix.
 
     Parameters
     ----------
     file_path: str
@@ -370,15 +371,15 @@
     command = (str('ffmpeg -i ') + '"' + str(file_path) + '"' + ' -ss ' + str(start_time) + ' -to ' + str(end_time) + ' -async 1 ' + '"' + save_name + '"')
     print('Clipping video... ')
     subprocess.call(command, shell=True, stdout=subprocess.PIPE)
     stdout_success(msg=f'SIMBA COMPLETE: Video converted! {save_name} generated!')
 
 def downsample_video(file_path: str,
                      video_height: int,
-                     video_width: int):
+                     video_width: int) -> None:
     """
     Helper to down-sample a video file. The results is stored in the same directory as the
     input file with the ``_downsampled.mp4`` suffix.
 
     Parameters
     ----------
     file_path: str
@@ -400,15 +401,15 @@
     print('Down-sampling video... ')
     subprocess.call(command, shell=True, stdout=subprocess.PIPE)
     stdout_success(msg=f'SIMBA COMPLETE: Video converted! {save_name} generated!')
 
 def gif_creator(file_path: str,
                 start_time: int,
                 duration: int,
-                width: int):
+                width: int) -> None:
     """
     Helper to create a sample gif from a video file. The results is stored in the same directory as the
     input file with the ``.mp4`` file-ending.
 
     Parameters
     ----------
     file_path: str
@@ -435,15 +436,15 @@
     print('Creating gif sample... ')
     subprocess.call(command, shell=True, stdout=subprocess.PIPE)
     stdout_success(msg=f'SIMBA COMPLETE: Video converted! {save_name} generated!')
 
 
 def batch_convert_video_format(directory: str,
                                input_format: str,
-                               output_format: str):
+                               output_format: str) -> None:
     """
     Helper to batch convert all videos in a folder of specific format into a different video format. The results are
     stored in the same directory as the input files.
 
     Parameters
     ----------
     directory: str
@@ -472,15 +473,15 @@
             raise FileExistError(msg='SIMBA ERROR: The outfile file already exist: {}.'.format(save_path))
         command = 'ffmpeg -y -i ' + '"' + file_path + '"' + ' -c:v libx264 -crf 5 -preset medium -c:a libmp3lame -b:a 320k '+'"' + save_path + '"'
         subprocess.call(command, shell=True, stdout=subprocess.PIPE)
         print('Video {} complete, (Video {}/{})...'.format(file_name, str(file_cnt+1), str(len(video_paths))))
 
     stdout_success(msg=f'SIMBA COMPLETE: {str(len(video_paths))} videos converted in {directory} directory!')
 
-def batch_create_frames(directory: str):
+def batch_create_frames(directory: str) -> None:
     """
     Helper to extract all frames for all videos in a directory. Results are stored within sub-directories in the input
     directory named according to the video files.
 
     Parameters
     ----------
     directory: str
@@ -502,15 +503,15 @@
         print('Processing video {}...'.format(file_name))
         save_dir = os.path.join(dir_name, file_name)
         if not os.path.exists(save_dir): os.makedirs(save_dir)
         video_to_frames(file_path, save_dir, overwrite=True, every=1, chunk_size=1000)
         print('Video {} complete, (Video {}/{})...'.format(file_name, str(file_cnt + 1), str(len(video_paths))))
     stdout_success(msg=f'{str(len(video_paths))} videos converted into frames in {directory} directory!')
 
-def extract_frames_single_video(file_path: str):
+def extract_frames_single_video(file_path: str) -> None:
     """
     Helper to extract all frames for a single. Results are stored within a sub-directory in the same
     directory as the input file.
 
     Parameters
     ----------
     file_path: str
@@ -523,27 +524,27 @@
     save_dir = os.path.join(dir_name, file_name)
     if not os.path.exists(save_dir): os.makedirs(save_dir)
     print('Processing video {}...'.format(file_name))
     video_to_frames(file_path, save_dir, overwrite=True, every=1, chunk_size=1000)
     stdout_success(msg=f'Video {file_name} converted to images in {dir_name} directory!')
 
 def multi_split_video(file_path: str,
-                      start_times: list,
-                      end_times: list):
+                      start_times: List[str],
+                      end_times: List[str]) -> None:
     """
     Helper divide a video file into multiple video files from specified start and stop times.
 
     Parameters
     ----------
     file_path: str
         Path to video file.
     start_times: list
-        List of clip start times in [HH:MM:SS] format.
+       Clip start times in [HH:MM:SS] format.
     end_times: list
-        List of clip end times in [HH:MM:SS] format.
+        Clip end times in [HH:MM:SS] format.
     """
 
     check_file_exist_and_readable(file_path=file_path)
     video_meta_data = get_video_meta_data(file_path)
     dir_name, file_name, ext = get_fn_ext(filepath=file_path)
     r = re.compile('.{2}:.{2}:.{2}')
     for start_time_cnt, start_time in enumerate(start_times):
@@ -567,15 +568,15 @@
         if os.path.isfile(save_path):
             raise FileExistError(msg=f'The outfile file already exist: {save_path}.')
         command = (str('ffmpeg -i ') + '"' + file_path + '"' + ' -ss ' + start_time + ' -to ' + end_time + ' -async 1 ' + '"' + save_path + '"')
         print('Processing video clip {}...'.format(str(clip_cnt+1)))
         subprocess.call(command, shell=True, stdout=subprocess.PIPE)
     stdout_success(msg=f'Video {file_name} converted into {str(len(start_times))} clips in directory {dir_name}!')
 
-def crop_single_video(file_path: str):
+def crop_single_video(file_path: str) -> None:
     """
     Helper to crop a single video,
 
     Parameters
     ----------
     file_path: str
         Path to video file.
@@ -600,15 +601,15 @@
     if os.path.isfile(save_path):
         raise FileExistError(msg='SIMBA ERROR: The out file file already exist: {}.'.format(save_path))
     command = str('ffmpeg -y -i ') + '"' + str(file_path) + '"' + str(' -vf ') + str('"crop=') + str(width) + ':' + str(height) + ':' + str(top_lext_x) + ':' + str(top_left_y) + '" ' + str('-c:v libx264 -crf 21 -c:a copy ') + '"' + str(save_path) + '"'
     subprocess.call(command, shell=True)
     stdout_success(f'Video {file_name} cropped and saved at {save_path}')
 
 def crop_multiple_videos(directory_path: str,
-                         output_path: str):
+                         output_path: str) -> None:
     """
     Helper to crop multiple videos in a folder according to coordinates defines in one video.
 
     Parameters
     ----------
     directory_path: str
         Path to directory holding video files.
@@ -647,15 +648,15 @@
         subprocess.call(command, shell=True)
         print('Video {} cropped (Video {}/{})'.format(file_name, str(file_cnt+1), str(len(video_paths))))
     stdout_success(msg=f'{str(len(video_paths))} videos cropped and saved in {directory_path} directory')
 
 def frames_to_movie(directory: str,
                     fps: int,
                     bitrate: int,
-                    img_format: str):
+                    img_format: str) -> None:
 
     """
     Helper to merge frames in a folder to a mp4 video file. Video file is stored in the same directory as the
     input directory sub-folder.
 
     Parameters
     ----------
@@ -686,16 +687,18 @@
     print('Creating {} from {} images...'.format(os.path.basename(save_path), str(len(img_paths_in_folder))))
     subprocess.call(command, shell=True)
     stdout_success(msg=f'Video created at {save_path}')
 
 
 def video_concatenator(video_one_path: str,
                        video_two_path: str,
-                       resolution: int or str,
+                       resolution: Union[int, str],
                        horizontal: bool):
+
+
     for file_path in [video_one_path, video_two_path]:
         check_file_exist_and_readable(file_path=file_path)
         _ = get_video_meta_data(file_path)
     if type(resolution) is int:
         video_meta_data = {}
         if horizontal:
             video_meta_data['height'] = resolution
@@ -717,15 +720,15 @@
     stdout_success(msg=f'Videos concatenated and saved at {save_path}')
 
 
 
 class VideoRotator(ConfigReader):
     def __init__(self,
                  input_path: str,
-                 output_dir: str):
+                 output_dir: str) -> None:
 
         _, self.cpu_cnt  = find_core_cnt()
         self.save_dir = output_dir
         self.datetime = datetime.now().strftime('%Y%m%d%H%M%S')
         if os.path.isfile(input_path):
             self.video_paths = [input_path]
         else:
```

### Comparing `Simba-UW-tf-dev-1.58.7/simba/video_processors/.DS_Store` & `Simba-UW-tf-dev-1.58.8/simba/video_processors/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.7/simba/video_processors/px_to_mm.py` & `Simba-UW-tf-dev-1.58.8/simba/video_processors/px_to_mm.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.7/simba/video_processors/batch_process_menus.py` & `Simba-UW-tf-dev-1.58.8/simba/video_processors/batch_process_menus.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.7/simba/video_processors/multi_cropper.py` & `Simba-UW-tf-dev-1.58.8/simba/video_processors/multi_cropper.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.7/simba/video_processors/extract_frames.py` & `Simba-UW-tf-dev-1.58.8/simba/video_processors/extract_frames.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.7/simba/video_processors/calculate_px_dist.py` & `Simba-UW-tf-dev-1.58.8/simba/video_processors/calculate_px_dist.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.7/simba/video_processors/extract_seqframes.py` & `Simba-UW-tf-dev-1.58.8/simba/video_processors/extract_seqframes.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.7/simba/video_processors/batch_process_create_ffmpeg_commands.py` & `Simba-UW-tf-dev-1.58.8/simba/video_processors/batch_process_create_ffmpeg_commands.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.7/simba/outlier_tools/outlier_corrector_movement.py` & `Simba-UW-tf-dev-1.58.8/simba/outlier_tools/outlier_corrector_movement.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.7/simba/outlier_tools/.DS_Store` & `Simba-UW-tf-dev-1.58.8/simba/outlier_tools/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.7/simba/outlier_tools/outlier_corrector_location.py` & `Simba-UW-tf-dev-1.58.8/simba/outlier_tools/outlier_corrector_location.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.7/simba/outlier_tools/skip_outlier_correction.py` & `Simba-UW-tf-dev-1.58.8/simba/outlier_tools/skip_outlier_correction.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.7/simba/outlier_tools/.idea/outlier_scripts.iml` & `Simba-UW-tf-dev-1.58.8/simba/outlier_tools/.idea/outlier_scripts.iml`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.7/simba/outlier_tools/.idea/inspectionProfiles/Project_Default.xml` & `Simba-UW-tf-dev-1.58.8/simba/outlier_tools/.idea/inspectionProfiles/Project_Default.xml`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.7/simba/outlier_tools/.idea/workspace.xml` & `Simba-UW-tf-dev-1.58.8/simba/outlier_tools/.idea/workspace.xml`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.7/simba/SimBA.py` & `Simba-UW-tf-dev-1.58.8/simba/SimBA.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.7/simba/assets/unsupervised/.DS_Store` & `Simba-UW-tf-dev-1.58.8/simba/assets/unsupervised/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.7/simba/assets/unsupervised/model_names.parquet` & `Simba-UW-tf-dev-1.58.8/simba/assets/unsupervised/model_names.parquet`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.7/simba/assets/unsupervised/features.csv` & `Simba-UW-tf-dev-1.58.8/simba/assets/unsupervised/features.csv`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.7/simba/assets/shap/down_arrow.jpg` & `Simba-UW-tf-dev-1.58.8/simba/assets/shap/down_arrow.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.7/simba/assets/shap/intruder_shape.jpg` & `Simba-UW-tf-dev-1.58.8/simba/assets/shap/intruder_shape.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.7/simba/assets/shap/feature_categories/shap_feature_categories.csv` & `Simba-UW-tf-dev-1.58.8/simba/assets/shap/feature_categories/shap_feature_categories.csv`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.7/simba/assets/shap/.DS_Store` & `Simba-UW-tf-dev-1.58.8/simba/assets/shap/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.7/simba/assets/shap/resident_shape.jpg` & `Simba-UW-tf-dev-1.58.8/simba/assets/shap/resident_shape.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.7/simba/assets/shap/resident_intruder_shape.jpg` & `Simba-UW-tf-dev-1.58.8/simba/assets/shap/resident_intruder_shape.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.7/simba/assets/shap/animal_distances.jpg` & `Simba-UW-tf-dev-1.58.8/simba/assets/shap/animal_distances.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.7/simba/assets/shap/baseline_scale.jpg` & `Simba-UW-tf-dev-1.58.8/simba/assets/shap/baseline_scale.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.7/simba/assets/shap/ubuntu.regular.ttf` & `Simba-UW-tf-dev-1.58.8/simba/assets/shap/ubuntu.regular.ttf`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.7/simba/assets/shap/side_scale.jpg` & `Simba-UW-tf-dev-1.58.8/simba/assets/shap/side_scale.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.7/simba/assets/shap/UbuntuMono-Regular.ttf` & `Simba-UW-tf-dev-1.58.8/simba/assets/shap/UbuntuMono-Regular.ttf`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.7/simba/assets/shap/side_scale_5.jpg` & `Simba-UW-tf-dev-1.58.8/simba/assets/shap/side_scale_5.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.7/simba/assets/shap/intruder_movement.jpg` & `Simba-UW-tf-dev-1.58.8/simba/assets/shap/intruder_movement.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.7/simba/assets/shap/resident_movement.jpg` & `Simba-UW-tf-dev-1.58.8/simba/assets/shap/resident_movement.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.7/simba/assets/shap/color_bar.jpg` & `Simba-UW-tf-dev-1.58.8/simba/assets/shap/color_bar.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.7/simba/assets/shap/resident_intruder_movement.jpg` & `Simba-UW-tf-dev-1.58.8/simba/assets/shap/resident_intruder_movement.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.7/simba/assets/.DS_Store` & `Simba-UW-tf-dev-1.58.8/simba/assets/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.7/simba/assets/lookups/.DS_Store` & `Simba-UW-tf-dev-1.58.8/simba/assets/lookups/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.7/simba/assets/lookups/model_names.parquet` & `Simba-UW-tf-dev-1.58.8/simba/assets/lookups/model_names.parquet`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.7/simba/assets/lookups/feature_extraction_headers.csv` & `Simba-UW-tf-dev-1.58.8/simba/assets/lookups/feature_extraction_headers.csv`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.7/simba/assets/lookups/features.csv` & `Simba-UW-tf-dev-1.58.8/simba/assets/lookups/features.csv`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.7/simba/assets/lookups/unsupervised_example_x.csv` & `Simba-UW-tf-dev-1.58.8/simba/assets/lookups/unsupervised_example_x.csv`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.7/simba/assets/stl/operant_tray.stl` & `Simba-UW-tf-dev-1.58.8/simba/assets/stl/operant_tray.stl`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.7/simba/assets/stl/operant_lever.stl` & `Simba-UW-tf-dev-1.58.8/simba/assets/stl/operant_lever.stl`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.7/simba/assets/stl/operant_walls.stl` & `Simba-UW-tf-dev-1.58.8/simba/assets/stl/operant_walls.stl`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.7/simba/assets/stl/grid_floor.stl` & `Simba-UW-tf-dev-1.58.8/simba/assets/stl/grid_floor.stl`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.7/simba/assets/img/.DS_Store` & `Simba-UW-tf-dev-1.58.8/simba/assets/img/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.7/simba/assets/img/about_me.png` & `Simba-UW-tf-dev-1.58.8/simba/assets/img/about_me.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.7/simba/assets/img/splash.mp4` & `Simba-UW-tf-dev-1.58.8/simba/assets/img/splash.mp4`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.7/simba/assets/img/bg_2.png` & `Simba-UW-tf-dev-1.58.8/simba/assets/img/bg_2.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.7/simba/assets/img/splash.pptx` & `Simba-UW-tf-dev-1.58.8/simba/assets/img/splash.pptx`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.7/simba/assets/img/bg.png` & `Simba-UW-tf-dev-1.58.8/simba/assets/img/bg.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.7/simba/assets/UbuntuMono-Regular.ttf` & `Simba-UW-tf-dev-1.58.8/simba/assets/UbuntuMono-Regular.ttf`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.7/simba/assets/icons/factory.png` & `Simba-UW-tf-dev-1.58.8/simba/assets/icons/factory.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.7/simba/assets/icons/cluster.png` & `Simba-UW-tf-dev-1.58.8/simba/assets/icons/cluster.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.7/simba/assets/icons/load.png` & `Simba-UW-tf-dev-1.58.8/simba/assets/icons/load.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.7/simba/assets/icons/gif.png` & `Simba-UW-tf-dev-1.58.8/simba/assets/icons/gif.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.7/simba/assets/icons/pose.png` & `Simba-UW-tf-dev-1.58.8/simba/assets/icons/pose.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.7/simba/assets/icons/features.png` & `Simba-UW-tf-dev-1.58.8/simba/assets/icons/features.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.7/simba/assets/icons/.DS_Store` & `Simba-UW-tf-dev-1.58.8/simba/assets/icons/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.7/simba/assets/icons/settings.png` & `Simba-UW-tf-dev-1.58.8/simba/assets/icons/settings.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.7/simba/assets/icons/stopwatch.png` & `Simba-UW-tf-dev-1.58.8/simba/assets/icons/stopwatch.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.7/simba/assets/icons/link.png` & `Simba-UW-tf-dev-1.58.8/simba/assets/icons/link.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.7/simba/assets/icons/dash_simba.css` & `Simba-UW-tf-dev-1.58.8/simba/assets/icons/dash_simba.css`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.7/simba/assets/icons/documentation.png` & `Simba-UW-tf-dev-1.58.8/simba/assets/icons/documentation.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.7/simba/assets/icons/fps.png` & `Simba-UW-tf-dev-1.58.8/simba/assets/icons/fps.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.7/simba/assets/icons/dimensionality_reduction.png` & `Simba-UW-tf-dev-1.58.8/simba/assets/icons/dimensionality_reduction.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.7/simba/assets/icons/roi.png` & `Simba-UW-tf-dev-1.58.8/simba/assets/icons/roi.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.7/simba/assets/icons/superimpose.png` & `Simba-UW-tf-dev-1.58.8/simba/assets/icons/superimpose.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.7/simba/assets/icons/label.png` & `Simba-UW-tf-dev-1.58.8/simba/assets/icons/label.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.7/simba/assets/icons/change.png` & `Simba-UW-tf-dev-1.58.8/simba/assets/icons/change.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.7/simba/assets/icons/crop.png` & `Simba-UW-tf-dev-1.58.8/simba/assets/icons/crop.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.7/simba/assets/icons/rotate.png` & `Simba-UW-tf-dev-1.58.8/simba/assets/icons/rotate.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.7/simba/assets/icons/path.png` & `Simba-UW-tf-dev-1.58.8/simba/assets/icons/path.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.7/simba/assets/icons/clip.png` & `Simba-UW-tf-dev-1.58.8/simba/assets/icons/clip.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.7/simba/assets/icons/restart.png` & `Simba-UW-tf-dev-1.58.8/simba/assets/icons/restart.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.7/simba/assets/icons/calipher.png` & `Simba-UW-tf-dev-1.58.8/simba/assets/icons/calipher.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.7/simba/assets/icons/add_on.png` & `Simba-UW-tf-dev-1.58.8/simba/assets/icons/add_on.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.7/simba/assets/icons/create.png` & `Simba-UW-tf-dev-1.58.8/simba/assets/icons/create.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.7/simba/assets/icons/SimBA_logo.ico` & `Simba-UW-tf-dev-1.58.8/simba/assets/icons/SimBA_logo.ico`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.7/simba/assets/icons/print.png` & `Simba-UW-tf-dev-1.58.8/simba/assets/icons/print.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.7/simba/assets/icons/clf.png` & `Simba-UW-tf-dev-1.58.8/simba/assets/icons/clf.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.7/simba/assets/icons/concat_icons/mosaic.png` & `Simba-UW-tf-dev-1.58.8/simba/assets/icons/concat_icons/mosaic.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.7/simba/assets/icons/concat_icons/vertical.png` & `Simba-UW-tf-dev-1.58.8/simba/assets/icons/concat_icons/vertical.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.7/simba/assets/icons/concat_icons/horizontal.png` & `Simba-UW-tf-dev-1.58.8/simba/assets/icons/concat_icons/horizontal.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.7/simba/assets/icons/concat_icons/mixed_mosaic.png` & `Simba-UW-tf-dev-1.58.8/simba/assets/icons/concat_icons/mixed_mosaic.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.7/simba/assets/icons/merge.png` & `Simba-UW-tf-dev-1.58.8/simba/assets/icons/merge.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.7/simba/assets/icons/clean.png` & `Simba-UW-tf-dev-1.58.8/simba/assets/icons/clean.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.7/simba/assets/icons/clf_2.png` & `Simba-UW-tf-dev-1.58.8/simba/assets/icons/clf_2.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.7/simba/assets/icons/visualize.png` & `Simba-UW-tf-dev-1.58.8/simba/assets/icons/visualize.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.7/simba/assets/icons/concat.png` & `Simba-UW-tf-dev-1.58.8/simba/assets/icons/concat.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.7/simba/assets/icons/boris.png` & `Simba-UW-tf-dev-1.58.8/simba/assets/icons/boris.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.7/simba/assets/icons/frames.png` & `Simba-UW-tf-dev-1.58.8/simba/assets/icons/frames.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.7/simba/assets/icons/video.png` & `Simba-UW-tf-dev-1.58.8/simba/assets/icons/video.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.7/simba/assets/icons/sample.png` & `Simba-UW-tf-dev-1.58.8/simba/assets/icons/sample.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.7/simba/assets/icons/metrics.png` & `Simba-UW-tf-dev-1.58.8/simba/assets/icons/metrics.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.7/simba/assets/icons/grey.png` & `Simba-UW-tf-dev-1.58.8/simba/assets/icons/grey.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.7/simba/assets/icons/exit.png` & `Simba-UW-tf-dev-1.58.8/simba/assets/icons/exit.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.7/simba/assets/icons/outlier.png` & `Simba-UW-tf-dev-1.58.8/simba/assets/icons/outlier.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.7/simba/assets/icons/clahe.png` & `Simba-UW-tf-dev-1.58.8/simba/assets/icons/clahe.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.7/simba/assets/icons/trash.png` & `Simba-UW-tf-dev-1.58.8/simba/assets/icons/trash.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.7/simba/assets/icons/about.png` & `Simba-UW-tf-dev-1.58.8/simba/assets/icons/about.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.7/simba/assets/icons/convert.png` & `Simba-UW-tf-dev-1.58.8/simba/assets/icons/convert.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.7/simba/assets/icons/SimBA_logo.icns` & `Simba-UW-tf-dev-1.58.8/simba/assets/icons/SimBA_logo.icns`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.7/simba/assets/icons/reorganize.png` & `Simba-UW-tf-dev-1.58.8/simba/assets/icons/reorganize.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.7/simba/assets/icons/browse.png` & `Simba-UW-tf-dev-1.58.8/simba/assets/icons/browse.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.7/simba/assets/icons/SimBA_logo.png` & `Simba-UW-tf-dev-1.58.8/simba/assets/icons/SimBA_logo.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.7/simba/assets/icons/ethovision.png` & `Simba-UW-tf-dev-1.58.8/simba/assets/icons/ethovision.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.7/simba/assets/icons/close.png` & `Simba-UW-tf-dev-1.58.8/simba/assets/icons/close.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.7/simba/assets/dash_simba_base.css` & `Simba-UW-tf-dev-1.58.8/simba/assets/dash_simba_base.css`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.7/simba/assets/TheGoldenLab.PNG` & `Simba-UW-tf-dev-1.58.8/simba/assets/TheGoldenLab.PNG`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.7/Simba_UW_tf_dev.egg-info/PKG-INFO` & `Simba-UW-tf-dev-1.58.8/Simba_UW_tf_dev.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Simba-UW-tf-dev
-Version: 1.58.7
+Version: 1.58.8
 Summary: Toolkit for computer classification of complex social behaviors in experimental animals
 Home-page: https://github.com/sgoldenlab/simba
 Author: Simon Nilsson, Jia Jie Choong, Sophia Hwang
 Author-email: sronilsson@gmail.com
 License: GNU Lesser General Public License v3 (LGPLv3)
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `Simba-UW-tf-dev-1.58.7/Simba_UW_tf_dev.egg-info/SOURCES.txt` & `Simba-UW-tf-dev-1.58.8/Simba_UW_tf_dev.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.7/Simba_UW_tf_dev.egg-info/requires.txt` & `Simba-UW-tf-dev-1.58.8/Simba_UW_tf_dev.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.7/LICENSE.md` & `Simba-UW-tf-dev-1.58.8/LICENSE.md`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.7/README.md` & `Simba-UW-tf-dev-1.58.8/README.md`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.7/setup.py` & `Simba-UW-tf-dev-1.58.8/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 Licensed under GNU Lesser General Public License v3.0
 """
 
 import setuptools
 
 setuptools.setup(
     name="Simba-UW-tf-dev",
-    version="1.58.7",
+    version="1.58.8",
     author="Simon Nilsson, Jia Jie Choong, Sophia Hwang",
     author_email="sronilsson@gmail.com",
     description="Toolkit for computer classification of complex social behaviors in experimental animals",
     url="https://github.com/sgoldenlab/simba",
     install_requires=['Pillow == 5.4.1', 'pyyaml == 5.3.1','shapely == 1.7','wxpython == 4.0.4',
               'dtreeviz == 0.8.1','eli5 == 0.10.1','graphviz == 0.11',
               'imblearn == 0.0','imgaug == 0.4.0','imutils == 0.5.2','matplotlib == 3.0.3', 'numpy == 1.18.1',
```

