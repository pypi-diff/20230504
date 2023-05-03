# Comparing `tmp/ultralytics-8.0.91.tar.gz` & `tmp/ultralytics-8.0.92.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ultralytics-8.0.91.tar", last modified: Mon May  1 20:21:39 2023, max compression
+gzip compressed data, was "ultralytics-8.0.92.tar", last modified: Wed May  3 23:28:53 2023, max compression
```

## Comparing `ultralytics-8.0.91.tar` & `ultralytics-8.0.92.tar`

### file list

```diff
@@ -1,179 +1,179 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 20:21:39.531917 ultralytics-8.0.91/
--rw-r--r--   0 runner    (1001) docker     (123)     5624 2023-05-01 20:20:18.000000 ultralytics-8.0.91/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-05-01 20:20:18.000000 ultralytics-8.0.91/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      213 2023-05-01 20:20:18.000000 ultralytics-8.0.91/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    25796 2023-05-01 20:21:39.531917 ultralytics-8.0.91/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    24235 2023-05-01 20:20:18.000000 ultralytics-8.0.91/README.md
--rw-r--r--   0 runner    (1001) docker     (123)    23225 2023-05-01 20:20:18.000000 ultralytics-8.0.91/README.zh-CN.md
--rw-r--r--   0 runner    (1001) docker     (123)     1107 2023-05-01 20:20:18.000000 ultralytics-8.0.91/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      682 2023-05-01 20:21:39.531917 ultralytics-8.0.91/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2875 2023-05-01 20:20:18.000000 ultralytics-8.0.91/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 20:21:39.511917 ultralytics-8.0.91/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     3165 2023-05-01 20:20:18.000000 ultralytics-8.0.91/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     4380 2023-05-01 20:20:18.000000 ultralytics-8.0.91/tests/test_engine.py
--rw-r--r--   0 runner    (1001) docker     (123)     7099 2023-05-01 20:20:18.000000 ultralytics-8.0.91/tests/test_python.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 20:21:39.511917 ultralytics-8.0.91/ultralytics/
--rw-r--r--   0 runner    (1001) docker     (123)      330 2023-05-01 20:20:18.000000 ultralytics-8.0.91/ultralytics/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 20:21:39.515917 ultralytics-8.0.91/ultralytics/assets/
--rw-r--r--   0 runner    (1001) docker     (123)   137419 2023-05-01 20:20:18.000000 ultralytics-8.0.91/ultralytics/assets/bus.jpg
--rw-r--r--   0 runner    (1001) docker     (123)    50427 2023-05-01 20:20:18.000000 ultralytics-8.0.91/ultralytics/assets/zidane.jpg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 20:21:39.515917 ultralytics-8.0.91/ultralytics/datasets/
--rw-r--r--   0 runner    (1001) docker     (123)     2751 2023-05-01 20:20:18.000000 ultralytics-8.0.91/ultralytics/datasets/Argoverse.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1918 2023-05-01 20:20:18.000000 ultralytics-8.0.91/ultralytics/datasets/GlobalWheat2020.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    42439 2023-05-01 20:20:18.000000 ultralytics-8.0.91/ultralytics/datasets/ImageNet.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     9270 2023-05-01 20:20:18.000000 ultralytics-8.0.91/ultralytics/datasets/Objects365.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2437 2023-05-01 20:20:18.000000 ultralytics-8.0.91/ultralytics/datasets/SKU-110K.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     3512 2023-05-01 20:20:18.000000 ultralytics-8.0.91/ultralytics/datasets/VOC.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     3012 2023-05-01 20:20:18.000000 ultralytics-8.0.91/ultralytics/datasets/VisDrone.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1547 2023-05-01 20:20:18.000000 ultralytics-8.0.91/ultralytics/datasets/coco-pose.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2526 2023-05-01 20:20:18.000000 ultralytics-8.0.91/ultralytics/datasets/coco.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1862 2023-05-01 20:20:18.000000 ultralytics-8.0.91/ultralytics/datasets/coco128-seg.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1846 2023-05-01 20:20:18.000000 ultralytics-8.0.91/ultralytics/datasets/coco128.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      895 2023-05-01 20:20:18.000000 ultralytics-8.0.91/ultralytics/datasets/coco8-pose.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1797 2023-05-01 20:20:18.000000 ultralytics-8.0.91/ultralytics/datasets/coco8-seg.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1777 2023-05-01 20:20:18.000000 ultralytics-8.0.91/ultralytics/datasets/coco8.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     5178 2023-05-01 20:20:18.000000 ultralytics-8.0.91/ultralytics/datasets/xView.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 20:21:39.515917 ultralytics-8.0.91/ultralytics/hub/
--rw-r--r--   0 runner    (1001) docker     (123)     3442 2023-05-01 20:20:18.000000 ultralytics-8.0.91/ultralytics/hub/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5209 2023-05-01 20:20:18.000000 ultralytics-8.0.91/ultralytics/hub/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)     8479 2023-05-01 20:20:18.000000 ultralytics-8.0.91/ultralytics/hub/session.py
--rw-r--r--   0 runner    (1001) docker     (123)     9157 2023-05-01 20:20:18.000000 ultralytics-8.0.91/ultralytics/hub/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 20:21:39.507917 ultralytics-8.0.91/ultralytics/models/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 20:21:39.519917 ultralytics-8.0.91/ultralytics/models/v3/
--rw-r--r--   0 runner    (1001) docker     (123)     1435 2023-05-01 20:20:18.000000 ultralytics-8.0.91/ultralytics/models/v3/yolov3-spp.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1136 2023-05-01 20:20:18.000000 ultralytics-8.0.91/ultralytics/models/v3/yolov3-tiny.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1426 2023-05-01 20:20:18.000000 ultralytics-8.0.91/ultralytics/models/v3/yolov3.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 20:21:39.519917 ultralytics-8.0.91/ultralytics/models/v5/
--rw-r--r--   0 runner    (1001) docker     (123)     1812 2023-05-01 20:20:18.000000 ultralytics-8.0.91/ultralytics/models/v5/yolov5-p6.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1439 2023-05-01 20:20:18.000000 ultralytics-8.0.91/ultralytics/models/v5/yolov5.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 20:21:39.519917 ultralytics-8.0.91/ultralytics/models/v8/
--rw-r--r--   0 runner    (1001) docker     (123)      920 2023-05-01 20:20:18.000000 ultralytics-8.0.91/ultralytics/models/v8/yolov8-cls.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1751 2023-05-01 20:20:18.000000 ultralytics-8.0.91/ultralytics/models/v8/yolov8-p2.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1856 2023-05-01 20:20:18.000000 ultralytics-8.0.91/ultralytics/models/v8/yolov8-p6.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1953 2023-05-01 20:20:18.000000 ultralytics-8.0.91/ultralytics/models/v8/yolov8-pose-p6.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1580 2023-05-01 20:20:18.000000 ultralytics-8.0.91/ultralytics/models/v8/yolov8-pose.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1490 2023-05-01 20:20:18.000000 ultralytics-8.0.91/ultralytics/models/v8/yolov8-seg.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1913 2023-05-01 20:20:18.000000 ultralytics-8.0.91/ultralytics/models/v8/yolov8.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 20:21:39.519917 ultralytics-8.0.91/ultralytics/nn/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 20:20:18.000000 ultralytics-8.0.91/ultralytics/nn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24243 2023-05-01 20:20:18.000000 ultralytics-8.0.91/ultralytics/nn/autobackend.py
--rw-r--r--   0 runner    (1001) docker     (123)    12509 2023-05-01 20:20:18.000000 ultralytics-8.0.91/ultralytics/nn/autoshape.py
--rw-r--r--   0 runner    (1001) docker     (123)    25079 2023-05-01 20:20:18.000000 ultralytics-8.0.91/ultralytics/nn/modules.py
--rw-r--r--   0 runner    (1001) docker     (123)    27170 2023-05-01 20:20:18.000000 ultralytics-8.0.91/ultralytics/nn/tasks.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 20:21:39.519917 ultralytics-8.0.91/ultralytics/tracker/
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-05-01 20:20:18.000000 ultralytics-8.0.91/ultralytics/tracker/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 20:21:39.519917 ultralytics-8.0.91/ultralytics/tracker/cfg/
--rw-r--r--   0 runner    (1001) docker     (123)      890 2023-05-01 20:20:18.000000 ultralytics-8.0.91/ultralytics/tracker/cfg/botsort.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      694 2023-05-01 20:20:18.000000 ultralytics-8.0.91/ultralytics/tracker/cfg/bytetrack.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2306 2023-05-01 20:20:18.000000 ultralytics-8.0.91/ultralytics/tracker/track.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 20:21:39.519917 ultralytics-8.0.91/ultralytics/tracker/trackers/
--rw-r--r--   0 runner    (1001) docker     (123)      171 2023-05-01 20:20:18.000000 ultralytics-8.0.91/ultralytics/tracker/trackers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1609 2023-05-01 20:20:18.000000 ultralytics-8.0.91/ultralytics/tracker/trackers/basetrack.py
--rw-r--r--   0 runner    (1001) docker     (123)     5684 2023-05-01 20:20:18.000000 ultralytics-8.0.91/ultralytics/tracker/trackers/bot_sort.py
--rw-r--r--   0 runner    (1001) docker     (123)    14448 2023-05-01 20:20:18.000000 ultralytics-8.0.91/ultralytics/tracker/trackers/byte_tracker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 20:21:39.519917 ultralytics-8.0.91/ultralytics/tracker/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 20:20:18.000000 ultralytics-8.0.91/ultralytics/tracker/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12214 2023-05-01 20:20:18.000000 ultralytics-8.0.91/ultralytics/tracker/utils/gmc.py
--rw-r--r--   0 runner    (1001) docker     (123)    18420 2023-05-01 20:20:18.000000 ultralytics-8.0.91/ultralytics/tracker/utils/kalman_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     8699 2023-05-01 20:20:18.000000 ultralytics-8.0.91/ultralytics/tracker/utils/matching.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 20:21:39.519917 ultralytics-8.0.91/ultralytics/vit/
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-05-01 20:20:18.000000 ultralytics-8.0.91/ultralytics/vit/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 20:21:39.523917 ultralytics-8.0.91/ultralytics/vit/sam/
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-05-01 20:20:18.000000 ultralytics-8.0.91/ultralytics/vit/sam/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13304 2023-05-01 20:20:18.000000 ultralytics-8.0.91/ultralytics/vit/sam/amg.py
--rw-r--r--   0 runner    (1001) docker     (123)     3878 2023-05-01 20:20:18.000000 ultralytics-8.0.91/ultralytics/vit/sam/autosize.py
--rw-r--r--   0 runner    (1001) docker     (123)     3686 2023-05-01 20:20:18.000000 ultralytics-8.0.91/ultralytics/vit/sam/build.py
--rw-r--r--   0 runner    (1001) docker     (123)     1450 2023-05-01 20:20:18.000000 ultralytics-8.0.91/ultralytics/vit/sam/model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 20:21:39.523917 ultralytics-8.0.91/ultralytics/vit/sam/modules/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 20:20:18.000000 ultralytics-8.0.91/ultralytics/vit/sam/modules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6347 2023-05-01 20:20:18.000000 ultralytics-8.0.91/ultralytics/vit/sam/modules/decoders.py
--rw-r--r--   0 runner    (1001) docker     (123)    22502 2023-05-01 20:20:18.000000 ultralytics-8.0.91/ultralytics/vit/sam/modules/encoders.py
--rw-r--r--   0 runner    (1001) docker     (123)    15281 2023-05-01 20:20:18.000000 ultralytics-8.0.91/ultralytics/vit/sam/modules/mask_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)    11201 2023-05-01 20:20:18.000000 ultralytics-8.0.91/ultralytics/vit/sam/modules/prompt_predictor.py
--rw-r--r--   0 runner    (1001) docker     (123)     7116 2023-05-01 20:20:18.000000 ultralytics-8.0.91/ultralytics/vit/sam/modules/sam.py
--rw-r--r--   0 runner    (1001) docker     (123)     8489 2023-05-01 20:20:18.000000 ultralytics-8.0.91/ultralytics/vit/sam/modules/transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2139 2023-05-01 20:20:18.000000 ultralytics-8.0.91/ultralytics/vit/sam/predict.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 20:21:39.523917 ultralytics-8.0.91/ultralytics/yolo/
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-05-01 20:20:18.000000 ultralytics-8.0.91/ultralytics/yolo/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 20:21:39.523917 ultralytics-8.0.91/ultralytics/yolo/cfg/
--rw-r--r--   0 runner    (1001) docker     (123)    17675 2023-05-01 20:20:18.000000 ultralytics-8.0.91/ultralytics/yolo/cfg/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6172 2023-05-01 20:20:18.000000 ultralytics-8.0.91/ultralytics/yolo/cfg/default.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 20:21:39.523917 ultralytics-8.0.91/ultralytics/yolo/data/
--rw-r--r--   0 runner    (1001) docker     (123)      458 2023-05-01 20:20:18.000000 ultralytics-8.0.91/ultralytics/yolo/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2250 2023-05-01 20:20:18.000000 ultralytics-8.0.91/ultralytics/yolo/data/annotator.py
--rw-r--r--   0 runner    (1001) docker     (123)    33512 2023-05-01 20:20:18.000000 ultralytics-8.0.91/ultralytics/yolo/data/augment.py
--rw-r--r--   0 runner    (1001) docker     (123)    11763 2023-05-01 20:20:18.000000 ultralytics-8.0.91/ultralytics/yolo/data/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     6556 2023-05-01 20:20:18.000000 ultralytics-8.0.91/ultralytics/yolo/data/build.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 20:21:39.523917 ultralytics-8.0.91/ultralytics/yolo/data/dataloaders/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 20:20:18.000000 ultralytics-8.0.91/ultralytics/yolo/data/dataloaders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13777 2023-05-01 20:20:18.000000 ultralytics-8.0.91/ultralytics/yolo/data/dataloaders/stream_loaders.py
--rw-r--r--   0 runner    (1001) docker     (123)    17646 2023-05-01 20:20:18.000000 ultralytics-8.0.91/ultralytics/yolo/data/dataloaders/v5augmentations.py
--rw-r--r--   0 runner    (1001) docker     (123)    51260 2023-05-01 20:20:18.000000 ultralytics-8.0.91/ultralytics/yolo/data/dataloaders/v5loader.py
--rw-r--r--   0 runner    (1001) docker     (123)    11980 2023-05-01 20:20:18.000000 ultralytics-8.0.91/ultralytics/yolo/data/dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     1816 2023-05-01 20:20:18.000000 ultralytics-8.0.91/ultralytics/yolo/data/dataset_wrappers.py
--rw-r--r--   0 runner    (1001) docker     (123)    22741 2023-05-01 20:20:18.000000 ultralytics-8.0.91/ultralytics/yolo/data/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 20:21:39.527917 ultralytics-8.0.91/ultralytics/yolo/engine/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 20:20:18.000000 ultralytics-8.0.91/ultralytics/yolo/engine/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    40265 2023-05-01 20:20:18.000000 ultralytics-8.0.91/ultralytics/yolo/engine/exporter.py
--rw-r--r--   0 runner    (1001) docker     (123)    21937 2023-05-01 20:20:18.000000 ultralytics-8.0.91/ultralytics/yolo/engine/model.py
--rw-r--r--   0 runner    (1001) docker     (123)    16049 2023-05-01 20:20:18.000000 ultralytics-8.0.91/ultralytics/yolo/engine/predictor.py
--rw-r--r--   0 runner    (1001) docker     (123)    20388 2023-05-01 20:20:18.000000 ultralytics-8.0.91/ultralytics/yolo/engine/results.py
--rw-r--r--   0 runner    (1001) docker     (123)    31310 2023-05-01 20:20:18.000000 ultralytics-8.0.91/ultralytics/yolo/engine/trainer.py
--rw-r--r--   0 runner    (1001) docker     (123)    11462 2023-05-01 20:20:18.000000 ultralytics-8.0.91/ultralytics/yolo/engine/validator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 20:21:39.527917 ultralytics-8.0.91/ultralytics/yolo/utils/
--rw-r--r--   0 runner    (1001) docker     (123)    27960 2023-05-01 20:20:18.000000 ultralytics-8.0.91/ultralytics/yolo/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3846 2023-05-01 20:20:18.000000 ultralytics-8.0.91/ultralytics/yolo/utils/autobatch.py
--rw-r--r--   0 runner    (1001) docker     (123)     6676 2023-05-01 20:20:18.000000 ultralytics-8.0.91/ultralytics/yolo/utils/benchmarks.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 20:21:39.531917 ultralytics-8.0.91/ultralytics/yolo/utils/callbacks/
--rw-r--r--   0 runner    (1001) docker     (123)      171 2023-05-01 20:20:18.000000 ultralytics-8.0.91/ultralytics/yolo/utils/callbacks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5544 2023-05-01 20:20:18.000000 ultralytics-8.0.91/ultralytics/yolo/utils/callbacks/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     5831 2023-05-01 20:20:18.000000 ultralytics-8.0.91/ultralytics/yolo/utils/callbacks/clearml.py
--rw-r--r--   0 runner    (1001) docker     (123)    13190 2023-05-01 20:20:18.000000 ultralytics-8.0.91/ultralytics/yolo/utils/callbacks/comet.py
--rw-r--r--   0 runner    (1001) docker     (123)     3537 2023-05-01 20:20:18.000000 ultralytics-8.0.91/ultralytics/yolo/utils/callbacks/hub.py
--rw-r--r--   0 runner    (1001) docker     (123)     2493 2023-05-01 20:20:18.000000 ultralytics-8.0.91/ultralytics/yolo/utils/callbacks/mlflow.py
--rw-r--r--   0 runner    (1001) docker     (123)     3830 2023-05-01 20:20:18.000000 ultralytics-8.0.91/ultralytics/yolo/utils/callbacks/neptune.py
--rw-r--r--   0 runner    (1001) docker     (123)      452 2023-05-01 20:20:18.000000 ultralytics-8.0.91/ultralytics/yolo/utils/callbacks/raytune.py
--rw-r--r--   0 runner    (1001) docker     (123)     1524 2023-05-01 20:20:18.000000 ultralytics-8.0.91/ultralytics/yolo/utils/callbacks/tensorboard.py
--rw-r--r--   0 runner    (1001) docker     (123)     1869 2023-05-01 20:20:18.000000 ultralytics-8.0.91/ultralytics/yolo/utils/callbacks/wb.py
--rw-r--r--   0 runner    (1001) docker     (123)    14881 2023-05-01 20:20:18.000000 ultralytics-8.0.91/ultralytics/yolo/utils/checks.py
--rw-r--r--   0 runner    (1001) docker     (123)     2542 2023-05-01 20:20:18.000000 ultralytics-8.0.91/ultralytics/yolo/utils/dist.py
--rw-r--r--   0 runner    (1001) docker     (123)    11486 2023-05-01 20:20:18.000000 ultralytics-8.0.91/ultralytics/yolo/utils/downloads.py
--rw-r--r--   0 runner    (1001) docker     (123)      317 2023-05-01 20:20:18.000000 ultralytics-8.0.91/ultralytics/yolo/utils/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     3316 2023-05-01 20:20:18.000000 ultralytics-8.0.91/ultralytics/yolo/utils/files.py
--rw-r--r--   0 runner    (1001) docker     (123)    14176 2023-05-01 20:20:18.000000 ultralytics-8.0.91/ultralytics/yolo/utils/instance.py
--rw-r--r--   0 runner    (1001) docker     (123)     3195 2023-05-01 20:20:18.000000 ultralytics-8.0.91/ultralytics/yolo/utils/loss.py
--rw-r--r--   0 runner    (1001) docker     (123)    41829 2023-05-01 20:20:18.000000 ultralytics-8.0.91/ultralytics/yolo/utils/metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)    28191 2023-05-01 20:20:18.000000 ultralytics-8.0.91/ultralytics/yolo/utils/ops.py
--rw-r--r--   0 runner    (1001) docker     (123)    24161 2023-05-01 20:20:18.000000 ultralytics-8.0.91/ultralytics/yolo/utils/plotting.py
--rw-r--r--   0 runner    (1001) docker     (123)    13220 2023-05-01 20:20:18.000000 ultralytics-8.0.91/ultralytics/yolo/utils/tal.py
--rw-r--r--   0 runner    (1001) docker     (123)    20019 2023-05-01 20:20:18.000000 ultralytics-8.0.91/ultralytics/yolo/utils/torch_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2209 2023-05-01 20:20:18.000000 ultralytics-8.0.91/ultralytics/yolo/utils/tuner.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 20:21:39.531917 ultralytics-8.0.91/ultralytics/yolo/v8/
--rw-r--r--   0 runner    (1001) docker     (123)      158 2023-05-01 20:20:18.000000 ultralytics-8.0.91/ultralytics/yolo/v8/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 20:21:39.531917 ultralytics-8.0.91/ultralytics/yolo/v8/classify/
--rw-r--r--   0 runner    (1001) docker     (123)      391 2023-05-01 20:20:18.000000 ultralytics-8.0.91/ultralytics/yolo/v8/classify/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1929 2023-05-01 20:20:18.000000 ultralytics-8.0.91/ultralytics/yolo/v8/classify/predict.py
--rw-r--r--   0 runner    (1001) docker     (123)     7194 2023-05-01 20:20:18.000000 ultralytics-8.0.91/ultralytics/yolo/v8/classify/train.py
--rw-r--r--   0 runner    (1001) docker     (123)     4413 2023-05-01 20:20:18.000000 ultralytics-8.0.91/ultralytics/yolo/v8/classify/val.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 20:21:39.531917 ultralytics-8.0.91/ultralytics/yolo/v8/detect/
--rw-r--r--   0 runner    (1001) docker     (123)      277 2023-05-01 20:20:18.000000 ultralytics-8.0.91/ultralytics/yolo/v8/detect/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1854 2023-05-01 20:20:18.000000 ultralytics-8.0.91/ultralytics/yolo/v8/detect/predict.py
--rw-r--r--   0 runner    (1001) docker     (123)    12195 2023-05-01 20:20:18.000000 ultralytics-8.0.91/ultralytics/yolo/v8/detect/train.py
--rw-r--r--   0 runner    (1001) docker     (123)    14425 2023-05-01 20:20:18.000000 ultralytics-8.0.91/ultralytics/yolo/v8/detect/val.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 20:21:39.531917 ultralytics-8.0.91/ultralytics/yolo/v8/pose/
--rw-r--r--   0 runner    (1001) docker     (123)      247 2023-05-01 20:20:18.000000 ultralytics-8.0.91/ultralytics/yolo/v8/pose/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2371 2023-05-01 20:20:18.000000 ultralytics-8.0.91/ultralytics/yolo/v8/pose/predict.py
--rw-r--r--   0 runner    (1001) docker     (123)     7836 2023-05-01 20:20:18.000000 ultralytics-8.0.91/ultralytics/yolo/v8/pose/train.py
--rw-r--r--   0 runner    (1001) docker     (123)    10840 2023-05-01 20:20:18.000000 ultralytics-8.0.91/ultralytics/yolo/v8/pose/val.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 20:21:39.531917 ultralytics-8.0.91/ultralytics/yolo/v8/segment/
--rw-r--r--   0 runner    (1001) docker     (123)      295 2023-05-01 20:20:18.000000 ultralytics-8.0.91/ultralytics/yolo/v8/segment/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2839 2023-05-01 20:20:18.000000 ultralytics-8.0.91/ultralytics/yolo/v8/segment/predict.py
--rw-r--r--   0 runner    (1001) docker     (123)     8283 2023-05-01 20:20:18.000000 ultralytics-8.0.91/ultralytics/yolo/v8/segment/train.py
--rw-r--r--   0 runner    (1001) docker     (123)    12776 2023-05-01 20:20:18.000000 ultralytics-8.0.91/ultralytics/yolo/v8/segment/val.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 20:21:39.515917 ultralytics-8.0.91/ultralytics.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    25796 2023-05-01 20:21:39.000000 ultralytics-8.0.91/ultralytics.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5023 2023-05-01 20:21:39.000000 ultralytics-8.0.91/ultralytics.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-01 20:21:39.000000 ultralytics-8.0.91/ultralytics.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-01 20:21:39.000000 ultralytics-8.0.91/ultralytics.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      366 2023-05-01 20:21:39.000000 ultralytics-8.0.91/ultralytics.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-01 20:21:39.000000 ultralytics-8.0.91/ultralytics.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 23:28:53.674922 ultralytics-8.0.92/
+-rw-r--r--   0 runner    (1001) docker     (123)     5624 2023-05-03 23:27:16.000000 ultralytics-8.0.92/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-05-03 23:27:16.000000 ultralytics-8.0.92/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      213 2023-05-03 23:27:16.000000 ultralytics-8.0.92/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    25796 2023-05-03 23:28:53.674922 ultralytics-8.0.92/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    24235 2023-05-03 23:27:16.000000 ultralytics-8.0.92/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)    23225 2023-05-03 23:27:16.000000 ultralytics-8.0.92/README.zh-CN.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1107 2023-05-03 23:27:16.000000 ultralytics-8.0.92/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      682 2023-05-03 23:28:53.674922 ultralytics-8.0.92/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3052 2023-05-03 23:27:16.000000 ultralytics-8.0.92/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 23:28:53.658922 ultralytics-8.0.92/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     3165 2023-05-03 23:27:16.000000 ultralytics-8.0.92/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4380 2023-05-03 23:27:16.000000 ultralytics-8.0.92/tests/test_engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7099 2023-05-03 23:27:16.000000 ultralytics-8.0.92/tests/test_python.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 23:28:53.658922 ultralytics-8.0.92/ultralytics/
+-rw-r--r--   0 runner    (1001) docker     (123)      330 2023-05-03 23:27:16.000000 ultralytics-8.0.92/ultralytics/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 23:28:53.658922 ultralytics-8.0.92/ultralytics/assets/
+-rw-r--r--   0 runner    (1001) docker     (123)   137419 2023-05-03 23:27:16.000000 ultralytics-8.0.92/ultralytics/assets/bus.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)    50427 2023-05-03 23:27:16.000000 ultralytics-8.0.92/ultralytics/assets/zidane.jpg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 23:28:53.658922 ultralytics-8.0.92/ultralytics/datasets/
+-rw-r--r--   0 runner    (1001) docker     (123)     2751 2023-05-03 23:27:16.000000 ultralytics-8.0.92/ultralytics/datasets/Argoverse.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1918 2023-05-03 23:27:16.000000 ultralytics-8.0.92/ultralytics/datasets/GlobalWheat2020.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    42439 2023-05-03 23:27:16.000000 ultralytics-8.0.92/ultralytics/datasets/ImageNet.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     9270 2023-05-03 23:27:16.000000 ultralytics-8.0.92/ultralytics/datasets/Objects365.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2437 2023-05-03 23:27:16.000000 ultralytics-8.0.92/ultralytics/datasets/SKU-110K.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3512 2023-05-03 23:27:16.000000 ultralytics-8.0.92/ultralytics/datasets/VOC.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3012 2023-05-03 23:27:16.000000 ultralytics-8.0.92/ultralytics/datasets/VisDrone.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1547 2023-05-03 23:27:16.000000 ultralytics-8.0.92/ultralytics/datasets/coco-pose.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2526 2023-05-03 23:27:16.000000 ultralytics-8.0.92/ultralytics/datasets/coco.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1862 2023-05-03 23:27:16.000000 ultralytics-8.0.92/ultralytics/datasets/coco128-seg.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1846 2023-05-03 23:27:16.000000 ultralytics-8.0.92/ultralytics/datasets/coco128.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      895 2023-05-03 23:27:16.000000 ultralytics-8.0.92/ultralytics/datasets/coco8-pose.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1797 2023-05-03 23:27:16.000000 ultralytics-8.0.92/ultralytics/datasets/coco8-seg.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1777 2023-05-03 23:27:16.000000 ultralytics-8.0.92/ultralytics/datasets/coco8.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     5178 2023-05-03 23:27:16.000000 ultralytics-8.0.92/ultralytics/datasets/xView.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 23:28:53.658922 ultralytics-8.0.92/ultralytics/hub/
+-rw-r--r--   0 runner    (1001) docker     (123)     3442 2023-05-03 23:27:16.000000 ultralytics-8.0.92/ultralytics/hub/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5209 2023-05-03 23:27:16.000000 ultralytics-8.0.92/ultralytics/hub/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8479 2023-05-03 23:27:16.000000 ultralytics-8.0.92/ultralytics/hub/session.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9157 2023-05-03 23:27:16.000000 ultralytics-8.0.92/ultralytics/hub/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 23:28:53.654922 ultralytics-8.0.92/ultralytics/models/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 23:28:53.662922 ultralytics-8.0.92/ultralytics/models/v3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1435 2023-05-03 23:27:16.000000 ultralytics-8.0.92/ultralytics/models/v3/yolov3-spp.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1136 2023-05-03 23:27:16.000000 ultralytics-8.0.92/ultralytics/models/v3/yolov3-tiny.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1426 2023-05-03 23:27:16.000000 ultralytics-8.0.92/ultralytics/models/v3/yolov3.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 23:28:53.662922 ultralytics-8.0.92/ultralytics/models/v5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1812 2023-05-03 23:27:16.000000 ultralytics-8.0.92/ultralytics/models/v5/yolov5-p6.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1439 2023-05-03 23:27:16.000000 ultralytics-8.0.92/ultralytics/models/v5/yolov5.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 23:28:53.662922 ultralytics-8.0.92/ultralytics/models/v8/
+-rw-r--r--   0 runner    (1001) docker     (123)      920 2023-05-03 23:27:16.000000 ultralytics-8.0.92/ultralytics/models/v8/yolov8-cls.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1751 2023-05-03 23:27:16.000000 ultralytics-8.0.92/ultralytics/models/v8/yolov8-p2.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1856 2023-05-03 23:27:16.000000 ultralytics-8.0.92/ultralytics/models/v8/yolov8-p6.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1953 2023-05-03 23:27:16.000000 ultralytics-8.0.92/ultralytics/models/v8/yolov8-pose-p6.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1580 2023-05-03 23:27:16.000000 ultralytics-8.0.92/ultralytics/models/v8/yolov8-pose.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1490 2023-05-03 23:27:16.000000 ultralytics-8.0.92/ultralytics/models/v8/yolov8-seg.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1913 2023-05-03 23:27:16.000000 ultralytics-8.0.92/ultralytics/models/v8/yolov8.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 23:28:53.662922 ultralytics-8.0.92/ultralytics/nn/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 23:27:16.000000 ultralytics-8.0.92/ultralytics/nn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24243 2023-05-03 23:27:16.000000 ultralytics-8.0.92/ultralytics/nn/autobackend.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12509 2023-05-03 23:27:16.000000 ultralytics-8.0.92/ultralytics/nn/autoshape.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25079 2023-05-03 23:27:16.000000 ultralytics-8.0.92/ultralytics/nn/modules.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27170 2023-05-03 23:27:16.000000 ultralytics-8.0.92/ultralytics/nn/tasks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 23:28:53.662922 ultralytics-8.0.92/ultralytics/tracker/
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-05-03 23:27:16.000000 ultralytics-8.0.92/ultralytics/tracker/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 23:28:53.662922 ultralytics-8.0.92/ultralytics/tracker/cfg/
+-rw-r--r--   0 runner    (1001) docker     (123)      890 2023-05-03 23:27:16.000000 ultralytics-8.0.92/ultralytics/tracker/cfg/botsort.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      694 2023-05-03 23:27:16.000000 ultralytics-8.0.92/ultralytics/tracker/cfg/bytetrack.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2309 2023-05-03 23:27:16.000000 ultralytics-8.0.92/ultralytics/tracker/track.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 23:28:53.662922 ultralytics-8.0.92/ultralytics/tracker/trackers/
+-rw-r--r--   0 runner    (1001) docker     (123)      171 2023-05-03 23:27:16.000000 ultralytics-8.0.92/ultralytics/tracker/trackers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1609 2023-05-03 23:27:16.000000 ultralytics-8.0.92/ultralytics/tracker/trackers/basetrack.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5684 2023-05-03 23:27:16.000000 ultralytics-8.0.92/ultralytics/tracker/trackers/bot_sort.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14448 2023-05-03 23:27:16.000000 ultralytics-8.0.92/ultralytics/tracker/trackers/byte_tracker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 23:28:53.662922 ultralytics-8.0.92/ultralytics/tracker/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 23:27:16.000000 ultralytics-8.0.92/ultralytics/tracker/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12214 2023-05-03 23:27:16.000000 ultralytics-8.0.92/ultralytics/tracker/utils/gmc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18420 2023-05-03 23:27:16.000000 ultralytics-8.0.92/ultralytics/tracker/utils/kalman_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8699 2023-05-03 23:27:16.000000 ultralytics-8.0.92/ultralytics/tracker/utils/matching.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 23:28:53.662922 ultralytics-8.0.92/ultralytics/vit/
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-05-03 23:27:16.000000 ultralytics-8.0.92/ultralytics/vit/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 23:28:53.662922 ultralytics-8.0.92/ultralytics/vit/sam/
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-05-03 23:27:16.000000 ultralytics-8.0.92/ultralytics/vit/sam/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13304 2023-05-03 23:27:16.000000 ultralytics-8.0.92/ultralytics/vit/sam/amg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3878 2023-05-03 23:27:16.000000 ultralytics-8.0.92/ultralytics/vit/sam/autosize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3686 2023-05-03 23:27:16.000000 ultralytics-8.0.92/ultralytics/vit/sam/build.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1450 2023-05-03 23:27:16.000000 ultralytics-8.0.92/ultralytics/vit/sam/model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 23:28:53.666922 ultralytics-8.0.92/ultralytics/vit/sam/modules/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 23:27:16.000000 ultralytics-8.0.92/ultralytics/vit/sam/modules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6347 2023-05-03 23:27:16.000000 ultralytics-8.0.92/ultralytics/vit/sam/modules/decoders.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22502 2023-05-03 23:27:16.000000 ultralytics-8.0.92/ultralytics/vit/sam/modules/encoders.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15250 2023-05-03 23:27:16.000000 ultralytics-8.0.92/ultralytics/vit/sam/modules/mask_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11201 2023-05-03 23:27:16.000000 ultralytics-8.0.92/ultralytics/vit/sam/modules/prompt_predictor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7116 2023-05-03 23:27:16.000000 ultralytics-8.0.92/ultralytics/vit/sam/modules/sam.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8489 2023-05-03 23:27:16.000000 ultralytics-8.0.92/ultralytics/vit/sam/modules/transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2139 2023-05-03 23:27:16.000000 ultralytics-8.0.92/ultralytics/vit/sam/predict.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 23:28:53.666922 ultralytics-8.0.92/ultralytics/yolo/
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-05-03 23:27:16.000000 ultralytics-8.0.92/ultralytics/yolo/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 23:28:53.666922 ultralytics-8.0.92/ultralytics/yolo/cfg/
+-rw-r--r--   0 runner    (1001) docker     (123)    17675 2023-05-03 23:27:16.000000 ultralytics-8.0.92/ultralytics/yolo/cfg/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6172 2023-05-03 23:27:16.000000 ultralytics-8.0.92/ultralytics/yolo/cfg/default.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 23:28:53.666922 ultralytics-8.0.92/ultralytics/yolo/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      458 2023-05-03 23:27:16.000000 ultralytics-8.0.92/ultralytics/yolo/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2250 2023-05-03 23:27:16.000000 ultralytics-8.0.92/ultralytics/yolo/data/annotator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33512 2023-05-03 23:27:16.000000 ultralytics-8.0.92/ultralytics/yolo/data/augment.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11763 2023-05-03 23:27:16.000000 ultralytics-8.0.92/ultralytics/yolo/data/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6556 2023-05-03 23:27:16.000000 ultralytics-8.0.92/ultralytics/yolo/data/build.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 23:28:53.666922 ultralytics-8.0.92/ultralytics/yolo/data/dataloaders/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 23:27:16.000000 ultralytics-8.0.92/ultralytics/yolo/data/dataloaders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13777 2023-05-03 23:27:16.000000 ultralytics-8.0.92/ultralytics/yolo/data/dataloaders/stream_loaders.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17646 2023-05-03 23:27:16.000000 ultralytics-8.0.92/ultralytics/yolo/data/dataloaders/v5augmentations.py
+-rw-r--r--   0 runner    (1001) docker     (123)    51260 2023-05-03 23:27:16.000000 ultralytics-8.0.92/ultralytics/yolo/data/dataloaders/v5loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11980 2023-05-03 23:27:16.000000 ultralytics-8.0.92/ultralytics/yolo/data/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1816 2023-05-03 23:27:16.000000 ultralytics-8.0.92/ultralytics/yolo/data/dataset_wrappers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22741 2023-05-03 23:27:16.000000 ultralytics-8.0.92/ultralytics/yolo/data/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 23:28:53.666922 ultralytics-8.0.92/ultralytics/yolo/engine/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 23:27:16.000000 ultralytics-8.0.92/ultralytics/yolo/engine/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40265 2023-05-03 23:27:16.000000 ultralytics-8.0.92/ultralytics/yolo/engine/exporter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21937 2023-05-03 23:27:16.000000 ultralytics-8.0.92/ultralytics/yolo/engine/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15913 2023-05-03 23:27:16.000000 ultralytics-8.0.92/ultralytics/yolo/engine/predictor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20388 2023-05-03 23:27:16.000000 ultralytics-8.0.92/ultralytics/yolo/engine/results.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31310 2023-05-03 23:27:16.000000 ultralytics-8.0.92/ultralytics/yolo/engine/trainer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11462 2023-05-03 23:27:16.000000 ultralytics-8.0.92/ultralytics/yolo/engine/validator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 23:28:53.670922 ultralytics-8.0.92/ultralytics/yolo/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)    27889 2023-05-03 23:27:16.000000 ultralytics-8.0.92/ultralytics/yolo/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3846 2023-05-03 23:27:16.000000 ultralytics-8.0.92/ultralytics/yolo/utils/autobatch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6676 2023-05-03 23:27:16.000000 ultralytics-8.0.92/ultralytics/yolo/utils/benchmarks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 23:28:53.670922 ultralytics-8.0.92/ultralytics/yolo/utils/callbacks/
+-rw-r--r--   0 runner    (1001) docker     (123)      171 2023-05-03 23:27:16.000000 ultralytics-8.0.92/ultralytics/yolo/utils/callbacks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5544 2023-05-03 23:27:16.000000 ultralytics-8.0.92/ultralytics/yolo/utils/callbacks/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5831 2023-05-03 23:27:16.000000 ultralytics-8.0.92/ultralytics/yolo/utils/callbacks/clearml.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13190 2023-05-03 23:27:16.000000 ultralytics-8.0.92/ultralytics/yolo/utils/callbacks/comet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3537 2023-05-03 23:27:16.000000 ultralytics-8.0.92/ultralytics/yolo/utils/callbacks/hub.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2493 2023-05-03 23:27:16.000000 ultralytics-8.0.92/ultralytics/yolo/utils/callbacks/mlflow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3830 2023-05-03 23:27:16.000000 ultralytics-8.0.92/ultralytics/yolo/utils/callbacks/neptune.py
+-rw-r--r--   0 runner    (1001) docker     (123)      452 2023-05-03 23:27:16.000000 ultralytics-8.0.92/ultralytics/yolo/utils/callbacks/raytune.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1524 2023-05-03 23:27:16.000000 ultralytics-8.0.92/ultralytics/yolo/utils/callbacks/tensorboard.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1869 2023-05-03 23:27:16.000000 ultralytics-8.0.92/ultralytics/yolo/utils/callbacks/wb.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14881 2023-05-03 23:27:16.000000 ultralytics-8.0.92/ultralytics/yolo/utils/checks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2542 2023-05-03 23:27:16.000000 ultralytics-8.0.92/ultralytics/yolo/utils/dist.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11486 2023-05-03 23:27:16.000000 ultralytics-8.0.92/ultralytics/yolo/utils/downloads.py
+-rw-r--r--   0 runner    (1001) docker     (123)      317 2023-05-03 23:27:16.000000 ultralytics-8.0.92/ultralytics/yolo/utils/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3316 2023-05-03 23:27:16.000000 ultralytics-8.0.92/ultralytics/yolo/utils/files.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14176 2023-05-03 23:27:16.000000 ultralytics-8.0.92/ultralytics/yolo/utils/instance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3195 2023-05-03 23:27:16.000000 ultralytics-8.0.92/ultralytics/yolo/utils/loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41829 2023-05-03 23:27:16.000000 ultralytics-8.0.92/ultralytics/yolo/utils/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28191 2023-05-03 23:27:16.000000 ultralytics-8.0.92/ultralytics/yolo/utils/ops.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24037 2023-05-03 23:27:16.000000 ultralytics-8.0.92/ultralytics/yolo/utils/plotting.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13220 2023-05-03 23:27:16.000000 ultralytics-8.0.92/ultralytics/yolo/utils/tal.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20019 2023-05-03 23:27:16.000000 ultralytics-8.0.92/ultralytics/yolo/utils/torch_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2209 2023-05-03 23:27:16.000000 ultralytics-8.0.92/ultralytics/yolo/utils/tuner.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 23:28:53.670922 ultralytics-8.0.92/ultralytics/yolo/v8/
+-rw-r--r--   0 runner    (1001) docker     (123)      158 2023-05-03 23:27:16.000000 ultralytics-8.0.92/ultralytics/yolo/v8/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 23:28:53.670922 ultralytics-8.0.92/ultralytics/yolo/v8/classify/
+-rw-r--r--   0 runner    (1001) docker     (123)      391 2023-05-03 23:27:16.000000 ultralytics-8.0.92/ultralytics/yolo/v8/classify/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1929 2023-05-03 23:27:16.000000 ultralytics-8.0.92/ultralytics/yolo/v8/classify/predict.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7194 2023-05-03 23:27:16.000000 ultralytics-8.0.92/ultralytics/yolo/v8/classify/train.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4413 2023-05-03 23:27:16.000000 ultralytics-8.0.92/ultralytics/yolo/v8/classify/val.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 23:28:53.670922 ultralytics-8.0.92/ultralytics/yolo/v8/detect/
+-rw-r--r--   0 runner    (1001) docker     (123)      277 2023-05-03 23:27:16.000000 ultralytics-8.0.92/ultralytics/yolo/v8/detect/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1854 2023-05-03 23:27:16.000000 ultralytics-8.0.92/ultralytics/yolo/v8/detect/predict.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12199 2023-05-03 23:27:16.000000 ultralytics-8.0.92/ultralytics/yolo/v8/detect/train.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14425 2023-05-03 23:27:16.000000 ultralytics-8.0.92/ultralytics/yolo/v8/detect/val.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 23:28:53.674922 ultralytics-8.0.92/ultralytics/yolo/v8/pose/
+-rw-r--r--   0 runner    (1001) docker     (123)      247 2023-05-03 23:27:16.000000 ultralytics-8.0.92/ultralytics/yolo/v8/pose/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2371 2023-05-03 23:27:16.000000 ultralytics-8.0.92/ultralytics/yolo/v8/pose/predict.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7836 2023-05-03 23:27:16.000000 ultralytics-8.0.92/ultralytics/yolo/v8/pose/train.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10840 2023-05-03 23:27:16.000000 ultralytics-8.0.92/ultralytics/yolo/v8/pose/val.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 23:28:53.674922 ultralytics-8.0.92/ultralytics/yolo/v8/segment/
+-rw-r--r--   0 runner    (1001) docker     (123)      295 2023-05-03 23:27:16.000000 ultralytics-8.0.92/ultralytics/yolo/v8/segment/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2839 2023-05-03 23:27:16.000000 ultralytics-8.0.92/ultralytics/yolo/v8/segment/predict.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8283 2023-05-03 23:27:16.000000 ultralytics-8.0.92/ultralytics/yolo/v8/segment/train.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12776 2023-05-03 23:27:16.000000 ultralytics-8.0.92/ultralytics/yolo/v8/segment/val.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 23:28:53.658922 ultralytics-8.0.92/ultralytics.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    25796 2023-05-03 23:28:53.000000 ultralytics-8.0.92/ultralytics.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5023 2023-05-03 23:28:53.000000 ultralytics-8.0.92/ultralytics.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-03 23:28:53.000000 ultralytics-8.0.92/ultralytics.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-03 23:28:53.000000 ultralytics-8.0.92/ultralytics.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      408 2023-05-03 23:28:53.000000 ultralytics-8.0.92/ultralytics.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-03 23:28:53.000000 ultralytics-8.0.92/ultralytics.egg-info/top_level.txt
```

### Comparing `ultralytics-8.0.91/CONTRIBUTING.md` & `ultralytics-8.0.92/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.91/LICENSE` & `ultralytics-8.0.92/LICENSE`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.91/PKG-INFO` & `ultralytics-8.0.92/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ultralytics
-Version: 8.0.91
+Version: 8.0.92
 Summary: Ultralytics YOLOv8
 Home-page: https://github.com/ultralytics/ultralytics
 Author: Ultralytics
 Author-email: hello@ultralytics.com
 License: AGPL-3.0
 Project-URL: Bug Reports, https://github.com/ultralytics/ultralytics/issues
 Project-URL: Funding, https://ultralytics.com
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: ultralytics Version: 8.0.91 Summary: Ultralytics
+Metadata-Version: 2.1 Name: ultralytics Version: 8.0.92 Summary: Ultralytics
 YOLOv8 Home-page: https://github.com/ultralytics/ultralytics Author:
 Ultralytics Author-email: hello@ultralytics.com License: AGPL-3.0 Project-URL:
 Bug Reports, https://github.com/ultralytics/ultralytics/issues Project-URL:
 Funding, https://ultralytics.com Project-URL: Source, https://github.com/
 ultralytics/ultralytics Keywords: machine-learning,deep-
 learning,vision,ML,DL,AI,YOLO,YOLOv3,YOLOv5,YOLOv8,HUB,Ultralytics Classifier:
 Development Status :: 4 - Beta Classifier: Intended Audience :: Developers
```

### Comparing `ultralytics-8.0.91/README.md` & `ultralytics-8.0.92/README.md`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.91/README.zh-CN.md` & `ultralytics-8.0.92/README.zh-CN.md`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.91/requirements.txt` & `ultralytics-8.0.92/requirements.txt`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.91/setup.cfg` & `ultralytics-8.0.92/setup.cfg`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.91/setup.py` & `ultralytics-8.0.92/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -35,16 +35,23 @@
     author='Ultralytics',
     author_email='hello@ultralytics.com',
     packages=find_packages(),  # required
     include_package_data=True,
     install_requires=REQUIREMENTS + PKG_REQUIREMENTS,
     extras_require={
         'dev': [
-            'check-manifest', 'pytest', 'pytest-cov', 'coverage', 'mkdocs-material', 'mkdocstrings[python]',
-            'mkdocs-redirects'],
+            'check-manifest',
+            'pytest',
+            'pytest-cov',
+            'coverage',
+            'mkdocs-material',
+            'mkdocstrings[python]',
+            'mkdocs-redirects',  # for 301 redirects
+            'mkdocs-git-revision-date-localized-plugin',  # for created/updated dates
+        ],
         'export': ['coremltools>=6.0', 'openvino-dev>=2022.3', 'tensorflowjs'],  # automatically installs tensorflow
     },
     classifiers=[
         'Development Status :: 4 - Beta',
         'Intended Audience :: Developers',
         'Intended Audience :: Education',
         'Intended Audience :: Science/Research',
```

### Comparing `ultralytics-8.0.91/tests/test_cli.py` & `ultralytics-8.0.92/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.91/tests/test_engine.py` & `ultralytics-8.0.92/tests/test_engine.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.91/tests/test_python.py` & `ultralytics-8.0.92/tests/test_python.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.91/ultralytics/assets/bus.jpg` & `ultralytics-8.0.92/ultralytics/assets/bus.jpg`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.91/ultralytics/assets/zidane.jpg` & `ultralytics-8.0.92/ultralytics/assets/zidane.jpg`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.91/ultralytics/datasets/Argoverse.yaml` & `ultralytics-8.0.92/ultralytics/datasets/Argoverse.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.91/ultralytics/datasets/GlobalWheat2020.yaml` & `ultralytics-8.0.92/ultralytics/datasets/GlobalWheat2020.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.91/ultralytics/datasets/ImageNet.yaml` & `ultralytics-8.0.92/ultralytics/datasets/ImageNet.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.91/ultralytics/datasets/Objects365.yaml` & `ultralytics-8.0.92/ultralytics/datasets/Objects365.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.91/ultralytics/datasets/SKU-110K.yaml` & `ultralytics-8.0.92/ultralytics/datasets/SKU-110K.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.91/ultralytics/datasets/VOC.yaml` & `ultralytics-8.0.92/ultralytics/datasets/VOC.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.91/ultralytics/datasets/VisDrone.yaml` & `ultralytics-8.0.92/ultralytics/datasets/VisDrone.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.91/ultralytics/datasets/coco-pose.yaml` & `ultralytics-8.0.92/ultralytics/datasets/coco-pose.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.91/ultralytics/datasets/coco.yaml` & `ultralytics-8.0.92/ultralytics/datasets/coco.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.91/ultralytics/datasets/coco128-seg.yaml` & `ultralytics-8.0.92/ultralytics/datasets/coco128-seg.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.91/ultralytics/datasets/coco128.yaml` & `ultralytics-8.0.92/ultralytics/datasets/coco128.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.91/ultralytics/datasets/coco8-pose.yaml` & `ultralytics-8.0.92/ultralytics/datasets/coco8-pose.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.91/ultralytics/datasets/coco8-seg.yaml` & `ultralytics-8.0.92/ultralytics/datasets/coco8-seg.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.91/ultralytics/datasets/coco8.yaml` & `ultralytics-8.0.92/ultralytics/datasets/coco8.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.91/ultralytics/datasets/xView.yaml` & `ultralytics-8.0.92/ultralytics/datasets/xView.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.91/ultralytics/hub/__init__.py` & `ultralytics-8.0.92/ultralytics/hub/__init__.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.91/ultralytics/hub/auth.py` & `ultralytics-8.0.92/ultralytics/hub/auth.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.91/ultralytics/hub/session.py` & `ultralytics-8.0.92/ultralytics/hub/session.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.91/ultralytics/hub/utils.py` & `ultralytics-8.0.92/ultralytics/hub/utils.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.91/ultralytics/models/v3/yolov3-spp.yaml` & `ultralytics-8.0.92/ultralytics/models/v3/yolov3-spp.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.91/ultralytics/models/v3/yolov3-tiny.yaml` & `ultralytics-8.0.92/ultralytics/models/v3/yolov3-tiny.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.91/ultralytics/models/v3/yolov3.yaml` & `ultralytics-8.0.92/ultralytics/models/v3/yolov3.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.91/ultralytics/models/v5/yolov5-p6.yaml` & `ultralytics-8.0.92/ultralytics/models/v5/yolov5-p6.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.91/ultralytics/models/v5/yolov5.yaml` & `ultralytics-8.0.92/ultralytics/models/v5/yolov5.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.91/ultralytics/models/v8/yolov8-cls.yaml` & `ultralytics-8.0.92/ultralytics/models/v8/yolov8-cls.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.91/ultralytics/models/v8/yolov8-p2.yaml` & `ultralytics-8.0.92/ultralytics/models/v8/yolov8-p2.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.91/ultralytics/models/v8/yolov8-p6.yaml` & `ultralytics-8.0.92/ultralytics/models/v8/yolov8-p6.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.91/ultralytics/models/v8/yolov8-pose-p6.yaml` & `ultralytics-8.0.92/ultralytics/models/v8/yolov8-pose-p6.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.91/ultralytics/models/v8/yolov8-pose.yaml` & `ultralytics-8.0.92/ultralytics/models/v8/yolov8-pose.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.91/ultralytics/models/v8/yolov8-seg.yaml` & `ultralytics-8.0.92/ultralytics/models/v8/yolov8-seg.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.91/ultralytics/models/v8/yolov8.yaml` & `ultralytics-8.0.92/ultralytics/models/v8/yolov8.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.91/ultralytics/nn/autobackend.py` & `ultralytics-8.0.92/ultralytics/nn/autobackend.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.91/ultralytics/nn/autoshape.py` & `ultralytics-8.0.92/ultralytics/nn/autoshape.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.91/ultralytics/nn/modules.py` & `ultralytics-8.0.92/ultralytics/nn/modules.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.91/ultralytics/nn/tasks.py` & `ultralytics-8.0.92/ultralytics/nn/tasks.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.91/ultralytics/tracker/cfg/botsort.yaml` & `ultralytics-8.0.92/ultralytics/tracker/cfg/botsort.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.91/ultralytics/tracker/cfg/bytetrack.yaml` & `ultralytics-8.0.92/ultralytics/tracker/cfg/bytetrack.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.91/ultralytics/tracker/track.py` & `ultralytics-8.0.92/ultralytics/tracker/track.py`

 * *Files 1% similar despite different names*

```diff
@@ -43,15 +43,15 @@
     for i in range(bs):
         det = predictor.results[i].boxes.cpu().numpy()
         if len(det) == 0:
             continue
         tracks = predictor.trackers[i].update(det, im0s[i])
         if len(tracks) == 0:
             continue
-        idx = tracks[:, -1].tolist()
+        idx = tracks[:, -1].astype(int)
         predictor.results[i] = predictor.results[i][idx]
         predictor.results[i].update(boxes=torch.as_tensor(tracks[:, :-1]))
 
 
 def register_tracker(model, persist):
     """
     Register tracking callbacks to the model for object tracking during prediction.
```

### Comparing `ultralytics-8.0.91/ultralytics/tracker/trackers/basetrack.py` & `ultralytics-8.0.92/ultralytics/tracker/trackers/basetrack.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.91/ultralytics/tracker/trackers/bot_sort.py` & `ultralytics-8.0.92/ultralytics/tracker/trackers/bot_sort.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.91/ultralytics/tracker/trackers/byte_tracker.py` & `ultralytics-8.0.92/ultralytics/tracker/trackers/byte_tracker.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.91/ultralytics/tracker/utils/gmc.py` & `ultralytics-8.0.92/ultralytics/tracker/utils/gmc.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.91/ultralytics/tracker/utils/kalman_filter.py` & `ultralytics-8.0.92/ultralytics/tracker/utils/kalman_filter.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.91/ultralytics/tracker/utils/matching.py` & `ultralytics-8.0.92/ultralytics/tracker/utils/matching.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.91/ultralytics/vit/sam/amg.py` & `ultralytics-8.0.92/ultralytics/vit/sam/amg.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.91/ultralytics/vit/sam/autosize.py` & `ultralytics-8.0.92/ultralytics/vit/sam/autosize.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.91/ultralytics/vit/sam/build.py` & `ultralytics-8.0.92/ultralytics/vit/sam/build.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.91/ultralytics/vit/sam/model.py` & `ultralytics-8.0.92/ultralytics/vit/sam/model.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.91/ultralytics/vit/sam/modules/decoders.py` & `ultralytics-8.0.92/ultralytics/vit/sam/modules/decoders.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.91/ultralytics/vit/sam/modules/encoders.py` & `ultralytics-8.0.92/ultralytics/vit/sam/modules/encoders.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.91/ultralytics/vit/sam/modules/mask_generator.py` & `ultralytics-8.0.92/ultralytics/vit/sam/modules/mask_generator.py`

 * *Files 0% similar despite different names*

```diff
@@ -78,16 +78,16 @@
             than min_mask_region_area. Requires opencv.
           output_mode (str): The form masks are returned in. Can be 'binary_mask',
             'uncompressed_rle', or 'coco_rle'. 'coco_rle' requires pycocotools.
             For large resolutions, 'binary_mask' may consume large amounts of
             memory.
         """
 
-        assert (points_per_side is None) != (point_grids is
-                                             None), 'Exactly one of points_per_side or point_grid must be provided.'
+        assert (points_per_side is None) != (point_grids is None), \
+            'Exactly one of points_per_side or point_grid must be provided.'
         if points_per_side is not None:
             self.point_grids = build_all_layer_point_grids(
                 points_per_side,
                 crop_n_layers,
                 crop_n_points_downscale_factor,
             )
         elif point_grids is not None:
```

### Comparing `ultralytics-8.0.91/ultralytics/vit/sam/modules/prompt_predictor.py` & `ultralytics-8.0.92/ultralytics/vit/sam/modules/prompt_predictor.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.91/ultralytics/vit/sam/modules/sam.py` & `ultralytics-8.0.92/ultralytics/vit/sam/modules/sam.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.91/ultralytics/vit/sam/modules/transformer.py` & `ultralytics-8.0.92/ultralytics/vit/sam/modules/transformer.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.91/ultralytics/vit/sam/predict.py` & `ultralytics-8.0.92/ultralytics/vit/sam/predict.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.91/ultralytics/yolo/cfg/__init__.py` & `ultralytics-8.0.92/ultralytics/yolo/cfg/__init__.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.91/ultralytics/yolo/cfg/default.yaml` & `ultralytics-8.0.92/ultralytics/yolo/cfg/default.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.91/ultralytics/yolo/data/annotator.py` & `ultralytics-8.0.92/ultralytics/yolo/data/annotator.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.91/ultralytics/yolo/data/augment.py` & `ultralytics-8.0.92/ultralytics/yolo/data/augment.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.91/ultralytics/yolo/data/base.py` & `ultralytics-8.0.92/ultralytics/yolo/data/base.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.91/ultralytics/yolo/data/build.py` & `ultralytics-8.0.92/ultralytics/yolo/data/build.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.91/ultralytics/yolo/data/dataloaders/stream_loaders.py` & `ultralytics-8.0.92/ultralytics/yolo/data/dataloaders/stream_loaders.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.91/ultralytics/yolo/data/dataloaders/v5augmentations.py` & `ultralytics-8.0.92/ultralytics/yolo/data/dataloaders/v5augmentations.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.91/ultralytics/yolo/data/dataloaders/v5loader.py` & `ultralytics-8.0.92/ultralytics/yolo/data/dataloaders/v5loader.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.91/ultralytics/yolo/data/dataset.py` & `ultralytics-8.0.92/ultralytics/yolo/data/dataset.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.91/ultralytics/yolo/data/dataset_wrappers.py` & `ultralytics-8.0.92/ultralytics/yolo/data/dataset_wrappers.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.91/ultralytics/yolo/data/utils.py` & `ultralytics-8.0.92/ultralytics/yolo/data/utils.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.91/ultralytics/yolo/engine/exporter.py` & `ultralytics-8.0.92/ultralytics/yolo/engine/exporter.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.91/ultralytics/yolo/engine/model.py` & `ultralytics-8.0.92/ultralytics/yolo/engine/model.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.91/ultralytics/yolo/engine/predictor.py` & `ultralytics-8.0.92/ultralytics/yolo/engine/predictor.py`

 * *Files 2% similar despite different names*

```diff
@@ -111,18 +111,16 @@
     def preprocess(self, im):
         """Prepares input image before inference.
 
         Args:
             im (torch.Tensor | List(np.ndarray)): (N, 3, h, w) for tensor, [(h, w, 3) x N] for list.
         """
         if not isinstance(im, torch.Tensor):
-            auto = all(x.shape == im[0].shape for x in im) and self.model.pt
-            if not auto:
-                LOGGER.warning(
-                    'WARNING ⚠️ Source shapes differ. For optimal performance supply similarly-shaped sources.')
+            same_shapes = all(x.shape == im[0].shape for x in im)
+            auto = same_shapes and self.model.pt
             im = np.stack([LetterBox(self.imgsz, auto=auto, stride=self.model.stride)(image=x) for x in im])
             im = im[..., ::-1].transpose((0, 3, 1, 2))  # BGR to RGB, BHWC to BCHW, (n, 3, h, w)
             im = np.ascontiguousarray(im)  # contiguous
             im = torch.from_numpy(im)
         # NOTE: assuming im with (b, 3, h, w) if it's a tensor
         img = im.to(self.device)
         img = img.half() if self.model.fp16 else img.float()  # uint8 to fp16/32
```

### Comparing `ultralytics-8.0.91/ultralytics/yolo/engine/results.py` & `ultralytics-8.0.92/ultralytics/yolo/engine/results.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.91/ultralytics/yolo/engine/trainer.py` & `ultralytics-8.0.92/ultralytics/yolo/engine/trainer.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.91/ultralytics/yolo/engine/validator.py` & `ultralytics-8.0.92/ultralytics/yolo/engine/validator.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.91/ultralytics/yolo/utils/__init__.py` & `ultralytics-8.0.92/ultralytics/yolo/utils/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -255,21 +255,22 @@
         None: Data is saved to the specified file.
     """
     file = Path(file)
     if not file.parent.exists():
         # Create parent directories if they don't exist
         file.parent.mkdir(parents=True, exist_ok=True)
 
+    # Convert Path objects to strings
+    for k, v in data.items():
+        if isinstance(v, Path):
+            dict[k] = str(v)
+
+    # Dump data to file in YAML format
     with open(file, 'w') as f:
-        # Dump data to file in YAML format, converting Path objects to strings
-        yaml.safe_dump({k: str(v) if isinstance(v, Path) else v
-                        for k, v in data.items()},
-                       f,
-                       sort_keys=False,
-                       allow_unicode=True)
+        yaml.safe_dump(data, f, sort_keys=False, allow_unicode=True)
 
 
 def yaml_load(file='data.yaml', append_filename=False):
     """
     Load YAML data from a file.
 
     Args:
@@ -755,15 +756,15 @@
 SETTINGS = get_settings()
 DATASETS_DIR = Path(SETTINGS['datasets_dir'])  # global datasets directory
 ENVIRONMENT = 'Colab' if is_colab() else 'Kaggle' if is_kaggle() else 'Jupyter' if is_jupyter() else \
     'Docker' if is_docker() else platform.system()
 TESTS_RUNNING = is_pytest_running() or is_github_actions_ci()
 set_sentry()
 
-# OpenCV Multilanguage-friendly functions ------------------------------------------------------------------------------------
+# OpenCV Multilanguage-friendly functions ------------------------------------------------------------------------------
 imshow_ = cv2.imshow  # copy to avoid recursion errors
 
 
 def imread(filename, flags=cv2.IMREAD_COLOR):
     return cv2.imdecode(np.fromfile(filename, np.uint8), flags)
```

### Comparing `ultralytics-8.0.91/ultralytics/yolo/utils/autobatch.py` & `ultralytics-8.0.92/ultralytics/yolo/utils/autobatch.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.91/ultralytics/yolo/utils/benchmarks.py` & `ultralytics-8.0.92/ultralytics/yolo/utils/benchmarks.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.91/ultralytics/yolo/utils/callbacks/base.py` & `ultralytics-8.0.92/ultralytics/yolo/utils/callbacks/base.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.91/ultralytics/yolo/utils/callbacks/clearml.py` & `ultralytics-8.0.92/ultralytics/yolo/utils/callbacks/clearml.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.91/ultralytics/yolo/utils/callbacks/comet.py` & `ultralytics-8.0.92/ultralytics/yolo/utils/callbacks/comet.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.91/ultralytics/yolo/utils/callbacks/hub.py` & `ultralytics-8.0.92/ultralytics/yolo/utils/callbacks/hub.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.91/ultralytics/yolo/utils/callbacks/mlflow.py` & `ultralytics-8.0.92/ultralytics/yolo/utils/callbacks/mlflow.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.91/ultralytics/yolo/utils/callbacks/neptune.py` & `ultralytics-8.0.92/ultralytics/yolo/utils/callbacks/neptune.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.91/ultralytics/yolo/utils/callbacks/tensorboard.py` & `ultralytics-8.0.92/ultralytics/yolo/utils/callbacks/tensorboard.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.91/ultralytics/yolo/utils/callbacks/wb.py` & `ultralytics-8.0.92/ultralytics/yolo/utils/callbacks/wb.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.91/ultralytics/yolo/utils/checks.py` & `ultralytics-8.0.92/ultralytics/yolo/utils/checks.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.91/ultralytics/yolo/utils/dist.py` & `ultralytics-8.0.92/ultralytics/yolo/utils/dist.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.91/ultralytics/yolo/utils/downloads.py` & `ultralytics-8.0.92/ultralytics/yolo/utils/downloads.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.91/ultralytics/yolo/utils/files.py` & `ultralytics-8.0.92/ultralytics/yolo/utils/files.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.91/ultralytics/yolo/utils/instance.py` & `ultralytics-8.0.92/ultralytics/yolo/utils/instance.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.91/ultralytics/yolo/utils/loss.py` & `ultralytics-8.0.92/ultralytics/yolo/utils/loss.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.91/ultralytics/yolo/utils/metrics.py` & `ultralytics-8.0.92/ultralytics/yolo/utils/metrics.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.91/ultralytics/yolo/utils/ops.py` & `ultralytics-8.0.92/ultralytics/yolo/utils/ops.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.91/ultralytics/yolo/utils/plotting.py` & `ultralytics-8.0.92/ultralytics/yolo/utils/plotting.py`

 * *Files 1% similar despite different names*

```diff
@@ -477,17 +477,14 @@
 
     Args:
         x (torch.Tensor): Features to be visualized.
         module_type (str): Module type.
         stage (int): Module stage within the model.
         n (int, optional): Maximum number of feature maps to plot. Defaults to 32.
         save_dir (Path, optional): Directory to save results. Defaults to Path('runs/detect/exp').
-
-    Returns:
-        None: This function does not return any value; it saves the visualization to the specified directory.
     """
     for m in ['Detect', 'Pose', 'Segment']:
         if m in module_type:
             return
     batch, channels, height, width = x.shape  # batch, channels, height, width
     if height > 1 and width > 1:
         f = save_dir / f"stage{stage}_{module_type.split('.')[-1]}_features.png"  # filename
```

### Comparing `ultralytics-8.0.91/ultralytics/yolo/utils/tal.py` & `ultralytics-8.0.92/ultralytics/yolo/utils/tal.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.91/ultralytics/yolo/utils/torch_utils.py` & `ultralytics-8.0.92/ultralytics/yolo/utils/torch_utils.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.91/ultralytics/yolo/utils/tuner.py` & `ultralytics-8.0.92/ultralytics/yolo/utils/tuner.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.91/ultralytics/yolo/v8/classify/predict.py` & `ultralytics-8.0.92/ultralytics/yolo/v8/classify/predict.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.91/ultralytics/yolo/v8/classify/train.py` & `ultralytics-8.0.92/ultralytics/yolo/v8/classify/train.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.91/ultralytics/yolo/v8/classify/val.py` & `ultralytics-8.0.92/ultralytics/yolo/v8/classify/val.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.91/ultralytics/yolo/v8/detect/predict.py` & `ultralytics-8.0.92/ultralytics/yolo/v8/detect/predict.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.91/ultralytics/yolo/v8/detect/train.py` & `ultralytics-8.0.92/ultralytics/yolo/v8/detect/train.py`

 * *Files 0% similar despite different names*

```diff
@@ -208,23 +208,23 @@
         # pboxes
         pred_bboxes = self.bbox_decode(anchor_points, pred_distri)  # xyxy, (b, h*w, 4)
 
         _, target_bboxes, target_scores, fg_mask, _ = self.assigner(
             pred_scores.detach().sigmoid(), (pred_bboxes.detach() * stride_tensor).type(gt_bboxes.dtype),
             anchor_points * stride_tensor, gt_labels, gt_bboxes, mask_gt)
 
-        target_bboxes /= stride_tensor
         target_scores_sum = max(target_scores.sum(), 1)
 
         # cls loss
         # loss[1] = self.varifocal_loss(pred_scores, target_scores, target_labels) / target_scores_sum  # VFL way
         loss[1] = self.bce(pred_scores, target_scores.to(dtype)).sum() / target_scores_sum  # BCE
 
         # bbox loss
         if fg_mask.sum():
+            target_bboxes /= stride_tensor
             loss[0], loss[2] = self.bbox_loss(pred_distri, pred_bboxes, anchor_points, target_bboxes, target_scores,
                                               target_scores_sum, fg_mask)
 
         loss[0] *= self.hyp.box  # box gain
         loss[1] *= self.hyp.cls  # cls gain
         loss[2] *= self.hyp.dfl  # dfl gain
```

### Comparing `ultralytics-8.0.91/ultralytics/yolo/v8/detect/val.py` & `ultralytics-8.0.92/ultralytics/yolo/v8/detect/val.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.91/ultralytics/yolo/v8/pose/predict.py` & `ultralytics-8.0.92/ultralytics/yolo/v8/pose/predict.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.91/ultralytics/yolo/v8/pose/train.py` & `ultralytics-8.0.92/ultralytics/yolo/v8/pose/train.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.91/ultralytics/yolo/v8/pose/val.py` & `ultralytics-8.0.92/ultralytics/yolo/v8/pose/val.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.91/ultralytics/yolo/v8/segment/predict.py` & `ultralytics-8.0.92/ultralytics/yolo/v8/segment/predict.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.91/ultralytics/yolo/v8/segment/train.py` & `ultralytics-8.0.92/ultralytics/yolo/v8/segment/train.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.91/ultralytics/yolo/v8/segment/val.py` & `ultralytics-8.0.92/ultralytics/yolo/v8/segment/val.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.91/ultralytics.egg-info/PKG-INFO` & `ultralytics-8.0.92/ultralytics.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ultralytics
-Version: 8.0.91
+Version: 8.0.92
 Summary: Ultralytics YOLOv8
 Home-page: https://github.com/ultralytics/ultralytics
 Author: Ultralytics
 Author-email: hello@ultralytics.com
 License: AGPL-3.0
 Project-URL: Bug Reports, https://github.com/ultralytics/ultralytics/issues
 Project-URL: Funding, https://ultralytics.com
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: ultralytics Version: 8.0.91 Summary: Ultralytics
+Metadata-Version: 2.1 Name: ultralytics Version: 8.0.92 Summary: Ultralytics
 YOLOv8 Home-page: https://github.com/ultralytics/ultralytics Author:
 Ultralytics Author-email: hello@ultralytics.com License: AGPL-3.0 Project-URL:
 Bug Reports, https://github.com/ultralytics/ultralytics/issues Project-URL:
 Funding, https://ultralytics.com Project-URL: Source, https://github.com/
 ultralytics/ultralytics Keywords: machine-learning,deep-
 learning,vision,ML,DL,AI,YOLO,YOLOv3,YOLOv5,YOLOv8,HUB,Ultralytics Classifier:
 Development Status :: 4 - Beta Classifier: Intended Audience :: Developers
```

### Comparing `ultralytics-8.0.91/ultralytics.egg-info/SOURCES.txt` & `ultralytics-8.0.92/ultralytics.egg-info/SOURCES.txt`

 * *Files identical despite different names*

