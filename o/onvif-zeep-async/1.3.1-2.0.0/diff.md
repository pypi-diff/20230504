# Comparing `tmp/onvif-zeep-async-1.3.1.tar.gz` & `tmp/onvif-zeep-async-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "onvif-zeep-async-1.3.1.tar", last modified: Mon May  1 14:51:10 2023, max compression
+gzip compressed data, was "onvif-zeep-async-2.0.0.tar", last modified: Thu May  4 15:11:53 2023, max compression
```

## Comparing `onvif-zeep-async-1.3.1.tar` & `onvif-zeep-async-2.0.0.tar`

### file list

```diff
@@ -1,71 +1,71 @@
-drwxr-xr-x   0 bdraco     (501) staff       (20)        0 2023-05-01 14:51:10.768321 onvif-zeep-async-1.3.1/
--rw-r--r--   0 bdraco     (501) staff       (20)      724 2023-04-30 15:25:07.000000 onvif-zeep-async-1.3.1/.gitignore
--rw-r--r--   0 bdraco     (501) staff       (20)     1139 2023-04-30 15:25:07.000000 onvif-zeep-async-1.3.1/.pre-commit-config.yaml
--rw-r--r--   0 bdraco     (501) staff       (20)        0 2023-03-23 19:23:45.000000 onvif-zeep-async-1.3.1/CHANGES.txt
--rw-r--r--   0 bdraco     (501) staff       (20)     1087 2023-03-23 19:23:45.000000 onvif-zeep-async-1.3.1/LICENSE
--rw-r--r--   0 bdraco     (501) staff       (20)      100 2023-04-30 15:25:07.000000 onvif-zeep-async-1.3.1/MANIFEST.in
--rw-r--r--   0 bdraco     (501) staff       (20)     1053 2023-04-30 15:25:07.000000 onvif-zeep-async-1.3.1/Makefile
--rw-r--r--   0 bdraco     (501) staff       (20)     5290 2023-05-01 14:51:10.768403 onvif-zeep-async-1.3.1/PKG-INFO
--rw-r--r--   0 bdraco     (501) staff       (20)     4926 2023-04-30 15:25:07.000000 onvif-zeep-async-1.3.1/README.rst
--rw-r--r--   0 bdraco     (501) staff       (20)      188 2023-04-30 15:25:07.000000 onvif-zeep-async-1.3.1/bandit.yaml
-drwxr-xr-x   0 bdraco     (501) staff       (20)        0 2023-05-01 14:51:10.762134 onvif-zeep-async-1.3.1/examples/
--rw-r--r--   0 bdraco     (501) staff       (20)     1497 2023-04-30 15:25:07.000000 onvif-zeep-async-1.3.1/examples/events.py
--rw-r--r--   0 bdraco     (501) staff       (20)     1264 2023-04-30 15:25:07.000000 onvif-zeep-async-1.3.1/examples/rotate_image.py
--rw-r--r--   0 bdraco     (501) staff       (20)     2459 2023-04-30 15:25:07.000000 onvif-zeep-async-1.3.1/examples/streaming.py
-drwxr-xr-x   0 bdraco     (501) staff       (20)        0 2023-05-01 14:51:10.762708 onvif-zeep-async-1.3.1/onvif/
--rw-r--r--   0 bdraco     (501) staff       (20)      599 2023-04-30 15:25:07.000000 onvif-zeep-async-1.3.1/onvif/__init__.py
--rw-r--r--   0 bdraco     (501) staff       (20)    23611 2023-05-01 14:50:31.000000 onvif-zeep-async-1.3.1/onvif/client.py
--rw-r--r--   0 bdraco     (501) staff       (20)     2190 2023-04-30 15:25:07.000000 onvif-zeep-async-1.3.1/onvif/definition.py
--rw-r--r--   0 bdraco     (501) staff       (20)      886 2023-04-30 15:25:07.000000 onvif-zeep-async-1.3.1/onvif/exceptions.py
--rw-r--r--   0 bdraco     (501) staff       (20)        6 2023-05-01 14:50:36.000000 onvif-zeep-async-1.3.1/onvif/version.txt
-drwxr-xr-x   0 bdraco     (501) staff       (20)        0 2023-05-01 14:51:10.767343 onvif-zeep-async-1.3.1/onvif/wsdl/
--rw-r--r--   0 bdraco     (501) staff       (20)    16384 2023-04-16 04:45:10.000000 onvif-zeep-async-1.3.1/onvif/wsdl/.events.wsdl.swn
--rw-r--r--   0 bdraco     (501) staff       (20)       26 2023-04-30 15:25:07.000000 onvif-zeep-async-1.3.1/onvif/wsdl/__init__.py
--rw-r--r--   0 bdraco     (501) staff       (20)    38072 2023-04-30 15:25:07.000000 onvif-zeep-async-1.3.1/onvif/wsdl/accesscontrol.wsdl
--rw-r--r--   0 bdraco     (501) staff       (20)    57255 2023-04-30 15:25:07.000000 onvif-zeep-async-1.3.1/onvif/wsdl/actionengine.wsdl
--rw-r--r--   0 bdraco     (501) staff       (20)     7263 2023-04-30 15:25:07.000000 onvif-zeep-async-1.3.1/onvif/wsdl/addressing
--rw-r--r--   0 bdraco     (501) staff       (20)    79284 2023-04-30 15:25:07.000000 onvif-zeep-async-1.3.1/onvif/wsdl/advancedsecurity.wsdl
--rw-r--r--   0 bdraco     (501) staff       (20)    24131 2023-04-30 15:25:07.000000 onvif-zeep-async-1.3.1/onvif/wsdl/analytics.wsdl
--rw-r--r--   0 bdraco     (501) staff       (20)    31976 2023-04-30 15:25:07.000000 onvif-zeep-async-1.3.1/onvif/wsdl/analyticsdevice.wsdl
--rw-r--r--   0 bdraco     (501) staff       (20)    23300 2023-04-30 15:25:07.000000 onvif-zeep-async-1.3.1/onvif/wsdl/b-2.xsd
--rw-r--r--   0 bdraco     (501) staff       (20)     5100 2023-04-30 15:25:07.000000 onvif-zeep-async-1.3.1/onvif/wsdl/bf-2.xsd
--rw-r--r--   0 bdraco     (501) staff       (20)    20498 2023-04-30 15:25:07.000000 onvif-zeep-async-1.3.1/onvif/wsdl/bw-2.wsdl
--rw-r--r--   0 bdraco     (501) staff       (20)    60231 2023-04-30 15:25:07.000000 onvif-zeep-async-1.3.1/onvif/wsdl/deviceio.wsdl
--rw-r--r--   0 bdraco     (501) staff       (20)   163209 2023-04-30 15:25:07.000000 onvif-zeep-async-1.3.1/onvif/wsdl/devicemgmt.wsdl
--rw-r--r--   0 bdraco     (501) staff       (20)    24593 2023-04-30 15:25:07.000000 onvif-zeep-async-1.3.1/onvif/wsdl/display.wsdl
--rw-r--r--   0 bdraco     (501) staff       (20)    53648 2023-04-30 15:25:07.000000 onvif-zeep-async-1.3.1/onvif/wsdl/doorcontrol.wsdl
--rw-r--r--   0 bdraco     (501) staff       (20)     6249 2023-04-30 15:25:07.000000 onvif-zeep-async-1.3.1/onvif/wsdl/envelope
--rw-r--r--   0 bdraco     (501) staff       (20)    37870 2023-04-30 15:25:07.000000 onvif-zeep-async-1.3.1/onvif/wsdl/events.wsdl
--rw-r--r--   0 bdraco     (501) staff       (20)    17998 2023-04-30 15:25:07.000000 onvif-zeep-async-1.3.1/onvif/wsdl/imaging.wsdl
--rw-r--r--   0 bdraco     (501) staff       (20)      511 2023-04-30 15:25:07.000000 onvif-zeep-async-1.3.1/onvif/wsdl/include
--rw-r--r--   0 bdraco     (501) staff       (20)   174812 2023-04-30 15:25:07.000000 onvif-zeep-async-1.3.1/onvif/wsdl/media.wsdl
--rw-r--r--   0 bdraco     (501) staff       (20)   363349 2023-04-30 15:25:07.000000 onvif-zeep-async-1.3.1/onvif/wsdl/onvif.xsd
--rw-r--r--   0 bdraco     (501) staff       (20)    54058 2023-04-30 15:25:07.000000 onvif-zeep-async-1.3.1/onvif/wsdl/ptz.wsdl
--rw-r--r--   0 bdraco     (501) staff       (20)     3660 2023-04-30 15:25:07.000000 onvif-zeep-async-1.3.1/onvif/wsdl/r-2.xsd
--rw-r--r--   0 bdraco     (501) staff       (20)    17214 2023-04-30 15:25:07.000000 onvif-zeep-async-1.3.1/onvif/wsdl/receiver.wsdl
--rw-r--r--   0 bdraco     (501) staff       (20)    40704 2023-04-30 15:25:07.000000 onvif-zeep-async-1.3.1/onvif/wsdl/recording.wsdl
--rw-r--r--   0 bdraco     (501) staff       (20)     5596 2023-04-30 15:25:07.000000 onvif-zeep-async-1.3.1/onvif/wsdl/remotediscovery.wsdl
--rw-r--r--   0 bdraco     (501) staff       (20)    10581 2023-04-30 15:25:07.000000 onvif-zeep-async-1.3.1/onvif/wsdl/replay.wsdl
--rw-r--r--   0 bdraco     (501) staff       (20)     3727 2023-04-30 15:25:07.000000 onvif-zeep-async-1.3.1/onvif/wsdl/rw-2.wsdl
--rw-r--r--   0 bdraco     (501) staff       (20)    43139 2023-04-30 15:25:07.000000 onvif-zeep-async-1.3.1/onvif/wsdl/search.wsdl
--rw-r--r--   0 bdraco     (501) staff       (20)     8960 2023-04-30 15:25:07.000000 onvif-zeep-async-1.3.1/onvif/wsdl/t-1.xsd
--rw-r--r--   0 bdraco     (501) staff       (20)     3738 2023-04-30 15:25:07.000000 onvif-zeep-async-1.3.1/onvif/wsdl/types.xsd
--rw-r--r--   0 bdraco     (501) staff       (20)     5849 2023-04-30 15:25:07.000000 onvif-zeep-async-1.3.1/onvif/wsdl/ws-addr.xsd
--rw-r--r--   0 bdraco     (501) staff       (20)    10455 2023-04-30 15:25:07.000000 onvif-zeep-async-1.3.1/onvif/wsdl/ws-discovery.xsd
--rw-r--r--   0 bdraco     (501) staff       (20)     8836 2023-04-30 15:25:07.000000 onvif-zeep-async-1.3.1/onvif/wsdl/xml.xsd
--rw-r--r--   0 bdraco     (501) staff       (20)     1639 2023-04-30 15:25:07.000000 onvif-zeep-async-1.3.1/onvif/wsdl/xmlmime
-drwxr-xr-x   0 bdraco     (501) staff       (20)        0 2023-05-01 14:51:10.768125 onvif-zeep-async-1.3.1/onvif_zeep_async.egg-info/
--rw-r--r--   0 bdraco     (501) staff       (20)     5290 2023-05-01 14:51:10.000000 onvif-zeep-async-1.3.1/onvif_zeep_async.egg-info/PKG-INFO
--rw-r--r--   0 bdraco     (501) staff       (20)     1445 2023-05-01 14:51:10.000000 onvif-zeep-async-1.3.1/onvif_zeep_async.egg-info/SOURCES.txt
--rw-r--r--   0 bdraco     (501) staff       (20)        1 2023-05-01 14:51:10.000000 onvif-zeep-async-1.3.1/onvif_zeep_async.egg-info/dependency_links.txt
--rw-r--r--   0 bdraco     (501) staff       (20)       45 2023-05-01 14:51:10.000000 onvif-zeep-async-1.3.1/onvif_zeep_async.egg-info/entry_points.txt
--rw-r--r--   0 bdraco     (501) staff       (20)        1 2023-03-23 19:28:21.000000 onvif-zeep-async-1.3.1/onvif_zeep_async.egg-info/not-zip-safe
--rw-r--r--   0 bdraco     (501) staff       (20)       47 2023-05-01 14:51:10.000000 onvif-zeep-async-1.3.1/onvif_zeep_async.egg-info/requires.txt
--rw-r--r--   0 bdraco     (501) staff       (20)        6 2023-05-01 14:51:10.000000 onvif-zeep-async-1.3.1/onvif_zeep_async.egg-info/top_level.txt
--rw-r--r--   0 bdraco     (501) staff       (20)     1741 2023-04-30 15:25:07.000000 onvif-zeep-async-1.3.1/pylintrc
--rw-r--r--   0 bdraco     (501) staff       (20)       77 2023-04-30 15:25:07.000000 onvif-zeep-async-1.3.1/pyproject.toml
--rw-r--r--   0 bdraco     (501) staff       (20)      224 2023-04-30 15:25:07.000000 onvif-zeep-async-1.3.1/requirements.txt
--rw-r--r--   0 bdraco     (501) staff       (20)      409 2023-05-01 14:51:10.768645 onvif-zeep-async-1.3.1/setup.cfg
--rw-r--r--   0 bdraco     (501) staff       (20)     1801 2023-04-30 15:25:07.000000 onvif-zeep-async-1.3.1/setup.py
-drwxr-xr-x   0 bdraco     (501) staff       (20)        0 2023-05-01 14:51:10.768227 onvif-zeep-async-1.3.1/tests/
--rw-r--r--   0 bdraco     (501) staff       (20)     4133 2023-04-30 15:25:07.000000 onvif-zeep-async-1.3.1/tests/test.py
+drwxr-xr-x   0 bdraco     (501) staff       (20)        0 2023-05-04 15:11:53.943804 onvif-zeep-async-2.0.0/
+-rw-r--r--   0 bdraco     (501) staff       (20)      724 2023-04-30 15:25:07.000000 onvif-zeep-async-2.0.0/.gitignore
+-rw-r--r--   0 bdraco     (501) staff       (20)     1139 2023-04-30 15:25:07.000000 onvif-zeep-async-2.0.0/.pre-commit-config.yaml
+-rw-r--r--   0 bdraco     (501) staff       (20)        0 2023-03-23 19:23:45.000000 onvif-zeep-async-2.0.0/CHANGES.txt
+-rw-r--r--   0 bdraco     (501) staff       (20)     1087 2023-03-23 19:23:45.000000 onvif-zeep-async-2.0.0/LICENSE
+-rw-r--r--   0 bdraco     (501) staff       (20)      100 2023-04-30 15:25:07.000000 onvif-zeep-async-2.0.0/MANIFEST.in
+-rw-r--r--   0 bdraco     (501) staff       (20)     1053 2023-04-30 15:25:07.000000 onvif-zeep-async-2.0.0/Makefile
+-rw-r--r--   0 bdraco     (501) staff       (20)     5290 2023-05-04 15:11:53.943872 onvif-zeep-async-2.0.0/PKG-INFO
+-rw-r--r--   0 bdraco     (501) staff       (20)     4926 2023-04-30 15:25:07.000000 onvif-zeep-async-2.0.0/README.rst
+-rw-r--r--   0 bdraco     (501) staff       (20)      188 2023-04-30 15:25:07.000000 onvif-zeep-async-2.0.0/bandit.yaml
+drwxr-xr-x   0 bdraco     (501) staff       (20)        0 2023-05-04 15:11:53.937467 onvif-zeep-async-2.0.0/examples/
+-rw-r--r--   0 bdraco     (501) staff       (20)     1497 2023-04-30 15:25:07.000000 onvif-zeep-async-2.0.0/examples/events.py
+-rw-r--r--   0 bdraco     (501) staff       (20)     1264 2023-04-30 15:25:07.000000 onvif-zeep-async-2.0.0/examples/rotate_image.py
+-rw-r--r--   0 bdraco     (501) staff       (20)     2459 2023-04-30 15:25:07.000000 onvif-zeep-async-2.0.0/examples/streaming.py
+drwxr-xr-x   0 bdraco     (501) staff       (20)        0 2023-05-04 15:11:53.938153 onvif-zeep-async-2.0.0/onvif/
+-rw-r--r--   0 bdraco     (501) staff       (20)      599 2023-04-30 15:25:07.000000 onvif-zeep-async-2.0.0/onvif/__init__.py
+-rw-r--r--   0 bdraco     (501) staff       (20)    24532 2023-05-04 15:11:27.000000 onvif-zeep-async-2.0.0/onvif/client.py
+-rw-r--r--   0 bdraco     (501) staff       (20)     2190 2023-04-30 15:25:07.000000 onvif-zeep-async-2.0.0/onvif/definition.py
+-rw-r--r--   0 bdraco     (501) staff       (20)      886 2023-04-30 15:25:07.000000 onvif-zeep-async-2.0.0/onvif/exceptions.py
+-rw-r--r--   0 bdraco     (501) staff       (20)        6 2023-05-04 15:11:34.000000 onvif-zeep-async-2.0.0/onvif/version.txt
+drwxr-xr-x   0 bdraco     (501) staff       (20)        0 2023-05-04 15:11:53.942818 onvif-zeep-async-2.0.0/onvif/wsdl/
+-rw-r--r--   0 bdraco     (501) staff       (20)    16384 2023-04-16 04:45:10.000000 onvif-zeep-async-2.0.0/onvif/wsdl/.events.wsdl.swn
+-rw-r--r--   0 bdraco     (501) staff       (20)       26 2023-04-30 15:25:07.000000 onvif-zeep-async-2.0.0/onvif/wsdl/__init__.py
+-rw-r--r--   0 bdraco     (501) staff       (20)    38072 2023-04-30 15:25:07.000000 onvif-zeep-async-2.0.0/onvif/wsdl/accesscontrol.wsdl
+-rw-r--r--   0 bdraco     (501) staff       (20)    57255 2023-04-30 15:25:07.000000 onvif-zeep-async-2.0.0/onvif/wsdl/actionengine.wsdl
+-rw-r--r--   0 bdraco     (501) staff       (20)     7263 2023-04-30 15:25:07.000000 onvif-zeep-async-2.0.0/onvif/wsdl/addressing
+-rw-r--r--   0 bdraco     (501) staff       (20)    79284 2023-04-30 15:25:07.000000 onvif-zeep-async-2.0.0/onvif/wsdl/advancedsecurity.wsdl
+-rw-r--r--   0 bdraco     (501) staff       (20)    24131 2023-04-30 15:25:07.000000 onvif-zeep-async-2.0.0/onvif/wsdl/analytics.wsdl
+-rw-r--r--   0 bdraco     (501) staff       (20)    31976 2023-04-30 15:25:07.000000 onvif-zeep-async-2.0.0/onvif/wsdl/analyticsdevice.wsdl
+-rw-r--r--   0 bdraco     (501) staff       (20)    23300 2023-04-30 15:25:07.000000 onvif-zeep-async-2.0.0/onvif/wsdl/b-2.xsd
+-rw-r--r--   0 bdraco     (501) staff       (20)     5100 2023-04-30 15:25:07.000000 onvif-zeep-async-2.0.0/onvif/wsdl/bf-2.xsd
+-rw-r--r--   0 bdraco     (501) staff       (20)    20498 2023-04-30 15:25:07.000000 onvif-zeep-async-2.0.0/onvif/wsdl/bw-2.wsdl
+-rw-r--r--   0 bdraco     (501) staff       (20)    60231 2023-04-30 15:25:07.000000 onvif-zeep-async-2.0.0/onvif/wsdl/deviceio.wsdl
+-rw-r--r--   0 bdraco     (501) staff       (20)   163209 2023-04-30 15:25:07.000000 onvif-zeep-async-2.0.0/onvif/wsdl/devicemgmt.wsdl
+-rw-r--r--   0 bdraco     (501) staff       (20)    24593 2023-04-30 15:25:07.000000 onvif-zeep-async-2.0.0/onvif/wsdl/display.wsdl
+-rw-r--r--   0 bdraco     (501) staff       (20)    53648 2023-04-30 15:25:07.000000 onvif-zeep-async-2.0.0/onvif/wsdl/doorcontrol.wsdl
+-rw-r--r--   0 bdraco     (501) staff       (20)     6249 2023-04-30 15:25:07.000000 onvif-zeep-async-2.0.0/onvif/wsdl/envelope
+-rw-r--r--   0 bdraco     (501) staff       (20)    37870 2023-04-30 15:25:07.000000 onvif-zeep-async-2.0.0/onvif/wsdl/events.wsdl
+-rw-r--r--   0 bdraco     (501) staff       (20)    17998 2023-04-30 15:25:07.000000 onvif-zeep-async-2.0.0/onvif/wsdl/imaging.wsdl
+-rw-r--r--   0 bdraco     (501) staff       (20)      511 2023-04-30 15:25:07.000000 onvif-zeep-async-2.0.0/onvif/wsdl/include
+-rw-r--r--   0 bdraco     (501) staff       (20)   174812 2023-04-30 15:25:07.000000 onvif-zeep-async-2.0.0/onvif/wsdl/media.wsdl
+-rw-r--r--   0 bdraco     (501) staff       (20)   363349 2023-04-30 15:25:07.000000 onvif-zeep-async-2.0.0/onvif/wsdl/onvif.xsd
+-rw-r--r--   0 bdraco     (501) staff       (20)    54058 2023-04-30 15:25:07.000000 onvif-zeep-async-2.0.0/onvif/wsdl/ptz.wsdl
+-rw-r--r--   0 bdraco     (501) staff       (20)     3660 2023-04-30 15:25:07.000000 onvif-zeep-async-2.0.0/onvif/wsdl/r-2.xsd
+-rw-r--r--   0 bdraco     (501) staff       (20)    17214 2023-04-30 15:25:07.000000 onvif-zeep-async-2.0.0/onvif/wsdl/receiver.wsdl
+-rw-r--r--   0 bdraco     (501) staff       (20)    40704 2023-04-30 15:25:07.000000 onvif-zeep-async-2.0.0/onvif/wsdl/recording.wsdl
+-rw-r--r--   0 bdraco     (501) staff       (20)     5596 2023-04-30 15:25:07.000000 onvif-zeep-async-2.0.0/onvif/wsdl/remotediscovery.wsdl
+-rw-r--r--   0 bdraco     (501) staff       (20)    10581 2023-04-30 15:25:07.000000 onvif-zeep-async-2.0.0/onvif/wsdl/replay.wsdl
+-rw-r--r--   0 bdraco     (501) staff       (20)     3727 2023-04-30 15:25:07.000000 onvif-zeep-async-2.0.0/onvif/wsdl/rw-2.wsdl
+-rw-r--r--   0 bdraco     (501) staff       (20)    43139 2023-04-30 15:25:07.000000 onvif-zeep-async-2.0.0/onvif/wsdl/search.wsdl
+-rw-r--r--   0 bdraco     (501) staff       (20)     8960 2023-04-30 15:25:07.000000 onvif-zeep-async-2.0.0/onvif/wsdl/t-1.xsd
+-rw-r--r--   0 bdraco     (501) staff       (20)     3738 2023-04-30 15:25:07.000000 onvif-zeep-async-2.0.0/onvif/wsdl/types.xsd
+-rw-r--r--   0 bdraco     (501) staff       (20)     5849 2023-04-30 15:25:07.000000 onvif-zeep-async-2.0.0/onvif/wsdl/ws-addr.xsd
+-rw-r--r--   0 bdraco     (501) staff       (20)    10455 2023-04-30 15:25:07.000000 onvif-zeep-async-2.0.0/onvif/wsdl/ws-discovery.xsd
+-rw-r--r--   0 bdraco     (501) staff       (20)     8836 2023-04-30 15:25:07.000000 onvif-zeep-async-2.0.0/onvif/wsdl/xml.xsd
+-rw-r--r--   0 bdraco     (501) staff       (20)     1639 2023-04-30 15:25:07.000000 onvif-zeep-async-2.0.0/onvif/wsdl/xmlmime
+drwxr-xr-x   0 bdraco     (501) staff       (20)        0 2023-05-04 15:11:53.943583 onvif-zeep-async-2.0.0/onvif_zeep_async.egg-info/
+-rw-r--r--   0 bdraco     (501) staff       (20)     5290 2023-05-04 15:11:53.000000 onvif-zeep-async-2.0.0/onvif_zeep_async.egg-info/PKG-INFO
+-rw-r--r--   0 bdraco     (501) staff       (20)     1445 2023-05-04 15:11:53.000000 onvif-zeep-async-2.0.0/onvif_zeep_async.egg-info/SOURCES.txt
+-rw-r--r--   0 bdraco     (501) staff       (20)        1 2023-05-04 15:11:53.000000 onvif-zeep-async-2.0.0/onvif_zeep_async.egg-info/dependency_links.txt
+-rw-r--r--   0 bdraco     (501) staff       (20)       45 2023-05-04 15:11:53.000000 onvif-zeep-async-2.0.0/onvif_zeep_async.egg-info/entry_points.txt
+-rw-r--r--   0 bdraco     (501) staff       (20)        1 2023-03-23 19:28:21.000000 onvif-zeep-async-2.0.0/onvif_zeep_async.egg-info/not-zip-safe
+-rw-r--r--   0 bdraco     (501) staff       (20)       47 2023-05-04 15:11:53.000000 onvif-zeep-async-2.0.0/onvif_zeep_async.egg-info/requires.txt
+-rw-r--r--   0 bdraco     (501) staff       (20)        6 2023-05-04 15:11:53.000000 onvif-zeep-async-2.0.0/onvif_zeep_async.egg-info/top_level.txt
+-rw-r--r--   0 bdraco     (501) staff       (20)     1741 2023-04-30 15:25:07.000000 onvif-zeep-async-2.0.0/pylintrc
+-rw-r--r--   0 bdraco     (501) staff       (20)       77 2023-04-30 15:25:07.000000 onvif-zeep-async-2.0.0/pyproject.toml
+-rw-r--r--   0 bdraco     (501) staff       (20)      224 2023-04-30 15:25:07.000000 onvif-zeep-async-2.0.0/requirements.txt
+-rw-r--r--   0 bdraco     (501) staff       (20)      409 2023-05-04 15:11:53.944110 onvif-zeep-async-2.0.0/setup.cfg
+-rw-r--r--   0 bdraco     (501) staff       (20)     1801 2023-04-30 15:25:07.000000 onvif-zeep-async-2.0.0/setup.py
+drwxr-xr-x   0 bdraco     (501) staff       (20)        0 2023-05-04 15:11:53.943705 onvif-zeep-async-2.0.0/tests/
+-rw-r--r--   0 bdraco     (501) staff       (20)     4133 2023-04-30 15:25:07.000000 onvif-zeep-async-2.0.0/tests/test.py
```

### Comparing `onvif-zeep-async-1.3.1/.gitignore` & `onvif-zeep-async-2.0.0/.gitignore`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-1.3.1/.pre-commit-config.yaml` & `onvif-zeep-async-2.0.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-1.3.1/LICENSE` & `onvif-zeep-async-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-1.3.1/Makefile` & `onvif-zeep-async-2.0.0/Makefile`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-1.3.1/PKG-INFO` & `onvif-zeep-async-2.0.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: onvif-zeep-async
-Version: 1.3.1
+Version: 2.0.0
 Summary: Async Python Client for ONVIF Camera
 Home-page: http://github.com/hunterjm/python-onvif-zeep-async
 Author: Cherish Chen
 Author-email: sinchb128@gmail.com
 Maintainer: sinchb
 Maintainer-email: sinchb128@gmail.com
 License: MIT
```

### Comparing `onvif-zeep-async-1.3.1/README.rst` & `onvif-zeep-async-2.0.0/README.rst`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-1.3.1/examples/events.py` & `onvif-zeep-async-2.0.0/examples/events.py`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-1.3.1/examples/rotate_image.py` & `onvif-zeep-async-2.0.0/examples/rotate_image.py`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-1.3.1/examples/streaming.py` & `onvif-zeep-async-2.0.0/examples/streaming.py`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-1.3.1/onvif/__init__.py` & `onvif-zeep-async-2.0.0/onvif/__init__.py`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-1.3.1/onvif/client.py` & `onvif-zeep-async-2.0.0/onvif/client.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import asyncio
 import contextlib
 import datetime as dt
 from functools import lru_cache
 import logging
 import os.path
 import ssl
-from typing import Any, Dict, Optional, Tuple
+from typing import Any, Callable, Dict, Optional, Tuple
 
 import httpx
 from httpx import AsyncClient, BasicAuth, DigestAuth, TransportError
 from zeep.cache import SqliteCache
 from zeep.client import AsyncClient as BaseZeepAsyncClient, Settings
 from zeep.exceptions import Fault, XMLSyntaxError
 import zeep.helpers
@@ -29,14 +29,16 @@
 logging.basicConfig(level=logging.INFO)
 logging.getLogger("zeep.client").setLevel(logging.CRITICAL)
 
 _DEFAULT_SETTINGS = Settings()
 _DEFAULT_SETTINGS.strict = False
 _DEFAULT_SETTINGS.xml_huge_tree = True
 
+_WSDL_PATH = os.path.join(os.path.dirname(os.path.dirname(__file__)), "wsdl")
+
 
 def create_no_verify_ssl_context() -> ssl.SSLContext:
     """Return an SSL context that does not verify the server certificate.
     This is a copy of aiohttp's create_default_context() function, with the
     ssl verify turned off and old SSL versions enabled.
 
     https://github.com/aio-libs/aiohttp/blob/33953f110e97eecc707e1402daa8d543f38a189b/aiohttp/connector.py#L911
@@ -172,48 +174,67 @@
         device_service.SetHostname(params)
     """
 
     @safe_func
     def __init__(
         self,
         xaddr: str,
-        user,
-        passwd,
-        url,
+        user: Optional[str],
+        passwd: Optional[str],
+        url: str,
         encrypt=True,
         no_cache=False,
         dt_diff=None,
         binding_name="",
         binding_key="",
-    ):
+    ) -> None:
         if not _path_isfile(url):
             raise ONVIFError("%s doesn`t exist!" % url)
 
         self.url = url
         self.xaddr = xaddr
         self.binding_key = binding_key
-        wsse = UsernameDigestTokenDtDiff(
-            user, passwd, dt_diff=dt_diff, use_digest=encrypt
-        )
+        # Set soap header for authentication
+        self.user = user
+        self.passwd = passwd
+        # Indicate wether password digest is needed
+        self.encrypt = encrypt
+        self.dt_diff = dt_diff
+        self.binding_name = binding_name
         # Create soap client
         client = AsyncClient(verify=_NO_VERIFY_SSL_CONTEXT, timeout=90)
         # The wsdl client should never actually be used, but it is required
         # to avoid creating another ssl context since the underlying code
         # will try to create a new one if it doesn't exist.
         wsdl_client = httpx.Client(verify=_NO_VERIFY_SSL_CONTEXT, timeout=90)
         self.transport = (
             AsyncTransport(client=client, wsdl_client=wsdl_client)
             if no_cache
             else AsyncTransport(
                 client=client, wsdl_client=wsdl_client, cache=SqliteCache()
             )
         )
+        self.document: Optional[Document] = None
+        self.zeep_client_authless: Optional[ZeepAsyncClient] = None
+        self.ws_client_authless: Optional[AsyncServiceProxy] = None
+        self.zeep_client: Optional[ZeepAsyncClient] = None
+        self.ws_client: Optional[AsyncServiceProxy] = None
+        self.create_type: Optional[Callable] = None
+        self.loop = asyncio.get_event_loop()
+
+    async def setup(self):
+        """Setup the transport."""
         settings = _DEFAULT_SETTINGS
-        self.document = _cached_document(url)
-        self.binding_name = binding_name
+        binding_name = self.binding_name
+        wsse = UsernameDigestTokenDtDiff(
+            self.user, self.passwd, dt_diff=self.dt_diff, use_digest=self.encrypt
+        )
+        self.document = await self.loop.run_in_executor(
+            None, _cached_document, self.url
+        )
         self.zeep_client_authless = ZeepAsyncClient(
             wsdl=self.document,
             transport=self.transport,
             settings=settings,
             plugins=[WsAddressingPlugin()],
         )
         self.ws_client_authless = self.zeep_client_authless.create_service(
@@ -223,22 +244,14 @@
             wsdl=self.document,
             wsse=wsse,
             transport=self.transport,
             settings=settings,
             plugins=[WsAddressingPlugin()],
         )
         self.ws_client = self.zeep_client.create_service(binding_name, self.xaddr)
-
-        # Set soap header for authentication
-        self.user = user
-        self.passwd = passwd
-        # Indicate wether password digest is needed
-        self.encrypt = encrypt
-        self.dt_diff = dt_diff
-
         namespace = binding_name[binding_name.find("{") + 1 : binding_name.find("}")]
         available_ns = self.zeep_client.namespaces
         active_ns = (
             list(available_ns.keys())[list(available_ns.values()).index(namespace)]
             or "ns0"
         )
         self.create_type = lambda x: self.zeep_client.get_element(active_ns + ":" + x)()
@@ -298,35 +311,35 @@
         self._service: Optional[ONVIFService] = None
         self._operation: Optional[SoapOperation] = None
         self._device = device
         self._config = config
 
     async def setup(self) -> ONVIFService:
         """Setup the notification processor."""
-        notify_service = self._device.create_notification_service()
+        notify_service = await self._device.create_notification_service()
         notify_subscribe = await notify_service.Subscribe(self._config)
         # pylint: disable=protected-access
         self._device.xaddrs[
             "http://www.onvif.org/ver10/events/wsdl/NotificationConsumer"
         ] = notify_subscribe.SubscriptionReference.Address._value_1
         # Create subscription manager
         # 5.2.3 BASIC NOTIFICATION INTERFACE - NOTIFY
         # Call SetSynchronizationPoint to generate a notification message
         # to ensure the webhooks are working.
         #
         # If this fails this is OK as it just means we will switch
         # to webhook later when the first notification is received.
-        service = self._device.create_onvif_service(
+        service = await self._device.create_onvif_service(
             "pullpoint", port_type="NotificationConsumer"
         )
         self._operation = service.document.bindings[service.binding_name].get(
             "PullMessages"
         )
         self._service = service
-        return self._device.create_subscription_service("NotificationConsumer")
+        return await self._device.create_subscription_service("NotificationConsumer")
 
     async def start(self) -> None:
         """Start the notification processor."""
         assert self._service, "Call setup first"
         try:
             await self._service.SetSynchronizationPoint()
         except (Fault, asyncio.TimeoutError, TransportError, TypeError):
@@ -368,23 +381,23 @@
     >>> mycam.ptz.GetConfiguration()
     # Another way:
     >>> ptz_service.GetConfiguration()
     """
 
     def __init__(
         self,
-        host,
-        port,
-        user,
-        passwd,
-        wsdl_dir=os.path.join(os.path.dirname(os.path.dirname(__file__)), "wsdl"),
+        host: str,
+        port: int,
+        user: Optional[str],
+        passwd: Optional[str],
+        wsdl_dir: str = _WSDL_PATH,
         encrypt=True,
         no_cache=False,
         adjust_time=False,
-    ):
+    ) -> None:
         os.environ.pop("http_proxy", None)
         os.environ.pop("https_proxy", None)
         self.host = host
         self.port = int(port)
         self.user = user
         self.passwd = passwd
         self.wsdl_dir = wsdl_dir
@@ -398,26 +411,25 @@
         # Active service client container
         self.services: Dict[Tuple[str, Optional[str]], ONVIFService] = {}
 
         self.to_dict = ONVIFService.to_dict
 
         self._snapshot_uris = {}
         self._snapshot_client = AsyncClient(verify=_NO_VERIFY_SSL_CONTEXT)
-        self._background_tasks = set()
 
     async def get_capabilities(self) -> Dict[str, Any]:
         """Get device capabilities."""
         if self._capabilities is None:
             await self.update_xaddrs()
         return self._capabilities
 
     async def update_xaddrs(self):
         """Update xaddrs for services."""
         self.dt_diff = None
-        devicemgmt = self.create_devicemgmt_service()
+        devicemgmt = await self.create_devicemgmt_service()
         if self.adjust_time:
             try:
                 sys_date = await devicemgmt.authless_GetSystemDateAndTime()
             except zeep.exceptions.Fault:
                 # Looks like we should try with auth
                 sys_date = await devicemgmt.GetSystemDateAndTime()
             cdate = sys_date.UTCDateTime
@@ -428,15 +440,15 @@
                 cdate.Time.Hour,
                 cdate.Time.Minute,
                 cdate.Time.Second,
             )
             self.dt_diff = cam_date - dt.datetime.utcnow()
             await devicemgmt.close()
             del self.services[devicemgmt.binding_key]
-            devicemgmt = self.create_devicemgmt_service()
+            devicemgmt = await self.create_devicemgmt_service()
 
         # Get XAddr of services on the device
         self.xaddrs = {}
         capabilities = await devicemgmt.GetCapabilities({"Category": "All"})
         for name in capabilities:
             capability = capabilities[name]
             try:
@@ -451,15 +463,15 @@
             logger.exception("Failed to parse capabilities")
 
     async def create_pullpoint_subscription(
         self, config: Optional[Dict[str, Any]] = None
     ) -> bool:
         """Create a pullpoint subscription."""
         try:
-            events = self.create_events_service()
+            events = await self.create_events_service()
             pullpoint = await events.CreatePullPointSubscription(config or {})
             # pylint: disable=protected-access
             self.xaddrs[
                 "http://www.onvif.org/ver10/events/wsdl/PullPointSubscription"
             ] = pullpoint.SubscriptionReference.Address._value_1
         except Fault:
             return False
@@ -477,15 +489,15 @@
         for service in self.services.values():
             await service.close()
 
     async def get_snapshot_uri(self, profile_token):
         """Get the snapshot uri for a given profile."""
         uri = self._snapshot_uris.get(profile_token)
         if uri is None:
-            media_service = self.create_media_service()
+            media_service = await self.create_media_service()
             req = media_service.create_type("GetSnapshotUri")
             req.ProfileToken = profile_token
             result = await media_service.GetSnapshotUri(req)
             uri = result.Uri
             self._snapshot_uris[profile_token] = uri
         return uri
 
@@ -513,15 +525,17 @@
             raise ONVIFAuthError(f"Failed to authenticate to {uri}")
 
         if response.status_code < 300:
             return response.content
 
         return None
 
-    def get_definition(self, name, port_type=None):
+    def get_definition(
+        self, name: str, port_type: Optional[str] = None
+    ) -> Tuple[str, str, str]:
         """Returns xaddr and wsdl of specified service"""
         # Check if the service is supported
         if name not in SERVICES:
             raise ONVIFError("Unknown service %s" % name)
         wsdl_file = SERVICES[name]["wsdl"]
         namespace = SERVICES[name]["ns"]
 
@@ -547,15 +561,17 @@
         # Get other XAddr
         xaddr = self.xaddrs.get(namespace)
         if not xaddr:
             raise ONVIFError("Device doesn`t support service: %s" % name)
 
         return xaddr, wsdlpath, binding_name
 
-    def create_onvif_service(self, name, port_type=None):
+    async def create_onvif_service(
+        self, name: str, port_type: Optional[str] = None
+    ) -> ONVIFService:
         """Create ONVIF service client"""
         name = name.lower()
         # Don't re-create bindings if the xaddr remains the same.
         # The xaddr can change when a new PullPointSubscription is created.
         binding_key = (name, port_type)
 
         xaddr, wsdl_file, binding_name = self.get_definition(name, port_type)
@@ -568,17 +584,15 @@
                 # Close the existing service since it's no longer valid.
                 # This can happen when a new PullPointSubscription is created.
                 logger.debug(
                     "Closing service %s with %s", binding_key, existing_service.xaddr
                 )
                 # Hold a reference to the task so it doesn't get
                 # garbage collected before it completes.
-                task = asyncio.create_task(existing_service.close())
-                task.add_done_callback(self._background_tasks.remove)
-                self._background_tasks.add(task)
+                await existing_service.close()
             self.services.pop(binding_key)
 
         logger.debug("Creating service %s with %s", binding_key, xaddr)
 
         service = ONVIFService(
             xaddr,
             self.user,
@@ -586,67 +600,70 @@
             wsdl_file,
             self.encrypt,
             no_cache=self.no_cache,
             dt_diff=self.dt_diff,
             binding_name=binding_name,
             binding_key=binding_key,
         )
+        await service.setup()
 
         self.services[binding_key] = service
 
         return service
 
-    def create_devicemgmt_service(self):
+    async def create_devicemgmt_service(self):
         """Service creation helper."""
-        return self.create_onvif_service("devicemgmt")
+        return await self.create_onvif_service("devicemgmt")
 
-    def create_media_service(self):
+    async def create_media_service(self):
         """Service creation helper."""
-        return self.create_onvif_service("media")
+        return await self.create_onvif_service("media")
 
-    def create_ptz_service(self):
+    async def create_ptz_service(self):
         """Service creation helper."""
-        return self.create_onvif_service("ptz")
+        return await self.create_onvif_service("ptz")
 
-    def create_imaging_service(self):
+    async def create_imaging_service(self):
         """Service creation helper."""
-        return self.create_onvif_service("imaging")
+        return await self.create_onvif_service("imaging")
 
-    def create_deviceio_service(self):
+    async def create_deviceio_service(self):
         """Service creation helper."""
-        return self.create_onvif_service("deviceio")
+        return await self.create_onvif_service("deviceio")
 
-    def create_events_service(self):
+    async def create_events_service(self):
         """Service creation helper."""
-        return self.create_onvif_service("events")
+        return await self.create_onvif_service("events")
 
-    def create_analytics_service(self):
+    async def create_analytics_service(self):
         """Service creation helper."""
-        return self.create_onvif_service("analytics")
+        return await self.create_onvif_service("analytics")
 
-    def create_recording_service(self):
+    async def create_recording_service(self):
         """Service creation helper."""
-        return self.create_onvif_service("recording")
+        return await self.create_onvif_service("recording")
 
-    def create_search_service(self):
+    async def create_search_service(self):
         """Service creation helper."""
-        return self.create_onvif_service("search")
+        return await self.create_onvif_service("search")
 
-    def create_replay_service(self):
+    async def create_replay_service(self):
         """Service creation helper."""
-        return self.create_onvif_service("replay")
+        return await self.create_onvif_service("replay")
 
-    def create_pullpoint_service(self):
+    async def create_pullpoint_service(self):
         """Service creation helper."""
-        return self.create_onvif_service("pullpoint", port_type="PullPointSubscription")
+        return await self.create_onvif_service(
+            "pullpoint", port_type="PullPointSubscription"
+        )
 
-    def create_notification_service(self):
+    async def create_notification_service(self):
         """Service creation helper."""
-        return self.create_onvif_service("notification")
+        return await self.create_onvif_service("notification")
 
-    def create_subscription_service(self, port_type=None):
+    async def create_subscription_service(self, port_type=None):
         """Service creation helper."""
-        return self.create_onvif_service("subscription", port_type=port_type)
+        return await self.create_onvif_service("subscription", port_type=port_type)
 
-    def create_receiver_service(self):
+    async def create_receiver_service(self):
         """Service creation helper."""
-        return self.create_onvif_service("receiver")
+        return await self.create_onvif_service("receiver")
```

### Comparing `onvif-zeep-async-1.3.1/onvif/definition.py` & `onvif-zeep-async-2.0.0/onvif/definition.py`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-1.3.1/onvif/exceptions.py` & `onvif-zeep-async-2.0.0/onvif/exceptions.py`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-1.3.1/onvif/wsdl/.events.wsdl.swn` & `onvif-zeep-async-2.0.0/onvif/wsdl/.events.wsdl.swn`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-1.3.1/onvif/wsdl/accesscontrol.wsdl` & `onvif-zeep-async-2.0.0/onvif/wsdl/accesscontrol.wsdl`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-1.3.1/onvif/wsdl/actionengine.wsdl` & `onvif-zeep-async-2.0.0/onvif/wsdl/actionengine.wsdl`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-1.3.1/onvif/wsdl/addressing` & `onvif-zeep-async-2.0.0/onvif/wsdl/addressing`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-1.3.1/onvif/wsdl/advancedsecurity.wsdl` & `onvif-zeep-async-2.0.0/onvif/wsdl/advancedsecurity.wsdl`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-1.3.1/onvif/wsdl/analytics.wsdl` & `onvif-zeep-async-2.0.0/onvif/wsdl/analytics.wsdl`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-1.3.1/onvif/wsdl/analyticsdevice.wsdl` & `onvif-zeep-async-2.0.0/onvif/wsdl/analyticsdevice.wsdl`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-1.3.1/onvif/wsdl/b-2.xsd` & `onvif-zeep-async-2.0.0/onvif/wsdl/b-2.xsd`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-1.3.1/onvif/wsdl/bf-2.xsd` & `onvif-zeep-async-2.0.0/onvif/wsdl/bf-2.xsd`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-1.3.1/onvif/wsdl/bw-2.wsdl` & `onvif-zeep-async-2.0.0/onvif/wsdl/bw-2.wsdl`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-1.3.1/onvif/wsdl/deviceio.wsdl` & `onvif-zeep-async-2.0.0/onvif/wsdl/deviceio.wsdl`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-1.3.1/onvif/wsdl/devicemgmt.wsdl` & `onvif-zeep-async-2.0.0/onvif/wsdl/devicemgmt.wsdl`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-1.3.1/onvif/wsdl/display.wsdl` & `onvif-zeep-async-2.0.0/onvif/wsdl/display.wsdl`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-1.3.1/onvif/wsdl/doorcontrol.wsdl` & `onvif-zeep-async-2.0.0/onvif/wsdl/doorcontrol.wsdl`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-1.3.1/onvif/wsdl/envelope` & `onvif-zeep-async-2.0.0/onvif/wsdl/envelope`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-1.3.1/onvif/wsdl/events.wsdl` & `onvif-zeep-async-2.0.0/onvif/wsdl/events.wsdl`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-1.3.1/onvif/wsdl/imaging.wsdl` & `onvif-zeep-async-2.0.0/onvif/wsdl/imaging.wsdl`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-1.3.1/onvif/wsdl/media.wsdl` & `onvif-zeep-async-2.0.0/onvif/wsdl/media.wsdl`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-1.3.1/onvif/wsdl/onvif.xsd` & `onvif-zeep-async-2.0.0/onvif/wsdl/onvif.xsd`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-1.3.1/onvif/wsdl/ptz.wsdl` & `onvif-zeep-async-2.0.0/onvif/wsdl/ptz.wsdl`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-1.3.1/onvif/wsdl/r-2.xsd` & `onvif-zeep-async-2.0.0/onvif/wsdl/r-2.xsd`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-1.3.1/onvif/wsdl/receiver.wsdl` & `onvif-zeep-async-2.0.0/onvif/wsdl/receiver.wsdl`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-1.3.1/onvif/wsdl/recording.wsdl` & `onvif-zeep-async-2.0.0/onvif/wsdl/recording.wsdl`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-1.3.1/onvif/wsdl/remotediscovery.wsdl` & `onvif-zeep-async-2.0.0/onvif/wsdl/remotediscovery.wsdl`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-1.3.1/onvif/wsdl/replay.wsdl` & `onvif-zeep-async-2.0.0/onvif/wsdl/replay.wsdl`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-1.3.1/onvif/wsdl/rw-2.wsdl` & `onvif-zeep-async-2.0.0/onvif/wsdl/rw-2.wsdl`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-1.3.1/onvif/wsdl/search.wsdl` & `onvif-zeep-async-2.0.0/onvif/wsdl/search.wsdl`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-1.3.1/onvif/wsdl/t-1.xsd` & `onvif-zeep-async-2.0.0/onvif/wsdl/t-1.xsd`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-1.3.1/onvif/wsdl/types.xsd` & `onvif-zeep-async-2.0.0/onvif/wsdl/types.xsd`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-1.3.1/onvif/wsdl/ws-addr.xsd` & `onvif-zeep-async-2.0.0/onvif/wsdl/ws-addr.xsd`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-1.3.1/onvif/wsdl/ws-discovery.xsd` & `onvif-zeep-async-2.0.0/onvif/wsdl/ws-discovery.xsd`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-1.3.1/onvif/wsdl/xml.xsd` & `onvif-zeep-async-2.0.0/onvif/wsdl/xml.xsd`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-1.3.1/onvif/wsdl/xmlmime` & `onvif-zeep-async-2.0.0/onvif/wsdl/xmlmime`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-1.3.1/onvif_zeep_async.egg-info/PKG-INFO` & `onvif-zeep-async-2.0.0/onvif_zeep_async.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: onvif-zeep-async
-Version: 1.3.1
+Version: 2.0.0
 Summary: Async Python Client for ONVIF Camera
 Home-page: http://github.com/hunterjm/python-onvif-zeep-async
 Author: Cherish Chen
 Author-email: sinchb128@gmail.com
 Maintainer: sinchb
 Maintainer-email: sinchb128@gmail.com
 License: MIT
```

### Comparing `onvif-zeep-async-1.3.1/onvif_zeep_async.egg-info/SOURCES.txt` & `onvif-zeep-async-2.0.0/onvif_zeep_async.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-1.3.1/pylintrc` & `onvif-zeep-async-2.0.0/pylintrc`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-1.3.1/setup.py` & `onvif-zeep-async-2.0.0/setup.py`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-1.3.1/tests/test.py` & `onvif-zeep-async-2.0.0/tests/test.py`

 * *Files identical despite different names*

