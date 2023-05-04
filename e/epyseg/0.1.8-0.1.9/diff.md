# Comparing `tmp/epyseg-0.1.8.tar.gz` & `tmp/epyseg-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/epyseg-0.1.8.tar", last modified: Wed Jul  8 10:27:37 2020, max compression
+gzip compressed data, was "dist/epyseg-0.1.9.tar", last modified: Wed Jul 15 07:57:02 2020, max compression
```

## Comparing `epyseg-0.1.8.tar` & `epyseg-0.1.9.tar`

### file list

```diff
@@ -1,90 +1,90 @@
-drwxrwxr-x   0 aigouy    (1000) aigouy    (1000)        0 2020-07-08 10:27:37.000000 epyseg-0.1.8/
--rw-rw-r--   0 aigouy    (1000) aigouy    (1000)     1910 2020-07-08 10:27:37.000000 epyseg-0.1.8/PKG-INFO
--rw-rw-rw-   0 aigouy    (1000) aigouy    (1000)     1143 2020-06-16 12:56:27.000000 epyseg-0.1.8/README.md
-drwxrwxr-x   0 aigouy    (1000) aigouy    (1000)        0 2020-07-08 10:27:37.000000 epyseg-0.1.8/epyseg/
--rw-rw-rw-   0 aigouy    (1000) aigouy    (1000)        0 2020-03-27 09:27:26.000000 epyseg-0.1.8/epyseg/__init__.py
--rw-rw-rw-   0 aigouy    (1000) aigouy    (1000)      351 2020-04-04 13:23:02.000000 epyseg-0.1.8/epyseg/__main__.py
-drwxrwxr-x   0 aigouy    (1000) aigouy    (1000)        0 2020-07-08 10:27:37.000000 epyseg-0.1.8/epyseg/binarytools/
--rw-r--r--   0 aigouy    (1000) aigouy    (1000)        0 2020-04-22 09:22:20.000000 epyseg-0.1.8/epyseg/binarytools/__init__.py
--rw-r--r--   0 aigouy    (1000) aigouy    (1000)     3471 2020-06-12 14:22:45.000000 epyseg-0.1.8/epyseg/binarytools/cell_center_detector.py
-drwxrwxr-x   0 aigouy    (1000) aigouy    (1000)        0 2020-07-08 10:27:37.000000 epyseg-0.1.8/epyseg/deeplearning/
--rw-rw-rw-   0 aigouy    (1000) aigouy    (1000)        0 2020-03-27 16:28:29.000000 epyseg-0.1.8/epyseg/deeplearning/__init__.py
-drwxrwxr-x   0 aigouy    (1000) aigouy    (1000)        0 2020-07-08 10:27:37.000000 epyseg-0.1.8/epyseg/deeplearning/augmentation/
--rw-rw-rw-   0 aigouy    (1000) aigouy    (1000)        0 2020-03-27 16:20:08.000000 epyseg-0.1.8/epyseg/deeplearning/augmentation/__init__.py
-drwxrwxr-x   0 aigouy    (1000) aigouy    (1000)        0 2020-07-08 10:27:37.000000 epyseg-0.1.8/epyseg/deeplearning/augmentation/generators/
--rw-rw-rw-   0 aigouy    (1000) aigouy    (1000)        0 2020-03-28 13:08:25.000000 epyseg-0.1.8/epyseg/deeplearning/augmentation/generators/__init__.py
--rw-rw-rw-   0 aigouy    (1000) aigouy    (1000)    64749 2020-06-23 08:06:14.000000 epyseg-0.1.8/epyseg/deeplearning/augmentation/generators/data.py
--rw-rw-rw-   0 aigouy    (1000) aigouy    (1000)     6508 2020-04-04 14:59:54.000000 epyseg-0.1.8/epyseg/deeplearning/augmentation/generators/meta.py
--rw-rw-rw-   0 aigouy    (1000) aigouy    (1000)    21190 2020-06-22 15:26:47.000000 epyseg-0.1.8/epyseg/deeplearning/augmentation/meta.py
-drwxrwxr-x   0 aigouy    (1000) aigouy    (1000)        0 2020-07-08 10:27:37.000000 epyseg-0.1.8/epyseg/deeplearning/callbacks/
--rw-rw-rw-   0 aigouy    (1000) aigouy    (1000)        0 2020-03-27 16:26:24.000000 epyseg-0.1.8/epyseg/deeplearning/callbacks/__init__.py
--rw-rw-rw-   0 aigouy    (1000) aigouy    (1000)    17454 2020-06-12 14:39:24.000000 epyseg-0.1.8/epyseg/deeplearning/callbacks/saver.py
--rw-rw-rw-   0 aigouy    (1000) aigouy    (1000)      626 2020-06-11 11:42:37.000000 epyseg-0.1.8/epyseg/deeplearning/callbacks/stop.py
--rw-rw-rw-   0 aigouy    (1000) aigouy    (1000)    72111 2020-07-08 09:13:52.000000 epyseg-0.1.8/epyseg/deeplearning/deepl.py
-drwxrwxr-x   0 aigouy    (1000) aigouy    (1000)        0 2020-07-08 10:27:37.000000 epyseg-0.1.8/epyseg/deeplearning/docs/
--rw-rw-rw-   0 aigouy    (1000) aigouy    (1000)        0 2020-03-27 09:27:26.000000 epyseg-0.1.8/epyseg/deeplearning/docs/__init__.py
-drwxrwxr-x   0 aigouy    (1000) aigouy    (1000)        0 2020-07-08 10:27:37.000000 epyseg-0.1.8/epyseg/dialogs/
--rw-rw-rw-   0 aigouy    (1000) aigouy    (1000)        0 2020-03-27 16:19:05.000000 epyseg-0.1.8/epyseg/dialogs/__init__.py
--rw-rw-rw-   0 aigouy    (1000) aigouy    (1000)     2431 2020-06-11 09:29:08.000000 epyseg-0.1.8/epyseg/dialogs/opensave.py
-drwxrwxr-x   0 aigouy    (1000) aigouy    (1000)        0 2020-07-08 10:27:37.000000 epyseg-0.1.8/epyseg/draw/
--rw-rw-rw-   0 aigouy    (1000) aigouy    (1000)        0 2020-03-27 09:27:26.000000 epyseg-0.1.8/epyseg/draw/__init__.py
-drwxrwxr-x   0 aigouy    (1000) aigouy    (1000)        0 2020-07-08 10:27:37.000000 epyseg-0.1.8/epyseg/draw/shapes/
--rw-rw-rw-   0 aigouy    (1000) aigouy    (1000)        0 2020-03-28 13:02:32.000000 epyseg-0.1.8/epyseg/draw/shapes/__init__.py
--rw-rw-rw-   0 aigouy    (1000) aigouy    (1000)     2408 2020-06-11 09:31:10.000000 epyseg-0.1.8/epyseg/draw/shapes/circle2d.py
--rw-rw-rw-   0 aigouy    (1000) aigouy    (1000)     3609 2020-06-11 09:31:15.000000 epyseg-0.1.8/epyseg/draw/shapes/ellipse2d.py
--rw-rw-rw-   0 aigouy    (1000) aigouy    (1000)     3487 2020-06-11 09:33:07.000000 epyseg-0.1.8/epyseg/draw/shapes/freehand2d.py
--rw-r--r--   0 aigouy    (1000) aigouy    (1000)     6234 2020-06-11 09:35:09.000000 epyseg-0.1.8/epyseg/draw/shapes/image2d.py
--rw-rw-rw-   0 aigouy    (1000) aigouy    (1000)     3760 2020-06-11 09:36:35.000000 epyseg-0.1.8/epyseg/draw/shapes/line2d.py
--rw-rw-rw-   0 aigouy    (1000) aigouy    (1000)     3791 2020-06-11 09:39:59.000000 epyseg-0.1.8/epyseg/draw/shapes/point2d.py
--rw-rw-rw-   0 aigouy    (1000) aigouy    (1000)     4240 2020-06-11 09:38:09.000000 epyseg-0.1.8/epyseg/draw/shapes/polygon2d.py
--rw-rw-rw-   0 aigouy    (1000) aigouy    (1000)     3712 2020-06-11 09:38:33.000000 epyseg-0.1.8/epyseg/draw/shapes/polyline2d.py
--rw-rw-rw-   0 aigouy    (1000) aigouy    (1000)     3190 2020-06-11 09:40:14.000000 epyseg-0.1.8/epyseg/draw/shapes/rect2d.py
--rw-rw-rw-   0 aigouy    (1000) aigouy    (1000)     2264 2020-06-11 09:39:59.000000 epyseg-0.1.8/epyseg/draw/shapes/square2d.py
--rw-r--r--   0 aigouy    (1000) aigouy    (1000)     6416 2020-06-11 09:43:03.000000 epyseg-0.1.8/epyseg/draw/shapes/txt2d.py
-drwxrwxr-x   0 aigouy    (1000) aigouy    (1000)        0 2020-07-08 10:27:37.000000 epyseg-0.1.8/epyseg/draw/widgets/
--rw-rw-rw-   0 aigouy    (1000) aigouy    (1000)        0 2020-03-28 13:11:30.000000 epyseg-0.1.8/epyseg/draw/widgets/__init__.py
--rw-rw-rw-   0 aigouy    (1000) aigouy    (1000)     7042 2020-04-04 13:21:02.000000 epyseg-0.1.8/epyseg/draw/widgets/paint.py
--rw-rw-rw-   0 aigouy    (1000) aigouy    (1000)     9827 2020-06-01 14:20:12.000000 epyseg-0.1.8/epyseg/draw/widgets/vectorial.py
--rw-rw-rw-   0 aigouy    (1000) aigouy    (1000)    68069 2020-07-08 10:20:41.000000 epyseg-0.1.8/epyseg/epygui.py
--rw-r--r--   0 aigouy    (1000) aigouy    (1000)    18430 2020-07-08 08:31:55.000000 epyseg-0.1.8/epyseg/ezfig.py
-drwxrwxr-x   0 aigouy    (1000) aigouy    (1000)        0 2020-07-08 10:27:37.000000 epyseg-0.1.8/epyseg/figure/
--rw-rw-rw-   0 aigouy    (1000) aigouy    (1000)        0 2020-03-27 09:27:26.000000 epyseg-0.1.8/epyseg/figure/__init__.py
--rw-r--r--   0 aigouy    (1000) aigouy    (1000)    11998 2020-06-02 09:57:17.000000 epyseg-0.1.8/epyseg/figure/column.py
--rw-rw-rw-   0 aigouy    (1000) aigouy    (1000)    26185 2020-06-11 09:27:23.000000 epyseg-0.1.8/epyseg/figure/panel.py
--rw-rw-rw-   0 aigouy    (1000) aigouy    (1000)    11884 2020-06-02 09:05:41.000000 epyseg-0.1.8/epyseg/figure/row.py
-drwxrwxr-x   0 aigouy    (1000) aigouy    (1000)        0 2020-07-08 10:27:37.000000 epyseg-0.1.8/epyseg/gui/
--rw-rw-rw-   0 aigouy    (1000) aigouy    (1000)        0 2020-03-28 12:55:34.000000 epyseg-0.1.8/epyseg/gui/__init__.py
--rw-rw-rw-   0 aigouy    (1000) aigouy    (1000)     3379 2020-06-19 12:20:47.000000 epyseg-0.1.8/epyseg/gui/augmenter.py
--rw-rw-rw-   0 aigouy    (1000) aigouy    (1000)    59050 2020-06-19 07:03:44.000000 epyseg-0.1.8/epyseg/gui/img.py
--rw-rw-rw-   0 aigouy    (1000) aigouy    (1000)     1654 2020-04-03 12:24:59.000000 epyseg-0.1.8/epyseg/gui/markdown.py
--rw-rw-rw-   0 aigouy    (1000) aigouy    (1000)    16003 2020-04-04 13:21:02.000000 epyseg-0.1.8/epyseg/gui/metaaugmenter.py
--rw-rw-rw-   0 aigouy    (1000) aigouy    (1000)     5797 2020-06-11 09:45:05.000000 epyseg-0.1.8/epyseg/gui/open.py
--rw-rw-rw-   0 aigouy    (1000) aigouy    (1000)     5040 2020-04-04 13:21:02.000000 epyseg-0.1.8/epyseg/gui/preview.py
--rw-rw-rw-   0 aigouy    (1000) aigouy    (1000)    68718 2020-06-18 07:02:26.000000 epyseg-0.1.8/epyseg/img.py
-drwxrwxr-x   0 aigouy    (1000) aigouy    (1000)        0 2020-07-08 10:27:37.000000 epyseg-0.1.8/epyseg/logs/
--rw-rw-rw-   0 aigouy    (1000) aigouy    (1000)        0 2020-03-27 09:27:26.000000 epyseg-0.1.8/epyseg/logs/__init__.py
-drwxrwxr-x   0 aigouy    (1000) aigouy    (1000)        0 2020-07-08 10:27:37.000000 epyseg-0.1.8/epyseg/postprocess/
--rw-r--r--   0 aigouy    (1000) aigouy    (1000)        0 2020-05-06 06:24:39.000000 epyseg-0.1.8/epyseg/postprocess/__init__.py
--rw-r--r--   0 aigouy    (1000) aigouy    (1000)     6335 2020-06-11 09:03:20.000000 epyseg-0.1.8/epyseg/postprocess/gui.py
--rw-r--r--   0 aigouy    (1000) aigouy    (1000)    33612 2020-07-03 13:05:14.000000 epyseg-0.1.8/epyseg/postprocess/refine.py
-drwxrwxr-x   0 aigouy    (1000) aigouy    (1000)        0 2020-07-08 10:27:37.000000 epyseg-0.1.8/epyseg/tests/
--rw-rw-rw-   0 aigouy    (1000) aigouy    (1000)        0 2020-03-27 09:27:26.000000 epyseg-0.1.8/epyseg/tests/__init__.py
-drwxrwxr-x   0 aigouy    (1000) aigouy    (1000)        0 2020-07-08 10:27:37.000000 epyseg-0.1.8/epyseg/tools/
--rw-rw-rw-   0 aigouy    (1000) aigouy    (1000)        0 2020-03-27 09:27:26.000000 epyseg-0.1.8/epyseg/tools/__init__.py
--rw-rw-rw-   0 aigouy    (1000) aigouy    (1000)     1977 2020-04-16 20:30:22.000000 epyseg-0.1.8/epyseg/tools/logger.py
--rw-rw-rw-   0 aigouy    (1000) aigouy    (1000)     1234 2020-04-04 14:49:05.000000 epyseg-0.1.8/epyseg/tools/qthandler.py
-drwxrwxr-x   0 aigouy    (1000) aigouy    (1000)        0 2020-07-08 10:27:37.000000 epyseg-0.1.8/epyseg/uitools/
--rw-rw-rw-   0 aigouy    (1000) aigouy    (1000)        0 2020-03-27 16:19:05.000000 epyseg-0.1.8/epyseg/uitools/__init__.py
--rw-rw-rw-   0 aigouy    (1000) aigouy    (1000)      828 2020-04-03 12:44:35.000000 epyseg-0.1.8/epyseg/uitools/blinker.py
-drwxrwxr-x   0 aigouy    (1000) aigouy    (1000)        0 2020-07-08 10:27:37.000000 epyseg-0.1.8/epyseg/worker/
--rw-rw-rw-   0 aigouy    (1000) aigouy    (1000)        0 2020-03-28 12:59:49.000000 epyseg-0.1.8/epyseg/worker/__init__.py
--rw-rw-rw-   0 aigouy    (1000) aigouy    (1000)     1954 2020-04-03 12:48:32.000000 epyseg-0.1.8/epyseg/worker/fake.py
--rw-rw-rw-   0 aigouy    (1000) aigouy    (1000)     2099 2020-04-03 12:48:28.000000 epyseg-0.1.8/epyseg/worker/threaded.py
-drwxrwxr-x   0 aigouy    (1000) aigouy    (1000)        0 2020-07-08 10:27:37.000000 epyseg-0.1.8/epyseg.egg-info/
--rw-rw-r--   0 aigouy    (1000) aigouy    (1000)     1910 2020-07-08 10:27:37.000000 epyseg-0.1.8/epyseg.egg-info/PKG-INFO
--rw-rw-r--   0 aigouy    (1000) aigouy    (1000)     1917 2020-07-08 10:27:37.000000 epyseg-0.1.8/epyseg.egg-info/SOURCES.txt
--rw-rw-r--   0 aigouy    (1000) aigouy    (1000)        1 2020-07-08 10:27:37.000000 epyseg-0.1.8/epyseg.egg-info/dependency_links.txt
--rw-rw-r--   0 aigouy    (1000) aigouy    (1000)      208 2020-07-08 10:27:37.000000 epyseg-0.1.8/epyseg.egg-info/requires.txt
--rw-rw-r--   0 aigouy    (1000) aigouy    (1000)        7 2020-07-08 10:27:37.000000 epyseg-0.1.8/epyseg.egg-info/top_level.txt
--rw-rw-r--   0 aigouy    (1000) aigouy    (1000)       38 2020-07-08 10:27:37.000000 epyseg-0.1.8/setup.cfg
--rw-rw-rw-   0 aigouy    (1000) aigouy    (1000)     2234 2020-07-08 09:46:34.000000 epyseg-0.1.8/setup.py
+drwxrwxr-x   0 aigouy    (1000) aigouy    (1000)        0 2020-07-15 07:57:02.000000 epyseg-0.1.9/
+-rw-rw-r--   0 aigouy    (1000) aigouy    (1000)     1986 2020-07-15 07:57:02.000000 epyseg-0.1.9/PKG-INFO
+-rw-rw-rw-   0 aigouy    (1000) aigouy    (1000)     1219 2020-07-09 07:57:56.000000 epyseg-0.1.9/README.md
+drwxrwxr-x   0 aigouy    (1000) aigouy    (1000)        0 2020-07-15 07:57:02.000000 epyseg-0.1.9/epyseg/
+-rw-rw-rw-   0 aigouy    (1000) aigouy    (1000)        0 2020-03-27 09:27:26.000000 epyseg-0.1.9/epyseg/__init__.py
+-rw-rw-rw-   0 aigouy    (1000) aigouy    (1000)      351 2020-04-04 13:23:02.000000 epyseg-0.1.9/epyseg/__main__.py
+drwxrwxr-x   0 aigouy    (1000) aigouy    (1000)        0 2020-07-15 07:57:02.000000 epyseg-0.1.9/epyseg/binarytools/
+-rw-r--r--   0 aigouy    (1000) aigouy    (1000)        0 2020-04-22 09:22:20.000000 epyseg-0.1.9/epyseg/binarytools/__init__.py
+-rw-r--r--   0 aigouy    (1000) aigouy    (1000)     3471 2020-06-12 14:22:45.000000 epyseg-0.1.9/epyseg/binarytools/cell_center_detector.py
+drwxrwxr-x   0 aigouy    (1000) aigouy    (1000)        0 2020-07-15 07:57:02.000000 epyseg-0.1.9/epyseg/deeplearning/
+-rw-rw-rw-   0 aigouy    (1000) aigouy    (1000)        0 2020-03-27 16:28:29.000000 epyseg-0.1.9/epyseg/deeplearning/__init__.py
+drwxrwxr-x   0 aigouy    (1000) aigouy    (1000)        0 2020-07-15 07:57:02.000000 epyseg-0.1.9/epyseg/deeplearning/augmentation/
+-rw-rw-rw-   0 aigouy    (1000) aigouy    (1000)        0 2020-03-27 16:20:08.000000 epyseg-0.1.9/epyseg/deeplearning/augmentation/__init__.py
+drwxrwxr-x   0 aigouy    (1000) aigouy    (1000)        0 2020-07-15 07:57:02.000000 epyseg-0.1.9/epyseg/deeplearning/augmentation/generators/
+-rw-rw-rw-   0 aigouy    (1000) aigouy    (1000)        0 2020-03-28 13:08:25.000000 epyseg-0.1.9/epyseg/deeplearning/augmentation/generators/__init__.py
+-rw-rw-rw-   0 aigouy    (1000) aigouy    (1000)    64749 2020-06-23 08:06:14.000000 epyseg-0.1.9/epyseg/deeplearning/augmentation/generators/data.py
+-rw-rw-rw-   0 aigouy    (1000) aigouy    (1000)     6508 2020-04-04 14:59:54.000000 epyseg-0.1.9/epyseg/deeplearning/augmentation/generators/meta.py
+-rw-rw-rw-   0 aigouy    (1000) aigouy    (1000)    21190 2020-06-22 15:26:47.000000 epyseg-0.1.9/epyseg/deeplearning/augmentation/meta.py
+drwxrwxr-x   0 aigouy    (1000) aigouy    (1000)        0 2020-07-15 07:57:02.000000 epyseg-0.1.9/epyseg/deeplearning/callbacks/
+-rw-rw-rw-   0 aigouy    (1000) aigouy    (1000)        0 2020-03-27 16:26:24.000000 epyseg-0.1.9/epyseg/deeplearning/callbacks/__init__.py
+-rw-rw-rw-   0 aigouy    (1000) aigouy    (1000)    17907 2020-07-15 07:44:22.000000 epyseg-0.1.9/epyseg/deeplearning/callbacks/saver.py
+-rw-rw-rw-   0 aigouy    (1000) aigouy    (1000)      626 2020-06-11 11:42:37.000000 epyseg-0.1.9/epyseg/deeplearning/callbacks/stop.py
+-rw-rw-rw-   0 aigouy    (1000) aigouy    (1000)    72120 2020-07-15 07:47:24.000000 epyseg-0.1.9/epyseg/deeplearning/deepl.py
+drwxrwxr-x   0 aigouy    (1000) aigouy    (1000)        0 2020-07-15 07:57:02.000000 epyseg-0.1.9/epyseg/deeplearning/docs/
+-rw-rw-rw-   0 aigouy    (1000) aigouy    (1000)        0 2020-03-27 09:27:26.000000 epyseg-0.1.9/epyseg/deeplearning/docs/__init__.py
+drwxrwxr-x   0 aigouy    (1000) aigouy    (1000)        0 2020-07-15 07:57:02.000000 epyseg-0.1.9/epyseg/dialogs/
+-rw-rw-rw-   0 aigouy    (1000) aigouy    (1000)        0 2020-03-27 16:19:05.000000 epyseg-0.1.9/epyseg/dialogs/__init__.py
+-rw-rw-rw-   0 aigouy    (1000) aigouy    (1000)     2431 2020-06-11 09:29:08.000000 epyseg-0.1.9/epyseg/dialogs/opensave.py
+drwxrwxr-x   0 aigouy    (1000) aigouy    (1000)        0 2020-07-15 07:57:02.000000 epyseg-0.1.9/epyseg/draw/
+-rw-rw-rw-   0 aigouy    (1000) aigouy    (1000)        0 2020-03-27 09:27:26.000000 epyseg-0.1.9/epyseg/draw/__init__.py
+drwxrwxr-x   0 aigouy    (1000) aigouy    (1000)        0 2020-07-15 07:57:02.000000 epyseg-0.1.9/epyseg/draw/shapes/
+-rw-rw-rw-   0 aigouy    (1000) aigouy    (1000)        0 2020-03-28 13:02:32.000000 epyseg-0.1.9/epyseg/draw/shapes/__init__.py
+-rw-rw-rw-   0 aigouy    (1000) aigouy    (1000)     2408 2020-06-11 09:31:10.000000 epyseg-0.1.9/epyseg/draw/shapes/circle2d.py
+-rw-rw-rw-   0 aigouy    (1000) aigouy    (1000)     3609 2020-06-11 09:31:15.000000 epyseg-0.1.9/epyseg/draw/shapes/ellipse2d.py
+-rw-rw-rw-   0 aigouy    (1000) aigouy    (1000)     3487 2020-06-11 09:33:07.000000 epyseg-0.1.9/epyseg/draw/shapes/freehand2d.py
+-rw-r--r--   0 aigouy    (1000) aigouy    (1000)     6234 2020-06-11 09:35:09.000000 epyseg-0.1.9/epyseg/draw/shapes/image2d.py
+-rw-rw-rw-   0 aigouy    (1000) aigouy    (1000)     3760 2020-06-11 09:36:35.000000 epyseg-0.1.9/epyseg/draw/shapes/line2d.py
+-rw-rw-rw-   0 aigouy    (1000) aigouy    (1000)     3791 2020-06-11 09:39:59.000000 epyseg-0.1.9/epyseg/draw/shapes/point2d.py
+-rw-rw-rw-   0 aigouy    (1000) aigouy    (1000)     4240 2020-06-11 09:38:09.000000 epyseg-0.1.9/epyseg/draw/shapes/polygon2d.py
+-rw-rw-rw-   0 aigouy    (1000) aigouy    (1000)     3712 2020-06-11 09:38:33.000000 epyseg-0.1.9/epyseg/draw/shapes/polyline2d.py
+-rw-rw-rw-   0 aigouy    (1000) aigouy    (1000)     3190 2020-06-11 09:40:14.000000 epyseg-0.1.9/epyseg/draw/shapes/rect2d.py
+-rw-rw-rw-   0 aigouy    (1000) aigouy    (1000)     2264 2020-06-11 09:39:59.000000 epyseg-0.1.9/epyseg/draw/shapes/square2d.py
+-rw-r--r--   0 aigouy    (1000) aigouy    (1000)     6416 2020-06-11 09:43:03.000000 epyseg-0.1.9/epyseg/draw/shapes/txt2d.py
+drwxrwxr-x   0 aigouy    (1000) aigouy    (1000)        0 2020-07-15 07:57:02.000000 epyseg-0.1.9/epyseg/draw/widgets/
+-rw-rw-rw-   0 aigouy    (1000) aigouy    (1000)        0 2020-03-28 13:11:30.000000 epyseg-0.1.9/epyseg/draw/widgets/__init__.py
+-rw-rw-rw-   0 aigouy    (1000) aigouy    (1000)     7042 2020-04-04 13:21:02.000000 epyseg-0.1.9/epyseg/draw/widgets/paint.py
+-rw-rw-rw-   0 aigouy    (1000) aigouy    (1000)     9827 2020-06-01 14:20:12.000000 epyseg-0.1.9/epyseg/draw/widgets/vectorial.py
+-rw-rw-rw-   0 aigouy    (1000) aigouy    (1000)    68069 2020-07-15 07:46:10.000000 epyseg-0.1.9/epyseg/epygui.py
+-rw-r--r--   0 aigouy    (1000) aigouy    (1000)    18430 2020-07-08 08:31:55.000000 epyseg-0.1.9/epyseg/ezfig.py
+drwxrwxr-x   0 aigouy    (1000) aigouy    (1000)        0 2020-07-15 07:57:02.000000 epyseg-0.1.9/epyseg/figure/
+-rw-rw-rw-   0 aigouy    (1000) aigouy    (1000)        0 2020-03-27 09:27:26.000000 epyseg-0.1.9/epyseg/figure/__init__.py
+-rw-r--r--   0 aigouy    (1000) aigouy    (1000)    11998 2020-06-02 09:57:17.000000 epyseg-0.1.9/epyseg/figure/column.py
+-rw-rw-rw-   0 aigouy    (1000) aigouy    (1000)    26185 2020-06-11 09:27:23.000000 epyseg-0.1.9/epyseg/figure/panel.py
+-rw-rw-rw-   0 aigouy    (1000) aigouy    (1000)    11884 2020-06-02 09:05:41.000000 epyseg-0.1.9/epyseg/figure/row.py
+drwxrwxr-x   0 aigouy    (1000) aigouy    (1000)        0 2020-07-15 07:57:02.000000 epyseg-0.1.9/epyseg/gui/
+-rw-rw-rw-   0 aigouy    (1000) aigouy    (1000)        0 2020-03-28 12:55:34.000000 epyseg-0.1.9/epyseg/gui/__init__.py
+-rw-rw-rw-   0 aigouy    (1000) aigouy    (1000)     3379 2020-06-19 12:20:47.000000 epyseg-0.1.9/epyseg/gui/augmenter.py
+-rw-rw-rw-   0 aigouy    (1000) aigouy    (1000)    59050 2020-06-19 07:03:44.000000 epyseg-0.1.9/epyseg/gui/img.py
+-rw-rw-rw-   0 aigouy    (1000) aigouy    (1000)     1654 2020-04-03 12:24:59.000000 epyseg-0.1.9/epyseg/gui/markdown.py
+-rw-rw-rw-   0 aigouy    (1000) aigouy    (1000)    16003 2020-04-04 13:21:02.000000 epyseg-0.1.9/epyseg/gui/metaaugmenter.py
+-rw-rw-rw-   0 aigouy    (1000) aigouy    (1000)     5797 2020-06-11 09:45:05.000000 epyseg-0.1.9/epyseg/gui/open.py
+-rw-rw-rw-   0 aigouy    (1000) aigouy    (1000)     5040 2020-04-04 13:21:02.000000 epyseg-0.1.9/epyseg/gui/preview.py
+-rw-rw-rw-   0 aigouy    (1000) aigouy    (1000)    68828 2020-07-09 13:38:42.000000 epyseg-0.1.9/epyseg/img.py
+drwxrwxr-x   0 aigouy    (1000) aigouy    (1000)        0 2020-07-15 07:57:02.000000 epyseg-0.1.9/epyseg/logs/
+-rw-rw-rw-   0 aigouy    (1000) aigouy    (1000)        0 2020-03-27 09:27:26.000000 epyseg-0.1.9/epyseg/logs/__init__.py
+drwxrwxr-x   0 aigouy    (1000) aigouy    (1000)        0 2020-07-15 07:57:02.000000 epyseg-0.1.9/epyseg/postprocess/
+-rw-r--r--   0 aigouy    (1000) aigouy    (1000)        0 2020-05-06 06:24:39.000000 epyseg-0.1.9/epyseg/postprocess/__init__.py
+-rw-r--r--   0 aigouy    (1000) aigouy    (1000)     6335 2020-06-11 09:03:20.000000 epyseg-0.1.9/epyseg/postprocess/gui.py
+-rw-r--r--   0 aigouy    (1000) aigouy    (1000)    33612 2020-07-03 13:05:14.000000 epyseg-0.1.9/epyseg/postprocess/refine.py
+drwxrwxr-x   0 aigouy    (1000) aigouy    (1000)        0 2020-07-15 07:57:02.000000 epyseg-0.1.9/epyseg/tests/
+-rw-rw-rw-   0 aigouy    (1000) aigouy    (1000)        0 2020-03-27 09:27:26.000000 epyseg-0.1.9/epyseg/tests/__init__.py
+drwxrwxr-x   0 aigouy    (1000) aigouy    (1000)        0 2020-07-15 07:57:02.000000 epyseg-0.1.9/epyseg/tools/
+-rw-rw-rw-   0 aigouy    (1000) aigouy    (1000)        0 2020-03-27 09:27:26.000000 epyseg-0.1.9/epyseg/tools/__init__.py
+-rw-rw-rw-   0 aigouy    (1000) aigouy    (1000)     1977 2020-04-16 20:30:22.000000 epyseg-0.1.9/epyseg/tools/logger.py
+-rw-rw-rw-   0 aigouy    (1000) aigouy    (1000)     1234 2020-04-04 14:49:05.000000 epyseg-0.1.9/epyseg/tools/qthandler.py
+drwxrwxr-x   0 aigouy    (1000) aigouy    (1000)        0 2020-07-15 07:57:02.000000 epyseg-0.1.9/epyseg/uitools/
+-rw-rw-rw-   0 aigouy    (1000) aigouy    (1000)        0 2020-03-27 16:19:05.000000 epyseg-0.1.9/epyseg/uitools/__init__.py
+-rw-rw-rw-   0 aigouy    (1000) aigouy    (1000)      828 2020-04-03 12:44:35.000000 epyseg-0.1.9/epyseg/uitools/blinker.py
+drwxrwxr-x   0 aigouy    (1000) aigouy    (1000)        0 2020-07-15 07:57:02.000000 epyseg-0.1.9/epyseg/worker/
+-rw-rw-rw-   0 aigouy    (1000) aigouy    (1000)        0 2020-03-28 12:59:49.000000 epyseg-0.1.9/epyseg/worker/__init__.py
+-rw-rw-rw-   0 aigouy    (1000) aigouy    (1000)     1954 2020-04-03 12:48:32.000000 epyseg-0.1.9/epyseg/worker/fake.py
+-rw-rw-rw-   0 aigouy    (1000) aigouy    (1000)     2099 2020-04-03 12:48:28.000000 epyseg-0.1.9/epyseg/worker/threaded.py
+drwxrwxr-x   0 aigouy    (1000) aigouy    (1000)        0 2020-07-15 07:57:02.000000 epyseg-0.1.9/epyseg.egg-info/
+-rw-rw-r--   0 aigouy    (1000) aigouy    (1000)     1986 2020-07-15 07:57:02.000000 epyseg-0.1.9/epyseg.egg-info/PKG-INFO
+-rw-rw-r--   0 aigouy    (1000) aigouy    (1000)     1917 2020-07-15 07:57:02.000000 epyseg-0.1.9/epyseg.egg-info/SOURCES.txt
+-rw-rw-r--   0 aigouy    (1000) aigouy    (1000)        1 2020-07-15 07:57:02.000000 epyseg-0.1.9/epyseg.egg-info/dependency_links.txt
+-rw-rw-r--   0 aigouy    (1000) aigouy    (1000)      208 2020-07-15 07:57:02.000000 epyseg-0.1.9/epyseg.egg-info/requires.txt
+-rw-rw-r--   0 aigouy    (1000) aigouy    (1000)        7 2020-07-15 07:57:02.000000 epyseg-0.1.9/epyseg.egg-info/top_level.txt
+-rw-rw-r--   0 aigouy    (1000) aigouy    (1000)       38 2020-07-15 07:57:02.000000 epyseg-0.1.9/setup.cfg
+-rw-rw-rw-   0 aigouy    (1000) aigouy    (1000)     2234 2020-07-08 09:46:34.000000 epyseg-0.1.9/setup.py
```

### Comparing `epyseg-0.1.8/PKG-INFO` & `epyseg-0.1.9/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: epyseg
-Version: 0.1.8
+Version: 0.1.9
 Summary: A deep learning based tool to segment epithelial tissues. The epyseg GUI can be uesd to build, train or run custom networks
 Home-page: https://github.com/baigouy/EPySeg
 Author: Benoit Aigouy
 Author-email: baigouy@gmail.com
 License: BSD
 Description: # EPySeg
         
-        EPySeg is a package for segmenting 2D epithelial tissues. EPySeg also ships with a graphical user interface that allows for building, training and running deep learning models. Training can be done with or without data augmentation (2D-xy and 3D-xyz data augmentation is supported). EPySeg relies on the [segmentation_models](https://github.com/qubvel/segmentation_models) library. EPySeg sources are available [here](https://github.com/baigouy/EPySeg).
+        EPySeg is a package for segmenting 2D epithelial tissues. EPySeg also ships with a graphical user interface that allows for building, training and running deep learning models. Training can be done with or without data augmentation (2D-xy and 3D-xyz data augmentation arejust  supported). EPySeg relies on the [segmentation_models](https://github.com/qubvel/segmentation_models) library. EPySeg sources are available [here](https://github.com/baigouy/EPySeg). Cloud version available [here](https://github.com/baigouy/notebooks).
         
         # Install
         
         1. Install [python 3.7](https://www.python.org/downloads/) or [Anaconda 3.7](https://www.anaconda.com/distribution/) (if not already present on your system)
         
         2. In a command prompt type:
```

### Comparing `epyseg-0.1.8/README.md` & `epyseg-0.1.9/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # EPySeg
 
-EPySeg is a package for segmenting 2D epithelial tissues. EPySeg also ships with a graphical user interface that allows for building, training and running deep learning models. Training can be done with or without data augmentation (2D-xy and 3D-xyz data augmentation is supported). EPySeg relies on the [segmentation_models](https://github.com/qubvel/segmentation_models) library. EPySeg sources are available [here](https://github.com/baigouy/EPySeg).
+EPySeg is a package for segmenting 2D epithelial tissues. EPySeg also ships with a graphical user interface that allows for building, training and running deep learning models. Training can be done with or without data augmentation (2D-xy and 3D-xyz data augmentation arejust  supported). EPySeg relies on the [segmentation_models](https://github.com/qubvel/segmentation_models) library. EPySeg sources are available [here](https://github.com/baigouy/EPySeg). Cloud version available [here](https://github.com/baigouy/notebooks).
 
 # Install
 
 1. Install [python 3.7](https://www.python.org/downloads/) or [Anaconda 3.7](https://www.anaconda.com/distribution/) (if not already present on your system)
 
 2. In a command prompt type:
```

### Comparing `epyseg-0.1.8/epyseg/binarytools/cell_center_detector.py` & `epyseg-0.1.9/epyseg/binarytools/cell_center_detector.py`

 * *Files identical despite different names*

### Comparing `epyseg-0.1.8/epyseg/deeplearning/augmentation/generators/data.py` & `epyseg-0.1.9/epyseg/deeplearning/augmentation/generators/data.py`

 * *Files identical despite different names*

### Comparing `epyseg-0.1.8/epyseg/deeplearning/augmentation/generators/meta.py` & `epyseg-0.1.9/epyseg/deeplearning/augmentation/generators/meta.py`

 * *Files identical despite different names*

### Comparing `epyseg-0.1.8/epyseg/deeplearning/augmentation/meta.py` & `epyseg-0.1.9/epyseg/deeplearning/augmentation/meta.py`

 * *Files identical despite different names*

### Comparing `epyseg-0.1.8/epyseg/deeplearning/callbacks/saver.py` & `epyseg-0.1.9/epyseg/deeplearning/callbacks/saver.py`

 * *Files 2% similar despite different names*

```diff
@@ -197,17 +197,16 @@
 
                                 new_index = self.best_kept.index(val)
                                 real_new_index = len(self.best_kept) - new_index -1
                                 # print('expected_new_index_for_the image', real_new_index)
                                 save_file_name2 = self.save_output_name + '-' + str(real_new_index) + '.h5'
                                 # print(os.path.exists(save_file_name2), self.loss_n_filename[val])
 
-                                os.rename( self.loss_n_filename[val],save_file_name2)
-
-
+                                # os.rename seems to cause a crash if file already exists on windows os see https://stackoverflow.com/questions/45636341/is-it-wise-to-remove-files-using-os-rename-instead-of-os-remove-in-python
+                                os.replace(self.loss_n_filename[val],save_file_name2)
 
                                 # print('new_name_for_the_file', save_file_name2, 'before', self.loss_n_filename[val])
                                 # self.loss_n_filename[val] = save_file_name2
                                 updates[val] = save_file_name2
 
                                 # if counter == 0:
                                 #     print(remove)
@@ -270,15 +269,16 @@
 
                                 if not val in self.loss_n_filename:
                                     continue
 
                                 new_index = self.best_kept.index(val)
                                 real_new_index = len(self.best_kept) - new_index - 1
                                 save_file_name2 = self.save_output_name + '-' + str(real_new_index) + '.h5'
-                                os.rename(self.loss_n_filename[val], save_file_name2)
+                                # os.rename seems to cause a crash if file already exists on windows os see https://stackoverflow.com/questions/45636341/is-it-wise-to-remove-files-using-os-rename-instead-of-os-remove-in-python
+                                os.replace(self.loss_n_filename[val], save_file_name2)
 
                                 # print('renaming 2', self.loss_n_filename[val], 'to', save_file_name2)
 
                                 updates[val] = save_file_name2
 
                             # print("updates", updates)
                             # print('orig', self.loss_n_filename)
```

### Comparing `epyseg-0.1.8/epyseg/deeplearning/callbacks/stop.py` & `epyseg-0.1.9/epyseg/deeplearning/callbacks/stop.py`

 * *Files identical despite different names*

### Comparing `epyseg-0.1.8/epyseg/deeplearning/deepl.py` & `epyseg-0.1.9/epyseg/deeplearning/deepl.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 # TODO add vgg normalization
 # TODO design a metrics BASED ON CELLS OR SEEDS --> HOW MANY SEEDS/CELLS OVELAP WITH EXPECTED --> COULD EVEN BE MY REAL METRIC ULTIMATELY
 
 import os
 os.environ['SM_FRAMEWORK'] = 'tf.keras'  # set env var for changing the segmentation_model framework
 import traceback
-import re
 import matplotlib.pyplot as plt
 from epyseg.img import Img
 from epyseg.deeplearning.augmentation.generators.data import DataGenerator
 import numpy as np
 import tensorflow as tf
 import urllib.request
 import hashlib
+import re
 from epyseg.postprocess.refine import EPySegPostProcess
 import segmentation_models as sm
 # sm.set_framework('tf.keras') # alternative fix = changing framework on the fly
 from epyseg.deeplearning.callbacks.saver import My_saver_callback
 from epyseg.deeplearning.callbacks.stop import myStopCallback
 from segmentation_models.metrics import *
 from segmentation_models.losses import *
@@ -253,15 +253,15 @@
 
         # gpu_options = tf.GPUOptions(allow_growth=True)
         # session = tf.InteractiveSession(config=tf.ConfigProto(gpu_options=gpu_options))
 
         try:
             physical_devices = tf.config.list_physical_devices('GPU')
         except:
-            # dirty hack for tf2.0 support for mac OS X
+            # dirty hack for tf2.0 support for mac OS X anaconda
             physical_devices = tf.config.experimental.list_physical_devices('GPU')
         for physical_device in physical_devices:
             try:
                 tf.config.experimental.set_memory_growth(physical_device, True)
             except:
                 # Invalid device or cannot modify.
                 pass
```

### Comparing `epyseg-0.1.8/epyseg/dialogs/opensave.py` & `epyseg-0.1.9/epyseg/dialogs/opensave.py`

 * *Files identical despite different names*

### Comparing `epyseg-0.1.8/epyseg/draw/shapes/circle2d.py` & `epyseg-0.1.9/epyseg/draw/shapes/circle2d.py`

 * *Files identical despite different names*

### Comparing `epyseg-0.1.8/epyseg/draw/shapes/ellipse2d.py` & `epyseg-0.1.9/epyseg/draw/shapes/ellipse2d.py`

 * *Files identical despite different names*

### Comparing `epyseg-0.1.8/epyseg/draw/shapes/freehand2d.py` & `epyseg-0.1.9/epyseg/draw/shapes/freehand2d.py`

 * *Files identical despite different names*

### Comparing `epyseg-0.1.8/epyseg/draw/shapes/image2d.py` & `epyseg-0.1.9/epyseg/draw/shapes/image2d.py`

 * *Files identical despite different names*

### Comparing `epyseg-0.1.8/epyseg/draw/shapes/line2d.py` & `epyseg-0.1.9/epyseg/draw/shapes/line2d.py`

 * *Files identical despite different names*

### Comparing `epyseg-0.1.8/epyseg/draw/shapes/point2d.py` & `epyseg-0.1.9/epyseg/draw/shapes/point2d.py`

 * *Files identical despite different names*

### Comparing `epyseg-0.1.8/epyseg/draw/shapes/polygon2d.py` & `epyseg-0.1.9/epyseg/draw/shapes/polygon2d.py`

 * *Files identical despite different names*

### Comparing `epyseg-0.1.8/epyseg/draw/shapes/polyline2d.py` & `epyseg-0.1.9/epyseg/draw/shapes/polyline2d.py`

 * *Files identical despite different names*

### Comparing `epyseg-0.1.8/epyseg/draw/shapes/rect2d.py` & `epyseg-0.1.9/epyseg/draw/shapes/rect2d.py`

 * *Files identical despite different names*

### Comparing `epyseg-0.1.8/epyseg/draw/shapes/square2d.py` & `epyseg-0.1.9/epyseg/draw/shapes/square2d.py`

 * *Files identical despite different names*

### Comparing `epyseg-0.1.8/epyseg/draw/shapes/txt2d.py` & `epyseg-0.1.9/epyseg/draw/shapes/txt2d.py`

 * *Files identical despite different names*

### Comparing `epyseg-0.1.8/epyseg/draw/widgets/paint.py` & `epyseg-0.1.9/epyseg/draw/widgets/paint.py`

 * *Files identical despite different names*

### Comparing `epyseg-0.1.8/epyseg/draw/widgets/vectorial.py` & `epyseg-0.1.9/epyseg/draw/widgets/vectorial.py`

 * *Files identical despite different names*

### Comparing `epyseg-0.1.8/epyseg/epygui.py` & `epyseg-0.1.9/epyseg/epygui.py`

 * *Files 0% similar despite different names*

```diff
@@ -32,15 +32,15 @@
 logger = TA_logger()
 
 QtWidgets.QApplication.setAttribute(QtCore.Qt.AA_EnableHighDpiScaling, True)  # high DPI fix
 
 DEBUG = False  # set to True if GUI crashes
 __MAJOR__ = 0
 __MINOR__ = 1
-__MICRO__ = 8
+__MICRO__ = 9
 __RELEASE__ = ''  # a #b  # https://www.python.org/dev/peps/pep-0440/#public-version-identifiers --> alpha beta, ...
 __VERSION__ = ''.join([str(__MAJOR__), '.', str(__MINOR__), '.', str(__MICRO__)])# if __MICRO__ != 0 else '', __RELEASE__]) # bug here fix some day
 __AUTHOR__ = 'Benoit Aigouy'
 __NAME__ = 'EPySeg'
 __EMAIL__ = 'baigouy@gmail.com'
 
 class EPySeg(QWidget):
```

### Comparing `epyseg-0.1.8/epyseg/ezfig.py` & `epyseg-0.1.9/epyseg/ezfig.py`

 * *Files identical despite different names*

### Comparing `epyseg-0.1.8/epyseg/figure/column.py` & `epyseg-0.1.9/epyseg/figure/column.py`

 * *Files identical despite different names*

### Comparing `epyseg-0.1.8/epyseg/figure/panel.py` & `epyseg-0.1.9/epyseg/figure/panel.py`

 * *Files identical despite different names*

### Comparing `epyseg-0.1.8/epyseg/figure/row.py` & `epyseg-0.1.9/epyseg/figure/row.py`

 * *Files identical despite different names*

### Comparing `epyseg-0.1.8/epyseg/gui/augmenter.py` & `epyseg-0.1.9/epyseg/gui/augmenter.py`

 * *Files identical despite different names*

### Comparing `epyseg-0.1.8/epyseg/gui/img.py` & `epyseg-0.1.9/epyseg/gui/img.py`

 * *Files identical despite different names*

### Comparing `epyseg-0.1.8/epyseg/gui/markdown.py` & `epyseg-0.1.9/epyseg/gui/markdown.py`

 * *Files identical despite different names*

### Comparing `epyseg-0.1.8/epyseg/gui/metaaugmenter.py` & `epyseg-0.1.9/epyseg/gui/metaaugmenter.py`

 * *Files identical despite different names*

### Comparing `epyseg-0.1.8/epyseg/gui/open.py` & `epyseg-0.1.9/epyseg/gui/open.py`

 * *Files identical despite different names*

### Comparing `epyseg-0.1.8/epyseg/gui/preview.py` & `epyseg-0.1.9/epyseg/gui/preview.py`

 * *Files identical despite different names*

### Comparing `epyseg-0.1.8/epyseg/img.py` & `epyseg-0.1.9/epyseg/img.py`

 * *Files 0% similar despite different names*

```diff
@@ -702,14 +702,15 @@
         Parameters
         ----------
         type : string
             projection type
 
         '''
 
+        # TODO implement that more wisely asking just which dimension should be projected and projection type
         proj_dimensions = []
         if self.has_t():
             proj_dimensions.append(self.get_dimension('t'))
         proj_dimensions.append(self.get_height())
         proj_dimensions.append(self.get_width())
         if self.has_c():
             proj_dimensions.append(self.get_dimension('c'))
```

### Comparing `epyseg-0.1.8/epyseg/postprocess/gui.py` & `epyseg-0.1.9/epyseg/postprocess/gui.py`

 * *Files identical despite different names*

### Comparing `epyseg-0.1.8/epyseg/postprocess/refine.py` & `epyseg-0.1.9/epyseg/postprocess/refine.py`

 * *Files identical despite different names*

### Comparing `epyseg-0.1.8/epyseg/tools/logger.py` & `epyseg-0.1.9/epyseg/tools/logger.py`

 * *Files identical despite different names*

### Comparing `epyseg-0.1.8/epyseg/tools/qthandler.py` & `epyseg-0.1.9/epyseg/tools/qthandler.py`

 * *Files identical despite different names*

### Comparing `epyseg-0.1.8/epyseg/uitools/blinker.py` & `epyseg-0.1.9/epyseg/uitools/blinker.py`

 * *Files identical despite different names*

### Comparing `epyseg-0.1.8/epyseg/worker/fake.py` & `epyseg-0.1.9/epyseg/worker/fake.py`

 * *Files identical despite different names*

### Comparing `epyseg-0.1.8/epyseg/worker/threaded.py` & `epyseg-0.1.9/epyseg/worker/threaded.py`

 * *Files identical despite different names*

### Comparing `epyseg-0.1.8/epyseg.egg-info/PKG-INFO` & `epyseg-0.1.9/epyseg.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: epyseg
-Version: 0.1.8
+Version: 0.1.9
 Summary: A deep learning based tool to segment epithelial tissues. The epyseg GUI can be uesd to build, train or run custom networks
 Home-page: https://github.com/baigouy/EPySeg
 Author: Benoit Aigouy
 Author-email: baigouy@gmail.com
 License: BSD
 Description: # EPySeg
         
-        EPySeg is a package for segmenting 2D epithelial tissues. EPySeg also ships with a graphical user interface that allows for building, training and running deep learning models. Training can be done with or without data augmentation (2D-xy and 3D-xyz data augmentation is supported). EPySeg relies on the [segmentation_models](https://github.com/qubvel/segmentation_models) library. EPySeg sources are available [here](https://github.com/baigouy/EPySeg).
+        EPySeg is a package for segmenting 2D epithelial tissues. EPySeg also ships with a graphical user interface that allows for building, training and running deep learning models. Training can be done with or without data augmentation (2D-xy and 3D-xyz data augmentation arejust  supported). EPySeg relies on the [segmentation_models](https://github.com/qubvel/segmentation_models) library. EPySeg sources are available [here](https://github.com/baigouy/EPySeg). Cloud version available [here](https://github.com/baigouy/notebooks).
         
         # Install
         
         1. Install [python 3.7](https://www.python.org/downloads/) or [Anaconda 3.7](https://www.anaconda.com/distribution/) (if not already present on your system)
         
         2. In a command prompt type:
```

### Comparing `epyseg-0.1.8/epyseg.egg-info/SOURCES.txt` & `epyseg-0.1.9/epyseg.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `epyseg-0.1.8/setup.py` & `epyseg-0.1.9/setup.py`

 * *Files identical despite different names*

