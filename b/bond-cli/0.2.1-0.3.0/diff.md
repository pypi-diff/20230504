# Comparing `tmp/bond-cli-0.2.1.tar.gz` & `tmp/bond-cli-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bond-cli-0.2.1.tar", last modified: Tue Apr 12 16:38:31 2022, max compression
+gzip compressed data, was "bond-cli-0.3.0.tar", last modified: Thu May  4 14:12:41 2023, max compression
```

## Comparing `bond-cli-0.2.1.tar` & `bond-cli-0.3.0.tar`

### file list

```diff
@@ -1,62 +1,62 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-12 16:38:31.658081 bond-cli-0.2.1/
--rw-r--r--   0 runner    (1001) docker     (121)     3480 2022-04-12 16:38:31.658081 bond-cli-0.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     3275 2022-04-12 16:38:22.000000 bond-cli-0.2.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-12 16:38:31.654082 bond-cli-0.2.1/bond/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-04-12 16:38:22.000000 bond-cli-0.2.1/bond/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      164 2022-04-12 16:38:22.000000 bond-cli-0.2.1/bond/__main__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1239 2022-04-12 16:38:22.000000 bond-cli-0.2.1/bond/app.py
--rwxr-xr-x   0 runner    (1001) docker     (121)      140 2022-04-12 16:38:22.000000 bond-cli-0.2.1/bond/bond
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-12 16:38:31.654082 bond-cli-0.2.1/bond/cli/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-04-12 16:38:22.000000 bond-cli-0.2.1/bond/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      631 2022-04-12 16:38:22.000000 bond-cli-0.2.1/bond/cli/console.py
--rw-r--r--   0 runner    (1001) docker     (121)     1267 2022-04-12 16:38:22.000000 bond-cli-0.2.1/bond/cli/main.py
--rw-r--r--   0 runner    (1001) docker     (121)     1320 2022-04-12 16:38:22.000000 bond-cli-0.2.1/bond/cli/table.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-12 16:38:31.658081 bond-cli-0.2.1/bond/commands/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-04-12 16:38:22.000000 bond-cli-0.2.1/bond/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     6057 2022-04-12 16:38:22.000000 bond-cli-0.2.1/bond/commands/backup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-12 16:38:31.658081 bond-cli-0.2.1/bond/commands/devices/
--rw-r--r--   0 runner    (1001) docker     (121)      303 2022-04-12 16:38:22.000000 bond-cli-0.2.1/bond/commands/devices/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1825 2022-04-12 16:38:22.000000 bond-cli-0.2.1/bond/commands/devices/create.py
--rw-r--r--   0 runner    (1001) docker     (121)     1648 2022-04-12 16:38:22.000000 bond-cli-0.2.1/bond/commands/devices/delete.py
--rw-r--r--   0 runner    (1001) docker     (121)     1131 2022-04-12 16:38:22.000000 bond-cli-0.2.1/bond/commands/devices/list.py
--rw-r--r--   0 runner    (1001) docker     (121)      531 2022-04-12 16:38:22.000000 bond-cli-0.2.1/bond/commands/discover.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-12 16:38:31.658081 bond-cli-0.2.1/bond/commands/groups/
--rw-r--r--   0 runner    (1001) docker     (121)      283 2022-04-12 16:38:22.000000 bond-cli-0.2.1/bond/commands/groups/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1325 2022-04-12 16:38:22.000000 bond-cli-0.2.1/bond/commands/groups/create.py
--rw-r--r--   0 runner    (1001) docker     (121)     3149 2022-04-12 16:38:22.000000 bond-cli-0.2.1/bond/commands/groups/delete.py
--rw-r--r--   0 runner    (1001) docker     (121)     2155 2022-04-12 16:38:22.000000 bond-cli-0.2.1/bond/commands/groups/list.py
--rw-r--r--   0 runner    (1001) docker     (121)     1190 2022-04-12 16:38:22.000000 bond-cli-0.2.1/bond/commands/list.py
--rw-r--r--   0 runner    (1001) docker     (121)     4055 2022-04-12 16:38:22.000000 bond-cli-0.2.1/bond/commands/livelog.py
--rw-r--r--   0 runner    (1001) docker     (121)      733 2022-04-12 16:38:22.000000 bond-cli-0.2.1/bond/commands/reboot.py
--rw-r--r--   0 runner    (1001) docker     (121)     1318 2022-04-12 16:38:22.000000 bond-cli-0.2.1/bond/commands/reset.py
--rw-r--r--   0 runner    (1001) docker     (121)     1152 2022-04-12 16:38:22.000000 bond-cli-0.2.1/bond/commands/rfman.py
--rw-r--r--   0 runner    (1001) docker     (121)     2515 2022-04-12 16:38:22.000000 bond-cli-0.2.1/bond/commands/select.py
--rw-r--r--   0 runner    (1001) docker     (121)     1497 2022-04-12 16:38:22.000000 bond-cli-0.2.1/bond/commands/signal.py
--rw-r--r--   0 runner    (1001) docker     (121)     1787 2022-04-12 16:38:22.000000 bond-cli-0.2.1/bond/commands/token.py
--rw-r--r--   0 runner    (1001) docker     (121)     5134 2022-04-12 16:38:22.000000 bond-cli-0.2.1/bond/commands/upgrade.py
--rw-r--r--   0 runner    (1001) docker     (121)      571 2022-04-12 16:38:22.000000 bond-cli-0.2.1/bond/commands/version.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-12 16:38:31.658081 bond-cli-0.2.1/bond/commands/wifi/
--rw-r--r--   0 runner    (1001) docker     (121)      241 2022-04-12 16:38:22.000000 bond-cli-0.2.1/bond/commands/wifi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      931 2022-04-12 16:38:22.000000 bond-cli-0.2.1/bond/commands/wifi/connect.py
--rw-r--r--   0 runner    (1001) docker     (121)      598 2022-04-12 16:38:22.000000 bond-cli-0.2.1/bond/commands/wifi/shutdown.py
--rw-r--r--   0 runner    (1001) docker     (121)     1467 2022-04-12 16:38:22.000000 bond-cli-0.2.1/bond/commands/wifi.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-12 16:38:31.658081 bond-cli-0.2.1/bond/database/
--rw-r--r--   0 runner    (1001) docker     (121)       74 2022-04-12 16:38:22.000000 bond-cli-0.2.1/bond/database/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2461 2022-04-12 16:38:22.000000 bond-cli-0.2.1/bond/database/database.py
--rw-r--r--   0 runner    (1001) docker     (121)      180 2022-04-12 16:38:22.000000 bond-cli-0.2.1/bond/database/test_database.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-12 16:38:31.658081 bond-cli-0.2.1/bond/endpoints/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-04-12 16:38:22.000000 bond-cli-0.2.1/bond/endpoints/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-12 16:38:31.658081 bond-cli-0.2.1/bond/proto/
--rw-r--r--   0 runner    (1001) docker     (121)      101 2022-04-12 16:38:22.000000 bond-cli-0.2.1/bond/proto/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      522 2022-04-12 16:38:22.000000 bond-cli-0.2.1/bond/proto/base_transport.py
--rw-r--r--   0 runner    (1001) docker     (121)     1687 2022-04-12 16:38:22.000000 bond-cli-0.2.1/bond/proto/http.py
--rw-r--r--   0 runner    (1001) docker     (121)     1102 2022-04-12 16:38:22.000000 bond-cli-0.2.1/bond/proto/mdns.py
--rw-r--r--   0 runner    (1001) docker     (121)     1693 2022-04-12 16:38:22.000000 bond-cli-0.2.1/bond/proto/wye.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-12 16:38:31.658081 bond-cli-0.2.1/bond_cli.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     3480 2022-04-12 16:38:31.000000 bond-cli-0.2.1/bond_cli.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1217 2022-04-12 16:38:31.000000 bond-cli-0.2.1/bond_cli.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-04-12 16:38:31.000000 bond-cli-0.2.1/bond_cli.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       18 2022-04-12 16:38:31.000000 bond-cli-0.2.1/bond_cli.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        5 2022-04-12 16:38:31.000000 bond-cli-0.2.1/bond_cli.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      179 2022-04-12 16:38:31.662079 bond-cli-0.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      573 2022-04-12 16:38:22.000000 bond-cli-0.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 14:12:41.540896 bond-cli-0.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     3424 2023-05-04 14:12:41.540896 bond-cli-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3275 2023-05-04 14:12:29.000000 bond-cli-0.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 14:12:41.536896 bond-cli-0.3.0/bond/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 14:12:29.000000 bond-cli-0.3.0/bond/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-05-04 14:12:29.000000 bond-cli-0.3.0/bond/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1239 2023-05-04 14:12:29.000000 bond-cli-0.3.0/bond/app.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      140 2023-05-04 14:12:29.000000 bond-cli-0.3.0/bond/bond
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 14:12:41.536896 bond-cli-0.3.0/bond/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 14:12:29.000000 bond-cli-0.3.0/bond/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      631 2023-05-04 14:12:29.000000 bond-cli-0.3.0/bond/cli/console.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1267 2023-05-04 14:12:29.000000 bond-cli-0.3.0/bond/cli/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1320 2023-05-04 14:12:29.000000 bond-cli-0.3.0/bond/cli/table.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 14:12:41.536896 bond-cli-0.3.0/bond/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 14:12:29.000000 bond-cli-0.3.0/bond/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6057 2023-05-04 14:12:29.000000 bond-cli-0.3.0/bond/commands/backup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 14:12:41.536896 bond-cli-0.3.0/bond/commands/devices/
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-05-04 14:12:29.000000 bond-cli-0.3.0/bond/commands/devices/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1825 2023-05-04 14:12:29.000000 bond-cli-0.3.0/bond/commands/devices/create.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1648 2023-05-04 14:12:29.000000 bond-cli-0.3.0/bond/commands/devices/delete.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1131 2023-05-04 14:12:29.000000 bond-cli-0.3.0/bond/commands/devices/list.py
+-rw-r--r--   0 runner    (1001) docker     (123)      531 2023-05-04 14:12:29.000000 bond-cli-0.3.0/bond/commands/discover.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 14:12:41.536896 bond-cli-0.3.0/bond/commands/groups/
+-rw-r--r--   0 runner    (1001) docker     (123)      283 2023-05-04 14:12:29.000000 bond-cli-0.3.0/bond/commands/groups/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1325 2023-05-04 14:12:29.000000 bond-cli-0.3.0/bond/commands/groups/create.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3149 2023-05-04 14:12:29.000000 bond-cli-0.3.0/bond/commands/groups/delete.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2155 2023-05-04 14:12:29.000000 bond-cli-0.3.0/bond/commands/groups/list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1190 2023-05-04 14:12:29.000000 bond-cli-0.3.0/bond/commands/list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4055 2023-05-04 14:12:29.000000 bond-cli-0.3.0/bond/commands/livelog.py
+-rw-r--r--   0 runner    (1001) docker     (123)      733 2023-05-04 14:12:29.000000 bond-cli-0.3.0/bond/commands/reboot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1318 2023-05-04 14:12:29.000000 bond-cli-0.3.0/bond/commands/reset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1152 2023-05-04 14:12:29.000000 bond-cli-0.3.0/bond/commands/rfman.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2645 2023-05-04 14:12:29.000000 bond-cli-0.3.0/bond/commands/select.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1497 2023-05-04 14:12:29.000000 bond-cli-0.3.0/bond/commands/signal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2083 2023-05-04 14:12:29.000000 bond-cli-0.3.0/bond/commands/token.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5134 2023-05-04 14:12:29.000000 bond-cli-0.3.0/bond/commands/upgrade.py
+-rw-r--r--   0 runner    (1001) docker     (123)      571 2023-05-04 14:12:29.000000 bond-cli-0.3.0/bond/commands/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 14:12:41.536896 bond-cli-0.3.0/bond/commands/wifi/
+-rw-r--r--   0 runner    (1001) docker     (123)      241 2023-05-04 14:12:29.000000 bond-cli-0.3.0/bond/commands/wifi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      931 2023-05-04 14:12:29.000000 bond-cli-0.3.0/bond/commands/wifi/connect.py
+-rw-r--r--   0 runner    (1001) docker     (123)      598 2023-05-04 14:12:29.000000 bond-cli-0.3.0/bond/commands/wifi/shutdown.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1467 2023-05-04 14:12:29.000000 bond-cli-0.3.0/bond/commands/wifi.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 14:12:41.536896 bond-cli-0.3.0/bond/database/
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-05-04 14:12:29.000000 bond-cli-0.3.0/bond/database/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2461 2023-05-04 14:12:29.000000 bond-cli-0.3.0/bond/database/database.py
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-05-04 14:12:29.000000 bond-cli-0.3.0/bond/database/test_database.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 14:12:41.536896 bond-cli-0.3.0/bond/endpoints/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 14:12:29.000000 bond-cli-0.3.0/bond/endpoints/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 14:12:41.536896 bond-cli-0.3.0/bond/proto/
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-05-04 14:12:29.000000 bond-cli-0.3.0/bond/proto/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      522 2023-05-04 14:12:29.000000 bond-cli-0.3.0/bond/proto/base_transport.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1687 2023-05-04 14:12:29.000000 bond-cli-0.3.0/bond/proto/http.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-05-04 14:12:29.000000 bond-cli-0.3.0/bond/proto/mdns.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1693 2023-05-04 14:12:29.000000 bond-cli-0.3.0/bond/proto/wye.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 14:12:41.540896 bond-cli-0.3.0/bond_cli.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3424 2023-05-04 14:12:41.000000 bond-cli-0.3.0/bond_cli.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1217 2023-05-04 14:12:41.000000 bond-cli-0.3.0/bond_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 14:12:41.000000 bond-cli-0.3.0/bond_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-04 14:12:41.000000 bond-cli-0.3.0/bond_cli.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-04 14:12:41.000000 bond-cli-0.3.0/bond_cli.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      179 2023-05-04 14:12:41.540896 bond-cli-0.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      627 2023-05-04 14:12:29.000000 bond-cli-0.3.0/setup.py
```

### Comparing `bond-cli-0.2.1/PKG-INFO` & `bond-cli-0.3.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,13 @@
 Metadata-Version: 2.1
 Name: bond-cli
-Version: 0.2.1
+Version: 0.3.0
 Summary: Bond CLI
-Home-page: UNKNOWN
 Author: Olibra
-License: UNKNOWN
-Platform: UNKNOWN
-Requires-Python: >=3.6
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 
 [![PyPI version](https://badge.fury.io/py/bond-cli.svg)](https://badge.fury.io/py/bond-cli)
 
 # Bond Command Line Interface
 
 EDIT: This project is in a beta state. We released it on the principle of release early & often. It is here just in case it benefits a member of the Bond Home community. Your mileage may vary!
@@ -164,9 +161,7 @@
 git tag -a "v1.8.7"
 ```
 
 with a version matching that in `setup.py`. You'll be prompted to write some release notes.
 Alternatively, use the Github repository's releases interface to create a release.
 
 Upon pushing the tag or publishing the release, CI will deploy to PyPi.
-
-
```

### Comparing `bond-cli-0.2.1/README.md` & `bond-cli-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `bond-cli-0.2.1/bond/app.py` & `bond-cli-0.3.0/bond/app.py`

 * *Files identical despite different names*

### Comparing `bond-cli-0.2.1/bond/cli/console.py` & `bond-cli-0.3.0/bond/cli/console.py`

 * *Files identical despite different names*

### Comparing `bond-cli-0.2.1/bond/cli/main.py` & `bond-cli-0.3.0/bond/cli/main.py`

 * *Files identical despite different names*

### Comparing `bond-cli-0.2.1/bond/cli/table.py` & `bond-cli-0.3.0/bond/cli/table.py`

 * *Files identical despite different names*

### Comparing `bond-cli-0.2.1/bond/commands/backup.py` & `bond-cli-0.3.0/bond/commands/backup.py`

 * *Files identical despite different names*

### Comparing `bond-cli-0.2.1/bond/commands/devices/create.py` & `bond-cli-0.3.0/bond/commands/devices/create.py`

 * *Files identical despite different names*

### Comparing `bond-cli-0.2.1/bond/commands/devices/delete.py` & `bond-cli-0.3.0/bond/commands/devices/delete.py`

 * *Files identical despite different names*

### Comparing `bond-cli-0.2.1/bond/commands/devices/list.py` & `bond-cli-0.3.0/bond/commands/devices/list.py`

 * *Files identical despite different names*

### Comparing `bond-cli-0.2.1/bond/commands/discover.py` & `bond-cli-0.3.0/bond/commands/discover.py`

 * *Files identical despite different names*

### Comparing `bond-cli-0.2.1/bond/commands/groups/create.py` & `bond-cli-0.3.0/bond/commands/groups/create.py`

 * *Files identical despite different names*

### Comparing `bond-cli-0.2.1/bond/commands/groups/delete.py` & `bond-cli-0.3.0/bond/commands/groups/delete.py`

 * *Files identical despite different names*

### Comparing `bond-cli-0.2.1/bond/commands/groups/list.py` & `bond-cli-0.3.0/bond/commands/groups/list.py`

 * *Files identical despite different names*

### Comparing `bond-cli-0.2.1/bond/commands/list.py` & `bond-cli-0.3.0/bond/commands/list.py`

 * *Files identical despite different names*

### Comparing `bond-cli-0.2.1/bond/commands/livelog.py` & `bond-cli-0.3.0/bond/commands/livelog.py`

 * *Files identical despite different names*

### Comparing `bond-cli-0.2.1/bond/commands/reboot.py` & `bond-cli-0.3.0/bond/commands/reboot.py`

 * *Files identical despite different names*

### Comparing `bond-cli-0.2.1/bond/commands/reset.py` & `bond-cli-0.3.0/bond/commands/reset.py`

 * *Files identical despite different names*

### Comparing `bond-cli-0.2.1/bond/commands/rfman.py` & `bond-cli-0.3.0/bond/commands/rfman.py`

 * *Files identical despite different names*

### Comparing `bond-cli-0.2.1/bond/commands/select.py` & `bond-cli-0.3.0/bond/commands/select.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from bond.commands.token import check_unlocked_token
+from bond.commands.token import check_unlocked_token, unlock_token
 from bond.database import BondDatabase
 
 
 class SelectCommand(object):
     subcmd = "select"
     help = """Select a single Bond to interact with,
               If the token of this Bond is unlocked, it will be set.
@@ -10,37 +10,32 @@
     arguments = {
         "bond_id": {
             "nargs": "?",
             "help": """Bond ID to interact with in subsequent commands
                        (you can also use a prefix, if it uniquely identifies an
                        already-discovered Bond""",
         },
+        "--pin": {"help": "specify Bond PIN to automatically unlock token"},
         "--clear": {"action": "store_true", "help": "clear selection"},
         "--ip": {"help": "specify Bond IP address"},
         "--port": {"help": "specify Bond HTTP port"},
     }
 
     def run(self, args):
         if args.bond_id:
-            matches = [
-                bond
-                for bond in BondDatabase.get_bonds()
-                if bond.lower().startswith(args.bond_id.lower())
-            ]
+            matches = [bond for bond in BondDatabase.get_bonds() if bond.lower().startswith(args.bond_id.lower())]
             if len(matches) == 0:
                 proceed = input(
                     f"{args.bond_id} hasn't been discovered by bond-cli ('bond discover').\n"
                     "Proceed with setting it? It may not be reachable. [y/N] "
                 )
                 if proceed.lower() == "y":
                     bond_id = args.bond_id
                 else:
-                    raise SystemExit(
-                        "Aborting. Try 'bond discover' on the same network as your Bond"
-                    )
+                    raise SystemExit("Aborting. Try 'bond discover' on the same network as your Bond")
             if len(matches) == 1:
                 bond_id = matches[0]
             if len(matches) > 1:
                 print("Ambiguous Bond ID prefix. Potential matches:")
                 for match in matches:
                     print(match)
                 exit(1)
@@ -48,13 +43,17 @@
             if args.ip:
                 BondDatabase.set_bond(bond_id, "ip", args.ip)
                 print(f"Set {bond_id} IP {args.ip}")
             if args.port:
                 BondDatabase.set_bond(bond_id, "port", args.port)
                 print(f"Set {bond_id} port {args.ip}")
             print(f"Selected Bond: {BondDatabase().get('selected_bondid')}")
-            token = check_unlocked_token()  # noqa: F841
+            if args.pin:
+                print("Unlocking token...")
+                token = unlock_token(bond_id, args.pin)
+            else:
+                token = check_unlocked_token()  # noqa: F841
         elif args.clear:
             BondDatabase().pop("selected_bondid", None)
             print("Cleared selected Bond")
         else:
             print(f"Bond selected: {BondDatabase().get_assert_selected_bondid()}")
```

### Comparing `bond-cli-0.2.1/bond/commands/signal.py` & `bond-cli-0.3.0/bond/commands/signal.py`

 * *Files identical despite different names*

### Comparing `bond-cli-0.2.1/bond/commands/upgrade.py` & `bond-cli-0.3.0/bond/commands/upgrade.py`

 * *Files identical despite different names*

### Comparing `bond-cli-0.2.1/bond/commands/version.py` & `bond-cli-0.3.0/bond/commands/version.py`

 * *Files identical despite different names*

### Comparing `bond-cli-0.2.1/bond/commands/wifi/connect.py` & `bond-cli-0.3.0/bond/commands/wifi/connect.py`

 * *Files identical despite different names*

### Comparing `bond-cli-0.2.1/bond/commands/wifi/shutdown.py` & `bond-cli-0.3.0/bond/commands/wifi/shutdown.py`

 * *Files identical despite different names*

### Comparing `bond-cli-0.2.1/bond/commands/wifi.py` & `bond-cli-0.3.0/bond/commands/wifi.py`

 * *Files identical despite different names*

### Comparing `bond-cli-0.2.1/bond/database/database.py` & `bond-cli-0.3.0/bond/database/database.py`

 * *Files identical despite different names*

### Comparing `bond-cli-0.2.1/bond/proto/base_transport.py` & `bond-cli-0.3.0/bond/proto/base_transport.py`

 * *Files identical despite different names*

### Comparing `bond-cli-0.2.1/bond/proto/http.py` & `bond-cli-0.3.0/bond/proto/http.py`

 * *Files identical despite different names*

### Comparing `bond-cli-0.2.1/bond/proto/mdns.py` & `bond-cli-0.3.0/bond/proto/mdns.py`

 * *Files identical despite different names*

### Comparing `bond-cli-0.2.1/bond/proto/wye.py` & `bond-cli-0.3.0/bond/proto/wye.py`

 * *Files identical despite different names*

### Comparing `bond-cli-0.2.1/bond_cli.egg-info/PKG-INFO` & `bond-cli-0.3.0/bond_cli.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,13 @@
 Metadata-Version: 2.1
 Name: bond-cli
-Version: 0.2.1
+Version: 0.3.0
 Summary: Bond CLI
-Home-page: UNKNOWN
 Author: Olibra
-License: UNKNOWN
-Platform: UNKNOWN
-Requires-Python: >=3.6
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 
 [![PyPI version](https://badge.fury.io/py/bond-cli.svg)](https://badge.fury.io/py/bond-cli)
 
 # Bond Command Line Interface
 
 EDIT: This project is in a beta state. We released it on the principle of release early & often. It is here just in case it benefits a member of the Bond Home community. Your mileage may vary!
@@ -164,9 +161,7 @@
 git tag -a "v1.8.7"
 ```
 
 with a version matching that in `setup.py`. You'll be prompted to write some release notes.
 Alternatively, use the Github repository's releases interface to create a release.
 
 Upon pushing the tag or publishing the release, CI will deploy to PyPi.
-
-
```

### Comparing `bond-cli-0.2.1/bond_cli.egg-info/SOURCES.txt` & `bond-cli-0.3.0/bond_cli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bond-cli-0.2.1/setup.py` & `bond-cli-0.3.0/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 from setuptools import find_packages, setup
 
-DEPS_ALL = open("requirements.txt").readlines()
+DEPS_ALL = open("requirements.txt", encoding="utf-8").readlines()
 
-DEPS_TEST = DEPS_ALL + open("requirements-test.txt").readlines()
+DEPS_TEST = DEPS_ALL + open("requirements-test.txt", encoding="utf-8").readlines()
 
 setup(
     name="bond-cli",
-    version="0.2.1",
+    version="0.3.0",
     author="Olibra",
     packages=find_packages(),
     scripts=["bond/bond"],
     include_package_data=True,
     description="Bond CLI",
-    long_description=open("README.md").read(),
+    long_description=open("README.md", encoding="utf-8").read(),
     long_description_content_type="text/markdown",
-    python_requires=">=3.6",
+    python_requires=">=3.7",
     setup_requires=["pytest-runner"],
     install_requires=DEPS_ALL,
     tests_require=DEPS_TEST,
 )
```

