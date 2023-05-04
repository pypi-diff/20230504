# Comparing `tmp/useis-0.9.9.tar.gz` & `tmp/useis-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "useis-0.9.9.tar", max compression
+gzip compressed data, was "useis-1.0.0.tar", max compression
```

## Comparing `useis-0.9.9.tar` & `useis-1.0.0.tar`

### file list

```diff
@@ -1,52 +1,105 @@
--rw-r--r--   0        0        0     1076 2021-03-26 21:23:47.497192 useis-0.9.9/LICENSE
--rw-r--r--   0        0        0      963 2021-11-25 20:12:05.204113 useis-0.9.9/pyproject.toml
--rw-r--r--   0        0        0        0 2021-03-26 21:38:32.877385 useis-0.9.9/useis/__init__.py
--rw-r--r--   0        0        0        0 2021-10-14 09:30:52.160262 useis-0.9.9/useis/ai/__init__.py
--rw-r--r--   0        0        0    10944 2021-05-12 16:55:26.280000 useis-0.9.9/useis/ai/dataset.py
--rw-r--r--   0        0        0    17320 2021-11-25 18:23:18.491640 useis-0.9.9/useis/ai/model.py
--rw-r--r--   0        0        0     9768 2021-05-04 19:27:55.987000 useis-0.9.9/useis/ai/resnet1d.py
--rw-r--r--   0        0        0     2109 2021-05-14 15:00:10.546000 useis-0.9.9/useis/ai/spectrogram.py
--rw-r--r--   0        0        0        0 2021-03-26 21:40:55.118730 useis-0.9.9/useis/core/__init__.py
--rw-r--r--   0        0        0    23807 2021-11-19 01:09:55.908700 useis-0.9.9/useis/core/project_manager.py
--rw-r--r--   0        0        0        0 2021-03-26 21:41:47.087784 useis-0.9.9/useis/processors/__init__.py
--rw-r--r--   0        0        0     1382 2021-11-25 19:21:56.289150 useis-0.9.9/useis/processors/classifier.py
--rw-r--r--   0        0        0    17442 2021-11-18 17:47:09.035850 useis-0.9.9/useis/processors/nlloc.py
--rw-r--r--   0        0        0     7149 2021-11-25 20:05:19.194745 useis-0.9.9/useis/processors/picker.py
--rw-r--r--   0        0        0      349 2021-08-23 11:49:31.705467 useis-0.9.9/useis/processors/ray_tracer.py
--rw-r--r--   0        0        0     2272 2021-11-19 00:58:44.458341 useis-0.9.9/useis/processors/simple_magnitude.py
--rw-r--r--   0        0        0        0 2021-09-25 09:38:47.869586 useis-0.9.9/useis/sandbox/__init__.py
--rw-r--r--   0        0        0      721 2021-09-27 01:19:38.267248 useis-0.9.9/useis/sandbox/demo_kafka/Dockerfile
--rw-r--r--   0        0        0        0 2021-09-27 00:20:33.269633 useis-0.9.9/useis/sandbox/demo_kafka/__init__.py
--rw-r--r--   0        0        0     1086 2021-09-27 17:41:51.119655 useis-0.9.9/useis/sandbox/demo_kafka/consumer.py
--rw-r--r--   0        0        0        2 2021-09-27 00:20:35.289724 useis-0.9.9/useis/sandbox/demo_kafka/demo_kafka.py
--rw-r--r--   0        0        0     6660 2021-09-27 17:46:25.823999 useis-0.9.9/useis/sandbox/demo_kafka/docker-compose.yml
--rw-r--r--   0        0        0      456 2021-09-27 17:34:43.328543 useis-0.9.9/useis/sandbox/demo_kafka/producer.py
--rw-r--r--   0        0        0    33387 2021-09-27 00:18:11.131162 useis-0.9.9/useis/sandbox/demo_useis/demo_useis_nlloc.ipynb
--rw-r--r--   0        0        0       46 2021-09-26 23:51:05.912912 useis-0.9.9/useis/sandbox/demo_useis/test/test/TN/config/services_settings
--rw-r--r--   0        0        0    11604 2021-09-26 23:51:05.912912 useis-0.9.9/useis/sandbox/demo_useis/test/test/TN/config/settings.toml
--rw-r--r--   0        0        0      820 2021-09-26 23:51:06.220926 useis-0.9.9/useis/sandbox/demo_useis/test/test/TN/templates/ctrl_template.pickle
--rw-r--r--   0        0        0        0 2021-08-30 00:23:25.795072 useis-0.9.9/useis/services/__init__.py
--rw-r--r--   0        0        0        0 2021-11-04 19:04:06.524406 useis-0.9.9/useis/services/file_server/__init__.py
--rw-r--r--   0        0        0       64 2021-11-04 19:14:43.501659 useis-0.9.9/useis/services/file_server/database.env
--rw-r--r--   0        0        0     1616 2021-11-04 20:15:02.525139 useis-0.9.9/useis/services/file_server/database.py
--rw-r--r--   0        0        0      236 2021-11-04 19:23:38.630074 useis-0.9.9/useis/services/file_server/docker-compose.yml
--rw-r--r--   0        0        0      655 2021-11-04 20:16:48.086081 useis-0.9.9/useis/services/file_server/indexer.py
--rw-r--r--   0        0        0       18 2021-09-27 19:56:13.124036 useis-0.9.9/useis/services/grid_service/.gitignore
--rw-r--r--   0        0        0        0 2021-08-31 09:47:03.774862 useis-0.9.9/useis/services/grid_service/__init__.py
--rw-r--r--   0        0        0     4139 2021-09-09 10:00:34.003524 useis-0.9.9/useis/services/grid_service/client.py
--rw-r--r--   0        0        0     5628 2021-09-28 00:21:07.767580 useis-0.9.9/useis/services/grid_service/server.py
--rw-r--r--   0        0        0       27 2021-09-01 00:37:46.961550 useis-0.9.9/useis/services/grid_service/start_service.sh
--rw-r--r--   0        0        0     1785 2021-09-09 09:55:49.034499 useis-0.9.9/useis/services/grid_service/test.py
--rw-r--r--   0        0        0        0 2021-09-07 00:29:58.307105 useis-0.9.9/useis/services/models/__init__.py
--rw-r--r--   0        0        0      492 2021-09-28 00:49:01.714688 useis-0.9.9/useis/services/models/base.py
--rw-r--r--   0        0        0     3982 2021-09-28 00:46:57.417030 useis-0.9.9/useis/services/models/event.py
--rw-r--r--   0        0        0     1700 2021-09-27 23:55:21.298181 useis-0.9.9/useis/services/models/grid.py
--rw-r--r--   0        0        0     2668 2021-09-28 00:53:25.395320 useis-0.9.9/useis/services/models/nlloc.py
--rw-r--r--   0        0        0        0 2021-03-27 00:51:54.695249 useis-0.9.9/useis/settings/__init__.py
--rw-r--r--   0        0        0      853 2021-11-18 16:22:14.186277 useis-0.9.9/useis/settings/nlloc_settings_template.py
--rw-r--r--   0        0        0      377 2021-11-24 20:46:41.128010 useis-0.9.9/useis/settings/picker_settings_template.toml
--rw-r--r--   0        0        0       46 2021-08-30 18:55:11.540792 useis-0.9.9/useis/settings/services_settings_template.toml
--rw-r--r--   0        0        0      880 2021-08-15 16:17:44.291764 useis-0.9.9/useis/settings/settings.py
--rw-r--r--   0        0        0    11604 2021-03-31 13:44:25.473599 useis-0.9.9/useis/settings/settings_template.toml
--rw-r--r--   0        0        0     1545 2021-11-25 20:12:07.718900 useis-0.9.9/setup.py
--rw-r--r--   0        0        0     1215 2021-11-25 20:12:07.719077 useis-0.9.9/PKG-INFO
+-rw-r--r--   0        0        0     1076 2023-01-15 00:22:18.530236 useis-1.0.0/LICENSE
+-rw-r--r--   0        0        0     1784 2023-05-04 15:07:54.244225 useis-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-01-15 00:22:18.530236 useis-1.0.0/useis/__init__.py
+-rw-r--r--   0        0        0        0 2023-01-15 00:22:18.530236 useis-1.0.0/useis/ai/__init__.py
+-rw-r--r--   0        0        0     5808 2023-01-15 00:27:33.009528 useis-1.0.0/useis/ai/create-picking_dataset.py
+-rw-r--r--   0        0        0     7725 2023-01-15 00:27:33.009528 useis-1.0.0/useis/ai/create_classification_dataset.py
+-rw-r--r--   0        0        0     5121 2023-04-30 10:55:33.035132 useis-1.0.0/useis/ai/database.py
+-rw-r--r--   0        0        0    16324 2023-04-25 01:04:54.358379 useis-1.0.0/useis/ai/dataset.py
+-rw-r--r--   0        0        0      686 2023-04-21 11:24:49.731581 useis-1.0.0/useis/ai/event_type_lookup.py
+-rw-r--r--   0        0        0    25078 2023-04-30 15:50:36.463629 useis-1.0.0/useis/ai/model.py
+-rw-r--r--   0        0        0      248 2023-04-21 13:03:02.416625 useis-1.0.0/useis/ai/params.py
+-rw-r--r--   0        0        0    10310 2023-01-15 00:22:18.530236 useis-1.0.0/useis/ai/resnet1d.py
+-rw-r--r--   0        0        0     2109 2023-01-15 00:22:18.530236 useis-1.0.0/useis/ai/spectrogram.py
+-rw-r--r--   0        0        0        0 2023-01-15 15:22:58.057061 useis-1.0.0/useis/clients/__init__.py
+-rw-r--r--   0        0        0     2474 2023-01-15 23:09:56.931370 useis-1.0.0/useis/clients/test_data.py
+-rw-r--r--   0        0        0        0 2023-01-15 00:22:18.530236 useis-1.0.0/useis/core/__init__.py
+-rw-r--r--   0        0        0    26080 2023-04-25 18:54:53.877703 useis-1.0.0/useis/core/project_manager.py
+-rw-r--r--   0        0        0     2241 2023-01-15 00:22:18.530236 useis-1.0.0/useis/core/projection.py
+-rw-r--r--   0        0        0       37 2023-04-23 11:28:19.261133 useis-1.0.0/useis/examples/classifier/.gitignore
+-rw-r--r--   0        0        0        0 2023-04-15 21:09:31.238146 useis-1.0.0/useis/examples/classifier/__init__.py
+-rw-r--r--   0        0        0      972 2023-04-25 18:54:53.877703 useis-1.0.0/useis/examples/classifier/classifier.py
+-rw-r--r--   0        0        0     6087 2023-05-02 15:29:21.101970 useis-1.0.0/useis/examples/classifier/example.ipynb
+-rw-r--r--   0        0        0        4 2023-01-15 23:17:05.571515 useis-1.0.0/useis/examples/picker/.gitignore
+-rw-r--r--   0        0        0      111 2023-01-15 15:24:07.968314 useis-1.0.0/useis/examples/picker/ai_picker.py
+-rw-r--r--   0        0        0        0 2023-01-15 00:22:18.534236 useis-1.0.0/useis/processors/__init__.py
+-rw-r--r--   0        0        0    13705 2023-03-01 13:50:47.712880 useis-1.0.0/useis/processors/beamforming.py
+-rw-r--r--   0        0        0    55005 2023-05-01 15:31:37.332087 useis-1.0.0/useis/processors/classifier.py
+-rw-r--r--   0        0        0     5627 2023-01-15 00:22:18.534236 useis-1.0.0/useis/processors/data_extractor.py
+-rw-r--r--   0        0        0      534 2023-03-01 13:36:57.561961 useis-1.0.0/useis/processors/file_manager.py
+-rw-r--r--   0        0        0     6759 2023-01-15 00:22:18.534236 useis-1.0.0/useis/processors/interloc.py
+-rw-r--r--   0        0        0     6645 2023-04-04 16:58:44.812525 useis-1.0.0/useis/processors/magnitude.py
+-rw-r--r--   0        0        0    27203 2023-01-15 00:22:18.534236 useis-1.0.0/useis/processors/nlloc.py
+-rw-r--r--   0        0        0    16230 2023-04-27 19:46:27.993238 useis-1.0.0/useis/processors/picker.py
+-rw-r--r--   0        0        0      349 2023-01-15 00:22:18.534236 useis-1.0.0/useis/processors/ray_tracer.py
+-rw-r--r--   0        0        0     2272 2023-01-15 00:22:18.534236 useis-1.0.0/useis/processors/simple_magnitude.py
+-rw-r--r--   0        0        0    20652 2023-01-15 00:22:18.534236 useis-1.0.0/useis/processors/tomography.py
+-rw-r--r--   0        0        0        0 2023-01-15 00:22:18.534236 useis-1.0.0/useis/sandbox/__init__.py
+-rw-r--r--   0        0        0     1167 2023-04-14 00:53:50.522884 useis-1.0.0/useis/sandbox/ai_picker/train_picker.py
+-rw-r--r--   0        0        0      721 2023-01-15 00:22:18.534236 useis-1.0.0/useis/sandbox/demo_kafka/Dockerfile
+-rw-r--r--   0        0        0        0 2023-01-15 00:22:18.534236 useis-1.0.0/useis/sandbox/demo_kafka/__init__.py
+-rw-r--r--   0        0        0     1086 2023-01-15 00:22:18.534236 useis-1.0.0/useis/sandbox/demo_kafka/consumer.py
+-rw-r--r--   0        0        0        2 2023-01-15 00:22:18.534236 useis-1.0.0/useis/sandbox/demo_kafka/demo_kafka.py
+-rw-r--r--   0        0        0     6660 2023-01-15 00:22:18.534236 useis-1.0.0/useis/sandbox/demo_kafka/docker-compose.yml
+-rw-r--r--   0        0        0      456 2023-01-15 00:22:18.534236 useis-1.0.0/useis/sandbox/demo_kafka/producer.py
+-rw-r--r--   0        0        0    13474 2023-03-19 10:30:35.680696 useis-1.0.0/useis/sandbox/event_classification/00_create_training_dataset.py
+-rw-r--r--   0        0        0     1731 2023-04-15 10:41:35.083898 useis-1.0.0/useis/sandbox/event_classification/01_train.py
+-rw-r--r--   0        0        0     6112 2023-04-23 20:46:56.290082 useis-1.0.0/useis/sandbox/event_classification/02_test.py
+-rw-r--r--   0        0        0        0 2023-03-01 01:20:41.974427 useis-1.0.0/useis/sandbox/event_classification/__init__.py
+-rw-r--r--   0        0        0      686 2023-03-10 11:19:47.286141 useis-1.0.0/useis/sandbox/event_classification/event_type_lookup.py
+-rw-r--r--   0        0        0  1484029 2023-04-16 21:56:26.987377 useis-1.0.0/useis/sandbox/event_classification/inventory/OT.xml
+-rw-r--r--   0        0        0  1421855 2023-03-01 00:12:03.885977 useis-1.0.0/useis/sandbox/event_classification/inventory/OT_old.xml
+-rw-r--r--   0        0        0        0 2023-03-01 01:20:41.970427 useis-1.0.0/useis/sandbox/event_classification/inventory/__init__.py
+-rw-r--r--   0        0        0     1726 2023-04-16 21:56:21.783139 useis-1.0.0/useis/sandbox/event_classification/inventory/update_inventory.py
+-rw-r--r--   0        0        0     1040 2023-03-01 13:26:33.688702 useis-1.0.0/useis/sandbox/event_classification/velocity.py
+-rw-r--r--   0        0        0      821 2023-04-30 11:13:53.179373 useis-1.0.0/useis/sandbox/event_classification_2/00_create_dataset.py
+-rw-r--r--   0        0        0      677 2023-05-01 10:46:23.751106 useis-1.0.0/useis/sandbox/event_classification_2/01_train_model.py
+-rw-r--r--   0        0        0     6871 2023-05-02 21:11:07.220700 useis-1.0.0/useis/sandbox/event_classification_2/02_test.py
+-rw-r--r--   0        0        0     1587 2023-01-15 00:22:18.534236 useis-1.0.0/useis/sandbox/tomography/Tomography.ipynb
+-rw-r--r--   0        0        0     1470 2023-01-15 00:22:18.534236 useis-1.0.0/useis/sandbox/tomography/test_tomography.py
+-rw-r--r--   0        0        0        0 2023-01-15 13:48:12.828128 useis-1.0.0/useis/scripts/__init__.py
+-rw-r--r--   0        0        0     5808 2023-01-15 00:27:33.009528 useis-1.0.0/useis/scripts/ai/create-picking_dataset.py
+-rw-r--r--   0        0        0     7725 2023-01-15 00:27:33.009528 useis-1.0.0/useis/scripts/ai/create_classification_dataset.py
+-rw-r--r--   0        0        0     6553 2023-01-15 00:27:33.009528 useis-1.0.0/useis/scripts/ai/create_classification_dataset_1D.py
+-rw-r--r--   0        0        0     9765 2023-01-15 00:27:33.009528 useis-1.0.0/useis/scripts/ai/train_classifier.py
+-rw-r--r--   0        0        0     9799 2023-01-15 00:27:33.009528 useis-1.0.0/useis/scripts/ai/train_classifier_1d.py
+-rw-r--r--   0        0        0     1028 2023-01-15 02:24:36.810810 useis-1.0.0/useis/scripts/ai/train_picker.py
+-rw-r--r--   0        0        0        0 2023-01-15 00:22:18.534236 useis-1.0.0/useis/services/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-02 00:00:54.034334 useis-1.0.0/useis/services/classifier/__init__.py
+-rw-r--r--   0        0        0     1087 2023-04-02 13:11:53.210462 useis-1.0.0/useis/services/classifier/client.py
+-rw-r--r--   0        0        0     2109 2023-05-02 14:56:20.990933 useis-1.0.0/useis/services/classifier/server.py
+-rw-r--r--   0        0        0        0 2023-04-02 00:07:12.075914 useis-1.0.0/useis/services/classifier/settings.toml
+-rw-r--r--   0        0        0       39 2023-04-04 00:52:49.274384 useis-1.0.0/useis/services/classifier/start_service.sh
+-rw-r--r--   0        0        0        0 2023-01-15 00:22:18.534236 useis-1.0.0/useis/services/file_server/__init__.py
+-rw-r--r--   0        0        0       64 2023-01-15 00:22:18.534236 useis-1.0.0/useis/services/file_server/database.env
+-rw-r--r--   0        0        0     1616 2023-01-15 00:22:18.534236 useis-1.0.0/useis/services/file_server/database.py
+-rw-r--r--   0        0        0      236 2023-01-15 00:22:18.534236 useis-1.0.0/useis/services/file_server/docker-compose.yml
+-rw-r--r--   0        0        0      655 2023-01-15 00:22:18.534236 useis-1.0.0/useis/services/file_server/indexer.py
+-rw-r--r--   0        0        0       18 2023-01-15 00:22:18.534236 useis-1.0.0/useis/services/grid_service/.gitignore
+-rw-r--r--   0        0        0        0 2023-01-15 00:22:18.534236 useis-1.0.0/useis/services/grid_service/__init__.py
+-rw-r--r--   0        0        0     4139 2023-01-15 00:22:18.534236 useis-1.0.0/useis/services/grid_service/client.py
+-rw-r--r--   0        0        0     5628 2023-01-15 00:22:18.534236 useis-1.0.0/useis/services/grid_service/server.py
+-rw-r--r--   0        0        0       27 2023-01-15 00:22:18.534236 useis-1.0.0/useis/services/grid_service/start_service.sh
+-rw-r--r--   0        0        0     1785 2023-01-15 00:22:18.534236 useis-1.0.0/useis/services/grid_service/test.py
+-rw-r--r--   0        0        0        0 2023-01-15 00:22:18.534236 useis-1.0.0/useis/services/models/__init__.py
+-rw-r--r--   0        0        0      492 2023-01-15 00:22:18.534236 useis-1.0.0/useis/services/models/base.py
+-rw-r--r--   0        0        0      756 2023-04-04 00:35:32.026107 useis-1.0.0/useis/services/models/classifier.py
+-rw-r--r--   0        0        0     3982 2023-01-15 00:22:18.534236 useis-1.0.0/useis/services/models/event.py
+-rw-r--r--   0        0        0     1700 2023-01-15 00:22:18.534236 useis-1.0.0/useis/services/models/grid.py
+-rw-r--r--   0        0        0     2668 2023-01-15 00:22:18.534236 useis-1.0.0/useis/services/models/nlloc.py
+-rw-r--r--   0        0        0       30 2023-01-23 17:06:39.892533 useis-1.0.0/useis/settings/__init__.py
+-rw-r--r--   0        0        0      225 2023-01-15 00:22:18.534236 useis-1.0.0/useis/settings/beamforming_settings_template.toml
+-rw-r--r--   0        0        0      209 2023-04-25 18:54:53.881703 useis-1.0.0/useis/settings/classifier_settings_template.toml
+-rw-r--r--   0        0        0      237 2023-01-15 00:22:18.534236 useis-1.0.0/useis/settings/interloc_settings_template.toml
+-rw-r--r--   0        0        0      182 2023-01-15 00:22:18.534236 useis-1.0.0/useis/settings/magnitude_settings_template.toml
+-rw-r--r--   0        0        0      853 2023-01-15 00:22:18.534236 useis-1.0.0/useis/settings/nlloc_settings_template.py
+-rw-r--r--   0        0        0      970 2023-01-15 00:22:18.534236 useis-1.0.0/useis/settings/picker_settings_template.toml
+-rw-r--r--   0        0        0       75 2023-01-15 00:22:18.534236 useis-1.0.0/useis/settings/projection_settings_template.toml
+-rw-r--r--   0        0        0       46 2023-01-15 00:22:18.534236 useis-1.0.0/useis/settings/services_settings_template.toml
+-rw-r--r--   0        0        0      893 2023-01-23 16:59:37.680786 useis-1.0.0/useis/settings/settings.py
+-rw-r--r--   0        0        0    12030 2023-03-01 00:12:58.744538 useis-1.0.0/useis/settings/settings_template.toml
+-rw-r--r--   0        0        0       12 2023-01-15 00:22:18.534236 useis-1.0.0/useis/settings/tomography_settings_template.toml
+-rw-r--r--   0        0        0        0 2023-01-15 00:22:18.534236 useis-1.0.0/useis/tomography/__init__.py
+-rwxr-xr-x   0        0        0     5197 2023-01-15 00:22:18.534236 useis-1.0.0/useis/tomography/data.py
+-rw-r--r--   0        0        0     1745 1970-01-01 00:00:00.000000 useis-1.0.0/setup.py
+-rw-r--r--   0        0        0     1260 1970-01-01 00:00:00.000000 useis-1.0.0/PKG-INFO
```

### Comparing `useis-0.9.9/LICENSE` & `useis-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `useis-0.9.9/useis/ai/dataset.py` & `useis-1.0.0/useis/ai/dataset.py`

 * *Files 24% similar despite different names*

```diff
@@ -8,37 +8,21 @@
 from pathlib import Path
 from os.path import sep
 from loguru import logger
 from torchaudio.transforms import MelSpectrogram, AmplitudeToDB
 from uquake.core.trace import Trace
 from abc import ABC
 import pickle
+from .params import *
+from typing import List, Dict
+import random
+from torchvision import transforms
+from ipdb import set_trace
 
 
-# class Label():
-#     def __init__(self, labels):
-#         self.full_labels = list(labels)
-#         self.labels = range(0, len(labels))
-#
-#         self.unique_labels = np.unique(labels)
-#         self.unique_numerical_labels = np.range(len(self.unique_labels))
-#
-#         self.labels_dict = {}
-#         for full_label, label  in zip(labels, self.unique_labels):
-#             self.labels_dict[full_label] = label
-#
-#     def __len__(self):
-#         return len(self.labels)
-#
-#     def __getitem__(self, item):
-#         label = self.full_labels[item]
-#         return self.labels_dict[label]
-#
-#     def get_full_label(self, item):
-
 def get_file_list(input_directory, suffix, extension='png'):
     path = os.path.join(input_directory, '*', f'*{suffix}.{extension}')
     return glob(path)
 
 
 def split_dataset(path, split=0.8, seed=None, max_item_per_category=100000):
     """
@@ -96,107 +80,119 @@
                                                  =number)
 
     def select1d(self, number):
         return ClassifierDataset1D.from_file_list(self,
                 max_number_signal_per_category=number)
 
 
-class SpectrogramDataset(Dataset):
-
-    def __init__(self, file_dict: dict,
-                 max_number_image_per_category: int = 1e5,
-                 seed: int = None):
-
-        categories = [key for key in file_dict.keys()]
-        self.category_list = categories
-        self.labels = np.arange(len(categories))
-
-        np.random.seed(seed)
-        self.labels_dict = {}
-        self.file_list = []
-        self.label_list = []
-        for category, label in zip(categories, self.labels):
-            self.labels_dict[category] = label
-            nb_files = int(max_number_image_per_category)
-            if len(file_dict[category]) < nb_files:
-                nb_files = int(len(file_dict[category]))
-            for f in np.random.choice(file_dict[category],
-                                      size=nb_files,
-                                      replace=False):
-                self.file_list.append(f)
-                self.label_list.append(label)
-
-        self.file_list = np.array(self.file_list)
-        self.label_list = np.array(self.label_list)
-
-    @classmethod
-    def from_file_list(cls, file_list: FileList,
-                       max_number_image_per_category=1e5, seed=None):
-        return cls(file_list.cat_file_list,
-                   max_number_image_per_category=max_number_image_per_category,
-                   seed=seed)
-
-    def __len__(self):
-        return len(self.file_list)
-
-    def __getitem__(self, idx):
-        if torch.is_tensor(idx):
-            idx = idx.tolist()
-
-        # label = self.df_data.iloc[idx]['label']
-        # category = self.category_list[idx]
-        label = self.label_list[idx]
-
-        image = torch.from_numpy((np.array(Image.open(
-            self.file_list[idx])) / 255).astype(np.float32))
 
-        # return {'data': image, 'label': label}
-        return image, label
-
-    @property
-    def shape(self):
-        px_x, px_y = self[0][0].shape
-        return len(self.label_list), px_x, px_y
-
-    @property
-    def nb_pixel(self):
-        return np.prod(self[0][0].shape)
-
-    @property
-    def categories(self):
-        return self.labels_dict
-
-    @property
-    def classes(self):
-        return self.categories
-
-    @property
-    def nb_categories(self):
-        return len(self.category_list)
-
-
-sampling_rate = 6000
-# num_threads = int(np.ceil(cpu_count() - 10))
-num_threads = 10
-replication_level = 5
-snr_threshold = 10
-sequence_length_second = 2
-perturbation_range_second = 1
-image_width = 128
-image_height = 128
-buffer_image_fraction = 0.05
+    # def __init__(self, base_path, image_files, categories, bounding_boxes, event_ids):
+    #     self.base_path = Path(base_path)
+    #     self.image_files = image_files
+    #     self.categories = categories
+    #     self.event_ids = event_ids
+
+
+    # def __init__(self, file_dict: dict,
+    #              max_number_image_per_category: int = 1e5,
+    #              seed: int = None):
+    #
+    #     categories = [key for key in file_dict.keys()]
+    #     self.category_list = categories
+    #     self.labels = np.arange(len(categories))
+    #
+    #     np.random.seed(seed)
+    #     self.labels_dict = {}
+    #     self.file_list = []
+    #     self.label_list = []
+    #     for category, label in zip(categories, self.labels):
+    #         self.labels_dict[category] = label
+    #         nb_files = int(max_number_image_per_category)
+    #         if len(file_dict[category]) < nb_files:
+    #             nb_files = int(len(file_dict[category]))
+    #         for f in np.random.choice(file_dict[category],
+    #                                   size=nb_files,
+    #                                   replace=False):
+    #             self.file_list.append(f)
+    #             self.label_list.append(label)
+    #
+    #     self.file_list = np.array(self.file_list)
+    #     self.label_list = np.array(self.label_list)
+    #
+    # @classmethod
+    # def from_file_list(cls, file_list: FileList,
+    #                    max_number_image_per_category=1e5, seed=None):
+    #     return cls(file_list.cat_file_list,
+    #                max_number_image_per_category=max_number_image_per_category,
+    #                seed=seed)
+    #
+    # def __len__(self):
+    #     return len(self.file_list)
+    #
+    # def __getitem__(self, idx):
+    #     if torch.is_tensor(idx):
+    #         idx = idx.tolist()
+    #
+    #     # label = self.df_data.iloc[idx]['label']
+    #     # category = self.category_list[idx]
+    #     label = self.label_list[idx]
+    #
+    #     image = torch.from_numpy((np.array(Image.open(
+    #         self.file_list[idx])) / 255).astype(np.float32))
+    #
+    #     # return {'data': image, 'label': label}
+    #     return image, label
+    #
+    # @property
+    # def shape(self):
+    #     px_x, px_y = self[0][0].shape
+    #     return len(self.label_list), px_x, px_y
+    #
+    # @property
+    # def nb_pixel(self):
+    #     return np.prod(self[0][0].shape)
+    #
+    # @property
+    # def categories(self):
+    #     return self.labels_dict
+    #
+    # @property
+    # def classes(self):
+    #     return self.categories
+    #
+    # @property
+    # def nb_categories(self):
+    #     return len(self.category_list)
+# sampling_rate = 6000
+# # num_threads = int(np.ceil(cpu_count() - 10))
+# num_threads = 10
+# replication_level = 5
+# snr_threshold = 10
+# # sequence_length_second = 2
+# perturbation_range_second = 1
+# image_width = 128
+# image_height = 128
+# buffer_image_fraction = 0.05
 
 buffer_image_sample = int(image_width * buffer_image_fraction)
 
-hop_length = int(sequence_length_second * sampling_rate //
-                 (image_width + 2 * buffer_image_sample))
+# hop_length = int(sequence_length_second * sampling_rate //
+#                  (image_width + 2 * buffer_image_sample))
 
 
 def spectrogram(trace: Trace):
 
+    sequence_length_second = trace.stats.endtime - trace.stats.starttime
+    # sampling_rate = trace.stats.sampling_rate
+    trace.detrend('demean').detrend('linear').taper(max_percentage=0.1, max_length=0.01)
+    # from ipdb import set_trace
+    # set_trace()
+    hop_length = int(np.floor(sequence_length_second * sampling_rate /
+                              (image_width + 2 * buffer_image_sample)))
+
     trace.resample(sampling_rate)
 
     mel_spec = MelSpectrogram(sample_rate=sampling_rate,
                               n_mels=image_height,
                               hop_length=hop_length,
                               power=1,
                               pad_mode='reflect',
@@ -204,25 +200,28 @@
 
     amplitude_to_db = AmplitudeToDB()
 
     # trace = trace.detrend('linear')
     # trace = trace.detrend('demean')
     trace.data = trace.data - np.mean(trace.data)
     trace = trace.taper(max_length=0.01, max_percentage=0.05)
-    trace = trace.trim(starttime=trace.stats.starttime,
-                       endtime=trace.stats.starttime + sequence_length_second,
-                       pad=True, fill_value=0)
+    # trace = trace.trim(starttime=trace.stats.starttime,
+    #                    endtime=trace.stats.starttime + sequence_length_second,
+    #                    pad=True, fill_value=0)
     data = trace.data
 
     torch_data = torch.tensor(data).type(torch.float32)
 
     spec = (mel_spec(torch_data))
     spec_db = amplitude_to_db(spec.abs() + 1e-3)
     spec_db = (spec_db - spec_db.min()).numpy()
-    # spec_db = (spec_db / spec_db.max()).type(torch.float32)
+    spec_db = spec_db[:, buffer_image_sample:-buffer_image_sample]
+    if spec_db.shape[1] > image_width:
+        spec_db = spec_db[:, spec_db.shape[1] - image_width:]
+    # spec_db = (s pec_db / spec_db.max()).type(torch.float32)
     return spec_db
 
 
 class ClassifierDataset1D(Dataset):
 
     def __init__(self, file_dict: dict,
                  max_number_signal_per_category: int = 1e5,
@@ -281,15 +280,15 @@
                 data_out = data[0:self.shape[1]]
             else:
                 data_out[0: len(data)] = data
         else:
             data_out = data
 
         data_out -= np.mean(data_out)
-        data_out /= np.max(data_out)
+        data_out /= np.max(np.abs(data_out))
 
         data_out = torch.from_numpy((np.array(data_out).astype(np.float32)))
 
         return data_out, label
 
     @property
     def shape(self):
@@ -305,14 +304,19 @@
         return self.categories
 
     @property
     def nb_categories(self):
         return len(self.category_list)
 
 
+class ClassificationDataset(Dataset):
+    def __init__(self, spectrograms: list, label: list):
+        self.spectrograms_images
+
+
 class PickingDataset(Dataset):
     def __init__(self, file_list):
         self.file_list = file_list
 
     def __len__(self):
         return len(self.file_list)
 
@@ -320,40 +324,185 @@
         if torch.is_tensor(idx):
             idx = idx.tolist()
 
         with open(self.file_list[idx], 'rb') as f_in:
             data = pickle.load(f_in)
 
         signal = data['data'].astype(np.float32)
+        # signal += np.min(signal)
+        # signal = np.abs(signal) / np.abs(signal)
 
         # ensuring the signal is between -1 and 1
         signal = signal - np.mean(signal)
-        signal = signal / np.max(signal)
+        signal = signal / np.max(np.abs(signal))
+
+        signal[np.isnan(signal)] = 0
 
         target = data['pick']
+        if np.isnan(target):
+            targer = 0
 
         return signal.astype(np.float32), np.float32(target)
 
     @property
     def shape(self):
         len_signal = self[0][0].shape
         return 1, len_signal[0]
 
-    def split(self, split_fraction: float = 0.8, random_seed: int = None):
+    def split(self, split_fraction: float = 0.8, random_seed: int = 24):
         np.random.seed(random_seed)
         choices = np.random.choice([False, True], size=len(self),
                                    p=[1 - split_fraction, split_fraction])
         not_choices = np.invert(choices)
         files_set_a = np.array(self.file_list)[choices]
         files_set_b = np.array(self.file_list)[not_choices]
 
         set_a = PickingDataset(files_set_a)
         set_b = PickingDataset(files_set_b)
 
         return set_a, set_b
 
 
+class SpectrogramDataset(Dataset):
+    def __init__(self, file_list: List[Dict], labels: List[int], labels_mapping: Dict,
+                 random_seed: int = 10):
+        self.file_list = file_list
+        self.labels = labels
+        self.random_seed = random_seed
+        self.window_lengths = []
+
+        self.unique_labels = np.unique(self.labels)
+        self.label_mapping = labels_mapping
+
+        # Set random seed for reproducibility
+        random.seed(self.random_seed)
+
+        # Define image transforms
+    @classmethod
+    def transform(cls, image):
+        transform = transforms.Compose([
+            transforms.Resize((224, 224)),
+            transforms.ToTensor(),
+            transforms.Normalize(mean=[0.5, 0.5, 0.5], std=[0.5, 0.5, 0.5])
+        ])
+        return transform(image)
+
+    def get_label(self, label_vect):
+        for key in self.label_mapping.keys():
+            if np.all(self.label_mapping[key] == np.array(label_vect)):
+                break
+        return key
+
+    @property
+    def num_classes(self):
+        return len(self.unique_labels)
+
+    def __len__(self):
+        return len(self.file_list)
+
+    def __getitem__(self, idx):
+        # Load the three channel images and combine them into an RGB image
+        red_image_path = self.file_list[idx]['s1']
+        green_image_path = self.file_list[idx]['s2']
+        blue_image_path = self.file_list[idx]['s3']
+        red_image = Image.open(red_image_path)
+        green_image = Image.open(green_image_path)
+        blue_image = Image.open(blue_image_path)
+        rgb_image = self.merge_reshape(red_image, green_image, blue_image)
+
+        # Get the corresponding label
+        label = self.label_mapping[self.labels[idx]]
+
+        return rgb_image, label
+
+    @classmethod
+    def merge_reshape(cls, short, medium, long):
+        """
+
+        @param short: spectrogram from the short window
+        @param medium: spectrogram from the medium size window
+        @param long: spectrogram from the long window
+        @return: the merge and transformed image
+        """
+        rgb = cls.transform(Image.merge("RGB", (short, medium, long)))
+        return rgb
+
+
+class SpectrogramDataset2(Dataset):
+    def __init__(self, file_list: List[Dict], labels: List[int], labels_mapping: Dict,
+                 random_seed: int = 10):
+        self.file_list = file_list
+        self.labels = labels
+        self.random_seed = random_seed
+        self.window_lengths = []
+
+        self.unique_labels = np.unique(self.labels)
+        self.label_mapping = labels_mapping
+
+        # Set random seed for reproducibility
+        random.seed(self.random_seed)
+
+        # Define image transforms
+    @classmethod
+    def transform(cls, image):
+        transform = transforms.Compose([
+            transforms.Resize((224, 224)),
+            transforms.Grayscale(num_output_channels=1),
+            transforms.ToTensor(),
+            transforms.Normalize(mean=[0.5], std=[0.5])
+        ])
+
+        ts_image = transform(image)
+        image_tensor = ts_image
+        # image_tensor = ts_image.unsqueeze(0)
+        return image_tensor
+
+    def get_label(self, label_vect):
+        for key in self.label_mapping.keys():
+            if np.all(self.label_mapping[key] == np.array(label_vect)):
+                break
+        return key
+
+    @property
+    def num_classes(self):
+        return len(self.unique_labels)
+
+    def __len__(self):
+        return len(self.file_list)
+
+    def __getitem__(self, idx):
+        # Load the three channel images and combine them into an RGB image
+        # red_image_path = self.file_list[idx]['s1']
+        # green_image_path = self.file_list[idx]['s2']
+        # blue_image_path = self.file_list[idx]['s3']
+        # red_image = Image.open(red_image_path)
+        # green_image = Image.open(green_image_path)
+        # blue_image = Image.open(blue_image_path)
+        # rgb_image = self.merge_reshape(red_image, green_image, blue_image)
+
+        # Get the corresponding label
+        label = self.label_mapping[self.labels[idx]]
+        image = Image.open(self.file_list[idx]['s1'])
+
+        return self.transform(image), label
+
+    # @classmethod
+    # def merge_reshape(cls, short, medium, long):
+    #     """
+    #
+    #     @param short: spectrogram from the short window
+    #     @param medium: spectrogram from the medium size window
+    #     @param long: spectrogram from the long window
+    #     @return: the merge and transformed image
+    #     """
+    #     rgb = cls.transform(Image.merge("RGB", (short, medium, long)))
+    #     return rgb
+
+
+
+
+
```

### Comparing `useis-0.9.9/useis/ai/model.py` & `useis-1.0.0/useis/ai/model.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,91 +1,118 @@
 from torchvision import models
+from torchvision.models import resnet34
 from .dataset import (Dataset, PickingDataset, ClassifierDataset1D,
                       spectrogram)
 from torch.utils.data import DataLoader
 import torch
 from torch import nn
 import numpy as np
 from loguru import logger
 from tqdm import tqdm
 import pickle
 from sklearn.metrics import confusion_matrix
 # from plotcm import plot_confusion_matrix
-from uquake.core import Stream, Trace
+from uquake.core import Stream, Trace, UTCDateTime
 # from torchaudio.transforms import MelSpectrogram, AmplitudeToDB
 from PIL import Image, ImageOps
 from torch import nn
 from .resnet1d import ResNet1D
 from importlib import reload
-# from .dataset as dataset
-# reload(dataset)
+from ipdb import set_trace
+# import urllib.request
+import requests
+from io import BytesIO
+from uquake.core.util.requests import download_file_from_url
+
+from .params import *
+
+
+# class SeismicResnet34(type(resnet34())):
+#     def __init__(self, num_input_channels=3, n_out_features=3):
+#         super(SeismicResnet34, self).__init__()
+#         self.conv1 = nn.Conv2d(num_input_channels, 64, kernel_size=7, stride=2,
+#                                padding=3, bias=False)
+#
+#         self.fc = nn.Linear(self.fc.in_features, n_out_features)
 
 
-sampling_rate = 6000
-# num_threads = int(np.ceil(cpu_count() - 10))
-num_threads = 10
-replication_level = 5
-snr_threshold = 10
-sequence_length_second = 2
-perturbation_range_second = 1
-image_width = 128
-image_height = 128
-buffer_image_fraction = 0.05
+class EventClassifier(object):
 
+    model_url = \
+            'https://www.dropbox.com/s/5d76v8hfi3dwsm0/classification_model.useis?dl=1'
+    n_out_features = 3
+    label_mapping = {
+        'noise': np.array([1., 0., 0.]),
+        'blast': np.array([0., 1., 0.]),
+        'seismic event': np.array([0., 0., 1.])
+    }
 
-class EventClassifier(object):
-    def __init__(self, n_features: int, gpu: bool = True):
+    def __init__(self, gpu: bool = True, learning_rate: float = 0.001, model_id=None,
+                 model=models.resnet34(), weight_decay: float = 0.001):
 
         # define the model
-        self.model = models.resnet34(pretrained=False)
-        self.model.conv1 = nn.Conv2d(1, 64, kernel_size=7, stride=2, padding=3,
-                                     bias=False)
+        self.model = model
+        num_input_channels = 3
+        self.num_imput_channels = num_input_channels
+        self.model.conv1 = nn.Conv2d(num_input_channels, 64, kernel_size=7, stride=2,
+                                     padding=3, bias=False)
+
+        self.model.fc = nn.Linear(self.model.fc.in_features, self.n_out_features)
+
+        self.model_id = model_id
+
+        self.n_features = self.n_out_features
+        self.num_classes = self.n_out_features
+        self.learning_rate = learning_rate
+        self.weight_decay = weight_decay
+
+        # Replace the last fully-connected layer to output the desired number of classes
+        self.model.fc = nn.Linear(self.model.fc.in_features, self.n_out_features)
+
+        # self.optimizer = torch.optim.SGD(self.model.parameters(), lr=learning_rate)
+        self.optimizer = torch.optim.Adam(self.model.parameters(), lr=learning_rate,
+                                          weight_decay=weight_decay)
+        self.criterion = nn.CrossEntropyLoss()
+        self.gpu = gpu
 
-        self.n_features = n_features
+        self.device = self.select_device(gpu=gpu)
 
-        self.model.fc = nn.Linear(self.model.fc.in_features, n_features)
+        self.model = self.model.to(self.device)
+        self.accuracies = []
+        self.losses = []
 
-        self.optimizer = torch.optim.Adam(self.model.parameters())
-        self.criterion = nn.CrossEntropyLoss()
-        self.gpu = gpu
+        self.iteration = 0
+        # Download the model from Dropbox
 
+    @classmethod
+    def from_pretrained_model(cls, model, gpu: bool = True):
+        cls_tmp = cls(gpu=gpu, model=model)
+        # cls_tmp.model = model.to(cls_tmp.device)
+        return cls_tmp
+
+    @staticmethod
+    def select_device(gpu=True):
         if gpu:
             device = torch.device("cuda:0" if
                                   torch.cuda.is_available() else "cpu")
             if device == "cpu":
                 logger.warning('GPU is not available, the CPU will be used')
             else:
                 logger.info('GPU will be used')
         else:
-            device = 'cpu'
+            device = torch.device('cpu')
             logger.info('The CPU will be used')
 
-        self.device = device
-
-        self.model = self.model.to(self.device)
-        self.display_memory()
-        self.accuracies = []
-        self.losses = []
+        return device
 
-        self.validation_predictions = None
-        self.validation_targets = None
 
     @classmethod
-    def from_pretrained_model(cls, model, gpu: bool = True):
-        n_features = model.fc.out_features
-        cls_tmp = cls(n_features, gpu=gpu)
-        cls_tmp.model = model.to(cls_tmp.device)
-
-        return cls_tmp
-
-    @classmethod
-    def from_pretrained_model_file(cls, path, gpu: bool = True):
-        with open(path, 'rb') as input_file:
-            model = pickle.load(input_file)
-
+    def from_pretrained_model_file(cls, file_name, gpu: bool = True):
+        # with open(path, 'rb') as input_file:
+        model = torch.load(file_name, map_location=cls.select_device(gpu=gpu))
         return cls.from_pretrained_model(model, gpu=gpu)
 
     # @classmethod
     # def load_model(cls, file_name):
     #     return pickle.load(open('filename', 'rb'))
 
     def train(self, dataset: Dataset, batch_size: int):
@@ -95,19 +122,20 @@
         self.accuracies = []
         self.losses = []
 
         training_loader = DataLoader(dataset, batch_size=batch_size,
                                      shuffle=True)
 
         for inputs, targets in tqdm(training_loader):
-            inputs = inputs.view(inputs.size()[0], -1, inputs.size()[1],
-                                 inputs.size()[2])
             self.iterate(inputs, targets)
             torch.cuda.empty_cache()
 
+    def forward(self, x):
+        return self.model.forward(x)
+
     def iterate(self, inputs, targets):
 
         self.optimizer.zero_grad()
 
         inputs = inputs.to(self.device)
         targets = targets.to(self.device)
 
@@ -115,100 +143,202 @@
         predictions = self.model(inputs)
 
         loss = self.criterion(predictions, targets)
         # loss.requires_grad = True
         loss.backward()
         self.optimizer.step()
 
-        self.accuracies.append(self.measure_accuracy(targets,
-                                                     predictions).item())
+        target_indices = torch.argmax(targets, dim=1)
+        predicted_indices = torch.argmax(predictions, dim=1)
+        loss = self.criterion(predictions, target_indices)
+        accuracy = (target_indices == predicted_indices).sum() / len(target_indices)
+        self.accuracies.append(accuracy.item())
         self.losses.append(loss.item())
+        self.iteration += 1
 
     def validate(self, dataset: Dataset, batch_size: int):
         self.model.eval()
         training_loader = DataLoader(dataset, batch_size=batch_size,
                                      shuffle=True)
         self.validation_targets = np.zeros(len(dataset))
         self.validation_predictions = np.zeros(len(dataset))
-        accuracy = 0
-        for i, (inputs, targets) in enumerate(tqdm(training_loader)):
-            inputs = inputs.view(inputs.size()[0], -1, inputs.size()[1],
-                                 inputs.size()[2])
-            inputs = inputs.to(self.device)
-
-            start = batch_size * i
-            end = start + batch_size
-            self.validation_targets[start:end] = targets
-            targets = targets.to(self.device)
-
-            # with torch.no_grad() pytorch does not compute the gradient,
-            # the gradient takes a significant amount of memory on the gpu.
-            # using torch.no_grad() consequently allows significantly
-            # increasing the batch size
-            with torch.no_grad():
+        accuracy = []
+        loss = []
+        with torch.no_grad():
+            for i, (inputs, targets) in enumerate(tqdm(training_loader)):
+                # inputs = inputs.view(inputs.size()[0], -1, inputs.size()[1],
+                #                      inputs.size()[2])
+                inputs = inputs.to(self.device)
+
+                start = batch_size * i
+                end = start + batch_size
+                self.validation_targets[start:end] = torch.argmax(targets).cpu().numpy()
+                targets = targets.to(self.device)
+
+                # with torch.no_grad() pytorch does not compute the gradient,
+                # the gradient takes a significant amount of memory on the gpu.
+                # using torch.no_grad() consequently allows significantly
+                # increasing the batch size
+                # with torch.no_grad():
                 outputs = self.model(inputs)
 
-            self.validation_predictions[start:end] = outputs.max(dim=1)[1].cpu(
-            ).detach().numpy()
+                self.validation_predictions[start:end] = torch.argmax(
+                    outputs).cpu().numpy()
 
-            accuracy += self.measure_accuracy(targets, outputs)
+                target_indices = torch.argmax(targets, dim=1)
+                predicted_indices = torch.argmax(outputs, dim=1)
+                tmp = (target_indices == predicted_indices).sum() / len(target_indices)
+                accuracy.append(float(tmp.cpu().numpy()))
+                loss.append(float(self.criterion(outputs, target_indices).cpu().numpy()))
         self.model.train()
-        return accuracy.cpu().detach().numpy() / (i + 1)
+        return accuracy, loss
 
     def display_memory(self):
         torch.cuda.empty_cache()
         memory = torch.cuda.memory_allocated(self.device)
         logger.info("{:.3f} GB".format(memory / 1024 ** 3))
 
+    # @property
+    # def model_state(self):
+    #     self.model.to('cpu')
+    #     out_dict = {'model_state': self.model.state_dict(),
+    #                 'out_features': self.n_features,
+    #                 'label_map': self.label_mapping,
+    #                 'learning_rate': self.learning_rate,
+    #                 'model_id': self.model_id}
+    #     return out_dict
+
     def save(self, file_name):
-        return pickle.dump(self, open(file_name, 'wb'))
+        return torch.save(self.model.state_dict(), file_name)
 
     def write(self, file_name):
         return self.save(file_name)
 
     @classmethod
-    def read(cls, file_name):
-        with open(file_name, 'rb') as f_in:
-            return pickle.load(f_in)
+    def from_model_state(cls, state_dict, gpu=True):
+        ec = cls(gpu=gpu)
+        ec.model.load_state_dict(state_dict)
+        ec.model.eval()
+        ec.model.to(cls.select_device(gpu=gpu))
+        return ec
+
+    @classmethod
+    def read(cls, file_name, gpu=True):
+        device = cls.select_device(gpu=gpu)
+        state_dict = torch.load(file_name, map_location=device)
+        # model_state = pickle.load(open(file_name, 'rb'))
+        return cls.from_model_state(state_dict, gpu=gpu)
+
+    @classmethod
+    def load(cls, gpu=True):
+        """
+        load the most recent model
+        """
+
+        model_data = download_file_from_url(cls.model_url)
+
+        # Load the model from the BytesIO object
+
+        device = cls.select_device(gpu=gpu)
+
+        state_dict = torch.load(model_data, map_location=device)
+        return cls.from_model_state(state_dict, gpu=gpu)
+        # model = MyModel(...)
+        # model.model.load_state_dict(state_dict['model_state'])
+        # model.n_features = state_dict['out_features']
+        # model.label_mapping = state_dict['label_map']
+        # model.learning_rate = state_dict['learning_rate']
+        # model.model_id = state_dict['model_id']
 
     @staticmethod
     def measure_accuracy(targets, predictions):
         max_index = predictions.max(dim=1)[1]
         return (max_index == targets).sum() / len(targets)
 
-    def predict(self, stream: Stream):
-        """
 
-        :param stream: A uquake.core.stream.Stream object containing the
-        waveforms
-        :return:
-        """
-        specs = generate_spectrogram(stream)
-        return self.predict_spectrogram(specs)
+class EventClassifier2(EventClassifier):
+    model_url = 'https://www.dropbox.com/s/klk2nfalqt8ugjj/1s_model_2023_04_30.pt?dl=1'
 
-    def predict_spectrogram(self, specs):
-        self.model.eval()
-        if isinstance(specs, list):
-            specs = np.array(specs)
-        if len(specs.shape) == 2:
-            specs = torch.from_numpy(specs).view(1, 1, specs.shape[0],
-                                                 specs.shape[1])
-        else:
-            specs = torch.from_numpy(specs).view(specs.shape[0], 1,
-                                                 specs.shape[1],
-                                                 specs.shape[2])
+    def __init__(self, gpu: bool = True,
+                 learning_rate: float = 0.001, model=models.resnet34(), model_id=None,
+                 weight_decay: float = 0.001, dropout_prob: float = 0.3):
+        super().__init__(gpu=gpu,
+                         learning_rate=learning_rate, model_id=model_id, model=model,
+                         weight_decay=weight_decay)
+        self.num_input_channels = 1
 
-        specs = specs.to(self.device)
-        # self.model.train()
-        with torch.no_grad():
-            predictions = (self.model(specs).argmax(axis=1).cpu(),
-                           self.model(specs).cpu())
+        self.model.conv1 = nn.Conv2d(self.num_input_channels, 64, kernel_size=7,
+                                     stride=2, padding=3, bias=False)
 
-        self.model.train()
-        return predictions
+        self.model.to(self.device)
+
+        self.dropout = nn.Dropout(p=dropout_prob)
+
+    def forward(self, x):
+        x = self.resnet34.conv1(x)
+        x = self.resnet34.bn1(x)
+        x = self.resnet34.relu(x)
+        x = self.resnet34.maxpool(x)
+
+        # Stage 1
+        x = self.resnet34.layer1(x)
+
+        # Stage 2
+        x = self.resnet34.layer2(x)
+
+        # Stage 3
+        x = self.resnet34.layer3(x)
+
+        # Stage 4
+        x = self.resnet34.layer4(x)
+
+        # Apply dropout to the output of the last convolutional layer
+        x = self.dropout(x)
+
+        x = self.resnet34.avgpool(x)
+        x = x.view(x.size(0), -1)
+        x = self.resnet34.fc(x)
+        return x
+
+    @staticmethod
+    def trace2spectrogram(trace: Trace):
+        return generate_spectrogram(Stream(traces=[trace]))
+
+    @staticmethod
+    def stream2spectrogram(stream: Stream):
+        return generate_spectrogram(stream)
+
+    @property
+    def model_state(self):
+        out_dict = {'model_state': self.model.state_dict(),
+                    'out_features': self.n_features,
+                    'label_map': self.label_mapping,
+                    'learning_rate': self.learning_rate,
+                    'model_id': self.model_id}
+        return out_dict
+
+    # def save(self, file_name):
+    #     return pickle.dump(self.model_state, open(file_name, 'wb'))
+    #
+    # def write(self, file_name):
+    #     return self.save(file_name)
+    #
+    # @classmethod
+    # def from_model_state(cls, model_state, gpu=True):
+    #     ec = cls(model_state['out_features'], model_state['label_map'],
+    #              gpu=gpu, learning_rate=model_state['learning_rate'],
+    #              model_id=model_state['model_id'])
+    #     ec.model.load_state_dict(model_state['model_state'])
+    #     ec.model.eval()
+    #     return ec
+
+    # @classmethod
+    # def read(cls, file_name, gpu=True):
+    #     model_state = pickle.load(open(file_name, 'rb'))
+    #     return cls.from_model_state(model_state, gpu=gpu)
 
 
 def read_classifier(file_name):
     return EventClassifier.read(file_name)
 
 
 def generate_spectrogram(stream: Stream):
@@ -218,34 +348,33 @@
     for tr in stream.copy():
         # check if tr contains NaN
         if np.any(np.isnan(tr.data)):
             continue
         trs.append(tr.copy())
 
     st2 = Stream(traces=trs)
-    st2 = st2.trim(endtime=tr.stats.starttime + 2, pad=True,
-                 fill_value=0)
     st2 = st2.detrend('demean').detrend('linear')
 
     st2 = st2.taper(max_percentage=1, max_length=1e-2)
 
     for tr in st2:
         spec = spectrogram(tr)
         spec /= np.max(spec)
-
+        spec = spec / np.max(spec) * 255
+        spec = Image.fromarray(np.array(spec.tolist()).astype(np.uint8))
         specs.append(spec)
 
     return specs
 
 
 class EventClassifier1D(EventClassifier):
     def __init__(self, n_classes: int, in_channels: int = 1,
                  base_filters: int = 16, kernel_size: int = 7,
                  stride: int = 3, groups: int = 1, n_block: int = 8,
-                 learning_rate=1e-3, gpu: bool = True):
+                 learning_rate=1e-3, gpu: bool = True, weight_decay: float = 0.001):
 
         if gpu:
             device = torch.device("cuda:0" if
                                   torch.cuda.is_available() else "cpu")
             if device == "cpu":
                 logger.warning('GPU is not available, the CPU will be used')
             else:
@@ -272,20 +401,21 @@
         self.gpu = gpu
 
         self.model = ResNet1D(in_channels, base_filters, kernel_size,
                               stride, groups, n_block,
                               n_classes).to(self.device)
 
         self.optimizer = torch.optim.Adam(self.model.parameters(),
-                                          lr=learning_rate)
+                                          lr=learning_rate,
+                                          weight_decay=weight_decay)
         # self.optimizer = torch.optim.SGD(self.model.parameters(),
         #                                  lr=learning_rate)
         self.criterion = nn.CrossEntropyLoss()
 
-        self.display_memory()
+        # self.display_memory()
         self.losses = []
 
         self.validation_predictions = None
         self.validation_targets = None
 
     def train(self, dataset: ClassifierDataset1D, batch_size: int):
 
@@ -310,14 +440,15 @@
         loss = self.criterion(predictions, targets)
         # print(loss.item())
         loss.backward()
         self.optimizer.step()
 
         # print(loss.item())
         self.losses.append(loss.cpu().item())
+        self.iteration += 1
 
     def validate(self, dataset: ClassifierDataset1D, batch_size: int):
         self.model.eval()
         training_loader = DataLoader(dataset, batch_size=batch_size,
                                      shuffle=True)
         self.validation_targets = np.zeros(len(dataset))
         self.validation_predictions = np.zeros(len(dataset))
@@ -378,89 +509,85 @@
         out = self.conv_layers(X)
         out = out.view(out.size(0), -1)
         out = self.dense_layers(out)
         # input(out)
         return out
 
 
-class AIPicker(EventClassifier):
+# class AIPicker(EventClassifier):
+class AIPicker(object):
     def __init__(self, in_channels: int = 1, base_filters: int = 64,
                  kernel_size: int = 15, stride: int = 3, n_classes: int = 1,
-                 groups: int = 1, n_block: int = 16, learning_rate=1e-3,
-                 gpu: bool = True):
+                 groups: int = 1, n_block: int = 16, learning_rate=1e-5,
+                 gpu: bool = True, n_sample: int = 256,
+                 sampling_rate: int=6000, to_device=True):
         self.in_channels = in_channels
         self.base_filters = base_filters
         self.kernel_size = kernel_size
         self.stride = stride
         self.n_classes = n_classes
         self.groups = groups
         self.n_block = n_block
         self.gpu = gpu
+        self.n_sample = n_sample
+        self.sampling_rate = sampling_rate
 
         if gpu:
             device = torch.device("cuda:0" if
                                   torch.cuda.is_available() else "cpu")
             if device == "cpu":
                 logger.warning('GPU is not available, the CPU will be used')
             else:
                 logger.info('GPU will be used')
         else:
             device = 'cpu'
             logger.info('The CPU will be used')
 
         self.device = device
 
-        self.model = ResNet1D(in_channels, base_filters, kernel_size,
-                              stride, groups, n_block,
-                              n_classes).to(self.device)
-
-        # self.model = PickerModel().to(device)
+        self.model = self.init_model()
 
-        # self.model = nn.Sequential(
-        #     nn.Conv1d(1, 64, 16),
-        #     nn.Conv1d(64, 64, 16),
-        #     nn.Conv1d(64, 64, 16),
-        #     nn.Conv1d(64, 128, 16),
-        #     nn.Conv1d(128, 128, 16),
-        #     nn.Conv1d(128, 128, 16),
-        #     nn.Linear(in_features=12 * 15, out_features=120),
-        #     nn.Linear(in_features=120, out_features=60),
-        #     nn.Linear(in_features=60, out_features=30),
-        #     nn.Linear(in_features=30, out_features=1)
-        # ).to(device)
+        if to_device:
+            self.model.to(self.device)
+        # self.model = ResNet1D(self.in_channels, self.base_filters, self.kernel_size,
+        #                       self.stride, self.groups, self.n_block,
+        #                       n_classes).to(self.device)
 
         self.optimizer = torch.optim.Adam(self.model.parameters(),
                                           lr=learning_rate)
-        # self.optimizer = torch.optim.SGD(self.model.parameters(),
-        #                                  lr=learning_rate)
         self.criterion = nn.MSELoss()
 
-        self.display_memory()
         self.losses = []
 
         self.validation_predictions = None
         self.validation_targets = None
 
+    def init_model(self):
+        return ResNet1D(self.in_channels, self.base_filters, self.kernel_size,
+                        self.stride, self.groups, self.n_block,
+                        self.n_classes)
+
     def train(self, dataset: PickingDataset, batch_size: int):
 
+        self.model.train()
+
         training_loader = DataLoader(dataset, batch_size=batch_size,
                                      shuffle=True)
 
         for inputs, targets in tqdm(training_loader):
             inputs = inputs.view(inputs.size()[0], -1, inputs.size()[1])
             self.iterate(inputs, targets)
             torch.cuda.empty_cache()
 
     def iterate(self, inputs, targets):
 
         self.optimizer.zero_grad()
 
         inputs = inputs.to(self.device)
         targets = targets.to(self.device)
-
         predictions = self.model(inputs)
 
         loss = self.criterion(predictions, targets.view(len(targets), -1))
         # print(loss.item())
         loss.backward()
         self.optimizer.step()
 
@@ -483,14 +610,53 @@
         inputs = inputs.view(dim1, -1, dim2).to(self.device)
         with torch.no_grad():
             outputs_tensor = self.model(inputs)
 
         outputs = [out.item() for out in outputs_tensor.cpu()]
         return outputs
 
+    def predict_trace(self, trace: Trace, pick_time: UTCDateTime, phase: str):
+        # import matplotlib.pyplot as plt
+
+        trace = trace.resample(sampling_rate=int(self.sampling_rate))
+
+        n_sample = int((pick_time - trace.stats.starttime)
+                       * trace.stats.sampling_rate)
+
+        if phase == 'P':
+            n_sample_start = int(n_sample - self.n_sample * 0.5)
+        else:
+            n_sample_start = int(n_sample - self.n_sample * 0.5)
+
+        n_sample_end = int(n_sample_start + self.n_sample)
+
+        data = trace.data[n_sample_start: n_sample_end]
+        data -= np.mean(data)
+        data /= np.max(np.abs(data))
+
+        predicted_arrival = self.predict(data)[0]
+
+        # import matplotlib.pyplot as plt
+        # plt.clf()
+        # plt.plot(data)
+        # plt.axvline(predicted_arrival)
+        # plt.show()
+        # input(predicted_arrival)
+
+        # return n_sample_start + predicted_arrival * self.n_sample
+
+        new_pick_time = trace.stats.starttime + \
+                        (n_sample_start + predicted_arrival *
+                        self.n_sample) / self.sampling_rate
+
+        return new_pick_time
+
+    def predict_stream(self, st: Stream, pick_times):
+        pass
+
     def validate(self, dataset: PickingDataset, batch_size):
         predictions = []
         training_loader = DataLoader(dataset, batch_size=batch_size,
                                      shuffle=True)
 
         losses = []
         for inputs, targets in tqdm(training_loader):
@@ -508,19 +674,62 @@
             # print(loss.cpu().item())
             losses.append(loss.cpu().item())
         return predictions, np.mean(losses), np.std(losses)
 
     def save(self, file_name):
         with(open(file_name, 'wb')) as f_out:
             pickle.dump(self, f_out)
+        # torch.save(self.model.state_dict(), file_name)
+
+    def write(self, file_name):
+        self.save(file_name)
 
     @classmethod
     def read(cls, file_name):
-        with(open(file_name, 'rb')) as f_in:
+        with open(file_name, 'rb') as f_in:
             return pickle.load(f_in)
 
+    @classmethod
+    def from_model(cls, file_name, gpu: bool = False):
+        ai_picker = cls(gpu=gpu)
+        with(open(file_name, 'rb')) as f_in:
+            picker = pickle.load(f_in)
+            ai_picker.model = picker.model
+            ai_picker.model.to(ai_picker.device)
+            ai_picker.model = ai_picker.model.double()
+            ai_picker.model = ai_picker.model.eval()
+        # picker = cls()
+        # picker.model.load_state_dict(torch.load(filename))
+        # picker.model.eval()
+        # picker.model.to(self.device)
+        #
+        # picker.in_channels = in_channels
+        # self.base_filters = base_filters
+        # self.kernel_size = kernel_size
+        # self.stride = stride
+        # self.n_classes = n_classes
+        # self.groups = groups
+        # self.n_block = n_block
+        # self.gpu = gpu
+        # self.n_sample = n_sample
+        # self.sampling_rate = sampling_rate
+
+        # if device == 'gpu':
+        #     device = torch.device("cuda:0" if
+        #                           torch.cuda.is_available() else "cpu")
+        #     if device == "cpu":
+        #         logger.warning('GPU is not available, '
+        #                        'the CPU will be used')
+        #     else:
+        #         logger.info('GPU will be used')
+        # else:
+        #     device = 'cpu'
+        #     logger.info('The CPU will be used')
+
+        return ai_picker
+
 
 def read_picker(file_name):
     return AIPicker.read(file_name)
```

### Comparing `useis-0.9.9/useis/ai/resnet1d.py` & `useis-1.0.0/useis/ai/resnet1d.py`

 * *Files 6% similar despite different names*

```diff
@@ -310,7 +310,19 @@
         if self.verbose:
             print('dense', out.shape)
         # out = self.softmax(out)
         if self.verbose:
             print('softmax', out.shape)
 
         return out
+
+    @classmethod
+    def from_resnet_1d(cls, resnet1d):
+        # in_channels: int = 1, base_filters: int = 64,
+        # kernel_size: int = 15, stride: int = 3, n_classes: int = 1,
+        # groups: int = 1, n_block: int = 16, learning_rate = 1e-3,
+        # gpu: bool = True
+        out_obj = cls(in_channels=1, base_filters=64, kernel_size=15,
+                      stride=3, n_classes=1, groups=1, n_block=16)
+        for key in resnet1d.__dict__.keys():
+            out_obj.__dict__[key] = resnet1d.__dict__[key]
+        return out_obj
```

### Comparing `useis-0.9.9/useis/ai/spectrogram.py` & `useis-1.0.0/useis/ai/spectrogram.py`

 * *Files identical despite different names*

### Comparing `useis-0.9.9/useis/core/project_manager.py` & `useis-1.0.0/useis/core/project_manager.py`

 * *Files 16% similar despite different names*

```diff
@@ -8,46 +8,24 @@
 from uquake.grid import read_grid
 from time import time
 import numpy as np
 import os
 import shutil
 from ..settings.settings import Settings
 from uquake.core.event import AttribDict
+from uquake.grid.hdf5 import H5TTable
+from .projection import Projection
+from pydantic import conlist
 
 
 def read_srces(fname):
     with open(fname, 'rb') as srces_file:
         return pickle.load(srces_file)
 
 
-# def read_inventory():
-#     if self.files.srces.exists() and use_srces:
-#         with open(self.files.srces, 'rb') as srces_file:
-#             logger.info('srces will be read from the file and not build'
-#                         'from the inventory file')
-#             self.srces = pickle.load(srces_file)
-#
-#         if self.files.inventory.exists():
-#             self.inventory = read_inventory(str(self.files.inventory))
-#
-#     elif self.files.inventory.exists():
-#         self.inventory = read_inventory(str(self.files.inventory))
-#         self.srces = Srces.from_inventory(self.inventory)
-#         logger.info('srces will be build from the inventory file. The '
-#                     'srces.pickle file will be replaced.')
-#         with open(self.files.srces, 'wb') as srces_file:
-#             pickle.dump(self.srces, srces_file)
-#
-#     elif self.files.srces.exists():
-#         logger.info('no inventory file in the project. srces file will be '
-#                     'used instead.')
-#         with open(self.files.srces, 'rb') as srces_file:
-#             self.srces = pickle.load(srces_file)
-
-
 class ProjectManager(object):
 
     inventory_file_name = 'inventory.xml'
 
     def __init__(self, base_projects_path, project_name, network_code,
                  use_srces=False, **kwargs):
         """
@@ -187,47 +165,60 @@
                       'root': base_project_path / project_name / network_code,
                       'archives': base_project_path / 'archives',
                       'inventory': root / 'inventory',
                       'config': root / 'config',
                       'velocities': root / 'velocities',
                       'times': root / 'times',
                       'hdf5_times': root / 'hdf5_times',
-                      'ai_models': root / 'ai_models'}
+                      'ai_models': root / 'ai_models',
+                      'debug': root / 'debug',
+                      'index': root / 'index',
+                      'databases' : root / 'databases'}
 
         self.paths = AttribDict(self.paths)
 
         self.files = {'inventory': self.paths.inventory / 'inventory.xml',
                       'srces': self.paths.inventory / 'srces.pickle',
                       'settings': self.paths.config / 'settings.toml',
                       'services_settings': self.paths.config /
-                                           'services_settings',
+                                           'services_settings.toml',
+                      'projection_settings': self.paths.config /
+                                             'projection_settings.toml',
                       'p_velocity': self.paths.velocities / p_vel_base_name,
                       's_velocity': self.paths.velocities / s_vel_base_name,
                       'hdf5_tt': self.paths.hdf5_times /
                                  'travel_times_tables.h5f',
                       'classification_model': self.paths.ai_models /
-                                              'classification.pickle'}
+                                              'classification.pt',
+                      'picker_model': self.paths.ai_models / 'picker.pickle'}
 
         self.files = AttribDict(self.files)
+        self.databases = AttribDict()
 
         # create the directory if it does not exist
         self.paths.root.mkdir(parents=True, exist_ok=True)
         for key in self.paths.keys():
             path = self.paths[key]
             logger.info(path)
             path.mkdir(parents=True, exist_ok=True)
 
         # SETTINGS
+        settings_path = Path(os.path.realpath(__file__)).parent.parent
 
         if not self.files.settings.is_file():
-            settings_template = Path(os.path.realpath(__file__)).parent / \
-                                    '../settings/settings_template.toml'
+            settings_template = settings_path / \
+                                    'settings/settings_template.toml'
 
             shutil.copyfile(settings_template, self.files.settings)
 
+        if not self.files.projection_settings.is_file():
+            settings_template = settings_path / \
+                                'settings/projection_settings_template.toml'
+            shutil.copyfile(settings_template, self.files.projection_settings)
+
         if not self.files.services_settings.is_file():
             settings_path = Path(os.path.realpath(__file__)).parent.parent
             settings_template = settings_path / \
                                 'settings/services_settings_template.toml'
 
             shutil.copyfile(settings_template, self.files.services_settings)
 
@@ -269,14 +260,82 @@
         self.travel_times = None
         try:
             self.travel_times = nlloc_grid.TravelTimeEnsemble.from_files(
                 self.paths.times)
         except Exception as e:
             logger.error(e)
 
+    @property
+    def htt(self):
+        return self.hdf5_tt
+
+    @property
+    def hdf5_tt(self):
+        return self.travel_times.to_hdf5(self.files.hdf5_tt)
+
+    @property
+    def projection(self):
+        offset = self.settings.projection.local.offset.to_list()
+        return Projection(global_epsg_code=
+                          self.settings.projection.GLOBAL.epsg,
+                          local_epsg_code=self.settings.projection.local.epsg,
+                          offset=offset)
+
+    def set_global_epsg_code(self, epsg_code: int):
+        self.settings.projection.GLOBAL.epsg = epsg_code
+        self.projection.write(self.files.projection_settings)
+
+    def set_local_epsg_code(self, epsg_code: int):
+        self.settings.projection.local.epsg = epsg_code
+        self.projection.write(self.files.projection_settings)
+
+    def set_projection_offset(self, offset: conlist(float, min_items=3,
+                                                    max_items=3)):
+        self.settings.projection.local.offset = offset
+        self.projection.write(self.files.projection_settings)
+
+    @property
+    def global_epsg_code(self):
+        return self.projection.global_epsg_code
+
+    @global_epsg_code.setter
+    def global_epsg_code(self, value):
+        self.projection.global_epsg_code = value
+        self.projection.write(self.files.projection_settings)
+
+    @property
+    def local_epsg_code(self):
+        return self.projection.local_epsg_code
+
+    @local_epsg_code.setter
+    def local_epsg_code(self, value):
+        self.projection.local_epsg_code = value
+        self.projection.write(self.files.projection_settings)
+
+    @property
+    def projection_offset(self):
+        return self.projection.offset
+
+    @local_epsg_code.setter
+    def local_epsg_code(self, value: conlist(float, min_items=3, max_items=3)):
+        self.projection.offset = value
+
+        self.projection.write(self.files.projection_settings)
+
+    def transform_to_global(self, easting: float = 0, northing: float = 0,
+                            z: float = 0):
+        return self.projection.transform_to_global(easting=easting,
+                                                   northing=northing,
+                                                   z=z)
+
+    def transform_to_local(self, longitude: float = 0, latitude: float = 0,
+                           z: float = 0):
+        return self.projection.transform_to_local(longitude=longitude,
+                                                  latitude=latitude)
+
     @staticmethod
     def exists(project_path, project_name, network_code):
         project_path = Path(project_path) / project_name / network_code
         return project_path.exists()
 
     def init_travel_time_grids(self, multi_threaded=True):
         """
@@ -306,33 +365,19 @@
         seed_labels = self.srces.labels
 
         tt = self.velocities.to_time(seeds, seed_labels,
                                      multi_threaded=multi_threaded)
 
         self.travel_times = tt
 
-        # if self.has_p_velocity():
-        #     tt_gs_p = self.p_velocity.to_time(seeds, seed_labels,
-        #                                       multi_threaded=multi_threaded)
-        #     self.travel_times = tt_gs_p
-        # if self.has_s_velocity():
-        #     tt_gs_s = self.s_velocity.to_time(seeds, seed_labels,
-        #                                       multi_threaded=multi_threaded)
-        #     self.travel_times = tt_gs_s
-        #
-        # if self.p_velocity and self.s_velocity:
-        #     self.travel_times = tt_gs_p + tt_gs_s
-
-        # cleaning the directory before writing the new files
-
         for fle in self.paths.times.glob('*time*'):
             fle.unlink(missing_ok=True)
 
         self.travel_times.write(self.paths.times)
-        # self.travel_times.write_hdf5(self.paths. / 'test.hf5')
+        self.travel_times.write_hdf5(self.files.hdf5_tt)
         t1 = time()
         logger.info(f'done initializing the travel time grids in '
                     f'{t1 - t0:0.2f} seconds')
 
     def add_inventory(self, inventory, create_srces_file: bool = True,
                       initialize_travel_time: bool = True):
         """
@@ -344,14 +389,15 @@
         :param initialize_travel_time: if True the travel time grids are
         initialized (default: True)
         :return:
         """
 
         inventory.write(str(self.files.inventory))
         self.srces = Srces.from_inventory(inventory)
+        self.inventory = inventory
         if create_srces_file:
             with open(self.files.srces, 'wb') as srces_file:
                 pickle.dump(self.srces, srces_file)
 
         if initialize_travel_time:
             self.init_travel_time_grids()
         else:
@@ -360,15 +406,15 @@
                            'be out of sync. To initialize the travel time '
                            'grids make sure initialize_travel_time is set to '
                            'True')
 
     def add_inventory_from_file(self, inventory_file: str, format='StationXML',
                                 create_srces_file: bool = True,
                                 initialize_travel_time: bool = True,
-                                xy_from_lat_lon: bool = True,
+                                xy_from_lat_lon: bool = False,
                                 input_projection=4326,
                                 output_projection=None):
         """
         adding a inventory object to the project from a file
         :param inventory_file: station xml inventory object
         :type inventory_file: uquake.core.inventory.Inventory
         :param format: file format for the inventory file
@@ -380,18 +426,23 @@
         cartesian coordinates
         :param input_projection: input projection (default=4326 for typical
         latitude and longitude)
         :param output_projection: output projection (default None)
         :return:
         """
 
-        inventory = read_inventory(inventory_file, format=format,
-                                   xy_from_lat_lon=xy_from_lat_lon,
-                                   input_projection=input_projection,
-                                   output_projection=output_projection)
+        if output_projection is not None:
+            inventory = read_inventory(inventory_file, format=format,
+                                       xy_from_lat_lon=xy_from_lat_lon,
+                                       input_projection=input_projection,
+                                       output_projection=output_projection)
+        else:
+            inventory = read_inventory(inventory_file, format=format,
+                                       xy_from_lat_lon=xy_from_lat_lon,
+                                       input_projection=input_projection)
 
         self.add_inventory(inventory, create_srces_file=create_srces_file,
                            initialize_travel_time=initialize_travel_time)
 
     def add_srces(self, srces, force=False, initialize_travel_time: bool=True,
                   multi_threaded: bool=True):
         """
@@ -581,8 +632,18 @@
         return False
 
     def has_inventory(self):
         if self.inventory or self.srces:
             return True
         return False
 
+    def clean_stream(self, stream):
+        if 'black_list'.upper() in self.settings.keys():
+            for sensor in self.settings.black_list:
+                station = sensor.split('.')[0]
+                location = sensor.split('.')[1]
+                for tr in stream.select(station=station, location=location):
+                    stream.remove(tr)
+
+        return stream
+
```

### Comparing `useis-0.9.9/useis/processors/nlloc.py` & `useis-1.0.0/useis/processors/nlloc.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,27 +1,144 @@
+import openpyxl.styles.stylesheet
+import uquake.core.inventory
+from uquake.core.inventory import Inventory
+
 from ..core.project_manager import *
 from uquake.nlloc.nlloc import *
-from uquake.core.event import (Catalog, Event, CreationInfo, Origin, Arrival)
+from uquake.core.event import (Catalog, Event, CreationInfo, Origin, Arrival,
+                               Pick, WaveformStreamID)
 from uquake.core import UTCDateTime
+from uquake.core.stream import Stream
 import numpy as np
 import sys
 import toml
 # from pydantic import BaseModel
 # from ..services import models
 # from typing import Optional, List
+import matplotlib.pyplot as plt
+
+
+def locate_hodogram(st: Stream, event: Event, inventory: Inventory,
+                    window_length: float = 20e-3, linearity_threshold=0.7):
+    """
+    measure the incidence angle from hodogram
+    :param st: a stream object containing the waveforms
+    :type st: uquake.core.stream.Stream
+    :param picks: a list of picks associated the the waveforms
+    :type picks: list of uquake.core.event.Picks
+    :param inventory: inventory file
+    :type inventory: uquake.core.inventory.Inventory
+    :param window_length: lenght of the window within which the hodogram is
+    measured
+    :return:
+    """
+
+    # Rotate the stream in "E", "N", "Z" if that is not yet the case
+    st_zne = st.copy().rotate('->ZNE', inventory=inventory)
+    st_zne = st_zne.filter('highpass', freq=10)
+
+    # for each pick measure the incidence angle using the hodogram
+    if event.preferred_origin() is not None:
+        origin = event.preferred_origin()
+    else:
+        origin = event.origins[-1]
+
+    azimuths = []
+    plunges = []
+    linearities = []
+    phases = []
+    scatters = event.preferred_origin().scatter
+    dot_prod = np.zeros(len(scatters))
+    for arrival in origin.arrivals:
+        pick = arrival.pick
+        network = pick.waveform_id.network_code
+        station = pick.waveform_id.station_code
+        location = pick.waveform_id.location_code
+
+        start_time = pick.time
+        end_time = pick.time + window_length
+
+        st_tmp = st_zne.copy().select(network=network, station=station,
+                                      location=location).trim(
+            starttime=start_time, endtime=end_time)
+
+        wave_mat = []
+        for component in ['E', 'N', 'Z']:
+            tr = st_tmp.select(component=component)[0]
+            wave_mat.append(tr.data)
+
+        wave_mat = np.array(wave_mat)
+        # plt.figure(2)
+        # plt.close('all')
+        # plt.clf()
+        # plt.plot(wave_mat[1, :] / np.max(wave_mat[1, :]),
+        #          wave_mat[0, :] / np.max(wave_mat[0, :]), 'k')
+
+        cov_mat = np.cov(np.array(wave_mat))
+
+        e = None
+
+        eig_vals, eig_vects = np.linalg.eig(cov_mat)
+        i_ = np.argsort(eig_vals)
+
+        if arrival.phase == 'P':
+            eig_vect = eig_vects[i_[-1]]
+            linearity =  (1 - np.linalg.norm(eig_vals[i_[:2]]) /
+                          eig_vals[i_[2]])
+            # input(f'grossomodo P {linearity}')
+            color = 'b'
+        elif arrival.phase == 'S':
+            eig_vect = eig_vects[i_[0]]
+            linearity = (1 - eig_vals[i_[0]] /
+                        np.linalg.norm(eig_vals[i_[1:]]))
+            color = 'r'
+
+        # if linearity < linearity_threshold:
+        #     continue
+
+        sta = inventory.select(network=network,
+                               station=station,
+                               location=location)[0][0]
+
+        eig_vect /= np.linalg.norm(eig_vect)
+
+        for i, scat in enumerate(scatters):
+            vect = sta.loc - scat[0:3]
+            vect /= np.linalg.norm(vect)
+            dot_prod[i] += np.abs(np.dot(vect, eig_vect)) * scat[-1] * \
+                           linearity
+
+    return scatters[np.argmax(dot_prod), :-1]
 
 
 def calculate_uncertainty(point_cloud):
     """
     :param point_cloud: location point cloud
     :type point_cloud: numpy 2d array
     :return: uncertainty
     :rtype: uquake.core.event.OriginUncertainty
     """
 
+    # horizontal uncertainty
+    if len(point_cloud) == 0:
+        ce = ConfidenceEllipsoid(semi_major_axis_length=0,
+                                 semi_intermediate_axis_length=0,
+                                 semi_minor_axis_length=0,
+                                 major_axis_plunge=0,
+                                 major_axis_azimuth=0,
+                                 major_axis_rotation=0)
+
+        return OriginUncertainty(horizontal_uncertainty=0,
+                                 confidence_ellipsoid=0,
+                                 preferred_description='confidence ellipsoid',
+                                 confidence_level=68)
+
+    v, u = np.linalg.eig(np.cov(point_cloud[:, 0:2].T))
+    horizontal_uncertainty = np.sqrt(np.max(v))
+
     v, u = np.linalg.eig(np.cov(point_cloud.T))
 
     major_axis_index = np.argmax(v)
 
     uncertainty = np.sort(np.sqrt(v))[-1::-1]
 
     h = np.linalg.norm(u[major_axis_index, :-1])
@@ -36,47 +153,48 @@
     ce = ConfidenceEllipsoid(semi_major_axis_length=uncertainty[0],
                              semi_intermediate_axis_length=uncertainty[1],
                              semi_minor_axis_length=uncertainty[2],
                              major_axis_plunge=major_axis_plunge,
                              major_axis_azimuth=major_axis_azimuth,
                              major_axis_rotation=major_axis_rotation)
 
-    return OriginUncertainty(confidence_ellipsoid=ce,
+    return OriginUncertainty(horizontal_uncertainty=horizontal_uncertainty,
+                             confidence_ellipsoid=ce,
                              preferred_description='confidence ellipsoid',
                              confidence_level=68)
 
 
-class NLLOCResult:
-
-    # hypocenter: List[float]
-    # event_time: datetime
-    # scatter_cloud: List[float]
-    # rays: List[Rays]
-    # observations: models.nlloc.Observations
-    # evaluation_mode: models.event.evaluation_mode
-    # evaluation_status: models.event.evaluation_status
+class NLLOCResult(object):
 
-    def __init__(self, hypocenter: np.array, event_time: UTCDateTime,
-                 scatter_cloud: np.ndarray, rays: list,
-                 observations: Observations, evaluation_mode: str,
-                 evaluation_status: str, hypocenter_file: str):
+    def __init__(self, nll_object, hypocenter: np.array,
+                 event_time: UTCDateTime, scatter_cloud: np.ndarray,
+                 rays: list, observations: Observations,
+                 evaluation_mode: str, evaluation_status: str,
+                 hypocenter_file: str):
+        self.nll_object = nll_object
         self.hypocenter = hypocenter
+        self.hypocenter_global = (self.nll_object.projection.
+                                  transform_to_global(hypocenter[0],
+                                                      hypocenter[1],
+                                                      hypocenter[2]))
         self.event_time = event_time
         self.scatter_cloud = scatter_cloud
         self.rays = rays
         self.observations = observations
         self.evaluation_mode = evaluation_mode
         self.evaluation_status = evaluation_status
 
-        self.uncertainty_ellipsoid = calculate_uncertainty(
+        self.origin_uncertainty = calculate_uncertainty(
             self.scatter_cloud[:, :-1])
 
         self.creation_info = CreationInfo(author='uQuake-nlloc',
                                           creation_time=UTCDateTime.now())
         self.hypocenter_file = hypocenter_file
+        self.unc = self.origin_uncertainty.confidence_ellipsoid.\
+            semi_major_axis_length
 
     def __repr__(self):
         out_str = f"""
         time (UTC)  : {self.t}
         location    : x- {self.x:>10.1f} (m)
                       y- {self.y:>10.1f} (m)
                       z- {self.z:>10.1f} (m)
@@ -92,14 +210,26 @@
         return self.append_to_event(other)
 
     @property
     def loc(self):
         return self.hypocenter
 
     @property
+    def latitude(self):
+        return self.hypocenter_global[1]
+
+    @property
+    def longitude(self):
+        return self.hypocenter_global[0]
+
+    @property
+    def depth(self):
+        return self.hypocenter_global[2]
+
+    @property
     def x(self):
         return self.loc[0]
 
     @property
     def y(self):
         return self.loc[1]
 
@@ -108,80 +238,295 @@
         return self.loc[2]
 
     @property
     def t(self):
         return self.event_time
 
     @property
+    def time(self):
+        return self.event_time
+
+    @property
     def arrivals(self) -> list:
         arrivals = []
+        predicted_times = self.nll_object.travel_times.travel_time(
+            self.hypocenter)
+        angles = self.nll_object.travel_times.angles(self.hypocenter)
         for pick in self.observations.picks:
             travel_time = pick.time - self.t
             phase = pick.phase_hint
             site_code = pick.site
-            for ray in self.rays:
-                if (ray.site_code == site_code) & (ray.phase == phase):
-                    break
-            distance = ray.length
 
-            time_residual = Arrival.calculate_time_residual(ray.travel_time,
-                                                            travel_time)
+            network = pick.waveform_id.network_code
+            station = pick.waveform_id.station_code
+            location = pick.waveform_id.location_code
+
+            if self.rays is not None:
+                for ray in self.rays:
+                    if (ray.site_code == site_code) & (ray.phase == phase):
+                        break
+                distance = ray.length
+
+                time_residual = Arrival.calculate_time_residual(
+                    ray.travel_time,
+                    travel_time)
+
+                azimuth = ray.azimuth
+                takeoff_angle = ray.takeoff_angle
+
+            else:
+                inv = self.nll_object.inventory.select(network=network,
+                                                       station=station,
+                                                       location=location)
+
+                distance = np.linalg.norm(self.hypocenter - inv[0][0][0].loc)
+
+                predicted_time = predicted_times[phase][site_code]
+
+                time_residual = Arrival.calculate_time_residual(predicted_time,
+                                                                travel_time)
+
+                azimuth = angles['azimuth'][phase][site_code]
+                takeoff_angle = angles['takeoff'][phase][site_code]
 
             time_weight = 1
-            azimuth = ray.azimuth
-            takeoff_angle = ray.takeoff_angle
 
             arrival = Arrival(phase=phase, distance=distance,
                               time_residual=time_residual,
                               time_weight=time_weight, azimuth=azimuth,
                               takeoff_angle=takeoff_angle,
                               pick_id=pick.resource_id)
 
             arrivals.append(arrival)
 
         return arrivals
 
     @property
     def origin(self):
         origin = Origin(x=self.x, y=self.y, z=self.z, time=self.t,
+                        latitude=self.latitude,
+                        longitude=self.longitude,
+                        depth=self.depth,
                         evaluation_mode=self.evaluation_mode,
                         evaluation_status=self.evaluation_status,
                         epicenter_fixed=False, method_id='uQuake-NLLOC',
                         creation_info=self.creation_info,
                         arrivals=self.arrivals,
-                        origin_uncertainty=self.uncertainty_ellipsoid,
+                        origin_uncertainty=self.origin_uncertainty,
+                        uncertainty=self.unc,
                         rays=self.rays,
                         scatter=self.scatter_cloud)
         origin.scatter = self.scatter_cloud
         origin.rays = self.rays
         return origin
 
     @property
     def event(self):
         return self.export_as_event()
 
     @property
     def uncertainty(self):
-        ce = self.uncertainty_ellipsoid.confidence_ellipsoid
+        ce = self.origin_uncertainty.confidence_ellipsoid
         return ce.semi_major_axis_length
 
+    @property
+    def predicted_picks(self):
+        if not self.rays:
+            return
+
+        predicted_picks = []
+        for ray in self.rays:
+            predicted_picks.append(ray.to_pick(self.time))
+
+        return predicted_picks
+
     def append_to_event(self, event: Event) -> Event:
         o = self.origin
         if isinstance(event, Catalog):
             event[0].append_origin_as_preferred_origin(o)
         elif isinstance(event, Event):
             event.append_origin_as_preferred_origin(o)
         return event
 
     def export_as_event(self):
         o = self.origin
         e = Event(origins=[o], picks=self.observations.picks)
         e.preferred_origin_id = o.resource_id
         return e
 
+    def to_2d(self, station):
+        return NLLOCResult2DCylindrical.from_nlloc_result(self, station)
+
+    def relocate(self, residual_threshold=10e-3):
+        event = self.event
+        picks = []
+        for arrival in event.preferred_origin().arrivals:
+            if arrival.time_residual < residual_threshold:
+                picks.append(arrival.pick)
+
+        observations = Observations(picks=picks)
+        return self.nll_object.run_location(observations)
+
+    def relocate_hodogram(self, stream: Stream, window_length: float = 20e-3):
+        loc = locate_hodogram(stream, self.event, self.nll_object.inventory,
+                               window_length=window_length)
+
+        self.hypocenter = np.array(loc)
+
+        return loc
+
+
+class NLLOCResult2DCylindrical(NLLOCResult):
+    """
+    Transform a NLLOCResult object into 2D Cylindrical solution with more
+    appropriate measurement of the uncertainty.
+    This object is used mainly in the case of a single borehole array.
+    It is assumed that the borehole is nearly vertical and that the deviation
+    can be neglected
+    """
+
+    def __init__(self, nlloc_object, hypocenter: np.array,
+                 event_time: UTCDateTime,
+                 scatter_cloud: np.ndarray, rays: list,
+                 observations: Observations, evaluation_mode: str,
+                 evaluation_status: str, hypocenter_file: str,
+                 inventory: uquake.core.inventory.Inventory, station: str):
+
+        """
+        :param nlloc_object:
+        :param hypocenter: event hypocenter location
+        :param event_time: event time
+        :param scatter_cloud: cloud of probable location
+        :param rays: a list of ray
+        :param observations: travel time observations used to calculate the
+        location
+        :param evaluation_mode: evaluation mode as defined by the QuakeML
+        standard
+        :param evaluation_status: evaluation status as defined by the QuakeML
+        standard
+        :param hypocenter_file: The hypocenter files output by NLLoc
+        :param inventory: an inventory file
+        :param station: station name
+        """
+
+        inv = inventory.select(station=station)
+        xs = []
+        ys = []
+        for site in inv.sites:
+            xs.append(site.x)
+            ys.append(site.y)
+
+        self.reference_x = np.mean(xs)
+        self.reference_y = np.mean(ys)
+
+        super().__init__(nlloc_object, hypocenter, event_time, scatter_cloud,
+                        rays, observations, evaluation_mode, evaluation_status,
+                         hypocenter_file)
+
+    @classmethod
+    def from_nlloc_result(cls, nlloc_result: NLLOCResult, station: str):
+        return cls(nlloc_result.nll_object,nlloc_result.hypocenter,
+                   nlloc_result.event_time,
+                   nlloc_result.scatter_cloud, nlloc_result.rays,
+                   nlloc_result.observations, nlloc_result.evaluation_mode,
+                   nlloc_result.evaluation_status,
+                   nlloc_result.hypocenter_file,
+                   nlloc_result.nll_object.inventory, station)
+
+    @property
+    def uncertainty_h(self):
+        xs = self.scatter_cloud[:, 0] - self.reference_x
+        ys = self.scatter_cloud[:, 1] - self.reference_y
+        return np.std(np.sqrt(xs ** 2 + ys ** 2))
+
+    @property
+    def uncertainty_z(self):
+        return np.std(self.scatter_cloud[:, -2])
+
+    @property
+    def uncertainty(self):
+        return np.sqrt(self.uncertainty_h ** 2 + self.uncertainty_z ** 2)
+
+    @property
+    def r(self):
+        return np.linalg.norm([self.x - self.reference_x,
+                               self.y - self.reference_y])
+
+    @property
+    def origin(self):
+
+        self.origin_uncertainty.horizontal_uncertainty = self.uncertainty_h
+
+        origin = Origin(x=self.r, y=0, z=self.z, time=self.t,
+                        evaluation_mode=self.evaluation_mode,
+                        evaluation_status=self.evaluation_status,
+                        epicenter_fixed=False, method_id='uQuake-NLLOC',
+                        creation_info=self.creation_info,
+                        arrivals=self.arrivals,
+                        origin_uncertainty=self.origin_uncertainty,
+                        uncertainty=self.uncertainty_h,
+                        rays=self.rays,
+                        scatter=self.scatter_cloud)
+        origin.scatter = self.scatter_cloud
+        origin.rays = self.rays
+        return origin
+
+    def __repr__(self):
+        out_str = f"""
+        time (UTC)             : {self.t}
+        location               : r- {self.r:>10.1f} (m)
+                                 z- {self.z:>10.1f} (m)
+        uncertainty Horizontal : {self.uncertainty_h:0.1f} (1 std - m)
+        uncertainty Vertical   : {self.uncertainty_z:0.1f} (1 std - m)
+        uncertainty            : {self.uncertainty:0.1f} (1 std - m)
+        """
+        return out_str
+
+    def to_3d(self, azimuth: float, std_azimuth: float) -> NLLOCResult:
+        """
+        :centroi
+        :param azimuth: azimuth in degrees
+        :param std_azimuth: standard deviation of the Azimuth in degrees
+        :return:
+        """
+
+        # converting degrees to radians
+
+        azimuth = (azimuth * np.pi / 180) % (2 * np.pi)
+
+        x = np.sin(azimuth) * self.r + self.reference_x  # Northing
+        y = np.cos(azimuth) * self.r + self.reference_y  # Easting
+
+        hypocenter = np.array([x, y, self.z])
+
+        d_s_x = self.scatter_cloud[:, 0] - self.reference_x
+        d_s_y = self.scatter_cloud[:, 1] - self.reference_y
+
+        scatter_azimuths = (np.arctan2(d_s_x, d_s_y)) % (2 * np.pi)
+
+        min_azimuth = (azimuth - std_azimuth) % (2 * np.pi)
+        max_azimuth = (azimuth + std_azimuth) % (2 * np.pi)
+
+        scatter_cloud = self.scatter_cloud[
+            (scatter_azimuths >= min_azimuth) &
+            (scatter_azimuths <= max_azimuth), :]
+
+        if len(scatter_cloud) == 0:
+            min_azimuth = (azimuth - 10 / 180 * np.pi) % (2 * np.pi)
+            max_azimuth = (azimuth + 10 / 180 * np.pi) % (2 * np.pi)
+
+            scatter_cloud = self.scatter_cloud[
+                            (scatter_azimuths >= min_azimuth) &
+                            (scatter_azimuths <= max_azimuth), :]
+
+        return NLLOCResult(self.nll_object, hypocenter, self.time,
+                           scatter_cloud, self.rays, self.observations,
+                           self.evaluation_mode, self.evaluation_status,
+                           self.hypocenter_file)
+
 
 class NLLOC(ProjectManager):
     def __init__(self, base_projects_path: Path, project_name: str,
                  network_code: str, use_srces: bool=False):
 
         """
         Object to control NLLoc execution and manage the required grids, inputs
@@ -207,39 +552,24 @@
         self.paths.observations.mkdir(parents=True, exist_ok=True)
         self.files.observations = self.paths.observations / 'picks.obs'
         self.observations = None
 
         self.paths.templates = self.paths.root / 'templates'
         self.paths.templates.mkdir(parents=True, exist_ok=True)
 
-        # self.files.template_ctrl = self.paths.templates / \
-        #                            'ctrl_template.pickle'
-
-        # if self.files.template_ctrl.exists():
-        #     with open(self.files.template_ctrl, 'rb') as template_ctrl:
-        #         self.control_template = pickle.load(template_ctrl)
-        # else:
-        #     self.control_template = None
-        #     self.add_template_control()
-
         self.files.control = self.paths.current_run / 'run.nll'
 
         self.last_event_hypocenter = None
         self.last_event_time = None
 
         self.files.nlloc_settings = self.paths.config / 'nlloc_settings.py'
 
         sys.path.append(str(self.paths.config))
 
-        # if not (self.paths.config / '__init__.py').is_file():
-        #     with open(self.paths.config / '__init__.py', 'w') as fp:
-        #         pass
-
         if not self.files.nlloc_settings.is_file():
-            # self.add_template_control()
             settings_template = Path(os.path.realpath(__file__)).parent / \
                                     '../settings/nlloc_settings_template.py'
 
             shutil.copyfile(settings_template, self.files.nlloc_settings)
 
         self.nlloc_settings = __import__('nlloc_settings')
         self.control_template = self.nlloc_settings.nlloc_control
@@ -249,85 +579,33 @@
     def __del__(self):
         self.remove_run_directory()
 
     def remove_run_directory(self):
         for fle in self.paths.observations.glob('*'):
             fle.unlink()
 
-        self.paths.observations.rmdir()
+        if self.paths.observations.exists():
+            self.paths.observations.rmdir()
 
         output_dir = self.paths.outputs
 
         for fle in output_dir.glob('*'):
             fle.unlink()
-        output_dir.rmdir()
+
+        if output_dir.exists():
+            output_dir.rmdir()
 
         for fle in self.paths.outputs.parent.glob('*'):
             fle.unlink()
 
-        self.paths.outputs.parent.rmdir()
-
-    # def add_template_control(self, control=Control(message_flag=1),
-    #                          transformation=GeographicTransformation(),
-    #                          locsig=None, loccom=None,
-    #                          locsearch=LocSearchOctTree.init_default(),
-    #                          locmeth=LocationMethod.init_default(),
-    #                          locgau=GaussianModelErrors.init_default(),
-    #                          locqual2err=LocQual2Err(0.0001, 0.0001, 0.0001,
-    #                                                  0.0001, 0.0001),
-    #                          **kwargs):
-    #
-    #     settings_template = Path(os.path.realpath(__file__)).parent / \
-    #         #                         '../settings/nlloc_settings_template.toml'
-    #     #
-    #     # shutil.copyfile(settings_template, self.files.nlloc_settings)
-    #
-    #
-    #
-    #     if not isinstance(control, Control):
-    #         raise TypeError(f'control is type {type(control)}. '
-    #                         f'control must be type {Control}.')
-    #
-    #     if not issubclass(type(transformation), GeographicTransformation):
-    #         raise TypeError(f'transformation is type {type(transformation)}. '
-    #                         f'expecting type'
-    #                         f'{GeographicTransformation}.')
-    #
-    #     if not locsearch.type == 'LOCSEARCH':
-    #         raise TypeError(f'locsearch is type {type(locsearch)}'
-    #                         f'expecting type '
-    #                         f'{LocSearchGrid} '
-    #                         f'{LocSearchMetropolis}, or '
-    #                         f'{LocSearchOctTree}.')
-    #
-    #     if not isinstance(locmeth, LocationMethod):
-    #         raise TypeError(f'locmeth is type {type(locmeth)}, '
-    #                         f'expecting type {LocationMethod}')
-    #
-    #     if not isinstance(locgau, GaussianModelErrors):
-    #         raise TypeError(f'locgau is type {type(locgau)}, '
-    #                         f'expecting type {GaussianModelErrors}')
-    #
-    #     if not isinstance(locqual2err, LocQual2Err):
-    #         raise TypeError(f'locqual2err is type {type(locqual2err)}, '
-    #                         f'expecting type {LocQual2Err}')
-    #
-    #     dict_out = {'control': control,
-    #                 'transformation': transformation,
-    #                 'locsig': locsig,
-    #                 'loccom': loccom,
-    #                 'locsearch': locsearch,
-    #                 'locmeth': locmeth,
-    #                 'locgau': locgau,
-    #                 'locqual2err': locqual2err}
-    #
-    #     # with open(self.files.nlloc_settings, 'w') as nlloc_settings:
-    #     #     toml.dump(dict_out, nlloc_settings)
-    #
-    #     self.control_template = dict_out
+        if self.paths.outputs.parent.exists():
+            self.paths.outputs.parent.rmdir()
+        else:
+            logger.info(f'{self.paths.outputs.parent} was already deleted...'
+                        f'nothing to do')
 
     def write_control_file(self):
         with open(self.files.control, 'w') as control_file:
             control_file.write(self.control)
 
     def __add_observations__(self, observations):
         """
@@ -384,41 +662,49 @@
                 event_time = event.preferred_origin().time
             else:
                 event_time = event.origins[-1].time
         else:
             p_times = []
             for pick in observations.picks:
                 p_times.append(pick.time)
+            if not p_times:
+                logger.error('empty results')
+                return
             event_time = np.min(p_times)
 
         if not (self.paths.outputs / 'last.hyp').exists():
             logger.error(f'event location failed for event {event_time}!')
+            return
 
         with open(self.paths.outputs / 'last.hyp') as hyp_file:
             hypocenter_file = hyp_file.readlines()
 
         t, x, y, z = read_hypocenter_file(self.paths.outputs / 'last.hyp')
 
+        eloc = np.array([x, y, z])
+
         scatters = read_scatter_file(self.paths.outputs / 'last.scat')
 
         rays = None
         if calculate_rays:
             logger.info('calculating rays')
             t0_ray = time()
             rays = self.travel_times.ray_tracer(np.array([x, y, z]),
                                                 multithreading=multithreading)
             t1_ray = time()
             logger.info(f'done calculating rays in {t1_ray - t0_ray:0.2f} '
                         f'seconds')
 
+        # for travel_time in self.travel_times.travel_time(eloc, )
+
         if delete_output_files:
             self.remove_run_directory()
 
-        result = NLLOCResult(np.array([x, y, z]), t, scatters, rays,
-                             observations, evaluation_mode, evaluation_status,
+        result = NLLOCResult(self, eloc, t, scatters, rays, observations,
+                             evaluation_mode, evaluation_status,
                              hypocenter_file)
 
         return result
 
     def rays(self, hypocenter_location):
         return self.travel_times.ray_tracer(hypocenter_location)
 
@@ -435,15 +721,15 @@
         if self.srces is None:
             raise ValueError('The project does not contain sites or '
                              'inventory. sites (srces) or inventory '
                              'information can be added using the add_srces or'
                              'add_inventory methods.')
 
         if self.observations is None:
-            raise ValueError('The current run does not contain travel time'
+            raise ValueError('The current run does not contain travel time '
                              'observations. Observations should be added to '
                              'the current run using the add_observations '
                              'method.')
 
         observations = str(self.observations)
 
         ctrl = ''
```

### Comparing `useis-0.9.9/useis/processors/simple_magnitude.py` & `useis-1.0.0/useis/processors/simple_magnitude.py`

 * *Files identical despite different names*

### Comparing `useis-0.9.9/useis/sandbox/demo_kafka/Dockerfile` & `useis-1.0.0/useis/sandbox/demo_kafka/Dockerfile`

 * *Files identical despite different names*

### Comparing `useis-0.9.9/useis/sandbox/demo_kafka/consumer.py` & `useis-1.0.0/useis/sandbox/demo_kafka/consumer.py`

 * *Files identical despite different names*

### Comparing `useis-0.9.9/useis/sandbox/demo_kafka/docker-compose.yml` & `useis-1.0.0/useis/sandbox/demo_kafka/docker-compose.yml`

 * *Files identical despite different names*

### Comparing `useis-0.9.9/useis/sandbox/demo_useis/test/test/TN/config/settings.toml` & `useis-1.0.0/useis/settings/settings_template.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,275 +1,285 @@
-[default]
-dynaconf_include = ["*.toml"]
-project.name = 'test'
-project.network = 'OT'
-project.base_directory = ''
-api_base_url = 'https://api.microquake.org/api/v1/'
-ims_base_url = 'http://10.95.74.35:8002/ims-database-server/databases/mgl'
-project_code = 'OT'
-site = 'Oyu Tolgoi'
-site_code = 'OT'
-network = 'Hugo North Ungerground Network'
-network_code = 'OT'
-redis_rq_url = ''
-logging_level = 0
-DEBUG_LEVEL = 0
-DEBUG_FILE_DIR = '.'
+dynaconf_include = ['*.toml']
 
-time_zone.type = 'UTC_offset'                # either 'UTC_offset or 'time_zone'
-time_zone.time_zone_code = 'ULN'             # time zone code. If type=time_zone, time_zone_code must be a valid pytz timezone
-time_zone.offset = 8                         # time offset in hours, ignored if type=time_zone
-
-pre_processing_message_queue = 'event_connector.pre_processing'
-automatic_pipeline_message_queue = 'workflow.automatic'
-api_message_queue = 'api'
-
-grids.units = 'meter'
-grids.method = 'ODS'
-grids.origin = [650200, 4766170, -500]
-grids.dimensions = [100, 101, 68]
-grids.spacing = [25, 25, 25]
-grids.velocities.source = 'local'
-grids.velocities.homogeneous = false
-grids.velocities.vp = 'velocities/vp'
-grids.velocities.vs = 'velocities/vs'
-grids.velocities.format = 'NLLOC'
-
-grids.travel_time_h5.fname = 'travel_time_tables.h5f'
-
-sites.source     = 'local'
-sites.units      = 'meter'
-sites.format     = 'csv'
-sites.path       = 'sites.csv'
-sites.stationXML = 'OT.xml'
-sites.black_list = ['7', '9', '10', '23', '25', '31', '32', '54', '91', '96', '99', '100', '102', '107', '88', '90', '77']
-
-ug_blast_windows_local_time = [7, 19]
-ug_blast_windows_tolerance_minutes = 30
-quakeml_ug_blast_type = 'explosion'
-
-data_connector.minimum_recovery_fraction = 0.85
-data_connector.maximum_attempts = 10 # maximum number of attempts at retrieving the data
-data_connector.minimum_delay_minutes = 0.5
-data_connector.context_trace.filter.freqmin = 60
-data_connector.context_trace.filter.freqmax = 500
-data_connector.likelihood_threshold = 0.50
-data_connector.reconciliation_delay_minutes = 60
-data_connector.reconciliation_interval_hours = 72
-data_connector.maximum_event_elevation = 900
-data_connector.request_range_hours = 72
-data_connector.closing_window_time_seconds = 60 # time after which we
-# consider the continuous data window closed after the event occurred
-data_connector.context_trace_forbiden_site = ['7', '9']  # Accelerometers
-
-event_detection.sta_lta_on_value = 3.0
-event_detection.sta_lta_off_value = 1.5
-event_detection.sta_length_second = 10e-3
-event_detection.lta_length_second = 100e-3
-event_detection.onset_threshold = 3
-event_detection.max_trigger_length_second = 0.2
-event_detection.association_time_window_length_second = 1
-event_detection.association_hold_off_time_second = 1.2 # from the start of the sequence
-#event_detection.seismogram_resulting_length_second = 2
-
-#<STALTA_on value="3.0"/>
-#        <STALTA_off value="1.25"/>
-#        <STA value="10e-3"/>
-#		<LTA value="100e-3"/>
-#        <onset_threshold value="3"/> <!-- STALTA function threshold to declare a trigger -->
-#        <max_trigger_length value="0.05"/> <!-- maximum trigger length to declare a trigger valid -->
-#        <association_time value="0.1"/> <!-- length of time window within which trigger are associated -->
-#        <hold_off_time value="0.1"/> <!-- hold off time after an event has been detected to trigger another event -->
-#        <min_number_trigger value="5"/>  <!-- minimum number of trigger required to declare an event -->
-#        <seismogram_length value="300"/>
-
-event_classifier.likelihood_threshold = 0.5
-event_classifier.blast_window_starts = [6, 18]
-event_classifier.blast_window_ends = [8, 20]
-event_classifier.valid_event_types = ['seismic event']
-event_classifier.blast_event_types = ['underground blast']
-event_classifier.uploaded_event_types = ['crusher noise', 'ore pass noise', 'test pulse', 'other blast', 'open pit blast']
-event_classifier.ignore_type_large_event = ['underground blast', 'test pulse', 'open pit blast']
-event_classifier.large_event_processing_threshold = 0.5
-
-interloc.nthreads = 4
-interloc.samplerate_decimated = 3000.0
-interloc.fixed_wlen_sec = 2.0
-interloc.whiten_corner_freqs = [40.0, 50.0, 350.0, 360.0]
-interloc.pair_dist_min = 0.0
-interloc.pair_dist_max = 2000.0
-interloc.cc_smooth_length_sec = 0.005
-interloc.detection_threshold = 0.2
-
-compute_xcorrs.rolling_database_keep_hours = 80
-compute_xcorrs.samplerate_decimated = 2000.0
-compute_xcorrs.onebit_normalization = true
-compute_xcorrs.whiten_corner_freqs = [40.0, 50.0, 390.0, 400.0]
-compute_xcorrs.request_continuous_length_sec = 600
-compute_xcorrs.request_continuous_lag_sec = 1800
-compute_xcorrs.wlen_sec = 10
-compute_xcorrs.stepsize_sec = 10
-compute_xcorrs.keeplag_sec = 1.0
-compute_xcorrs.stack_length_hours = 24.0
-compute_xcorrs.pair_dist_min = 50.0
-compute_xcorrs.pair_dist_max = 500.0
-compute_xcorrs.channel_blacklist = ['.131.X', '.131.Y', '.131.Z', '.56.Y', '.67.Y', '.83.X', '.86.X', '.86.Y', '.86.Z', '.88.X', '.88.Y', '.88.Z', '.90.X', '.90.Z']
-
-
-compute_velchange.coda_start_velocity = 3000.0
-compute_velchange.coda_end_sec = 0.8
-compute_velchange.freq_band_measure = [70.0, 240.0]
-compute_velchange.wlen_sec = 0.02
-compute_velchange.step_factor = 10
-compute_velchange.coherence_welch_nwin = 10
-
-# parameter of the PPV vs Magnitude relationship
-quick_magnitude.a = 1.2
-quick_magnitude.c = 1.1
-
-picker.snr_threshold = 8
-picker.min_num_picks = 20
-picker.residual_tolerance = 100e-3
-picker.waveform_filter.frequency_min = 100
-picker.waveform_filter.frequency_max = 1000
-picker.p_wave.snr_window.noise = 0.005
-picker.p_wave.snr_window.signal = 0.01
-picker.s_wave.snr_window.noise = 0.005
-picker.s_wave.snr_window.signal = 0.01
-picker.p_wave.search_window.start = -100e-3        # start of search window relative to predicted arrival time (s)
-picker.p_wave.search_window.end = 10e-3           # end of the search window relative to predicted arrival time (s)
-picker.p_wave.search_window.resolution = 0.0005   # time resolution of search window (s)
-picker.s_wave.search_window.start = -100e-3        # start of search window relative to predicted arrival time (s)
-picker.s_wave.search_window.end = 20e-3           # end of the search window relative to predicted arrival time (s)
-picker.s_wave.search_window.resolution = 0.0005   # time resolution of search window (s)
-
-picker.second_pass.snr_threshold = 6
-picker.second_pass.min_num_picks = 20
-picker.second_pass.residual_tolerance = 25e-3
-picker.second_pass.waveform_filter.frequency_min = 100
-picker.second_pass.waveform_filter.frequency_max = 1000
-picker.second_pass.p_wave.snr_window.noise = 0.005
-picker.second_pass.p_wave.snr_window.signal = 0.01
-picker.second_pass.s_wave.snr_window.noise = 0.005
-picker.second_pass.s_wave.snr_window.signal = 0.01
-picker.second_pass.p_wave.search_window.start = -25e-3        # start of search window relative to predicted arrival time (s)
-picker.second_pass.p_wave.search_window.end = 25e-3           # end of the search window relative to predicted arrival time (s)
-picker.second_pass.p_wave.search_window.resolution = 0.0005   # time resolution of search window (s)
-picker.second_pass.s_wave.search_window.start = -25e-3        # start of search window relative to predicted arrival time (s)
-picker.second_pass.s_wave.search_window.end = 25e-3           # end of the search window relative to predicted arrival time (s)
-picker.second_pass.s_wave.search_window.resolution = 0.0005   # time resolution of search window (s)
-
-
-location.max_uncertainty = 75
-
-magnitude.ttpath = 'None'
-magnitude.only_triaxial = true
-magnitude.phase_list = 'P'
-magnitude.density = 2700
-magnitude.min_dist = 20
-magnitude.win_length = 0.02
-# len_spectrum is specified in exponent of 2. For instance 14 is equal to 2 ** 14
-magnitude.len_spectrum_exponent = 14
-# could instead specify <len_spectrum> directly
-magnitude.freq = 100
-magnitude.use_sdr_rad = false
-magnitude.use_free_surface_correction = false
-magnitude.make_preferred = true
-magnitude.use_smom = false
-
-magnitude.frequency.phase_list = ['P', 'S']
-magnitude.frequency.use_sdr_rad = false
-magnitude.frequency.make_preferred = false
-magnitude.frequency.use_smom = true
-magnitude.frequency.min_dist = 20
-
-focal_mechanism.npolmin = 8
-focal_mechanism.max_agap = 180
-focal_mechanism.max_pgap = 60
-focal_mechanism.dang = 5
-focal_mechanism.nmc = 30
-focal_mechanism.maxout = 500
-focal_mechanism.badfrac = 0.1
-focal_mechanism.delmax = 120
-focal_mechanism.cangle = 45
-focal_mechanism.prob_max = 0.25
-focal_mechanism.plot_focal_mechs = false
-
-measure_amplitudes.pulse_min_snr_P = 9
-measure_amplitudes.pulse_min_snr_S = 6
-measure_amplitudes.pulse_min_width = 0.0014
-measure_amplitudes.phase_list = 'P'
-
-measure_energy.phase_list = ['P', 'S']
-measure_energy.correct_attenuation = false
-measure_energy.attenuation_Q = 200
-measure_energy.use_sdr_rad = false
-
-measure_smom.phase_list = ['P', 'S']
-measure_smom.S_win_len = 0.1
-measure_smom.pre_window_start_sec = 0.01
-measure_smom.max_S_P_time = 0.25
-measure_smom.use_fixed_fmin_fmax = false
-# These are only used if use_fixed_fmin_fmax = true:
-measure_smom.fmin = 30.0
-measure_smom.fmax = 600.0
-
-kafka.brokers = 'spp-confluent-cp-kafka-headless:9092'
-kafka.group_id = 'seismic_processing_platform'
-kafka.threads = 3
-
-services.channel.interloc = 'spp.services.interloc'
-services.channel.picker = 'spp.services.picker'
-services.channel.nlloc = 'spp.services.nlloc'
-services.channel.magnitude = 'spp.services.magnitude'
-
-# this describes the kafka channel to which the message should be routed
-processing_flow.extract_waveforms.message_queue = 'spp.processing_flow.extract_waveforms'
-processing_flow.automatic.message_queue = 'spp.processing_flow.automatic'
-processing_flow.interactive.message_queue = 'spp.processing_flow.interactive'
-
-processing_flow.automatic.steps = [
-{ module='interloc', input='automatic'},
-{ module='picker'},
-{ module='nlloc'},
-{ module='measure_amplitudes'},
-{ module='measure_smom'},
-{ module='focal_mechanism'},
-{ module='measure_energy'},
-{ module='magnitude'},
-{ module='magnitude', type='frequency'},
-{ module='event_database'}
-]
-
-processing_flow.interactive.steps=[
-{ module='nlloc', input='interactive', output='magnitude'},
-{ module='magnitude', input='magnitude', output='magnitude_frequency'},
-{ module='magnitude', type='frequency', input='magnitude_frequency', output='event_database'},
-{ module='event_database', input='event_database'}
-]
-
-processing_flow.interactive_accepted.trigger_data_name = 'interactive_accepted'
-processing_flow.interactive_accepted.dataset = 'seismic_event'
-processing_flow.interactive_accepted.steps=[
-{ module='measure_smom', input='data_interactive_accepted', output='focal_mechanism'},
-{ module='focal_mechanism', input='focal_mechanism', output='measure_energy'},
-{ module='measure_energy', input='measure_energy', output='magnitude'},
-{ module='magnitude', input='magnitude', output='magnitude_frequency'},
-{ module='magnitude', type='frequency', input='magnitude_frequency', output='event_database'},
-{ module='event_database', input='event_database'}
-]
-
-
-# Settings used in tests to make sure dynaconf behaves as expected
-# (these tests are currently in seismic-api)
-
-testable_settings.def_only_in_microquake = 'not overridden'
-
-testable_settings.def_in_microquake_overrid_in_project = 'this should be overridden'
-
-testable_settings.foo.bar = "this should also be overridden"
-testable_settings.foo.baz = "also not overridden"
-
-testable_settings.bar.zzz = 'not touched from project'
-
-poor_testable_settings.lost = 'this should not be present in final settings'
-poor_testable_settings.why = 'because dynaconf_merge is not used here'
+time_zone.type = "UTC_offset"
+time_zone.time_zone_code = ""
+time_zone.offset = -6
+
+logger_level = '0'
+
+[site]
+black_list = []
+
+#dynaconf_include = ["*.toml"]
+#project.name = 'test'
+#project.network = 'OT'
+#project.base_directory = ''
+#api_base_url = 'https://api.microquake.org/api/v1/'
+#ims_base_url = 'http://10.95.74.35:8002/ims-database-server/databases/mgl'
+#project_code = 'OT'
+#site = 'Oyu Tolgoi'
+#site_code = 'OT'
+#network = 'Hugo North Ungerground Network'
+#network_code = 'OT'
+#redis_rq_url = ''
+#logging_level = 0
+#DEBUG_LEVEL = 0
+#DEBUG_FILE_DIR = '.'
+#
+#time_zone.type = 'UTC_offset'                # either 'UTC_offset or 'time_zone'
+#time_zone.time_zone_code = 'ULN'             # time zone code. If type=time_zone, time_zone_code must be a valid pytz timezone
+#time_zone.offset = 8                         # time offset in hours, ignored if type=time_zone
+#
+#pre_processing_message_queue = 'event_connector.pre_processing'
+#automatic_pipeline_message_queue = 'workflow.automatic'
+#api_message_queue = 'api'
+#
+#grids.units = 'meter'
+#grids.method = 'ODS'
+#grids.origin = [650200, 4766170, -500]
+#grids.dimensions = [100, 101, 68]
+#grids.spacing = [25, 25, 25]
+#grids.velocities.source = 'local'
+#grids.velocities.homogeneous = false
+#grids.velocities.vp = 'velocities/vp'
+#grids.velocities.vs = 'velocities/vs'
+#grids.velocities.format = 'NLLOC'
+#
+#grids.travel_time_h5.fname = 'travel_time_tables.h5f'
+#
+#sites.source     = 'local'
+#sites.units      = 'meter'
+#sites.format     = 'csv'
+#sites.path       = 'sites.csv'
+#sites.stationXML = 'OT_old.xml'
+#sites.black_list = ['7', '9', '10', '23', '25', '31', '32', '54', '91', '96', '99', '100', '102', '107', '88', '90', '77']
+#
+#ug_blast_windows_local_time = [7, 19]
+#ug_blast_windows_tolerance_minutes = 30
+#quakeml_ug_blast_type = 'explosion'
+#
+#data_connector.minimum_recovery_fraction = 0.85
+#data_connector.maximum_attempts = 10 # maximum number of attempts at retrieving the data
+#data_connector.minimum_delay_minutes = 0.5
+#data_connector.context_trace.filter.freqmin = 60
+#data_connector.context_trace.filter.freqmax = 500
+#data_connector.likelihood_threshold = 0.50
+#data_connector.reconciliation_delay_minutes = 60
+#data_connector.reconciliation_interval_hours = 72
+#data_connector.maximum_event_elevation = 900
+#data_connector.request_range_hours = 72
+#data_connector.closing_window_time_seconds = 60 # time after which we
+## consider the continuous data window closed after the event occurred
+#data_connector.context_trace_forbiden_site = ['7', '9']  # Accelerometers
+#
+#event_detection.sta_lta_on_value = 3.0
+#event_detection.sta_lta_off_value = 1.5
+#event_detection.sta_length_second = 10e-3
+#event_detection.lta_length_second = 100e-3
+#event_detection.onset_threshold = 3
+#event_detection.max_trigger_length_second = 0.2
+#event_detection.association_time_window_length_second = 1
+#event_detection.association_hold_off_time_second = 1.2 # from the start of the sequence
+##event_detection.seismogram_resulting_length_second = 2
+#
+##<STALTA_on value="3.0"/>
+##        <STALTA_off value="1.25"/>
+##        <STA value="10e-3"/>
+##		<LTA value="100e-3"/>
+##        <onset_threshold value="3"/> <!-- STALTA function threshold to declare a trigger -->
+##        <max_trigger_length value="0.05"/> <!-- maximum trigger length to declare a trigger valid -->
+##        <association_time value="0.1"/> <!-- length of time window within which trigger are associated -->
+##        <hold_off_time value="0.1"/> <!-- hold off time after an event has been detected to trigger another event -->
+##        <min_number_trigger value="5"/>  <!-- minimum number of trigger required to declare an event -->
+##        <seismogram_length value="300"/>
+#
+#event_classifier.likelihood_threshold = 0.5
+#event_classifier.blast_window_starts = [6, 18]
+#event_classifier.blast_window_ends = [8, 20]
+#event_classifier.valid_event_types = ['seismic event']
+#event_classifier.blast_event_types = ['underground blast']
+#event_classifier.uploaded_event_types = ['crusher noise', 'ore pass noise', 'test pulse', 'other blast', 'open pit blast']
+#event_classifier.ignore_type_large_event = ['underground blast', 'test pulse', 'open pit blast']
+#event_classifier.large_event_processing_threshold = 0.5
+#
+#interloc.nthreads = 4
+#interloc.samplerate_decimated = 3000.0
+#interloc.fixed_wlen_sec = 2.0
+#interloc.whiten_corner_freqs = [40.0, 50.0, 350.0, 360.0]
+#interloc.pair_dist_min = 0.0
+#interloc.pair_dist_max = 2000.0
+#interloc.cc_smooth_length_sec = 0.005
+#interloc.detection_threshold = 0.2
+#
+#compute_xcorrs.rolling_database_keep_hours = 80
+#compute_xcorrs.samplerate_decimated = 2000.0
+#compute_xcorrs.onebit_normalization = true
+#compute_xcorrs.whiten_corner_freqs = [40.0, 50.0, 390.0, 400.0]
+#compute_xcorrs.request_continuous_length_sec = 600
+#compute_xcorrs.request_continuous_lag_sec = 1800
+#compute_xcorrs.wlen_sec = 10
+#compute_xcorrs.stepsize_sec = 10
+#compute_xcorrs.keeplag_sec = 1.0
+#compute_xcorrs.stack_length_hours = 24.0
+#compute_xcorrs.pair_dist_min = 50.0
+#compute_xcorrs.pair_dist_max = 500.0
+#compute_xcorrs.channel_blacklist = ['.131.X', '.131.Y', '.131.Z', '.56.Y', '.67.Y', '.83.X', '.86.X', '.86.Y', '.86.Z', '.88.X', '.88.Y', '.88.Z', '.90.X', '.90.Z']
+#
+#
+#compute_velchange.coda_start_velocity = 3000.0
+#compute_velchange.coda_end_sec = 0.8
+#compute_velchange.freq_band_measure = [70.0, 240.0]
+#compute_velchange.wlen_sec = 0.02
+#compute_velchange.step_factor = 10
+#compute_velchange.coherence_welch_nwin = 10
+#
+## parameter of the PPV vs Magnitude relationship
+#quick_magnitude.a = 1.2
+#quick_magnitude.c = 1.1
+#
+#picker.snr_threshold = 8
+#picker.min_num_picks = 20
+#picker.residual_tolerance = 100e-3
+#picker.waveform_filter.frequency_min = 100
+#picker.waveform_filter.frequency_max = 1000
+#picker.p_wave.snr_window.noise = 0.005
+#picker.p_wave.snr_window.signal = 0.01
+#picker.s_wave.snr_window.noise = 0.005
+#picker.s_wave.snr_window.signal = 0.01
+#picker.p_wave.search_window.start = -100e-3        # start of search window relative to predicted arrival time (s)
+#picker.p_wave.search_window.end = 10e-3           # end of the search window relative to predicted arrival time (s)
+#picker.p_wave.search_window.resolution = 0.0005   # time resolution of search window (s)
+#picker.s_wave.search_window.start = -100e-3        # start of search window relative to predicted arrival time (s)
+#picker.s_wave.search_window.end = 20e-3           # end of the search window relative to predicted arrival time (s)
+#picker.s_wave.search_window.resolution = 0.0005   # time resolution of search window (s)
+#
+#picker.second_pass.snr_threshold = 6
+#picker.second_pass.min_num_picks = 20
+#picker.second_pass.residual_tolerance = 25e-3
+#picker.second_pass.waveform_filter.frequency_min = 100
+#picker.second_pass.waveform_filter.frequency_max = 1000
+#picker.second_pass.p_wave.snr_window.noise = 0.005
+#picker.second_pass.p_wave.snr_window.signal = 0.01
+#picker.second_pass.s_wave.snr_window.noise = 0.005
+#picker.second_pass.s_wave.snr_window.signal = 0.01
+#picker.second_pass.p_wave.search_window.start = -25e-3        # start of search window relative to predicted arrival time (s)
+#picker.second_pass.p_wave.search_window.end = 25e-3           # end of the search window relative to predicted arrival time (s)
+#picker.second_pass.p_wave.search_window.resolution = 0.0005   # time resolution of search window (s)
+#picker.second_pass.s_wave.search_window.start = -25e-3        # start of search window relative to predicted arrival time (s)
+#picker.second_pass.s_wave.search_window.end = 25e-3           # end of the search window relative to predicted arrival time (s)
+#picker.second_pass.s_wave.search_window.resolution = 0.0005   # time resolution of search window (s)
+#
+#
+#location.max_uncertainty = 75
+#
+#magnitude.ttpath = 'None'
+#magnitude.only_triaxial = true
+#magnitude.phase_list = 'P'
+#magnitude.density = 2700
+#magnitude.min_dist = 20
+#magnitude.win_length = 0.02
+## len_spectrum is specified in exponent of 2. For instance 14 is equal to 2 ** 14
+#magnitude.len_spectrum_exponent = 14
+## could instead specify <len_spectrum> directly
+#magnitude.freq = 100
+#magnitude.use_sdr_rad = false
+#magnitude.use_free_surface_correction = false
+#magnitude.make_preferred = true
+#magnitude.use_smom = false
+#
+#magnitude.frequency.phase_list = ['P', 'S']
+#magnitude.frequency.use_sdr_rad = false
+#magnitude.frequency.make_preferred = false
+#magnitude.frequency.use_smom = true
+#magnitude.frequency.min_dist = 20
+#
+#focal_mechanism.npolmin = 8
+#focal_mechanism.max_agap = 180
+#focal_mechanism.max_pgap = 60
+#focal_mechanism.dang = 5
+#focal_mechanism.nmc = 30
+#focal_mechanism.maxout = 500
+#focal_mechanism.badfrac = 0.1
+#focal_mechanism.delmax = 120
+#focal_mechanism.cangle = 45
+#focal_mechanism.prob_max = 0.25
+#focal_mechanism.plot_focal_mechs = false
+#
+#measure_amplitudes.pulse_min_snr_P = 9
+#measure_amplitudes.pulse_min_snr_S = 6
+#measure_amplitudes.pulse_min_width = 0.0014
+#measure_amplitudes.phase_list = 'P'
+#
+#measure_energy.phase_list = ['P', 'S']
+#measure_energy.correct_attenuation = false
+#measure_energy.attenuation_Q = 200
+#measure_energy.use_sdr_rad = false
+#
+#measure_smom.phase_list = ['P', 'S']
+#measure_smom.S_win_len = 0.1
+#measure_smom.pre_window_start_sec = 0.01
+#measure_smom.max_S_P_time = 0.25
+#measure_smom.use_fixed_fmin_fmax = false
+## These are only used if use_fixed_fmin_fmax = true:
+#measure_smom.fmin = 30.0
+#measure_smom.fmax = 600.0
+#
+#kafka.brokers = 'spp-confluent-cp-kafka-headless:9092'
+#kafka.group_id = 'seismic_processing_platform'
+#kafka.threads = 3
+#
+#services.channel.interloc = 'spp.services.interloc'
+#services.channel.picker = 'spp.services.picker'
+#services.channel.nlloc = 'spp.services.nlloc'
+#services.channel.magnitude = 'spp.services.magnitude'
+#
+## this describes the kafka channel to which the message should be routed
+#processing_flow.extract_waveforms.message_queue = 'spp.processing_flow.extract_waveforms'
+#processing_flow.automatic.message_queue = 'spp.processing_flow.automatic'
+#processing_flow.interactive.message_queue = 'spp.processing_flow.interactive'
+#
+#processing_flow.automatic.steps = [
+#{ module='interloc', input='automatic'},
+#{ module='picker'},
+#{ module='nlloc'},
+#{ module='measure_amplitudes'},
+#{ module='measure_smom'},
+#{ module='focal_mechanism'},
+#{ module='measure_energy'},
+#{ module='magnitude'},
+#{ module='magnitude', type='frequency'},
+#{ module='event_database'}
+#]
+#
+#processing_flow.interactive.steps=[
+#{ module='nlloc', input='interactive', output='magnitude'},
+#{ module='magnitude', input='magnitude', output='magnitude_frequency'},
+#{ module='magnitude', type='frequency', input='magnitude_frequency', output='event_database'},
+#{ module='event_database', input='event_database'}
+#]
+#
+#processing_flow.interactive_accepted.trigger_data_name = 'interactive_accepted'
+#processing_flow.interactive_accepted.dataset = 'seismic_event'
+#processing_flow.interactive_accepted.steps=[
+#{ module='measure_smom', input='data_interactive_accepted', output='focal_mechanism'},
+#{ module='focal_mechanism', input='focal_mechanism', output='measure_energy'},
+#{ module='measure_energy', input='measure_energy', output='magnitude'},
+#{ module='magnitude', input='magnitude', output='magnitude_frequency'},
+#{ module='magnitude', type='frequency', input='magnitude_frequency', output='event_database'},
+#{ module='event_database', input='event_database'}
+#]
+#
+#
+## Settings used in tests to make sure dynaconf behaves as expected
+## (these tests are currently in seismic-api)
+#
+#testable_settings.def_only_in_microquake = 'not overridden'
+#
+#testable_settings.def_in_microquake_overrid_in_project = 'this should be overridden'
+#
+#testable_settings.foo.bar = "this should also be overridden"
+#testable_settings.foo.baz = "also not overridden"
+#
+#testable_settings.bar.zzz = 'not touched from project'
+#
+#poor_testable_settings.lost = 'this should not be present in final settings'
+#poor_testable_settings.why = 'because dynaconf_merge is not used here'
```

### Comparing `useis-0.9.9/useis/services/file_server/database.py` & `useis-1.0.0/useis/services/file_server/database.py`

 * *Files identical despite different names*

### Comparing `useis-0.9.9/useis/services/file_server/indexer.py` & `useis-1.0.0/useis/services/file_server/indexer.py`

 * *Files identical despite different names*

### Comparing `useis-0.9.9/useis/services/grid_service/client.py` & `useis-1.0.0/useis/services/grid_service/client.py`

 * *Files identical despite different names*

### Comparing `useis-0.9.9/useis/services/grid_service/server.py` & `useis-1.0.0/useis/services/grid_service/server.py`

 * *Files identical despite different names*

### Comparing `useis-0.9.9/useis/services/grid_service/test.py` & `useis-1.0.0/useis/services/grid_service/test.py`

 * *Files identical despite different names*

### Comparing `useis-0.9.9/useis/services/models/event.py` & `useis-1.0.0/useis/services/models/event.py`

 * *Files identical despite different names*

### Comparing `useis-0.9.9/useis/services/models/grid.py` & `useis-1.0.0/useis/services/models/grid.py`

 * *Files identical despite different names*

### Comparing `useis-0.9.9/useis/services/models/nlloc.py` & `useis-1.0.0/useis/services/models/nlloc.py`

 * *Files identical despite different names*

### Comparing `useis-0.9.9/useis/settings/nlloc_settings_template.py` & `useis-1.0.0/useis/settings/nlloc_settings_template.py`

 * *Files identical despite different names*

### Comparing `useis-0.9.9/useis/settings/settings.py` & `useis-1.0.0/useis/settings/settings.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 import os
 from dynaconf import LazySettings
 from pathlib import Path
 
 
 class Settings(LazySettings):
-    def __init__(self, settings_location, settings_file='settings.toml'):
+    def __init__(self, settings_location):
         """
         Init function currently just initializes the object allowing
         """
 
+        settings_file = 'settings.toml'
+    
         config_dir = Path(settings_location)
 
         dconf = {}
-        dconf.setdefault('ENVVAR_PREFIX_FOR_DYNACONF', 'UQUAKE')
+        dconf.setdefault('ENVVAR_PREFIX_FOR_DYNACONF', 'USEIS')
 
         env_prefix = '{0}_ENV'.format(
             dconf['ENVVAR_PREFIX_FOR_DYNACONF']
         )  # SPP_ENV
 
         dconf.setdefault(
             'ENV_FOR_DYNACONF',
```

### Comparing `useis-0.9.9/setup.py` & `useis-1.0.0/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,63 +1,72 @@
 # -*- coding: utf-8 -*-
 from setuptools import setup
 
 packages = \
 ['useis',
  'useis.ai',
+ 'useis.clients',
  'useis.core',
+ 'useis.examples.classifier',
+ 'useis.examples.picker',
  'useis.processors',
  'useis.sandbox',
+ 'useis.sandbox.ai_picker',
  'useis.sandbox.demo_kafka',
+ 'useis.sandbox.event_classification',
+ 'useis.sandbox.event_classification.inventory',
+ 'useis.sandbox.event_classification_2',
+ 'useis.sandbox.tomography',
+ 'useis.scripts',
+ 'useis.scripts.ai',
  'useis.services',
+ 'useis.services.classifier',
  'useis.services.file_server',
  'useis.services.grid_service',
  'useis.services.models',
- 'useis.settings']
+ 'useis.settings',
+ 'useis.tomography']
 
 package_data = \
-{'': ['*'],
- 'useis.sandbox': ['demo_useis/*',
-                   'demo_useis/test/test/TN/config/*',
-                   'demo_useis/test/test/TN/templates/*']}
+{'': ['*']}
 
 install_requires = \
 ['confluent-kafka>=1.7.0,<2.0.0',
  'dynaconf>=3.1.4,<4.0.0',
  'fastapi>=0.68.1,<0.69.0',
  'furl>=2.1.2,<3.0.0',
  'myst-parser>=0.15.1,<0.16.0',
  'numpy>=1.21.3,<2.0.0',
+ 'pillow>=9.4.0,<10.0.0',
  'pydantic>=1.8.2,<2.0.0',
+ 'pyproj==3.4.1',
  'python-multipart>=0.0.5,<0.0.6',
  'rinohtype>=0.5.3,<0.6.0',
  'scikit-learn>=1.0.1,<2.0.0',
- 'sklearn>=0.0,<0.1',
- 'torch>=1.10.0,<2.0.0',
- 'torchaudio>=0.10.0,<0.11.0',
- 'torchvision>=0.11.1,<0.12.0',
- 'tqdm>=4.59.0,<5.0.0',
- 'uquake>=0.9.6,<0.10.0',
+ 'torch>=2.0.0,<3.0.0',
+ 'torchaudio>=2.0.1,<3.0.0',
+ 'torchvision>=0.15.1,<0.16.0',
+ 'uquake>=1.2.4,<2.0.0',
  'uvicorn>=0.15.0,<0.16.0']
 
 extras_require = \
 {':extra == "docs"': ['Sphinx>=4.1.2,<5.0.0', 'sphinx-rtd-theme>=0.5.2,<0.6.0']}
 
 setup_kwargs = {
     'name': 'useis',
-    'version': '0.9.9',
+    'version': '1.0.0',
     'description': '',
-    'long_description': None,
+    'long_description': 'None',
     'author': 'jpmercier',
     'author_email': 'jpmercier01@gmail.com',
-    'maintainer': None,
-    'maintainer_email': None,
-    'url': None,
+    'maintainer': 'None',
+    'maintainer_email': 'None',
+    'url': 'None',
     'packages': packages,
     'package_data': package_data,
     'install_requires': install_requires,
     'extras_require': extras_require,
-    'python_requires': '>=3.7.1,<3.11',
+    'python_requires': '>=3.9,<4.0',
 }
 
 
 setup(**setup_kwargs)
```

### Comparing `useis-0.9.9/PKG-INFO` & `useis-1.0.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,32 +1,33 @@
 Metadata-Version: 2.1
 Name: useis
-Version: 0.9.9
+Version: 1.0.0
 Summary: 
 License: MIT
 Author: jpmercier
 Author-email: jpmercier01@gmail.com
-Requires-Python: >=3.7.1,<3.11
+Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Provides-Extra: docs
-Requires-Dist: Sphinx (>=4.1.2,<5.0.0); extra == "docs"
+Requires-Dist: Sphinx (>=4.1.2,<5.0.0) ; extra == "docs"
 Requires-Dist: confluent-kafka (>=1.7.0,<2.0.0)
 Requires-Dist: dynaconf (>=3.1.4,<4.0.0)
 Requires-Dist: fastapi (>=0.68.1,<0.69.0)
 Requires-Dist: furl (>=2.1.2,<3.0.0)
 Requires-Dist: myst-parser (>=0.15.1,<0.16.0)
 Requires-Dist: numpy (>=1.21.3,<2.0.0)
+Requires-Dist: pillow (>=9.4.0,<10.0.0)
 Requires-Dist: pydantic (>=1.8.2,<2.0.0)
+Requires-Dist: pyproj (==3.4.1)
 Requires-Dist: python-multipart (>=0.0.5,<0.0.6)
 Requires-Dist: rinohtype (>=0.5.3,<0.6.0)
 Requires-Dist: scikit-learn (>=1.0.1,<2.0.0)
-Requires-Dist: sklearn (>=0.0,<0.1)
-Requires-Dist: sphinx-rtd-theme (>=0.5.2,<0.6.0); extra == "docs"
-Requires-Dist: torch (>=1.10.0,<2.0.0)
-Requires-Dist: torchaudio (>=0.10.0,<0.11.0)
-Requires-Dist: torchvision (>=0.11.1,<0.12.0)
-Requires-Dist: tqdm (>=4.59.0,<5.0.0)
-Requires-Dist: uquake (>=0.9.6,<0.10.0)
+Requires-Dist: sphinx-rtd-theme (>=0.5.2,<0.6.0) ; extra == "docs"
+Requires-Dist: torch (>=2.0.0,<3.0.0)
+Requires-Dist: torchaudio (>=2.0.1,<3.0.0)
+Requires-Dist: torchvision (>=0.15.1,<0.16.0)
+Requires-Dist: uquake (>=1.2.4,<2.0.0)
 Requires-Dist: uvicorn (>=0.15.0,<0.16.0)
```

