# Comparing `tmp/fc-server-0.5.0.tar.gz` & `tmp/fc-server-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/fc-server-0.5.0.tar", last modified: Thu May  4 03:24:10 2023, max compression
+gzip compressed data, was "dist/fc-server-0.5.1.tar", last modified: Thu May  4 06:09:39 2023, max compression
```

## Comparing `fc-server-0.5.0.tar` & `fc-server-0.5.1.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxrwxr-x   0 shubuntu1  (1000) shubuntu1  (1000)        0 2023-05-04 03:24:10.000000 fc-server-0.5.0/
--rw-rw-r--   0 shubuntu1  (1000) shubuntu1  (1000)     2535 2023-04-10 02:26:18.000000 fc-server-0.5.0/README.rst
--rw-rw-r--   0 shubuntu1  (1000) shubuntu1  (1000)      614 2023-05-04 03:24:10.000000 fc-server-0.5.0/setup.cfg
-drwxrwxr-x   0 shubuntu1  (1000) shubuntu1  (1000)        0 2023-05-04 03:24:10.000000 fc-server-0.5.0/fc_server.egg-info/
--rw-rw-r--   0 shubuntu1  (1000) shubuntu1  (1000)      109 2023-05-04 03:24:09.000000 fc-server-0.5.0/fc_server.egg-info/requires.txt
--rw-rw-r--   0 shubuntu1  (1000) shubuntu1  (1000)        1 2023-05-04 03:24:09.000000 fc-server-0.5.0/fc_server.egg-info/dependency_links.txt
--rw-rw-r--   0 shubuntu1  (1000) shubuntu1  (1000)      897 2023-05-04 03:24:09.000000 fc-server-0.5.0/fc_server.egg-info/SOURCES.txt
--rw-rw-r--   0 shubuntu1  (1000) shubuntu1  (1000)      715 2023-05-04 03:24:09.000000 fc-server-0.5.0/fc_server.egg-info/PKG-INFO
--rw-rw-r--   0 shubuntu1  (1000) shubuntu1  (1000)       53 2023-05-04 03:24:09.000000 fc-server-0.5.0/fc_server.egg-info/entry_points.txt
--rw-rw-r--   0 shubuntu1  (1000) shubuntu1  (1000)       20 2023-05-04 03:24:09.000000 fc-server-0.5.0/fc_server.egg-info/top_level.txt
--rw-rw-r--   0 shubuntu1  (1000) shubuntu1  (1000)     1071 2023-04-10 02:26:18.000000 fc-server-0.5.0/LICENSE
-drwxrwxr-x   0 shubuntu1  (1000) shubuntu1  (1000)        0 2023-05-04 03:24:10.000000 fc-server-0.5.0/fc_server/
-drwxrwxr-x   0 shubuntu1  (1000) shubuntu1  (1000)        0 2023-05-04 03:24:10.000000 fc-server-0.5.0/fc_server/config/
--rw-rw-r--   0 shubuntu1  (1000) shubuntu1  (1000)       82 2023-04-10 02:26:18.000000 fc-server-0.5.0/fc_server/config/sample_lavacli.yaml
--rw-rw-r--   0 shubuntu1  (1000) shubuntu1  (1000)      357 2023-04-10 02:26:18.000000 fc-server-0.5.0/fc_server/config/sample_cfg.yaml
-drwxrwxr-x   0 shubuntu1  (1000) shubuntu1  (1000)        0 2023-05-04 03:24:10.000000 fc-server-0.5.0/fc_server/plugins/
-drwxrwxr-x   0 shubuntu1  (1000) shubuntu1  (1000)        0 2023-05-04 03:24:10.000000 fc-server-0.5.0/fc_server/plugins/utils/
--rw-rw-r--   0 shubuntu1  (1000) shubuntu1  (1000)     2359 2023-05-04 03:23:04.000000 fc-server-0.5.0/fc_server/plugins/utils/labgrid.py
--rw-rw-r--   0 shubuntu1  (1000) shubuntu1  (1000)     5185 2023-05-04 03:23:04.000000 fc-server-0.5.0/fc_server/plugins/utils/lava.py
--rw-rw-r--   0 shubuntu1  (1000) shubuntu1  (1000)        0 2023-04-10 02:26:18.000000 fc-server-0.5.0/fc_server/plugins/utils/__init__.py
--rw-rw-r--   0 shubuntu1  (1000) shubuntu1  (1000)     7526 2023-05-04 03:23:04.000000 fc-server-0.5.0/fc_server/plugins/labgrid.py
--rw-rw-r--   0 shubuntu1  (1000) shubuntu1  (1000)    17626 2023-05-04 03:23:04.000000 fc-server-0.5.0/fc_server/plugins/lava.py
--rw-rw-r--   0 shubuntu1  (1000) shubuntu1  (1000)        0 2023-04-10 02:26:18.000000 fc-server-0.5.0/fc_server/plugins/__init__.py
-drwxrwxr-x   0 shubuntu1  (1000) shubuntu1  (1000)        0 2023-05-04 03:24:10.000000 fc-server-0.5.0/fc_server/core/
--rw-rw-r--   0 shubuntu1  (1000) shubuntu1  (1000)      681 2023-05-04 03:23:04.000000 fc-server-0.5.0/fc_server/core/logger.py
--rw-rw-r--   0 shubuntu1  (1000) shubuntu1  (1000)    11568 2023-05-04 03:23:04.000000 fc-server-0.5.0/fc_server/core/coordinator.py
--rw-rw-r--   0 shubuntu1  (1000) shubuntu1  (1000)     6024 2023-05-04 03:23:04.000000 fc-server-0.5.0/fc_server/core/api_svr.py
--rw-rw-r--   0 shubuntu1  (1000) shubuntu1  (1000)     1951 2023-05-04 03:23:04.000000 fc-server-0.5.0/fc_server/core/decorators.py
--rw-rw-r--   0 shubuntu1  (1000) shubuntu1  (1000)      929 2023-05-04 03:23:04.000000 fc-server-0.5.0/fc_server/core/__init__.py
--rw-rw-r--   0 shubuntu1  (1000) shubuntu1  (1000)      623 2023-05-04 03:23:04.000000 fc-server-0.5.0/fc_server/core/plugin.py
--rw-rw-r--   0 shubuntu1  (1000) shubuntu1  (1000)     2828 2023-05-04 03:23:04.000000 fc-server-0.5.0/fc_server/core/config.py
--rw-rw-r--   0 shubuntu1  (1000) shubuntu1  (1000)     1071 2023-05-04 03:23:04.000000 fc-server-0.5.0/fc_server/server.py
--rw-rw-r--   0 shubuntu1  (1000) shubuntu1  (1000)        0 2023-04-10 02:26:18.000000 fc-server-0.5.0/fc_server/__init__.py
-drwxrwxr-x   0 shubuntu1  (1000) shubuntu1  (1000)        0 2023-05-04 03:24:10.000000 fc-server-0.5.0/fc_server/management/
--rw-rw-r--   0 shubuntu1  (1000) shubuntu1  (1000)      212 2023-05-04 03:23:04.000000 fc-server-0.5.0/fc_server/management/common.py
--rw-rw-r--   0 shubuntu1  (1000) shubuntu1  (1000)        0 2023-04-10 02:26:18.000000 fc-server-0.5.0/fc_server/management/__init__.py
--rw-rw-r--   0 shubuntu1  (1000) shubuntu1  (1000)     2498 2023-05-04 03:23:04.000000 fc-server-0.5.0/fc_server/management/cmd_online_lava_devices.py
-drwxrwxr-x   0 shubuntu1  (1000) shubuntu1  (1000)        0 2023-05-04 03:24:10.000000 fc-server-0.5.0/fc_common/
--rw-rw-r--   0 shubuntu1  (1000) shubuntu1  (1000)        6 2023-05-04 03:23:04.000000 fc-server-0.5.0/fc_common/VERSION
--rw-rw-r--   0 shubuntu1  (1000) shubuntu1  (1000)      482 2023-05-04 03:23:04.000000 fc-server-0.5.0/fc_common/__init__.py
--rw-rw-r--   0 shubuntu1  (1000) shubuntu1  (1000)      712 2023-05-04 03:23:04.000000 fc-server-0.5.0/fc_common/version.py
--rw-rw-r--   0 shubuntu1  (1000) shubuntu1  (1000)     2642 2023-05-04 03:23:04.000000 fc-server-0.5.0/setup.py
--rw-rw-r--   0 shubuntu1  (1000) shubuntu1  (1000)      715 2023-05-04 03:24:10.000000 fc-server-0.5.0/PKG-INFO
+drwxrwxr-x   0 shubuntu1  (1000) shubuntu1  (1000)        0 2023-05-04 06:09:39.000000 fc-server-0.5.1/
+-rw-rw-r--   0 shubuntu1  (1000) shubuntu1  (1000)     2535 2023-04-10 02:26:18.000000 fc-server-0.5.1/README.rst
+-rw-rw-r--   0 shubuntu1  (1000) shubuntu1  (1000)      614 2023-05-04 06:09:39.000000 fc-server-0.5.1/setup.cfg
+drwxrwxr-x   0 shubuntu1  (1000) shubuntu1  (1000)        0 2023-05-04 06:09:39.000000 fc-server-0.5.1/fc_server.egg-info/
+-rw-rw-r--   0 shubuntu1  (1000) shubuntu1  (1000)      109 2023-05-04 06:09:38.000000 fc-server-0.5.1/fc_server.egg-info/requires.txt
+-rw-rw-r--   0 shubuntu1  (1000) shubuntu1  (1000)        1 2023-05-04 06:09:38.000000 fc-server-0.5.1/fc_server.egg-info/dependency_links.txt
+-rw-rw-r--   0 shubuntu1  (1000) shubuntu1  (1000)      897 2023-05-04 06:09:38.000000 fc-server-0.5.1/fc_server.egg-info/SOURCES.txt
+-rw-rw-r--   0 shubuntu1  (1000) shubuntu1  (1000)      715 2023-05-04 06:09:38.000000 fc-server-0.5.1/fc_server.egg-info/PKG-INFO
+-rw-rw-r--   0 shubuntu1  (1000) shubuntu1  (1000)       53 2023-05-04 06:09:38.000000 fc-server-0.5.1/fc_server.egg-info/entry_points.txt
+-rw-rw-r--   0 shubuntu1  (1000) shubuntu1  (1000)       20 2023-05-04 06:09:38.000000 fc-server-0.5.1/fc_server.egg-info/top_level.txt
+-rw-rw-r--   0 shubuntu1  (1000) shubuntu1  (1000)     1071 2023-04-10 02:26:18.000000 fc-server-0.5.1/LICENSE
+drwxrwxr-x   0 shubuntu1  (1000) shubuntu1  (1000)        0 2023-05-04 06:09:39.000000 fc-server-0.5.1/fc_server/
+drwxrwxr-x   0 shubuntu1  (1000) shubuntu1  (1000)        0 2023-05-04 06:09:39.000000 fc-server-0.5.1/fc_server/config/
+-rw-rw-r--   0 shubuntu1  (1000) shubuntu1  (1000)       82 2023-04-10 02:26:18.000000 fc-server-0.5.1/fc_server/config/sample_lavacli.yaml
+-rw-rw-r--   0 shubuntu1  (1000) shubuntu1  (1000)      357 2023-04-10 02:26:18.000000 fc-server-0.5.1/fc_server/config/sample_cfg.yaml
+drwxrwxr-x   0 shubuntu1  (1000) shubuntu1  (1000)        0 2023-05-04 06:09:39.000000 fc-server-0.5.1/fc_server/plugins/
+drwxrwxr-x   0 shubuntu1  (1000) shubuntu1  (1000)        0 2023-05-04 06:09:39.000000 fc-server-0.5.1/fc_server/plugins/utils/
+-rw-rw-r--   0 shubuntu1  (1000) shubuntu1  (1000)     2359 2023-05-04 03:23:04.000000 fc-server-0.5.1/fc_server/plugins/utils/labgrid.py
+-rw-rw-r--   0 shubuntu1  (1000) shubuntu1  (1000)     5185 2023-05-04 03:23:04.000000 fc-server-0.5.1/fc_server/plugins/utils/lava.py
+-rw-rw-r--   0 shubuntu1  (1000) shubuntu1  (1000)        0 2023-04-10 02:26:18.000000 fc-server-0.5.1/fc_server/plugins/utils/__init__.py
+-rw-rw-r--   0 shubuntu1  (1000) shubuntu1  (1000)     7526 2023-05-04 03:23:04.000000 fc-server-0.5.1/fc_server/plugins/labgrid.py
+-rw-rw-r--   0 shubuntu1  (1000) shubuntu1  (1000)    17626 2023-05-04 03:23:04.000000 fc-server-0.5.1/fc_server/plugins/lava.py
+-rw-rw-r--   0 shubuntu1  (1000) shubuntu1  (1000)        0 2023-04-10 02:26:18.000000 fc-server-0.5.1/fc_server/plugins/__init__.py
+drwxrwxr-x   0 shubuntu1  (1000) shubuntu1  (1000)        0 2023-05-04 06:09:39.000000 fc-server-0.5.1/fc_server/core/
+-rw-rw-r--   0 shubuntu1  (1000) shubuntu1  (1000)      681 2023-05-04 03:23:04.000000 fc-server-0.5.1/fc_server/core/logger.py
+-rw-rw-r--   0 shubuntu1  (1000) shubuntu1  (1000)    11568 2023-05-04 03:23:04.000000 fc-server-0.5.1/fc_server/core/coordinator.py
+-rw-rw-r--   0 shubuntu1  (1000) shubuntu1  (1000)     6024 2023-05-04 03:23:04.000000 fc-server-0.5.1/fc_server/core/api_svr.py
+-rw-rw-r--   0 shubuntu1  (1000) shubuntu1  (1000)     1951 2023-05-04 03:23:04.000000 fc-server-0.5.1/fc_server/core/decorators.py
+-rw-rw-r--   0 shubuntu1  (1000) shubuntu1  (1000)      929 2023-05-04 03:23:04.000000 fc-server-0.5.1/fc_server/core/__init__.py
+-rw-rw-r--   0 shubuntu1  (1000) shubuntu1  (1000)      623 2023-05-04 03:23:04.000000 fc-server-0.5.1/fc_server/core/plugin.py
+-rw-rw-r--   0 shubuntu1  (1000) shubuntu1  (1000)     2828 2023-05-04 03:23:04.000000 fc-server-0.5.1/fc_server/core/config.py
+-rw-rw-r--   0 shubuntu1  (1000) shubuntu1  (1000)     1071 2023-05-04 03:23:04.000000 fc-server-0.5.1/fc_server/server.py
+-rw-rw-r--   0 shubuntu1  (1000) shubuntu1  (1000)        0 2023-04-10 02:26:18.000000 fc-server-0.5.1/fc_server/__init__.py
+drwxrwxr-x   0 shubuntu1  (1000) shubuntu1  (1000)        0 2023-05-04 06:09:39.000000 fc-server-0.5.1/fc_server/management/
+-rw-rw-r--   0 shubuntu1  (1000) shubuntu1  (1000)      212 2023-05-04 03:23:04.000000 fc-server-0.5.1/fc_server/management/common.py
+-rw-rw-r--   0 shubuntu1  (1000) shubuntu1  (1000)        0 2023-04-10 02:26:18.000000 fc-server-0.5.1/fc_server/management/__init__.py
+-rw-rw-r--   0 shubuntu1  (1000) shubuntu1  (1000)     2498 2023-05-04 03:23:04.000000 fc-server-0.5.1/fc_server/management/cmd_online_lava_devices.py
+drwxrwxr-x   0 shubuntu1  (1000) shubuntu1  (1000)        0 2023-05-04 06:09:39.000000 fc-server-0.5.1/fc_common/
+-rw-rw-r--   0 shubuntu1  (1000) shubuntu1  (1000)        6 2023-05-04 06:09:15.000000 fc-server-0.5.1/fc_common/VERSION
+-rw-rw-r--   0 shubuntu1  (1000) shubuntu1  (1000)      482 2023-05-04 03:23:04.000000 fc-server-0.5.1/fc_common/__init__.py
+-rw-rw-r--   0 shubuntu1  (1000) shubuntu1  (1000)      712 2023-05-04 03:23:04.000000 fc-server-0.5.1/fc_common/version.py
+-rw-rw-r--   0 shubuntu1  (1000) shubuntu1  (1000)     2642 2023-05-04 06:09:15.000000 fc-server-0.5.1/setup.py
+-rw-rw-r--   0 shubuntu1  (1000) shubuntu1  (1000)      715 2023-05-04 06:09:39.000000 fc-server-0.5.1/PKG-INFO
```

### Comparing `fc-server-0.5.0/README.rst` & `fc-server-0.5.1/README.rst`

 * *Files identical despite different names*

### Comparing `fc-server-0.5.0/setup.cfg` & `fc-server-0.5.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `fc-server-0.5.0/fc_server.egg-info/SOURCES.txt` & `fc-server-0.5.1/fc_server.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fc-server-0.5.0/fc_server.egg-info/PKG-INFO` & `fc-server-0.5.1/fc_server.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fc-server
-Version: 0.5.0
+Version: 0.5.1
 Summary: UNKNOWN
 Home-page: https://fc.readthedocs.io/
 Author: Larry Shen
 Author-email: larry.shen@nxp.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
```

### Comparing `fc-server-0.5.0/LICENSE` & `fc-server-0.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `fc-server-0.5.0/fc_server/plugins/utils/labgrid.py` & `fc-server-0.5.1/fc_server/plugins/utils/labgrid.py`

 * *Files identical despite different names*

### Comparing `fc-server-0.5.0/fc_server/plugins/utils/lava.py` & `fc-server-0.5.1/fc_server/plugins/utils/lava.py`

 * *Files identical despite different names*

### Comparing `fc-server-0.5.0/fc_server/plugins/labgrid.py` & `fc-server-0.5.1/fc_server/plugins/labgrid.py`

 * *Files identical despite different names*

### Comparing `fc-server-0.5.0/fc_server/plugins/lava.py` & `fc-server-0.5.1/fc_server/plugins/lava.py`

 * *Files identical despite different names*

### Comparing `fc-server-0.5.0/fc_server/core/logger.py` & `fc-server-0.5.1/fc_server/core/logger.py`

 * *Files identical despite different names*

### Comparing `fc-server-0.5.0/fc_server/core/coordinator.py` & `fc-server-0.5.1/fc_server/core/coordinator.py`

 * *Files identical despite different names*

### Comparing `fc-server-0.5.0/fc_server/core/api_svr.py` & `fc-server-0.5.1/fc_server/core/api_svr.py`

 * *Files identical despite different names*

### Comparing `fc-server-0.5.0/fc_server/core/decorators.py` & `fc-server-0.5.1/fc_server/core/decorators.py`

 * *Files identical despite different names*

### Comparing `fc-server-0.5.0/fc_server/core/__init__.py` & `fc-server-0.5.1/fc_server/core/__init__.py`

 * *Files identical despite different names*

### Comparing `fc-server-0.5.0/fc_server/core/plugin.py` & `fc-server-0.5.1/fc_server/core/plugin.py`

 * *Files identical despite different names*

### Comparing `fc-server-0.5.0/fc_server/core/config.py` & `fc-server-0.5.1/fc_server/core/config.py`

 * *Files identical despite different names*

### Comparing `fc-server-0.5.0/fc_server/server.py` & `fc-server-0.5.1/fc_server/server.py`

 * *Files identical despite different names*

### Comparing `fc-server-0.5.0/fc_server/management/cmd_online_lava_devices.py` & `fc-server-0.5.1/fc_server/management/cmd_online_lava_devices.py`

 * *Files identical despite different names*

### Comparing `fc-server-0.5.0/fc_common/version.py` & `fc-server-0.5.1/fc_common/version.py`

 * *Files identical despite different names*

### Comparing `fc-server-0.5.0/setup.py` & `fc-server-0.5.1/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -67,20 +67,20 @@
         },
         entry_points={
             "console_scripts": [
                 "fc-server = fc_server.server:main",
             ]
         },
         install_requires=[
-            "aiohttp==3.7.4.post0",
-            "async-lru==1.0.3",
-            "flatdict==4.0.1",
+            "aiohttp>=3.7.4.post0",
+            "async-lru>=1.0.3",
+            "flatdict>=4.0.1",
             "lavacli==1.2",
             "labgrid==23.0.1",
-            "singledispatchmethod==1.0",
+            "singledispatchmethod>=1.0",
         ],
     )
 elif PKG == "fc-guarder":
     setup(
         **common_setup,
         name="fc-guarder",
         packages=["fc_guarder"],
@@ -101,11 +101,11 @@
         },
         entry_points={
             "console_scripts": [
                 "fc-client = fc_client.client:main",
             ]
         },
         install_requires=[
-            "prettytable==2.2.1",
+            "prettytable>=2.2.1",
             "labgrid==23.0.1",
         ],
     )
```

### Comparing `fc-server-0.5.0/PKG-INFO` & `fc-server-0.5.1/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fc-server
-Version: 0.5.0
+Version: 0.5.1
 Summary: UNKNOWN
 Home-page: https://fc.readthedocs.io/
 Author: Larry Shen
 Author-email: larry.shen@nxp.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
```

