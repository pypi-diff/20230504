# Comparing `tmp/nerfstudio-0.2.1.tar.gz` & `tmp/nerfstudio-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nerfstudio-0.2.1.tar", last modified: Wed Apr 19 00:30:37 2023, max compression
+gzip compressed data, was "nerfstudio-0.2.2.tar", last modified: Thu May  4 21:45:43 2023, max compression
```

## Comparing `nerfstudio-0.2.1.tar` & `nerfstudio-0.2.2.tar`

### file list

```diff
@@ -1,237 +1,244 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 00:30:37.935915 nerfstudio-0.2.1/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-19 00:30:24.000000 nerfstudio-0.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    19021 2023-04-19 00:30:37.935915 nerfstudio-0.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    18600 2023-04-19 00:30:31.000000 nerfstudio-0.2.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 00:30:37.879915 nerfstudio-0.2.1/nerfstudio/
--rw-r--r--   0 runner    (1001) docker     (123)      605 2023-04-19 00:30:24.000000 nerfstudio-0.2.1/nerfstudio/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 00:30:37.883915 nerfstudio-0.2.1/nerfstudio/cameras/
--rw-r--r--   0 runner    (1001) docker     (123)      605 2023-04-19 00:30:24.000000 nerfstudio-0.2.1/nerfstudio/cameras/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4893 2023-04-19 00:30:24.000000 nerfstudio-0.2.1/nerfstudio/cameras/camera_optimizers.py
--rw-r--r--   0 runner    (1001) docker     (123)     5940 2023-04-19 00:30:24.000000 nerfstudio-0.2.1/nerfstudio/cameras/camera_paths.py
--rw-r--r--   0 runner    (1001) docker     (123)    21340 2023-04-19 00:30:24.000000 nerfstudio-0.2.1/nerfstudio/cameras/camera_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    41365 2023-04-19 00:30:24.000000 nerfstudio-0.2.1/nerfstudio/cameras/cameras.py
--rw-r--r--   0 runner    (1001) docker     (123)     4772 2023-04-19 00:30:24.000000 nerfstudio-0.2.1/nerfstudio/cameras/lie_groups.py
--rw-r--r--   0 runner    (1001) docker     (123)    10287 2023-04-19 00:30:24.000000 nerfstudio-0.2.1/nerfstudio/cameras/rays.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 00:30:37.883915 nerfstudio-0.2.1/nerfstudio/configs/
--rw-r--r--   0 runner    (1001) docker     (123)      605 2023-04-19 00:30:24.000000 nerfstudio-0.2.1/nerfstudio/configs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5521 2023-04-19 00:30:24.000000 nerfstudio-0.2.1/nerfstudio/configs/base_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1547 2023-04-19 00:30:24.000000 nerfstudio-0.2.1/nerfstudio/configs/config_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     5125 2023-04-19 00:30:24.000000 nerfstudio-0.2.1/nerfstudio/configs/experiment_config.py
--rw-r--r--   0 runner    (1001) docker     (123)    21798 2023-04-19 00:30:24.000000 nerfstudio-0.2.1/nerfstudio/configs/method_configs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 00:30:37.883915 nerfstudio-0.2.1/nerfstudio/data/
--rw-r--r--   0 runner    (1001) docker     (123)      605 2023-04-19 00:30:24.000000 nerfstudio-0.2.1/nerfstudio/data/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 00:30:37.887915 nerfstudio-0.2.1/nerfstudio/data/datamanagers/
--rw-r--r--   0 runner    (1001) docker     (123)      605 2023-04-19 00:30:24.000000 nerfstudio-0.2.1/nerfstudio/data/datamanagers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24424 2023-04-19 00:30:24.000000 nerfstudio-0.2.1/nerfstudio/data/datamanagers/base_datamanager.py
--rw-r--r--   0 runner    (1001) docker     (123)     1738 2023-04-19 00:30:24.000000 nerfstudio-0.2.1/nerfstudio/data/datamanagers/depth_datamanager.py
--rw-r--r--   0 runner    (1001) docker     (123)     1714 2023-04-19 00:30:24.000000 nerfstudio-0.2.1/nerfstudio/data/datamanagers/sdf_datamanager.py
--rw-r--r--   0 runner    (1001) docker     (123)     1923 2023-04-19 00:30:24.000000 nerfstudio-0.2.1/nerfstudio/data/datamanagers/semantic_datamanager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 00:30:37.891915 nerfstudio-0.2.1/nerfstudio/data/dataparsers/
--rw-r--r--   0 runner    (1001) docker     (123)      605 2023-04-19 00:30:24.000000 nerfstudio-0.2.1/nerfstudio/data/dataparsers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9094 2023-04-19 00:30:24.000000 nerfstudio-0.2.1/nerfstudio/data/dataparsers/arkitscenes_dataparser.py
--rw-r--r--   0 runner    (1001) docker     (123)     7230 2023-04-19 00:30:24.000000 nerfstudio-0.2.1/nerfstudio/data/dataparsers/base_dataparser.py
--rw-r--r--   0 runner    (1001) docker     (123)     3731 2023-04-19 00:30:24.000000 nerfstudio-0.2.1/nerfstudio/data/dataparsers/blender_dataparser.py
--rw-r--r--   0 runner    (1001) docker     (123)     3774 2023-04-19 00:30:24.000000 nerfstudio-0.2.1/nerfstudio/data/dataparsers/dnerf_dataparser.py
--rw-r--r--   0 runner    (1001) docker     (123)    13531 2023-04-19 00:30:24.000000 nerfstudio-0.2.1/nerfstudio/data/dataparsers/dycheck_dataparser.py
--rw-r--r--   0 runner    (1001) docker     (123)     6511 2023-04-19 00:30:24.000000 nerfstudio-0.2.1/nerfstudio/data/dataparsers/instant_ngp_dataparser.py
--rw-r--r--   0 runner    (1001) docker     (123)     4211 2023-04-19 00:30:24.000000 nerfstudio-0.2.1/nerfstudio/data/dataparsers/minimal_dataparser.py
--rw-r--r--   0 runner    (1001) docker     (123)     8553 2023-04-19 00:30:24.000000 nerfstudio-0.2.1/nerfstudio/data/dataparsers/nerfosr_dataparser.py
--rw-r--r--   0 runner    (1001) docker     (123)    14847 2023-04-19 00:30:24.000000 nerfstudio-0.2.1/nerfstudio/data/dataparsers/nerfstudio_dataparser.py
--rw-r--r--   0 runner    (1001) docker     (123)     8573 2023-04-19 00:30:24.000000 nerfstudio-0.2.1/nerfstudio/data/dataparsers/nuscenes_dataparser.py
--rw-r--r--   0 runner    (1001) docker     (123)     7016 2023-04-19 00:30:24.000000 nerfstudio-0.2.1/nerfstudio/data/dataparsers/phototourism_dataparser.py
--rw-r--r--   0 runner    (1001) docker     (123)     6755 2023-04-19 00:30:24.000000 nerfstudio-0.2.1/nerfstudio/data/dataparsers/scannet_dataparser.py
--rw-r--r--   0 runner    (1001) docker     (123)     5692 2023-04-19 00:30:24.000000 nerfstudio-0.2.1/nerfstudio/data/dataparsers/sdfstudio_dataparser.py
--rw-r--r--   0 runner    (1001) docker     (123)     6004 2023-04-19 00:30:24.000000 nerfstudio-0.2.1/nerfstudio/data/dataparsers/sitcoms3d_dataparser.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 00:30:37.891915 nerfstudio-0.2.1/nerfstudio/data/datasets/
--rw-r--r--   0 runner    (1001) docker     (123)      605 2023-04-19 00:30:24.000000 nerfstudio-0.2.1/nerfstudio/data/datasets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4996 2023-04-19 00:30:24.000000 nerfstudio-0.2.1/nerfstudio/data/datasets/base_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     2214 2023-04-19 00:30:24.000000 nerfstudio-0.2.1/nerfstudio/data/datasets/depth_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     3694 2023-04-19 00:30:24.000000 nerfstudio-0.2.1/nerfstudio/data/datasets/sdf_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     2035 2023-04-19 00:30:24.000000 nerfstudio-0.2.1/nerfstudio/data/datasets/semantic_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)    12763 2023-04-19 00:30:24.000000 nerfstudio-0.2.1/nerfstudio/data/pixel_samplers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2689 2023-04-19 00:30:24.000000 nerfstudio-0.2.1/nerfstudio/data/scene_box.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 00:30:37.895915 nerfstudio-0.2.1/nerfstudio/data/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      605 2023-04-19 00:30:24.000000 nerfstudio-0.2.1/nerfstudio/data/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20570 2023-04-19 00:30:24.000000 nerfstudio-0.2.1/nerfstudio/data/utils/colmap_parsing_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3408 2023-04-19 00:30:24.000000 nerfstudio-0.2.1/nerfstudio/data/utils/data_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     8937 2023-04-19 00:30:24.000000 nerfstudio-0.2.1/nerfstudio/data/utils/dataloaders.py
--rw-r--r--   0 runner    (1001) docker     (123)     9620 2023-04-19 00:30:24.000000 nerfstudio-0.2.1/nerfstudio/data/utils/nerfstudio_collate.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 00:30:37.895915 nerfstudio-0.2.1/nerfstudio/engine/
--rw-r--r--   0 runner    (1001) docker     (123)      605 2023-04-19 00:30:24.000000 nerfstudio-0.2.1/nerfstudio/engine/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3915 2023-04-19 00:30:24.000000 nerfstudio-0.2.1/nerfstudio/engine/callbacks.py
--rw-r--r--   0 runner    (1001) docker     (123)     5738 2023-04-19 00:30:24.000000 nerfstudio-0.2.1/nerfstudio/engine/optimizers.py
--rw-r--r--   0 runner    (1001) docker     (123)     6038 2023-04-19 00:30:24.000000 nerfstudio-0.2.1/nerfstudio/engine/schedulers.py
--rw-r--r--   0 runner    (1001) docker     (123)    20511 2023-04-19 00:30:24.000000 nerfstudio-0.2.1/nerfstudio/engine/trainer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 00:30:37.895915 nerfstudio-0.2.1/nerfstudio/exporter/
--rw-r--r--   0 runner    (1001) docker     (123)      605 2023-04-19 00:30:24.000000 nerfstudio-0.2.1/nerfstudio/exporter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12314 2023-04-19 00:30:24.000000 nerfstudio-0.2.1/nerfstudio/exporter/exporter_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    10345 2023-04-19 00:30:24.000000 nerfstudio-0.2.1/nerfstudio/exporter/marching_cubes.py
--rw-r--r--   0 runner    (1001) docker     (123)    21276 2023-04-19 00:30:24.000000 nerfstudio-0.2.1/nerfstudio/exporter/texture_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    13842 2023-04-19 00:30:24.000000 nerfstudio-0.2.1/nerfstudio/exporter/tsdf_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 00:30:37.899915 nerfstudio-0.2.1/nerfstudio/field_components/
--rw-r--r--   0 runner    (1001) docker     (123)      751 2023-04-19 00:30:24.000000 nerfstudio-0.2.1/nerfstudio/field_components/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1441 2023-04-19 00:30:24.000000 nerfstudio-0.2.1/nerfstudio/field_components/activations.py
--rw-r--r--   0 runner    (1001) docker     (123)     2090 2023-04-19 00:30:24.000000 nerfstudio-0.2.1/nerfstudio/field_components/base_field_component.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 00:30:37.899915 nerfstudio-0.2.1/nerfstudio/field_components/cuda/
--rw-r--r--   0 runner    (1001) docker     (123)     1125 2023-04-19 00:30:24.000000 nerfstudio-0.2.1/nerfstudio/field_components/cuda/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2185 2023-04-19 00:30:24.000000 nerfstudio-0.2.1/nerfstudio/field_components/cuda/_backend.py
--rw-r--r--   0 runner    (1001) docker     (123)     1657 2023-04-19 00:30:24.000000 nerfstudio-0.2.1/nerfstudio/field_components/embedding.py
--rw-r--r--   0 runner    (1001) docker     (123)    26684 2023-04-19 00:30:24.000000 nerfstudio-0.2.1/nerfstudio/field_components/encodings.py
--rw-r--r--   0 runner    (1001) docker     (123)     6880 2023-04-19 00:30:24.000000 nerfstudio-0.2.1/nerfstudio/field_components/field_heads.py
--rw-r--r--   0 runner    (1001) docker     (123)     3646 2023-04-19 00:30:24.000000 nerfstudio-0.2.1/nerfstudio/field_components/mlp.py
--rw-r--r--   0 runner    (1001) docker     (123)     3191 2023-04-19 00:30:24.000000 nerfstudio-0.2.1/nerfstudio/field_components/spatial_distortions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3339 2023-04-19 00:30:24.000000 nerfstudio-0.2.1/nerfstudio/field_components/temporal_distortions.py
--rw-r--r--   0 runner    (1001) docker     (123)    16288 2023-04-19 00:30:24.000000 nerfstudio-0.2.1/nerfstudio/field_components/temporal_grid.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 00:30:37.903915 nerfstudio-0.2.1/nerfstudio/fields/
--rw-r--r--   0 runner    (1001) docker     (123)      605 2023-04-19 00:30:24.000000 nerfstudio-0.2.1/nerfstudio/fields/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4935 2023-04-19 00:30:24.000000 nerfstudio-0.2.1/nerfstudio/fields/base_field.py
--rw-r--r--   0 runner    (1001) docker     (123)     4877 2023-04-19 00:30:24.000000 nerfstudio-0.2.1/nerfstudio/fields/density_fields.py
--rw-r--r--   0 runner    (1001) docker     (123)     8348 2023-04-19 00:30:24.000000 nerfstudio-0.2.1/nerfstudio/fields/instant_ngp_field.py
--rw-r--r--   0 runner    (1001) docker     (123)    17622 2023-04-19 00:30:24.000000 nerfstudio-0.2.1/nerfstudio/fields/nerfacto_field.py
--rw-r--r--   0 runner    (1001) docker     (123)    17504 2023-04-19 00:30:24.000000 nerfstudio-0.2.1/nerfstudio/fields/nerfplayer_nerfacto_field.py
--rw-r--r--   0 runner    (1001) docker     (123)    10726 2023-04-19 00:30:24.000000 nerfstudio-0.2.1/nerfstudio/fields/nerfplayer_ngp_field.py
--rw-r--r--   0 runner    (1001) docker     (123)     6864 2023-04-19 00:30:24.000000 nerfstudio-0.2.1/nerfstudio/fields/nerfw_field.py
--rw-r--r--   0 runner    (1001) docker     (123)    17598 2023-04-19 00:30:24.000000 nerfstudio-0.2.1/nerfstudio/fields/sdf_field.py
--rw-r--r--   0 runner    (1001) docker     (123)     4297 2023-04-19 00:30:24.000000 nerfstudio-0.2.1/nerfstudio/fields/semantic_nerf_field.py
--rw-r--r--   0 runner    (1001) docker     (123)     5865 2023-04-19 00:30:24.000000 nerfstudio-0.2.1/nerfstudio/fields/tensorf_field.py
--rw-r--r--   0 runner    (1001) docker     (123)     4666 2023-04-19 00:30:24.000000 nerfstudio-0.2.1/nerfstudio/fields/vanilla_nerf_field.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 00:30:37.903915 nerfstudio-0.2.1/nerfstudio/generative/
--rw-r--r--   0 runner    (1001) docker     (123)      605 2023-04-19 00:30:24.000000 nerfstudio-0.2.1/nerfstudio/generative/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13907 2023-04-19 00:30:24.000000 nerfstudio-0.2.1/nerfstudio/generative/stable_diffusion.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 00:30:37.907915 nerfstudio-0.2.1/nerfstudio/model_components/
--rw-r--r--   0 runner    (1001) docker     (123)      605 2023-04-19 00:30:24.000000 nerfstudio-0.2.1/nerfstudio/model_components/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18593 2023-04-19 00:30:24.000000 nerfstudio-0.2.1/nerfstudio/model_components/losses.py
--rw-r--r--   0 runner    (1001) docker     (123)     2159 2023-04-19 00:30:24.000000 nerfstudio-0.2.1/nerfstudio/model_components/ray_generators.py
--rw-r--r--   0 runner    (1001) docker     (123)    28619 2023-04-19 00:30:24.000000 nerfstudio-0.2.1/nerfstudio/model_components/ray_samplers.py
--rw-r--r--   0 runner    (1001) docker     (123)    12300 2023-04-19 00:30:24.000000 nerfstudio-0.2.1/nerfstudio/model_components/renderers.py
--rw-r--r--   0 runner    (1001) docker     (123)     6615 2023-04-19 00:30:24.000000 nerfstudio-0.2.1/nerfstudio/model_components/scene_colliders.py
--rw-r--r--   0 runner    (1001) docker     (123)     2478 2023-04-19 00:30:24.000000 nerfstudio-0.2.1/nerfstudio/model_components/shaders.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 00:30:37.911915 nerfstudio-0.2.1/nerfstudio/models/
--rw-r--r--   0 runner    (1001) docker     (123)      605 2023-04-19 00:30:24.000000 nerfstudio-0.2.1/nerfstudio/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8427 2023-04-19 00:30:24.000000 nerfstudio-0.2.1/nerfstudio/models/base_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    16122 2023-04-19 00:30:24.000000 nerfstudio-0.2.1/nerfstudio/models/base_surface_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     5511 2023-04-19 00:30:24.000000 nerfstudio-0.2.1/nerfstudio/models/depth_nerfacto.py
--rw-r--r--   0 runner    (1001) docker     (123)    10102 2023-04-19 00:30:24.000000 nerfstudio-0.2.1/nerfstudio/models/instant_ngp.py
--rw-r--r--   0 runner    (1001) docker     (123)     7763 2023-04-19 00:30:24.000000 nerfstudio-0.2.1/nerfstudio/models/mipnerf.py
--rw-r--r--   0 runner    (1001) docker     (123)    15990 2023-04-19 00:30:24.000000 nerfstudio-0.2.1/nerfstudio/models/nerfacto.py
--rw-r--r--   0 runner    (1001) docker     (123)    11345 2023-04-19 00:30:24.000000 nerfstudio-0.2.1/nerfstudio/models/nerfplayer_nerfacto.py
--rw-r--r--   0 runner    (1001) docker     (123)    11190 2023-04-19 00:30:24.000000 nerfstudio-0.2.1/nerfstudio/models/nerfplayer_ngp.py
--rw-r--r--   0 runner    (1001) docker     (123)     4103 2023-04-19 00:30:24.000000 nerfstudio-0.2.1/nerfstudio/models/neus.py
--rw-r--r--   0 runner    (1001) docker     (123)     9418 2023-04-19 00:30:24.000000 nerfstudio-0.2.1/nerfstudio/models/neus_facto.py
--rw-r--r--   0 runner    (1001) docker     (123)    13345 2023-04-19 00:30:24.000000 nerfstudio-0.2.1/nerfstudio/models/semantic_nerfw.py
--rw-r--r--   0 runner    (1001) docker     (123)    12781 2023-04-19 00:30:24.000000 nerfstudio-0.2.1/nerfstudio/models/tensorf.py
--rw-r--r--   0 runner    (1001) docker     (123)     9815 2023-04-19 00:30:24.000000 nerfstudio-0.2.1/nerfstudio/models/vanilla_nerf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 00:30:37.911915 nerfstudio-0.2.1/nerfstudio/pipelines/
--rw-r--r--   0 runner    (1001) docker     (123)      605 2023-04-19 00:30:24.000000 nerfstudio-0.2.1/nerfstudio/pipelines/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16520 2023-04-19 00:30:24.000000 nerfstudio-0.2.1/nerfstudio/pipelines/base_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (123)     4346 2023-04-19 00:30:24.000000 nerfstudio-0.2.1/nerfstudio/pipelines/dynamic_batch.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 00:30:37.911915 nerfstudio-0.2.1/nerfstudio/plugins/
--rw-r--r--   0 runner    (1001) docker     (123)      605 2023-04-19 00:30:24.000000 nerfstudio-0.2.1/nerfstudio/plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1933 2023-04-19 00:30:24.000000 nerfstudio-0.2.1/nerfstudio/plugins/registry.py
--rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-04-19 00:30:24.000000 nerfstudio-0.2.1/nerfstudio/plugins/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 00:30:37.915915 nerfstudio-0.2.1/nerfstudio/process_data/
--rw-r--r--   0 runner    (1001) docker     (123)      605 2023-04-19 00:30:24.000000 nerfstudio-0.2.1/nerfstudio/process_data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24631 2023-04-19 00:30:24.000000 nerfstudio-0.2.1/nerfstudio/process_data/colmap_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     8215 2023-04-19 00:30:24.000000 nerfstudio-0.2.1/nerfstudio/process_data/equirect_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     5179 2023-04-19 00:30:24.000000 nerfstudio-0.2.1/nerfstudio/process_data/hloc_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     6881 2023-04-19 00:30:24.000000 nerfstudio-0.2.1/nerfstudio/process_data/metashape_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     9185 2023-04-19 00:30:24.000000 nerfstudio-0.2.1/nerfstudio/process_data/polycam_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    19948 2023-04-19 00:30:24.000000 nerfstudio-0.2.1/nerfstudio/process_data/process_data_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4787 2023-04-19 00:30:24.000000 nerfstudio-0.2.1/nerfstudio/process_data/realitycapture_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3130 2023-04-19 00:30:24.000000 nerfstudio-0.2.1/nerfstudio/process_data/record3d_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 00:30:24.000000 nerfstudio-0.2.1/nerfstudio/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 00:30:37.919915 nerfstudio-0.2.1/nerfstudio/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      605 2023-04-19 00:30:24.000000 nerfstudio-0.2.1/nerfstudio/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3370 2023-04-19 00:30:24.000000 nerfstudio-0.2.1/nerfstudio/utils/colormaps.py
--rw-r--r--   0 runner    (1001) docker     (123)     1673 2023-04-19 00:30:24.000000 nerfstudio-0.2.1/nerfstudio/utils/colors.py
--rw-r--r--   0 runner    (1001) docker     (123)     2409 2023-04-19 00:30:24.000000 nerfstudio-0.2.1/nerfstudio/utils/comms.py
--rw-r--r--   0 runner    (1001) docker     (123)     2465 2023-04-19 00:30:24.000000 nerfstudio-0.2.1/nerfstudio/utils/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)     4222 2023-04-19 00:30:24.000000 nerfstudio-0.2.1/nerfstudio/utils/eval_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1659 2023-04-19 00:30:24.000000 nerfstudio-0.2.1/nerfstudio/utils/install_checks.py
--rw-r--r--   0 runner    (1001) docker     (123)     1264 2023-04-19 00:30:24.000000 nerfstudio-0.2.1/nerfstudio/utils/io.py
--rw-r--r--   0 runner    (1001) docker     (123)    12347 2023-04-19 00:30:24.000000 nerfstudio-0.2.1/nerfstudio/utils/math.py
--rw-r--r--   0 runner    (1001) docker     (123)     4984 2023-04-19 00:30:24.000000 nerfstudio-0.2.1/nerfstudio/utils/misc.py
--rw-r--r--   0 runner    (1001) docker     (123)    16501 2023-04-19 00:30:24.000000 nerfstudio-0.2.1/nerfstudio/utils/plotly_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2622 2023-04-19 00:30:24.000000 nerfstudio-0.2.1/nerfstudio/utils/poses.py
--rw-r--r--   0 runner    (1001) docker     (123)     1573 2023-04-19 00:30:24.000000 nerfstudio-0.2.1/nerfstudio/utils/printing.py
--rw-r--r--   0 runner    (1001) docker     (123)     7229 2023-04-19 00:30:24.000000 nerfstudio-0.2.1/nerfstudio/utils/profiler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2315 2023-04-19 00:30:24.000000 nerfstudio-0.2.1/nerfstudio/utils/rich_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1543 2023-04-19 00:30:24.000000 nerfstudio-0.2.1/nerfstudio/utils/scripts.py
--rw-r--r--   0 runner    (1001) docker     (123)    13383 2023-04-19 00:30:24.000000 nerfstudio-0.2.1/nerfstudio/utils/tensor_dataclass.py
--rw-r--r--   0 runner    (1001) docker     (123)    17010 2023-04-19 00:30:24.000000 nerfstudio-0.2.1/nerfstudio/utils/writer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 00:30:37.919915 nerfstudio-0.2.1/nerfstudio/viewer/
--rw-r--r--   0 runner    (1001) docker     (123)      605 2023-04-19 00:30:24.000000 nerfstudio-0.2.1/nerfstudio/viewer/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 00:30:37.923915 nerfstudio-0.2.1/nerfstudio/viewer/app/
--rw-r--r--   0 runner    (1001) docker     (123)     2352 2023-04-19 00:30:24.000000 nerfstudio-0.2.1/nerfstudio/viewer/app/package.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 00:30:37.923915 nerfstudio-0.2.1/nerfstudio/viewer/app/public/
--rw-r--r--   0 runner    (1001) docker     (123)      185 2023-04-19 00:30:24.000000 nerfstudio-0.2.1/nerfstudio/viewer/app/public/manifest.json
--rw-r--r--   0 runner    (1001) docker     (123)     4658 2023-04-19 00:30:24.000000 nerfstudio-0.2.1/nerfstudio/viewer/app/run_deploy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 00:30:37.875915 nerfstudio-0.2.1/nerfstudio/viewer/app/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 00:30:37.923915 nerfstudio-0.2.1/nerfstudio/viewer/app/src/themes/
--rw-r--r--   0 runner    (1001) docker     (123)     1165 2023-04-19 00:30:24.000000 nerfstudio-0.2.1/nerfstudio/viewer/app/src/themes/leva_theme.json
--rw-r--r--   0 runner    (1001) docker     (123)      503 2023-04-19 00:30:24.000000 nerfstudio-0.2.1/nerfstudio/viewer/app/tsconfig.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 00:30:37.923915 nerfstudio-0.2.1/nerfstudio/viewer/server/
--rw-r--r--   0 runner    (1001) docker     (123)      605 2023-04-19 00:30:24.000000 nerfstudio-0.2.1/nerfstudio/viewer/server/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9530 2023-04-19 00:30:24.000000 nerfstudio-0.2.1/nerfstudio/viewer/server/control_panel.py
--rw-r--r--   0 runner    (1001) docker     (123)     2784 2023-04-19 00:30:24.000000 nerfstudio-0.2.1/nerfstudio/viewer/server/gui_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1551 2023-04-19 00:30:24.000000 nerfstudio-0.2.1/nerfstudio/viewer/server/path.py
--rw-r--r--   0 runner    (1001) docker     (123)    11826 2023-04-19 00:30:24.000000 nerfstudio-0.2.1/nerfstudio/viewer/server/render_state_machine.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 00:30:37.923915 nerfstudio-0.2.1/nerfstudio/viewer/server/state/
--rw-r--r--   0 runner    (1001) docker     (123)     1715 2023-04-19 00:30:24.000000 nerfstudio-0.2.1/nerfstudio/viewer/server/state/node.py
--rw-r--r--   0 runner    (1001) docker     (123)      922 2023-04-19 00:30:24.000000 nerfstudio-0.2.1/nerfstudio/viewer/server/state/state_node.py
--rw-r--r--   0 runner    (1001) docker     (123)     4351 2023-04-19 00:30:24.000000 nerfstudio-0.2.1/nerfstudio/viewer/server/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    11592 2023-04-19 00:30:24.000000 nerfstudio-0.2.1/nerfstudio/viewer/server/viewer_elements.py
--rw-r--r--   0 runner    (1001) docker     (123)    15004 2023-04-19 00:30:24.000000 nerfstudio-0.2.1/nerfstudio/viewer/server/viewer_state.py
--rw-r--r--   0 runner    (1001) docker     (123)     6059 2023-04-19 00:30:24.000000 nerfstudio-0.2.1/nerfstudio/viewer/server/viewer_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 00:30:37.927915 nerfstudio-0.2.1/nerfstudio/viewer/viser/
--rw-r--r--   0 runner    (1001) docker     (123)      917 2023-04-19 00:30:24.000000 nerfstudio-0.2.1/nerfstudio/viewer/viser/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6413 2023-04-19 00:30:24.000000 nerfstudio-0.2.1/nerfstudio/viewer/viser/gui.py
--rw-r--r--   0 runner    (1001) docker     (123)    18392 2023-04-19 00:30:24.000000 nerfstudio-0.2.1/nerfstudio/viewer/viser/message_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     6244 2023-04-19 00:30:24.000000 nerfstudio-0.2.1/nerfstudio/viewer/viser/messages.py
--rw-r--r--   0 runner    (1001) docker     (123)     2318 2023-04-19 00:30:24.000000 nerfstudio-0.2.1/nerfstudio/viewer/viser/server.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 00:30:37.879915 nerfstudio-0.2.1/nerfstudio.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    19021 2023-04-19 00:30:37.000000 nerfstudio-0.2.1/nerfstudio.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7030 2023-04-19 00:30:37.000000 nerfstudio-0.2.1/nerfstudio.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 00:30:37.000000 nerfstudio-0.2.1/nerfstudio.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      518 2023-04-19 00:30:37.000000 nerfstudio-0.2.1/nerfstudio.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1127 2023-04-19 00:30:37.000000 nerfstudio-0.2.1/nerfstudio.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-04-19 00:30:37.000000 nerfstudio-0.2.1/nerfstudio.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     4290 2023-04-19 00:30:24.000000 nerfstudio-0.2.1/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 00:30:37.927915 nerfstudio-0.2.1/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 00:30:24.000000 nerfstudio-0.2.1/scripts/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 00:30:37.927915 nerfstudio-0.2.1/scripts/blender/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 00:30:24.000000 nerfstudio-0.2.1/scripts/blender/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16781 2023-04-19 00:30:24.000000 nerfstudio-0.2.1/scripts/blender/nerfstudio_blender.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 00:30:37.931915 nerfstudio-0.2.1/scripts/completions/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 00:30:24.000000 nerfstudio-0.2.1/scripts/completions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14909 2023-04-19 00:30:24.000000 nerfstudio-0.2.1/scripts/completions/install.py
--rw-r--r--   0 runner    (1001) docker     (123)      442 2023-04-19 00:30:24.000000 nerfstudio-0.2.1/scripts/completions/setup.bash
--rw-r--r--   0 runner    (1001) docker     (123)      999 2023-04-19 00:30:24.000000 nerfstudio-0.2.1/scripts/completions/setup.zsh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 00:30:37.931915 nerfstudio-0.2.1/scripts/datasets/
--rw-r--r--   0 runner    (1001) docker     (123)     5490 2023-04-19 00:30:24.000000 nerfstudio-0.2.1/scripts/datasets/process_nuscenes_masks.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 00:30:37.931915 nerfstudio-0.2.1/scripts/docs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 00:30:24.000000 nerfstudio-0.2.1/scripts/docs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2648 2023-04-19 00:30:24.000000 nerfstudio-0.2.1/scripts/docs/add_nb_tags.py
--rw-r--r--   0 runner    (1001) docker     (123)     1402 2023-04-19 00:30:24.000000 nerfstudio-0.2.1/scripts/docs/build_docs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 00:30:37.931915 nerfstudio-0.2.1/scripts/downloads/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 00:30:24.000000 nerfstudio-0.2.1/scripts/downloads/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19561 2023-04-19 00:30:24.000000 nerfstudio-0.2.1/scripts/downloads/download_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     1587 2023-04-19 00:30:24.000000 nerfstudio-0.2.1/scripts/eval.py
--rw-r--r--   0 runner    (1001) docker     (123)    17407 2023-04-19 00:30:24.000000 nerfstudio-0.2.1/scripts/exporter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 00:30:37.931915 nerfstudio-0.2.1/scripts/generative/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 00:30:24.000000 nerfstudio-0.2.1/scripts/generative/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3226 2023-04-19 00:30:24.000000 nerfstudio-0.2.1/scripts/generative/trace_stable_diffusion.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 00:30:37.935915 nerfstudio-0.2.1/scripts/github/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 00:30:24.000000 nerfstudio-0.2.1/scripts/github/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3438 2023-04-19 00:30:24.000000 nerfstudio-0.2.1/scripts/github/run_actions.py
--rw-r--r--   0 runner    (1001) docker     (123)    35406 2023-04-19 00:30:24.000000 nerfstudio-0.2.1/scripts/process_data.py
--rw-r--r--   0 runner    (1001) docker     (123)    14237 2023-04-19 00:30:24.000000 nerfstudio-0.2.1/scripts/render.py
--rw-r--r--   0 runner    (1001) docker     (123)     2341 2023-04-19 00:30:24.000000 nerfstudio-0.2.1/scripts/texture.py
--rw-r--r--   0 runner    (1001) docker     (123)     8810 2023-04-19 00:30:24.000000 nerfstudio-0.2.1/scripts/train.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 00:30:37.935915 nerfstudio-0.2.1/scripts/viewer/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 00:30:24.000000 nerfstudio-0.2.1/scripts/viewer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3326 2023-04-19 00:30:24.000000 nerfstudio-0.2.1/scripts/viewer/run_viewer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1326 2023-04-19 00:30:24.000000 nerfstudio-0.2.1/scripts/viewer/sync_viser_message_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-19 00:30:37.935915 nerfstudio-0.2.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 00:30:37.935915 nerfstudio-0.2.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2591 2023-04-19 00:30:24.000000 nerfstudio-0.2.1/tests/test_train.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 21:45:43.438244 nerfstudio-0.2.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-04 21:45:23.000000 nerfstudio-0.2.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    19505 2023-05-04 21:45:43.438244 nerfstudio-0.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    19084 2023-05-04 21:45:33.000000 nerfstudio-0.2.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 21:45:43.410243 nerfstudio-0.2.2/nerfstudio/
+-rw-r--r--   0 runner    (1001) docker     (123)      605 2023-05-04 21:45:23.000000 nerfstudio-0.2.2/nerfstudio/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 21:45:43.410243 nerfstudio-0.2.2/nerfstudio/cameras/
+-rw-r--r--   0 runner    (1001) docker     (123)      605 2023-05-04 21:45:23.000000 nerfstudio-0.2.2/nerfstudio/cameras/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4893 2023-05-04 21:45:23.000000 nerfstudio-0.2.2/nerfstudio/cameras/camera_optimizers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5940 2023-05-04 21:45:23.000000 nerfstudio-0.2.2/nerfstudio/cameras/camera_paths.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21340 2023-05-04 21:45:23.000000 nerfstudio-0.2.2/nerfstudio/cameras/camera_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41257 2023-05-04 21:45:23.000000 nerfstudio-0.2.2/nerfstudio/cameras/cameras.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4772 2023-05-04 21:45:23.000000 nerfstudio-0.2.2/nerfstudio/cameras/lie_groups.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10287 2023-05-04 21:45:23.000000 nerfstudio-0.2.2/nerfstudio/cameras/rays.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 21:45:43.414244 nerfstudio-0.2.2/nerfstudio/configs/
+-rw-r--r--   0 runner    (1001) docker     (123)      605 2023-05-04 21:45:23.000000 nerfstudio-0.2.2/nerfstudio/configs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5617 2023-05-04 21:45:23.000000 nerfstudio-0.2.2/nerfstudio/configs/base_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1547 2023-05-04 21:45:23.000000 nerfstudio-0.2.2/nerfstudio/configs/config_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5125 2023-05-04 21:45:23.000000 nerfstudio-0.2.2/nerfstudio/configs/experiment_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21975 2023-05-04 21:45:23.000000 nerfstudio-0.2.2/nerfstudio/configs/method_configs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 21:45:43.414244 nerfstudio-0.2.2/nerfstudio/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      605 2023-05-04 21:45:23.000000 nerfstudio-0.2.2/nerfstudio/data/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 21:45:43.414244 nerfstudio-0.2.2/nerfstudio/data/datamanagers/
+-rw-r--r--   0 runner    (1001) docker     (123)      605 2023-05-04 21:45:23.000000 nerfstudio-0.2.2/nerfstudio/data/datamanagers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24424 2023-05-04 21:45:23.000000 nerfstudio-0.2.2/nerfstudio/data/datamanagers/base_datamanager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1738 2023-05-04 21:45:23.000000 nerfstudio-0.2.2/nerfstudio/data/datamanagers/depth_datamanager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1714 2023-05-04 21:45:23.000000 nerfstudio-0.2.2/nerfstudio/data/datamanagers/sdf_datamanager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1923 2023-05-04 21:45:23.000000 nerfstudio-0.2.2/nerfstudio/data/datamanagers/semantic_datamanager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 21:45:43.414244 nerfstudio-0.2.2/nerfstudio/data/dataparsers/
+-rw-r--r--   0 runner    (1001) docker     (123)      605 2023-05-04 21:45:23.000000 nerfstudio-0.2.2/nerfstudio/data/dataparsers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9094 2023-05-04 21:45:23.000000 nerfstudio-0.2.2/nerfstudio/data/dataparsers/arkitscenes_dataparser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7230 2023-05-04 21:45:23.000000 nerfstudio-0.2.2/nerfstudio/data/dataparsers/base_dataparser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3731 2023-05-04 21:45:23.000000 nerfstudio-0.2.2/nerfstudio/data/dataparsers/blender_dataparser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3774 2023-05-04 21:45:23.000000 nerfstudio-0.2.2/nerfstudio/data/dataparsers/dnerf_dataparser.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13531 2023-05-04 21:45:23.000000 nerfstudio-0.2.2/nerfstudio/data/dataparsers/dycheck_dataparser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6783 2023-05-04 21:45:23.000000 nerfstudio-0.2.2/nerfstudio/data/dataparsers/instant_ngp_dataparser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4211 2023-05-04 21:45:23.000000 nerfstudio-0.2.2/nerfstudio/data/dataparsers/minimal_dataparser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8553 2023-05-04 21:45:23.000000 nerfstudio-0.2.2/nerfstudio/data/dataparsers/nerfosr_dataparser.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14847 2023-05-04 21:45:23.000000 nerfstudio-0.2.2/nerfstudio/data/dataparsers/nerfstudio_dataparser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8573 2023-05-04 21:45:23.000000 nerfstudio-0.2.2/nerfstudio/data/dataparsers/nuscenes_dataparser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7016 2023-05-04 21:45:23.000000 nerfstudio-0.2.2/nerfstudio/data/dataparsers/phototourism_dataparser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6755 2023-05-04 21:45:23.000000 nerfstudio-0.2.2/nerfstudio/data/dataparsers/scannet_dataparser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5692 2023-05-04 21:45:23.000000 nerfstudio-0.2.2/nerfstudio/data/dataparsers/sdfstudio_dataparser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6004 2023-05-04 21:45:23.000000 nerfstudio-0.2.2/nerfstudio/data/dataparsers/sitcoms3d_dataparser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 21:45:43.418244 nerfstudio-0.2.2/nerfstudio/data/datasets/
+-rw-r--r--   0 runner    (1001) docker     (123)      605 2023-05-04 21:45:23.000000 nerfstudio-0.2.2/nerfstudio/data/datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4996 2023-05-04 21:45:23.000000 nerfstudio-0.2.2/nerfstudio/data/datasets/base_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2214 2023-05-04 21:45:23.000000 nerfstudio-0.2.2/nerfstudio/data/datasets/depth_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3694 2023-05-04 21:45:23.000000 nerfstudio-0.2.2/nerfstudio/data/datasets/sdf_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2035 2023-05-04 21:45:23.000000 nerfstudio-0.2.2/nerfstudio/data/datasets/semantic_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12741 2023-05-04 21:45:23.000000 nerfstudio-0.2.2/nerfstudio/data/pixel_samplers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2689 2023-05-04 21:45:23.000000 nerfstudio-0.2.2/nerfstudio/data/scene_box.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 21:45:43.418244 nerfstudio-0.2.2/nerfstudio/data/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      605 2023-05-04 21:45:23.000000 nerfstudio-0.2.2/nerfstudio/data/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20570 2023-05-04 21:45:23.000000 nerfstudio-0.2.2/nerfstudio/data/utils/colmap_parsing_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3408 2023-05-04 21:45:23.000000 nerfstudio-0.2.2/nerfstudio/data/utils/data_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8937 2023-05-04 21:45:23.000000 nerfstudio-0.2.2/nerfstudio/data/utils/dataloaders.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9620 2023-05-04 21:45:23.000000 nerfstudio-0.2.2/nerfstudio/data/utils/nerfstudio_collate.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 21:45:43.418244 nerfstudio-0.2.2/nerfstudio/engine/
+-rw-r--r--   0 runner    (1001) docker     (123)      605 2023-05-04 21:45:23.000000 nerfstudio-0.2.2/nerfstudio/engine/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3915 2023-05-04 21:45:23.000000 nerfstudio-0.2.2/nerfstudio/engine/callbacks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5738 2023-05-04 21:45:23.000000 nerfstudio-0.2.2/nerfstudio/engine/optimizers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6038 2023-05-04 21:45:23.000000 nerfstudio-0.2.2/nerfstudio/engine/schedulers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21082 2023-05-04 21:45:23.000000 nerfstudio-0.2.2/nerfstudio/engine/trainer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 21:45:43.418244 nerfstudio-0.2.2/nerfstudio/exporter/
+-rw-r--r--   0 runner    (1001) docker     (123)      605 2023-05-04 21:45:23.000000 nerfstudio-0.2.2/nerfstudio/exporter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12314 2023-05-04 21:45:23.000000 nerfstudio-0.2.2/nerfstudio/exporter/exporter_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10345 2023-05-04 21:45:23.000000 nerfstudio-0.2.2/nerfstudio/exporter/marching_cubes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21276 2023-05-04 21:45:23.000000 nerfstudio-0.2.2/nerfstudio/exporter/texture_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13842 2023-05-04 21:45:23.000000 nerfstudio-0.2.2/nerfstudio/exporter/tsdf_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 21:45:43.418244 nerfstudio-0.2.2/nerfstudio/field_components/
+-rw-r--r--   0 runner    (1001) docker     (123)      751 2023-05-04 21:45:23.000000 nerfstudio-0.2.2/nerfstudio/field_components/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1441 2023-05-04 21:45:23.000000 nerfstudio-0.2.2/nerfstudio/field_components/activations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2090 2023-05-04 21:45:23.000000 nerfstudio-0.2.2/nerfstudio/field_components/base_field_component.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 21:45:43.418244 nerfstudio-0.2.2/nerfstudio/field_components/cuda/
+-rw-r--r--   0 runner    (1001) docker     (123)     1125 2023-05-04 21:45:23.000000 nerfstudio-0.2.2/nerfstudio/field_components/cuda/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2185 2023-05-04 21:45:23.000000 nerfstudio-0.2.2/nerfstudio/field_components/cuda/_backend.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 21:45:43.422244 nerfstudio-0.2.2/nerfstudio/field_components/cuda/csrc/
+-rw-r--r--   0 runner    (1001) docker     (123)      446 2023-05-04 21:45:23.000000 nerfstudio-0.2.2/nerfstudio/field_components/cuda/csrc/pybind.cu
+-rw-r--r--   0 runner    (1001) docker     (123)    25118 2023-05-04 21:45:23.000000 nerfstudio-0.2.2/nerfstudio/field_components/cuda/csrc/temporal_gridencoder.cu
+-rw-r--r--   0 runner    (1001) docker     (123)     1657 2023-05-04 21:45:23.000000 nerfstudio-0.2.2/nerfstudio/field_components/embedding.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26684 2023-05-04 21:45:23.000000 nerfstudio-0.2.2/nerfstudio/field_components/encodings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6880 2023-05-04 21:45:23.000000 nerfstudio-0.2.2/nerfstudio/field_components/field_heads.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3646 2023-05-04 21:45:23.000000 nerfstudio-0.2.2/nerfstudio/field_components/mlp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3191 2023-05-04 21:45:23.000000 nerfstudio-0.2.2/nerfstudio/field_components/spatial_distortions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3339 2023-05-04 21:45:23.000000 nerfstudio-0.2.2/nerfstudio/field_components/temporal_distortions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16288 2023-05-04 21:45:23.000000 nerfstudio-0.2.2/nerfstudio/field_components/temporal_grid.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 21:45:43.422244 nerfstudio-0.2.2/nerfstudio/fields/
+-rw-r--r--   0 runner    (1001) docker     (123)      605 2023-05-04 21:45:23.000000 nerfstudio-0.2.2/nerfstudio/fields/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4935 2023-05-04 21:45:23.000000 nerfstudio-0.2.2/nerfstudio/fields/base_field.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4877 2023-05-04 21:45:23.000000 nerfstudio-0.2.2/nerfstudio/fields/density_fields.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7948 2023-05-04 21:45:23.000000 nerfstudio-0.2.2/nerfstudio/fields/instant_ngp_field.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17947 2023-05-04 21:45:23.000000 nerfstudio-0.2.2/nerfstudio/fields/nerfacto_field.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17504 2023-05-04 21:45:23.000000 nerfstudio-0.2.2/nerfstudio/fields/nerfplayer_nerfacto_field.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10793 2023-05-04 21:45:23.000000 nerfstudio-0.2.2/nerfstudio/fields/nerfplayer_ngp_field.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6864 2023-05-04 21:45:23.000000 nerfstudio-0.2.2/nerfstudio/fields/nerfw_field.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17642 2023-05-04 21:45:23.000000 nerfstudio-0.2.2/nerfstudio/fields/sdf_field.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4297 2023-05-04 21:45:23.000000 nerfstudio-0.2.2/nerfstudio/fields/semantic_nerf_field.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5865 2023-05-04 21:45:23.000000 nerfstudio-0.2.2/nerfstudio/fields/tensorf_field.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4666 2023-05-04 21:45:23.000000 nerfstudio-0.2.2/nerfstudio/fields/vanilla_nerf_field.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 21:45:43.422244 nerfstudio-0.2.2/nerfstudio/generative/
+-rw-r--r--   0 runner    (1001) docker     (123)      605 2023-05-04 21:45:23.000000 nerfstudio-0.2.2/nerfstudio/generative/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13907 2023-05-04 21:45:23.000000 nerfstudio-0.2.2/nerfstudio/generative/stable_diffusion.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 21:45:43.422244 nerfstudio-0.2.2/nerfstudio/model_components/
+-rw-r--r--   0 runner    (1001) docker     (123)      605 2023-05-04 21:45:23.000000 nerfstudio-0.2.2/nerfstudio/model_components/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18593 2023-05-04 21:45:23.000000 nerfstudio-0.2.2/nerfstudio/model_components/losses.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2159 2023-05-04 21:45:23.000000 nerfstudio-0.2.2/nerfstudio/model_components/ray_generators.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28665 2023-05-04 21:45:23.000000 nerfstudio-0.2.2/nerfstudio/model_components/ray_samplers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12636 2023-05-04 21:45:23.000000 nerfstudio-0.2.2/nerfstudio/model_components/renderers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6615 2023-05-04 21:45:23.000000 nerfstudio-0.2.2/nerfstudio/model_components/scene_colliders.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2478 2023-05-04 21:45:23.000000 nerfstudio-0.2.2/nerfstudio/model_components/shaders.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 21:45:43.426244 nerfstudio-0.2.2/nerfstudio/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      605 2023-05-04 21:45:23.000000 nerfstudio-0.2.2/nerfstudio/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8427 2023-05-04 21:45:23.000000 nerfstudio-0.2.2/nerfstudio/models/base_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16122 2023-05-04 21:45:23.000000 nerfstudio-0.2.2/nerfstudio/models/base_surface_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5511 2023-05-04 21:45:23.000000 nerfstudio-0.2.2/nerfstudio/models/depth_nerfacto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9810 2023-05-04 21:45:23.000000 nerfstudio-0.2.2/nerfstudio/models/instant_ngp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7763 2023-05-04 21:45:23.000000 nerfstudio-0.2.2/nerfstudio/models/mipnerf.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15990 2023-05-04 21:45:23.000000 nerfstudio-0.2.2/nerfstudio/models/nerfacto.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11345 2023-05-04 21:45:23.000000 nerfstudio-0.2.2/nerfstudio/models/nerfplayer_nerfacto.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11869 2023-05-04 21:45:23.000000 nerfstudio-0.2.2/nerfstudio/models/nerfplayer_ngp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4103 2023-05-04 21:45:23.000000 nerfstudio-0.2.2/nerfstudio/models/neus.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9418 2023-05-04 21:45:23.000000 nerfstudio-0.2.2/nerfstudio/models/neus_facto.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13345 2023-05-04 21:45:23.000000 nerfstudio-0.2.2/nerfstudio/models/semantic_nerfw.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12781 2023-05-04 21:45:23.000000 nerfstudio-0.2.2/nerfstudio/models/tensorf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9815 2023-05-04 21:45:23.000000 nerfstudio-0.2.2/nerfstudio/models/vanilla_nerf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 21:45:43.426244 nerfstudio-0.2.2/nerfstudio/pipelines/
+-rw-r--r--   0 runner    (1001) docker     (123)      605 2023-05-04 21:45:23.000000 nerfstudio-0.2.2/nerfstudio/pipelines/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16520 2023-05-04 21:45:23.000000 nerfstudio-0.2.2/nerfstudio/pipelines/base_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4346 2023-05-04 21:45:23.000000 nerfstudio-0.2.2/nerfstudio/pipelines/dynamic_batch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 21:45:43.426244 nerfstudio-0.2.2/nerfstudio/plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)      605 2023-05-04 21:45:23.000000 nerfstudio-0.2.2/nerfstudio/plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2971 2023-05-04 21:45:23.000000 nerfstudio-0.2.2/nerfstudio/plugins/registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-05-04 21:45:23.000000 nerfstudio-0.2.2/nerfstudio/plugins/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 21:45:43.426244 nerfstudio-0.2.2/nerfstudio/process_data/
+-rw-r--r--   0 runner    (1001) docker     (123)      605 2023-05-04 21:45:23.000000 nerfstudio-0.2.2/nerfstudio/process_data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1632 2023-05-04 21:45:23.000000 nerfstudio-0.2.2/nerfstudio/process_data/base_converter_to_nerfstudio_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9586 2023-05-04 21:45:23.000000 nerfstudio-0.2.2/nerfstudio/process_data/colmap_converter_to_nerfstudio_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24632 2023-05-04 21:45:23.000000 nerfstudio-0.2.2/nerfstudio/process_data/colmap_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8215 2023-05-04 21:45:23.000000 nerfstudio-0.2.2/nerfstudio/process_data/equirect_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5179 2023-05-04 21:45:23.000000 nerfstudio-0.2.2/nerfstudio/process_data/hloc_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4447 2023-05-04 21:45:23.000000 nerfstudio-0.2.2/nerfstudio/process_data/images_to_nerfstudio_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7387 2023-05-04 21:45:23.000000 nerfstudio-0.2.2/nerfstudio/process_data/metashape_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9185 2023-05-04 21:45:23.000000 nerfstudio-0.2.2/nerfstudio/process_data/polycam_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19997 2023-05-04 21:45:23.000000 nerfstudio-0.2.2/nerfstudio/process_data/process_data_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4787 2023-05-04 21:45:23.000000 nerfstudio-0.2.2/nerfstudio/process_data/realitycapture_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3130 2023-05-04 21:45:23.000000 nerfstudio-0.2.2/nerfstudio/process_data/record3d_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4660 2023-05-04 21:45:23.000000 nerfstudio-0.2.2/nerfstudio/process_data/video_to_nerfstudio_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 21:45:23.000000 nerfstudio-0.2.2/nerfstudio/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 21:45:43.430244 nerfstudio-0.2.2/nerfstudio/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      605 2023-05-04 21:45:23.000000 nerfstudio-0.2.2/nerfstudio/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3370 2023-05-04 21:45:23.000000 nerfstudio-0.2.2/nerfstudio/utils/colormaps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1673 2023-05-04 21:45:23.000000 nerfstudio-0.2.2/nerfstudio/utils/colors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2409 2023-05-04 21:45:23.000000 nerfstudio-0.2.2/nerfstudio/utils/comms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2465 2023-05-04 21:45:23.000000 nerfstudio-0.2.2/nerfstudio/utils/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4222 2023-05-04 21:45:23.000000 nerfstudio-0.2.2/nerfstudio/utils/eval_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1659 2023-05-04 21:45:23.000000 nerfstudio-0.2.2/nerfstudio/utils/install_checks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1264 2023-05-04 21:45:23.000000 nerfstudio-0.2.2/nerfstudio/utils/io.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11127 2023-05-04 21:45:23.000000 nerfstudio-0.2.2/nerfstudio/utils/math.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4984 2023-05-04 21:45:23.000000 nerfstudio-0.2.2/nerfstudio/utils/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16501 2023-05-04 21:45:23.000000 nerfstudio-0.2.2/nerfstudio/utils/plotly_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2622 2023-05-04 21:45:23.000000 nerfstudio-0.2.2/nerfstudio/utils/poses.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1573 2023-05-04 21:45:23.000000 nerfstudio-0.2.2/nerfstudio/utils/printing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7394 2023-05-04 21:45:23.000000 nerfstudio-0.2.2/nerfstudio/utils/profiler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2315 2023-05-04 21:45:23.000000 nerfstudio-0.2.2/nerfstudio/utils/rich_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1543 2023-05-04 21:45:23.000000 nerfstudio-0.2.2/nerfstudio/utils/scripts.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13383 2023-05-04 21:45:23.000000 nerfstudio-0.2.2/nerfstudio/utils/tensor_dataclass.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17010 2023-05-04 21:45:23.000000 nerfstudio-0.2.2/nerfstudio/utils/writer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 21:45:43.430244 nerfstudio-0.2.2/nerfstudio/viewer/
+-rw-r--r--   0 runner    (1001) docker     (123)      605 2023-05-04 21:45:23.000000 nerfstudio-0.2.2/nerfstudio/viewer/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 21:45:43.430244 nerfstudio-0.2.2/nerfstudio/viewer/app/
+-rw-r--r--   0 runner    (1001) docker     (123)     2582 2023-05-04 21:45:23.000000 nerfstudio-0.2.2/nerfstudio/viewer/app/package.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 21:45:43.430244 nerfstudio-0.2.2/nerfstudio/viewer/app/public/
+-rw-r--r--   0 runner    (1001) docker     (123)      185 2023-05-04 21:45:23.000000 nerfstudio-0.2.2/nerfstudio/viewer/app/public/manifest.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4658 2023-05-04 21:45:23.000000 nerfstudio-0.2.2/nerfstudio/viewer/app/run_deploy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 21:45:43.406243 nerfstudio-0.2.2/nerfstudio/viewer/app/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 21:45:43.430244 nerfstudio-0.2.2/nerfstudio/viewer/app/src/themes/
+-rw-r--r--   0 runner    (1001) docker     (123)     1165 2023-05-04 21:45:23.000000 nerfstudio-0.2.2/nerfstudio/viewer/app/src/themes/leva_theme.json
+-rw-r--r--   0 runner    (1001) docker     (123)      503 2023-05-04 21:45:23.000000 nerfstudio-0.2.2/nerfstudio/viewer/app/tsconfig.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 21:45:43.434244 nerfstudio-0.2.2/nerfstudio/viewer/server/
+-rw-r--r--   0 runner    (1001) docker     (123)      605 2023-05-04 21:45:23.000000 nerfstudio-0.2.2/nerfstudio/viewer/server/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9530 2023-05-04 21:45:23.000000 nerfstudio-0.2.2/nerfstudio/viewer/server/control_panel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2258 2023-05-04 21:45:23.000000 nerfstudio-0.2.2/nerfstudio/viewer/server/gui_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1551 2023-05-04 21:45:23.000000 nerfstudio-0.2.2/nerfstudio/viewer/server/path.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12076 2023-05-04 21:45:23.000000 nerfstudio-0.2.2/nerfstudio/viewer/server/render_state_machine.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 21:45:43.434244 nerfstudio-0.2.2/nerfstudio/viewer/server/state/
+-rw-r--r--   0 runner    (1001) docker     (123)     1715 2023-05-04 21:45:23.000000 nerfstudio-0.2.2/nerfstudio/viewer/server/state/node.py
+-rw-r--r--   0 runner    (1001) docker     (123)      922 2023-05-04 21:45:23.000000 nerfstudio-0.2.2/nerfstudio/viewer/server/state/state_node.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4351 2023-05-04 21:45:23.000000 nerfstudio-0.2.2/nerfstudio/viewer/server/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11592 2023-05-04 21:45:23.000000 nerfstudio-0.2.2/nerfstudio/viewer/server/viewer_elements.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15219 2023-05-04 21:45:23.000000 nerfstudio-0.2.2/nerfstudio/viewer/server/viewer_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6059 2023-05-04 21:45:23.000000 nerfstudio-0.2.2/nerfstudio/viewer/server/viewer_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 21:45:43.434244 nerfstudio-0.2.2/nerfstudio/viewer/viser/
+-rw-r--r--   0 runner    (1001) docker     (123)      917 2023-05-04 21:45:23.000000 nerfstudio-0.2.2/nerfstudio/viewer/viser/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6413 2023-05-04 21:45:23.000000 nerfstudio-0.2.2/nerfstudio/viewer/viser/gui.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18638 2023-05-04 21:45:23.000000 nerfstudio-0.2.2/nerfstudio/viewer/viser/message_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6516 2023-05-04 21:45:23.000000 nerfstudio-0.2.2/nerfstudio/viewer/viser/messages.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2318 2023-05-04 21:45:23.000000 nerfstudio-0.2.2/nerfstudio/viewer/viser/server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 21:45:43.410243 nerfstudio-0.2.2/nerfstudio.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    19505 2023-05-04 21:45:43.000000 nerfstudio-0.2.2/nerfstudio.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7381 2023-05-04 21:45:43.000000 nerfstudio-0.2.2/nerfstudio.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 21:45:43.000000 nerfstudio-0.2.2/nerfstudio.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      518 2023-05-04 21:45:43.000000 nerfstudio-0.2.2/nerfstudio.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1127 2023-05-04 21:45:43.000000 nerfstudio-0.2.2/nerfstudio.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-04 21:45:43.000000 nerfstudio-0.2.2/nerfstudio.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     4298 2023-05-04 21:45:23.000000 nerfstudio-0.2.2/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 21:45:43.434244 nerfstudio-0.2.2/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 21:45:23.000000 nerfstudio-0.2.2/scripts/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 21:45:43.434244 nerfstudio-0.2.2/scripts/blender/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 21:45:23.000000 nerfstudio-0.2.2/scripts/blender/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16781 2023-05-04 21:45:23.000000 nerfstudio-0.2.2/scripts/blender/nerfstudio_blender.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 21:45:43.434244 nerfstudio-0.2.2/scripts/completions/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 21:45:23.000000 nerfstudio-0.2.2/scripts/completions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14909 2023-05-04 21:45:23.000000 nerfstudio-0.2.2/scripts/completions/install.py
+-rw-r--r--   0 runner    (1001) docker     (123)      442 2023-05-04 21:45:23.000000 nerfstudio-0.2.2/scripts/completions/setup.bash
+-rw-r--r--   0 runner    (1001) docker     (123)      999 2023-05-04 21:45:23.000000 nerfstudio-0.2.2/scripts/completions/setup.zsh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 21:45:43.434244 nerfstudio-0.2.2/scripts/datasets/
+-rw-r--r--   0 runner    (1001) docker     (123)     5634 2023-05-04 21:45:23.000000 nerfstudio-0.2.2/scripts/datasets/process_nuscenes_masks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 21:45:43.434244 nerfstudio-0.2.2/scripts/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 21:45:23.000000 nerfstudio-0.2.2/scripts/docs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2648 2023-05-04 21:45:23.000000 nerfstudio-0.2.2/scripts/docs/add_nb_tags.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1402 2023-05-04 21:45:23.000000 nerfstudio-0.2.2/scripts/docs/build_docs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 21:45:43.434244 nerfstudio-0.2.2/scripts/downloads/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 21:45:23.000000 nerfstudio-0.2.2/scripts/downloads/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19561 2023-05-04 21:45:23.000000 nerfstudio-0.2.2/scripts/downloads/download_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1587 2023-05-04 21:45:23.000000 nerfstudio-0.2.2/scripts/eval.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17407 2023-05-04 21:45:23.000000 nerfstudio-0.2.2/scripts/exporter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 21:45:43.438244 nerfstudio-0.2.2/scripts/generative/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 21:45:23.000000 nerfstudio-0.2.2/scripts/generative/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3226 2023-05-04 21:45:23.000000 nerfstudio-0.2.2/scripts/generative/trace_stable_diffusion.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 21:45:43.438244 nerfstudio-0.2.2/scripts/github/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 21:45:23.000000 nerfstudio-0.2.2/scripts/github/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3438 2023-05-04 21:45:23.000000 nerfstudio-0.2.2/scripts/github/run_actions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16389 2023-05-04 21:45:23.000000 nerfstudio-0.2.2/scripts/process_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14683 2023-05-04 21:45:23.000000 nerfstudio-0.2.2/scripts/render.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2341 2023-05-04 21:45:23.000000 nerfstudio-0.2.2/scripts/texture.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8810 2023-05-04 21:45:23.000000 nerfstudio-0.2.2/scripts/train.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 21:45:43.438244 nerfstudio-0.2.2/scripts/viewer/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 21:45:23.000000 nerfstudio-0.2.2/scripts/viewer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3326 2023-05-04 21:45:23.000000 nerfstudio-0.2.2/scripts/viewer/run_viewer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1693 2023-05-04 21:45:23.000000 nerfstudio-0.2.2/scripts/viewer/sync_viser_message_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-04 21:45:43.438244 nerfstudio-0.2.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 21:45:43.438244 nerfstudio-0.2.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2591 2023-05-04 21:45:23.000000 nerfstudio-0.2.2/tests/test_train.py
```

### Comparing `nerfstudio-0.2.1/LICENSE` & `nerfstudio-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `nerfstudio-0.2.1/PKG-INFO` & `nerfstudio-0.2.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,7 @@
-Metadata-Version: 2.1
-Name: nerfstudio
-Version: 0.2.1
-Summary: All-in-one repository for state-of-the-art NeRFs
-License: Apache 2.0
-Project-URL: Documentation, https://docs.nerf.studio
-Classifier: Development Status :: 3 - Alpha
-Classifier: Programming Language :: Python
-Requires-Python: >=3.7.3
-Description-Content-Type: text/markdown
-Provides-Extra: gen
-Provides-Extra: dev
-Provides-Extra: docs
-License-File: LICENSE
-
 <p align="center">
     <!-- community badges -->
     <a href="https://discord.gg/uMbNqcraFc"><img src="https://img.shields.io/badge/Join-Discord-blue.svg"/></a>
     <!-- doc badges -->
     <a href='https://plenoptix-nerfstudio.readthedocs-hosted.com/en/latest/?badge=latest'>
         <img src='https://readthedocs.com/projects/plenoptix-nerfstudio/badge/?version=latest' alt='Documentation Status' />
     </a>
@@ -62,20 +47,22 @@
 
 - [Quickstart](#quickstart)
 - [Learn more](#learn-more)
 - [Supported Features](#supported-features)
 
 # About
 
+_It’s as simple as plug and play with nerfstudio!_
+
 Nerfstudio provides a simple API that allows for a simplified end-to-end process of creating, training, and testing NeRFs.
 The library supports a **more interpretable implementation of NeRFs by modularizing each component.**
 With more modular NeRFs, we hope to create a more user-friendly experience in exploring the technology.
-Nerfstudio is a contributor-friendly repo with the goal of building a community where users can more easily build upon each other's contributions.
 
-It’s as simple as plug and play with nerfstudio!
+This is a contributor-friendly repo with the goal of building a community where users can more easily build upon each other's contributions.
+Nerfstudio initially launched as an opensource project by Berkeley students in [KAIR lab](https://people.eecs.berkeley.edu/~kanazawa/index.html#kair) at [Berkeley AI Research (BAIR)](https://bair.berkeley.edu/) in October 2022 as a part of a research project ([paper](https://arxiv.org/abs/2302.04264)). It is currently developed by Berkeley students and community contributors.
 
 We are committed to providing learning resources to help you understand the basics of (if you're just getting started), and keep up-to-date with (if you're a seasoned veteran) all things NeRF. As researchers, we know just how hard it is to get onboarded with this next-gen technology. So we're here to help with tutorials, documentation, and more!
 
 Have feature requests? Want to add your brand-spankin'-new NeRF model? Have a new dataset? **We welcome any and all [contributions](https://docs.nerf.studio/en/latest/reference/contributing.html)!** Please do not hesitate to reach out to the nerfstudio team with any questions via [Discord](https://discord.gg/uMbNqcraFc).
 
 We hope nerfstudio enables you to build faster :hammer: learn together :books: and contribute to our NeRF community :sparkling_heart:.
 
@@ -231,17 +218,17 @@
 
 Each model contains many parameters that can be changed, too many to list here. Use the `--help` command to see the full list of configuration options.
 
 ```bash
 ns-train nerfacto --help
 ```
 
-### Tensorboard / WandB
+### Tensorboard / WandB / Viewer
 
-We support three different methods to track training progress, using the viewer, [tensorboard](https://www.tensorflow.org/tensorboard), and [Weights and Biases](https://wandb.ai/site). You can specify which visualizer to use by appending `--vis {viewer, tensorboard, wandb}` to the training command. Note that only one may be used at a time. Additionally the viewer only works for methods that are fast (ie. nerfacto, instant-ngp), for slower methods like NeRF, use the other loggers.
+We support three different methods to track training progress, using the viewer, [tensorboard](https://www.tensorflow.org/tensorboard), and [Weights and Biases](https://wandb.ai/site). You can specify which visualizer to use by appending `--vis {viewer, tensorboard, wandb, viewer+wandb, viewer+tensorboard}` to the training command. Simultaneously utilizing the viewer alongside wandb or tensorboard may cause stuttering issues during evaluation steps. The viewer only works for methods that are fast (ie. nerfacto, instant-ngp), for slower methods like NeRF, use the other loggers.
 
 # Learn More
 
 And that's it for getting started with the basics of nerfstudio.
 
 If you're interested in learning more on how to create your own pipelines, develop with the viewer, run benchmarks, and more, please check out some of the quicklinks below or visit our [documentation](https://docs.nerf.studio/en/latest/) directly.
```

#### html2text {}

```diff
@@ -1,32 +1,31 @@
-Metadata-Version: 2.1 Name: nerfstudio Version: 0.2.1 Summary: All-in-one
-repository for state-of-the-art NeRFs License: Apache 2.0 Project-URL:
-Documentation, https://docs.nerf.studio Classifier: Development Status :: 3 -
-Alpha Classifier: Programming Language :: Python Requires-Python: >=3.7.3
-Description-Content-Type: text/markdown Provides-Extra: gen Provides-Extra: dev
-Provides-Extra: docs License-File: LICENSE
  [https://img.shields.io/badge/Join-Discord-blue.svg]  [Documentation_Status]
         [PyPI_version]  [Test_Status] [Viewer_build_Status]  [License]
                                  [nerfstudio]
 
                    A collaboration friendly studio for NeRFs
                        [documentation] [viewer] [colab]
 [https://user-images.githubusercontent.com/3310961/194017985-ade69503-9d68-
 46a2-b518-2db1a012f090.gif] [https://user-images.githubusercontent.com/3310961/
 194020648-7e5f380c-15ca-461d-8c1c-20beb586defe.gif] - [Quickstart](#quickstart)
 - [Learn more](#learn-more) - [Supported Features](#supported-features) # About
-Nerfstudio provides a simple API that allows for a simplified end-to-end
-process of creating, training, and testing NeRFs. The library supports a **more
-interpretable implementation of NeRFs by modularizing each component.** With
-more modular NeRFs, we hope to create a more user-friendly experience in
-exploring the technology. Nerfstudio is a contributor-friendly repo with the
-goal of building a community where users can more easily build upon each
-other's contributions. Itâs as simple as plug and play with nerfstudio! We
-are committed to providing learning resources to help you understand the basics
-of (if you're just getting started), and keep up-to-date with (if you're a
+_Itâs as simple as plug and play with nerfstudio!_ Nerfstudio provides a
+simple API that allows for a simplified end-to-end process of creating,
+training, and testing NeRFs. The library supports a **more interpretable
+implementation of NeRFs by modularizing each component.** With more modular
+NeRFs, we hope to create a more user-friendly experience in exploring the
+technology. This is a contributor-friendly repo with the goal of building a
+community where users can more easily build upon each other's contributions.
+Nerfstudio initially launched as an opensource project by Berkeley students in
+[KAIR lab](https://people.eecs.berkeley.edu/~kanazawa/index.html#kair) at
+[Berkeley AI Research (BAIR)](https://bair.berkeley.edu/) in October 2022 as a
+part of a research project ([paper](https://arxiv.org/abs/2302.04264)). It is
+currently developed by Berkeley students and community contributors. We are
+committed to providing learning resources to help you understand the basics of
+(if you're just getting started), and keep up-to-date with (if you're a
 seasoned veteran) all things NeRF. As researchers, we know just how hard it is
 to get onboarded with this next-gen technology. So we're here to help with
 tutorials, documentation, and more! Have feature requests? Want to add your
 brand-spankin'-new NeRF model? Have a new dataset? **We welcome any and all
 [contributions](https://docs.nerf.studio/en/latest/reference/
 contributing.html)!** Please do not hesitate to reach out to the nerfstudio
 team with any questions via [Discord](https://discord.gg/uMbNqcraFc). We hope
@@ -125,68 +124,69 @@
 Poses | ð | ## 5. Advanced Options ### Training models other than nerfacto
 We provide other models than nerfacto, for example if you want to train the
 original nerf model, use the following command ```bash ns-train vanilla-nerf --
 data DATA_PATH ``` For a full list of included models run `ns-train --help`.
 ### Modify Configuration Each model contains many parameters that can be
 changed, too many to list here. Use the `--help` command to see the full list
 of configuration options. ```bash ns-train nerfacto --help ``` ### Tensorboard
-/ WandB We support three different methods to track training progress, using
-the viewer, [tensorboard](https://www.tensorflow.org/tensorboard), and [Weights
-and Biases](https://wandb.ai/site). You can specify which visualizer to use by
-appending `--vis {viewer, tensorboard, wandb}` to the training command. Note
-that only one may be used at a time. Additionally the viewer only works for
-methods that are fast (ie. nerfacto, instant-ngp), for slower methods like
-NeRF, use the other loggers. # Learn More And that's it for getting started
-with the basics of nerfstudio. If you're interested in learning more on how to
-create your own pipelines, develop with the viewer, run benchmarks, and more,
-please check out some of the quicklinks below or visit our [documentation]
-(https://docs.nerf.studio/en/latest/) directly. | Section | Description | | ---
+/ WandB / Viewer We support three different methods to track training progress,
+using the viewer, [tensorboard](https://www.tensorflow.org/tensorboard), and
+[Weights and Biases](https://wandb.ai/site). You can specify which visualizer
+to use by appending `--vis {viewer, tensorboard, wandb, viewer+wandb,
+viewer+tensorboard}` to the training command. Simultaneously utilizing the
+viewer alongside wandb or tensorboard may cause stuttering issues during
+evaluation steps. The viewer only works for methods that are fast (ie.
+nerfacto, instant-ngp), for slower methods like NeRF, use the other loggers. #
+Learn More And that's it for getting started with the basics of nerfstudio. If
+you're interested in learning more on how to create your own pipelines, develop
+with the viewer, run benchmarks, and more, please check out some of the
+quicklinks below or visit our [documentation](https://docs.nerf.studio/en/
+latest/) directly. | Section | Description | | --------------------------------
+------------------------------------------------------------------ | ----------
 -------------------------------------------------------------------------------
----------------- | ------------------------------------------------------------
--------------------------------------- | | [Documentation](https://
-docs.nerf.studio/en/latest/) | Full API documentation and tutorials | |
-[Viewer](https://viewer.nerf.studio/) | Home page for our web viewer | | ð
-**Educational** | | [Model Descriptions](https://docs.nerf.studio/en/latest/
-nerfology/methods/index.html) | Description of all the models supported by
-nerfstudio and explanations of component parts. | | [Component Descriptions]
-(https://docs.nerf.studio/en/latest/nerfology/model_components/index.html) |
-Interactive notebooks that explain notable/commonly used modules in various
-models. | | ð **Tutorials** | | [Getting Started](https://docs.nerf.studio/
-en/latest/quickstart/installation.html) | A more in-depth guide on how to get
-started with nerfstudio from installation to contributing. | | [Using the
-Viewer](https://docs.nerf.studio/en/latest/quickstart/viewer_quickstart.html) |
-A quick demo video on how to navigate the viewer. | | [Using Record3D](https://
-www.youtube.com/watch?v=XwKq7qDQCQk) | Demo video on how to run nerfstudio
-without using COLMAP. | | ð» **For Developers** | | [Creating pipelines]
-(https://docs.nerf.studio/en/latest/developer_guides/pipelines/index.html) |
-Learn how to easily build new neural rendering pipelines by using and/or
-implementing new modules. | | [Creating datasets](https://docs.nerf.studio/en/
-latest/quickstart/custom_dataset.html) | Have a new dataset? Learn how to run
-it with nerfstudio. | | [Contributing](https://docs.nerf.studio/en/latest/
-reference/contributing.html) | Walk-through for how you can start contributing
-now. | | ð **Community** | | [Discord](https://discord.gg/uMbNqcraFc) | Join
-our community to discuss more. We would love to hear from you! | | [Twitter]
-(https://twitter.com/nerfstudioteam) | Follow us on Twitter @nerfstudioteam to
-see cool updates and announcements | # Supported Features We provide the
-following support structures to make life easier for getting started with
-NeRFs. **If you are looking for a feature that is not currently supported,
-please do not hesitate to contact the Nerfstudio Team on [Discord](https://
-discord.gg/uMbNqcraFc)!** - :mag_right: Web-based visualizer that allows you
-to: - Visualize training in real-time + interact with the scene - Create and
-render out scenes with custom camera trajectories - View different output types
-- And more! - :pencil2: Support for multiple logging interfaces (Tensorboard,
-Wandb), code profiling, and other built-in debugging tools - :
-chart_with_upwards_trend: Easy-to-use benchmarking scripts on the Blender
-dataset - :iphone: Full pipeline support (w/ Colmap, Polycam, or Record3D) for
-going from a video on your phone to a full 3D render. # Built On [tyro_logo] -
-Easy-to-use config system - Developed by [Brent Yi](https://brentyi.com/) [tyro
-logo] - Library for accelerating NeRF renders - Developed by [Ruilong Li]
-(https://www.liruilong.cn/) # Citation You can find a paper writeup of the
-framework on [arXiv](https://arxiv.org/abs/2302.04264). If you use this library
-or find the documentation useful for your research, please consider citing: ```
-@article{nerfstudio, author = {Tancik, Matthew and Weber, Ethan and Ng, Evonne
-and Li, Ruilong and Yi, Brent and Kerr, Justin and Wang, Terrance and
-Kristoffersen, Alexander and Austin, Jake and Salahi, Kamyar and Ahuja, Abhik
-and McAllister, David and Kanazawa, Angjoo}, title = {Nerfstudio: A Modular
-Framework for Neural Radiance Field Development}, journal = {arXiv preprint
-arXiv:2302.04264}, year = {2023}, } ``` # Contributors [https://contrib.rocks/
-image?repo=nerfstudio-project/nerfstudio]
+--------- | | [Documentation](https://docs.nerf.studio/en/latest/) | Full API
+documentation and tutorials | | [Viewer](https://viewer.nerf.studio/) | Home
+page for our web viewer | | ð **Educational** | | [Model Descriptions]
+(https://docs.nerf.studio/en/latest/nerfology/methods/index.html) | Description
+of all the models supported by nerfstudio and explanations of component parts.
+| | [Component Descriptions](https://docs.nerf.studio/en/latest/nerfology/
+model_components/index.html) | Interactive notebooks that explain notable/
+commonly used modules in various models. | | ð **Tutorials** | | [Getting
+Started](https://docs.nerf.studio/en/latest/quickstart/installation.html) | A
+more in-depth guide on how to get started with nerfstudio from installation to
+contributing. | | [Using the Viewer](https://docs.nerf.studio/en/latest/
+quickstart/viewer_quickstart.html) | A quick demo video on how to navigate the
+viewer. | | [Using Record3D](https://www.youtube.com/watch?v=XwKq7qDQCQk) |
+Demo video on how to run nerfstudio without using COLMAP. | | ð» **For
+Developers** | | [Creating pipelines](https://docs.nerf.studio/en/latest/
+developer_guides/pipelines/index.html) | Learn how to easily build new neural
+rendering pipelines by using and/or implementing new modules. | | [Creating
+datasets](https://docs.nerf.studio/en/latest/quickstart/custom_dataset.html) |
+Have a new dataset? Learn how to run it with nerfstudio. | | [Contributing]
+(https://docs.nerf.studio/en/latest/reference/contributing.html) | Walk-through
+for how you can start contributing now. | | ð **Community** | | [Discord]
+(https://discord.gg/uMbNqcraFc) | Join our community to discuss more. We would
+love to hear from you! | | [Twitter](https://twitter.com/nerfstudioteam) |
+Follow us on Twitter @nerfstudioteam to see cool updates and announcements | #
+Supported Features We provide the following support structures to make life
+easier for getting started with NeRFs. **If you are looking for a feature that
+is not currently supported, please do not hesitate to contact the Nerfstudio
+Team on [Discord](https://discord.gg/uMbNqcraFc)!** - :mag_right: Web-based
+visualizer that allows you to: - Visualize training in real-time + interact
+with the scene - Create and render out scenes with custom camera trajectories -
+View different output types - And more! - :pencil2: Support for multiple
+logging interfaces (Tensorboard, Wandb), code profiling, and other built-in
+debugging tools - :chart_with_upwards_trend: Easy-to-use benchmarking scripts
+on the Blender dataset - :iphone: Full pipeline support (w/ Colmap, Polycam, or
+Record3D) for going from a video on your phone to a full 3D render. # Built On
+[tyro_logo] - Easy-to-use config system - Developed by [Brent Yi](https://
+brentyi.com/) [tyro_logo] - Library for accelerating NeRF renders - Developed
+by [Ruilong Li](https://www.liruilong.cn/) # Citation You can find a paper
+writeup of the framework on [arXiv](https://arxiv.org/abs/2302.04264). If you
+use this library or find the documentation useful for your research, please
+consider citing: ``` @article{nerfstudio, author = {Tancik, Matthew and Weber,
+Ethan and Ng, Evonne and Li, Ruilong and Yi, Brent and Kerr, Justin and Wang,
+Terrance and Kristoffersen, Alexander and Austin, Jake and Salahi, Kamyar and
+Ahuja, Abhik and McAllister, David and Kanazawa, Angjoo}, title = {Nerfstudio:
+A Modular Framework for Neural Radiance Field Development}, journal = {arXiv
+preprint arXiv:2302.04264}, year = {2023}, } ``` # Contributors [https://
+contrib.rocks/image?repo=nerfstudio-project/nerfstudio]
```

### Comparing `nerfstudio-0.2.1/README.md` & `nerfstudio-0.2.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,22 @@
+Metadata-Version: 2.1
+Name: nerfstudio
+Version: 0.2.2
+Summary: All-in-one repository for state-of-the-art NeRFs
+License: Apache 2.0
+Project-URL: Documentation, https://docs.nerf.studio
+Classifier: Development Status :: 3 - Alpha
+Classifier: Programming Language :: Python
+Requires-Python: >=3.7.3
+Description-Content-Type: text/markdown
+Provides-Extra: gen
+Provides-Extra: dev
+Provides-Extra: docs
+License-File: LICENSE
+
 <p align="center">
     <!-- community badges -->
     <a href="https://discord.gg/uMbNqcraFc"><img src="https://img.shields.io/badge/Join-Discord-blue.svg"/></a>
     <!-- doc badges -->
     <a href='https://plenoptix-nerfstudio.readthedocs-hosted.com/en/latest/?badge=latest'>
         <img src='https://readthedocs.com/projects/plenoptix-nerfstudio/badge/?version=latest' alt='Documentation Status' />
     </a>
@@ -47,20 +62,22 @@
 
 - [Quickstart](#quickstart)
 - [Learn more](#learn-more)
 - [Supported Features](#supported-features)
 
 # About
 
+_It’s as simple as plug and play with nerfstudio!_
+
 Nerfstudio provides a simple API that allows for a simplified end-to-end process of creating, training, and testing NeRFs.
 The library supports a **more interpretable implementation of NeRFs by modularizing each component.**
 With more modular NeRFs, we hope to create a more user-friendly experience in exploring the technology.
-Nerfstudio is a contributor-friendly repo with the goal of building a community where users can more easily build upon each other's contributions.
 
-It’s as simple as plug and play with nerfstudio!
+This is a contributor-friendly repo with the goal of building a community where users can more easily build upon each other's contributions.
+Nerfstudio initially launched as an opensource project by Berkeley students in [KAIR lab](https://people.eecs.berkeley.edu/~kanazawa/index.html#kair) at [Berkeley AI Research (BAIR)](https://bair.berkeley.edu/) in October 2022 as a part of a research project ([paper](https://arxiv.org/abs/2302.04264)). It is currently developed by Berkeley students and community contributors.
 
 We are committed to providing learning resources to help you understand the basics of (if you're just getting started), and keep up-to-date with (if you're a seasoned veteran) all things NeRF. As researchers, we know just how hard it is to get onboarded with this next-gen technology. So we're here to help with tutorials, documentation, and more!
 
 Have feature requests? Want to add your brand-spankin'-new NeRF model? Have a new dataset? **We welcome any and all [contributions](https://docs.nerf.studio/en/latest/reference/contributing.html)!** Please do not hesitate to reach out to the nerfstudio team with any questions via [Discord](https://discord.gg/uMbNqcraFc).
 
 We hope nerfstudio enables you to build faster :hammer: learn together :books: and contribute to our NeRF community :sparkling_heart:.
 
@@ -216,17 +233,17 @@
 
 Each model contains many parameters that can be changed, too many to list here. Use the `--help` command to see the full list of configuration options.
 
 ```bash
 ns-train nerfacto --help
 ```
 
-### Tensorboard / WandB
+### Tensorboard / WandB / Viewer
 
-We support three different methods to track training progress, using the viewer, [tensorboard](https://www.tensorflow.org/tensorboard), and [Weights and Biases](https://wandb.ai/site). You can specify which visualizer to use by appending `--vis {viewer, tensorboard, wandb}` to the training command. Note that only one may be used at a time. Additionally the viewer only works for methods that are fast (ie. nerfacto, instant-ngp), for slower methods like NeRF, use the other loggers.
+We support three different methods to track training progress, using the viewer, [tensorboard](https://www.tensorflow.org/tensorboard), and [Weights and Biases](https://wandb.ai/site). You can specify which visualizer to use by appending `--vis {viewer, tensorboard, wandb, viewer+wandb, viewer+tensorboard}` to the training command. Simultaneously utilizing the viewer alongside wandb or tensorboard may cause stuttering issues during evaluation steps. The viewer only works for methods that are fast (ie. nerfacto, instant-ngp), for slower methods like NeRF, use the other loggers.
 
 # Learn More
 
 And that's it for getting started with the basics of nerfstudio.
 
 If you're interested in learning more on how to create your own pipelines, develop with the viewer, run benchmarks, and more, please check out some of the quicklinks below or visit our [documentation](https://docs.nerf.studio/en/latest/) directly.
```

#### html2text {}

```diff
@@ -1,26 +1,37 @@
+Metadata-Version: 2.1 Name: nerfstudio Version: 0.2.2 Summary: All-in-one
+repository for state-of-the-art NeRFs License: Apache 2.0 Project-URL:
+Documentation, https://docs.nerf.studio Classifier: Development Status :: 3 -
+Alpha Classifier: Programming Language :: Python Requires-Python: >=3.7.3
+Description-Content-Type: text/markdown Provides-Extra: gen Provides-Extra: dev
+Provides-Extra: docs License-File: LICENSE
  [https://img.shields.io/badge/Join-Discord-blue.svg]  [Documentation_Status]
         [PyPI_version]  [Test_Status] [Viewer_build_Status]  [License]
                                  [nerfstudio]
 
                    A collaboration friendly studio for NeRFs
                        [documentation] [viewer] [colab]
 [https://user-images.githubusercontent.com/3310961/194017985-ade69503-9d68-
 46a2-b518-2db1a012f090.gif] [https://user-images.githubusercontent.com/3310961/
 194020648-7e5f380c-15ca-461d-8c1c-20beb586defe.gif] - [Quickstart](#quickstart)
 - [Learn more](#learn-more) - [Supported Features](#supported-features) # About
-Nerfstudio provides a simple API that allows for a simplified end-to-end
-process of creating, training, and testing NeRFs. The library supports a **more
-interpretable implementation of NeRFs by modularizing each component.** With
-more modular NeRFs, we hope to create a more user-friendly experience in
-exploring the technology. Nerfstudio is a contributor-friendly repo with the
-goal of building a community where users can more easily build upon each
-other's contributions. Itâs as simple as plug and play with nerfstudio! We
-are committed to providing learning resources to help you understand the basics
-of (if you're just getting started), and keep up-to-date with (if you're a
+_Itâs as simple as plug and play with nerfstudio!_ Nerfstudio provides a
+simple API that allows for a simplified end-to-end process of creating,
+training, and testing NeRFs. The library supports a **more interpretable
+implementation of NeRFs by modularizing each component.** With more modular
+NeRFs, we hope to create a more user-friendly experience in exploring the
+technology. This is a contributor-friendly repo with the goal of building a
+community where users can more easily build upon each other's contributions.
+Nerfstudio initially launched as an opensource project by Berkeley students in
+[KAIR lab](https://people.eecs.berkeley.edu/~kanazawa/index.html#kair) at
+[Berkeley AI Research (BAIR)](https://bair.berkeley.edu/) in October 2022 as a
+part of a research project ([paper](https://arxiv.org/abs/2302.04264)). It is
+currently developed by Berkeley students and community contributors. We are
+committed to providing learning resources to help you understand the basics of
+(if you're just getting started), and keep up-to-date with (if you're a
 seasoned veteran) all things NeRF. As researchers, we know just how hard it is
 to get onboarded with this next-gen technology. So we're here to help with
 tutorials, documentation, and more! Have feature requests? Want to add your
 brand-spankin'-new NeRF model? Have a new dataset? **We welcome any and all
 [contributions](https://docs.nerf.studio/en/latest/reference/
 contributing.html)!** Please do not hesitate to reach out to the nerfstudio
 team with any questions via [Discord](https://discord.gg/uMbNqcraFc). We hope
@@ -119,68 +130,69 @@
 Poses | ð | ## 5. Advanced Options ### Training models other than nerfacto
 We provide other models than nerfacto, for example if you want to train the
 original nerf model, use the following command ```bash ns-train vanilla-nerf --
 data DATA_PATH ``` For a full list of included models run `ns-train --help`.
 ### Modify Configuration Each model contains many parameters that can be
 changed, too many to list here. Use the `--help` command to see the full list
 of configuration options. ```bash ns-train nerfacto --help ``` ### Tensorboard
-/ WandB We support three different methods to track training progress, using
-the viewer, [tensorboard](https://www.tensorflow.org/tensorboard), and [Weights
-and Biases](https://wandb.ai/site). You can specify which visualizer to use by
-appending `--vis {viewer, tensorboard, wandb}` to the training command. Note
-that only one may be used at a time. Additionally the viewer only works for
-methods that are fast (ie. nerfacto, instant-ngp), for slower methods like
-NeRF, use the other loggers. # Learn More And that's it for getting started
-with the basics of nerfstudio. If you're interested in learning more on how to
-create your own pipelines, develop with the viewer, run benchmarks, and more,
-please check out some of the quicklinks below or visit our [documentation]
-(https://docs.nerf.studio/en/latest/) directly. | Section | Description | | ---
+/ WandB / Viewer We support three different methods to track training progress,
+using the viewer, [tensorboard](https://www.tensorflow.org/tensorboard), and
+[Weights and Biases](https://wandb.ai/site). You can specify which visualizer
+to use by appending `--vis {viewer, tensorboard, wandb, viewer+wandb,
+viewer+tensorboard}` to the training command. Simultaneously utilizing the
+viewer alongside wandb or tensorboard may cause stuttering issues during
+evaluation steps. The viewer only works for methods that are fast (ie.
+nerfacto, instant-ngp), for slower methods like NeRF, use the other loggers. #
+Learn More And that's it for getting started with the basics of nerfstudio. If
+you're interested in learning more on how to create your own pipelines, develop
+with the viewer, run benchmarks, and more, please check out some of the
+quicklinks below or visit our [documentation](https://docs.nerf.studio/en/
+latest/) directly. | Section | Description | | --------------------------------
+------------------------------------------------------------------ | ----------
 -------------------------------------------------------------------------------
----------------- | ------------------------------------------------------------
--------------------------------------- | | [Documentation](https://
-docs.nerf.studio/en/latest/) | Full API documentation and tutorials | |
-[Viewer](https://viewer.nerf.studio/) | Home page for our web viewer | | ð
-**Educational** | | [Model Descriptions](https://docs.nerf.studio/en/latest/
-nerfology/methods/index.html) | Description of all the models supported by
-nerfstudio and explanations of component parts. | | [Component Descriptions]
-(https://docs.nerf.studio/en/latest/nerfology/model_components/index.html) |
-Interactive notebooks that explain notable/commonly used modules in various
-models. | | ð **Tutorials** | | [Getting Started](https://docs.nerf.studio/
-en/latest/quickstart/installation.html) | A more in-depth guide on how to get
-started with nerfstudio from installation to contributing. | | [Using the
-Viewer](https://docs.nerf.studio/en/latest/quickstart/viewer_quickstart.html) |
-A quick demo video on how to navigate the viewer. | | [Using Record3D](https://
-www.youtube.com/watch?v=XwKq7qDQCQk) | Demo video on how to run nerfstudio
-without using COLMAP. | | ð» **For Developers** | | [Creating pipelines]
-(https://docs.nerf.studio/en/latest/developer_guides/pipelines/index.html) |
-Learn how to easily build new neural rendering pipelines by using and/or
-implementing new modules. | | [Creating datasets](https://docs.nerf.studio/en/
-latest/quickstart/custom_dataset.html) | Have a new dataset? Learn how to run
-it with nerfstudio. | | [Contributing](https://docs.nerf.studio/en/latest/
-reference/contributing.html) | Walk-through for how you can start contributing
-now. | | ð **Community** | | [Discord](https://discord.gg/uMbNqcraFc) | Join
-our community to discuss more. We would love to hear from you! | | [Twitter]
-(https://twitter.com/nerfstudioteam) | Follow us on Twitter @nerfstudioteam to
-see cool updates and announcements | # Supported Features We provide the
-following support structures to make life easier for getting started with
-NeRFs. **If you are looking for a feature that is not currently supported,
-please do not hesitate to contact the Nerfstudio Team on [Discord](https://
-discord.gg/uMbNqcraFc)!** - :mag_right: Web-based visualizer that allows you
-to: - Visualize training in real-time + interact with the scene - Create and
-render out scenes with custom camera trajectories - View different output types
-- And more! - :pencil2: Support for multiple logging interfaces (Tensorboard,
-Wandb), code profiling, and other built-in debugging tools - :
-chart_with_upwards_trend: Easy-to-use benchmarking scripts on the Blender
-dataset - :iphone: Full pipeline support (w/ Colmap, Polycam, or Record3D) for
-going from a video on your phone to a full 3D render. # Built On [tyro_logo] -
-Easy-to-use config system - Developed by [Brent Yi](https://brentyi.com/) [tyro
-logo] - Library for accelerating NeRF renders - Developed by [Ruilong Li]
-(https://www.liruilong.cn/) # Citation You can find a paper writeup of the
-framework on [arXiv](https://arxiv.org/abs/2302.04264). If you use this library
-or find the documentation useful for your research, please consider citing: ```
-@article{nerfstudio, author = {Tancik, Matthew and Weber, Ethan and Ng, Evonne
-and Li, Ruilong and Yi, Brent and Kerr, Justin and Wang, Terrance and
-Kristoffersen, Alexander and Austin, Jake and Salahi, Kamyar and Ahuja, Abhik
-and McAllister, David and Kanazawa, Angjoo}, title = {Nerfstudio: A Modular
-Framework for Neural Radiance Field Development}, journal = {arXiv preprint
-arXiv:2302.04264}, year = {2023}, } ``` # Contributors [https://contrib.rocks/
-image?repo=nerfstudio-project/nerfstudio]
+--------- | | [Documentation](https://docs.nerf.studio/en/latest/) | Full API
+documentation and tutorials | | [Viewer](https://viewer.nerf.studio/) | Home
+page for our web viewer | | ð **Educational** | | [Model Descriptions]
+(https://docs.nerf.studio/en/latest/nerfology/methods/index.html) | Description
+of all the models supported by nerfstudio and explanations of component parts.
+| | [Component Descriptions](https://docs.nerf.studio/en/latest/nerfology/
+model_components/index.html) | Interactive notebooks that explain notable/
+commonly used modules in various models. | | ð **Tutorials** | | [Getting
+Started](https://docs.nerf.studio/en/latest/quickstart/installation.html) | A
+more in-depth guide on how to get started with nerfstudio from installation to
+contributing. | | [Using the Viewer](https://docs.nerf.studio/en/latest/
+quickstart/viewer_quickstart.html) | A quick demo video on how to navigate the
+viewer. | | [Using Record3D](https://www.youtube.com/watch?v=XwKq7qDQCQk) |
+Demo video on how to run nerfstudio without using COLMAP. | | ð» **For
+Developers** | | [Creating pipelines](https://docs.nerf.studio/en/latest/
+developer_guides/pipelines/index.html) | Learn how to easily build new neural
+rendering pipelines by using and/or implementing new modules. | | [Creating
+datasets](https://docs.nerf.studio/en/latest/quickstart/custom_dataset.html) |
+Have a new dataset? Learn how to run it with nerfstudio. | | [Contributing]
+(https://docs.nerf.studio/en/latest/reference/contributing.html) | Walk-through
+for how you can start contributing now. | | ð **Community** | | [Discord]
+(https://discord.gg/uMbNqcraFc) | Join our community to discuss more. We would
+love to hear from you! | | [Twitter](https://twitter.com/nerfstudioteam) |
+Follow us on Twitter @nerfstudioteam to see cool updates and announcements | #
+Supported Features We provide the following support structures to make life
+easier for getting started with NeRFs. **If you are looking for a feature that
+is not currently supported, please do not hesitate to contact the Nerfstudio
+Team on [Discord](https://discord.gg/uMbNqcraFc)!** - :mag_right: Web-based
+visualizer that allows you to: - Visualize training in real-time + interact
+with the scene - Create and render out scenes with custom camera trajectories -
+View different output types - And more! - :pencil2: Support for multiple
+logging interfaces (Tensorboard, Wandb), code profiling, and other built-in
+debugging tools - :chart_with_upwards_trend: Easy-to-use benchmarking scripts
+on the Blender dataset - :iphone: Full pipeline support (w/ Colmap, Polycam, or
+Record3D) for going from a video on your phone to a full 3D render. # Built On
+[tyro_logo] - Easy-to-use config system - Developed by [Brent Yi](https://
+brentyi.com/) [tyro_logo] - Library for accelerating NeRF renders - Developed
+by [Ruilong Li](https://www.liruilong.cn/) # Citation You can find a paper
+writeup of the framework on [arXiv](https://arxiv.org/abs/2302.04264). If you
+use this library or find the documentation useful for your research, please
+consider citing: ``` @article{nerfstudio, author = {Tancik, Matthew and Weber,
+Ethan and Ng, Evonne and Li, Ruilong and Yi, Brent and Kerr, Justin and Wang,
+Terrance and Kristoffersen, Alexander and Austin, Jake and Salahi, Kamyar and
+Ahuja, Abhik and McAllister, David and Kanazawa, Angjoo}, title = {Nerfstudio:
+A Modular Framework for Neural Radiance Field Development}, journal = {arXiv
+preprint arXiv:2302.04264}, year = {2023}, } ``` # Contributors [https://
+contrib.rocks/image?repo=nerfstudio-project/nerfstudio]
```

### Comparing `nerfstudio-0.2.1/nerfstudio/__init__.py` & `nerfstudio-0.2.2/nerfstudio/__init__.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-0.2.1/nerfstudio/cameras/__init__.py` & `nerfstudio-0.2.2/nerfstudio/cameras/__init__.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-0.2.1/nerfstudio/cameras/camera_optimizers.py` & `nerfstudio-0.2.2/nerfstudio/cameras/camera_optimizers.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-0.2.1/nerfstudio/cameras/camera_paths.py` & `nerfstudio-0.2.2/nerfstudio/cameras/camera_paths.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-0.2.1/nerfstudio/cameras/camera_utils.py` & `nerfstudio-0.2.2/nerfstudio/cameras/camera_utils.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-0.2.1/nerfstudio/cameras/cameras.py` & `nerfstudio-0.2.2/nerfstudio/cameras/cameras.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,14 @@
 # limitations under the License.
 
 """
 Camera Models
 """
 import base64
 import math
-import os
 from dataclasses import dataclass
 from enum import Enum, auto
 from typing import Dict, List, Optional, Tuple, Union
 
 import cv2
 import torch
 import torchvision
@@ -29,15 +28,14 @@
 from torchtyping import TensorType
 
 import nerfstudio.utils.math
 import nerfstudio.utils.poses as pose_utils
 from nerfstudio.cameras import camera_utils
 from nerfstudio.cameras.rays import RayBundle
 from nerfstudio.data.scene_box import SceneBox
-from nerfstudio.utils.misc import strtobool
 from nerfstudio.utils.tensor_dataclass import TensorDataclass
 
 TORCH_DEVICE = Union[torch.device, str]  # pylint: disable=invalid-name
 
 
 class CameraType(Enum):
     """Supported camera types."""
@@ -146,16 +144,14 @@
         self.camera_type = self._init_get_camera_type(camera_type)
         self.times = self._init_get_times(times)
 
         self.metadata = metadata
 
         self.__post_init__()  # This will do the dataclass post_init and broadcast all the tensors
 
-        self._use_nerfacc = strtobool(os.environ.get("INTERSECT_WITH_NERFACC", "TRUE"))
-
     def _init_get_fc_xy(self, fc_xy: Union[float, torch.Tensor], name: str) -> torch.Tensor:
         """
         Parses the input focal length / principle point x or y and returns a tensor of the correct shape
 
         Only needs to make sure that we a 1 in the last dimension if it is a tensor. If it is a float, we
         just need to make it into a tensor and it will be broadcasted later in the __post_init__ function.
 
@@ -629,15 +625,15 @@
             elif distortion_params_delta is not None:
                 distortion_params = distortion_params_delta
 
             # Do not apply distortion for equirectangular images
             if distortion_params is not None:
                 mask = (self.camera_type[true_indices] != CameraType.EQUIRECTANGULAR.value).squeeze(-1)  # (num_rays)
                 coord_mask = torch.stack([mask, mask, mask], dim=0)
-                if mask.any():
+                if mask.any() and (distortion_params != 0).any():
                     coord_stack[coord_mask, :] = camera_utils.radial_and_tangential_undistort(
                         coord_stack[coord_mask, :].reshape(3, -1, 2),
                         distortion_params[mask, :],
                     ).reshape(-1, 2)
 
         # Make sure after we have undistorted our images, the shapes are still correct
         assert coord_stack.shape == (3,) + num_rays_shape + (2,)
```

### Comparing `nerfstudio-0.2.1/nerfstudio/cameras/lie_groups.py` & `nerfstudio-0.2.2/nerfstudio/cameras/lie_groups.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-0.2.1/nerfstudio/cameras/rays.py` & `nerfstudio-0.2.2/nerfstudio/cameras/rays.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-0.2.1/nerfstudio/configs/__init__.py` & `nerfstudio-0.2.2/nerfstudio/configs/__init__.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-0.2.1/nerfstudio/configs/base_config.py` & `nerfstudio-0.2.2/nerfstudio/configs/base_config.py`

 * *Files 2% similar despite different names*

```diff
@@ -133,14 +133,16 @@
 
     relative_log_filename: str = "viewer_log_filename.txt"
     """Filename to use for the log file."""
     websocket_port: Optional[int] = None
     """The websocket port to connect to. If None, find an available port."""
     websocket_port_default: int = 7007
     """The default websocket port to connect to if websocket_port is not specified"""
+    websocket_host: str = "0.0.0.0"
+    """The host address to bind the websocket server to."""
     num_rays_per_chunk: int = 32768
     """number of rays per chunk to render with viewer"""
     max_num_display_images: int = 512
     """Maximum number of training images to display in the viewer, to avoid lag. This does not change which images are
     actually used in training/evaluation. If -1, display all."""
     quit_on_train_completion: bool = False
     """Whether to kill the training job when it has completed. Note this will stop rendering in the viewer."""
```

### Comparing `nerfstudio-0.2.1/nerfstudio/configs/config_utils.py` & `nerfstudio-0.2.2/nerfstudio/configs/config_utils.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-0.2.1/nerfstudio/configs/experiment_config.py` & `nerfstudio-0.2.2/nerfstudio/configs/experiment_config.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-0.2.1/nerfstudio/configs/method_configs.py` & `nerfstudio-0.2.2/nerfstudio/configs/method_configs.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,14 @@
 """
 
 from __future__ import annotations
 
 from typing import Dict
 
 import tyro
-from nerfacc import ContractionType
 
 from nerfstudio.cameras.camera_optimizers import CameraOptimizerConfig
 from nerfstudio.configs.base_config import ViewerConfig
 from nerfstudio.data.datamanagers.base_datamanager import VanillaDataManagerConfig
 from nerfstudio.data.datamanagers.depth_datamanager import DepthDataManagerConfig
 from nerfstudio.data.datamanagers.sdf_datamanager import SDFDataManagerConfig
 from nerfstudio.data.datamanagers.semantic_datamanager import SemanticDataManagerConfig
@@ -231,52 +230,57 @@
 method_configs["instant-ngp"] = TrainerConfig(
     method_name="instant-ngp",
     steps_per_eval_batch=500,
     steps_per_save=2000,
     max_num_iterations=30000,
     mixed_precision=True,
     pipeline=DynamicBatchPipelineConfig(
-        datamanager=VanillaDataManagerConfig(dataparser=NerfstudioDataParserConfig(), train_num_rays_per_batch=8192),
+        datamanager=VanillaDataManagerConfig(
+            dataparser=NerfstudioDataParserConfig(),
+            train_num_rays_per_batch=4096,
+            eval_num_rays_per_batch=4096,
+        ),
         model=InstantNGPModelConfig(eval_num_rays_per_chunk=8192),
     ),
     optimizers={
         "fields": {
             "optimizer": AdamOptimizerConfig(lr=1e-2, eps=1e-15),
-            "scheduler": None,
+            "scheduler": ExponentialDecaySchedulerConfig(lr_final=0.0001, max_steps=200000),
         }
     },
-    viewer=ViewerConfig(num_rays_per_chunk=64000),
+    viewer=ViewerConfig(num_rays_per_chunk=1 << 12),
     vis="viewer",
 )
 
 
 method_configs["instant-ngp-bounded"] = TrainerConfig(
     method_name="instant-ngp-bounded",
     steps_per_eval_batch=500,
     steps_per_save=2000,
     max_num_iterations=30000,
     mixed_precision=True,
     pipeline=DynamicBatchPipelineConfig(
         datamanager=VanillaDataManagerConfig(dataparser=InstantNGPDataParserConfig(), train_num_rays_per_batch=8192),
         model=InstantNGPModelConfig(
             eval_num_rays_per_chunk=8192,
-            contraction_type=ContractionType.AABB,
-            render_step_size=0.001,
-            max_num_samples_per_ray=48,
+            grid_levels=1,
+            alpha_thre=0.0,
+            cone_angle=0.0,
+            disable_scene_contraction=True,
             near_plane=0.01,
             background_color="black",
         ),
     ),
     optimizers={
         "fields": {
             "optimizer": AdamOptimizerConfig(lr=1e-2, eps=1e-15),
-            "scheduler": None,
+            "scheduler": ExponentialDecaySchedulerConfig(lr_final=0.0001, max_steps=200000),
         }
     },
-    viewer=ViewerConfig(num_rays_per_chunk=64000),
+    viewer=ViewerConfig(num_rays_per_chunk=1 << 12),
     vis="viewer",
 )
 
 
 method_configs["mipnerf"] = TrainerConfig(
     method_name="mipnerf",
     pipeline=VanillaPipelineConfig(
@@ -466,17 +470,18 @@
     steps_per_save=2000,
     max_num_iterations=30000,
     mixed_precision=True,
     pipeline=DynamicBatchPipelineConfig(
         datamanager=DepthDataManagerConfig(dataparser=DycheckDataParserConfig(), train_num_rays_per_batch=8192),
         model=NerfplayerNGPModelConfig(
             eval_num_rays_per_chunk=8192,
-            contraction_type=ContractionType.AABB,
+            grid_levels=1,
+            alpha_thre=0.0,
             render_step_size=0.001,
-            max_num_samples_per_ray=48,
+            disable_scene_contraction=True,
             near_plane=0.01,
         ),
     ),
     optimizers={
         "fields": {
             "optimizer": AdamOptimizerConfig(lr=1e-2, eps=1e-15),
             "scheduler": None,
```

### Comparing `nerfstudio-0.2.1/nerfstudio/data/__init__.py` & `nerfstudio-0.2.2/nerfstudio/data/__init__.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-0.2.1/nerfstudio/data/datamanagers/__init__.py` & `nerfstudio-0.2.2/nerfstudio/data/datamanagers/__init__.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-0.2.1/nerfstudio/data/datamanagers/base_datamanager.py` & `nerfstudio-0.2.2/nerfstudio/data/datamanagers/base_datamanager.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-0.2.1/nerfstudio/data/datamanagers/depth_datamanager.py` & `nerfstudio-0.2.2/nerfstudio/data/datamanagers/depth_datamanager.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-0.2.1/nerfstudio/data/datamanagers/sdf_datamanager.py` & `nerfstudio-0.2.2/nerfstudio/data/datamanagers/sdf_datamanager.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-0.2.1/nerfstudio/data/datamanagers/semantic_datamanager.py` & `nerfstudio-0.2.2/nerfstudio/data/datamanagers/semantic_datamanager.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-0.2.1/nerfstudio/data/dataparsers/__init__.py` & `nerfstudio-0.2.2/nerfstudio/data/dataparsers/__init__.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-0.2.1/nerfstudio/data/dataparsers/arkitscenes_dataparser.py` & `nerfstudio-0.2.2/nerfstudio/data/dataparsers/arkitscenes_dataparser.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-0.2.1/nerfstudio/data/dataparsers/base_dataparser.py` & `nerfstudio-0.2.2/nerfstudio/data/dataparsers/base_dataparser.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-0.2.1/nerfstudio/data/dataparsers/blender_dataparser.py` & `nerfstudio-0.2.2/nerfstudio/data/dataparsers/blender_dataparser.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-0.2.1/nerfstudio/data/dataparsers/dnerf_dataparser.py` & `nerfstudio-0.2.2/nerfstudio/data/dataparsers/dnerf_dataparser.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-0.2.1/nerfstudio/data/dataparsers/dycheck_dataparser.py` & `nerfstudio-0.2.2/nerfstudio/data/dataparsers/dycheck_dataparser.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-0.2.1/nerfstudio/data/dataparsers/instant_ngp_dataparser.py` & `nerfstudio-0.2.2/nerfstudio/data/dataparsers/instant_ngp_dataparser.py`

 * *Files 9% similar despite different names*

```diff
@@ -61,14 +61,15 @@
             meta = load_from_json(self.config.data)
             data_dir = self.config.data.parent
         else:
             meta = load_from_json(self.config.data / "transforms.json")
             data_dir = self.config.data
 
         image_filenames = []
+        mask_filenames = []
         poses = []
         num_skipped_image_filenames = 0
         for frame in meta["frames"]:
             fname = data_dir / Path(frame["file_path"])
             # search for png file
             if not fname.exists():
                 fname = data_dir / Path(frame["file_path"] + ".png")
@@ -83,14 +84,17 @@
                     if "h" in meta:
                         meta_h = meta["h"]
                         assert meta_h == h, f"height of image dont not correspond metadata {h} != {meta_h}"
                     else:
                         meta["h"] = h
                 image_filenames.append(fname)
                 poses.append(np.array(frame["transform_matrix"]))
+                if "mask_path" in frame:
+                    mask_fname = data_dir / Path(frame["mask_path"])
+                    mask_filenames.append(mask_fname)
         if num_skipped_image_filenames >= 0:
             CONSOLE.print(f"Skipping {num_skipped_image_filenames} files in dataset split {split}.")
         assert (
             len(image_filenames) != 0
         ), """
         No image files found. 
         You should check the file_paths in the transforms.json file to make sure they are correct.
@@ -140,14 +144,15 @@
         )
 
         # TODO(ethan): add alpha background color
         dataparser_outputs = DataparserOutputs(
             image_filenames=image_filenames,
             cameras=cameras,
             scene_box=scene_box,
+            mask_filenames=mask_filenames if len(mask_filenames) > 0 else None,
             dataparser_scale=self.config.scene_scale,
         )
 
         return dataparser_outputs
 
     @classmethod
     def get_focal_lengths(cls, meta: Dict) -> Tuple[float, float]:
```

### Comparing `nerfstudio-0.2.1/nerfstudio/data/dataparsers/minimal_dataparser.py` & `nerfstudio-0.2.2/nerfstudio/data/dataparsers/minimal_dataparser.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-0.2.1/nerfstudio/data/dataparsers/nerfosr_dataparser.py` & `nerfstudio-0.2.2/nerfstudio/data/dataparsers/nerfosr_dataparser.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-0.2.1/nerfstudio/data/dataparsers/nerfstudio_dataparser.py` & `nerfstudio-0.2.2/nerfstudio/data/dataparsers/nerfstudio_dataparser.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-0.2.1/nerfstudio/data/dataparsers/nuscenes_dataparser.py` & `nerfstudio-0.2.2/nerfstudio/data/dataparsers/nuscenes_dataparser.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-0.2.1/nerfstudio/data/dataparsers/phototourism_dataparser.py` & `nerfstudio-0.2.2/nerfstudio/data/dataparsers/phototourism_dataparser.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-0.2.1/nerfstudio/data/dataparsers/scannet_dataparser.py` & `nerfstudio-0.2.2/nerfstudio/data/dataparsers/scannet_dataparser.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-0.2.1/nerfstudio/data/dataparsers/sdfstudio_dataparser.py` & `nerfstudio-0.2.2/nerfstudio/data/dataparsers/sdfstudio_dataparser.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-0.2.1/nerfstudio/data/dataparsers/sitcoms3d_dataparser.py` & `nerfstudio-0.2.2/nerfstudio/data/dataparsers/sitcoms3d_dataparser.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-0.2.1/nerfstudio/data/datasets/__init__.py` & `nerfstudio-0.2.2/nerfstudio/data/datasets/__init__.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-0.2.1/nerfstudio/data/datasets/base_dataset.py` & `nerfstudio-0.2.2/nerfstudio/data/datasets/base_dataset.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-0.2.1/nerfstudio/data/datasets/depth_dataset.py` & `nerfstudio-0.2.2/nerfstudio/data/datasets/depth_dataset.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-0.2.1/nerfstudio/data/datasets/sdf_dataset.py` & `nerfstudio-0.2.2/nerfstudio/data/datasets/sdf_dataset.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-0.2.1/nerfstudio/data/datasets/semantic_dataset.py` & `nerfstudio-0.2.2/nerfstudio/data/datasets/semantic_dataset.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-0.2.1/nerfstudio/data/pixel_samplers.py` & `nerfstudio-0.2.2/nerfstudio/data/pixel_samplers.py`

 * *Files 2% similar despite different names*

```diff
@@ -92,19 +92,20 @@
             indices = self.sample_method(
                 num_rays_per_batch, num_images, image_height, image_width, mask=batch["mask"], device=device
             )
         else:
             indices = self.sample_method(num_rays_per_batch, num_images, image_height, image_width, device=device)
 
         c, y, x = (i.flatten() for i in torch.split(indices, 1, dim=-1))
+        c, y, x = c.cpu(), y.cpu(), x.cpu()
         collated_batch = {
             key: value[c, y, x] for key, value in batch.items() if key != "image_idx" and value is not None
         }
 
-        assert collated_batch["image"].shape == (num_rays_per_batch, 3), collated_batch["image"].shape
+        assert collated_batch["image"].shape[0] == num_rays_per_batch
 
         # Needed to correct the random indices to their actual camera idx locations.
         indices[:, 0] = batch["image_idx"][c]
         collated_batch["indices"] = indices  # with the abs camera indices
 
         if keep_full_image:
             collated_batch["full_image"] = batch["image"]
@@ -167,15 +168,15 @@
             key: value[c, y, x]
             for key, value in batch.items()
             if key != "image_idx" and key != "image" and key != "mask" and value is not None
         }
 
         collated_batch["image"] = torch.cat(all_images, dim=0)
 
-        assert collated_batch["image"].shape == (num_rays_per_batch, 3), collated_batch["image"].shape
+        assert collated_batch["image"].shape[0] == num_rays_per_batch
 
         # Needed to correct the random indices to their actual camera idx locations.
         indices[:, 0] = batch["image_idx"][c]
         collated_batch["indices"] = indices  # with the abs camera indices
 
         if keep_full_image:
             collated_batch["full_image"] = batch["image"]
```

### Comparing `nerfstudio-0.2.1/nerfstudio/data/scene_box.py` & `nerfstudio-0.2.2/nerfstudio/data/scene_box.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-0.2.1/nerfstudio/data/utils/__init__.py` & `nerfstudio-0.2.2/nerfstudio/data/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-0.2.1/nerfstudio/data/utils/colmap_parsing_utils.py` & `nerfstudio-0.2.2/nerfstudio/data/utils/colmap_parsing_utils.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-0.2.1/nerfstudio/data/utils/data_utils.py` & `nerfstudio-0.2.2/nerfstudio/data/utils/data_utils.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-0.2.1/nerfstudio/data/utils/dataloaders.py` & `nerfstudio-0.2.2/nerfstudio/data/utils/dataloaders.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-0.2.1/nerfstudio/data/utils/nerfstudio_collate.py` & `nerfstudio-0.2.2/nerfstudio/data/utils/nerfstudio_collate.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-0.2.1/nerfstudio/engine/__init__.py` & `nerfstudio-0.2.2/nerfstudio/engine/__init__.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-0.2.1/nerfstudio/engine/callbacks.py` & `nerfstudio-0.2.2/nerfstudio/engine/callbacks.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-0.2.1/nerfstudio/engine/optimizers.py` & `nerfstudio-0.2.2/nerfstudio/engine/optimizers.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-0.2.1/nerfstudio/engine/schedulers.py` & `nerfstudio-0.2.2/nerfstudio/engine/schedulers.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-0.2.1/nerfstudio/engine/trainer.py` & `nerfstudio-0.2.2/nerfstudio/engine/trainer.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,15 +23,18 @@
 import time
 from dataclasses import dataclass, field
 from pathlib import Path
 from threading import Lock
 from typing import Dict, List, Optional, Tuple, Type, Union
 
 import torch
+from rich import box, style
 from rich.console import Console
+from rich.panel import Panel
+from rich.table import Table
 from torch.cuda.amp.grad_scaler import GradScaler
 from typing_extensions import Literal
 
 from nerfstudio.configs.experiment_config import ExperimentConfig
 from nerfstudio.engine.callbacks import (
     TrainingCallback,
     TrainingCallbackAttributes,
@@ -71,14 +74,16 @@
     """Number of steps between single eval images."""
     steps_per_eval_all_images: int = 25000
     """Number of steps between eval all images."""
     max_num_iterations: int = 1000000
     """Maximum number of iterations to run."""
     mixed_precision: bool = False
     """Whether or not to use mixed precision for training."""
+    use_grad_scaler: bool = False
+    """Use gradient scaler even if the automatic mixed precision is disabled."""
     save_only_latest_checkpoint: bool = True
     """Whether to only save the latest checkpoint or all checkpoints."""
     # optional parameters if we want to resume training
     load_dir: Optional[Path] = None
     """Optionally specify a pre-trained model directory to load from."""
     load_step: Optional[int] = None
     """Optionally specify model step to load from; if none, will find most recent model in load_dir."""
@@ -114,21 +119,23 @@
     def __init__(self, config: TrainerConfig, local_rank: int = 0, world_size: int = 1) -> None:
         self.train_lock = Lock()
         self.config = config
         self.local_rank = local_rank
         self.world_size = world_size
         self.device: TORCH_DEVICE = "cpu" if world_size == 0 else f"cuda:{local_rank}"
         self.mixed_precision: bool = self.config.mixed_precision
+        self.use_grad_scaler: bool = self.mixed_precision or self.config.use_grad_scaler
         self.training_state: Literal["training", "paused", "completed"] = "training"
+
         if self.device == "cpu":
             self.mixed_precision = False
             CONSOLE.print("Mixed precision is disabled for CPU training.")
         self._start_step: int = 0
         # optimizers
-        self.grad_scaler = GradScaler(enabled=self.mixed_precision)
+        self.grad_scaler = GradScaler(enabled=self.use_grad_scaler)
 
         self.base_dir: Path = config.get_base_dir()
         # directory to save checkpoints
         self.checkpoint_dir: Path = config.get_checkpoint_dir()
         CONSOLE.log(f"Saving checkpoints to: {self.checkpoint_dir}")
 
         self.viewer_state = None
@@ -273,22 +280,25 @@
 
         # save checkpoint at the end of training
         self.save_checkpoint(step)
 
         # write out any remaining events (e.g., total train time)
         writer.write_out_storage()
 
-        CONSOLE.rule()
-        CONSOLE.print("[bold green]:tada: :tada: :tada: Training Finished :tada: :tada: :tada:", justify="center")
-        if not self.config.viewer.quit_on_train_completion:
-            self.training_state = "completed"
-            self._train_complete_viewer()
-            CONSOLE.print("Use ctrl+c to quit", justify="center")
-            while True:
-                time.sleep(0.01)
+        table = Table(
+            title=None,
+            show_header=False,
+            box=box.MINIMAL,
+            title_style=style.Style(bold=True),
+        )
+        table.add_row("Config File", str(self.config.get_base_dir() / "config.yml"))
+        table.add_row("Checkpoint Directory", str(self.checkpoint_dir))
+        CONSOLE.print(Panel(table, title="[bold][green]:tada: Training Finished :tada:[/bold]", expand=False))
+
+        self._train_complete_viewer()
 
     @check_main_thread
     def _check_viewer_warnings(self) -> None:
         """Helper to print out any warnings regarding the way the viewer/loggers are enabled"""
         if (
             self.config.is_viewer_enabled()
             and not self.config.is_tensorboard_enabled()
@@ -325,19 +335,24 @@
             time.sleep(0.03)  # sleep to allow buffer to reset
             CONSOLE.log("Viewer failed. Continuing training.")
 
     @check_viewer_enabled
     def _train_complete_viewer(self) -> None:
         """Let the viewer know that the training is complete"""
         assert self.viewer_state is not None
+        if not self.config.viewer.quit_on_train_completion:
+            self.training_state = "completed"
         try:
             self.viewer_state.training_complete()
         except RuntimeError:
             time.sleep(0.03)  # sleep to allow buffer to reset
             CONSOLE.log("Viewer failed. Continuing training.")
+        CONSOLE.print("Use ctrl+c to quit", justify="center")
+        while True:
+            time.sleep(0.01)
 
     @check_viewer_enabled
     def _update_viewer_rays_per_sec(self, train_t: TimeWriter, vis_t: TimeWriter, step: int) -> None:
         """Performs update on rays/sec calculation for training
 
         Args:
             train_t: timer object carrying time to execute total training iteration
```

### Comparing `nerfstudio-0.2.1/nerfstudio/exporter/__init__.py` & `nerfstudio-0.2.2/nerfstudio/exporter/__init__.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-0.2.1/nerfstudio/exporter/exporter_utils.py` & `nerfstudio-0.2.2/nerfstudio/exporter/exporter_utils.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-0.2.1/nerfstudio/exporter/marching_cubes.py` & `nerfstudio-0.2.2/nerfstudio/exporter/marching_cubes.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-0.2.1/nerfstudio/exporter/texture_utils.py` & `nerfstudio-0.2.2/nerfstudio/exporter/texture_utils.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-0.2.1/nerfstudio/exporter/tsdf_utils.py` & `nerfstudio-0.2.2/nerfstudio/exporter/tsdf_utils.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-0.2.1/nerfstudio/field_components/__init__.py` & `nerfstudio-0.2.2/nerfstudio/field_components/__init__.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-0.2.1/nerfstudio/field_components/activations.py` & `nerfstudio-0.2.2/nerfstudio/field_components/activations.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-0.2.1/nerfstudio/field_components/base_field_component.py` & `nerfstudio-0.2.2/nerfstudio/field_components/base_field_component.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-0.2.1/nerfstudio/field_components/cuda/__init__.py` & `nerfstudio-0.2.2/nerfstudio/field_components/cuda/__init__.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-0.2.1/nerfstudio/field_components/cuda/_backend.py` & `nerfstudio-0.2.2/nerfstudio/field_components/cuda/_backend.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-0.2.1/nerfstudio/field_components/embedding.py` & `nerfstudio-0.2.2/nerfstudio/field_components/embedding.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-0.2.1/nerfstudio/field_components/encodings.py` & `nerfstudio-0.2.2/nerfstudio/field_components/encodings.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-0.2.1/nerfstudio/field_components/field_heads.py` & `nerfstudio-0.2.2/nerfstudio/field_components/field_heads.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-0.2.1/nerfstudio/field_components/mlp.py` & `nerfstudio-0.2.2/nerfstudio/field_components/mlp.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-0.2.1/nerfstudio/field_components/spatial_distortions.py` & `nerfstudio-0.2.2/nerfstudio/field_components/spatial_distortions.py`

 * *Files 0% similar despite different names*

```diff
@@ -47,15 +47,15 @@
 
             f(x) = \\begin{cases}
                 x & ||x|| \\leq 1 \\\\
                 (2 - \\frac{1}{||x||})(\\frac{x}{||x||}) & ||x|| > 1
             \\end{cases}
 
         If the order is not specified, we use the Frobenius norm, this will contract the space to a sphere of
-        radius 1. If the order is L_inf (order=float("inf")), we will contract the space to a cube of side length 2.
+        radius 2. If the order is L_inf (order=float("inf")), we will contract the space to a cube of side length 4.
         If using voxel based encodings such as the Hash encoder, we recommend using the L_inf norm.
 
         Args:
             order: Order of the norm. Default to the Frobenius norm. Must be set to None for Gaussians.
 
     """
```

### Comparing `nerfstudio-0.2.1/nerfstudio/field_components/temporal_distortions.py` & `nerfstudio-0.2.2/nerfstudio/field_components/temporal_distortions.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-0.2.1/nerfstudio/field_components/temporal_grid.py` & `nerfstudio-0.2.2/nerfstudio/field_components/temporal_grid.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-0.2.1/nerfstudio/fields/__init__.py` & `nerfstudio-0.2.2/nerfstudio/fields/__init__.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-0.2.1/nerfstudio/fields/base_field.py` & `nerfstudio-0.2.2/nerfstudio/fields/base_field.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-0.2.1/nerfstudio/fields/density_fields.py` & `nerfstudio-0.2.2/nerfstudio/fields/density_fields.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-0.2.1/nerfstudio/fields/instant_ngp_field.py` & `nerfstudio-0.2.2/nerfstudio/fields/instant_ngp_field.py`

 * *Files 11% similar despite different names*

```diff
@@ -17,23 +17,26 @@
 """
 
 
 from typing import Dict, Optional, Tuple
 
 import numpy as np
 import torch
-from nerfacc import ContractionType, contract
 from torch.nn.parameter import Parameter
 from torchtyping import TensorType
 
 from nerfstudio.cameras.rays import RaySamples
 from nerfstudio.data.scene_box import SceneBox
 from nerfstudio.field_components.activations import trunc_exp
 from nerfstudio.field_components.embedding import Embedding
 from nerfstudio.field_components.field_heads import FieldHeadNames
+from nerfstudio.field_components.spatial_distortions import (
+    SceneContraction,
+    SpatialDistortion,
+)
 from nerfstudio.fields.base_field import Field, shift_directions_for_tcnn
 
 try:
     import tinycudann as tcnn
 except ImportError:
     # tinycudann module doesn't exist
     pass
@@ -65,34 +68,35 @@
         hidden_dim: int = 64,
         geo_feat_dim: int = 15,
         num_layers_color: int = 3,
         hidden_dim_color: int = 64,
         use_appearance_embedding: Optional[bool] = False,
         num_images: Optional[int] = None,
         appearance_embedding_dim: int = 32,
-        contraction_type: ContractionType = ContractionType.UN_BOUNDED_SPHERE,
         num_levels: int = 16,
         log2_hashmap_size: int = 19,
         max_res: int = 2048,
+        spatial_distortion: Optional[SpatialDistortion] = SceneContraction(),
     ) -> None:
         super().__init__()
 
         self.aabb = Parameter(aabb, requires_grad=False)
         self.geo_feat_dim = geo_feat_dim
-        self.contraction_type = contraction_type
+        self.spatial_distortion = spatial_distortion
 
         self.use_appearance_embedding = use_appearance_embedding
         if use_appearance_embedding:
             assert num_images is not None
             self.appearance_embedding_dim = appearance_embedding_dim
             self.appearance_embedding = Embedding(num_images, appearance_embedding_dim)
 
         # TODO: set this properly based on the aabb
         base_res: int = 16
-        per_level_scale = np.exp((np.log(max_res) - np.log(base_res)) / (num_levels - 1))
+        features_per_level: int = 2
+        growth_factor = np.exp((np.log(max_res) - np.log(base_res)) / (num_levels - 1))
 
         self.direction_encoding = tcnn.Encoding(
             n_input_dims=3,
             encoding_config={
                 "otype": "SphericalHarmonics",
                 "degree": 4,
             },
@@ -100,18 +104,18 @@
 
         self.mlp_base = tcnn.NetworkWithInputEncoding(
             n_input_dims=3,
             n_output_dims=1 + self.geo_feat_dim,
             encoding_config={
                 "otype": "HashGrid",
                 "n_levels": num_levels,
-                "n_features_per_level": 2,
+                "n_features_per_level": features_per_level,
                 "log2_hashmap_size": log2_hashmap_size,
                 "base_resolution": base_res,
-                "per_level_scale": per_level_scale,
+                "per_level_scale": growth_factor,
             },
             network_config={
                 "otype": "FullyFusedMLP",
                 "activation": "ReLU",
                 "output_activation": "None",
                 "n_neurons": hidden_dim,
                 "n_hidden_layers": num_layers - 1,
@@ -130,39 +134,44 @@
                 "output_activation": "Sigmoid",
                 "n_neurons": hidden_dim_color,
                 "n_hidden_layers": num_layers_color - 1,
             },
         )
 
     def get_density(self, ray_samples: RaySamples) -> Tuple[TensorType, TensorType]:
-        positions = ray_samples.frustums.get_positions()
+        if self.spatial_distortion is not None:
+            positions = ray_samples.frustums.get_positions()
+            positions = self.spatial_distortion(positions)
+            positions = (positions + 2.0) / 4.0
+        else:
+            positions = SceneBox.get_normalized_positions(ray_samples.frustums.get_positions(), self.aabb)
+        # Make sure the tcnn gets inputs between 0 and 1.
+        selector = ((positions > 0.0) & (positions < 1.0)).all(dim=-1)
+        positions = positions * selector[..., None]
         positions_flat = positions.view(-1, 3)
-        positions_flat = contract(x=positions_flat, roi=self.aabb, type=self.contraction_type)
 
         h = self.mlp_base(positions_flat).view(*ray_samples.frustums.shape, -1)
         density_before_activation, base_mlp_out = torch.split(h, [1, self.geo_feat_dim], dim=-1)
 
         # Rectifying the density with an exponential is much more stable than a ReLU or
         # softplus, because it enables high post-activation (float32) density outputs
         # from smaller internal (float16) parameters.
         density = trunc_exp(density_before_activation.to(positions))
+        density = density * selector[..., None]
         return density, base_mlp_out
 
     def get_outputs(
         self, ray_samples: RaySamples, density_embedding: Optional[TensorType] = None
     ) -> Dict[FieldHeadNames, TensorType]:
+        assert density_embedding is not None
         directions = shift_directions_for_tcnn(ray_samples.frustums.directions)
         directions_flat = directions.view(-1, 3)
-
         d = self.direction_encoding(directions_flat)
-        if density_embedding is None:
-            positions = SceneBox.get_normalized_positions(ray_samples.frustums.get_positions(), self.aabb)
-            h = torch.cat([d, positions.view(-1, 3)], dim=-1)
-        else:
-            h = torch.cat([d, density_embedding.view(-1, self.geo_feat_dim)], dim=-1)
+
+        h = torch.cat([d, density_embedding.view(-1, self.geo_feat_dim)], dim=-1)
 
         if self.use_appearance_embedding:
             if ray_samples.camera_indices is None:
                 raise AttributeError("Camera indices are not provided.")
             camera_indices = ray_samples.camera_indices.squeeze()
             if self.training:
                 embedded_appearance = self.appearance_embedding(camera_indices)
@@ -179,24 +188,9 @@
         """Returns the opacity for a position. Used primarily by the occupancy grid.
 
         Args:
             positions: the positions to evaluate the opacity at.
             step_size: the step size to use for the opacity evaluation.
         """
         density = self.density_fn(positions)
-        ## TODO: We should scale step size based on the distortion. Currently it uses too much memory.
-        # aabb_min, aabb_max = self.aabb[0], self.aabb[1]
-        # if self.contraction_type is not ContractionType.AABB:
-        #     x = (positions - aabb_min) / (aabb_max - aabb_min)
-        #     x = x * 2 - 1  # aabb is at [-1, 1]
-        #     mag = x.norm(dim=-1, keepdim=True)
-        #     mask = mag.squeeze(-1) > 1
-
-        #     dev = (2 * mag - 1) / mag**2 + 2 * x**2 * (1 / mag**3 - (2 * mag - 1) / mag**4)
-        #     dev[~mask] = 1.0
-        #     dev = torch.clamp(dev, min=1e-6)
-        #     step_size = step_size / dev.norm(dim=-1, keepdim=True)
-        # else:
-        #     step_size = step_size * (aabb_max - aabb_min)
-
         opacity = density * step_size
         return opacity
```

### Comparing `nerfstudio-0.2.1/nerfstudio/fields/nerfacto_field.py` & `nerfstudio-0.2.2/nerfstudio/fields/nerfacto_field.py`

 * *Files 2% similar despite different names*

```diff
@@ -99,15 +99,15 @@
         transient_embedding_dim: int = 16,
         use_transient_embedding: bool = False,
         use_semantics: bool = False,
         num_semantic_classes: int = 100,
         pass_semantic_gradients: bool = False,
         use_pred_normals: bool = False,
         use_average_appearance_embedding: bool = False,
-        spatial_distortion: SpatialDistortion = None,
+        spatial_distortion: Optional[SpatialDistortion] = None,
     ) -> None:
         super().__init__()
 
         self.register_buffer("aabb", aabb)
         self.geo_feat_dim = geo_feat_dim
 
         self.register_buffer("max_res", torch.tensor(max_res))
@@ -377,16 +377,16 @@
 
     def get_density(self, ray_samples: RaySamples) -> Tuple[TensorType, TensorType]:
         if self.spatial_distortion is not None:
             positions = ray_samples.frustums.get_positions()
             positions = self.spatial_distortion(positions)
         else:
             positions = ray_samples.frustums.get_positions()
-        encoded_xyz = self.position_encoding(positions)
-        base_mlp_out = self.mlp_base(encoded_xyz)
+        encoded_xyz = self.position_encoding(positions.view(-1, 3)).to(torch.float32)
+        base_mlp_out = self.mlp_base(encoded_xyz).view(*ray_samples.frustums.shape, -1)
         density = self.field_output_density(base_mlp_out)
         return density, base_mlp_out
 
     def get_outputs(
         self, ray_samples: RaySamples, density_embedding: Optional[TensorType] = None
     ) -> Dict[FieldHeadNames, TensorType]:
         outputs_shape = ray_samples.frustums.directions.shape[:-1]
@@ -400,23 +400,25 @@
             embedded_appearance = torch.zeros(
                 (*outputs_shape, self.appearance_embedding_dim),
                 device=ray_samples.frustums.directions.device,
             )
 
         outputs = {}
         for field_head in self.field_heads:
-            encoded_dir = self.direction_encoding(ray_samples.frustums.directions)
+            directions = shift_directions_for_tcnn(ray_samples.frustums.directions)
+            directions_flat = directions.view(-1, 3)
+            encoded_dir = self.direction_encoding(directions_flat)
             mlp_out = self.mlp_head(
                 torch.cat(
                     [
-                        encoded_dir,
-                        density_embedding,  # type:ignore
+                        encoded_dir.view(-1, self.direction_encoding.get_out_dim()),
+                        density_embedding.view(-1, self.mlp_base.get_out_dim()),  # type:ignore
                         embedded_appearance.view(-1, self.appearance_embedding_dim),
                     ],
                     dim=-1,  # type:ignore
                 )
             )
-            outputs[field_head.field_head_name] = field_head(mlp_out)
+            outputs[field_head.field_head_name] = field_head(mlp_out).view(*outputs_shape, -1).to(directions)
         return outputs
 
 
 field_implementation_to_class: Dict[str, Field] = {"tcnn": TCNNNerfactoField, "torch": TorchNerfactoField}
```

### Comparing `nerfstudio-0.2.1/nerfstudio/fields/nerfplayer_nerfacto_field.py` & `nerfstudio-0.2.2/nerfstudio/fields/nerfplayer_nerfacto_field.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-0.2.1/nerfstudio/fields/nerfplayer_ngp_field.py` & `nerfstudio-0.2.2/nerfstudio/fields/nerfplayer_ngp_field.py`

 * *Files 8% similar despite different names*

```diff
@@ -16,23 +16,26 @@
 NeRFPlayer (https://arxiv.org/abs/2210.15947) field implementations with InstantNGP backbone
 """
 
 
 from typing import Dict, Optional, Tuple
 
 import torch
-from nerfacc import ContractionType, contract
 from torch.nn.parameter import Parameter
 from torchtyping import TensorType
 
 from nerfstudio.cameras.rays import Frustums, RaySamples
 from nerfstudio.data.scene_box import SceneBox
 from nerfstudio.field_components.activations import trunc_exp
 from nerfstudio.field_components.embedding import Embedding
 from nerfstudio.field_components.field_heads import FieldHeadNames
+from nerfstudio.field_components.spatial_distortions import (
+    SceneContraction,
+    SpatialDistortion,
+)
 from nerfstudio.field_components.temporal_grid import TemporalGridEncoder
 from nerfstudio.fields.base_field import Field, shift_directions_for_tcnn
 
 try:
     import tinycudann as tcnn
 except ImportError:
     # tinycudann module doesn't exist
@@ -78,21 +81,21 @@
         geo_feat_dim: int = 15,
         num_layers_color: int = 3,
         hidden_dim_color: int = 64,
         use_appearance_embedding: bool = False,
         disable_viewing_dependent: bool = False,
         num_images: Optional[int] = None,
         appearance_embedding_dim: int = 32,
-        contraction_type: ContractionType = ContractionType.UN_BOUNDED_SPHERE,
+        spatial_distortion: Optional[SpatialDistortion] = SceneContraction(),
     ) -> None:
         super().__init__()
 
         self.aabb = Parameter(aabb, requires_grad=False)
         self.geo_feat_dim = geo_feat_dim
-        self.contraction_type = contraction_type
+        self.spatial_distortion = spatial_distortion
 
         self.use_appearance_embedding = use_appearance_embedding
         if use_appearance_embedding:
             assert num_images is not None
             self.appearance_embedding_dim = appearance_embedding_dim
             self.appearance_embedding = Embedding(num_images, appearance_embedding_dim)
 
@@ -140,50 +143,51 @@
                 "output_activation": "Sigmoid",
                 "n_neurons": hidden_dim_color,
                 "n_hidden_layers": num_layers_color - 1,
             },
         )
 
     def get_density(self, ray_samples: RaySamples) -> Tuple[TensorType, TensorType]:
-        positions = ray_samples.frustums.get_positions()
+        if self.spatial_distortion is not None:
+            positions = ray_samples.frustums.get_positions()
+            positions = self.spatial_distortion(positions)
+            positions = (positions + 2.0) / 4.0
+        else:
+            positions = SceneBox.get_normalized_positions(ray_samples.frustums.get_positions(), self.aabb)
+        # Make sure the tcnn gets inputs between 0 and 1.
+        selector = ((positions > 0.0) & (positions < 1.0)).all(dim=-1)
+        positions = positions * selector[..., None]
         positions_flat = positions.view(-1, 3)
-        positions_flat = contract(x=positions_flat, roi=self.aabb, type=self.contraction_type)
         assert ray_samples.times is not None, "Time should be included in the input for NeRFPlayer"
         times_flat = ray_samples.times.view(-1, 1)
 
         h = self.mlp_base(positions_flat, times_flat)
         h = self.mlp_base_decode(h).view(*ray_samples.frustums.shape, -1)
         density_before_activation, base_mlp_out = torch.split(h, [1, self.geo_feat_dim], dim=-1)
 
         # Rectifying the density with an exponential is much more stable than a ReLU or
         # softplus, because it enables high post-activation (float32) density outputs
         # from smaller internal (float16) parameters.
         density = trunc_exp(density_before_activation.to(positions))
+        density = density * selector[..., None]
         return density, base_mlp_out
 
     def get_outputs(
         self, ray_samples: RaySamples, density_embedding: Optional[TensorType] = None
     ) -> Dict[FieldHeadNames, TensorType]:
+        assert density_embedding is not None
         directions = shift_directions_for_tcnn(ray_samples.frustums.directions)
         directions_flat = directions.view(-1, 3)
 
         if self.direction_encoding is not None:
             d = self.direction_encoding(directions_flat)
-            if density_embedding is None:
-                positions = SceneBox.get_normalized_positions(ray_samples.frustums.get_positions(), self.aabb)
-                h = torch.cat([d, positions.view(-1, 3)], dim=-1)
-            else:
-                h = torch.cat([d, density_embedding.view(-1, self.geo_feat_dim)], dim=-1)
+            h = torch.cat([d, density_embedding.view(-1, self.geo_feat_dim)], dim=-1)
         else:
             # viewing direction is disabled
-            if density_embedding is None:
-                positions = SceneBox.get_normalized_positions(ray_samples.frustums.get_positions(), self.aabb)
-                h = positions.view(-1, 3)
-            else:
-                h = density_embedding.view(-1, self.geo_feat_dim)
+            h = density_embedding.view(-1, self.geo_feat_dim)
 
         if self.use_appearance_embedding:
             if ray_samples.camera_indices is None:
                 raise AttributeError("Camera indices are not provided.")
             camera_indices = ray_samples.camera_indices.squeeze()
             if self.training:
                 embedded_appearance = self.appearance_embedding(camera_indices)
```

### Comparing `nerfstudio-0.2.1/nerfstudio/fields/nerfw_field.py` & `nerfstudio-0.2.2/nerfstudio/fields/nerfw_field.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-0.2.1/nerfstudio/fields/sdf_field.py` & `nerfstudio-0.2.2/nerfstudio/fields/sdf_field.py`

 * *Files 2% similar despite different names*

```diff
@@ -76,21 +76,21 @@
     num_layers_color: int = 4
     """Number of layers for color network"""
     hidden_dim_color: int = 256
     """Number of hidden dimension of color network"""
     appearance_embedding_dim: int = 32
     """Dimension of appearance embedding"""
     use_appearance_embedding: bool = False
-    """Dimension of appearance embedding"""
+    """Whether to use appearance embedding"""
     bias: float = 0.8
-    """sphere size of geometric initializaion"""
+    """Sphere size of geometric initialization"""
     geometric_init: bool = True
     """Whether to use geometric initialization"""
     inside_outside: bool = True
-    """whether to revert signed distance value, set to True for indoor scene"""
+    """Whether to revert signed distance value, set to True for indoor scene"""
     weight_norm: bool = True
     """Whether to use weight norm for linear layer"""
     use_grid_feature: bool = False
     """Whether to use multi-resolution feature grids"""
     divide_factor: float = 2.0
     """Normalization factor for multi-resolution grids"""
     beta_init: float = 0.1
@@ -253,16 +253,16 @@
         """Set the anneal value for the proposal network."""
         self._cos_anneal_ratio = anneal
 
     def forward_geonetwork(self, inputs: TensorType[..., 3]) -> TensorType[..., "geo-features+1"]:
         """forward the geonetwork"""
         if self.use_grid_feature:
             positions = self.spatial_distortion(inputs)
-
-            positions = (positions + 1.0) / 2.0
+            # map range [-2, 2] to [0, 1]
+            positions = (positions + 2.0) / 4.0
             feature = self.encoding(positions)
         else:
             feature = torch.zeros_like(inputs[:, :1].repeat(1, self.encoding.n_output_dims))
 
         pe = self.position_encoding(inputs)
 
         inputs = torch.cat((inputs, pe, feature), dim=-1)
```

### Comparing `nerfstudio-0.2.1/nerfstudio/fields/semantic_nerf_field.py` & `nerfstudio-0.2.2/nerfstudio/fields/semantic_nerf_field.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-0.2.1/nerfstudio/fields/tensorf_field.py` & `nerfstudio-0.2.2/nerfstudio/fields/tensorf_field.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-0.2.1/nerfstudio/fields/vanilla_nerf_field.py` & `nerfstudio-0.2.2/nerfstudio/fields/vanilla_nerf_field.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-0.2.1/nerfstudio/generative/__init__.py` & `nerfstudio-0.2.2/nerfstudio/generative/__init__.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-0.2.1/nerfstudio/generative/stable_diffusion.py` & `nerfstudio-0.2.2/nerfstudio/generative/stable_diffusion.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-0.2.1/nerfstudio/model_components/__init__.py` & `nerfstudio-0.2.2/nerfstudio/model_components/__init__.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-0.2.1/nerfstudio/model_components/losses.py` & `nerfstudio-0.2.2/nerfstudio/model_components/losses.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-0.2.1/nerfstudio/model_components/ray_generators.py` & `nerfstudio-0.2.2/nerfstudio/model_components/ray_generators.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-0.2.1/nerfstudio/model_components/ray_samplers.py` & `nerfstudio-0.2.2/nerfstudio/model_components/ray_samplers.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,17 +15,16 @@
 """
 Collection of sampling strategies
 """
 
 from abc import abstractmethod
 from typing import Callable, List, Optional, Tuple, Union
 
-import nerfacc
 import torch
-from nerfacc import OccupancyGrid
+from nerfacc import OccGridEstimator
 from torch import nn
 from torchtyping import TensorType
 
 from nerfstudio.cameras.rays import Frustums, RayBundle, RaySamples
 
 
 class Sampler(nn.Module):
@@ -378,46 +377,46 @@
     occupancy_grid: Occupancy grid to sample from.
     density_fn: Function that evaluates density at a given point.
     scene_aabb: Axis-aligned bounding box of the scene, should be set to None if the scene is unbounded.
     """
 
     def __init__(
         self,
-        occupancy_grid: Optional[OccupancyGrid] = None,
+        occupancy_grid: OccGridEstimator,
         density_fn: Optional[Callable[[TensorType[..., 3]], TensorType[..., 1]]] = None,
-        scene_aabb: Optional[TensorType[2, 3]] = None,
     ) -> None:
 
         super().__init__()
-        self.scene_aabb = scene_aabb
+        assert occupancy_grid is not None
         self.density_fn = density_fn
         self.occupancy_grid = occupancy_grid
-        if self.scene_aabb is not None:
-            self.scene_aabb = self.scene_aabb.to("cuda").flatten()
 
-    def get_sigma_fn(self, origins, directions) -> Optional[Callable]:
+    def get_sigma_fn(self, origins, directions, times=None) -> Optional[Callable]:
         """Returns a function that returns the density of a point.
 
         Args:
             origins: Origins of rays
             directions: Directions of rays
+            times: Times at which rays are sampled
         Returns:
             Function that returns the density of a point or None if a density function is not provided.
         """
 
         if self.density_fn is None or not self.training:
             return None
 
         density_fn = self.density_fn
 
         def sigma_fn(t_starts, t_ends, ray_indices):
             t_origins = origins[ray_indices]
             t_dirs = directions[ray_indices]
-            positions = t_origins + t_dirs * (t_starts + t_ends) / 2.0
-            return density_fn(positions)
+            positions = t_origins + t_dirs * (t_starts + t_ends)[:, None] / 2.0
+            if times is None:
+                return density_fn(positions).squeeze(-1)
+            return density_fn(positions, times[ray_indices]).squeeze(-1)
 
         return sigma_fn
 
     def generate_ray_samples(self) -> RaySamples:
         raise RuntimeError(
             "The VolumetricSampler fuses sample generation and density check together. Please call forward() directly."
         )
@@ -425,83 +424,85 @@
     # pylint: disable=arguments-differ
     def forward(
         self,
         ray_bundle: RayBundle,
         render_step_size: float,
         near_plane: float = 0.0,
         far_plane: Optional[float] = None,
+        alpha_thre: float = 0.01,
         cone_angle: float = 0.0,
     ) -> Tuple[RaySamples, TensorType["total_samples",]]:
         """Generate ray samples in a bounding box.
 
         Args:
             ray_bundle: Rays to generate samples for
             render_step_size: Minimum step size to use for rendering
             near_plane: Near plane for raymarching
             far_plane: Far plane for raymarching
+            alpha_thre: Opacity threshold skipping samples.
             cone_angle: Cone angle for raymarching, set to 0 for uniform marching.
 
         Returns:
             a tuple of (ray_samples, packed_info, ray_indices)
             The ray_samples are packed, only storing the valid samples.
             The ray_indices contains the indices of the rays that each sample belongs to.
         """
 
         rays_o = ray_bundle.origins.contiguous()
         rays_d = ray_bundle.directions.contiguous()
+        times = ray_bundle.times
 
         if ray_bundle.nears is not None and ray_bundle.fars is not None:
             t_min = ray_bundle.nears.contiguous().reshape(-1)
             t_max = ray_bundle.fars.contiguous().reshape(-1)
 
         else:
             t_min = None
             t_max = None
 
+        if far_plane is None:
+            far_plane = 1e10
+
         if ray_bundle.camera_indices is not None:
             camera_indices = ray_bundle.camera_indices.contiguous()
         else:
             camera_indices = None
-
-        ray_indices, starts, ends = nerfacc.ray_marching(
+        ray_indices, starts, ends = self.occupancy_grid.sampling(
             rays_o=rays_o,
             rays_d=rays_d,
             t_min=t_min,
             t_max=t_max,
-            scene_aabb=self.scene_aabb,
-            grid=self.occupancy_grid,
-            # this is a workaround - using density causes crash and damage quality. should be fixed
-            sigma_fn=None,  # self.get_sigma_fn(rays_o, rays_d),
+            sigma_fn=self.get_sigma_fn(rays_o, rays_d, times),
             render_step_size=render_step_size,
             near_plane=near_plane,
             far_plane=far_plane,
             stratified=self.training,
             cone_angle=cone_angle,
-            alpha_thre=1e-2,
+            alpha_thre=alpha_thre,
         )
         num_samples = starts.shape[0]
         if num_samples == 0:
             # create a single fake sample and update packed_info accordingly
             # this says the last ray in packed_info has 1 sample, which starts and ends at 1
             ray_indices = torch.zeros((1,), dtype=torch.long, device=rays_o.device)
-            starts = torch.ones((1, 1), dtype=starts.dtype, device=rays_o.device)
-            ends = torch.ones((1, 1), dtype=ends.dtype, device=rays_o.device)
+            starts = torch.ones((1,), dtype=starts.dtype, device=rays_o.device)
+            ends = torch.ones((1,), dtype=ends.dtype, device=rays_o.device)
 
         origins = rays_o[ray_indices]
         dirs = rays_d[ray_indices]
         if camera_indices is not None:
             camera_indices = camera_indices[ray_indices]
 
         zeros = torch.zeros_like(origins[:, :1])
         ray_samples = RaySamples(
             frustums=Frustums(
                 origins=origins,
                 directions=dirs,
-                starts=starts,
-                ends=ends,
+                starts=starts[..., None],
+                ends=ends[..., None],
                 pixel_area=zeros,
             ),
             camera_indices=camera_indices,
         )
         if ray_bundle.times is not None:
             ray_samples.times = ray_bundle.times[ray_indices]
         return ray_samples, ray_indices
```

### Comparing `nerfstudio-0.2.1/nerfstudio/model_components/renderers.py` & `nerfstudio-0.2.2/nerfstudio/model_components/renderers.py`

 * *Files 6% similar despite different names*

```diff
@@ -87,16 +87,20 @@
         Returns:
             Outputs rgb values.
         """
         if ray_indices is not None and num_rays is not None:
             # Necessary for packed samples from volumetric ray sampler
             if background_color == "last_sample":
                 raise NotImplementedError("Background color 'last_sample' not implemented for packed samples.")
-            comp_rgb = nerfacc.accumulate_along_rays(weights, ray_indices, rgb, num_rays)
-            accumulated_weight = nerfacc.accumulate_along_rays(weights, ray_indices, None, num_rays)
+            comp_rgb = nerfacc.accumulate_along_rays(
+                weights[..., 0], values=rgb, ray_indices=ray_indices, n_rays=num_rays
+            )
+            accumulated_weight = nerfacc.accumulate_along_rays(
+                weights[..., 0], values=None, ray_indices=ray_indices, n_rays=num_rays
+            )
         else:
             comp_rgb = torch.sum(weights * rgb, dim=-2)
             accumulated_weight = torch.sum(weights, dim=-2)
 
         if BACKGROUND_COLOR_OVERRIDE is not None:
             background_color = BACKGROUND_COLOR_OVERRIDE
         if background_color == "last_sample":
@@ -213,15 +217,17 @@
 
         Returns:
             Outputs of accumulated values.
         """
 
         if ray_indices is not None and num_rays is not None:
             # Necessary for packed samples from volumetric ray sampler
-            accumulation = nerfacc.accumulate_along_rays(weights, ray_indices, None, num_rays)
+            accumulation = nerfacc.accumulate_along_rays(
+                weights[..., 0], values=None, ray_indices=ray_indices, n_rays=num_rays
+            )
         else:
             accumulation = torch.sum(weights, dim=-2)
         return accumulation
 
 
 class DepthRenderer(nn.Module):
     """Calculate depth along ray.
@@ -270,16 +276,20 @@
             return median_depth
         if self.method == "expected":
             eps = 1e-10
             steps = (ray_samples.frustums.starts + ray_samples.frustums.ends) / 2
 
             if ray_indices is not None and num_rays is not None:
                 # Necessary for packed samples from volumetric ray sampler
-                depth = nerfacc.accumulate_along_rays(weights, ray_indices, steps, num_rays)
-                accumulation = nerfacc.accumulate_along_rays(weights, ray_indices, None, num_rays)
+                depth = nerfacc.accumulate_along_rays(
+                    weights[..., 0], values=steps, ray_indices=ray_indices, n_rays=num_rays
+                )
+                accumulation = nerfacc.accumulate_along_rays(
+                    weights[..., 0], values=None, ray_indices=ray_indices, n_rays=num_rays
+                )
                 depth = depth / (accumulation + eps)
             else:
                 depth = torch.sum(weights * steps, dim=-2) / (torch.sum(weights, -2) + eps)
 
             depth = torch.clip(depth, steps.min(), steps.max())
 
             return depth
```

### Comparing `nerfstudio-0.2.1/nerfstudio/model_components/scene_colliders.py` & `nerfstudio-0.2.2/nerfstudio/model_components/scene_colliders.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-0.2.1/nerfstudio/model_components/shaders.py` & `nerfstudio-0.2.2/nerfstudio/model_components/shaders.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-0.2.1/nerfstudio/models/__init__.py` & `nerfstudio-0.2.2/nerfstudio/models/__init__.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-0.2.1/nerfstudio/models/base_model.py` & `nerfstudio-0.2.2/nerfstudio/models/base_model.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-0.2.1/nerfstudio/models/base_surface_model.py` & `nerfstudio-0.2.2/nerfstudio/models/base_surface_model.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-0.2.1/nerfstudio/models/depth_nerfacto.py` & `nerfstudio-0.2.2/nerfstudio/models/depth_nerfacto.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-0.2.1/nerfstudio/models/instant_ngp.py` & `nerfstudio-0.2.2/nerfstudio/models/instant_ngp.py`

 * *Files 8% similar despite different names*

```diff
@@ -19,29 +19,29 @@
 from __future__ import annotations
 
 from dataclasses import dataclass, field
 from typing import Dict, List, Optional, Tuple, Type
 
 import nerfacc
 import torch
-from nerfacc import ContractionType
 from torch.nn import Parameter
 from torchmetrics import PeakSignalNoiseRatio
 from torchmetrics.functional import structural_similarity_index_measure
 from torchmetrics.image.lpip import LearnedPerceptualImagePatchSimilarity
 from typing_extensions import Literal
 
 from nerfstudio.cameras.rays import RayBundle
 from nerfstudio.engine.callbacks import (
     TrainingCallback,
     TrainingCallbackAttributes,
     TrainingCallbackLocation,
 )
 from nerfstudio.field_components.field_heads import FieldHeadNames
-from nerfstudio.fields.instant_ngp_field import TCNNInstantNGPField
+from nerfstudio.field_components.spatial_distortions import SceneContraction
+from nerfstudio.fields.nerfacto_field import TCNNNerfactoField
 from nerfstudio.model_components.losses import MSELoss
 from nerfstudio.model_components.ray_samplers import VolumetricSampler
 from nerfstudio.model_components.renderers import (
     AccumulationRenderer,
     DepthRenderer,
     RGBRenderer,
 )
@@ -57,77 +57,84 @@
         default_factory=lambda: NGPModel
     )  # We can't write `NGPModel` directly, because `NGPModel` doesn't exist yet
     """target class to instantiate"""
     enable_collider: bool = False
     """Whether to create a scene collider to filter rays."""
     collider_params: Optional[Dict[str, float]] = None
     """Instant NGP doesn't use a collider."""
-    max_num_samples_per_ray: int = 24
-    """Number of samples in field evaluation."""
     grid_resolution: int = 128
     """Resolution of the grid used for the field."""
+    grid_levels: int = 4
+    """Levels of the grid used for the field."""
     max_res: int = 2048
     """Maximum resolution of the hashmap for the base mlp."""
     log2_hashmap_size: int = 19
     """Size of the hashmap for the base mlp"""
-    contraction_type: ContractionType = ContractionType.UN_BOUNDED_SPHERE
-    """Contraction type used for spatial deformation of the field."""
+    alpha_thre: float = 0.01
+    """Threshold for opacity skipping."""
     cone_angle: float = 0.004
     """Should be set to 0.0 for blender scenes but 1./256 for real scenes."""
-    render_step_size: float = 0.01
+    render_step_size: Optional[float] = None
     """Minimum step size for rendering."""
     near_plane: float = 0.05
     """How far along ray to start sampling."""
     far_plane: float = 1e3
     """How far along ray to stop sampling."""
     use_appearance_embedding: bool = False
     """Whether to use an appearance embedding."""
     background_color: Literal["random", "black", "white"] = "random"
     """The color that is given to untrained areas."""
+    disable_scene_contraction: bool = False
+    """Whether to disable scene contraction or not."""
 
 
 class NGPModel(Model):
     """Instant NGP model
 
     Args:
         config: instant NGP configuration to instantiate model
     """
 
     config: InstantNGPModelConfig
-    field: TCNNInstantNGPField
+    field: TCNNNerfactoField
 
     def __init__(self, config: InstantNGPModelConfig, **kwargs) -> None:
         super().__init__(config=config, **kwargs)
 
     def populate_modules(self):
         """Set the fields and modules."""
         super().populate_modules()
 
-        self.field = TCNNInstantNGPField(
+        if self.config.disable_scene_contraction:
+            scene_contraction = None
+        else:
+            scene_contraction = SceneContraction(order=float("inf"))
+
+        self.field = TCNNNerfactoField(
             aabb=self.scene_box.aabb,
-            contraction_type=self.config.contraction_type,
-            use_appearance_embedding=self.config.use_appearance_embedding,
             num_images=self.num_train_data,
             log2_hashmap_size=self.config.log2_hashmap_size,
             max_res=self.config.max_res,
+            spatial_distortion=scene_contraction,
         )
 
         self.scene_aabb = Parameter(self.scene_box.aabb.flatten(), requires_grad=False)
 
-        # Occupancy Grid
-        self.occupancy_grid = nerfacc.OccupancyGrid(
+        if self.config.render_step_size is None:
+            # auto step size: ~1000 samples in the base level grid
+            self.config.render_step_size = ((self.scene_aabb[3:] - self.scene_aabb[:3]) ** 2).sum().sqrt().item() / 1000
+        # Occupancy Grid.
+        self.occupancy_grid = nerfacc.OccGridEstimator(
             roi_aabb=self.scene_aabb,
             resolution=self.config.grid_resolution,
-            contraction_type=self.config.contraction_type,
+            levels=self.config.grid_levels,
         )
 
         # Sampler
-        vol_sampler_aabb = self.scene_box.aabb if self.config.contraction_type == ContractionType.AABB else None
         self.sampler = VolumetricSampler(
-            scene_aabb=vol_sampler_aabb,
             occupancy_grid=self.occupancy_grid,
             density_fn=self.field.density_fn,
         )
 
         # renderers
         self.renderer_rgb = RGBRenderer(background_color=self.config.background_color)
         self.renderer_accumulation = AccumulationRenderer()
@@ -141,19 +148,17 @@
         self.ssim = structural_similarity_index_measure
         self.lpips = LearnedPerceptualImagePatchSimilarity(normalize=True)
 
     def get_training_callbacks(
         self, training_callback_attributes: TrainingCallbackAttributes
     ) -> List[TrainingCallback]:
         def update_occupancy_grid(step: int):
-            # TODO: needs to get access to the sampler, on how the step size is determinated at each x. See
-            # https://github.com/KAIR-BAIR/nerfacc/blob/127223b11401125a9fce5ce269bb0546ee4de6e8/examples/train_ngp_nerf.py#L190-L213
-            self.occupancy_grid.every_n_step(
+            self.occupancy_grid.update_every_n_steps(
                 step=step,
-                occ_eval_fn=lambda x: self.field.get_opacity(x, self.config.render_step_size),
+                occ_eval_fn=lambda x: self.field.density_fn(x) * self.config.render_step_size,
             )
 
         return [
             TrainingCallback(
                 where_to_run=[TrainingCallbackLocation.BEFORE_TRAIN_ITERATION],
                 update_every_num_iters=1,
                 func=update_occupancy_grid,
@@ -173,80 +178,77 @@
 
         with torch.no_grad():
             ray_samples, ray_indices = self.sampler(
                 ray_bundle=ray_bundle,
                 near_plane=self.config.near_plane,
                 far_plane=self.config.far_plane,
                 render_step_size=self.config.render_step_size,
+                alpha_thre=self.config.alpha_thre,
                 cone_angle=self.config.cone_angle,
             )
 
         field_outputs = self.field(ray_samples)
 
         # accumulation
         packed_info = nerfacc.pack_info(ray_indices, num_rays)
         weights = nerfacc.render_weight_from_density(
+            t_starts=ray_samples.frustums.starts[..., 0],
+            t_ends=ray_samples.frustums.ends[..., 0],
+            sigmas=field_outputs[FieldHeadNames.DENSITY][..., 0],
             packed_info=packed_info,
-            sigmas=field_outputs[FieldHeadNames.DENSITY],
-            t_starts=ray_samples.frustums.starts,
-            t_ends=ray_samples.frustums.ends,
-        )
+        )[0]
+        weights = weights[..., None]
 
         rgb = self.renderer_rgb(
             rgb=field_outputs[FieldHeadNames.RGB],
             weights=weights,
             ray_indices=ray_indices,
             num_rays=num_rays,
         )
         depth = self.renderer_depth(
             weights=weights, ray_samples=ray_samples, ray_indices=ray_indices, num_rays=num_rays
         )
         accumulation = self.renderer_accumulation(weights=weights, ray_indices=ray_indices, num_rays=num_rays)
-        alive_ray_mask = accumulation.squeeze(-1) > 0
 
         outputs = {
             "rgb": rgb,
             "accumulation": accumulation,
             "depth": depth,
-            "alive_ray_mask": alive_ray_mask,  # the rays we kept from sampler
             "num_samples_per_ray": packed_info[:, 1],
         }
         return outputs
 
     def get_metrics_dict(self, outputs, batch):
         image = batch["image"].to(self.device)
         metrics_dict = {}
         metrics_dict["psnr"] = self.psnr(outputs["rgb"], image)
         metrics_dict["num_samples_per_batch"] = outputs["num_samples_per_ray"].sum()
         return metrics_dict
 
     def get_loss_dict(self, outputs, batch, metrics_dict=None):
         image = batch["image"].to(self.device)
-        mask = outputs["alive_ray_mask"]
-        rgb_loss = self.rgb_loss(image[mask], outputs["rgb"][mask])
+        rgb_loss = self.rgb_loss(image, outputs["rgb"])
         loss_dict = {"rgb_loss": rgb_loss}
         return loss_dict
 
     def get_image_metrics_and_images(
         self, outputs: Dict[str, torch.Tensor], batch: Dict[str, torch.Tensor]
     ) -> Tuple[Dict[str, float], Dict[str, torch.Tensor]]:
 
         image = batch["image"].to(self.device)
         rgb = outputs["rgb"]
         acc = colormaps.apply_colormap(outputs["accumulation"])
         depth = colormaps.apply_depth_colormap(
             outputs["depth"],
             accumulation=outputs["accumulation"],
         )
-        alive_ray_mask = colormaps.apply_colormap(outputs["alive_ray_mask"])
 
         combined_rgb = torch.cat([image, rgb], dim=1)
         combined_acc = torch.cat([acc], dim=1)
         combined_depth = torch.cat([depth], dim=1)
-        combined_alive_ray_mask = torch.cat([alive_ray_mask], dim=1)
 
         # Switch images from [H, W, C] to [1, C, H, W] for metrics computations
         image = torch.moveaxis(image, -1, 0)[None, ...]
         rgb = torch.moveaxis(rgb, -1, 0)[None, ...]
 
         psnr = self.psnr(image, rgb)
         ssim = self.ssim(image, rgb)
@@ -256,11 +258,10 @@
         metrics_dict = {"psnr": float(psnr.item()), "ssim": float(ssim), "lpips": float(lpips)}  # type: ignore
         # TODO(ethan): return an image dictionary
 
         images_dict = {
             "img": combined_rgb,
             "accumulation": combined_acc,
             "depth": combined_depth,
-            "alive_ray_mask": combined_alive_ray_mask,
         }
 
         return metrics_dict, images_dict
```

### Comparing `nerfstudio-0.2.1/nerfstudio/models/mipnerf.py` & `nerfstudio-0.2.2/nerfstudio/models/mipnerf.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-0.2.1/nerfstudio/models/nerfacto.py` & `nerfstudio-0.2.2/nerfstudio/models/nerfacto.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-0.2.1/nerfstudio/models/nerfplayer_nerfacto.py` & `nerfstudio-0.2.2/nerfstudio/models/nerfplayer_nerfacto.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-0.2.1/nerfstudio/models/nerfplayer_ngp.py` & `nerfstudio-0.2.2/nerfstudio/models/nerfplayer_ngp.py`

 * *Files 8% similar despite different names*

```diff
@@ -15,27 +15,32 @@
 """
 Implementation of NeRFPlayer (https://arxiv.org/abs/2210.15947) with InstantNGP backbone.
 """
 
 from __future__ import annotations
 
 from dataclasses import dataclass, field
-from typing import Type
+from typing import List, Type
 
 import nerfacc
 import torch
-from nerfacc import ContractionType
 from torch.nn import Parameter
 from torchmetrics import PeakSignalNoiseRatio
 from torchmetrics.functional import structural_similarity_index_measure
 from torchmetrics.image.lpip import LearnedPerceptualImagePatchSimilarity
 from typing_extensions import Literal
 
 from nerfstudio.cameras.rays import RayBundle
+from nerfstudio.engine.callbacks import (
+    TrainingCallback,
+    TrainingCallbackAttributes,
+    TrainingCallbackLocation,
+)
 from nerfstudio.field_components.field_heads import FieldHeadNames
+from nerfstudio.field_components.spatial_distortions import SceneContraction
 from nerfstudio.fields.nerfplayer_ngp_field import NerfplayerNGPField
 from nerfstudio.model_components.losses import MSELoss
 from nerfstudio.model_components.ray_samplers import VolumetricSampler
 from nerfstudio.model_components.renderers import (
     AccumulationRenderer,
     DepthRenderer,
     RGBRenderer,
@@ -76,14 +81,16 @@
     """depth loss balancing weight for feature channels."""
     train_background_color: Literal["random", "black", "white"] = "random"
     """The training background color that is given to untrained areas."""
     eval_background_color: Literal["random", "black", "white"] = "white"
     """The training background color that is given to untrained areas."""
     disable_viewing_dependent: bool = True
     """Disable viewing dependent effects."""
+    disable_scene_contraction: bool = False
+    """Whether to disable scene contraction or not."""
 
 
 class NerfplayerNGPModel(NGPModel):
     """NeRFPlayer Model with InstantNGP backbone.
 
     Args:
         config: NeRFPlayer NGP configuration to instantiate model
@@ -92,40 +99,43 @@
     config: NerfplayerNGPModelConfig
     field: NerfplayerNGPField
 
     def populate_modules(self):
         """Set the fields and modules."""
         Model.populate_modules(self)
 
+        if self.config.disable_scene_contraction:
+            scene_contraction = None
+        else:
+            scene_contraction = SceneContraction(order=float("inf"))
+
         self.field = NerfplayerNGPField(
             aabb=self.scene_box.aabb,
-            contraction_type=self.config.contraction_type,
             use_appearance_embedding=self.config.use_appearance_embedding,
             num_images=self.num_train_data,
             temporal_dim=self.config.temporal_dim,
             num_levels=self.config.num_levels,
             features_per_level=self.config.features_per_level,
             log2_hashmap_size=self.config.log2_hashmap_size,
             base_resolution=self.config.base_resolution,
             disable_viewing_dependent=self.config.disable_viewing_dependent,
+            spatial_distortion=scene_contraction,
         )
 
         self.scene_aabb = Parameter(self.scene_box.aabb.flatten(), requires_grad=False)
 
         # Occupancy Grid
-        self.occupancy_grid = nerfacc.OccupancyGrid(
+        self.occupancy_grid = nerfacc.OccGridEstimator(
             roi_aabb=self.scene_aabb,
             resolution=self.config.grid_resolution,
-            contraction_type=self.config.contraction_type,
+            levels=self.config.grid_levels,
         )
 
         # Sampler
-        vol_sampler_aabb = self.scene_box.aabb if self.config.contraction_type == ContractionType.AABB else None
         self.sampler = VolumetricSampler(
-            scene_aabb=vol_sampler_aabb,
             occupancy_grid=self.occupancy_grid,
             density_fn=self.field.density_fn,
         )  # need to update the density_fn later during forward (for input time)
 
         # renderers
         self.renderer_rgb = RGBRenderer()  # will update bgcolor later during forward
         self.renderer_accumulation = AccumulationRenderer()
@@ -136,38 +146,55 @@
 
         # metrics
         self.psnr = PeakSignalNoiseRatio(data_range=1.0)
         self.ssim = structural_similarity_index_measure
         self.lpips = LearnedPerceptualImagePatchSimilarity(normalize=True)
         self.temporal_distortion = True  # for viewer
 
+    def get_training_callbacks(
+        self, training_callback_attributes: TrainingCallbackAttributes
+    ) -> List[TrainingCallback]:
+        def update_occupancy_grid(step: int):
+            self.occupancy_grid.update_every_n_steps(
+                step=step,
+                occ_eval_fn=lambda x: self.field.get_opacity(x, self.config.render_step_size),
+            )
+
+        return [
+            TrainingCallback(
+                where_to_run=[TrainingCallbackLocation.BEFORE_TRAIN_ITERATION],
+                update_every_num_iters=1,
+                func=update_occupancy_grid,
+            ),
+        ]
+
     def get_outputs(self, ray_bundle: RayBundle):
         num_rays = len(ray_bundle)
 
-        # update the density_fn of the sampler so that the density is time aware
-        self.sampler.density_fn = lambda x: self.field.density_fn(x, ray_bundle.times)
         with torch.no_grad():
             ray_samples, ray_indices = self.sampler(
                 ray_bundle=ray_bundle,
                 near_plane=self.config.near_plane,
                 far_plane=self.config.far_plane,
                 render_step_size=self.config.render_step_size,
                 cone_angle=self.config.cone_angle,
+                alpha_thre=self.config.alpha_thre,
             )
 
         field_outputs = self.field(ray_samples)
 
         # accumulation
         packed_info = nerfacc.pack_info(ray_indices, num_rays)
         weights = nerfacc.render_weight_from_density(
             packed_info=packed_info,
-            sigmas=field_outputs[FieldHeadNames.DENSITY],
-            t_starts=ray_samples.frustums.starts,
-            t_ends=ray_samples.frustums.ends,
-        )
+            sigmas=field_outputs[FieldHeadNames.DENSITY][..., 0],
+            t_starts=ray_samples.frustums.starts[..., 0],
+            t_ends=ray_samples.frustums.ends[..., 0],
+        )[0]
+        weights = weights[..., None]
 
         # update bgcolor in the renderer; usually random color for training and fixed color for inference
         if self.training:
             self.renderer_rgb.background_color = self.config.train_background_color
         else:
             self.renderer_rgb.background_color = self.config.eval_background_color
         rgb = self.renderer_rgb(
@@ -176,37 +203,34 @@
             ray_indices=ray_indices,
             num_rays=num_rays,
         )
         depth = self.renderer_depth(
             weights=weights, ray_samples=ray_samples, ray_indices=ray_indices, num_rays=num_rays
         )
         accumulation = self.renderer_accumulation(weights=weights, ray_indices=ray_indices, num_rays=num_rays)
-        alive_ray_mask = accumulation.squeeze(-1) > 0
 
         outputs = {
             "rgb": rgb,
             "accumulation": accumulation,
             "depth": depth,
-            "alive_ray_mask": alive_ray_mask,  # the rays we kept from sampler
             "num_samples_per_ray": packed_info[:, 1],
         }
         # adding them to outputs for calculating losses
         if self.training and self.config.depth_weight > 0:
             outputs["ray_indices"] = ray_indices
             outputs["ray_samples"] = ray_samples
             outputs["weights"] = weights
             outputs["sigmas"] = field_outputs[FieldHeadNames.DENSITY]
         return outputs
 
     def get_loss_dict(self, outputs, batch, metrics_dict=None):
         image = batch["image"].to(self.device)
-        mask = outputs["alive_ray_mask"]
-        rgb_loss = self.rgb_loss(image[mask], outputs["rgb"][mask])
+        rgb_loss = self.rgb_loss(image, outputs["rgb"])
         loss_dict = {"rgb_loss": rgb_loss}
-        if "depth_image" in batch.keys() and self.config.depth_weight > 0:
+        if "depth_image" in batch.keys() and self.config.depth_weight > 0 and self.training:
             mask = batch["depth_image"] != 0
             # First we calculate the depth value, just like most of the papers.
             loss_dict["depth_loss"] = (outputs["depth"][mask] - batch["depth_image"][mask]).abs().mean()
             # But this is not enough -- it will lead to fog like reconstructions, even with depth supervision.
             # Because this loss only cares about the mean value.
             # (Feel free to try it and see the fog-like effects on DyCheck by commenting out the following loss.)
             # > The fog can be effectively penalized by multiview inputs (i.e., from another viewing point).
@@ -224,10 +248,10 @@
             gt_depth_packed = batch["depth_image"][outputs["ray_indices"]]
             steps = (outputs["ray_samples"].frustums.starts + outputs["ray_samples"].frustums.ends) / 2
             # empty area should not be too close to the given depth, so lets add a margin to the gt depth
             margin = (self.scene_box.aabb.max() - self.scene_box.aabb.min()) / 128
             density_min_mask = (gt_depth_packed - steps > margin) & (gt_depth_packed != 0)
             loss_dict["depth_loss"] += (outputs["sigmas"][density_min_mask[..., 0]].pow(2)).mean() * 1e-2
             loss_dict["depth_loss"] *= self.config.depth_weight
-        if self.config.temporal_tv_weight > 0:
+        if self.config.temporal_tv_weight > 0 and self.training:
             loss_dict["temporal_tv_loss"] = self.config.temporal_tv_weight * self.field.mlp_base.get_temporal_tv_loss()
         return loss_dict
```

### Comparing `nerfstudio-0.2.1/nerfstudio/models/neus.py` & `nerfstudio-0.2.2/nerfstudio/models/neus.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-0.2.1/nerfstudio/models/neus_facto.py` & `nerfstudio-0.2.2/nerfstudio/models/neus_facto.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-0.2.1/nerfstudio/models/semantic_nerfw.py` & `nerfstudio-0.2.2/nerfstudio/models/semantic_nerfw.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-0.2.1/nerfstudio/models/tensorf.py` & `nerfstudio-0.2.2/nerfstudio/models/tensorf.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-0.2.1/nerfstudio/models/vanilla_nerf.py` & `nerfstudio-0.2.2/nerfstudio/models/vanilla_nerf.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-0.2.1/nerfstudio/pipelines/__init__.py` & `nerfstudio-0.2.2/nerfstudio/pipelines/__init__.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-0.2.1/nerfstudio/pipelines/base_pipeline.py` & `nerfstudio-0.2.2/nerfstudio/pipelines/base_pipeline.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-0.2.1/nerfstudio/pipelines/dynamic_batch.py` & `nerfstudio-0.2.2/nerfstudio/pipelines/dynamic_batch.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-0.2.1/nerfstudio/plugins/__init__.py` & `nerfstudio-0.2.2/nerfstudio/plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-0.2.1/nerfstudio/plugins/registry.py` & `nerfstudio-0.2.2/nerfstudio/plugins/registry.py`

 * *Files 24% similar despite different names*

```diff
@@ -12,14 +12,16 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """
 Module that keeps all registered plugins and allows for plugin discovery.
 """
 
+import importlib
+import os
 import sys
 import typing as t
 
 from rich.progress import Console
 
 from nerfstudio.engine.trainer import TrainerConfig
 from nerfstudio.plugins.types import MethodSpecification
@@ -30,22 +32,41 @@
     from importlib.metadata import entry_points
 CONSOLE = Console(width=120)
 
 
 def discover_methods() -> t.Tuple[t.Dict[str, TrainerConfig], t.Dict[str, str]]:
     """
     Discovers all methods registered using the `nerfstudio.method_configs` entrypoint.
+    And also methods in the NERFSTUDIO_METHOD_CONFIGS environment variable.
     """
     methods = {}
     descriptions = {}
     discovered_entry_points = entry_points(group="nerfstudio.method_configs")
     for name in discovered_entry_points.names:
         specification = discovered_entry_points[name].load()
         if not isinstance(specification, MethodSpecification):
             CONSOLE.print(
                 "[bold yellow]Warning: Could not entry point {n} as it is not an instance of MethodSpecification"
             )
             continue
         specification = t.cast(MethodSpecification, specification)
         methods[specification.config.method_name] = specification.config
         descriptions[specification.config.method_name] = specification.description
+
+    if "NERFSTUDIO_METHOD_CONFIGS" in os.environ:
+        try:
+            strings = os.environ["NERFSTUDIO_METHOD_CONFIGS"].split(",")
+            for definition in strings:
+                if not definition:
+                    continue
+                name, path = definition.split("=")
+                CONSOLE.print(f"[bold green]Info: Loading method {name} from environment variable")
+                module, config_name = path.split(":")
+                method_config = getattr(importlib.import_module(module), config_name)
+                assert isinstance(method_config, MethodSpecification)
+                methods[name] = method_config.config
+                descriptions[name] = method_config.description
+        except Exception:  # pylint: disable=broad-except
+            CONSOLE.print_exception()
+            CONSOLE.print("[bold red]Error: Could not load methods from environment variable NERFSTUDIO_METHOD_CONFIGS")
+
     return methods, descriptions
```

### Comparing `nerfstudio-0.2.1/nerfstudio/plugins/types.py` & `nerfstudio-0.2.2/nerfstudio/plugins/types.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-0.2.1/nerfstudio/process_data/__init__.py` & `nerfstudio-0.2.2/nerfstudio/process_data/__init__.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-0.2.1/nerfstudio/process_data/colmap_utils.py` & `nerfstudio-0.2.2/nerfstudio/process_data/colmap_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """
-Tools supporting the execution of COLMAP and preparation of COLMAP-based datasets for nerstudio training.
+Tools supporting the execution of COLMAP and preparation of COLMAP-based datasets for nerfstudio training.
 """
 
 import json
 from pathlib import Path
 from typing import Any, Dict, Optional
 
 import appdirs
```

### Comparing `nerfstudio-0.2.1/nerfstudio/process_data/equirect_utils.py` & `nerfstudio-0.2.2/nerfstudio/process_data/equirect_utils.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-0.2.1/nerfstudio/process_data/hloc_utils.py` & `nerfstudio-0.2.2/nerfstudio/process_data/hloc_utils.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-0.2.1/nerfstudio/process_data/metashape_utils.py` & `nerfstudio-0.2.2/nerfstudio/process_data/metashape_utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -57,20 +57,25 @@
     chunk = root[0]
     sensors = chunk.find("sensors")
 
     # TODO Add support for per-frame intrinsics
     if sensors is None:
         raise ValueError("No sensors found")
 
-    calibrated_sensors = [sensor for sensor in sensors if sensor.find("calibration")]
+    calibrated_sensors = [
+        sensor for sensor in sensors if sensor.get("type") == "spherical" or sensor.find("calibration")
+    ]
     if not calibrated_sensors:
         raise ValueError("No calibrated sensor found in Metashape XML")
     sensor_type = [s.get("type") for s in calibrated_sensors]
     if sensor_type.count(sensor_type[0]) != len(sensor_type):
-        raise ValueError("All Metashape sensors do not have the same sensor type")
+        raise ValueError(
+            "All Metashape sensors do not have the same sensor type. "
+            "nerfstudio does not support per-frame camera_model."
+        )
     data = {}
     if sensor_type[0] == "frame":
         data["camera_model"] = CAMERA_MODELS["perspective"].value
     elif sensor_type[0] == "fisheye":
         data["camera_model"] = CAMERA_MODELS["fisheye"].value
     elif sensor_type[0] == "spherical":
         data["camera_model"] = CAMERA_MODELS["equirectangular"].value
@@ -83,26 +88,33 @@
         s = {}
         resolution = sensor.find("resolution")
         assert resolution is not None, "Resolution not found in Metashape xml"
         s["w"] = int(resolution.get("width"))  # type: ignore
         s["h"] = int(resolution.get("height"))  # type: ignore
 
         calib = sensor.find("calibration")
-        f = calib.find("f")
-        if f is not None:
+        if calib is None:
+            assert sensor_type[0] == "spherical", "Only spherical sensors should have no intrinsics"
+            s["fl_x"] = s["w"] / 2.0
+            s["fl_y"] = s["h"]
+            s["cx"] = s["w"] / 2.0
+            s["cy"] = s["h"] / 2.0
+        else:
+            f = calib.find("f")
+            assert f is not None, "Focal length not found in Metashape xml"
             s["fl_x"] = s["fl_y"] = float(f.text)  # type: ignore
-        s["cx"] = _find_param(calib, "cx") + s["w"] / 2.0  # type: ignore
-        s["cy"] = _find_param(calib, "cy") + s["h"] / 2.0  # type: ignore
+            s["cx"] = _find_param(calib, "cx") + s["w"] / 2.0  # type: ignore
+            s["cy"] = _find_param(calib, "cy") + s["h"] / 2.0  # type: ignore
 
-        s["k1"] = _find_param(calib, "k1")
-        s["k2"] = _find_param(calib, "k2")
-        s["k3"] = _find_param(calib, "k3")
-        s["k4"] = _find_param(calib, "k4")
-        s["p1"] = _find_param(calib, "p1")
-        s["p2"] = _find_param(calib, "p2")
+            s["k1"] = _find_param(calib, "k1")
+            s["k2"] = _find_param(calib, "k2")
+            s["k3"] = _find_param(calib, "k3")
+            s["k4"] = _find_param(calib, "k4")
+            s["p1"] = _find_param(calib, "p1")
+            s["p2"] = _find_param(calib, "p2")
 
         sensor_dict[sensor.get("id")] = s
 
     components = chunk.find("components")
     component_dict = {}
     for component in components:
         transform = component.find("transform")
```

### Comparing `nerfstudio-0.2.1/nerfstudio/process_data/polycam_utils.py` & `nerfstudio-0.2.2/nerfstudio/process_data/polycam_utils.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-0.2.1/nerfstudio/process_data/process_data_utils.py` & `nerfstudio-0.2.2/nerfstudio/process_data/process_data_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,20 +35,21 @@
 
 
 class CameraModel(Enum):
     """Enum for camera types."""
 
     OPENCV = "OPENCV"
     OPENCV_FISHEYE = "OPENCV_FISHEYE"
+    EQUIRECTANGULAR = "EQUIRECTANGULAR"
 
 
 CAMERA_MODELS = {
     "perspective": CameraModel.OPENCV,
     "fisheye": CameraModel.OPENCV_FISHEYE,
-    "equirectangular": CameraModel.OPENCV,
+    "equirectangular": CameraModel.EQUIRECTANGULAR,
 }
 
 
 def list_images(data: Path) -> List[Path]:
     """Lists all supported images in a directory
 
     Args:
```

### Comparing `nerfstudio-0.2.1/nerfstudio/process_data/realitycapture_utils.py` & `nerfstudio-0.2.2/nerfstudio/process_data/realitycapture_utils.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-0.2.1/nerfstudio/process_data/record3d_utils.py` & `nerfstudio-0.2.2/nerfstudio/process_data/record3d_utils.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-0.2.1/nerfstudio/utils/__init__.py` & `nerfstudio-0.2.2/nerfstudio/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-0.2.1/nerfstudio/utils/colormaps.py` & `nerfstudio-0.2.2/nerfstudio/utils/colormaps.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-0.2.1/nerfstudio/utils/colors.py` & `nerfstudio-0.2.2/nerfstudio/utils/colors.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-0.2.1/nerfstudio/utils/comms.py` & `nerfstudio-0.2.2/nerfstudio/utils/comms.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-0.2.1/nerfstudio/utils/decorators.py` & `nerfstudio-0.2.2/nerfstudio/utils/decorators.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-0.2.1/nerfstudio/utils/eval_utils.py` & `nerfstudio-0.2.2/nerfstudio/utils/eval_utils.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-0.2.1/nerfstudio/utils/install_checks.py` & `nerfstudio-0.2.2/nerfstudio/utils/install_checks.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-0.2.1/nerfstudio/utils/io.py` & `nerfstudio-0.2.2/nerfstudio/utils/io.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-0.2.1/nerfstudio/utils/math.py` & `nerfstudio-0.2.2/nerfstudio/utils/math.py`

 * *Files 6% similar despite different names*

```diff
@@ -17,16 +17,14 @@
 from dataclasses import dataclass
 from typing import Tuple
 
 import torch
 from torchtyping import TensorType
 from typing_extensions import Literal
 
-_USE_NERFACC = True
-
 
 def components_from_spherical_harmonics(levels: int, directions: TensorType[..., 3]) -> TensorType[..., "components"]:
     """
     Returns value for each component of spherical harmonics.
 
     Args:
         levels: Number of spherical harmonic levels to compute.
@@ -194,15 +192,15 @@
         torch.Tensor: The expected value of sin.
     """
 
     return torch.exp(-0.5 * x_vars) * torch.sin(x_means)
 
 
 @torch.jit.script
-def _intersect_aabb(
+def intersect_aabb(
     origins: torch.Tensor,
     directions: torch.Tensor,
     aabb: torch.Tensor,
     max_bound: float = 1e10,
     invalid_value: float = 1e10,
 ) -> Tuple[torch.Tensor, torch.Tensor]:
     """
@@ -234,48 +232,14 @@
     cond = t_max <= t_min
     t_min = torch.where(cond, invalid_value, t_min)
     t_max = torch.where(cond, invalid_value, t_max)
 
     return t_min, t_max
 
 
-def intersect_aabb(
-    origins: TensorType["N", 3],
-    directions: TensorType["N", 3],
-    aabb: TensorType[6],
-) -> Tuple[TensorType["N"], TensorType["N"]]:
-    """
-    Implementation of ray intersection with AABB box
-
-    Args:
-        origins: 3d positions
-        directions: Normalized directions
-        aabb: array of aabb box in the form of [x_min, y_min, z_min, x_max, y_max, z_max]
-        max_bound: Maximum value of t_max
-        invalid_value: Value to return in case of no intersection
-
-    Returns:
-        t_min, t_max - two tensors of shapes N representing distance of intersection from the origin.
-    """
-
-    global _USE_NERFACC  # pylint: disable=global-statement
-    if _USE_NERFACC:
-        try:
-            import nerfacc  # pylint: disable=import-outside-toplevel
-
-            t_min, t_max = nerfacc.ray_aabb_intersect(origins, directions, aabb)
-        except:  # pylint: disable=bare-except
-            t_min, t_max = _intersect_aabb(origins, directions, aabb, max_bound=1e10, invalid_value=1e10)
-            _USE_NERFACC = False
-    else:
-        t_min, t_max = _intersect_aabb(origins, directions, aabb, max_bound=1e10, invalid_value=1e10)
-
-    return t_min, t_max
-
-
 def safe_normalize(
     vectors: TensorType["batch_dim":..., "N"],
     eps: float = 1e-10,
 ) -> TensorType["batch_dim":..., "N"]:
     """Normalizes vectors.
 
     Args:
```

### Comparing `nerfstudio-0.2.1/nerfstudio/utils/misc.py` & `nerfstudio-0.2.2/nerfstudio/utils/misc.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-0.2.1/nerfstudio/utils/plotly_utils.py` & `nerfstudio-0.2.2/nerfstudio/utils/plotly_utils.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-0.2.1/nerfstudio/utils/poses.py` & `nerfstudio-0.2.2/nerfstudio/utils/poses.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-0.2.1/nerfstudio/utils/printing.py` & `nerfstudio-0.2.2/nerfstudio/utils/printing.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-0.2.1/nerfstudio/utils/profiler.py` & `nerfstudio-0.2.2/nerfstudio/utils/profiler.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,21 +16,21 @@
 Profiler base class and functionality
 """
 from __future__ import annotations
 
 import functools
 import os
 import time
+import typing
 from collections import deque
-from contextlib import contextmanager
+from contextlib import ContextDecorator, contextmanager
 from pathlib import Path
 from typing import Callable, Dict, List, Optional, Tuple, Union
 
 from rich.console import Console
-from torch.autograd.profiler import ContextDecorator
 from torch.profiler import ProfilerActivity, profile, record_function
 
 from nerfstudio.configs import base_config as cfg
 from nerfstudio.utils import comms
 from nerfstudio.utils.decorators import (
     check_main_thread,
     check_profiler_enabled,
@@ -42,16 +42,18 @@
 PROFILER = []
 PYTORCH_PROFILER = None
 
 
 class time_function(ContextDecorator):  # pylint: disable=invalid-name
     """Decorator/Context manager: time a function call or a block of code"""
 
-    def __init__(self, name: str):
-        self.name = name
+    def __init__(self, name: Union[str, Callable]):
+        # NOTE: This is a workaround for the fact that the __new__ method of a ContextDecorator
+        # is not picked up by VSCode intellisense
+        self.name: str = typing.cast(str, name)
         self.start = None
         self._profiler_contexts = deque()
         self._function_call_args: Optional[Tuple[Tuple, Dict]] = None
 
     def __new__(cls, func: Union[str, Callable]):
         instance = super().__new__(cls)
         if isinstance(func, str):
```

### Comparing `nerfstudio-0.2.1/nerfstudio/utils/rich_utils.py` & `nerfstudio-0.2.2/nerfstudio/utils/rich_utils.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-0.2.1/nerfstudio/utils/scripts.py` & `nerfstudio-0.2.2/nerfstudio/utils/scripts.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-0.2.1/nerfstudio/utils/tensor_dataclass.py` & `nerfstudio-0.2.2/nerfstudio/utils/tensor_dataclass.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-0.2.1/nerfstudio/utils/writer.py` & `nerfstudio-0.2.2/nerfstudio/utils/writer.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-0.2.1/nerfstudio/viewer/__init__.py` & `nerfstudio-0.2.2/nerfstudio/viewer/__init__.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-0.2.1/nerfstudio/viewer/app/package.json` & `nerfstudio-0.2.2/nerfstudio/viewer/app/package.json`

 * *Files 4% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9330357142857143%*

 * *Differences: {"'resolutions'": "{'babel-loader': '^9.1.2', 'json5': '^2.2.3', 'loader-utils': '^3.2.1', "*

 * *                  "'@pmmmwh/react-refresh-webpack-plugin': '^0.5.10', 'recursive-readdir': "*

 * *                  "'^2.2.3', 'resolve-url-loader': '^5.0.0', 'yaml': '^2.2.2'}",*

 * * "'version'": "'23-05-01-0'"}*

```diff
@@ -70,20 +70,27 @@
     },
     "homepage": ".",
     "license": "ISC",
     "main": "public/electron.js",
     "name": "viewer",
     "private": true,
     "resolutions": {
-        "nth-check": "^2.0.1"
+        "@pmmmwh/react-refresh-webpack-plugin": "^0.5.10",
+        "babel-loader": "^9.1.2",
+        "json5": "^2.2.3",
+        "loader-utils": "^3.2.1",
+        "nth-check": "^2.0.1",
+        "recursive-readdir": "^2.2.3",
+        "resolve-url-loader": "^5.0.0",
+        "yaml": "^2.2.2"
     },
     "scripts": {
         "build": "react-scripts build",
         "eject": "react-scripts eject",
         "electron": "electron .",
         "lint": "eslint --ext .js,.jsx .",
         "lint:fix": "eslint --fix --ext .js,.jsx .",
         "start": "react-scripts start",
         "test": "react-scripts test"
     },
-    "version": "23-04-18-0"
+    "version": "23-05-01-0"
 }
```

### Comparing `nerfstudio-0.2.1/nerfstudio/viewer/app/run_deploy.py` & `nerfstudio-0.2.2/nerfstudio/viewer/app/run_deploy.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-0.2.1/nerfstudio/viewer/app/src/themes/leva_theme.json` & `nerfstudio-0.2.2/nerfstudio/viewer/app/src/themes/leva_theme.json`

 * *Files identical despite different names*

### Comparing `nerfstudio-0.2.1/nerfstudio/viewer/server/__init__.py` & `nerfstudio-0.2.2/nerfstudio/viewer/server/__init__.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-0.2.1/nerfstudio/viewer/server/control_panel.py` & `nerfstudio-0.2.2/nerfstudio/viewer/server/control_panel.py`

 * *Files 0% similar despite different names*

```diff
@@ -49,27 +49,27 @@
         self._train_speed = ViewerDropdown(
             "Train Speed", "Balanced", ["Fast", "Balanced", "Slow"], cb_hook=lambda han: self._train_speed_cb()
         )
         self._output_render = ViewerDropdown(
             "Output Render",
             "not set",
             ["not set"],
-            cb_hook=lambda han: [self.update_control_panel(), rerender_cb(han), update_output_cb(han)],
+            cb_hook=lambda han: [self.update_control_panel(), update_output_cb(han), rerender_cb(han)],
         )
         self._colormap = ViewerDropdown("Colormap", "default", ["default"], cb_hook=rerender_cb)
         self._invert = ViewerCheckbox("| Invert", False, cb_hook=rerender_cb)
         self._normalize = ViewerCheckbox("| Normalize", False, cb_hook=rerender_cb)
         self._min = ViewerNumber("| Min", 0.0, cb_hook=rerender_cb)
         self._max = ViewerNumber("| Max", 1.0, cb_hook=rerender_cb)
         self._train_util = ViewerSlider("Train Util", 0.85, 0, 1, 0.05)
         self._max_res = ViewerSlider("Max Res", 512, 64, 2048, 100, cb_hook=rerender_cb)
         self._crop_viewport = ViewerCheckbox(
             "Crop Viewport",
             False,
-            cb_hook=lambda han: [self.update_control_panel(), rerender_cb(han), crop_update_cb(han)],
+            cb_hook=lambda han: [self.update_control_panel(), crop_update_cb(han), rerender_cb(han)],
         )
         self._background_color = ViewerRGB("| Background color", (38, 42, 55), cb_hook=crop_update_cb)
         self._crop_min = ViewerVec3("| Crop Min", (-1, -1, -1), 0.05, cb_hook=crop_update_cb)
         self._crop_max = ViewerVec3("| Crop Max", (1, 1, 1), 0.05, cb_hook=crop_update_cb)
         self._time = ViewerSlider("Time", 0.0, 0.0, 1.0, 0.01, cb_hook=rerender_cb)
         self._time_enabled = time_enabled
```

### Comparing `nerfstudio-0.2.1/nerfstudio/viewer/server/gui_utils.py` & `nerfstudio-0.2.2/nerfstudio/viewer/server/gui_utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -16,17 +16,14 @@
 
 from __future__ import annotations
 
 from typing import Any, List, Tuple
 
 from torch import nn
 
-from nerfstudio.pipelines.base_pipeline import Pipeline
-from nerfstudio.viewer.server.viewer_elements import ViewerElement
-
 
 def parse_object(
     obj: Any,
     type_check,
     tree_stub: str,
 ) -> List[Tuple[str, Any]]:
     """
@@ -64,18 +61,7 @@
             add(ret, new_tree_stub, v)
         elif isinstance(v, nn.Module):
             lower_rets = parse_object(v, type_check, new_tree_stub)
             # check that the values aren't already in the tree
             for ts, o in lower_rets:
                 add(ret, ts, o)
     return ret
-
-
-def get_viewer_elements(pipeline: Pipeline) -> List[Tuple[str, ViewerElement]]:
-    """
-    Recursively parse the pipeline object and return a tree of all the ViewerElements contained
-
-    returns a list of (path/to/object, param), which represents the path down the object tree as well as
-    the ViewerElement itself
-    """
-    ret = parse_object(pipeline, ViewerElement, "Custom")
-    return ret
```

### Comparing `nerfstudio-0.2.1/nerfstudio/viewer/server/path.py` & `nerfstudio-0.2.2/nerfstudio/viewer/server/path.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-0.2.1/nerfstudio/viewer/server/render_state_machine.py` & `nerfstudio-0.2.2/nerfstudio/viewer/server/render_state_machine.py`

 * *Files 4% similar despite different names*

```diff
@@ -75,14 +75,15 @@
         self.next_action: Optional[RenderAction] = None
         self.state: RenderStates = "low_static"
         self.render_trigger = threading.Event()
         self.target_fps = 24
         self.viewer = viewer
         self.interrupt_render_flag = False
         self.daemon = True
+        self.output_keys = {}
 
     def action(self, action: RenderAction):
         """Takes an action and updates the state machine
 
         Args:
             action: the action to take
         """
@@ -223,15 +224,19 @@
 
     def _send_output_to_viewer(self, outputs: Dict[str, Any]):
         """Chooses the correct output and sends it to the viewer
 
         Args:
             outputs: the dictionary of outputs to choose from, from the model
         """
-        self.viewer.control_panel.update_output_options(list(outputs.keys()))
+        output_keys = set(outputs.keys())
+        if self.output_keys != output_keys:
+            self.output_keys = output_keys
+            self.viewer.viser_server.send_output_options_message(list(outputs.keys()))
+            self.viewer.control_panel.update_output_options(list(outputs.keys()))
 
         output_render = self.viewer.control_panel.output_render
         self.viewer.update_colormap_options(
             dimensions=outputs[output_render].shape[-1], dtype=outputs[output_render].dtype
         )
         selected_output = (viewer_utils.apply_colormap(self.viewer.control_panel, outputs) * 255).type(torch.uint8)
```

### Comparing `nerfstudio-0.2.1/nerfstudio/viewer/server/state/node.py` & `nerfstudio-0.2.2/nerfstudio/viewer/server/state/node.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-0.2.1/nerfstudio/viewer/server/state/state_node.py` & `nerfstudio-0.2.2/nerfstudio/viewer/server/state/state_node.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-0.2.1/nerfstudio/viewer/server/utils.py` & `nerfstudio-0.2.2/nerfstudio/viewer/server/utils.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-0.2.1/nerfstudio/viewer/server/viewer_elements.py` & `nerfstudio-0.2.2/nerfstudio/viewer/server/viewer_elements.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-0.2.1/nerfstudio/viewer/server/viewer_state.py` & `nerfstudio-0.2.2/nerfstudio/viewer/server/viewer_state.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,15 +33,15 @@
 from nerfstudio.models.base_model import Model
 from nerfstudio.pipelines.base_pipeline import Pipeline
 from nerfstudio.utils.decorators import check_main_thread, decorate_all
 from nerfstudio.utils.io import load_from_json, write_to_json
 from nerfstudio.utils.writer import GLOBAL_BUFFER, EventName
 from nerfstudio.viewer.server import viewer_utils
 from nerfstudio.viewer.server.control_panel import ControlPanel
-from nerfstudio.viewer.server.gui_utils import get_viewer_elements
+from nerfstudio.viewer.server.gui_utils import parse_object
 from nerfstudio.viewer.server.render_state_machine import (
     RenderAction,
     RenderStateMachine,
 )
 from nerfstudio.viewer.server.viewer_elements import ViewerElement
 from nerfstudio.viewer.viser import ViserServer
 from nerfstudio.viewer.viser.messages import (
@@ -118,15 +118,15 @@
         self.output_type_changed = True
         self.step = 0
         self.train_btn_state: Literal["training", "paused", "completed"] = "training"
         self._prev_train_state: Literal["training", "paused", "completed"] = "training"
 
         self.camera_message = None
 
-        self.viser_server = ViserServer(host="127.0.0.1", port=websocket_port)
+        self.viser_server = ViserServer(host=config.websocket_host, port=websocket_port)
 
         self.viser_server.register_handler(TrainingStateMessage, self._handle_training_state_message)
         self.viser_server.register_handler(SaveCheckpointMessage, self._handle_save_checkpoint)
         self.viser_server.register_handler(CameraMessage, self._handle_camera_update)
         self.viser_server.register_handler(CameraPathOptionsRequest, self._handle_camera_path_option_request)
         self.viser_server.register_handler(CameraPathPayloadMessage, self._handle_camera_path_payload)
         self.viser_server.register_handler(CropParamsMessage, self._handle_crop_params_message)
@@ -145,15 +145,19 @@
                 # also rewire the hook to rerender
                 prev_cb = element.cb_hook
                 element.cb_hook = lambda element: [self._interrupt_render(element), prev_cb(element)]
             else:
                 with self.viser_server.gui_folder(folder_labels[0]):
                     nested_folder_install(folder_labels[1:], element)
 
-        self.viewer_elements = get_viewer_elements(self.pipeline)
+        self.viewer_elements = []
+        if self.trainer is not None:
+            self.viewer_elements.extend(parse_object(self.trainer, ViewerElement, "Trainer"))
+        else:
+            self.viewer_elements.extend(parse_object(pipeline, ViewerElement, "Pipeline"))
         for param_path, element in self.viewer_elements:
             folder_labels = param_path.split("/")[:-1]
             nested_folder_install(folder_labels, element)
 
         self.render_statemachine = RenderStateMachine(self)
         self.render_statemachine.start()
 
@@ -169,15 +173,15 @@
         """Update crop parameters"""
         self.render_statemachine.action(RenderAction("rerender", self.camera_message))
         crop_min = torch.tensor(self.control_panel.crop_min, dtype=torch.float32)
         crop_max = torch.tensor(self.control_panel.crop_max, dtype=torch.float32)
         scene_box = SceneBox(aabb=torch.stack([crop_min, crop_max], dim=0))
         self.viser_server.update_scene_box(scene_box)
         crop_scale = crop_max - crop_min
-        crop_center = crop_max + crop_min
+        crop_center = (crop_max + crop_min) / 2.0
         self.viser_server.send_crop_params(
             crop_enabled=self.control_panel.crop_viewport,
             crop_bg_color=self.control_panel.background_color,
             crop_scale=tuple(crop_scale.tolist()),
             crop_center=tuple(crop_center.tolist()),
         )
```

### Comparing `nerfstudio-0.2.1/nerfstudio/viewer/server/viewer_utils.py` & `nerfstudio-0.2.2/nerfstudio/viewer/server/viewer_utils.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-0.2.1/nerfstudio/viewer/viser/__init__.py` & `nerfstudio-0.2.2/nerfstudio/viewer/viser/__init__.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-0.2.1/nerfstudio/viewer/viser/gui.py` & `nerfstudio-0.2.2/nerfstudio/viewer/viser/gui.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-0.2.1/nerfstudio/viewer/viser/message_api.py` & `nerfstudio-0.2.2/nerfstudio/viewer/viser/message_api.py`

 * *Files 5% similar despite different names*

```diff
@@ -481,14 +481,22 @@
 
         Args:
             eval_res: The resolution of the render in plain text.
             step: The current step.
         """
         self._queue(messages.StatusMessage(eval_res=eval_res, step=step))
 
+    def send_output_options_message(self, options: List[str]):
+        """Send output options message
+
+        Args:
+            options: The list of output options
+        """
+        self._queue(messages.OutputOptionsMessage(options=options))
+
     def _add_gui_impl(
         self,
         name: str,
         initial_value: T,
         leva_conf: dict,
         is_button: bool = False,
         encoder: Callable[[T], Any] = lambda x: x,
```

### Comparing `nerfstudio-0.2.1/nerfstudio/viewer/viser/messages.py` & `nerfstudio-0.2.2/nerfstudio/viewer/viser/messages.py`

 * *Files 1% similar despite different names*

```diff
@@ -41,15 +41,15 @@
 
 
 @dataclasses.dataclass
 class GuiAddMessage(NerfstudioMessage):
     """Sent server->client to add a new GUI input."""
 
     name: str
-    folder_labels: Tuple[str]
+    folder_labels: Tuple[str, ...]
     leva_conf: Any
 
     @override
     def redundancy_key(self) -> str:
         return f"{type(self).__name__}_{self.name}"
 
 
@@ -237,7 +237,17 @@
 
 @dataclasses.dataclass
 class TimeConditionMessage(NerfstudioMessage):
     """Time conditioning message."""
 
     time: float
     """ Time conditioning value """
+
+
+@dataclasses.dataclass
+class OutputOptionsMessage(NerfstudioMessage):
+    """Output options message which are used in the export panel.
+    TODO: remove when export panel is becomes python defined.
+    """
+
+    options: Any
+    """ List of output option strings"""
```

### Comparing `nerfstudio-0.2.1/nerfstudio/viewer/viser/server.py` & `nerfstudio-0.2.2/nerfstudio/viewer/viser/server.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-0.2.1/nerfstudio.egg-info/PKG-INFO` & `nerfstudio-0.2.2/nerfstudio.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nerfstudio
-Version: 0.2.1
+Version: 0.2.2
 Summary: All-in-one repository for state-of-the-art NeRFs
 License: Apache 2.0
 Project-URL: Documentation, https://docs.nerf.studio
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python
 Requires-Python: >=3.7.3
 Description-Content-Type: text/markdown
@@ -62,20 +62,22 @@
 
 - [Quickstart](#quickstart)
 - [Learn more](#learn-more)
 - [Supported Features](#supported-features)
 
 # About
 
+_It’s as simple as plug and play with nerfstudio!_
+
 Nerfstudio provides a simple API that allows for a simplified end-to-end process of creating, training, and testing NeRFs.
 The library supports a **more interpretable implementation of NeRFs by modularizing each component.**
 With more modular NeRFs, we hope to create a more user-friendly experience in exploring the technology.
-Nerfstudio is a contributor-friendly repo with the goal of building a community where users can more easily build upon each other's contributions.
 
-It’s as simple as plug and play with nerfstudio!
+This is a contributor-friendly repo with the goal of building a community where users can more easily build upon each other's contributions.
+Nerfstudio initially launched as an opensource project by Berkeley students in [KAIR lab](https://people.eecs.berkeley.edu/~kanazawa/index.html#kair) at [Berkeley AI Research (BAIR)](https://bair.berkeley.edu/) in October 2022 as a part of a research project ([paper](https://arxiv.org/abs/2302.04264)). It is currently developed by Berkeley students and community contributors.
 
 We are committed to providing learning resources to help you understand the basics of (if you're just getting started), and keep up-to-date with (if you're a seasoned veteran) all things NeRF. As researchers, we know just how hard it is to get onboarded with this next-gen technology. So we're here to help with tutorials, documentation, and more!
 
 Have feature requests? Want to add your brand-spankin'-new NeRF model? Have a new dataset? **We welcome any and all [contributions](https://docs.nerf.studio/en/latest/reference/contributing.html)!** Please do not hesitate to reach out to the nerfstudio team with any questions via [Discord](https://discord.gg/uMbNqcraFc).
 
 We hope nerfstudio enables you to build faster :hammer: learn together :books: and contribute to our NeRF community :sparkling_heart:.
 
@@ -231,17 +233,17 @@
 
 Each model contains many parameters that can be changed, too many to list here. Use the `--help` command to see the full list of configuration options.
 
 ```bash
 ns-train nerfacto --help
 ```
 
-### Tensorboard / WandB
+### Tensorboard / WandB / Viewer
 
-We support three different methods to track training progress, using the viewer, [tensorboard](https://www.tensorflow.org/tensorboard), and [Weights and Biases](https://wandb.ai/site). You can specify which visualizer to use by appending `--vis {viewer, tensorboard, wandb}` to the training command. Note that only one may be used at a time. Additionally the viewer only works for methods that are fast (ie. nerfacto, instant-ngp), for slower methods like NeRF, use the other loggers.
+We support three different methods to track training progress, using the viewer, [tensorboard](https://www.tensorflow.org/tensorboard), and [Weights and Biases](https://wandb.ai/site). You can specify which visualizer to use by appending `--vis {viewer, tensorboard, wandb, viewer+wandb, viewer+tensorboard}` to the training command. Simultaneously utilizing the viewer alongside wandb or tensorboard may cause stuttering issues during evaluation steps. The viewer only works for methods that are fast (ie. nerfacto, instant-ngp), for slower methods like NeRF, use the other loggers.
 
 # Learn More
 
 And that's it for getting started with the basics of nerfstudio.
 
 If you're interested in learning more on how to create your own pipelines, develop with the viewer, run benchmarks, and more, please check out some of the quicklinks below or visit our [documentation](https://docs.nerf.studio/en/latest/) directly.
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nerfstudio Version: 0.2.1 Summary: All-in-one
+Metadata-Version: 2.1 Name: nerfstudio Version: 0.2.2 Summary: All-in-one
 repository for state-of-the-art NeRFs License: Apache 2.0 Project-URL:
 Documentation, https://docs.nerf.studio Classifier: Development Status :: 3 -
 Alpha Classifier: Programming Language :: Python Requires-Python: >=3.7.3
 Description-Content-Type: text/markdown Provides-Extra: gen Provides-Extra: dev
 Provides-Extra: docs License-File: LICENSE
  [https://img.shields.io/badge/Join-Discord-blue.svg]  [Documentation_Status]
         [PyPI_version]  [Test_Status] [Viewer_build_Status]  [License]
@@ -10,23 +10,28 @@
 
                    A collaboration friendly studio for NeRFs
                        [documentation] [viewer] [colab]
 [https://user-images.githubusercontent.com/3310961/194017985-ade69503-9d68-
 46a2-b518-2db1a012f090.gif] [https://user-images.githubusercontent.com/3310961/
 194020648-7e5f380c-15ca-461d-8c1c-20beb586defe.gif] - [Quickstart](#quickstart)
 - [Learn more](#learn-more) - [Supported Features](#supported-features) # About
-Nerfstudio provides a simple API that allows for a simplified end-to-end
-process of creating, training, and testing NeRFs. The library supports a **more
-interpretable implementation of NeRFs by modularizing each component.** With
-more modular NeRFs, we hope to create a more user-friendly experience in
-exploring the technology. Nerfstudio is a contributor-friendly repo with the
-goal of building a community where users can more easily build upon each
-other's contributions. Itâs as simple as plug and play with nerfstudio! We
-are committed to providing learning resources to help you understand the basics
-of (if you're just getting started), and keep up-to-date with (if you're a
+_Itâs as simple as plug and play with nerfstudio!_ Nerfstudio provides a
+simple API that allows for a simplified end-to-end process of creating,
+training, and testing NeRFs. The library supports a **more interpretable
+implementation of NeRFs by modularizing each component.** With more modular
+NeRFs, we hope to create a more user-friendly experience in exploring the
+technology. This is a contributor-friendly repo with the goal of building a
+community where users can more easily build upon each other's contributions.
+Nerfstudio initially launched as an opensource project by Berkeley students in
+[KAIR lab](https://people.eecs.berkeley.edu/~kanazawa/index.html#kair) at
+[Berkeley AI Research (BAIR)](https://bair.berkeley.edu/) in October 2022 as a
+part of a research project ([paper](https://arxiv.org/abs/2302.04264)). It is
+currently developed by Berkeley students and community contributors. We are
+committed to providing learning resources to help you understand the basics of
+(if you're just getting started), and keep up-to-date with (if you're a
 seasoned veteran) all things NeRF. As researchers, we know just how hard it is
 to get onboarded with this next-gen technology. So we're here to help with
 tutorials, documentation, and more! Have feature requests? Want to add your
 brand-spankin'-new NeRF model? Have a new dataset? **We welcome any and all
 [contributions](https://docs.nerf.studio/en/latest/reference/
 contributing.html)!** Please do not hesitate to reach out to the nerfstudio
 team with any questions via [Discord](https://discord.gg/uMbNqcraFc). We hope
@@ -125,68 +130,69 @@
 Poses | ð | ## 5. Advanced Options ### Training models other than nerfacto
 We provide other models than nerfacto, for example if you want to train the
 original nerf model, use the following command ```bash ns-train vanilla-nerf --
 data DATA_PATH ``` For a full list of included models run `ns-train --help`.
 ### Modify Configuration Each model contains many parameters that can be
 changed, too many to list here. Use the `--help` command to see the full list
 of configuration options. ```bash ns-train nerfacto --help ``` ### Tensorboard
-/ WandB We support three different methods to track training progress, using
-the viewer, [tensorboard](https://www.tensorflow.org/tensorboard), and [Weights
-and Biases](https://wandb.ai/site). You can specify which visualizer to use by
-appending `--vis {viewer, tensorboard, wandb}` to the training command. Note
-that only one may be used at a time. Additionally the viewer only works for
-methods that are fast (ie. nerfacto, instant-ngp), for slower methods like
-NeRF, use the other loggers. # Learn More And that's it for getting started
-with the basics of nerfstudio. If you're interested in learning more on how to
-create your own pipelines, develop with the viewer, run benchmarks, and more,
-please check out some of the quicklinks below or visit our [documentation]
-(https://docs.nerf.studio/en/latest/) directly. | Section | Description | | ---
+/ WandB / Viewer We support three different methods to track training progress,
+using the viewer, [tensorboard](https://www.tensorflow.org/tensorboard), and
+[Weights and Biases](https://wandb.ai/site). You can specify which visualizer
+to use by appending `--vis {viewer, tensorboard, wandb, viewer+wandb,
+viewer+tensorboard}` to the training command. Simultaneously utilizing the
+viewer alongside wandb or tensorboard may cause stuttering issues during
+evaluation steps. The viewer only works for methods that are fast (ie.
+nerfacto, instant-ngp), for slower methods like NeRF, use the other loggers. #
+Learn More And that's it for getting started with the basics of nerfstudio. If
+you're interested in learning more on how to create your own pipelines, develop
+with the viewer, run benchmarks, and more, please check out some of the
+quicklinks below or visit our [documentation](https://docs.nerf.studio/en/
+latest/) directly. | Section | Description | | --------------------------------
+------------------------------------------------------------------ | ----------
 -------------------------------------------------------------------------------
----------------- | ------------------------------------------------------------
--------------------------------------- | | [Documentation](https://
-docs.nerf.studio/en/latest/) | Full API documentation and tutorials | |
-[Viewer](https://viewer.nerf.studio/) | Home page for our web viewer | | ð
-**Educational** | | [Model Descriptions](https://docs.nerf.studio/en/latest/
-nerfology/methods/index.html) | Description of all the models supported by
-nerfstudio and explanations of component parts. | | [Component Descriptions]
-(https://docs.nerf.studio/en/latest/nerfology/model_components/index.html) |
-Interactive notebooks that explain notable/commonly used modules in various
-models. | | ð **Tutorials** | | [Getting Started](https://docs.nerf.studio/
-en/latest/quickstart/installation.html) | A more in-depth guide on how to get
-started with nerfstudio from installation to contributing. | | [Using the
-Viewer](https://docs.nerf.studio/en/latest/quickstart/viewer_quickstart.html) |
-A quick demo video on how to navigate the viewer. | | [Using Record3D](https://
-www.youtube.com/watch?v=XwKq7qDQCQk) | Demo video on how to run nerfstudio
-without using COLMAP. | | ð» **For Developers** | | [Creating pipelines]
-(https://docs.nerf.studio/en/latest/developer_guides/pipelines/index.html) |
-Learn how to easily build new neural rendering pipelines by using and/or
-implementing new modules. | | [Creating datasets](https://docs.nerf.studio/en/
-latest/quickstart/custom_dataset.html) | Have a new dataset? Learn how to run
-it with nerfstudio. | | [Contributing](https://docs.nerf.studio/en/latest/
-reference/contributing.html) | Walk-through for how you can start contributing
-now. | | ð **Community** | | [Discord](https://discord.gg/uMbNqcraFc) | Join
-our community to discuss more. We would love to hear from you! | | [Twitter]
-(https://twitter.com/nerfstudioteam) | Follow us on Twitter @nerfstudioteam to
-see cool updates and announcements | # Supported Features We provide the
-following support structures to make life easier for getting started with
-NeRFs. **If you are looking for a feature that is not currently supported,
-please do not hesitate to contact the Nerfstudio Team on [Discord](https://
-discord.gg/uMbNqcraFc)!** - :mag_right: Web-based visualizer that allows you
-to: - Visualize training in real-time + interact with the scene - Create and
-render out scenes with custom camera trajectories - View different output types
-- And more! - :pencil2: Support for multiple logging interfaces (Tensorboard,
-Wandb), code profiling, and other built-in debugging tools - :
-chart_with_upwards_trend: Easy-to-use benchmarking scripts on the Blender
-dataset - :iphone: Full pipeline support (w/ Colmap, Polycam, or Record3D) for
-going from a video on your phone to a full 3D render. # Built On [tyro_logo] -
-Easy-to-use config system - Developed by [Brent Yi](https://brentyi.com/) [tyro
-logo] - Library for accelerating NeRF renders - Developed by [Ruilong Li]
-(https://www.liruilong.cn/) # Citation You can find a paper writeup of the
-framework on [arXiv](https://arxiv.org/abs/2302.04264). If you use this library
-or find the documentation useful for your research, please consider citing: ```
-@article{nerfstudio, author = {Tancik, Matthew and Weber, Ethan and Ng, Evonne
-and Li, Ruilong and Yi, Brent and Kerr, Justin and Wang, Terrance and
-Kristoffersen, Alexander and Austin, Jake and Salahi, Kamyar and Ahuja, Abhik
-and McAllister, David and Kanazawa, Angjoo}, title = {Nerfstudio: A Modular
-Framework for Neural Radiance Field Development}, journal = {arXiv preprint
-arXiv:2302.04264}, year = {2023}, } ``` # Contributors [https://contrib.rocks/
-image?repo=nerfstudio-project/nerfstudio]
+--------- | | [Documentation](https://docs.nerf.studio/en/latest/) | Full API
+documentation and tutorials | | [Viewer](https://viewer.nerf.studio/) | Home
+page for our web viewer | | ð **Educational** | | [Model Descriptions]
+(https://docs.nerf.studio/en/latest/nerfology/methods/index.html) | Description
+of all the models supported by nerfstudio and explanations of component parts.
+| | [Component Descriptions](https://docs.nerf.studio/en/latest/nerfology/
+model_components/index.html) | Interactive notebooks that explain notable/
+commonly used modules in various models. | | ð **Tutorials** | | [Getting
+Started](https://docs.nerf.studio/en/latest/quickstart/installation.html) | A
+more in-depth guide on how to get started with nerfstudio from installation to
+contributing. | | [Using the Viewer](https://docs.nerf.studio/en/latest/
+quickstart/viewer_quickstart.html) | A quick demo video on how to navigate the
+viewer. | | [Using Record3D](https://www.youtube.com/watch?v=XwKq7qDQCQk) |
+Demo video on how to run nerfstudio without using COLMAP. | | ð» **For
+Developers** | | [Creating pipelines](https://docs.nerf.studio/en/latest/
+developer_guides/pipelines/index.html) | Learn how to easily build new neural
+rendering pipelines by using and/or implementing new modules. | | [Creating
+datasets](https://docs.nerf.studio/en/latest/quickstart/custom_dataset.html) |
+Have a new dataset? Learn how to run it with nerfstudio. | | [Contributing]
+(https://docs.nerf.studio/en/latest/reference/contributing.html) | Walk-through
+for how you can start contributing now. | | ð **Community** | | [Discord]
+(https://discord.gg/uMbNqcraFc) | Join our community to discuss more. We would
+love to hear from you! | | [Twitter](https://twitter.com/nerfstudioteam) |
+Follow us on Twitter @nerfstudioteam to see cool updates and announcements | #
+Supported Features We provide the following support structures to make life
+easier for getting started with NeRFs. **If you are looking for a feature that
+is not currently supported, please do not hesitate to contact the Nerfstudio
+Team on [Discord](https://discord.gg/uMbNqcraFc)!** - :mag_right: Web-based
+visualizer that allows you to: - Visualize training in real-time + interact
+with the scene - Create and render out scenes with custom camera trajectories -
+View different output types - And more! - :pencil2: Support for multiple
+logging interfaces (Tensorboard, Wandb), code profiling, and other built-in
+debugging tools - :chart_with_upwards_trend: Easy-to-use benchmarking scripts
+on the Blender dataset - :iphone: Full pipeline support (w/ Colmap, Polycam, or
+Record3D) for going from a video on your phone to a full 3D render. # Built On
+[tyro_logo] - Easy-to-use config system - Developed by [Brent Yi](https://
+brentyi.com/) [tyro_logo] - Library for accelerating NeRF renders - Developed
+by [Ruilong Li](https://www.liruilong.cn/) # Citation You can find a paper
+writeup of the framework on [arXiv](https://arxiv.org/abs/2302.04264). If you
+use this library or find the documentation useful for your research, please
+consider citing: ``` @article{nerfstudio, author = {Tancik, Matthew and Weber,
+Ethan and Ng, Evonne and Li, Ruilong and Yi, Brent and Kerr, Justin and Wang,
+Terrance and Kristoffersen, Alexander and Austin, Jake and Salahi, Kamyar and
+Ahuja, Abhik and McAllister, David and Kanazawa, Angjoo}, title = {Nerfstudio:
+A Modular Framework for Neural Radiance Field Development}, journal = {arXiv
+preprint arXiv:2302.04264}, year = {2023}, } ``` # Contributors [https://
+contrib.rocks/image?repo=nerfstudio-project/nerfstudio]
```

### Comparing `nerfstudio-0.2.1/nerfstudio.egg-info/SOURCES.txt` & `nerfstudio-0.2.2/nerfstudio.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -72,14 +72,16 @@
 nerfstudio/field_components/field_heads.py
 nerfstudio/field_components/mlp.py
 nerfstudio/field_components/spatial_distortions.py
 nerfstudio/field_components/temporal_distortions.py
 nerfstudio/field_components/temporal_grid.py
 nerfstudio/field_components/cuda/__init__.py
 nerfstudio/field_components/cuda/_backend.py
+nerfstudio/field_components/cuda/csrc/pybind.cu
+nerfstudio/field_components/cuda/csrc/temporal_gridencoder.cu
 nerfstudio/fields/__init__.py
 nerfstudio/fields/base_field.py
 nerfstudio/fields/density_fields.py
 nerfstudio/fields/instant_ngp_field.py
 nerfstudio/fields/nerfacto_field.py
 nerfstudio/fields/nerfplayer_nerfacto_field.py
 nerfstudio/fields/nerfplayer_ngp_field.py
@@ -114,22 +116,26 @@
 nerfstudio/pipelines/__init__.py
 nerfstudio/pipelines/base_pipeline.py
 nerfstudio/pipelines/dynamic_batch.py
 nerfstudio/plugins/__init__.py
 nerfstudio/plugins/registry.py
 nerfstudio/plugins/types.py
 nerfstudio/process_data/__init__.py
+nerfstudio/process_data/base_converter_to_nerfstudio_dataset.py
+nerfstudio/process_data/colmap_converter_to_nerfstudio_dataset.py
 nerfstudio/process_data/colmap_utils.py
 nerfstudio/process_data/equirect_utils.py
 nerfstudio/process_data/hloc_utils.py
+nerfstudio/process_data/images_to_nerfstudio_dataset.py
 nerfstudio/process_data/metashape_utils.py
 nerfstudio/process_data/polycam_utils.py
 nerfstudio/process_data/process_data_utils.py
 nerfstudio/process_data/realitycapture_utils.py
 nerfstudio/process_data/record3d_utils.py
+nerfstudio/process_data/video_to_nerfstudio_dataset.py
 nerfstudio/utils/__init__.py
 nerfstudio/utils/colormaps.py
 nerfstudio/utils/colors.py
 nerfstudio/utils/comms.py
 nerfstudio/utils/decorators.py
 nerfstudio/utils/eval_utils.py
 nerfstudio/utils/install_checks.py
```

### Comparing `nerfstudio-0.2.1/nerfstudio.egg-info/entry_points.txt` & `nerfstudio-0.2.2/nerfstudio.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `nerfstudio-0.2.1/nerfstudio.egg-info/requires.txt` & `nerfstudio-0.2.2/nerfstudio.egg-info/requires.txt`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 imageio>=2.21.1
 ipywidgets>=7.6
 jupyterlab>=3.3.4
 matplotlib>=3.5.3
 mediapy>=1.1.0
 msgpack>=1.0.4
 msgpack_numpy>=0.4.8
-nerfacc==0.3.5
+nerfacc==0.5.2
 open3d>=0.16.0
 opencv-python==4.6.0.66
 Pillow>=9.3.0
 plotly>=5.7.0
 protobuf!=3.20.0,<=3.20.3
 pyequilib>=0.5.6
 pymeshlab>=2022.2.post2
```

### Comparing `nerfstudio-0.2.1/pyproject.toml` & `nerfstudio-0.2.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "nerfstudio"
-version = "0.2.1"
+version = "0.2.2"
 description = "All-in-one repository for state-of-the-art NeRFs"
 readme = "README.md"
 license = { text="Apache 2.0"}
 requires-python = ">=3.7.3"
 classifiers = [
     "Development Status :: 3 - Alpha",
     "Programming Language :: Python",
@@ -26,15 +26,15 @@
     'importlib-metadata>=6.0.0; python_version < "3.10"',
     "ipywidgets>=7.6",
     "jupyterlab>=3.3.4",
     "matplotlib>=3.5.3",
     "mediapy>=1.1.0",
     "msgpack>=1.0.4",
     "msgpack_numpy>=0.4.8",
-    "nerfacc==0.3.5",
+    "nerfacc==0.5.2",
     "open3d>=0.16.0",
     "opencv-python==4.6.0.66",
     "Pillow>=9.3.0",
     "plotly>=5.7.0",
     "protobuf<=3.20.3,!=3.20.0",
     # TODO(1480) enable when pycolmap windows wheels are available
     # "pycolmap==0.3.0",
@@ -117,15 +117,15 @@
     "https://download.pytorch.org/whl/cu113"
 ]
 
 [tool.setuptools.packages.find]
 include = ["nerfstudio*","scripts*"]
 
 [tool.setuptools.package-data]
-"*" = ["*.json", "py.typed", "setup.bash", "setup.zsh"]
+"*" = ["*.cu", "*.json", "py.typed", "setup.bash", "setup.zsh"]
 
 # black
 [tool.black]
 line-length = 120
 
 # pylint
 [tool.pylint.messages_control]
```

### Comparing `nerfstudio-0.2.1/scripts/blender/nerfstudio_blender.py` & `nerfstudio-0.2.2/scripts/blender/nerfstudio_blender.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-0.2.1/scripts/completions/install.py` & `nerfstudio-0.2.2/scripts/completions/install.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-0.2.1/scripts/completions/setup.zsh` & `nerfstudio-0.2.2/scripts/completions/setup.zsh`

 * *Files identical despite different names*

### Comparing `nerfstudio-0.2.1/scripts/datasets/process_nuscenes_masks.py` & `nerfstudio-0.2.2/scripts/datasets/process_nuscenes_masks.py`

 * *Files 6% similar despite different names*

```diff
@@ -75,16 +75,19 @@
                 intrinsics = np.array(calibrated_sensor["camera_intrinsic"])
 
                 _, boxes, _ = nusc.get_sample_data(sample["data"][camera], box_vis_level=BoxVisibility.ANY)
                 # TODO: BoxVisibility.ANY misses boxes that are partially behind the camera leading to missed masks
                 # Instead use BoxVisibility.NONE and make sure to rasterize box faces correctly
 
                 mask = np.ones((900, 1600), dtype=np.uint8)
-                for box in boxes:
+                # If is backcam, mask the truck of the ego vehicle
+                if camera == "CAM_BACK":
+                    mask[-100:] = 0
 
+                for box in boxes:
                     # Dont mask out static objects (static in all frames)
                     instance_token = nusc.get("sample_annotation", box.token)["instance_token"]
                     if not instances_is_dynamic[instance_token]:
                         continue
 
                     # project box to image plane and rasterize each face
                     corners_3d = box.corners()
```

### Comparing `nerfstudio-0.2.1/scripts/docs/add_nb_tags.py` & `nerfstudio-0.2.2/scripts/docs/add_nb_tags.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-0.2.1/scripts/docs/build_docs.py` & `nerfstudio-0.2.2/scripts/docs/build_docs.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-0.2.1/scripts/downloads/download_data.py` & `nerfstudio-0.2.2/scripts/downloads/download_data.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-0.2.1/scripts/eval.py` & `nerfstudio-0.2.2/scripts/eval.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-0.2.1/scripts/exporter.py` & `nerfstudio-0.2.2/scripts/exporter.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-0.2.1/scripts/generative/trace_stable_diffusion.py` & `nerfstudio-0.2.2/scripts/generative/trace_stable_diffusion.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-0.2.1/scripts/github/run_actions.py` & `nerfstudio-0.2.2/scripts/github/run_actions.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-0.2.1/scripts/render.py` & `nerfstudio-0.2.2/scripts/render.py`

 * *Files 5% similar despite different names*

```diff
@@ -13,22 +13,25 @@
 from pathlib import Path
 from typing import Any, Dict, List, Optional
 
 import mediapy as media
 import numpy as np
 import torch
 import tyro
+from rich import box, style
 from rich.console import Console
+from rich.panel import Panel
 from rich.progress import (
     BarColumn,
     Progress,
     TaskProgressColumn,
     TextColumn,
     TimeRemainingColumn,
 )
+from rich.table import Table
 from torchtyping import TensorType
 from typing_extensions import Literal, assert_never
 
 from nerfstudio.cameras.camera_paths import (
     get_interpolated_camera_path,
     get_path_from_json,
     get_spiral_path,
@@ -76,16 +79,16 @@
     progress = Progress(
         TextColumn(":movie_camera: Rendering :movie_camera:"),
         BarColumn(),
         TaskProgressColumn(show_speed=True),
         ItersPerSecColumn(suffix="fps"),
         TimeRemainingColumn(elapsed_when_finished=True, compact=True),
     )
+    output_image_dir = output_filename.parent / output_filename.stem
     if output_format == "images":
-        output_image_dir = output_filename.parent / output_filename.stem
         output_image_dir.mkdir(parents=True, exist_ok=True)
     if output_format == "video":
         # make the folder if it doesn't exist
         output_filename.parent.mkdir(parents=True, exist_ok=True)
         # NOTE:
         # we could use ffmpeg_args "-movflags faststart" for progressive download,
         # which would force moov atom into known position before mdat,
@@ -139,17 +142,27 @@
                                 path=output_filename,
                                 shape=(render_height, render_width),
                                 fps=fps,
                             )
                         )
                     writer.add_image(render_image)
 
+    table = Table(
+        title=None,
+        show_header=False,
+        box=box.MINIMAL,
+        title_style=style.Style(bold=True),
+    )
     if output_format == "video":
         if camera_type == CameraType.EQUIRECTANGULAR:
             insert_spherical_metadata_into_file(output_filename)
+        table.add_row("Video", str(output_filename))
+    else:
+        table.add_row("Images", str(output_image_dir))
+    CONSOLE.print(Panel(table, title="[bold][green]:tada: Render Complete :tada:[/bold]", expand=False))
 
 
 def insert_spherical_metadata_into_file(
     output_filename: Path,
 ) -> None:
     """Inserts spherical metadata into MP4 video file in-place.
     Args:
```

### Comparing `nerfstudio-0.2.1/scripts/texture.py` & `nerfstudio-0.2.2/scripts/texture.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-0.2.1/scripts/train.py` & `nerfstudio-0.2.2/scripts/train.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-0.2.1/scripts/viewer/run_viewer.py` & `nerfstudio-0.2.2/scripts/viewer/run_viewer.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-0.2.1/tests/test_train.py` & `nerfstudio-0.2.2/tests/test_train.py`

 * *Files identical despite different names*

