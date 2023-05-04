# Comparing `tmp/fc-guarder-0.5.0.tar.gz` & `tmp/fc-guarder-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/fc-guarder-0.5.0.tar", last modified: Thu May  4 03:24:10 2023, max compression
+gzip compressed data, was "dist/fc-guarder-0.5.1.tar", last modified: Thu May  4 06:09:39 2023, max compression
```

## Comparing `fc-guarder-0.5.0.tar` & `fc-guarder-0.5.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 shubuntu1  (1000) shubuntu1  (1000)        0 2023-05-04 03:24:10.000000 fc-guarder-0.5.0/
--rw-rw-r--   0 shubuntu1  (1000) shubuntu1  (1000)     2535 2023-04-10 02:26:18.000000 fc-guarder-0.5.0/README.rst
-drwxrwxr-x   0 shubuntu1  (1000) shubuntu1  (1000)        0 2023-05-04 03:24:10.000000 fc-guarder-0.5.0/fc_guarder/
--rw-rw-r--   0 shubuntu1  (1000) shubuntu1  (1000)     1928 2023-05-04 03:23:04.000000 fc-guarder-0.5.0/fc_guarder/guarder.py
--rw-rw-r--   0 shubuntu1  (1000) shubuntu1  (1000)      614 2023-05-04 03:24:10.000000 fc-guarder-0.5.0/setup.cfg
-drwxrwxr-x   0 shubuntu1  (1000) shubuntu1  (1000)        0 2023-05-04 03:24:10.000000 fc-guarder-0.5.0/fc_guarder.egg-info/
--rw-rw-r--   0 shubuntu1  (1000) shubuntu1  (1000)       17 2023-05-04 03:24:10.000000 fc-guarder-0.5.0/fc_guarder.egg-info/requires.txt
--rw-rw-r--   0 shubuntu1  (1000) shubuntu1  (1000)        1 2023-05-04 03:24:10.000000 fc-guarder-0.5.0/fc_guarder.egg-info/dependency_links.txt
--rw-rw-r--   0 shubuntu1  (1000) shubuntu1  (1000)      265 2023-05-04 03:24:10.000000 fc-guarder-0.5.0/fc_guarder.egg-info/SOURCES.txt
--rw-rw-r--   0 shubuntu1  (1000) shubuntu1  (1000)      716 2023-05-04 03:24:10.000000 fc-guarder-0.5.0/fc_guarder.egg-info/PKG-INFO
--rw-rw-r--   0 shubuntu1  (1000) shubuntu1  (1000)       56 2023-05-04 03:24:10.000000 fc-guarder-0.5.0/fc_guarder.egg-info/entry_points.txt
--rw-rw-r--   0 shubuntu1  (1000) shubuntu1  (1000)       11 2023-05-04 03:24:10.000000 fc-guarder-0.5.0/fc_guarder.egg-info/top_level.txt
--rw-rw-r--   0 shubuntu1  (1000) shubuntu1  (1000)     1071 2023-04-10 02:26:18.000000 fc-guarder-0.5.0/LICENSE
--rw-rw-r--   0 shubuntu1  (1000) shubuntu1  (1000)     2642 2023-05-04 03:23:04.000000 fc-guarder-0.5.0/setup.py
--rw-rw-r--   0 shubuntu1  (1000) shubuntu1  (1000)      716 2023-05-04 03:24:10.000000 fc-guarder-0.5.0/PKG-INFO
+drwxrwxr-x   0 shubuntu1  (1000) shubuntu1  (1000)        0 2023-05-04 06:09:39.000000 fc-guarder-0.5.1/
+-rw-rw-r--   0 shubuntu1  (1000) shubuntu1  (1000)     2535 2023-04-10 02:26:18.000000 fc-guarder-0.5.1/README.rst
+drwxrwxr-x   0 shubuntu1  (1000) shubuntu1  (1000)        0 2023-05-04 06:09:39.000000 fc-guarder-0.5.1/fc_guarder/
+-rw-rw-r--   0 shubuntu1  (1000) shubuntu1  (1000)     1928 2023-05-04 03:23:04.000000 fc-guarder-0.5.1/fc_guarder/guarder.py
+-rw-rw-r--   0 shubuntu1  (1000) shubuntu1  (1000)      614 2023-05-04 06:09:39.000000 fc-guarder-0.5.1/setup.cfg
+drwxrwxr-x   0 shubuntu1  (1000) shubuntu1  (1000)        0 2023-05-04 06:09:39.000000 fc-guarder-0.5.1/fc_guarder.egg-info/
+-rw-rw-r--   0 shubuntu1  (1000) shubuntu1  (1000)       17 2023-05-04 06:09:39.000000 fc-guarder-0.5.1/fc_guarder.egg-info/requires.txt
+-rw-rw-r--   0 shubuntu1  (1000) shubuntu1  (1000)        1 2023-05-04 06:09:39.000000 fc-guarder-0.5.1/fc_guarder.egg-info/dependency_links.txt
+-rw-rw-r--   0 shubuntu1  (1000) shubuntu1  (1000)      265 2023-05-04 06:09:39.000000 fc-guarder-0.5.1/fc_guarder.egg-info/SOURCES.txt
+-rw-rw-r--   0 shubuntu1  (1000) shubuntu1  (1000)      716 2023-05-04 06:09:39.000000 fc-guarder-0.5.1/fc_guarder.egg-info/PKG-INFO
+-rw-rw-r--   0 shubuntu1  (1000) shubuntu1  (1000)       56 2023-05-04 06:09:39.000000 fc-guarder-0.5.1/fc_guarder.egg-info/entry_points.txt
+-rw-rw-r--   0 shubuntu1  (1000) shubuntu1  (1000)       11 2023-05-04 06:09:39.000000 fc-guarder-0.5.1/fc_guarder.egg-info/top_level.txt
+-rw-rw-r--   0 shubuntu1  (1000) shubuntu1  (1000)     1071 2023-04-10 02:26:18.000000 fc-guarder-0.5.1/LICENSE
+-rw-rw-r--   0 shubuntu1  (1000) shubuntu1  (1000)     2642 2023-05-04 06:09:15.000000 fc-guarder-0.5.1/setup.py
+-rw-rw-r--   0 shubuntu1  (1000) shubuntu1  (1000)      716 2023-05-04 06:09:39.000000 fc-guarder-0.5.1/PKG-INFO
```

### Comparing `fc-guarder-0.5.0/README.rst` & `fc-guarder-0.5.1/README.rst`

 * *Files identical despite different names*

### Comparing `fc-guarder-0.5.0/fc_guarder/guarder.py` & `fc-guarder-0.5.1/fc_guarder/guarder.py`

 * *Files identical despite different names*

### Comparing `fc-guarder-0.5.0/setup.cfg` & `fc-guarder-0.5.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `fc-guarder-0.5.0/fc_guarder.egg-info/PKG-INFO` & `fc-guarder-0.5.1/fc_guarder.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fc-guarder
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

### Comparing `fc-guarder-0.5.0/LICENSE` & `fc-guarder-0.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `fc-guarder-0.5.0/setup.py` & `fc-guarder-0.5.1/setup.py`

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

### Comparing `fc-guarder-0.5.0/PKG-INFO` & `fc-guarder-0.5.1/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fc-guarder
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

