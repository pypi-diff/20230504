# Comparing `tmp/annotation_tool-0.8.2.tar.gz` & `tmp/annotation_tool-0.8.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "annotation_tool-0.8.2.tar", max compression
+gzip compressed data, was "annotation_tool-0.8.3.tar", max compression
```

## Comparing `annotation_tool-0.8.2.tar` & `annotation_tool-0.8.3.tar`

### file list

```diff
@@ -1,96 +1,96 @@
--rw-r--r--   0        0        0     1085 2023-04-21 14:45:35.790131 annotation_tool-0.8.2/LICENSE
--rw-r--r--   0        0        0     1280 2023-04-21 14:45:35.790131 annotation_tool-0.8.2/README.md
--rw-r--r--   0        0        0       68 2023-04-21 14:45:35.790131 annotation_tool-0.8.2/annotation_tool/__init__.py
--rw-r--r--   0        0        0        0 2023-04-21 14:45:35.790131 annotation_tool-0.8.2/annotation_tool/annotation/__init__.py
--rw-r--r--   0        0        0     8480 2023-04-21 14:45:35.790131 annotation_tool-0.8.2/annotation_tool/annotation/annotation_base.py
--rw-r--r--   0        0        0     5170 2023-04-21 14:45:35.790131 annotation_tool-0.8.2/annotation_tool/annotation/controller.py
--rw-r--r--   0        0        0        0 2023-04-21 14:45:35.790131 annotation_tool-0.8.2/annotation_tool/annotation/manual/__init__.py
--rw-r--r--   0        0        0     5852 2023-04-21 14:45:35.790131 annotation_tool-0.8.2/annotation_tool/annotation/manual/controller.py
--rw-r--r--   0        0        0     3075 2023-04-21 14:45:35.790131 annotation_tool-0.8.2/annotation_tool/annotation/manual/main_widget.py
--rw-r--r--   0        0        0     2456 2023-04-21 14:45:35.790131 annotation_tool-0.8.2/annotation_tool/annotation/manual/tool_widget.py
--rw-r--r--   0        0        0       80 2023-04-21 14:45:35.790131 annotation_tool-0.8.2/annotation_tool/annotation/modes.py
--rw-r--r--   0        0        0        0 2023-04-21 14:45:35.790131 annotation_tool-0.8.2/annotation_tool/annotation/retrieval/__init__.py
--rw-r--r--   0        0        0    12649 2023-04-21 14:45:35.790131 annotation_tool-0.8.2/annotation_tool/annotation/retrieval/controller.py
--rw-r--r--   0        0        0     3828 2023-04-21 14:45:35.790131 annotation_tool-0.8.2/annotation_tool/annotation/retrieval/main_widget.py
--rw-r--r--   0        0        0        0 2023-04-21 14:45:35.790131 annotation_tool-0.8.2/annotation_tool/annotation/retrieval/retrieval_backend/__init__.py
--rw-r--r--   0        0        0      917 2023-04-21 14:45:35.790131 annotation_tool-0.8.2/annotation_tool/annotation/retrieval/retrieval_backend/element.py
--rw-r--r--   0        0        0     1969 2023-04-21 14:45:35.790131 annotation_tool-0.8.2/annotation_tool/annotation/retrieval/retrieval_backend/filter.py
--rw-r--r--   0        0        0     2184 2023-04-21 14:45:35.790131 annotation_tool-0.8.2/annotation_tool/annotation/retrieval/retrieval_backend/filter_dialog.py
--rw-r--r--   0        0        0     6370 2023-04-21 14:45:35.790131 annotation_tool-0.8.2/annotation_tool/annotation/retrieval/retrieval_backend/loader.py
--rw-r--r--   0        0        0    12318 2023-04-21 14:45:35.790131 annotation_tool-0.8.2/annotation_tool/annotation/retrieval/retrieval_backend/query.py
--rw-r--r--   0        0        0     8256 2023-04-21 14:45:35.790131 annotation_tool-0.8.2/annotation_tool/annotation/retrieval/retrieval_backend/queue.py
--rw-r--r--   0        0        0     2013 2023-04-21 14:45:35.794131 annotation_tool-0.8.2/annotation_tool/annotation/retrieval/tool_widget.py
--rw-r--r--   0        0        0    14145 2023-04-21 14:45:35.794131 annotation_tool-0.8.2/annotation_tool/annotation/timeline.py
--rw-r--r--   0        0        0      479 2023-04-21 14:45:35.794131 annotation_tool-0.8.2/annotation_tool/data_model/__init__.py
--rw-r--r--   0        0        0     7726 2023-04-21 14:45:35.794131 annotation_tool-0.8.2/annotation_tool/data_model/annotation.py
--rw-r--r--   0        0        0     2077 2023-04-21 14:45:35.794131 annotation_tool-0.8.2/annotation_tool/data_model/annotation_scheme.py
--rw-r--r--   0        0        0     3003 2023-04-21 14:45:35.794131 annotation_tool-0.8.2/annotation_tool/data_model/dataset.py
--rw-r--r--   0        0        0      795 2023-04-21 14:45:35.794131 annotation_tool-0.8.2/annotation_tool/data_model/media_type.py
--rw-r--r--   0        0        0     4014 2023-04-21 14:45:35.794131 annotation_tool-0.8.2/annotation_tool/data_model/model.py
--rw-r--r--   0        0        0     2040 2023-04-21 14:45:35.794131 annotation_tool-0.8.2/annotation_tool/data_model/project.py
--rw-r--r--   0        0        0     3664 2023-04-21 14:45:35.794131 annotation_tool-0.8.2/annotation_tool/data_model/sample.py
--rw-r--r--   0        0        0     6412 2023-04-21 14:45:35.794131 annotation_tool-0.8.2/annotation_tool/data_model/single_annotation.py
--rw-r--r--   0        0        0        0 2023-04-21 14:45:35.794131 annotation_tool-0.8.2/annotation_tool/dialogs/__init__.py
--rw-r--r--   0        0        0    12197 2023-04-21 14:45:35.794131 annotation_tool-0.8.2/annotation_tool/dialogs/annotation_dialog.py
--rw-r--r--   0        0        0    10523 2023-04-21 14:45:35.794131 annotation_tool-0.8.2/annotation_tool/dialogs/annotation_list.py
--rw-r--r--   0        0        0     1956 2023-04-21 14:45:35.794131 annotation_tool-0.8.2/annotation_tool/dialogs/dialog_manager.py
--rw-r--r--   0        0        0     7082 2023-04-21 14:45:35.794131 annotation_tool-0.8.2/annotation_tool/dialogs/edit_datasets.py
--rw-r--r--   0        0        0    10994 2023-04-21 14:45:35.794131 annotation_tool-0.8.2/annotation_tool/dialogs/import_annotation_dialog.py
--rw-r--r--   0        0        0     5706 2023-04-21 14:45:35.794131 annotation_tool-0.8.2/annotation_tool/dialogs/load_annotation_dialog.py
--rw-r--r--   0        0        0     3670 2023-04-21 14:45:35.794131 annotation_tool-0.8.2/annotation_tool/dialogs/local_files.py
--rw-r--r--   0        0        0    10576 2023-04-21 14:45:35.794131 annotation_tool-0.8.2/annotation_tool/dialogs/network_list.py
--rw-r--r--   0        0        0     6899 2023-04-21 14:45:35.794131 annotation_tool-0.8.2/annotation_tool/dialogs/new_annotation_dialog.py
--rw-r--r--   0        0        0    19491 2023-04-21 14:45:35.794131 annotation_tool-0.8.2/annotation_tool/dialogs/settings_dialog.py
--rw-r--r--   0        0        0      197 2023-04-21 14:45:35.794131 annotation_tool-0.8.2/annotation_tool/file_cache/__init__.py
--rw-r--r--   0        0        0     9586 2023-04-21 14:45:35.794131 annotation_tool-0.8.2/annotation_tool/file_cache/_file_cache.py
--rw-r--r--   0        0        0     8506 2023-04-21 14:45:35.794131 annotation_tool-0.8.2/annotation_tool/gui.py
--rw-r--r--   0        0        0    12322 2023-04-21 14:45:35.794131 annotation_tool-0.8.2/annotation_tool/main_controller.py
--rw-r--r--   0        0        0        0 2023-04-21 14:45:35.794131 annotation_tool-0.8.2/annotation_tool/media/__init__.py
--rw-r--r--   0        0        0        0 2023-04-21 14:45:35.794131 annotation_tool-0.8.2/annotation_tool/media/backend/__init__.py
--rw-r--r--   0        0        0    10152 2023-04-21 14:45:35.794131 annotation_tool-0.8.2/annotation_tool/media/backend/controller.py
--rw-r--r--   0        0        0     4220 2023-04-21 14:45:35.794131 annotation_tool-0.8.2/annotation_tool/media/backend/player.py
--rw-r--r--   0        0        0     5327 2023-04-21 14:45:35.794131 annotation_tool-0.8.2/annotation_tool/media/backend/timer.py
--rw-r--r--   0        0        0        0 2023-04-21 14:45:35.794131 annotation_tool-0.8.2/annotation_tool/media/backend/type_specific_player/__init__.py
--rw-r--r--   0        0        0     8424 2023-04-21 14:45:35.794131 annotation_tool-0.8.2/annotation_tool/media/backend/type_specific_player/mocap.py
--rw-r--r--   0        0        0     7082 2023-04-21 14:45:35.794131 annotation_tool-0.8.2/annotation_tool/media/backend/type_specific_player/video.py
--rw-r--r--   0        0        0     2286 2023-04-21 14:45:35.794131 annotation_tool-0.8.2/annotation_tool/media/media.py
--rw-r--r--   0        0        0      357 2023-04-21 14:45:35.794131 annotation_tool-0.8.2/annotation_tool/media_reader/__init__.py
--rw-r--r--   0        0        0     8866 2023-04-21 14:45:35.794131 annotation_tool-0.8.2/annotation_tool/media_reader/base.py
--rw-r--r--   0        0        0     2167 2023-04-21 14:45:35.794131 annotation_tool-0.8.2/annotation_tool/media_reader/mocap.py
--rw-r--r--   0        0        0      121 2023-04-21 14:45:35.794131 annotation_tool-0.8.2/annotation_tool/media_reader/mocap_readers/__init__.py
--rw-r--r--   0        0        0     3128 2023-04-21 14:45:35.794131 annotation_tool-0.8.2/annotation_tool/media_reader/mocap_readers/base.py
--rw-r--r--   0        0        0     4745 2023-04-21 14:45:35.794131 annotation_tool-0.8.2/annotation_tool/media_reader/mocap_readers/cache.py
--rw-r--r--   0        0        0     6020 2023-04-21 14:45:35.794131 annotation_tool-0.8.2/annotation_tool/media_reader/mocap_readers/lara_reader.py
--rw-r--r--   0        0        0     1787 2023-04-21 14:45:35.794131 annotation_tool-0.8.2/annotation_tool/media_reader/video.py
--rw-r--r--   0        0        0      157 2023-04-21 14:45:35.794131 annotation_tool-0.8.2/annotation_tool/media_reader/video_readers/__init__.py
--rw-r--r--   0        0        0     4096 2023-04-21 14:45:35.794131 annotation_tool-0.8.2/annotation_tool/media_reader/video_readers/base.py
--rw-r--r--   0        0        0     3668 2023-04-21 14:45:35.794131 annotation_tool-0.8.2/annotation_tool/media_reader/video_readers/decord_reader.py
--rw-r--r--   0        0        0     4321 2023-04-21 14:45:35.794131 annotation_tool-0.8.2/annotation_tool/media_reader/video_readers/evaluation.py
--rw-r--r--   0        0        0     7496 2023-04-21 14:45:35.794131 annotation_tool-0.8.2/annotation_tool/media_reader/video_readers/opencv_reader.py
--rw-r--r--   0        0        0     4170 2023-04-21 14:45:35.794131 annotation_tool-0.8.2/annotation_tool/mediator.py
--rw-r--r--   0        0        0        0 2023-04-21 14:45:35.798131 annotation_tool-0.8.2/annotation_tool/network/LARa/__init__.py
--rw-r--r--   0        0        0    12119 2023-04-21 14:45:35.798131 annotation_tool-0.8.2/annotation_tool/network/LARa/attr_per_class.txt
--rw-r--r--   0        0        0     5583 2023-04-21 14:45:35.798131 annotation_tool-0.8.2/annotation_tool/network/LARa/lara_specifics.py
--rw-r--r--   0        0        0        0 2023-04-21 14:45:35.798131 annotation_tool-0.8.2/annotation_tool/network/__init__.py
--rw-r--r--   0        0        0     7267 2023-04-21 14:45:35.798131 annotation_tool-0.8.2/annotation_tool/network/controller.py
--rw-r--r--   0        0        0    27224 2023-04-21 14:45:35.798131 annotation_tool-0.8.2/annotation_tool/network/network.py
--rw-r--r--   0        0        0     7556 2023-04-21 14:45:35.798131 annotation_tool-0.8.2/annotation_tool/playback.py
--rw-r--r--   0        0        0     1546 2023-04-21 14:45:35.798131 annotation_tool-0.8.2/annotation_tool/qt_helper_widgets/adaptive_scroll_area.py
--rw-r--r--   0        0        0     4401 2023-04-21 14:45:35.798131 annotation_tool-0.8.2/annotation_tool/qt_helper_widgets/checkable_combobox.py
--rw-r--r--   0        0        0     2170 2023-04-21 14:45:35.798131 annotation_tool-0.8.2/annotation_tool/qt_helper_widgets/display_scheme.py
--rw-r--r--   0        0        0     1798 2023-04-21 14:45:35.798131 annotation_tool-0.8.2/annotation_tool/qt_helper_widgets/histogram.py
--rw-r--r--   0        0        0      458 2023-04-21 14:45:35.798131 annotation_tool-0.8.2/annotation_tool/qt_helper_widgets/line_edit_adapted.py
--rw-r--r--   0        0        0      403 2023-04-21 14:45:35.798131 annotation_tool-0.8.2/annotation_tool/qt_helper_widgets/lines.py
--rw-r--r--   0        0        0     1077 2023-04-21 14:45:35.798131 annotation_tool-0.8.2/annotation_tool/qt_helper_widgets/own_slider.py
--rw-r--r--   0        0        0     1480 2023-04-21 14:45:35.798131 annotation_tool-0.8.2/annotation_tool/settings.py
--rw-r--r--   0        0        0     4037 2023-04-21 14:45:35.798131 annotation_tool-0.8.2/annotation_tool/user_actions.py
--rw-r--r--   0        0        0        0 2023-04-21 14:45:35.798131 annotation_tool-0.8.2/annotation_tool/utility/__init__.py
--rw-r--r--   0        0        0     4818 2023-04-21 14:45:35.798131 annotation_tool-0.8.2/annotation_tool/utility/decorators.py
--rw-r--r--   0        0        0    11854 2023-04-21 14:45:35.798131 annotation_tool-0.8.2/annotation_tool/utility/filehandler.py
--rw-r--r--   0        0        0     4059 2023-04-21 14:45:35.798131 annotation_tool-0.8.2/annotation_tool/utility/functions.py
--rw-r--r--   0        0        0     2153 2023-04-21 14:45:35.798131 annotation_tool-0.8.2/annotation_tool/utility/networking.py
--rw-r--r--   0        0        0     4469 2023-04-21 14:45:35.798131 annotation_tool-0.8.2/annotation_tool/utility/priority_queue.py
--rw-r--r--   0        0        0    53863 2023-04-21 14:45:35.798131 annotation_tool-0.8.2/annotation_tool/utility/resources.py
--rw-r--r--   0        0        0     1938 2023-04-21 14:45:35.802132 annotation_tool-0.8.2/main.py
--rw-r--r--   0        0        0     1949 2023-04-21 14:45:35.802132 annotation_tool-0.8.2/pyproject.toml
--rw-r--r--   0        0        0     2522 1970-01-01 00:00:00.000000 annotation_tool-0.8.2/PKG-INFO
+-rw-r--r--   0        0        0     1085 2023-05-04 12:28:40.283202 annotation_tool-0.8.3/LICENSE
+-rw-r--r--   0        0        0     1280 2023-05-04 12:28:40.283202 annotation_tool-0.8.3/README.md
+-rw-r--r--   0        0        0       68 2023-05-04 12:28:40.283202 annotation_tool-0.8.3/annotation_tool/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-04 12:28:40.283202 annotation_tool-0.8.3/annotation_tool/annotation/__init__.py
+-rw-r--r--   0        0        0     8480 2023-05-04 12:28:40.283202 annotation_tool-0.8.3/annotation_tool/annotation/annotation_base.py
+-rw-r--r--   0        0        0     5170 2023-05-04 12:28:40.283202 annotation_tool-0.8.3/annotation_tool/annotation/controller.py
+-rw-r--r--   0        0        0        0 2023-05-04 12:28:40.283202 annotation_tool-0.8.3/annotation_tool/annotation/manual/__init__.py
+-rw-r--r--   0        0        0     5852 2023-05-04 12:28:40.283202 annotation_tool-0.8.3/annotation_tool/annotation/manual/controller.py
+-rw-r--r--   0        0        0     3075 2023-05-04 12:28:40.283202 annotation_tool-0.8.3/annotation_tool/annotation/manual/main_widget.py
+-rw-r--r--   0        0        0     2456 2023-05-04 12:28:40.283202 annotation_tool-0.8.3/annotation_tool/annotation/manual/tool_widget.py
+-rw-r--r--   0        0        0       80 2023-05-04 12:28:40.283202 annotation_tool-0.8.3/annotation_tool/annotation/modes.py
+-rw-r--r--   0        0        0        0 2023-05-04 12:28:40.283202 annotation_tool-0.8.3/annotation_tool/annotation/retrieval/__init__.py
+-rw-r--r--   0        0        0    12649 2023-05-04 12:28:40.283202 annotation_tool-0.8.3/annotation_tool/annotation/retrieval/controller.py
+-rw-r--r--   0        0        0     3828 2023-05-04 12:28:40.283202 annotation_tool-0.8.3/annotation_tool/annotation/retrieval/main_widget.py
+-rw-r--r--   0        0        0        0 2023-05-04 12:28:40.283202 annotation_tool-0.8.3/annotation_tool/annotation/retrieval/retrieval_backend/__init__.py
+-rw-r--r--   0        0        0      917 2023-05-04 12:28:40.283202 annotation_tool-0.8.3/annotation_tool/annotation/retrieval/retrieval_backend/element.py
+-rw-r--r--   0        0        0     1969 2023-05-04 12:28:40.283202 annotation_tool-0.8.3/annotation_tool/annotation/retrieval/retrieval_backend/filter.py
+-rw-r--r--   0        0        0     2184 2023-05-04 12:28:40.283202 annotation_tool-0.8.3/annotation_tool/annotation/retrieval/retrieval_backend/filter_dialog.py
+-rw-r--r--   0        0        0     6370 2023-05-04 12:28:40.283202 annotation_tool-0.8.3/annotation_tool/annotation/retrieval/retrieval_backend/loader.py
+-rw-r--r--   0        0        0    12318 2023-05-04 12:28:40.283202 annotation_tool-0.8.3/annotation_tool/annotation/retrieval/retrieval_backend/query.py
+-rw-r--r--   0        0        0     8256 2023-05-04 12:28:40.283202 annotation_tool-0.8.3/annotation_tool/annotation/retrieval/retrieval_backend/queue.py
+-rw-r--r--   0        0        0     2013 2023-05-04 12:28:40.283202 annotation_tool-0.8.3/annotation_tool/annotation/retrieval/tool_widget.py
+-rw-r--r--   0        0        0    14145 2023-05-04 12:28:40.283202 annotation_tool-0.8.3/annotation_tool/annotation/timeline.py
+-rw-r--r--   0        0        0      479 2023-05-04 12:28:40.283202 annotation_tool-0.8.3/annotation_tool/data_model/__init__.py
+-rw-r--r--   0        0        0     7726 2023-05-04 12:28:40.287202 annotation_tool-0.8.3/annotation_tool/data_model/annotation.py
+-rw-r--r--   0        0        0     2077 2023-05-04 12:28:40.287202 annotation_tool-0.8.3/annotation_tool/data_model/annotation_scheme.py
+-rw-r--r--   0        0        0     3003 2023-05-04 12:28:40.287202 annotation_tool-0.8.3/annotation_tool/data_model/dataset.py
+-rw-r--r--   0        0        0      795 2023-05-04 12:28:40.287202 annotation_tool-0.8.3/annotation_tool/data_model/media_type.py
+-rw-r--r--   0        0        0     4014 2023-05-04 12:28:40.287202 annotation_tool-0.8.3/annotation_tool/data_model/model.py
+-rw-r--r--   0        0        0     2040 2023-05-04 12:28:40.287202 annotation_tool-0.8.3/annotation_tool/data_model/project.py
+-rw-r--r--   0        0        0     3664 2023-05-04 12:28:40.287202 annotation_tool-0.8.3/annotation_tool/data_model/sample.py
+-rw-r--r--   0        0        0     6412 2023-05-04 12:28:40.287202 annotation_tool-0.8.3/annotation_tool/data_model/single_annotation.py
+-rw-r--r--   0        0        0        0 2023-05-04 12:28:40.287202 annotation_tool-0.8.3/annotation_tool/dialogs/__init__.py
+-rw-r--r--   0        0        0    12197 2023-05-04 12:28:40.287202 annotation_tool-0.8.3/annotation_tool/dialogs/annotation_dialog.py
+-rw-r--r--   0        0        0    10523 2023-05-04 12:28:40.287202 annotation_tool-0.8.3/annotation_tool/dialogs/annotation_list.py
+-rw-r--r--   0        0        0     1956 2023-05-04 12:28:40.287202 annotation_tool-0.8.3/annotation_tool/dialogs/dialog_manager.py
+-rw-r--r--   0        0        0     7082 2023-05-04 12:28:40.287202 annotation_tool-0.8.3/annotation_tool/dialogs/edit_datasets.py
+-rw-r--r--   0        0        0    10994 2023-05-04 12:28:40.287202 annotation_tool-0.8.3/annotation_tool/dialogs/import_annotation_dialog.py
+-rw-r--r--   0        0        0     5706 2023-05-04 12:28:40.287202 annotation_tool-0.8.3/annotation_tool/dialogs/load_annotation_dialog.py
+-rw-r--r--   0        0        0     3670 2023-05-04 12:28:40.287202 annotation_tool-0.8.3/annotation_tool/dialogs/local_files.py
+-rw-r--r--   0        0        0    10576 2023-05-04 12:28:40.287202 annotation_tool-0.8.3/annotation_tool/dialogs/network_list.py
+-rw-r--r--   0        0        0     6899 2023-05-04 12:28:40.287202 annotation_tool-0.8.3/annotation_tool/dialogs/new_annotation_dialog.py
+-rw-r--r--   0        0        0    19491 2023-05-04 12:28:40.287202 annotation_tool-0.8.3/annotation_tool/dialogs/settings_dialog.py
+-rw-r--r--   0        0        0      197 2023-05-04 12:28:40.287202 annotation_tool-0.8.3/annotation_tool/file_cache/__init__.py
+-rw-r--r--   0        0        0     9586 2023-05-04 12:28:40.287202 annotation_tool-0.8.3/annotation_tool/file_cache/_file_cache.py
+-rw-r--r--   0        0        0     8506 2023-05-04 12:28:40.287202 annotation_tool-0.8.3/annotation_tool/gui.py
+-rw-r--r--   0        0        0    12322 2023-05-04 12:28:40.287202 annotation_tool-0.8.3/annotation_tool/main_controller.py
+-rw-r--r--   0        0        0        0 2023-05-04 12:28:40.287202 annotation_tool-0.8.3/annotation_tool/media/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-04 12:28:40.287202 annotation_tool-0.8.3/annotation_tool/media/backend/__init__.py
+-rw-r--r--   0        0        0    10152 2023-05-04 12:28:40.287202 annotation_tool-0.8.3/annotation_tool/media/backend/controller.py
+-rw-r--r--   0        0        0     4220 2023-05-04 12:28:40.287202 annotation_tool-0.8.3/annotation_tool/media/backend/player.py
+-rw-r--r--   0        0        0     5373 2023-05-04 12:28:40.287202 annotation_tool-0.8.3/annotation_tool/media/backend/timer.py
+-rw-r--r--   0        0        0        0 2023-05-04 12:28:40.287202 annotation_tool-0.8.3/annotation_tool/media/backend/type_specific_player/__init__.py
+-rw-r--r--   0        0        0     8424 2023-05-04 12:28:40.287202 annotation_tool-0.8.3/annotation_tool/media/backend/type_specific_player/mocap.py
+-rw-r--r--   0        0        0     7082 2023-05-04 12:28:40.287202 annotation_tool-0.8.3/annotation_tool/media/backend/type_specific_player/video.py
+-rw-r--r--   0        0        0     2286 2023-05-04 12:28:40.287202 annotation_tool-0.8.3/annotation_tool/media/media.py
+-rw-r--r--   0        0        0      357 2023-05-04 12:28:40.287202 annotation_tool-0.8.3/annotation_tool/media_reader/__init__.py
+-rw-r--r--   0        0        0     8866 2023-05-04 12:28:40.287202 annotation_tool-0.8.3/annotation_tool/media_reader/base.py
+-rw-r--r--   0        0        0     2167 2023-05-04 12:28:40.287202 annotation_tool-0.8.3/annotation_tool/media_reader/mocap.py
+-rw-r--r--   0        0        0      121 2023-05-04 12:28:40.287202 annotation_tool-0.8.3/annotation_tool/media_reader/mocap_readers/__init__.py
+-rw-r--r--   0        0        0     3128 2023-05-04 12:28:40.287202 annotation_tool-0.8.3/annotation_tool/media_reader/mocap_readers/base.py
+-rw-r--r--   0        0        0     4745 2023-05-04 12:28:40.287202 annotation_tool-0.8.3/annotation_tool/media_reader/mocap_readers/cache.py
+-rw-r--r--   0        0        0     6020 2023-05-04 12:28:40.287202 annotation_tool-0.8.3/annotation_tool/media_reader/mocap_readers/lara_reader.py
+-rw-r--r--   0        0        0     1787 2023-05-04 12:28:40.287202 annotation_tool-0.8.3/annotation_tool/media_reader/video.py
+-rw-r--r--   0        0        0      157 2023-05-04 12:28:40.287202 annotation_tool-0.8.3/annotation_tool/media_reader/video_readers/__init__.py
+-rw-r--r--   0        0        0     4096 2023-05-04 12:28:40.287202 annotation_tool-0.8.3/annotation_tool/media_reader/video_readers/base.py
+-rw-r--r--   0        0        0     3668 2023-05-04 12:28:40.287202 annotation_tool-0.8.3/annotation_tool/media_reader/video_readers/decord_reader.py
+-rw-r--r--   0        0        0     4321 2023-05-04 12:28:40.287202 annotation_tool-0.8.3/annotation_tool/media_reader/video_readers/evaluation.py
+-rw-r--r--   0        0        0     7496 2023-05-04 12:28:40.287202 annotation_tool-0.8.3/annotation_tool/media_reader/video_readers/opencv_reader.py
+-rw-r--r--   0        0        0     4170 2023-05-04 12:28:40.287202 annotation_tool-0.8.3/annotation_tool/mediator.py
+-rw-r--r--   0        0        0        0 2023-05-04 12:28:40.287202 annotation_tool-0.8.3/annotation_tool/network/LARa/__init__.py
+-rw-r--r--   0        0        0    12119 2023-05-04 12:28:40.287202 annotation_tool-0.8.3/annotation_tool/network/LARa/attr_per_class.txt
+-rw-r--r--   0        0        0     5583 2023-05-04 12:28:40.287202 annotation_tool-0.8.3/annotation_tool/network/LARa/lara_specifics.py
+-rw-r--r--   0        0        0        0 2023-05-04 12:28:40.287202 annotation_tool-0.8.3/annotation_tool/network/__init__.py
+-rw-r--r--   0        0        0     7267 2023-05-04 12:28:40.287202 annotation_tool-0.8.3/annotation_tool/network/controller.py
+-rw-r--r--   0        0        0    27224 2023-05-04 12:28:40.287202 annotation_tool-0.8.3/annotation_tool/network/network.py
+-rw-r--r--   0        0        0     7556 2023-05-04 12:28:40.287202 annotation_tool-0.8.3/annotation_tool/playback.py
+-rw-r--r--   0        0        0     1546 2023-05-04 12:28:40.287202 annotation_tool-0.8.3/annotation_tool/qt_helper_widgets/adaptive_scroll_area.py
+-rw-r--r--   0        0        0     4401 2023-05-04 12:28:40.287202 annotation_tool-0.8.3/annotation_tool/qt_helper_widgets/checkable_combobox.py
+-rw-r--r--   0        0        0     2170 2023-05-04 12:28:40.287202 annotation_tool-0.8.3/annotation_tool/qt_helper_widgets/display_scheme.py
+-rw-r--r--   0        0        0     1798 2023-05-04 12:28:40.287202 annotation_tool-0.8.3/annotation_tool/qt_helper_widgets/histogram.py
+-rw-r--r--   0        0        0      458 2023-05-04 12:28:40.287202 annotation_tool-0.8.3/annotation_tool/qt_helper_widgets/line_edit_adapted.py
+-rw-r--r--   0        0        0      403 2023-05-04 12:28:40.287202 annotation_tool-0.8.3/annotation_tool/qt_helper_widgets/lines.py
+-rw-r--r--   0        0        0     1077 2023-05-04 12:28:40.287202 annotation_tool-0.8.3/annotation_tool/qt_helper_widgets/own_slider.py
+-rw-r--r--   0        0        0     1480 2023-05-04 12:28:40.287202 annotation_tool-0.8.3/annotation_tool/settings.py
+-rw-r--r--   0        0        0     4037 2023-05-04 12:28:40.287202 annotation_tool-0.8.3/annotation_tool/user_actions.py
+-rw-r--r--   0        0        0        0 2023-05-04 12:28:40.287202 annotation_tool-0.8.3/annotation_tool/utility/__init__.py
+-rw-r--r--   0        0        0     4818 2023-05-04 12:28:40.287202 annotation_tool-0.8.3/annotation_tool/utility/decorators.py
+-rw-r--r--   0        0        0    11854 2023-05-04 12:28:40.287202 annotation_tool-0.8.3/annotation_tool/utility/filehandler.py
+-rw-r--r--   0        0        0     4059 2023-05-04 12:28:40.287202 annotation_tool-0.8.3/annotation_tool/utility/functions.py
+-rw-r--r--   0        0        0     2153 2023-05-04 12:28:40.287202 annotation_tool-0.8.3/annotation_tool/utility/networking.py
+-rw-r--r--   0        0        0     4469 2023-05-04 12:28:40.287202 annotation_tool-0.8.3/annotation_tool/utility/priority_queue.py
+-rw-r--r--   0        0        0    53863 2023-05-04 12:28:40.287202 annotation_tool-0.8.3/annotation_tool/utility/resources.py
+-rw-r--r--   0        0        0     1938 2023-05-04 12:28:40.291202 annotation_tool-0.8.3/main.py
+-rw-r--r--   0        0        0     1949 2023-05-04 12:28:40.295202 annotation_tool-0.8.3/pyproject.toml
+-rw-r--r--   0        0        0     2522 1970-01-01 00:00:00.000000 annotation_tool-0.8.3/PKG-INFO
```

### Comparing `annotation_tool-0.8.2/LICENSE` & `annotation_tool-0.8.3/LICENSE`

 * *Files identical despite different names*

### Comparing `annotation_tool-0.8.2/README.md` & `annotation_tool-0.8.3/README.md`

 * *Files identical despite different names*

### Comparing `annotation_tool-0.8.2/annotation_tool/annotation/annotation_base.py` & `annotation_tool-0.8.3/annotation_tool/annotation/annotation_base.py`

 * *Files identical despite different names*

### Comparing `annotation_tool-0.8.2/annotation_tool/annotation/controller.py` & `annotation_tool-0.8.3/annotation_tool/annotation/controller.py`

 * *Files identical despite different names*

### Comparing `annotation_tool-0.8.2/annotation_tool/annotation/manual/controller.py` & `annotation_tool-0.8.3/annotation_tool/annotation/manual/controller.py`

 * *Files identical despite different names*

### Comparing `annotation_tool-0.8.2/annotation_tool/annotation/manual/main_widget.py` & `annotation_tool-0.8.3/annotation_tool/annotation/manual/main_widget.py`

 * *Files identical despite different names*

### Comparing `annotation_tool-0.8.2/annotation_tool/annotation/manual/tool_widget.py` & `annotation_tool-0.8.3/annotation_tool/annotation/manual/tool_widget.py`

 * *Files identical despite different names*

### Comparing `annotation_tool-0.8.2/annotation_tool/annotation/retrieval/controller.py` & `annotation_tool-0.8.3/annotation_tool/annotation/retrieval/controller.py`

 * *Files identical despite different names*

### Comparing `annotation_tool-0.8.2/annotation_tool/annotation/retrieval/main_widget.py` & `annotation_tool-0.8.3/annotation_tool/annotation/retrieval/main_widget.py`

 * *Files identical despite different names*

### Comparing `annotation_tool-0.8.2/annotation_tool/annotation/retrieval/retrieval_backend/element.py` & `annotation_tool-0.8.3/annotation_tool/annotation/retrieval/retrieval_backend/element.py`

 * *Files identical despite different names*

### Comparing `annotation_tool-0.8.2/annotation_tool/annotation/retrieval/retrieval_backend/filter.py` & `annotation_tool-0.8.3/annotation_tool/annotation/retrieval/retrieval_backend/filter.py`

 * *Files identical despite different names*

### Comparing `annotation_tool-0.8.2/annotation_tool/annotation/retrieval/retrieval_backend/filter_dialog.py` & `annotation_tool-0.8.3/annotation_tool/annotation/retrieval/retrieval_backend/filter_dialog.py`

 * *Files identical despite different names*

### Comparing `annotation_tool-0.8.2/annotation_tool/annotation/retrieval/retrieval_backend/loader.py` & `annotation_tool-0.8.3/annotation_tool/annotation/retrieval/retrieval_backend/loader.py`

 * *Files identical despite different names*

### Comparing `annotation_tool-0.8.2/annotation_tool/annotation/retrieval/retrieval_backend/query.py` & `annotation_tool-0.8.3/annotation_tool/annotation/retrieval/retrieval_backend/query.py`

 * *Files identical despite different names*

### Comparing `annotation_tool-0.8.2/annotation_tool/annotation/retrieval/retrieval_backend/queue.py` & `annotation_tool-0.8.3/annotation_tool/annotation/retrieval/retrieval_backend/queue.py`

 * *Files identical despite different names*

### Comparing `annotation_tool-0.8.2/annotation_tool/annotation/retrieval/tool_widget.py` & `annotation_tool-0.8.3/annotation_tool/annotation/retrieval/tool_widget.py`

 * *Files identical despite different names*

### Comparing `annotation_tool-0.8.2/annotation_tool/annotation/timeline.py` & `annotation_tool-0.8.3/annotation_tool/annotation/timeline.py`

 * *Files identical despite different names*

### Comparing `annotation_tool-0.8.2/annotation_tool/data_model/annotation.py` & `annotation_tool-0.8.3/annotation_tool/data_model/annotation.py`

 * *Files identical despite different names*

### Comparing `annotation_tool-0.8.2/annotation_tool/data_model/annotation_scheme.py` & `annotation_tool-0.8.3/annotation_tool/data_model/annotation_scheme.py`

 * *Files identical despite different names*

### Comparing `annotation_tool-0.8.2/annotation_tool/data_model/dataset.py` & `annotation_tool-0.8.3/annotation_tool/data_model/dataset.py`

 * *Files identical despite different names*

### Comparing `annotation_tool-0.8.2/annotation_tool/data_model/media_type.py` & `annotation_tool-0.8.3/annotation_tool/data_model/media_type.py`

 * *Files identical despite different names*

### Comparing `annotation_tool-0.8.2/annotation_tool/data_model/model.py` & `annotation_tool-0.8.3/annotation_tool/data_model/model.py`

 * *Files identical despite different names*

### Comparing `annotation_tool-0.8.2/annotation_tool/data_model/project.py` & `annotation_tool-0.8.3/annotation_tool/data_model/project.py`

 * *Files identical despite different names*

### Comparing `annotation_tool-0.8.2/annotation_tool/data_model/sample.py` & `annotation_tool-0.8.3/annotation_tool/data_model/sample.py`

 * *Files identical despite different names*

### Comparing `annotation_tool-0.8.2/annotation_tool/data_model/single_annotation.py` & `annotation_tool-0.8.3/annotation_tool/data_model/single_annotation.py`

 * *Files identical despite different names*

### Comparing `annotation_tool-0.8.2/annotation_tool/dialogs/annotation_dialog.py` & `annotation_tool-0.8.3/annotation_tool/dialogs/annotation_dialog.py`

 * *Files identical despite different names*

### Comparing `annotation_tool-0.8.2/annotation_tool/dialogs/annotation_list.py` & `annotation_tool-0.8.3/annotation_tool/dialogs/annotation_list.py`

 * *Files identical despite different names*

### Comparing `annotation_tool-0.8.2/annotation_tool/dialogs/dialog_manager.py` & `annotation_tool-0.8.3/annotation_tool/dialogs/dialog_manager.py`

 * *Files identical despite different names*

### Comparing `annotation_tool-0.8.2/annotation_tool/dialogs/edit_datasets.py` & `annotation_tool-0.8.3/annotation_tool/dialogs/edit_datasets.py`

 * *Files identical despite different names*

### Comparing `annotation_tool-0.8.2/annotation_tool/dialogs/import_annotation_dialog.py` & `annotation_tool-0.8.3/annotation_tool/dialogs/import_annotation_dialog.py`

 * *Files identical despite different names*

### Comparing `annotation_tool-0.8.2/annotation_tool/dialogs/load_annotation_dialog.py` & `annotation_tool-0.8.3/annotation_tool/dialogs/load_annotation_dialog.py`

 * *Files identical despite different names*

### Comparing `annotation_tool-0.8.2/annotation_tool/dialogs/local_files.py` & `annotation_tool-0.8.3/annotation_tool/dialogs/local_files.py`

 * *Files identical despite different names*

### Comparing `annotation_tool-0.8.2/annotation_tool/dialogs/network_list.py` & `annotation_tool-0.8.3/annotation_tool/dialogs/network_list.py`

 * *Files identical despite different names*

### Comparing `annotation_tool-0.8.2/annotation_tool/dialogs/new_annotation_dialog.py` & `annotation_tool-0.8.3/annotation_tool/dialogs/new_annotation_dialog.py`

 * *Files identical despite different names*

### Comparing `annotation_tool-0.8.2/annotation_tool/dialogs/settings_dialog.py` & `annotation_tool-0.8.3/annotation_tool/dialogs/settings_dialog.py`

 * *Files identical despite different names*

### Comparing `annotation_tool-0.8.2/annotation_tool/file_cache/_file_cache.py` & `annotation_tool-0.8.3/annotation_tool/file_cache/_file_cache.py`

 * *Files identical despite different names*

### Comparing `annotation_tool-0.8.2/annotation_tool/gui.py` & `annotation_tool-0.8.3/annotation_tool/gui.py`

 * *Files identical despite different names*

### Comparing `annotation_tool-0.8.2/annotation_tool/main_controller.py` & `annotation_tool-0.8.3/annotation_tool/main_controller.py`

 * *Files identical despite different names*

### Comparing `annotation_tool-0.8.2/annotation_tool/media/backend/controller.py` & `annotation_tool-0.8.3/annotation_tool/media/backend/controller.py`

 * *Files identical despite different names*

### Comparing `annotation_tool-0.8.2/annotation_tool/media/backend/player.py` & `annotation_tool-0.8.3/annotation_tool/media/backend/player.py`

 * *Files identical despite different names*

### Comparing `annotation_tool-0.8.2/annotation_tool/media/backend/timer.py` & `annotation_tool-0.8.3/annotation_tool/media/backend/timer.py`

 * *Files 1% similar despite different names*

```diff
@@ -128,15 +128,15 @@
     @qtc.pyqtSlot(float)
     def set_replay_speed(self, x):
         self._replay_speed = max(0.01, x)
         self.sync_time()
 
     @qtc.pyqtSlot(int)
     def set_position(self, x):
-        self.sync_time()
+        self.sync_time(x)
         self.update_positions(from_timeout=False, new_pos=x)
 
     @qtc.pyqtSlot()
     def stop(self):
         self._active = False
         self._timer.stop()
         self._timer.deleteLater()
@@ -167,10 +167,10 @@
         self.update_positions()
 
     @qtc.pyqtSlot(qtc.QObject)
     def unsubscribe(self, subscriber):
         self._subscribers = [x for x in self._subscribers if x != subscriber]
         self.position_changed.disconnect(subscriber.set_position_)
 
-    def sync_time(self):
-        self._start_pos = self.frame_position
+    def sync_time(self, new_pos: int = None):
+        self._start_pos = new_pos if new_pos else self.frame_position
         self._start_time = time_in_millis() if not self._paused else None
```

### Comparing `annotation_tool-0.8.2/annotation_tool/media/backend/type_specific_player/mocap.py` & `annotation_tool-0.8.3/annotation_tool/media/backend/type_specific_player/mocap.py`

 * *Files identical despite different names*

### Comparing `annotation_tool-0.8.2/annotation_tool/media/backend/type_specific_player/video.py` & `annotation_tool-0.8.3/annotation_tool/media/backend/type_specific_player/video.py`

 * *Files identical despite different names*

### Comparing `annotation_tool-0.8.2/annotation_tool/media/media.py` & `annotation_tool-0.8.3/annotation_tool/media/media.py`

 * *Files identical despite different names*

### Comparing `annotation_tool-0.8.2/annotation_tool/media_reader/base.py` & `annotation_tool-0.8.3/annotation_tool/media_reader/base.py`

 * *Files identical despite different names*

### Comparing `annotation_tool-0.8.2/annotation_tool/media_reader/mocap.py` & `annotation_tool-0.8.3/annotation_tool/media_reader/mocap.py`

 * *Files identical despite different names*

### Comparing `annotation_tool-0.8.2/annotation_tool/media_reader/mocap_readers/base.py` & `annotation_tool-0.8.3/annotation_tool/media_reader/mocap_readers/base.py`

 * *Files identical despite different names*

### Comparing `annotation_tool-0.8.2/annotation_tool/media_reader/mocap_readers/cache.py` & `annotation_tool-0.8.3/annotation_tool/media_reader/mocap_readers/cache.py`

 * *Files identical despite different names*

### Comparing `annotation_tool-0.8.2/annotation_tool/media_reader/mocap_readers/lara_reader.py` & `annotation_tool-0.8.3/annotation_tool/media_reader/mocap_readers/lara_reader.py`

 * *Files identical despite different names*

### Comparing `annotation_tool-0.8.2/annotation_tool/media_reader/video.py` & `annotation_tool-0.8.3/annotation_tool/media_reader/video.py`

 * *Files identical despite different names*

### Comparing `annotation_tool-0.8.2/annotation_tool/media_reader/video_readers/base.py` & `annotation_tool-0.8.3/annotation_tool/media_reader/video_readers/base.py`

 * *Files identical despite different names*

### Comparing `annotation_tool-0.8.2/annotation_tool/media_reader/video_readers/decord_reader.py` & `annotation_tool-0.8.3/annotation_tool/media_reader/video_readers/decord_reader.py`

 * *Files identical despite different names*

### Comparing `annotation_tool-0.8.2/annotation_tool/media_reader/video_readers/evaluation.py` & `annotation_tool-0.8.3/annotation_tool/media_reader/video_readers/evaluation.py`

 * *Files identical despite different names*

### Comparing `annotation_tool-0.8.2/annotation_tool/media_reader/video_readers/opencv_reader.py` & `annotation_tool-0.8.3/annotation_tool/media_reader/video_readers/opencv_reader.py`

 * *Files identical despite different names*

### Comparing `annotation_tool-0.8.2/annotation_tool/mediator.py` & `annotation_tool-0.8.3/annotation_tool/mediator.py`

 * *Files identical despite different names*

### Comparing `annotation_tool-0.8.2/annotation_tool/network/LARa/attr_per_class.txt` & `annotation_tool-0.8.3/annotation_tool/network/LARa/attr_per_class.txt`

 * *Files identical despite different names*

### Comparing `annotation_tool-0.8.2/annotation_tool/network/LARa/lara_specifics.py` & `annotation_tool-0.8.3/annotation_tool/network/LARa/lara_specifics.py`

 * *Files identical despite different names*

### Comparing `annotation_tool-0.8.2/annotation_tool/network/controller.py` & `annotation_tool-0.8.3/annotation_tool/network/controller.py`

 * *Files identical despite different names*

### Comparing `annotation_tool-0.8.2/annotation_tool/network/network.py` & `annotation_tool-0.8.3/annotation_tool/network/network.py`

 * *Files identical despite different names*

### Comparing `annotation_tool-0.8.2/annotation_tool/playback.py` & `annotation_tool-0.8.3/annotation_tool/playback.py`

 * *Files identical despite different names*

### Comparing `annotation_tool-0.8.2/annotation_tool/qt_helper_widgets/adaptive_scroll_area.py` & `annotation_tool-0.8.3/annotation_tool/qt_helper_widgets/adaptive_scroll_area.py`

 * *Files identical despite different names*

### Comparing `annotation_tool-0.8.2/annotation_tool/qt_helper_widgets/checkable_combobox.py` & `annotation_tool-0.8.3/annotation_tool/qt_helper_widgets/checkable_combobox.py`

 * *Files identical despite different names*

### Comparing `annotation_tool-0.8.2/annotation_tool/qt_helper_widgets/display_scheme.py` & `annotation_tool-0.8.3/annotation_tool/qt_helper_widgets/display_scheme.py`

 * *Files identical despite different names*

### Comparing `annotation_tool-0.8.2/annotation_tool/qt_helper_widgets/histogram.py` & `annotation_tool-0.8.3/annotation_tool/qt_helper_widgets/histogram.py`

 * *Files identical despite different names*

### Comparing `annotation_tool-0.8.2/annotation_tool/qt_helper_widgets/own_slider.py` & `annotation_tool-0.8.3/annotation_tool/qt_helper_widgets/own_slider.py`

 * *Files identical despite different names*

### Comparing `annotation_tool-0.8.2/annotation_tool/settings.py` & `annotation_tool-0.8.3/annotation_tool/settings.py`

 * *Files identical despite different names*

### Comparing `annotation_tool-0.8.2/annotation_tool/user_actions.py` & `annotation_tool-0.8.3/annotation_tool/user_actions.py`

 * *Files identical despite different names*

### Comparing `annotation_tool-0.8.2/annotation_tool/utility/decorators.py` & `annotation_tool-0.8.3/annotation_tool/utility/decorators.py`

 * *Files identical despite different names*

### Comparing `annotation_tool-0.8.2/annotation_tool/utility/filehandler.py` & `annotation_tool-0.8.3/annotation_tool/utility/filehandler.py`

 * *Files identical despite different names*

### Comparing `annotation_tool-0.8.2/annotation_tool/utility/functions.py` & `annotation_tool-0.8.3/annotation_tool/utility/functions.py`

 * *Files identical despite different names*

### Comparing `annotation_tool-0.8.2/annotation_tool/utility/networking.py` & `annotation_tool-0.8.3/annotation_tool/utility/networking.py`

 * *Files identical despite different names*

### Comparing `annotation_tool-0.8.2/annotation_tool/utility/priority_queue.py` & `annotation_tool-0.8.3/annotation_tool/utility/priority_queue.py`

 * *Files identical despite different names*

### Comparing `annotation_tool-0.8.2/annotation_tool/utility/resources.py` & `annotation_tool-0.8.3/annotation_tool/utility/resources.py`

 * *Files identical despite different names*

### Comparing `annotation_tool-0.8.2/main.py` & `annotation_tool-0.8.3/main.py`

 * *Files identical despite different names*

### Comparing `annotation_tool-0.8.2/pyproject.toml` & `annotation_tool-0.8.3/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "annotation-tool"
-version = "0.8.2"
+version = "0.8.3"
 description = "Tool for annotating time series data from sources such as IMUs, MoCap, Videos and more."
 readme = "README.md"
 license = "MIT"
 homepage = "https://github.com/TUD-Patrec/annotation-tool"
 authors = [
     "Fernando Moya Rueda <fernando.moya@cs.tu-dortmund.de>",
     "Erik Altermann <erik.altermann@tu-dortmund.de>",
@@ -64,15 +64,15 @@
 [tool.isort]
 profile = "black"
 force_sort_within_sections = true
 line_length = 88
 
 [tool.commitizen]
 name = "cz_conventional_commits"
-version = "0.8.2"
+version = "0.8.3"
 tag_format = "v$version"
 major_version_zero = true
 version_files = [
     "annotation_tool/__init__.py:^__version__",
     "pyproject.toml:^version"
 ]
 update_changelog_on_bump = false
```

### Comparing `annotation_tool-0.8.2/PKG-INFO` & `annotation_tool-0.8.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: annotation-tool
-Version: 0.8.2
+Version: 0.8.3
 Summary: Tool for annotating time series data from sources such as IMUs, MoCap, Videos and more.
 Home-page: https://github.com/TUD-Patrec/annotation-tool
 License: MIT
 Author: Fernando Moya Rueda
 Author-email: fernando.moya@cs.tu-dortmund.de
 Requires-Python: >=3.8,<3.11
 Classifier: License :: OSI Approved :: MIT License
```

