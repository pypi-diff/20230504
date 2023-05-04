# Comparing `tmp/tf-models-official-2.9.1.tar.gz` & `tmp/tf-models-official-2.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tf-models-official-2.9.1.tar", last modified: Thu May 19 23:14:06 2022, max compression
+gzip compressed data, was "tf-models-official-2.9.2.tar", last modified: Fri May 20 04:44:40 2022, max compression
```

## Comparing `tf-models-official-2.9.1.tar` & `tf-models-official-2.9.2.tar`

### file list

```diff
@@ -1,990 +1,990 @@
-drwxr-x---   0 hongkuny (405338) primarygroup (89939)        0 2022-05-19 23:14:06.796168 tf-models-official-2.9.1/
--rw-r-----   0 hongkuny (405338) primarygroup (89939)      337 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/AUTHORS
--rw-r-----   0 hongkuny (405338) primarygroup (89939)    11405 2022-05-18 02:34:16.000000 tf-models-official-2.9.1/LICENSE
--rw-r-----   0 hongkuny (405338) primarygroup (89939)      603 2022-05-19 23:14:06.796168 tf-models-official-2.9.1/PKG-INFO
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     3072 2022-05-18 02:34:16.000000 tf-models-official-2.9.1/README.md
-drwxr-x---   0 hongkuny (405338) primarygroup (89939)        0 2022-05-19 23:14:06.724169 tf-models-official-2.9.1/official/
--rw-r-----   0 hongkuny (405338) primarygroup (89939)      609 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/__init__.py
-drwxr-x---   0 hongkuny (405338) primarygroup (89939)        0 2022-05-19 23:14:06.728169 tf-models-official-2.9.1/official/common/
--rw-r-----   0 hongkuny (405338) primarygroup (89939)      610 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/common/__init__.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     1848 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/common/dataset_fn.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     8585 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/common/distribute_utils.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     4904 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/common/distribute_utils_test.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     4166 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/common/flags.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)      843 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/common/registry_imports.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     1057 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/common/streamz_counters.py
-drwxr-x---   0 hongkuny (405338) primarygroup (89939)        0 2022-05-19 23:14:06.728169 tf-models-official-2.9.1/official/core/
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     1075 2022-05-19 22:57:12.000000 tf-models-official-2.9.1/official/core/__init__.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     8083 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/core/actions.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     4515 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/core/actions_test.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)    12890 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/core/base_task.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)    17377 2022-05-18 02:34:16.000000 tf-models-official-2.9.1/official/core/base_trainer.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)    13804 2022-05-18 02:34:16.000000 tf-models-official-2.9.1/official/core/base_trainer_test.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)    12208 2022-05-18 02:34:16.000000 tf-models-official-2.9.1/official/core/config_definitions.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     1115 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/core/exp_factory.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     7025 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/core/export_base.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     4426 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/core/export_base_test.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)    21463 2022-05-18 02:34:16.000000 tf-models-official-2.9.1/official/core/input_reader.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     4300 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/core/registry.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     2350 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/core/registry_test.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     2513 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/core/task_factory.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     1802 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/core/test_utils.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     5562 2022-05-18 02:34:16.000000 tf-models-official-2.9.1/official/core/train_lib.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     7917 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/core/train_lib_test.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)    19771 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/core/train_utils.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     7169 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/core/train_utils_test.py
-drwxr-x---   0 hongkuny (405338) primarygroup (89939)        0 2022-05-19 23:14:06.728169 tf-models-official-2.9.1/official/legacy/
--rw-r-----   0 hongkuny (405338) primarygroup (89939)      609 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/legacy/__init__.py
-drwxr-x---   0 hongkuny (405338) primarygroup (89939)        0 2022-05-19 23:14:06.728169 tf-models-official-2.9.1/official/legacy/albert/
--rw-r-----   0 hongkuny (405338) primarygroup (89939)      609 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/legacy/albert/__init__.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     2012 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/legacy/albert/configs.py
-drwxr-x---   0 hongkuny (405338) primarygroup (89939)        0 2022-05-19 23:14:06.728169 tf-models-official-2.9.1/official/legacy/bert/
--rw-r-----   0 hongkuny (405338) primarygroup (89939)      610 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/legacy/bert/__init__.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)    14931 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/legacy/bert/bert_models.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     3883 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/legacy/bert/bert_models_test.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     4832 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/legacy/bert/common_flags.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     4167 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/legacy/bert/configs.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     5966 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/legacy/bert/export_tfhub.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     4688 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/legacy/bert/export_tfhub_test.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)    11724 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/legacy/bert/input_pipeline.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     2875 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/legacy/bert/model_saving_utils.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)    25317 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/legacy/bert/model_training_utils.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)    11705 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/legacy/bert/model_training_utils_test.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)    18826 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/legacy/bert/run_classifier.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     8410 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/legacy/bert/run_pretraining.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     5366 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/legacy/bert/run_squad.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)    18945 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/legacy/bert/run_squad_helper.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     5054 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/legacy/bert/serving.py
-drwxr-x---   0 hongkuny (405338) primarygroup (89939)        0 2022-05-19 23:14:06.728169 tf-models-official-2.9.1/official/legacy/detection/
--rw-r-----   0 hongkuny (405338) primarygroup (89939)      609 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/legacy/detection/__init__.py
-drwxr-x---   0 hongkuny (405338) primarygroup (89939)        0 2022-05-19 23:14:06.732169 tf-models-official-2.9.1/official/legacy/detection/configs/
--rw-r-----   0 hongkuny (405338) primarygroup (89939)      609 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/legacy/detection/configs/__init__.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     4468 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/legacy/detection/configs/base_config.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     1692 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/legacy/detection/configs/factory.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     3328 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/legacy/detection/configs/maskrcnn_config.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     4271 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/legacy/detection/configs/olnmask_config.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     1776 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/legacy/detection/configs/retinanet_config.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     3204 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/legacy/detection/configs/shapemask_config.py
-drwxr-x---   0 hongkuny (405338) primarygroup (89939)        0 2022-05-19 23:14:06.732169 tf-models-official-2.9.1/official/legacy/detection/dataloader/
--rw-r-----   0 hongkuny (405338) primarygroup (89939)      609 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/legacy/detection/dataloader/__init__.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)    20689 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/legacy/detection/dataloader/anchor.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     6563 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/legacy/detection/dataloader/factory.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     3653 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/legacy/detection/dataloader/input_reader.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)    15731 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/legacy/detection/dataloader/maskrcnn_parser.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     1061 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/legacy/detection/dataloader/mode_keys.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)    14218 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/legacy/detection/dataloader/olnmask_parser.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)    18283 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/legacy/detection/dataloader/retinanet_parser.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)    22331 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/legacy/detection/dataloader/shapemask_parser.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     6219 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/legacy/detection/dataloader/tf_example_decoder.py
-drwxr-x---   0 hongkuny (405338) primarygroup (89939)        0 2022-05-19 23:14:06.732169 tf-models-official-2.9.1/official/legacy/detection/evaluation/
--rw-r-----   0 hongkuny (405338) primarygroup (89939)      609 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/legacy/detection/evaluation/__init__.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)    24838 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/legacy/detection/evaluation/coco_evaluator.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)    15169 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/legacy/detection/evaluation/coco_utils.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     2169 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/legacy/detection/evaluation/factory.py
-drwxr-x---   0 hongkuny (405338) primarygroup (89939)        0 2022-05-19 23:14:06.732169 tf-models-official-2.9.1/official/legacy/detection/executor/
--rw-r-----   0 hongkuny (405338) primarygroup (89939)      609 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/legacy/detection/executor/__init__.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     6259 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/legacy/detection/executor/detection_executor.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)    30080 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/legacy/detection/executor/distributed_executor.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     9015 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/legacy/detection/main.py
-drwxr-x---   0 hongkuny (405338) primarygroup (89939)        0 2022-05-19 23:14:06.732169 tf-models-official-2.9.1/official/legacy/detection/modeling/
--rw-r-----   0 hongkuny (405338) primarygroup (89939)      609 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/legacy/detection/modeling/__init__.py
-drwxr-x---   0 hongkuny (405338) primarygroup (89939)        0 2022-05-19 23:14:06.732169 tf-models-official-2.9.1/official/legacy/detection/modeling/architecture/
--rw-r-----   0 hongkuny (405338) primarygroup (89939)      609 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/legacy/detection/modeling/architecture/__init__.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     7994 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/legacy/detection/modeling/architecture/factory.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     5976 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/legacy/detection/modeling/architecture/fpn.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)    49476 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/legacy/detection/modeling/architecture/heads.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)      974 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/legacy/detection/modeling/architecture/identity.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)    11219 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/legacy/detection/modeling/architecture/nn_blocks.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     3853 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/legacy/detection/modeling/architecture/nn_ops.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)    13159 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/legacy/detection/modeling/architecture/resnet.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)    17270 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/legacy/detection/modeling/architecture/spinenet.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     4439 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/legacy/detection/modeling/base_model.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     4862 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/legacy/detection/modeling/checkpoint_utils.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     1402 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/legacy/detection/modeling/factory.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     3800 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/legacy/detection/modeling/learning_rates.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)    30203 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/legacy/detection/modeling/losses.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)    13458 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/legacy/detection/modeling/maskrcnn_model.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)    16774 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/legacy/detection/modeling/olnmask_model.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     1716 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/legacy/detection/modeling/optimizers.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     6661 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/legacy/detection/modeling/retinanet_model.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)    12110 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/legacy/detection/modeling/shapemask_model.py
-drwxr-x---   0 hongkuny (405338) primarygroup (89939)        0 2022-05-19 23:14:06.732169 tf-models-official-2.9.1/official/legacy/detection/ops/
--rw-r-----   0 hongkuny (405338) primarygroup (89939)      609 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/legacy/detection/ops/__init__.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     8125 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/legacy/detection/ops/nms.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)    21942 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/legacy/detection/ops/postprocess_ops.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)    22986 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/legacy/detection/ops/roi_ops.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)    25998 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/legacy/detection/ops/spatial_transform_ops.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)    28304 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/legacy/detection/ops/target_ops.py
-drwxr-x---   0 hongkuny (405338) primarygroup (89939)        0 2022-05-19 23:14:06.736169 tf-models-official-2.9.1/official/legacy/detection/utils/
--rw-r-----   0 hongkuny (405338) primarygroup (89939)      609 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/legacy/detection/utils/__init__.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)    26050 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/legacy/detection/utils/box_utils.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     1465 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/legacy/detection/utils/class_utils.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     1575 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/legacy/detection/utils/dataloader_utils.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)    14297 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/legacy/detection/utils/input_utils.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     6647 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/legacy/detection/utils/mask_utils.py
-drwxr-x---   0 hongkuny (405338) primarygroup (89939)        0 2022-05-19 23:14:06.736169 tf-models-official-2.9.1/official/legacy/image_classification/
--rw-r-----   0 hongkuny (405338) primarygroup (89939)      609 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/legacy/image_classification/__init__.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)    34315 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/legacy/image_classification/augment.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     4313 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/legacy/image_classification/augment_test.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     9355 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/legacy/image_classification/callbacks.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)    16195 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/legacy/image_classification/classifier_trainer.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     7755 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/legacy/image_classification/classifier_trainer_test.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     6047 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/legacy/image_classification/classifier_trainer_util_test.py
-drwxr-x---   0 hongkuny (405338) primarygroup (89939)        0 2022-05-19 23:14:06.736169 tf-models-official-2.9.1/official/legacy/image_classification/configs/
--rw-r-----   0 hongkuny (405338) primarygroup (89939)      609 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/legacy/image_classification/configs/__init__.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     8668 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/legacy/image_classification/configs/base_configs.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     6110 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/legacy/image_classification/configs/configs.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)    19517 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/legacy/image_classification/dataset_factory.py
-drwxr-x---   0 hongkuny (405338) primarygroup (89939)        0 2022-05-19 23:14:06.736169 tf-models-official-2.9.1/official/legacy/image_classification/efficientnet/
--rw-r-----   0 hongkuny (405338) primarygroup (89939)      609 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/legacy/image_classification/efficientnet/__init__.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     4609 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/legacy/image_classification/efficientnet/common_modules.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     2867 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/legacy/image_classification/efficientnet/efficientnet_config.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)    16417 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/legacy/image_classification/efficientnet/efficientnet_model.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     2317 2022-05-18 02:34:16.000000 tf-models-official-2.9.1/official/legacy/image_classification/efficientnet/tfhub_export.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     4272 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/legacy/image_classification/learning_rate.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     1941 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/legacy/image_classification/learning_rate_test.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     6114 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/legacy/image_classification/mnist_main.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     2581 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/legacy/image_classification/mnist_test.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     6844 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/legacy/image_classification/optimizer_factory.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     4067 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/legacy/image_classification/optimizer_factory_test.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)    13537 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/legacy/image_classification/preprocessing.py
-drwxr-x---   0 hongkuny (405338) primarygroup (89939)        0 2022-05-19 23:14:06.736169 tf-models-official-2.9.1/official/legacy/image_classification/resnet/
--rw-r-----   0 hongkuny (405338) primarygroup (89939)      609 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/legacy/image_classification/resnet/__init__.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)    16094 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/legacy/image_classification/resnet/common.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)    21168 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/legacy/image_classification/resnet/imagenet_preprocessing.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     2070 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/legacy/image_classification/resnet/resnet_config.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     6916 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/legacy/image_classification/resnet/resnet_ctl_imagenet_main.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)    10945 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/legacy/image_classification/resnet/resnet_model.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     8124 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/legacy/image_classification/resnet/resnet_runnable.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     2189 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/legacy/image_classification/resnet/tfhub_export.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     1322 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/legacy/image_classification/test_utils.py
-drwxr-x---   0 hongkuny (405338) primarygroup (89939)        0 2022-05-19 23:14:06.736169 tf-models-official-2.9.1/official/legacy/image_classification/vgg/
--rw-r-----   0 hongkuny (405338) primarygroup (89939)      610 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/legacy/image_classification/vgg/__init__.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     1803 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/legacy/image_classification/vgg/vgg_config.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     7607 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/legacy/image_classification/vgg/vgg_model.py
-drwxr-x---   0 hongkuny (405338) primarygroup (89939)        0 2022-05-19 23:14:06.740169 tf-models-official-2.9.1/official/legacy/transformer/
--rw-r-----   0 hongkuny (405338) primarygroup (89939)      609 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/legacy/transformer/__init__.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     7047 2022-05-18 02:34:16.000000 tf-models-official-2.9.1/official/legacy/transformer/attention_layer.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     3679 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/legacy/transformer/beam_search_v1.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     5141 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/legacy/transformer/compute_bleu.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     2585 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/legacy/transformer/compute_bleu_test.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)    15295 2022-05-18 02:34:16.000000 tf-models-official-2.9.1/official/legacy/transformer/data_download.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)    13237 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/legacy/transformer/data_pipeline.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     3684 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/legacy/transformer/embedding_layer.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     2320 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/legacy/transformer/ffn_layer.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     7007 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/legacy/transformer/metrics.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)    10346 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/legacy/transformer/misc.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     2936 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/legacy/transformer/model_params.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     4427 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/legacy/transformer/model_utils.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     1891 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/legacy/transformer/model_utils_test.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     2434 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/legacy/transformer/optimizer.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)    21751 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/legacy/transformer/transformer.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     6060 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/legacy/transformer/transformer_forward_test.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     3566 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/legacy/transformer/transformer_layers_test.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)    18183 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/legacy/transformer/transformer_main.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     6631 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/legacy/transformer/transformer_main_test.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     3628 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/legacy/transformer/transformer_test.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     6951 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/legacy/transformer/translate.py
-drwxr-x---   0 hongkuny (405338) primarygroup (89939)        0 2022-05-19 23:14:06.740169 tf-models-official-2.9.1/official/legacy/transformer/utils/
--rw-r-----   0 hongkuny (405338) primarygroup (89939)      609 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/legacy/transformer/utils/__init__.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)    16706 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/legacy/transformer/utils/metrics.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)    24517 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/legacy/transformer/utils/tokenizer.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     6658 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/legacy/transformer/utils/tokenizer_test.py
-drwxr-x---   0 hongkuny (405338) primarygroup (89939)        0 2022-05-19 23:14:06.740169 tf-models-official-2.9.1/official/legacy/xlnet/
--rw-r-----   0 hongkuny (405338) primarygroup (89939)      610 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/legacy/xlnet/__init__.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     5421 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/legacy/xlnet/classifier_utils.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     5367 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/legacy/xlnet/common_flags.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)    30095 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/legacy/xlnet/data_utils.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     3762 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/legacy/xlnet/optimization.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)    15344 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/legacy/xlnet/preprocess_classification_data.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)    32400 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/legacy/xlnet/preprocess_pretrain_data.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     4046 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/legacy/xlnet/preprocess_squad_data.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     3693 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/legacy/xlnet/preprocess_utils.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     6976 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/legacy/xlnet/run_classifier.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     5710 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/legacy/xlnet/run_pretrain.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)    11597 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/legacy/xlnet/run_squad.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)    32226 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/legacy/xlnet/squad_utils.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)    11664 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/legacy/xlnet/training_utils.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     5894 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/legacy/xlnet/xlnet_config.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)    47595 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/legacy/xlnet/xlnet_modeling.py
-drwxr-x---   0 hongkuny (405338) primarygroup (89939)        0 2022-05-19 23:14:06.740169 tf-models-official-2.9.1/official/modeling/
--rw-r-----   0 hongkuny (405338) primarygroup (89939)      609 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/modeling/__init__.py
-drwxr-x---   0 hongkuny (405338) primarygroup (89939)        0 2022-05-19 23:14:06.744169 tf-models-official-2.9.1/official/modeling/activations/
--rw-r-----   0 hongkuny (405338) primarygroup (89939)      992 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/modeling/activations/__init__.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     1037 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/modeling/activations/gelu.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     1212 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/modeling/activations/gelu_test.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)      984 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/modeling/activations/relu.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     1200 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/modeling/activations/relu_test.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     1041 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/modeling/activations/sigmoid.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     1364 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/modeling/activations/sigmoid_test.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     2291 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/modeling/activations/swish.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     1566 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/modeling/activations/swish_test.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     6730 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/modeling/grad_utils.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     2786 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/modeling/grad_utils_test.py
-drwxr-x---   0 hongkuny (405338) primarygroup (89939)        0 2022-05-19 23:14:06.744169 tf-models-official-2.9.1/official/modeling/hyperparams/
--rw-r-----   0 hongkuny (405338) primarygroup (89939)      846 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/modeling/hyperparams/__init__.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)    11213 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/modeling/hyperparams/base_config.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)    11413 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/modeling/hyperparams/base_config_test.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     1870 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/modeling/hyperparams/oneof.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     1882 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/modeling/hyperparams/oneof_test.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)    16402 2022-05-18 02:34:16.000000 tf-models-official-2.9.1/official/modeling/hyperparams/params_dict.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)    13657 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/modeling/hyperparams/params_dict_test.py
-drwxr-x---   0 hongkuny (405338) primarygroup (89939)        0 2022-05-19 23:14:06.744169 tf-models-official-2.9.1/official/modeling/multitask/
--rw-r-----   0 hongkuny (405338) primarygroup (89939)      609 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/modeling/multitask/__init__.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     1538 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/modeling/multitask/base_model.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     5846 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/modeling/multitask/base_trainer.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     3653 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/modeling/multitask/base_trainer_test.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     2683 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/modeling/multitask/configs.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     6068 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/modeling/multitask/evaluator.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     4633 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/modeling/multitask/evaluator_test.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     3948 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/modeling/multitask/interleaving_trainer.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     4295 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/modeling/multitask/interleaving_trainer_test.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     5946 2022-05-18 02:34:16.000000 tf-models-official-2.9.1/official/modeling/multitask/multitask.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     4887 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/modeling/multitask/task_sampler.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     3027 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/modeling/multitask/task_sampler_test.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     3887 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/modeling/multitask/test_utils.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     9741 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/modeling/multitask/train_lib.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     4622 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/modeling/multitask/train_lib_test.py
-drwxr-x---   0 hongkuny (405338) primarygroup (89939)        0 2022-05-19 23:14:06.744169 tf-models-official-2.9.1/official/modeling/optimization/
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     1201 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/modeling/optimization/__init__.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)      792 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/modeling/optimization/adafactor_optimizer.py
-drwxr-x---   0 hongkuny (405338) primarygroup (89939)        0 2022-05-19 23:14:06.744169 tf-models-official-2.9.1/official/modeling/optimization/configs/
--rw-r-----   0 hongkuny (405338) primarygroup (89939)      609 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/modeling/optimization/configs/__init__.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)    11122 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/modeling/optimization/configs/learning_rate_config.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     4707 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/modeling/optimization/configs/optimization_config.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     2009 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/modeling/optimization/configs/optimization_config_test.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)    10717 2022-05-18 02:34:16.000000 tf-models-official-2.9.1/official/modeling/optimization/configs/optimizer_config.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     9086 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/modeling/optimization/ema_optimizer.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     7331 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/modeling/optimization/lars_optimizer.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)    19101 2022-05-18 02:34:16.000000 tf-models-official-2.9.1/official/modeling/optimization/lr_schedule.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     3951 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/modeling/optimization/lr_schedule_test.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     7854 2022-05-18 02:34:16.000000 tf-models-official-2.9.1/official/modeling/optimization/optimizer_factory.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)    14110 2022-05-18 02:34:16.000000 tf-models-official-2.9.1/official/modeling/optimization/optimizer_factory_test.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)      707 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/modeling/optimization/slide_optimizer.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     2159 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/modeling/performance.py
-drwxr-x---   0 hongkuny (405338) primarygroup (89939)        0 2022-05-19 23:14:06.744169 tf-models-official-2.9.1/official/modeling/privacy/
--rw-r-----   0 hongkuny (405338) primarygroup (89939)      609 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/modeling/privacy/__init__.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)      960 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/modeling/privacy/configs.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     1359 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/modeling/privacy/configs_test.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     1452 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/modeling/privacy/ops.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     1684 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/modeling/privacy/ops_test.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     8834 2022-05-18 02:34:16.000000 tf-models-official-2.9.1/official/modeling/tf_utils.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     2967 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/modeling/tf_utils_test.py
-drwxr-x---   0 hongkuny (405338) primarygroup (89939)        0 2022-05-19 23:14:06.744169 tf-models-official-2.9.1/official/nlp/
--rw-r-----   0 hongkuny (405338) primarygroup (89939)      609 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/nlp/__init__.py
-drwxr-x---   0 hongkuny (405338) primarygroup (89939)        0 2022-05-19 23:14:06.748169 tf-models-official-2.9.1/official/nlp/configs/
--rw-r-----   0 hongkuny (405338) primarygroup (89939)      609 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/nlp/configs/__init__.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     1423 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/nlp/configs/bert.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     1381 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/nlp/configs/electra.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)    22095 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/nlp/configs/encoders.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     1963 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/nlp/configs/encoders_test.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)      899 2022-05-18 02:34:16.000000 tf-models-official-2.9.1/official/nlp/configs/experiment_configs.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     6571 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/nlp/configs/finetuning_experiments.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     2968 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/nlp/configs/pretraining_experiments.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     3791 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/nlp/configs/wmt_transformer_experiments.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     7884 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/nlp/continuous_finetune_lib.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     3182 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/nlp/continuous_finetune_lib_test.py
-drwxr-x---   0 hongkuny (405338) primarygroup (89939)        0 2022-05-19 23:14:06.748169 tf-models-official-2.9.1/official/nlp/data/
--rw-r-----   0 hongkuny (405338) primarygroup (89939)      609 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/nlp/data/__init__.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)    56381 2022-05-18 02:34:16.000000 tf-models-official-2.9.1/official/nlp/data/classifier_data_lib.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     3352 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/nlp/data/classifier_data_lib_test.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)    16693 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/nlp/data/create_finetuning_data.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)    23360 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/nlp/data/create_pretraining_data.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     4857 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/nlp/data/create_pretraining_data_test.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)    24192 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/nlp/data/create_xlnet_pretraining_data.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)    10930 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/nlp/data/create_xlnet_pretraining_data_test.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     1688 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/nlp/data/data_loader.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     1788 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/nlp/data/data_loader_factory.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     1325 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/nlp/data/data_loader_factory_test.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     5713 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/nlp/data/dual_encoder_dataloader.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     5040 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/nlp/data/dual_encoder_dataloader_test.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)    24634 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/nlp/data/pretrain_dataloader.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     9141 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/nlp/data/pretrain_dataloader_test.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     9814 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/nlp/data/pretrain_dynamic_dataloader.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     9620 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/nlp/data/pretrain_dynamic_dataloader_test.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     4308 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/nlp/data/question_answering_dataloader.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     2830 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/nlp/data/question_answering_dataloader_test.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)    10337 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/nlp/data/sentence_prediction_dataloader.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)    11662 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/nlp/data/sentence_prediction_dataloader_test.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     6413 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/nlp/data/sentence_retrieval_lib.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)    36512 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/nlp/data/squad_lib.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)    34939 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/nlp/data/squad_lib_sp.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)    15489 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/nlp/data/tagging_data_lib.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     3737 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/nlp/data/tagging_data_lib_test.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     3181 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/nlp/data/tagging_dataloader.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     3196 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/nlp/data/tagging_dataloader_test.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     4517 2022-05-18 02:34:16.000000 tf-models-official-2.9.1/official/nlp/data/train_sentencepiece.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)    11174 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/nlp/data/wmt_dataloader.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     4892 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/nlp/data/wmt_dataloader_test.py
-drwxr-x---   0 hongkuny (405338) primarygroup (89939)        0 2022-05-19 23:14:06.748169 tf-models-official-2.9.1/official/nlp/metrics/
--rw-r-----   0 hongkuny (405338) primarygroup (89939)      609 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/nlp/metrics/__init__.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     6577 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/nlp/metrics/bleu.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     2498 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/nlp/metrics/bleu_test.py
-drwxr-x---   0 hongkuny (405338) primarygroup (89939)        0 2022-05-19 23:14:06.748169 tf-models-official-2.9.1/official/nlp/modeling/
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     1062 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/nlp/modeling/__init__.py
-drwxr-x---   0 hongkuny (405338) primarygroup (89939)        0 2022-05-19 23:14:06.756169 tf-models-official-2.9.1/official/nlp/modeling/layers/
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     3712 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/nlp/modeling/layers/__init__.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     3909 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/nlp/modeling/layers/attention.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     3681 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/nlp/modeling/layers/attention_test.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)    21026 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/nlp/modeling/layers/bigbird_attention.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     2196 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/nlp/modeling/layers/bigbird_attention_test.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     6915 2022-05-18 02:34:16.000000 tf-models-official-2.9.1/official/nlp/modeling/layers/block_diag_feedforward.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     4302 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/nlp/modeling/layers/block_diag_feedforward_test.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)    13104 2022-05-18 02:34:16.000000 tf-models-official-2.9.1/official/nlp/modeling/layers/cls_head.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     7841 2022-05-18 02:34:16.000000 tf-models-official-2.9.1/official/nlp/modeling/layers/cls_head_test.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     9058 2022-05-18 02:34:16.000000 tf-models-official-2.9.1/official/nlp/modeling/layers/gated_feedforward.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     4806 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/nlp/modeling/layers/gated_feedforward_test.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)    20472 2022-05-18 02:34:16.000000 tf-models-official-2.9.1/official/nlp/modeling/layers/gaussian_process.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)    10091 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/nlp/modeling/layers/gaussian_process_test.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)    15968 2022-05-18 02:34:16.000000 tf-models-official-2.9.1/official/nlp/modeling/layers/kernel_attention.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     4190 2022-05-18 02:34:16.000000 tf-models-official-2.9.1/official/nlp/modeling/layers/kernel_attention_test.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     4826 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/nlp/modeling/layers/masked_lm.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     5853 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/nlp/modeling/layers/masked_lm_test.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     3028 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/nlp/modeling/layers/masked_softmax.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     4694 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/nlp/modeling/layers/masked_softmax_test.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     2294 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/nlp/modeling/layers/mat_mul_with_margin.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     2136 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/nlp/modeling/layers/mat_mul_with_margin_test.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)    22368 2022-05-18 02:34:16.000000 tf-models-official-2.9.1/official/nlp/modeling/layers/mobile_bert_layers.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)    10880 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/nlp/modeling/layers/mobile_bert_layers_test.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     7192 2022-05-18 02:34:16.000000 tf-models-official-2.9.1/official/nlp/modeling/layers/multi_channel_attention.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     1912 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/nlp/modeling/layers/multi_channel_attention_test.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     3960 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/nlp/modeling/layers/on_device_embedding.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     8880 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/nlp/modeling/layers/on_device_embedding_test.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)    11393 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/nlp/modeling/layers/position_embedding.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     8538 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/nlp/modeling/layers/position_embedding_test.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)    20486 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/nlp/modeling/layers/relative_attention.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     6806 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/nlp/modeling/layers/relative_attention_test.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)    24761 2022-05-18 02:34:16.000000 tf-models-official-2.9.1/official/nlp/modeling/layers/reuse_attention.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)    14319 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/nlp/modeling/layers/reuse_attention_test.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)    15396 2022-05-18 02:34:16.000000 tf-models-official-2.9.1/official/nlp/modeling/layers/reuse_transformer.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)    17478 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/nlp/modeling/layers/reuse_transformer_test.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)    11686 2022-05-18 02:34:16.000000 tf-models-official-2.9.1/official/nlp/modeling/layers/rezero_transformer.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     5874 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/nlp/modeling/layers/rezero_transformer_test.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     4559 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/nlp/modeling/layers/routing.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     2216 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/nlp/modeling/layers/routing_test.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     2030 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/nlp/modeling/layers/self_attention_mask.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)    10735 2022-05-18 02:34:16.000000 tf-models-official-2.9.1/official/nlp/modeling/layers/spectral_normalization.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     3111 2022-05-18 02:34:16.000000 tf-models-official-2.9.1/official/nlp/modeling/layers/spectral_normalization_test.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     6807 2022-05-18 02:34:16.000000 tf-models-official-2.9.1/official/nlp/modeling/layers/talking_heads_attention.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     7289 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/nlp/modeling/layers/talking_heads_attention_test.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)    32516 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/nlp/modeling/layers/text_layers.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)    24245 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/nlp/modeling/layers/text_layers_test.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     6617 2022-05-18 02:34:16.000000 tf-models-official-2.9.1/official/nlp/modeling/layers/tn_expand_condense.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     6720 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/nlp/modeling/layers/tn_expand_condense_test.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)    11015 2022-05-18 02:34:16.000000 tf-models-official-2.9.1/official/nlp/modeling/layers/tn_transformer_expand_condense.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     9160 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/nlp/modeling/layers/tn_transformer_test.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)    18312 2022-05-18 02:34:16.000000 tf-models-official-2.9.1/official/nlp/modeling/layers/transformer.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)    16791 2022-05-18 02:34:16.000000 tf-models-official-2.9.1/official/nlp/modeling/layers/transformer_encoder_block.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)    24495 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/nlp/modeling/layers/transformer_encoder_block_test.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)    13372 2022-05-18 02:34:16.000000 tf-models-official-2.9.1/official/nlp/modeling/layers/transformer_scaffold.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)    20384 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/nlp/modeling/layers/transformer_scaffold_test.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     3718 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/nlp/modeling/layers/transformer_test.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)    22109 2022-05-18 02:34:16.000000 tf-models-official-2.9.1/official/nlp/modeling/layers/transformer_xl.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     9514 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/nlp/modeling/layers/transformer_xl_test.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     2723 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/nlp/modeling/layers/util.py
-drwxr-x---   0 hongkuny (405338) primarygroup (89939)        0 2022-05-19 23:14:06.756169 tf-models-official-2.9.1/official/nlp/modeling/losses/
--rw-r-----   0 hongkuny (405338) primarygroup (89939)      824 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/nlp/modeling/losses/__init__.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     2859 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/nlp/modeling/losses/weighted_sparse_categorical_crossentropy.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     8619 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/nlp/modeling/losses/weighted_sparse_categorical_crossentropy_test.py
-drwxr-x---   0 hongkuny (405338) primarygroup (89939)        0 2022-05-19 23:14:06.756169 tf-models-official-2.9.1/official/nlp/modeling/models/
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     1654 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/nlp/modeling/models/__init__.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     5896 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/nlp/modeling/models/bert_classifier.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     5092 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/nlp/modeling/models/bert_classifier_test.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)    11310 2022-05-18 02:34:16.000000 tf-models-official-2.9.1/official/nlp/modeling/models/bert_pretrainer.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)    10116 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/nlp/modeling/models/bert_pretrainer_test.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     4997 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/nlp/modeling/models/bert_span_labeler.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     5053 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/nlp/modeling/models/bert_span_labeler_test.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     5216 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/nlp/modeling/models/bert_token_classifier.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     5112 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/nlp/modeling/models/bert_token_classifier_test.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     6583 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/nlp/modeling/models/dual_encoder.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     5377 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/nlp/modeling/models/dual_encoder_test.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)    12841 2022-05-18 02:34:16.000000 tf-models-official-2.9.1/official/nlp/modeling/models/electra_pretrainer.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     6804 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/nlp/modeling/models/electra_pretrainer_test.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)    25716 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/nlp/modeling/models/seq2seq_transformer.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     5402 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/nlp/modeling/models/seq2seq_transformer_test.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)    54288 2022-05-18 02:34:16.000000 tf-models-official-2.9.1/official/nlp/modeling/models/t5.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)    24241 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/nlp/modeling/models/t5_test.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)    11779 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/nlp/modeling/models/xlnet.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)    13044 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/nlp/modeling/models/xlnet_test.py
-drwxr-x---   0 hongkuny (405338) primarygroup (89939)        0 2022-05-19 23:14:06.756169 tf-models-official-2.9.1/official/nlp/modeling/networks/
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     1718 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/nlp/modeling/networks/__init__.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     8702 2022-05-18 02:34:16.000000 tf-models-official-2.9.1/official/nlp/modeling/networks/albert_encoder.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     7494 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/nlp/modeling/networks/albert_encoder_test.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)    14506 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/nlp/modeling/networks/bert_dense_encoder_test.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)    23007 2022-05-18 02:34:16.000000 tf-models-official-2.9.1/official/nlp/modeling/networks/bert_encoder.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)    24661 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/nlp/modeling/networks/bert_encoder_test.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     4242 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/nlp/modeling/networks/classification.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     7448 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/nlp/modeling/networks/classification_test.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)    16903 2022-05-18 02:34:16.000000 tf-models-official-2.9.1/official/nlp/modeling/networks/encoder_scaffold.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)    29410 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/nlp/modeling/networks/encoder_scaffold_test.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)    20834 2022-05-18 02:34:16.000000 tf-models-official-2.9.1/official/nlp/modeling/networks/funnel_transformer.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)    14442 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/nlp/modeling/networks/funnel_transformer_test.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     7569 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/nlp/modeling/networks/mobile_bert_encoder.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     7105 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/nlp/modeling/networks/mobile_bert_encoder_test.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)    12841 2022-05-18 02:34:16.000000 tf-models-official-2.9.1/official/nlp/modeling/networks/packed_sequence_embedding.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     5066 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/nlp/modeling/networks/packed_sequence_embedding_test.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)    13033 2022-05-18 02:34:16.000000 tf-models-official-2.9.1/official/nlp/modeling/networks/span_labeling.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)    12330 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/nlp/modeling/networks/span_labeling_test.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)    25837 2022-05-18 02:34:16.000000 tf-models-official-2.9.1/official/nlp/modeling/networks/xlnet_base.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)    14869 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/nlp/modeling/networks/xlnet_base_test.py
-drwxr-x---   0 hongkuny (405338) primarygroup (89939)        0 2022-05-19 23:14:06.760169 tf-models-official-2.9.1/official/nlp/modeling/ops/
--rw-r-----   0 hongkuny (405338) primarygroup (89939)      873 2022-05-18 02:34:16.000000 tf-models-official-2.9.1/official/nlp/modeling/ops/__init__.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)    28925 2022-05-18 02:34:16.000000 tf-models-official-2.9.1/official/nlp/modeling/ops/beam_search.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     3505 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/nlp/modeling/ops/beam_search_test.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)    10047 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/nlp/modeling/ops/decoding_module.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     2573 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/nlp/modeling/ops/decoding_module_test.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)    18023 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/nlp/modeling/ops/sampling_module.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     9596 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/nlp/modeling/ops/segment_extractor.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     5398 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/nlp/modeling/ops/segment_extractor_test.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     9024 2022-05-18 02:34:16.000000 tf-models-official-2.9.1/official/nlp/optimization.py
-drwxr-x---   0 hongkuny (405338) primarygroup (89939)        0 2022-05-19 23:14:06.760169 tf-models-official-2.9.1/official/nlp/serving/
--rw-r-----   0 hongkuny (405338) primarygroup (89939)      610 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/nlp/serving/__init__.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     5618 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/nlp/serving/export_savedmodel.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     6513 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/nlp/serving/export_savedmodel_test.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     2312 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/nlp/serving/export_savedmodel_util.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)    18889 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/nlp/serving/serving_modules.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)    15068 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/nlp/serving/serving_modules_test.py
-drwxr-x---   0 hongkuny (405338) primarygroup (89939)        0 2022-05-19 23:14:06.760169 tf-models-official-2.9.1/official/nlp/tasks/
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     1178 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/nlp/tasks/__init__.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     7634 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/nlp/tasks/dual_encoder.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     4561 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/nlp/tasks/dual_encoder_test.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     9637 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/nlp/tasks/electra_task.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     2282 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/nlp/tasks/electra_task_test.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     7703 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/nlp/tasks/masked_lm.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     2160 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/nlp/tasks/masked_lm_test.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)    19817 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/nlp/tasks/question_answering.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     9939 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/nlp/tasks/question_answering_test.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)    12386 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/nlp/tasks/sentence_prediction.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)    10358 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/nlp/tasks/sentence_prediction_test.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)    10088 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/nlp/tasks/tagging.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     6407 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/nlp/tasks/tagging_test.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)    13381 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/nlp/tasks/translation.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     6871 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/nlp/tasks/translation_test.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     2575 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/nlp/tasks/utils.py
-drwxr-x---   0 hongkuny (405338) primarygroup (89939)        0 2022-05-19 23:14:06.760169 tf-models-official-2.9.1/official/nlp/tools/
--rw-r-----   0 hongkuny (405338) primarygroup (89939)      610 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/nlp/tools/__init__.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     9443 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/nlp/tools/export_tfhub.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)    21271 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/nlp/tools/export_tfhub_lib.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)    46347 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/nlp/tools/export_tfhub_lib_test.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     3724 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/nlp/tools/squad_evaluate_v1_1.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     8625 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/nlp/tools/squad_evaluate_v2_0.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     7865 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/nlp/tools/tf1_bert_checkpoint_converter_lib.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     6676 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/nlp/tools/tf2_albert_encoder_checkpoint_converter.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     5826 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/nlp/tools/tf2_bert_encoder_checkpoint_converter.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)    16591 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/nlp/tools/tokenization.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     5217 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/nlp/tools/tokenization_test.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     3043 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/nlp/train.py
-drwxr-x---   0 hongkuny (405338) primarygroup (89939)        0 2022-05-19 23:14:06.760169 tf-models-official-2.9.1/official/projects/
--rw-r-----   0 hongkuny (405338) primarygroup (89939)      609 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/projects/__init__.py
-drwxr-x---   0 hongkuny (405338) primarygroup (89939)        0 2022-05-19 23:14:06.760169 tf-models-official-2.9.1/official/projects/bigbird/
--rw-r-----   0 hongkuny (405338) primarygroup (89939)      609 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/projects/bigbird/__init__.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     9233 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/projects/bigbird/encoder.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     2340 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/projects/bigbird/encoder_test.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     3774 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/projects/bigbird/experiment_configs.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     9027 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/projects/bigbird/recompute_grad.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     5942 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/projects/bigbird/recomputing_dropout.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     4921 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/projects/bigbird/stateless_dropout.py
-drwxr-x---   0 hongkuny (405338) primarygroup (89939)        0 2022-05-19 23:14:06.764169 tf-models-official-2.9.1/official/projects/deepmac_maskrcnn/
--rw-r-----   0 hongkuny (405338) primarygroup (89939)      609 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/projects/deepmac_maskrcnn/__init__.py
-drwxr-x---   0 hongkuny (405338) primarygroup (89939)        0 2022-05-19 23:14:06.764169 tf-models-official-2.9.1/official/projects/deepmac_maskrcnn/common/
--rw-r-----   0 hongkuny (405338) primarygroup (89939)      609 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/projects/deepmac_maskrcnn/common/__init__.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)      775 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/projects/deepmac_maskrcnn/common/registry_imports.py
-drwxr-x---   0 hongkuny (405338) primarygroup (89939)        0 2022-05-19 23:14:06.764169 tf-models-official-2.9.1/official/projects/deepmac_maskrcnn/configs/
--rw-r-----   0 hongkuny (405338) primarygroup (89939)      609 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/projects/deepmac_maskrcnn/configs/__init__.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     7948 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/projects/deepmac_maskrcnn/configs/deep_mask_head_rcnn.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     1218 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/projects/deepmac_maskrcnn/configs/deep_mask_head_rcnn_config_test.py
-drwxr-x---   0 hongkuny (405338) primarygroup (89939)        0 2022-05-19 23:14:06.764169 tf-models-official-2.9.1/official/projects/deepmac_maskrcnn/modeling/
--rw-r-----   0 hongkuny (405338) primarygroup (89939)      609 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/projects/deepmac_maskrcnn/modeling/__init__.py
-drwxr-x---   0 hongkuny (405338) primarygroup (89939)        0 2022-05-19 23:14:06.764169 tf-models-official-2.9.1/official/projects/deepmac_maskrcnn/modeling/heads/
--rw-r-----   0 hongkuny (405338) primarygroup (89939)      609 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/projects/deepmac_maskrcnn/modeling/heads/__init__.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)    21630 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/projects/deepmac_maskrcnn/modeling/heads/hourglass_network.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)    12058 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/projects/deepmac_maskrcnn/modeling/heads/instance_heads.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     3172 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/projects/deepmac_maskrcnn/modeling/heads/instance_heads_test.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     8566 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/projects/deepmac_maskrcnn/modeling/maskrcnn_model.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     5471 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/projects/deepmac_maskrcnn/modeling/maskrcnn_model_test.py
-drwxr-x---   0 hongkuny (405338) primarygroup (89939)        0 2022-05-19 23:14:06.764169 tf-models-official-2.9.1/official/projects/deepmac_maskrcnn/serving/
--rw-r-----   0 hongkuny (405338) primarygroup (89939)      609 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/projects/deepmac_maskrcnn/serving/__init__.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     5494 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/projects/deepmac_maskrcnn/serving/detection.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     6352 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/projects/deepmac_maskrcnn/serving/detection_test.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     3991 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/projects/deepmac_maskrcnn/serving/export_saved_model.py
-drwxr-x---   0 hongkuny (405338) primarygroup (89939)        0 2022-05-19 23:14:06.764169 tf-models-official-2.9.1/official/projects/deepmac_maskrcnn/tasks/
--rw-r-----   0 hongkuny (405338) primarygroup (89939)      609 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/projects/deepmac_maskrcnn/tasks/__init__.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     8585 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/projects/deepmac_maskrcnn/tasks/deep_mask_head_rcnn.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     2630 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/projects/deepmac_maskrcnn/train.py
-drwxr-x---   0 hongkuny (405338) primarygroup (89939)        0 2022-05-19 23:14:06.764169 tf-models-official-2.9.1/official/projects/mobilebert/
--rw-r-----   0 hongkuny (405338) primarygroup (89939)      609 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/projects/mobilebert/__init__.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)    24889 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/projects/mobilebert/distillation.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     7239 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/projects/mobilebert/distillation_test.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     3689 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/projects/mobilebert/export_tfhub.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     7470 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/projects/mobilebert/model_utils.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     5486 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/projects/mobilebert/run_distillation.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)    10709 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/projects/mobilebert/tf2_model_checkpoint_converter.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     1036 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/projects/mobilebert/utils.py
-drwxr-x---   0 hongkuny (405338) primarygroup (89939)        0 2022-05-19 23:14:06.764169 tf-models-official-2.9.1/official/projects/movinet/
--rw-r-----   0 hongkuny (405338) primarygroup (89939)      609 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/projects/movinet/__init__.py
-drwxr-x---   0 hongkuny (405338) primarygroup (89939)        0 2022-05-19 23:14:06.764169 tf-models-official-2.9.1/official/projects/movinet/configs/
--rw-r-----   0 hongkuny (405338) primarygroup (89939)      609 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/projects/movinet/configs/__init__.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     4298 2022-05-18 02:34:16.000000 tf-models-official-2.9.1/official/projects/movinet/configs/movinet.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     1596 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/projects/movinet/configs/movinet_test.py
-drwxr-x---   0 hongkuny (405338) primarygroup (89939)        0 2022-05-19 23:14:06.764169 tf-models-official-2.9.1/official/projects/movinet/modeling/
--rw-r-----   0 hongkuny (405338) primarygroup (89939)      609 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/projects/movinet/modeling/__init__.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)    29032 2022-05-18 02:34:16.000000 tf-models-official-2.9.1/official/projects/movinet/modeling/movinet.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)    60645 2022-05-18 02:34:16.000000 tf-models-official-2.9.1/official/projects/movinet/modeling/movinet_layers.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)    14957 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/projects/movinet/modeling/movinet_layers_test.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     9800 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/projects/movinet/modeling/movinet_model.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     8838 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/projects/movinet/modeling/movinet_model_test.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     7863 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/projects/movinet/modeling/movinet_test.py
-drwxr-x---   0 hongkuny (405338) primarygroup (89939)        0 2022-05-19 23:14:06.764169 tf-models-official-2.9.1/official/projects/movinet/tools/
--rw-r-----   0 hongkuny (405338) primarygroup (89939)      609 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/projects/movinet/tools/__init__.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     3809 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/projects/movinet/tools/convert_3d_2plus1d.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     1997 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/projects/movinet/tools/convert_3d_2plus1d_test.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)    10999 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/projects/movinet/tools/export_saved_model.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     4451 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/projects/movinet/tools/export_saved_model_test.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)    11994 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/projects/movinet/tools/quantize_movinet.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     3320 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/projects/movinet/train.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     3119 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/projects/movinet/train_test.py
-drwxr-x---   0 hongkuny (405338) primarygroup (89939)        0 2022-05-19 23:14:06.768169 tf-models-official-2.9.1/official/projects/nhnet/
--rw-r-----   0 hongkuny (405338) primarygroup (89939)      609 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/projects/nhnet/__init__.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     3202 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/projects/nhnet/configs.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     3116 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/projects/nhnet/configs_test.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)    15312 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/projects/nhnet/decoder.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     6024 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/projects/nhnet/decoder_test.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     6091 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/projects/nhnet/evaluation.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     9053 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/projects/nhnet/input_pipeline.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)    23056 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/projects/nhnet/models.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)    11786 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/projects/nhnet/models_test.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     2809 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/projects/nhnet/optimizer.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     3735 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/projects/nhnet/raw_data_process.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     9238 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/projects/nhnet/raw_data_processor.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     8723 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/projects/nhnet/trainer.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     3289 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/projects/nhnet/trainer_test.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     3294 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/projects/nhnet/utils.py
-drwxr-x---   0 hongkuny (405338) primarygroup (89939)        0 2022-05-19 23:14:06.768169 tf-models-official-2.9.1/official/projects/roformer/
--rw-r-----   0 hongkuny (405338) primarygroup (89939)      610 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/projects/roformer/__init__.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     2002 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/projects/roformer/roformer.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     4462 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/projects/roformer/roformer_attention.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     4133 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/projects/roformer/roformer_attention_test.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)    11208 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/projects/roformer/roformer_encoder.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)    13399 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/projects/roformer/roformer_encoder_block.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)    13069 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/projects/roformer/roformer_encoder_block_test.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     9791 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/projects/roformer/roformer_encoder_test.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     4797 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/projects/roformer/roformer_experiments.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     2566 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/projects/roformer/train.py
-drwxr-x---   0 hongkuny (405338) primarygroup (89939)        0 2022-05-19 23:14:06.768169 tf-models-official-2.9.1/official/projects/teams/
--rw-r-----   0 hongkuny (405338) primarygroup (89939)      609 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/projects/teams/__init__.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     4010 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/projects/teams/teams.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     4424 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/projects/teams/teams_experiments.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     1272 2022-05-18 02:34:16.000000 tf-models-official-2.9.1/official/projects/teams/teams_experiments_test.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)    18516 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/projects/teams/teams_pretrainer.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     7737 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/projects/teams/teams_pretrainer_test.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)    10170 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/projects/teams/teams_task.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     2184 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/projects/teams/teams_task_test.py
-drwxr-x---   0 hongkuny (405338) primarygroup (89939)        0 2022-05-19 23:14:06.768169 tf-models-official-2.9.1/official/projects/triviaqa/
--rw-r-----   0 hongkuny (405338) primarygroup (89939)      609 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/projects/triviaqa/__init__.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)    16320 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/projects/triviaqa/dataset.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     2497 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/projects/triviaqa/download_and_prepare.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     1550 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/projects/triviaqa/evaluate.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     5293 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/projects/triviaqa/evaluation.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)    21718 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/projects/triviaqa/inputs.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     4629 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/projects/triviaqa/modeling.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     7087 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/projects/triviaqa/predict.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     2735 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/projects/triviaqa/prediction.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)    18797 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/projects/triviaqa/preprocess.py
--rwxr-x---   0 hongkuny (405338) primarygroup (89939)    10818 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/projects/triviaqa/sentencepiece_pb2.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)    14287 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/projects/triviaqa/train.py
-drwxr-x---   0 hongkuny (405338) primarygroup (89939)        0 2022-05-19 23:14:06.768169 tf-models-official-2.9.1/official/projects/yt8m/
--rw-r-----   0 hongkuny (405338) primarygroup (89939)      609 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/projects/yt8m/__init__.py
-drwxr-x---   0 hongkuny (405338) primarygroup (89939)        0 2022-05-19 23:14:06.768169 tf-models-official-2.9.1/official/projects/yt8m/configs/
--rw-r-----   0 hongkuny (405338) primarygroup (89939)      692 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/projects/yt8m/configs/__init__.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     6378 2022-05-18 02:34:16.000000 tf-models-official-2.9.1/official/projects/yt8m/configs/yt8m.py
-drwxr-x---   0 hongkuny (405338) primarygroup (89939)        0 2022-05-19 23:14:06.772168 tf-models-official-2.9.1/official/projects/yt8m/modeling/
--rw-r-----   0 hongkuny (405338) primarygroup (89939)      609 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/projects/yt8m/modeling/__init__.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     4632 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/projects/yt8m/modeling/yt8m_agg_models.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     7040 2022-05-18 02:34:16.000000 tf-models-official-2.9.1/official/projects/yt8m/modeling/yt8m_model.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     2150 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/projects/yt8m/modeling/yt8m_model_test.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     8408 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/projects/yt8m/modeling/yt8m_model_utils.py
-drwxr-x---   0 hongkuny (405338) primarygroup (89939)        0 2022-05-19 23:14:06.772168 tf-models-official-2.9.1/official/projects/yt8m/tasks/
--rw-r-----   0 hongkuny (405338) primarygroup (89939)      692 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/projects/yt8m/tasks/__init__.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)    10969 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/projects/yt8m/tasks/yt8m_task.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)      987 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/projects/yt8m/train.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     3394 2022-05-18 02:34:16.000000 tf-models-official-2.9.1/official/projects/yt8m/train_test.py
-drwxr-x---   0 hongkuny (405338) primarygroup (89939)        0 2022-05-19 23:14:06.772168 tf-models-official-2.9.1/official/recommendation/
--rw-r-----   0 hongkuny (405338) primarygroup (89939)      609 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/recommendation/__init__.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     2877 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/recommendation/constants.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     4008 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/recommendation/create_ncf_data.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)    37218 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/recommendation/data_pipeline.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)    10308 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/recommendation/data_preprocessing.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)    12821 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/recommendation/data_test.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     9734 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/recommendation/movielens.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)    12278 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/recommendation/ncf_common.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     6964 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/recommendation/ncf_input_pipeline.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)    19840 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/recommendation/ncf_keras_main.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     4134 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/recommendation/ncf_test.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)    16940 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/recommendation/neumf_model.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     1917 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/recommendation/popen_helper.py
-drwxr-x---   0 hongkuny (405338) primarygroup (89939)        0 2022-05-19 23:14:06.772168 tf-models-official-2.9.1/official/recommendation/ranking/
--rw-r-----   0 hongkuny (405338) primarygroup (89939)      609 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/recommendation/ranking/__init__.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     3988 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/recommendation/ranking/common.py
-drwxr-x---   0 hongkuny (405338) primarygroup (89939)        0 2022-05-19 23:14:06.772168 tf-models-official-2.9.1/official/recommendation/ranking/configs/
--rw-r-----   0 hongkuny (405338) primarygroup (89939)      609 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/recommendation/ranking/configs/__init__.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)    10418 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/recommendation/ranking/configs/config.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     1464 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/recommendation/ranking/configs/config_test.py
-drwxr-x---   0 hongkuny (405338) primarygroup (89939)        0 2022-05-19 23:14:06.772168 tf-models-official-2.9.1/official/recommendation/ranking/data/
--rw-r-----   0 hongkuny (405338) primarygroup (89939)      609 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/recommendation/ranking/data/__init__.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     7319 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/recommendation/ranking/data/data_pipeline.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     2335 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/recommendation/ranking/data/data_pipeline_test.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     7689 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/recommendation/ranking/task.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     2182 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/recommendation/ranking/task_test.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     6613 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/recommendation/ranking/train.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     4823 2022-05-18 02:34:16.000000 tf-models-official-2.9.1/official/recommendation/ranking/train_test.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     3076 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/recommendation/stat_utils.py
-drwxr-x---   0 hongkuny (405338) primarygroup (89939)        0 2022-05-19 23:14:06.772168 tf-models-official-2.9.1/official/utils/
--rw-r-----   0 hongkuny (405338) primarygroup (89939)      609 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/utils/__init__.py
-drwxr-x---   0 hongkuny (405338) primarygroup (89939)        0 2022-05-19 23:14:06.772168 tf-models-official-2.9.1/official/utils/docs/
--rw-r-----   0 hongkuny (405338) primarygroup (89939)      609 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/utils/docs/__init__.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     3622 2022-05-18 02:34:16.000000 tf-models-official-2.9.1/official/utils/docs/build_all_api_docs.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     1569 2022-05-18 02:34:16.000000 tf-models-official-2.9.1/official/utils/docs/build_all_api_docs_test.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     1928 2022-05-18 02:34:16.000000 tf-models-official-2.9.1/official/utils/docs/build_api_docs_lib.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     3617 2022-05-18 02:34:16.000000 tf-models-official-2.9.1/official/utils/docs/build_nlp_api_docs.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     3576 2022-05-18 02:34:16.000000 tf-models-official-2.9.1/official/utils/docs/build_vision_api_docs.py
-drwxr-x---   0 hongkuny (405338) primarygroup (89939)        0 2022-05-19 23:14:06.772168 tf-models-official-2.9.1/official/utils/flags/
--rw-r-----   0 hongkuny (405338) primarygroup (89939)      609 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/utils/flags/__init__.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     6395 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/utils/flags/_base.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     4082 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/utils/flags/_benchmark.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     1618 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/utils/flags/_conventions.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     2826 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/utils/flags/_device.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     1694 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/utils/flags/_distribution.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     1541 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/utils/flags/_misc.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)    11566 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/utils/flags/_performance.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     4427 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/utils/flags/core.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     5302 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/utils/flags/flags_test.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     4607 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/utils/hyperparams_flags.py
-drwxr-x---   0 hongkuny (405338) primarygroup (89939)        0 2022-05-19 23:14:06.776168 tf-models-official-2.9.1/official/utils/misc/
--rw-r-----   0 hongkuny (405338) primarygroup (89939)      609 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/utils/misc/__init__.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     7783 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/utils/misc/keras_utils.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     3360 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/utils/misc/model_helpers.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     4549 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/utils/misc/model_helpers_test.py
-drwxr-x---   0 hongkuny (405338) primarygroup (89939)        0 2022-05-19 23:14:06.776168 tf-models-official-2.9.1/official/utils/testing/
--rw-r-----   0 hongkuny (405338) primarygroup (89939)      609 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/utils/testing/__init__.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     2220 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/utils/testing/integration.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     3227 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/utils/testing/mock_task.py
-drwxr-x---   0 hongkuny (405338) primarygroup (89939)        0 2022-05-19 23:14:06.776168 tf-models-official-2.9.1/official/vision/
--rw-r-----   0 hongkuny (405338) primarygroup (89939)      763 2022-05-18 02:34:16.000000 tf-models-official-2.9.1/official/vision/__init__.py
-drwxr-x---   0 hongkuny (405338) primarygroup (89939)        0 2022-05-19 23:14:06.776168 tf-models-official-2.9.1/official/vision/beta/
--rw-r-----   0 hongkuny (405338) primarygroup (89939)      609 2022-05-19 23:03:19.000000 tf-models-official-2.9.1/official/vision/beta/__init__.py
-drwxr-x---   0 hongkuny (405338) primarygroup (89939)        0 2022-05-19 23:14:06.776168 tf-models-official-2.9.1/official/vision/beta/projects/
--rw-r-----   0 hongkuny (405338) primarygroup (89939)      609 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/vision/beta/projects/__init__.py
-drwxr-x---   0 hongkuny (405338) primarygroup (89939)        0 2022-05-19 23:14:06.776168 tf-models-official-2.9.1/official/vision/beta/projects/panoptic_maskrcnn/
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     1217 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/vision/beta/projects/panoptic_maskrcnn/__init__.py
-drwxr-x---   0 hongkuny (405338) primarygroup (89939)        0 2022-05-19 23:14:06.776168 tf-models-official-2.9.1/official/vision/beta/projects/panoptic_maskrcnn/configs/
--rw-r-----   0 hongkuny (405338) primarygroup (89939)      609 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/vision/beta/projects/panoptic_maskrcnn/configs/__init__.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)    10246 2022-05-18 02:34:16.000000 tf-models-official-2.9.1/official/vision/beta/projects/panoptic_maskrcnn/configs/panoptic_maskrcnn.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     1667 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/vision/beta/projects/panoptic_maskrcnn/configs/panoptic_maskrcnn_test.py
-drwxr-x---   0 hongkuny (405338) primarygroup (89939)        0 2022-05-19 23:14:06.776168 tf-models-official-2.9.1/official/vision/beta/projects/panoptic_maskrcnn/tasks/
--rw-r-----   0 hongkuny (405338) primarygroup (89939)      609 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/vision/beta/projects/panoptic_maskrcnn/tasks/__init__.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)    18150 2022-05-18 02:34:16.000000 tf-models-official-2.9.1/official/vision/beta/projects/panoptic_maskrcnn/tasks/panoptic_maskrcnn.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     2735 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/vision/beta/projects/panoptic_maskrcnn/tasks/panoptic_maskrcnn_test.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     1075 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/vision/beta/projects/panoptic_maskrcnn/train.py
-drwxr-x---   0 hongkuny (405338) primarygroup (89939)        0 2022-05-19 23:14:06.776168 tf-models-official-2.9.1/official/vision/beta/projects/yolo/
--rw-r-----   0 hongkuny (405338) primarygroup (89939)      609 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/vision/beta/projects/yolo/__init__.py
-drwxr-x---   0 hongkuny (405338) primarygroup (89939)        0 2022-05-19 23:14:06.776168 tf-models-official-2.9.1/official/vision/beta/projects/yolo/common/
--rw-r-----   0 hongkuny (405338) primarygroup (89939)      609 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/vision/beta/projects/yolo/common/__init__.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     1567 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/vision/beta/projects/yolo/common/registry_imports.py
-drwxr-x---   0 hongkuny (405338) primarygroup (89939)        0 2022-05-19 23:14:06.776168 tf-models-official-2.9.1/official/vision/beta/projects/yolo/configs/
--rw-r-----   0 hongkuny (405338) primarygroup (89939)      609 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/vision/beta/projects/yolo/configs/__init__.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     1143 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/vision/beta/projects/yolo/configs/backbones.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     2580 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/vision/beta/projects/yolo/configs/darknet_classification.py
--rwxr-x---   0 hongkuny (405338) primarygroup (89939)     1640 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/vision/beta/projects/yolo/configs/decoders.py
--rwxr-x---   0 hongkuny (405338) primarygroup (89939)    17638 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/vision/beta/projects/yolo/configs/yolo.py
-drwxr-x---   0 hongkuny (405338) primarygroup (89939)        0 2022-05-19 23:14:06.776168 tf-models-official-2.9.1/official/vision/beta/projects/yolo/dataloaders/
--rw-r-----   0 hongkuny (405338) primarygroup (89939)      610 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/vision/beta/projects/yolo/dataloaders/__init__.py
--rwxr-x---   0 hongkuny (405338) primarygroup (89939)     3279 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/vision/beta/projects/yolo/dataloaders/classification_input.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     4810 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/vision/beta/projects/yolo/dataloaders/tf_example_decoder.py
--rwxr-x---   0 hongkuny (405338) primarygroup (89939)    14697 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/vision/beta/projects/yolo/dataloaders/yolo_input.py
-drwxr-x---   0 hongkuny (405338) primarygroup (89939)        0 2022-05-19 23:14:06.776168 tf-models-official-2.9.1/official/vision/beta/projects/yolo/losses/
--rw-r-----   0 hongkuny (405338) primarygroup (89939)      609 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/vision/beta/projects/yolo/losses/__init__.py
--rwxr-x---   0 hongkuny (405338) primarygroup (89939)    31760 2022-05-18 02:34:16.000000 tf-models-official-2.9.1/official/vision/beta/projects/yolo/losses/yolo_loss.py
--rwxr-x---   0 hongkuny (405338) primarygroup (89939)     3010 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/vision/beta/projects/yolo/losses/yolo_loss_test.py
-drwxr-x---   0 hongkuny (405338) primarygroup (89939)        0 2022-05-19 23:14:06.776168 tf-models-official-2.9.1/official/vision/beta/projects/yolo/ops/
--rw-r-----   0 hongkuny (405338) primarygroup (89939)      610 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/vision/beta/projects/yolo/ops/__init__.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)    19345 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/vision/beta/projects/yolo/ops/anchor.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)    11205 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/vision/beta/projects/yolo/ops/box_ops.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     2017 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/vision/beta/projects/yolo/ops/box_ops_test.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)    11630 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/vision/beta/projects/yolo/ops/kmeans_anchors.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     1457 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/vision/beta/projects/yolo/ops/kmeans_anchors_test.py
--rwxr-x---   0 hongkuny (405338) primarygroup (89939)    23506 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/vision/beta/projects/yolo/ops/loss_utils.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     1676 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/vision/beta/projects/yolo/ops/math_ops.py
--rwxr-x---   0 hongkuny (405338) primarygroup (89939)    16395 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/vision/beta/projects/yolo/ops/mosaic.py
--rwxr-x---   0 hongkuny (405338) primarygroup (89939)    36261 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/vision/beta/projects/yolo/ops/preprocessing_ops.py
--rwxr-x---   0 hongkuny (405338) primarygroup (89939)     5480 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/vision/beta/projects/yolo/ops/preprocessing_ops_test.py
-drwxr-x---   0 hongkuny (405338) primarygroup (89939)        0 2022-05-19 23:14:06.776168 tf-models-official-2.9.1/official/vision/beta/projects/yolo/optimization/
--rwxr-x---   0 hongkuny (405338) primarygroup (89939)     1135 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/vision/beta/projects/yolo/optimization/__init__.py
-drwxr-x---   0 hongkuny (405338) primarygroup (89939)        0 2022-05-19 23:14:06.780168 tf-models-official-2.9.1/official/vision/beta/projects/yolo/optimization/configs/
--rwxr-x---   0 hongkuny (405338) primarygroup (89939)      609 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/vision/beta/projects/yolo/optimization/configs/__init__.py
--rwxr-x---   0 hongkuny (405338) primarygroup (89939)     2010 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/vision/beta/projects/yolo/optimization/configs/optimization_config.py
--rwxr-x---   0 hongkuny (405338) primarygroup (89939)     2283 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/vision/beta/projects/yolo/optimization/configs/optimizer_config.py
--rwxr-x---   0 hongkuny (405338) primarygroup (89939)     3401 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/vision/beta/projects/yolo/optimization/optimizer_factory.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)    11218 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/vision/beta/projects/yolo/optimization/sgd_torch.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)      998 2022-05-18 02:34:16.000000 tf-models-official-2.9.1/official/vision/beta/projects/yolo/train.py
-drwxr-x---   0 hongkuny (405338) primarygroup (89939)        0 2022-05-19 23:14:06.780168 tf-models-official-2.9.1/official/vision/configs/
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     1045 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/vision/configs/__init__.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     3835 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/vision/configs/backbones.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     3650 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/vision/configs/backbones_3d.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     4342 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/vision/configs/common.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     1916 2022-05-18 02:34:16.000000 tf-models-official-2.9.1/official/vision/configs/decoders.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)    14934 2022-05-18 02:34:16.000000 tf-models-official-2.9.1/official/vision/configs/image_classification.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     1753 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/vision/configs/image_classification_test.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)    18750 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/vision/configs/maskrcnn.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     1722 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/vision/configs/maskrcnn_test.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)    15680 2022-05-18 02:34:16.000000 tf-models-official-2.9.1/official/vision/configs/retinanet.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     1688 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/vision/configs/retinanet_test.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)    27641 2022-05-18 02:34:16.000000 tf-models-official-2.9.1/official/vision/configs/semantic_segmentation.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     1721 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/vision/configs/semantic_segmentation_test.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)    13867 2022-05-18 02:34:16.000000 tf-models-official-2.9.1/official/vision/configs/video_classification.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     1700 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/vision/configs/video_classification_test.py
-drwxr-x---   0 hongkuny (405338) primarygroup (89939)        0 2022-05-19 23:14:06.780168 tf-models-official-2.9.1/official/vision/data/
--rw-r-----   0 hongkuny (405338) primarygroup (89939)      609 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/vision/data/__init__.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)    22181 2022-05-18 02:34:16.000000 tf-models-official-2.9.1/official/vision/data/create_coco_tf_record.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     6051 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/vision/data/process_coco_few_shot_json_files.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     5951 2022-05-18 02:34:16.000000 tf-models-official-2.9.1/official/vision/data/tfrecord_lib.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     2770 2022-05-18 02:34:16.000000 tf-models-official-2.9.1/official/vision/data/tfrecord_lib_test.py
-drwxr-x---   0 hongkuny (405338) primarygroup (89939)        0 2022-05-19 23:14:06.780168 tf-models-official-2.9.1/official/vision/dataloaders/
--rw-r-----   0 hongkuny (405338) primarygroup (89939)      609 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/vision/dataloaders/__init__.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)    10713 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/vision/dataloaders/classification_input.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     1032 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/vision/dataloaders/decoder.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     7720 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/vision/dataloaders/input_reader.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     1623 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/vision/dataloaders/input_reader_factory.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)    14269 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/vision/dataloaders/maskrcnn_input.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     2315 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/vision/dataloaders/parser.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)    13706 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/vision/dataloaders/retinanet_input.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     8610 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/vision/dataloaders/segmentation_input.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     7288 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/vision/dataloaders/tf_example_decoder.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)    11548 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/vision/dataloaders/tf_example_decoder_test.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     2588 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/vision/dataloaders/tf_example_label_map_decoder.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     7746 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/vision/dataloaders/tf_example_label_map_decoder_test.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     1242 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/vision/dataloaders/tfds_classification_decoders.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     2272 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/vision/dataloaders/tfds_detection_decoders.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     2568 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/vision/dataloaders/tfds_factory.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     4010 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/vision/dataloaders/tfds_factory_test.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     2418 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/vision/dataloaders/tfds_segmentation_decoders.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)    11261 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/vision/dataloaders/tfexample_utils.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     2543 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/vision/dataloaders/utils.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     2557 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/vision/dataloaders/utils_test.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)    15203 2022-05-18 02:34:16.000000 tf-models-official-2.9.1/official/vision/dataloaders/video_input.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     6657 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/vision/dataloaders/video_input_test.py
-drwxr-x---   0 hongkuny (405338) primarygroup (89939)        0 2022-05-19 23:14:06.784168 tf-models-official-2.9.1/official/vision/evaluation/
--rw-r-----   0 hongkuny (405338) primarygroup (89939)      609 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/vision/evaluation/__init__.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)    13722 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/vision/evaluation/coco_evaluator.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)    16492 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/vision/evaluation/coco_utils.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     1710 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/vision/evaluation/coco_utils_test.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     4594 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/vision/evaluation/iou.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     3949 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/vision/evaluation/iou_test.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)    12510 2022-05-18 02:34:16.000000 tf-models-official-2.9.1/official/vision/evaluation/panoptic_quality.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     7500 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/vision/evaluation/panoptic_quality_evaluator.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     3323 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/vision/evaluation/panoptic_quality_evaluator_test.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)    11082 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/vision/evaluation/panoptic_quality_test.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     9909 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/vision/evaluation/segmentation_metrics.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     3014 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/vision/evaluation/segmentation_metrics_test.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     6598 2022-05-18 02:34:16.000000 tf-models-official-2.9.1/official/vision/evaluation/wod_detection_evaluator.py
-drwxr-x---   0 hongkuny (405338) primarygroup (89939)        0 2022-05-19 23:14:06.784168 tf-models-official-2.9.1/official/vision/losses/
--rw-r-----   0 hongkuny (405338) primarygroup (89939)      609 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/vision/losses/__init__.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     3229 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/vision/losses/focal_loss.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     1569 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/vision/losses/loss_utils.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)    13380 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/vision/losses/maskrcnn_losses.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     8097 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/vision/losses/retinanet_losses.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     5259 2022-05-18 02:34:16.000000 tf-models-official-2.9.1/official/vision/losses/segmentation_losses.py
-drwxr-x---   0 hongkuny (405338) primarygroup (89939)        0 2022-05-19 23:14:06.784168 tf-models-official-2.9.1/official/vision/modeling/
--rw-r-----   0 hongkuny (405338) primarygroup (89939)      825 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/vision/modeling/__init__.py
-drwxr-x---   0 hongkuny (405338) primarygroup (89939)        0 2022-05-19 23:14:06.784168 tf-models-official-2.9.1/official/vision/modeling/backbones/
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     1260 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/vision/modeling/backbones/__init__.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)    12005 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/vision/modeling/backbones/efficientnet.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     3752 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/vision/modeling/backbones/efficientnet_test.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     3494 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/vision/modeling/backbones/factory.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     8383 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/vision/modeling/backbones/factory_test.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)    24886 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/vision/modeling/backbones/mobiledet.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     3794 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/vision/modeling/backbones/mobiledet_test.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)    41069 2022-05-18 02:34:16.000000 tf-models-official-2.9.1/official/vision/modeling/backbones/mobilenet.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)    10596 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/vision/modeling/backbones/mobilenet_test.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)    15932 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/vision/modeling/backbones/resnet.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)    18573 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/vision/modeling/backbones/resnet_3d.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     3789 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/vision/modeling/backbones/resnet_3d_test.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)    14077 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/vision/modeling/backbones/resnet_deeplab.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     5009 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/vision/modeling/backbones/resnet_deeplab_test.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     5503 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/vision/modeling/backbones/resnet_test.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     8840 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/vision/modeling/backbones/revnet.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     3215 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/vision/modeling/backbones/revnet_test.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)    20858 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/vision/modeling/backbones/spinenet.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)    20433 2022-05-18 02:34:16.000000 tf-models-official-2.9.1/official/vision/modeling/backbones/spinenet_mobile.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     3948 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/vision/modeling/backbones/spinenet_mobile_test.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     4308 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/vision/modeling/backbones/spinenet_test.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     4607 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/vision/modeling/classification_model.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     6003 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/vision/modeling/classification_model_test.py
-drwxr-x---   0 hongkuny (405338) primarygroup (89939)        0 2022-05-19 23:14:06.788168 tf-models-official-2.9.1/official/vision/modeling/decoders/
--rw-r-----   0 hongkuny (405338) primarygroup (89939)      815 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/vision/modeling/decoders/__init__.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     8600 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/vision/modeling/decoders/aspp.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     3001 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/vision/modeling/decoders/aspp_test.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     4387 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/vision/modeling/decoders/factory.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     5621 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/vision/modeling/decoders/factory_test.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     9233 2022-05-18 02:34:16.000000 tf-models-official-2.9.1/official/vision/modeling/decoders/fpn.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     3913 2022-05-18 02:34:16.000000 tf-models-official-2.9.1/official/vision/modeling/decoders/fpn_test.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)    14437 2022-05-18 02:34:16.000000 tf-models-official-2.9.1/official/vision/modeling/decoders/nasfpn.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     1887 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/vision/modeling/decoders/nasfpn_test.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)    16833 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/vision/modeling/factory.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     3530 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/vision/modeling/factory_3d.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     4960 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/vision/modeling/factory_test.py
-drwxr-x---   0 hongkuny (405338) primarygroup (89939)        0 2022-05-19 23:14:06.788168 tf-models-official-2.9.1/official/vision/modeling/heads/
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     1014 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/vision/modeling/heads/__init__.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)    20824 2022-05-18 02:34:16.000000 tf-models-official-2.9.1/official/vision/modeling/heads/dense_prediction_heads.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     4799 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/vision/modeling/heads/dense_prediction_heads_test.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)    18091 2022-05-18 02:34:16.000000 tf-models-official-2.9.1/official/vision/modeling/heads/instance_heads.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     4197 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/vision/modeling/heads/instance_heads_test.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)    18344 2022-05-18 02:34:16.000000 tf-models-official-2.9.1/official/vision/modeling/heads/segmentation_heads.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     3620 2022-05-18 02:34:16.000000 tf-models-official-2.9.1/official/vision/modeling/heads/segmentation_heads_test.py
-drwxr-x---   0 hongkuny (405338) primarygroup (89939)        0 2022-05-19 23:14:06.788168 tf-models-official-2.9.1/official/vision/modeling/layers/
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     2597 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/vision/modeling/layers/__init__.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     3401 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/vision/modeling/layers/box_sampler.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     8279 2022-05-18 02:34:16.000000 tf-models-official-2.9.1/official/vision/modeling/layers/deeplab.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     1935 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/vision/modeling/layers/deeplab_test.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)    45278 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/vision/modeling/layers/detection_generator.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)    10473 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/vision/modeling/layers/detection_generator_test.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     7914 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/vision/modeling/layers/mask_sampler.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)    57663 2022-05-18 02:34:16.000000 tf-models-official-2.9.1/official/vision/modeling/layers/nn_blocks.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)    10353 2022-05-18 02:34:16.000000 tf-models-official-2.9.1/official/vision/modeling/layers/nn_blocks_3d.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     2028 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/vision/modeling/layers/nn_blocks_3d_test.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)    12575 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/vision/modeling/layers/nn_blocks_test.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)    47761 2022-05-18 02:34:16.000000 tf-models-official-2.9.1/official/vision/modeling/layers/nn_layers.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)    12711 2022-05-18 02:34:16.000000 tf-models-official-2.9.1/official/vision/modeling/layers/nn_layers_test.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     2533 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/vision/modeling/layers/roi_aligner.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     1275 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/vision/modeling/layers/roi_aligner_test.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)    14408 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/vision/modeling/layers/roi_generator.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     8270 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/vision/modeling/layers/roi_sampler.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)    17359 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/vision/modeling/maskrcnn_model.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)    14252 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/vision/modeling/maskrcnn_model_test.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     8635 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/vision/modeling/retinanet_model.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)    10976 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/vision/modeling/retinanet_model_test.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     3353 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/vision/modeling/segmentation_model.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     2807 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/vision/modeling/segmentation_model_test.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     4703 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/vision/modeling/video_classification_model.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     3261 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/vision/modeling/video_classification_model_test.py
-drwxr-x---   0 hongkuny (405338) primarygroup (89939)        0 2022-05-19 23:14:06.792168 tf-models-official-2.9.1/official/vision/ops/
--rw-r-----   0 hongkuny (405338) primarygroup (89939)      609 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/vision/ops/__init__.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)    16891 2022-05-18 02:34:16.000000 tf-models-official-2.9.1/official/vision/ops/anchor.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     7233 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/vision/ops/anchor_generator.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     5286 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/vision/ops/anchor_generator_test.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     7623 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/vision/ops/anchor_test.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)    86454 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/vision/ops/augment.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)    15890 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/vision/ops/augment_test.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     8163 2022-05-18 02:34:16.000000 tf-models-official-2.9.1/official/vision/ops/box_matcher.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     2428 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/vision/ops/box_matcher_test.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)    28961 2022-05-18 02:34:16.000000 tf-models-official-2.9.1/official/vision/ops/box_ops.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     5841 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/vision/ops/iou_similarity.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     1898 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/vision/ops/iou_similarity_test.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     6806 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/vision/ops/mask_ops.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     1677 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/vision/ops/mask_ops_test.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     8099 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/vision/ops/nms.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)    35530 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/vision/ops/preprocess_ops.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)    13283 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/vision/ops/preprocess_ops_3d.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     6822 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/vision/ops/preprocess_ops_3d_test.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     9792 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/vision/ops/preprocess_ops_test.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)    16062 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/vision/ops/sampling_ops.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)    23505 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/vision/ops/spatial_transform_ops.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     3955 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/vision/ops/target_gather.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     2551 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/vision/ops/target_gather_test.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)      843 2022-05-18 02:34:16.000000 tf-models-official-2.9.1/official/vision/registry_imports.py
-drwxr-x---   0 hongkuny (405338) primarygroup (89939)        0 2022-05-19 23:14:06.792168 tf-models-official-2.9.1/official/vision/serving/
--rw-r-----   0 hongkuny (405338) primarygroup (89939)      702 2022-05-19 22:55:50.000000 tf-models-official-2.9.1/official/vision/serving/__init__.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     8225 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/vision/serving/detection.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     5867 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/vision/serving/detection_test.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     7180 2022-05-18 02:34:16.000000 tf-models-official-2.9.1/official/vision/serving/export_base.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     2731 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/vision/serving/export_base_v2.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     2870 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/vision/serving/export_base_v2_test.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     3539 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/vision/serving/export_module_factory.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     4595 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/vision/serving/export_module_factory_test.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     4039 2022-05-18 02:34:16.000000 tf-models-official-2.9.1/official/vision/serving/export_saved_model.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     6653 2022-05-18 02:34:16.000000 tf-models-official-2.9.1/official/vision/serving/export_saved_model_lib.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     2399 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/vision/serving/export_saved_model_lib_test.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     3358 2022-05-18 02:34:16.000000 tf-models-official-2.9.1/official/vision/serving/export_saved_model_lib_v2.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     3737 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/vision/serving/export_tfhub.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     3979 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/vision/serving/export_tflite.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     4819 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/vision/serving/export_tflite_lib.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     6283 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/vision/serving/export_tflite_lib_test.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     4607 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/vision/serving/export_utils.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     2864 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/vision/serving/image_classification.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     4612 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/vision/serving/image_classification_test.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     3065 2022-05-18 02:34:16.000000 tf-models-official-2.9.1/official/vision/serving/semantic_segmentation.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     4241 2022-05-18 02:34:16.000000 tf-models-official-2.9.1/official/vision/serving/semantic_segmentation_test.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     6979 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/vision/serving/video_classification.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     4222 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/vision/serving/video_classification_test.py
-drwxr-x---   0 hongkuny (405338) primarygroup (89939)        0 2022-05-19 23:14:06.792168 tf-models-official-2.9.1/official/vision/tasks/
--rw-r-----   0 hongkuny (405338) primarygroup (89939)      895 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/vision/tasks/__init__.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)    11888 2022-05-18 02:34:16.000000 tf-models-official-2.9.1/official/vision/tasks/image_classification.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)    18417 2022-05-18 02:34:16.000000 tf-models-official-2.9.1/official/vision/tasks/maskrcnn.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)    16001 2022-05-18 02:34:16.000000 tf-models-official-2.9.1/official/vision/tasks/retinanet.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)    12853 2022-05-18 02:34:16.000000 tf-models-official-2.9.1/official/vision/tasks/semantic_segmentation.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)    13486 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/vision/tasks/video_classification.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     2598 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/vision/train.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     5725 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/vision/train_spatial_partitioning.py
-drwxr-x---   0 hongkuny (405338) primarygroup (89939)        0 2022-05-19 23:14:06.792168 tf-models-official-2.9.1/official/vision/utils/
--rw-r-----   0 hongkuny (405338) primarygroup (89939)      609 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/vision/utils/__init__.py
-drwxr-x---   0 hongkuny (405338) primarygroup (89939)        0 2022-05-19 23:14:06.796168 tf-models-official-2.9.1/official/vision/utils/object_detection/
--rw-r-----   0 hongkuny (405338) primarygroup (89939)      609 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/vision/utils/object_detection/__init__.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     9011 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/vision/utils/object_detection/argmax_matcher.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)    11981 2022-05-18 02:34:16.000000 tf-models-official-2.9.1/official/vision/utils/object_detection/balanced_positive_negative_sampler.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     4776 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/vision/utils/object_detection/box_coder.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     6739 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/vision/utils/object_detection/box_list.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)    41925 2022-05-18 02:34:16.000000 tf-models-official-2.9.1/official/vision/utils/object_detection/box_list_ops.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     3806 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/vision/utils/object_detection/faster_rcnn_box_coder.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     8751 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/vision/utils/object_detection/matcher.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     3074 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/vision/utils/object_detection/minibatch_sampler.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     3212 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/vision/utils/object_detection/ops.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)    20356 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/vision/utils/object_detection/preprocessor.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     4544 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/vision/utils/object_detection/region_similarity_calculator.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     3608 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/vision/utils/object_detection/shape_utils.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)    24198 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/vision/utils/object_detection/target_assigner.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)    28966 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/official/vision/utils/object_detection/visualization_utils.py
-drwxr-x---   0 hongkuny (405338) primarygroup (89939)        0 2022-05-19 23:14:06.796168 tf-models-official-2.9.1/orbit/
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     1092 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/orbit/__init__.py
-drwxr-x---   0 hongkuny (405338) primarygroup (89939)        0 2022-05-19 23:14:06.796168 tf-models-official-2.9.1/orbit/actions/
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     3245 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/orbit/actions/__init__.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     1978 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/orbit/actions/conditional_action.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     1325 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/orbit/actions/conditional_action_test.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     4990 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/orbit/actions/export_saved_model.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     5864 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/orbit/actions/export_saved_model_test.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     8479 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/orbit/actions/new_best_metric.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     4014 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/orbit/actions/new_best_metric_test.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)    21772 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/orbit/controller.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)    28650 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/orbit/controller_test.py
-drwxr-x---   0 hongkuny (405338) primarygroup (89939)        0 2022-05-19 23:14:06.796168 tf-models-official-2.9.1/orbit/examples/
--rw-r-----   0 hongkuny (405338) primarygroup (89939)      604 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/orbit/examples/__init__.py
-drwxr-x---   0 hongkuny (405338) primarygroup (89939)        0 2022-05-19 23:14:06.796168 tf-models-official-2.9.1/orbit/examples/single_task/
--rw-r-----   0 hongkuny (405338) primarygroup (89939)      604 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/orbit/examples/single_task/__init__.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     3195 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/orbit/examples/single_task/single_task_evaluator.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     2088 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/orbit/examples/single_task/single_task_evaluator_test.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     5647 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/orbit/examples/single_task/single_task_trainer.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     1961 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/orbit/examples/single_task/single_task_trainer_test.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     3509 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/orbit/runner.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)    17400 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/orbit/standard_runner.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     5100 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/orbit/standard_runner_test.py
-drwxr-x---   0 hongkuny (405338) primarygroup (89939)        0 2022-05-19 23:14:06.796168 tf-models-official-2.9.1/orbit/utils/
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     1144 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/orbit/utils/__init__.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     3913 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/orbit/utils/common.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     1032 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/orbit/utils/common_test.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     2136 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/orbit/utils/epoch_helper.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     8016 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/orbit/utils/loop_fns.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     4177 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/orbit/utils/summary_manager.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     5631 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/orbit/utils/tpu_summaries.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     4513 2022-05-18 02:33:27.000000 tf-models-official-2.9.1/orbit/utils/tpu_summaries_test.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)       38 2022-05-19 23:14:06.796168 tf-models-official-2.9.1/setup.cfg
-drwxr-x---   0 hongkuny (405338) primarygroup (89939)        0 2022-05-19 23:14:06.796168 tf-models-official-2.9.1/tensorflow_models/
--rw-r-----   0 hongkuny (405338) primarygroup (89939)      909 2022-05-18 02:33:28.000000 tf-models-official-2.9.1/tensorflow_models/__init__.py
-drwxr-x---   0 hongkuny (405338) primarygroup (89939)        0 2022-05-19 23:14:06.796168 tf-models-official-2.9.1/tensorflow_models/nlp/
--rw-r-----   0 hongkuny (405338) primarygroup (89939)      807 2022-05-18 02:33:28.000000 tf-models-official-2.9.1/tensorflow_models/nlp/__init__.py
--rw-r-----   0 hongkuny (405338) primarygroup (89939)     1385 2022-05-18 02:33:28.000000 tf-models-official-2.9.1/tensorflow_models/tensorflow_models_test.py
-drwxr-x---   0 hongkuny (405338) primarygroup (89939)        0 2022-05-19 23:14:06.796168 tf-models-official-2.9.1/tensorflow_models/vision/
--rw-r-----   0 hongkuny (405338) primarygroup (89939)      762 2022-05-19 22:55:50.000000 tf-models-official-2.9.1/tensorflow_models/vision/__init__.py
-drwxr-x---   0 hongkuny (405338) primarygroup (89939)        0 2022-05-19 23:14:06.796168 tf-models-official-2.9.1/tf_models_official.egg-info/
--rw-r-----   0 hongkuny (405338) primarygroup (89939)      603 2022-05-19 23:14:06.000000 tf-models-official-2.9.1/tf_models_official.egg-info/PKG-INFO
--rw-r-----   0 hongkuny (405338) primarygroup (89939)    40366 2022-05-19 23:14:06.000000 tf-models-official-2.9.1/tf_models_official.egg-info/SOURCES.txt
--rw-r-----   0 hongkuny (405338) primarygroup (89939)        1 2022-05-19 23:14:06.000000 tf-models-official-2.9.1/tf_models_official.egg-info/dependency_links.txt
--rw-r-----   0 hongkuny (405338) primarygroup (89939)      448 2022-05-19 23:14:06.000000 tf-models-official-2.9.1/tf_models_official.egg-info/requires.txt
--rw-r-----   0 hongkuny (405338) primarygroup (89939)       33 2022-05-19 23:14:06.000000 tf-models-official-2.9.1/tf_models_official.egg-info/top_level.txt
+drwxr-x---   0 hongkuny (405338) primarygroup (89939)        0 2022-05-20 04:44:40.736379 tf-models-official-2.9.2/
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)      337 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/AUTHORS
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)    11405 2022-05-18 02:34:16.000000 tf-models-official-2.9.2/LICENSE
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)      603 2022-05-20 04:44:40.736379 tf-models-official-2.9.2/PKG-INFO
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     3072 2022-05-18 02:34:16.000000 tf-models-official-2.9.2/README.md
+drwxr-x---   0 hongkuny (405338) primarygroup (89939)        0 2022-05-20 04:44:40.676379 tf-models-official-2.9.2/official/
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)      609 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/__init__.py
+drwxr-x---   0 hongkuny (405338) primarygroup (89939)        0 2022-05-20 04:44:40.676379 tf-models-official-2.9.2/official/common/
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)      610 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/common/__init__.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     1848 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/common/dataset_fn.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     8585 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/common/distribute_utils.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     4904 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/common/distribute_utils_test.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     4166 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/common/flags.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)      843 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/common/registry_imports.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     1057 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/common/streamz_counters.py
+drwxr-x---   0 hongkuny (405338) primarygroup (89939)        0 2022-05-20 04:44:40.676379 tf-models-official-2.9.2/official/core/
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     1075 2022-05-19 22:57:12.000000 tf-models-official-2.9.2/official/core/__init__.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     8083 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/core/actions.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     4515 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/core/actions_test.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)    12890 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/core/base_task.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)    17377 2022-05-18 02:34:16.000000 tf-models-official-2.9.2/official/core/base_trainer.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)    13804 2022-05-18 02:34:16.000000 tf-models-official-2.9.2/official/core/base_trainer_test.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)    12208 2022-05-18 02:34:16.000000 tf-models-official-2.9.2/official/core/config_definitions.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     1115 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/core/exp_factory.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     7025 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/core/export_base.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     4426 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/core/export_base_test.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)    21463 2022-05-18 02:34:16.000000 tf-models-official-2.9.2/official/core/input_reader.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     4300 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/core/registry.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     2350 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/core/registry_test.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     2513 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/core/task_factory.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     1802 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/core/test_utils.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     5562 2022-05-18 02:34:16.000000 tf-models-official-2.9.2/official/core/train_lib.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     7917 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/core/train_lib_test.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)    19771 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/core/train_utils.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     7169 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/core/train_utils_test.py
+drwxr-x---   0 hongkuny (405338) primarygroup (89939)        0 2022-05-20 04:44:40.676379 tf-models-official-2.9.2/official/legacy/
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)      609 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/legacy/__init__.py
+drwxr-x---   0 hongkuny (405338) primarygroup (89939)        0 2022-05-20 04:44:40.676379 tf-models-official-2.9.2/official/legacy/albert/
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)      609 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/legacy/albert/__init__.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     2012 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/legacy/albert/configs.py
+drwxr-x---   0 hongkuny (405338) primarygroup (89939)        0 2022-05-20 04:44:40.680379 tf-models-official-2.9.2/official/legacy/bert/
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)      610 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/legacy/bert/__init__.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)    14931 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/legacy/bert/bert_models.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     3883 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/legacy/bert/bert_models_test.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     4832 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/legacy/bert/common_flags.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     4167 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/legacy/bert/configs.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     5966 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/legacy/bert/export_tfhub.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     4688 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/legacy/bert/export_tfhub_test.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)    11724 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/legacy/bert/input_pipeline.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     2875 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/legacy/bert/model_saving_utils.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)    25317 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/legacy/bert/model_training_utils.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)    11705 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/legacy/bert/model_training_utils_test.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)    18826 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/legacy/bert/run_classifier.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     8410 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/legacy/bert/run_pretraining.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     5366 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/legacy/bert/run_squad.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)    18945 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/legacy/bert/run_squad_helper.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     5054 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/legacy/bert/serving.py
+drwxr-x---   0 hongkuny (405338) primarygroup (89939)        0 2022-05-20 04:44:40.680379 tf-models-official-2.9.2/official/legacy/detection/
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)      609 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/legacy/detection/__init__.py
+drwxr-x---   0 hongkuny (405338) primarygroup (89939)        0 2022-05-20 04:44:40.680379 tf-models-official-2.9.2/official/legacy/detection/configs/
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)      609 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/legacy/detection/configs/__init__.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     4468 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/legacy/detection/configs/base_config.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     1692 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/legacy/detection/configs/factory.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     3328 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/legacy/detection/configs/maskrcnn_config.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     4271 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/legacy/detection/configs/olnmask_config.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     1776 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/legacy/detection/configs/retinanet_config.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     3204 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/legacy/detection/configs/shapemask_config.py
+drwxr-x---   0 hongkuny (405338) primarygroup (89939)        0 2022-05-20 04:44:40.680379 tf-models-official-2.9.2/official/legacy/detection/dataloader/
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)      609 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/legacy/detection/dataloader/__init__.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)    20689 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/legacy/detection/dataloader/anchor.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     6563 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/legacy/detection/dataloader/factory.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     3653 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/legacy/detection/dataloader/input_reader.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)    15731 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/legacy/detection/dataloader/maskrcnn_parser.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     1061 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/legacy/detection/dataloader/mode_keys.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)    14218 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/legacy/detection/dataloader/olnmask_parser.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)    18283 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/legacy/detection/dataloader/retinanet_parser.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)    22331 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/legacy/detection/dataloader/shapemask_parser.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     6219 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/legacy/detection/dataloader/tf_example_decoder.py
+drwxr-x---   0 hongkuny (405338) primarygroup (89939)        0 2022-05-20 04:44:40.680379 tf-models-official-2.9.2/official/legacy/detection/evaluation/
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)      609 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/legacy/detection/evaluation/__init__.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)    24838 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/legacy/detection/evaluation/coco_evaluator.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)    15169 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/legacy/detection/evaluation/coco_utils.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     2169 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/legacy/detection/evaluation/factory.py
+drwxr-x---   0 hongkuny (405338) primarygroup (89939)        0 2022-05-20 04:44:40.680379 tf-models-official-2.9.2/official/legacy/detection/executor/
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)      609 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/legacy/detection/executor/__init__.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     6259 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/legacy/detection/executor/detection_executor.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)    30080 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/legacy/detection/executor/distributed_executor.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     9015 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/legacy/detection/main.py
+drwxr-x---   0 hongkuny (405338) primarygroup (89939)        0 2022-05-20 04:44:40.680379 tf-models-official-2.9.2/official/legacy/detection/modeling/
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)      609 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/legacy/detection/modeling/__init__.py
+drwxr-x---   0 hongkuny (405338) primarygroup (89939)        0 2022-05-20 04:44:40.680379 tf-models-official-2.9.2/official/legacy/detection/modeling/architecture/
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)      609 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/legacy/detection/modeling/architecture/__init__.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     7994 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/legacy/detection/modeling/architecture/factory.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     5976 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/legacy/detection/modeling/architecture/fpn.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)    49476 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/legacy/detection/modeling/architecture/heads.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)      974 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/legacy/detection/modeling/architecture/identity.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)    11219 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/legacy/detection/modeling/architecture/nn_blocks.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     3853 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/legacy/detection/modeling/architecture/nn_ops.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)    13159 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/legacy/detection/modeling/architecture/resnet.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)    17270 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/legacy/detection/modeling/architecture/spinenet.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     4439 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/legacy/detection/modeling/base_model.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     4862 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/legacy/detection/modeling/checkpoint_utils.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     1402 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/legacy/detection/modeling/factory.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     3800 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/legacy/detection/modeling/learning_rates.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)    30203 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/legacy/detection/modeling/losses.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)    13458 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/legacy/detection/modeling/maskrcnn_model.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)    16774 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/legacy/detection/modeling/olnmask_model.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     1716 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/legacy/detection/modeling/optimizers.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     6661 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/legacy/detection/modeling/retinanet_model.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)    12110 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/legacy/detection/modeling/shapemask_model.py
+drwxr-x---   0 hongkuny (405338) primarygroup (89939)        0 2022-05-20 04:44:40.684379 tf-models-official-2.9.2/official/legacy/detection/ops/
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)      609 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/legacy/detection/ops/__init__.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     8125 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/legacy/detection/ops/nms.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)    21942 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/legacy/detection/ops/postprocess_ops.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)    22986 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/legacy/detection/ops/roi_ops.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)    25998 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/legacy/detection/ops/spatial_transform_ops.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)    28304 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/legacy/detection/ops/target_ops.py
+drwxr-x---   0 hongkuny (405338) primarygroup (89939)        0 2022-05-20 04:44:40.684379 tf-models-official-2.9.2/official/legacy/detection/utils/
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)      609 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/legacy/detection/utils/__init__.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)    26050 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/legacy/detection/utils/box_utils.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     1465 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/legacy/detection/utils/class_utils.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     1575 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/legacy/detection/utils/dataloader_utils.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)    14297 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/legacy/detection/utils/input_utils.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     6647 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/legacy/detection/utils/mask_utils.py
+drwxr-x---   0 hongkuny (405338) primarygroup (89939)        0 2022-05-20 04:44:40.684379 tf-models-official-2.9.2/official/legacy/image_classification/
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)      609 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/legacy/image_classification/__init__.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)    34315 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/legacy/image_classification/augment.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     4313 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/legacy/image_classification/augment_test.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     9355 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/legacy/image_classification/callbacks.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)    16195 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/legacy/image_classification/classifier_trainer.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     7755 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/legacy/image_classification/classifier_trainer_test.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     6047 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/legacy/image_classification/classifier_trainer_util_test.py
+drwxr-x---   0 hongkuny (405338) primarygroup (89939)        0 2022-05-20 04:44:40.684379 tf-models-official-2.9.2/official/legacy/image_classification/configs/
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)      609 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/legacy/image_classification/configs/__init__.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     8668 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/legacy/image_classification/configs/base_configs.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     6110 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/legacy/image_classification/configs/configs.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)    19517 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/legacy/image_classification/dataset_factory.py
+drwxr-x---   0 hongkuny (405338) primarygroup (89939)        0 2022-05-20 04:44:40.684379 tf-models-official-2.9.2/official/legacy/image_classification/efficientnet/
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)      609 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/legacy/image_classification/efficientnet/__init__.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     4609 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/legacy/image_classification/efficientnet/common_modules.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     2867 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/legacy/image_classification/efficientnet/efficientnet_config.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)    16417 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/legacy/image_classification/efficientnet/efficientnet_model.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     2317 2022-05-18 02:34:16.000000 tf-models-official-2.9.2/official/legacy/image_classification/efficientnet/tfhub_export.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     4272 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/legacy/image_classification/learning_rate.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     1941 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/legacy/image_classification/learning_rate_test.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     6114 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/legacy/image_classification/mnist_main.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     2581 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/legacy/image_classification/mnist_test.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     6844 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/legacy/image_classification/optimizer_factory.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     4067 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/legacy/image_classification/optimizer_factory_test.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)    13537 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/legacy/image_classification/preprocessing.py
+drwxr-x---   0 hongkuny (405338) primarygroup (89939)        0 2022-05-20 04:44:40.684379 tf-models-official-2.9.2/official/legacy/image_classification/resnet/
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)      609 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/legacy/image_classification/resnet/__init__.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)    16094 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/legacy/image_classification/resnet/common.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)    21168 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/legacy/image_classification/resnet/imagenet_preprocessing.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     2070 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/legacy/image_classification/resnet/resnet_config.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     6916 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/legacy/image_classification/resnet/resnet_ctl_imagenet_main.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)    10945 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/legacy/image_classification/resnet/resnet_model.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     8124 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/legacy/image_classification/resnet/resnet_runnable.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     2189 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/legacy/image_classification/resnet/tfhub_export.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     1322 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/legacy/image_classification/test_utils.py
+drwxr-x---   0 hongkuny (405338) primarygroup (89939)        0 2022-05-20 04:44:40.684379 tf-models-official-2.9.2/official/legacy/image_classification/vgg/
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)      610 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/legacy/image_classification/vgg/__init__.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     1803 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/legacy/image_classification/vgg/vgg_config.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     7607 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/legacy/image_classification/vgg/vgg_model.py
+drwxr-x---   0 hongkuny (405338) primarygroup (89939)        0 2022-05-20 04:44:40.688379 tf-models-official-2.9.2/official/legacy/transformer/
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)      609 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/legacy/transformer/__init__.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     7047 2022-05-18 02:34:16.000000 tf-models-official-2.9.2/official/legacy/transformer/attention_layer.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     3679 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/legacy/transformer/beam_search_v1.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     5141 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/legacy/transformer/compute_bleu.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     2585 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/legacy/transformer/compute_bleu_test.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)    15295 2022-05-18 02:34:16.000000 tf-models-official-2.9.2/official/legacy/transformer/data_download.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)    13237 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/legacy/transformer/data_pipeline.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     3684 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/legacy/transformer/embedding_layer.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     2320 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/legacy/transformer/ffn_layer.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     7007 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/legacy/transformer/metrics.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)    10346 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/legacy/transformer/misc.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     2936 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/legacy/transformer/model_params.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     4427 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/legacy/transformer/model_utils.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     1891 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/legacy/transformer/model_utils_test.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     2434 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/legacy/transformer/optimizer.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)    21751 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/legacy/transformer/transformer.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     6060 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/legacy/transformer/transformer_forward_test.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     3566 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/legacy/transformer/transformer_layers_test.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)    18183 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/legacy/transformer/transformer_main.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     6631 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/legacy/transformer/transformer_main_test.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     3628 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/legacy/transformer/transformer_test.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     6951 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/legacy/transformer/translate.py
+drwxr-x---   0 hongkuny (405338) primarygroup (89939)        0 2022-05-20 04:44:40.688379 tf-models-official-2.9.2/official/legacy/transformer/utils/
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)      609 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/legacy/transformer/utils/__init__.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)    16706 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/legacy/transformer/utils/metrics.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)    24517 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/legacy/transformer/utils/tokenizer.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     6658 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/legacy/transformer/utils/tokenizer_test.py
+drwxr-x---   0 hongkuny (405338) primarygroup (89939)        0 2022-05-20 04:44:40.688379 tf-models-official-2.9.2/official/legacy/xlnet/
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)      610 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/legacy/xlnet/__init__.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     5421 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/legacy/xlnet/classifier_utils.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     5367 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/legacy/xlnet/common_flags.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)    30095 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/legacy/xlnet/data_utils.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     3762 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/legacy/xlnet/optimization.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)    15344 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/legacy/xlnet/preprocess_classification_data.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)    32400 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/legacy/xlnet/preprocess_pretrain_data.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     4046 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/legacy/xlnet/preprocess_squad_data.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     3693 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/legacy/xlnet/preprocess_utils.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     6976 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/legacy/xlnet/run_classifier.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     5710 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/legacy/xlnet/run_pretrain.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)    11597 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/legacy/xlnet/run_squad.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)    32226 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/legacy/xlnet/squad_utils.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)    11664 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/legacy/xlnet/training_utils.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     5894 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/legacy/xlnet/xlnet_config.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)    47595 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/legacy/xlnet/xlnet_modeling.py
+drwxr-x---   0 hongkuny (405338) primarygroup (89939)        0 2022-05-20 04:44:40.688379 tf-models-official-2.9.2/official/modeling/
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)      609 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/modeling/__init__.py
+drwxr-x---   0 hongkuny (405338) primarygroup (89939)        0 2022-05-20 04:44:40.688379 tf-models-official-2.9.2/official/modeling/activations/
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)      992 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/modeling/activations/__init__.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     1037 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/modeling/activations/gelu.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     1212 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/modeling/activations/gelu_test.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)      984 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/modeling/activations/relu.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     1200 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/modeling/activations/relu_test.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     1041 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/modeling/activations/sigmoid.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     1364 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/modeling/activations/sigmoid_test.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     2291 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/modeling/activations/swish.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     1566 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/modeling/activations/swish_test.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     6730 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/modeling/grad_utils.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     2786 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/modeling/grad_utils_test.py
+drwxr-x---   0 hongkuny (405338) primarygroup (89939)        0 2022-05-20 04:44:40.688379 tf-models-official-2.9.2/official/modeling/hyperparams/
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)      846 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/modeling/hyperparams/__init__.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)    11213 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/modeling/hyperparams/base_config.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)    11413 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/modeling/hyperparams/base_config_test.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     1870 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/modeling/hyperparams/oneof.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     1882 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/modeling/hyperparams/oneof_test.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)    16402 2022-05-18 02:34:16.000000 tf-models-official-2.9.2/official/modeling/hyperparams/params_dict.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)    13657 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/modeling/hyperparams/params_dict_test.py
+drwxr-x---   0 hongkuny (405338) primarygroup (89939)        0 2022-05-20 04:44:40.692379 tf-models-official-2.9.2/official/modeling/multitask/
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)      609 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/modeling/multitask/__init__.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     1538 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/modeling/multitask/base_model.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     5846 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/modeling/multitask/base_trainer.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     3653 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/modeling/multitask/base_trainer_test.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     2683 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/modeling/multitask/configs.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     6068 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/modeling/multitask/evaluator.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     4633 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/modeling/multitask/evaluator_test.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     3948 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/modeling/multitask/interleaving_trainer.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     4295 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/modeling/multitask/interleaving_trainer_test.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     5946 2022-05-18 02:34:16.000000 tf-models-official-2.9.2/official/modeling/multitask/multitask.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     4887 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/modeling/multitask/task_sampler.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     3027 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/modeling/multitask/task_sampler_test.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     3887 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/modeling/multitask/test_utils.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     9741 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/modeling/multitask/train_lib.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     4622 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/modeling/multitask/train_lib_test.py
+drwxr-x---   0 hongkuny (405338) primarygroup (89939)        0 2022-05-20 04:44:40.692379 tf-models-official-2.9.2/official/modeling/optimization/
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     1201 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/modeling/optimization/__init__.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)      792 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/modeling/optimization/adafactor_optimizer.py
+drwxr-x---   0 hongkuny (405338) primarygroup (89939)        0 2022-05-20 04:44:40.692379 tf-models-official-2.9.2/official/modeling/optimization/configs/
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)      609 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/modeling/optimization/configs/__init__.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)    11122 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/modeling/optimization/configs/learning_rate_config.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     4707 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/modeling/optimization/configs/optimization_config.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     2009 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/modeling/optimization/configs/optimization_config_test.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)    10717 2022-05-18 02:34:16.000000 tf-models-official-2.9.2/official/modeling/optimization/configs/optimizer_config.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     9086 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/modeling/optimization/ema_optimizer.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     7331 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/modeling/optimization/lars_optimizer.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)    19101 2022-05-18 02:34:16.000000 tf-models-official-2.9.2/official/modeling/optimization/lr_schedule.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     3951 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/modeling/optimization/lr_schedule_test.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     7854 2022-05-18 02:34:16.000000 tf-models-official-2.9.2/official/modeling/optimization/optimizer_factory.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)    14110 2022-05-18 02:34:16.000000 tf-models-official-2.9.2/official/modeling/optimization/optimizer_factory_test.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)      707 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/modeling/optimization/slide_optimizer.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     2159 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/modeling/performance.py
+drwxr-x---   0 hongkuny (405338) primarygroup (89939)        0 2022-05-20 04:44:40.692379 tf-models-official-2.9.2/official/modeling/privacy/
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)      609 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/modeling/privacy/__init__.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)      960 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/modeling/privacy/configs.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     1359 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/modeling/privacy/configs_test.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     1452 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/modeling/privacy/ops.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     1684 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/modeling/privacy/ops_test.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     8834 2022-05-18 02:34:16.000000 tf-models-official-2.9.2/official/modeling/tf_utils.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     2967 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/modeling/tf_utils_test.py
+drwxr-x---   0 hongkuny (405338) primarygroup (89939)        0 2022-05-20 04:44:40.692379 tf-models-official-2.9.2/official/nlp/
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)      609 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/nlp/__init__.py
+drwxr-x---   0 hongkuny (405338) primarygroup (89939)        0 2022-05-20 04:44:40.692379 tf-models-official-2.9.2/official/nlp/configs/
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)      609 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/nlp/configs/__init__.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     1423 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/nlp/configs/bert.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     1381 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/nlp/configs/electra.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)    22095 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/nlp/configs/encoders.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     1963 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/nlp/configs/encoders_test.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)      899 2022-05-18 02:34:16.000000 tf-models-official-2.9.2/official/nlp/configs/experiment_configs.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     6571 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/nlp/configs/finetuning_experiments.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     2968 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/nlp/configs/pretraining_experiments.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     3791 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/nlp/configs/wmt_transformer_experiments.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     7884 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/nlp/continuous_finetune_lib.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     3182 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/nlp/continuous_finetune_lib_test.py
+drwxr-x---   0 hongkuny (405338) primarygroup (89939)        0 2022-05-20 04:44:40.696379 tf-models-official-2.9.2/official/nlp/data/
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)      609 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/nlp/data/__init__.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)    56381 2022-05-18 02:34:16.000000 tf-models-official-2.9.2/official/nlp/data/classifier_data_lib.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     3352 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/nlp/data/classifier_data_lib_test.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)    16693 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/nlp/data/create_finetuning_data.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)    23360 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/nlp/data/create_pretraining_data.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     4857 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/nlp/data/create_pretraining_data_test.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)    24192 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/nlp/data/create_xlnet_pretraining_data.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)    10930 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/nlp/data/create_xlnet_pretraining_data_test.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     1688 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/nlp/data/data_loader.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     1788 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/nlp/data/data_loader_factory.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     1325 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/nlp/data/data_loader_factory_test.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     5713 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/nlp/data/dual_encoder_dataloader.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     5040 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/nlp/data/dual_encoder_dataloader_test.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)    24634 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/nlp/data/pretrain_dataloader.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     9141 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/nlp/data/pretrain_dataloader_test.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     9814 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/nlp/data/pretrain_dynamic_dataloader.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     9620 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/nlp/data/pretrain_dynamic_dataloader_test.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     4308 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/nlp/data/question_answering_dataloader.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     2830 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/nlp/data/question_answering_dataloader_test.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)    10337 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/nlp/data/sentence_prediction_dataloader.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)    11662 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/nlp/data/sentence_prediction_dataloader_test.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     6413 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/nlp/data/sentence_retrieval_lib.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)    36512 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/nlp/data/squad_lib.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)    34939 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/nlp/data/squad_lib_sp.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)    15489 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/nlp/data/tagging_data_lib.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     3737 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/nlp/data/tagging_data_lib_test.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     3181 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/nlp/data/tagging_dataloader.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     3196 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/nlp/data/tagging_dataloader_test.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     4517 2022-05-18 02:34:16.000000 tf-models-official-2.9.2/official/nlp/data/train_sentencepiece.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)    11174 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/nlp/data/wmt_dataloader.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     4892 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/nlp/data/wmt_dataloader_test.py
+drwxr-x---   0 hongkuny (405338) primarygroup (89939)        0 2022-05-20 04:44:40.696379 tf-models-official-2.9.2/official/nlp/metrics/
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)      609 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/nlp/metrics/__init__.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     6577 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/nlp/metrics/bleu.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     2498 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/nlp/metrics/bleu_test.py
+drwxr-x---   0 hongkuny (405338) primarygroup (89939)        0 2022-05-20 04:44:40.696379 tf-models-official-2.9.2/official/nlp/modeling/
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     1062 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/nlp/modeling/__init__.py
+drwxr-x---   0 hongkuny (405338) primarygroup (89939)        0 2022-05-20 04:44:40.700379 tf-models-official-2.9.2/official/nlp/modeling/layers/
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     3712 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/nlp/modeling/layers/__init__.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     3909 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/nlp/modeling/layers/attention.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     3681 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/nlp/modeling/layers/attention_test.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)    21026 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/nlp/modeling/layers/bigbird_attention.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     2196 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/nlp/modeling/layers/bigbird_attention_test.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     6915 2022-05-18 02:34:16.000000 tf-models-official-2.9.2/official/nlp/modeling/layers/block_diag_feedforward.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     4302 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/nlp/modeling/layers/block_diag_feedforward_test.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)    13104 2022-05-18 02:34:16.000000 tf-models-official-2.9.2/official/nlp/modeling/layers/cls_head.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     7841 2022-05-18 02:34:16.000000 tf-models-official-2.9.2/official/nlp/modeling/layers/cls_head_test.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     9058 2022-05-18 02:34:16.000000 tf-models-official-2.9.2/official/nlp/modeling/layers/gated_feedforward.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     4806 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/nlp/modeling/layers/gated_feedforward_test.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)    20472 2022-05-18 02:34:16.000000 tf-models-official-2.9.2/official/nlp/modeling/layers/gaussian_process.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)    10091 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/nlp/modeling/layers/gaussian_process_test.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)    15968 2022-05-18 02:34:16.000000 tf-models-official-2.9.2/official/nlp/modeling/layers/kernel_attention.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     4190 2022-05-18 02:34:16.000000 tf-models-official-2.9.2/official/nlp/modeling/layers/kernel_attention_test.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     4826 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/nlp/modeling/layers/masked_lm.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     5853 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/nlp/modeling/layers/masked_lm_test.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     3028 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/nlp/modeling/layers/masked_softmax.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     4694 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/nlp/modeling/layers/masked_softmax_test.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     2294 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/nlp/modeling/layers/mat_mul_with_margin.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     2136 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/nlp/modeling/layers/mat_mul_with_margin_test.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)    22368 2022-05-18 02:34:16.000000 tf-models-official-2.9.2/official/nlp/modeling/layers/mobile_bert_layers.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)    10880 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/nlp/modeling/layers/mobile_bert_layers_test.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     7192 2022-05-18 02:34:16.000000 tf-models-official-2.9.2/official/nlp/modeling/layers/multi_channel_attention.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     1912 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/nlp/modeling/layers/multi_channel_attention_test.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     3960 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/nlp/modeling/layers/on_device_embedding.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     8880 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/nlp/modeling/layers/on_device_embedding_test.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)    11393 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/nlp/modeling/layers/position_embedding.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     8538 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/nlp/modeling/layers/position_embedding_test.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)    20486 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/nlp/modeling/layers/relative_attention.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     6806 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/nlp/modeling/layers/relative_attention_test.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)    24761 2022-05-18 02:34:16.000000 tf-models-official-2.9.2/official/nlp/modeling/layers/reuse_attention.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)    14319 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/nlp/modeling/layers/reuse_attention_test.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)    15396 2022-05-18 02:34:16.000000 tf-models-official-2.9.2/official/nlp/modeling/layers/reuse_transformer.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)    17478 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/nlp/modeling/layers/reuse_transformer_test.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)    11686 2022-05-18 02:34:16.000000 tf-models-official-2.9.2/official/nlp/modeling/layers/rezero_transformer.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     5874 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/nlp/modeling/layers/rezero_transformer_test.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     4559 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/nlp/modeling/layers/routing.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     2216 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/nlp/modeling/layers/routing_test.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     2030 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/nlp/modeling/layers/self_attention_mask.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)    10735 2022-05-18 02:34:16.000000 tf-models-official-2.9.2/official/nlp/modeling/layers/spectral_normalization.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     3111 2022-05-18 02:34:16.000000 tf-models-official-2.9.2/official/nlp/modeling/layers/spectral_normalization_test.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     6807 2022-05-18 02:34:16.000000 tf-models-official-2.9.2/official/nlp/modeling/layers/talking_heads_attention.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     7289 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/nlp/modeling/layers/talking_heads_attention_test.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)    32516 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/nlp/modeling/layers/text_layers.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)    24245 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/nlp/modeling/layers/text_layers_test.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     6617 2022-05-18 02:34:16.000000 tf-models-official-2.9.2/official/nlp/modeling/layers/tn_expand_condense.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     6720 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/nlp/modeling/layers/tn_expand_condense_test.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)    11015 2022-05-18 02:34:16.000000 tf-models-official-2.9.2/official/nlp/modeling/layers/tn_transformer_expand_condense.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     9160 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/nlp/modeling/layers/tn_transformer_test.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)    18312 2022-05-18 02:34:16.000000 tf-models-official-2.9.2/official/nlp/modeling/layers/transformer.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)    16791 2022-05-18 02:34:16.000000 tf-models-official-2.9.2/official/nlp/modeling/layers/transformer_encoder_block.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)    24495 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/nlp/modeling/layers/transformer_encoder_block_test.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)    13372 2022-05-18 02:34:16.000000 tf-models-official-2.9.2/official/nlp/modeling/layers/transformer_scaffold.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)    20384 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/nlp/modeling/layers/transformer_scaffold_test.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     3718 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/nlp/modeling/layers/transformer_test.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)    22109 2022-05-18 02:34:16.000000 tf-models-official-2.9.2/official/nlp/modeling/layers/transformer_xl.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     9514 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/nlp/modeling/layers/transformer_xl_test.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     2723 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/nlp/modeling/layers/util.py
+drwxr-x---   0 hongkuny (405338) primarygroup (89939)        0 2022-05-20 04:44:40.700379 tf-models-official-2.9.2/official/nlp/modeling/losses/
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)      824 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/nlp/modeling/losses/__init__.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     2859 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/nlp/modeling/losses/weighted_sparse_categorical_crossentropy.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     8619 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/nlp/modeling/losses/weighted_sparse_categorical_crossentropy_test.py
+drwxr-x---   0 hongkuny (405338) primarygroup (89939)        0 2022-05-20 04:44:40.700379 tf-models-official-2.9.2/official/nlp/modeling/models/
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     1654 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/nlp/modeling/models/__init__.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     5896 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/nlp/modeling/models/bert_classifier.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     5092 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/nlp/modeling/models/bert_classifier_test.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)    11310 2022-05-18 02:34:16.000000 tf-models-official-2.9.2/official/nlp/modeling/models/bert_pretrainer.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)    10116 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/nlp/modeling/models/bert_pretrainer_test.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     4997 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/nlp/modeling/models/bert_span_labeler.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     5053 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/nlp/modeling/models/bert_span_labeler_test.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     5216 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/nlp/modeling/models/bert_token_classifier.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     5112 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/nlp/modeling/models/bert_token_classifier_test.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     6583 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/nlp/modeling/models/dual_encoder.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     5377 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/nlp/modeling/models/dual_encoder_test.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)    12841 2022-05-18 02:34:16.000000 tf-models-official-2.9.2/official/nlp/modeling/models/electra_pretrainer.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     6804 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/nlp/modeling/models/electra_pretrainer_test.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)    25716 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/nlp/modeling/models/seq2seq_transformer.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     5402 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/nlp/modeling/models/seq2seq_transformer_test.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)    54288 2022-05-18 02:34:16.000000 tf-models-official-2.9.2/official/nlp/modeling/models/t5.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)    24241 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/nlp/modeling/models/t5_test.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)    11779 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/nlp/modeling/models/xlnet.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)    13044 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/nlp/modeling/models/xlnet_test.py
+drwxr-x---   0 hongkuny (405338) primarygroup (89939)        0 2022-05-20 04:44:40.704379 tf-models-official-2.9.2/official/nlp/modeling/networks/
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     1718 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/nlp/modeling/networks/__init__.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     8702 2022-05-18 02:34:16.000000 tf-models-official-2.9.2/official/nlp/modeling/networks/albert_encoder.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     7494 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/nlp/modeling/networks/albert_encoder_test.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)    14506 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/nlp/modeling/networks/bert_dense_encoder_test.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)    23007 2022-05-18 02:34:16.000000 tf-models-official-2.9.2/official/nlp/modeling/networks/bert_encoder.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)    24661 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/nlp/modeling/networks/bert_encoder_test.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     4242 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/nlp/modeling/networks/classification.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     7448 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/nlp/modeling/networks/classification_test.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)    16903 2022-05-18 02:34:16.000000 tf-models-official-2.9.2/official/nlp/modeling/networks/encoder_scaffold.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)    29410 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/nlp/modeling/networks/encoder_scaffold_test.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)    20834 2022-05-18 02:34:16.000000 tf-models-official-2.9.2/official/nlp/modeling/networks/funnel_transformer.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)    14442 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/nlp/modeling/networks/funnel_transformer_test.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     7569 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/nlp/modeling/networks/mobile_bert_encoder.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     7105 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/nlp/modeling/networks/mobile_bert_encoder_test.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)    12841 2022-05-18 02:34:16.000000 tf-models-official-2.9.2/official/nlp/modeling/networks/packed_sequence_embedding.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     5066 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/nlp/modeling/networks/packed_sequence_embedding_test.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)    13033 2022-05-18 02:34:16.000000 tf-models-official-2.9.2/official/nlp/modeling/networks/span_labeling.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)    12330 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/nlp/modeling/networks/span_labeling_test.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)    25837 2022-05-18 02:34:16.000000 tf-models-official-2.9.2/official/nlp/modeling/networks/xlnet_base.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)    14869 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/nlp/modeling/networks/xlnet_base_test.py
+drwxr-x---   0 hongkuny (405338) primarygroup (89939)        0 2022-05-20 04:44:40.704379 tf-models-official-2.9.2/official/nlp/modeling/ops/
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)      873 2022-05-18 02:34:16.000000 tf-models-official-2.9.2/official/nlp/modeling/ops/__init__.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)    28925 2022-05-18 02:34:16.000000 tf-models-official-2.9.2/official/nlp/modeling/ops/beam_search.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     3505 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/nlp/modeling/ops/beam_search_test.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)    10047 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/nlp/modeling/ops/decoding_module.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     2573 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/nlp/modeling/ops/decoding_module_test.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)    18023 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/nlp/modeling/ops/sampling_module.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     9596 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/nlp/modeling/ops/segment_extractor.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     5398 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/nlp/modeling/ops/segment_extractor_test.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     9024 2022-05-18 02:34:16.000000 tf-models-official-2.9.2/official/nlp/optimization.py
+drwxr-x---   0 hongkuny (405338) primarygroup (89939)        0 2022-05-20 04:44:40.704379 tf-models-official-2.9.2/official/nlp/serving/
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)      610 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/nlp/serving/__init__.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     5618 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/nlp/serving/export_savedmodel.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     6513 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/nlp/serving/export_savedmodel_test.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     2312 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/nlp/serving/export_savedmodel_util.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)    18889 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/nlp/serving/serving_modules.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)    15068 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/nlp/serving/serving_modules_test.py
+drwxr-x---   0 hongkuny (405338) primarygroup (89939)        0 2022-05-20 04:44:40.704379 tf-models-official-2.9.2/official/nlp/tasks/
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     1178 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/nlp/tasks/__init__.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     7634 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/nlp/tasks/dual_encoder.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     4561 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/nlp/tasks/dual_encoder_test.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     9637 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/nlp/tasks/electra_task.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     2282 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/nlp/tasks/electra_task_test.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     7703 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/nlp/tasks/masked_lm.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     2160 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/nlp/tasks/masked_lm_test.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)    19817 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/nlp/tasks/question_answering.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     9939 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/nlp/tasks/question_answering_test.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)    12386 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/nlp/tasks/sentence_prediction.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)    10358 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/nlp/tasks/sentence_prediction_test.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)    10088 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/nlp/tasks/tagging.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     6407 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/nlp/tasks/tagging_test.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)    13381 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/nlp/tasks/translation.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     6871 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/nlp/tasks/translation_test.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     2575 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/nlp/tasks/utils.py
+drwxr-x---   0 hongkuny (405338) primarygroup (89939)        0 2022-05-20 04:44:40.704379 tf-models-official-2.9.2/official/nlp/tools/
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)      610 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/nlp/tools/__init__.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     9443 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/nlp/tools/export_tfhub.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)    21271 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/nlp/tools/export_tfhub_lib.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)    46347 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/nlp/tools/export_tfhub_lib_test.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     3724 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/nlp/tools/squad_evaluate_v1_1.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     8625 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/nlp/tools/squad_evaluate_v2_0.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     7865 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/nlp/tools/tf1_bert_checkpoint_converter_lib.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     6676 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/nlp/tools/tf2_albert_encoder_checkpoint_converter.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     5826 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/nlp/tools/tf2_bert_encoder_checkpoint_converter.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)    16591 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/nlp/tools/tokenization.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     5217 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/nlp/tools/tokenization_test.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     3043 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/nlp/train.py
+drwxr-x---   0 hongkuny (405338) primarygroup (89939)        0 2022-05-20 04:44:40.704379 tf-models-official-2.9.2/official/projects/
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)      609 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/projects/__init__.py
+drwxr-x---   0 hongkuny (405338) primarygroup (89939)        0 2022-05-20 04:44:40.704379 tf-models-official-2.9.2/official/projects/bigbird/
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)      609 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/projects/bigbird/__init__.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     9233 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/projects/bigbird/encoder.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     2340 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/projects/bigbird/encoder_test.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     3774 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/projects/bigbird/experiment_configs.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     9027 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/projects/bigbird/recompute_grad.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     5942 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/projects/bigbird/recomputing_dropout.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     4921 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/projects/bigbird/stateless_dropout.py
+drwxr-x---   0 hongkuny (405338) primarygroup (89939)        0 2022-05-20 04:44:40.704379 tf-models-official-2.9.2/official/projects/deepmac_maskrcnn/
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)      609 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/projects/deepmac_maskrcnn/__init__.py
+drwxr-x---   0 hongkuny (405338) primarygroup (89939)        0 2022-05-20 04:44:40.704379 tf-models-official-2.9.2/official/projects/deepmac_maskrcnn/common/
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)      609 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/projects/deepmac_maskrcnn/common/__init__.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)      775 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/projects/deepmac_maskrcnn/common/registry_imports.py
+drwxr-x---   0 hongkuny (405338) primarygroup (89939)        0 2022-05-20 04:44:40.704379 tf-models-official-2.9.2/official/projects/deepmac_maskrcnn/configs/
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)      609 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/projects/deepmac_maskrcnn/configs/__init__.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     7948 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/projects/deepmac_maskrcnn/configs/deep_mask_head_rcnn.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     1218 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/projects/deepmac_maskrcnn/configs/deep_mask_head_rcnn_config_test.py
+drwxr-x---   0 hongkuny (405338) primarygroup (89939)        0 2022-05-20 04:44:40.708379 tf-models-official-2.9.2/official/projects/deepmac_maskrcnn/modeling/
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)      609 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/projects/deepmac_maskrcnn/modeling/__init__.py
+drwxr-x---   0 hongkuny (405338) primarygroup (89939)        0 2022-05-20 04:44:40.708379 tf-models-official-2.9.2/official/projects/deepmac_maskrcnn/modeling/heads/
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)      609 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/projects/deepmac_maskrcnn/modeling/heads/__init__.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)    21630 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/projects/deepmac_maskrcnn/modeling/heads/hourglass_network.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)    12058 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/projects/deepmac_maskrcnn/modeling/heads/instance_heads.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     3172 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/projects/deepmac_maskrcnn/modeling/heads/instance_heads_test.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     8566 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/projects/deepmac_maskrcnn/modeling/maskrcnn_model.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     5471 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/projects/deepmac_maskrcnn/modeling/maskrcnn_model_test.py
+drwxr-x---   0 hongkuny (405338) primarygroup (89939)        0 2022-05-20 04:44:40.708379 tf-models-official-2.9.2/official/projects/deepmac_maskrcnn/serving/
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)      609 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/projects/deepmac_maskrcnn/serving/__init__.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     5494 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/projects/deepmac_maskrcnn/serving/detection.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     6352 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/projects/deepmac_maskrcnn/serving/detection_test.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     3991 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/projects/deepmac_maskrcnn/serving/export_saved_model.py
+drwxr-x---   0 hongkuny (405338) primarygroup (89939)        0 2022-05-20 04:44:40.708379 tf-models-official-2.9.2/official/projects/deepmac_maskrcnn/tasks/
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)      609 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/projects/deepmac_maskrcnn/tasks/__init__.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     8585 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/projects/deepmac_maskrcnn/tasks/deep_mask_head_rcnn.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     2630 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/projects/deepmac_maskrcnn/train.py
+drwxr-x---   0 hongkuny (405338) primarygroup (89939)        0 2022-05-20 04:44:40.708379 tf-models-official-2.9.2/official/projects/mobilebert/
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)      609 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/projects/mobilebert/__init__.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)    24889 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/projects/mobilebert/distillation.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     7239 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/projects/mobilebert/distillation_test.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     3689 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/projects/mobilebert/export_tfhub.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     7470 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/projects/mobilebert/model_utils.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     5486 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/projects/mobilebert/run_distillation.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)    10709 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/projects/mobilebert/tf2_model_checkpoint_converter.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     1036 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/projects/mobilebert/utils.py
+drwxr-x---   0 hongkuny (405338) primarygroup (89939)        0 2022-05-20 04:44:40.708379 tf-models-official-2.9.2/official/projects/movinet/
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)      609 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/projects/movinet/__init__.py
+drwxr-x---   0 hongkuny (405338) primarygroup (89939)        0 2022-05-20 04:44:40.708379 tf-models-official-2.9.2/official/projects/movinet/configs/
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)      609 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/projects/movinet/configs/__init__.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     4298 2022-05-18 02:34:16.000000 tf-models-official-2.9.2/official/projects/movinet/configs/movinet.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     1596 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/projects/movinet/configs/movinet_test.py
+drwxr-x---   0 hongkuny (405338) primarygroup (89939)        0 2022-05-20 04:44:40.708379 tf-models-official-2.9.2/official/projects/movinet/modeling/
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)      609 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/projects/movinet/modeling/__init__.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)    29032 2022-05-18 02:34:16.000000 tf-models-official-2.9.2/official/projects/movinet/modeling/movinet.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)    60645 2022-05-18 02:34:16.000000 tf-models-official-2.9.2/official/projects/movinet/modeling/movinet_layers.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)    14957 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/projects/movinet/modeling/movinet_layers_test.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     9800 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/projects/movinet/modeling/movinet_model.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     8838 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/projects/movinet/modeling/movinet_model_test.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     7863 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/projects/movinet/modeling/movinet_test.py
+drwxr-x---   0 hongkuny (405338) primarygroup (89939)        0 2022-05-20 04:44:40.708379 tf-models-official-2.9.2/official/projects/movinet/tools/
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)      609 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/projects/movinet/tools/__init__.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     3809 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/projects/movinet/tools/convert_3d_2plus1d.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     1997 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/projects/movinet/tools/convert_3d_2plus1d_test.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)    10999 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/projects/movinet/tools/export_saved_model.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     4451 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/projects/movinet/tools/export_saved_model_test.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)    11994 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/projects/movinet/tools/quantize_movinet.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     3320 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/projects/movinet/train.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     3119 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/projects/movinet/train_test.py
+drwxr-x---   0 hongkuny (405338) primarygroup (89939)        0 2022-05-20 04:44:40.708379 tf-models-official-2.9.2/official/projects/nhnet/
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)      609 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/projects/nhnet/__init__.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     3202 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/projects/nhnet/configs.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     3116 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/projects/nhnet/configs_test.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)    15312 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/projects/nhnet/decoder.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     6024 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/projects/nhnet/decoder_test.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     6091 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/projects/nhnet/evaluation.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     9053 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/projects/nhnet/input_pipeline.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)    23056 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/projects/nhnet/models.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)    11786 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/projects/nhnet/models_test.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     2809 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/projects/nhnet/optimizer.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     3735 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/projects/nhnet/raw_data_process.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     9238 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/projects/nhnet/raw_data_processor.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     8723 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/projects/nhnet/trainer.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     3289 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/projects/nhnet/trainer_test.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     3294 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/projects/nhnet/utils.py
+drwxr-x---   0 hongkuny (405338) primarygroup (89939)        0 2022-05-20 04:44:40.712379 tf-models-official-2.9.2/official/projects/roformer/
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)      610 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/projects/roformer/__init__.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     2002 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/projects/roformer/roformer.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     4462 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/projects/roformer/roformer_attention.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     4133 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/projects/roformer/roformer_attention_test.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)    11208 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/projects/roformer/roformer_encoder.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)    13399 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/projects/roformer/roformer_encoder_block.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)    13069 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/projects/roformer/roformer_encoder_block_test.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     9791 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/projects/roformer/roformer_encoder_test.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     4797 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/projects/roformer/roformer_experiments.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     2566 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/projects/roformer/train.py
+drwxr-x---   0 hongkuny (405338) primarygroup (89939)        0 2022-05-20 04:44:40.712379 tf-models-official-2.9.2/official/projects/teams/
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)      609 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/projects/teams/__init__.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     4010 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/projects/teams/teams.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     4424 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/projects/teams/teams_experiments.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     1272 2022-05-18 02:34:16.000000 tf-models-official-2.9.2/official/projects/teams/teams_experiments_test.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)    18516 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/projects/teams/teams_pretrainer.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     7737 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/projects/teams/teams_pretrainer_test.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)    10170 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/projects/teams/teams_task.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     2184 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/projects/teams/teams_task_test.py
+drwxr-x---   0 hongkuny (405338) primarygroup (89939)        0 2022-05-20 04:44:40.712379 tf-models-official-2.9.2/official/projects/triviaqa/
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)      609 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/projects/triviaqa/__init__.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)    16320 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/projects/triviaqa/dataset.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     2497 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/projects/triviaqa/download_and_prepare.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     1550 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/projects/triviaqa/evaluate.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     5293 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/projects/triviaqa/evaluation.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)    21718 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/projects/triviaqa/inputs.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     4629 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/projects/triviaqa/modeling.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     7087 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/projects/triviaqa/predict.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     2735 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/projects/triviaqa/prediction.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)    18797 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/projects/triviaqa/preprocess.py
+-rwxr-x---   0 hongkuny (405338) primarygroup (89939)    10818 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/projects/triviaqa/sentencepiece_pb2.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)    14287 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/projects/triviaqa/train.py
+drwxr-x---   0 hongkuny (405338) primarygroup (89939)        0 2022-05-20 04:44:40.712379 tf-models-official-2.9.2/official/projects/yt8m/
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)      609 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/projects/yt8m/__init__.py
+drwxr-x---   0 hongkuny (405338) primarygroup (89939)        0 2022-05-20 04:44:40.712379 tf-models-official-2.9.2/official/projects/yt8m/configs/
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)      692 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/projects/yt8m/configs/__init__.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     6378 2022-05-18 02:34:16.000000 tf-models-official-2.9.2/official/projects/yt8m/configs/yt8m.py
+drwxr-x---   0 hongkuny (405338) primarygroup (89939)        0 2022-05-20 04:44:40.712379 tf-models-official-2.9.2/official/projects/yt8m/modeling/
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)      609 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/projects/yt8m/modeling/__init__.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     4632 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/projects/yt8m/modeling/yt8m_agg_models.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     7040 2022-05-18 02:34:16.000000 tf-models-official-2.9.2/official/projects/yt8m/modeling/yt8m_model.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     2150 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/projects/yt8m/modeling/yt8m_model_test.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     8408 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/projects/yt8m/modeling/yt8m_model_utils.py
+drwxr-x---   0 hongkuny (405338) primarygroup (89939)        0 2022-05-20 04:44:40.712379 tf-models-official-2.9.2/official/projects/yt8m/tasks/
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)      692 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/projects/yt8m/tasks/__init__.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)    10969 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/projects/yt8m/tasks/yt8m_task.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)      987 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/projects/yt8m/train.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     3394 2022-05-18 02:34:16.000000 tf-models-official-2.9.2/official/projects/yt8m/train_test.py
+drwxr-x---   0 hongkuny (405338) primarygroup (89939)        0 2022-05-20 04:44:40.712379 tf-models-official-2.9.2/official/recommendation/
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)      609 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/recommendation/__init__.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     2877 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/recommendation/constants.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     4008 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/recommendation/create_ncf_data.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)    37218 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/recommendation/data_pipeline.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)    10308 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/recommendation/data_preprocessing.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)    12821 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/recommendation/data_test.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     9734 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/recommendation/movielens.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)    12278 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/recommendation/ncf_common.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     6964 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/recommendation/ncf_input_pipeline.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)    19840 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/recommendation/ncf_keras_main.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     4134 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/recommendation/ncf_test.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)    16940 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/recommendation/neumf_model.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     1917 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/recommendation/popen_helper.py
+drwxr-x---   0 hongkuny (405338) primarygroup (89939)        0 2022-05-20 04:44:40.712379 tf-models-official-2.9.2/official/recommendation/ranking/
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)      609 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/recommendation/ranking/__init__.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     3988 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/recommendation/ranking/common.py
+drwxr-x---   0 hongkuny (405338) primarygroup (89939)        0 2022-05-20 04:44:40.712379 tf-models-official-2.9.2/official/recommendation/ranking/configs/
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)      609 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/recommendation/ranking/configs/__init__.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)    10418 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/recommendation/ranking/configs/config.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     1464 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/recommendation/ranking/configs/config_test.py
+drwxr-x---   0 hongkuny (405338) primarygroup (89939)        0 2022-05-20 04:44:40.716379 tf-models-official-2.9.2/official/recommendation/ranking/data/
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)      609 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/recommendation/ranking/data/__init__.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     7319 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/recommendation/ranking/data/data_pipeline.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     2335 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/recommendation/ranking/data/data_pipeline_test.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     7689 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/recommendation/ranking/task.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     2182 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/recommendation/ranking/task_test.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     6613 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/recommendation/ranking/train.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     4823 2022-05-18 02:34:16.000000 tf-models-official-2.9.2/official/recommendation/ranking/train_test.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     3076 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/recommendation/stat_utils.py
+drwxr-x---   0 hongkuny (405338) primarygroup (89939)        0 2022-05-20 04:44:40.716379 tf-models-official-2.9.2/official/utils/
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)      609 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/utils/__init__.py
+drwxr-x---   0 hongkuny (405338) primarygroup (89939)        0 2022-05-20 04:44:40.716379 tf-models-official-2.9.2/official/utils/docs/
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)      609 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/utils/docs/__init__.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     3622 2022-05-18 02:34:16.000000 tf-models-official-2.9.2/official/utils/docs/build_all_api_docs.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     1569 2022-05-18 02:34:16.000000 tf-models-official-2.9.2/official/utils/docs/build_all_api_docs_test.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     1928 2022-05-18 02:34:16.000000 tf-models-official-2.9.2/official/utils/docs/build_api_docs_lib.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     3617 2022-05-18 02:34:16.000000 tf-models-official-2.9.2/official/utils/docs/build_nlp_api_docs.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     3576 2022-05-18 02:34:16.000000 tf-models-official-2.9.2/official/utils/docs/build_vision_api_docs.py
+drwxr-x---   0 hongkuny (405338) primarygroup (89939)        0 2022-05-20 04:44:40.716379 tf-models-official-2.9.2/official/utils/flags/
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)      609 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/utils/flags/__init__.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     6395 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/utils/flags/_base.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     4082 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/utils/flags/_benchmark.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     1618 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/utils/flags/_conventions.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     2826 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/utils/flags/_device.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     1694 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/utils/flags/_distribution.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     1541 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/utils/flags/_misc.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)    11566 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/utils/flags/_performance.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     4427 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/utils/flags/core.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     5302 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/utils/flags/flags_test.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     4607 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/utils/hyperparams_flags.py
+drwxr-x---   0 hongkuny (405338) primarygroup (89939)        0 2022-05-20 04:44:40.716379 tf-models-official-2.9.2/official/utils/misc/
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)      609 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/utils/misc/__init__.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     7783 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/utils/misc/keras_utils.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     3360 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/utils/misc/model_helpers.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     4549 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/utils/misc/model_helpers_test.py
+drwxr-x---   0 hongkuny (405338) primarygroup (89939)        0 2022-05-20 04:44:40.716379 tf-models-official-2.9.2/official/utils/testing/
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)      609 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/utils/testing/__init__.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     2220 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/utils/testing/integration.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     3227 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/utils/testing/mock_task.py
+drwxr-x---   0 hongkuny (405338) primarygroup (89939)        0 2022-05-20 04:44:40.716379 tf-models-official-2.9.2/official/vision/
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)      763 2022-05-18 02:34:16.000000 tf-models-official-2.9.2/official/vision/__init__.py
+drwxr-x---   0 hongkuny (405338) primarygroup (89939)        0 2022-05-20 04:44:40.716379 tf-models-official-2.9.2/official/vision/beta/
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)      609 2022-05-19 23:03:19.000000 tf-models-official-2.9.2/official/vision/beta/__init__.py
+drwxr-x---   0 hongkuny (405338) primarygroup (89939)        0 2022-05-20 04:44:40.716379 tf-models-official-2.9.2/official/vision/beta/projects/
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)      609 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/vision/beta/projects/__init__.py
+drwxr-x---   0 hongkuny (405338) primarygroup (89939)        0 2022-05-20 04:44:40.716379 tf-models-official-2.9.2/official/vision/beta/projects/panoptic_maskrcnn/
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     1217 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/vision/beta/projects/panoptic_maskrcnn/__init__.py
+drwxr-x---   0 hongkuny (405338) primarygroup (89939)        0 2022-05-20 04:44:40.716379 tf-models-official-2.9.2/official/vision/beta/projects/panoptic_maskrcnn/configs/
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)      609 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/vision/beta/projects/panoptic_maskrcnn/configs/__init__.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)    10246 2022-05-18 02:34:16.000000 tf-models-official-2.9.2/official/vision/beta/projects/panoptic_maskrcnn/configs/panoptic_maskrcnn.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     1667 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/vision/beta/projects/panoptic_maskrcnn/configs/panoptic_maskrcnn_test.py
+drwxr-x---   0 hongkuny (405338) primarygroup (89939)        0 2022-05-20 04:44:40.716379 tf-models-official-2.9.2/official/vision/beta/projects/panoptic_maskrcnn/tasks/
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)      609 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/vision/beta/projects/panoptic_maskrcnn/tasks/__init__.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)    18150 2022-05-18 02:34:16.000000 tf-models-official-2.9.2/official/vision/beta/projects/panoptic_maskrcnn/tasks/panoptic_maskrcnn.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     2735 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/vision/beta/projects/panoptic_maskrcnn/tasks/panoptic_maskrcnn_test.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     1075 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/vision/beta/projects/panoptic_maskrcnn/train.py
+drwxr-x---   0 hongkuny (405338) primarygroup (89939)        0 2022-05-20 04:44:40.716379 tf-models-official-2.9.2/official/vision/beta/projects/yolo/
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)      609 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/vision/beta/projects/yolo/__init__.py
+drwxr-x---   0 hongkuny (405338) primarygroup (89939)        0 2022-05-20 04:44:40.716379 tf-models-official-2.9.2/official/vision/beta/projects/yolo/common/
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)      609 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/vision/beta/projects/yolo/common/__init__.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     1567 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/vision/beta/projects/yolo/common/registry_imports.py
+drwxr-x---   0 hongkuny (405338) primarygroup (89939)        0 2022-05-20 04:44:40.716379 tf-models-official-2.9.2/official/vision/beta/projects/yolo/configs/
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)      609 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/vision/beta/projects/yolo/configs/__init__.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     1143 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/vision/beta/projects/yolo/configs/backbones.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     2580 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/vision/beta/projects/yolo/configs/darknet_classification.py
+-rwxr-x---   0 hongkuny (405338) primarygroup (89939)     1640 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/vision/beta/projects/yolo/configs/decoders.py
+-rwxr-x---   0 hongkuny (405338) primarygroup (89939)    17638 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/vision/beta/projects/yolo/configs/yolo.py
+drwxr-x---   0 hongkuny (405338) primarygroup (89939)        0 2022-05-20 04:44:40.716379 tf-models-official-2.9.2/official/vision/beta/projects/yolo/dataloaders/
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)      610 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/vision/beta/projects/yolo/dataloaders/__init__.py
+-rwxr-x---   0 hongkuny (405338) primarygroup (89939)     3279 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/vision/beta/projects/yolo/dataloaders/classification_input.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     4810 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/vision/beta/projects/yolo/dataloaders/tf_example_decoder.py
+-rwxr-x---   0 hongkuny (405338) primarygroup (89939)    14697 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/vision/beta/projects/yolo/dataloaders/yolo_input.py
+drwxr-x---   0 hongkuny (405338) primarygroup (89939)        0 2022-05-20 04:44:40.716379 tf-models-official-2.9.2/official/vision/beta/projects/yolo/losses/
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)      609 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/vision/beta/projects/yolo/losses/__init__.py
+-rwxr-x---   0 hongkuny (405338) primarygroup (89939)    31760 2022-05-18 02:34:16.000000 tf-models-official-2.9.2/official/vision/beta/projects/yolo/losses/yolo_loss.py
+-rwxr-x---   0 hongkuny (405338) primarygroup (89939)     3010 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/vision/beta/projects/yolo/losses/yolo_loss_test.py
+drwxr-x---   0 hongkuny (405338) primarygroup (89939)        0 2022-05-20 04:44:40.720379 tf-models-official-2.9.2/official/vision/beta/projects/yolo/ops/
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)      610 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/vision/beta/projects/yolo/ops/__init__.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)    19345 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/vision/beta/projects/yolo/ops/anchor.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)    11205 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/vision/beta/projects/yolo/ops/box_ops.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     2017 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/vision/beta/projects/yolo/ops/box_ops_test.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)    11630 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/vision/beta/projects/yolo/ops/kmeans_anchors.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     1457 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/vision/beta/projects/yolo/ops/kmeans_anchors_test.py
+-rwxr-x---   0 hongkuny (405338) primarygroup (89939)    23506 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/vision/beta/projects/yolo/ops/loss_utils.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     1676 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/vision/beta/projects/yolo/ops/math_ops.py
+-rwxr-x---   0 hongkuny (405338) primarygroup (89939)    16395 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/vision/beta/projects/yolo/ops/mosaic.py
+-rwxr-x---   0 hongkuny (405338) primarygroup (89939)    36261 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/vision/beta/projects/yolo/ops/preprocessing_ops.py
+-rwxr-x---   0 hongkuny (405338) primarygroup (89939)     5480 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/vision/beta/projects/yolo/ops/preprocessing_ops_test.py
+drwxr-x---   0 hongkuny (405338) primarygroup (89939)        0 2022-05-20 04:44:40.720379 tf-models-official-2.9.2/official/vision/beta/projects/yolo/optimization/
+-rwxr-x---   0 hongkuny (405338) primarygroup (89939)     1135 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/vision/beta/projects/yolo/optimization/__init__.py
+drwxr-x---   0 hongkuny (405338) primarygroup (89939)        0 2022-05-20 04:44:40.720379 tf-models-official-2.9.2/official/vision/beta/projects/yolo/optimization/configs/
+-rwxr-x---   0 hongkuny (405338) primarygroup (89939)      609 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/vision/beta/projects/yolo/optimization/configs/__init__.py
+-rwxr-x---   0 hongkuny (405338) primarygroup (89939)     2010 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/vision/beta/projects/yolo/optimization/configs/optimization_config.py
+-rwxr-x---   0 hongkuny (405338) primarygroup (89939)     2283 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/vision/beta/projects/yolo/optimization/configs/optimizer_config.py
+-rwxr-x---   0 hongkuny (405338) primarygroup (89939)     3401 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/vision/beta/projects/yolo/optimization/optimizer_factory.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)    11218 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/vision/beta/projects/yolo/optimization/sgd_torch.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)      998 2022-05-18 02:34:16.000000 tf-models-official-2.9.2/official/vision/beta/projects/yolo/train.py
+drwxr-x---   0 hongkuny (405338) primarygroup (89939)        0 2022-05-20 04:44:40.720379 tf-models-official-2.9.2/official/vision/configs/
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     1045 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/vision/configs/__init__.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     3835 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/vision/configs/backbones.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     3650 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/vision/configs/backbones_3d.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     4342 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/vision/configs/common.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     1916 2022-05-18 02:34:16.000000 tf-models-official-2.9.2/official/vision/configs/decoders.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)    14934 2022-05-18 02:34:16.000000 tf-models-official-2.9.2/official/vision/configs/image_classification.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     1753 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/vision/configs/image_classification_test.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)    18750 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/vision/configs/maskrcnn.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     1722 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/vision/configs/maskrcnn_test.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)    15680 2022-05-18 02:34:16.000000 tf-models-official-2.9.2/official/vision/configs/retinanet.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     1688 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/vision/configs/retinanet_test.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)    27641 2022-05-18 02:34:16.000000 tf-models-official-2.9.2/official/vision/configs/semantic_segmentation.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     1721 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/vision/configs/semantic_segmentation_test.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)    13867 2022-05-18 02:34:16.000000 tf-models-official-2.9.2/official/vision/configs/video_classification.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     1700 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/vision/configs/video_classification_test.py
+drwxr-x---   0 hongkuny (405338) primarygroup (89939)        0 2022-05-20 04:44:40.720379 tf-models-official-2.9.2/official/vision/data/
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)      609 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/vision/data/__init__.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)    22181 2022-05-18 02:34:16.000000 tf-models-official-2.9.2/official/vision/data/create_coco_tf_record.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     6051 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/vision/data/process_coco_few_shot_json_files.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     5951 2022-05-18 02:34:16.000000 tf-models-official-2.9.2/official/vision/data/tfrecord_lib.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     2770 2022-05-18 02:34:16.000000 tf-models-official-2.9.2/official/vision/data/tfrecord_lib_test.py
+drwxr-x---   0 hongkuny (405338) primarygroup (89939)        0 2022-05-20 04:44:40.720379 tf-models-official-2.9.2/official/vision/dataloaders/
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)      609 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/vision/dataloaders/__init__.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)    10713 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/vision/dataloaders/classification_input.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     1032 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/vision/dataloaders/decoder.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     7720 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/vision/dataloaders/input_reader.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     1623 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/vision/dataloaders/input_reader_factory.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)    14269 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/vision/dataloaders/maskrcnn_input.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     2315 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/vision/dataloaders/parser.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)    13706 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/vision/dataloaders/retinanet_input.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     8610 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/vision/dataloaders/segmentation_input.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     7288 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/vision/dataloaders/tf_example_decoder.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)    11548 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/vision/dataloaders/tf_example_decoder_test.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     2588 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/vision/dataloaders/tf_example_label_map_decoder.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     7746 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/vision/dataloaders/tf_example_label_map_decoder_test.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     1242 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/vision/dataloaders/tfds_classification_decoders.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     2272 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/vision/dataloaders/tfds_detection_decoders.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     2568 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/vision/dataloaders/tfds_factory.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     4010 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/vision/dataloaders/tfds_factory_test.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     2418 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/vision/dataloaders/tfds_segmentation_decoders.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)    11261 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/vision/dataloaders/tfexample_utils.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     2543 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/vision/dataloaders/utils.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     2557 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/vision/dataloaders/utils_test.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)    15203 2022-05-18 02:34:16.000000 tf-models-official-2.9.2/official/vision/dataloaders/video_input.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     6657 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/vision/dataloaders/video_input_test.py
+drwxr-x---   0 hongkuny (405338) primarygroup (89939)        0 2022-05-20 04:44:40.724379 tf-models-official-2.9.2/official/vision/evaluation/
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)      609 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/vision/evaluation/__init__.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)    13722 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/vision/evaluation/coco_evaluator.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)    16492 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/vision/evaluation/coco_utils.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     1710 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/vision/evaluation/coco_utils_test.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     4594 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/vision/evaluation/iou.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     3949 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/vision/evaluation/iou_test.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)    12510 2022-05-18 02:34:16.000000 tf-models-official-2.9.2/official/vision/evaluation/panoptic_quality.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     7500 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/vision/evaluation/panoptic_quality_evaluator.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     3323 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/vision/evaluation/panoptic_quality_evaluator_test.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)    11082 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/vision/evaluation/panoptic_quality_test.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     9909 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/vision/evaluation/segmentation_metrics.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     3014 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/vision/evaluation/segmentation_metrics_test.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     6598 2022-05-18 02:34:16.000000 tf-models-official-2.9.2/official/vision/evaluation/wod_detection_evaluator.py
+drwxr-x---   0 hongkuny (405338) primarygroup (89939)        0 2022-05-20 04:44:40.724379 tf-models-official-2.9.2/official/vision/losses/
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)      609 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/vision/losses/__init__.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     3229 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/vision/losses/focal_loss.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     1569 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/vision/losses/loss_utils.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)    13380 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/vision/losses/maskrcnn_losses.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     8097 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/vision/losses/retinanet_losses.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     5259 2022-05-18 02:34:16.000000 tf-models-official-2.9.2/official/vision/losses/segmentation_losses.py
+drwxr-x---   0 hongkuny (405338) primarygroup (89939)        0 2022-05-20 04:44:40.724379 tf-models-official-2.9.2/official/vision/modeling/
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)      825 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/vision/modeling/__init__.py
+drwxr-x---   0 hongkuny (405338) primarygroup (89939)        0 2022-05-20 04:44:40.724379 tf-models-official-2.9.2/official/vision/modeling/backbones/
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     1260 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/vision/modeling/backbones/__init__.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)    12005 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/vision/modeling/backbones/efficientnet.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     3752 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/vision/modeling/backbones/efficientnet_test.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     3494 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/vision/modeling/backbones/factory.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     8383 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/vision/modeling/backbones/factory_test.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)    24886 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/vision/modeling/backbones/mobiledet.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     3794 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/vision/modeling/backbones/mobiledet_test.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)    41069 2022-05-18 02:34:16.000000 tf-models-official-2.9.2/official/vision/modeling/backbones/mobilenet.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)    10596 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/vision/modeling/backbones/mobilenet_test.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)    15932 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/vision/modeling/backbones/resnet.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)    18573 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/vision/modeling/backbones/resnet_3d.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     3789 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/vision/modeling/backbones/resnet_3d_test.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)    14077 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/vision/modeling/backbones/resnet_deeplab.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     5009 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/vision/modeling/backbones/resnet_deeplab_test.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     5503 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/vision/modeling/backbones/resnet_test.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     8840 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/vision/modeling/backbones/revnet.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     3215 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/vision/modeling/backbones/revnet_test.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)    20858 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/vision/modeling/backbones/spinenet.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)    20433 2022-05-18 02:34:16.000000 tf-models-official-2.9.2/official/vision/modeling/backbones/spinenet_mobile.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     3948 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/vision/modeling/backbones/spinenet_mobile_test.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     4308 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/vision/modeling/backbones/spinenet_test.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     4607 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/vision/modeling/classification_model.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     6003 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/vision/modeling/classification_model_test.py
+drwxr-x---   0 hongkuny (405338) primarygroup (89939)        0 2022-05-20 04:44:40.728379 tf-models-official-2.9.2/official/vision/modeling/decoders/
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)      815 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/vision/modeling/decoders/__init__.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     8600 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/vision/modeling/decoders/aspp.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     3001 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/vision/modeling/decoders/aspp_test.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     4387 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/vision/modeling/decoders/factory.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     5621 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/vision/modeling/decoders/factory_test.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     9233 2022-05-18 02:34:16.000000 tf-models-official-2.9.2/official/vision/modeling/decoders/fpn.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     3913 2022-05-18 02:34:16.000000 tf-models-official-2.9.2/official/vision/modeling/decoders/fpn_test.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)    14437 2022-05-18 02:34:16.000000 tf-models-official-2.9.2/official/vision/modeling/decoders/nasfpn.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     1887 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/vision/modeling/decoders/nasfpn_test.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)    16833 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/vision/modeling/factory.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     3530 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/vision/modeling/factory_3d.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     4960 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/vision/modeling/factory_test.py
+drwxr-x---   0 hongkuny (405338) primarygroup (89939)        0 2022-05-20 04:44:40.728379 tf-models-official-2.9.2/official/vision/modeling/heads/
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     1014 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/vision/modeling/heads/__init__.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)    20824 2022-05-18 02:34:16.000000 tf-models-official-2.9.2/official/vision/modeling/heads/dense_prediction_heads.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     4799 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/vision/modeling/heads/dense_prediction_heads_test.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)    18091 2022-05-18 02:34:16.000000 tf-models-official-2.9.2/official/vision/modeling/heads/instance_heads.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     4197 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/vision/modeling/heads/instance_heads_test.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)    18344 2022-05-18 02:34:16.000000 tf-models-official-2.9.2/official/vision/modeling/heads/segmentation_heads.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     3620 2022-05-18 02:34:16.000000 tf-models-official-2.9.2/official/vision/modeling/heads/segmentation_heads_test.py
+drwxr-x---   0 hongkuny (405338) primarygroup (89939)        0 2022-05-20 04:44:40.728379 tf-models-official-2.9.2/official/vision/modeling/layers/
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     2597 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/vision/modeling/layers/__init__.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     3401 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/vision/modeling/layers/box_sampler.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     8279 2022-05-18 02:34:16.000000 tf-models-official-2.9.2/official/vision/modeling/layers/deeplab.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     1935 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/vision/modeling/layers/deeplab_test.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)    45278 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/vision/modeling/layers/detection_generator.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)    10473 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/vision/modeling/layers/detection_generator_test.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     7914 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/vision/modeling/layers/mask_sampler.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)    57663 2022-05-18 02:34:16.000000 tf-models-official-2.9.2/official/vision/modeling/layers/nn_blocks.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)    10353 2022-05-18 02:34:16.000000 tf-models-official-2.9.2/official/vision/modeling/layers/nn_blocks_3d.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     2028 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/vision/modeling/layers/nn_blocks_3d_test.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)    12575 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/vision/modeling/layers/nn_blocks_test.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)    47761 2022-05-18 02:34:16.000000 tf-models-official-2.9.2/official/vision/modeling/layers/nn_layers.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)    12711 2022-05-18 02:34:16.000000 tf-models-official-2.9.2/official/vision/modeling/layers/nn_layers_test.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     2533 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/vision/modeling/layers/roi_aligner.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     1275 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/vision/modeling/layers/roi_aligner_test.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)    14408 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/vision/modeling/layers/roi_generator.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     8270 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/vision/modeling/layers/roi_sampler.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)    17359 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/vision/modeling/maskrcnn_model.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)    14252 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/vision/modeling/maskrcnn_model_test.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     8635 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/vision/modeling/retinanet_model.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)    10976 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/vision/modeling/retinanet_model_test.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     3353 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/vision/modeling/segmentation_model.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     2807 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/vision/modeling/segmentation_model_test.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     4703 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/vision/modeling/video_classification_model.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     3261 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/vision/modeling/video_classification_model_test.py
+drwxr-x---   0 hongkuny (405338) primarygroup (89939)        0 2022-05-20 04:44:40.728379 tf-models-official-2.9.2/official/vision/ops/
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)      609 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/vision/ops/__init__.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)    16891 2022-05-18 02:34:16.000000 tf-models-official-2.9.2/official/vision/ops/anchor.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     7233 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/vision/ops/anchor_generator.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     5286 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/vision/ops/anchor_generator_test.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     7623 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/vision/ops/anchor_test.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)    86454 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/vision/ops/augment.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)    15890 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/vision/ops/augment_test.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     8163 2022-05-18 02:34:16.000000 tf-models-official-2.9.2/official/vision/ops/box_matcher.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     2428 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/vision/ops/box_matcher_test.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)    28961 2022-05-18 02:34:16.000000 tf-models-official-2.9.2/official/vision/ops/box_ops.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     5841 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/vision/ops/iou_similarity.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     1898 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/vision/ops/iou_similarity_test.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     6806 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/vision/ops/mask_ops.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     1677 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/vision/ops/mask_ops_test.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     8099 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/vision/ops/nms.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)    35530 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/vision/ops/preprocess_ops.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)    13283 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/vision/ops/preprocess_ops_3d.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     6822 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/vision/ops/preprocess_ops_3d_test.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     9792 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/vision/ops/preprocess_ops_test.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)    16062 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/vision/ops/sampling_ops.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)    23505 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/vision/ops/spatial_transform_ops.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     3955 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/vision/ops/target_gather.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     2551 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/vision/ops/target_gather_test.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)      843 2022-05-18 02:34:16.000000 tf-models-official-2.9.2/official/vision/registry_imports.py
+drwxr-x---   0 hongkuny (405338) primarygroup (89939)        0 2022-05-20 04:44:40.732379 tf-models-official-2.9.2/official/vision/serving/
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)      702 2022-05-19 22:55:50.000000 tf-models-official-2.9.2/official/vision/serving/__init__.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     8225 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/vision/serving/detection.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     5867 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/vision/serving/detection_test.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     7180 2022-05-18 02:34:16.000000 tf-models-official-2.9.2/official/vision/serving/export_base.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     2731 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/vision/serving/export_base_v2.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     2870 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/vision/serving/export_base_v2_test.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     3539 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/vision/serving/export_module_factory.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     4595 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/vision/serving/export_module_factory_test.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     4039 2022-05-18 02:34:16.000000 tf-models-official-2.9.2/official/vision/serving/export_saved_model.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     6653 2022-05-18 02:34:16.000000 tf-models-official-2.9.2/official/vision/serving/export_saved_model_lib.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     2399 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/vision/serving/export_saved_model_lib_test.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     3358 2022-05-18 02:34:16.000000 tf-models-official-2.9.2/official/vision/serving/export_saved_model_lib_v2.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     3737 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/vision/serving/export_tfhub.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     3979 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/vision/serving/export_tflite.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     4819 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/vision/serving/export_tflite_lib.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     6283 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/vision/serving/export_tflite_lib_test.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     4607 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/vision/serving/export_utils.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     2864 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/vision/serving/image_classification.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     4612 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/vision/serving/image_classification_test.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     3065 2022-05-18 02:34:16.000000 tf-models-official-2.9.2/official/vision/serving/semantic_segmentation.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     4241 2022-05-18 02:34:16.000000 tf-models-official-2.9.2/official/vision/serving/semantic_segmentation_test.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     6979 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/vision/serving/video_classification.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     4222 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/vision/serving/video_classification_test.py
+drwxr-x---   0 hongkuny (405338) primarygroup (89939)        0 2022-05-20 04:44:40.732379 tf-models-official-2.9.2/official/vision/tasks/
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)      895 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/vision/tasks/__init__.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)    11888 2022-05-18 02:34:16.000000 tf-models-official-2.9.2/official/vision/tasks/image_classification.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)    18417 2022-05-18 02:34:16.000000 tf-models-official-2.9.2/official/vision/tasks/maskrcnn.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)    16001 2022-05-18 02:34:16.000000 tf-models-official-2.9.2/official/vision/tasks/retinanet.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)    12853 2022-05-18 02:34:16.000000 tf-models-official-2.9.2/official/vision/tasks/semantic_segmentation.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)    13486 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/vision/tasks/video_classification.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     2598 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/vision/train.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     5725 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/vision/train_spatial_partitioning.py
+drwxr-x---   0 hongkuny (405338) primarygroup (89939)        0 2022-05-20 04:44:40.732379 tf-models-official-2.9.2/official/vision/utils/
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)      609 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/vision/utils/__init__.py
+drwxr-x---   0 hongkuny (405338) primarygroup (89939)        0 2022-05-20 04:44:40.732379 tf-models-official-2.9.2/official/vision/utils/object_detection/
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)      609 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/vision/utils/object_detection/__init__.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     9011 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/vision/utils/object_detection/argmax_matcher.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)    11981 2022-05-18 02:34:16.000000 tf-models-official-2.9.2/official/vision/utils/object_detection/balanced_positive_negative_sampler.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     4776 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/vision/utils/object_detection/box_coder.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     6739 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/vision/utils/object_detection/box_list.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)    41925 2022-05-18 02:34:16.000000 tf-models-official-2.9.2/official/vision/utils/object_detection/box_list_ops.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     3806 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/vision/utils/object_detection/faster_rcnn_box_coder.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     8751 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/vision/utils/object_detection/matcher.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     3074 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/vision/utils/object_detection/minibatch_sampler.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     3212 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/vision/utils/object_detection/ops.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)    20356 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/vision/utils/object_detection/preprocessor.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     4544 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/vision/utils/object_detection/region_similarity_calculator.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     3608 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/vision/utils/object_detection/shape_utils.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)    24198 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/vision/utils/object_detection/target_assigner.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)    28966 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/official/vision/utils/object_detection/visualization_utils.py
+drwxr-x---   0 hongkuny (405338) primarygroup (89939)        0 2022-05-20 04:44:40.732379 tf-models-official-2.9.2/orbit/
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     1092 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/orbit/__init__.py
+drwxr-x---   0 hongkuny (405338) primarygroup (89939)        0 2022-05-20 04:44:40.732379 tf-models-official-2.9.2/orbit/actions/
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     3245 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/orbit/actions/__init__.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     1978 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/orbit/actions/conditional_action.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     1325 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/orbit/actions/conditional_action_test.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     4990 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/orbit/actions/export_saved_model.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     5864 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/orbit/actions/export_saved_model_test.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     8479 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/orbit/actions/new_best_metric.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     4014 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/orbit/actions/new_best_metric_test.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)    21772 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/orbit/controller.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)    28650 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/orbit/controller_test.py
+drwxr-x---   0 hongkuny (405338) primarygroup (89939)        0 2022-05-20 04:44:40.732379 tf-models-official-2.9.2/orbit/examples/
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)      604 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/orbit/examples/__init__.py
+drwxr-x---   0 hongkuny (405338) primarygroup (89939)        0 2022-05-20 04:44:40.736379 tf-models-official-2.9.2/orbit/examples/single_task/
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)      604 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/orbit/examples/single_task/__init__.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     3195 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/orbit/examples/single_task/single_task_evaluator.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     2088 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/orbit/examples/single_task/single_task_evaluator_test.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     5647 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/orbit/examples/single_task/single_task_trainer.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     1961 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/orbit/examples/single_task/single_task_trainer_test.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     3509 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/orbit/runner.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)    17400 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/orbit/standard_runner.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     5100 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/orbit/standard_runner_test.py
+drwxr-x---   0 hongkuny (405338) primarygroup (89939)        0 2022-05-20 04:44:40.736379 tf-models-official-2.9.2/orbit/utils/
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     1144 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/orbit/utils/__init__.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     3913 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/orbit/utils/common.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     1032 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/orbit/utils/common_test.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     2136 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/orbit/utils/epoch_helper.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     8016 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/orbit/utils/loop_fns.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     4177 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/orbit/utils/summary_manager.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     5631 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/orbit/utils/tpu_summaries.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     4513 2022-05-18 02:33:27.000000 tf-models-official-2.9.2/orbit/utils/tpu_summaries_test.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)       38 2022-05-20 04:44:40.736379 tf-models-official-2.9.2/setup.cfg
+drwxr-x---   0 hongkuny (405338) primarygroup (89939)        0 2022-05-20 04:44:40.736379 tf-models-official-2.9.2/tensorflow_models/
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)      909 2022-05-18 02:33:28.000000 tf-models-official-2.9.2/tensorflow_models/__init__.py
+drwxr-x---   0 hongkuny (405338) primarygroup (89939)        0 2022-05-20 04:44:40.736379 tf-models-official-2.9.2/tensorflow_models/nlp/
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)      807 2022-05-18 02:33:28.000000 tf-models-official-2.9.2/tensorflow_models/nlp/__init__.py
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)     1385 2022-05-18 02:33:28.000000 tf-models-official-2.9.2/tensorflow_models/tensorflow_models_test.py
+drwxr-x---   0 hongkuny (405338) primarygroup (89939)        0 2022-05-20 04:44:40.736379 tf-models-official-2.9.2/tensorflow_models/vision/
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)      796 2022-05-19 23:31:57.000000 tf-models-official-2.9.2/tensorflow_models/vision/__init__.py
+drwxr-x---   0 hongkuny (405338) primarygroup (89939)        0 2022-05-20 04:44:40.736379 tf-models-official-2.9.2/tf_models_official.egg-info/
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)      603 2022-05-20 04:44:40.000000 tf-models-official-2.9.2/tf_models_official.egg-info/PKG-INFO
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)    40366 2022-05-20 04:44:40.000000 tf-models-official-2.9.2/tf_models_official.egg-info/SOURCES.txt
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)        1 2022-05-20 04:44:40.000000 tf-models-official-2.9.2/tf_models_official.egg-info/dependency_links.txt
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)      448 2022-05-20 04:44:40.000000 tf-models-official-2.9.2/tf_models_official.egg-info/requires.txt
+-rw-r-----   0 hongkuny (405338) primarygroup (89939)       33 2022-05-20 04:44:40.000000 tf-models-official-2.9.2/tf_models_official.egg-info/top_level.txt
```

### Comparing `tf-models-official-2.9.1/LICENSE` & `tf-models-official-2.9.2/LICENSE`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/PKG-INFO` & `tf-models-official-2.9.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tf-models-official
-Version: 2.9.1
+Version: 2.9.2
 Summary: TensorFlow Official Models
 Home-page: https://github.com/tensorflow/models
 Author: Google Inc.
 Author-email: packages@tensorflow.org
 License: Apache 2.0
 Platform: UNKNOWN
 Requires-Python: >=3.7
```

### Comparing `tf-models-official-2.9.1/README.md` & `tf-models-official-2.9.2/README.md`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/__init__.py` & `tf-models-official-2.9.2/official/__init__.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/common/__init__.py` & `tf-models-official-2.9.2/official/common/__init__.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/common/dataset_fn.py` & `tf-models-official-2.9.2/official/common/dataset_fn.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/common/distribute_utils.py` & `tf-models-official-2.9.2/official/common/distribute_utils.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/common/distribute_utils_test.py` & `tf-models-official-2.9.2/official/common/distribute_utils_test.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/common/flags.py` & `tf-models-official-2.9.2/official/common/flags.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/common/registry_imports.py` & `tf-models-official-2.9.2/official/common/registry_imports.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/common/streamz_counters.py` & `tf-models-official-2.9.2/official/common/streamz_counters.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/core/__init__.py` & `tf-models-official-2.9.2/official/core/__init__.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/core/actions.py` & `tf-models-official-2.9.2/official/core/actions.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/core/actions_test.py` & `tf-models-official-2.9.2/official/core/actions_test.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/core/base_task.py` & `tf-models-official-2.9.2/official/core/base_task.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/core/base_trainer.py` & `tf-models-official-2.9.2/official/core/base_trainer.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/core/base_trainer_test.py` & `tf-models-official-2.9.2/official/core/base_trainer_test.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/core/config_definitions.py` & `tf-models-official-2.9.2/official/core/config_definitions.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/core/exp_factory.py` & `tf-models-official-2.9.2/official/core/exp_factory.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/core/export_base.py` & `tf-models-official-2.9.2/official/core/export_base.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/core/export_base_test.py` & `tf-models-official-2.9.2/official/core/export_base_test.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/core/input_reader.py` & `tf-models-official-2.9.2/official/core/input_reader.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/core/registry.py` & `tf-models-official-2.9.2/official/core/registry.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/core/registry_test.py` & `tf-models-official-2.9.2/official/core/registry_test.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/core/task_factory.py` & `tf-models-official-2.9.2/official/core/task_factory.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/core/test_utils.py` & `tf-models-official-2.9.2/official/core/test_utils.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/core/train_lib.py` & `tf-models-official-2.9.2/official/core/train_lib.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/core/train_lib_test.py` & `tf-models-official-2.9.2/official/core/train_lib_test.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/core/train_utils.py` & `tf-models-official-2.9.2/official/core/train_utils.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/core/train_utils_test.py` & `tf-models-official-2.9.2/official/core/train_utils_test.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/legacy/__init__.py` & `tf-models-official-2.9.2/official/legacy/__init__.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/legacy/albert/__init__.py` & `tf-models-official-2.9.2/official/legacy/albert/__init__.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/legacy/albert/configs.py` & `tf-models-official-2.9.2/official/legacy/albert/configs.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/legacy/bert/__init__.py` & `tf-models-official-2.9.2/official/legacy/bert/__init__.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/legacy/bert/bert_models.py` & `tf-models-official-2.9.2/official/legacy/bert/bert_models.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/legacy/bert/bert_models_test.py` & `tf-models-official-2.9.2/official/legacy/bert/bert_models_test.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/legacy/bert/common_flags.py` & `tf-models-official-2.9.2/official/legacy/bert/common_flags.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/legacy/bert/configs.py` & `tf-models-official-2.9.2/official/legacy/bert/configs.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/legacy/bert/export_tfhub.py` & `tf-models-official-2.9.2/official/legacy/bert/export_tfhub.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/legacy/bert/export_tfhub_test.py` & `tf-models-official-2.9.2/official/legacy/bert/export_tfhub_test.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/legacy/bert/input_pipeline.py` & `tf-models-official-2.9.2/official/legacy/bert/input_pipeline.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/legacy/bert/model_saving_utils.py` & `tf-models-official-2.9.2/official/legacy/bert/model_saving_utils.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/legacy/bert/model_training_utils.py` & `tf-models-official-2.9.2/official/legacy/bert/model_training_utils.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/legacy/bert/model_training_utils_test.py` & `tf-models-official-2.9.2/official/legacy/bert/model_training_utils_test.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/legacy/bert/run_classifier.py` & `tf-models-official-2.9.2/official/legacy/bert/run_classifier.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/legacy/bert/run_pretraining.py` & `tf-models-official-2.9.2/official/legacy/bert/run_pretraining.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/legacy/bert/run_squad.py` & `tf-models-official-2.9.2/official/legacy/bert/run_squad.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/legacy/bert/run_squad_helper.py` & `tf-models-official-2.9.2/official/legacy/bert/run_squad_helper.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/legacy/bert/serving.py` & `tf-models-official-2.9.2/official/legacy/bert/serving.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/legacy/detection/__init__.py` & `tf-models-official-2.9.2/official/legacy/detection/__init__.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/legacy/detection/configs/__init__.py` & `tf-models-official-2.9.2/official/legacy/detection/configs/__init__.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/legacy/detection/configs/base_config.py` & `tf-models-official-2.9.2/official/legacy/detection/configs/base_config.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/legacy/detection/configs/factory.py` & `tf-models-official-2.9.2/official/legacy/detection/configs/factory.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/legacy/detection/configs/maskrcnn_config.py` & `tf-models-official-2.9.2/official/legacy/detection/configs/maskrcnn_config.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/legacy/detection/configs/olnmask_config.py` & `tf-models-official-2.9.2/official/legacy/detection/configs/olnmask_config.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/legacy/detection/configs/retinanet_config.py` & `tf-models-official-2.9.2/official/legacy/detection/configs/retinanet_config.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/legacy/detection/configs/shapemask_config.py` & `tf-models-official-2.9.2/official/legacy/detection/configs/shapemask_config.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/legacy/detection/dataloader/__init__.py` & `tf-models-official-2.9.2/official/legacy/detection/dataloader/__init__.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/legacy/detection/dataloader/anchor.py` & `tf-models-official-2.9.2/official/legacy/detection/dataloader/anchor.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/legacy/detection/dataloader/factory.py` & `tf-models-official-2.9.2/official/legacy/detection/dataloader/factory.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/legacy/detection/dataloader/input_reader.py` & `tf-models-official-2.9.2/official/legacy/detection/dataloader/input_reader.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/legacy/detection/dataloader/maskrcnn_parser.py` & `tf-models-official-2.9.2/official/legacy/detection/dataloader/maskrcnn_parser.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/legacy/detection/dataloader/mode_keys.py` & `tf-models-official-2.9.2/official/legacy/detection/dataloader/mode_keys.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/legacy/detection/dataloader/olnmask_parser.py` & `tf-models-official-2.9.2/official/legacy/detection/dataloader/olnmask_parser.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/legacy/detection/dataloader/retinanet_parser.py` & `tf-models-official-2.9.2/official/legacy/detection/dataloader/retinanet_parser.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/legacy/detection/dataloader/shapemask_parser.py` & `tf-models-official-2.9.2/official/legacy/detection/dataloader/shapemask_parser.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/legacy/detection/dataloader/tf_example_decoder.py` & `tf-models-official-2.9.2/official/legacy/detection/dataloader/tf_example_decoder.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/legacy/detection/evaluation/__init__.py` & `tf-models-official-2.9.2/official/legacy/detection/evaluation/__init__.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/legacy/detection/evaluation/coco_evaluator.py` & `tf-models-official-2.9.2/official/legacy/detection/evaluation/coco_evaluator.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/legacy/detection/evaluation/coco_utils.py` & `tf-models-official-2.9.2/official/legacy/detection/evaluation/coco_utils.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/legacy/detection/evaluation/factory.py` & `tf-models-official-2.9.2/official/legacy/detection/evaluation/factory.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/legacy/detection/executor/__init__.py` & `tf-models-official-2.9.2/official/legacy/detection/executor/__init__.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/legacy/detection/executor/detection_executor.py` & `tf-models-official-2.9.2/official/legacy/detection/executor/detection_executor.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/legacy/detection/executor/distributed_executor.py` & `tf-models-official-2.9.2/official/legacy/detection/executor/distributed_executor.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/legacy/detection/main.py` & `tf-models-official-2.9.2/official/legacy/detection/main.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/legacy/detection/modeling/__init__.py` & `tf-models-official-2.9.2/official/legacy/detection/modeling/__init__.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/legacy/detection/modeling/architecture/__init__.py` & `tf-models-official-2.9.2/official/legacy/detection/modeling/architecture/__init__.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/legacy/detection/modeling/architecture/factory.py` & `tf-models-official-2.9.2/official/legacy/detection/modeling/architecture/factory.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/legacy/detection/modeling/architecture/fpn.py` & `tf-models-official-2.9.2/official/legacy/detection/modeling/architecture/fpn.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/legacy/detection/modeling/architecture/heads.py` & `tf-models-official-2.9.2/official/legacy/detection/modeling/architecture/heads.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/legacy/detection/modeling/architecture/identity.py` & `tf-models-official-2.9.2/official/legacy/detection/modeling/architecture/identity.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/legacy/detection/modeling/architecture/nn_blocks.py` & `tf-models-official-2.9.2/official/legacy/detection/modeling/architecture/nn_blocks.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/legacy/detection/modeling/architecture/nn_ops.py` & `tf-models-official-2.9.2/official/legacy/detection/modeling/architecture/nn_ops.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/legacy/detection/modeling/architecture/resnet.py` & `tf-models-official-2.9.2/official/legacy/detection/modeling/architecture/resnet.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/legacy/detection/modeling/architecture/spinenet.py` & `tf-models-official-2.9.2/official/legacy/detection/modeling/architecture/spinenet.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/legacy/detection/modeling/base_model.py` & `tf-models-official-2.9.2/official/legacy/detection/modeling/base_model.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/legacy/detection/modeling/checkpoint_utils.py` & `tf-models-official-2.9.2/official/legacy/detection/modeling/checkpoint_utils.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/legacy/detection/modeling/factory.py` & `tf-models-official-2.9.2/official/legacy/detection/modeling/factory.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/legacy/detection/modeling/learning_rates.py` & `tf-models-official-2.9.2/official/legacy/detection/modeling/learning_rates.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/legacy/detection/modeling/losses.py` & `tf-models-official-2.9.2/official/legacy/detection/modeling/losses.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/legacy/detection/modeling/maskrcnn_model.py` & `tf-models-official-2.9.2/official/legacy/detection/modeling/maskrcnn_model.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/legacy/detection/modeling/olnmask_model.py` & `tf-models-official-2.9.2/official/legacy/detection/modeling/olnmask_model.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/legacy/detection/modeling/optimizers.py` & `tf-models-official-2.9.2/official/legacy/detection/modeling/optimizers.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/legacy/detection/modeling/retinanet_model.py` & `tf-models-official-2.9.2/official/legacy/detection/modeling/retinanet_model.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/legacy/detection/modeling/shapemask_model.py` & `tf-models-official-2.9.2/official/legacy/detection/modeling/shapemask_model.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/legacy/detection/ops/__init__.py` & `tf-models-official-2.9.2/official/legacy/detection/ops/__init__.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/legacy/detection/ops/nms.py` & `tf-models-official-2.9.2/official/legacy/detection/ops/nms.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/legacy/detection/ops/postprocess_ops.py` & `tf-models-official-2.9.2/official/legacy/detection/ops/postprocess_ops.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/legacy/detection/ops/roi_ops.py` & `tf-models-official-2.9.2/official/legacy/detection/ops/roi_ops.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/legacy/detection/ops/spatial_transform_ops.py` & `tf-models-official-2.9.2/official/legacy/detection/ops/spatial_transform_ops.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/legacy/detection/ops/target_ops.py` & `tf-models-official-2.9.2/official/legacy/detection/ops/target_ops.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/legacy/detection/utils/__init__.py` & `tf-models-official-2.9.2/official/legacy/detection/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/legacy/detection/utils/box_utils.py` & `tf-models-official-2.9.2/official/legacy/detection/utils/box_utils.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/legacy/detection/utils/class_utils.py` & `tf-models-official-2.9.2/official/legacy/detection/utils/class_utils.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/legacy/detection/utils/dataloader_utils.py` & `tf-models-official-2.9.2/official/legacy/detection/utils/dataloader_utils.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/legacy/detection/utils/input_utils.py` & `tf-models-official-2.9.2/official/legacy/detection/utils/input_utils.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/legacy/detection/utils/mask_utils.py` & `tf-models-official-2.9.2/official/legacy/detection/utils/mask_utils.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/legacy/image_classification/__init__.py` & `tf-models-official-2.9.2/official/legacy/image_classification/__init__.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/legacy/image_classification/augment.py` & `tf-models-official-2.9.2/official/legacy/image_classification/augment.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/legacy/image_classification/augment_test.py` & `tf-models-official-2.9.2/official/legacy/image_classification/augment_test.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/legacy/image_classification/callbacks.py` & `tf-models-official-2.9.2/official/legacy/image_classification/callbacks.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/legacy/image_classification/classifier_trainer.py` & `tf-models-official-2.9.2/official/legacy/image_classification/classifier_trainer.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/legacy/image_classification/classifier_trainer_test.py` & `tf-models-official-2.9.2/official/legacy/image_classification/classifier_trainer_test.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/legacy/image_classification/classifier_trainer_util_test.py` & `tf-models-official-2.9.2/official/legacy/image_classification/classifier_trainer_util_test.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/legacy/image_classification/configs/__init__.py` & `tf-models-official-2.9.2/official/legacy/image_classification/configs/__init__.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/legacy/image_classification/configs/base_configs.py` & `tf-models-official-2.9.2/official/legacy/image_classification/configs/base_configs.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/legacy/image_classification/configs/configs.py` & `tf-models-official-2.9.2/official/legacy/image_classification/configs/configs.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/legacy/image_classification/dataset_factory.py` & `tf-models-official-2.9.2/official/legacy/image_classification/dataset_factory.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/legacy/image_classification/efficientnet/__init__.py` & `tf-models-official-2.9.2/official/legacy/image_classification/efficientnet/__init__.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/legacy/image_classification/efficientnet/common_modules.py` & `tf-models-official-2.9.2/official/legacy/image_classification/efficientnet/common_modules.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/legacy/image_classification/efficientnet/efficientnet_config.py` & `tf-models-official-2.9.2/official/legacy/image_classification/efficientnet/efficientnet_config.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/legacy/image_classification/efficientnet/efficientnet_model.py` & `tf-models-official-2.9.2/official/legacy/image_classification/efficientnet/efficientnet_model.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/legacy/image_classification/efficientnet/tfhub_export.py` & `tf-models-official-2.9.2/official/legacy/image_classification/efficientnet/tfhub_export.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/legacy/image_classification/learning_rate.py` & `tf-models-official-2.9.2/official/legacy/image_classification/learning_rate.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/legacy/image_classification/learning_rate_test.py` & `tf-models-official-2.9.2/official/legacy/image_classification/learning_rate_test.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/legacy/image_classification/mnist_main.py` & `tf-models-official-2.9.2/official/legacy/image_classification/mnist_main.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/legacy/image_classification/mnist_test.py` & `tf-models-official-2.9.2/official/legacy/image_classification/mnist_test.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/legacy/image_classification/optimizer_factory.py` & `tf-models-official-2.9.2/official/legacy/image_classification/optimizer_factory.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/legacy/image_classification/optimizer_factory_test.py` & `tf-models-official-2.9.2/official/legacy/image_classification/optimizer_factory_test.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/legacy/image_classification/preprocessing.py` & `tf-models-official-2.9.2/official/legacy/image_classification/preprocessing.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/legacy/image_classification/resnet/__init__.py` & `tf-models-official-2.9.2/official/legacy/image_classification/resnet/__init__.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/legacy/image_classification/resnet/common.py` & `tf-models-official-2.9.2/official/legacy/image_classification/resnet/common.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/legacy/image_classification/resnet/imagenet_preprocessing.py` & `tf-models-official-2.9.2/official/legacy/image_classification/resnet/imagenet_preprocessing.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/legacy/image_classification/resnet/resnet_config.py` & `tf-models-official-2.9.2/official/legacy/image_classification/resnet/resnet_config.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/legacy/image_classification/resnet/resnet_ctl_imagenet_main.py` & `tf-models-official-2.9.2/official/legacy/image_classification/resnet/resnet_ctl_imagenet_main.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/legacy/image_classification/resnet/resnet_model.py` & `tf-models-official-2.9.2/official/legacy/image_classification/resnet/resnet_model.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/legacy/image_classification/resnet/resnet_runnable.py` & `tf-models-official-2.9.2/official/legacy/image_classification/resnet/resnet_runnable.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/legacy/image_classification/resnet/tfhub_export.py` & `tf-models-official-2.9.2/official/legacy/image_classification/resnet/tfhub_export.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/legacy/image_classification/test_utils.py` & `tf-models-official-2.9.2/official/legacy/image_classification/test_utils.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/legacy/image_classification/vgg/__init__.py` & `tf-models-official-2.9.2/official/legacy/image_classification/vgg/__init__.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/legacy/image_classification/vgg/vgg_config.py` & `tf-models-official-2.9.2/official/legacy/image_classification/vgg/vgg_config.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/legacy/image_classification/vgg/vgg_model.py` & `tf-models-official-2.9.2/official/legacy/image_classification/vgg/vgg_model.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/legacy/transformer/__init__.py` & `tf-models-official-2.9.2/official/legacy/transformer/__init__.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/legacy/transformer/attention_layer.py` & `tf-models-official-2.9.2/official/legacy/transformer/attention_layer.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/legacy/transformer/beam_search_v1.py` & `tf-models-official-2.9.2/official/legacy/transformer/beam_search_v1.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/legacy/transformer/compute_bleu.py` & `tf-models-official-2.9.2/official/legacy/transformer/compute_bleu.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/legacy/transformer/compute_bleu_test.py` & `tf-models-official-2.9.2/official/legacy/transformer/compute_bleu_test.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/legacy/transformer/data_download.py` & `tf-models-official-2.9.2/official/legacy/transformer/data_download.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/legacy/transformer/data_pipeline.py` & `tf-models-official-2.9.2/official/legacy/transformer/data_pipeline.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/legacy/transformer/embedding_layer.py` & `tf-models-official-2.9.2/official/legacy/transformer/embedding_layer.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/legacy/transformer/ffn_layer.py` & `tf-models-official-2.9.2/official/legacy/transformer/ffn_layer.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/legacy/transformer/metrics.py` & `tf-models-official-2.9.2/official/legacy/transformer/metrics.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/legacy/transformer/misc.py` & `tf-models-official-2.9.2/official/legacy/transformer/misc.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/legacy/transformer/model_params.py` & `tf-models-official-2.9.2/official/legacy/transformer/model_params.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/legacy/transformer/model_utils.py` & `tf-models-official-2.9.2/official/legacy/transformer/model_utils.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/legacy/transformer/model_utils_test.py` & `tf-models-official-2.9.2/official/legacy/transformer/model_utils_test.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/legacy/transformer/optimizer.py` & `tf-models-official-2.9.2/official/legacy/transformer/optimizer.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/legacy/transformer/transformer.py` & `tf-models-official-2.9.2/official/legacy/transformer/transformer.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/legacy/transformer/transformer_forward_test.py` & `tf-models-official-2.9.2/official/legacy/transformer/transformer_forward_test.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/legacy/transformer/transformer_layers_test.py` & `tf-models-official-2.9.2/official/legacy/transformer/transformer_layers_test.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/legacy/transformer/transformer_main.py` & `tf-models-official-2.9.2/official/legacy/transformer/transformer_main.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/legacy/transformer/transformer_main_test.py` & `tf-models-official-2.9.2/official/legacy/transformer/transformer_main_test.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/legacy/transformer/transformer_test.py` & `tf-models-official-2.9.2/official/legacy/transformer/transformer_test.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/legacy/transformer/translate.py` & `tf-models-official-2.9.2/official/legacy/transformer/translate.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/legacy/transformer/utils/__init__.py` & `tf-models-official-2.9.2/official/legacy/transformer/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/legacy/transformer/utils/metrics.py` & `tf-models-official-2.9.2/official/legacy/transformer/utils/metrics.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/legacy/transformer/utils/tokenizer.py` & `tf-models-official-2.9.2/official/legacy/transformer/utils/tokenizer.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/legacy/transformer/utils/tokenizer_test.py` & `tf-models-official-2.9.2/official/legacy/transformer/utils/tokenizer_test.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/legacy/xlnet/__init__.py` & `tf-models-official-2.9.2/official/legacy/xlnet/__init__.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/legacy/xlnet/classifier_utils.py` & `tf-models-official-2.9.2/official/legacy/xlnet/classifier_utils.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/legacy/xlnet/common_flags.py` & `tf-models-official-2.9.2/official/legacy/xlnet/common_flags.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/legacy/xlnet/data_utils.py` & `tf-models-official-2.9.2/official/legacy/xlnet/data_utils.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/legacy/xlnet/optimization.py` & `tf-models-official-2.9.2/official/legacy/xlnet/optimization.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/legacy/xlnet/preprocess_classification_data.py` & `tf-models-official-2.9.2/official/legacy/xlnet/preprocess_classification_data.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/legacy/xlnet/preprocess_pretrain_data.py` & `tf-models-official-2.9.2/official/legacy/xlnet/preprocess_pretrain_data.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/legacy/xlnet/preprocess_squad_data.py` & `tf-models-official-2.9.2/official/legacy/xlnet/preprocess_squad_data.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/legacy/xlnet/preprocess_utils.py` & `tf-models-official-2.9.2/official/legacy/xlnet/preprocess_utils.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/legacy/xlnet/run_classifier.py` & `tf-models-official-2.9.2/official/legacy/xlnet/run_classifier.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/legacy/xlnet/run_pretrain.py` & `tf-models-official-2.9.2/official/legacy/xlnet/run_pretrain.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/legacy/xlnet/run_squad.py` & `tf-models-official-2.9.2/official/legacy/xlnet/run_squad.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/legacy/xlnet/squad_utils.py` & `tf-models-official-2.9.2/official/legacy/xlnet/squad_utils.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/legacy/xlnet/training_utils.py` & `tf-models-official-2.9.2/official/legacy/xlnet/training_utils.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/legacy/xlnet/xlnet_config.py` & `tf-models-official-2.9.2/official/legacy/xlnet/xlnet_config.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/legacy/xlnet/xlnet_modeling.py` & `tf-models-official-2.9.2/official/legacy/xlnet/xlnet_modeling.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/modeling/__init__.py` & `tf-models-official-2.9.2/official/modeling/__init__.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/modeling/activations/__init__.py` & `tf-models-official-2.9.2/official/modeling/activations/__init__.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/modeling/activations/gelu.py` & `tf-models-official-2.9.2/official/modeling/activations/gelu.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/modeling/activations/gelu_test.py` & `tf-models-official-2.9.2/official/modeling/activations/gelu_test.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/modeling/activations/relu.py` & `tf-models-official-2.9.2/official/modeling/activations/relu.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/modeling/activations/relu_test.py` & `tf-models-official-2.9.2/official/modeling/activations/relu_test.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/modeling/activations/sigmoid.py` & `tf-models-official-2.9.2/official/modeling/activations/sigmoid.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/modeling/activations/sigmoid_test.py` & `tf-models-official-2.9.2/official/modeling/activations/sigmoid_test.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/modeling/activations/swish.py` & `tf-models-official-2.9.2/official/modeling/activations/swish.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/modeling/activations/swish_test.py` & `tf-models-official-2.9.2/official/modeling/activations/swish_test.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/modeling/grad_utils.py` & `tf-models-official-2.9.2/official/modeling/grad_utils.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/modeling/grad_utils_test.py` & `tf-models-official-2.9.2/official/modeling/grad_utils_test.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/modeling/hyperparams/__init__.py` & `tf-models-official-2.9.2/official/modeling/hyperparams/__init__.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/modeling/hyperparams/base_config.py` & `tf-models-official-2.9.2/official/modeling/hyperparams/base_config.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/modeling/hyperparams/base_config_test.py` & `tf-models-official-2.9.2/official/modeling/hyperparams/base_config_test.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/modeling/hyperparams/oneof.py` & `tf-models-official-2.9.2/official/modeling/hyperparams/oneof.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/modeling/hyperparams/oneof_test.py` & `tf-models-official-2.9.2/official/modeling/hyperparams/oneof_test.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/modeling/hyperparams/params_dict.py` & `tf-models-official-2.9.2/official/modeling/hyperparams/params_dict.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/modeling/hyperparams/params_dict_test.py` & `tf-models-official-2.9.2/official/modeling/hyperparams/params_dict_test.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/modeling/multitask/__init__.py` & `tf-models-official-2.9.2/official/modeling/multitask/__init__.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/modeling/multitask/base_model.py` & `tf-models-official-2.9.2/official/modeling/multitask/base_model.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/modeling/multitask/base_trainer.py` & `tf-models-official-2.9.2/official/modeling/multitask/base_trainer.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/modeling/multitask/base_trainer_test.py` & `tf-models-official-2.9.2/official/modeling/multitask/base_trainer_test.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/modeling/multitask/configs.py` & `tf-models-official-2.9.2/official/modeling/multitask/configs.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/modeling/multitask/evaluator.py` & `tf-models-official-2.9.2/official/modeling/multitask/evaluator.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/modeling/multitask/evaluator_test.py` & `tf-models-official-2.9.2/official/modeling/multitask/evaluator_test.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/modeling/multitask/interleaving_trainer.py` & `tf-models-official-2.9.2/official/modeling/multitask/interleaving_trainer.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/modeling/multitask/interleaving_trainer_test.py` & `tf-models-official-2.9.2/official/modeling/multitask/interleaving_trainer_test.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/modeling/multitask/multitask.py` & `tf-models-official-2.9.2/official/modeling/multitask/multitask.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/modeling/multitask/task_sampler.py` & `tf-models-official-2.9.2/official/modeling/multitask/task_sampler.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/modeling/multitask/task_sampler_test.py` & `tf-models-official-2.9.2/official/modeling/multitask/task_sampler_test.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/modeling/multitask/test_utils.py` & `tf-models-official-2.9.2/official/modeling/multitask/test_utils.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/modeling/multitask/train_lib.py` & `tf-models-official-2.9.2/official/modeling/multitask/train_lib.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/modeling/multitask/train_lib_test.py` & `tf-models-official-2.9.2/official/modeling/multitask/train_lib_test.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/modeling/optimization/__init__.py` & `tf-models-official-2.9.2/official/modeling/optimization/__init__.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/modeling/optimization/adafactor_optimizer.py` & `tf-models-official-2.9.2/official/modeling/optimization/adafactor_optimizer.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/modeling/optimization/configs/__init__.py` & `tf-models-official-2.9.2/official/modeling/optimization/configs/__init__.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/modeling/optimization/configs/learning_rate_config.py` & `tf-models-official-2.9.2/official/modeling/optimization/configs/learning_rate_config.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/modeling/optimization/configs/optimization_config.py` & `tf-models-official-2.9.2/official/modeling/optimization/configs/optimization_config.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/modeling/optimization/configs/optimization_config_test.py` & `tf-models-official-2.9.2/official/modeling/optimization/configs/optimization_config_test.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/modeling/optimization/configs/optimizer_config.py` & `tf-models-official-2.9.2/official/modeling/optimization/configs/optimizer_config.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/modeling/optimization/ema_optimizer.py` & `tf-models-official-2.9.2/official/modeling/optimization/ema_optimizer.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/modeling/optimization/lars_optimizer.py` & `tf-models-official-2.9.2/official/modeling/optimization/lars_optimizer.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/modeling/optimization/lr_schedule.py` & `tf-models-official-2.9.2/official/modeling/optimization/lr_schedule.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/modeling/optimization/lr_schedule_test.py` & `tf-models-official-2.9.2/official/modeling/optimization/lr_schedule_test.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/modeling/optimization/optimizer_factory.py` & `tf-models-official-2.9.2/official/modeling/optimization/optimizer_factory.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/modeling/optimization/optimizer_factory_test.py` & `tf-models-official-2.9.2/official/modeling/optimization/optimizer_factory_test.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/modeling/optimization/slide_optimizer.py` & `tf-models-official-2.9.2/official/modeling/optimization/slide_optimizer.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/modeling/performance.py` & `tf-models-official-2.9.2/official/modeling/performance.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/modeling/privacy/__init__.py` & `tf-models-official-2.9.2/official/modeling/privacy/__init__.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/modeling/privacy/configs.py` & `tf-models-official-2.9.2/official/modeling/privacy/configs.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/modeling/privacy/configs_test.py` & `tf-models-official-2.9.2/official/modeling/privacy/configs_test.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/modeling/privacy/ops.py` & `tf-models-official-2.9.2/official/modeling/privacy/ops.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/modeling/privacy/ops_test.py` & `tf-models-official-2.9.2/official/modeling/privacy/ops_test.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/modeling/tf_utils.py` & `tf-models-official-2.9.2/official/modeling/tf_utils.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/modeling/tf_utils_test.py` & `tf-models-official-2.9.2/official/modeling/tf_utils_test.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/nlp/__init__.py` & `tf-models-official-2.9.2/official/nlp/__init__.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/nlp/configs/__init__.py` & `tf-models-official-2.9.2/official/nlp/configs/__init__.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/nlp/configs/bert.py` & `tf-models-official-2.9.2/official/nlp/configs/bert.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/nlp/configs/electra.py` & `tf-models-official-2.9.2/official/nlp/configs/electra.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/nlp/configs/encoders.py` & `tf-models-official-2.9.2/official/nlp/configs/encoders.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/nlp/configs/encoders_test.py` & `tf-models-official-2.9.2/official/nlp/configs/encoders_test.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/nlp/configs/experiment_configs.py` & `tf-models-official-2.9.2/official/nlp/configs/experiment_configs.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/nlp/configs/finetuning_experiments.py` & `tf-models-official-2.9.2/official/nlp/configs/finetuning_experiments.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/nlp/configs/pretraining_experiments.py` & `tf-models-official-2.9.2/official/nlp/configs/pretraining_experiments.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/nlp/configs/wmt_transformer_experiments.py` & `tf-models-official-2.9.2/official/nlp/configs/wmt_transformer_experiments.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/nlp/continuous_finetune_lib.py` & `tf-models-official-2.9.2/official/nlp/continuous_finetune_lib.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/nlp/continuous_finetune_lib_test.py` & `tf-models-official-2.9.2/official/nlp/continuous_finetune_lib_test.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/nlp/data/__init__.py` & `tf-models-official-2.9.2/official/nlp/data/__init__.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/nlp/data/classifier_data_lib.py` & `tf-models-official-2.9.2/official/nlp/data/classifier_data_lib.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/nlp/data/classifier_data_lib_test.py` & `tf-models-official-2.9.2/official/nlp/data/classifier_data_lib_test.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/nlp/data/create_finetuning_data.py` & `tf-models-official-2.9.2/official/nlp/data/create_finetuning_data.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/nlp/data/create_pretraining_data.py` & `tf-models-official-2.9.2/official/nlp/data/create_pretraining_data.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/nlp/data/create_pretraining_data_test.py` & `tf-models-official-2.9.2/official/nlp/data/create_pretraining_data_test.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/nlp/data/create_xlnet_pretraining_data.py` & `tf-models-official-2.9.2/official/nlp/data/create_xlnet_pretraining_data.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/nlp/data/create_xlnet_pretraining_data_test.py` & `tf-models-official-2.9.2/official/nlp/data/create_xlnet_pretraining_data_test.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/nlp/data/data_loader.py` & `tf-models-official-2.9.2/official/nlp/data/data_loader.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/nlp/data/data_loader_factory.py` & `tf-models-official-2.9.2/official/nlp/data/data_loader_factory.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/nlp/data/data_loader_factory_test.py` & `tf-models-official-2.9.2/official/nlp/data/data_loader_factory_test.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/nlp/data/dual_encoder_dataloader.py` & `tf-models-official-2.9.2/official/nlp/data/dual_encoder_dataloader.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/nlp/data/dual_encoder_dataloader_test.py` & `tf-models-official-2.9.2/official/nlp/data/dual_encoder_dataloader_test.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/nlp/data/pretrain_dataloader.py` & `tf-models-official-2.9.2/official/nlp/data/pretrain_dataloader.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/nlp/data/pretrain_dataloader_test.py` & `tf-models-official-2.9.2/official/nlp/data/pretrain_dataloader_test.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/nlp/data/pretrain_dynamic_dataloader.py` & `tf-models-official-2.9.2/official/nlp/data/pretrain_dynamic_dataloader.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/nlp/data/pretrain_dynamic_dataloader_test.py` & `tf-models-official-2.9.2/official/nlp/data/pretrain_dynamic_dataloader_test.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/nlp/data/question_answering_dataloader.py` & `tf-models-official-2.9.2/official/nlp/data/question_answering_dataloader.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/nlp/data/question_answering_dataloader_test.py` & `tf-models-official-2.9.2/official/nlp/data/question_answering_dataloader_test.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/nlp/data/sentence_prediction_dataloader.py` & `tf-models-official-2.9.2/official/nlp/data/sentence_prediction_dataloader.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/nlp/data/sentence_prediction_dataloader_test.py` & `tf-models-official-2.9.2/official/nlp/data/sentence_prediction_dataloader_test.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/nlp/data/sentence_retrieval_lib.py` & `tf-models-official-2.9.2/official/nlp/data/sentence_retrieval_lib.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/nlp/data/squad_lib.py` & `tf-models-official-2.9.2/official/nlp/data/squad_lib.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/nlp/data/squad_lib_sp.py` & `tf-models-official-2.9.2/official/nlp/data/squad_lib_sp.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/nlp/data/tagging_data_lib.py` & `tf-models-official-2.9.2/official/nlp/data/tagging_data_lib.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/nlp/data/tagging_data_lib_test.py` & `tf-models-official-2.9.2/official/nlp/data/tagging_data_lib_test.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/nlp/data/tagging_dataloader.py` & `tf-models-official-2.9.2/official/nlp/data/tagging_dataloader.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/nlp/data/tagging_dataloader_test.py` & `tf-models-official-2.9.2/official/nlp/data/tagging_dataloader_test.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/nlp/data/train_sentencepiece.py` & `tf-models-official-2.9.2/official/nlp/data/train_sentencepiece.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/nlp/data/wmt_dataloader.py` & `tf-models-official-2.9.2/official/nlp/data/wmt_dataloader.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/nlp/data/wmt_dataloader_test.py` & `tf-models-official-2.9.2/official/nlp/data/wmt_dataloader_test.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/nlp/metrics/__init__.py` & `tf-models-official-2.9.2/official/nlp/metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/nlp/metrics/bleu.py` & `tf-models-official-2.9.2/official/nlp/metrics/bleu.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/nlp/metrics/bleu_test.py` & `tf-models-official-2.9.2/official/nlp/metrics/bleu_test.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/nlp/modeling/__init__.py` & `tf-models-official-2.9.2/official/nlp/modeling/__init__.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/nlp/modeling/layers/__init__.py` & `tf-models-official-2.9.2/official/nlp/modeling/layers/__init__.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/nlp/modeling/layers/attention.py` & `tf-models-official-2.9.2/official/nlp/modeling/layers/attention.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/nlp/modeling/layers/attention_test.py` & `tf-models-official-2.9.2/official/nlp/modeling/layers/attention_test.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/nlp/modeling/layers/bigbird_attention.py` & `tf-models-official-2.9.2/official/nlp/modeling/layers/bigbird_attention.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/nlp/modeling/layers/bigbird_attention_test.py` & `tf-models-official-2.9.2/official/nlp/modeling/layers/bigbird_attention_test.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/nlp/modeling/layers/block_diag_feedforward.py` & `tf-models-official-2.9.2/official/nlp/modeling/layers/block_diag_feedforward.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/nlp/modeling/layers/block_diag_feedforward_test.py` & `tf-models-official-2.9.2/official/nlp/modeling/layers/block_diag_feedforward_test.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/nlp/modeling/layers/cls_head.py` & `tf-models-official-2.9.2/official/nlp/modeling/layers/cls_head.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/nlp/modeling/layers/cls_head_test.py` & `tf-models-official-2.9.2/official/nlp/modeling/layers/cls_head_test.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/nlp/modeling/layers/gated_feedforward.py` & `tf-models-official-2.9.2/official/nlp/modeling/layers/gated_feedforward.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/nlp/modeling/layers/gated_feedforward_test.py` & `tf-models-official-2.9.2/official/nlp/modeling/layers/gated_feedforward_test.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/nlp/modeling/layers/gaussian_process.py` & `tf-models-official-2.9.2/official/nlp/modeling/layers/gaussian_process.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/nlp/modeling/layers/gaussian_process_test.py` & `tf-models-official-2.9.2/official/nlp/modeling/layers/gaussian_process_test.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/nlp/modeling/layers/kernel_attention.py` & `tf-models-official-2.9.2/official/nlp/modeling/layers/kernel_attention.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/nlp/modeling/layers/kernel_attention_test.py` & `tf-models-official-2.9.2/official/nlp/modeling/layers/kernel_attention_test.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/nlp/modeling/layers/masked_lm.py` & `tf-models-official-2.9.2/official/nlp/modeling/layers/masked_lm.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/nlp/modeling/layers/masked_lm_test.py` & `tf-models-official-2.9.2/official/nlp/modeling/layers/masked_lm_test.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/nlp/modeling/layers/masked_softmax.py` & `tf-models-official-2.9.2/official/nlp/modeling/layers/masked_softmax.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/nlp/modeling/layers/masked_softmax_test.py` & `tf-models-official-2.9.2/official/nlp/modeling/layers/masked_softmax_test.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/nlp/modeling/layers/mat_mul_with_margin.py` & `tf-models-official-2.9.2/official/nlp/modeling/layers/mat_mul_with_margin.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/nlp/modeling/layers/mat_mul_with_margin_test.py` & `tf-models-official-2.9.2/official/nlp/modeling/layers/mat_mul_with_margin_test.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/nlp/modeling/layers/mobile_bert_layers.py` & `tf-models-official-2.9.2/official/nlp/modeling/layers/mobile_bert_layers.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/nlp/modeling/layers/mobile_bert_layers_test.py` & `tf-models-official-2.9.2/official/nlp/modeling/layers/mobile_bert_layers_test.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/nlp/modeling/layers/multi_channel_attention.py` & `tf-models-official-2.9.2/official/nlp/modeling/layers/multi_channel_attention.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/nlp/modeling/layers/multi_channel_attention_test.py` & `tf-models-official-2.9.2/official/nlp/modeling/layers/multi_channel_attention_test.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/nlp/modeling/layers/on_device_embedding.py` & `tf-models-official-2.9.2/official/nlp/modeling/layers/on_device_embedding.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/nlp/modeling/layers/on_device_embedding_test.py` & `tf-models-official-2.9.2/official/nlp/modeling/layers/on_device_embedding_test.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/nlp/modeling/layers/position_embedding.py` & `tf-models-official-2.9.2/official/nlp/modeling/layers/position_embedding.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/nlp/modeling/layers/position_embedding_test.py` & `tf-models-official-2.9.2/official/nlp/modeling/layers/position_embedding_test.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/nlp/modeling/layers/relative_attention.py` & `tf-models-official-2.9.2/official/nlp/modeling/layers/relative_attention.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/nlp/modeling/layers/relative_attention_test.py` & `tf-models-official-2.9.2/official/nlp/modeling/layers/relative_attention_test.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/nlp/modeling/layers/reuse_attention.py` & `tf-models-official-2.9.2/official/nlp/modeling/layers/reuse_attention.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/nlp/modeling/layers/reuse_attention_test.py` & `tf-models-official-2.9.2/official/nlp/modeling/layers/reuse_attention_test.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/nlp/modeling/layers/reuse_transformer.py` & `tf-models-official-2.9.2/official/nlp/modeling/layers/reuse_transformer.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/nlp/modeling/layers/reuse_transformer_test.py` & `tf-models-official-2.9.2/official/nlp/modeling/layers/reuse_transformer_test.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/nlp/modeling/layers/rezero_transformer.py` & `tf-models-official-2.9.2/official/nlp/modeling/layers/rezero_transformer.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/nlp/modeling/layers/rezero_transformer_test.py` & `tf-models-official-2.9.2/official/nlp/modeling/layers/rezero_transformer_test.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/nlp/modeling/layers/routing.py` & `tf-models-official-2.9.2/official/nlp/modeling/layers/routing.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/nlp/modeling/layers/routing_test.py` & `tf-models-official-2.9.2/official/nlp/modeling/layers/routing_test.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/nlp/modeling/layers/self_attention_mask.py` & `tf-models-official-2.9.2/official/nlp/modeling/layers/self_attention_mask.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/nlp/modeling/layers/spectral_normalization.py` & `tf-models-official-2.9.2/official/nlp/modeling/layers/spectral_normalization.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/nlp/modeling/layers/spectral_normalization_test.py` & `tf-models-official-2.9.2/official/nlp/modeling/layers/spectral_normalization_test.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/nlp/modeling/layers/talking_heads_attention.py` & `tf-models-official-2.9.2/official/nlp/modeling/layers/talking_heads_attention.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/nlp/modeling/layers/talking_heads_attention_test.py` & `tf-models-official-2.9.2/official/nlp/modeling/layers/talking_heads_attention_test.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/nlp/modeling/layers/text_layers.py` & `tf-models-official-2.9.2/official/nlp/modeling/layers/text_layers.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/nlp/modeling/layers/text_layers_test.py` & `tf-models-official-2.9.2/official/nlp/modeling/layers/text_layers_test.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/nlp/modeling/layers/tn_expand_condense.py` & `tf-models-official-2.9.2/official/nlp/modeling/layers/tn_expand_condense.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/nlp/modeling/layers/tn_expand_condense_test.py` & `tf-models-official-2.9.2/official/nlp/modeling/layers/tn_expand_condense_test.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/nlp/modeling/layers/tn_transformer_expand_condense.py` & `tf-models-official-2.9.2/official/nlp/modeling/layers/tn_transformer_expand_condense.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/nlp/modeling/layers/tn_transformer_test.py` & `tf-models-official-2.9.2/official/nlp/modeling/layers/tn_transformer_test.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/nlp/modeling/layers/transformer.py` & `tf-models-official-2.9.2/official/nlp/modeling/layers/transformer.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/nlp/modeling/layers/transformer_encoder_block.py` & `tf-models-official-2.9.2/official/nlp/modeling/layers/transformer_encoder_block.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/nlp/modeling/layers/transformer_encoder_block_test.py` & `tf-models-official-2.9.2/official/nlp/modeling/layers/transformer_encoder_block_test.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/nlp/modeling/layers/transformer_scaffold.py` & `tf-models-official-2.9.2/official/nlp/modeling/layers/transformer_scaffold.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/nlp/modeling/layers/transformer_scaffold_test.py` & `tf-models-official-2.9.2/official/nlp/modeling/layers/transformer_scaffold_test.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/nlp/modeling/layers/transformer_test.py` & `tf-models-official-2.9.2/official/nlp/modeling/layers/transformer_test.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/nlp/modeling/layers/transformer_xl.py` & `tf-models-official-2.9.2/official/nlp/modeling/layers/transformer_xl.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/nlp/modeling/layers/transformer_xl_test.py` & `tf-models-official-2.9.2/official/nlp/modeling/layers/transformer_xl_test.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/nlp/modeling/layers/util.py` & `tf-models-official-2.9.2/official/nlp/modeling/layers/util.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/nlp/modeling/losses/__init__.py` & `tf-models-official-2.9.2/official/nlp/modeling/losses/__init__.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/nlp/modeling/losses/weighted_sparse_categorical_crossentropy.py` & `tf-models-official-2.9.2/official/nlp/modeling/losses/weighted_sparse_categorical_crossentropy.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/nlp/modeling/losses/weighted_sparse_categorical_crossentropy_test.py` & `tf-models-official-2.9.2/official/nlp/modeling/losses/weighted_sparse_categorical_crossentropy_test.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/nlp/modeling/models/__init__.py` & `tf-models-official-2.9.2/official/nlp/modeling/models/__init__.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/nlp/modeling/models/bert_classifier.py` & `tf-models-official-2.9.2/official/nlp/modeling/models/bert_classifier.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/nlp/modeling/models/bert_classifier_test.py` & `tf-models-official-2.9.2/official/nlp/modeling/models/bert_classifier_test.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/nlp/modeling/models/bert_pretrainer.py` & `tf-models-official-2.9.2/official/nlp/modeling/models/bert_pretrainer.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/nlp/modeling/models/bert_pretrainer_test.py` & `tf-models-official-2.9.2/official/nlp/modeling/models/bert_pretrainer_test.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/nlp/modeling/models/bert_span_labeler.py` & `tf-models-official-2.9.2/official/nlp/modeling/models/bert_span_labeler.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/nlp/modeling/models/bert_span_labeler_test.py` & `tf-models-official-2.9.2/official/nlp/modeling/models/bert_span_labeler_test.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/nlp/modeling/models/bert_token_classifier.py` & `tf-models-official-2.9.2/official/nlp/modeling/models/bert_token_classifier.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/nlp/modeling/models/bert_token_classifier_test.py` & `tf-models-official-2.9.2/official/nlp/modeling/models/bert_token_classifier_test.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/nlp/modeling/models/dual_encoder.py` & `tf-models-official-2.9.2/official/nlp/modeling/models/dual_encoder.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/nlp/modeling/models/dual_encoder_test.py` & `tf-models-official-2.9.2/official/nlp/modeling/models/dual_encoder_test.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/nlp/modeling/models/electra_pretrainer.py` & `tf-models-official-2.9.2/official/nlp/modeling/models/electra_pretrainer.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/nlp/modeling/models/electra_pretrainer_test.py` & `tf-models-official-2.9.2/official/nlp/modeling/models/electra_pretrainer_test.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/nlp/modeling/models/seq2seq_transformer.py` & `tf-models-official-2.9.2/official/nlp/modeling/models/seq2seq_transformer.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/nlp/modeling/models/seq2seq_transformer_test.py` & `tf-models-official-2.9.2/official/nlp/modeling/models/seq2seq_transformer_test.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/nlp/modeling/models/t5.py` & `tf-models-official-2.9.2/official/nlp/modeling/models/t5.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/nlp/modeling/models/t5_test.py` & `tf-models-official-2.9.2/official/nlp/modeling/models/t5_test.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/nlp/modeling/models/xlnet.py` & `tf-models-official-2.9.2/official/nlp/modeling/models/xlnet.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/nlp/modeling/models/xlnet_test.py` & `tf-models-official-2.9.2/official/nlp/modeling/models/xlnet_test.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/nlp/modeling/networks/__init__.py` & `tf-models-official-2.9.2/official/nlp/modeling/networks/__init__.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/nlp/modeling/networks/albert_encoder.py` & `tf-models-official-2.9.2/official/nlp/modeling/networks/albert_encoder.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/nlp/modeling/networks/albert_encoder_test.py` & `tf-models-official-2.9.2/official/nlp/modeling/networks/albert_encoder_test.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/nlp/modeling/networks/bert_dense_encoder_test.py` & `tf-models-official-2.9.2/official/nlp/modeling/networks/bert_dense_encoder_test.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/nlp/modeling/networks/bert_encoder.py` & `tf-models-official-2.9.2/official/nlp/modeling/networks/bert_encoder.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/nlp/modeling/networks/bert_encoder_test.py` & `tf-models-official-2.9.2/official/nlp/modeling/networks/bert_encoder_test.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/nlp/modeling/networks/classification.py` & `tf-models-official-2.9.2/official/nlp/modeling/networks/classification.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/nlp/modeling/networks/classification_test.py` & `tf-models-official-2.9.2/official/nlp/modeling/networks/classification_test.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/nlp/modeling/networks/encoder_scaffold.py` & `tf-models-official-2.9.2/official/nlp/modeling/networks/encoder_scaffold.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/nlp/modeling/networks/encoder_scaffold_test.py` & `tf-models-official-2.9.2/official/nlp/modeling/networks/encoder_scaffold_test.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/nlp/modeling/networks/funnel_transformer.py` & `tf-models-official-2.9.2/official/nlp/modeling/networks/funnel_transformer.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/nlp/modeling/networks/funnel_transformer_test.py` & `tf-models-official-2.9.2/official/nlp/modeling/networks/funnel_transformer_test.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/nlp/modeling/networks/mobile_bert_encoder.py` & `tf-models-official-2.9.2/official/nlp/modeling/networks/mobile_bert_encoder.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/nlp/modeling/networks/mobile_bert_encoder_test.py` & `tf-models-official-2.9.2/official/nlp/modeling/networks/mobile_bert_encoder_test.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/nlp/modeling/networks/packed_sequence_embedding.py` & `tf-models-official-2.9.2/official/nlp/modeling/networks/packed_sequence_embedding.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/nlp/modeling/networks/packed_sequence_embedding_test.py` & `tf-models-official-2.9.2/official/nlp/modeling/networks/packed_sequence_embedding_test.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/nlp/modeling/networks/span_labeling.py` & `tf-models-official-2.9.2/official/nlp/modeling/networks/span_labeling.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/nlp/modeling/networks/span_labeling_test.py` & `tf-models-official-2.9.2/official/nlp/modeling/networks/span_labeling_test.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/nlp/modeling/networks/xlnet_base.py` & `tf-models-official-2.9.2/official/nlp/modeling/networks/xlnet_base.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/nlp/modeling/networks/xlnet_base_test.py` & `tf-models-official-2.9.2/official/nlp/modeling/networks/xlnet_base_test.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/nlp/modeling/ops/__init__.py` & `tf-models-official-2.9.2/official/nlp/modeling/ops/__init__.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/nlp/modeling/ops/beam_search.py` & `tf-models-official-2.9.2/official/nlp/modeling/ops/beam_search.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/nlp/modeling/ops/beam_search_test.py` & `tf-models-official-2.9.2/official/nlp/modeling/ops/beam_search_test.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/nlp/modeling/ops/decoding_module.py` & `tf-models-official-2.9.2/official/nlp/modeling/ops/decoding_module.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/nlp/modeling/ops/decoding_module_test.py` & `tf-models-official-2.9.2/official/nlp/modeling/ops/decoding_module_test.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/nlp/modeling/ops/sampling_module.py` & `tf-models-official-2.9.2/official/nlp/modeling/ops/sampling_module.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/nlp/modeling/ops/segment_extractor.py` & `tf-models-official-2.9.2/official/nlp/modeling/ops/segment_extractor.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/nlp/modeling/ops/segment_extractor_test.py` & `tf-models-official-2.9.2/official/nlp/modeling/ops/segment_extractor_test.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/nlp/optimization.py` & `tf-models-official-2.9.2/official/nlp/optimization.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/nlp/serving/__init__.py` & `tf-models-official-2.9.2/official/nlp/serving/__init__.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/nlp/serving/export_savedmodel.py` & `tf-models-official-2.9.2/official/nlp/serving/export_savedmodel.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/nlp/serving/export_savedmodel_test.py` & `tf-models-official-2.9.2/official/nlp/serving/export_savedmodel_test.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/nlp/serving/export_savedmodel_util.py` & `tf-models-official-2.9.2/official/nlp/serving/export_savedmodel_util.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/nlp/serving/serving_modules.py` & `tf-models-official-2.9.2/official/nlp/serving/serving_modules.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/nlp/serving/serving_modules_test.py` & `tf-models-official-2.9.2/official/nlp/serving/serving_modules_test.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/nlp/tasks/__init__.py` & `tf-models-official-2.9.2/official/nlp/tasks/__init__.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/nlp/tasks/dual_encoder.py` & `tf-models-official-2.9.2/official/nlp/tasks/dual_encoder.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/nlp/tasks/dual_encoder_test.py` & `tf-models-official-2.9.2/official/nlp/tasks/dual_encoder_test.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/nlp/tasks/electra_task.py` & `tf-models-official-2.9.2/official/nlp/tasks/electra_task.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/nlp/tasks/electra_task_test.py` & `tf-models-official-2.9.2/official/nlp/tasks/electra_task_test.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/nlp/tasks/masked_lm.py` & `tf-models-official-2.9.2/official/nlp/tasks/masked_lm.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/nlp/tasks/masked_lm_test.py` & `tf-models-official-2.9.2/official/nlp/tasks/masked_lm_test.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/nlp/tasks/question_answering.py` & `tf-models-official-2.9.2/official/nlp/tasks/question_answering.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/nlp/tasks/question_answering_test.py` & `tf-models-official-2.9.2/official/nlp/tasks/question_answering_test.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/nlp/tasks/sentence_prediction.py` & `tf-models-official-2.9.2/official/nlp/tasks/sentence_prediction.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/nlp/tasks/sentence_prediction_test.py` & `tf-models-official-2.9.2/official/nlp/tasks/sentence_prediction_test.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/nlp/tasks/tagging.py` & `tf-models-official-2.9.2/official/nlp/tasks/tagging.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/nlp/tasks/tagging_test.py` & `tf-models-official-2.9.2/official/nlp/tasks/tagging_test.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/nlp/tasks/translation.py` & `tf-models-official-2.9.2/official/nlp/tasks/translation.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/nlp/tasks/translation_test.py` & `tf-models-official-2.9.2/official/nlp/tasks/translation_test.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/nlp/tasks/utils.py` & `tf-models-official-2.9.2/official/nlp/tasks/utils.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/nlp/tools/__init__.py` & `tf-models-official-2.9.2/official/nlp/tools/__init__.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/nlp/tools/export_tfhub.py` & `tf-models-official-2.9.2/official/nlp/tools/export_tfhub.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/nlp/tools/export_tfhub_lib.py` & `tf-models-official-2.9.2/official/nlp/tools/export_tfhub_lib.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/nlp/tools/export_tfhub_lib_test.py` & `tf-models-official-2.9.2/official/nlp/tools/export_tfhub_lib_test.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/nlp/tools/squad_evaluate_v1_1.py` & `tf-models-official-2.9.2/official/nlp/tools/squad_evaluate_v1_1.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/nlp/tools/squad_evaluate_v2_0.py` & `tf-models-official-2.9.2/official/nlp/tools/squad_evaluate_v2_0.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/nlp/tools/tf1_bert_checkpoint_converter_lib.py` & `tf-models-official-2.9.2/official/nlp/tools/tf1_bert_checkpoint_converter_lib.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/nlp/tools/tf2_albert_encoder_checkpoint_converter.py` & `tf-models-official-2.9.2/official/nlp/tools/tf2_albert_encoder_checkpoint_converter.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/nlp/tools/tf2_bert_encoder_checkpoint_converter.py` & `tf-models-official-2.9.2/official/nlp/tools/tf2_bert_encoder_checkpoint_converter.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/nlp/tools/tokenization.py` & `tf-models-official-2.9.2/official/nlp/tools/tokenization.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/nlp/tools/tokenization_test.py` & `tf-models-official-2.9.2/official/nlp/tools/tokenization_test.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/nlp/train.py` & `tf-models-official-2.9.2/official/nlp/train.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/projects/__init__.py` & `tf-models-official-2.9.2/official/projects/__init__.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/projects/bigbird/__init__.py` & `tf-models-official-2.9.2/official/projects/bigbird/__init__.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/projects/bigbird/encoder.py` & `tf-models-official-2.9.2/official/projects/bigbird/encoder.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/projects/bigbird/encoder_test.py` & `tf-models-official-2.9.2/official/projects/bigbird/encoder_test.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/projects/bigbird/experiment_configs.py` & `tf-models-official-2.9.2/official/projects/bigbird/experiment_configs.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/projects/bigbird/recompute_grad.py` & `tf-models-official-2.9.2/official/projects/bigbird/recompute_grad.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/projects/bigbird/recomputing_dropout.py` & `tf-models-official-2.9.2/official/projects/bigbird/recomputing_dropout.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/projects/bigbird/stateless_dropout.py` & `tf-models-official-2.9.2/official/projects/bigbird/stateless_dropout.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/projects/deepmac_maskrcnn/__init__.py` & `tf-models-official-2.9.2/official/projects/deepmac_maskrcnn/__init__.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/projects/deepmac_maskrcnn/common/__init__.py` & `tf-models-official-2.9.2/official/projects/deepmac_maskrcnn/common/__init__.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/projects/deepmac_maskrcnn/common/registry_imports.py` & `tf-models-official-2.9.2/official/projects/deepmac_maskrcnn/common/registry_imports.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/projects/deepmac_maskrcnn/configs/__init__.py` & `tf-models-official-2.9.2/official/projects/deepmac_maskrcnn/configs/__init__.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/projects/deepmac_maskrcnn/configs/deep_mask_head_rcnn.py` & `tf-models-official-2.9.2/official/projects/deepmac_maskrcnn/configs/deep_mask_head_rcnn.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/projects/deepmac_maskrcnn/configs/deep_mask_head_rcnn_config_test.py` & `tf-models-official-2.9.2/official/projects/deepmac_maskrcnn/configs/deep_mask_head_rcnn_config_test.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/projects/deepmac_maskrcnn/modeling/__init__.py` & `tf-models-official-2.9.2/official/projects/deepmac_maskrcnn/modeling/__init__.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/projects/deepmac_maskrcnn/modeling/heads/__init__.py` & `tf-models-official-2.9.2/official/projects/deepmac_maskrcnn/modeling/heads/__init__.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/projects/deepmac_maskrcnn/modeling/heads/hourglass_network.py` & `tf-models-official-2.9.2/official/projects/deepmac_maskrcnn/modeling/heads/hourglass_network.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/projects/deepmac_maskrcnn/modeling/heads/instance_heads.py` & `tf-models-official-2.9.2/official/projects/deepmac_maskrcnn/modeling/heads/instance_heads.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/projects/deepmac_maskrcnn/modeling/heads/instance_heads_test.py` & `tf-models-official-2.9.2/official/projects/deepmac_maskrcnn/modeling/heads/instance_heads_test.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/projects/deepmac_maskrcnn/modeling/maskrcnn_model.py` & `tf-models-official-2.9.2/official/projects/deepmac_maskrcnn/modeling/maskrcnn_model.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/projects/deepmac_maskrcnn/modeling/maskrcnn_model_test.py` & `tf-models-official-2.9.2/official/projects/deepmac_maskrcnn/modeling/maskrcnn_model_test.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/projects/deepmac_maskrcnn/serving/__init__.py` & `tf-models-official-2.9.2/official/projects/deepmac_maskrcnn/serving/__init__.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/projects/deepmac_maskrcnn/serving/detection.py` & `tf-models-official-2.9.2/official/projects/deepmac_maskrcnn/serving/detection.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/projects/deepmac_maskrcnn/serving/detection_test.py` & `tf-models-official-2.9.2/official/projects/deepmac_maskrcnn/serving/detection_test.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/projects/deepmac_maskrcnn/serving/export_saved_model.py` & `tf-models-official-2.9.2/official/projects/deepmac_maskrcnn/serving/export_saved_model.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/projects/deepmac_maskrcnn/tasks/__init__.py` & `tf-models-official-2.9.2/official/projects/deepmac_maskrcnn/tasks/__init__.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/projects/deepmac_maskrcnn/tasks/deep_mask_head_rcnn.py` & `tf-models-official-2.9.2/official/projects/deepmac_maskrcnn/tasks/deep_mask_head_rcnn.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/projects/deepmac_maskrcnn/train.py` & `tf-models-official-2.9.2/official/projects/deepmac_maskrcnn/train.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/projects/mobilebert/__init__.py` & `tf-models-official-2.9.2/official/projects/mobilebert/__init__.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/projects/mobilebert/distillation.py` & `tf-models-official-2.9.2/official/projects/mobilebert/distillation.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/projects/mobilebert/distillation_test.py` & `tf-models-official-2.9.2/official/projects/mobilebert/distillation_test.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/projects/mobilebert/export_tfhub.py` & `tf-models-official-2.9.2/official/projects/mobilebert/export_tfhub.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/projects/mobilebert/model_utils.py` & `tf-models-official-2.9.2/official/projects/mobilebert/model_utils.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/projects/mobilebert/run_distillation.py` & `tf-models-official-2.9.2/official/projects/mobilebert/run_distillation.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/projects/mobilebert/tf2_model_checkpoint_converter.py` & `tf-models-official-2.9.2/official/projects/mobilebert/tf2_model_checkpoint_converter.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/projects/mobilebert/utils.py` & `tf-models-official-2.9.2/official/projects/mobilebert/utils.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/projects/movinet/__init__.py` & `tf-models-official-2.9.2/official/projects/movinet/__init__.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/projects/movinet/configs/__init__.py` & `tf-models-official-2.9.2/official/projects/movinet/configs/__init__.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/projects/movinet/configs/movinet.py` & `tf-models-official-2.9.2/official/projects/movinet/configs/movinet.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/projects/movinet/configs/movinet_test.py` & `tf-models-official-2.9.2/official/projects/movinet/configs/movinet_test.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/projects/movinet/modeling/__init__.py` & `tf-models-official-2.9.2/official/projects/movinet/modeling/__init__.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/projects/movinet/modeling/movinet.py` & `tf-models-official-2.9.2/official/projects/movinet/modeling/movinet.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/projects/movinet/modeling/movinet_layers.py` & `tf-models-official-2.9.2/official/projects/movinet/modeling/movinet_layers.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/projects/movinet/modeling/movinet_layers_test.py` & `tf-models-official-2.9.2/official/projects/movinet/modeling/movinet_layers_test.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/projects/movinet/modeling/movinet_model.py` & `tf-models-official-2.9.2/official/projects/movinet/modeling/movinet_model.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/projects/movinet/modeling/movinet_model_test.py` & `tf-models-official-2.9.2/official/projects/movinet/modeling/movinet_model_test.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/projects/movinet/modeling/movinet_test.py` & `tf-models-official-2.9.2/official/projects/movinet/modeling/movinet_test.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/projects/movinet/tools/__init__.py` & `tf-models-official-2.9.2/official/projects/movinet/tools/__init__.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/projects/movinet/tools/convert_3d_2plus1d.py` & `tf-models-official-2.9.2/official/projects/movinet/tools/convert_3d_2plus1d.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/projects/movinet/tools/convert_3d_2plus1d_test.py` & `tf-models-official-2.9.2/official/projects/movinet/tools/convert_3d_2plus1d_test.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/projects/movinet/tools/export_saved_model.py` & `tf-models-official-2.9.2/official/projects/movinet/tools/export_saved_model.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/projects/movinet/tools/export_saved_model_test.py` & `tf-models-official-2.9.2/official/projects/movinet/tools/export_saved_model_test.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/projects/movinet/tools/quantize_movinet.py` & `tf-models-official-2.9.2/official/projects/movinet/tools/quantize_movinet.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/projects/movinet/train.py` & `tf-models-official-2.9.2/official/projects/movinet/train.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/projects/movinet/train_test.py` & `tf-models-official-2.9.2/official/projects/movinet/train_test.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/projects/nhnet/__init__.py` & `tf-models-official-2.9.2/official/projects/nhnet/__init__.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/projects/nhnet/configs.py` & `tf-models-official-2.9.2/official/projects/nhnet/configs.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/projects/nhnet/configs_test.py` & `tf-models-official-2.9.2/official/projects/nhnet/configs_test.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/projects/nhnet/decoder.py` & `tf-models-official-2.9.2/official/projects/nhnet/decoder.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/projects/nhnet/decoder_test.py` & `tf-models-official-2.9.2/official/projects/nhnet/decoder_test.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/projects/nhnet/evaluation.py` & `tf-models-official-2.9.2/official/projects/nhnet/evaluation.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/projects/nhnet/input_pipeline.py` & `tf-models-official-2.9.2/official/projects/nhnet/input_pipeline.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/projects/nhnet/models.py` & `tf-models-official-2.9.2/official/projects/nhnet/models.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/projects/nhnet/models_test.py` & `tf-models-official-2.9.2/official/projects/nhnet/models_test.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/projects/nhnet/optimizer.py` & `tf-models-official-2.9.2/official/projects/nhnet/optimizer.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/projects/nhnet/raw_data_process.py` & `tf-models-official-2.9.2/official/projects/nhnet/raw_data_process.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/projects/nhnet/raw_data_processor.py` & `tf-models-official-2.9.2/official/projects/nhnet/raw_data_processor.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/projects/nhnet/trainer.py` & `tf-models-official-2.9.2/official/projects/nhnet/trainer.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/projects/nhnet/trainer_test.py` & `tf-models-official-2.9.2/official/projects/nhnet/trainer_test.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/projects/nhnet/utils.py` & `tf-models-official-2.9.2/official/projects/nhnet/utils.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/projects/roformer/__init__.py` & `tf-models-official-2.9.2/official/projects/roformer/__init__.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/projects/roformer/roformer.py` & `tf-models-official-2.9.2/official/projects/roformer/roformer.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/projects/roformer/roformer_attention.py` & `tf-models-official-2.9.2/official/projects/roformer/roformer_attention.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/projects/roformer/roformer_attention_test.py` & `tf-models-official-2.9.2/official/projects/roformer/roformer_attention_test.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/projects/roformer/roformer_encoder.py` & `tf-models-official-2.9.2/official/projects/roformer/roformer_encoder.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/projects/roformer/roformer_encoder_block.py` & `tf-models-official-2.9.2/official/projects/roformer/roformer_encoder_block.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/projects/roformer/roformer_encoder_block_test.py` & `tf-models-official-2.9.2/official/projects/roformer/roformer_encoder_block_test.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/projects/roformer/roformer_encoder_test.py` & `tf-models-official-2.9.2/official/projects/roformer/roformer_encoder_test.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/projects/roformer/roformer_experiments.py` & `tf-models-official-2.9.2/official/projects/roformer/roformer_experiments.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/projects/roformer/train.py` & `tf-models-official-2.9.2/official/projects/roformer/train.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/projects/teams/__init__.py` & `tf-models-official-2.9.2/official/projects/teams/__init__.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/projects/teams/teams.py` & `tf-models-official-2.9.2/official/projects/teams/teams.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/projects/teams/teams_experiments.py` & `tf-models-official-2.9.2/official/projects/teams/teams_experiments.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/projects/teams/teams_experiments_test.py` & `tf-models-official-2.9.2/official/projects/teams/teams_experiments_test.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/projects/teams/teams_pretrainer.py` & `tf-models-official-2.9.2/official/projects/teams/teams_pretrainer.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/projects/teams/teams_pretrainer_test.py` & `tf-models-official-2.9.2/official/projects/teams/teams_pretrainer_test.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/projects/teams/teams_task.py` & `tf-models-official-2.9.2/official/projects/teams/teams_task.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/projects/teams/teams_task_test.py` & `tf-models-official-2.9.2/official/projects/teams/teams_task_test.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/projects/triviaqa/__init__.py` & `tf-models-official-2.9.2/official/projects/triviaqa/__init__.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/projects/triviaqa/dataset.py` & `tf-models-official-2.9.2/official/projects/triviaqa/dataset.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/projects/triviaqa/download_and_prepare.py` & `tf-models-official-2.9.2/official/projects/triviaqa/download_and_prepare.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/projects/triviaqa/evaluate.py` & `tf-models-official-2.9.2/official/projects/triviaqa/evaluate.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/projects/triviaqa/evaluation.py` & `tf-models-official-2.9.2/official/projects/triviaqa/evaluation.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/projects/triviaqa/inputs.py` & `tf-models-official-2.9.2/official/projects/triviaqa/inputs.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/projects/triviaqa/modeling.py` & `tf-models-official-2.9.2/official/projects/triviaqa/modeling.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/projects/triviaqa/predict.py` & `tf-models-official-2.9.2/official/projects/triviaqa/predict.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/projects/triviaqa/prediction.py` & `tf-models-official-2.9.2/official/projects/triviaqa/prediction.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/projects/triviaqa/preprocess.py` & `tf-models-official-2.9.2/official/projects/triviaqa/preprocess.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/projects/triviaqa/sentencepiece_pb2.py` & `tf-models-official-2.9.2/official/projects/triviaqa/sentencepiece_pb2.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/projects/triviaqa/train.py` & `tf-models-official-2.9.2/official/projects/triviaqa/train.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/projects/yt8m/__init__.py` & `tf-models-official-2.9.2/official/projects/yt8m/__init__.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/projects/yt8m/configs/__init__.py` & `tf-models-official-2.9.2/official/projects/yt8m/configs/__init__.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/projects/yt8m/configs/yt8m.py` & `tf-models-official-2.9.2/official/projects/yt8m/configs/yt8m.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/projects/yt8m/modeling/__init__.py` & `tf-models-official-2.9.2/official/projects/yt8m/modeling/__init__.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/projects/yt8m/modeling/yt8m_agg_models.py` & `tf-models-official-2.9.2/official/projects/yt8m/modeling/yt8m_agg_models.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/projects/yt8m/modeling/yt8m_model.py` & `tf-models-official-2.9.2/official/projects/yt8m/modeling/yt8m_model.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/projects/yt8m/modeling/yt8m_model_test.py` & `tf-models-official-2.9.2/official/projects/yt8m/modeling/yt8m_model_test.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/projects/yt8m/modeling/yt8m_model_utils.py` & `tf-models-official-2.9.2/official/projects/yt8m/modeling/yt8m_model_utils.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/projects/yt8m/tasks/__init__.py` & `tf-models-official-2.9.2/official/projects/yt8m/tasks/__init__.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/projects/yt8m/tasks/yt8m_task.py` & `tf-models-official-2.9.2/official/projects/yt8m/tasks/yt8m_task.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/projects/yt8m/train.py` & `tf-models-official-2.9.2/official/projects/yt8m/train.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/projects/yt8m/train_test.py` & `tf-models-official-2.9.2/official/projects/yt8m/train_test.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/recommendation/__init__.py` & `tf-models-official-2.9.2/official/recommendation/__init__.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/recommendation/constants.py` & `tf-models-official-2.9.2/official/recommendation/constants.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/recommendation/create_ncf_data.py` & `tf-models-official-2.9.2/official/recommendation/create_ncf_data.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/recommendation/data_pipeline.py` & `tf-models-official-2.9.2/official/recommendation/data_pipeline.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/recommendation/data_preprocessing.py` & `tf-models-official-2.9.2/official/recommendation/data_preprocessing.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/recommendation/data_test.py` & `tf-models-official-2.9.2/official/recommendation/data_test.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/recommendation/movielens.py` & `tf-models-official-2.9.2/official/recommendation/movielens.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/recommendation/ncf_common.py` & `tf-models-official-2.9.2/official/recommendation/ncf_common.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/recommendation/ncf_input_pipeline.py` & `tf-models-official-2.9.2/official/recommendation/ncf_input_pipeline.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/recommendation/ncf_keras_main.py` & `tf-models-official-2.9.2/official/recommendation/ncf_keras_main.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/recommendation/ncf_test.py` & `tf-models-official-2.9.2/official/recommendation/ncf_test.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/recommendation/neumf_model.py` & `tf-models-official-2.9.2/official/recommendation/neumf_model.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/recommendation/popen_helper.py` & `tf-models-official-2.9.2/official/recommendation/popen_helper.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/recommendation/ranking/__init__.py` & `tf-models-official-2.9.2/official/recommendation/ranking/__init__.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/recommendation/ranking/common.py` & `tf-models-official-2.9.2/official/recommendation/ranking/common.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/recommendation/ranking/configs/__init__.py` & `tf-models-official-2.9.2/official/recommendation/ranking/configs/__init__.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/recommendation/ranking/configs/config.py` & `tf-models-official-2.9.2/official/recommendation/ranking/configs/config.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/recommendation/ranking/configs/config_test.py` & `tf-models-official-2.9.2/official/recommendation/ranking/configs/config_test.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/recommendation/ranking/data/__init__.py` & `tf-models-official-2.9.2/official/recommendation/ranking/data/__init__.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/recommendation/ranking/data/data_pipeline.py` & `tf-models-official-2.9.2/official/recommendation/ranking/data/data_pipeline.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/recommendation/ranking/data/data_pipeline_test.py` & `tf-models-official-2.9.2/official/recommendation/ranking/data/data_pipeline_test.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/recommendation/ranking/task.py` & `tf-models-official-2.9.2/official/recommendation/ranking/task.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/recommendation/ranking/task_test.py` & `tf-models-official-2.9.2/official/recommendation/ranking/task_test.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/recommendation/ranking/train.py` & `tf-models-official-2.9.2/official/recommendation/ranking/train.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/recommendation/ranking/train_test.py` & `tf-models-official-2.9.2/official/recommendation/ranking/train_test.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/recommendation/stat_utils.py` & `tf-models-official-2.9.2/official/recommendation/stat_utils.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/utils/__init__.py` & `tf-models-official-2.9.2/official/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/utils/docs/__init__.py` & `tf-models-official-2.9.2/official/utils/docs/__init__.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/utils/docs/build_all_api_docs.py` & `tf-models-official-2.9.2/official/utils/docs/build_all_api_docs.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/utils/docs/build_all_api_docs_test.py` & `tf-models-official-2.9.2/official/utils/docs/build_all_api_docs_test.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/utils/docs/build_api_docs_lib.py` & `tf-models-official-2.9.2/official/utils/docs/build_api_docs_lib.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/utils/docs/build_nlp_api_docs.py` & `tf-models-official-2.9.2/official/utils/docs/build_nlp_api_docs.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/utils/docs/build_vision_api_docs.py` & `tf-models-official-2.9.2/official/utils/docs/build_vision_api_docs.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/utils/flags/__init__.py` & `tf-models-official-2.9.2/official/utils/flags/__init__.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/utils/flags/_base.py` & `tf-models-official-2.9.2/official/utils/flags/_base.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/utils/flags/_benchmark.py` & `tf-models-official-2.9.2/official/utils/flags/_benchmark.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/utils/flags/_conventions.py` & `tf-models-official-2.9.2/official/utils/flags/_conventions.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/utils/flags/_device.py` & `tf-models-official-2.9.2/official/utils/flags/_device.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/utils/flags/_distribution.py` & `tf-models-official-2.9.2/official/utils/flags/_distribution.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/utils/flags/_misc.py` & `tf-models-official-2.9.2/official/utils/flags/_misc.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/utils/flags/_performance.py` & `tf-models-official-2.9.2/official/utils/flags/_performance.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/utils/flags/core.py` & `tf-models-official-2.9.2/official/utils/flags/core.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/utils/flags/flags_test.py` & `tf-models-official-2.9.2/official/utils/flags/flags_test.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/utils/hyperparams_flags.py` & `tf-models-official-2.9.2/official/utils/hyperparams_flags.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/utils/misc/__init__.py` & `tf-models-official-2.9.2/official/utils/misc/__init__.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/utils/misc/keras_utils.py` & `tf-models-official-2.9.2/official/utils/misc/keras_utils.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/utils/misc/model_helpers.py` & `tf-models-official-2.9.2/official/utils/misc/model_helpers.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/utils/misc/model_helpers_test.py` & `tf-models-official-2.9.2/official/utils/misc/model_helpers_test.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/utils/testing/__init__.py` & `tf-models-official-2.9.2/official/utils/testing/__init__.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/utils/testing/integration.py` & `tf-models-official-2.9.2/official/utils/testing/integration.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/utils/testing/mock_task.py` & `tf-models-official-2.9.2/official/utils/testing/mock_task.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/vision/__init__.py` & `tf-models-official-2.9.2/official/vision/__init__.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/vision/beta/__init__.py` & `tf-models-official-2.9.2/official/vision/beta/__init__.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/vision/beta/projects/__init__.py` & `tf-models-official-2.9.2/official/vision/beta/projects/__init__.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/vision/beta/projects/panoptic_maskrcnn/__init__.py` & `tf-models-official-2.9.2/official/vision/beta/projects/panoptic_maskrcnn/__init__.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/vision/beta/projects/panoptic_maskrcnn/configs/__init__.py` & `tf-models-official-2.9.2/official/vision/beta/projects/panoptic_maskrcnn/configs/__init__.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/vision/beta/projects/panoptic_maskrcnn/configs/panoptic_maskrcnn.py` & `tf-models-official-2.9.2/official/vision/beta/projects/panoptic_maskrcnn/configs/panoptic_maskrcnn.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/vision/beta/projects/panoptic_maskrcnn/configs/panoptic_maskrcnn_test.py` & `tf-models-official-2.9.2/official/vision/beta/projects/panoptic_maskrcnn/configs/panoptic_maskrcnn_test.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/vision/beta/projects/panoptic_maskrcnn/tasks/__init__.py` & `tf-models-official-2.9.2/official/vision/beta/projects/panoptic_maskrcnn/tasks/__init__.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/vision/beta/projects/panoptic_maskrcnn/tasks/panoptic_maskrcnn.py` & `tf-models-official-2.9.2/official/vision/beta/projects/panoptic_maskrcnn/tasks/panoptic_maskrcnn.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/vision/beta/projects/panoptic_maskrcnn/tasks/panoptic_maskrcnn_test.py` & `tf-models-official-2.9.2/official/vision/beta/projects/panoptic_maskrcnn/tasks/panoptic_maskrcnn_test.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/vision/beta/projects/panoptic_maskrcnn/train.py` & `tf-models-official-2.9.2/official/vision/beta/projects/panoptic_maskrcnn/train.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/vision/beta/projects/yolo/__init__.py` & `tf-models-official-2.9.2/official/vision/beta/projects/yolo/__init__.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/vision/beta/projects/yolo/common/__init__.py` & `tf-models-official-2.9.2/official/vision/beta/projects/yolo/common/__init__.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/vision/beta/projects/yolo/common/registry_imports.py` & `tf-models-official-2.9.2/official/vision/beta/projects/yolo/common/registry_imports.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/vision/beta/projects/yolo/configs/__init__.py` & `tf-models-official-2.9.2/official/vision/beta/projects/yolo/configs/__init__.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/vision/beta/projects/yolo/configs/backbones.py` & `tf-models-official-2.9.2/official/vision/beta/projects/yolo/configs/backbones.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/vision/beta/projects/yolo/configs/darknet_classification.py` & `tf-models-official-2.9.2/official/vision/beta/projects/yolo/configs/darknet_classification.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/vision/beta/projects/yolo/configs/decoders.py` & `tf-models-official-2.9.2/official/vision/beta/projects/yolo/configs/decoders.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/vision/beta/projects/yolo/configs/yolo.py` & `tf-models-official-2.9.2/official/vision/beta/projects/yolo/configs/yolo.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/vision/beta/projects/yolo/dataloaders/__init__.py` & `tf-models-official-2.9.2/official/vision/beta/projects/yolo/dataloaders/__init__.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/vision/beta/projects/yolo/dataloaders/classification_input.py` & `tf-models-official-2.9.2/official/vision/beta/projects/yolo/dataloaders/classification_input.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/vision/beta/projects/yolo/dataloaders/tf_example_decoder.py` & `tf-models-official-2.9.2/official/vision/beta/projects/yolo/dataloaders/tf_example_decoder.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/vision/beta/projects/yolo/dataloaders/yolo_input.py` & `tf-models-official-2.9.2/official/vision/beta/projects/yolo/dataloaders/yolo_input.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/vision/beta/projects/yolo/losses/__init__.py` & `tf-models-official-2.9.2/official/vision/beta/projects/yolo/losses/__init__.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/vision/beta/projects/yolo/losses/yolo_loss.py` & `tf-models-official-2.9.2/official/vision/beta/projects/yolo/losses/yolo_loss.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/vision/beta/projects/yolo/losses/yolo_loss_test.py` & `tf-models-official-2.9.2/official/vision/beta/projects/yolo/losses/yolo_loss_test.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/vision/beta/projects/yolo/ops/__init__.py` & `tf-models-official-2.9.2/official/vision/beta/projects/yolo/ops/__init__.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/vision/beta/projects/yolo/ops/anchor.py` & `tf-models-official-2.9.2/official/vision/beta/projects/yolo/ops/anchor.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/vision/beta/projects/yolo/ops/box_ops.py` & `tf-models-official-2.9.2/official/vision/beta/projects/yolo/ops/box_ops.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/vision/beta/projects/yolo/ops/box_ops_test.py` & `tf-models-official-2.9.2/official/vision/beta/projects/yolo/ops/box_ops_test.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/vision/beta/projects/yolo/ops/kmeans_anchors.py` & `tf-models-official-2.9.2/official/vision/beta/projects/yolo/ops/kmeans_anchors.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/vision/beta/projects/yolo/ops/kmeans_anchors_test.py` & `tf-models-official-2.9.2/official/vision/beta/projects/yolo/ops/kmeans_anchors_test.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/vision/beta/projects/yolo/ops/loss_utils.py` & `tf-models-official-2.9.2/official/vision/beta/projects/yolo/ops/loss_utils.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/vision/beta/projects/yolo/ops/math_ops.py` & `tf-models-official-2.9.2/official/vision/beta/projects/yolo/ops/math_ops.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/vision/beta/projects/yolo/ops/mosaic.py` & `tf-models-official-2.9.2/official/vision/beta/projects/yolo/ops/mosaic.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/vision/beta/projects/yolo/ops/preprocessing_ops.py` & `tf-models-official-2.9.2/official/vision/beta/projects/yolo/ops/preprocessing_ops.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/vision/beta/projects/yolo/ops/preprocessing_ops_test.py` & `tf-models-official-2.9.2/official/vision/beta/projects/yolo/ops/preprocessing_ops_test.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/vision/beta/projects/yolo/optimization/__init__.py` & `tf-models-official-2.9.2/official/vision/beta/projects/yolo/optimization/__init__.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/vision/beta/projects/yolo/optimization/configs/__init__.py` & `tf-models-official-2.9.2/official/vision/beta/projects/yolo/optimization/configs/__init__.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/vision/beta/projects/yolo/optimization/configs/optimization_config.py` & `tf-models-official-2.9.2/official/vision/beta/projects/yolo/optimization/configs/optimization_config.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/vision/beta/projects/yolo/optimization/configs/optimizer_config.py` & `tf-models-official-2.9.2/official/vision/beta/projects/yolo/optimization/configs/optimizer_config.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/vision/beta/projects/yolo/optimization/optimizer_factory.py` & `tf-models-official-2.9.2/official/vision/beta/projects/yolo/optimization/optimizer_factory.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/vision/beta/projects/yolo/optimization/sgd_torch.py` & `tf-models-official-2.9.2/official/vision/beta/projects/yolo/optimization/sgd_torch.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/vision/beta/projects/yolo/train.py` & `tf-models-official-2.9.2/official/vision/beta/projects/yolo/train.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/vision/configs/__init__.py` & `tf-models-official-2.9.2/official/vision/configs/__init__.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/vision/configs/backbones.py` & `tf-models-official-2.9.2/official/vision/configs/backbones.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/vision/configs/backbones_3d.py` & `tf-models-official-2.9.2/official/vision/configs/backbones_3d.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/vision/configs/common.py` & `tf-models-official-2.9.2/official/vision/configs/common.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/vision/configs/decoders.py` & `tf-models-official-2.9.2/official/vision/configs/decoders.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/vision/configs/image_classification.py` & `tf-models-official-2.9.2/official/vision/configs/image_classification.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/vision/configs/image_classification_test.py` & `tf-models-official-2.9.2/official/vision/configs/image_classification_test.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/vision/configs/maskrcnn.py` & `tf-models-official-2.9.2/official/vision/configs/maskrcnn.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/vision/configs/maskrcnn_test.py` & `tf-models-official-2.9.2/official/vision/configs/maskrcnn_test.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/vision/configs/retinanet.py` & `tf-models-official-2.9.2/official/vision/configs/retinanet.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/vision/configs/retinanet_test.py` & `tf-models-official-2.9.2/official/vision/configs/retinanet_test.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/vision/configs/semantic_segmentation.py` & `tf-models-official-2.9.2/official/vision/configs/semantic_segmentation.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/vision/configs/semantic_segmentation_test.py` & `tf-models-official-2.9.2/official/vision/configs/semantic_segmentation_test.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/vision/configs/video_classification.py` & `tf-models-official-2.9.2/official/vision/configs/video_classification.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/vision/configs/video_classification_test.py` & `tf-models-official-2.9.2/official/vision/configs/video_classification_test.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/vision/data/__init__.py` & `tf-models-official-2.9.2/official/vision/data/__init__.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/vision/data/create_coco_tf_record.py` & `tf-models-official-2.9.2/official/vision/data/create_coco_tf_record.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/vision/data/process_coco_few_shot_json_files.py` & `tf-models-official-2.9.2/official/vision/data/process_coco_few_shot_json_files.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/vision/data/tfrecord_lib.py` & `tf-models-official-2.9.2/official/vision/data/tfrecord_lib.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/vision/data/tfrecord_lib_test.py` & `tf-models-official-2.9.2/official/vision/data/tfrecord_lib_test.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/vision/dataloaders/__init__.py` & `tf-models-official-2.9.2/official/vision/dataloaders/__init__.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/vision/dataloaders/classification_input.py` & `tf-models-official-2.9.2/official/vision/dataloaders/classification_input.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/vision/dataloaders/decoder.py` & `tf-models-official-2.9.2/official/vision/dataloaders/decoder.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/vision/dataloaders/input_reader.py` & `tf-models-official-2.9.2/official/vision/dataloaders/input_reader.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/vision/dataloaders/input_reader_factory.py` & `tf-models-official-2.9.2/official/vision/dataloaders/input_reader_factory.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/vision/dataloaders/maskrcnn_input.py` & `tf-models-official-2.9.2/official/vision/dataloaders/maskrcnn_input.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/vision/dataloaders/parser.py` & `tf-models-official-2.9.2/official/vision/dataloaders/parser.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/vision/dataloaders/retinanet_input.py` & `tf-models-official-2.9.2/official/vision/dataloaders/retinanet_input.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/vision/dataloaders/segmentation_input.py` & `tf-models-official-2.9.2/official/vision/dataloaders/segmentation_input.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/vision/dataloaders/tf_example_decoder.py` & `tf-models-official-2.9.2/official/vision/dataloaders/tf_example_decoder.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/vision/dataloaders/tf_example_decoder_test.py` & `tf-models-official-2.9.2/official/vision/dataloaders/tf_example_decoder_test.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/vision/dataloaders/tf_example_label_map_decoder.py` & `tf-models-official-2.9.2/official/vision/dataloaders/tf_example_label_map_decoder.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/vision/dataloaders/tf_example_label_map_decoder_test.py` & `tf-models-official-2.9.2/official/vision/dataloaders/tf_example_label_map_decoder_test.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/vision/dataloaders/tfds_classification_decoders.py` & `tf-models-official-2.9.2/official/vision/dataloaders/tfds_classification_decoders.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/vision/dataloaders/tfds_detection_decoders.py` & `tf-models-official-2.9.2/official/vision/dataloaders/tfds_detection_decoders.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/vision/dataloaders/tfds_factory.py` & `tf-models-official-2.9.2/official/vision/dataloaders/tfds_factory.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/vision/dataloaders/tfds_factory_test.py` & `tf-models-official-2.9.2/official/vision/dataloaders/tfds_factory_test.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/vision/dataloaders/tfds_segmentation_decoders.py` & `tf-models-official-2.9.2/official/vision/dataloaders/tfds_segmentation_decoders.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/vision/dataloaders/tfexample_utils.py` & `tf-models-official-2.9.2/official/vision/dataloaders/tfexample_utils.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/vision/dataloaders/utils.py` & `tf-models-official-2.9.2/official/vision/dataloaders/utils.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/vision/dataloaders/utils_test.py` & `tf-models-official-2.9.2/official/vision/dataloaders/utils_test.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/vision/dataloaders/video_input.py` & `tf-models-official-2.9.2/official/vision/dataloaders/video_input.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/vision/dataloaders/video_input_test.py` & `tf-models-official-2.9.2/official/vision/dataloaders/video_input_test.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/vision/evaluation/__init__.py` & `tf-models-official-2.9.2/official/vision/evaluation/__init__.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/vision/evaluation/coco_evaluator.py` & `tf-models-official-2.9.2/official/vision/evaluation/coco_evaluator.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/vision/evaluation/coco_utils.py` & `tf-models-official-2.9.2/official/vision/evaluation/coco_utils.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/vision/evaluation/coco_utils_test.py` & `tf-models-official-2.9.2/official/vision/evaluation/coco_utils_test.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/vision/evaluation/iou.py` & `tf-models-official-2.9.2/official/vision/evaluation/iou.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/vision/evaluation/iou_test.py` & `tf-models-official-2.9.2/official/vision/evaluation/iou_test.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/vision/evaluation/panoptic_quality.py` & `tf-models-official-2.9.2/official/vision/evaluation/panoptic_quality.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/vision/evaluation/panoptic_quality_evaluator.py` & `tf-models-official-2.9.2/official/vision/evaluation/panoptic_quality_evaluator.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/vision/evaluation/panoptic_quality_evaluator_test.py` & `tf-models-official-2.9.2/official/vision/evaluation/panoptic_quality_evaluator_test.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/vision/evaluation/panoptic_quality_test.py` & `tf-models-official-2.9.2/official/vision/evaluation/panoptic_quality_test.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/vision/evaluation/segmentation_metrics.py` & `tf-models-official-2.9.2/official/vision/evaluation/segmentation_metrics.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/vision/evaluation/segmentation_metrics_test.py` & `tf-models-official-2.9.2/official/vision/evaluation/segmentation_metrics_test.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/vision/evaluation/wod_detection_evaluator.py` & `tf-models-official-2.9.2/official/vision/evaluation/wod_detection_evaluator.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/vision/losses/__init__.py` & `tf-models-official-2.9.2/official/vision/losses/__init__.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/vision/losses/focal_loss.py` & `tf-models-official-2.9.2/official/vision/losses/focal_loss.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/vision/losses/loss_utils.py` & `tf-models-official-2.9.2/official/vision/losses/loss_utils.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/vision/losses/maskrcnn_losses.py` & `tf-models-official-2.9.2/official/vision/losses/maskrcnn_losses.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/vision/losses/retinanet_losses.py` & `tf-models-official-2.9.2/official/vision/losses/retinanet_losses.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/vision/losses/segmentation_losses.py` & `tf-models-official-2.9.2/official/vision/losses/segmentation_losses.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/vision/modeling/__init__.py` & `tf-models-official-2.9.2/official/vision/modeling/__init__.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/vision/modeling/backbones/__init__.py` & `tf-models-official-2.9.2/official/vision/modeling/backbones/__init__.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/vision/modeling/backbones/efficientnet.py` & `tf-models-official-2.9.2/official/vision/modeling/backbones/efficientnet.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/vision/modeling/backbones/efficientnet_test.py` & `tf-models-official-2.9.2/official/vision/modeling/backbones/efficientnet_test.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/vision/modeling/backbones/factory.py` & `tf-models-official-2.9.2/official/vision/modeling/backbones/factory.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/vision/modeling/backbones/factory_test.py` & `tf-models-official-2.9.2/official/vision/modeling/backbones/factory_test.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/vision/modeling/backbones/mobiledet.py` & `tf-models-official-2.9.2/official/vision/modeling/backbones/mobiledet.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/vision/modeling/backbones/mobiledet_test.py` & `tf-models-official-2.9.2/official/vision/modeling/backbones/mobiledet_test.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/vision/modeling/backbones/mobilenet.py` & `tf-models-official-2.9.2/official/vision/modeling/backbones/mobilenet.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/vision/modeling/backbones/mobilenet_test.py` & `tf-models-official-2.9.2/official/vision/modeling/backbones/mobilenet_test.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/vision/modeling/backbones/resnet.py` & `tf-models-official-2.9.2/official/vision/modeling/backbones/resnet.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/vision/modeling/backbones/resnet_3d.py` & `tf-models-official-2.9.2/official/vision/modeling/backbones/resnet_3d.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/vision/modeling/backbones/resnet_3d_test.py` & `tf-models-official-2.9.2/official/vision/modeling/backbones/resnet_3d_test.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/vision/modeling/backbones/resnet_deeplab.py` & `tf-models-official-2.9.2/official/vision/modeling/backbones/resnet_deeplab.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/vision/modeling/backbones/resnet_deeplab_test.py` & `tf-models-official-2.9.2/official/vision/modeling/backbones/resnet_deeplab_test.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/vision/modeling/backbones/resnet_test.py` & `tf-models-official-2.9.2/official/vision/modeling/backbones/resnet_test.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/vision/modeling/backbones/revnet.py` & `tf-models-official-2.9.2/official/vision/modeling/backbones/revnet.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/vision/modeling/backbones/revnet_test.py` & `tf-models-official-2.9.2/official/vision/modeling/backbones/revnet_test.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/vision/modeling/backbones/spinenet.py` & `tf-models-official-2.9.2/official/vision/modeling/backbones/spinenet.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/vision/modeling/backbones/spinenet_mobile.py` & `tf-models-official-2.9.2/official/vision/modeling/backbones/spinenet_mobile.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/vision/modeling/backbones/spinenet_mobile_test.py` & `tf-models-official-2.9.2/official/vision/modeling/backbones/spinenet_mobile_test.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/vision/modeling/backbones/spinenet_test.py` & `tf-models-official-2.9.2/official/vision/modeling/backbones/spinenet_test.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/vision/modeling/classification_model.py` & `tf-models-official-2.9.2/official/vision/modeling/classification_model.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/vision/modeling/classification_model_test.py` & `tf-models-official-2.9.2/official/vision/modeling/classification_model_test.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/vision/modeling/decoders/__init__.py` & `tf-models-official-2.9.2/official/vision/modeling/decoders/__init__.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/vision/modeling/decoders/aspp.py` & `tf-models-official-2.9.2/official/vision/modeling/decoders/aspp.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/vision/modeling/decoders/aspp_test.py` & `tf-models-official-2.9.2/official/vision/modeling/decoders/aspp_test.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/vision/modeling/decoders/factory.py` & `tf-models-official-2.9.2/official/vision/modeling/decoders/factory.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/vision/modeling/decoders/factory_test.py` & `tf-models-official-2.9.2/official/vision/modeling/decoders/factory_test.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/vision/modeling/decoders/fpn.py` & `tf-models-official-2.9.2/official/vision/modeling/decoders/fpn.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/vision/modeling/decoders/fpn_test.py` & `tf-models-official-2.9.2/official/vision/modeling/decoders/fpn_test.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/vision/modeling/decoders/nasfpn.py` & `tf-models-official-2.9.2/official/vision/modeling/decoders/nasfpn.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/vision/modeling/decoders/nasfpn_test.py` & `tf-models-official-2.9.2/official/vision/modeling/decoders/nasfpn_test.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/vision/modeling/factory.py` & `tf-models-official-2.9.2/official/vision/modeling/factory.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/vision/modeling/factory_3d.py` & `tf-models-official-2.9.2/official/vision/modeling/factory_3d.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/vision/modeling/factory_test.py` & `tf-models-official-2.9.2/official/vision/modeling/factory_test.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/vision/modeling/heads/__init__.py` & `tf-models-official-2.9.2/official/vision/modeling/heads/__init__.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/vision/modeling/heads/dense_prediction_heads.py` & `tf-models-official-2.9.2/official/vision/modeling/heads/dense_prediction_heads.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/vision/modeling/heads/dense_prediction_heads_test.py` & `tf-models-official-2.9.2/official/vision/modeling/heads/dense_prediction_heads_test.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/vision/modeling/heads/instance_heads.py` & `tf-models-official-2.9.2/official/vision/modeling/heads/instance_heads.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/vision/modeling/heads/instance_heads_test.py` & `tf-models-official-2.9.2/official/vision/modeling/heads/instance_heads_test.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/vision/modeling/heads/segmentation_heads.py` & `tf-models-official-2.9.2/official/vision/modeling/heads/segmentation_heads.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/vision/modeling/heads/segmentation_heads_test.py` & `tf-models-official-2.9.2/official/vision/modeling/heads/segmentation_heads_test.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/vision/modeling/layers/__init__.py` & `tf-models-official-2.9.2/official/vision/modeling/layers/__init__.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/vision/modeling/layers/box_sampler.py` & `tf-models-official-2.9.2/official/vision/modeling/layers/box_sampler.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/vision/modeling/layers/deeplab.py` & `tf-models-official-2.9.2/official/vision/modeling/layers/deeplab.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/vision/modeling/layers/deeplab_test.py` & `tf-models-official-2.9.2/official/vision/modeling/layers/deeplab_test.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/vision/modeling/layers/detection_generator.py` & `tf-models-official-2.9.2/official/vision/modeling/layers/detection_generator.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/vision/modeling/layers/detection_generator_test.py` & `tf-models-official-2.9.2/official/vision/modeling/layers/detection_generator_test.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/vision/modeling/layers/mask_sampler.py` & `tf-models-official-2.9.2/official/vision/modeling/layers/mask_sampler.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/vision/modeling/layers/nn_blocks.py` & `tf-models-official-2.9.2/official/vision/modeling/layers/nn_blocks.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/vision/modeling/layers/nn_blocks_3d.py` & `tf-models-official-2.9.2/official/vision/modeling/layers/nn_blocks_3d.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/vision/modeling/layers/nn_blocks_3d_test.py` & `tf-models-official-2.9.2/official/vision/modeling/layers/nn_blocks_3d_test.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/vision/modeling/layers/nn_blocks_test.py` & `tf-models-official-2.9.2/official/vision/modeling/layers/nn_blocks_test.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/vision/modeling/layers/nn_layers.py` & `tf-models-official-2.9.2/official/vision/modeling/layers/nn_layers.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/vision/modeling/layers/nn_layers_test.py` & `tf-models-official-2.9.2/official/vision/modeling/layers/nn_layers_test.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/vision/modeling/layers/roi_aligner.py` & `tf-models-official-2.9.2/official/vision/modeling/layers/roi_aligner.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/vision/modeling/layers/roi_aligner_test.py` & `tf-models-official-2.9.2/official/vision/modeling/layers/roi_aligner_test.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/vision/modeling/layers/roi_generator.py` & `tf-models-official-2.9.2/official/vision/modeling/layers/roi_generator.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/vision/modeling/layers/roi_sampler.py` & `tf-models-official-2.9.2/official/vision/modeling/layers/roi_sampler.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/vision/modeling/maskrcnn_model.py` & `tf-models-official-2.9.2/official/vision/modeling/maskrcnn_model.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/vision/modeling/maskrcnn_model_test.py` & `tf-models-official-2.9.2/official/vision/modeling/maskrcnn_model_test.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/vision/modeling/retinanet_model.py` & `tf-models-official-2.9.2/official/vision/modeling/retinanet_model.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/vision/modeling/retinanet_model_test.py` & `tf-models-official-2.9.2/official/vision/modeling/retinanet_model_test.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/vision/modeling/segmentation_model.py` & `tf-models-official-2.9.2/official/vision/modeling/segmentation_model.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/vision/modeling/segmentation_model_test.py` & `tf-models-official-2.9.2/official/vision/modeling/segmentation_model_test.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/vision/modeling/video_classification_model.py` & `tf-models-official-2.9.2/official/vision/modeling/video_classification_model.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/vision/modeling/video_classification_model_test.py` & `tf-models-official-2.9.2/official/vision/modeling/video_classification_model_test.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/vision/ops/__init__.py` & `tf-models-official-2.9.2/official/vision/ops/__init__.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/vision/ops/anchor.py` & `tf-models-official-2.9.2/official/vision/ops/anchor.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/vision/ops/anchor_generator.py` & `tf-models-official-2.9.2/official/vision/ops/anchor_generator.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/vision/ops/anchor_generator_test.py` & `tf-models-official-2.9.2/official/vision/ops/anchor_generator_test.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/vision/ops/anchor_test.py` & `tf-models-official-2.9.2/official/vision/ops/anchor_test.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/vision/ops/augment.py` & `tf-models-official-2.9.2/official/vision/ops/augment.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/vision/ops/augment_test.py` & `tf-models-official-2.9.2/official/vision/ops/augment_test.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/vision/ops/box_matcher.py` & `tf-models-official-2.9.2/official/vision/ops/box_matcher.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/vision/ops/box_matcher_test.py` & `tf-models-official-2.9.2/official/vision/ops/box_matcher_test.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/vision/ops/box_ops.py` & `tf-models-official-2.9.2/official/vision/ops/box_ops.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/vision/ops/iou_similarity.py` & `tf-models-official-2.9.2/official/vision/ops/iou_similarity.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/vision/ops/iou_similarity_test.py` & `tf-models-official-2.9.2/official/vision/ops/iou_similarity_test.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/vision/ops/mask_ops.py` & `tf-models-official-2.9.2/official/vision/ops/mask_ops.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/vision/ops/mask_ops_test.py` & `tf-models-official-2.9.2/official/vision/ops/mask_ops_test.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/vision/ops/nms.py` & `tf-models-official-2.9.2/official/vision/ops/nms.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/vision/ops/preprocess_ops.py` & `tf-models-official-2.9.2/official/vision/ops/preprocess_ops.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/vision/ops/preprocess_ops_3d.py` & `tf-models-official-2.9.2/official/vision/ops/preprocess_ops_3d.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/vision/ops/preprocess_ops_3d_test.py` & `tf-models-official-2.9.2/official/vision/ops/preprocess_ops_3d_test.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/vision/ops/preprocess_ops_test.py` & `tf-models-official-2.9.2/official/vision/ops/preprocess_ops_test.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/vision/ops/sampling_ops.py` & `tf-models-official-2.9.2/official/vision/ops/sampling_ops.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/vision/ops/spatial_transform_ops.py` & `tf-models-official-2.9.2/official/vision/ops/spatial_transform_ops.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/vision/ops/target_gather.py` & `tf-models-official-2.9.2/official/vision/ops/target_gather.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/vision/ops/target_gather_test.py` & `tf-models-official-2.9.2/official/vision/ops/target_gather_test.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/vision/registry_imports.py` & `tf-models-official-2.9.2/official/vision/registry_imports.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/vision/serving/__init__.py` & `tf-models-official-2.9.2/official/vision/serving/__init__.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/vision/serving/detection.py` & `tf-models-official-2.9.2/official/vision/serving/detection.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/vision/serving/detection_test.py` & `tf-models-official-2.9.2/official/vision/serving/detection_test.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/vision/serving/export_base.py` & `tf-models-official-2.9.2/official/vision/serving/export_base.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/vision/serving/export_base_v2.py` & `tf-models-official-2.9.2/official/vision/serving/export_base_v2.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/vision/serving/export_base_v2_test.py` & `tf-models-official-2.9.2/official/vision/serving/export_base_v2_test.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/vision/serving/export_module_factory.py` & `tf-models-official-2.9.2/official/vision/serving/export_module_factory.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/vision/serving/export_module_factory_test.py` & `tf-models-official-2.9.2/official/vision/serving/export_module_factory_test.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/vision/serving/export_saved_model.py` & `tf-models-official-2.9.2/official/vision/serving/export_saved_model.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/vision/serving/export_saved_model_lib.py` & `tf-models-official-2.9.2/official/vision/serving/export_saved_model_lib.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/vision/serving/export_saved_model_lib_test.py` & `tf-models-official-2.9.2/official/vision/serving/export_saved_model_lib_test.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/vision/serving/export_saved_model_lib_v2.py` & `tf-models-official-2.9.2/official/vision/serving/export_saved_model_lib_v2.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/vision/serving/export_tfhub.py` & `tf-models-official-2.9.2/official/vision/serving/export_tfhub.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/vision/serving/export_tflite.py` & `tf-models-official-2.9.2/official/vision/serving/export_tflite.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/vision/serving/export_tflite_lib.py` & `tf-models-official-2.9.2/official/vision/serving/export_tflite_lib.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/vision/serving/export_tflite_lib_test.py` & `tf-models-official-2.9.2/official/vision/serving/export_tflite_lib_test.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/vision/serving/export_utils.py` & `tf-models-official-2.9.2/official/vision/serving/export_utils.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/vision/serving/image_classification.py` & `tf-models-official-2.9.2/official/vision/serving/image_classification.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/vision/serving/image_classification_test.py` & `tf-models-official-2.9.2/official/vision/serving/image_classification_test.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/vision/serving/semantic_segmentation.py` & `tf-models-official-2.9.2/official/vision/serving/semantic_segmentation.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/vision/serving/semantic_segmentation_test.py` & `tf-models-official-2.9.2/official/vision/serving/semantic_segmentation_test.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/vision/serving/video_classification.py` & `tf-models-official-2.9.2/official/vision/serving/video_classification.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/vision/serving/video_classification_test.py` & `tf-models-official-2.9.2/official/vision/serving/video_classification_test.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/vision/tasks/__init__.py` & `tf-models-official-2.9.2/official/vision/tasks/__init__.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/vision/tasks/image_classification.py` & `tf-models-official-2.9.2/official/vision/tasks/image_classification.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/vision/tasks/maskrcnn.py` & `tf-models-official-2.9.2/official/vision/tasks/maskrcnn.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/vision/tasks/retinanet.py` & `tf-models-official-2.9.2/official/vision/tasks/retinanet.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/vision/tasks/semantic_segmentation.py` & `tf-models-official-2.9.2/official/vision/tasks/semantic_segmentation.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/vision/tasks/video_classification.py` & `tf-models-official-2.9.2/official/vision/tasks/video_classification.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/vision/train.py` & `tf-models-official-2.9.2/official/vision/train.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/vision/train_spatial_partitioning.py` & `tf-models-official-2.9.2/official/vision/train_spatial_partitioning.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/vision/utils/__init__.py` & `tf-models-official-2.9.2/official/vision/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/vision/utils/object_detection/__init__.py` & `tf-models-official-2.9.2/official/vision/utils/object_detection/__init__.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/vision/utils/object_detection/argmax_matcher.py` & `tf-models-official-2.9.2/official/vision/utils/object_detection/argmax_matcher.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/vision/utils/object_detection/balanced_positive_negative_sampler.py` & `tf-models-official-2.9.2/official/vision/utils/object_detection/balanced_positive_negative_sampler.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/vision/utils/object_detection/box_coder.py` & `tf-models-official-2.9.2/official/vision/utils/object_detection/box_coder.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/vision/utils/object_detection/box_list.py` & `tf-models-official-2.9.2/official/vision/utils/object_detection/box_list.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/vision/utils/object_detection/box_list_ops.py` & `tf-models-official-2.9.2/official/vision/utils/object_detection/box_list_ops.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/vision/utils/object_detection/faster_rcnn_box_coder.py` & `tf-models-official-2.9.2/official/vision/utils/object_detection/faster_rcnn_box_coder.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/vision/utils/object_detection/matcher.py` & `tf-models-official-2.9.2/official/vision/utils/object_detection/matcher.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/vision/utils/object_detection/minibatch_sampler.py` & `tf-models-official-2.9.2/official/vision/utils/object_detection/minibatch_sampler.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/vision/utils/object_detection/ops.py` & `tf-models-official-2.9.2/official/vision/utils/object_detection/ops.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/vision/utils/object_detection/preprocessor.py` & `tf-models-official-2.9.2/official/vision/utils/object_detection/preprocessor.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/vision/utils/object_detection/region_similarity_calculator.py` & `tf-models-official-2.9.2/official/vision/utils/object_detection/region_similarity_calculator.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/vision/utils/object_detection/shape_utils.py` & `tf-models-official-2.9.2/official/vision/utils/object_detection/shape_utils.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/vision/utils/object_detection/target_assigner.py` & `tf-models-official-2.9.2/official/vision/utils/object_detection/target_assigner.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/official/vision/utils/object_detection/visualization_utils.py` & `tf-models-official-2.9.2/official/vision/utils/object_detection/visualization_utils.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/orbit/__init__.py` & `tf-models-official-2.9.2/orbit/__init__.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/orbit/actions/__init__.py` & `tf-models-official-2.9.2/orbit/actions/__init__.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/orbit/actions/conditional_action.py` & `tf-models-official-2.9.2/orbit/actions/conditional_action.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/orbit/actions/conditional_action_test.py` & `tf-models-official-2.9.2/orbit/actions/conditional_action_test.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/orbit/actions/export_saved_model.py` & `tf-models-official-2.9.2/orbit/actions/export_saved_model.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/orbit/actions/export_saved_model_test.py` & `tf-models-official-2.9.2/orbit/actions/export_saved_model_test.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/orbit/actions/new_best_metric.py` & `tf-models-official-2.9.2/orbit/actions/new_best_metric.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/orbit/actions/new_best_metric_test.py` & `tf-models-official-2.9.2/orbit/actions/new_best_metric_test.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/orbit/controller.py` & `tf-models-official-2.9.2/orbit/controller.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/orbit/controller_test.py` & `tf-models-official-2.9.2/orbit/controller_test.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/orbit/examples/__init__.py` & `tf-models-official-2.9.2/orbit/examples/__init__.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/orbit/examples/single_task/__init__.py` & `tf-models-official-2.9.2/orbit/examples/single_task/__init__.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/orbit/examples/single_task/single_task_evaluator.py` & `tf-models-official-2.9.2/orbit/examples/single_task/single_task_evaluator.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/orbit/examples/single_task/single_task_evaluator_test.py` & `tf-models-official-2.9.2/orbit/examples/single_task/single_task_evaluator_test.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/orbit/examples/single_task/single_task_trainer.py` & `tf-models-official-2.9.2/orbit/examples/single_task/single_task_trainer.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/orbit/examples/single_task/single_task_trainer_test.py` & `tf-models-official-2.9.2/orbit/examples/single_task/single_task_trainer_test.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/orbit/runner.py` & `tf-models-official-2.9.2/orbit/runner.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/orbit/standard_runner.py` & `tf-models-official-2.9.2/orbit/standard_runner.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/orbit/standard_runner_test.py` & `tf-models-official-2.9.2/orbit/standard_runner_test.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/orbit/utils/__init__.py` & `tf-models-official-2.9.2/orbit/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/orbit/utils/common.py` & `tf-models-official-2.9.2/orbit/utils/common.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/orbit/utils/common_test.py` & `tf-models-official-2.9.2/orbit/utils/common_test.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/orbit/utils/epoch_helper.py` & `tf-models-official-2.9.2/orbit/utils/epoch_helper.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/orbit/utils/loop_fns.py` & `tf-models-official-2.9.2/orbit/utils/loop_fns.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/orbit/utils/summary_manager.py` & `tf-models-official-2.9.2/orbit/utils/summary_manager.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/orbit/utils/tpu_summaries.py` & `tf-models-official-2.9.2/orbit/utils/tpu_summaries.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/orbit/utils/tpu_summaries_test.py` & `tf-models-official-2.9.2/orbit/utils/tpu_summaries_test.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/tensorflow_models/__init__.py` & `tf-models-official-2.9.2/tensorflow_models/__init__.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/tensorflow_models/nlp/__init__.py` & `tf-models-official-2.9.2/tensorflow_models/nlp/__init__.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/tensorflow_models/tensorflow_models_test.py` & `tf-models-official-2.9.2/tensorflow_models/tensorflow_models_test.py`

 * *Files identical despite different names*

### Comparing `tf-models-official-2.9.1/tensorflow_models/vision/__init__.py` & `tf-models-official-2.9.2/tensorflow_models/vision/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -12,7 +12,8 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """TensorFlow Models Vision Libraries."""
 from official.vision import configs
 from official.vision import serving
 from official.vision.modeling import *
+from official.vision.ops import *
```

### Comparing `tf-models-official-2.9.1/tf_models_official.egg-info/PKG-INFO` & `tf-models-official-2.9.2/tf_models_official.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tf-models-official
-Version: 2.9.1
+Version: 2.9.2
 Summary: TensorFlow Official Models
 Home-page: https://github.com/tensorflow/models
 Author: Google Inc.
 Author-email: packages@tensorflow.org
 License: Apache 2.0
 Platform: UNKNOWN
 Requires-Python: >=3.7
```

### Comparing `tf-models-official-2.9.1/tf_models_official.egg-info/SOURCES.txt` & `tf-models-official-2.9.2/tf_models_official.egg-info/SOURCES.txt`

 * *Files identical despite different names*

