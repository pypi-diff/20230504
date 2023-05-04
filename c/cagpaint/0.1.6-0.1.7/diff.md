# Comparing `tmp/cagpaint-0.1.6.tar.gz` & `tmp/cagpaint-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cagpaint-0.1.6.tar", last modified: Thu May  4 15:19:22 2023, max compression
+gzip compressed data, was "cagpaint-0.1.7.tar", last modified: Thu May  4 15:23:04 2023, max compression
```

## Comparing `cagpaint-0.1.6.tar` & `cagpaint-0.1.7.tar`

### file list

```diff
@@ -1,58 +1,58 @@
-drwxrwxr-x   0 alatar    (1000) alatar    (1000)        0 2023-05-04 15:19:22.649759 cagpaint-0.1.6/
--rw-rw-r--   0 alatar    (1000) alatar    (1000)    35149 2022-09-20 07:40:57.000000 cagpaint-0.1.6/LICENSE
--rw-rw-r--   0 alatar    (1000) alatar    (1000)      215 2023-05-04 15:19:22.649759 cagpaint-0.1.6/PKG-INFO
--rw-rw-r--   0 alatar    (1000) alatar    (1000)      242 2022-09-20 12:22:50.000000 cagpaint-0.1.6/README.md
-drwxrwxr-x   0 alatar    (1000) alatar    (1000)        0 2023-05-04 15:19:22.645759 cagpaint-0.1.6/cagpaint/
--rw-rw-r--   0 alatar    (1000) alatar    (1000)        0 2023-05-04 14:53:02.000000 cagpaint-0.1.6/cagpaint/__init__.py
-drwxrwxr-x   0 alatar    (1000) alatar    (1000)        0 2023-05-04 15:19:22.645759 cagpaint-0.1.6/cagpaint/painter/
--rw-rw-r--   0 alatar    (1000) alatar    (1000)        0 2023-05-04 13:56:49.000000 cagpaint-0.1.6/cagpaint/painter/__init__.py
--rw-rw-r--   0 alatar    (1000) alatar    (1000)     3932 2022-09-20 07:40:58.000000 cagpaint-0.1.6/cagpaint/painter/install_fixes.py
-drwxrwxr-x   0 alatar    (1000) alatar    (1000)        0 2023-05-04 15:19:22.645759 cagpaint-0.1.6/cagpaint/painter/src/
--rw-rw-r--   0 alatar    (1000) alatar    (1000)        0 2023-05-04 13:56:53.000000 cagpaint-0.1.6/cagpaint/painter/src/__init__.py
--rw-rw-r--   0 alatar    (1000) alatar    (1000)    43783 2022-09-20 07:40:58.000000 cagpaint-0.1.6/cagpaint/painter/src/about.py
--rw-rw-r--   0 alatar    (1000) alatar    (1000)     6548 2022-09-20 07:40:58.000000 cagpaint-0.1.6/cagpaint/painter/src/contrast_slider.py
--rw-rw-r--   0 alatar    (1000) alatar    (1000)    12206 2022-11-29 09:34:29.000000 cagpaint-0.1.6/cagpaint/painter/src/create_project.py
--rw-rw-r--   0 alatar    (1000) alatar    (1000)     6631 2022-09-20 07:43:51.000000 cagpaint-0.1.6/cagpaint/painter/src/file_utils.py
--rw-rw-r--   0 alatar    (1000) alatar    (1000)    15984 2022-09-20 07:40:58.000000 cagpaint-0.1.6/cagpaint/painter/src/graphics_scene.py
--rw-rw-r--   0 alatar    (1000) alatar    (1000)     2853 2022-09-20 07:40:58.000000 cagpaint-0.1.6/cagpaint/painter/src/graphics_view.py
--rw-rw-r--   0 alatar    (1000) alatar    (1000)    12990 2023-05-03 08:00:12.000000 cagpaint-0.1.6/cagpaint/painter/src/im_utils.py
--rw-rw-r--   0 alatar    (1000) alatar    (1000)    23982 2022-09-20 07:40:58.000000 cagpaint-0.1.6/cagpaint/painter/src/im_viewer.py
--rw-rw-r--   0 alatar    (1000) alatar    (1000)     3161 2022-11-29 09:34:29.000000 cagpaint-0.1.6/cagpaint/painter/src/instructions.py
--rw-rw-r--   0 alatar    (1000) alatar    (1000)     2347 2022-09-20 07:40:58.000000 cagpaint-0.1.6/cagpaint/painter/src/lock.py
--rw-rw-r--   0 alatar    (1000) alatar    (1000)     3412 2022-11-29 09:34:29.000000 cagpaint-0.1.6/cagpaint/painter/src/main.py
--rw-rw-r--   0 alatar    (1000) alatar    (1000)    13121 2022-09-20 07:40:58.000000 cagpaint-0.1.6/cagpaint/painter/src/menus.py
--rw-rw-r--   0 alatar    (1000) alatar    (1000)     1649 2022-09-20 07:40:58.000000 cagpaint-0.1.6/cagpaint/painter/src/name_edit_widget.py
--rw-rw-r--   0 alatar    (1000) alatar    (1000)     5400 2022-11-29 09:34:29.000000 cagpaint-0.1.6/cagpaint/painter/src/nav.py
--rw-rw-r--   0 alatar    (1000) alatar    (1000)     3620 2022-09-20 07:40:58.000000 cagpaint-0.1.6/cagpaint/painter/src/palette.py
--rw-rw-r--   0 alatar    (1000) alatar    (1000)     8541 2022-09-20 07:40:58.000000 cagpaint-0.1.6/cagpaint/painter/src/patch_seg.py
--rw-rw-r--   0 alatar    (1000) alatar    (1000)     1808 2022-09-20 07:40:58.000000 cagpaint-0.1.6/cagpaint/painter/src/progress_widget.py
--rw-rw-r--   0 alatar    (1000) alatar    (1000)    36880 2022-11-29 09:34:29.000000 cagpaint-0.1.6/cagpaint/painter/src/root_painter.py
--rw-rw-r--   0 alatar    (1000) alatar    (1000)     1304 2022-11-29 09:34:29.000000 cagpaint-0.1.6/cagpaint/painter/src/segment.py
--rw-rw-r--   0 alatar    (1000) alatar    (1000)     8409 2022-11-17 19:02:25.000000 cagpaint-0.1.6/cagpaint/painter/src/segment_folder.py
--rw-rw-r--   0 alatar    (1000) alatar    (1000)     4572 2022-09-20 07:40:58.000000 cagpaint-0.1.6/cagpaint/painter/src/slice_nav.py
--rw-rw-r--   0 alatar    (1000) alatar    (1000)     3039 2022-09-20 07:40:58.000000 cagpaint-0.1.6/cagpaint/painter/src/tcp_utils.py
--rw-rw-r--   0 alatar    (1000) alatar    (1000)       85 2022-09-20 07:40:58.000000 cagpaint-0.1.6/cagpaint/painter/src/view_state.py
--rw-rw-r--   0 alatar    (1000) alatar    (1000)     3080 2022-09-20 07:40:58.000000 cagpaint-0.1.6/cagpaint/painter/src/visibility_widget.py
-drwxrwxr-x   0 alatar    (1000) alatar    (1000)        0 2023-05-04 15:19:22.649759 cagpaint-0.1.6/cagpaint/trainer/
--rw-rw-r--   0 alatar    (1000) alatar    (1000)      703 2023-05-04 15:18:39.000000 cagpaint-0.1.6/cagpaint/trainer/__init__.py
--rw-rw-r--   0 alatar    (1000) alatar    (1000)     1204 2022-09-20 07:40:58.000000 cagpaint-0.1.6/cagpaint/trainer/data_utils.py
--rw-rw-r--   0 alatar    (1000) alatar    (1000)    19205 2023-05-03 14:16:20.000000 cagpaint-0.1.6/cagpaint/trainer/datasets.py
--rw-rw-r--   0 alatar    (1000) alatar    (1000)     2650 2022-11-26 14:08:31.000000 cagpaint-0.1.6/cagpaint/trainer/file_utils.py
--rw-rw-r--   0 alatar    (1000) alatar    (1000)    21190 2023-05-03 08:05:58.000000 cagpaint-0.1.6/cagpaint/trainer/im_utils.py
--rw-rw-r--   0 alatar    (1000) alatar    (1000)     1789 2022-11-29 09:34:29.000000 cagpaint-0.1.6/cagpaint/trainer/instructions.py
--rw-rw-r--   0 alatar    (1000) alatar    (1000)     7388 2022-11-29 09:34:29.000000 cagpaint-0.1.6/cagpaint/trainer/loss.py
--rw-rw-r--   0 alatar    (1000) alatar    (1000)     2196 2023-05-04 15:03:08.000000 cagpaint-0.1.6/cagpaint/trainer/main.py
--rw-rw-r--   0 alatar    (1000) alatar    (1000)     2922 2022-09-20 07:40:58.000000 cagpaint-0.1.6/cagpaint/trainer/metrics.py
--rw-rw-r--   0 alatar    (1000) alatar    (1000)    15203 2023-05-03 08:07:17.000000 cagpaint-0.1.6/cagpaint/trainer/model_utils.py
--rw-rw-r--   0 alatar    (1000) alatar    (1000)     7463 2022-11-29 09:34:29.000000 cagpaint-0.1.6/cagpaint/trainer/patch_seg.py
--rw-rw-r--   0 alatar    (1000) alatar    (1000)     1373 2022-09-20 07:40:58.000000 cagpaint-0.1.6/cagpaint/trainer/scp_utils.py
--rw-rw-r--   0 alatar    (1000) alatar    (1000)     2587 2022-11-17 08:42:24.000000 cagpaint-0.1.6/cagpaint/trainer/startup.py
--rw-rw-r--   0 alatar    (1000) alatar    (1000)    29553 2022-11-29 09:34:29.000000 cagpaint-0.1.6/cagpaint/trainer/trainer.py
--rw-rw-r--   0 alatar    (1000) alatar    (1000)     7698 2022-09-20 07:47:16.000000 cagpaint-0.1.6/cagpaint/trainer/unet3d.py
-drwxrwxr-x   0 alatar    (1000) alatar    (1000)        0 2023-05-04 15:19:22.645759 cagpaint-0.1.6/cagpaint.egg-info/
--rw-rw-r--   0 alatar    (1000) alatar    (1000)      215 2023-05-04 15:19:22.000000 cagpaint-0.1.6/cagpaint.egg-info/PKG-INFO
--rw-rw-r--   0 alatar    (1000) alatar    (1000)     1547 2023-05-04 15:19:22.000000 cagpaint-0.1.6/cagpaint.egg-info/SOURCES.txt
--rw-rw-r--   0 alatar    (1000) alatar    (1000)        1 2023-05-04 15:19:22.000000 cagpaint-0.1.6/cagpaint.egg-info/dependency_links.txt
--rw-rw-r--   0 alatar    (1000) alatar    (1000)        9 2023-05-04 15:19:22.000000 cagpaint-0.1.6/cagpaint.egg-info/top_level.txt
--rw-rw-r--   0 alatar    (1000) alatar    (1000)       38 2023-05-04 15:19:22.649759 cagpaint-0.1.6/setup.cfg
--rw-rw-r--   0 alatar    (1000) alatar    (1000)      397 2023-05-04 15:19:12.000000 cagpaint-0.1.6/setup.py
+drwxrwxr-x   0 alatar    (1000) alatar    (1000)        0 2023-05-04 15:23:04.846233 cagpaint-0.1.7/
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)    35149 2022-09-20 07:40:57.000000 cagpaint-0.1.7/LICENSE
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)      215 2023-05-04 15:23:04.846233 cagpaint-0.1.7/PKG-INFO
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)      242 2022-09-20 12:22:50.000000 cagpaint-0.1.7/README.md
+drwxrwxr-x   0 alatar    (1000) alatar    (1000)        0 2023-05-04 15:23:04.838233 cagpaint-0.1.7/cagpaint/
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)        0 2023-05-04 14:53:02.000000 cagpaint-0.1.7/cagpaint/__init__.py
+drwxrwxr-x   0 alatar    (1000) alatar    (1000)        0 2023-05-04 15:23:04.838233 cagpaint-0.1.7/cagpaint/painter/
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)        0 2023-05-04 13:56:49.000000 cagpaint-0.1.7/cagpaint/painter/__init__.py
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)     3932 2022-09-20 07:40:58.000000 cagpaint-0.1.7/cagpaint/painter/install_fixes.py
+drwxrwxr-x   0 alatar    (1000) alatar    (1000)        0 2023-05-04 15:23:04.842233 cagpaint-0.1.7/cagpaint/painter/src/
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)        0 2023-05-04 13:56:53.000000 cagpaint-0.1.7/cagpaint/painter/src/__init__.py
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)    43783 2022-09-20 07:40:58.000000 cagpaint-0.1.7/cagpaint/painter/src/about.py
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)     6548 2022-09-20 07:40:58.000000 cagpaint-0.1.7/cagpaint/painter/src/contrast_slider.py
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)    12206 2022-11-29 09:34:29.000000 cagpaint-0.1.7/cagpaint/painter/src/create_project.py
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)     6631 2022-09-20 07:43:51.000000 cagpaint-0.1.7/cagpaint/painter/src/file_utils.py
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)    15984 2022-09-20 07:40:58.000000 cagpaint-0.1.7/cagpaint/painter/src/graphics_scene.py
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)     2853 2022-09-20 07:40:58.000000 cagpaint-0.1.7/cagpaint/painter/src/graphics_view.py
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)    12990 2023-05-03 08:00:12.000000 cagpaint-0.1.7/cagpaint/painter/src/im_utils.py
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)    23982 2022-09-20 07:40:58.000000 cagpaint-0.1.7/cagpaint/painter/src/im_viewer.py
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)     3161 2022-11-29 09:34:29.000000 cagpaint-0.1.7/cagpaint/painter/src/instructions.py
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)     2347 2022-09-20 07:40:58.000000 cagpaint-0.1.7/cagpaint/painter/src/lock.py
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)     3412 2022-11-29 09:34:29.000000 cagpaint-0.1.7/cagpaint/painter/src/main.py
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)    13121 2022-09-20 07:40:58.000000 cagpaint-0.1.7/cagpaint/painter/src/menus.py
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)     1649 2022-09-20 07:40:58.000000 cagpaint-0.1.7/cagpaint/painter/src/name_edit_widget.py
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)     5400 2022-11-29 09:34:29.000000 cagpaint-0.1.7/cagpaint/painter/src/nav.py
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)     3620 2022-09-20 07:40:58.000000 cagpaint-0.1.7/cagpaint/painter/src/palette.py
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)     8541 2022-09-20 07:40:58.000000 cagpaint-0.1.7/cagpaint/painter/src/patch_seg.py
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)     1808 2022-09-20 07:40:58.000000 cagpaint-0.1.7/cagpaint/painter/src/progress_widget.py
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)    36880 2022-11-29 09:34:29.000000 cagpaint-0.1.7/cagpaint/painter/src/root_painter.py
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)     1304 2022-11-29 09:34:29.000000 cagpaint-0.1.7/cagpaint/painter/src/segment.py
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)     8409 2022-11-17 19:02:25.000000 cagpaint-0.1.7/cagpaint/painter/src/segment_folder.py
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)     4572 2022-09-20 07:40:58.000000 cagpaint-0.1.7/cagpaint/painter/src/slice_nav.py
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)     3039 2022-09-20 07:40:58.000000 cagpaint-0.1.7/cagpaint/painter/src/tcp_utils.py
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)       85 2022-09-20 07:40:58.000000 cagpaint-0.1.7/cagpaint/painter/src/view_state.py
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)     3080 2022-09-20 07:40:58.000000 cagpaint-0.1.7/cagpaint/painter/src/visibility_widget.py
+drwxrwxr-x   0 alatar    (1000) alatar    (1000)        0 2023-05-04 15:23:04.842233 cagpaint-0.1.7/cagpaint/trainer/
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)      972 2023-05-04 15:22:42.000000 cagpaint-0.1.7/cagpaint/trainer/__init__.py
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)     1204 2022-09-20 07:40:58.000000 cagpaint-0.1.7/cagpaint/trainer/data_utils.py
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)    19205 2023-05-03 14:16:20.000000 cagpaint-0.1.7/cagpaint/trainer/datasets.py
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)     2650 2022-11-26 14:08:31.000000 cagpaint-0.1.7/cagpaint/trainer/file_utils.py
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)    21190 2023-05-03 08:05:58.000000 cagpaint-0.1.7/cagpaint/trainer/im_utils.py
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)     1789 2022-11-29 09:34:29.000000 cagpaint-0.1.7/cagpaint/trainer/instructions.py
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)     7388 2022-11-29 09:34:29.000000 cagpaint-0.1.7/cagpaint/trainer/loss.py
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)     2196 2023-05-04 15:03:08.000000 cagpaint-0.1.7/cagpaint/trainer/main.py
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)     2922 2022-09-20 07:40:58.000000 cagpaint-0.1.7/cagpaint/trainer/metrics.py
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)    15203 2023-05-03 08:07:17.000000 cagpaint-0.1.7/cagpaint/trainer/model_utils.py
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)     7463 2022-11-29 09:34:29.000000 cagpaint-0.1.7/cagpaint/trainer/patch_seg.py
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)     1373 2022-09-20 07:40:58.000000 cagpaint-0.1.7/cagpaint/trainer/scp_utils.py
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)     2587 2022-11-17 08:42:24.000000 cagpaint-0.1.7/cagpaint/trainer/startup.py
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)    29553 2022-11-29 09:34:29.000000 cagpaint-0.1.7/cagpaint/trainer/trainer.py
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)     7698 2022-09-20 07:47:16.000000 cagpaint-0.1.7/cagpaint/trainer/unet3d.py
+drwxrwxr-x   0 alatar    (1000) alatar    (1000)        0 2023-05-04 15:23:04.838233 cagpaint-0.1.7/cagpaint.egg-info/
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)      215 2023-05-04 15:23:04.000000 cagpaint-0.1.7/cagpaint.egg-info/PKG-INFO
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)     1547 2023-05-04 15:23:04.000000 cagpaint-0.1.7/cagpaint.egg-info/SOURCES.txt
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)        1 2023-05-04 15:23:04.000000 cagpaint-0.1.7/cagpaint.egg-info/dependency_links.txt
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)        9 2023-05-04 15:23:04.000000 cagpaint-0.1.7/cagpaint.egg-info/top_level.txt
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)       38 2023-05-04 15:23:04.846233 cagpaint-0.1.7/setup.cfg
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)      397 2023-05-04 15:23:02.000000 cagpaint-0.1.7/setup.py
```

### Comparing `cagpaint-0.1.6/LICENSE` & `cagpaint-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `cagpaint-0.1.6/cagpaint/painter/install_fixes.py` & `cagpaint-0.1.7/cagpaint/painter/install_fixes.py`

 * *Files identical despite different names*

### Comparing `cagpaint-0.1.6/cagpaint/painter/src/about.py` & `cagpaint-0.1.7/cagpaint/painter/src/about.py`

 * *Files identical despite different names*

### Comparing `cagpaint-0.1.6/cagpaint/painter/src/contrast_slider.py` & `cagpaint-0.1.7/cagpaint/painter/src/contrast_slider.py`

 * *Files identical despite different names*

### Comparing `cagpaint-0.1.6/cagpaint/painter/src/create_project.py` & `cagpaint-0.1.7/cagpaint/painter/src/create_project.py`

 * *Files identical despite different names*

### Comparing `cagpaint-0.1.6/cagpaint/painter/src/file_utils.py` & `cagpaint-0.1.7/cagpaint/painter/src/file_utils.py`

 * *Files identical despite different names*

### Comparing `cagpaint-0.1.6/cagpaint/painter/src/graphics_scene.py` & `cagpaint-0.1.7/cagpaint/painter/src/graphics_scene.py`

 * *Files identical despite different names*

### Comparing `cagpaint-0.1.6/cagpaint/painter/src/graphics_view.py` & `cagpaint-0.1.7/cagpaint/painter/src/graphics_view.py`

 * *Files identical despite different names*

### Comparing `cagpaint-0.1.6/cagpaint/painter/src/im_utils.py` & `cagpaint-0.1.7/cagpaint/painter/src/im_utils.py`

 * *Files identical despite different names*

### Comparing `cagpaint-0.1.6/cagpaint/painter/src/im_viewer.py` & `cagpaint-0.1.7/cagpaint/painter/src/im_viewer.py`

 * *Files identical despite different names*

### Comparing `cagpaint-0.1.6/cagpaint/painter/src/instructions.py` & `cagpaint-0.1.7/cagpaint/painter/src/instructions.py`

 * *Files identical despite different names*

### Comparing `cagpaint-0.1.6/cagpaint/painter/src/lock.py` & `cagpaint-0.1.7/cagpaint/painter/src/lock.py`

 * *Files identical despite different names*

### Comparing `cagpaint-0.1.6/cagpaint/painter/src/main.py` & `cagpaint-0.1.7/cagpaint/painter/src/main.py`

 * *Files identical despite different names*

### Comparing `cagpaint-0.1.6/cagpaint/painter/src/menus.py` & `cagpaint-0.1.7/cagpaint/painter/src/menus.py`

 * *Files identical despite different names*

### Comparing `cagpaint-0.1.6/cagpaint/painter/src/name_edit_widget.py` & `cagpaint-0.1.7/cagpaint/painter/src/name_edit_widget.py`

 * *Files identical despite different names*

### Comparing `cagpaint-0.1.6/cagpaint/painter/src/nav.py` & `cagpaint-0.1.7/cagpaint/painter/src/nav.py`

 * *Files identical despite different names*

### Comparing `cagpaint-0.1.6/cagpaint/painter/src/palette.py` & `cagpaint-0.1.7/cagpaint/painter/src/palette.py`

 * *Files identical despite different names*

### Comparing `cagpaint-0.1.6/cagpaint/painter/src/patch_seg.py` & `cagpaint-0.1.7/cagpaint/painter/src/patch_seg.py`

 * *Files identical despite different names*

### Comparing `cagpaint-0.1.6/cagpaint/painter/src/progress_widget.py` & `cagpaint-0.1.7/cagpaint/painter/src/progress_widget.py`

 * *Files identical despite different names*

### Comparing `cagpaint-0.1.6/cagpaint/painter/src/root_painter.py` & `cagpaint-0.1.7/cagpaint/painter/src/root_painter.py`

 * *Files identical despite different names*

### Comparing `cagpaint-0.1.6/cagpaint/painter/src/segment.py` & `cagpaint-0.1.7/cagpaint/painter/src/segment.py`

 * *Files identical despite different names*

### Comparing `cagpaint-0.1.6/cagpaint/painter/src/segment_folder.py` & `cagpaint-0.1.7/cagpaint/painter/src/segment_folder.py`

 * *Files identical despite different names*

### Comparing `cagpaint-0.1.6/cagpaint/painter/src/slice_nav.py` & `cagpaint-0.1.7/cagpaint/painter/src/slice_nav.py`

 * *Files identical despite different names*

### Comparing `cagpaint-0.1.6/cagpaint/painter/src/tcp_utils.py` & `cagpaint-0.1.7/cagpaint/painter/src/tcp_utils.py`

 * *Files identical despite different names*

### Comparing `cagpaint-0.1.6/cagpaint/painter/src/visibility_widget.py` & `cagpaint-0.1.7/cagpaint/painter/src/visibility_widget.py`

 * *Files identical despite different names*

### Comparing `cagpaint-0.1.6/cagpaint/trainer/data_utils.py` & `cagpaint-0.1.7/cagpaint/trainer/data_utils.py`

 * *Files identical despite different names*

### Comparing `cagpaint-0.1.6/cagpaint/trainer/datasets.py` & `cagpaint-0.1.7/cagpaint/trainer/datasets.py`

 * *Files identical despite different names*

### Comparing `cagpaint-0.1.6/cagpaint/trainer/file_utils.py` & `cagpaint-0.1.7/cagpaint/trainer/file_utils.py`

 * *Files identical despite different names*

### Comparing `cagpaint-0.1.6/cagpaint/trainer/im_utils.py` & `cagpaint-0.1.7/cagpaint/trainer/im_utils.py`

 * *Files identical despite different names*

### Comparing `cagpaint-0.1.6/cagpaint/trainer/instructions.py` & `cagpaint-0.1.7/cagpaint/trainer/instructions.py`

 * *Files identical despite different names*

### Comparing `cagpaint-0.1.6/cagpaint/trainer/loss.py` & `cagpaint-0.1.7/cagpaint/trainer/loss.py`

 * *Files identical despite different names*

### Comparing `cagpaint-0.1.6/cagpaint/trainer/main.py` & `cagpaint-0.1.7/cagpaint/trainer/main.py`

 * *Files identical despite different names*

### Comparing `cagpaint-0.1.6/cagpaint/trainer/metrics.py` & `cagpaint-0.1.7/cagpaint/trainer/metrics.py`

 * *Files identical despite different names*

### Comparing `cagpaint-0.1.6/cagpaint/trainer/model_utils.py` & `cagpaint-0.1.7/cagpaint/trainer/model_utils.py`

 * *Files identical despite different names*

### Comparing `cagpaint-0.1.6/cagpaint/trainer/patch_seg.py` & `cagpaint-0.1.7/cagpaint/trainer/patch_seg.py`

 * *Files identical despite different names*

### Comparing `cagpaint-0.1.6/cagpaint/trainer/scp_utils.py` & `cagpaint-0.1.7/cagpaint/trainer/scp_utils.py`

 * *Files identical despite different names*

### Comparing `cagpaint-0.1.6/cagpaint/trainer/startup.py` & `cagpaint-0.1.7/cagpaint/trainer/startup.py`

 * *Files identical despite different names*

### Comparing `cagpaint-0.1.6/cagpaint/trainer/trainer.py` & `cagpaint-0.1.7/cagpaint/trainer/trainer.py`

 * *Files identical despite different names*

### Comparing `cagpaint-0.1.6/cagpaint/trainer/unet3d.py` & `cagpaint-0.1.7/cagpaint/trainer/unet3d.py`

 * *Files identical despite different names*

### Comparing `cagpaint-0.1.6/cagpaint.egg-info/SOURCES.txt` & `cagpaint-0.1.7/cagpaint.egg-info/SOURCES.txt`

 * *Files identical despite different names*

