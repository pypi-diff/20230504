# Comparing `tmp/material_zui-0.0.4.tar.gz` & `tmp/material_zui-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "material_zui-0.0.4.tar", last modified: Thu May  4 07:38:15 2023, max compression
+gzip compressed data, was "material_zui-0.0.5.tar", last modified: Thu May  4 09:24:52 2023, max compression
```

## Comparing `material_zui-0.0.4.tar` & `material_zui-0.0.5.tar`

### file list

```diff
@@ -1,47 +1,9 @@
-drwxrwxr-x   0 chaunguyen  (1001) chaunguyen  (1001)        0 2023-05-04 07:38:15.903938 material_zui-0.0.4/
--rw-rw-r--   0 chaunguyen  (1001) chaunguyen  (1001)      710 2023-05-04 07:38:15.903938 material_zui-0.0.4/PKG-INFO
-drwxrwxr-x   0 chaunguyen  (1001) chaunguyen  (1001)        0 2023-05-04 07:38:15.891938 material_zui-0.0.4/crawl/
--rw-rw-r--   0 chaunguyen  (1001) chaunguyen  (1001)       36 2023-05-02 13:44:44.000000 material_zui-0.0.4/crawl/__init__.py
--rw-rw-r--   0 chaunguyen  (1001) chaunguyen  (1001)        0 2023-05-02 13:44:44.000000 material_zui-0.0.4/crawl/index.py
-drwxrwxr-x   0 chaunguyen  (1001) chaunguyen  (1001)        0 2023-05-04 07:38:15.895938 material_zui-0.0.4/image/
--rw-rw-r--   0 chaunguyen  (1001) chaunguyen  (1001)      162 2023-05-03 05:30:05.000000 material_zui-0.0.4/image/__init__.py
--rw-rw-r--   0 chaunguyen  (1001) chaunguyen  (1001)     1445 2023-05-03 14:42:30.000000 material_zui-0.0.4/image/combine.py
--rw-rw-r--   0 chaunguyen  (1001) chaunguyen  (1001)     1904 2023-05-03 05:27:27.000000 material_zui-0.0.4/image/convert.py
--rw-rw-r--   0 chaunguyen  (1001) chaunguyen  (1001)       78 2023-04-28 09:55:18.000000 material_zui-0.0.4/image/data.py
--rw-rw-r--   0 chaunguyen  (1001) chaunguyen  (1001)     1755 2023-05-03 05:42:32.000000 material_zui-0.0.4/image/index.py
--rw-rw-r--   0 chaunguyen  (1001) chaunguyen  (1001)      801 2023-04-29 15:11:22.000000 material_zui-0.0.4/image/remove_background.py
--rw-rw-r--   0 chaunguyen  (1001) chaunguyen  (1001)      278 2023-04-29 15:11:37.000000 material_zui-0.0.4/image/transparent_background.py
--rw-rw-r--   0 chaunguyen  (1001) chaunguyen  (1001)      249 2023-04-28 09:24:02.000000 material_zui-0.0.4/image/type.py
--rw-rw-r--   0 chaunguyen  (1001) chaunguyen  (1001)     4458 2023-05-03 14:24:10.000000 material_zui-0.0.4/image/upscale.py
-drwxrwxr-x   0 chaunguyen  (1001) chaunguyen  (1001)        0 2023-05-04 07:38:15.895938 material_zui-0.0.4/language_model/
--rw-rw-r--   0 chaunguyen  (1001) chaunguyen  (1001)       48 2023-05-02 05:21:47.000000 material_zui-0.0.4/language_model/__init__.py
--rw-rw-r--   0 chaunguyen  (1001) chaunguyen  (1001)      987 2023-05-02 05:36:54.000000 material_zui-0.0.4/language_model/index.py
-drwxrwxr-x   0 chaunguyen  (1001) chaunguyen  (1001)        0 2023-05-04 07:38:15.895938 material_zui-0.0.4/log/
--rw-rw-r--   0 chaunguyen  (1001) chaunguyen  (1001)       37 2023-04-30 11:48:06.000000 material_zui-0.0.4/log/__init__.py
--rw-rw-r--   0 chaunguyen  (1001) chaunguyen  (1001)      858 2023-04-28 04:39:06.000000 material_zui-0.0.4/log/index.py
-drwxrwxr-x   0 chaunguyen  (1001) chaunguyen  (1001)        0 2023-05-04 07:38:15.899938 material_zui-0.0.4/material_zui.egg-info/
--rw-rw-r--   0 chaunguyen  (1001) chaunguyen  (1001)      710 2023-05-04 07:38:15.000000 material_zui-0.0.4/material_zui.egg-info/PKG-INFO
--rw-rw-r--   0 chaunguyen  (1001) chaunguyen  (1001)      691 2023-05-04 07:38:15.000000 material_zui-0.0.4/material_zui.egg-info/SOURCES.txt
--rw-rw-r--   0 chaunguyen  (1001) chaunguyen  (1001)        1 2023-05-04 07:38:15.000000 material_zui-0.0.4/material_zui.egg-info/dependency_links.txt
--rw-rw-r--   0 chaunguyen  (1001) chaunguyen  (1001)        8 2023-05-04 07:38:15.000000 material_zui-0.0.4/material_zui.egg-info/requires.txt
--rw-rw-r--   0 chaunguyen  (1001) chaunguyen  (1001)       78 2023-05-04 07:38:15.000000 material_zui-0.0.4/material_zui.egg-info/top_level.txt
-drwxrwxr-x   0 chaunguyen  (1001) chaunguyen  (1001)        0 2023-05-04 07:38:15.899938 material_zui-0.0.4/regex/
--rw-rw-r--   0 chaunguyen  (1001) chaunguyen  (1001)       39 2023-05-02 05:15:13.000000 material_zui-0.0.4/regex/__init__.py
--rw-rw-r--   0 chaunguyen  (1001) chaunguyen  (1001)     5344 2023-05-02 05:18:47.000000 material_zui-0.0.4/regex/index.py
-drwxrwxr-x   0 chaunguyen  (1001) chaunguyen  (1001)        0 2023-05-04 07:38:15.899938 material_zui-0.0.4/replicate/
--rw-rw-r--   0 chaunguyen  (1001) chaunguyen  (1001)       43 2023-04-30 11:47:27.000000 material_zui-0.0.4/replicate/__init__.py
--rw-rw-r--   0 chaunguyen  (1001) chaunguyen  (1001)     2481 2023-05-01 15:33:18.000000 material_zui-0.0.4/replicate/index.py
--rw-rw-r--   0 chaunguyen  (1001) chaunguyen  (1001)       38 2023-05-04 07:38:15.903938 material_zui-0.0.4/setup.cfg
--rw-rw-r--   0 chaunguyen  (1001) chaunguyen  (1001)      864 2023-05-04 07:36:57.000000 material_zui-0.0.4/setup.py
-drwxrwxr-x   0 chaunguyen  (1001) chaunguyen  (1001)        0 2023-05-04 07:38:15.899938 material_zui-0.0.4/telegram_bot/
--rw-rw-r--   0 chaunguyen  (1001) chaunguyen  (1001)       46 2023-05-02 13:44:38.000000 material_zui-0.0.4/telegram_bot/__init__.py
--rw-rw-r--   0 chaunguyen  (1001) chaunguyen  (1001)      129 2023-05-02 14:08:52.000000 material_zui-0.0.4/telegram_bot/index.py
-drwxrwxr-x   0 chaunguyen  (1001) chaunguyen  (1001)        0 2023-05-04 07:38:15.899938 material_zui-0.0.4/time/
--rw-rw-r--   0 chaunguyen  (1001) chaunguyen  (1001)       38 2023-05-02 14:46:45.000000 material_zui-0.0.4/time/__init__.py
--rw-rw-r--   0 chaunguyen  (1001) chaunguyen  (1001)      692 2023-05-02 15:04:19.000000 material_zui-0.0.4/time/index.py
-drwxrwxr-x   0 chaunguyen  (1001) chaunguyen  (1001)        0 2023-05-04 07:38:15.899938 material_zui-0.0.4/tmp/
--rw-rw-r--   0 chaunguyen  (1001) chaunguyen  (1001)       36 2023-04-30 11:48:06.000000 material_zui-0.0.4/tmp/__init__.py
--rw-rw-r--   0 chaunguyen  (1001) chaunguyen  (1001)        0 2023-04-28 03:39:00.000000 material_zui-0.0.4/tmp/index.py
-drwxrwxr-x   0 chaunguyen  (1001) chaunguyen  (1001)        0 2023-05-04 07:38:15.903938 material_zui-0.0.4/validate/
--rw-rw-r--   0 chaunguyen  (1001) chaunguyen  (1001)       36 2023-05-01 14:11:23.000000 material_zui-0.0.4/validate/__init__.py
--rw-rw-r--   0 chaunguyen  (1001) chaunguyen  (1001)        0 2023-05-01 14:11:23.000000 material_zui-0.0.4/validate/index.py
+drwxrwxr-x   0 chaunguyen  (1001) chaunguyen  (1001)        0 2023-05-04 09:24:52.925284 material_zui-0.0.5/
+-rw-rw-r--   0 chaunguyen  (1001) chaunguyen  (1001)      719 2023-05-04 09:24:52.925284 material_zui-0.0.5/PKG-INFO
+drwxrwxr-x   0 chaunguyen  (1001) chaunguyen  (1001)        0 2023-05-04 09:24:52.925284 material_zui-0.0.5/material_zui.egg-info/
+-rw-rw-r--   0 chaunguyen  (1001) chaunguyen  (1001)      719 2023-05-04 09:24:52.000000 material_zui-0.0.5/material_zui.egg-info/PKG-INFO
+-rw-rw-r--   0 chaunguyen  (1001) chaunguyen  (1001)      178 2023-05-04 09:24:52.000000 material_zui-0.0.5/material_zui.egg-info/SOURCES.txt
+-rw-rw-r--   0 chaunguyen  (1001) chaunguyen  (1001)        1 2023-05-04 09:24:52.000000 material_zui-0.0.5/material_zui.egg-info/dependency_links.txt
+-rw-rw-r--   0 chaunguyen  (1001) chaunguyen  (1001)        8 2023-05-04 09:24:52.000000 material_zui-0.0.5/material_zui.egg-info/requires.txt
+-rw-rw-r--   0 chaunguyen  (1001) chaunguyen  (1001)        1 2023-05-04 09:24:52.000000 material_zui-0.0.5/material_zui.egg-info/top_level.txt
+-rw-rw-r--   0 chaunguyen  (1001) chaunguyen  (1001)       38 2023-05-04 09:24:52.925284 material_zui-0.0.5/setup.cfg
```

