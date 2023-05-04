# Comparing `tmp/tartanair-1.0.2.tar.gz` & `tmp/tartanair-1.0.3.tar.gz`

## Comparing `tartanair-1.0.2.tar` & `tartanair-1.0.3.tar`

### file list

```diff
@@ -1,125 +1,126 @@
--rw-r--r--   0        0        0      748 2020-02-02 00:00:00.000000 tartanair-1.0.2/.gitmodules
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 tartanair-1.0.2/__init__.py
--rw-r--r--   0        0        0      694 2020-02-02 00:00:00.000000 tartanair-1.0.2/.github/workflows/documentation.yaml
--rw-r--r--   0        0        0     2154 2020-02-02 00:00:00.000000 tartanair-1.0.2/docs/conf.py
--rw-r--r--   0        0        0     9378 2020-02-02 00:00:00.000000 tartanair-1.0.2/docs/examples.rst
--rw-r--r--   0        0        0     1146 2020-02-02 00:00:00.000000 tartanair-1.0.2/docs/index.rst
--rw-r--r--   0        0        0     2663 2020-02-02 00:00:00.000000 tartanair-1.0.2/docs/installation.rst
--rw-r--r--   0        0        0      654 2020-02-02 00:00:00.000000 tartanair-1.0.2/docs/usage.rst
--rw-r--r--   0        0        0     1695 2020-02-02 00:00:00.000000 tartanair-1.0.2/examples/customization_example.py
--rw-r--r--   0        0        0     5833 2020-02-02 00:00:00.000000 tartanair-1.0.2/examples/dataloader_example.py
--rw-r--r--   0        0        0     4216 2020-02-02 00:00:00.000000 tartanair-1.0.2/examples/dataset_example.py
--rw-r--r--   0        0        0      365 2020-02-02 00:00:00.000000 tartanair-1.0.2/examples/download_config.yaml
--rw-r--r--   0        0        0     1310 2020-02-02 00:00:00.000000 tartanair-1.0.2/examples/download_example.py
--rw-r--r--   0        0        0     1350 2020-02-02 00:00:00.000000 tartanair-1.0.2/examples/evaluator_example.py
--rw-r--r--   0        0        0      595 2020-02-02 00:00:00.000000 tartanair-1.0.2/examples/get_traj_example.py
--rw-r--r--   0        0        0      553 2020-02-02 00:00:00.000000 tartanair-1.0.2/examples/iterator_example.py
--rw-r--r--   0        0        0      551 2020-02-02 00:00:00.000000 tartanair-1.0.2/examples/list_example.py
--rw-r--r--   0        0        0     6754 2020-02-02 00:00:00.000000 tartanair-1.0.2/examples/sanity_test.py
--rw-r--r--   0        0        0     6203 2020-02-02 00:00:00.000000 tartanair-1.0.2/examples/slowloader_example.py
--rw-r--r--   0        0        0     8836 2020-02-02 00:00:00.000000 tartanair-1.0.2/examples/trippy_video.py
--rw-r--r--   0        0        0      565 2020-02-02 00:00:00.000000 tartanair-1.0.2/examples/visualization_example.py
--rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 tartanair-1.0.2/tartanair/__init__.py
--rw-r--r--   0        0        0    25971 2020-02-02 00:00:00.000000 tartanair-1.0.2/tartanair/customizer.py
--rw-r--r--   0        0        0    14773 2020-02-02 00:00:00.000000 tartanair-1.0.2/tartanair/dataloader.py
--rw-r--r--   0        0        0    40499 2020-02-02 00:00:00.000000 tartanair-1.0.2/tartanair/dataset.py
--rw-r--r--   0        0        0    11978 2020-02-02 00:00:00.000000 tartanair-1.0.2/tartanair/downloader.py
--rw-r--r--   0        0        0     4645 2020-02-02 00:00:00.000000 tartanair-1.0.2/tartanair/evaluator.py
--rw-r--r--   0        0        0    16084 2020-02-02 00:00:00.000000 tartanair-1.0.2/tartanair/iterator.py
--rw-r--r--   0        0        0     1190 2020-02-02 00:00:00.000000 tartanair-1.0.2/tartanair/lister.py
--rw-r--r--   0        0        0     4249 2020-02-02 00:00:00.000000 tartanair-1.0.2/tartanair/reader.py
--rw-r--r--   0        0        0    23789 2020-02-02 00:00:00.000000 tartanair-1.0.2/tartanair/tartanair.py
--rw-r--r--   0        0        0     4285 2020-02-02 00:00:00.000000 tartanair-1.0.2/tartanair/tartanair_module.py
--rw-r--r--   0        0        0     4938 2020-02-02 00:00:00.000000 tartanair-1.0.2/tartanair/visualizer.py
--rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 tartanair-1.0.2/tartanair/data_cacher/.git
--rw-r--r--   0        0        0     4962 2020-02-02 00:00:00.000000 tartanair-1.0.2/tartanair/data_cacher/CacherDataset.py
--rw-r--r--   0        0        0     4487 2020-02-02 00:00:00.000000 tartanair-1.0.2/tartanair/data_cacher/ConfigParser.py
--rw-r--r--   0        0        0     9452 2020-02-02 00:00:00.000000 tartanair-1.0.2/tartanair/data_cacher/DataCacher.py
--rw-r--r--   0        0        0     3466 2020-02-02 00:00:00.000000 tartanair-1.0.2/tartanair/data_cacher/DataSplitter.py
--rw-r--r--   0        0        0     1298 2020-02-02 00:00:00.000000 tartanair-1.0.2/tartanair/data_cacher/LICENSE
--rw-r--r--   0        0        0     9715 2020-02-02 00:00:00.000000 tartanair-1.0.2/tartanair/data_cacher/MultiDatasets.py
--rw-r--r--   0        0        0     2884 2020-02-02 00:00:00.000000 tartanair-1.0.2/tartanair/data_cacher/RAMBuffer.py
--rw-r--r--   0        0        0    10184 2020-02-02 00:00:00.000000 tartanair-1.0.2/tartanair/data_cacher/RAMDataset.py
--rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 tartanair-1.0.2/tartanair/data_cacher/README.md
--rw-r--r--   0        0        0     5346 2020-02-02 00:00:00.000000 tartanair-1.0.2/tartanair/data_cacher/TrajBuffer.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tartanair-1.0.2/tartanair/data_cacher/__init__.py
--rw-r--r--   0        0        0     9001 2020-02-02 00:00:00.000000 tartanair-1.0.2/tartanair/data_cacher/data_roots.py
--rw-r--r--   0        0        0     1275 2020-02-02 00:00:00.000000 tartanair-1.0.2/tartanair/data_cacher/input_parser.py
--rw-r--r--   0        0        0    43545 2020-02-02 00:00:00.000000 tartanair-1.0.2/tartanair/data_cacher/utils.py
--rw-r--r--   0        0        0     1168 2020-02-02 00:00:00.000000 tartanair-1.0.2/tartanair/data_cacher/dataspec/flowvo_train_local_v1.yaml
--rw-r--r--   0        0        0     1200 2020-02-02 00:00:00.000000 tartanair-1.0.2/tartanair/data_cacher/dataspec/flowvo_train_local_v2.yaml
--rw-r--r--   0        0        0     5009 2020-02-02 00:00:00.000000 tartanair-1.0.2/tartanair/data_cacher/modality_type/ModBase.py
--rw-r--r--   0        0        0      130 2020-02-02 00:00:00.000000 tartanair-1.0.2/tartanair/data_cacher/modality_type/__init__.py
--rw-r--r--   0        0        0      600 2020-02-02 00:00:00.000000 tartanair-1.0.2/tartanair/data_cacher/modality_type/ply_io.py
--rw-r--r--   0        0        0    22699 2020-02-02 00:00:00.000000 tartanair-1.0.2/tartanair/data_cacher/modality_type/tartanair_types.py
--rw-r--r--   0        0        0     9737 2020-02-02 00:00:00.000000 tartanair-1.0.2/tartanair/data_cacher/modality_type/tartanairv1_types.py
--rw-r--r--   0        0        0     7968 2020-02-02 00:00:00.000000 tartanair-1.0.2/tartanair/data_cacher/modality_type/tartandrive_types.py
--rw-r--r--   0        0        0      544 2020-02-02 00:00:00.000000 tartanair-1.0.2/tartanair/data_cacher/modality_type/test_register.py
--rw-r--r--   0        0        0     4551 2020-02-02 00:00:00.000000 tartanair-1.0.2/tartanair/eval_utils/trajectory_evaluator_ate.py
--rw-r--r--   0        0        0     9795 2020-02-02 00:00:00.000000 tartanair-1.0.2/tartanair/eval_utils/trajectory_evaluator_base.py
--rw-r--r--   0        0        0     4972 2020-02-02 00:00:00.000000 tartanair-1.0.2/tartanair/eval_utils/trajectory_evaluator_rpe.py
--rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 tartanair-1.0.2/tartanair/image_resampling/image_sampler/.git
--rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 tartanair-1.0.2/tartanair/image_resampling/image_sampler/LICENSE
--rw-r--r--   0        0        0      614 2020-02-02 00:00:00.000000 tartanair-1.0.2/tartanair/image_resampling/image_sampler/__init__.py
--rw-r--r--   0        0        0     3636 2020-02-02 00:00:00.000000 tartanair-1.0.2/tartanair/image_resampling/image_sampler/blend_function.py
--rw-r--r--   0        0        0     6911 2020-02-02 00:00:00.000000 tartanair-1.0.2/tartanair/image_resampling/image_sampler/camera_model_sampler.py
--rw-r--r--   0        0        0    11078 2020-02-02 00:00:00.000000 tartanair-1.0.2/tartanair/image_resampling/image_sampler/full_view_rotation.py
--rw-r--r--   0        0        0     3048 2020-02-02 00:00:00.000000 tartanair-1.0.2/tartanair/image_resampling/image_sampler/generic_camera_model_sampler.py
--rw-r--r--   0        0        0      551 2020-02-02 00:00:00.000000 tartanair-1.0.2/tartanair/image_resampling/image_sampler/numba_support_check.py
--rw-r--r--   0        0        0     3945 2020-02-02 00:00:00.000000 tartanair-1.0.2/tartanair/image_resampling/image_sampler/ocv_torch.py
--rw-r--r--   0        0        0     9941 2020-02-02 00:00:00.000000 tartanair-1.0.2/tartanair/image_resampling/image_sampler/planar_as_base.py
--rw-r--r--   0        0        0      779 2020-02-02 00:00:00.000000 tartanair-1.0.2/tartanair/image_resampling/image_sampler/register.py
--rw-r--r--   0        0        0     9238 2020-02-02 00:00:00.000000 tartanair-1.0.2/tartanair/image_resampling/image_sampler/six_images.py
--rw-r--r--   0        0        0     5297 2020-02-02 00:00:00.000000 tartanair-1.0.2/tartanair/image_resampling/image_sampler/six_images_common.py
--rw-r--r--   0        0        0     3420 2020-02-02 00:00:00.000000 tartanair-1.0.2/tartanair/image_resampling/image_sampler/six_images_cupy.cu
--rw-r--r--   0        0        0     6908 2020-02-02 00:00:00.000000 tartanair-1.0.2/tartanair/image_resampling/image_sampler/six_images_numba.py
--rw-r--r--   0        0        0     6475 2020-02-02 00:00:00.000000 tartanair-1.0.2/tartanair/image_resampling/image_sampler/six_images_py_numba.py
--rw-r--r--   0        0        0     1117 2020-02-02 00:00:00.000000 tartanair-1.0.2/tartanair/image_resampling/image_sampler/examples/README.md
--rw-r--r--   0        0        0     8745 2020-02-02 00:00:00.000000 tartanair-1.0.2/tartanair/image_resampling/image_sampler/examples/generic_sampler_optical_flow_sampling_example.py
--rw-r--r--   0        0        0   445601 2020-02-02 00:00:00.000000 tartanair-1.0.2/tartanair/image_resampling/image_sampler/examples/data/flow_img.pt
--rw-r--r--   0        0        0     9716 2020-02-02 00:00:00.000000 tartanair-1.0.2/tartanair/image_resampling/image_sampler/examples/examples_utils/visualization_utils.py
--rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 tartanair-1.0.2/tartanair/image_resampling/mvs_utils/.git
--rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 tartanair-1.0.2/tartanair/image_resampling/mvs_utils/.gitmodules
--rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 tartanair-1.0.2/tartanair/image_resampling/mvs_utils/LICENSE
--rw-r--r--   0        0        0      496 2020-02-02 00:00:00.000000 tartanair-1.0.2/tartanair/image_resampling/mvs_utils/README.md
--rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 tartanair-1.0.2/tartanair/image_resampling/mvs_utils/__init__.py
--rw-r--r--   0        0        0    50658 2020-02-02 00:00:00.000000 tartanair-1.0.2/tartanair/image_resampling/mvs_utils/camera_models.py
--rw-r--r--   0        0        0     1334 2020-02-02 00:00:00.000000 tartanair-1.0.2/tartanair/image_resampling/mvs_utils/compatible_torch.py
--rw-r--r--   0        0        0     1835 2020-02-02 00:00:00.000000 tartanair-1.0.2/tartanair/image_resampling/mvs_utils/debug.py
--rw-r--r--   0        0        0      488 2020-02-02 00:00:00.000000 tartanair-1.0.2/tartanair/image_resampling/mvs_utils/file_sys.py
--rw-r--r--   0        0        0     5006 2020-02-02 00:00:00.000000 tartanair-1.0.2/tartanair/image_resampling/mvs_utils/frame_io.py
--rw-r--r--   0        0        0     9602 2020-02-02 00:00:00.000000 tartanair-1.0.2/tartanair/image_resampling/mvs_utils/kalibr_parser.py
--rw-r--r--   0        0        0     7146 2020-02-02 00:00:00.000000 tartanair-1.0.2/tartanair/image_resampling/mvs_utils/metadata_reader.py
--rw-r--r--   0        0        0     1868 2020-02-02 00:00:00.000000 tartanair-1.0.2/tartanair/image_resampling/mvs_utils/point_cloud_helper.py
--rw-r--r--   0        0        0     3784 2020-02-02 00:00:00.000000 tartanair-1.0.2/tartanair/image_resampling/mvs_utils/pose.py
--rw-r--r--   0        0        0    14499 2020-02-02 00:00:00.000000 tartanair-1.0.2/tartanair/image_resampling/mvs_utils/pretty_dict.py
--rw-r--r--   0        0        0     1236 2020-02-02 00:00:00.000000 tartanair-1.0.2/tartanair/image_resampling/mvs_utils/shape_struct.py
--rw-r--r--   0        0        0     6392 2020-02-02 00:00:00.000000 tartanair-1.0.2/tartanair/image_resampling/mvs_utils/simulated_lidar_pre_def_models.py
--rw-r--r--   0        0        0     1949 2020-02-02 00:00:00.000000 tartanair-1.0.2/tartanair/image_resampling/mvs_utils/test_frame_io.py
--rw-r--r--   0        0        0     1085 2020-02-02 00:00:00.000000 tartanair-1.0.2/tartanair/image_resampling/mvs_utils/test_inheritance.py
--rw-r--r--   0        0        0     1604 2020-02-02 00:00:00.000000 tartanair-1.0.2/tartanair/image_resampling/mvs_utils/examples/README.md
--rw-r--r--   0        0        0     4941 2020-02-02 00:00:00.000000 tartanair-1.0.2/tartanair/image_resampling/mvs_utils/examples/linear_fisheye_camera_model.py
--rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 tartanair-1.0.2/tartanair/image_resampling/mvs_utils/ftensor/.git
--rw-r--r--   0        0        0     1065 2020-02-02 00:00:00.000000 tartanair-1.0.2/tartanair/image_resampling/mvs_utils/ftensor/LICENSE
--rw-r--r--   0        0        0     3170 2020-02-02 00:00:00.000000 tartanair-1.0.2/tartanair/image_resampling/mvs_utils/ftensor/README.md
--rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 tartanair-1.0.2/tartanair/image_resampling/mvs_utils/ftensor/__init__.py
--rw-r--r--   0        0        0     8218 2020-02-02 00:00:00.000000 tartanair-1.0.2/tartanair/image_resampling/mvs_utils/ftensor/_pytree.py
--rw-r--r--   0        0        0      368 2020-02-02 00:00:00.000000 tartanair-1.0.2/tartanair/image_resampling/mvs_utils/ftensor/compatible_pytree.py
--rw-r--r--   0        0        0     5422 2020-02-02 00:00:00.000000 tartanair-1.0.2/tartanair/image_resampling/mvs_utils/ftensor/frame_graph.py
--rw-r--r--   0        0        0    18394 2020-02-02 00:00:00.000000 tartanair-1.0.2/tartanair/image_resampling/mvs_utils/ftensor/ftensor.py
--rw-r--r--   0        0        0     2406 2020-02-02 00:00:00.000000 tartanair-1.0.2/tartanair/image_resampling/mvs_utils/ftensor/test_frame_graph.py
--rw-r--r--   0        0        0    18694 2020-02-02 00:00:00.000000 tartanair-1.0.2/tartanair/image_resampling/mvs_utils/ftensor/test_ftensor.py
--rw-r--r--   0        0        0      447 2020-02-02 00:00:00.000000 tartanair-1.0.2/tartanair/image_resampling/mvs_utils/image_io/__init__.py
--rw-r--r--   0        0        0      704 2020-02-02 00:00:00.000000 tartanair-1.0.2/tartanair/image_resampling/mvs_utils/image_io/float_type.py
--rw-r--r--   0        0        0      604 2020-02-02 00:00:00.000000 tartanair-1.0.2/tartanair/image_resampling/mvs_utils/image_io/image_read.py
--rw-r--r--   0        0        0     3446 2020-02-02 00:00:00.000000 tartanair-1.0.2/tartanair/image_resampling/mvs_utils/image_io/image_write.py
--rw-r--r--   0        0        0     3774 2020-02-02 00:00:00.000000 tartanair-1.0.2/tartanair/image_resampling/mvs_utils/test_data/frame_graph.json
--rw-r--r--   0        0        0      798 2020-02-02 00:00:00.000000 tartanair-1.0.2/tests/README.md
--rw-r--r--   0        0        0    14286 2020-02-02 00:00:00.000000 tartanair-1.0.2/tests/tartanairpy_test.py
--rw-r--r--   0        0        0      567 2020-02-02 00:00:00.000000 tartanair-1.0.2/tests/sample_tartanair_v2_data_root/ArchVizTinyHouseDayExposure/Data_hard/P000/image_lcam_custom0_doublesphere/camera_model_params_lcam_image_custom0_doublesphere.json
--rw-r--r--   0        0        0      461 2020-02-02 00:00:00.000000 tartanair-1.0.2/tests/sample_tartanair_v2_data_root/ArchVizTinyHouseDayExposure/Data_hard/P000/image_lcam_custom0_pinhole/camera_model_params_lcam_image_custom0_pinhole.json
--rw-r--r--   0        0        0     2031 2020-02-02 00:00:00.000000 tartanair-1.0.2/.gitignore
--rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 tartanair-1.0.2/LICENSE
--rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 tartanair-1.0.2/README.md
--rw-r--r--   0        0        0      855 2020-02-02 00:00:00.000000 tartanair-1.0.2/pyproject.toml
--rw-r--r--   0        0        0     1020 2020-02-02 00:00:00.000000 tartanair-1.0.2/PKG-INFO
+-rw-r--r--   0        0        0      748 2020-02-02 00:00:00.000000 tartanair-1.0.3/.gitmodules
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 tartanair-1.0.3/__init__.py
+-rw-r--r--   0        0        0      694 2020-02-02 00:00:00.000000 tartanair-1.0.3/.github/workflows/documentation.yaml
+-rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 tartanair-1.0.3/docs/CNAME
+-rw-r--r--   0        0        0     2154 2020-02-02 00:00:00.000000 tartanair-1.0.3/docs/conf.py
+-rw-r--r--   0        0        0     9378 2020-02-02 00:00:00.000000 tartanair-1.0.3/docs/examples.rst
+-rw-r--r--   0        0        0     1146 2020-02-02 00:00:00.000000 tartanair-1.0.3/docs/index.rst
+-rw-r--r--   0        0        0     2513 2020-02-02 00:00:00.000000 tartanair-1.0.3/docs/installation.rst
+-rw-r--r--   0        0        0      654 2020-02-02 00:00:00.000000 tartanair-1.0.3/docs/usage.rst
+-rw-r--r--   0        0        0     2337 2020-02-02 00:00:00.000000 tartanair-1.0.3/examples/customization_example.py
+-rw-r--r--   0        0        0     5833 2020-02-02 00:00:00.000000 tartanair-1.0.3/examples/dataloader_example.py
+-rw-r--r--   0        0        0     4215 2020-02-02 00:00:00.000000 tartanair-1.0.3/examples/dataset_example.py
+-rw-r--r--   0        0        0      365 2020-02-02 00:00:00.000000 tartanair-1.0.3/examples/download_config.yaml
+-rw-r--r--   0        0        0     1211 2020-02-02 00:00:00.000000 tartanair-1.0.3/examples/download_example.py
+-rw-r--r--   0        0        0     1350 2020-02-02 00:00:00.000000 tartanair-1.0.3/examples/evaluator_example.py
+-rw-r--r--   0        0        0      595 2020-02-02 00:00:00.000000 tartanair-1.0.3/examples/get_traj_example.py
+-rw-r--r--   0        0        0      553 2020-02-02 00:00:00.000000 tartanair-1.0.3/examples/iterator_example.py
+-rw-r--r--   0        0        0      551 2020-02-02 00:00:00.000000 tartanair-1.0.3/examples/list_example.py
+-rw-r--r--   0        0        0     6754 2020-02-02 00:00:00.000000 tartanair-1.0.3/examples/sanity_test.py
+-rw-r--r--   0        0        0     6196 2020-02-02 00:00:00.000000 tartanair-1.0.3/examples/slowloader_example.py
+-rw-r--r--   0        0        0     8836 2020-02-02 00:00:00.000000 tartanair-1.0.3/examples/trippy_video.py
+-rw-r--r--   0        0        0      565 2020-02-02 00:00:00.000000 tartanair-1.0.3/examples/visualization_example.py
+-rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 tartanair-1.0.3/tartanair/__init__.py
+-rw-r--r--   0        0        0    26194 2020-02-02 00:00:00.000000 tartanair-1.0.3/tartanair/customizer.py
+-rw-r--r--   0        0        0    14773 2020-02-02 00:00:00.000000 tartanair-1.0.3/tartanair/dataloader.py
+-rw-r--r--   0        0        0    40499 2020-02-02 00:00:00.000000 tartanair-1.0.3/tartanair/dataset.py
+-rw-r--r--   0        0        0    11978 2020-02-02 00:00:00.000000 tartanair-1.0.3/tartanair/downloader.py
+-rw-r--r--   0        0        0     4645 2020-02-02 00:00:00.000000 tartanair-1.0.3/tartanair/evaluator.py
+-rw-r--r--   0        0        0    16084 2020-02-02 00:00:00.000000 tartanair-1.0.3/tartanair/iterator.py
+-rw-r--r--   0        0        0     1190 2020-02-02 00:00:00.000000 tartanair-1.0.3/tartanair/lister.py
+-rw-r--r--   0        0        0     4249 2020-02-02 00:00:00.000000 tartanair-1.0.3/tartanair/reader.py
+-rw-r--r--   0        0        0    23789 2020-02-02 00:00:00.000000 tartanair-1.0.3/tartanair/tartanair.py
+-rw-r--r--   0        0        0     4285 2020-02-02 00:00:00.000000 tartanair-1.0.3/tartanair/tartanair_module.py
+-rw-r--r--   0        0        0     4938 2020-02-02 00:00:00.000000 tartanair-1.0.3/tartanair/visualizer.py
+-rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 tartanair-1.0.3/tartanair/data_cacher/.git
+-rw-r--r--   0        0        0     4962 2020-02-02 00:00:00.000000 tartanair-1.0.3/tartanair/data_cacher/CacherDataset.py
+-rw-r--r--   0        0        0     4487 2020-02-02 00:00:00.000000 tartanair-1.0.3/tartanair/data_cacher/ConfigParser.py
+-rw-r--r--   0        0        0     9452 2020-02-02 00:00:00.000000 tartanair-1.0.3/tartanair/data_cacher/DataCacher.py
+-rw-r--r--   0        0        0     3466 2020-02-02 00:00:00.000000 tartanair-1.0.3/tartanair/data_cacher/DataSplitter.py
+-rw-r--r--   0        0        0     1298 2020-02-02 00:00:00.000000 tartanair-1.0.3/tartanair/data_cacher/LICENSE
+-rw-r--r--   0        0        0     9715 2020-02-02 00:00:00.000000 tartanair-1.0.3/tartanair/data_cacher/MultiDatasets.py
+-rw-r--r--   0        0        0     2884 2020-02-02 00:00:00.000000 tartanair-1.0.3/tartanair/data_cacher/RAMBuffer.py
+-rw-r--r--   0        0        0    10184 2020-02-02 00:00:00.000000 tartanair-1.0.3/tartanair/data_cacher/RAMDataset.py
+-rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 tartanair-1.0.3/tartanair/data_cacher/README.md
+-rw-r--r--   0        0        0     5346 2020-02-02 00:00:00.000000 tartanair-1.0.3/tartanair/data_cacher/TrajBuffer.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tartanair-1.0.3/tartanair/data_cacher/__init__.py
+-rw-r--r--   0        0        0     9001 2020-02-02 00:00:00.000000 tartanair-1.0.3/tartanair/data_cacher/data_roots.py
+-rw-r--r--   0        0        0     1275 2020-02-02 00:00:00.000000 tartanair-1.0.3/tartanair/data_cacher/input_parser.py
+-rw-r--r--   0        0        0    43545 2020-02-02 00:00:00.000000 tartanair-1.0.3/tartanair/data_cacher/utils.py
+-rw-r--r--   0        0        0     1168 2020-02-02 00:00:00.000000 tartanair-1.0.3/tartanair/data_cacher/dataspec/flowvo_train_local_v1.yaml
+-rw-r--r--   0        0        0     1200 2020-02-02 00:00:00.000000 tartanair-1.0.3/tartanair/data_cacher/dataspec/flowvo_train_local_v2.yaml
+-rw-r--r--   0        0        0     5009 2020-02-02 00:00:00.000000 tartanair-1.0.3/tartanair/data_cacher/modality_type/ModBase.py
+-rw-r--r--   0        0        0      130 2020-02-02 00:00:00.000000 tartanair-1.0.3/tartanair/data_cacher/modality_type/__init__.py
+-rw-r--r--   0        0        0      600 2020-02-02 00:00:00.000000 tartanair-1.0.3/tartanair/data_cacher/modality_type/ply_io.py
+-rw-r--r--   0        0        0    22699 2020-02-02 00:00:00.000000 tartanair-1.0.3/tartanair/data_cacher/modality_type/tartanair_types.py
+-rw-r--r--   0        0        0     9737 2020-02-02 00:00:00.000000 tartanair-1.0.3/tartanair/data_cacher/modality_type/tartanairv1_types.py
+-rw-r--r--   0        0        0     7968 2020-02-02 00:00:00.000000 tartanair-1.0.3/tartanair/data_cacher/modality_type/tartandrive_types.py
+-rw-r--r--   0        0        0      544 2020-02-02 00:00:00.000000 tartanair-1.0.3/tartanair/data_cacher/modality_type/test_register.py
+-rw-r--r--   0        0        0     4551 2020-02-02 00:00:00.000000 tartanair-1.0.3/tartanair/eval_utils/trajectory_evaluator_ate.py
+-rw-r--r--   0        0        0     9795 2020-02-02 00:00:00.000000 tartanair-1.0.3/tartanair/eval_utils/trajectory_evaluator_base.py
+-rw-r--r--   0        0        0     4972 2020-02-02 00:00:00.000000 tartanair-1.0.3/tartanair/eval_utils/trajectory_evaluator_rpe.py
+-rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 tartanair-1.0.3/tartanair/image_resampling/image_sampler/.git
+-rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 tartanair-1.0.3/tartanair/image_resampling/image_sampler/LICENSE
+-rw-r--r--   0        0        0      614 2020-02-02 00:00:00.000000 tartanair-1.0.3/tartanair/image_resampling/image_sampler/__init__.py
+-rw-r--r--   0        0        0     3636 2020-02-02 00:00:00.000000 tartanair-1.0.3/tartanair/image_resampling/image_sampler/blend_function.py
+-rw-r--r--   0        0        0     6911 2020-02-02 00:00:00.000000 tartanair-1.0.3/tartanair/image_resampling/image_sampler/camera_model_sampler.py
+-rw-r--r--   0        0        0    11078 2020-02-02 00:00:00.000000 tartanair-1.0.3/tartanair/image_resampling/image_sampler/full_view_rotation.py
+-rw-r--r--   0        0        0     3048 2020-02-02 00:00:00.000000 tartanair-1.0.3/tartanair/image_resampling/image_sampler/generic_camera_model_sampler.py
+-rw-r--r--   0        0        0      551 2020-02-02 00:00:00.000000 tartanair-1.0.3/tartanair/image_resampling/image_sampler/numba_support_check.py
+-rw-r--r--   0        0        0     3945 2020-02-02 00:00:00.000000 tartanair-1.0.3/tartanair/image_resampling/image_sampler/ocv_torch.py
+-rw-r--r--   0        0        0     9941 2020-02-02 00:00:00.000000 tartanair-1.0.3/tartanair/image_resampling/image_sampler/planar_as_base.py
+-rw-r--r--   0        0        0      779 2020-02-02 00:00:00.000000 tartanair-1.0.3/tartanair/image_resampling/image_sampler/register.py
+-rw-r--r--   0        0        0     9238 2020-02-02 00:00:00.000000 tartanair-1.0.3/tartanair/image_resampling/image_sampler/six_images.py
+-rw-r--r--   0        0        0     5297 2020-02-02 00:00:00.000000 tartanair-1.0.3/tartanair/image_resampling/image_sampler/six_images_common.py
+-rw-r--r--   0        0        0     3420 2020-02-02 00:00:00.000000 tartanair-1.0.3/tartanair/image_resampling/image_sampler/six_images_cupy.cu
+-rw-r--r--   0        0        0     6908 2020-02-02 00:00:00.000000 tartanair-1.0.3/tartanair/image_resampling/image_sampler/six_images_numba.py
+-rw-r--r--   0        0        0     6475 2020-02-02 00:00:00.000000 tartanair-1.0.3/tartanair/image_resampling/image_sampler/six_images_py_numba.py
+-rw-r--r--   0        0        0     1117 2020-02-02 00:00:00.000000 tartanair-1.0.3/tartanair/image_resampling/image_sampler/examples/README.md
+-rw-r--r--   0        0        0     8745 2020-02-02 00:00:00.000000 tartanair-1.0.3/tartanair/image_resampling/image_sampler/examples/generic_sampler_optical_flow_sampling_example.py
+-rw-r--r--   0        0        0   445601 2020-02-02 00:00:00.000000 tartanair-1.0.3/tartanair/image_resampling/image_sampler/examples/data/flow_img.pt
+-rw-r--r--   0        0        0     9716 2020-02-02 00:00:00.000000 tartanair-1.0.3/tartanair/image_resampling/image_sampler/examples/examples_utils/visualization_utils.py
+-rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 tartanair-1.0.3/tartanair/image_resampling/mvs_utils/.git
+-rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 tartanair-1.0.3/tartanair/image_resampling/mvs_utils/.gitmodules
+-rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 tartanair-1.0.3/tartanair/image_resampling/mvs_utils/LICENSE
+-rw-r--r--   0        0        0      496 2020-02-02 00:00:00.000000 tartanair-1.0.3/tartanair/image_resampling/mvs_utils/README.md
+-rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 tartanair-1.0.3/tartanair/image_resampling/mvs_utils/__init__.py
+-rw-r--r--   0        0        0    74909 2020-02-02 00:00:00.000000 tartanair-1.0.3/tartanair/image_resampling/mvs_utils/camera_models.py
+-rw-r--r--   0        0        0     1334 2020-02-02 00:00:00.000000 tartanair-1.0.3/tartanair/image_resampling/mvs_utils/compatible_torch.py
+-rw-r--r--   0        0        0     1835 2020-02-02 00:00:00.000000 tartanair-1.0.3/tartanair/image_resampling/mvs_utils/debug.py
+-rw-r--r--   0        0        0      488 2020-02-02 00:00:00.000000 tartanair-1.0.3/tartanair/image_resampling/mvs_utils/file_sys.py
+-rw-r--r--   0        0        0     5006 2020-02-02 00:00:00.000000 tartanair-1.0.3/tartanair/image_resampling/mvs_utils/frame_io.py
+-rw-r--r--   0        0        0     9602 2020-02-02 00:00:00.000000 tartanair-1.0.3/tartanair/image_resampling/mvs_utils/kalibr_parser.py
+-rw-r--r--   0        0        0     7146 2020-02-02 00:00:00.000000 tartanair-1.0.3/tartanair/image_resampling/mvs_utils/metadata_reader.py
+-rw-r--r--   0        0        0     1868 2020-02-02 00:00:00.000000 tartanair-1.0.3/tartanair/image_resampling/mvs_utils/point_cloud_helper.py
+-rw-r--r--   0        0        0     3784 2020-02-02 00:00:00.000000 tartanair-1.0.3/tartanair/image_resampling/mvs_utils/pose.py
+-rw-r--r--   0        0        0    14499 2020-02-02 00:00:00.000000 tartanair-1.0.3/tartanair/image_resampling/mvs_utils/pretty_dict.py
+-rw-r--r--   0        0        0     1236 2020-02-02 00:00:00.000000 tartanair-1.0.3/tartanair/image_resampling/mvs_utils/shape_struct.py
+-rw-r--r--   0        0        0     6392 2020-02-02 00:00:00.000000 tartanair-1.0.3/tartanair/image_resampling/mvs_utils/simulated_lidar_pre_def_models.py
+-rw-r--r--   0        0        0     1949 2020-02-02 00:00:00.000000 tartanair-1.0.3/tartanair/image_resampling/mvs_utils/test_frame_io.py
+-rw-r--r--   0        0        0     1085 2020-02-02 00:00:00.000000 tartanair-1.0.3/tartanair/image_resampling/mvs_utils/test_inheritance.py
+-rw-r--r--   0        0        0     1604 2020-02-02 00:00:00.000000 tartanair-1.0.3/tartanair/image_resampling/mvs_utils/examples/README.md
+-rw-r--r--   0        0        0     4941 2020-02-02 00:00:00.000000 tartanair-1.0.3/tartanair/image_resampling/mvs_utils/examples/linear_fisheye_camera_model.py
+-rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 tartanair-1.0.3/tartanair/image_resampling/mvs_utils/ftensor/.git
+-rw-r--r--   0        0        0     1065 2020-02-02 00:00:00.000000 tartanair-1.0.3/tartanair/image_resampling/mvs_utils/ftensor/LICENSE
+-rw-r--r--   0        0        0     3170 2020-02-02 00:00:00.000000 tartanair-1.0.3/tartanair/image_resampling/mvs_utils/ftensor/README.md
+-rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 tartanair-1.0.3/tartanair/image_resampling/mvs_utils/ftensor/__init__.py
+-rw-r--r--   0        0        0     8218 2020-02-02 00:00:00.000000 tartanair-1.0.3/tartanair/image_resampling/mvs_utils/ftensor/_pytree.py
+-rw-r--r--   0        0        0      368 2020-02-02 00:00:00.000000 tartanair-1.0.3/tartanair/image_resampling/mvs_utils/ftensor/compatible_pytree.py
+-rw-r--r--   0        0        0     5422 2020-02-02 00:00:00.000000 tartanair-1.0.3/tartanair/image_resampling/mvs_utils/ftensor/frame_graph.py
+-rw-r--r--   0        0        0    18394 2020-02-02 00:00:00.000000 tartanair-1.0.3/tartanair/image_resampling/mvs_utils/ftensor/ftensor.py
+-rw-r--r--   0        0        0     2406 2020-02-02 00:00:00.000000 tartanair-1.0.3/tartanair/image_resampling/mvs_utils/ftensor/test_frame_graph.py
+-rw-r--r--   0        0        0    18694 2020-02-02 00:00:00.000000 tartanair-1.0.3/tartanair/image_resampling/mvs_utils/ftensor/test_ftensor.py
+-rw-r--r--   0        0        0      447 2020-02-02 00:00:00.000000 tartanair-1.0.3/tartanair/image_resampling/mvs_utils/image_io/__init__.py
+-rw-r--r--   0        0        0      704 2020-02-02 00:00:00.000000 tartanair-1.0.3/tartanair/image_resampling/mvs_utils/image_io/float_type.py
+-rw-r--r--   0        0        0      604 2020-02-02 00:00:00.000000 tartanair-1.0.3/tartanair/image_resampling/mvs_utils/image_io/image_read.py
+-rw-r--r--   0        0        0     3446 2020-02-02 00:00:00.000000 tartanair-1.0.3/tartanair/image_resampling/mvs_utils/image_io/image_write.py
+-rw-r--r--   0        0        0     3774 2020-02-02 00:00:00.000000 tartanair-1.0.3/tartanair/image_resampling/mvs_utils/test_data/frame_graph.json
+-rw-r--r--   0        0        0      798 2020-02-02 00:00:00.000000 tartanair-1.0.3/tests/README.md
+-rw-r--r--   0        0        0    14286 2020-02-02 00:00:00.000000 tartanair-1.0.3/tests/tartanairpy_test.py
+-rw-r--r--   0        0        0      567 2020-02-02 00:00:00.000000 tartanair-1.0.3/tests/sample_tartanair_v2_data_root/ArchVizTinyHouseDayExposure/Data_hard/P000/image_lcam_custom0_doublesphere/camera_model_params_lcam_image_custom0_doublesphere.json
+-rw-r--r--   0        0        0      461 2020-02-02 00:00:00.000000 tartanair-1.0.3/tests/sample_tartanair_v2_data_root/ArchVizTinyHouseDayExposure/Data_hard/P000/image_lcam_custom0_pinhole/camera_model_params_lcam_image_custom0_pinhole.json
+-rw-r--r--   0        0        0     2031 2020-02-02 00:00:00.000000 tartanair-1.0.3/.gitignore
+-rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 tartanair-1.0.3/LICENSE
+-rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 tartanair-1.0.3/README.md
+-rw-r--r--   0        0        0      818 2020-02-02 00:00:00.000000 tartanair-1.0.3/pyproject.toml
+-rw-r--r--   0        0        0      975 2020-02-02 00:00:00.000000 tartanair-1.0.3/PKG-INFO
```

### Comparing `tartanair-1.0.2/.gitmodules` & `tartanair-1.0.3/.gitmodules`

 * *Files identical despite different names*

### Comparing `tartanair-1.0.2/.github/workflows/documentation.yaml` & `tartanair-1.0.3/.github/workflows/documentation.yaml`

 * *Files identical despite different names*

### Comparing `tartanair-1.0.2/docs/conf.py` & `tartanair-1.0.3/docs/conf.py`

 * *Files identical despite different names*

### Comparing `tartanair-1.0.2/docs/examples.rst` & `tartanair-1.0.3/docs/examples.rst`

 * *Files identical despite different names*

### Comparing `tartanair-1.0.2/docs/index.rst` & `tartanair-1.0.3/docs/index.rst`

 * *Files identical despite different names*

### Comparing `tartanair-1.0.2/docs/installation.rst` & `tartanair-1.0.3/docs/installation.rst`

 * *Files 6% similar despite different names*

```diff
@@ -4,23 +4,17 @@
 =====================================
 To install the TartanAir Python package:
 
 .. code-block:: bash
 
     pip install tartanair
 
-TartanAir depends on PyTorch for some customization functionalities. Please install it on your system (we don't do it for you to avoid version conflicts). Please follow the instructions on the PyTorch website: https://pytorch.org/get-started/locally/ .
+TartanAir depends on PyTorch for some customization functionalities. Please install it, and Torchvision, on your system (we don't do it for you to avoid version conflicts). Please follow the instructions on the PyTorch website: https://pytorch.org/get-started/locally/ .
 That's it! You're ready to go.
 
-**Note while we are in development, please install using the following command:**   
-
-.. code-block:: bash
-
-    pip install -i https://test.pypi.org/simple/ tartanair
-
 Requirements
 ------------
 
 Currently the TartanAir Python package was only tested on Ubuntu 20.04. We will be testing on other operating systems in the future.
 
 Known Installation Issues and Solutions
 ---------------------------------------
```

### Comparing `tartanair-1.0.2/docs/usage.rst` & `tartanair-1.0.3/docs/usage.rst`

 * *Files identical despite different names*

### Comparing `tartanair-1.0.2/examples/customization_example.py` & `tartanair-1.0.3/examples/customization_example.py`

 * *Files 10% similar despite different names*

```diff
@@ -37,10 +37,26 @@
                         'cx': 500, 
                         'cy': 500, 
                         'width': 1000, 
                         'height': 1000, 
                         'alpha': 0.6, 
                         'xi': -0.2, 
                         'fov_degree': 195},
-                'R_raw_new': R_raw_new1}
+                'R_raw_new': np.eye(3).tolist()}
 
-ta.customize(env = 'ModularNeighborhoodIntExt', difficulty = 'easy', trajectory_id = ['P000'], modality = ['image'], new_camera_models_params=[cam_model_1, cam_model_0], num_workers = 2, device='cuda') # Or cpu.
+cam_model_2 = {'name': 'radtan', # TUM Fisheye parameters for cam0.
+                'raw_side': 'left',
+                'params':
+                        {
+                        'fx': 190.9227077601815,
+                        'fy': 190.89761005621563,
+                        'cx': 254.9135474328476,
+                        'cy': 256.8281792099312,
+                        'width': 1000,
+                        'height': 1000,
+                        'k1': 0.6288947328627524,
+                        'k2': 1.0441360489134845,
+                        'p1': 0.1,
+                        'p2': 0.1},
+                'R_raw_new': np.eye(3).tolist()}
+
+ta.customize(env = 'MiddleEastExposure', difficulty = 'easy', trajectory_id = ['P000'], modality = ['image'], new_camera_models_params=[cam_model_1], num_workers = 12, device='cuda') # Or cpu.
```

### Comparing `tartanair-1.0.2/examples/dataloader_example.py` & `tartanair-1.0.3/examples/dataloader_example.py`

 * *Files identical despite different names*

### Comparing `tartanair-1.0.2/examples/dataset_example.py` & `tartanair-1.0.3/examples/dataset_example.py`

 * *Files 0% similar despite different names*

```diff
@@ -66,15 +66,14 @@
     transforms.ToTensor(),
     
     # Resize the image.
     transforms.Resize((224, 224)),
 
     # Randomly flip the image.
     transforms.RandomHorizontalFlip(p = 1.0),
-
 ])
 
 # Set up a dataset.
 dataset = ta.create_image_dataset(env = [], difficulty = 'easy', trajectory_id = [], modality = ['image', 'depth'], camera_name = ['lcam_fish', 'lcam_front'], transform = transform)
 
 dataloader = DataLoader(dataset, batch_size = 3, shuffle = True, num_workers = 0)
```

### Comparing `tartanair-1.0.2/examples/evaluator_example.py` & `tartanair-1.0.3/examples/evaluator_example.py`

 * *Files identical despite different names*

### Comparing `tartanair-1.0.2/examples/get_traj_example.py` & `tartanair-1.0.3/examples/get_traj_example.py`

 * *Files identical despite different names*

### Comparing `tartanair-1.0.2/examples/iterator_example.py` & `tartanair-1.0.3/examples/iterator_example.py`

 * *Files identical despite different names*

### Comparing `tartanair-1.0.2/examples/list_example.py` & `tartanair-1.0.3/examples/list_example.py`

 * *Files identical despite different names*

### Comparing `tartanair-1.0.2/examples/sanity_test.py` & `tartanair-1.0.3/examples/sanity_test.py`

 * *Files identical despite different names*

### Comparing `tartanair-1.0.2/examples/slowloader_example.py` & `tartanair-1.0.3/examples/slowloader_example.py`

 * *Files 0% similar despite different names*

```diff
@@ -85,15 +85,14 @@
             batch_size = batch_size, 
             num_workers = num_workers, 
             shuffle = shuffle)
 
 
 print("Slowloader created in %f seconds." % (time.time() - starttime))
 
-exit()
 # Iterate over the batches.
 for i in range(30):    
     # Get the next batch.
     batch = dataloader.load_sample()
     # Check if the batch is None.
     if batch is None:
         break
```

### Comparing `tartanair-1.0.2/examples/trippy_video.py` & `tartanair-1.0.3/examples/trippy_video.py`

 * *Files identical despite different names*

### Comparing `tartanair-1.0.2/examples/visualization_example.py` & `tartanair-1.0.3/examples/visualization_example.py`

 * *Files identical despite different names*

### Comparing `tartanair-1.0.2/tartanair/customizer.py` & `tartanair-1.0.3/tartanair/customizer.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,28 +20,32 @@
 
 # Local imports.
 from .tartanair_module import TartanAirModule
 
 # Image resampling.
 from .image_resampling.image_sampler import SixPlanarNumba
 
-from .image_resampling.mvs_utils.camera_models import Pinhole, DoubleSphere, LinearSphere, Equirectangular
+from .image_resampling.mvs_utils.camera_models import Pinhole, DoubleSphere, LinearSphere, Equirectangular, PinholeRadTanFast
 from .image_resampling.mvs_utils.shape_struct import ShapeStruct
 from .image_resampling.image_sampler.blend_function import BlendBy2ndOrderGradTorch
 
 class TartanAirCustomizer(TartanAirModule):
     def __init__(self, tartanair_data_root):
         super().__init__(tartanair_data_root)
 
         # Member variables.
         # The root directory for the dataset.
         self.data_root = tartanair_data_root
 
         # Available camera models.
-        self.camera_model_name_to_class = {'pinhole': Pinhole, 'doublesphere': DoubleSphere, 'linearsphere': LinearSphere, 'equirect': Equirectangular}
+        self.camera_model_name_to_class = {'pinhole': Pinhole, 
+                                           'doublesphere': DoubleSphere, 
+                                           'linearsphere': LinearSphere, 
+                                           'equirect': Equirectangular,
+                                           'radtan': PinholeRadTanFast}
 
     def customize(self, env, difficulty = [], trajectory_id = [], modality = [], new_camera_models_params = [], R_raw_new = np.eye(4), num_workers = 1, device = 'cpu'):
         ###############################
         # Check the input arguments.
         ###############################
 
         print("Customizing the TartanAir dataset... With {} workers.".format(num_workers))
```

### Comparing `tartanair-1.0.2/tartanair/dataloader.py` & `tartanair-1.0.3/tartanair/dataloader.py`

 * *Files identical despite different names*

### Comparing `tartanair-1.0.2/tartanair/dataset.py` & `tartanair-1.0.3/tartanair/dataset.py`

 * *Files identical despite different names*

### Comparing `tartanair-1.0.2/tartanair/downloader.py` & `tartanair-1.0.3/tartanair/downloader.py`

 * *Files identical despite different names*

### Comparing `tartanair-1.0.2/tartanair/evaluator.py` & `tartanair-1.0.3/tartanair/evaluator.py`

 * *Files identical despite different names*

### Comparing `tartanair-1.0.2/tartanair/iterator.py` & `tartanair-1.0.3/tartanair/iterator.py`

 * *Files identical despite different names*

### Comparing `tartanair-1.0.2/tartanair/lister.py` & `tartanair-1.0.3/tartanair/lister.py`

 * *Files identical despite different names*

### Comparing `tartanair-1.0.2/tartanair/reader.py` & `tartanair-1.0.3/tartanair/reader.py`

 * *Files identical despite different names*

### Comparing `tartanair-1.0.2/tartanair/tartanair.py` & `tartanair-1.0.3/tartanair/tartanair.py`

 * *Files identical despite different names*

### Comparing `tartanair-1.0.2/tartanair/tartanair_module.py` & `tartanair-1.0.3/tartanair/tartanair_module.py`

 * *Files identical despite different names*

### Comparing `tartanair-1.0.2/tartanair/visualizer.py` & `tartanair-1.0.3/tartanair/visualizer.py`

 * *Files identical despite different names*

### Comparing `tartanair-1.0.2/tartanair/data_cacher/CacherDataset.py` & `tartanair-1.0.3/tartanair/data_cacher/CacherDataset.py`

 * *Files identical despite different names*

### Comparing `tartanair-1.0.2/tartanair/data_cacher/ConfigParser.py` & `tartanair-1.0.3/tartanair/data_cacher/ConfigParser.py`

 * *Files identical despite different names*

### Comparing `tartanair-1.0.2/tartanair/data_cacher/DataCacher.py` & `tartanair-1.0.3/tartanair/data_cacher/DataCacher.py`

 * *Files identical despite different names*

### Comparing `tartanair-1.0.2/tartanair/data_cacher/DataSplitter.py` & `tartanair-1.0.3/tartanair/data_cacher/DataSplitter.py`

 * *Files identical despite different names*

### Comparing `tartanair-1.0.2/tartanair/data_cacher/LICENSE` & `tartanair-1.0.3/tartanair/data_cacher/LICENSE`

 * *Files identical despite different names*

### Comparing `tartanair-1.0.2/tartanair/data_cacher/MultiDatasets.py` & `tartanair-1.0.3/tartanair/data_cacher/MultiDatasets.py`

 * *Files identical despite different names*

### Comparing `tartanair-1.0.2/tartanair/data_cacher/RAMBuffer.py` & `tartanair-1.0.3/tartanair/data_cacher/RAMBuffer.py`

 * *Files identical despite different names*

### Comparing `tartanair-1.0.2/tartanair/data_cacher/RAMDataset.py` & `tartanair-1.0.3/tartanair/data_cacher/RAMDataset.py`

 * *Files identical despite different names*

### Comparing `tartanair-1.0.2/tartanair/data_cacher/TrajBuffer.py` & `tartanair-1.0.3/tartanair/data_cacher/TrajBuffer.py`

 * *Files identical despite different names*

### Comparing `tartanair-1.0.2/tartanair/data_cacher/data_roots.py` & `tartanair-1.0.3/tartanair/data_cacher/data_roots.py`

 * *Files identical despite different names*

### Comparing `tartanair-1.0.2/tartanair/data_cacher/input_parser.py` & `tartanair-1.0.3/tartanair/data_cacher/input_parser.py`

 * *Files identical despite different names*

### Comparing `tartanair-1.0.2/tartanair/data_cacher/utils.py` & `tartanair-1.0.3/tartanair/data_cacher/utils.py`

 * *Files identical despite different names*

### Comparing `tartanair-1.0.2/tartanair/data_cacher/dataspec/flowvo_train_local_v1.yaml` & `tartanair-1.0.3/tartanair/data_cacher/dataspec/flowvo_train_local_v1.yaml`

 * *Files identical despite different names*

### Comparing `tartanair-1.0.2/tartanair/data_cacher/dataspec/flowvo_train_local_v2.yaml` & `tartanair-1.0.3/tartanair/data_cacher/dataspec/flowvo_train_local_v2.yaml`

 * *Files identical despite different names*

### Comparing `tartanair-1.0.2/tartanair/data_cacher/modality_type/ModBase.py` & `tartanair-1.0.3/tartanair/data_cacher/modality_type/ModBase.py`

 * *Files identical despite different names*

### Comparing `tartanair-1.0.2/tartanair/data_cacher/modality_type/ply_io.py` & `tartanair-1.0.3/tartanair/data_cacher/modality_type/ply_io.py`

 * *Files identical despite different names*

### Comparing `tartanair-1.0.2/tartanair/data_cacher/modality_type/tartanair_types.py` & `tartanair-1.0.3/tartanair/data_cacher/modality_type/tartanair_types.py`

 * *Files identical despite different names*

### Comparing `tartanair-1.0.2/tartanair/data_cacher/modality_type/tartanairv1_types.py` & `tartanair-1.0.3/tartanair/data_cacher/modality_type/tartanairv1_types.py`

 * *Files identical despite different names*

### Comparing `tartanair-1.0.2/tartanair/data_cacher/modality_type/tartandrive_types.py` & `tartanair-1.0.3/tartanair/data_cacher/modality_type/tartandrive_types.py`

 * *Files identical despite different names*

### Comparing `tartanair-1.0.2/tartanair/data_cacher/modality_type/test_register.py` & `tartanair-1.0.3/tartanair/data_cacher/modality_type/test_register.py`

 * *Files identical despite different names*

### Comparing `tartanair-1.0.2/tartanair/eval_utils/trajectory_evaluator_ate.py` & `tartanair-1.0.3/tartanair/eval_utils/trajectory_evaluator_ate.py`

 * *Files identical despite different names*

### Comparing `tartanair-1.0.2/tartanair/eval_utils/trajectory_evaluator_base.py` & `tartanair-1.0.3/tartanair/eval_utils/trajectory_evaluator_base.py`

 * *Files identical despite different names*

### Comparing `tartanair-1.0.2/tartanair/eval_utils/trajectory_evaluator_rpe.py` & `tartanair-1.0.3/tartanair/eval_utils/trajectory_evaluator_rpe.py`

 * *Files identical despite different names*

### Comparing `tartanair-1.0.2/tartanair/image_resampling/image_sampler/LICENSE` & `tartanair-1.0.3/tartanair/image_resampling/image_sampler/LICENSE`

 * *Files identical despite different names*

### Comparing `tartanair-1.0.2/tartanair/image_resampling/image_sampler/__init__.py` & `tartanair-1.0.3/tartanair/image_resampling/image_sampler/__init__.py`

 * *Files identical despite different names*

### Comparing `tartanair-1.0.2/tartanair/image_resampling/image_sampler/blend_function.py` & `tartanair-1.0.3/tartanair/image_resampling/image_sampler/blend_function.py`

 * *Files identical despite different names*

### Comparing `tartanair-1.0.2/tartanair/image_resampling/image_sampler/camera_model_sampler.py` & `tartanair-1.0.3/tartanair/image_resampling/image_sampler/camera_model_sampler.py`

 * *Files identical despite different names*

### Comparing `tartanair-1.0.2/tartanair/image_resampling/image_sampler/full_view_rotation.py` & `tartanair-1.0.3/tartanair/image_resampling/image_sampler/full_view_rotation.py`

 * *Files identical despite different names*

### Comparing `tartanair-1.0.2/tartanair/image_resampling/image_sampler/generic_camera_model_sampler.py` & `tartanair-1.0.3/tartanair/image_resampling/image_sampler/generic_camera_model_sampler.py`

 * *Files identical despite different names*

### Comparing `tartanair-1.0.2/tartanair/image_resampling/image_sampler/numba_support_check.py` & `tartanair-1.0.3/tartanair/image_resampling/image_sampler/numba_support_check.py`

 * *Files identical despite different names*

### Comparing `tartanair-1.0.2/tartanair/image_resampling/image_sampler/ocv_torch.py` & `tartanair-1.0.3/tartanair/image_resampling/image_sampler/ocv_torch.py`

 * *Files identical despite different names*

### Comparing `tartanair-1.0.2/tartanair/image_resampling/image_sampler/planar_as_base.py` & `tartanair-1.0.3/tartanair/image_resampling/image_sampler/planar_as_base.py`

 * *Files identical despite different names*

### Comparing `tartanair-1.0.2/tartanair/image_resampling/image_sampler/register.py` & `tartanair-1.0.3/tartanair/image_resampling/image_sampler/register.py`

 * *Files identical despite different names*

### Comparing `tartanair-1.0.2/tartanair/image_resampling/image_sampler/six_images.py` & `tartanair-1.0.3/tartanair/image_resampling/image_sampler/six_images.py`

 * *Files identical despite different names*

### Comparing `tartanair-1.0.2/tartanair/image_resampling/image_sampler/six_images_common.py` & `tartanair-1.0.3/tartanair/image_resampling/image_sampler/six_images_common.py`

 * *Files identical despite different names*

### Comparing `tartanair-1.0.2/tartanair/image_resampling/image_sampler/six_images_cupy.cu` & `tartanair-1.0.3/tartanair/image_resampling/image_sampler/six_images_cupy.cu`

 * *Files identical despite different names*

### Comparing `tartanair-1.0.2/tartanair/image_resampling/image_sampler/six_images_numba.py` & `tartanair-1.0.3/tartanair/image_resampling/image_sampler/six_images_numba.py`

 * *Files identical despite different names*

### Comparing `tartanair-1.0.2/tartanair/image_resampling/image_sampler/six_images_py_numba.py` & `tartanair-1.0.3/tartanair/image_resampling/image_sampler/six_images_py_numba.py`

 * *Files identical despite different names*

### Comparing `tartanair-1.0.2/tartanair/image_resampling/image_sampler/examples/README.md` & `tartanair-1.0.3/tartanair/image_resampling/image_sampler/examples/README.md`

 * *Files identical despite different names*

### Comparing `tartanair-1.0.2/tartanair/image_resampling/image_sampler/examples/generic_sampler_optical_flow_sampling_example.py` & `tartanair-1.0.3/tartanair/image_resampling/image_sampler/examples/generic_sampler_optical_flow_sampling_example.py`

 * *Files identical despite different names*

### Comparing `tartanair-1.0.2/tartanair/image_resampling/image_sampler/examples/data/flow_img.pt` & `tartanair-1.0.3/tartanair/image_resampling/image_sampler/examples/data/flow_img.pt`

 * *Files identical despite different names*

### Comparing `tartanair-1.0.2/tartanair/image_resampling/image_sampler/examples/examples_utils/visualization_utils.py` & `tartanair-1.0.3/tartanair/image_resampling/image_sampler/examples/examples_utils/visualization_utils.py`

 * *Files identical despite different names*

### Comparing `tartanair-1.0.2/tartanair/image_resampling/mvs_utils/LICENSE` & `tartanair-1.0.3/tartanair/image_resampling/mvs_utils/LICENSE`

 * *Files identical despite different names*

### Comparing `tartanair-1.0.2/tartanair/image_resampling/mvs_utils/camera_models.py` & `tartanair-1.0.3/tartanair/image_resampling/mvs_utils/camera_models.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,26 +1,32 @@
 
 import copy
 import torch
 import torch.nn.functional as F
 import math
 import sys
+import matplotlib.pyplot as plt
 
 from .debug import ( show_msg, show_obj, show_sum )
 
 from .ftensor import ( FTensor, f_eye )
 from .shape_struct import ShapeStruct
 
 from .compatible_torch import torch_meshgrid
 
 CAMERA_MODELS = dict()
 LIDAR_MODELS = dict()
 
 LOCAL_PI = math.pi
 
+from scipy.sparse import csc_matrix
+from scipy.sparse.linalg import inv
+pinholeradtan_solver = 'torch'
+
+
 def deg2rad(deg):
     global LOCAL_PI
     return deg / 180.0 * LOCAL_PI
 
 def register(dst):
     '''Register a class to a destination dictionary. '''
     def dec_register(cls):
@@ -1019,14 +1025,621 @@
         device: {self._device}'''
 
     def __str__(self) -> str:
         return f'''Pinhole
         Shape : {self.ss.shape}
         FoV degrees (lon/lat, y/x, h/w): {self.fov_degree_longitude}, {self.fov_degree_latitude}'''
 
+
+@register(CAMERA_MODELS)
+class PinholeRadTan(CameraModel):
+    def __init__(self, fx, fy, cx, cy, k1, k2, p1, p2, shape_struct, in_to_tensor=False, out_to_numpy=False,device='cpu'):
+        
+        # Compute the FoV from the specified parameters.
+        im_h, im_w = shape_struct.shape 
+        fov_degree = 2 * math.atan2(im_w, 2 * fx) * 180.0 / LOCAL_PI
+        
+        super().__init__('PinholeRadTan', fx, fy, cx, cy, fov_degree, shape_struct, in_to_tensor=in_to_tensor, out_to_numpy=out_to_numpy)
+
+        self.k1 = k1
+        self.k2 = k2 
+        self.p1 = p1
+        self.p2 = p2
+
+        # FoV for both longitude (x and width) and latitude (y and height).
+        self.fov_degree_longitude = 2 * math.atan2(im_w, 2 * fx) * 180.0 / LOCAL_PI
+        self.fov_degree_latitude  = 2 * math.atan2(im_h, 2 * fy) * 180.0 / LOCAL_PI
+        print(f"Created a new fisheye camera model with lon/lat FoV of {self.fov_degree_longitude, self.fov_degree_latitude} degrees.")
+
+        if isinstance( shape_struct, dict ):
+            self.ss = ShapeStruct( **shape_struct )
+        elif isinstance( shape_struct, ShapeStruct ):
+            self.ss = shape_struct
+        else:
+            raise Exception(f'shape_struct must be a dict or ShapeStruct object. Get {type(shape_struct)}')
+        
+        # The (inverse) intrinsics matrix is fixed throughout, keep a copy here.
+        self.intrinsics = torch.tensor([[self.fx, 0      , self.cx ],
+                                   [ 0,      self.fy, self.cy ],
+                                   [ 0,      0      ,      1.0]]).to(dtype=torch.float32, device=self._device)
+
+        self.inv_intrinsics = torch.tensor([[1.0/self.fx, 0      , -self.cx / self.fx],
+                                            [ 0,      1.0/self.fy, -self.cy / self.fy],
+                                            [ 0,      0      ,                1.0]]).to(dtype=torch.float32, device=self._device)
+
+    @SensorModel.device.setter
+    def device(self, d):
+        SensorModel.device.fset(self, d)
+        self.inv_intrinsics.to(device=d)
+        self.intrinsics.to(device=d)
+    
+
+    def distort(self,y_input,jacobian=True):
+        
+        y = y_input.clone()
+        y = self.in_wrap(y).to(dtype=torch.float32)
+
+        mx2_u = y[0] * y[0]
+        my2_u = y[1] * y[1]
+        mxy_u = y[0] * y[1]
+        rho2_u = mx2_u + my2_u
+
+        rad_dist_u = self.k1 * rho2_u + self.k2 * rho2_u * rho2_u
+        if len(y.shape) > 1:
+            n_points = y.shape[1]
+        else:
+            n_points = 1 
+
+        J = torch.zeros((2,2,n_points)).to(dtype=torch.float32, device=self._device)
+
+        if jacobian:
+            J[0,0] = 1 + rad_dist_u + self.k1 * 2.0 * mx2_u + self.k2 * rho2_u * 4 * mx2_u + 2.0 * self.p1 * y[1] + 6 * self.p2 * y[0]
+            J[1, 0] = self.k1 * 2.0 * y[0] * y[1] + self.k2 * 4 * rho2_u * y[0] * y[1]  + self.p1 * 2.0 * y[0] + 2.0 * self.p2 * y[1]
+            J[0, 1] = J[1, 0]
+            J[1, 1] = 1 + rad_dist_u + self.k1 * 2.0 * my2_u + self.k2 * rho2_u * 4 * my2_u + 6 * self.p1 * y[1] + 2.0 * self.p2 * y[0]
+
+        y[0] += y[0] * rad_dist_u + 2.0 * self.p1 * mxy_u + self.p2 * (rho2_u + 2.0 * mx2_u)
+        y[1] += y[1] * rad_dist_u + 2.0 * self.p2 * mxy_u + self.p1 * (rho2_u + 2.0 * my2_u)
+
+        return y, J
+
+
+    def undistort_single(self,y,homogeneous = False,debug=False):
+        n = 5
+        y_tmp = None
+        ybar = y.clone()
+
+        for i in range(n):
+            y_tmp = ybar.clone()
+            y_tmp, F = self.distort(y_tmp)
+            
+            F = torch.squeeze(F)
+            
+            e = y - y_tmp
+
+            du = torch.linalg.inv(F.T @ F) @ F.T @ e
+            ybar += du
+
+            if (e.dot(e) < 1e-15):
+                break
+        
+        if homogeneous:
+            ybar = torch.tensor([ybar[0],ybar[1],1.0]).to(dtype=torch.float32, device=self._device)
+
+        return ybar
+    
+    def undistort(self,y,homogeneous = False,debug=False):
+
+        n = 5
+        y_tmp = None
+        ybar = y.clone()
+
+        for i in range(n):
+            y_tmp = ybar.clone()
+            y_tmp, F = self.distort(y_tmp)
+
+            F = torch.swapaxes(F,-1,0)
+            F_block = torch.block_diag(*F).to(dtype=torch.float32, device=self._device)
+
+            # to scipy
+            if pinholeradtan_solver == 'scipy':
+                F_block = csc_matrix(F_block.cpu().numpy())
+
+            e = y - y_tmp
+            e_flat = torch.zeros((e.shape[1]*2,1)).to(dtype=torch.float32, device=self._device)
+            e_flat[::2] = e[0].reshape((-1,1))
+            e_flat[1 :: 2] = e[1].reshape((-1,1))
+
+            e = e_flat
+            if pinholeradtan_solver == 'scipy':
+                e = csc_matrix(e.cpu().numpy())
+
+            if pinholeradtan_solver == 'scipy':
+                du = inv(F_block.T @ F_block) @ F_block.T @ e
+                du = torch.tensor(du.toarray()).to(dtype=torch.float32, device=self._device)
+            else:
+                du = torch.linalg.inv(F_block.T @ F_block) @ F_block.T @ e
+            #
+            
+            ybar[0] += du[::2].flatten()
+            ybar[1] += du[1::2].flatten()
+
+            if debug:
+                print("Iteration {0}, loss: {1}".format(i,torch.linalg.norm(e)))
+                if (torch.linalg.norm(e) < 1e-15):
+                    break
+            
+        if homogeneous:
+            ybar = torch.cat((ybar,torch.ones_like(ybar[0]).reshape((1,-1))),dim=0)
+
+        return ybar
+
+
+    def normalize_point(self,y,homogeneous=False):
+        if homogeneous:
+            y_bar = torch.tensor([(y[0]-self.cx)/self.fx,(y[1]-self.cy)/self.fy,1.0]).to(dtype=torch.float32, device=self._device)
+        else:
+            y_bar = torch.tensor([(y[0]-self.cx)/self.fx,(y[1]-self.cy)/self.fy]).to(dtype=torch.float32, device=self._device)
+        return y_bar
+    
+    def normalize_points(self,y,homogeneous=False):
+        y_bar = torch.zeros_like(y).to(dtype=torch.float32, device=self._device)
+
+        y_bar[0] = (y[0]-self.cx)/self.fx
+        y_bar[1] = (y[1]-self.cy)/self.fy
+        y_bar = y_bar[:2]
+
+        # print(y_bar.shape)
+        if homogeneous:
+            y_bar = torch.cat((y_bar,torch.ones_like(y_bar[0]).reshape((1,-1))),dim=0)
+       
+        return y_bar
+    
+    def unnormalize_point(self,y,homogeneous=False):
+        y_bar = torch.zeros_like(y).to(dtype=torch.float32, device=self._device)
+        if homogeneous:
+            y_bar = torch.tensor([y[0]*self.fx+self.cx,y[1]*self.fy+self.cy,1.0]).to(dtype=torch.float32, device=self._device)
+        else:
+            y_bar = torch.tensor([y[0]*self.fx+self.cx,y[1]*self.fy+self.cy]).to(dtype=torch.float32, device=self._device)
+        return y_bar
+    
+    def unnormalize_points(self,y,homogeneous=False):
+        y_bar = torch.zeros_like(y).to(dtype=torch.float32, device=self._device)
+
+        y_bar[0] = y[0]*self.fx+self.cx
+        y_bar[1] = y[1]*self.fy+self.cy
+        y_bar = y_bar[:2]
+
+        # print(y_bar.shape)
+        if homogeneous:
+            y_bar = torch.cat((y_bar,torch.ones_like(y_bar[0]).reshape((1,-1))),dim=0)
+       
+        return y_bar
+
+    def pixel_2_ray(self, uv):
+        '''
+        Arguments:
+        uv (Tensor): A 2xN Tensor contains the pixel coordinates. 
+        
+        NOTE: pixel_coor can also have a dimension of Bx2xN, where B is the 
+        batch size.
+        
+        Returns:
+        A 3xN Tensor representing the 3D rays. Bx3xN if batched.
+        A (N,) Tensor representing the valid mask. BxN if batched.
+        '''
+
+        # Warp to desired datatype.
+        uv = self.in_wrap(uv).to(dtype=torch.float32)
+
+        # can we remove the for loop? Not sure, this is how Kalibr does it
+        N = uv.shape[1]
+        xyz = torch.zeros((3,N)).to(dtype=torch.float32, device=self._device)
+
+        batch_size = 1000
+
+        time_start = time.time()
+        print("Started calculations for pinhole-radtan.. Might take a couple minutes.")
+        for start_batch_idx in tqdm(torch.arange(0,N,batch_size)):
+            end_batch = min(start_batch_idx+batch_size,N)
+
+            xyz[:,start_batch_idx:end_batch] = self.undistort(self.normalize_points(uv[:,start_batch_idx:end_batch]),homogeneous=True,debug=False)
+
+        print("Elapsed time: {0}, for {1} images.".format(time.time()-time_start,N))
+        # xyz = torch.zeros((3,N)).to(dtype=torch.float32, device=self._device)
+        # for i in range(N):
+        #     debug = False
+        #     if i == 0:
+        #         debug = True
+
+        #     xyz[:,i] = self.undistort_single(self.normalize_point(uv[:,i]),homogeneous=True,debug=debug)
+        
+
+        # print("Single")
+        # print(xyz[:,:4])
+
+
+        # Convert to honmogeneous coordinates.
+        # uv1 = F.pad(uv, (0, 0, 0, 1), value=1)
+
+        # Convert to camera-frame (metric).
+
+        # xyz = self.inv_intrinsics @ uv1
+
+        # Normalize rays to be unit length.
+        xyz = xyz / torch.linalg.norm(xyz, dim = -2, keepdims= True)
+
+        # Mask points that are out of field of view.
+        # Currently returning a mask of only ones as all pixels are assumed to be with valid values, and the projection out of the image frame of all pixels is valid.
+        # The following if-statements match the dimensionality of batched inputs.
+        # NOTE(yoraish): why should there be any??
+        if len(uv.shape) == 2:
+            mask = torch.ones(uv.shape[1])
+        if len(uv.shape) == 3:
+            mask = torch.ones((uv.shape[0], uv.shape[2]))
+        
+        return self.out_wrap(xyz), \
+               self.out_wrap(mask)
+    
+    def point_3d_2_pixel(self, point_3d, normalized=False):
+        '''
+        Arguments:
+        point_3d (Tensor): A 3xN Tensor contains 3D point coordinates. 
+        normalized (bool): If True, then the returned coordinates are normalized to [-1, 1]
+        
+        NOTE: point_3d can also have a dimension of Bx3xN, where B is the 
+        batch number.
+        
+        Returns: 
+        A 2xN Tensor representing the 2D pixels. Bx2xN if batched.
+        A (N,) Tensor representing the valid mask. BxN if batched.
+        '''
+        point_3d = self.in_wrap(point_3d).to(dtype=torch.float32)
+
+
+        # can we remove the for loop? Not sure, this is how Kalibr does it
+        N = point_3d.shape[1]
+        # for i in range(N):
+        point_3d = torch.div(point_3d,point_3d[-1,:])
+        
+        point_3d = self.unnormalize_points(self.distort(point_3d,jacobian=False)[0],homogeneous=True)
+
+        # _, Js_parallel = self.distort(point_3d,jacobian=True)
+
+
+        # for i in range(N):
+        #     point_tmp, J = self.distort(torch.tensor([point_3d[0,i],point_3d[1,i]]),jacobian=True)
+        #     point_3d[:,i] = self.unnormalize_point(point_tmp,homogeneous=True)
+
+        # print(point_3d.shape)
+        uv = point_3d
+        # Pixel coordinates projected from the world points. 
+        # uv_unnormalized = self.intrinsics @ point_3d
+
+        # Normalize the homogenous coordinate-points such that their z-value is 1. The expression uv_unnormalized[..., -1:, :] keeps the dimension of the tensor, which is required by the division operation since PyTorch has trouble to broadcast the operation. 
+        # uv = torch.div(uv_unnormalized, uv_unnormalized[..., -1:, :])
+
+        # Warp to desired datatype.
+        uv = self.in_wrap(uv).to(dtype=torch.float32)
+
+        # Do torch.split results in Bx1XN.
+        px, py, _ = torch.split( uv, 1, dim=-2 )
+
+        if normalized:
+            # Using shape - 1 is the way for cv2.remap() and align_corners=True of torch.nn.functional.grid_sample().
+            # px = px / ( self.ss.W - 1 ) * 2 - 1
+            # py = py / ( self.ss.H - 1 ) * 2 - 1
+            # Using shape is the way for torch.nn.functional.grid_sample() with align_corners=False.
+            px = px / self.ss.W * 2 - 1
+            py = py / self.ss.H * 2 - 1
+
+        # pixel_coor = torch.stack( (px, py), dim=0 )
+        pixel_coor = torch.cat( (px, py), dim=-2 )
+
+        # Filter the invalid pixels by the image size. Valid mask takes on shape [B] x N
+        valid_mask_px = torch.logical_and(px < self.ss.W, px > 0)
+        valid_mask_py = torch.logical_and(py < self.ss.H, py > 0)
+        valid_mask = torch.logical_and(valid_mask_py, valid_mask_px)
+
+        # This is for the batched dimension.
+        valid_mask = valid_mask.squeeze(-2)
+
+        return self.out_wrap(pixel_coor), self.out_wrap(valid_mask)
+        
+    
+    def __repr__(self) -> str:
+        return f'''An instance of Pinhole CameraModel
+        Height : {self.ss.shape[0]}
+        Width : {self.ss.shape[1]}
+        fx : {self.fx}
+        fy : {self.fy}
+        cx : {self.cx}
+        cy : {self.cy}
+        FoV degrees (lon/lat, y/x, h/w): {self.fov_degree_longitude}, {self.fov_degree_latitude}
+        device: {self._device}'''
+
+    def __str__(self) -> str:
+        return f'''Pinhole
+        Shape : {self.ss.shape}
+        FoV degrees (lon/lat, y/x, h/w): {self.fov_degree_longitude}, {self.fov_degree_latitude}'''
+
+
+class UndistortNet(torch.nn.Module):
+    """Custom Pytorch model for gradient optimization of .
+    """
+    def __init__(self,init_weights,distort_func):
+        
+        super().__init__()
+        # initialize weights with random numbers
+        # weights = torch.distributions.Uniform(0, 0.1).sample((3,))
+        # make weights torch parameters
+        self.weights = torch.nn.Parameter(init_weights)
+        self.distort_func = distort_func
+        
+    def forward(self):
+        """Implement function to be optimised. In this case, an exponential decay
+        function (a + exp(-k * X) + b),
+        """
+        return self.distort_func(self.weights)
+    
+def training_loop(model, optimizer, GT, n=1000):
+    "Training loop for torch model."
+    losses = []
+    for i in range(n):
+        preds = model()
+        loss = F.mse_loss(preds, GT).sqrt()
+        loss.backward()
+        optimizer.step()
+        optimizer.zero_grad()
+        losses.append(loss)  
+    return losses
+
+
+@register(CAMERA_MODELS)
+class PinholeRadTanFast(CameraModel):
+    def __init__(self, fx, fy, cx, cy, k1, k2, p1, p2, shape_struct, in_to_tensor=False, out_to_numpy=False, device='cpu'):
+        
+        # Compute the FoV from the specified parameters.
+        im_h, im_w = shape_struct.shape 
+        fov_degree = 2 * math.atan2(im_w, 2 * fx) * 180.0 / LOCAL_PI
+        
+        super().__init__('PinholeRadTan', fx, fy, cx, cy, fov_degree, shape_struct, in_to_tensor=in_to_tensor, out_to_numpy=out_to_numpy)
+
+        self.k1 = k1
+        self.k2 = k2 
+        self.p1 = p1
+        self.p2 = p2
+
+        # FoV for both longitude (x and width) and latitude (y and height).
+        self.fov_degree_longitude = 2 * math.atan2(im_w, 2 * fx) * 180.0 / LOCAL_PI
+        self.fov_degree_latitude  = 2 * math.atan2(im_h, 2 * fy) * 180.0 / LOCAL_PI
+        print(f"Created a new fisheye camera model with lon/lat FoV of {self.fov_degree_longitude, self.fov_degree_latitude} degrees.")
+
+        if isinstance( shape_struct, dict ):
+            self.ss = ShapeStruct( **shape_struct )
+        elif isinstance( shape_struct, ShapeStruct ):
+            self.ss = shape_struct
+        else:
+            raise Exception(f'shape_struct must be a dict or ShapeStruct object. Get {type(shape_struct)}')
+        
+        # The (inverse) intrinsics matrix is fixed throughout, keep a copy here.
+        self.intrinsics = torch.tensor([[self.fx, 0      , self.cx ],
+                                   [ 0,      self.fy, self.cy ],
+                                   [ 0,      0      ,      1.0]]).to(dtype=torch.float32, device=self._device)
+
+        self.inv_intrinsics = torch.tensor([[1.0/self.fx, 0      , -self.cx / self.fx],
+                                            [ 0,      1.0/self.fy, -self.cy / self.fy],
+                                            [ 0,      0      ,                1.0]]).to(dtype=torch.float32, device=self._device)
+
+    @SensorModel.device.setter
+    def device(self, d):
+        SensorModel.device.fset(self, d)
+        self.inv_intrinsics.to(device=d)
+        self.intrinsics.to(device=d)
+    
+
+    def distort(self,y_input):
+        
+        y = y_input.clone()
+        y = self.in_wrap(y).to(dtype=torch.float32)
+
+        mx2_u = y[0] * y[0]
+        my2_u = y[1] * y[1]
+        mxy_u = y[0] * y[1]
+        rho2_u = mx2_u + my2_u
+
+        rad_dist_u = self.k1 * rho2_u + self.k2 * rho2_u * rho2_u
+
+        y_output = y.clone()
+        y_output[0] = y[0] +  y[0] * rad_dist_u + 2.0 * self.p1 * mxy_u + self.p2 * (rho2_u + 2.0 * mx2_u)
+        y_output[1] = y[1] +  y[1] * rad_dist_u + 2.0 * self.p2 * mxy_u + self.p1 * (rho2_u + 2.0 * my2_u)
+
+        return y_output
+
+    
+    def undistort(self,y,homogeneous = False,debug=False):
+
+        ybar = y.clone()
+
+        undistort_nn = UndistortNet(ybar,self.distort)
+        opt = torch.optim.Adam(undistort_nn.parameters(), lr=0.001)
+
+        loss = training_loop(undistort_nn,opt,y.clone())
+        loss = [tensor.detach().cpu().numpy() for tensor in loss]
+
+        ybar = undistort_nn.weights.detach().clone()
+
+        if debug:
+            plt.plot(loss)
+            plt.xlabel('Episode')
+            plt.ylabel('Loss')
+            plt.savefig('pinhole-radtan-opt.png')
+
+        if homogeneous:
+            ybar = torch.cat((ybar,torch.ones_like(ybar[0]).reshape((1,-1))),dim=0)
+
+        return ybar
+
+
+    def normalize_point(self,y,homogeneous=False):
+        if homogeneous:
+            y_bar = torch.tensor([(y[0]-self.cx)/self.fx,(y[1]-self.cy)/self.fy,1.0]).to(dtype=torch.float32, device=self._device)
+        else:
+            y_bar = torch.tensor([(y[0]-self.cx)/self.fx,(y[1]-self.cy)/self.fy]).to(dtype=torch.float32, device=self._device)
+        return y_bar
+    
+    def normalize_points(self,y,homogeneous=False):
+        y_bar = torch.zeros_like(y).to(dtype=torch.float32, device=self._device)
+
+        y_bar[0] = (y[0]-self.cx)/self.fx
+        y_bar[1] = (y[1]-self.cy)/self.fy
+        y_bar = y_bar[:2]
+
+        # print(y_bar.shape)
+        if homogeneous:
+            y_bar = torch.cat((y_bar,torch.ones_like(y_bar[0]).reshape((1,-1))),dim=0)
+       
+        return y_bar
+    
+    def unnormalize_point(self,y,homogeneous=False):
+        y_bar = torch.zeros_like(y).to(dtype=torch.float32, device=self._device)
+        if homogeneous:
+            y_bar = torch.tensor([y[0]*self.fx+self.cx,y[1]*self.fy+self.cy,1.0]).to(dtype=torch.float32, device=self._device)
+        else:
+            y_bar = torch.tensor([y[0]*self.fx+self.cx,y[1]*self.fy+self.cy]).to(dtype=torch.float32, device=self._device)
+        return y_bar
+    
+    def unnormalize_points(self,y,homogeneous=False):
+        y_bar = torch.zeros_like(y).to(dtype=torch.float32, device=self._device)
+
+        y_bar[0] = y[0]*self.fx+self.cx
+        y_bar[1] = y[1]*self.fy+self.cy
+        y_bar = y_bar[:2]
+
+        # print(y_bar.shape)
+        if homogeneous:
+            y_bar = torch.cat((y_bar,torch.ones_like(y_bar[0]).reshape((1,-1))),dim=0)
+       
+        return y_bar
+
+    def pixel_2_ray(self, uv):
+        '''
+        Arguments:
+        uv (Tensor): A 2xN Tensor contains the pixel coordinates. 
+        
+        NOTE: pixel_coor can also have a dimension of Bx2xN, where B is the 
+        batch size.
+        
+        Returns:
+        A 3xN Tensor representing the 3D rays. Bx3xN if batched.
+        A (N,) Tensor representing the valid mask. BxN if batched.
+        '''
+
+        # Warp to desired datatype.
+        uv = self.in_wrap(uv).to(dtype=torch.float32)
+
+        # can we remove the for loop? Not sure, this is how Kalibr does it
+        N = uv.shape[1]
+        # xyz = torch.zeros((3,N)).to(dtype=torch.float32, device=self._device)
+
+        xyz_grad = self.undistort(self.normalize_points(uv),homogeneous=True,debug=True)
+        xyz = xyz_grad.detach()
+
+        # NOTE(yoraish): why should there be any??
+        if len(uv.shape) == 2:
+            mask = torch.ones(uv.shape[1])
+        if len(uv.shape) == 3:
+            mask = torch.ones((uv.shape[0], uv.shape[2]))
+        
+        return self.out_wrap(xyz), \
+               self.out_wrap(mask)
+    
+    def point_3d_2_pixel(self, point_3d, normalized=False):
+        '''
+        Arguments:
+        point_3d (Tensor): A 3xN Tensor contains 3D point coordinates. 
+        normalized (bool): If True, then the returned coordinates are normalized to [-1, 1]
+        
+        NOTE: point_3d can also have a dimension of Bx3xN, where B is the 
+        batch number.
+        
+        Returns: 
+        A 2xN Tensor representing the 2D pixels. Bx2xN if batched.
+        A (N,) Tensor representing the valid mask. BxN if batched.
+        '''
+        point_3d = self.in_wrap(point_3d).to(dtype=torch.float32)
+
+
+        # can we remove the for loop? Not sure, this is how Kalibr does it
+        N = point_3d.shape[1]
+        # for i in range(N):
+        point_3d = torch.div(point_3d,point_3d[-1,:])
+        
+        point_3d = self.unnormalize_points(self.distort(point_3d),homogeneous=True)
+
+        # _, Js_parallel = self.distort(point_3d,jacobian=True)
+
+
+        # for i in range(N):
+        #     point_tmp, J = self.distort(torch.tensor([point_3d[0,i],point_3d[1,i]]),jacobian=True)
+        #     point_3d[:,i] = self.unnormalize_point(point_tmp,homogeneous=True)
+
+        # print(point_3d.shape)
+        uv = point_3d
+        # Pixel coordinates projected from the world points. 
+        # uv_unnormalized = self.intrinsics @ point_3d
+
+        # Normalize the homogenous coordinate-points such that their z-value is 1. The expression uv_unnormalized[..., -1:, :] keeps the dimension of the tensor, which is required by the division operation since PyTorch has trouble to broadcast the operation. 
+        # uv = torch.div(uv_unnormalized, uv_unnormalized[..., -1:, :])
+
+        # Warp to desired datatype.
+        uv = self.in_wrap(uv).to(dtype=torch.float32)
+
+        # Do torch.split results in Bx1XN.
+        px, py, _ = torch.split( uv, 1, dim=-2 )
+
+        if normalized:
+            # Using shape - 1 is the way for cv2.remap() and align_corners=True of torch.nn.functional.grid_sample().
+            # px = px / ( self.ss.W - 1 ) * 2 - 1
+            # py = py / ( self.ss.H - 1 ) * 2 - 1
+            # Using shape is the way for torch.nn.functional.grid_sample() with align_corners=False.
+            px = px / self.ss.W * 2 - 1
+            py = py / self.ss.H * 2 - 1
+
+        # pixel_coor = torch.stack( (px, py), dim=0 )
+        pixel_coor = torch.cat( (px, py), dim=-2 )
+
+        # Filter the invalid pixels by the image size. Valid mask takes on shape [B] x N
+        valid_mask_px = torch.logical_and(px < self.ss.W, px > 0)
+        valid_mask_py = torch.logical_and(py < self.ss.H, py > 0)
+        valid_mask = torch.logical_and(valid_mask_py, valid_mask_px)
+
+        # This is for the batched dimension.
+        valid_mask = valid_mask.squeeze(-2)
+
+        return self.out_wrap(pixel_coor), self.out_wrap(valid_mask)
+        
+    
+    def __repr__(self) -> str:
+        return f'''An instance of Pinhole CameraModel
+        Height : {self.ss.shape[0]}
+        Width : {self.ss.shape[1]}
+        fx : {self.fx}
+        fy : {self.fy}
+        cx : {self.cx}
+        cy : {self.cy}
+        FoV degrees (lon/lat, y/x, h/w): {self.fov_degree_longitude}, {self.fov_degree_latitude}
+        device: {self._device}'''
+
+    def __str__(self) -> str:
+        return f'''Pinhole
+        Shape : {self.ss.shape}
+        FoV degrees (lon/lat, y/x, h/w): {self.fov_degree_longitude}, {self.fov_degree_latitude}'''
+
+
 class LiDAR(SensorModel):
     def __init__(self, name, shape_struct, in_to_tensor=False, out_to_numpy=False):
         super().__init__(
             name=name,
             shape_struct=shape_struct, 
             in_to_tensor=in_to_tensor, 
             out_to_numpy=out_to_numpy )
```

### Comparing `tartanair-1.0.2/tartanair/image_resampling/mvs_utils/compatible_torch.py` & `tartanair-1.0.3/tartanair/image_resampling/mvs_utils/compatible_torch.py`

 * *Files identical despite different names*

### Comparing `tartanair-1.0.2/tartanair/image_resampling/mvs_utils/debug.py` & `tartanair-1.0.3/tartanair/image_resampling/mvs_utils/debug.py`

 * *Files identical despite different names*

### Comparing `tartanair-1.0.2/tartanair/image_resampling/mvs_utils/frame_io.py` & `tartanair-1.0.3/tartanair/image_resampling/mvs_utils/frame_io.py`

 * *Files identical despite different names*

### Comparing `tartanair-1.0.2/tartanair/image_resampling/mvs_utils/kalibr_parser.py` & `tartanair-1.0.3/tartanair/image_resampling/mvs_utils/kalibr_parser.py`

 * *Files identical despite different names*

### Comparing `tartanair-1.0.2/tartanair/image_resampling/mvs_utils/metadata_reader.py` & `tartanair-1.0.3/tartanair/image_resampling/mvs_utils/metadata_reader.py`

 * *Files identical despite different names*

### Comparing `tartanair-1.0.2/tartanair/image_resampling/mvs_utils/point_cloud_helper.py` & `tartanair-1.0.3/tartanair/image_resampling/mvs_utils/point_cloud_helper.py`

 * *Files identical despite different names*

### Comparing `tartanair-1.0.2/tartanair/image_resampling/mvs_utils/pose.py` & `tartanair-1.0.3/tartanair/image_resampling/mvs_utils/pose.py`

 * *Files identical despite different names*

### Comparing `tartanair-1.0.2/tartanair/image_resampling/mvs_utils/pretty_dict.py` & `tartanair-1.0.3/tartanair/image_resampling/mvs_utils/pretty_dict.py`

 * *Files identical despite different names*

### Comparing `tartanair-1.0.2/tartanair/image_resampling/mvs_utils/shape_struct.py` & `tartanair-1.0.3/tartanair/image_resampling/mvs_utils/shape_struct.py`

 * *Files identical despite different names*

### Comparing `tartanair-1.0.2/tartanair/image_resampling/mvs_utils/simulated_lidar_pre_def_models.py` & `tartanair-1.0.3/tartanair/image_resampling/mvs_utils/simulated_lidar_pre_def_models.py`

 * *Files identical despite different names*

### Comparing `tartanair-1.0.2/tartanair/image_resampling/mvs_utils/test_frame_io.py` & `tartanair-1.0.3/tartanair/image_resampling/mvs_utils/test_frame_io.py`

 * *Files identical despite different names*

### Comparing `tartanair-1.0.2/tartanair/image_resampling/mvs_utils/test_inheritance.py` & `tartanair-1.0.3/tartanair/image_resampling/mvs_utils/test_inheritance.py`

 * *Files identical despite different names*

### Comparing `tartanair-1.0.2/tartanair/image_resampling/mvs_utils/examples/README.md` & `tartanair-1.0.3/tartanair/image_resampling/mvs_utils/examples/README.md`

 * *Files identical despite different names*

### Comparing `tartanair-1.0.2/tartanair/image_resampling/mvs_utils/examples/linear_fisheye_camera_model.py` & `tartanair-1.0.3/tartanair/image_resampling/mvs_utils/examples/linear_fisheye_camera_model.py`

 * *Files identical despite different names*

### Comparing `tartanair-1.0.2/tartanair/image_resampling/mvs_utils/ftensor/LICENSE` & `tartanair-1.0.3/tartanair/image_resampling/mvs_utils/ftensor/LICENSE`

 * *Files identical despite different names*

### Comparing `tartanair-1.0.2/tartanair/image_resampling/mvs_utils/ftensor/README.md` & `tartanair-1.0.3/tartanair/image_resampling/mvs_utils/ftensor/README.md`

 * *Files identical despite different names*

### Comparing `tartanair-1.0.2/tartanair/image_resampling/mvs_utils/ftensor/_pytree.py` & `tartanair-1.0.3/tartanair/image_resampling/mvs_utils/ftensor/_pytree.py`

 * *Files identical despite different names*

### Comparing `tartanair-1.0.2/tartanair/image_resampling/mvs_utils/ftensor/frame_graph.py` & `tartanair-1.0.3/tartanair/image_resampling/mvs_utils/ftensor/frame_graph.py`

 * *Files identical despite different names*

### Comparing `tartanair-1.0.2/tartanair/image_resampling/mvs_utils/ftensor/ftensor.py` & `tartanair-1.0.3/tartanair/image_resampling/mvs_utils/ftensor/ftensor.py`

 * *Files identical despite different names*

### Comparing `tartanair-1.0.2/tartanair/image_resampling/mvs_utils/ftensor/test_frame_graph.py` & `tartanair-1.0.3/tartanair/image_resampling/mvs_utils/ftensor/test_frame_graph.py`

 * *Files identical despite different names*

### Comparing `tartanair-1.0.2/tartanair/image_resampling/mvs_utils/ftensor/test_ftensor.py` & `tartanair-1.0.3/tartanair/image_resampling/mvs_utils/ftensor/test_ftensor.py`

 * *Files identical despite different names*

### Comparing `tartanair-1.0.2/tartanair/image_resampling/mvs_utils/image_io/float_type.py` & `tartanair-1.0.3/tartanair/image_resampling/mvs_utils/image_io/float_type.py`

 * *Files identical despite different names*

### Comparing `tartanair-1.0.2/tartanair/image_resampling/mvs_utils/image_io/image_read.py` & `tartanair-1.0.3/tartanair/image_resampling/mvs_utils/image_io/image_read.py`

 * *Files identical despite different names*

### Comparing `tartanair-1.0.2/tartanair/image_resampling/mvs_utils/image_io/image_write.py` & `tartanair-1.0.3/tartanair/image_resampling/mvs_utils/image_io/image_write.py`

 * *Files identical despite different names*

### Comparing `tartanair-1.0.2/tartanair/image_resampling/mvs_utils/test_data/frame_graph.json` & `tartanair-1.0.3/tartanair/image_resampling/mvs_utils/test_data/frame_graph.json`

 * *Files identical despite different names*

### Comparing `tartanair-1.0.2/tests/README.md` & `tartanair-1.0.3/tests/README.md`

 * *Files identical despite different names*

### Comparing `tartanair-1.0.2/tests/tartanairpy_test.py` & `tartanair-1.0.3/tests/tartanairpy_test.py`

 * *Files identical despite different names*

### Comparing `tartanair-1.0.2/tests/sample_tartanair_v2_data_root/ArchVizTinyHouseDayExposure/Data_hard/P000/image_lcam_custom0_doublesphere/camera_model_params_lcam_image_custom0_doublesphere.json` & `tartanair-1.0.3/tests/sample_tartanair_v2_data_root/ArchVizTinyHouseDayExposure/Data_hard/P000/image_lcam_custom0_doublesphere/camera_model_params_lcam_image_custom0_doublesphere.json`

 * *Files identical despite different names*

### Comparing `tartanair-1.0.2/.gitignore` & `tartanair-1.0.3/.gitignore`

 * *Files identical despite different names*

### Comparing `tartanair-1.0.2/LICENSE` & `tartanair-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `tartanair-1.0.2/pyproject.toml` & `tartanair-1.0.3/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "tartanair"
-version = "1.0.2"
+version = "1.0.3"
 authors = [
   { name="Yorai Shaoul", email="yorai@cmu.edu" },
   { name="Wenshan Wang", email="wenshanw@cs.cmu.edu " } 
 ]
 description = "TartanAir"
 readme = "README.md"
 requires-python = ">=3.7"
@@ -28,14 +28,13 @@
     "opencv_contrib_python",
     "Pillow",
     "plyfile",
     "pyquaternion",
     "pytransform3d",
     "PyYAML",
     "scipy",
-    "torchvision",
     "pyyaml",
     "pandas"
     ]
 
 [project.urls]
-"Homepage" = "http://theairlab.org/tartanair-dataset/"
+"Homepage" = "https://tartanair.org"
```

### Comparing `tartanair-1.0.2/PKG-INFO` & `tartanair-1.0.3/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: tartanair
-Version: 1.0.2
+Version: 1.0.3
 Summary: TartanAir
-Project-URL: Homepage, http://theairlab.org/tartanair-dataset/
+Project-URL: Homepage, https://tartanair.org
 Author-email: Yorai Shaoul <yorai@cmu.edu>, Wenshan Wang <wenshanw@cs.cmu.edu>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Requires-Dist: colorama>=0.4.0
@@ -19,13 +19,12 @@
 Requires-Dist: pandas
 Requires-Dist: pillow
 Requires-Dist: plyfile
 Requires-Dist: pyquaternion
 Requires-Dist: pytransform3d
 Requires-Dist: pyyaml
 Requires-Dist: scipy
-Requires-Dist: torchvision
 Description-Content-Type: text/markdown
 
 # TartanAir
 
 Hello and welcome to the official TartanAir repository. This repository includes a set of tools that complement the [TartanAir Dataset](https://www.tartanair.org/)).
```

