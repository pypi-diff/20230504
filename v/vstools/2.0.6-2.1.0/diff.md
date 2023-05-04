# Comparing `tmp/vstools-2.0.6.tar.gz` & `tmp/vstools-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vstools-2.0.6.tar", last modified: Tue Mar 28 18:21:12 2023, max compression
+gzip compressed data, was "vstools-2.1.0.tar", last modified: Thu May  4 21:57:25 2023, max compression
```

## Comparing `vstools-2.0.6.tar` & `vstools-2.1.0.tar`

### file list

```diff
@@ -1,69 +1,69 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 18:21:12.051456 vstools-2.0.6/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-03-28 18:20:50.000000 vstools-2.0.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1276 2023-03-28 18:21:12.051456 vstools-2.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      610 2023-03-28 18:20:50.000000 vstools-2.0.6/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      860 2023-03-28 18:21:12.051456 vstools-2.0.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1666 2023-03-28 18:20:50.000000 vstools-2.0.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 18:21:12.043455 vstools-2.0.6/vstools/
--rw-r--r--   0 runner    (1001) docker     (123)      214 2023-03-28 18:20:50.000000 vstools-2.0.6/vstools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      373 2023-03-28 18:20:50.000000 vstools-2.0.6/vstools/_metadata.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 18:21:12.043455 vstools-2.0.6/vstools/enums/
--rw-r--r--   0 runner    (1001) docker     (123)      206 2023-03-28 18:20:50.000000 vstools-2.0.6/vstools/enums/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2016 2023-03-28 18:20:50.000000 vstools-2.0.6/vstools/enums/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    34191 2023-03-28 18:20:50.000000 vstools-2.0.6/vstools/enums/color.py
--rw-r--r--   0 runner    (1001) docker     (123)      367 2023-03-28 18:20:50.000000 vstools-2.0.6/vstools/enums/funcs.py
--rw-r--r--   0 runner    (1001) docker     (123)     6748 2023-03-28 18:20:50.000000 vstools-2.0.6/vstools/enums/generic.py
--rw-r--r--   0 runner    (1001) docker     (123)     8806 2023-03-28 18:20:50.000000 vstools-2.0.6/vstools/enums/other.py
--rw-r--r--   0 runner    (1001) docker     (123)    13477 2023-03-28 18:20:50.000000 vstools-2.0.6/vstools/enums/stubs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 18:21:12.043455 vstools-2.0.6/vstools/exceptions/
--rw-r--r--   0 runner    (1001) docker     (123)      246 2023-03-28 18:20:50.000000 vstools-2.0.6/vstools/exceptions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6242 2023-03-28 18:20:50.000000 vstools-2.0.6/vstools/exceptions/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2971 2023-03-28 18:20:50.000000 vstools-2.0.6/vstools/exceptions/color.py
--rw-r--r--   0 runner    (1001) docker     (123)      842 2023-03-28 18:20:50.000000 vstools-2.0.6/vstools/exceptions/enum.py
--rw-r--r--   0 runner    (1001) docker     (123)      929 2023-03-28 18:20:50.000000 vstools-2.0.6/vstools/exceptions/file.py
--rw-r--r--   0 runner    (1001) docker     (123)    14356 2023-03-28 18:20:50.000000 vstools-2.0.6/vstools/exceptions/generic.py
--rw-r--r--   0 runner    (1001) docker     (123)     1207 2023-03-28 18:20:50.000000 vstools-2.0.6/vstools/exceptions/module.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 18:21:12.047456 vstools-2.0.6/vstools/functions/
--rw-r--r--   0 runner    (1001) docker     (123)      385 2023-03-28 18:20:50.000000 vstools-2.0.6/vstools/functions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5534 2023-03-28 18:20:50.000000 vstools-2.0.6/vstools/functions/check.py
--rw-r--r--   0 runner    (1001) docker     (123)     3287 2023-03-28 18:20:50.000000 vstools-2.0.6/vstools/functions/clip.py
--rw-r--r--   0 runner    (1001) docker     (123)    10040 2023-03-28 18:20:50.000000 vstools-2.0.6/vstools/functions/funcs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1452 2023-03-28 18:20:50.000000 vstools-2.0.6/vstools/functions/heuristics.py
--rw-r--r--   0 runner    (1001) docker     (123)     6818 2023-03-28 18:20:50.000000 vstools-2.0.6/vstools/functions/normalize.py
--rw-r--r--   0 runner    (1001) docker     (123)     2154 2023-03-28 18:20:50.000000 vstools-2.0.6/vstools/functions/progress.py
--rw-r--r--   0 runner    (1001) docker     (123)     6802 2023-03-28 18:20:50.000000 vstools-2.0.6/vstools/functions/render.py
--rw-r--r--   0 runner    (1001) docker     (123)    14551 2023-03-28 18:20:50.000000 vstools-2.0.6/vstools/functions/timecodes.py
--rw-r--r--   0 runner    (1001) docker     (123)    20043 2023-03-28 18:20:50.000000 vstools-2.0.6/vstools/functions/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-28 18:20:50.000000 vstools-2.0.6/vstools/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 18:21:12.047456 vstools-2.0.6/vstools/types/
--rw-r--r--   0 runner    (1001) docker     (123)      209 2023-03-28 18:20:50.000000 vstools-2.0.6/vstools/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4995 2023-03-28 18:20:50.000000 vstools-2.0.6/vstools/types/builtins.py
--rw-r--r--   0 runner    (1001) docker     (123)     1675 2023-03-28 18:20:50.000000 vstools-2.0.6/vstools/types/file.py
--rw-r--r--   0 runner    (1001) docker     (123)     3151 2023-03-28 18:20:50.000000 vstools-2.0.6/vstools/types/funcs.py
--rw-r--r--   0 runner    (1001) docker     (123)     3465 2023-03-28 18:20:50.000000 vstools-2.0.6/vstools/types/generic.py
--rw-r--r--   0 runner    (1001) docker     (123)    16614 2023-03-28 18:20:50.000000 vstools-2.0.6/vstools/types/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 18:21:12.051456 vstools-2.0.6/vstools/utils/
--rw-r--r--   0 runner    (1001) docker     (123)    17595 2023-03-28 18:20:50.000000 vstools-2.0.6/vstools/utils/__file_headers.json
--rw-r--r--   0 runner    (1001) docker     (123)      650 2023-03-28 18:20:50.000000 vstools-2.0.6/vstools/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14310 2023-03-28 18:20:50.000000 vstools-2.0.6/vstools/utils/clips.py
--rw-r--r--   0 runner    (1001) docker     (123)    11326 2023-03-28 18:20:50.000000 vstools-2.0.6/vstools/utils/colors.py
--rw-r--r--   0 runner    (1001) docker     (123)     6141 2023-03-28 18:20:50.000000 vstools-2.0.6/vstools/utils/ffprobe.py
--rw-r--r--   0 runner    (1001) docker     (123)     9837 2023-03-28 18:20:50.000000 vstools-2.0.6/vstools/utils/file.py
--rw-r--r--   0 runner    (1001) docker     (123)      856 2023-03-28 18:20:50.000000 vstools-2.0.6/vstools/utils/funcs.py
--rw-r--r--   0 runner    (1001) docker     (123)     8407 2023-03-28 18:20:50.000000 vstools-2.0.6/vstools/utils/info.py
--rw-r--r--   0 runner    (1001) docker     (123)     3175 2023-03-28 18:20:50.000000 vstools-2.0.6/vstools/utils/math.py
--rw-r--r--   0 runner    (1001) docker     (123)    10234 2023-03-28 18:20:50.000000 vstools-2.0.6/vstools/utils/mime.py
--rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-03-28 18:20:50.000000 vstools-2.0.6/vstools/utils/mime_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     5909 2023-03-28 18:20:50.000000 vstools-2.0.6/vstools/utils/misc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1371 2023-03-28 18:20:50.000000 vstools-2.0.6/vstools/utils/other.py
--rw-r--r--   0 runner    (1001) docker     (123)     4332 2023-03-28 18:20:50.000000 vstools-2.0.6/vstools/utils/props.py
--rw-r--r--   0 runner    (1001) docker     (123)     7362 2023-03-28 18:20:50.000000 vstools-2.0.6/vstools/utils/ranges.py
--rw-r--r--   0 runner    (1001) docker     (123)     8019 2023-03-28 18:20:50.000000 vstools-2.0.6/vstools/utils/scale.py
--rw-r--r--   0 runner    (1001) docker     (123)    23662 2023-03-28 18:20:50.000000 vstools-2.0.6/vstools/utils/vs_enums.py
--rw-r--r--   0 runner    (1001) docker     (123)    25526 2023-03-28 18:20:50.000000 vstools-2.0.6/vstools/utils/vs_proxy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 18:21:12.043455 vstools-2.0.6/vstools.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1276 2023-03-28 18:21:12.000000 vstools-2.0.6/vstools.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1483 2023-03-28 18:21:12.000000 vstools-2.0.6/vstools.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-28 18:21:12.000000 vstools-2.0.6/vstools.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-03-28 18:21:12.000000 vstools-2.0.6/vstools.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-03-28 18:21:12.000000 vstools-2.0.6/vstools.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 21:57:25.836536 vstools-2.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-05-04 21:57:03.000000 vstools-2.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1276 2023-05-04 21:57:25.836536 vstools-2.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      610 2023-05-04 21:57:03.000000 vstools-2.1.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      860 2023-05-04 21:57:25.836536 vstools-2.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1666 2023-05-04 21:57:03.000000 vstools-2.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 21:57:25.832536 vstools-2.1.0/vstools/
+-rw-r--r--   0 runner    (1001) docker     (123)      214 2023-05-04 21:57:03.000000 vstools-2.1.0/vstools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      373 2023-05-04 21:57:03.000000 vstools-2.1.0/vstools/_metadata.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 21:57:25.832536 vstools-2.1.0/vstools/enums/
+-rw-r--r--   0 runner    (1001) docker     (123)      206 2023-05-04 21:57:03.000000 vstools-2.1.0/vstools/enums/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2016 2023-05-04 21:57:03.000000 vstools-2.1.0/vstools/enums/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34196 2023-05-04 21:57:03.000000 vstools-2.1.0/vstools/enums/color.py
+-rw-r--r--   0 runner    (1001) docker     (123)      367 2023-05-04 21:57:03.000000 vstools-2.1.0/vstools/enums/funcs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6748 2023-05-04 21:57:03.000000 vstools-2.1.0/vstools/enums/generic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9318 2023-05-04 21:57:03.000000 vstools-2.1.0/vstools/enums/other.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13666 2023-05-04 21:57:03.000000 vstools-2.1.0/vstools/enums/stubs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 21:57:25.832536 vstools-2.1.0/vstools/exceptions/
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-05-04 21:57:03.000000 vstools-2.1.0/vstools/exceptions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6287 2023-05-04 21:57:03.000000 vstools-2.1.0/vstools/exceptions/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2971 2023-05-04 21:57:03.000000 vstools-2.1.0/vstools/exceptions/color.py
+-rw-r--r--   0 runner    (1001) docker     (123)      843 2023-05-04 21:57:03.000000 vstools-2.1.0/vstools/exceptions/enum.py
+-rw-r--r--   0 runner    (1001) docker     (123)      929 2023-05-04 21:57:03.000000 vstools-2.1.0/vstools/exceptions/file.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14418 2023-05-04 21:57:03.000000 vstools-2.1.0/vstools/exceptions/generic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1207 2023-05-04 21:57:03.000000 vstools-2.1.0/vstools/exceptions/module.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 21:57:25.832536 vstools-2.1.0/vstools/functions/
+-rw-r--r--   0 runner    (1001) docker     (123)      385 2023-05-04 21:57:03.000000 vstools-2.1.0/vstools/functions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5534 2023-05-04 21:57:03.000000 vstools-2.1.0/vstools/functions/check.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3286 2023-05-04 21:57:03.000000 vstools-2.1.0/vstools/functions/clip.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10040 2023-05-04 21:57:03.000000 vstools-2.1.0/vstools/functions/funcs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1452 2023-05-04 21:57:03.000000 vstools-2.1.0/vstools/functions/heuristics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7466 2023-05-04 21:57:03.000000 vstools-2.1.0/vstools/functions/normalize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2154 2023-05-04 21:57:03.000000 vstools-2.1.0/vstools/functions/progress.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9822 2023-05-04 21:57:03.000000 vstools-2.1.0/vstools/functions/render.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15207 2023-05-04 21:57:03.000000 vstools-2.1.0/vstools/functions/timecodes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20161 2023-05-04 21:57:03.000000 vstools-2.1.0/vstools/functions/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 21:57:03.000000 vstools-2.1.0/vstools/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 21:57:25.836536 vstools-2.1.0/vstools/types/
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-05-04 21:57:03.000000 vstools-2.1.0/vstools/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4995 2023-05-04 21:57:03.000000 vstools-2.1.0/vstools/types/builtins.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1675 2023-05-04 21:57:03.000000 vstools-2.1.0/vstools/types/file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3151 2023-05-04 21:57:03.000000 vstools-2.1.0/vstools/types/funcs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3464 2023-05-04 21:57:03.000000 vstools-2.1.0/vstools/types/generic.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18463 2023-05-04 21:57:03.000000 vstools-2.1.0/vstools/types/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 21:57:25.836536 vstools-2.1.0/vstools/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)    17595 2023-05-04 21:57:03.000000 vstools-2.1.0/vstools/utils/__file_headers.json
+-rw-r--r--   0 runner    (1001) docker     (123)      650 2023-05-04 21:57:03.000000 vstools-2.1.0/vstools/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14310 2023-05-04 21:57:03.000000 vstools-2.1.0/vstools/utils/clips.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11326 2023-05-04 21:57:03.000000 vstools-2.1.0/vstools/utils/colors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6141 2023-05-04 21:57:03.000000 vstools-2.1.0/vstools/utils/ffprobe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9837 2023-05-04 21:57:03.000000 vstools-2.1.0/vstools/utils/file.py
+-rw-r--r--   0 runner    (1001) docker     (123)      856 2023-05-04 21:57:03.000000 vstools-2.1.0/vstools/utils/funcs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8407 2023-05-04 21:57:03.000000 vstools-2.1.0/vstools/utils/info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3218 2023-05-04 21:57:03.000000 vstools-2.1.0/vstools/utils/math.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10234 2023-05-04 21:57:03.000000 vstools-2.1.0/vstools/utils/mime.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-05-04 21:57:03.000000 vstools-2.1.0/vstools/utils/mime_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5818 2023-05-04 21:57:03.000000 vstools-2.1.0/vstools/utils/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1371 2023-05-04 21:57:03.000000 vstools-2.1.0/vstools/utils/other.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4332 2023-05-04 21:57:03.000000 vstools-2.1.0/vstools/utils/props.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11406 2023-05-04 21:57:03.000000 vstools-2.1.0/vstools/utils/ranges.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7859 2023-05-04 21:57:03.000000 vstools-2.1.0/vstools/utils/scale.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23662 2023-05-04 21:57:03.000000 vstools-2.1.0/vstools/utils/vs_enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25122 2023-05-04 21:57:03.000000 vstools-2.1.0/vstools/utils/vs_proxy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 21:57:25.832536 vstools-2.1.0/vstools.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1276 2023-05-04 21:57:25.000000 vstools-2.1.0/vstools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1483 2023-05-04 21:57:25.000000 vstools-2.1.0/vstools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 21:57:25.000000 vstools-2.1.0/vstools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-05-04 21:57:25.000000 vstools-2.1.0/vstools.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-04 21:57:25.000000 vstools-2.1.0/vstools.egg-info/top_level.txt
```

### Comparing `vstools-2.0.6/LICENSE` & `vstools-2.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `vstools-2.0.6/PKG-INFO` & `vstools-2.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vstools
-Version: 2.0.6
+Version: 2.1.0
 Summary: Functions and utils related to VapourSynth
 Author: Setsugen no ao
 Author-email: setsugen@setsugen.dev
 Maintainer: Setsugen no ao
 Maintainer-email: setsugen@setsugen.dev
 Project-URL: Source Code, https://github.com/Irrational-Encoding-Wizardry/vs-tools
 Project-URL: Documentation, https://vstools.encoding.moe/en/latest/
```

### Comparing `vstools-2.0.6/README.md` & `vstools-2.1.0/README.md`

 * *Files identical despite different names*

### Comparing `vstools-2.0.6/setup.cfg` & `vstools-2.1.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `vstools-2.0.6/setup.py` & `vstools-2.1.0/setup.py`

 * *Files identical despite different names*

### Comparing `vstools-2.0.6/vstools/enums/base.py` & `vstools-2.1.0/vstools/enums/base.py`

 * *Files identical despite different names*

### Comparing `vstools-2.0.6/vstools/enums/color.py` & `vstools-2.1.0/vstools/enums/color.py`

 * *Files 1% similar despite different names*

```diff
@@ -402,15 +402,15 @@
     ARIB_B67 = 18
     """
     Association of Radio Industries and Businesses (ARIB) STD-B67\n
     Rec. ITU-R BT.2100-2 hybrid loggamma (HLG) system
     """
 
     """
-    Extra tranfer characterists from libplacebo
+    Extra transfer characterists from libplacebo
     https://github.com/haasn/libplacebo/blob/master/src/include/libplacebo/colorspace.h#L193
     """
 
     # Standard gamut:
     BT601_525 = 100
     """ITU-R Rec. BT.601 (525-line = NTSC, SMPTE-C)"""
 
@@ -927,21 +927,21 @@
 
         if matrix not in _matrix_matrixcoeff_map:
             raise UnsupportedMatrixError(f'{matrix} is not supported!', cls.from_matrix)
 
         return _matrix_matrixcoeff_map[matrix]
 
     @classmethod
-    def from_transfer(cls, tranfer: Transfer) -> MatrixCoefficients:
+    def from_transfer(cls, transfer: Transfer) -> MatrixCoefficients:
         """Matrix Coefficients from a Transfer object's value."""
 
-        if tranfer not in _transfer_matrixcoeff_map:
-            raise UnsupportedTransferError(f'{tranfer} is not supported!', cls.from_transfer)
+        if transfer not in _transfer_matrixcoeff_map:
+            raise UnsupportedTransferError(f'{transfer} is not supported!', cls.from_transfer)
 
-        return _transfer_matrixcoeff_map[tranfer]
+        return _transfer_matrixcoeff_map[transfer]
 
     @classmethod
     def from_primaries(cls, primaries: Primaries) -> MatrixCoefficients:
         """Matrix Coefficients from a Primaries object's value."""
 
         if primaries not in _primaries_matrixcoeff_map:
             raise UnsupportedPrimariesError(f'{primaries} is not supported!', cls.from_primaries)
```

### Comparing `vstools-2.0.6/vstools/enums/generic.py` & `vstools-2.1.0/vstools/enums/generic.py`

 * *Files identical despite different names*

### Comparing `vstools-2.0.6/vstools/enums/other.py` & `vstools-2.1.0/vstools/enums/other.py`

 * *Files 9% similar despite different names*

```diff
@@ -2,21 +2,21 @@
 
 from fractions import Fraction
 from math import gcd as max_common_div
 from typing import Callable, Iterable, NamedTuple, TypeVar, overload
 
 import vapoursynth as vs
 
-from ..types import FuncExceptT, Sentinel
+from ..types import Sentinel
 from ..types.funcs import SentinelDispatcher
 from .base import CustomIntEnum, CustomStrEnum
 
 __all__ = [
     'Direction',
-    'Dar', 'Par',
+    'Dar', 'Sar',
     'Region',
     'Resolution',
     'Coordinate',
     'Position',
     'Size',
     'SceneChangeMode'
 ]
@@ -45,68 +45,67 @@
 
     @property
     def string(self) -> str:
         """A string representation of the Direction."""
         return self._name_.lower()
 
 
-class Par(Fraction):
+class Dar(Fraction):
+    height: int
+
+    def __new__(cls, numerator: int, denominator: int, height: int) -> Dar:
+        self = super().__new__(cls, numerator, denominator)
+
+        self.height = height
+
+        return self
+
     @overload
     @staticmethod
-    def get_ar(width: int, height: int, /) -> Fraction:
-        """Calculate the aspect ratio using a given width and height."""
+    def from_size(width: int, height: int, /) -> Dar:
+        ...
 
     @overload
     @staticmethod
-    def get_ar(clip: vs.VideoNode, /) -> Fraction:
-        """Calculate the aspect ratio using a given clip's width and height."""
+    def from_size(clip: vs.VideoNode, /) -> Dar:
+        ...
 
     @staticmethod
-    def get_ar(clip_width: vs.VideoNode | int, height: int = 0, /) -> Fraction:
+    def from_size(clip_width: vs.VideoNode | int, height: int = 0, /) -> Dar:
         if isinstance(clip_width, vs.VideoNode):
             width, height = clip_width.width, clip_width.height  # type: ignore
         else:
             width, height = clip_width, height
 
         gcd = max_common_div(width, height)
 
-        return Fraction(int(width / gcd), int(height / gcd))
+        return Dar(width // gcd, height // gcd, height)
 
+    def to_sar(self, active_area: float) -> Sar:
+        return Sar.from_dar(self, active_area)
 
-class Dar(CustomStrEnum):
-    """StrEnum signifying an analog television aspect ratio."""
 
-    WIDE = 'wide'
-    FULL = 'full'
-    SQUARE = 'square'
+class Sar(Fraction):
+    @staticmethod
+    def from_ar(den: int, num: int, height: int, active_area: float) -> Sar:
+        return Dar(den, num, height).to_sar(active_area)
 
-    @classmethod
-    def from_video(
-        cls, src: vs.VideoNode | vs.VideoFrame | vs.FrameProps, strict: bool = False, func: FuncExceptT | None = None
-    ) -> Dar:
-        """Calculate the Dar using a given clip's frame properties."""
-
-        from ..exceptions import CustomValueError, FramePropError
-        from ..utils import get_prop
-
-        try:
-            sar = get_prop(src, "_SARDen", int), get_prop(src, "_SARNum", int)
-        except FramePropError:
-            if strict:
-                raise FramePropError(
-                    '', '', 'SAR props not found! Make sure your video indexing plugin sets them!'
-                )
+    @staticmethod
+    def from_dar(dar: Dar, active_area: float) -> Sar:
+        sar_n, sar_d = dar.numerator * dar.height, dar.denominator * active_area
+
+        if isinstance(active_area, float):
+            sar_n, sar_d = int(sar_n * 10000), int(sar_d * 10000)
 
-            return Dar.WIDE
+        gcd = max_common_div(sar_n, sar_d)
 
-        match sar:
-            case (11, 10) | (9, 8): return Dar.FULL
-            case (33, 40) | (27, 32): return Dar.WIDE
+        return Sar(sar_n // gcd, sar_d // gcd)
 
-        raise CustomValueError("Could not calculate DAR. Please set the DAR manually.")
+    def apply(self, clip: vs.VideoNode) -> vs.VideoNode:
+        return clip.std.SetFrameProps(_SARNum=self.numerator, _SARDen=self.denominator)
 
 
 class Region(CustomStrEnum):
     """StrEnum signifying an analog television region."""
 
     UNKNOWN = 'unknown'
     """Unknown region."""
@@ -245,15 +244,15 @@
     @property
     def is_SCXVID(self) -> bool:
         return self in (
             SceneChangeMode.SCXVID, SceneChangeMode.WWXD_SCXVID_UNION,
             SceneChangeMode.WWXD_SCXVID_INTERSECTION
         )
 
-    def ensure_presence(self, clip: vs.VideoNode, akarin: bool = False) -> vs.VideoNode:
+    def ensure_presence(self, clip: vs.VideoNode, akarin: bool | None = None) -> vs.VideoNode:
         from ..exceptions import CustomRuntimeError
         from ..utils import merge_clip_props
 
         stats_clip = []
 
         if self.is_SCXVID:
             if not hasattr(vs.core, 'scxvid'):
@@ -267,14 +266,17 @@
             if not hasattr(vs.core, 'wwxd'):
                 raise CustomRuntimeError(
                     'You are missing wwxd!\n\tDownload it from https://github.com/dubhater/vapoursynth-wwxd',
                     self.ensure_presence
                 )
             stats_clip.append(clip.wwxd.WWXD())
 
+        if akarin is None:
+            akarin = hasattr(vs.core, 'akarin')
+
         if akarin:
             keys = list(self.prop_keys)
 
             expr = ' '.join([f'x.{k}' for k in keys]) + (' and' * (len(keys) - 1))
 
             blank = clip.std.BlankClip(1, 1, vs.GRAY8, keep=True)
 
@@ -292,19 +294,38 @@
     def prop_keys(self) -> Iterable[str]:
         if self.is_WWXD:
             yield 'Scenechange'
 
         if self.is_SCXVID:
             yield '_SceneChangePrev'
 
-    def lambda_cb(self, akarin: bool) -> Callable[[int, vs.VideoFrame], SentinelDispatcher | int]:
+    def check_cb(self, akarin: bool | None = None) -> Callable[[vs.VideoFrame], bool]:
+        if akarin is None:
+            akarin = hasattr(vs.core, 'akarin')
+
         if akarin:
-            return (lambda n, f: Sentinel.check(n, f[0][0, 0]))  # type: ignore
+            return (lambda f: bool(f[0][0, 0]))
+
+        keys = set(self.prop_keys)
+        prop_key = next(iter(keys))
 
         if self is SceneChangeMode.WWXD_SCXVID_UNION:
-            return (lambda n, f: Sentinel.check(n, any(f.props[key] == 1 for key in self.prop_keys)))
-        elif self is SceneChangeMode.WWXD_SCXVID_INTERSECTION:
-            return (lambda n, f: Sentinel.check(n, all(f.props[key] == 1 for key in self.prop_keys)))
+            return (lambda f: any(f.props[key] == 1 for key in keys))
+
+        if self is SceneChangeMode.WWXD_SCXVID_INTERSECTION:
+            return (lambda f: all(f.props[key] == 1 for key in keys))
+
+        return (lambda f: f.props[prop_key] == 1)
+
+    def lambda_cb(self, akarin: bool | None = None) -> Callable[[int, vs.VideoFrame], SentinelDispatcher | int]:
+        callback = self.check_cb(akarin)
+        return (lambda n, f: Sentinel.check(n, callback(f)))
+
+    def prepare_clip(self, clip: vs.VideoNode, height: int | None = 360, akarin: bool | None = None) -> vs.VideoNode:
+        from ..utils import get_w
 
-        prop_key = next(iter(self.prop_keys))
+        if height is not None:
+            clip = clip.resize.Bilinear(get_w(height, clip), height, vs.YUV420P8)
+        elif not clip.format or (clip.format and clip.format.id != vs.YUV420P8):
+            clip = clip.resize.Bilinear(format=vs.YUV420P8)
 
-        return (lambda n, f: Sentinel.check(n, f.props[prop_key] == 1))
+        return self.ensure_presence(clip, akarin)
```

### Comparing `vstools-2.0.6/vstools/enums/stubs.py` & `vstools-2.1.0/vstools/enums/stubs.py`

 * *Files 1% similar despite different names*

```diff
@@ -91,14 +91,18 @@
         cls: type[SelfPropEnum], clip: vs.VideoNode, value: int | SelfPropEnum | None, func: FuncExceptT | None = None
     ) -> vs.VideoNode:
         """Ensure the presence of the property in the VideoNode."""
         enum_value = cls.from_param(value, func) or cls.from_video(clip, True)
 
         return clip.std.SetFrameProp(enum_value.prop_key, enum_value.value)
 
+    def apply(self: SelfPropEnum, clip: vs.VideoNode) -> vs.VideoNode:
+        """Applies the property in the VideoNode."""
+        return clip.std.SetFrameProp(self.prop_key, self.value)
+
     @staticmethod
     def ensure_presences(
         clip: vs.VideoNode, prop_enums: Iterable[type[SelfPropEnum] | SelfPropEnum], func: FuncExceptT | None = None
     ) -> vs.VideoNode:
         """Ensure the presence of multiple PropEnums at once."""
         return clip.std.SetFrameProps(**{
             value.prop_key: value.value  # type: ignore
```

### Comparing `vstools-2.0.6/vstools/exceptions/base.py` & `vstools-2.1.0/vstools/exceptions/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -161,20 +161,21 @@
             kwargs = {
                 key: norm_display_name(value) for key, value in kwargs.items()
             }
 
         if self.reason:
             reason = norm_display_name(self.reason)
 
-            if not isinstance(self.reason, dict):
-                reason = f'({reason})'
-
-            if sys.stdout and sys.stdout.isatty():
-                reason = f'\033[0;33m{reason}\033[0m'
-            reason = f' {reason}'
+            if reason:
+                if not isinstance(self.reason, dict):
+                    reason = f'({reason})'
+
+                if sys.stdout and sys.stdout.isatty():
+                    reason = f'\033[0;33m{reason}\033[0m'
+                reason = f' {reason}'
         else:
             reason = ''
 
         return f'{func_header}{self.message!s}{reason}'.format(**kwargs).strip()
 
 
 SelfError = TypeVar('SelfError', bound=CustomError)
@@ -189,24 +190,24 @@
 
 
 class CustomOverflowError(CustomError, OverflowError):
     """Thrown when a value is out of range. e.g. temporal radius too big."""
 
 
 class CustomKeyError(CustomError, KeyError):
-    """Thrown when tring to access an non-existant key."""
+    """Thrown when trying to access an non-existent key."""
 
 
 class CustomTypeError(CustomError, TypeError):
     """Thrown when a passed argument is of wrong type."""
 
 
 class CustomRuntimeError(CustomError, RuntimeError):
     """Thrown when a runtime error occurs."""
 
 
 class CustomNotImplementedError(CustomError, NotImplementedError):
-    """Thrown when you encounter a yet not implemented brach of code."""
+    """Thrown when you encounter a yet not implemented branch of code."""
 
 
 class CustomPermissionError(CustomError, PermissionError):
     """Thrown when the user can't perform an action."""
```

### Comparing `vstools-2.0.6/vstools/exceptions/color.py` & `vstools-2.1.0/vstools/exceptions/color.py`

 * *Files identical despite different names*

### Comparing `vstools-2.0.6/vstools/exceptions/enum.py` & `vstools-2.1.0/vstools/exceptions/enum.py`

 * *Files 8% similar despite different names*

```diff
@@ -24,8 +24,8 @@
 
 
 class UnsupportedFieldBasedError(CustomValueError):
     """Raised when an unsupported field type is passed."""
 
 
 class NotFoundEnumValue(CustomKeyError):
-    """Raised when you try to instantiate an Enum with unkown value"""
+    """Raised when you try to instantiate an Enum with unknown value"""
```

### Comparing `vstools-2.0.6/vstools/exceptions/file.py` & `vstools-2.1.0/vstools/exceptions/file.py`

 * *Files identical despite different names*

### Comparing `vstools-2.0.6/vstools/exceptions/generic.py` & `vstools-2.1.0/vstools/exceptions/generic.py`

 * *Files 1% similar despite different names*

```diff
@@ -280,17 +280,19 @@
 
     @classmethod
     def _item_to_name(cls, item: int | Sized) -> str:
         return str(int(item if isinstance(item, int) else len(item)))
 
     def __init__(
         self, func: FuncExceptT, lengths: Iterable[int | Sized],
-        message: SupportsString = 'All the lenghts must be equal!', **kwargs: Any
+        message: SupportsString = 'All the lengths must be equal!', **kwargs: Any
     ) -> None:
-        super().__init__(func, lengths, message, **kwargs)
+        super().__init__(
+            func, lengths, message, iter(map(self._item_to_name, lengths)), **kwargs
+        )
 
     if TYPE_CHECKING:
         @classmethod
         def check(  # type: ignore[override]
             cls, func: FuncExceptT, *lengths: int | Sized, **kwargs: Any
         ) -> None:
             ...
```

### Comparing `vstools-2.0.6/vstools/exceptions/module.py` & `vstools-2.1.0/vstools/exceptions/module.py`

 * *Files identical despite different names*

### Comparing `vstools-2.0.6/vstools/functions/check.py` & `vstools-2.1.0/vstools/functions/check.py`

 * *Files identical despite different names*

### Comparing `vstools-2.0.6/vstools/functions/clip.py` & `vstools-2.1.0/vstools/functions/clip.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
 def shift_clip(clip: vs.VideoNode, offset: int) -> vs.VideoNode:
     """
     Shift a clip forwards or backwards by *n* frames.
 
     This is useful for cases where you must compare every frame of a clip
     with the frame that comes before or after the current frame,
-    like for example when performing termporal operations.
+    like for example when performing temporal operations.
 
     Both positive and negative integers are allowed.
     Positive values will shift a clip forward, negative will shift a clip backward.
 
     :param clip:            Input clip.
     :param offset:          Number of frames to offset the clip with. Negative values are allowed.
                             Positive values will shift a clip forward,
```

### Comparing `vstools-2.0.6/vstools/functions/funcs.py` & `vstools-2.1.0/vstools/functions/funcs.py`

 * *Files identical despite different names*

### Comparing `vstools-2.0.6/vstools/functions/heuristics.py` & `vstools-2.1.0/vstools/functions/heuristics.py`

 * *Files identical despite different names*

### Comparing `vstools-2.0.6/vstools/functions/normalize.py` & `vstools-2.1.0/vstools/functions/normalize.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,14 +8,16 @@
 from ..types import F, FrameRange, FrameRangeN, FrameRangesN, PlanesT, SupportsString, T, VideoNodeIterable
 
 __all__ = [
     'normalize_seq',
     'normalize_planes',
     'to_arr',
     'flatten', 'flatten_vnodes',
+    'normalize_list_to_ranges',
+    'normalize_ranges_to_list',
     'normalize_franges',
     'normalize_ranges',
     'norm_func_name', 'norm_display_name'
 ]
 
 
 @overload
@@ -44,15 +46,15 @@
         return [val] * length
 
     val = list(val) + [val[-1]] * (length - len(val))
 
     return val[:length]
 
 
-def normalize_planes(clip: vs.VideoNode, planes: PlanesT = None, pad: bool = False) -> list[int]:
+def normalize_planes(clip: vs.VideoNode, planes: PlanesT = None) -> list[int]:
     """
     Normalize a sequence of planes.
 
     :param clip:        Input clip.
     :param planes:      Array of planes. If None, returns all planes of the input clip's format.
                         Default: None.
     :param pad:         Whether to pad the output list.
@@ -64,21 +66,14 @@
     assert clip.format
 
     if planes is None or planes == 4:
         planes = list(range(clip.format.num_planes))
     else:
         planes = to_arr(planes, sub=True)
 
-    if pad:
-        print(DeprecationWarning(
-            'normalize_planes: pad=True is deprecated as it leads to undefined behaviour!\n'
-            'Please stop using it as it will be removed at a later date'
-        ))
-        return normalize_seq(planes, clip.format.num_planes)
-
     return list(sorted(set(planes).intersection(range(clip.format.num_planes))))
 
 
 _iterables_t = (list, tuple, range, zip, set, map, enumerate)
 
 
 @overload
@@ -161,14 +156,48 @@
         step = -1 if stop < start else 1
 
         return range(start, stop + step, step)
 
     return franges
 
 
+def normalize_list_to_ranges(flist: Sequence[int], min_length: int = 0) -> list[tuple[int, int]]:
+    flist2 = list[list[int]]()
+    flist3 = list[int]()
+
+    prev_n = -1
+
+    for n in sorted(set(flist)):
+        if prev_n + 1 != n:
+            if flist3:
+                flist2.append(flist3)
+                flist3 = []
+        flist3.append(n)
+        prev_n = n
+
+    if flist3:
+        flist2.append(flist3)
+
+    flist4 = [i for i in flist2 if len(i) > min_length]
+
+    return list(zip(
+        [i[0] for i in flist4],
+        [i[-1] for j, i in enumerate(flist4)]
+    ))
+
+
+def normalize_ranges_to_list(franges: Iterable[FrameRange]) -> list[int]:
+    out = list[int]()
+
+    for frange in franges:
+        out.extend(normalize_franges(frange))
+
+    return out
+
+
 def normalize_ranges(clip: vs.VideoNode, ranges: FrameRangeN | FrameRangesN) -> list[tuple[int, int]]:
     """
     Normalize ranges to a list of positive ranges.
 
     Frame ranges can include None and negative values.
     None will be converted to either 0 if it's the first value in a FrameRange,
     or the clip's length if it's the second item.
@@ -180,49 +209,53 @@
 
         >>> clip.num_frames
         1000
         >>> normalize_ranges(clip, (None, None))
         [(0, 1000)]
         >>> normalize_ranges(clip, (24, -24))
         [(24, 976)]
+        >>> normalize_ranges(clip, [(24, 100), (80, 150)])
+        [(24, 150)]
 
 
     :param clip:        Input clip.
     :param franges:     Frame range or list of frame ranges.
 
     :return:            List of positive frame ranges.
     """
 
     ranges = ranges if isinstance(ranges, list) else [ranges]  # type:ignore
 
     out = []
 
     for r in ranges:
+        if r is None:
+            r = (None, None)
+
         if isinstance(r, tuple):
             start, end = r
             if start is None:
                 start = 0
             if end is None:
                 end = clip.num_frames - 1
-        elif r is None:
-            start = clip.num_frames - 1
-            end = clip.num_frames - 1
         else:
             start = r
             end = r
 
         if start < 0:
             start = clip.num_frames - 1 + start
 
         if end < 0:
             end = clip.num_frames - 1 + end
 
         out.append((start, end))
 
-    return out
+    return normalize_list_to_ranges([
+        x for start, end in out for x in range(start, end + 1)
+    ])
 
 
 def norm_func_name(func_name: SupportsString | F) -> str:
     """Normalize a class, function, or other object to obtain its name"""
 
     if isinstance(func_name, str):
         return func_name.strip()
```

### Comparing `vstools-2.0.6/vstools/functions/progress.py` & `vstools-2.1.0/vstools/functions/progress.py`

 * *Files identical despite different names*

### Comparing `vstools-2.0.6/vstools/functions/timecodes.py` & `vstools-2.1.0/vstools/functions/timecodes.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from pathlib import Path
 from typing import Any, ClassVar, Iterable, NamedTuple, TypeVar, overload
 
 import vapoursynth as vs
 
 from ..enums import SceneChangeMode, Matrix
 from ..exceptions import CustomValueError, FramesLengthError
-from ..types import FilePathType, FuncExceptT, Sentinel
+from ..types import FilePathType, FuncExceptT, Sentinel, inject_self
 from .render import clip_async_render
 
 __all__ = [
     'Timecodes',
     'Keyframes',
     'LWIndex'
 ]
@@ -278,68 +278,90 @@
         out_path.write_text('\n'.join(out_text + ['']))
 
 
 TimecodesBoundT = TypeVar('TimecodesBoundT', bound=Timecodes)
 
 
 class Keyframes(list[int]):
+    """
+    Class representing keyframes, or scenechanges.
+
+    They follow the convention of signaling the start of the new scene.
+    """
+
     V1 = 1
     XVID = -1
 
     WWXD: ClassVar = SceneChangeMode.WWXD
     SCXVID: ClassVar = SceneChangeMode.SCXVID
 
-    def __init__(self, iterable: Iterable[int], end_frame: int) -> None:
+    @overload  # type: ignore
+    def __init__(self, iterable: Iterable[int]) -> None:
+        ...
+
+    def __init__(self, iterable: Iterable[int] = [], *, _dummy: bool = False) -> None:
         super().__init__(sorted(list(iterable)))
 
-        self.end_frame = end_frame
+        self._dummy = _dummy
 
     @classmethod
     def from_clip(
         cls: type[KeyframesBoundT], clip: vs.VideoNode, mode: SceneChangeMode | int = WWXD, height: int | None = 360,
         **kwargs: Any
     ) -> KeyframesBoundT:
-        from ..utils import get_w
 
         mode = SceneChangeMode(mode)
 
-        if height is not None:
-            clip = clip.resize.Bilinear(get_w(360, clip), 360, vs.YUV420P8)
-        else:
-            clip = clip.resize.Bilinear(format=vs.YUV420P8)
+        clip = mode.prepare_clip(clip, height)
 
-        aka_available = hasattr(vs.core, 'akarin')
+        frames = clip_async_render(clip, None, 'Detecting scene changes...', mode.lambda_cb(), **kwargs)
 
-        frames = clip_async_render(
-            mode.ensure_presence(clip, aka_available), None,
-            'Detecting scene changes...', mode.lambda_cb(aka_available), **kwargs
-        )
+        return cls(Sentinel.filter(frames))
 
-        return cls(Sentinel.filter(frames), clip.num_frames)
+    @inject_self.with_args(_dummy=True)
+    def to_clip(
+        self, clip: vs.VideoNode, *, mode: SceneChangeMode | int = WWXD, height: int | None = 360,
+        prop_key: str = next(iter(SceneChangeMode.SCXVID.prop_keys))
+    ) -> vs.VideoNode:
+        from ..utils import replace_ranges
+
+        propset_clip = clip.std.SetFrameProp(prop_key, True)
+
+        if self._dummy:
+            mode = SceneChangeMode(mode)
+
+            prop_clip, callback = mode.prepare_clip(clip, height), mode.check_cb()
+
+            return replace_ranges(clip, propset_clip, callback, prop_src=prop_clip)
+
+        return replace_ranges(clip, propset_clip, self)
 
     def to_file(self, out: FilePathType, format: int = V1, func: FuncExceptT | None = None) -> None:
         from ..utils import check_perms
 
         func = func or self.to_file
 
         out_path = Path(str(out)).resolve()
 
+        out_path.parent.mkdir(parents=True, exist_ok=True)
+
         check_perms(out_path, 'w+', func=func)
 
         if format == Keyframes.V1:
             out_text = [
-                '# keyframe format v1', 'fps 0', '', *map(str, self), ''
+                '# keyframe format v1', 'fps 0', '',
+                *(f'{n} I -1' for n in self), ''
             ]
         elif format == Keyframes.XVID:
             lut_self = set(self)
             out_text = [
                 '# XviD 2pass stat file', '',
                 *(
                     (lut_self.remove(i) or 'i') if i in lut_self else 'b'  # type: ignore
-                    for i in range(self.end_frame)
+                    for i in range(max(self))
                 )
             ]
 
         out_path.unlink(True)
         out_path.touch()
         out_path.write_text('\n'.join(out_text))
 
@@ -432,10 +454,10 @@
                         (LWIndex.Regex.frame_second.match(data[i + 1]), ['Key', 'Pic', 'POC', 'Repeat', 'Field'])
                     ] for key in match[1]
                 )
             ))
             for i in range(indexstart, indexend, 2)
         ], key=lambda x: x.pts)
 
-        keyframes = Keyframes([i for i, f in enumerate(frames) if f.key], len(frames))
+        keyframes = Keyframes(i for i, f in enumerate(frames) if f.key)
 
         return LWIndex(streaminfo, frames, keyframes)
```

### Comparing `vstools-2.0.6/vstools/functions/utils.py` & `vstools-2.1.0/vstools/functions/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from __future__ import annotations
 
 import string
-from typing import Any, Literal, Mapping, Sequence, cast, overload
+from typing import Any, Iterable, Literal, Mapping, cast, overload
 from weakref import WeakValueDictionary
 
 import vapoursynth as vs
 
 from ..enums import ColorRange, ColorRangeT, CustomStrEnum, Matrix
 from ..exceptions import ClipLengthError, CustomIndexError, CustomValueError, InvalidColorFamilyError
-from ..types import HoldsVideoFormatT, VideoFormatT, PlanesT
+from ..types import HoldsVideoFormatT, PlanesT, VideoFormatT
 from .check import disallow_variable_format
 
 __all__ = [
     'EXPR_VARS',
 
     'DitherType',
 
@@ -218,15 +218,16 @@
         dither_type = DitherType.ERROR_DIFFUSION if should_dither else DitherType.NONE
 
     new_format = in_fmt.replace(
         bits_per_sample=out_fmt.bits_per_sample, sample_type=out_fmt.sample_type
     )
 
     return clip.resize.Point(
-        format=new_format.id, range_in=range_in, range=range_out, dither_type=dither_type
+        format=new_format.id, range_in=range_in and range_in.value_zimg, range=range_out and range_out.value_zimg,
+        dither_type=dither_type
     )
 
 
 _f2c_cache = WeakValueDictionary[int, vs.VideoNode]()
 
 
 def frame2clip(frame: vs.VideoFrame) -> vs.VideoNode:
@@ -475,15 +476,15 @@
                         Default: first clip or detected from props if GRAY and len(planes) > 1.
 
     :return:            Clip of combined planes.
     """
 
 
 @overload
-def join(planes: Sequence[vs.VideoNode], family: vs.ColorFamily | None = None) -> vs.VideoNode:
+def join(planes: Iterable[vs.VideoNode], family: vs.ColorFamily | None = None) -> vs.VideoNode:
     """
     Join a list of planes together to form a single clip.
 
     :param planes:      Planes to combine.
     :param family:      Output clip family.
                         Default: first clip or detected from props if GRAY and len(planes) > 1.
 
@@ -501,16 +502,16 @@
                         Default: first clip or detected from props if GRAY and len(planes) > 1.
 
     :return:            Clip of combined planes.
     """
 
 
 def join(*_planes: Any, **kwargs: Any) -> vs.VideoNode:
-    from ..utils import get_color_family, get_video_format
     from ..functions import flatten_vnodes, to_arr
+    from ..utils import get_color_family, get_video_format
 
     family: vs.ColorFamily | None = kwargs.get('family', None)
 
     if isinstance(_planes[-1], vs.ColorFamily):
         family = _planes[-1]
         _planes = _planes[:-1]
 
@@ -524,15 +525,17 @@
             if p_key is None:
                 planes_map |= {i: n for i, n in enumerate(flatten_vnodes(node, split_planes=True))}
             else:
                 planes_map |= {i: plane(node, min(i, node.format.num_planes - 1)) for i in to_arr(p_key)}
 
         return join(*(planes_map[i] for i in sorted(planes_map.keys())))
 
-    planes = list[vs.VideoNode](_planes[0] if isinstance(_planes[0], Sequence) else _planes)
+    planes = list[vs.VideoNode](_planes[0] if (
+        isinstance(_planes[0], Iterable) and not isinstance(_planes[0], vs.VideoNode)
+    ) else _planes)
 
     n_clips = len(planes)
 
     if not n_clips:
         raise CustomIndexError('Not enough clips/planes passed!', join)
 
     if n_clips == 1 and (family is None or family is (planes[0].format and planes[0].format.color_family)):
```

### Comparing `vstools-2.0.6/vstools/types/builtins.py` & `vstools-2.1.0/vstools/types/builtins.py`

 * *Files identical despite different names*

### Comparing `vstools-2.0.6/vstools/types/file.py` & `vstools-2.1.0/vstools/types/file.py`

 * *Files identical despite different names*

### Comparing `vstools-2.0.6/vstools/types/funcs.py` & `vstools-2.1.0/vstools/types/funcs.py`

 * *Files identical despite different names*

### Comparing `vstools-2.0.6/vstools/types/generic.py` & `vstools-2.1.0/vstools/types/generic.py`

 * *Files 0% similar despite different names*

```diff
@@ -77,15 +77,15 @@
     if some_error:
         raise CustomValueError('Some error occurred!!', func)
 
 def some_func() -> None:
     ...
     can_throw(..., func=some_func)
 ```
-If an error occurrs, this will print a clear error ->\n
+If an error occurs, this will print a clear error ->\n
 ``ValueError: (some_func) Some error occurred!!``
 """
 
 FuncExceptT = str | Callable[..., Any] | tuple[Callable[..., Any] | str, str]  # type: ignore
 
 
 class VSFunctionNoArgs(Protocol):
```

### Comparing `vstools-2.0.6/vstools/types/utils.py` & `vstools-2.1.0/vstools/types/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -101,50 +101,77 @@
         """
         Wrap ``function`` to always have a self provided to it.
 
         :param function:    Method to wrap.
         :param cache:       Whether to cache the self object.
         """
 
-        self.function = function
+        self.cache = self.init_kwargs = None
+
         if isinstance(self, inject_self.cached):
             self.cache = True
-        else:
-            self.cache = cache
+
+        self.function = function
+
+        self.signature = self.first_key = self.init_kwargs = None
+
         self.args = tuple[Any]()
         self.kwargs = dict[str, Any]()
 
+        self.clean_kwargs = False
+
     def __get__(
         self, class_obj: type[T] | T | None, class_type: type[T] | type[type[T]]  # type: ignore
     ) -> injected_self_func[T, P, R]:
-        signature = Signature.from_callable(self.function, follow_wrapped=True, eval_str=True)
-        first_key = next(iter(list(signature.parameters.keys())), None)
+        if not self.signature or not self.first_key:  # type: ignore
+            self.signature = Signature.from_callable(self.function, follow_wrapped=True, eval_str=True)  # type: ignore
+            self.first_key = next(iter(list(self.signature.parameters.keys())), None)  # type: ignore
+
+            if isinstance(self, inject_self.init_kwargs):
+                from ..exceptions import CustomValueError
+
+                if 4 not in {x.kind for x in self.signature.parameters.values()}:  # type: ignore
+                    raise CustomValueError(
+                        'This function hasn\'t got any kwargs!', 'inject_self.init_kwargs', self.function
+                    )
+
+                self.init_kwargs = list[str](  # type: ignore
+                    k for k, x in self.signature.parameters.items() if x.kind != 4  # type: ignore
+                )
 
         @wraps(self.function)
         def _wrapper(*args: Any, **kwargs: Any) -> Any:
-            first_arg = (args[0] if args else None) or (kwargs.get(first_key, None) if first_key else None)
+            first_arg = (args[0] if args else None) or (
+                kwargs.get(self.first_key, None) if self.first_key else None  # type: ignore
+            )
 
             if (
                 first_arg and (
                     (is_obj := isinstance(first_arg, class_type))
                     or isinstance(first_arg, type(class_type))
                     or first_arg is class_type
                 )
             ):
                 obj = first_arg if is_obj else first_arg()
                 if args:
                     args = args[1:]
-                elif kwargs and first_key:
-                    kwargs.pop(first_key)
+                elif kwargs and self.first_key:
+                    kwargs.pop(self.first_key)  # type: ignore
             elif class_obj is None:
                 if self.cache:
                     if class_type not in self_objects_cache:
                         obj = self_objects_cache[class_type] = class_type(*self.args, **self.kwargs)
                     else:
                         obj = self_objects_cache[class_type]
+                elif self.init_kwargs:
+                    obj = class_type(  # type: ignore
+                        *self.args, **(self.kwargs | {k: v for k, v in kwargs.items() if k not in self.init_kwargs})
+                    )
+                    if self.clean_kwargs:
+                        kwargs = {k: v for k, v in kwargs.items() if k in self.init_kwargs}
                 else:
                     obj = class_type(*self.args, **self.kwargs)
             else:
                 obj = class_obj
 
             return self.function(obj, *args, **kwargs)
 
@@ -169,14 +196,27 @@
 
     class cached(Generic[T0, P0, R0], inject_self_base[T0, P0, R0]):  # type: ignore
         """
         Wrap a method so it always has a constructed ``self`` provided to it.
         Once ``self`` is constructed, it will be reused.
         """
 
+    class init_kwargs(Generic[T0, P0, R0], inject_self_base[T0, P0, R0]):  # type: ignore
+        """
+        Wrap a method so it always has a constructed ``self`` provided to it.
+        When constructed, kwargs to the function will be passed to the constructor.
+        """
+
+        @classmethod
+        def clean(cls, function: Callable[Concatenate[T0, P0], R0]) -> inject_self[T0, P0, R0]:
+            """Wrap a method, pass kwargs to the constructor and remove them from actual **kwargs."""
+            inj = cls(function)
+            inj.clean_kwargs = True
+            return inj  # type: ignore
+
 
 class complex_hash(Generic[T]):
     """
     Decorator for classes to add a ``__hash__`` method to them.
 
     Especially useful for NamedTuples.
     """
```

### Comparing `vstools-2.0.6/vstools/utils/__file_headers.json` & `vstools-2.1.0/vstools/utils/__file_headers.json`

 * *Files identical despite different names*

### Comparing `vstools-2.0.6/vstools/utils/__init__.py` & `vstools-2.1.0/vstools/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `vstools-2.0.6/vstools/utils/clips.py` & `vstools-2.1.0/vstools/utils/clips.py`

 * *Files identical despite different names*

### Comparing `vstools-2.0.6/vstools/utils/colors.py` & `vstools-2.1.0/vstools/utils/colors.py`

 * *Files identical despite different names*

### Comparing `vstools-2.0.6/vstools/utils/ffprobe.py` & `vstools-2.1.0/vstools/utils/ffprobe.py`

 * *Files identical despite different names*

### Comparing `vstools-2.0.6/vstools/utils/file.py` & `vstools-2.1.0/vstools/utils/file.py`

 * *Files identical despite different names*

### Comparing `vstools-2.0.6/vstools/utils/funcs.py` & `vstools-2.1.0/vstools/utils/funcs.py`

 * *Files identical despite different names*

### Comparing `vstools-2.0.6/vstools/utils/info.py` & `vstools-2.1.0/vstools/utils/info.py`

 * *Files identical despite different names*

### Comparing `vstools-2.0.6/vstools/utils/math.py` & `vstools-2.1.0/vstools/utils/math.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,14 +35,17 @@
 
     return round(x + (eps if x > 0. else - eps))
 
 
 def mod_x(val: int | float, x: int) -> int:
     """Force a value to be divisible by x (val % x == 0)."""
 
+    if x == 0:
+        return cround(val)
+
     return cround(val / x) * x
 
 
 def mod2(val: int | float) -> int:
     """Force a value to be mod 2"""
 
     return mod_x(val, x=2)
```

### Comparing `vstools-2.0.6/vstools/utils/mime.py` & `vstools-2.1.0/vstools/utils/mime.py`

 * *Files 0% similar despite different names*

```diff
@@ -35,15 +35,15 @@
 class ParsedFile(NamedTuple):
     """Structure for file info."""
 
     path: Path
     """Resolved path of the file."""
 
     ext: str
-    """Extention of the file, from the binary data, not path."""
+    """Extension of the file, from the binary data, not path."""
 
     encoding: str | None
     """Present for text files."""
 
     file_type: FileType
     """Type of the file. It will hold other useful information."""
 
@@ -55,15 +55,15 @@
 class FileSignature(NamedTuple):
     """Child structure of FileSignatures, holding info of certain types of files and their signatures."""
 
     file_type: str
     """FileType as a str."""
 
     ext: str
-    """Extention from the signature."""
+    """Extension from the signature."""
 
     mime: str
     """MIME type of the signature."""
 
     offset: int
     """Offset from the start of the file of the signatures."""
```

### Comparing `vstools-2.0.6/vstools/utils/mime_base.py` & `vstools-2.1.0/vstools/utils/mime_base.py`

 * *Files identical despite different names*

### Comparing `vstools-2.0.6/vstools/utils/misc.py` & `vstools-2.1.0/vstools/utils/misc.py`

 * *Files 4% similar despite different names*

```diff
@@ -26,36 +26,32 @@
     """
     Convert the framerate of a clip.
 
     This is different from AssumeFPS as this will actively adjust
     the framerate of a clip, not simply set one.
 
     :param clip:        Input clip.
-    :param fps:         Framerate to conver the clip to. Must be a Fration.
+    :param fps:         Framerate to convert the clip to. Must be a Fration.
 
     :return:            Clip with the framerate converted and frames adjusted as necessary.
     """
 
     src_num, src_den = clip.fps_num, clip.fps_den
     dest_num, dest_den = fps.as_integer_ratio()
 
     if (dest_num, dest_den) == (src_num, src_den):
         return clip
 
     factor = (dest_num / dest_den) * (src_den / src_num)
 
-    def _frame_adjuster(n: int) -> vs.VideoNode:
-        original = floor(n / factor)
-        return clip[original] * (clip.num_frames + 100)
-
     new_fps_clip = clip.std.BlankClip(
         length=floor(clip.num_frames * factor), fpsnum=dest_num, fpsden=dest_den
     )
 
-    return new_fps_clip.std.FrameEval(_frame_adjuster)
+    return new_fps_clip.std.FrameEval(lambda n: clip[round(n / factor)])
 
 
 @disallow_variable_format
 @disallow_variable_resolution
 def padder(
     clip: vs.VideoNode, left: int = 0, right: int = 0, top: int = 0, bottom: int = 0, reflect: bool = True
 ) -> vs.VideoNode:
@@ -152,15 +148,15 @@
     checktype = node[0] if isinstance(node, list) else node
 
     if isinstance(checktype, vs.VideoNode):
         title = 'Clip'
     elif isinstance(checktype, vs.AudioNode):
         title = 'Audio'
 
-    if not name or name is True:
+    if (not name and name is not False) or name is True:
         name = f"{title}{index}"
 
         current_frame = inspect.currentframe()
 
         assert current_frame
         assert current_frame.f_back
 
@@ -169,15 +165,15 @@
                 name = vname
                 break
 
     try:
         from vspreview import set_output as vsp_set_output
         if isinstance(node, list):
             for idx, n in enumerate(node, 0 if index else last_index):
-                vsp_set_output(n, f'{name} {idx}', **kwargs)
+                vsp_set_output(n, name and f'{name} {idx}', **kwargs)
         else:
             vsp_set_output(node, name, **kwargs)
     except ModuleNotFoundError:
         if isinstance(name, str) and isinstance(node, vs.VideoNode):
             if isinstance(node, list):
                 for idx, n in enumerate(node, 0 if index else last_index):
                     n.std.SetFrameProp('Name', data=f'{name.title()} {idx}').set_output(last_index)
```

### Comparing `vstools-2.0.6/vstools/utils/other.py` & `vstools-2.1.0/vstools/utils/other.py`

 * *Files identical despite different names*

### Comparing `vstools-2.0.6/vstools/utils/props.py` & `vstools-2.1.0/vstools/utils/props.py`

 * *Files identical despite different names*

### Comparing `vstools-2.0.6/vstools/utils/scale.py` & `vstools-2.1.0/vstools/utils/scale.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,36 +1,35 @@
 from __future__ import annotations
-from typing import Sequence
+
+from typing import Literal, Sequence, overload
 
 import vapoursynth as vs
 
 from ..enums import ColorRange, ColorRangeT
-from ..exceptions import CustomIndexError
 from ..functions import disallow_variable_format, normalize_seq
 from ..types import HoldsVideoFormatT, VideoFormatT
 from .info import get_depth, get_video_format
 
 __all__ = [
-    'scale_8bit', 'scale_thresh', 'scale_value',
+    'scale_8bit', 'scale_value',
 
     'get_lowest_value', 'get_neutral_value', 'get_peak_value',
     'get_lowest_values', 'get_neutral_values', 'get_peak_values',
 ]
 
 
 def scale_8bit(clip: VideoFormatT | HoldsVideoFormatT, value: int, chroma: bool = False) -> float:
     """
-    Scale to an 8-bit value.
+    Scale from an 8-bit value.
 
     :param clip:        Input clip, frame, or value representing a bitdepth.
     :param value:       Value to scale.
-    :param chroma:      Values are chroma ranges, and must be converted as such.
-                        Default: False.
+    :param chroma:      Values are chroma ranges, and must be converted as such. Default: False.
 
-    :return:            Value scaled to 8-bit.
+    :return:            Value scaled to the clip's bit-depth.
     """
 
     fmt = get_video_format(clip)
 
     if fmt.sample_type is vs.FLOAT:
         out = value / 255
 
@@ -38,52 +37,51 @@
             out -= .5
 
         return out
 
     return value << get_depth(fmt) - 8
 
 
-def scale_thresh(
-    thresh: float, clip: VideoFormatT | HoldsVideoFormatT,
-    assume: int | None = None, peak: int | float | None = None
-) -> float:
-    """
-    Scale thresholds from float to int or vice versa.
-
-    :param thresh:              Threshold to scale.
-    :param clip:                Input clip.
-    :param assume:              Assumed bit depth of the treshold.
-                                `None` to automatically detect it.
-    :param peak:                Peak value of the clip.
-
-    :return:                    Scaled value.
-
-    :raises CustomValueError:   Threshold is not positive.
-    """
-
-    import warnings
-
-    warnings.warn(
-        'scale_thresh is buggy and deprecated! Please replace it. It will be removed in the next major update.'
-    )
-
-    fmt = get_video_format(clip)
-
-    if thresh < 0:
-        raise CustomIndexError('Thresholds must be positive!', scale_thresh)
+@overload
+def scale_value(  # type: ignore
+    value: int | float,
+    input_depth: int | VideoFormatT | HoldsVideoFormatT,
+    output_depth: Literal[8, 9, 10, 11, 12, 13, 14, 15, 16, 17, 18, 19, 20, 21, 22, 23, 24, 25, 26, 27, 28, 29, 30, 31],
+    range_in: ColorRangeT = ColorRange.LIMITED,
+    range_out: ColorRangeT | None = None,
+    scale_offsets: bool = False,
+    chroma: bool = False
+) -> int:
+    ...
 
-    peak = get_peak_value(fmt, False) if peak is None else peak
 
-    if fmt.sample_type == vs.FLOAT or thresh > 1 and not assume:
-        return thresh
+@overload
+def scale_value(
+    value: int | float,
+    input_depth: int | VideoFormatT | HoldsVideoFormatT,
+    output_depth: Literal[32],
+    range_in: ColorRangeT = ColorRange.LIMITED,
+    range_out: ColorRangeT | None = None,
+    scale_offsets: bool = False,
+    chroma: bool = False
+) -> float:
+    ...
 
-    if assume:
-        return round(thresh / (get_peak_value(assume) * peak))
 
-    return round(thresh * peak)
+@overload
+def scale_value(
+    value: int | float,
+    input_depth: int | VideoFormatT | HoldsVideoFormatT,
+    output_depth: int | VideoFormatT | HoldsVideoFormatT,
+    range_in: ColorRangeT = ColorRange.LIMITED,
+    range_out: ColorRangeT | None = None,
+    scale_offsets: bool = False,
+    chroma: bool = False
+) -> float:
+    ...
 
 
 def scale_value(
     value: int | float,
     input_depth: int | VideoFormatT | HoldsVideoFormatT,
     output_depth: int | VideoFormatT | HoldsVideoFormatT,
     range_in: ColorRangeT = ColorRange.LIMITED,
```

### Comparing `vstools-2.0.6/vstools/utils/vs_enums.py` & `vstools-2.1.0/vstools/utils/vs_enums.py`

 * *Files identical despite different names*

### Comparing `vstools-2.0.6/vstools/utils/vs_proxy.py` & `vstools-2.1.0/vstools/utils/vs_proxy.py`

 * *Files 2% similar despite different names*

```diff
@@ -356,24 +356,14 @@
     return core
 
 
 class VSCoreProxy(CoreProxyBase):
     """Class for wrapping a VapourSynth core."""
 
     def __init__(self, core: Core | None = None) -> None:
-        """
-        Obtain the color range of a clip from the frame properties.
-
-        :param src:                         Input clip, frame, or props.
-        :param strict:                      Be strict about the properties.
-                                            Sets the ColorRange as MISSING if prop is not there.
-
-        :return:                            ColorRange object.
-        """
-
         self._own_core = core is not None
         self._core = core and weakref.ref(core)
 
     def __getattr__(self, name: str) -> Plugin:
         return getattr(_get_core_with_cb(self), name)  # type: ignore
 
     @property
```

### Comparing `vstools-2.0.6/vstools.egg-info/PKG-INFO` & `vstools-2.1.0/vstools.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vstools
-Version: 2.0.6
+Version: 2.1.0
 Summary: Functions and utils related to VapourSynth
 Author: Setsugen no ao
 Author-email: setsugen@setsugen.dev
 Maintainer: Setsugen no ao
 Maintainer-email: setsugen@setsugen.dev
 Project-URL: Source Code, https://github.com/Irrational-Encoding-Wizardry/vs-tools
 Project-URL: Documentation, https://vstools.encoding.moe/en/latest/
```

### Comparing `vstools-2.0.6/vstools.egg-info/SOURCES.txt` & `vstools-2.1.0/vstools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

