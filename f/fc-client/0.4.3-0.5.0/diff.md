# Comparing `tmp/fc-client-0.4.3.tar.gz` & `tmp/fc-client-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/fc-client-0.4.3.tar", last modified: Wed Mar 22 02:13:30 2023, max compression
+gzip compressed data, was "dist/fc-client-0.5.0.tar", last modified: Thu May  4 03:24:11 2023, max compression
```

## Comparing `fc-client-0.4.3.tar` & `fc-client-0.5.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxr-x   0 shubuntu1  (1000) shubuntu1  (1000)        0 2023-03-22 02:13:30.000000 fc-client-0.4.3/
-drwxrwxr-x   0 shubuntu1  (1000) shubuntu1  (1000)        0 2023-03-22 02:13:30.000000 fc-client-0.4.3/fc_client.egg-info/
--rw-rw-r--   0 shubuntu1  (1000) shubuntu1  (1000)       71 2023-03-22 02:13:30.000000 fc-client-0.4.3/fc_client.egg-info/requires.txt
--rw-rw-r--   0 shubuntu1  (1000) shubuntu1  (1000)        1 2023-03-22 02:13:30.000000 fc-client-0.4.3/fc_client.egg-info/dependency_links.txt
--rw-rw-r--   0 shubuntu1  (1000) shubuntu1  (1000)      318 2023-03-22 02:13:30.000000 fc-client-0.4.3/fc_client.egg-info/SOURCES.txt
--rw-rw-r--   0 shubuntu1  (1000) shubuntu1  (1000)      789 2023-03-22 02:13:30.000000 fc-client-0.4.3/fc_client.egg-info/PKG-INFO
--rw-rw-r--   0 shubuntu1  (1000) shubuntu1  (1000)       53 2023-03-22 02:13:30.000000 fc-client-0.4.3/fc_client.egg-info/entry_points.txt
--rw-rw-r--   0 shubuntu1  (1000) shubuntu1  (1000)       20 2023-03-22 02:13:30.000000 fc-client-0.4.3/fc_client.egg-info/top_level.txt
--rw-rw-r--   0 shubuntu1  (1000) shubuntu1  (1000)     2535 2022-08-17 07:02:28.000000 fc-client-0.4.3/README.rst
--rw-rw-r--   0 shubuntu1  (1000) shubuntu1  (1000)      653 2023-03-22 02:13:30.000000 fc-client-0.4.3/setup.cfg
-drwxrwxr-x   0 shubuntu1  (1000) shubuntu1  (1000)        0 2023-03-22 02:13:30.000000 fc-client-0.4.3/fc_client/
--rw-rw-r--   0 shubuntu1  (1000) shubuntu1  (1000)     7776 2022-03-07 07:28:36.000000 fc-client-0.4.3/fc_client/client.py
--rw-rw-r--   0 shubuntu1  (1000) shubuntu1  (1000)     1071 2022-03-07 07:28:36.000000 fc-client-0.4.3/LICENSE
-drwxrwxr-x   0 shubuntu1  (1000) shubuntu1  (1000)        0 2023-03-22 02:13:30.000000 fc-client-0.4.3/fc_common/
--rw-rw-r--   0 shubuntu1  (1000) shubuntu1  (1000)        6 2023-03-22 02:13:00.000000 fc-client-0.4.3/fc_common/VERSION
--rw-rw-r--   0 shubuntu1  (1000) shubuntu1  (1000)        0 2022-03-07 07:28:36.000000 fc-client-0.4.3/fc_common/__init__.py
--rw-rw-r--   0 shubuntu1  (1000) shubuntu1  (1000)     1759 2022-03-07 07:28:36.000000 fc-client-0.4.3/fc_common/version.py
--rw-rw-r--   0 shubuntu1  (1000) shubuntu1  (1000)     3857 2023-03-22 02:13:00.000000 fc-client-0.4.3/setup.py
--rw-rw-r--   0 shubuntu1  (1000) shubuntu1  (1000)      789 2023-03-22 02:13:30.000000 fc-client-0.4.3/PKG-INFO
+drwxrwxr-x   0 shubuntu1  (1000) shubuntu1  (1000)        0 2023-05-04 03:24:11.000000 fc-client-0.5.0/
+drwxrwxr-x   0 shubuntu1  (1000) shubuntu1  (1000)        0 2023-05-04 03:24:11.000000 fc-client-0.5.0/fc_client.egg-info/
+-rw-rw-r--   0 shubuntu1  (1000) shubuntu1  (1000)       35 2023-05-04 03:24:11.000000 fc-client-0.5.0/fc_client.egg-info/requires.txt
+-rw-rw-r--   0 shubuntu1  (1000) shubuntu1  (1000)        1 2023-05-04 03:24:11.000000 fc-client-0.5.0/fc_client.egg-info/dependency_links.txt
+-rw-rw-r--   0 shubuntu1  (1000) shubuntu1  (1000)      318 2023-05-04 03:24:11.000000 fc-client-0.5.0/fc_client.egg-info/SOURCES.txt
+-rw-rw-r--   0 shubuntu1  (1000) shubuntu1  (1000)      715 2023-05-04 03:24:11.000000 fc-client-0.5.0/fc_client.egg-info/PKG-INFO
+-rw-rw-r--   0 shubuntu1  (1000) shubuntu1  (1000)       53 2023-05-04 03:24:11.000000 fc-client-0.5.0/fc_client.egg-info/entry_points.txt
+-rw-rw-r--   0 shubuntu1  (1000) shubuntu1  (1000)       20 2023-05-04 03:24:11.000000 fc-client-0.5.0/fc_client.egg-info/top_level.txt
+-rw-rw-r--   0 shubuntu1  (1000) shubuntu1  (1000)     2535 2023-04-10 02:26:18.000000 fc-client-0.5.0/README.rst
+-rw-rw-r--   0 shubuntu1  (1000) shubuntu1  (1000)      614 2023-05-04 03:24:11.000000 fc-client-0.5.0/setup.cfg
+drwxrwxr-x   0 shubuntu1  (1000) shubuntu1  (1000)        0 2023-05-04 03:24:11.000000 fc-client-0.5.0/fc_client/
+-rw-rw-r--   0 shubuntu1  (1000) shubuntu1  (1000)     7005 2023-05-04 03:23:04.000000 fc-client-0.5.0/fc_client/client.py
+-rw-rw-r--   0 shubuntu1  (1000) shubuntu1  (1000)     1071 2023-04-10 02:26:18.000000 fc-client-0.5.0/LICENSE
+drwxrwxr-x   0 shubuntu1  (1000) shubuntu1  (1000)        0 2023-05-04 03:24:11.000000 fc-client-0.5.0/fc_common/
+-rw-rw-r--   0 shubuntu1  (1000) shubuntu1  (1000)        6 2023-05-04 03:23:04.000000 fc-client-0.5.0/fc_common/VERSION
+-rw-rw-r--   0 shubuntu1  (1000) shubuntu1  (1000)      482 2023-05-04 03:23:04.000000 fc-client-0.5.0/fc_common/__init__.py
+-rw-rw-r--   0 shubuntu1  (1000) shubuntu1  (1000)      712 2023-05-04 03:23:04.000000 fc-client-0.5.0/fc_common/version.py
+-rw-rw-r--   0 shubuntu1  (1000) shubuntu1  (1000)     2642 2023-05-04 03:23:04.000000 fc-client-0.5.0/setup.py
+-rw-rw-r--   0 shubuntu1  (1000) shubuntu1  (1000)      715 2023-05-04 03:24:11.000000 fc-client-0.5.0/PKG-INFO
```

### Comparing `fc-client-0.4.3/fc_client.egg-info/PKG-INFO` & `fc-client-0.5.0/fc_client.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,26 +1,24 @@
 Metadata-Version: 2.1
 Name: fc-client
-Version: 0.4.3
+Version: 0.5.0
 Summary: UNKNOWN
 Home-page: https://fc.readthedocs.io/
 Author: Larry Shen
 Author-email: larry.shen@nxp.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3 :: Only
-Requires-Python: >=3.6
-Provides-Extra: labgrid
+Requires-Python: >=3.7
 License-File: LICENSE
 
 UNKNOWN
```

### Comparing `fc-client-0.4.3/README.rst` & `fc-client-0.5.0/README.rst`

 * *Files identical despite different names*

### Comparing `fc-client-0.4.3/setup.cfg` & `fc-client-0.5.0/setup.cfg`

 * *Files 19% similar despite different names*

```diff
@@ -7,20 +7,19 @@
 classifiers = 
 	Development Status :: 4 - Beta
 	Environment :: Console
 	Intended Audience :: Developers
 	License :: OSI Approved :: MIT License
 	Operating System :: POSIX :: Linux
 	Programming Language :: Python
-	Programming Language :: Python :: 3.6
 	Programming Language :: Python :: 3.7
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3 :: Only
 
 [options]
-python_requires = >=3.6
+python_requires = >=3.7
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `fc-client-0.4.3/fc_client/client.py` & `fc-client-0.5.0/fc_client/client.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,46 +1,29 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 #
 # Copyright 2021-2022 NXP
 #
-# The MIT License (MIT)
-# Permission is hereby granted, free of charge, to any person obtaining a copy
-# of this software and associated documentation files (the "Software"), to deal
-# in the Software without restriction, including without limitation the rights
-# to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-# copies of the Software, and to permit persons to whom the Software is
-# furnished to do so, subject to the following conditions:
-#
-# The above copyright notice and this permission notice shall be included in
-# all copies or substantial portions of the Software.
-#
-# THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-# IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-# FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-# AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-# LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-# OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
-# THE SOFTWARE.
+# SPDX-License-Identifier: MIT
 
 
 import argparse
 import json
 import os
 import signal
 import subprocess
 import sys
-
 from getpass import getuser
 from socket import gethostname
 
 import prettytable
 import requests
 import yaml
 
+from fc_common import which
 from fc_common.version import get_runtime_version
 
 
 class Client:
     @staticmethod
     def booking(_):
         fc_server = os.environ.get("FC_SERVER", "http://127.0.0.1:8600")
@@ -84,14 +67,18 @@
             table.field_names = ["Resource", "Farm", "Status", "Comment", "Info"]
         else:
             table.field_names = ["Resource", "Farm", "Status", "Comment"]
 
         print(table.get_string(sortby="Resource"))
 
     @staticmethod
+    @which(
+        "labgrid-client",
+        "Use 'pip3 install labgrid-client' to install labgrid software please.",
+    )
     def lock(args):
         resource = args.resource
         if resource:
             print(f"Try to acquire resource {resource}...")
             with subprocess.Popen(
                 ["labgrid-client", "reserve", "--wait", f"name={resource}"],
                 stdout=subprocess.PIPE,
@@ -116,14 +103,18 @@
                             stderr=subprocess.STDOUT,
                         )
         else:
             print("No resource specified.")
             sys.exit(1)
 
     @staticmethod
+    @which(
+        "labgrid-client",
+        "Use 'pip3 install labgrid-client' to install labgrid software please.",
+    )
     def unlock(args):
         me = "/".join(  # pylint: disable=invalid-name
             (
                 os.environ.get("LG_HOSTNAME", gethostname()),
                 os.environ.get("LG_USERNAME", getuser()),
             )
         )
```

### Comparing `fc-client-0.4.3/LICENSE` & `fc-client-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `fc-client-0.4.3/PKG-INFO` & `fc-client-0.5.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,26 +1,24 @@
 Metadata-Version: 2.1
 Name: fc-client
-Version: 0.4.3
+Version: 0.5.0
 Summary: UNKNOWN
 Home-page: https://fc.readthedocs.io/
 Author: Larry Shen
 Author-email: larry.shen@nxp.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3 :: Only
-Requires-Python: >=3.6
-Provides-Extra: labgrid
+Requires-Python: >=3.7
 License-File: LICENSE
 
 UNKNOWN
```

