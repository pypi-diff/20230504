# Comparing `tmp/rohdeschwarz-1.9.1.dev1.tar.gz` & `tmp/rohdeschwarz-1.9.2.dev1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rohdeschwarz-1.9.1.dev1.tar", last modified: Thu Aug 19 19:48:03 2021, max compression
+gzip compressed data, was "rohdeschwarz-1.9.2.dev1.tar", last modified: Wed Mar 23 16:14:33 2022, max compression
```

## Comparing `rohdeschwarz-1.9.1.dev1.tar` & `rohdeschwarz-1.9.2.dev1.tar`

### file list

```diff
@@ -1,84 +1,84 @@
-drwxr-xr-x   0 lalic      (501) staff       (20)        0 2021-08-19 19:48:03.390290 rohdeschwarz-1.9.1.dev1/
--rw-r--r--   0 lalic      (501) staff       (20)      209 2020-04-16 06:49:26.000000 rohdeschwarz-1.9.1.dev1/DESCRIPTION.rst
--rw-r--r--   0 lalic      (501) staff       (20)       14 2020-04-16 06:49:26.000000 rohdeschwarz-1.9.1.dev1/MANIFEST.in
--rw-r--r--   0 lalic      (501) staff       (20)     1214 2021-08-19 19:48:03.389817 rohdeschwarz-1.9.1.dev1/PKG-INFO
-drwxr-xr-x   0 lalic      (501) staff       (20)        0 2021-08-19 19:48:03.355723 rohdeschwarz-1.9.1.dev1/rohdeschwarz/
--rw-r--r--   0 lalic      (501) staff       (20)      109 2021-08-19 17:55:23.000000 rohdeschwarz-1.9.1.dev1/rohdeschwarz/__init__.py
-drwxr-xr-x   0 lalic      (501) staff       (20)        0 2021-08-19 19:48:03.361000 rohdeschwarz-1.9.1.dev1/rohdeschwarz/bin/
--rw-r--r--   0 lalic      (501) staff       (20)        0 2020-04-16 06:49:26.000000 rohdeschwarz-1.9.1.dev1/rohdeschwarz/bin/__init__.py
--rwxr-xr-x   0 lalic      (501) staff       (20)     2204 2021-08-19 17:55:23.000000 rohdeschwarz-1.9.1.dev1/rohdeschwarz/bin/instr.py
--rw-r--r--   0 lalic      (501) staff       (20)     2720 2021-08-19 17:55:23.000000 rohdeschwarz-1.9.1.dev1/rohdeschwarz/bin/osp.py
--rwxr-xr-x   0 lalic      (501) staff       (20)     2168 2021-08-19 17:55:23.000000 rohdeschwarz-1.9.1.dev1/rohdeschwarz/bin/vna.py
--rw-r--r--   0 lalic      (501) staff       (20)     2168 2021-08-19 17:55:23.000000 rohdeschwarz-1.9.1.dev1/rohdeschwarz/bin/vsg.py
-drwxr-xr-x   0 lalic      (501) staff       (20)        0 2021-08-19 19:48:03.362571 rohdeschwarz-1.9.1.dev1/rohdeschwarz/bus/
--rw-r--r--   0 lalic      (501) staff       (20)       82 2021-08-19 17:55:23.000000 rohdeschwarz-1.9.1.dev1/rohdeschwarz/bus/__init__.py
--rw-r--r--   0 lalic      (501) staff       (20)     4094 2021-08-19 17:55:23.000000 rohdeschwarz-1.9.1.dev1/rohdeschwarz/bus/tcp.py
--rw-r--r--   0 lalic      (501) staff       (20)     4635 2021-08-19 17:55:23.000000 rohdeschwarz-1.9.1.dev1/rohdeschwarz/bus/visa.py
-drwxr-xr-x   0 lalic      (501) staff       (20)        0 2021-08-19 19:48:03.363567 rohdeschwarz-1.9.1.dev1/rohdeschwarz/general/
--rw-r--r--   0 lalic      (501) staff       (20)       52 2021-08-19 17:55:23.000000 rohdeschwarz-1.9.1.dev1/rohdeschwarz/general/__init__.py
--rw-r--r--   0 lalic      (501) staff       (20)     6371 2021-08-19 17:55:23.000000 rohdeschwarz-1.9.1.dev1/rohdeschwarz/general/general.py
-drwxr-xr-x   0 lalic      (501) staff       (20)        0 2021-08-19 19:48:03.364477 rohdeschwarz-1.9.1.dev1/rohdeschwarz/instruments/
--rw-r--r--   0 lalic      (501) staff       (20)       45 2021-08-19 17:55:23.000000 rohdeschwarz-1.9.1.dev1/rohdeschwarz/instruments/__init__.py
--rw-r--r--   0 lalic      (501) staff       (20)     9694 2021-08-19 17:55:23.000000 rohdeschwarz-1.9.1.dev1/rohdeschwarz/instruments/genericinstrument.py
-drwxr-xr-x   0 lalic      (501) staff       (20)        0 2021-08-19 19:48:03.366288 rohdeschwarz-1.9.1.dev1/rohdeschwarz/instruments/ospswitch/
--rw-r--r--   0 lalic      (501) staff       (20)      135 2021-08-19 17:55:23.000000 rohdeschwarz-1.9.1.dev1/rohdeschwarz/instruments/ospswitch/__init__.py
--rw-r--r--   0 lalic      (501) staff       (20)      271 2021-08-19 17:55:23.000000 rohdeschwarz-1.9.1.dev1/rohdeschwarz/instruments/ospswitch/enums.py
--rw-r--r--   0 lalic      (501) staff       (20)     2898 2021-08-19 17:55:23.000000 rohdeschwarz-1.9.1.dev1/rohdeschwarz/instruments/ospswitch/ospswitch.py
-drwxr-xr-x   0 lalic      (501) staff       (20)        0 2021-08-19 19:48:03.374956 rohdeschwarz-1.9.1.dev1/rohdeschwarz/instruments/vna/
--rw-r--r--   0 lalic      (501) staff       (20)      508 2021-08-19 17:55:23.000000 rohdeschwarz-1.9.1.dev1/rohdeschwarz/instruments/vna/__init__.py
--rw-r--r--   0 lalic      (501) staff       (20)     2479 2021-08-19 17:55:23.000000 rohdeschwarz-1.9.1.dev1/rohdeschwarz/instruments/vna/calunit.py
--rw-r--r--   0 lalic      (501) staff       (20)    20877 2021-08-19 17:55:23.000000 rohdeschwarz-1.9.1.dev1/rohdeschwarz/instruments/vna/channel.py
--rw-r--r--   0 lalic      (501) staff       (20)     3574 2021-08-19 17:55:23.000000 rohdeschwarz-1.9.1.dev1/rohdeschwarz/instruments/vna/diagram.py
--rw-r--r--   0 lalic      (501) staff       (20)     6300 2021-08-19 17:55:23.000000 rohdeschwarz-1.9.1.dev1/rohdeschwarz/instruments/vna/filesystem.py
--rw-r--r--   0 lalic      (501) staff       (20)     2311 2021-08-19 18:00:42.000000 rohdeschwarz-1.9.1.dev1/rohdeschwarz/instruments/vna/limits.py
--rw-r--r--   0 lalic      (501) staff       (20)     2536 2020-12-05 01:33:52.000000 rohdeschwarz-1.9.1.dev1/rohdeschwarz/instruments/vna/marker.py
--rw-r--r--   0 lalic      (501) staff       (20)     2048 2021-08-19 17:55:23.000000 rohdeschwarz-1.9.1.dev1/rohdeschwarz/instruments/vna/multistep_autocal.py
--rw-r--r--   0 lalic      (501) staff       (20)     3580 2021-08-19 17:55:23.000000 rohdeschwarz-1.9.1.dev1/rohdeschwarz/instruments/vna/properties.py
--rw-r--r--   0 lalic      (501) staff       (20)    11339 2021-08-19 17:55:23.000000 rohdeschwarz-1.9.1.dev1/rohdeschwarz/instruments/vna/settings.py
--rw-r--r--   0 lalic      (501) staff       (20)      534 2020-04-16 06:49:26.000000 rohdeschwarz-1.9.1.dev1/rohdeschwarz/instruments/vna/timedomain.py
--rw-r--r--   0 lalic      (501) staff       (20)    16442 2021-08-19 17:55:23.000000 rohdeschwarz-1.9.1.dev1/rohdeschwarz/instruments/vna/trace.py
--rw-r--r--   0 lalic      (501) staff       (20)    17268 2021-08-19 19:22:36.000000 rohdeschwarz-1.9.1.dev1/rohdeschwarz/instruments/vna/vna.py
-drwxr-xr-x   0 lalic      (501) staff       (20)        0 2021-08-19 19:48:03.376433 rohdeschwarz-1.9.1.dev1/rohdeschwarz/instruments/vsg/
--rw-r--r--   0 lalic      (501) staff       (20)       49 2021-08-19 17:55:23.000000 rohdeschwarz-1.9.1.dev1/rohdeschwarz/instruments/vsg/__init__.py
--rw-r--r--   0 lalic      (501) staff       (20)     1916 2021-08-19 17:55:23.000000 rohdeschwarz-1.9.1.dev1/rohdeschwarz/instruments/vsg/filesystem.py
--rw-r--r--   0 lalic      (501) staff       (20)      272 2021-08-19 17:55:23.000000 rohdeschwarz-1.9.1.dev1/rohdeschwarz/instruments/vsg/vsg.py
-drwxr-xr-x   0 lalic      (501) staff       (20)        0 2021-08-19 19:48:03.376960 rohdeschwarz-1.9.1.dev1/rohdeschwarz/test/
--rw-r--r--   0 lalic      (501) staff       (20)        0 2020-04-16 06:49:26.000000 rohdeschwarz-1.9.1.dev1/rohdeschwarz/test/__init__.py
-drwxr-xr-x   0 lalic      (501) staff       (20)        0 2021-08-19 19:48:03.377324 rohdeschwarz-1.9.1.dev1/rohdeschwarz/test/mock/
--rw-r--r--   0 lalic      (501) staff       (20)        0 2020-04-16 06:49:26.000000 rohdeschwarz-1.9.1.dev1/rohdeschwarz/test/mock/__init__.py
-drwxr-xr-x   0 lalic      (501) staff       (20)        0 2021-08-19 19:48:03.379172 rohdeschwarz-1.9.1.dev1/rohdeschwarz/test/mock/bus/
--rw-r--r--   0 lalic      (501) staff       (20)      103 2021-08-19 17:55:23.000000 rohdeschwarz-1.9.1.dev1/rohdeschwarz/test/mock/bus/__init__.py
--rw-r--r--   0 lalic      (501) staff       (20)      936 2021-03-29 05:27:54.000000 rohdeschwarz-1.9.1.dev1/rohdeschwarz/test/mock/bus/base.py
--rw-r--r--   0 lalic      (501) staff       (20)      813 2021-03-29 05:27:54.000000 rohdeschwarz-1.9.1.dev1/rohdeschwarz/test/mock/bus/fifo.py
--rw-r--r--   0 lalic      (501) staff       (20)     2317 2020-04-16 06:49:26.000000 rohdeschwarz-1.9.1.dev1/rohdeschwarz/test/mock/bus/osp.py
-drwxr-xr-x   0 lalic      (501) staff       (20)        0 2021-08-19 19:48:03.380079 rohdeschwarz-1.9.1.dev1/rohdeschwarz/test/mock/instruments/
--rw-r--r--   0 lalic      (501) staff       (20)        1 2020-04-16 06:49:26.000000 rohdeschwarz-1.9.1.dev1/rohdeschwarz/test/mock/instruments/__init__.py
--rw-r--r--   0 lalic      (501) staff       (20)     1474 2020-04-16 06:49:26.000000 rohdeschwarz-1.9.1.dev1/rohdeschwarz/test/mock/instruments/genericinstrument.py
-drwxr-xr-x   0 lalic      (501) staff       (20)        0 2021-08-19 19:48:03.384630 rohdeschwarz-1.9.1.dev1/rohdeschwarz/test/mock/instruments/vna/
--rw-r--r--   0 lalic      (501) staff       (20)       59 2020-04-16 06:49:26.000000 rohdeschwarz-1.9.1.dev1/rohdeschwarz/test/mock/instruments/vna/__init__.py
--rw-r--r--   0 lalic      (501) staff       (20)      443 2020-04-16 06:49:26.000000 rohdeschwarz-1.9.1.dev1/rohdeschwarz/test/mock/instruments/vna/calunit.py
--rw-r--r--   0 lalic      (501) staff       (20)     1375 2020-04-16 06:49:26.000000 rohdeschwarz-1.9.1.dev1/rohdeschwarz/test/mock/instruments/vna/channel.py
--rw-r--r--   0 lalic      (501) staff       (20)      603 2020-04-16 06:49:26.000000 rohdeschwarz-1.9.1.dev1/rohdeschwarz/test/mock/instruments/vna/diagram.py
--rw-r--r--   0 lalic      (501) staff       (20)      621 2020-04-16 06:49:26.000000 rohdeschwarz-1.9.1.dev1/rohdeschwarz/test/mock/instruments/vna/marker.py
--rw-r--r--   0 lalic      (501) staff       (20)      529 2020-04-16 06:49:26.000000 rohdeschwarz-1.9.1.dev1/rohdeschwarz/test/mock/instruments/vna/properties.py
--rw-r--r--   0 lalic      (501) staff       (20)      154 2020-04-16 06:49:26.000000 rohdeschwarz-1.9.1.dev1/rohdeschwarz/test/mock/instruments/vna/settings.py
--rw-r--r--   0 lalic      (501) staff       (20)     1520 2020-04-16 06:49:26.000000 rohdeschwarz-1.9.1.dev1/rohdeschwarz/test/mock/instruments/vna/trace.py
--rw-r--r--   0 lalic      (501) staff       (20)     7165 2020-04-16 06:49:26.000000 rohdeschwarz-1.9.1.dev1/rohdeschwarz/test/mock/instruments/vna/vna.py
-drwxr-xr-x   0 lalic      (501) staff       (20)        0 2021-08-19 19:48:03.358765 rohdeschwarz-1.9.1.dev1/rohdeschwarz.egg-info/
--rw-r--r--   0 lalic      (501) staff       (20)     1214 2021-08-19 19:48:03.000000 rohdeschwarz-1.9.1.dev1/rohdeschwarz.egg-info/PKG-INFO
--rw-r--r--   0 lalic      (501) staff       (20)     2348 2021-08-19 19:48:03.000000 rohdeschwarz-1.9.1.dev1/rohdeschwarz.egg-info/SOURCES.txt
--rw-r--r--   0 lalic      (501) staff       (20)        1 2021-08-19 19:48:03.000000 rohdeschwarz-1.9.1.dev1/rohdeschwarz.egg-info/dependency_links.txt
--rw-r--r--   0 lalic      (501) staff       (20)      151 2021-08-19 19:48:03.000000 rohdeschwarz-1.9.1.dev1/rohdeschwarz.egg-info/entry_points.txt
--rw-r--r--   0 lalic      (501) staff       (20)       68 2021-08-19 19:48:03.000000 rohdeschwarz-1.9.1.dev1/rohdeschwarz.egg-info/requires.txt
--rw-r--r--   0 lalic      (501) staff       (20)       18 2021-08-19 19:48:03.000000 rohdeschwarz-1.9.1.dev1/rohdeschwarz.egg-info/top_level.txt
--rw-r--r--   0 lalic      (501) staff       (20)       38 2021-08-19 19:48:03.390478 rohdeschwarz-1.9.1.dev1/setup.cfg
--rw-r--r--   0 lalic      (501) staff       (20)     4195 2021-08-19 19:47:24.000000 rohdeschwarz-1.9.1.dev1/setup.py
-drwxr-xr-x   0 lalic      (501) staff       (20)        0 2021-08-19 19:48:03.389049 rohdeschwarz-1.9.1.dev1/test/
--rw-r--r--   0 lalic      (501) staff       (20)        0 2020-04-16 06:49:26.000000 rohdeschwarz-1.9.1.dev1/test/__init__.py
--rw-r--r--   0 lalic      (501) staff       (20)     1588 2021-08-19 17:55:23.000000 rohdeschwarz-1.9.1.dev1/test/test_general.py
--rw-r--r--   0 lalic      (501) staff       (20)      549 2020-04-16 06:49:26.000000 rohdeschwarz-1.9.1.dev1/test/test_mockbus.py
--rw-r--r--   0 lalic      (501) staff       (20)     1681 2021-08-19 17:55:23.000000 rohdeschwarz-1.9.1.dev1/test/test_ospbus.py
--rw-r--r--   0 lalic      (501) staff       (20)     1135 2021-08-19 17:55:23.000000 rohdeschwarz-1.9.1.dev1/test/test_ospswitch.py
--rw-r--r--   0 lalic      (501) staff       (20)      529 2020-04-16 06:49:26.000000 rohdeschwarz-1.9.1.dev1/test/test_vna.py
--rw-r--r--   0 lalic      (501) staff       (20)     1913 2020-04-16 07:32:32.000000 rohdeschwarz-1.9.1.dev1/test/test_vnachannel.py
--rw-r--r--   0 lalic      (501) staff       (20)     4447 2021-08-19 17:55:23.000000 rohdeschwarz-1.9.1.dev1/test/test_vnatrace.py
+drwxr-xr-x   0 lalic      (501) staff       (20)        0 2022-03-23 16:14:33.238694 rohdeschwarz-1.9.2.dev1/
+-rw-r--r--   0 lalic      (501) staff       (20)      209 2020-04-16 06:49:26.000000 rohdeschwarz-1.9.2.dev1/DESCRIPTION.rst
+-rw-r--r--   0 lalic      (501) staff       (20)       14 2020-04-16 06:49:26.000000 rohdeschwarz-1.9.2.dev1/MANIFEST.in
+-rw-r--r--   0 lalic      (501) staff       (20)     1214 2022-03-23 16:14:33.238263 rohdeschwarz-1.9.2.dev1/PKG-INFO
+drwxr-xr-x   0 lalic      (501) staff       (20)        0 2022-03-23 16:14:33.206503 rohdeschwarz-1.9.2.dev1/rohdeschwarz/
+-rw-r--r--   0 lalic      (501) staff       (20)      109 2021-08-19 17:55:23.000000 rohdeschwarz-1.9.2.dev1/rohdeschwarz/__init__.py
+drwxr-xr-x   0 lalic      (501) staff       (20)        0 2022-03-23 16:14:33.211786 rohdeschwarz-1.9.2.dev1/rohdeschwarz/bin/
+-rw-r--r--   0 lalic      (501) staff       (20)        0 2020-04-16 06:49:26.000000 rohdeschwarz-1.9.2.dev1/rohdeschwarz/bin/__init__.py
+-rwxr-xr-x   0 lalic      (501) staff       (20)     2204 2021-08-19 17:55:23.000000 rohdeschwarz-1.9.2.dev1/rohdeschwarz/bin/instr.py
+-rw-r--r--   0 lalic      (501) staff       (20)     2720 2021-08-19 17:55:23.000000 rohdeschwarz-1.9.2.dev1/rohdeschwarz/bin/osp.py
+-rwxr-xr-x   0 lalic      (501) staff       (20)     2168 2021-08-19 17:55:23.000000 rohdeschwarz-1.9.2.dev1/rohdeschwarz/bin/vna.py
+-rw-r--r--   0 lalic      (501) staff       (20)     2168 2021-08-19 17:55:23.000000 rohdeschwarz-1.9.2.dev1/rohdeschwarz/bin/vsg.py
+drwxr-xr-x   0 lalic      (501) staff       (20)        0 2022-03-23 16:14:33.213233 rohdeschwarz-1.9.2.dev1/rohdeschwarz/bus/
+-rw-r--r--   0 lalic      (501) staff       (20)       82 2021-08-19 17:55:23.000000 rohdeschwarz-1.9.2.dev1/rohdeschwarz/bus/__init__.py
+-rw-r--r--   0 lalic      (501) staff       (20)     4094 2021-08-19 17:55:23.000000 rohdeschwarz-1.9.2.dev1/rohdeschwarz/bus/tcp.py
+-rw-r--r--   0 lalic      (501) staff       (20)     4635 2021-08-19 17:55:23.000000 rohdeschwarz-1.9.2.dev1/rohdeschwarz/bus/visa.py
+drwxr-xr-x   0 lalic      (501) staff       (20)        0 2022-03-23 16:14:33.214181 rohdeschwarz-1.9.2.dev1/rohdeschwarz/general/
+-rw-r--r--   0 lalic      (501) staff       (20)       52 2021-08-19 17:55:23.000000 rohdeschwarz-1.9.2.dev1/rohdeschwarz/general/__init__.py
+-rw-r--r--   0 lalic      (501) staff       (20)     6371 2021-08-19 17:55:23.000000 rohdeschwarz-1.9.2.dev1/rohdeschwarz/general/general.py
+drwxr-xr-x   0 lalic      (501) staff       (20)        0 2022-03-23 16:14:33.215109 rohdeschwarz-1.9.2.dev1/rohdeschwarz/instruments/
+-rw-r--r--   0 lalic      (501) staff       (20)       45 2021-08-19 17:55:23.000000 rohdeschwarz-1.9.2.dev1/rohdeschwarz/instruments/__init__.py
+-rw-r--r--   0 lalic      (501) staff       (20)     9694 2022-03-23 15:53:38.000000 rohdeschwarz-1.9.2.dev1/rohdeschwarz/instruments/genericinstrument.py
+drwxr-xr-x   0 lalic      (501) staff       (20)        0 2022-03-23 16:14:33.216548 rohdeschwarz-1.9.2.dev1/rohdeschwarz/instruments/ospswitch/
+-rw-r--r--   0 lalic      (501) staff       (20)      135 2021-08-19 17:55:23.000000 rohdeschwarz-1.9.2.dev1/rohdeschwarz/instruments/ospswitch/__init__.py
+-rw-r--r--   0 lalic      (501) staff       (20)      271 2021-08-19 17:55:23.000000 rohdeschwarz-1.9.2.dev1/rohdeschwarz/instruments/ospswitch/enums.py
+-rw-r--r--   0 lalic      (501) staff       (20)     2898 2021-08-19 17:55:23.000000 rohdeschwarz-1.9.2.dev1/rohdeschwarz/instruments/ospswitch/ospswitch.py
+drwxr-xr-x   0 lalic      (501) staff       (20)        0 2022-03-23 16:14:33.223194 rohdeschwarz-1.9.2.dev1/rohdeschwarz/instruments/vna/
+-rw-r--r--   0 lalic      (501) staff       (20)      508 2022-03-23 15:53:38.000000 rohdeschwarz-1.9.2.dev1/rohdeschwarz/instruments/vna/__init__.py
+-rw-r--r--   0 lalic      (501) staff       (20)     2479 2022-03-23 15:53:38.000000 rohdeschwarz-1.9.2.dev1/rohdeschwarz/instruments/vna/calunit.py
+-rw-r--r--   0 lalic      (501) staff       (20)    20877 2021-08-19 17:55:23.000000 rohdeschwarz-1.9.2.dev1/rohdeschwarz/instruments/vna/channel.py
+-rw-r--r--   0 lalic      (501) staff       (20)     3574 2021-08-19 17:55:23.000000 rohdeschwarz-1.9.2.dev1/rohdeschwarz/instruments/vna/diagram.py
+-rw-r--r--   0 lalic      (501) staff       (20)     6300 2021-08-19 17:55:23.000000 rohdeschwarz-1.9.2.dev1/rohdeschwarz/instruments/vna/filesystem.py
+-rw-r--r--   0 lalic      (501) staff       (20)     2311 2021-08-19 18:00:42.000000 rohdeschwarz-1.9.2.dev1/rohdeschwarz/instruments/vna/limits.py
+-rw-r--r--   0 lalic      (501) staff       (20)     2536 2020-12-05 01:33:52.000000 rohdeschwarz-1.9.2.dev1/rohdeschwarz/instruments/vna/marker.py
+-rw-r--r--   0 lalic      (501) staff       (20)     2048 2021-08-19 17:55:23.000000 rohdeschwarz-1.9.2.dev1/rohdeschwarz/instruments/vna/multistep_autocal.py
+-rw-r--r--   0 lalic      (501) staff       (20)     3580 2021-08-19 17:55:23.000000 rohdeschwarz-1.9.2.dev1/rohdeschwarz/instruments/vna/properties.py
+-rw-r--r--   0 lalic      (501) staff       (20)    11339 2021-08-19 17:55:23.000000 rohdeschwarz-1.9.2.dev1/rohdeschwarz/instruments/vna/settings.py
+-rw-r--r--   0 lalic      (501) staff       (20)      534 2020-04-16 06:49:26.000000 rohdeschwarz-1.9.2.dev1/rohdeschwarz/instruments/vna/timedomain.py
+-rw-r--r--   0 lalic      (501) staff       (20)    16442 2021-08-19 17:55:23.000000 rohdeschwarz-1.9.2.dev1/rohdeschwarz/instruments/vna/trace.py
+-rw-r--r--   0 lalic      (501) staff       (20)    17268 2022-03-23 15:53:38.000000 rohdeschwarz-1.9.2.dev1/rohdeschwarz/instruments/vna/vna.py
+drwxr-xr-x   0 lalic      (501) staff       (20)        0 2022-03-23 16:14:33.224847 rohdeschwarz-1.9.2.dev1/rohdeschwarz/instruments/vsg/
+-rw-r--r--   0 lalic      (501) staff       (20)       49 2021-08-19 17:55:23.000000 rohdeschwarz-1.9.2.dev1/rohdeschwarz/instruments/vsg/__init__.py
+-rw-r--r--   0 lalic      (501) staff       (20)     1916 2021-08-19 17:55:23.000000 rohdeschwarz-1.9.2.dev1/rohdeschwarz/instruments/vsg/filesystem.py
+-rw-r--r--   0 lalic      (501) staff       (20)      272 2021-08-19 17:55:23.000000 rohdeschwarz-1.9.2.dev1/rohdeschwarz/instruments/vsg/vsg.py
+drwxr-xr-x   0 lalic      (501) staff       (20)        0 2022-03-23 16:14:33.225264 rohdeschwarz-1.9.2.dev1/rohdeschwarz/test/
+-rw-r--r--   0 lalic      (501) staff       (20)        0 2020-04-16 06:49:26.000000 rohdeschwarz-1.9.2.dev1/rohdeschwarz/test/__init__.py
+drwxr-xr-x   0 lalic      (501) staff       (20)        0 2022-03-23 16:14:33.225600 rohdeschwarz-1.9.2.dev1/rohdeschwarz/test/mock/
+-rw-r--r--   0 lalic      (501) staff       (20)        0 2020-04-16 06:49:26.000000 rohdeschwarz-1.9.2.dev1/rohdeschwarz/test/mock/__init__.py
+drwxr-xr-x   0 lalic      (501) staff       (20)        0 2022-03-23 16:14:33.227213 rohdeschwarz-1.9.2.dev1/rohdeschwarz/test/mock/bus/
+-rw-r--r--   0 lalic      (501) staff       (20)      103 2021-08-19 17:55:23.000000 rohdeschwarz-1.9.2.dev1/rohdeschwarz/test/mock/bus/__init__.py
+-rw-r--r--   0 lalic      (501) staff       (20)      936 2021-03-29 05:27:54.000000 rohdeschwarz-1.9.2.dev1/rohdeschwarz/test/mock/bus/base.py
+-rw-r--r--   0 lalic      (501) staff       (20)      813 2021-03-29 05:27:54.000000 rohdeschwarz-1.9.2.dev1/rohdeschwarz/test/mock/bus/fifo.py
+-rw-r--r--   0 lalic      (501) staff       (20)     2317 2020-04-16 06:49:26.000000 rohdeschwarz-1.9.2.dev1/rohdeschwarz/test/mock/bus/osp.py
+drwxr-xr-x   0 lalic      (501) staff       (20)        0 2022-03-23 16:14:33.228312 rohdeschwarz-1.9.2.dev1/rohdeschwarz/test/mock/instruments/
+-rw-r--r--   0 lalic      (501) staff       (20)        1 2020-04-16 06:49:26.000000 rohdeschwarz-1.9.2.dev1/rohdeschwarz/test/mock/instruments/__init__.py
+-rw-r--r--   0 lalic      (501) staff       (20)     1474 2020-04-16 06:49:26.000000 rohdeschwarz-1.9.2.dev1/rohdeschwarz/test/mock/instruments/genericinstrument.py
+drwxr-xr-x   0 lalic      (501) staff       (20)        0 2022-03-23 16:14:33.233077 rohdeschwarz-1.9.2.dev1/rohdeschwarz/test/mock/instruments/vna/
+-rw-r--r--   0 lalic      (501) staff       (20)       59 2020-04-16 06:49:26.000000 rohdeschwarz-1.9.2.dev1/rohdeschwarz/test/mock/instruments/vna/__init__.py
+-rw-r--r--   0 lalic      (501) staff       (20)      443 2020-04-16 06:49:26.000000 rohdeschwarz-1.9.2.dev1/rohdeschwarz/test/mock/instruments/vna/calunit.py
+-rw-r--r--   0 lalic      (501) staff       (20)     1375 2020-04-16 06:49:26.000000 rohdeschwarz-1.9.2.dev1/rohdeschwarz/test/mock/instruments/vna/channel.py
+-rw-r--r--   0 lalic      (501) staff       (20)      603 2020-04-16 06:49:26.000000 rohdeschwarz-1.9.2.dev1/rohdeschwarz/test/mock/instruments/vna/diagram.py
+-rw-r--r--   0 lalic      (501) staff       (20)      621 2020-04-16 06:49:26.000000 rohdeschwarz-1.9.2.dev1/rohdeschwarz/test/mock/instruments/vna/marker.py
+-rw-r--r--   0 lalic      (501) staff       (20)      529 2020-04-16 06:49:26.000000 rohdeschwarz-1.9.2.dev1/rohdeschwarz/test/mock/instruments/vna/properties.py
+-rw-r--r--   0 lalic      (501) staff       (20)      154 2020-04-16 06:49:26.000000 rohdeschwarz-1.9.2.dev1/rohdeschwarz/test/mock/instruments/vna/settings.py
+-rw-r--r--   0 lalic      (501) staff       (20)     1520 2020-04-16 06:49:26.000000 rohdeschwarz-1.9.2.dev1/rohdeschwarz/test/mock/instruments/vna/trace.py
+-rw-r--r--   0 lalic      (501) staff       (20)     7165 2020-04-16 06:49:26.000000 rohdeschwarz-1.9.2.dev1/rohdeschwarz/test/mock/instruments/vna/vna.py
+drwxr-xr-x   0 lalic      (501) staff       (20)        0 2022-03-23 16:14:33.209259 rohdeschwarz-1.9.2.dev1/rohdeschwarz.egg-info/
+-rw-r--r--   0 lalic      (501) staff       (20)     1214 2022-03-23 16:14:32.000000 rohdeschwarz-1.9.2.dev1/rohdeschwarz.egg-info/PKG-INFO
+-rw-r--r--   0 lalic      (501) staff       (20)     2348 2022-03-23 16:14:33.000000 rohdeschwarz-1.9.2.dev1/rohdeschwarz.egg-info/SOURCES.txt
+-rw-r--r--   0 lalic      (501) staff       (20)        1 2022-03-23 16:14:32.000000 rohdeschwarz-1.9.2.dev1/rohdeschwarz.egg-info/dependency_links.txt
+-rw-r--r--   0 lalic      (501) staff       (20)      150 2022-03-23 16:14:32.000000 rohdeschwarz-1.9.2.dev1/rohdeschwarz.egg-info/entry_points.txt
+-rw-r--r--   0 lalic      (501) staff       (20)       69 2022-03-23 16:14:32.000000 rohdeschwarz-1.9.2.dev1/rohdeschwarz.egg-info/requires.txt
+-rw-r--r--   0 lalic      (501) staff       (20)       18 2022-03-23 16:14:33.000000 rohdeschwarz-1.9.2.dev1/rohdeschwarz.egg-info/top_level.txt
+-rw-r--r--   0 lalic      (501) staff       (20)       38 2022-03-23 16:14:33.238966 rohdeschwarz-1.9.2.dev1/setup.cfg
+-rw-r--r--   0 lalic      (501) staff       (20)     4196 2022-03-23 16:14:06.000000 rohdeschwarz-1.9.2.dev1/setup.py
+drwxr-xr-x   0 lalic      (501) staff       (20)        0 2022-03-23 16:14:33.237261 rohdeschwarz-1.9.2.dev1/test/
+-rw-r--r--   0 lalic      (501) staff       (20)        0 2020-04-16 06:49:26.000000 rohdeschwarz-1.9.2.dev1/test/__init__.py
+-rw-r--r--   0 lalic      (501) staff       (20)     1588 2021-08-19 17:55:23.000000 rohdeschwarz-1.9.2.dev1/test/test_general.py
+-rw-r--r--   0 lalic      (501) staff       (20)      549 2020-04-16 06:49:26.000000 rohdeschwarz-1.9.2.dev1/test/test_mockbus.py
+-rw-r--r--   0 lalic      (501) staff       (20)     1681 2021-08-19 17:55:23.000000 rohdeschwarz-1.9.2.dev1/test/test_ospbus.py
+-rw-r--r--   0 lalic      (501) staff       (20)     1135 2021-08-19 17:55:23.000000 rohdeschwarz-1.9.2.dev1/test/test_ospswitch.py
+-rw-r--r--   0 lalic      (501) staff       (20)      529 2020-04-16 06:49:26.000000 rohdeschwarz-1.9.2.dev1/test/test_vna.py
+-rw-r--r--   0 lalic      (501) staff       (20)     1913 2020-04-16 07:32:32.000000 rohdeschwarz-1.9.2.dev1/test/test_vnachannel.py
+-rw-r--r--   0 lalic      (501) staff       (20)     4447 2021-08-19 17:55:23.000000 rohdeschwarz-1.9.2.dev1/test/test_vnatrace.py
```

### Comparing `rohdeschwarz-1.9.1.dev1/PKG-INFO` & `rohdeschwarz-1.9.2.dev1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rohdeschwarz
-Version: 1.9.1.dev1
+Version: 1.9.2.dev1
 Summary: Rohde & Schwarz general purpose instrument control toolbox
 Home-page: https://github.com/Terrabits/rohdeschwarz
 Author: Nick Lalic
 Author-email: nick.lalic@rsa.rohde-schwarz.com
 License: R&S Terms and Conditions for Royalty-Free Products
 Keywords: RF test equipment automation ATE
 Platform: UNKNOWN
```

### Comparing `rohdeschwarz-1.9.1.dev1/rohdeschwarz/bin/instr.py` & `rohdeschwarz-1.9.2.dev1/rohdeschwarz/bin/instr.py`

 * *Files identical despite different names*

### Comparing `rohdeschwarz-1.9.1.dev1/rohdeschwarz/bin/osp.py` & `rohdeschwarz-1.9.2.dev1/rohdeschwarz/bin/osp.py`

 * *Files identical despite different names*

### Comparing `rohdeschwarz-1.9.1.dev1/rohdeschwarz/bin/vna.py` & `rohdeschwarz-1.9.2.dev1/rohdeschwarz/bin/vna.py`

 * *Files identical despite different names*

### Comparing `rohdeschwarz-1.9.1.dev1/rohdeschwarz/bin/vsg.py` & `rohdeschwarz-1.9.2.dev1/rohdeschwarz/bin/vsg.py`

 * *Files identical despite different names*

### Comparing `rohdeschwarz-1.9.1.dev1/rohdeschwarz/bus/tcp.py` & `rohdeschwarz-1.9.2.dev1/rohdeschwarz/bus/tcp.py`

 * *Files identical despite different names*

### Comparing `rohdeschwarz-1.9.1.dev1/rohdeschwarz/bus/visa.py` & `rohdeschwarz-1.9.2.dev1/rohdeschwarz/bus/visa.py`

 * *Files identical despite different names*

### Comparing `rohdeschwarz-1.9.1.dev1/rohdeschwarz/general/general.py` & `rohdeschwarz-1.9.2.dev1/rohdeschwarz/general/general.py`

 * *Files identical despite different names*

### Comparing `rohdeschwarz-1.9.1.dev1/rohdeschwarz/instruments/genericinstrument.py` & `rohdeschwarz-1.9.2.dev1/rohdeschwarz/instruments/genericinstrument.py`

 * *Files identical despite different names*

### Comparing `rohdeschwarz-1.9.1.dev1/rohdeschwarz/instruments/ospswitch/ospswitch.py` & `rohdeschwarz-1.9.2.dev1/rohdeschwarz/instruments/ospswitch/ospswitch.py`

 * *Files identical despite different names*

### Comparing `rohdeschwarz-1.9.1.dev1/rohdeschwarz/instruments/vna/calunit.py` & `rohdeschwarz-1.9.2.dev1/rohdeschwarz/instruments/vna/calunit.py`

 * *Files identical despite different names*

### Comparing `rohdeschwarz-1.9.1.dev1/rohdeschwarz/instruments/vna/channel.py` & `rohdeschwarz-1.9.2.dev1/rohdeschwarz/instruments/vna/channel.py`

 * *Files identical despite different names*

### Comparing `rohdeschwarz-1.9.1.dev1/rohdeschwarz/instruments/vna/diagram.py` & `rohdeschwarz-1.9.2.dev1/rohdeschwarz/instruments/vna/diagram.py`

 * *Files identical despite different names*

### Comparing `rohdeschwarz-1.9.1.dev1/rohdeschwarz/instruments/vna/filesystem.py` & `rohdeschwarz-1.9.2.dev1/rohdeschwarz/instruments/vna/filesystem.py`

 * *Files identical despite different names*

### Comparing `rohdeschwarz-1.9.1.dev1/rohdeschwarz/instruments/vna/limits.py` & `rohdeschwarz-1.9.2.dev1/rohdeschwarz/instruments/vna/limits.py`

 * *Files identical despite different names*

### Comparing `rohdeschwarz-1.9.1.dev1/rohdeschwarz/instruments/vna/marker.py` & `rohdeschwarz-1.9.2.dev1/rohdeschwarz/instruments/vna/marker.py`

 * *Files identical despite different names*

### Comparing `rohdeschwarz-1.9.1.dev1/rohdeschwarz/instruments/vna/multistep_autocal.py` & `rohdeschwarz-1.9.2.dev1/rohdeschwarz/instruments/vna/multistep_autocal.py`

 * *Files identical despite different names*

### Comparing `rohdeschwarz-1.9.1.dev1/rohdeschwarz/instruments/vna/properties.py` & `rohdeschwarz-1.9.2.dev1/rohdeschwarz/instruments/vna/properties.py`

 * *Files identical despite different names*

### Comparing `rohdeschwarz-1.9.1.dev1/rohdeschwarz/instruments/vna/settings.py` & `rohdeschwarz-1.9.2.dev1/rohdeschwarz/instruments/vna/settings.py`

 * *Files identical despite different names*

### Comparing `rohdeschwarz-1.9.1.dev1/rohdeschwarz/instruments/vna/timedomain.py` & `rohdeschwarz-1.9.2.dev1/rohdeschwarz/instruments/vna/timedomain.py`

 * *Files identical despite different names*

### Comparing `rohdeschwarz-1.9.1.dev1/rohdeschwarz/instruments/vna/trace.py` & `rohdeschwarz-1.9.2.dev1/rohdeschwarz/instruments/vna/trace.py`

 * *Files identical despite different names*

### Comparing `rohdeschwarz-1.9.1.dev1/rohdeschwarz/instruments/vna/vna.py` & `rohdeschwarz-1.9.2.dev1/rohdeschwarz/instruments/vna/vna.py`

 * *Files identical despite different names*

### Comparing `rohdeschwarz-1.9.1.dev1/rohdeschwarz/instruments/vsg/filesystem.py` & `rohdeschwarz-1.9.2.dev1/rohdeschwarz/instruments/vsg/filesystem.py`

 * *Files identical despite different names*

### Comparing `rohdeschwarz-1.9.1.dev1/rohdeschwarz/test/mock/bus/base.py` & `rohdeschwarz-1.9.2.dev1/rohdeschwarz/test/mock/bus/base.py`

 * *Files identical despite different names*

### Comparing `rohdeschwarz-1.9.1.dev1/rohdeschwarz/test/mock/bus/fifo.py` & `rohdeschwarz-1.9.2.dev1/rohdeschwarz/test/mock/bus/fifo.py`

 * *Files identical despite different names*

### Comparing `rohdeschwarz-1.9.1.dev1/rohdeschwarz/test/mock/bus/osp.py` & `rohdeschwarz-1.9.2.dev1/rohdeschwarz/test/mock/bus/osp.py`

 * *Files identical despite different names*

### Comparing `rohdeschwarz-1.9.1.dev1/rohdeschwarz/test/mock/instruments/genericinstrument.py` & `rohdeschwarz-1.9.2.dev1/rohdeschwarz/test/mock/instruments/genericinstrument.py`

 * *Files identical despite different names*

### Comparing `rohdeschwarz-1.9.1.dev1/rohdeschwarz/test/mock/instruments/vna/channel.py` & `rohdeschwarz-1.9.2.dev1/rohdeschwarz/test/mock/instruments/vna/channel.py`

 * *Files identical despite different names*

### Comparing `rohdeschwarz-1.9.1.dev1/rohdeschwarz/test/mock/instruments/vna/diagram.py` & `rohdeschwarz-1.9.2.dev1/rohdeschwarz/test/mock/instruments/vna/diagram.py`

 * *Files identical despite different names*

### Comparing `rohdeschwarz-1.9.1.dev1/rohdeschwarz/test/mock/instruments/vna/marker.py` & `rohdeschwarz-1.9.2.dev1/rohdeschwarz/test/mock/instruments/vna/marker.py`

 * *Files identical despite different names*

### Comparing `rohdeschwarz-1.9.1.dev1/rohdeschwarz/test/mock/instruments/vna/properties.py` & `rohdeschwarz-1.9.2.dev1/rohdeschwarz/test/mock/instruments/vna/properties.py`

 * *Files identical despite different names*

### Comparing `rohdeschwarz-1.9.1.dev1/rohdeschwarz/test/mock/instruments/vna/trace.py` & `rohdeschwarz-1.9.2.dev1/rohdeschwarz/test/mock/instruments/vna/trace.py`

 * *Files identical despite different names*

### Comparing `rohdeschwarz-1.9.1.dev1/rohdeschwarz/test/mock/instruments/vna/vna.py` & `rohdeschwarz-1.9.2.dev1/rohdeschwarz/test/mock/instruments/vna/vna.py`

 * *Files identical despite different names*

### Comparing `rohdeschwarz-1.9.1.dev1/rohdeschwarz.egg-info/PKG-INFO` & `rohdeschwarz-1.9.2.dev1/rohdeschwarz.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rohdeschwarz
-Version: 1.9.1.dev1
+Version: 1.9.2.dev1
 Summary: Rohde & Schwarz general purpose instrument control toolbox
 Home-page: https://github.com/Terrabits/rohdeschwarz
 Author: Nick Lalic
 Author-email: nick.lalic@rsa.rohde-schwarz.com
 License: R&S Terms and Conditions for Royalty-Free Products
 Keywords: RF test equipment automation ATE
 Platform: UNKNOWN
```

### Comparing `rohdeschwarz-1.9.1.dev1/rohdeschwarz.egg-info/SOURCES.txt` & `rohdeschwarz-1.9.2.dev1/rohdeschwarz.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `rohdeschwarz-1.9.1.dev1/setup.py` & `rohdeschwarz-1.9.2.dev1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 setup(
     name='rohdeschwarz',
 
     # Versions should comply with PEP440.  For a discussion on single-sourcing
     # the version across setup.py and the project code, see
     # https://packaging.python.org/en/latest/single_source_version.html
-    version='1.9.1.dev1',
+    version='1.9.2.dev1',
 
     description='Rohde & Schwarz general purpose instrument control toolbox',
     long_description=long_description,
 
     # The project's main homepage.
     url='https://github.com/Terrabits/rohdeschwarz',
 
@@ -77,15 +77,15 @@
     # simple. Or you can use find_packages().
     packages=find_packages(exclude=['tests']),
 
     # List run-time dependencies here.  These will be installed by pip when
     # your project is installed. For an analysis of "install_requires" vs pip's
     # requirements files see:
     # https://packaging.python.org/en/latest/requirements.html
-    install_requires=['pathlib', 'pyvisa', 'numpy', 'ruamel.yaml'],
+    install_requires=['pathlib2', 'pyvisa', 'numpy', 'ruamel.yaml'],
 
     # List additional groups of dependencies here (e.g. development
     # dependencies). You can install these using the following syntax,
     # for example:
     # $ pip install -e .[dev,test]
     extras_require={
         'dev':  ['ddt', 'twine', 'wheel'],
```

### Comparing `rohdeschwarz-1.9.1.dev1/test/test_general.py` & `rohdeschwarz-1.9.2.dev1/test/test_general.py`

 * *Files identical despite different names*

### Comparing `rohdeschwarz-1.9.1.dev1/test/test_mockbus.py` & `rohdeschwarz-1.9.2.dev1/test/test_mockbus.py`

 * *Files identical despite different names*

### Comparing `rohdeschwarz-1.9.1.dev1/test/test_ospbus.py` & `rohdeschwarz-1.9.2.dev1/test/test_ospbus.py`

 * *Files identical despite different names*

### Comparing `rohdeschwarz-1.9.1.dev1/test/test_ospswitch.py` & `rohdeschwarz-1.9.2.dev1/test/test_ospswitch.py`

 * *Files identical despite different names*

### Comparing `rohdeschwarz-1.9.1.dev1/test/test_vna.py` & `rohdeschwarz-1.9.2.dev1/test/test_vna.py`

 * *Files identical despite different names*

### Comparing `rohdeschwarz-1.9.1.dev1/test/test_vnachannel.py` & `rohdeschwarz-1.9.2.dev1/test/test_vnachannel.py`

 * *Files identical despite different names*

### Comparing `rohdeschwarz-1.9.1.dev1/test/test_vnatrace.py` & `rohdeschwarz-1.9.2.dev1/test/test_vnatrace.py`

 * *Files identical despite different names*

