# Comparing `tmp/py-Ayiin-0.2.5.tar.gz` & `tmp/py-Ayiin-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py-Ayiin-0.2.5.tar", last modified: Wed May  3 15:59:58 2023, max compression
+gzip compressed data, was "py-Ayiin-0.2.6.tar", last modified: Thu May  4 05:33:24 2023, max compression
```

## Comparing `py-Ayiin-0.2.5.tar` & `py-Ayiin-0.2.6.tar`

### file list

```diff
@@ -1,76 +1,76 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:59:58.464795 py-Ayiin-0.2.5/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-03 15:59:47.000000 py-Ayiin-0.2.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-05-03 15:59:47.000000 py-Ayiin-0.2.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      775 2023-05-03 15:59:47.000000 py-Ayiin-0.2.5/NOTICE
--rw-r--r--   0 runner    (1001) docker     (123)     2403 2023-05-03 15:59:58.464795 py-Ayiin-0.2.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1479 2023-05-03 15:59:47.000000 py-Ayiin-0.2.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:59:58.456795 py-Ayiin-0.2.5/pyAyiin/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:59:58.460795 py-Ayiin-0.2.5/pyAyiin/Clients/
--rw-r--r--   0 runner    (1001) docker     (123)      639 2023-05-03 15:59:47.000000 py-Ayiin-0.2.5/pyAyiin/Clients/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12287 2023-05-03 15:59:47.000000 py-Ayiin-0.2.5/pyAyiin/Clients/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    15803 2023-05-03 15:59:47.000000 py-Ayiin-0.2.5/pyAyiin/Clients/pytgcalls.py
--rw-r--r--   0 runner    (1001) docker     (123)    38206 2023-05-03 15:59:47.000000 py-Ayiin-0.2.5/pyAyiin/Clients/startup.py
--rw-r--r--   0 runner    (1001) docker     (123)     3704 2023-05-03 15:59:47.000000 py-Ayiin-0.2.5/pyAyiin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1465 2023-05-03 15:59:47.000000 py-Ayiin-0.2.5/pyAyiin/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6208 2023-05-03 15:59:47.000000 py-Ayiin-0.2.5/pyAyiin/assistant.py
--rw-r--r--   0 runner    (1001) docker     (123)     5043 2023-05-03 15:59:47.000000 py-Ayiin-0.2.5/pyAyiin/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:59:58.460795 py-Ayiin-0.2.5/pyAyiin/dB/
--rw-r--r--   0 runner    (1001) docker     (123)     1388 2023-05-03 15:59:47.000000 py-Ayiin-0.2.5/pyAyiin/dB/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      170 2023-05-03 15:59:47.000000 py-Ayiin-0.2.5/pyAyiin/dB/_core.py
--rw-r--r--   0 runner    (1001) docker     (123)     1330 2023-05-03 15:59:47.000000 py-Ayiin-0.2.5/pyAyiin/dB/absen.py
--rw-r--r--   0 runner    (1001) docker     (123)      816 2023-05-03 15:59:47.000000 py-Ayiin-0.2.5/pyAyiin/dB/admins.py
--rw-r--r--   0 runner    (1001) docker     (123)     2255 2023-05-03 15:59:47.000000 py-Ayiin-0.2.5/pyAyiin/dB/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)     1406 2023-05-03 15:59:47.000000 py-Ayiin-0.2.5/pyAyiin/dB/blacklistfilter.py
--rw-r--r--   0 runner    (1001) docker     (123)      783 2023-05-03 15:59:47.000000 py-Ayiin-0.2.5/pyAyiin/dB/blacklistuser.py
--rw-r--r--   0 runner    (1001) docker     (123)      706 2023-05-03 15:59:47.000000 py-Ayiin-0.2.5/pyAyiin/dB/gban.py
--rw-r--r--   0 runner    (1001) docker     (123)      560 2023-05-03 15:59:47.000000 py-Ayiin-0.2.5/pyAyiin/dB/langs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1029 2023-05-03 15:59:47.000000 py-Ayiin-0.2.5/pyAyiin/dB/logdb.py
--rw-r--r--   0 runner    (1001) docker     (123)      621 2023-05-03 15:59:47.000000 py-Ayiin-0.2.5/pyAyiin/dB/pmpermit.py
--rw-r--r--   0 runner    (1001) docker     (123)     1332 2023-05-03 15:59:47.000000 py-Ayiin-0.2.5/pyAyiin/dB/premium.py
--rw-r--r--   0 runner    (1001) docker     (123)      914 2023-05-03 15:59:47.000000 py-Ayiin-0.2.5/pyAyiin/dB/start.py
--rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-05-03 15:59:47.000000 py-Ayiin-0.2.5/pyAyiin/dB/sudo.py
--rw-r--r--   0 runner    (1001) docker     (123)      746 2023-05-03 15:59:47.000000 py-Ayiin-0.2.5/pyAyiin/dB/variable.py
--rw-r--r--   0 runner    (1001) docker     (123)     1251 2023-05-03 15:59:47.000000 py-Ayiin-0.2.5/pyAyiin/dB/videocalls.py
--rw-r--r--   0 runner    (1001) docker     (123)     2012 2023-05-03 15:59:47.000000 py-Ayiin-0.2.5/pyAyiin/dB/welcome.py
--rw-r--r--   0 runner    (1001) docker     (123)    33254 2023-05-03 15:59:47.000000 py-Ayiin-0.2.5/pyAyiin/decorator.py
--rw-r--r--   0 runner    (1001) docker     (123)      959 2023-05-03 15:59:47.000000 py-Ayiin-0.2.5/pyAyiin/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:59:58.460795 py-Ayiin-0.2.5/pyAyiin/methods/
--rw-r--r--   0 runner    (1001) docker     (123)      923 2023-05-03 15:59:47.000000 py-Ayiin-0.2.5/pyAyiin/methods/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3935 2023-05-03 15:59:47.000000 py-Ayiin-0.2.5/pyAyiin/methods/_misc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1897 2023-05-03 15:59:47.000000 py-Ayiin-0.2.5/pyAyiin/methods/changer.py
--rw-r--r--   0 runner    (1001) docker     (123)      853 2023-05-03 15:59:47.000000 py-Ayiin-0.2.5/pyAyiin/methods/converter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2813 2023-05-03 15:59:47.000000 py-Ayiin-0.2.5/pyAyiin/methods/func.py
--rw-r--r--   0 runner    (1001) docker     (123)     2274 2023-05-03 15:59:47.000000 py-Ayiin-0.2.5/pyAyiin/methods/funcb.py
--rw-r--r--   0 runner    (1001) docker     (123)     8828 2023-05-03 15:59:47.000000 py-Ayiin-0.2.5/pyAyiin/methods/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1213 2023-05-03 15:59:47.000000 py-Ayiin-0.2.5/pyAyiin/methods/hosting.py
--rw-r--r--   0 runner    (1001) docker     (123)     3658 2023-05-03 15:59:47.000000 py-Ayiin-0.2.5/pyAyiin/methods/inlinebot.py
--rw-r--r--   0 runner    (1001) docker     (123)     2911 2023-05-03 15:59:47.000000 py-Ayiin-0.2.5/pyAyiin/methods/queue.py
--rw-r--r--   0 runner    (1001) docker     (123)     5704 2023-05-03 15:59:47.000000 py-Ayiin-0.2.5/pyAyiin/methods/thumbnail.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:59:58.460795 py-Ayiin-0.2.5/pyAyiin/pyrogram/
--rw-r--r--   0 runner    (1001) docker     (123)      626 2023-05-03 15:59:47.000000 py-Ayiin-0.2.5/pyAyiin/pyrogram/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2446 2023-05-03 15:59:47.000000 py-Ayiin-0.2.5/pyAyiin/pyrogram/_wrappers.py
--rw-r--r--   0 runner    (1001) docker     (123)     8164 2023-05-03 15:59:47.000000 py-Ayiin-0.2.5/pyAyiin/pyrogram/func.py
--rw-r--r--   0 runner    (1001) docker     (123)     3559 2023-05-03 15:59:47.000000 py-Ayiin-0.2.5/pyAyiin/pyrogram/misc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1734 2023-05-03 15:59:47.000000 py-Ayiin-0.2.5/pyAyiin/pyrogram/pastebin.py
--rw-r--r--   0 runner    (1001) docker     (123)      832 2023-05-03 15:59:47.000000 py-Ayiin-0.2.5/pyAyiin/pyrogram/sections.py
--rw-r--r--   0 runner    (1001) docker     (123)     2138 2023-05-03 15:59:47.000000 py-Ayiin-0.2.5/pyAyiin/pyrogram/toolbot.py
--rw-r--r--   0 runner    (1001) docker     (123)     8684 2023-05-03 15:59:47.000000 py-Ayiin-0.2.5/pyAyiin/pyrogram/tools.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:59:58.460795 py-Ayiin-0.2.5/pyAyiin/resources/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 15:59:47.000000 py-Ayiin-0.2.5/pyAyiin/resources/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:59:58.460795 py-Ayiin-0.2.5/pyAyiin/telethon/
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-05-03 15:59:47.000000 py-Ayiin-0.2.5/pyAyiin/telethon/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:59:58.464795 py-Ayiin-0.2.5/pyAyiin/telethon/ayiin/
--rw-r--r--   0 runner    (1001) docker     (123)      152 2023-05-03 15:59:47.000000 py-Ayiin-0.2.5/pyAyiin/telethon/ayiin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1803 2023-05-03 15:59:47.000000 py-Ayiin-0.2.5/pyAyiin/telethon/ayiin/_wrappers.py
--rw-r--r--   0 runner    (1001) docker     (123)     3848 2023-05-03 15:59:47.000000 py-Ayiin-0.2.5/pyAyiin/telethon/ayiin/events.py
--rw-r--r--   0 runner    (1001) docker     (123)     6803 2023-05-03 15:59:47.000000 py-Ayiin-0.2.5/pyAyiin/telethon/ayiin/misc.py
--rw-r--r--   0 runner    (1001) docker     (123)    16802 2023-05-03 15:59:47.000000 py-Ayiin-0.2.5/pyAyiin/xd.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:59:58.464795 py-Ayiin-0.2.5/py_Ayiin.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2403 2023-05-03 15:59:58.000000 py-Ayiin-0.2.5/py_Ayiin.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1551 2023-05-03 15:59:58.000000 py-Ayiin-0.2.5/py_Ayiin.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-03 15:59:58.000000 py-Ayiin-0.2.5/py_Ayiin.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      146 2023-05-03 15:59:58.000000 py-Ayiin-0.2.5/py_Ayiin.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-03 15:59:58.000000 py-Ayiin-0.2.5/py_Ayiin.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      146 2023-05-03 15:59:47.000000 py-Ayiin-0.2.5/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-03 15:59:58.464795 py-Ayiin-0.2.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1641 2023-05-03 15:59:47.000000 py-Ayiin-0.2.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 05:33:24.153133 py-Ayiin-0.2.6/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-04 05:33:13.000000 py-Ayiin-0.2.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-05-04 05:33:13.000000 py-Ayiin-0.2.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      775 2023-05-04 05:33:13.000000 py-Ayiin-0.2.6/NOTICE
+-rw-r--r--   0 runner    (1001) docker     (123)     2403 2023-05-04 05:33:24.153133 py-Ayiin-0.2.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1479 2023-05-04 05:33:13.000000 py-Ayiin-0.2.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 05:33:24.149133 py-Ayiin-0.2.6/pyAyiin/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 05:33:24.149133 py-Ayiin-0.2.6/pyAyiin/Clients/
+-rw-r--r--   0 runner    (1001) docker     (123)      639 2023-05-04 05:33:13.000000 py-Ayiin-0.2.6/pyAyiin/Clients/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12287 2023-05-04 05:33:13.000000 py-Ayiin-0.2.6/pyAyiin/Clients/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15803 2023-05-04 05:33:13.000000 py-Ayiin-0.2.6/pyAyiin/Clients/pytgcalls.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38206 2023-05-04 05:33:13.000000 py-Ayiin-0.2.6/pyAyiin/Clients/startup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3704 2023-05-04 05:33:13.000000 py-Ayiin-0.2.6/pyAyiin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1465 2023-05-04 05:33:13.000000 py-Ayiin-0.2.6/pyAyiin/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6208 2023-05-04 05:33:13.000000 py-Ayiin-0.2.6/pyAyiin/assistant.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5043 2023-05-04 05:33:13.000000 py-Ayiin-0.2.6/pyAyiin/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 05:33:24.149133 py-Ayiin-0.2.6/pyAyiin/dB/
+-rw-r--r--   0 runner    (1001) docker     (123)     1388 2023-05-04 05:33:13.000000 py-Ayiin-0.2.6/pyAyiin/dB/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      170 2023-05-04 05:33:13.000000 py-Ayiin-0.2.6/pyAyiin/dB/_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1330 2023-05-04 05:33:13.000000 py-Ayiin-0.2.6/pyAyiin/dB/absen.py
+-rw-r--r--   0 runner    (1001) docker     (123)      816 2023-05-04 05:33:13.000000 py-Ayiin-0.2.6/pyAyiin/dB/admins.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2255 2023-05-04 05:33:13.000000 py-Ayiin-0.2.6/pyAyiin/dB/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1406 2023-05-04 05:33:13.000000 py-Ayiin-0.2.6/pyAyiin/dB/blacklistfilter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      783 2023-05-04 05:33:13.000000 py-Ayiin-0.2.6/pyAyiin/dB/blacklistuser.py
+-rw-r--r--   0 runner    (1001) docker     (123)      706 2023-05-04 05:33:13.000000 py-Ayiin-0.2.6/pyAyiin/dB/gban.py
+-rw-r--r--   0 runner    (1001) docker     (123)      560 2023-05-04 05:33:13.000000 py-Ayiin-0.2.6/pyAyiin/dB/langs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1029 2023-05-04 05:33:13.000000 py-Ayiin-0.2.6/pyAyiin/dB/logdb.py
+-rw-r--r--   0 runner    (1001) docker     (123)      621 2023-05-04 05:33:13.000000 py-Ayiin-0.2.6/pyAyiin/dB/pmpermit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1332 2023-05-04 05:33:13.000000 py-Ayiin-0.2.6/pyAyiin/dB/premium.py
+-rw-r--r--   0 runner    (1001) docker     (123)      914 2023-05-04 05:33:13.000000 py-Ayiin-0.2.6/pyAyiin/dB/start.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-05-04 05:33:13.000000 py-Ayiin-0.2.6/pyAyiin/dB/sudo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      746 2023-05-04 05:33:13.000000 py-Ayiin-0.2.6/pyAyiin/dB/variable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1251 2023-05-04 05:33:13.000000 py-Ayiin-0.2.6/pyAyiin/dB/videocalls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2012 2023-05-04 05:33:13.000000 py-Ayiin-0.2.6/pyAyiin/dB/welcome.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33254 2023-05-04 05:33:13.000000 py-Ayiin-0.2.6/pyAyiin/decorator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      959 2023-05-04 05:33:13.000000 py-Ayiin-0.2.6/pyAyiin/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 05:33:24.149133 py-Ayiin-0.2.6/pyAyiin/methods/
+-rw-r--r--   0 runner    (1001) docker     (123)      923 2023-05-04 05:33:13.000000 py-Ayiin-0.2.6/pyAyiin/methods/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3939 2023-05-04 05:33:13.000000 py-Ayiin-0.2.6/pyAyiin/methods/_misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1897 2023-05-04 05:33:13.000000 py-Ayiin-0.2.6/pyAyiin/methods/changer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      853 2023-05-04 05:33:13.000000 py-Ayiin-0.2.6/pyAyiin/methods/converter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2813 2023-05-04 05:33:13.000000 py-Ayiin-0.2.6/pyAyiin/methods/func.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2274 2023-05-04 05:33:13.000000 py-Ayiin-0.2.6/pyAyiin/methods/funcb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8828 2023-05-04 05:33:13.000000 py-Ayiin-0.2.6/pyAyiin/methods/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1213 2023-05-04 05:33:13.000000 py-Ayiin-0.2.6/pyAyiin/methods/hosting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3658 2023-05-04 05:33:13.000000 py-Ayiin-0.2.6/pyAyiin/methods/inlinebot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2911 2023-05-04 05:33:13.000000 py-Ayiin-0.2.6/pyAyiin/methods/queue.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5704 2023-05-04 05:33:13.000000 py-Ayiin-0.2.6/pyAyiin/methods/thumbnail.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 05:33:24.153133 py-Ayiin-0.2.6/pyAyiin/pyrogram/
+-rw-r--r--   0 runner    (1001) docker     (123)      626 2023-05-04 05:33:13.000000 py-Ayiin-0.2.6/pyAyiin/pyrogram/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2446 2023-05-04 05:33:13.000000 py-Ayiin-0.2.6/pyAyiin/pyrogram/_wrappers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8164 2023-05-04 05:33:13.000000 py-Ayiin-0.2.6/pyAyiin/pyrogram/func.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3559 2023-05-04 05:33:13.000000 py-Ayiin-0.2.6/pyAyiin/pyrogram/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1734 2023-05-04 05:33:13.000000 py-Ayiin-0.2.6/pyAyiin/pyrogram/pastebin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      832 2023-05-04 05:33:13.000000 py-Ayiin-0.2.6/pyAyiin/pyrogram/sections.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2138 2023-05-04 05:33:13.000000 py-Ayiin-0.2.6/pyAyiin/pyrogram/toolbot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8684 2023-05-04 05:33:13.000000 py-Ayiin-0.2.6/pyAyiin/pyrogram/tools.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 05:33:24.153133 py-Ayiin-0.2.6/pyAyiin/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 05:33:13.000000 py-Ayiin-0.2.6/pyAyiin/resources/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 05:33:24.153133 py-Ayiin-0.2.6/pyAyiin/telethon/
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-05-04 05:33:13.000000 py-Ayiin-0.2.6/pyAyiin/telethon/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 05:33:24.153133 py-Ayiin-0.2.6/pyAyiin/telethon/ayiin/
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-05-04 05:33:13.000000 py-Ayiin-0.2.6/pyAyiin/telethon/ayiin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1803 2023-05-04 05:33:13.000000 py-Ayiin-0.2.6/pyAyiin/telethon/ayiin/_wrappers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3848 2023-05-04 05:33:13.000000 py-Ayiin-0.2.6/pyAyiin/telethon/ayiin/events.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6803 2023-05-04 05:33:13.000000 py-Ayiin-0.2.6/pyAyiin/telethon/ayiin/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16802 2023-05-04 05:33:13.000000 py-Ayiin-0.2.6/pyAyiin/xd.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 05:33:24.153133 py-Ayiin-0.2.6/py_Ayiin.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2403 2023-05-04 05:33:24.000000 py-Ayiin-0.2.6/py_Ayiin.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1551 2023-05-04 05:33:24.000000 py-Ayiin-0.2.6/py_Ayiin.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 05:33:24.000000 py-Ayiin-0.2.6/py_Ayiin.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-05-04 05:33:24.000000 py-Ayiin-0.2.6/py_Ayiin.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-04 05:33:24.000000 py-Ayiin-0.2.6/py_Ayiin.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-05-04 05:33:13.000000 py-Ayiin-0.2.6/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-04 05:33:24.153133 py-Ayiin-0.2.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1641 2023-05-04 05:33:13.000000 py-Ayiin-0.2.6/setup.py
```

### Comparing `py-Ayiin-0.2.5/LICENSE` & `py-Ayiin-0.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.2.5/NOTICE` & `py-Ayiin-0.2.6/NOTICE`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.2.5/PKG-INFO` & `py-Ayiin-0.2.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-Ayiin
-Version: 0.2.5
+Version: 0.2.6
 Summary: A Secure and Powerful Python-Telethon Based and Python-Pyrogram Based Library For Your Userbot Module.
 Home-page: https://github.com/AyiinXd/AyiinXd
 Author: AyiinXd
 Author-email: ayingaming98@gmail.com
 License: GNU General Public License v3.0 (GPL-3.0)
 Project-URL: Bug Tracker, https://github.com/AyiinXd/AyiinXd/issues
 Project-URL: Source Code, https://github.com/AyiinXd/AyiinXd
```

### Comparing `py-Ayiin-0.2.5/README.md` & `py-Ayiin-0.2.6/README.md`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.2.5/pyAyiin/Clients/__init__.py` & `py-Ayiin-0.2.6/pyAyiin/Clients/__init__.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.2.5/pyAyiin/Clients/client.py` & `py-Ayiin-0.2.6/pyAyiin/Clients/client.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.2.5/pyAyiin/Clients/pytgcalls.py` & `py-Ayiin-0.2.6/pyAyiin/Clients/pytgcalls.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.2.5/pyAyiin/Clients/startup.py` & `py-Ayiin-0.2.6/pyAyiin/Clients/startup.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.2.5/pyAyiin/__init__.py` & `py-Ayiin-0.2.6/pyAyiin/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -40,15 +40,15 @@
 
 
 logs = logging.getLogger(__name__)
 
 
 __copyright__ = "Copyright (C) 2022-present AyiinXd <https://github.com/AyiinXd>"
 __license__ = "GNU General Public License v3.0 (GPL-3.0)"
-__version__ = "0.2.5"
+__version__ = "0.2.6"
 ayiin_ver = "0.0.9"
 
 
 DEVS = [
     607067484, # Ayiin
     997461844, #Ayang_Ayiin
     2130526178, # Alfa
```

### Comparing `py-Ayiin-0.2.5/pyAyiin/__main__.py` & `py-Ayiin-0.2.6/pyAyiin/__main__.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.2.5/pyAyiin/assistant.py` & `py-Ayiin-0.2.6/pyAyiin/assistant.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.2.5/pyAyiin/config.py` & `py-Ayiin-0.2.6/pyAyiin/config.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.2.5/pyAyiin/dB/__init__.py` & `py-Ayiin-0.2.6/pyAyiin/dB/__init__.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.2.5/pyAyiin/dB/absen.py` & `py-Ayiin-0.2.6/pyAyiin/dB/absen.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.2.5/pyAyiin/dB/admins.py` & `py-Ayiin-0.2.6/pyAyiin/dB/admins.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.2.5/pyAyiin/dB/auth.py` & `py-Ayiin-0.2.6/pyAyiin/dB/auth.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.2.5/pyAyiin/dB/blacklistfilter.py` & `py-Ayiin-0.2.6/pyAyiin/dB/blacklistfilter.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.2.5/pyAyiin/dB/blacklistuser.py` & `py-Ayiin-0.2.6/pyAyiin/dB/blacklistuser.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.2.5/pyAyiin/dB/gban.py` & `py-Ayiin-0.2.6/pyAyiin/dB/gban.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.2.5/pyAyiin/dB/langs.py` & `py-Ayiin-0.2.6/pyAyiin/dB/langs.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.2.5/pyAyiin/dB/logdb.py` & `py-Ayiin-0.2.6/pyAyiin/dB/logdb.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.2.5/pyAyiin/dB/pmpermit.py` & `py-Ayiin-0.2.6/pyAyiin/dB/pmpermit.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.2.5/pyAyiin/dB/premium.py` & `py-Ayiin-0.2.6/pyAyiin/dB/premium.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.2.5/pyAyiin/dB/start.py` & `py-Ayiin-0.2.6/pyAyiin/dB/start.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.2.5/pyAyiin/dB/sudo.py` & `py-Ayiin-0.2.6/pyAyiin/dB/sudo.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.2.5/pyAyiin/dB/variable.py` & `py-Ayiin-0.2.6/pyAyiin/dB/variable.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.2.5/pyAyiin/dB/videocalls.py` & `py-Ayiin-0.2.6/pyAyiin/dB/videocalls.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.2.5/pyAyiin/dB/welcome.py` & `py-Ayiin-0.2.6/pyAyiin/dB/welcome.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.2.5/pyAyiin/decorator.py` & `py-Ayiin-0.2.6/pyAyiin/decorator.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.2.5/pyAyiin/exceptions.py` & `py-Ayiin-0.2.6/pyAyiin/exceptions.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.2.5/pyAyiin/methods/__init__.py` & `py-Ayiin-0.2.6/pyAyiin/methods/__init__.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.2.5/pyAyiin/methods/_misc.py` & `py-Ayiin-0.2.6/pyAyiin/methods/_misc.py`

 * *Files 1% similar despite different names*

```diff
@@ -97,15 +97,15 @@
                 title="Found Peer.",
                 input_message_content=InputTextMessageContent(
                     caption, disable_web_page_preview=True
                 ),
             )
         )
     
-    def heroku():
+    def heroku(self):
         from pyAyiin import logs
         
         if HOSTED_ON == "Heroku":
             if var.HEROKU_API and var.HEROKU_APP_NAME:
                 try:
                     Heroku = heroku3.from_key(var.HEROKU_API)
                     HAPP = Heroku.app(var.HEROKU_APP_NAME)
```

### Comparing `py-Ayiin-0.2.5/pyAyiin/methods/changer.py` & `py-Ayiin-0.2.6/pyAyiin/methods/changer.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.2.5/pyAyiin/methods/converter.py` & `py-Ayiin-0.2.6/pyAyiin/methods/converter.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.2.5/pyAyiin/methods/func.py` & `py-Ayiin-0.2.6/pyAyiin/methods/func.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.2.5/pyAyiin/methods/funcb.py` & `py-Ayiin-0.2.6/pyAyiin/methods/funcb.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.2.5/pyAyiin/methods/helpers.py` & `py-Ayiin-0.2.6/pyAyiin/methods/helpers.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.2.5/pyAyiin/methods/hosting.py` & `py-Ayiin-0.2.6/pyAyiin/methods/hosting.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.2.5/pyAyiin/methods/inlinebot.py` & `py-Ayiin-0.2.6/pyAyiin/methods/inlinebot.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.2.5/pyAyiin/methods/queue.py` & `py-Ayiin-0.2.6/pyAyiin/methods/queue.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.2.5/pyAyiin/methods/thumbnail.py` & `py-Ayiin-0.2.6/pyAyiin/methods/thumbnail.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.2.5/pyAyiin/pyrogram/__init__.py` & `py-Ayiin-0.2.6/pyAyiin/pyrogram/__init__.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.2.5/pyAyiin/pyrogram/_wrappers.py` & `py-Ayiin-0.2.6/pyAyiin/pyrogram/_wrappers.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.2.5/pyAyiin/pyrogram/func.py` & `py-Ayiin-0.2.6/pyAyiin/pyrogram/func.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.2.5/pyAyiin/pyrogram/misc.py` & `py-Ayiin-0.2.6/pyAyiin/pyrogram/misc.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.2.5/pyAyiin/pyrogram/pastebin.py` & `py-Ayiin-0.2.6/pyAyiin/pyrogram/pastebin.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.2.5/pyAyiin/pyrogram/sections.py` & `py-Ayiin-0.2.6/pyAyiin/pyrogram/sections.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.2.5/pyAyiin/pyrogram/toolbot.py` & `py-Ayiin-0.2.6/pyAyiin/pyrogram/toolbot.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.2.5/pyAyiin/pyrogram/tools.py` & `py-Ayiin-0.2.6/pyAyiin/pyrogram/tools.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.2.5/pyAyiin/telethon/ayiin/_wrappers.py` & `py-Ayiin-0.2.6/pyAyiin/telethon/ayiin/_wrappers.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.2.5/pyAyiin/telethon/ayiin/events.py` & `py-Ayiin-0.2.6/pyAyiin/telethon/ayiin/events.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.2.5/pyAyiin/telethon/ayiin/misc.py` & `py-Ayiin-0.2.6/pyAyiin/telethon/ayiin/misc.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.2.5/pyAyiin/xd.py` & `py-Ayiin-0.2.6/pyAyiin/xd.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.2.5/py_Ayiin.egg-info/PKG-INFO` & `py-Ayiin-0.2.6/py_Ayiin.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-Ayiin
-Version: 0.2.5
+Version: 0.2.6
 Summary: A Secure and Powerful Python-Telethon Based and Python-Pyrogram Based Library For Your Userbot Module.
 Home-page: https://github.com/AyiinXd/AyiinXd
 Author: AyiinXd
 Author-email: ayingaming98@gmail.com
 License: GNU General Public License v3.0 (GPL-3.0)
 Project-URL: Bug Tracker, https://github.com/AyiinXd/AyiinXd/issues
 Project-URL: Source Code, https://github.com/AyiinXd/AyiinXd
```

### Comparing `py-Ayiin-0.2.5/py_Ayiin.egg-info/SOURCES.txt` & `py-Ayiin-0.2.6/py_Ayiin.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.2.5/setup.py` & `py-Ayiin-0.2.6/setup.py`

 * *Files identical despite different names*

