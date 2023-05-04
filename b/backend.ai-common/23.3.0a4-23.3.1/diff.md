# Comparing `tmp/backend.ai-common-23.3.0a4.tar.gz` & `tmp/backend.ai-common-23.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "backend.ai-common-23.3.0a4.tar", last modified: Thu Mar 16 02:52:59 2023, max compression
+gzip compressed data, was "backend.ai-common-23.3.1.tar", last modified: Thu May  4 05:10:14 2023, max compression
```

## Comparing `backend.ai-common-23.3.0a4.tar` & `backend.ai-common-23.3.1.tar`

### file list

```diff
@@ -1,58 +1,59 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 02:52:59.764138 backend.ai-common-23.3.0a4/
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-03-16 02:52:59.000000 backend.ai-common-23.3.0a4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2304 2023-03-16 02:52:59.764138 backend.ai-common-23.3.0a4/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 02:52:59.744137 backend.ai-common-23.3.0a4/ai/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 02:52:59.744137 backend.ai-common-23.3.0a4/ai/backend/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 02:52:59.752137 backend.ai-common-23.3.0a4/ai/backend/common/
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-03-16 02:52:59.000000 backend.ai-common-23.3.0a4/ai/backend/common/VERSION
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-03-16 02:52:59.000000 backend.ai-common-23.3.0a4/ai/backend/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      484 2023-03-16 02:52:59.000000 backend.ai-common-23.3.0a4/ai/backend/common/arch.py
--rw-r--r--   0 runner    (1001) docker     (123)     3117 2023-03-16 02:52:59.000000 backend.ai-common-23.3.0a4/ai/backend/common/argparse.py
--rw-r--r--   0 runner    (1001) docker     (123)     3057 2023-03-16 02:52:59.000000 backend.ai-common-23.3.0a4/ai/backend/common/asyncio.py
--rw-r--r--   0 runner    (1001) docker     (123)    11022 2023-03-16 02:52:59.000000 backend.ai-common-23.3.0a4/ai/backend/common/bgtask.py
--rw-r--r--   0 runner    (1001) docker     (123)     2226 2023-03-16 02:52:59.000000 backend.ai-common-23.3.0a4/ai/backend/common/cgroup.py
--rw-r--r--   0 runner    (1001) docker     (123)     3021 2023-03-16 02:52:59.000000 backend.ai-common-23.3.0a4/ai/backend/common/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     4574 2023-03-16 02:52:59.000000 backend.ai-common-23.3.0a4/ai/backend/common/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2245 2023-03-16 02:52:59.000000 backend.ai-common-23.3.0a4/ai/backend/common/distributed.py
--rw-r--r--   0 runner    (1001) docker     (123)    18064 2023-03-16 02:52:59.000000 backend.ai-common-23.3.0a4/ai/backend/common/docker.py
--rw-r--r--   0 runner    (1001) docker     (123)     1373 2023-03-16 02:52:59.000000 backend.ai-common-23.3.0a4/ai/backend/common/enum_extension.py
--rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-03-16 02:52:59.000000 backend.ai-common-23.3.0a4/ai/backend/common/enum_extension.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    19237 2023-03-16 02:52:59.000000 backend.ai-common-23.3.0a4/ai/backend/common/etcd.py
--rw-r--r--   0 runner    (1001) docker     (123)    26327 2023-03-16 02:52:59.000000 backend.ai-common-23.3.0a4/ai/backend/common/events.py
--rw-r--r--   0 runner    (1001) docker     (123)     2032 2023-03-16 02:52:59.000000 backend.ai-common-23.3.0a4/ai/backend/common/exception.py
--rw-r--r--   0 runner    (1001) docker     (123)     1899 2023-03-16 02:52:59.000000 backend.ai-common-23.3.0a4/ai/backend/common/files.py
--rw-r--r--   0 runner    (1001) docker     (123)     9077 2023-03-16 02:52:59.000000 backend.ai-common-23.3.0a4/ai/backend/common/identity.py
--rw-r--r--   0 runner    (1001) docker     (123)      290 2023-03-16 02:52:59.000000 backend.ai-common-23.3.0a4/ai/backend/common/json.py
--rw-r--r--   0 runner    (1001) docker     (123)     7882 2023-03-16 02:52:59.000000 backend.ai-common-23.3.0a4/ai/backend/common/lock.py
--rw-r--r--   0 runner    (1001) docker     (123)    21147 2023-03-16 02:52:59.000000 backend.ai-common-23.3.0a4/ai/backend/common/logging.py
--rw-r--r--   0 runner    (1001) docker     (123)      567 2023-03-16 02:52:59.000000 backend.ai-common-23.3.0a4/ai/backend/common/logging_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2729 2023-03-16 02:52:59.000000 backend.ai-common-23.3.0a4/ai/backend/common/msgpack.py
--rw-r--r--   0 runner    (1001) docker     (123)     1555 2023-03-16 02:52:59.000000 backend.ai-common-23.3.0a4/ai/backend/common/networking.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 02:52:59.756137 backend.ai-common-23.3.0a4/ai/backend/common/plugin/
--rw-r--r--   0 runner    (1001) docker     (123)     7022 2023-03-16 02:52:59.000000 backend.ai-common-23.3.0a4/ai/backend/common/plugin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5652 2023-03-16 02:52:59.000000 backend.ai-common-23.3.0a4/ai/backend/common/plugin/hook.py
--rw-r--r--   0 runner    (1001) docker     (123)     2326 2023-03-16 02:52:59.000000 backend.ai-common-23.3.0a4/ai/backend/common/plugin/monitor.py
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-03-16 02:52:59.000000 backend.ai-common-23.3.0a4/ai/backend/common/plugin/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-03-16 02:52:59.000000 backend.ai-common-23.3.0a4/ai/backend/common/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    16479 2023-03-16 02:52:59.000000 backend.ai-common-23.3.0a4/ai/backend/common/redis_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)     3914 2023-03-16 02:52:59.000000 backend.ai-common-23.3.0a4/ai/backend/common/sd_notify.py
--rw-r--r--   0 runner    (1001) docker     (123)     2994 2023-03-16 02:52:59.000000 backend.ai-common-23.3.0a4/ai/backend/common/service_ports.py
--rw-r--r--   0 runner    (1001) docker     (123)     1401 2023-03-16 02:52:59.000000 backend.ai-common-23.3.0a4/ai/backend/common/testutils.py
--rw-r--r--   0 runner    (1001) docker     (123)    30192 2023-03-16 02:52:59.000000 backend.ai-common-23.3.0a4/ai/backend/common/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     8900 2023-03-16 02:52:59.000000 backend.ai-common-23.3.0a4/ai/backend/common/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    22692 2023-03-16 02:52:59.000000 backend.ai-common-23.3.0a4/ai/backend/common/validators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 02:52:59.744137 backend.ai-common-23.3.0a4/ai/backend/common/web/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 02:52:59.756137 backend.ai-common-23.3.0a4/ai/backend/common/web/session/
--rw-r--r--   0 runner    (1001) docker     (123)    10834 2023-03-16 02:52:59.000000 backend.ai-common-23.3.0a4/ai/backend/common/web/session/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3962 2023-03-16 02:52:59.000000 backend.ai-common-23.3.0a4/ai/backend/common/web/session/redis_storage.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 02:52:59.764138 backend.ai-common-23.3.0a4/backend.ai_common.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2304 2023-03-16 02:52:59.000000 backend.ai-common-23.3.0a4/backend.ai_common.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1506 2023-03-16 02:52:59.000000 backend.ai-common-23.3.0a4/backend.ai_common.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-16 02:52:59.000000 backend.ai-common-23.3.0a4/backend.ai_common.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-16 02:52:59.000000 backend.ai-common-23.3.0a4/backend.ai_common.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-16 02:52:59.000000 backend.ai-common-23.3.0a4/backend.ai_common.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      506 2023-03-16 02:52:59.000000 backend.ai-common-23.3.0a4/backend.ai_common.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        3 2023-03-16 02:52:59.000000 backend.ai-common-23.3.0a4/backend.ai_common.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      626 2023-03-16 02:52:59.000000 backend.ai-common-23.3.0a4/backend_shim.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-16 02:52:59.764138 backend.ai-common-23.3.0a4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3872 2023-03-16 02:52:59.000000 backend.ai-common-23.3.0a4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 05:10:14.430715 backend.ai-common-23.3.1/
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-04 05:10:14.000000 backend.ai-common-23.3.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2314 2023-05-04 05:10:14.430715 backend.ai-common-23.3.1/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 05:10:14.426715 backend.ai-common-23.3.1/ai/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 05:10:14.426715 backend.ai-common-23.3.1/ai/backend/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 05:10:14.430715 backend.ai-common-23.3.1/ai/backend/common/
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-04 05:10:14.000000 backend.ai-common-23.3.1/ai/backend/common/VERSION
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-04 05:10:14.000000 backend.ai-common-23.3.1/ai/backend/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      484 2023-05-04 05:10:14.000000 backend.ai-common-23.3.1/ai/backend/common/arch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3117 2023-05-04 05:10:14.000000 backend.ai-common-23.3.1/ai/backend/common/argparse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3057 2023-05-04 05:10:14.000000 backend.ai-common-23.3.1/ai/backend/common/asyncio.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11022 2023-05-04 05:10:14.000000 backend.ai-common-23.3.1/ai/backend/common/bgtask.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2226 2023-05-04 05:10:14.000000 backend.ai-common-23.3.1/ai/backend/common/cgroup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3021 2023-05-04 05:10:14.000000 backend.ai-common-23.3.1/ai/backend/common/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4622 2023-05-04 05:10:14.000000 backend.ai-common-23.3.1/ai/backend/common/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2245 2023-05-04 05:10:14.000000 backend.ai-common-23.3.1/ai/backend/common/distributed.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18046 2023-05-04 05:10:14.000000 backend.ai-common-23.3.1/ai/backend/common/docker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1373 2023-05-04 05:10:14.000000 backend.ai-common-23.3.1/ai/backend/common/enum_extension.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-05-04 05:10:14.000000 backend.ai-common-23.3.1/ai/backend/common/enum_extension.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    19237 2023-05-04 05:10:14.000000 backend.ai-common-23.3.1/ai/backend/common/etcd.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26166 2023-05-04 05:10:14.000000 backend.ai-common-23.3.1/ai/backend/common/events.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2032 2023-05-04 05:10:14.000000 backend.ai-common-23.3.1/ai/backend/common/exception.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1899 2023-05-04 05:10:14.000000 backend.ai-common-23.3.1/ai/backend/common/files.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9077 2023-05-04 05:10:14.000000 backend.ai-common-23.3.1/ai/backend/common/identity.py
+-rw-r--r--   0 runner    (1001) docker     (123)      290 2023-05-04 05:10:14.000000 backend.ai-common-23.3.1/ai/backend/common/json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7882 2023-05-04 05:10:14.000000 backend.ai-common-23.3.1/ai/backend/common/lock.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21123 2023-05-04 05:10:14.000000 backend.ai-common-23.3.1/ai/backend/common/logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)      637 2023-05-04 05:10:14.000000 backend.ai-common-23.3.1/ai/backend/common/logging_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2729 2023-05-04 05:10:14.000000 backend.ai-common-23.3.1/ai/backend/common/msgpack.py
+-rw-r--r--   0 runner    (1001) docker     (123)      700 2023-05-04 05:10:14.000000 backend.ai-common-23.3.1/ai/backend/common/netns.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1555 2023-05-04 05:10:14.000000 backend.ai-common-23.3.1/ai/backend/common/networking.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 05:10:14.430715 backend.ai-common-23.3.1/ai/backend/common/plugin/
+-rw-r--r--   0 runner    (1001) docker     (123)     7078 2023-05-04 05:10:14.000000 backend.ai-common-23.3.1/ai/backend/common/plugin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5652 2023-05-04 05:10:14.000000 backend.ai-common-23.3.1/ai/backend/common/plugin/hook.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2326 2023-05-04 05:10:14.000000 backend.ai-common-23.3.1/ai/backend/common/plugin/monitor.py
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-04 05:10:14.000000 backend.ai-common-23.3.1/ai/backend/common/plugin/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-04 05:10:14.000000 backend.ai-common-23.3.1/ai/backend/common/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    16476 2023-05-04 05:10:14.000000 backend.ai-common-23.3.1/ai/backend/common/redis_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3914 2023-05-04 05:10:14.000000 backend.ai-common-23.3.1/ai/backend/common/sd_notify.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2970 2023-05-04 05:10:14.000000 backend.ai-common-23.3.1/ai/backend/common/service_ports.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1401 2023-05-04 05:10:14.000000 backend.ai-common-23.3.1/ai/backend/common/testutils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30192 2023-05-04 05:10:14.000000 backend.ai-common-23.3.1/ai/backend/common/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8911 2023-05-04 05:10:14.000000 backend.ai-common-23.3.1/ai/backend/common/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22692 2023-05-04 05:10:14.000000 backend.ai-common-23.3.1/ai/backend/common/validators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 05:10:14.426715 backend.ai-common-23.3.1/ai/backend/common/web/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 05:10:14.430715 backend.ai-common-23.3.1/ai/backend/common/web/session/
+-rw-r--r--   0 runner    (1001) docker     (123)    10798 2023-05-04 05:10:14.000000 backend.ai-common-23.3.1/ai/backend/common/web/session/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3962 2023-05-04 05:10:14.000000 backend.ai-common-23.3.1/ai/backend/common/web/session/redis_storage.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 05:10:14.430715 backend.ai-common-23.3.1/backend.ai_common.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2314 2023-05-04 05:10:14.000000 backend.ai-common-23.3.1/backend.ai_common.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1533 2023-05-04 05:10:14.000000 backend.ai-common-23.3.1/backend.ai_common.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 05:10:14.000000 backend.ai-common-23.3.1/backend.ai_common.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 05:10:14.000000 backend.ai-common-23.3.1/backend.ai_common.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 05:10:14.000000 backend.ai-common-23.3.1/backend.ai_common.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      504 2023-05-04 05:10:14.000000 backend.ai-common-23.3.1/backend.ai_common.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        3 2023-05-04 05:10:14.000000 backend.ai-common-23.3.1/backend.ai_common.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      626 2023-05-04 05:10:14.000000 backend.ai-common-23.3.1/backend_shim.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-04 05:10:14.430715 backend.ai-common-23.3.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3880 2023-05-04 05:10:14.000000 backend.ai-common-23.3.1/setup.py
```

### Comparing `backend.ai-common-23.3.0a4/PKG-INFO` & `backend.ai-common-23.3.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: backend.ai-common
-Version: 23.3.0a4
+Version: 23.3.1
 Summary: Backend.AI commons library
 Home-page: https://github.com/lablup/backend.ai
 Author: Lablup Inc. and contributors
 License: LGPLv3
 Project-URL: Documentation, https://docs.backend.ai/
 Project-URL: Source, https://github.com/lablup/backend.ai
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Environment :: No Input/Output (Daemon)
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Software Development
-Classifier: Development Status :: 3 - Alpha
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 or later (LGPLv3+)
 Requires-Python: >=3.11,<3.12
 Description-Content-Type: text/markdown
 
 Backend.AI Commons
 ==================
```

### Comparing `backend.ai-common-23.3.0a4/ai/backend/common/argparse.py` & `backend.ai-common-23.3.1/ai/backend/common/argparse.py`

 * *Files identical despite different names*

### Comparing `backend.ai-common-23.3.0a4/ai/backend/common/asyncio.py` & `backend.ai-common-23.3.1/ai/backend/common/asyncio.py`

 * *Files identical despite different names*

### Comparing `backend.ai-common-23.3.0a4/ai/backend/common/bgtask.py` & `backend.ai-common-23.3.1/ai/backend/common/bgtask.py`

 * *Files identical despite different names*

### Comparing `backend.ai-common-23.3.0a4/ai/backend/common/cgroup.py` & `backend.ai-common-23.3.1/ai/backend/common/cgroup.py`

 * *Files identical despite different names*

### Comparing `backend.ai-common-23.3.0a4/ai/backend/common/cli.py` & `backend.ai-common-23.3.1/ai/backend/common/cli.py`

 * *Files identical despite different names*

### Comparing `backend.ai-common-23.3.0a4/ai/backend/common/config.py` & `backend.ai-common-23.3.1/ai/backend/common/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -66,15 +66,17 @@
             toml_paths += [
                 Path.home() / ".config" / "backend.ai" / f"{daemon_name}.toml",
                 Path(f"/etc/backend.ai/{daemon_name}.toml"),
             ]
         else:
             raise ConfigurationError(
                 {
-                    "read_from_file()": f"Unsupported platform for config path auto-discovery: {sys.platform}",
+                    "read_from_file()": (
+                        f"Unsupported platform for config path auto-discovery: {sys.platform}"
+                    ),
                 }
             )
     else:
         toml_paths = [Path(toml_path_from_env)]
     for _path in toml_paths:
         if _path.is_file():
             return _path
```

### Comparing `backend.ai-common-23.3.0a4/ai/backend/common/distributed.py` & `backend.ai-common-23.3.1/ai/backend/common/distributed.py`

 * *Files identical despite different names*

### Comparing `backend.ai-common-23.3.0a4/ai/backend/common/docker.py` & `backend.ai-common-23.3.1/ai/backend/common/docker.py`

 * *Files 1% similar despite different names*

```diff
@@ -78,15 +78,15 @@
         t.Key("ai.backend.kernelspec"): t.ToInt(lte=MAX_KERNELSPEC, gte=MIN_KERNELSPEC),
         t.Key("ai.backend.features"): tx.StringList(delimiter=" "),
         # ai.backend.resource.min.*
         t.Key("ai.backend.base-distro"): t.String(),
         t.Key("ai.backend.runtime-type"): t.String(),
         t.Key("ai.backend.runtime-path"): tx.PurePath(),
         # Optional labels
-        t.Key("ai.backend.role", default="COMPUTE"): t.Enum("COMPUTE", "INFERENCE"),
+        t.Key("ai.backend.role", default="COMPUTE"): t.Enum("COMPUTE", "INFERENCE", "SYSTEM"),
         t.Key("ai.backend.envs.corecount", optional=True): tx.StringList(allow_blank=True),
         t.Key("ai.backend.accelerators", optional=True): tx.StringList(allow_blank=True),
         t.Key("ai.backend.service-ports", optional=True): tx.StringList(allow_blank=True),
     }
 ).allow_extra("*")
 
 inference_image_label_schema = t.Dict(
@@ -171,17 +171,15 @@
             match = re.search(r'service="([^"]+)"', www_auth_header)
             if match:
                 service = match.group(1)
     if ping_status == 200:
         log.debug("docker-registry: {0} -> basic-auth", registry_url)
         return {"auth": basic_auth, "headers": {}}
     elif ping_status == 404:
-        raise RuntimeError(
-            f"Unsupported docker registry: {registry_url}! " "(API v2 not implemented)"
-        )
+        raise RuntimeError(f"Unsupported docker registry: {registry_url}! (API v2 not implemented)")
     elif ping_status == 401:
         params = {
             "scope": scope,
             "offline_token": "true",
             "client_id": "docker",
             "service": service,
         }
@@ -192,15 +190,15 @@
                 token = data.get("token", None)
                 return {
                     "auth": None,
                     "headers": {
                         "Authorization": f"Bearer {token}",
                     },
                 }
-    raise RuntimeError("authentication for docker registry " f"{registry_url} failed")
+    raise RuntimeError(f"authentication for docker registry {registry_url} failed")
 
 
 async def get_known_registries(etcd: AsyncEtcd) -> Mapping[str, yarl.URL]:
     data = await etcd.get_prefix("config/docker/registry/")
     results: MutableMapping[str, yarl.URL] = {}
     for key, value in data.items():
         name = etcd_unquote(key)
```

### Comparing `backend.ai-common-23.3.0a4/ai/backend/common/enum_extension.py` & `backend.ai-common-23.3.1/ai/backend/common/enum_extension.py`

 * *Files identical despite different names*

### Comparing `backend.ai-common-23.3.0a4/ai/backend/common/enum_extension.pyi` & `backend.ai-common-23.3.1/ai/backend/common/enum_extension.pyi`

 * *Files identical despite different names*

### Comparing `backend.ai-common-23.3.0a4/ai/backend/common/etcd.py` & `backend.ai-common-23.3.1/ai/backend/common/etcd.py`

 * *Files identical despite different names*

### Comparing `backend.ai-common-23.3.0a4/ai/backend/common/events.py` & `backend.ai-common-23.3.1/ai/backend/common/events.py`

 * *Files 3% similar despite different names*

```diff
@@ -16,15 +16,14 @@
     Callable,
     ClassVar,
     Coroutine,
     Generic,
     Mapping,
     Optional,
     Protocol,
-    Sequence,
     Type,
     TypedDict,
     TypeVar,
     Union,
     cast,
 )
 
@@ -224,30 +223,33 @@
             pass
         return None
 
 
 @attrs.define(slots=True, frozen=True)
 class KernelCreationEventArgs:
     kernel_id: KernelId = attrs.field()
+    session_id: SessionId = attrs.field()
     reason: str = attrs.field(default="")
     creation_info: Mapping[str, Any] = attrs.field(factory=dict)
 
     def serialize(self) -> tuple:
         return (
             str(self.kernel_id),
+            str(self.session_id),
             self.reason,
             self.creation_info,
         )
 
     @classmethod
     def deserialize(cls, value: tuple):
         return cls(
             kernel_id=KernelId(uuid.UUID(value[0])),
-            reason=value[1],
-            creation_info=value[2],
+            session_id=SessionId(uuid.UUID(value[1])),
+            reason=value[2],
+            creation_info=value[3],
         )
 
 
 class KernelPreparingEvent(KernelCreationEventArgs, AbstractEvent):
     name = "kernel_preparing"
 
 
@@ -292,30 +294,33 @@
 class KernelCancelledEvent(KernelCreationEventArgs, AbstractEvent):
     name = "kernel_cancelled"
 
 
 @attrs.define(slots=True, frozen=True)
 class KernelTerminationEventArgs:
     kernel_id: KernelId = attrs.field()
+    session_id: SessionId = attrs.field()
     reason: KernelLifecycleEventReason = attrs.field(default=KernelLifecycleEventReason.UNKNOWN)
     exit_code: int = attrs.field(default=-1)
 
     def serialize(self) -> tuple:
         return (
             str(self.kernel_id),
+            str(self.session_id),
             self.reason,
             self.exit_code,
         )
 
     @classmethod
     def deserialize(cls, value: tuple):
         return cls(
             KernelId(uuid.UUID(value[0])),
-            value[1],
-            value[2],
+            session_id=SessionId(uuid.UUID(value[1])),
+            reason=value[2],
+            exit_code=value[3],
         )
 
 
 class KernelTerminatingEvent(KernelTerminationEventArgs, AbstractEvent):
     name = "kernel_terminating"
 
 
@@ -440,30 +445,14 @@
         return cls(
             KernelId(uuid.UUID(value[0])),
             value[1],
         )
 
 
 @attrs.define(auto_attribs=True, slots=True)
-class DoSyncKernelStatsEvent(AbstractEvent):
-    name = "do_sync_kernel_stats"
-
-    kernel_ids: Sequence[KernelId] = attrs.field()
-
-    def serialize(self) -> tuple:
-        return ([*map(str, self.kernel_ids)],)
-
-    @classmethod
-    def deserialize(cls, value: tuple):
-        return cls(
-            kernel_ids=tuple(KernelId(uuid.UUID(item)) for item in value[0]),
-        )
-
-
-@attrs.define(auto_attribs=True, slots=True)
 class GenericSessionEventArgs(AbstractEvent):
     session_id: SessionId = attrs.field()
 
     def serialize(self) -> tuple:
         return (str(self.session_id),)
 
     @classmethod
```

### Comparing `backend.ai-common-23.3.0a4/ai/backend/common/exception.py` & `backend.ai-common-23.3.1/ai/backend/common/exception.py`

 * *Files identical despite different names*

### Comparing `backend.ai-common-23.3.0a4/ai/backend/common/files.py` & `backend.ai-common-23.3.1/ai/backend/common/files.py`

 * *Files identical despite different names*

### Comparing `backend.ai-common-23.3.0a4/ai/backend/common/identity.py` & `backend.ai-common-23.3.1/ai/backend/common/identity.py`

 * *Files identical despite different names*

### Comparing `backend.ai-common-23.3.0a4/ai/backend/common/lock.py` & `backend.ai-common-23.3.1/ai/backend/common/lock.py`

 * *Files identical despite different names*

### Comparing `backend.ai-common-23.3.0a4/ai/backend/common/logging.py` & `backend.ai-common-23.3.1/ai/backend/common/logging.py`

 * *Files 0% similar despite different names*

```diff
@@ -51,33 +51,30 @@
 }
 
 logging_config_iv = t.Dict(
     {
         t.Key("level", default="INFO"): loglevel_iv,
         t.Key("pkg-ns", default=default_pkg_ns): t.Mapping(t.String(allow_blank=True), loglevel_iv),
         t.Key("drivers", default=["console"]): t.List(t.Enum("console", "logstash", "file")),
-        t.Key("console", default=None): t.Null
-        | t.Dict(
+        t.Key("console", default=None): t.Null | t.Dict(
             {
                 t.Key("colored", default=None): t.Null | t.Bool,
                 t.Key("format", default="verbose"): logformat_iv,
             }
         ).allow_extra("*"),
-        t.Key("file", default=None): t.Null
-        | t.Dict(
+        t.Key("file", default=None): t.Null | t.Dict(
             {
                 t.Key("path"): tx.Path(type="dir", auto_create=True),
                 t.Key("filename"): t.String,
                 t.Key("backup-count", default=5): t.Int[1:100],
                 t.Key("rotation-size", default="10M"): tx.BinarySize,
                 t.Key("format", default="verbose"): logformat_iv,
             }
         ).allow_extra("*"),
-        t.Key("logstash", default=None): t.Null
-        | t.Dict(
+        t.Key("logstash", default=None): t.Null | t.Dict(
             {
                 t.Key("endpoint"): tx.HostPortPair,
                 t.Key("protocol", default="tcp"): t.Enum("zmq.push", "zmq.pub", "tcp", "udp"),
                 t.Key("ssl-enabled", default=True): t.Bool,
                 t.Key("ssl-verify", default=True): t.Bool,
                 # NOTE: logstash does not have format option.
             }
```

### Comparing `backend.ai-common-23.3.0a4/ai/backend/common/logging_utils.py` & `backend.ai-common-23.3.1/ai/backend/common/logging_utils.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import logging
+from typing import Any, LiteralString
 
 
 class BraceMessage:
     __slots__ = ("fmt", "args")
 
-    def __init__(self, fmt, args):
+    def __init__(self, fmt: LiteralString, args: tuple[Any, ...]):
         self.fmt = fmt
         self.args = args
 
     def __str__(self):
         return self.fmt.format(*self.args)
```

### Comparing `backend.ai-common-23.3.0a4/ai/backend/common/msgpack.py` & `backend.ai-common-23.3.1/ai/backend/common/msgpack.py`

 * *Files identical despite different names*

### Comparing `backend.ai-common-23.3.0a4/ai/backend/common/networking.py` & `backend.ai-common-23.3.1/ai/backend/common/networking.py`

 * *Files identical despite different names*

### Comparing `backend.ai-common-23.3.0a4/ai/backend/common/plugin/__init__.py` & `backend.ai-common-23.3.1/ai/backend/common/plugin/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -140,15 +140,17 @@
         allowlist: Optional[set] = None,
         blocklist: Optional[set] = None,
     ) -> None:
         if allowlist is not None and blocklist is not None:
             if union := allowlist & blocklist:
                 raise ConfigurationError(
                     {
-                        "plugin.BasePluginContext": f"allowlist and blocklist has union value '{union}'"
+                        "plugin.BasePluginContext": (
+                            f"allowlist and blocklist has union value '{union}'"
+                        )
                     }
                 )
         scanned_plugins = self.discover_plugins(
             self.plugin_group,
             allowlist=allowlist,
             blocklist=blocklist,
         )
```

### Comparing `backend.ai-common-23.3.0a4/ai/backend/common/plugin/hook.py` & `backend.ai-common-23.3.1/ai/backend/common/plugin/hook.py`

 * *Files identical despite different names*

### Comparing `backend.ai-common-23.3.0a4/ai/backend/common/plugin/monitor.py` & `backend.ai-common-23.3.1/ai/backend/common/plugin/monitor.py`

 * *Files identical despite different names*

### Comparing `backend.ai-common-23.3.0a4/ai/backend/common/redis_helper.py` & `backend.ai-common-23.3.1/ai/backend/common/redis_helper.py`

 * *Files 0% similar despite different names*

```diff
@@ -242,15 +242,15 @@
     while True:
         try:
             async with r:
                 if callable(func):
                     aw_or_pipe = func(r)
                 else:
                     raise TypeError(
-                        "The func must be a function or a coroutinefunction " "with no arguments."
+                        "The func must be a function or a coroutinefunction with no arguments."
                     )
                 if isinstance(aw_or_pipe, Pipeline):
                     result = await aw_or_pipe.execute()
                 elif inspect.isawaitable(aw_or_pipe):
                     result = await aw_or_pipe
                 else:
                     raise TypeError(
```

### Comparing `backend.ai-common-23.3.0a4/ai/backend/common/sd_notify.py` & `backend.ai-common-23.3.1/ai/backend/common/sd_notify.py`

 * *Files identical despite different names*

### Comparing `backend.ai-common-23.3.0a4/ai/backend/common/service_ports.py` & `backend.ai-common-23.3.1/ai/backend/common/service_ports.py`

 * *Files 0% similar despite different names*

```diff
@@ -55,22 +55,21 @@
         ports = tuple(map(int, match.group("ports").strip("[]").split(",")))
         for p in ports:
             if p in used_ports:
                 raise exception_cls(f"The port {p} is already used by another service port.")
             if p <= 1024:
                 raise exception_cls(
                     f"The service port number {p} must be "
-                    f"larger than 1024 to run without the root privilege."
+                    "larger than 1024 to run without the root privilege."
                 )
             if p >= 65535:
                 raise exception_cls(f"The service port number {p} must be smaller than 65535.")
             if p in (2000, 2001, 2002, 2003, 2200, 7681):
                 raise exception_cls(
-                    "The service ports 2000 to 2003, 2200 and 7681 "
-                    "are reserved for internal use."
+                    "The service ports 2000 to 2003, 2200 and 7681 are reserved for internal use."
                 )
             used_ports.add(p)
         items.append(
             {
                 "name": name,
                 "protocol": ServicePortProtocols(protocol),
                 "container_ports": ports,
```

### Comparing `backend.ai-common-23.3.0a4/ai/backend/common/testutils.py` & `backend.ai-common-23.3.1/ai/backend/common/testutils.py`

 * *Files identical despite different names*

### Comparing `backend.ai-common-23.3.0a4/ai/backend/common/types.py` & `backend.ai-common-23.3.1/ai/backend/common/types.py`

 * *Files identical despite different names*

### Comparing `backend.ai-common-23.3.0a4/ai/backend/common/utils.py` & `backend.ai-common-23.3.1/ai/backend/common/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -86,17 +86,18 @@
 
     Note that X ( = the minimum distance d x the number of points N) must be equivalent to or smaller than
     the length L + d to guarantee the the minimum distance between the points.
     If X == L + d, the points are always equally spaced with d.
 
     :return: An iterator over the generated sequence
     """
-    assert (
-        num_points * min_distance <= length + min_distance
-    ), "There are too many points or it has a too large distance which cannot be fit into the given length."
+    assert num_points * min_distance <= length + min_distance, (
+        "There are too many points or it has a too large distance which cannot be fit into the"
+        " given length."
+    )
     extra = length - (num_points - 1) * min_distance
     ro = [random.uniform(0, 1) for _ in range(num_points + 1)]
     sum_ro = sum(ro)
     rn = [extra * r / sum_ro for r in ro[0:num_points]]
     spacing = [min_distance + rn[i] for i in range(num_points)]
     cumulative_sum = 0.0
     for s in spacing:
```

### Comparing `backend.ai-common-23.3.0a4/ai/backend/common/validators.py` & `backend.ai-common-23.3.1/ai/backend/common/validators.py`

 * *Files identical despite different names*

### Comparing `backend.ai-common-23.3.0a4/ai/backend/common/web/session/__init__.py` & `backend.ai-common-23.3.1/ai/backend/common/web/session/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -150,32 +150,30 @@
 
 
 async def get_session(request: web.Request) -> Session:
     session = request.get(SESSION_KEY)
     if session is None:
         storage = request.get(STORAGE_KEY)
         if storage is None:
-            raise RuntimeError(
-                "Install aiohttp_session middleware " "in your aiohttp.web.Application"
-            )
+            raise RuntimeError("Install aiohttp_session middleware in your aiohttp.web.Application")
 
         session = await storage.load_session(request)
         if not isinstance(session, Session):
             raise RuntimeError(
                 "Installed {!r} storage should return session instance "
                 "on .load_session() call, got {!r}.".format(storage, session)
             )
         request[SESSION_KEY] = session
     return session
 
 
 async def new_session(request: web.Request) -> Session:
     storage = request.get(STORAGE_KEY)
     if storage is None:
-        raise RuntimeError("Install aiohttp_session middleware " "in your aiohttp.web.Application")
+        raise RuntimeError("Install aiohttp_session middleware in your aiohttp.web.Application")
 
     session = await storage.new_session()
     if not isinstance(session, Session):
         raise RuntimeError(
             "Installed {!r} storage should return session instance "
             "on .load_session() call, got {!r}.".format(storage, session)
         )
```

### Comparing `backend.ai-common-23.3.0a4/ai/backend/common/web/session/redis_storage.py` & `backend.ai-common-23.3.1/ai/backend/common/web/session/redis_storage.py`

 * *Files identical despite different names*

### Comparing `backend.ai-common-23.3.0a4/backend.ai_common.egg-info/PKG-INFO` & `backend.ai-common-23.3.1/backend.ai_common.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: backend.ai-common
-Version: 23.3.0a4
+Version: 23.3.1
 Summary: Backend.AI commons library
 Home-page: https://github.com/lablup/backend.ai
 Author: Lablup Inc. and contributors
 License: LGPLv3
 Project-URL: Documentation, https://docs.backend.ai/
 Project-URL: Source, https://github.com/lablup/backend.ai
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Environment :: No Input/Output (Daemon)
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Software Development
-Classifier: Development Status :: 3 - Alpha
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 or later (LGPLv3+)
 Requires-Python: >=3.11,<3.12
 Description-Content-Type: text/markdown
 
 Backend.AI Commons
 ==================
```

### Comparing `backend.ai-common-23.3.0a4/backend.ai_common.egg-info/SOURCES.txt` & `backend.ai-common-23.3.1/backend.ai_common.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -20,14 +20,15 @@
 ai/backend/common/files.py
 ai/backend/common/identity.py
 ai/backend/common/json.py
 ai/backend/common/lock.py
 ai/backend/common/logging.py
 ai/backend/common/logging_utils.py
 ai/backend/common/msgpack.py
+ai/backend/common/netns.py
 ai/backend/common/networking.py
 ai/backend/common/py.typed
 ai/backend/common/redis_helper.py
 ai/backend/common/sd_notify.py
 ai/backend/common/service_ports.py
 ai/backend/common/testutils.py
 ai/backend/common/types.py
```

### Comparing `backend.ai-common-23.3.0a4/backend_shim.py` & `backend.ai-common-23.3.1/backend_shim.py`

 * *Files identical despite different names*

### Comparing `backend.ai-common-23.3.0a4/setup.py` & `backend.ai-common-23.3.1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,34 +11,34 @@
         'Operating System :: MacOS :: MacOS X',
         'Operating System :: POSIX :: Linux',
         'Programming Language :: Python',
         'Programming Language :: Python :: 3',
         'Environment :: No Input/Output (Daemon)',
         'Topic :: Scientific/Engineering',
         'Topic :: Software Development',
-        'Development Status :: 3 - Alpha',
+        'Development Status :: 5 - Production/Stable',
         'License :: OSI Approved :: GNU Lesser General Public License v3 or later (LGPLv3+)',
     ],
     'description': 'Backend.AI commons library',
     'install_requires': (
         'PyJWT~=2.0',
         'aiodns>=3.0',
         'aiohttp_sse>=2.0',
         'aiohttp~=3.8.1',
-        'aiomonitor-ng~=0.7.0',
-        'aiotools~=1.5.9',
+        'aiomonitor-ng~=0.7.2',
+        'aiotools~=1.6.1',
         'async_timeout~=4.0',
         'asynctest>=0.13.0',
         'asyncudp>=0.4',
         'attrs>=20.3',
-        """backend.ai-plugin==23.03.0a4
+        """backend.ai-plugin==23.03.1
 """,
         'click>=7.1.2',
         'coloredlogs~=15.0',
-        'etcetra==0.1.14',
+        'etcetra==0.1.15',
         'ifaddr~=0.2',
         'janus~=1.0.0',
         'msgpack>=1.0.5rc1',
         'multidict>=6.0',
         'packaging>=21.3',
         'python-dateutil>=2.8',
         'python-json-logger>=2.0.1',
@@ -115,11 +115,11 @@
     ),
     'project_urls': {
         'Documentation': 'https://docs.backend.ai/',
         'Source': 'https://github.com/lablup/backend.ai',
     },
     'python_requires': '>=3.11,<3.12',
     'url': 'https://github.com/lablup/backend.ai',
-    'version': """23.03.0a4
+    'version': """23.03.1
 """,
     'zip_safe': False,
 })
```

