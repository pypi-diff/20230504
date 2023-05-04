# Comparing `tmp/fc-client-0.5.0.tar.gz` & `tmp/fc-client-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/fc-client-0.5.0.tar", last modified: Thu May  4 03:24:11 2023, max compression
+gzip compressed data, was "dist/fc-client-0.5.1.tar", last modified: Thu May  4 06:09:39 2023, max compression
```

## Comparing `fc-client-0.5.0.tar` & `fc-client-0.5.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxr-x   0 shubuntu1  (1000) shubuntu1  (1000)        0 2023-05-04 03:24:11.000000 fc-client-0.5.0/
-drwxrwxr-x   0 shubuntu1  (1000) shubuntu1  (1000)        0 2023-05-04 03:24:11.000000 fc-client-0.5.0/fc_client.egg-info/
--rw-rw-r--   0 shubuntu1  (1000) shubuntu1  (1000)       35 2023-05-04 03:24:11.000000 fc-client-0.5.0/fc_client.egg-info/requires.txt
--rw-rw-r--   0 shubuntu1  (1000) shubuntu1  (1000)        1 2023-05-04 03:24:11.000000 fc-client-0.5.0/fc_client.egg-info/dependency_links.txt
--rw-rw-r--   0 shubuntu1  (1000) shubuntu1  (1000)      318 2023-05-04 03:24:11.000000 fc-client-0.5.0/fc_client.egg-info/SOURCES.txt
--rw-rw-r--   0 shubuntu1  (1000) shubuntu1  (1000)      715 2023-05-04 03:24:11.000000 fc-client-0.5.0/fc_client.egg-info/PKG-INFO
--rw-rw-r--   0 shubuntu1  (1000) shubuntu1  (1000)       53 2023-05-04 03:24:11.000000 fc-client-0.5.0/fc_client.egg-info/entry_points.txt
--rw-rw-r--   0 shubuntu1  (1000) shubuntu1  (1000)       20 2023-05-04 03:24:11.000000 fc-client-0.5.0/fc_client.egg-info/top_level.txt
--rw-rw-r--   0 shubuntu1  (1000) shubuntu1  (1000)     2535 2023-04-10 02:26:18.000000 fc-client-0.5.0/README.rst
--rw-rw-r--   0 shubuntu1  (1000) shubuntu1  (1000)      614 2023-05-04 03:24:11.000000 fc-client-0.5.0/setup.cfg
-drwxrwxr-x   0 shubuntu1  (1000) shubuntu1  (1000)        0 2023-05-04 03:24:11.000000 fc-client-0.5.0/fc_client/
--rw-rw-r--   0 shubuntu1  (1000) shubuntu1  (1000)     7005 2023-05-04 03:23:04.000000 fc-client-0.5.0/fc_client/client.py
--rw-rw-r--   0 shubuntu1  (1000) shubuntu1  (1000)     1071 2023-04-10 02:26:18.000000 fc-client-0.5.0/LICENSE
-drwxrwxr-x   0 shubuntu1  (1000) shubuntu1  (1000)        0 2023-05-04 03:24:11.000000 fc-client-0.5.0/fc_common/
--rw-rw-r--   0 shubuntu1  (1000) shubuntu1  (1000)        6 2023-05-04 03:23:04.000000 fc-client-0.5.0/fc_common/VERSION
--rw-rw-r--   0 shubuntu1  (1000) shubuntu1  (1000)      482 2023-05-04 03:23:04.000000 fc-client-0.5.0/fc_common/__init__.py
--rw-rw-r--   0 shubuntu1  (1000) shubuntu1  (1000)      712 2023-05-04 03:23:04.000000 fc-client-0.5.0/fc_common/version.py
--rw-rw-r--   0 shubuntu1  (1000) shubuntu1  (1000)     2642 2023-05-04 03:23:04.000000 fc-client-0.5.0/setup.py
--rw-rw-r--   0 shubuntu1  (1000) shubuntu1  (1000)      715 2023-05-04 03:24:11.000000 fc-client-0.5.0/PKG-INFO
+drwxrwxr-x   0 shubuntu1  (1000) shubuntu1  (1000)        0 2023-05-04 06:09:39.000000 fc-client-0.5.1/
+drwxrwxr-x   0 shubuntu1  (1000) shubuntu1  (1000)        0 2023-05-04 06:09:39.000000 fc-client-0.5.1/fc_client.egg-info/
+-rw-rw-r--   0 shubuntu1  (1000) shubuntu1  (1000)       35 2023-05-04 06:09:39.000000 fc-client-0.5.1/fc_client.egg-info/requires.txt
+-rw-rw-r--   0 shubuntu1  (1000) shubuntu1  (1000)        1 2023-05-04 06:09:39.000000 fc-client-0.5.1/fc_client.egg-info/dependency_links.txt
+-rw-rw-r--   0 shubuntu1  (1000) shubuntu1  (1000)      318 2023-05-04 06:09:39.000000 fc-client-0.5.1/fc_client.egg-info/SOURCES.txt
+-rw-rw-r--   0 shubuntu1  (1000) shubuntu1  (1000)      715 2023-05-04 06:09:39.000000 fc-client-0.5.1/fc_client.egg-info/PKG-INFO
+-rw-rw-r--   0 shubuntu1  (1000) shubuntu1  (1000)       53 2023-05-04 06:09:39.000000 fc-client-0.5.1/fc_client.egg-info/entry_points.txt
+-rw-rw-r--   0 shubuntu1  (1000) shubuntu1  (1000)       20 2023-05-04 06:09:39.000000 fc-client-0.5.1/fc_client.egg-info/top_level.txt
+-rw-rw-r--   0 shubuntu1  (1000) shubuntu1  (1000)     2535 2023-04-10 02:26:18.000000 fc-client-0.5.1/README.rst
+-rw-rw-r--   0 shubuntu1  (1000) shubuntu1  (1000)      614 2023-05-04 06:09:39.000000 fc-client-0.5.1/setup.cfg
+drwxrwxr-x   0 shubuntu1  (1000) shubuntu1  (1000)        0 2023-05-04 06:09:39.000000 fc-client-0.5.1/fc_client/
+-rw-rw-r--   0 shubuntu1  (1000) shubuntu1  (1000)     7005 2023-05-04 03:23:04.000000 fc-client-0.5.1/fc_client/client.py
+-rw-rw-r--   0 shubuntu1  (1000) shubuntu1  (1000)     1071 2023-04-10 02:26:18.000000 fc-client-0.5.1/LICENSE
+drwxrwxr-x   0 shubuntu1  (1000) shubuntu1  (1000)        0 2023-05-04 06:09:39.000000 fc-client-0.5.1/fc_common/
+-rw-rw-r--   0 shubuntu1  (1000) shubuntu1  (1000)        6 2023-05-04 06:09:15.000000 fc-client-0.5.1/fc_common/VERSION
+-rw-rw-r--   0 shubuntu1  (1000) shubuntu1  (1000)      482 2023-05-04 03:23:04.000000 fc-client-0.5.1/fc_common/__init__.py
+-rw-rw-r--   0 shubuntu1  (1000) shubuntu1  (1000)      712 2023-05-04 03:23:04.000000 fc-client-0.5.1/fc_common/version.py
+-rw-rw-r--   0 shubuntu1  (1000) shubuntu1  (1000)     2642 2023-05-04 06:09:15.000000 fc-client-0.5.1/setup.py
+-rw-rw-r--   0 shubuntu1  (1000) shubuntu1  (1000)      715 2023-05-04 06:09:39.000000 fc-client-0.5.1/PKG-INFO
```

### Comparing `fc-client-0.5.0/fc_client.egg-info/PKG-INFO` & `fc-client-0.5.1/fc_client.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fc-client
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

### Comparing `fc-client-0.5.0/README.rst` & `fc-client-0.5.1/README.rst`

 * *Files identical despite different names*

### Comparing `fc-client-0.5.0/setup.cfg` & `fc-client-0.5.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `fc-client-0.5.0/fc_client/client.py` & `fc-client-0.5.1/fc_client/client.py`

 * *Files identical despite different names*

### Comparing `fc-client-0.5.0/LICENSE` & `fc-client-0.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `fc-client-0.5.0/fc_common/version.py` & `fc-client-0.5.1/fc_common/version.py`

 * *Files identical despite different names*

### Comparing `fc-client-0.5.0/setup.py` & `fc-client-0.5.1/setup.py`

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

### Comparing `fc-client-0.5.0/PKG-INFO` & `fc-client-0.5.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fc-client
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

