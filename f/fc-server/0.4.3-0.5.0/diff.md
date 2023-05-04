# Comparing `tmp/fc-server-0.4.3.tar.gz` & `tmp/fc-server-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/fc-server-0.4.3.tar", last modified: Wed Mar 22 02:13:29 2023, max compression
+gzip compressed data, was "dist/fc-server-0.5.0.tar", last modified: Thu May  4 03:24:10 2023, max compression
```

## Comparing `fc-server-0.4.3.tar` & `fc-server-0.5.0.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxrwxr-x   0 shubuntu1  (1000) shubuntu1  (1000)        0 2023-03-22 02:13:29.000000 fc-server-0.4.3/
--rw-rw-r--   0 shubuntu1  (1000) shubuntu1  (1000)     2535 2022-08-17 07:02:28.000000 fc-server-0.4.3/README.rst
--rw-rw-r--   0 shubuntu1  (1000) shubuntu1  (1000)      653 2023-03-22 02:13:29.000000 fc-server-0.4.3/setup.cfg
-drwxrwxr-x   0 shubuntu1  (1000) shubuntu1  (1000)        0 2023-03-22 02:13:29.000000 fc-server-0.4.3/fc_server.egg-info/
--rw-rw-r--   0 shubuntu1  (1000) shubuntu1  (1000)      134 2023-03-22 02:13:28.000000 fc-server-0.4.3/fc_server.egg-info/requires.txt
--rw-rw-r--   0 shubuntu1  (1000) shubuntu1  (1000)        1 2023-03-22 02:13:28.000000 fc-server-0.4.3/fc_server.egg-info/dependency_links.txt
--rw-rw-r--   0 shubuntu1  (1000) shubuntu1  (1000)      897 2023-03-22 02:13:28.000000 fc-server-0.4.3/fc_server.egg-info/SOURCES.txt
--rw-rw-r--   0 shubuntu1  (1000) shubuntu1  (1000)      765 2023-03-22 02:13:28.000000 fc-server-0.4.3/fc_server.egg-info/PKG-INFO
--rw-rw-r--   0 shubuntu1  (1000) shubuntu1  (1000)       53 2023-03-22 02:13:28.000000 fc-server-0.4.3/fc_server.egg-info/entry_points.txt
--rw-rw-r--   0 shubuntu1  (1000) shubuntu1  (1000)       20 2023-03-22 02:13:28.000000 fc-server-0.4.3/fc_server.egg-info/top_level.txt
--rw-rw-r--   0 shubuntu1  (1000) shubuntu1  (1000)     1071 2022-03-07 07:28:36.000000 fc-server-0.4.3/LICENSE
-drwxrwxr-x   0 shubuntu1  (1000) shubuntu1  (1000)        0 2023-03-22 02:13:29.000000 fc-server-0.4.3/fc_server/
-drwxrwxr-x   0 shubuntu1  (1000) shubuntu1  (1000)        0 2023-03-22 02:13:29.000000 fc-server-0.4.3/fc_server/config/
--rw-rw-r--   0 shubuntu1  (1000) shubuntu1  (1000)       82 2022-03-07 07:28:36.000000 fc-server-0.4.3/fc_server/config/sample_lavacli.yaml
--rw-rw-r--   0 shubuntu1  (1000) shubuntu1  (1000)      357 2022-03-07 07:28:36.000000 fc-server-0.4.3/fc_server/config/sample_cfg.yaml
-drwxrwxr-x   0 shubuntu1  (1000) shubuntu1  (1000)        0 2023-03-22 02:13:29.000000 fc-server-0.4.3/fc_server/plugins/
-drwxrwxr-x   0 shubuntu1  (1000) shubuntu1  (1000)        0 2023-03-22 02:13:29.000000 fc-server-0.4.3/fc_server/plugins/utils/
--rw-rw-r--   0 shubuntu1  (1000) shubuntu1  (1000)     3215 2022-08-17 07:02:28.000000 fc-server-0.4.3/fc_server/plugins/utils/labgrid.py
--rw-rw-r--   0 shubuntu1  (1000) shubuntu1  (1000)     6121 2022-10-13 05:45:44.000000 fc-server-0.4.3/fc_server/plugins/utils/lava.py
--rw-rw-r--   0 shubuntu1  (1000) shubuntu1  (1000)        0 2022-08-17 07:02:28.000000 fc-server-0.4.3/fc_server/plugins/utils/__init__.py
--rw-rw-r--   0 shubuntu1  (1000) shubuntu1  (1000)     8574 2022-08-17 07:02:28.000000 fc-server-0.4.3/fc_server/plugins/labgrid.py
--rw-rw-r--   0 shubuntu1  (1000) shubuntu1  (1000)    18674 2022-12-08 01:54:49.000000 fc-server-0.4.3/fc_server/plugins/lava.py
--rw-rw-r--   0 shubuntu1  (1000) shubuntu1  (1000)        0 2022-03-07 07:28:36.000000 fc-server-0.4.3/fc_server/plugins/__init__.py
-drwxrwxr-x   0 shubuntu1  (1000) shubuntu1  (1000)        0 2023-03-22 02:13:29.000000 fc-server-0.4.3/fc_server/core/
--rw-rw-r--   0 shubuntu1  (1000) shubuntu1  (1000)     1729 2022-03-07 07:28:36.000000 fc-server-0.4.3/fc_server/core/logger.py
--rw-rw-r--   0 shubuntu1  (1000) shubuntu1  (1000)    11704 2022-10-13 05:45:44.000000 fc-server-0.4.3/fc_server/core/coordinator.py
--rw-rw-r--   0 shubuntu1  (1000) shubuntu1  (1000)     7071 2022-03-07 07:28:36.000000 fc-server-0.4.3/fc_server/core/api_svr.py
--rw-rw-r--   0 shubuntu1  (1000) shubuntu1  (1000)     2999 2022-08-17 07:02:28.000000 fc-server-0.4.3/fc_server/core/decorators.py
--rw-rw-r--   0 shubuntu1  (1000) shubuntu1  (1000)     1978 2022-03-07 07:28:36.000000 fc-server-0.4.3/fc_server/core/__init__.py
--rw-rw-r--   0 shubuntu1  (1000) shubuntu1  (1000)     1670 2022-10-13 05:45:44.000000 fc-server-0.4.3/fc_server/core/plugin.py
--rw-rw-r--   0 shubuntu1  (1000) shubuntu1  (1000)     3875 2022-10-13 05:45:44.000000 fc-server-0.4.3/fc_server/core/config.py
--rw-rw-r--   0 shubuntu1  (1000) shubuntu1  (1000)     2150 2022-03-07 07:28:36.000000 fc-server-0.4.3/fc_server/server.py
--rw-rw-r--   0 shubuntu1  (1000) shubuntu1  (1000)        0 2022-03-07 07:28:36.000000 fc-server-0.4.3/fc_server/__init__.py
-drwxrwxr-x   0 shubuntu1  (1000) shubuntu1  (1000)        0 2023-03-22 02:13:29.000000 fc-server-0.4.3/fc_server/management/
--rw-rw-r--   0 shubuntu1  (1000) shubuntu1  (1000)     1260 2022-03-07 07:28:36.000000 fc-server-0.4.3/fc_server/management/common.py
--rw-rw-r--   0 shubuntu1  (1000) shubuntu1  (1000)        0 2022-03-07 07:28:36.000000 fc-server-0.4.3/fc_server/management/__init__.py
--rw-rw-r--   0 shubuntu1  (1000) shubuntu1  (1000)     3547 2022-10-13 05:45:44.000000 fc-server-0.4.3/fc_server/management/cmd_online_lava_devices.py
-drwxrwxr-x   0 shubuntu1  (1000) shubuntu1  (1000)        0 2023-03-22 02:13:29.000000 fc-server-0.4.3/fc_common/
--rw-rw-r--   0 shubuntu1  (1000) shubuntu1  (1000)        6 2023-03-22 02:13:00.000000 fc-server-0.4.3/fc_common/VERSION
--rw-rw-r--   0 shubuntu1  (1000) shubuntu1  (1000)        0 2022-03-07 07:28:36.000000 fc-server-0.4.3/fc_common/__init__.py
--rw-rw-r--   0 shubuntu1  (1000) shubuntu1  (1000)     1759 2022-03-07 07:28:36.000000 fc-server-0.4.3/fc_common/version.py
--rw-rw-r--   0 shubuntu1  (1000) shubuntu1  (1000)     3857 2023-03-22 02:13:00.000000 fc-server-0.4.3/setup.py
--rw-rw-r--   0 shubuntu1  (1000) shubuntu1  (1000)      765 2023-03-22 02:13:29.000000 fc-server-0.4.3/PKG-INFO
+drwxrwxr-x   0 shubuntu1  (1000) shubuntu1  (1000)        0 2023-05-04 03:24:10.000000 fc-server-0.5.0/
+-rw-rw-r--   0 shubuntu1  (1000) shubuntu1  (1000)     2535 2023-04-10 02:26:18.000000 fc-server-0.5.0/README.rst
+-rw-rw-r--   0 shubuntu1  (1000) shubuntu1  (1000)      614 2023-05-04 03:24:10.000000 fc-server-0.5.0/setup.cfg
+drwxrwxr-x   0 shubuntu1  (1000) shubuntu1  (1000)        0 2023-05-04 03:24:10.000000 fc-server-0.5.0/fc_server.egg-info/
+-rw-rw-r--   0 shubuntu1  (1000) shubuntu1  (1000)      109 2023-05-04 03:24:09.000000 fc-server-0.5.0/fc_server.egg-info/requires.txt
+-rw-rw-r--   0 shubuntu1  (1000) shubuntu1  (1000)        1 2023-05-04 03:24:09.000000 fc-server-0.5.0/fc_server.egg-info/dependency_links.txt
+-rw-rw-r--   0 shubuntu1  (1000) shubuntu1  (1000)      897 2023-05-04 03:24:09.000000 fc-server-0.5.0/fc_server.egg-info/SOURCES.txt
+-rw-rw-r--   0 shubuntu1  (1000) shubuntu1  (1000)      715 2023-05-04 03:24:09.000000 fc-server-0.5.0/fc_server.egg-info/PKG-INFO
+-rw-rw-r--   0 shubuntu1  (1000) shubuntu1  (1000)       53 2023-05-04 03:24:09.000000 fc-server-0.5.0/fc_server.egg-info/entry_points.txt
+-rw-rw-r--   0 shubuntu1  (1000) shubuntu1  (1000)       20 2023-05-04 03:24:09.000000 fc-server-0.5.0/fc_server.egg-info/top_level.txt
+-rw-rw-r--   0 shubuntu1  (1000) shubuntu1  (1000)     1071 2023-04-10 02:26:18.000000 fc-server-0.5.0/LICENSE
+drwxrwxr-x   0 shubuntu1  (1000) shubuntu1  (1000)        0 2023-05-04 03:24:10.000000 fc-server-0.5.0/fc_server/
+drwxrwxr-x   0 shubuntu1  (1000) shubuntu1  (1000)        0 2023-05-04 03:24:10.000000 fc-server-0.5.0/fc_server/config/
+-rw-rw-r--   0 shubuntu1  (1000) shubuntu1  (1000)       82 2023-04-10 02:26:18.000000 fc-server-0.5.0/fc_server/config/sample_lavacli.yaml
+-rw-rw-r--   0 shubuntu1  (1000) shubuntu1  (1000)      357 2023-04-10 02:26:18.000000 fc-server-0.5.0/fc_server/config/sample_cfg.yaml
+drwxrwxr-x   0 shubuntu1  (1000) shubuntu1  (1000)        0 2023-05-04 03:24:10.000000 fc-server-0.5.0/fc_server/plugins/
+drwxrwxr-x   0 shubuntu1  (1000) shubuntu1  (1000)        0 2023-05-04 03:24:10.000000 fc-server-0.5.0/fc_server/plugins/utils/
+-rw-rw-r--   0 shubuntu1  (1000) shubuntu1  (1000)     2359 2023-05-04 03:23:04.000000 fc-server-0.5.0/fc_server/plugins/utils/labgrid.py
+-rw-rw-r--   0 shubuntu1  (1000) shubuntu1  (1000)     5185 2023-05-04 03:23:04.000000 fc-server-0.5.0/fc_server/plugins/utils/lava.py
+-rw-rw-r--   0 shubuntu1  (1000) shubuntu1  (1000)        0 2023-04-10 02:26:18.000000 fc-server-0.5.0/fc_server/plugins/utils/__init__.py
+-rw-rw-r--   0 shubuntu1  (1000) shubuntu1  (1000)     7526 2023-05-04 03:23:04.000000 fc-server-0.5.0/fc_server/plugins/labgrid.py
+-rw-rw-r--   0 shubuntu1  (1000) shubuntu1  (1000)    17626 2023-05-04 03:23:04.000000 fc-server-0.5.0/fc_server/plugins/lava.py
+-rw-rw-r--   0 shubuntu1  (1000) shubuntu1  (1000)        0 2023-04-10 02:26:18.000000 fc-server-0.5.0/fc_server/plugins/__init__.py
+drwxrwxr-x   0 shubuntu1  (1000) shubuntu1  (1000)        0 2023-05-04 03:24:10.000000 fc-server-0.5.0/fc_server/core/
+-rw-rw-r--   0 shubuntu1  (1000) shubuntu1  (1000)      681 2023-05-04 03:23:04.000000 fc-server-0.5.0/fc_server/core/logger.py
+-rw-rw-r--   0 shubuntu1  (1000) shubuntu1  (1000)    11568 2023-05-04 03:23:04.000000 fc-server-0.5.0/fc_server/core/coordinator.py
+-rw-rw-r--   0 shubuntu1  (1000) shubuntu1  (1000)     6024 2023-05-04 03:23:04.000000 fc-server-0.5.0/fc_server/core/api_svr.py
+-rw-rw-r--   0 shubuntu1  (1000) shubuntu1  (1000)     1951 2023-05-04 03:23:04.000000 fc-server-0.5.0/fc_server/core/decorators.py
+-rw-rw-r--   0 shubuntu1  (1000) shubuntu1  (1000)      929 2023-05-04 03:23:04.000000 fc-server-0.5.0/fc_server/core/__init__.py
+-rw-rw-r--   0 shubuntu1  (1000) shubuntu1  (1000)      623 2023-05-04 03:23:04.000000 fc-server-0.5.0/fc_server/core/plugin.py
+-rw-rw-r--   0 shubuntu1  (1000) shubuntu1  (1000)     2828 2023-05-04 03:23:04.000000 fc-server-0.5.0/fc_server/core/config.py
+-rw-rw-r--   0 shubuntu1  (1000) shubuntu1  (1000)     1071 2023-05-04 03:23:04.000000 fc-server-0.5.0/fc_server/server.py
+-rw-rw-r--   0 shubuntu1  (1000) shubuntu1  (1000)        0 2023-04-10 02:26:18.000000 fc-server-0.5.0/fc_server/__init__.py
+drwxrwxr-x   0 shubuntu1  (1000) shubuntu1  (1000)        0 2023-05-04 03:24:10.000000 fc-server-0.5.0/fc_server/management/
+-rw-rw-r--   0 shubuntu1  (1000) shubuntu1  (1000)      212 2023-05-04 03:23:04.000000 fc-server-0.5.0/fc_server/management/common.py
+-rw-rw-r--   0 shubuntu1  (1000) shubuntu1  (1000)        0 2023-04-10 02:26:18.000000 fc-server-0.5.0/fc_server/management/__init__.py
+-rw-rw-r--   0 shubuntu1  (1000) shubuntu1  (1000)     2498 2023-05-04 03:23:04.000000 fc-server-0.5.0/fc_server/management/cmd_online_lava_devices.py
+drwxrwxr-x   0 shubuntu1  (1000) shubuntu1  (1000)        0 2023-05-04 03:24:10.000000 fc-server-0.5.0/fc_common/
+-rw-rw-r--   0 shubuntu1  (1000) shubuntu1  (1000)        6 2023-05-04 03:23:04.000000 fc-server-0.5.0/fc_common/VERSION
+-rw-rw-r--   0 shubuntu1  (1000) shubuntu1  (1000)      482 2023-05-04 03:23:04.000000 fc-server-0.5.0/fc_common/__init__.py
+-rw-rw-r--   0 shubuntu1  (1000) shubuntu1  (1000)      712 2023-05-04 03:23:04.000000 fc-server-0.5.0/fc_common/version.py
+-rw-rw-r--   0 shubuntu1  (1000) shubuntu1  (1000)     2642 2023-05-04 03:23:04.000000 fc-server-0.5.0/setup.py
+-rw-rw-r--   0 shubuntu1  (1000) shubuntu1  (1000)      715 2023-05-04 03:24:10.000000 fc-server-0.5.0/PKG-INFO
```

### Comparing `fc-server-0.4.3/README.rst` & `fc-server-0.5.0/README.rst`

 * *Files identical despite different names*

### Comparing `fc-server-0.4.3/setup.cfg` & `fc-server-0.5.0/setup.cfg`

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

### Comparing `fc-server-0.4.3/fc_server.egg-info/SOURCES.txt` & `fc-server-0.5.0/fc_server.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fc-server-0.4.3/fc_server.egg-info/PKG-INFO` & `fc-server-0.5.0/fc_server.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 Metadata-Version: 2.1
 Name: fc-server
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
+Requires-Python: >=3.7
 License-File: LICENSE
 
 UNKNOWN
```

### Comparing `fc-server-0.4.3/LICENSE` & `fc-server-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `fc-server-0.4.3/fc_server/plugins/utils/lava.py` & `fc-server-0.5.0/fc_server/plugins/utils/lava.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,49 +1,35 @@
 # -*- coding: utf-8 -*-
 #
 # Copyright 2022 NXP
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
 
 # pylint: disable=no-member
 
 import asyncio
 import logging
 import traceback
 import types
+
 import yaml
 
+from fc_common import which
 from fc_server.core import AsyncRunMixin
 from fc_server.core.config import Config
 from fc_server.core.decorators import verify_cmd_results
 
 try:
     from functools import singledispatchmethod
 except ImportError:
     from singledispatchmethod import singledispatchmethod
 
 
 class Lava(AsyncRunMixin):
+    @which("lavacli", "Use 'pip3 install lavacli' to install lava client please.")
     def __init__(self):
         self.identities = Config.frameworks_config["lava"]["identities"]
         self.device_description_prefix = "[FC]"
         self.lava_default_description = "Created automatically by LAVA."
 
     @singledispatchmethod
     async def lava_maintenance_devices(
```

### Comparing `fc-server-0.4.3/fc_server/plugins/labgrid.py` & `fc-server-0.5.0/fc_server/plugins/labgrid.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,40 +1,23 @@
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
 
 
 import asyncio
 import logging
 import os
+
 from fc_server.core.decorators import (
     check_priority_scheduler,
     check_seize_strategy,
     safe_cache,
 )
-
 from fc_server.core.plugin import FCPlugin
 from fc_server.plugins.utils.labgrid import Labgrid
 
 
 class Plugin(FCPlugin, Labgrid):
     """
     Plugin for [labgrid framework](https://github.com/labgrid-project/labgrid)
```

### Comparing `fc-server-0.4.3/fc_server/plugins/lava.py` & `fc-server-0.5.0/fc_server/plugins/lava.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,29 +1,12 @@
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
 
 
 import asyncio
 import logging
 
 from async_lru import alru_cache
```

### Comparing `fc-server-0.4.3/fc_server/core/coordinator.py` & `fc-server-0.5.0/fc_server/core/coordinator.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,36 +1,19 @@
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
 
 
 import asyncio
 import logging
 import sys
-
 from importlib import import_module
+
 from fc_server.core.api_svr import ApiSvr
 from fc_server.core.config import Config
 from fc_server.core.decorators import check_priority_scheduler
 
 
 class Coordinator:
     """
@@ -81,14 +64,17 @@
 
         for resource in Config.managed_resources:
             self.__managed_resources_status[resource] = "fc"
 
         # assure no seize for this job when already a seize for this job there
         self.coordinating_job_records = {}
 
+        # record timeout task for seized status
+        self.seized_status_timeout_records = {}
+
         logging.info("FC managed resource list:")
         logging.info(Config.managed_resources)
 
     async def __init_frameworks(self):
         logging.info("Start to init following frameworks:")
 
         init_tasks = []
@@ -213,14 +199,19 @@
             if device == self.coordinating_job_records[job_id]:
                 self.coordinating_job_records.pop(job_id)
 
     def is_seized_job(self, job_id):
         # pylint: disable=consider-iterating-dictionary
         return job_id in list(self.coordinating_job_records.keys())
 
+    async def __seized_status_timeout(self, resource):
+        await asyncio.sleep(90)
+        logging.info("* %s seized status be reset to fc due to timeout", resource)
+        self.reset_resource(resource)
+
     @check_priority_scheduler()
     async def coordinate_resources(self, context, job_id, *candidated_resources):
         """
         Seize resource from low priority framework
         """
 
         if not candidated_resources:
@@ -262,14 +253,23 @@
                         "Force kick off the resource %s.", candidated_seized_resource
                     )
                     await framework.force_kick_off(candidated_seized_resource)
                     self.__set_resource_status(
                         candidated_seized_resource,
                         context.__module__.split(".")[-1] + "_seized",
                     )
+
+                    # timeout for seized status
+                    timeout_task = asyncio.create_task(
+                        self.__seized_status_timeout(candidated_seized_resource)
+                    )
+                    self.seized_status_timeout_records[
+                        candidated_seized_resource
+                    ] = timeout_task
+
                     break
             low_priority_resources.append(candidated_seized_resource)
 
         logging.info(
             "[done] seize resource requirement from %s for %s",
             context.__module__.split(".")[-1],
             job_id,
@@ -294,14 +294,19 @@
             if not await self.__default_framework_plugin.default_framework_connect(
                 resource
             ):
                 # delay default framework connect for this resource if connect api call failure
                 self.__managed_issue_disconnect_resources.append(resource)
 
     def accept_resource(self, resource, context):
+        # cancel seized status timeout task if this resource is seized from others
+        if resource in self.seized_status_timeout_records:
+            timeout_task = self.seized_status_timeout_records.pop(resource)
+            timeout_task.cancel()
+
         self.__set_resource_status(resource, context.__module__.split(".")[-1])
 
     def retire_resource(self, resource):
         self.__set_resource_status(resource, "retired")
 
     def reset_resource(self, resource):
         self.__set_resource_status(resource, "fc")
```

### Comparing `fc-server-0.4.3/PKG-INFO` & `fc-server-0.5.0/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 Metadata-Version: 2.1
 Name: fc-server
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
+Requires-Python: >=3.7
 License-File: LICENSE
 
 UNKNOWN
```

