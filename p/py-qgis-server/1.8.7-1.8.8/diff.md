# Comparing `tmp/py-qgis-server-1.8.7.tar.gz` & `tmp/py-qgis-server-1.8.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py-qgis-server-1.8.7.tar", last modified: Fri Feb 10 15:18:39 2023, max compression
+gzip compressed data, was "py-qgis-server-1.8.8.tar", last modified: Thu May  4 15:32:26 2023, max compression
```

## Comparing `py-qgis-server-1.8.7.tar` & `py-qgis-server-1.8.8.tar`

### file list

```diff
@@ -1,83 +1,83 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-10 15:18:39.978964 py-qgis-server-1.8.7/
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-02-10 15:18:25.000000 py-qgis-server-1.8.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     6971 2023-02-10 15:18:39.978964 py-qgis-server-1.8.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5990 2023-02-10 15:18:25.000000 py-qgis-server-1.8.7/README.md
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-02-10 15:18:26.000000 py-qgis-server-1.8.7/VERSION
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-10 15:18:39.974964 py-qgis-server-1.8.7/py_qgis_server.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6971 2023-02-10 15:18:39.000000 py-qgis-server-1.8.7/py_qgis_server.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2115 2023-02-10 15:18:39.000000 py-qgis-server-1.8.7/py_qgis_server.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-10 15:18:39.000000 py-qgis-server-1.8.7/py_qgis_server.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      327 2023-02-10 15:18:39.000000 py-qgis-server-1.8.7/py_qgis_server.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-02-10 15:18:39.000000 py-qgis-server-1.8.7/py_qgis_server.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-02-10 15:18:39.000000 py-qgis-server-1.8.7/py_qgis_server.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-10 15:18:39.974964 py-qgis-server-1.8.7/pyqgisserver/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-10 15:18:25.000000 py-qgis-server-1.8.7/pyqgisserver/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-02-10 15:18:29.000000 py-qgis-server-1.8.7/pyqgisserver/build.manifest
--rw-r--r--   0 runner    (1001) docker     (123)    12410 2023-02-10 15:18:25.000000 py-qgis-server-1.8.7/pyqgisserver/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-10 15:18:39.974964 py-qgis-server-1.8.7/pyqgisserver/handlers/
--rw-r--r--   0 runner    (1001) docker     (123)      352 2023-02-10 15:18:25.000000 py-qgis-server-1.8.7/pyqgisserver/handlers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6237 2023-02-10 15:18:25.000000 py-qgis-server-1.8.7/pyqgisserver/handlers/asynchandler.py
--rw-r--r--   0 runner    (1001) docker     (123)     5660 2023-02-10 15:18:25.000000 py-qgis-server-1.8.7/pyqgisserver/handlers/basehandler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2178 2023-02-10 15:18:25.000000 py-qgis-server-1.8.7/pyqgisserver/handlers/landingpage.py
--rw-r--r--   0 runner    (1001) docker     (123)     1693 2023-02-10 15:18:25.000000 py-qgis-server-1.8.7/pyqgisserver/handlers/oapihandler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2417 2023-02-10 15:18:25.000000 py-qgis-server-1.8.7/pyqgisserver/handlers/owshandler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2483 2023-02-10 15:18:25.000000 py-qgis-server-1.8.7/pyqgisserver/handlers/statushandler.py
--rw-r--r--   0 runner    (1001) docker     (123)     3581 2023-02-10 15:18:25.000000 py-qgis-server-1.8.7/pyqgisserver/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-10 15:18:39.974964 py-qgis-server-1.8.7/pyqgisserver/management/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-10 15:18:25.000000 py-qgis-server-1.8.7/pyqgisserver/management/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-10 15:18:39.978964 py-qgis-server-1.8.7/pyqgisserver/management/apis/
--rw-r--r--   0 runner    (1001) docker     (123)      467 2023-02-10 15:18:25.000000 py-qgis-server-1.8.7/pyqgisserver/management/apis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1384 2023-02-10 15:18:25.000000 py-qgis-server-1.8.7/pyqgisserver/management/apis/cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     6887 2023-02-10 15:18:25.000000 py-qgis-server-1.8.7/pyqgisserver/management/apis/handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2025 2023-02-10 15:18:25.000000 py-qgis-server-1.8.7/pyqgisserver/management/apis/plugins.py
--rw-r--r--   0 runner    (1001) docker     (123)     6103 2023-02-10 15:18:25.000000 py-qgis-server-1.8.7/pyqgisserver/management/server.py
--rw-r--r--   0 runner    (1001) docker     (123)     2718 2023-02-10 15:18:25.000000 py-qgis-server-1.8.7/pyqgisserver/middleware.py
--rw-r--r--   0 runner    (1001) docker     (123)      824 2023-02-10 15:18:25.000000 py-qgis-server-1.8.7/pyqgisserver/monitor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-10 15:18:39.978964 py-qgis-server-1.8.7/pyqgisserver/monitors/
--rw-r--r--   0 runner    (1001) docker     (123)     4318 2023-02-10 15:18:25.000000 py-qgis-server-1.8.7/pyqgisserver/monitors/amqp.py
--rw-r--r--   0 runner    (1001) docker     (123)      702 2023-02-10 15:18:25.000000 py-qgis-server-1.8.7/pyqgisserver/monitors/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      884 2023-02-10 15:18:25.000000 py-qgis-server-1.8.7/pyqgisserver/monitors/test.py
--rw-r--r--   0 runner    (1001) docker     (123)     4723 2023-02-10 15:18:25.000000 py-qgis-server-1.8.7/pyqgisserver/plugins.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-10 15:18:39.978964 py-qgis-server-1.8.7/pyqgisserver/qgscache/
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-02-10 15:18:25.000000 py-qgis-server-1.8.7/pyqgisserver/qgscache/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19195 2023-02-10 15:18:25.000000 py-qgis-server-1.8.7/pyqgisserver/qgscache/cachemanager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-10 15:18:39.978964 py-qgis-server-1.8.7/pyqgisserver/qgscache/handlers/
--rw-r--r--   0 runner    (1001) docker     (123)      365 2023-02-10 15:18:25.000000 py-qgis-server-1.8.7/pyqgisserver/qgscache/handlers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2529 2023-02-10 15:18:25.000000 py-qgis-server-1.8.7/pyqgisserver/qgscache/handlers/file_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     5557 2023-02-10 15:18:25.000000 py-qgis-server-1.8.7/pyqgisserver/qgscache/handlers/postgres_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     6237 2023-02-10 15:18:25.000000 py-qgis-server-1.8.7/pyqgisserver/qgscache/observer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-10 15:18:39.978964 py-qgis-server-1.8.7/pyqgisserver/qgscache/observers/
--rw-r--r--   0 runner    (1001) docker     (123)     1542 2023-02-10 15:18:25.000000 py-qgis-server-1.8.7/pyqgisserver/qgscache/observers/ban.py
--rw-r--r--   0 runner    (1001) docker     (123)      676 2023-02-10 15:18:25.000000 py-qgis-server-1.8.7/pyqgisserver/qgscache/observers/test.py
--rw-r--r--   0 runner    (1001) docker     (123)      383 2023-02-10 15:18:25.000000 py-qgis-server-1.8.7/pyqgisserver/qgscache/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     7722 2023-02-10 15:18:25.000000 py-qgis-server-1.8.7/pyqgisserver/qgspool.py
--rw-r--r--   0 runner    (1001) docker     (123)    20790 2023-02-10 15:18:25.000000 py-qgis-server-1.8.7/pyqgisserver/qgsworker.py
--rw-r--r--   0 runner    (1001) docker     (123)     9304 2023-02-10 15:18:25.000000 py-qgis-server-1.8.7/pyqgisserver/runtime.py
--rw-r--r--   0 runner    (1001) docker     (123)     3784 2023-02-10 15:18:25.000000 py-qgis-server-1.8.7/pyqgisserver/server.py
--rw-r--r--   0 runner    (1001) docker     (123)      872 2023-02-10 15:18:25.000000 py-qgis-server-1.8.7/pyqgisserver/stats.py
--rw-r--r--   0 runner    (1001) docker     (123)     4652 2023-02-10 15:18:25.000000 py-qgis-server-1.8.7/pyqgisserver/tests.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-10 15:18:39.978964 py-qgis-server-1.8.7/pyqgisserver/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-10 15:18:25.000000 py-qgis-server-1.8.7/pyqgisserver/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2550 2023-02-10 15:18:25.000000 py-qgis-server-1.8.7/pyqgisserver/utils/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)     3523 2023-02-10 15:18:25.000000 py-qgis-server-1.8.7/pyqgisserver/utils/lru.py
--rw-r--r--   0 runner    (1001) docker     (123)     5964 2023-02-10 15:18:25.000000 py-qgis-server-1.8.7/pyqgisserver/utils/qgis.py
--rw-r--r--   0 runner    (1001) docker     (123)      793 2023-02-10 15:18:25.000000 py-qgis-server-1.8.7/pyqgisserver/utils/stats.py
--rw-r--r--   0 runner    (1001) docker     (123)      862 2023-02-10 15:18:25.000000 py-qgis-server-1.8.7/pyqgisserver/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-10 15:18:39.978964 py-qgis-server-1.8.7/pyqgisserver/zeromq/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-10 15:18:25.000000 py-qgis-server-1.8.7/pyqgisserver/zeromq/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7193 2023-02-10 15:18:25.000000 py-qgis-server-1.8.7/pyqgisserver/zeromq/broker.py
--rw-r--r--   0 runner    (1001) docker     (123)     8356 2023-02-10 15:18:25.000000 py-qgis-server-1.8.7/pyqgisserver/zeromq/client.py
--rw-r--r--   0 runner    (1001) docker     (123)      537 2023-02-10 15:18:25.000000 py-qgis-server-1.8.7/pyqgisserver/zeromq/messages.py
--rw-r--r--   0 runner    (1001) docker     (123)     3970 2023-02-10 15:18:25.000000 py-qgis-server-1.8.7/pyqgisserver/zeromq/pool.py
--rw-r--r--   0 runner    (1001) docker     (123)     4627 2023-02-10 15:18:25.000000 py-qgis-server-1.8.7/pyqgisserver/zeromq/supervisor.py
--rw-r--r--   0 runner    (1001) docker     (123)      297 2023-02-10 15:18:25.000000 py-qgis-server-1.8.7/pyqgisserver/zeromq/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     8204 2023-02-10 15:18:25.000000 py-qgis-server-1.8.7/pyqgisserver/zeromq/worker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-10 15:18:39.970964 py-qgis-server-1.8.7/pyqgisservercontrib/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-10 15:18:39.978964 py-qgis-server-1.8.7/pyqgisservercontrib/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-10 15:18:25.000000 py-qgis-server-1.8.7/pyqgisservercontrib/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5194 2023-02-10 15:18:25.000000 py-qgis-server-1.8.7/pyqgisservercontrib/core/componentmanager.py
--rw-r--r--   0 runner    (1001) docker     (123)     2668 2023-02-10 15:18:25.000000 py-qgis-server-1.8.7/pyqgisservercontrib/core/filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     1549 2023-02-10 15:18:25.000000 py-qgis-server-1.8.7/pyqgisservercontrib/core/watchfiles.py
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-02-10 15:18:25.000000 py-qgis-server-1.8.7/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      186 2023-02-10 15:18:39.978964 py-qgis-server-1.8.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2572 2023-02-10 15:18:25.000000 py-qgis-server-1.8.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:32:26.362457 py-qgis-server-1.8.8/
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-05-04 15:32:01.000000 py-qgis-server-1.8.8/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     7098 2023-05-04 15:32:26.362457 py-qgis-server-1.8.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6117 2023-05-04 15:32:01.000000 py-qgis-server-1.8.8/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-04 15:32:02.000000 py-qgis-server-1.8.8/VERSION
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:32:26.358456 py-qgis-server-1.8.8/py_qgis_server.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7098 2023-05-04 15:32:26.000000 py-qgis-server-1.8.8/py_qgis_server.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2115 2023-05-04 15:32:26.000000 py-qgis-server-1.8.8/py_qgis_server.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 15:32:26.000000 py-qgis-server-1.8.8/py_qgis_server.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      327 2023-05-04 15:32:26.000000 py-qgis-server-1.8.8/py_qgis_server.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-04 15:32:26.000000 py-qgis-server-1.8.8/py_qgis_server.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-05-04 15:32:26.000000 py-qgis-server-1.8.8/py_qgis_server.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:32:26.358456 py-qgis-server-1.8.8/pyqgisserver/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 15:32:01.000000 py-qgis-server-1.8.8/pyqgisserver/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-05-04 15:32:04.000000 py-qgis-server-1.8.8/pyqgisserver/build.manifest
+-rw-r--r--   0 runner    (1001) docker     (123)    12382 2023-05-04 15:32:01.000000 py-qgis-server-1.8.8/pyqgisserver/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:32:26.358456 py-qgis-server-1.8.8/pyqgisserver/handlers/
+-rw-r--r--   0 runner    (1001) docker     (123)      351 2023-05-04 15:32:01.000000 py-qgis-server-1.8.8/pyqgisserver/handlers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6326 2023-05-04 15:32:01.000000 py-qgis-server-1.8.8/pyqgisserver/handlers/asynchandler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6049 2023-05-04 15:32:01.000000 py-qgis-server-1.8.8/pyqgisserver/handlers/basehandler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2178 2023-05-04 15:32:01.000000 py-qgis-server-1.8.8/pyqgisserver/handlers/landingpage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1693 2023-05-04 15:32:01.000000 py-qgis-server-1.8.8/pyqgisserver/handlers/oapihandler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2417 2023-05-04 15:32:01.000000 py-qgis-server-1.8.8/pyqgisserver/handlers/owshandler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2483 2023-05-04 15:32:01.000000 py-qgis-server-1.8.8/pyqgisserver/handlers/statushandler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3581 2023-05-04 15:32:01.000000 py-qgis-server-1.8.8/pyqgisserver/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:32:26.358456 py-qgis-server-1.8.8/pyqgisserver/management/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 15:32:01.000000 py-qgis-server-1.8.8/pyqgisserver/management/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:32:26.358456 py-qgis-server-1.8.8/pyqgisserver/management/apis/
+-rw-r--r--   0 runner    (1001) docker     (123)      467 2023-05-04 15:32:01.000000 py-qgis-server-1.8.8/pyqgisserver/management/apis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1384 2023-05-04 15:32:01.000000 py-qgis-server-1.8.8/pyqgisserver/management/apis/cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6887 2023-05-04 15:32:01.000000 py-qgis-server-1.8.8/pyqgisserver/management/apis/handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2025 2023-05-04 15:32:01.000000 py-qgis-server-1.8.8/pyqgisserver/management/apis/plugins.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6103 2023-05-04 15:32:01.000000 py-qgis-server-1.8.8/pyqgisserver/management/server.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2718 2023-05-04 15:32:01.000000 py-qgis-server-1.8.8/pyqgisserver/middleware.py
+-rw-r--r--   0 runner    (1001) docker     (123)      824 2023-05-04 15:32:01.000000 py-qgis-server-1.8.8/pyqgisserver/monitor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:32:26.362457 py-qgis-server-1.8.8/pyqgisserver/monitors/
+-rw-r--r--   0 runner    (1001) docker     (123)     4318 2023-05-04 15:32:01.000000 py-qgis-server-1.8.8/pyqgisserver/monitors/amqp.py
+-rw-r--r--   0 runner    (1001) docker     (123)      702 2023-05-04 15:32:01.000000 py-qgis-server-1.8.8/pyqgisserver/monitors/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      884 2023-05-04 15:32:01.000000 py-qgis-server-1.8.8/pyqgisserver/monitors/test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4711 2023-05-04 15:32:01.000000 py-qgis-server-1.8.8/pyqgisserver/plugins.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:32:26.362457 py-qgis-server-1.8.8/pyqgisserver/qgscache/
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-05-04 15:32:01.000000 py-qgis-server-1.8.8/pyqgisserver/qgscache/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19186 2023-05-04 15:32:01.000000 py-qgis-server-1.8.8/pyqgisserver/qgscache/cachemanager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:32:26.362457 py-qgis-server-1.8.8/pyqgisserver/qgscache/handlers/
+-rw-r--r--   0 runner    (1001) docker     (123)      365 2023-05-04 15:32:01.000000 py-qgis-server-1.8.8/pyqgisserver/qgscache/handlers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2529 2023-05-04 15:32:01.000000 py-qgis-server-1.8.8/pyqgisserver/qgscache/handlers/file_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5551 2023-05-04 15:32:01.000000 py-qgis-server-1.8.8/pyqgisserver/qgscache/handlers/postgres_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6237 2023-05-04 15:32:01.000000 py-qgis-server-1.8.8/pyqgisserver/qgscache/observer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:32:26.362457 py-qgis-server-1.8.8/pyqgisserver/qgscache/observers/
+-rw-r--r--   0 runner    (1001) docker     (123)     1542 2023-05-04 15:32:01.000000 py-qgis-server-1.8.8/pyqgisserver/qgscache/observers/ban.py
+-rw-r--r--   0 runner    (1001) docker     (123)      676 2023-05-04 15:32:01.000000 py-qgis-server-1.8.8/pyqgisserver/qgscache/observers/test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      383 2023-05-04 15:32:01.000000 py-qgis-server-1.8.8/pyqgisserver/qgscache/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7722 2023-05-04 15:32:01.000000 py-qgis-server-1.8.8/pyqgisserver/qgspool.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20749 2023-05-04 15:32:01.000000 py-qgis-server-1.8.8/pyqgisserver/qgsworker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9274 2023-05-04 15:32:01.000000 py-qgis-server-1.8.8/pyqgisserver/runtime.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3765 2023-05-04 15:32:01.000000 py-qgis-server-1.8.8/pyqgisserver/server.py
+-rw-r--r--   0 runner    (1001) docker     (123)      872 2023-05-04 15:32:01.000000 py-qgis-server-1.8.8/pyqgisserver/stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4652 2023-05-04 15:32:01.000000 py-qgis-server-1.8.8/pyqgisserver/tests.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:32:26.362457 py-qgis-server-1.8.8/pyqgisserver/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 15:32:01.000000 py-qgis-server-1.8.8/pyqgisserver/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2550 2023-05-04 15:32:01.000000 py-qgis-server-1.8.8/pyqgisserver/utils/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3523 2023-05-04 15:32:01.000000 py-qgis-server-1.8.8/pyqgisserver/utils/lru.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6045 2023-05-04 15:32:01.000000 py-qgis-server-1.8.8/pyqgisserver/utils/qgis.py
+-rw-r--r--   0 runner    (1001) docker     (123)      793 2023-05-04 15:32:01.000000 py-qgis-server-1.8.8/pyqgisserver/utils/stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)      862 2023-05-04 15:32:01.000000 py-qgis-server-1.8.8/pyqgisserver/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:32:26.362457 py-qgis-server-1.8.8/pyqgisserver/zeromq/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 15:32:01.000000 py-qgis-server-1.8.8/pyqgisserver/zeromq/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7185 2023-05-04 15:32:01.000000 py-qgis-server-1.8.8/pyqgisserver/zeromq/broker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8348 2023-05-04 15:32:01.000000 py-qgis-server-1.8.8/pyqgisserver/zeromq/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      537 2023-05-04 15:32:01.000000 py-qgis-server-1.8.8/pyqgisserver/zeromq/messages.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3970 2023-05-04 15:32:01.000000 py-qgis-server-1.8.8/pyqgisserver/zeromq/pool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4627 2023-05-04 15:32:01.000000 py-qgis-server-1.8.8/pyqgisserver/zeromq/supervisor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      296 2023-05-04 15:32:01.000000 py-qgis-server-1.8.8/pyqgisserver/zeromq/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8188 2023-05-04 15:32:01.000000 py-qgis-server-1.8.8/pyqgisserver/zeromq/worker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:32:26.354456 py-qgis-server-1.8.8/pyqgisservercontrib/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:32:26.362457 py-qgis-server-1.8.8/pyqgisservercontrib/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 15:32:01.000000 py-qgis-server-1.8.8/pyqgisservercontrib/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5194 2023-05-04 15:32:01.000000 py-qgis-server-1.8.8/pyqgisservercontrib/core/componentmanager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2668 2023-05-04 15:32:01.000000 py-qgis-server-1.8.8/pyqgisservercontrib/core/filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1549 2023-05-04 15:32:01.000000 py-qgis-server-1.8.8/pyqgisservercontrib/core/watchfiles.py
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-05-04 15:32:01.000000 py-qgis-server-1.8.8/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-05-04 15:32:26.362457 py-qgis-server-1.8.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2572 2023-05-04 15:32:01.000000 py-qgis-server-1.8.8/setup.py
```

### Comparing `py-qgis-server-1.8.7/PKG-INFO` & `py-qgis-server-1.8.8/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-qgis-server
-Version: 1.8.7
+Version: 1.8.8
 Summary: Py-Qgis-Server is an implementation of the OWS standards standard from the Open Geospatial Consortium.Py-Qgis-Server written in Python and built on top of Qgis serverimplementation
 Home-page: https://github.com/3liz/py-qgis-server
 Author: 3Liz
 Author-email: david.marteau@3liz.com
 Maintainer: David Marteau
 Maintainer-email: dmarteau@3liz.com
 Keywords: QGIS OWS OGC
@@ -22,15 +22,15 @@
 Description-Content-Type: text/markdown
 
 # QGIS embedded WMS/WFS/WCS asynchronous scalable server
 
 [![PyPi version badge](https://badgen.net/pypi/v/py-qgis-server)](https://pypi.org/project/py-qgis-server/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/py-qgis-server)](https://pypi.org/project/py-qgis-server/)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/py-qgis-server)](https://pypi.org/project/py-qgis-server/)
-
+[![Docker Pulls](https://img.shields.io/docker/pulls/3liz/qgis-map-server)](https://hub.docker.com/r/3liz/qgis-map-server/tags)
 
 ## Description
 
 This is an asynchronous HTTP QGIS server written in python on top of the [tornado](http://www.tornadoweb.org/en/stable/) framework and the
 0MQ messaging framework for distributing requests workers.
 
 It is based on the QGIS 3 server API for efficiently passing requests/responses using 0MQ messaging framework to workers.
```

### Comparing `py-qgis-server-1.8.7/README.md` & `py-qgis-server-1.8.8/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # QGIS embedded WMS/WFS/WCS asynchronous scalable server
 
 [![PyPi version badge](https://badgen.net/pypi/v/py-qgis-server)](https://pypi.org/project/py-qgis-server/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/py-qgis-server)](https://pypi.org/project/py-qgis-server/)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/py-qgis-server)](https://pypi.org/project/py-qgis-server/)
-
+[![Docker Pulls](https://img.shields.io/docker/pulls/3liz/qgis-map-server)](https://hub.docker.com/r/3liz/qgis-map-server/tags)
 
 ## Description
 
 This is an asynchronous HTTP QGIS server written in python on top of the [tornado](http://www.tornadoweb.org/en/stable/) framework and the
 0MQ messaging framework for distributing requests workers.
 
 It is based on the QGIS 3 server API for efficiently passing requests/responses using 0MQ messaging framework to workers.
```

### Comparing `py-qgis-server-1.8.7/py_qgis_server.egg-info/PKG-INFO` & `py-qgis-server-1.8.8/py_qgis_server.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-qgis-server
-Version: 1.8.7
+Version: 1.8.8
 Summary: Py-Qgis-Server is an implementation of the OWS standards standard from the Open Geospatial Consortium.Py-Qgis-Server written in Python and built on top of Qgis serverimplementation
 Home-page: https://github.com/3liz/py-qgis-server
 Author: 3Liz
 Author-email: david.marteau@3liz.com
 Maintainer: David Marteau
 Maintainer-email: dmarteau@3liz.com
 Keywords: QGIS OWS OGC
@@ -22,15 +22,15 @@
 Description-Content-Type: text/markdown
 
 # QGIS embedded WMS/WFS/WCS asynchronous scalable server
 
 [![PyPi version badge](https://badgen.net/pypi/v/py-qgis-server)](https://pypi.org/project/py-qgis-server/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/py-qgis-server)](https://pypi.org/project/py-qgis-server/)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/py-qgis-server)](https://pypi.org/project/py-qgis-server/)
-
+[![Docker Pulls](https://img.shields.io/docker/pulls/3liz/qgis-map-server)](https://hub.docker.com/r/3liz/qgis-map-server/tags)
 
 ## Description
 
 This is an asynchronous HTTP QGIS server written in python on top of the [tornado](http://www.tornadoweb.org/en/stable/) framework and the
 0MQ messaging framework for distributing requests workers.
 
 It is based on the QGIS 3 server API for efficiently passing requests/responses using 0MQ messaging framework to workers.
```

### Comparing `py-qgis-server-1.8.7/py_qgis_server.egg-info/SOURCES.txt` & `py-qgis-server-1.8.8/py_qgis_server.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `py-qgis-server-1.8.7/pyqgisserver/config.py` & `py-qgis-server-1.8.8/pyqgisserver/config.py`

 * *Files 3% similar despite different names*

```diff
@@ -86,15 +86,15 @@
 
     #
     # Api configuration
     #
 
     # Qgis api endpoints
     CONFIG.add_section('api.endpoints')
-    CONFIG.set('api.endpoints', 'landing_page', getenv('QGSRV_API_ENDPOINTS_LANDING_PAGE', '/ows/catalog'))
+    CONFIG.set('api.endpoints', 'landing_page', getenv('QGSRV_API_ENDPOINTS_LANDING_PAGE', '/catalog'))
     CONFIG.set('api.endpoints', 'lizmap_api', getenv('QGSRV_API_ENDPOINTS_LIZMAP', '/lizmap'))
 
     # Services enabled
     CONFIG.add_section('api.enabled')
     CONFIG.set('api.enabled', 'landing_page', getenv('QGSRV_API_ENABLED_LANDING_PAGE', 'no'))
     CONFIG.set('api.enabled', 'lizmap_api', getenv('QGSRV_API_ENABLED_LIZMAP', 'no'))
 
@@ -208,19 +208,19 @@
     confvalue = CONFIG[confname].get(confid, '')
 
     if not confvalue and optional:
         return
 
     confvalue = os.path.normpath(confvalue)
     if not os.path.isdir(confvalue):
-        LOGGER.error('server->%s configuration value %s is not directory' % (confid, confvalue))
+        LOGGER.error(f'server->{confid} configuration value {confvalue} is not directory')
         raise ValueError(confvalue)
 
     if not os.path.isabs(confvalue):
-        LOGGER.error('server->%s configuration value %s is not absolute path' % (confid, confvalue))
+        LOGGER.error(f'server->{confid} configuration value {confvalue} is not absolute path')
         raise ValueError(confvalue)
 
     CONFIG.set(confname, confid, confvalue)
 
 
 def configure_qgis_api(name: str) -> None:
     """ Configure qgis service environnement variables
@@ -269,26 +269,26 @@
         """
         value = _get_fun(section, option, fallback=NO_DEFAULT)
         if value is NO_DEFAULT:
             # Look in environment
             # Note that the section must exists
             if self.allow_env:
                 LOGGER.debug("Looking for option '%s.%s' in environment", section, option)
-                varname = 'QGSRV_%s_%s' % (section.upper(), option.upper())
+                varname = f'QGSRV_{section.upper()}_{option.upper()}'
                 varname = functools.reduce(lambda s, c: s.replace(c, '_'), ENV_REPLACE_CHARS, varname)
                 varvalue = os.getenv(varname)
                 if varvalue is not None:
                     LOGGER.debug("Setting config value from %s", varname)
                     CONFIG.set(section, option, varvalue)
                 # Let config parser translate the value for us
                 value = _get_fun(section, option, fallback=fallback)
             else:
                 value = fallback
         if value is NO_DEFAULT:
-            raise KeyError('[%s] %s' % (section, option))
+            raise KeyError(f'[{section}] {option}')
         return value
 
     get = functools.partialmethod(__get_impl, CONFIG.get)
     getint = functools.partialmethod(__get_impl, CONFIG.getint)
     getboolean = functools.partialmethod(__get_impl, CONFIG.getboolean)
     getfloat = functools.partialmethod(__get_impl, CONFIG.getfloat)
```

### Comparing `py-qgis-server-1.8.7/pyqgisserver/handlers/asynchandler.py` & `py-qgis-server-1.8.8/pyqgisserver/handlers/asynchandler.py`

 * *Files 2% similar despite different names*

```diff
@@ -75,15 +75,18 @@
             delta = None
             query = self.encode_arguments()
 
             headers = {}
             proxy_url = self.proxy_url()
             if proxy_url:
                 # Send the full path to Qgis
-                headers['X-Qgis-Forwarded-Url'] = f"{proxy_url}{self.request.path.lstrip('/')}"
+                req_url = f"{proxy_url}{self.request.path.lstrip('/')}"
+                headers['X-Qgis-Forwarded-Url'] = req_url
+            else:
+                req_url = self.request.uri
 
             self.set_backend_headers(headers)
 
             data = self.request.body
 
             if self.get_argument('SERVICE', default=None) and self.has_body_arguments:
                 # Do not let qgis server handle url encoded parameters
@@ -96,15 +99,15 @@
             response = await self._client.fetch(query=query, method=method,
                                                 headers=headers, data=data,
                                                 timeout=self._timeout)
             status = response.status
             hdrs = response.headers
             delta = time() - reqtime
 
-            log_rrequest(proxy_url, status, method, query, delta, hdrs)
+            log_rrequest(req_url, status, method, query, delta, hdrs)
 
             # Send response
             for k, v in hdrs.items():
                 self.set_header(k, v)
 
             # Send CORS Header
             self.set_access_control_headers()
@@ -130,21 +133,21 @@
             meta = response.metadata
 
         except RequestTimeoutError:
             status = 504
             delta = time() - reqtime
             # Log the request with status code 499 indicating
             # that the request has not returned
-            log_rrequest(proxy_url, 499, method, query, delta, {})
+            log_rrequest(req_url, 499, method, query, delta, {})
             self.send_error(status, reason="Request timeout error")
         except RequestGatewayError:
             status = 502
             delta = time() - reqtime
             # Log the request
-            log_rrequest(proxy_url, 499, method, query, delta, {})
+            log_rrequest(req_url, 499, method, query, delta, {})
             self.send_error(status, reason="Backend request error")
 
         if status >= 500:
             self._stats.num_errors += 1
 
         # Send monitoring info
         self.emit(status, delta, meta or {})
```

### Comparing `py-qgis-server-1.8.7/pyqgisserver/handlers/basehandler.py` & `py-qgis-server-1.8.8/pyqgisserver/handlers/basehandler.py`

 * *Files 4% similar despite different names*

```diff
@@ -47,23 +47,28 @@
         self.clear_header("Content-Type")
         self.set_header("Server", f"Py-Qgis-Server {__version__}")
 
     def on_connection_close(self) -> None:
         """ Override, log and set 'connection_closed' to True
         """
         self.connection_closed = True
-        self.logger.warning("Connection closed by client: {}".format(self.request.uri))
+        self.logger.warning(f"Connection closed by client: {self.request.uri}")
 
     def set_option_headers(self, allow_header: Optional[str] = None) -> None:
         """  Set correct headers for 'OPTIONS' method
         """
         if not allow_header:
             allow_header = ', '.join(me for me in self.SUPPORTED_METHODS if hasattr(self, me.lower()))
 
         self.set_header("Allow", allow_header)
+        # Required if the request has an "Authorization" header.
+        # This is useful to implement authentification on top QGIS SERVER
+        # see https://developer.mozilla.org/en-US/docs/Web/HTTP/Headers/Access-Control-Allow-Headers &
+        # https://developer.mozilla.org/en-US/docs/Web/HTTP/Headers/Authorization
+        self.set_header('Access-Control-Allow-Headers', 'Authorization')
         if self.set_access_control_headers():
             # Required in CORS context
             # see https://developer.mozilla.org/fr/docs/Web/HTTP/M%C3%A9thode/OPTIONS
             self.set_header('Access-Control-Allow-Methods', allow_header)
 
     def set_access_control_headers(self) -> bool:
         """  Handle Access control and cross origin headers (CORS)
```

### Comparing `py-qgis-server-1.8.7/pyqgisserver/handlers/landingpage.py` & `py-qgis-server-1.8.8/pyqgisserver/handlers/landingpage.py`

 * *Files identical despite different names*

### Comparing `py-qgis-server-1.8.7/pyqgisserver/handlers/oapihandler.py` & `py-qgis-server-1.8.8/pyqgisserver/handlers/oapihandler.py`

 * *Files identical despite different names*

### Comparing `py-qgis-server-1.8.7/pyqgisserver/handlers/owshandler.py` & `py-qgis-server-1.8.8/pyqgisserver/handlers/owshandler.py`

 * *Files identical despite different names*

### Comparing `py-qgis-server-1.8.7/pyqgisserver/handlers/statushandler.py` & `py-qgis-server-1.8.8/pyqgisserver/handlers/statushandler.py`

 * *Files identical despite different names*

### Comparing `py-qgis-server-1.8.7/pyqgisserver/logger.py` & `py-qgis-server-1.8.8/pyqgisserver/logger.py`

 * *Files identical despite different names*

### Comparing `py-qgis-server-1.8.7/pyqgisserver/management/apis/cache.py` & `py-qgis-server-1.8.8/pyqgisserver/management/apis/cache.py`

 * *Files identical despite different names*

### Comparing `py-qgis-server-1.8.7/pyqgisserver/management/apis/handler.py` & `py-qgis-server-1.8.8/pyqgisserver/management/apis/handler.py`

 * *Files identical despite different names*

### Comparing `py-qgis-server-1.8.7/pyqgisserver/management/apis/plugins.py` & `py-qgis-server-1.8.8/pyqgisserver/management/apis/plugins.py`

 * *Files identical despite different names*

### Comparing `py-qgis-server-1.8.7/pyqgisserver/management/server.py` & `py-qgis-server-1.8.8/pyqgisserver/management/server.py`

 * *Files identical despite different names*

### Comparing `py-qgis-server-1.8.7/pyqgisserver/middleware.py` & `py-qgis-server-1.8.8/pyqgisserver/middleware.py`

 * *Files identical despite different names*

### Comparing `py-qgis-server-1.8.7/pyqgisserver/monitor.py` & `py-qgis-server-1.8.8/pyqgisserver/monitor.py`

 * *Files identical despite different names*

### Comparing `py-qgis-server-1.8.7/pyqgisserver/monitors/amqp.py` & `py-qgis-server-1.8.8/pyqgisserver/monitors/amqp.py`

 * *Files identical despite different names*

### Comparing `py-qgis-server-1.8.7/pyqgisserver/monitors/base.py` & `py-qgis-server-1.8.8/pyqgisserver/monitors/base.py`

 * *Files identical despite different names*

### Comparing `py-qgis-server-1.8.7/pyqgisserver/monitors/test.py` & `py-qgis-server-1.8.8/pyqgisserver/monitors/test.py`

 * *Files identical despite different names*

### Comparing `py-qgis-server-1.8.7/pyqgisserver/plugins.py` & `py-qgis-server-1.8.8/pyqgisserver/plugins.py`

 * *Files 3% similar despite different names*

```diff
@@ -34,15 +34,15 @@
         minor = int(ver[0]) if len(ver) > 0 else 0
         rev = int(ver[1]) if len(ver) > 1 else 0
         if minor >= 99:
             minor = rev = 0
             major += 1
         if rev > 99:
             rev = 99
-        return int("{:d}{:02d}{:02d}".format(major, minor, rev))
+        return int(f"{major:d}{minor:02d}{rev:02d}")
 
     version = to_int(Qgis.QGIS_VERSION.split('-')[0])
     minver = to_int(minver) if minver else version
     maxver = to_int(maxver) if maxver else version
 
     return minver <= version <= maxver
```

### Comparing `py-qgis-server-1.8.7/pyqgisserver/qgscache/cachemanager.py` & `py-qgis-server-1.8.8/pyqgisserver/qgscache/cachemanager.py`

 * *Files 0% similar despite different names*

```diff
@@ -67,15 +67,15 @@
 def _merge_qs(query1: str, query2: str) -> str:
     """ Merge query1 with query2 but coerce values
         from query1
     """
     params_1 = parse_qs(query1)
     params_2 = parse_qs(query2)
     params_2.update(params_1)
-    return '&'.join('%s=%s' % (k, v[0]) for k, v in params_2.items())
+    return '&'.join(f'{k}={v[0]}' for k, v in params_2.items())
 
 
 class CacheType(Enum):
     LRU = 'lru'
     STATIC = 'static'
 
 
@@ -448,15 +448,15 @@
 
     def handleBadLayers(self, layers) -> None:
         """ See https://qgis.org/pyqgis/3.0/core/Project/QgsProjectBadLayerHandler.html
         """
         super().handleBadLayers(layers)
 
         nameElements = (lyr.firstChildElement("layername") for lyr in layers if lyr)
-        self.badLayerNames = set(elem.text() for elem in nameElements if elem)
+        self.badLayerNames = {elem.text() for elem in nameElements if elem}
 
     def validateLayers(self, project: QgsProject) -> bool:
         """ Check layers
 
             If layers are excluded do not count them as bad layers
             see https://github.com/qgis/QGIS/pull/33668
         """
```

### Comparing `py-qgis-server-1.8.7/pyqgisserver/qgscache/handlers/file_handler.py` & `py-qgis-server-1.8.8/pyqgisserver/qgscache/handlers/file_handler.py`

 * *Files identical despite different names*

### Comparing `py-qgis-server-1.8.7/pyqgisserver/qgscache/handlers/postgres_handler.py` & `py-qgis-server-1.8.8/pyqgisserver/qgscache/handlers/postgres_handler.py`

 * *Files 1% similar despite different names*

```diff
@@ -91,15 +91,15 @@
         netloc = f'{url.username}@' if url.username else ''
 
     # Create secure url
     params.update(project=prjname, schema=schema)
     if database:
         params.update(dbname=database)
 
-    params = '&'.join('%s=%s' % (k, v) for k, v in params.items())
+    params = '&'.join(f'{k}={v}' for k, v in params.items())
     urlstr = f"postgresql://{netloc}/?{params}"
 
     try:
         LOGGER.debug("**** Postgresql connection params %s", connexion_params)
         conn = psycopg2.connect(**connexion_params)
         cursor = conn.cursor()
         cursor.execute(f"select metadata from {schema}.qgis_projects where name='{prjname}'")
```

### Comparing `py-qgis-server-1.8.7/pyqgisserver/qgscache/observer.py` & `py-qgis-server-1.8.8/pyqgisserver/qgscache/observer.py`

 * *Files identical despite different names*

### Comparing `py-qgis-server-1.8.7/pyqgisserver/qgscache/observers/ban.py` & `py-qgis-server-1.8.8/pyqgisserver/qgscache/observers/ban.py`

 * *Files identical despite different names*

### Comparing `py-qgis-server-1.8.7/pyqgisserver/qgscache/observers/test.py` & `py-qgis-server-1.8.8/pyqgisserver/qgscache/observers/test.py`

 * *Files identical despite different names*

### Comparing `py-qgis-server-1.8.7/pyqgisserver/qgspool.py` & `py-qgis-server-1.8.8/pyqgisserver/qgspool.py`

 * *Files identical despite different names*

### Comparing `py-qgis-server-1.8.7/pyqgisserver/qgsworker.py` & `py-qgis-server-1.8.8/pyqgisserver/qgsworker.py`

 * *Files 2% similar despite different names*

```diff
@@ -470,15 +470,15 @@
         else:
             # See https://github.com/qgis/QGIS/pull/9773
             iface.setConfigFilePath(config_path)
             self.qgis_server.handleRequest(request, response, project=project)
 
     @classmethod
     def get_report(cls):
-        report = super(QgsRequestHandler, cls).get_report()
+        report = super().get_report()
 
         def _to_json(key: str, project: QgsProject, static: bool):
             return dict(
                 key=key,
                 filename=project.fileName(),
                 last_modified=project.lastModified().toString(Qt.ISODate),
                 num_layers=project.count(),
@@ -528,15 +528,15 @@
         sys.exit(1)
     else:
         print_version()
 
     load_configuration()
 
     if args.config:
-        with open(args.config, mode='rt') as config_file:
+        with open(args.config) as config_file:
             read_config_file(config_file)
 
     # Override config
     def set_arg(section: str, name: str) -> None:
         if name in args:
             confservice.set(section, name, str(getattr(args, name)))
 
@@ -548,15 +548,15 @@
         confservice.set('logging', 'level', 'DEBUG')
 
     print_version()
 
     validate_config_path('projects.cache', 'rootdir')
 
     setup_log_handler(confservice.get('logging', 'level'))
-    print("Log level set to {}\n".format(logging.getLevelName(LOGGER.level)), file=sys.stderr)
+    print(f"Log level set to {logging.getLevelName(LOGGER.level)}\n", file=sys.stderr)
 
     broadcastaddr = confservice.get('zmq', 'broadcastaddr')
     router = confservice.get('zmq', 'bindaddr')
 
     QgsRequestHandler.run(router, identity=args.identity,
                           broadcastaddr=broadcastaddr)
```

### Comparing `py-qgis-server-1.8.7/pyqgisserver/runtime.py` & `py-qgis-server-1.8.8/pyqgisserver/runtime.py`

 * *Files 2% similar despite different names*

```diff
@@ -105,15 +105,15 @@
 
 class Application(tornado.web.Application):
 
     def __init__(self, router: str) -> None:
         """
         """
         identity = confservice['zmq']['identity']
-        identity = "{}-{}".format(identity, os.getpid())
+        identity = f"{identity}-{os.getpid()}"
 
         self._broker_client = client.AsyncClient(router, bytes(identity.encode('ascii')))
         self.stats = Stats()
 
         self.http_proxy = confservice.getboolean('server', 'http_proxy')
 
         super().__init__(configure_handlers(self._broker_client),
@@ -130,15 +130,15 @@
 
 def setuid(username: str) -> None:
     """ setuid to username uid """
     from pwd import getpwnam, getpwuid
     pw = getpwnam(username)
     os.setgid(pw.pw_gid)
     os.setuid(pw.pw_uid)
-    LOGGER.info("Setuid to user {} ({}:{})".format(getpwuid(os.getuid()).pw_name, os.getuid(), os.getgid()))
+    LOGGER.info(f"Setuid to user {getpwuid(os.getuid()).pw_name} ({os.getuid()}:{os.getgid()})")
 
 
 def create_broker_process(ipcaddr: str) -> Process:
     """ Create a brker process
     """
     cfg = confservice['zmq']
 
@@ -298,15 +298,15 @@
         server.stop()
     if management is not None:
         management.terminate()
         management = None
     if application is not None:
         application.terminate()
         application = None
-        print("PID {}: Server instance stopped".format(os.getpid()), flush=True)
+        print(f"PID {os.getpid()}: Server instance stopped", flush=True)
     if cache_observer:
         cache_observer.stop()
     if worker_pool:
         print("Stopping workers", flush=True)
         worker_pool.terminate()
     if broker_pr:
         print("Stopping broker", flush=True)
```

### Comparing `py-qgis-server-1.8.7/pyqgisserver/server.py` & `py-qgis-server-1.8.8/pyqgisserver/server.py`

 * *Files 1% similar despite different names*

```diff
@@ -62,15 +62,15 @@
         sys.exit(1)
     else:
         print_version()
 
     load_configuration()
 
     if args.config:
-        with open(args.config, mode='rt') as config_file:
+        with open(args.config) as config_file:
             read_config_file(config_file)
 
     # Override config
     def set_arg(section: str, name: str) -> None:
         if name in args:
             confservice.set(section, name, str(getattr(args, name)))
 
@@ -81,15 +81,15 @@
 
     if args.debug:
         # Force debug mode
         confservice.set('logging', 'level', 'DEBUG')
 
     # set log level
     setup_log_handler(confservice.get('logging', 'level'))
-    print("Log level set to {}\n".format(logging.getLevelName(LOGGER.level)), file=sys.stderr)
+    print(f"Log level set to {logging.getLevelName(LOGGER.level)}\n", file=sys.stderr)
 
     conf = confservice['server']
     args.port = conf.getint('port')
     args.workers = conf.getint('workers')
     args.interfaces = conf.get('interfaces')
 
     return args
```

### Comparing `py-qgis-server-1.8.7/pyqgisserver/stats.py` & `py-qgis-server-1.8.8/pyqgisserver/stats.py`

 * *Files identical despite different names*

### Comparing `py-qgis-server-1.8.7/pyqgisserver/tests.py` & `py-qgis-server-1.8.8/pyqgisserver/tests.py`

 * *Files identical despite different names*

### Comparing `py-qgis-server-1.8.7/pyqgisserver/utils/decorators.py` & `py-qgis-server-1.8.8/pyqgisserver/utils/decorators.py`

 * *Files identical despite different names*

### Comparing `py-qgis-server-1.8.7/pyqgisserver/utils/lru.py` & `py-qgis-server-1.8.8/pyqgisserver/utils/lru.py`

 * *Files identical despite different names*

### Comparing `py-qgis-server-1.8.7/pyqgisserver/utils/qgis.py` & `py-qgis-server-1.8.8/pyqgisserver/utils/qgis.py`

 * *Files 2% similar despite different names*

```diff
@@ -50,17 +50,20 @@
 
     if QgsApplication.QGIS_APPLICATION_NAME != "QGIS3":
         raise RuntimeError("You need QGIS3 (found %s)" % QgsApplication.QGIS_APPLICATION_NAME)
 
     if not enable_gui:
         #  We MUST set the QT_QPA_PLATFORM to prevent
         #  Qt trying to connect to display in containers
-        if os.environ.get('DISPLAY') is None:
+        display = os.environ.get('DISPLAY')
+        if display is None:
             logger.info("Setting offscreen mode")
             os.environ['QT_QPA_PLATFORM'] = 'offscreen'
+        else:
+            logger.info(f"Using DISPLAY: {display}")
 
     qgis_prefix = os.environ.get('QGIS3_HOME', '/usr')
 
     # XXX Set QGIS_PREFIX_PATH, it seems that setPrefixPath
     # does not do the job correctly
     os.environ['QGIS_PREFIX_PATH'] = qgis_prefix
 
@@ -109,15 +112,15 @@
 def install_logger_hook(logger: logging.Logger, logprefix: str, verbose: bool = False) -> None:
     """ Install message log hook
     """
     from qgis.core import Qgis, QgsApplication
     # Add a hook to qgis  message log
 
     def writelogmessage(message, tag, level):
-        arg = '{} {}: {}'.format(logprefix, tag, message)
+        arg = f'{logprefix} {tag}: {message}'
         if level == Qgis.Warning:
             logger.warning(arg)
         elif level == Qgis.Critical:
             logger.error(arg)
         elif verbose:
             # Qgis is somehow very noisy
             # log only if verbose is set
```

### Comparing `py-qgis-server-1.8.7/pyqgisserver/utils/stats.py` & `py-qgis-server-1.8.8/pyqgisserver/utils/stats.py`

 * *Files identical despite different names*

### Comparing `py-qgis-server-1.8.7/pyqgisserver/version.py` & `py-qgis-server-1.8.8/pyqgisserver/version.py`

 * *Files identical despite different names*

### Comparing `py-qgis-server-1.8.7/pyqgisserver/zeromq/broker.py` & `py-qgis-server-1.8.8/pyqgisserver/zeromq/broker.py`

 * *Files 2% similar despite different names*

```diff
@@ -166,15 +166,15 @@
                         help="Max waiting queue")
     parser.add_argument('--timeout', metavar='NUM', type=int, default=3000,
                         help="Set timeout in ms for waiting requests")
 
     args = parser.parse_args()
 
     setup_log_handler(args.logging)
-    print("Log level set to {}\n".format(logging.getLevelName(LOGGER.level)), file=sys.stderr)
+    print(f"Log level set to {logging.getLevelName(LOGGER.level)}\n", file=sys.stderr)
 
     LOGGER.setLevel(getattr(logging, args.logging.upper()))
 
     run_broker(args.inaddr.format(iface=args.iface),
                args.outaddr.format(iface=args.iface),
                maxqueue=args.maxqueue,
                timeout=args.timeout)
```

### Comparing `py-qgis-server-1.8.7/pyqgisserver/zeromq/client.py` & `py-qgis-server-1.8.8/pyqgisserver/zeromq/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -214,15 +214,15 @@
                         help="set log level")
     parser.add_argument('--identity', default='', help="Set worker identity")
     parser.add_argument('--count', default=1, type=int, help="Number of requests")
 
     args = parser.parse_args()
 
     setup_log_handler(args.logging)
-    print("Log level set to {}\n".format(logging.getLevelName(LOGGER.level)), file=sys.stderr)
+    print(f"Log level set to {logging.getLevelName(LOGGER.level)}\n", file=sys.stderr)
 
     LOGGER.setLevel(getattr(logging, args.logging.upper()))
 
     client = AsyncClient(args.router.format(host=args.host), bytes(args.identity.encode('ascii')))
     sleep(1)  # Give some time to connection to establish
 
     async def fetch(index):
```

### Comparing `py-qgis-server-1.8.7/pyqgisserver/zeromq/messages.py` & `py-qgis-server-1.8.8/pyqgisserver/zeromq/messages.py`

 * *Files identical despite different names*

### Comparing `py-qgis-server-1.8.7/pyqgisserver/zeromq/pool.py` & `py-qgis-server-1.8.8/pyqgisserver/zeromq/pool.py`

 * *Files identical despite different names*

### Comparing `py-qgis-server-1.8.7/pyqgisserver/zeromq/supervisor.py` & `py-qgis-server-1.8.8/pyqgisserver/zeromq/supervisor.py`

 * *Files identical despite different names*

### Comparing `py-qgis-server-1.8.7/pyqgisserver/zeromq/worker.py` & `py-qgis-server-1.8.8/pyqgisserver/zeromq/worker.py`

 * *Files 2% similar despite different names*

```diff
@@ -175,15 +175,15 @@
                 LOGGER.error("Worker Error %s", exc)
                 # Print trace outside LOGGER because
                 # logging output in sub-processe
                 # is not captured by pytest
                 traceback.print_exc()
                 if handler and not handler.header_written:
                     handler.status_code = 500
-                    handler.send("Worker internal error".encode())
+                    handler.send(b"Worker internal error")
                     # Got error 500, do not presume worker state
                     break
             finally:
                 supervisor.notify_done()
 
             # Handle broadcast notifications
             try:
@@ -224,14 +224,14 @@
     parser.add_argument('--logging', choices=['debug', 'info', 'warning', 'error'], default='info',
                         help="set log level")
     parser.add_argument('--identity', default="", help="Set worker identity")
 
     args = parser.parse_args()
 
     setup_log_handler(args.logging)
-    print("Log level set to {}\n".format(logging.getLevelName(LOGGER.level)), file=sys.stderr)
+    print(f"Log level set to {logging.getLevelName(LOGGER.level)}\n", file=sys.stderr)
 
     LOGGER.setLevel(getattr(logging, args.logging.upper()))
 
     run_worker(args.router.format(host=args.host), RequestHandler,
                identity=bytes(args.identity.encode('ascii')))
     print("DONE", file=sys.stderr)
```

### Comparing `py-qgis-server-1.8.7/pyqgisservercontrib/core/componentmanager.py` & `py-qgis-server-1.8.8/pyqgisservercontrib/core/componentmanager.py`

 * *Files identical despite different names*

### Comparing `py-qgis-server-1.8.7/pyqgisservercontrib/core/filters.py` & `py-qgis-server-1.8.8/pyqgisservercontrib/core/filters.py`

 * *Files identical despite different names*

### Comparing `py-qgis-server-1.8.7/pyqgisservercontrib/core/watchfiles.py` & `py-qgis-server-1.8.8/pyqgisservercontrib/core/watchfiles.py`

 * *Files identical despite different names*

### Comparing `py-qgis-server-1.8.7/setup.py` & `py-qgis-server-1.8.8/setup.py`

 * *Files identical despite different names*

