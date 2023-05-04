# Comparing `tmp/mxproc-2023.5.0.tar.gz` & `tmp/mxproc-2023.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mxproc-2023.5.0.tar", last modified: Wed May  3 16:39:58 2023, max compression
+gzip compressed data, was "mxproc-2023.5.1.tar", last modified: Thu May  4 20:20:57 2023, max compression
```

## Comparing `mxproc-2023.5.0.tar` & `mxproc-2023.5.1.tar`

### file list

```diff
@@ -1,80 +1,80 @@
-drwxr-xr-x   0 michel   (70005) michel   (70005)        0 2023-05-03 16:39:58.843596 mxproc-2023.5.0/
--rw-r--r--   0 michel   (70005) michel   (70005)     1830 2023-04-07 16:35:59.000000 mxproc-2023.5.0/.gitignore
-drwxr-xr-x   0 michel   (70005) michel   (70005)        0 2023-05-03 16:39:58.832596 mxproc-2023.5.0/.idea/
--rw-r--r--   0 michel   (70005) michel   (70005)      176 2023-01-05 16:54:49.000000 mxproc-2023.5.0/.idea/.gitignore
-drwxr-xr-x   0 michel   (70005) michel   (70005)        0 2023-05-03 16:39:58.832596 mxproc-2023.5.0/.idea/inspectionProfiles/
--rw-r--r--   0 michel   (70005) michel   (70005)      174 2023-01-05 17:07:44.000000 mxproc-2023.5.0/.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0 michel   (70005) michel   (70005)      300 2023-01-05 17:07:44.000000 mxproc-2023.5.0/.idea/misc.xml
--rw-r--r--   0 michel   (70005) michel   (70005)      264 2023-01-05 17:07:44.000000 mxproc-2023.5.0/.idea/modules.xml
--rw-r--r--   0 michel   (70005) michel   (70005)      518 2023-03-14 15:28:26.000000 mxproc-2023.5.0/.idea/mxproc.iml
--rw-r--r--   0 michel   (70005) michel   (70005)      176 2023-03-14 15:31:15.000000 mxproc-2023.5.0/.idea/other.xml
--rw-r--r--   0 michel   (70005) michel   (70005)      167 2023-01-05 17:07:44.000000 mxproc-2023.5.0/.idea/vcs.xml
--rw-r--r--   0 michel   (70005) michel   (70005)      200 2023-04-28 19:44:58.000000 mxproc-2023.5.0/.idea/watcherTasks.xml
--rw-r--r--   0 michel   (70005) michel   (70005)     1066 2023-01-05 16:53:41.000000 mxproc-2023.5.0/LICENSE
--rw-r--r--   0 michel   (70005) michel   (70005)      864 2023-05-03 16:39:58.843596 mxproc-2023.5.0/PKG-INFO
--rw-r--r--   0 michel   (70005) michel   (70005)      281 2023-01-05 16:53:41.000000 mxproc-2023.5.0/README.md
-drwxr-xr-x   0 michel   (70005) michel   (70005)        0 2023-05-03 16:39:58.832596 mxproc-2023.5.0/bin/
--rwxr-xr-x   0 michel   (70005) michel   (70005)      230 2023-05-01 14:55:13.000000 mxproc-2023.5.0/bin/auto.index
--rwxr-xr-x   0 michel   (70005) michel   (70005)      249 2023-05-01 14:54:07.000000 mxproc-2023.5.0/bin/auto.init
--rwxr-xr-x   0 michel   (70005) michel   (70005)      235 2023-05-01 14:53:57.000000 mxproc-2023.5.0/bin/auto.integrate
--rwxr-xr-x   0 michel   (70005) michel   (70005)      188 2023-05-01 14:53:32.000000 mxproc-2023.5.0/bin/auto.process
--rwxr-xr-x   0 michel   (70005) michel   (70005)      227 2023-05-01 14:53:32.000000 mxproc-2023.5.0/bin/auto.scale
--rwxr-xr-x   0 michel   (70005) michel   (70005)      230 2023-05-01 14:52:50.000000 mxproc-2023.5.0/bin/auto.spots
--rwxr-xr-x   0 michel   (70005) michel   (70005)      245 2023-05-01 14:52:50.000000 mxproc-2023.5.0/bin/auto.strategy
--rwxr-xr-x   0 michel   (70005) michel   (70005)      244 2023-05-01 14:52:50.000000 mxproc-2023.5.0/bin/auto.symmetry
-drwxr-xr-x   0 michel   (70005) michel   (70005)        0 2023-05-03 16:39:58.832596 mxproc-2023.5.0/mxproc/
--rw-r--r--   0 michel   (70005) michel   (70005)    17199 2023-05-02 15:59:52.000000 mxproc-2023.5.0/mxproc/__init__.py
--rw-r--r--   0 michel   (70005) michel   (70005)     3752 2023-05-01 14:29:49.000000 mxproc-2023.5.0/mxproc/command.py
--rw-r--r--   0 michel   (70005) michel   (70005)    11936 2023-04-28 18:30:27.000000 mxproc-2023.5.0/mxproc/common.py
-drwxr-xr-x   0 michel   (70005) michel   (70005)        0 2023-05-03 16:39:58.833596 mxproc-2023.5.0/mxproc/engines/
--rw-r--r--   0 michel   (70005) michel   (70005)        3 2023-01-06 16:23:54.000000 mxproc-2023.5.0/mxproc/engines/__init__.py
-drwxr-xr-x   0 michel   (70005) michel   (70005)        0 2023-05-03 16:39:58.833596 mxproc-2023.5.0/mxproc/engines/dials/
--rw-r--r--   0 michel   (70005) michel   (70005)     2417 2023-03-29 19:51:55.000000 mxproc-2023.5.0/mxproc/engines/dials/__init__.py
-drwxr-xr-x   0 michel   (70005) michel   (70005)        0 2023-05-03 16:39:58.833596 mxproc-2023.5.0/mxproc/engines/dials/data/
--rw-r--r--   0 michel   (70005) michel   (70005)      403 2023-03-02 17:15:40.000000 mxproc-2023.5.0/mxproc/engines/dials/data/spots.yml
--rw-r--r--   0 michel   (70005) michel   (70005)      325 2023-03-03 18:52:44.000000 mxproc-2023.5.0/mxproc/engines/dials/parser.py
-drwxr-xr-x   0 michel   (70005) michel   (70005)        0 2023-05-03 16:39:58.833596 mxproc-2023.5.0/mxproc/engines/xds/
--rw-r--r--   0 michel   (70005) michel   (70005)    41164 2023-05-01 19:11:31.000000 mxproc-2023.5.0/mxproc/engines/xds/__init__.py
--rw-r--r--   0 michel   (70005) michel   (70005)     1491 2023-04-03 14:59:31.000000 mxproc-2023.5.0/mxproc/engines/xds/indexing.py
--rw-r--r--   0 michel   (70005) michel   (70005)    13830 2023-04-27 21:26:24.000000 mxproc-2023.5.0/mxproc/engines/xds/io.py
-drwxr-xr-x   0 michel   (70005) michel   (70005)        0 2023-05-03 16:39:58.842596 mxproc-2023.5.0/mxproc/engines/xds/parser/
--rw-r--r--   0 michel   (70005) michel   (70005)    11448 2023-05-01 13:53:04.000000 mxproc-2023.5.0/mxproc/engines/xds/parser/__init__.py
-drwxr-xr-x   0 michel   (70005) michel   (70005)        0 2023-05-03 16:39:58.842596 mxproc-2023.5.0/mxproc/engines/xds/parser/data/
--rw-r--r--   0 michel   (70005) michel   (70005)     2970 2023-04-03 20:40:43.000000 mxproc-2023.5.0/mxproc/engines/xds/parser/data/correct.yml
--rw-r--r--   0 michel   (70005) michel   (70005)     2516 2023-03-30 18:23:30.000000 mxproc-2023.5.0/mxproc/engines/xds/parser/data/idxref.yml
--rw-r--r--   0 michel   (70005) michel   (70005)     1530 2023-04-27 20:54:18.000000 mxproc-2023.5.0/mxproc/engines/xds/parser/data/integrate.yml
--rw-r--r--   0 michel   (70005) michel   (70005)      402 2023-03-02 17:15:13.000000 mxproc-2023.5.0/mxproc/engines/xds/parser/data/spots.yml
--rw-r--r--   0 michel   (70005) michel   (70005)      441 2020-04-23 23:03:01.000000 mxproc-2023.5.0/mxproc/engines/xds/parser/data/xdsstat.yml
--rw-r--r--   0 michel   (70005) michel   (70005)     1001 2023-03-30 19:14:20.000000 mxproc-2023.5.0/mxproc/engines/xds/parser/data/xparm.yml
--rw-r--r--   0 michel   (70005) michel   (70005)      587 2023-04-02 17:48:26.000000 mxproc-2023.5.0/mxproc/engines/xds/parser/data/xplan.yml
--rw-r--r--   0 michel   (70005) michel   (70005)     1828 2023-03-24 18:58:42.000000 mxproc-2023.5.0/mxproc/engines/xds/parser/data/xscale.yml
--rw-r--r--   0 michel   (70005) michel   (70005)     1080 2023-03-23 15:22:44.000000 mxproc-2023.5.0/mxproc/engines/xds/parser/data/xtriage.yml
--rw-r--r--   0 michel   (70005) michel   (70005)     3133 2023-04-01 20:58:37.000000 mxproc-2023.5.0/mxproc/engines/xds/parser/pointless.py
--rw-r--r--   0 michel   (70005) michel   (70005)     1603 2023-03-31 21:44:47.000000 mxproc-2023.5.0/mxproc/engines/xds/stats.py
--rw-r--r--   0 michel   (70005) michel   (70005)     5901 2023-05-01 14:11:46.000000 mxproc-2023.5.0/mxproc/log.py
-drwxr-xr-x   0 michel   (70005) michel   (70005)        0 2023-05-03 16:39:58.843596 mxproc-2023.5.0/mxproc/programs/
--rw-r--r--   0 michel   (70005) michel   (70005)        0 2023-04-01 20:59:20.000000 mxproc-2023.5.0/mxproc/programs/__init__.py
--rw-r--r--   0 michel   (70005) michel   (70005)     3471 2023-05-01 18:49:21.000000 mxproc-2023.5.0/mxproc/programs/raddose.py
-drwxr-xr-x   0 michel   (70005) michel   (70005)        0 2023-05-03 16:39:58.843596 mxproc-2023.5.0/mxproc/reporting/
--rw-r--r--   0 michel   (70005) michel   (70005)     3705 2023-04-28 18:40:37.000000 mxproc-2023.5.0/mxproc/reporting/__init__.py
-drwxr-xr-x   0 michel   (70005) michel   (70005)        0 2023-05-03 16:39:58.843596 mxproc-2023.5.0/mxproc/reporting/data/
--rw-r--r--   0 michel   (70005) michel   (70005)     3131 2023-04-28 20:21:36.000000 mxproc-2023.5.0/mxproc/reporting/data/report.html
--rw-r--r--   0 michel   (70005) michel   (70005)    24042 2020-04-23 23:03:01.000000 mxproc-2023.5.0/mxproc/reporting/data/report.js
--rw-r--r--   0 michel   (70005) michel   (70005)     2674 2023-04-28 20:41:26.000000 mxproc-2023.5.0/mxproc/reporting/data/report.min.css
--rw-r--r--   0 michel   (70005) michel   (70005)    12431 2023-04-03 17:07:52.000000 mxproc-2023.5.0/mxproc/reporting/data/report.min.js
--rw-r--r--   0 michel   (70005) michel   (70005)     2565 2023-04-28 20:41:26.000000 mxproc-2023.5.0/mxproc/reporting/data/report.scss
--rw-r--r--   0 michel   (70005) michel   (70005)    18850 2023-04-28 20:26:22.000000 mxproc-2023.5.0/mxproc/reporting/generic.py
--rw-r--r--   0 michel   (70005) michel   (70005)     6295 2023-05-01 19:53:17.000000 mxproc-2023.5.0/mxproc/reporting/screening.py
--rw-r--r--   0 michel   (70005) michel   (70005)     3634 2023-04-28 16:55:38.000000 mxproc-2023.5.0/mxproc/reporting/text.py
--rw-r--r--   0 michel   (70005) michel   (70005)    11901 2023-04-26 23:08:21.000000 mxproc-2023.5.0/mxproc/xtal.py
-drwxr-xr-x   0 michel   (70005) michel   (70005)        0 2023-05-03 16:39:58.833596 mxproc-2023.5.0/mxproc.egg-info/
--rw-r--r--   0 michel   (70005) michel   (70005)      864 2023-05-03 16:39:58.000000 mxproc-2023.5.0/mxproc.egg-info/PKG-INFO
--rw-r--r--   0 michel   (70005) michel   (70005)     1650 2023-05-03 16:39:58.000000 mxproc-2023.5.0/mxproc.egg-info/SOURCES.txt
--rw-r--r--   0 michel   (70005) michel   (70005)        1 2023-05-03 16:39:58.000000 mxproc-2023.5.0/mxproc.egg-info/dependency_links.txt
--rw-r--r--   0 michel   (70005) michel   (70005)       62 2023-05-03 16:39:58.000000 mxproc-2023.5.0/mxproc.egg-info/requires.txt
--rw-r--r--   0 michel   (70005) michel   (70005)        7 2023-05-03 16:39:58.000000 mxproc-2023.5.0/mxproc.egg-info/top_level.txt
--rw-r--r--   0 michel   (70005) michel   (70005)     1071 2023-04-28 21:29:32.000000 mxproc-2023.5.0/pyproject.toml
--rw-r--r--   0 michel   (70005) michel   (70005)       38 2023-05-03 16:39:58.843596 mxproc-2023.5.0/setup.cfg
-drwxr-xr-x   0 michel   (70005) michel   (70005)        0 2023-05-03 16:39:58.843596 mxproc-2023.5.0/test/
--rw-r--r--   0 michel   (70005) michel   (70005)        0 2023-04-03 15:56:13.000000 mxproc-2023.5.0/test/__init__.py
--rw-r--r--   0 michel   (70005) michel   (70005)     2303 2023-04-03 16:27:52.000000 mxproc-2023.5.0/test/test_common.py
+drwxr-xr-x   0 michel   (70005) michel   (70005)        0 2023-05-04 20:20:57.227202 mxproc-2023.5.1/
+-rw-r--r--   0 michel   (70005) michel   (70005)     1830 2023-04-07 16:35:59.000000 mxproc-2023.5.1/.gitignore
+drwxr-xr-x   0 michel   (70005) michel   (70005)        0 2023-05-04 20:20:57.225202 mxproc-2023.5.1/.idea/
+-rw-r--r--   0 michel   (70005) michel   (70005)      176 2023-01-05 16:54:49.000000 mxproc-2023.5.1/.idea/.gitignore
+drwxr-xr-x   0 michel   (70005) michel   (70005)        0 2023-05-04 20:20:57.225202 mxproc-2023.5.1/.idea/inspectionProfiles/
+-rw-r--r--   0 michel   (70005) michel   (70005)      174 2023-01-05 17:07:44.000000 mxproc-2023.5.1/.idea/inspectionProfiles/profiles_settings.xml
+-rw-r--r--   0 michel   (70005) michel   (70005)      300 2023-01-05 17:07:44.000000 mxproc-2023.5.1/.idea/misc.xml
+-rw-r--r--   0 michel   (70005) michel   (70005)      264 2023-01-05 17:07:44.000000 mxproc-2023.5.1/.idea/modules.xml
+-rw-r--r--   0 michel   (70005) michel   (70005)      518 2023-03-14 15:28:26.000000 mxproc-2023.5.1/.idea/mxproc.iml
+-rw-r--r--   0 michel   (70005) michel   (70005)      176 2023-03-14 15:31:15.000000 mxproc-2023.5.1/.idea/other.xml
+-rw-r--r--   0 michel   (70005) michel   (70005)      167 2023-01-05 17:07:44.000000 mxproc-2023.5.1/.idea/vcs.xml
+-rw-r--r--   0 michel   (70005) michel   (70005)      200 2023-04-28 19:44:58.000000 mxproc-2023.5.1/.idea/watcherTasks.xml
+-rw-r--r--   0 michel   (70005) michel   (70005)     1066 2023-01-05 16:53:41.000000 mxproc-2023.5.1/LICENSE
+-rw-r--r--   0 michel   (70005) michel   (70005)      864 2023-05-04 20:20:57.227202 mxproc-2023.5.1/PKG-INFO
+-rw-r--r--   0 michel   (70005) michel   (70005)      281 2023-01-05 16:53:41.000000 mxproc-2023.5.1/README.md
+drwxr-xr-x   0 michel   (70005) michel   (70005)        0 2023-05-04 20:20:57.225202 mxproc-2023.5.1/bin/
+-rwxr-xr-x   0 michel   (70005) michel   (70005)      230 2023-05-01 14:55:13.000000 mxproc-2023.5.1/bin/auto.index
+-rwxr-xr-x   0 michel   (70005) michel   (70005)      249 2023-05-01 14:54:07.000000 mxproc-2023.5.1/bin/auto.init
+-rwxr-xr-x   0 michel   (70005) michel   (70005)      235 2023-05-01 14:53:57.000000 mxproc-2023.5.1/bin/auto.integrate
+-rwxr-xr-x   0 michel   (70005) michel   (70005)      188 2023-05-01 14:53:32.000000 mxproc-2023.5.1/bin/auto.process
+-rwxr-xr-x   0 michel   (70005) michel   (70005)      227 2023-05-01 14:53:32.000000 mxproc-2023.5.1/bin/auto.scale
+-rwxr-xr-x   0 michel   (70005) michel   (70005)      230 2023-05-01 14:52:50.000000 mxproc-2023.5.1/bin/auto.spots
+-rwxr-xr-x   0 michel   (70005) michel   (70005)      245 2023-05-01 14:52:50.000000 mxproc-2023.5.1/bin/auto.strategy
+-rwxr-xr-x   0 michel   (70005) michel   (70005)      244 2023-05-01 14:52:50.000000 mxproc-2023.5.1/bin/auto.symmetry
+drwxr-xr-x   0 michel   (70005) michel   (70005)        0 2023-05-04 20:20:57.225202 mxproc-2023.5.1/mxproc/
+-rw-r--r--   0 michel   (70005) michel   (70005)    17226 2023-05-04 15:53:34.000000 mxproc-2023.5.1/mxproc/__init__.py
+-rw-r--r--   0 michel   (70005) michel   (70005)     3752 2023-05-01 14:29:49.000000 mxproc-2023.5.1/mxproc/command.py
+-rw-r--r--   0 michel   (70005) michel   (70005)    11915 2023-05-04 15:09:21.000000 mxproc-2023.5.1/mxproc/common.py
+drwxr-xr-x   0 michel   (70005) michel   (70005)        0 2023-05-04 20:20:57.226202 mxproc-2023.5.1/mxproc/engines/
+-rw-r--r--   0 michel   (70005) michel   (70005)        3 2023-01-06 16:23:54.000000 mxproc-2023.5.1/mxproc/engines/__init__.py
+drwxr-xr-x   0 michel   (70005) michel   (70005)        0 2023-05-04 20:20:57.226202 mxproc-2023.5.1/mxproc/engines/dials/
+-rw-r--r--   0 michel   (70005) michel   (70005)     2417 2023-03-29 19:51:55.000000 mxproc-2023.5.1/mxproc/engines/dials/__init__.py
+drwxr-xr-x   0 michel   (70005) michel   (70005)        0 2023-05-04 20:20:57.226202 mxproc-2023.5.1/mxproc/engines/dials/data/
+-rw-r--r--   0 michel   (70005) michel   (70005)      403 2023-03-02 17:15:40.000000 mxproc-2023.5.1/mxproc/engines/dials/data/spots.yml
+-rw-r--r--   0 michel   (70005) michel   (70005)      325 2023-03-03 18:52:44.000000 mxproc-2023.5.1/mxproc/engines/dials/parser.py
+drwxr-xr-x   0 michel   (70005) michel   (70005)        0 2023-05-04 20:20:57.226202 mxproc-2023.5.1/mxproc/engines/xds/
+-rw-r--r--   0 michel   (70005) michel   (70005)    40710 2023-05-04 16:29:40.000000 mxproc-2023.5.1/mxproc/engines/xds/__init__.py
+-rw-r--r--   0 michel   (70005) michel   (70005)     1504 2023-05-04 16:33:01.000000 mxproc-2023.5.1/mxproc/engines/xds/indexing.py
+-rw-r--r--   0 michel   (70005) michel   (70005)    13827 2023-05-04 15:19:52.000000 mxproc-2023.5.1/mxproc/engines/xds/io.py
+drwxr-xr-x   0 michel   (70005) michel   (70005)        0 2023-05-04 20:20:57.226202 mxproc-2023.5.1/mxproc/engines/xds/parser/
+-rw-r--r--   0 michel   (70005) michel   (70005)    11448 2023-05-01 13:53:04.000000 mxproc-2023.5.1/mxproc/engines/xds/parser/__init__.py
+drwxr-xr-x   0 michel   (70005) michel   (70005)        0 2023-05-04 20:20:57.227202 mxproc-2023.5.1/mxproc/engines/xds/parser/data/
+-rw-r--r--   0 michel   (70005) michel   (70005)     2970 2023-04-03 20:40:43.000000 mxproc-2023.5.1/mxproc/engines/xds/parser/data/correct.yml
+-rw-r--r--   0 michel   (70005) michel   (70005)     2516 2023-03-30 18:23:30.000000 mxproc-2023.5.1/mxproc/engines/xds/parser/data/idxref.yml
+-rw-r--r--   0 michel   (70005) michel   (70005)     1530 2023-04-27 20:54:18.000000 mxproc-2023.5.1/mxproc/engines/xds/parser/data/integrate.yml
+-rw-r--r--   0 michel   (70005) michel   (70005)      402 2023-03-02 17:15:13.000000 mxproc-2023.5.1/mxproc/engines/xds/parser/data/spots.yml
+-rw-r--r--   0 michel   (70005) michel   (70005)      441 2020-04-23 23:03:01.000000 mxproc-2023.5.1/mxproc/engines/xds/parser/data/xdsstat.yml
+-rw-r--r--   0 michel   (70005) michel   (70005)     1001 2023-03-30 19:14:20.000000 mxproc-2023.5.1/mxproc/engines/xds/parser/data/xparm.yml
+-rw-r--r--   0 michel   (70005) michel   (70005)      587 2023-04-02 17:48:26.000000 mxproc-2023.5.1/mxproc/engines/xds/parser/data/xplan.yml
+-rw-r--r--   0 michel   (70005) michel   (70005)     1828 2023-03-24 18:58:42.000000 mxproc-2023.5.1/mxproc/engines/xds/parser/data/xscale.yml
+-rw-r--r--   0 michel   (70005) michel   (70005)     1080 2023-03-23 15:22:44.000000 mxproc-2023.5.1/mxproc/engines/xds/parser/data/xtriage.yml
+-rw-r--r--   0 michel   (70005) michel   (70005)     3142 2023-05-04 15:59:28.000000 mxproc-2023.5.1/mxproc/engines/xds/parser/pointless.py
+-rw-r--r--   0 michel   (70005) michel   (70005)     1603 2023-03-31 21:44:47.000000 mxproc-2023.5.1/mxproc/engines/xds/stats.py
+-rw-r--r--   0 michel   (70005) michel   (70005)     5901 2023-05-01 14:11:46.000000 mxproc-2023.5.1/mxproc/log.py
+drwxr-xr-x   0 michel   (70005) michel   (70005)        0 2023-05-04 20:20:57.227202 mxproc-2023.5.1/mxproc/programs/
+-rw-r--r--   0 michel   (70005) michel   (70005)        0 2023-04-01 20:59:20.000000 mxproc-2023.5.1/mxproc/programs/__init__.py
+-rw-r--r--   0 michel   (70005) michel   (70005)     3471 2023-05-01 18:49:21.000000 mxproc-2023.5.1/mxproc/programs/raddose.py
+drwxr-xr-x   0 michel   (70005) michel   (70005)        0 2023-05-04 20:20:57.227202 mxproc-2023.5.1/mxproc/reporting/
+-rw-r--r--   0 michel   (70005) michel   (70005)     3705 2023-04-28 18:40:37.000000 mxproc-2023.5.1/mxproc/reporting/__init__.py
+drwxr-xr-x   0 michel   (70005) michel   (70005)        0 2023-05-04 20:20:57.227202 mxproc-2023.5.1/mxproc/reporting/data/
+-rw-r--r--   0 michel   (70005) michel   (70005)     3131 2023-04-28 20:21:36.000000 mxproc-2023.5.1/mxproc/reporting/data/report.html
+-rw-r--r--   0 michel   (70005) michel   (70005)    24042 2020-04-23 23:03:01.000000 mxproc-2023.5.1/mxproc/reporting/data/report.js
+-rw-r--r--   0 michel   (70005) michel   (70005)     2674 2023-04-28 20:41:26.000000 mxproc-2023.5.1/mxproc/reporting/data/report.min.css
+-rw-r--r--   0 michel   (70005) michel   (70005)    12431 2023-04-03 17:07:52.000000 mxproc-2023.5.1/mxproc/reporting/data/report.min.js
+-rw-r--r--   0 michel   (70005) michel   (70005)     2565 2023-04-28 20:41:26.000000 mxproc-2023.5.1/mxproc/reporting/data/report.scss
+-rw-r--r--   0 michel   (70005) michel   (70005)    18850 2023-04-28 20:26:22.000000 mxproc-2023.5.1/mxproc/reporting/generic.py
+-rw-r--r--   0 michel   (70005) michel   (70005)     6295 2023-05-01 19:53:17.000000 mxproc-2023.5.1/mxproc/reporting/screening.py
+-rw-r--r--   0 michel   (70005) michel   (70005)     3634 2023-04-28 16:55:38.000000 mxproc-2023.5.1/mxproc/reporting/text.py
+-rw-r--r--   0 michel   (70005) michel   (70005)    11646 2023-05-04 15:26:22.000000 mxproc-2023.5.1/mxproc/xtal.py
+drwxr-xr-x   0 michel   (70005) michel   (70005)        0 2023-05-04 20:20:57.226202 mxproc-2023.5.1/mxproc.egg-info/
+-rw-r--r--   0 michel   (70005) michel   (70005)      864 2023-05-04 20:20:57.000000 mxproc-2023.5.1/mxproc.egg-info/PKG-INFO
+-rw-r--r--   0 michel   (70005) michel   (70005)     1650 2023-05-04 20:20:57.000000 mxproc-2023.5.1/mxproc.egg-info/SOURCES.txt
+-rw-r--r--   0 michel   (70005) michel   (70005)        1 2023-05-04 20:20:57.000000 mxproc-2023.5.1/mxproc.egg-info/dependency_links.txt
+-rw-r--r--   0 michel   (70005) michel   (70005)       62 2023-05-04 20:20:57.000000 mxproc-2023.5.1/mxproc.egg-info/requires.txt
+-rw-r--r--   0 michel   (70005) michel   (70005)        7 2023-05-04 20:20:57.000000 mxproc-2023.5.1/mxproc.egg-info/top_level.txt
+-rw-r--r--   0 michel   (70005) michel   (70005)     1071 2023-04-28 21:29:32.000000 mxproc-2023.5.1/pyproject.toml
+-rw-r--r--   0 michel   (70005) michel   (70005)       38 2023-05-04 20:20:57.227202 mxproc-2023.5.1/setup.cfg
+drwxr-xr-x   0 michel   (70005) michel   (70005)        0 2023-05-04 20:20:57.227202 mxproc-2023.5.1/test/
+-rw-r--r--   0 michel   (70005) michel   (70005)        0 2023-04-03 15:56:13.000000 mxproc-2023.5.1/test/__init__.py
+-rw-r--r--   0 michel   (70005) michel   (70005)     2303 2023-04-03 16:27:52.000000 mxproc-2023.5.1/test/test_common.py
```

### Comparing `mxproc-2023.5.0/.gitignore` & `mxproc-2023.5.1/.gitignore`

 * *Files identical despite different names*

### Comparing `mxproc-2023.5.0/.idea/mxproc.iml` & `mxproc-2023.5.1/.idea/mxproc.iml`

 * *Files identical despite different names*

### Comparing `mxproc-2023.5.0/LICENSE` & `mxproc-2023.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `mxproc-2023.5.0/PKG-INFO` & `mxproc-2023.5.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mxproc
-Version: 2023.5.0
+Version: 2023.5.1
 Summary: MX Automated Data Processing Pipeline
 Author-email: Michel Fodje <michel4j@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/michel4j/mxproc
 Keywords: Data Processing Pipeline,MX,AutoProcess
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `mxproc-2023.5.0/mxproc/__init__.py` & `mxproc-2023.5.1/mxproc/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -92,26 +92,28 @@
     def __init__(self, args: argparse.Namespace):
         """
         Data analysis objects
         :param args: arguments parsed from command line
         """
 
         self.args = args
-
+        self.experiments = ()
         # Prepare working directory
         directory = self.args.dir
-        if directory in ["", None]:
+        if directory in ["", None] and args.images:
             index = 1
             directory = Path(f"{self.prefix}-{index}")
             while directory.exists():
                 index += 1
                 directory = Path(f"{self.prefix}-{index}")
+            self.experiments = load_multiple(self.args.images)
+        elif directory is None:
+            directory = ""
         directory = Path(directory).absolute()
 
-        self.experiments = load_multiple(self.args.images)
         self.options = AnalysisOptions(
             directory=directory, extras=self.get_extras(self.args), **self.get_options(self.args)
         )
 
         if not directory.exists():
             directory.mkdir(parents=True, exist_ok=True)
         log.log_to_file(str(directory / "auto.log"))
@@ -157,20 +159,24 @@
             'multi': len(self.experiments) > 1 and args.multi,
             'beam_flux': args.beam_flux,
             'beam_fwhm': args.beam_fwhm,
             'beam_size': args.beam_size,
         }
         return {key: value for key, value in options.items() if value}
 
-    def load(self, step: StepType):
+    def load(self, step: StepType | None = None):
         """
         Load an Analysis from a meta file and reset the state to it.
-        :param step: analysis step corresponding to the saved metadata
+        :param step: analysis step corresponding to the saved metadata reads the latest meta file if None
         """
-        meta_file = self.options.directory / f'{step.slug()}.meta'
+
+        realm = 'latest' if step is None else step.slug()
+
+        meta_file = self.options.directory / f'{realm}.meta'
+
         try:
             with gzip.open(meta_file, 'rb') as handle:  # gzip compressed yaml file
                 meta = yaml.load(handle, yaml.Loader)
 
             self.options = meta['options']
             self.experiments = meta['experiments']
             self.results = meta['results']
@@ -194,21 +200,26 @@
         meta = {
             'options': self.options,
             'experiments': self.experiments,
             'results': self.results,
             'settings': self.settings
         }
         meta_file = self.options.directory / f'{step.slug()}.meta'
+        latest_file = self.options.directory / 'latest.meta'
 
         # backup file if needed
         if meta_file.exists() and backup:
             meta_file.rename(f"{str(meta_file)}.bk")
 
         with gzip.open(meta_file, 'wb') as handle:  # gzip compressed yaml file
             yaml.dump(meta, handle, encoding='utf-8')
+        try:
+            latest_file.unlink(missing_ok=True)
+        finally:
+            latest_file.hardlink_to(meta_file)
 
     def update_result(self, results: Dict[str, Result], step: StepType):
         """
         Update the results dictionary and save a checkpoint meta file
 
         :param results: dictionary of results keyed by the experiment identifier
         :param step: AnalysisStep
@@ -254,22 +265,14 @@
         :param step: AnalysisStep to run
         :return: valid python exit code, 0 = success, 1 = error, etc
         """
 
         exit_code = 0
         # If anything other than initialize, load the previous metadata and use that
         if step != StepType.INITIALIZE:
-            # Find bootstrap step based on active workflow
-            if bootstrap is None:
-                for prev_step, next_step in WORKFLOWS[self.workflow].items():
-                    if next_step == step:
-                        bootstrap = prev_step
-                        break
-                else:
-                    bootstrap = step.prev()
             self.load(bootstrap)
 
         start_time = time.time()
         header = f'MX Auto Proces (version: {__version__})'
         sub_header = f"{datetime.now().isoformat()} {self.workflow.desc()} [{len(self.experiments):d} dataset(s)]"
         logger.banner(header)
         logger.banner(sub_header, overline=False, line='-')
@@ -280,15 +283,15 @@
                 os.chdir(self.options.directory)
 
             step_method = self.methods.get(step)
             try:
                 logger.info_value(step.desc(), '', spacer='-')
                 results = step_method()
             except CommandFailed as err:
-                logger.error(f'Data Processing Failed at {step.name}: {err}. Aborting!')
+                logger.error(f'Failed at {step.name}: {err}. Aborting!')
                 exit_code = 1
                 break
             else:
                 # REPORTING step does not have results
                 if step != StepType.REPORT and results:
                     self.update_result(results, step)
```

### Comparing `mxproc-2023.5.0/mxproc/command.py` & `mxproc-2023.5.1/mxproc/command.py`

 * *Files identical despite different names*

### Comparing `mxproc-2023.5.0/mxproc/common.py` & `mxproc-2023.5.1/mxproc/common.py`

 * *Files 1% similar despite different names*

```diff
@@ -396,23 +396,26 @@
     :return: text summary for example, "1-10,16,18,25-26"
     """
     return ','.join([
         f'{p[0]}-{p[1]-1}' if p[1] > p[0] + 1 else f'{p[0]}' for p in series
     ])
 
 
+### FIXME: replace with itertools.pairwise eventually
+def pairwise(iterable):
+    # pairwise('ABCDEFG') --> AB BC CD DE EF FG
+    a, b = tee(iterable)
+    next(b, None)
+    return zip(a, b)
+
+
 def find_missing(series: Sequence[Tuple[int, int]]) -> Sequence[Tuple[int, int]]:
     """
     Takes the output of parse_ranges and returns another sequence of tuples representing inverse of the range
     specification.
 
     :param series: Sequence of tuples, e.g.  [(1, 11), (16, 17), (18, 19), (25, 27)]
     :return: Another sequence of tuples, for the above example, it would be [(11, 16), (17, 18), (19, 25)]
     """
-    ### FIXME: replace with itertools.pairwise eventually
-    def pairwise(iterable):
-        # pairwise('ABCDEFG') --> AB BC CD DE EF FG
-        a, b = tee(iterable)
-        next(b, None)
-        return zip(a, b)
+
 
     return [(a[1], b[0]) for a, b in pairwise(series)]
```

### Comparing `mxproc-2023.5.0/mxproc/engines/dials/__init__.py` & `mxproc-2023.5.1/mxproc/engines/dials/__init__.py`

 * *Files identical despite different names*

### Comparing `mxproc-2023.5.0/mxproc/engines/xds/__init__.py` & `mxproc-2023.5.1/mxproc/engines/xds/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -38,23 +38,22 @@
     degrees: dict  # parameter degrees
     params: dict  # previous parameters
     min_sigma: float  # Maximum Spot Sigma Value
     max_sigma: float  # Minimum Spot Sigma Value
 
     def __init__(
             self,
-            data_range: Tuple[int, int],
+            data_range: Sequence[Tuple[int, int]],
             spot_range: Sequence[Tuple[int, int]],
-            skip_range: Sequence[Tuple[int, int]],
             min_sigma: float = DEFAULT_MIN_SIGMA,
             max_sigma: float = 100,
             **extras
     ):
         self.degrees = {}
-        self.params = {'spot_range': spot_range, "data_range": data_range, 'skip_range': skip_range, **extras}
+        self.params = {'spot_range': spot_range, "data_range": data_range, **extras}
         self.min_sigma = min_sigma
         self.max_sigma = max_sigma
 
     def get_degree(self, name: str) -> int:
         """
         Update the degree and return its count
         :param name: name of parameter
@@ -123,19 +122,15 @@
 
 class XDSAnalysis(Analysis):
     prefix = 'xds'
 
     def get_extras(self, args: argparse.Namespace) -> dict:
         extras = {}
         if args.frames:
-            extras.update(
-                data_range=(args.frames[0][0], args.frames[-1][1]),
-                skip_range=find_missing(args.frames),
-                spot_range=args.frames,
-            )
+            extras.update(data_range=args.frames, spot_range=args.frames)
 
         if args.beam_center:
             extras.update(beam_center=XYPair(*args.beam_center))
 
         if args.anom is not None:
             extras.update(anomalous=args.anom)
 
@@ -160,31 +155,31 @@
             # create sub-directories if multiple processing
             directory = self.options.directory
             directory = directory if len(self.experiments) == 1 else directory / experiment.name
             directory.mkdir(parents=True, exist_ok=True)
             self.options.working_directories[experiment.identifier] = directory
             os.chdir(self.options.working_directories[experiment.identifier])
             io_options = {
-                'data_range': (experiment.frames[0][0], experiment.frames[-1][1]), 'spot_range': experiment.frames,
-                'skip_range': experiment.missing, 'beam_center': experiment.detector_origin
+                'data_range': experiment.frames, 'spot_range': experiment.frames,
+                'beam_center': experiment.detector_origin
             }
             io_options.update(self.options.extras)
             io.create_input_file(('ALL',), experiment, io.XDSParameters(**io_options))
             path_str = str(directory)
             path_str = path_str.replace(os.path.expanduser('~'), '~', 1)
             logger.info_value(f'{experiment.name}', path_str)
             results[experiment.identifier] = Result(state=StateType.SUCCESS, details={"directory": directory})
         return results
 
     def find_spots(self, **kwargs):
         results = {}
         for experiment in self.experiments:
             io_options = {
-                'data_range': (experiment.frames[0][0], experiment.frames[-1][1]), 'spot_range': experiment.frames,
-                'skip_range': experiment.missing, 'beam_center': experiment.detector_origin
+                'data_range': experiment.frames, 'spot_range': experiment.frames,
+                'beam_center': experiment.detector_origin
             }
             io_options.update(self.options.extras)
             os.chdir(self.options.working_directories[experiment.identifier])
             io.create_input_file(('XYCORR', 'INIT', 'COLSPOT'), experiment, io.XDSParameters(**io_options))
             image_range = summarize_ranges(io_options['spot_range'])
 
             try:
@@ -205,20 +200,24 @@
                 continue
 
             os.chdir(self.options.working_directories[experiment.identifier])
 
             result = generate_failure('')
             logger.info(f'{experiment.name}:')
             io_options = {
-                'data_range': (experiment.frames[0][0], experiment.frames[-1][1]),
-                'spot_range': experiment.frames, 'skip_range': experiment.missing,
-                'anomalous': self.options.anomalous, 'beam_center': experiment.detector_origin
+                'data_range': experiment.frames,
+                'spot_range': experiment.frames,
+                'anomalous': self.options.anomalous,
+                'beam_center': experiment.detector_origin
             }
             io_options.update(**self.options.extras)
 
+            # ignore lattice
+            io_options.pop('lattice', None)
+
             param_manager = IndexParamManager(**io_options)
             for trial_number in range(MAX_INDEX_TRIES):
                 backup_files('IDXREF.LP')
                 result, retry_requested, retry_messages = autoindex_trial(experiment, param_manager, trial_number)
                 if retry_requested:
                     show_warnings(f'Retrying Indexing:', retry_messages)
                 else:
@@ -243,16 +242,16 @@
         results = {}
         for experiment in self.experiments:
             os.chdir(self.options.working_directories[experiment.identifier])
             index_result = self.get_step_result(experiment, StepType.INDEX)
             lattice = index_result.get('lattice')
 
             io_options = {
-                'data_range': (experiment.frames[0][0], experiment.frames[-1][1]),
-                'spot_range': experiment.frames, 'skip_range': experiment.missing,
+                'data_range': experiment.frames,
+                'spot_range': experiment.frames,
                 'anomalous': self.options.anomalous, 'lattice': lattice,
                 'beam_center': experiment.detector_origin,
                 'min_fraction': 0.10
             }
             io_options.update(**self.options.extras)
             io.filter_spots()
             io.create_input_file(('IDXREF', 'DEFPIX', 'XPLAN'), experiment, io.XDSParameters(**io_options))
@@ -370,21 +369,22 @@
             os.chdir(self.options.working_directories[experiment.identifier])
 
             if not self.get_step_result(experiment, StepType.INDEX):
                 continue
 
             logger.info(f'{experiment.name}:')
             io_options = {
-                'data_range': (experiment.frames[0][0], experiment.frames[-1][1]),
-                'spot_range': experiment.frames, 'skip_range': experiment.missing,
+                'data_range': experiment.frames,
+                'spot_range': experiment.frames,
                 'anomalous': self.options.anomalous,
             }
             io_options.update(**self.options.extras)
-            #FIXME:  when overridden, update range_text
-            range_text = summarize_ranges(experiment.frames)
+            io_options.pop('lattice', None)     # ignore lattice parameter if specified,
+
+            range_text = summarize_ranges(io_options['data_range'])
 
             previous_integration = self.get_step_result(experiment, StepType.INTEGRATE)
             if self.options.optimize and previous_integration is not None:
                 # copy parameter to new file
                 shutil.copy('GXPARM.XDS', 'XPARM.XDS')
 
                 # inject parameters to extra options
@@ -485,16 +485,17 @@
                 reference_directory = self.options.working_directories[reference.identifier]
                 reference_data = Path(os.path.relpath((reference_directory / "XDS_ASCII.HKL"), directory))
             else:
                 reference_data = None
 
             try:
                 io_options = {
-                    "data_range": (experiment.frames[0][0], experiment.frames[-1][1]),
-                    "spot_range": experiment.frames, "skip_range": experiment.missing,  "reference": reference_data,
+                    "data_range": experiment.frames,
+                    "spot_range": experiment.frames,
+                    "reference": reference_data,
                 }
                 io_options.update(**self.options.extras)
                 io_options.update(lattice=reindex_lattice, reindex=reindex_matrix)
                 io.create_input_file(('CORRECT',), experiment, io.XDSParameters(**io_options))
                 run_command(
                     'xds_par', desc=f'- Applying symmetry {reindex_lattice.name} - #{reindex_lattice.spacegroup}'
                 )
```

### Comparing `mxproc-2023.5.0/mxproc/engines/xds/indexing.py` & `mxproc-2023.5.1/mxproc/engines/xds/indexing.py`

 * *Files 5% similar despite different names*

```diff
@@ -22,18 +22,17 @@
     try:
         run_command('xds_par', desc=f'- Attempt #{trial + 1} of auto-indexing')
         result = XDSParser.parse_index()
     except (CommandFailed, FileNotFoundError, KeyError) as err:
         result = generate_failure(f"Command failed: {err}")
 
     retry_messages = []
-
     request_retry = (
-            result.state == StateType.FAILURE and
-            IndexProblem.SOFTWARE_ERROR not in result.flags
+            result.state == StateType.FAILURE
+            and IndexProblem.SOFTWARE_ERROR not in IndexProblem(result.flags)
     )
 
     if request_retry:
         show_warnings(f'Indexing Problems:', result.messages)
         request_retry, retry_messages = manager.update_parameters(
             result.flags, spot_range=result.details['spots']['best_range']
         )
```

### Comparing `mxproc-2023.5.0/mxproc/engines/xds/io.py` & `mxproc-2023.5.1/mxproc/engines/xds/io.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,26 +5,26 @@
 from pathlib import Path
 from dataclasses import dataclass, field
 from typing import Union, Literal, Tuple, Sequence
 
 import numpy
 
 from mxproc.xtal import Lattice, Experiment
+from mxproc.common import find_missing
 from mxio import XYPair
-from mxproc.log import logger
+
 
 XDSJob = Literal["XYCORR", "INIT", "COLSPOT", "IDXREF",  "XPLAN", "DEFPIX", "INTEGRATE", "CORRECT", "ALL"]
 XDSRefinement = Literal["CELL", "BEAM", "ORIENTATION", "AXIS",  "DISTANCE", "POSITION", "SEGMENT", "ALL"]
 
 
 @dataclass
 class XDSParameters:
-    data_range: Tuple[int, int]
+    data_range: Sequence[Tuple[int, int]]
     spot_range: Sequence[Tuple[int, int]]
-    skip_range: Sequence[Tuple[int, int]] = ()
 
     format: str = ""
     beam_center: XYPair | None = None
     lattice: Lattice = field(default_factory=Lattice)
     reindex: Sequence[int] | None = None
     reference: Path | None = None
     plugin: str | None = None
@@ -105,24 +105,24 @@
         f"JOB=   {jobs_flag}\n"
     )
     dataset_text = (
         f"!------------------- Dataset parameters\n"
         f"X-RAY_WAVELENGTH=  {experiment.wavelength:7.5f}\n"
         f"DETECTOR_DISTANCE= {experiment.distance:5.1f}\n"
         f"STARTING_ANGLE=    {experiment.start_angle:5.1f}\n"
-        f"STARTING_FRAME=    {parameters.data_range[0]}\n"
+        f"STARTING_FRAME=    {parameters.data_range[0][0]}\n"
         f"OSCILLATION_RANGE= {experiment.delta_angle:4.2f}\n"
         f"FRIEDEL'S_LAW= {friedel_flag}\n"
         f"NAME_TEMPLATE_OF_DATA_FRAMES={template_path} {parameters.format}\n"
-        f"DATA_RANGE=    {parameters.data_range[0]} {parameters.data_range[1]}\n"
+        f"DATA_RANGE=    {parameters.data_range[0][0]} {parameters.data_range[-1][1]}\n"
     )
     for start, end in parameters.spot_range:
         dataset_text += f"SPOT_RANGE=    {start} {end}\n"
 
-    for start, end in parameters.skip_range:
+    for start, end in find_missing(parameters.data_range):
         dataset_text += f"EXCLUDE_DATA_RANGE=    {start} {end}\n"
 
     # Allow injecting an external library for reading dataset files
     if parameters.plugin is not None:
         dataset_text += f'LIB= {parameters.plugin}\n'
 
     if parameters.lattice.spacegroup > 0:
```

### Comparing `mxproc-2023.5.0/mxproc/engines/xds/parser/__init__.py` & `mxproc-2023.5.1/mxproc/engines/xds/parser/__init__.py`

 * *Files identical despite different names*

### Comparing `mxproc-2023.5.0/mxproc/engines/xds/parser/data/correct.yml` & `mxproc-2023.5.1/mxproc/engines/xds/parser/data/correct.yml`

 * *Files identical despite different names*

### Comparing `mxproc-2023.5.0/mxproc/engines/xds/parser/data/idxref.yml` & `mxproc-2023.5.1/mxproc/engines/xds/parser/data/idxref.yml`

 * *Files identical despite different names*

### Comparing `mxproc-2023.5.0/mxproc/engines/xds/parser/data/integrate.yml` & `mxproc-2023.5.1/mxproc/engines/xds/parser/data/integrate.yml`

 * *Files identical despite different names*

### Comparing `mxproc-2023.5.0/mxproc/engines/xds/parser/data/xparm.yml` & `mxproc-2023.5.1/mxproc/engines/xds/parser/data/xparm.yml`

 * *Files identical despite different names*

### Comparing `mxproc-2023.5.0/mxproc/engines/xds/parser/data/xplan.yml` & `mxproc-2023.5.1/mxproc/engines/xds/parser/data/xplan.yml`

 * *Files identical despite different names*

### Comparing `mxproc-2023.5.0/mxproc/engines/xds/parser/data/xscale.yml` & `mxproc-2023.5.1/mxproc/engines/xds/parser/data/xscale.yml`

 * *Files identical despite different names*

### Comparing `mxproc-2023.5.0/mxproc/engines/xds/parser/data/xtriage.yml` & `mxproc-2023.5.1/mxproc/engines/xds/parser/data/xtriage.yml`

 * *Files identical despite different names*

### Comparing `mxproc-2023.5.0/mxproc/engines/xds/parser/pointless.py` & `mxproc-2023.5.1/mxproc/engines/xds/parser/pointless.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 import xml.dom.minidom
-from typing import Sequence
+from fractions import Fraction
 from mxproc.xtal import Lattice, SPACEGROUP_NAMES
 
 
 def get_spacegroup(element: xml.dom.minidom.Element) -> dict:
     """
     Extract Spacegroup dictionary from xml element representing a spacegroup solution
     :param element: XML element of
     :return: dictionary of parameters
     """
 
     number = int(element.getElementsByTagName('SGnumber')[0].firstChild.nodeValue)
     probability = float(element.getElementsByTagName('TotalProb')[0].firstChild.nodeValue)
     screw_axis_prob = float(element.getElementsByTagName('SysAbsProb')[0].firstChild.nodeValue)
     reindex_list = element.getElementsByTagName('ReindexMatrix')[0].firstChild.nodeValue.split()
-    reindex = list(map(int, reindex_list))
+
+    reindex = list(map(Fraction, reindex_list))
     reindex_matrix = (
         reindex[0], reindex[3], reindex[6], 0,
         reindex[1], reindex[4], reindex[7], 0,
         reindex[2], reindex[5], reindex[8], 0
     )
     spacegroup = {
         'name': SPACEGROUP_NAMES.get(number, 'P1'), 'number': number, 'probability': probability,
```

### Comparing `mxproc-2023.5.0/mxproc/engines/xds/stats.py` & `mxproc-2023.5.1/mxproc/engines/xds/stats.py`

 * *Files identical despite different names*

### Comparing `mxproc-2023.5.0/mxproc/log.py` & `mxproc-2023.5.1/mxproc/log.py`

 * *Files identical despite different names*

### Comparing `mxproc-2023.5.0/mxproc/programs/raddose.py` & `mxproc-2023.5.1/mxproc/programs/raddose.py`

 * *Files identical despite different names*

### Comparing `mxproc-2023.5.0/mxproc/reporting/__init__.py` & `mxproc-2023.5.1/mxproc/reporting/__init__.py`

 * *Files identical despite different names*

### Comparing `mxproc-2023.5.0/mxproc/reporting/data/report.html` & `mxproc-2023.5.1/mxproc/reporting/data/report.html`

 * *Files identical despite different names*

### Comparing `mxproc-2023.5.0/mxproc/reporting/data/report.js` & `mxproc-2023.5.1/mxproc/reporting/data/report.js`

 * *Files identical despite different names*

### Comparing `mxproc-2023.5.0/mxproc/reporting/data/report.min.css` & `mxproc-2023.5.1/mxproc/reporting/data/report.min.css`

 * *Files identical despite different names*

### Comparing `mxproc-2023.5.0/mxproc/reporting/data/report.min.js` & `mxproc-2023.5.1/mxproc/reporting/data/report.min.js`

 * *Files identical despite different names*

### Comparing `mxproc-2023.5.0/mxproc/reporting/data/report.scss` & `mxproc-2023.5.1/mxproc/reporting/data/report.scss`

 * *Files identical despite different names*

### Comparing `mxproc-2023.5.0/mxproc/reporting/generic.py` & `mxproc-2023.5.1/mxproc/reporting/generic.py`

 * *Files identical despite different names*

### Comparing `mxproc-2023.5.0/mxproc/reporting/screening.py` & `mxproc-2023.5.1/mxproc/reporting/screening.py`

 * *Files identical despite different names*

### Comparing `mxproc-2023.5.0/mxproc/reporting/text.py` & `mxproc-2023.5.1/mxproc/reporting/text.py`

 * *Files identical despite different names*

### Comparing `mxproc-2023.5.0/mxproc/xtal.py` & `mxproc-2023.5.1/mxproc/xtal.py`

 * *Files 3% similar despite different names*

```diff
@@ -153,30 +153,28 @@
     detector_size: XYPair
     detector_origin: XYPair
     geometry: Geometry
     cutoff_value: float
     sensor_thickness: float
     start_angle: float = 0.0
     lattice: Lattice = field(default_factory=Lattice)
-    missing: Sequence[Tuple[int, int]] = ()
 
 
 def compress_series(values: ArrayLike) -> Sequence[Tuple[int, int]]:
     """
     Takes a sequence of integers such as [1,2,3,4,6,7,8,10] and compress it as a list of
-    contiguous tuples [(1,4),(6,8), (10,10)]"
+    contiguous range tuples [(1,5),(6,9), (10,11)]"
 
     :param values: ArrayLike
     :return: Sequence of Tuples.
     """
-
     values = numpy.array(values).astype(int)
     values.sort()
     return [
-        (int(chunk[0]), int(chunk[-1]))
+        (int(chunk[0]), int(chunk[-1]) + 1)
         for chunk in numpy.split(values, numpy.where(numpy.diff(values) > 1)[0] + 1)
         if len(chunk)
     ]
 
 
 def load_experiment(filename: Union[str, Path]) -> Sequence[Experiment]:
     """
@@ -228,21 +226,15 @@
             sensor_thickness=dset.frame.sensor_thickness,
             pixel_size=dset.frame.pixel_size,
             detector_size=dset.frame.size,
             detector_origin=dset.frame.center,
             geometry=dset.frame.geometry,
             delta_angle=dset.frame.delta_angle,
             start_angle=sweep[0, 1],
-            glob=wildcard,
-            missing=compress_series(
-                numpy.setdiff1d(
-                    numpy.arange(sweep[0, 0], sweep[-1, 0] + 1),
-                    sweep[:, 0], assume_unique=True
-                )
-            )
+            glob=wildcard
         )
         for i, sweep in enumerate(sweeps)
     ]
 
 
 def load_multiple(file_names: Sequence[Union[str, Path]]) -> Sequence[Experiment]:
     """
```

### Comparing `mxproc-2023.5.0/mxproc.egg-info/PKG-INFO` & `mxproc-2023.5.1/mxproc.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mxproc
-Version: 2023.5.0
+Version: 2023.5.1
 Summary: MX Automated Data Processing Pipeline
 Author-email: Michel Fodje <michel4j@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/michel4j/mxproc
 Keywords: Data Processing Pipeline,MX,AutoProcess
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `mxproc-2023.5.0/mxproc.egg-info/SOURCES.txt` & `mxproc-2023.5.1/mxproc.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mxproc-2023.5.0/pyproject.toml` & `mxproc-2023.5.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `mxproc-2023.5.0/test/test_common.py` & `mxproc-2023.5.1/test/test_common.py`

 * *Files identical despite different names*

