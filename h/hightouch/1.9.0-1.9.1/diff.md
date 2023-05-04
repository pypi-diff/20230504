# Comparing `tmp/hightouch-1.9.0.tar.gz` & `tmp/hightouch-1.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hightouch-1.9.0.tar", last modified: Tue Mar  7 04:40:21 2023, max compression
+gzip compressed data, was "hightouch-1.9.1.tar", last modified: Wed Mar  8 22:53:19 2023, max compression
```

## Comparing `hightouch-1.9.0.tar` & `hightouch-1.9.1.tar`

### file list

```diff
@@ -1,71 +1,71 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 04:40:21.400530 hightouch-1.9.0/
--rw-r--r--   0 runner    (1001) docker     (123)     3435 2023-03-07 04:40:21.400530 hightouch-1.9.0/PKG-INFO
--rwxr-xr-x   0 runner    (1001) docker     (123)     3206 2023-03-07 04:40:10.000000 hightouch-1.9.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-07 04:40:21.400530 hightouch-1.9.0/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     1014 2023-03-07 04:40:10.000000 hightouch-1.9.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 04:40:21.396530 hightouch-1.9.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 04:40:21.396530 hightouch-1.9.0/src/hightouch/
--rwxr-xr-x   0 runner    (1001) docker     (123)       19 2023-03-07 04:40:10.000000 hightouch-1.9.0/src/hightouch/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 04:40:21.396530 hightouch-1.9.0/src/hightouch/models/
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 04:40:10.000000 hightouch-1.9.0/src/hightouch/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 04:40:21.400530 hightouch-1.9.0/src/hightouch/models/operations/
--rwxr-xr-x   0 runner    (1001) docker     (123)     2444 2023-03-07 04:40:10.000000 hightouch-1.9.0/src/hightouch/models/operations/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1320 2023-03-07 04:40:10.000000 hightouch-1.9.0/src/hightouch/models/operations/createdestination.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1272 2023-03-07 04:40:10.000000 hightouch-1.9.0/src/hightouch/models/operations/createmodel.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1280 2023-03-07 04:40:10.000000 hightouch-1.9.0/src/hightouch/models/operations/createsource.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1264 2023-03-07 04:40:10.000000 hightouch-1.9.0/src/hightouch/models/operations/createsync.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1031 2023-03-07 04:40:10.000000 hightouch-1.9.0/src/hightouch/models/operations/getdestination.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      959 2023-03-07 04:40:10.000000 hightouch-1.9.0/src/hightouch/models/operations/getmodel.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1150 2023-03-07 04:40:10.000000 hightouch-1.9.0/src/hightouch/models/operations/getsource.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      947 2023-03-07 04:40:10.000000 hightouch-1.9.0/src/hightouch/models/operations/getsync.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2392 2023-03-07 04:40:10.000000 hightouch-1.9.0/src/hightouch/models/operations/listdestination.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2308 2023-03-07 04:40:10.000000 hightouch-1.9.0/src/hightouch/models/operations/listmodel.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2143 2023-03-07 04:40:10.000000 hightouch-1.9.0/src/hightouch/models/operations/listsource.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2691 2023-03-07 04:40:10.000000 hightouch-1.9.0/src/hightouch/models/operations/listsync.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2991 2023-03-07 04:40:10.000000 hightouch-1.9.0/src/hightouch/models/operations/listsyncruns.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1420 2023-03-07 04:40:10.000000 hightouch-1.9.0/src/hightouch/models/operations/triggerrun.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1125 2023-03-07 04:40:10.000000 hightouch-1.9.0/src/hightouch/models/operations/triggerruncustom.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1594 2023-03-07 04:40:10.000000 hightouch-1.9.0/src/hightouch/models/operations/updatedestination.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1522 2023-03-07 04:40:10.000000 hightouch-1.9.0/src/hightouch/models/operations/updatemodel.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1534 2023-03-07 04:40:10.000000 hightouch-1.9.0/src/hightouch/models/operations/updatesource.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1510 2023-03-07 04:40:10.000000 hightouch-1.9.0/src/hightouch/models/operations/updatesync.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 04:40:21.400530 hightouch-1.9.0/src/hightouch/models/shared/
--rwxr-xr-x   0 runner    (1001) docker     (123)     1735 2023-03-07 04:40:10.000000 hightouch-1.9.0/src/hightouch/models/shared/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      357 2023-03-07 04:40:10.000000 hightouch-1.9.0/src/hightouch/models/shared/cronschedule.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1042 2023-03-07 04:40:10.000000 hightouch-1.9.0/src/hightouch/models/shared/dbtschedule.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1820 2023-03-07 04:40:10.000000 hightouch-1.9.0/src/hightouch/models/shared/destination.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      824 2023-03-07 04:40:10.000000 hightouch-1.9.0/src/hightouch/models/shared/destinationcreate.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      718 2023-03-07 04:40:10.000000 hightouch-1.9.0/src/hightouch/models/shared/destinationupdate.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      152 2023-03-07 04:40:10.000000 hightouch-1.9.0/src/hightouch/models/shared/internalservererror_enum.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      570 2023-03-07 04:40:10.000000 hightouch-1.9.0/src/hightouch/models/shared/interval.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      427 2023-03-07 04:40:10.000000 hightouch-1.9.0/src/hightouch/models/shared/intervalschedule.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      167 2023-03-07 04:40:10.000000 hightouch-1.9.0/src/hightouch/models/shared/intervalunit_enum.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5751 2023-03-07 04:40:10.000000 hightouch-1.9.0/src/hightouch/models/shared/model.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3788 2023-03-07 04:40:10.000000 hightouch-1.9.0/src/hightouch/models/shared/modelcreate.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3594 2023-03-07 04:40:10.000000 hightouch-1.9.0/src/hightouch/models/shared/modelupdate.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1622 2023-03-07 04:40:10.000000 hightouch-1.9.0/src/hightouch/models/shared/record_day_boolean_or_undefined_.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1701 2023-03-07 04:40:10.000000 hightouch-1.9.0/src/hightouch/models/shared/source.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      809 2023-03-07 04:40:10.000000 hightouch-1.9.0/src/hightouch/models/shared/sourcecreate.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      703 2023-03-07 04:40:10.000000 hightouch-1.9.0/src/hightouch/models/shared/sourceupdate.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3601 2023-03-07 04:40:10.000000 hightouch-1.9.0/src/hightouch/models/shared/sync.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1890 2023-03-07 04:40:10.000000 hightouch-1.9.0/src/hightouch/models/shared/synccreate.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4391 2023-03-07 04:40:10.000000 hightouch-1.9.0/src/hightouch/models/shared/syncrun.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      330 2023-03-07 04:40:10.000000 hightouch-1.9.0/src/hightouch/models/shared/syncrunstatus_enum.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      377 2023-03-07 04:40:10.000000 hightouch-1.9.0/src/hightouch/models/shared/syncstatus_enum.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1700 2023-03-07 04:40:10.000000 hightouch-1.9.0/src/hightouch/models/shared/syncupdate.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      936 2023-03-07 04:40:10.000000 hightouch-1.9.0/src/hightouch/models/shared/triggerruncustominput.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      530 2023-03-07 04:40:10.000000 hightouch-1.9.0/src/hightouch/models/shared/triggerruninput.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      431 2023-03-07 04:40:10.000000 hightouch-1.9.0/src/hightouch/models/shared/triggerrunoutput.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      649 2023-03-07 04:40:10.000000 hightouch-1.9.0/src/hightouch/models/shared/validateerrorjson.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      897 2023-03-07 04:40:10.000000 hightouch-1.9.0/src/hightouch/models/shared/visualcronschedule.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    35734 2023-03-07 04:40:10.000000 hightouch-1.9.0/src/hightouch/sdk.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 04:40:21.400530 hightouch-1.9.0/src/hightouch/utils/
--rwxr-xr-x   0 runner    (1001) docker     (123)       44 2023-03-07 04:40:10.000000 hightouch-1.9.0/src/hightouch/utils/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3629 2023-03-07 04:40:10.000000 hightouch-1.9.0/src/hightouch/utils/retries.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    23642 2023-03-07 04:40:10.000000 hightouch-1.9.0/src/hightouch/utils/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 04:40:21.396530 hightouch-1.9.0/src/hightouch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3435 2023-03-07 04:40:21.000000 hightouch-1.9.0/src/hightouch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2597 2023-03-07 04:40:21.000000 hightouch-1.9.0/src/hightouch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-07 04:40:21.000000 hightouch-1.9.0/src/hightouch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      321 2023-03-07 04:40:21.000000 hightouch-1.9.0/src/hightouch.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-03-07 04:40:21.000000 hightouch-1.9.0/src/hightouch.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 22:53:19.041298 hightouch-1.9.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     3435 2023-03-08 22:53:19.041298 hightouch-1.9.1/PKG-INFO
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3206 2023-03-08 22:52:44.000000 hightouch-1.9.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-08 22:53:19.041298 hightouch-1.9.1/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1014 2023-03-08 22:52:44.000000 hightouch-1.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 22:53:19.025295 hightouch-1.9.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 22:53:19.029296 hightouch-1.9.1/src/hightouch/
+-rwxr-xr-x   0 runner    (1001) docker     (123)       19 2023-03-08 22:52:44.000000 hightouch-1.9.1/src/hightouch/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 22:53:19.033296 hightouch-1.9.1/src/hightouch/models/
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 22:52:44.000000 hightouch-1.9.1/src/hightouch/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 22:53:19.033296 hightouch-1.9.1/src/hightouch/models/operations/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2444 2023-03-08 22:52:44.000000 hightouch-1.9.1/src/hightouch/models/operations/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1320 2023-03-08 22:52:44.000000 hightouch-1.9.1/src/hightouch/models/operations/createdestination.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1272 2023-03-08 22:52:44.000000 hightouch-1.9.1/src/hightouch/models/operations/createmodel.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1280 2023-03-08 22:52:44.000000 hightouch-1.9.1/src/hightouch/models/operations/createsource.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1264 2023-03-08 22:52:44.000000 hightouch-1.9.1/src/hightouch/models/operations/createsync.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1031 2023-03-08 22:52:44.000000 hightouch-1.9.1/src/hightouch/models/operations/getdestination.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      959 2023-03-08 22:52:44.000000 hightouch-1.9.1/src/hightouch/models/operations/getmodel.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1150 2023-03-08 22:52:44.000000 hightouch-1.9.1/src/hightouch/models/operations/getsource.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      947 2023-03-08 22:52:44.000000 hightouch-1.9.1/src/hightouch/models/operations/getsync.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2392 2023-03-08 22:52:44.000000 hightouch-1.9.1/src/hightouch/models/operations/listdestination.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2308 2023-03-08 22:52:44.000000 hightouch-1.9.1/src/hightouch/models/operations/listmodel.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2143 2023-03-08 22:52:44.000000 hightouch-1.9.1/src/hightouch/models/operations/listsource.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2691 2023-03-08 22:52:44.000000 hightouch-1.9.1/src/hightouch/models/operations/listsync.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2991 2023-03-08 22:52:44.000000 hightouch-1.9.1/src/hightouch/models/operations/listsyncruns.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1420 2023-03-08 22:52:44.000000 hightouch-1.9.1/src/hightouch/models/operations/triggerrun.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1125 2023-03-08 22:52:44.000000 hightouch-1.9.1/src/hightouch/models/operations/triggerruncustom.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1594 2023-03-08 22:52:44.000000 hightouch-1.9.1/src/hightouch/models/operations/updatedestination.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1522 2023-03-08 22:52:44.000000 hightouch-1.9.1/src/hightouch/models/operations/updatemodel.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1534 2023-03-08 22:52:44.000000 hightouch-1.9.1/src/hightouch/models/operations/updatesource.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1510 2023-03-08 22:52:44.000000 hightouch-1.9.1/src/hightouch/models/operations/updatesync.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 22:53:19.041298 hightouch-1.9.1/src/hightouch/models/shared/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1735 2023-03-08 22:52:44.000000 hightouch-1.9.1/src/hightouch/models/shared/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      357 2023-03-08 22:52:44.000000 hightouch-1.9.1/src/hightouch/models/shared/cronschedule.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1042 2023-03-08 22:52:44.000000 hightouch-1.9.1/src/hightouch/models/shared/dbtschedule.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1820 2023-03-08 22:52:44.000000 hightouch-1.9.1/src/hightouch/models/shared/destination.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      824 2023-03-08 22:52:44.000000 hightouch-1.9.1/src/hightouch/models/shared/destinationcreate.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      718 2023-03-08 22:52:44.000000 hightouch-1.9.1/src/hightouch/models/shared/destinationupdate.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      152 2023-03-08 22:52:44.000000 hightouch-1.9.1/src/hightouch/models/shared/internalservererror_enum.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      570 2023-03-08 22:52:44.000000 hightouch-1.9.1/src/hightouch/models/shared/interval.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      427 2023-03-08 22:52:44.000000 hightouch-1.9.1/src/hightouch/models/shared/intervalschedule.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      167 2023-03-08 22:52:44.000000 hightouch-1.9.1/src/hightouch/models/shared/intervalunit_enum.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5751 2023-03-08 22:52:44.000000 hightouch-1.9.1/src/hightouch/models/shared/model.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3788 2023-03-08 22:52:44.000000 hightouch-1.9.1/src/hightouch/models/shared/modelcreate.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3594 2023-03-08 22:52:44.000000 hightouch-1.9.1/src/hightouch/models/shared/modelupdate.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1622 2023-03-08 22:52:44.000000 hightouch-1.9.1/src/hightouch/models/shared/record_day_boolean_or_undefined_.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1701 2023-03-08 22:52:44.000000 hightouch-1.9.1/src/hightouch/models/shared/source.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      809 2023-03-08 22:52:44.000000 hightouch-1.9.1/src/hightouch/models/shared/sourcecreate.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      703 2023-03-08 22:52:44.000000 hightouch-1.9.1/src/hightouch/models/shared/sourceupdate.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3601 2023-03-08 22:52:44.000000 hightouch-1.9.1/src/hightouch/models/shared/sync.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1890 2023-03-08 22:52:44.000000 hightouch-1.9.1/src/hightouch/models/shared/synccreate.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4391 2023-03-08 22:52:44.000000 hightouch-1.9.1/src/hightouch/models/shared/syncrun.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      330 2023-03-08 22:52:44.000000 hightouch-1.9.1/src/hightouch/models/shared/syncrunstatus_enum.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      377 2023-03-08 22:52:44.000000 hightouch-1.9.1/src/hightouch/models/shared/syncstatus_enum.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1700 2023-03-08 22:52:44.000000 hightouch-1.9.1/src/hightouch/models/shared/syncupdate.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      936 2023-03-08 22:52:44.000000 hightouch-1.9.1/src/hightouch/models/shared/triggerruncustominput.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      530 2023-03-08 22:52:44.000000 hightouch-1.9.1/src/hightouch/models/shared/triggerruninput.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      431 2023-03-08 22:52:44.000000 hightouch-1.9.1/src/hightouch/models/shared/triggerrunoutput.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      649 2023-03-08 22:52:44.000000 hightouch-1.9.1/src/hightouch/models/shared/validateerrorjson.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      897 2023-03-08 22:52:44.000000 hightouch-1.9.1/src/hightouch/models/shared/visualcronschedule.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    35734 2023-03-08 22:52:44.000000 hightouch-1.9.1/src/hightouch/sdk.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 22:53:19.041298 hightouch-1.9.1/src/hightouch/utils/
+-rwxr-xr-x   0 runner    (1001) docker     (123)       44 2023-03-08 22:52:44.000000 hightouch-1.9.1/src/hightouch/utils/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3629 2023-03-08 22:52:44.000000 hightouch-1.9.1/src/hightouch/utils/retries.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    23642 2023-03-08 22:52:44.000000 hightouch-1.9.1/src/hightouch/utils/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 22:53:19.033296 hightouch-1.9.1/src/hightouch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3435 2023-03-08 22:53:18.000000 hightouch-1.9.1/src/hightouch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2597 2023-03-08 22:53:18.000000 hightouch-1.9.1/src/hightouch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-08 22:53:18.000000 hightouch-1.9.1/src/hightouch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      321 2023-03-08 22:53:18.000000 hightouch-1.9.1/src/hightouch.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-03-08 22:53:18.000000 hightouch-1.9.1/src/hightouch.egg-info/top_level.txt
```

### Comparing `hightouch-1.9.0/PKG-INFO` & `hightouch-1.9.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hightouch
-Version: 1.9.0
+Version: 1.9.1
 Summary: Python SDK for Hightouch API
 Home-page: UNKNOWN
 Author: Speakeasy
 License: UNKNOWN
 Platform: UNKNOWN
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: hightouch Version: 1.9.0 Summary: Python SDK for
+Metadata-Version: 2.1 Name: hightouch Version: 1.9.1 Summary: Python SDK for
 Hightouch API Home-page: UNKNOWN Author: Speakeasy License: UNKNOWN Platform:
 UNKNOWN Requires-Python: >=3.9 Description-Content-Type: text/markdown
    [https://user-images.githubusercontent.com/6267663/221538828-de1343f2-b249-
                          4ba2-85e3-a2e43cc5f265.svg]
                            ****** Python SDK ******
    Hightouch exposes a REST API that lets users interact with resources like
                    syncs, models, sources and destinations.
```

### Comparing `hightouch-1.9.0/README.md` & `hightouch-1.9.1/README.md`

 * *Files identical despite different names*

### Comparing `hightouch-1.9.0/setup.py` & `hightouch-1.9.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     with open("README.md", "r") as fh:
         long_description = fh.read()
 except FileNotFoundError:
     long_description = ""
 
 setuptools.setup(
     name="hightouch",
-    version="1.9.0",
+    version="1.9.1",
     author="Speakeasy",
     description="Python SDK for Hightouch API",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages(where="src"),
     install_requires=[
         "certifi==2022.12.07",
```

### Comparing `hightouch-1.9.0/src/hightouch/models/operations/__init__.py` & `hightouch-1.9.1/src/hightouch/models/operations/__init__.py`

 * *Files identical despite different names*

### Comparing `hightouch-1.9.0/src/hightouch/models/operations/createdestination.py` & `hightouch-1.9.1/src/hightouch/models/operations/createdestination.py`

 * *Files identical despite different names*

### Comparing `hightouch-1.9.0/src/hightouch/models/operations/createmodel.py` & `hightouch-1.9.1/src/hightouch/models/operations/createmodel.py`

 * *Files identical despite different names*

### Comparing `hightouch-1.9.0/src/hightouch/models/operations/createsource.py` & `hightouch-1.9.1/src/hightouch/models/operations/createsource.py`

 * *Files identical despite different names*

### Comparing `hightouch-1.9.0/src/hightouch/models/operations/createsync.py` & `hightouch-1.9.1/src/hightouch/models/operations/createsync.py`

 * *Files identical despite different names*

### Comparing `hightouch-1.9.0/src/hightouch/models/operations/getdestination.py` & `hightouch-1.9.1/src/hightouch/models/operations/getdestination.py`

 * *Files identical despite different names*

### Comparing `hightouch-1.9.0/src/hightouch/models/operations/getmodel.py` & `hightouch-1.9.1/src/hightouch/models/operations/getmodel.py`

 * *Files identical despite different names*

### Comparing `hightouch-1.9.0/src/hightouch/models/operations/getsource.py` & `hightouch-1.9.1/src/hightouch/models/operations/getsource.py`

 * *Files identical despite different names*

### Comparing `hightouch-1.9.0/src/hightouch/models/operations/getsync.py` & `hightouch-1.9.1/src/hightouch/models/operations/getsync.py`

 * *Files identical despite different names*

### Comparing `hightouch-1.9.0/src/hightouch/models/operations/listdestination.py` & `hightouch-1.9.1/src/hightouch/models/operations/listdestination.py`

 * *Files identical despite different names*

### Comparing `hightouch-1.9.0/src/hightouch/models/operations/listmodel.py` & `hightouch-1.9.1/src/hightouch/models/operations/listmodel.py`

 * *Files identical despite different names*

### Comparing `hightouch-1.9.0/src/hightouch/models/operations/listsource.py` & `hightouch-1.9.1/src/hightouch/models/operations/listsource.py`

 * *Files identical despite different names*

### Comparing `hightouch-1.9.0/src/hightouch/models/operations/listsync.py` & `hightouch-1.9.1/src/hightouch/models/operations/listsync.py`

 * *Files identical despite different names*

### Comparing `hightouch-1.9.0/src/hightouch/models/operations/listsyncruns.py` & `hightouch-1.9.1/src/hightouch/models/operations/listsyncruns.py`

 * *Files identical despite different names*

### Comparing `hightouch-1.9.0/src/hightouch/models/operations/triggerrun.py` & `hightouch-1.9.1/src/hightouch/models/operations/triggerrun.py`

 * *Files identical despite different names*

### Comparing `hightouch-1.9.0/src/hightouch/models/operations/triggerruncustom.py` & `hightouch-1.9.1/src/hightouch/models/operations/triggerruncustom.py`

 * *Files identical despite different names*

### Comparing `hightouch-1.9.0/src/hightouch/models/operations/updatedestination.py` & `hightouch-1.9.1/src/hightouch/models/operations/updatedestination.py`

 * *Files identical despite different names*

### Comparing `hightouch-1.9.0/src/hightouch/models/operations/updatemodel.py` & `hightouch-1.9.1/src/hightouch/models/operations/updatemodel.py`

 * *Files identical despite different names*

### Comparing `hightouch-1.9.0/src/hightouch/models/operations/updatesource.py` & `hightouch-1.9.1/src/hightouch/models/operations/updatesource.py`

 * *Files identical despite different names*

### Comparing `hightouch-1.9.0/src/hightouch/models/operations/updatesync.py` & `hightouch-1.9.1/src/hightouch/models/operations/updatesync.py`

 * *Files identical despite different names*

### Comparing `hightouch-1.9.0/src/hightouch/models/shared/__init__.py` & `hightouch-1.9.1/src/hightouch/models/shared/__init__.py`

 * *Files identical despite different names*

### Comparing `hightouch-1.9.0/src/hightouch/models/shared/dbtschedule.py` & `hightouch-1.9.1/src/hightouch/models/shared/dbtschedule.py`

 * *Files identical despite different names*

### Comparing `hightouch-1.9.0/src/hightouch/models/shared/destination.py` & `hightouch-1.9.1/src/hightouch/models/shared/destination.py`

 * *Files identical despite different names*

### Comparing `hightouch-1.9.0/src/hightouch/models/shared/destinationcreate.py` & `hightouch-1.9.1/src/hightouch/models/shared/destinationcreate.py`

 * *Files identical despite different names*

### Comparing `hightouch-1.9.0/src/hightouch/models/shared/destinationupdate.py` & `hightouch-1.9.1/src/hightouch/models/shared/destinationupdate.py`

 * *Files identical despite different names*

### Comparing `hightouch-1.9.0/src/hightouch/models/shared/interval.py` & `hightouch-1.9.1/src/hightouch/models/shared/interval.py`

 * *Files identical despite different names*

### Comparing `hightouch-1.9.0/src/hightouch/models/shared/model.py` & `hightouch-1.9.1/src/hightouch/models/shared/model.py`

 * *Files identical despite different names*

### Comparing `hightouch-1.9.0/src/hightouch/models/shared/modelcreate.py` & `hightouch-1.9.1/src/hightouch/models/shared/modelcreate.py`

 * *Files identical despite different names*

### Comparing `hightouch-1.9.0/src/hightouch/models/shared/modelupdate.py` & `hightouch-1.9.1/src/hightouch/models/shared/modelupdate.py`

 * *Files identical despite different names*

### Comparing `hightouch-1.9.0/src/hightouch/models/shared/record_day_boolean_or_undefined_.py` & `hightouch-1.9.1/src/hightouch/models/shared/record_day_boolean_or_undefined_.py`

 * *Files identical despite different names*

### Comparing `hightouch-1.9.0/src/hightouch/models/shared/source.py` & `hightouch-1.9.1/src/hightouch/models/shared/source.py`

 * *Files identical despite different names*

### Comparing `hightouch-1.9.0/src/hightouch/models/shared/sourcecreate.py` & `hightouch-1.9.1/src/hightouch/models/shared/sourcecreate.py`

 * *Files identical despite different names*

### Comparing `hightouch-1.9.0/src/hightouch/models/shared/sourceupdate.py` & `hightouch-1.9.1/src/hightouch/models/shared/sourceupdate.py`

 * *Files identical despite different names*

### Comparing `hightouch-1.9.0/src/hightouch/models/shared/sync.py` & `hightouch-1.9.1/src/hightouch/models/shared/sync.py`

 * *Files identical despite different names*

### Comparing `hightouch-1.9.0/src/hightouch/models/shared/synccreate.py` & `hightouch-1.9.1/src/hightouch/models/shared/synccreate.py`

 * *Files identical despite different names*

### Comparing `hightouch-1.9.0/src/hightouch/models/shared/syncrun.py` & `hightouch-1.9.1/src/hightouch/models/shared/syncrun.py`

 * *Files identical despite different names*

### Comparing `hightouch-1.9.0/src/hightouch/models/shared/syncupdate.py` & `hightouch-1.9.1/src/hightouch/models/shared/syncupdate.py`

 * *Files identical despite different names*

### Comparing `hightouch-1.9.0/src/hightouch/models/shared/triggerruncustominput.py` & `hightouch-1.9.1/src/hightouch/models/shared/triggerruncustominput.py`

 * *Files identical despite different names*

### Comparing `hightouch-1.9.0/src/hightouch/models/shared/triggerruninput.py` & `hightouch-1.9.1/src/hightouch/models/shared/triggerruninput.py`

 * *Files identical despite different names*

### Comparing `hightouch-1.9.0/src/hightouch/models/shared/validateerrorjson.py` & `hightouch-1.9.1/src/hightouch/models/shared/validateerrorjson.py`

 * *Files identical despite different names*

### Comparing `hightouch-1.9.0/src/hightouch/models/shared/visualcronschedule.py` & `hightouch-1.9.1/src/hightouch/models/shared/visualcronschedule.py`

 * *Files identical despite different names*

### Comparing `hightouch-1.9.0/src/hightouch/sdk.py` & `hightouch-1.9.1/src/hightouch/sdk.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,16 +12,16 @@
     r"""SDK Documentation: Hightouch Public Rest API to access syncs, models, sources and destinations"""
     
     _client: requests_http.Session
     _security_client: requests_http.Session
     
     _server_url: str = SERVERS[0]
     _language: str = "python"
-    _sdk_version: str = "1.9.0"
-    _gen_version: str = "1.8.5"
+    _sdk_version: str = "1.9.1"
+    _gen_version: str = "1.8.6"
 
     def __init__(self) -> None:
         self._client = requests_http.Session()
         self._security_client = requests_http.Session()
         
 
     def config_server_url(self, server_url: str, params: dict[str, str] = None):
```

### Comparing `hightouch-1.9.0/src/hightouch/utils/retries.py` & `hightouch-1.9.1/src/hightouch/utils/retries.py`

 * *Files identical despite different names*

### Comparing `hightouch-1.9.0/src/hightouch/utils/utils.py` & `hightouch-1.9.1/src/hightouch/utils/utils.py`

 * *Files identical despite different names*

### Comparing `hightouch-1.9.0/src/hightouch.egg-info/PKG-INFO` & `hightouch-1.9.1/src/hightouch.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hightouch
-Version: 1.9.0
+Version: 1.9.1
 Summary: Python SDK for Hightouch API
 Home-page: UNKNOWN
 Author: Speakeasy
 License: UNKNOWN
 Platform: UNKNOWN
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: hightouch Version: 1.9.0 Summary: Python SDK for
+Metadata-Version: 2.1 Name: hightouch Version: 1.9.1 Summary: Python SDK for
 Hightouch API Home-page: UNKNOWN Author: Speakeasy License: UNKNOWN Platform:
 UNKNOWN Requires-Python: >=3.9 Description-Content-Type: text/markdown
    [https://user-images.githubusercontent.com/6267663/221538828-de1343f2-b249-
                          4ba2-85e3-a2e43cc5f265.svg]
                            ****** Python SDK ******
    Hightouch exposes a REST API that lets users interact with resources like
                    syncs, models, sources and destinations.
```

### Comparing `hightouch-1.9.0/src/hightouch.egg-info/SOURCES.txt` & `hightouch-1.9.1/src/hightouch.egg-info/SOURCES.txt`

 * *Files identical despite different names*

