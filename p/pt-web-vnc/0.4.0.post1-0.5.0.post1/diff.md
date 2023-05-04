# Comparing `tmp/pt-web-vnc-0.4.0.post1.tar.gz` & `tmp/pt-web-vnc-0.5.0.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pt-web-vnc-0.4.0.post1.tar", last modified: Wed Apr 19 13:04:32 2023, max compression
+gzip compressed data, was "dist/pt-web-vnc-0.5.0.post1.tar", last modified: Thu May  4 13:15:29 2023, max compression
```

## Comparing `pt-web-vnc-0.4.0.post1.tar` & `pt-web-vnc-0.5.0.post1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 13:04:32.000000 pt-web-vnc-0.4.0.post1/
--rw-r--r--   0 runner    (1001) docker     (122)      263 2023-04-19 13:04:22.000000 pt-web-vnc-0.4.0.post1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)     7030 2023-04-19 13:04:32.000000 pt-web-vnc-0.4.0.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     5114 2023-04-19 13:04:22.000000 pt-web-vnc-0.4.0.post1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 13:04:32.000000 pt-web-vnc-0.4.0.post1/pt_web_vnc/
--rw-r--r--   0 runner    (1001) docker     (122)      194 2023-04-19 13:04:22.000000 pt-web-vnc-0.4.0.post1/pt_web_vnc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      547 2023-04-19 13:04:22.000000 pt-web-vnc-0.4.0.post1/pt_web_vnc/connection_details.py
--rw-r--r--   0 runner    (1001) docker     (122)     2946 2023-04-19 13:04:22.000000 pt-web-vnc-0.4.0.post1/pt_web_vnc/display_activity_monitor.py
--rw-r--r--   0 runner    (1001) docker     (122)     1381 2023-04-19 13:04:22.000000 pt-web-vnc-0.4.0.post1/pt_web_vnc/screenshot_monitor.py
--rw-r--r--   0 runner    (1001) docker     (122)      572 2023-04-19 13:04:22.000000 pt-web-vnc-0.4.0.post1/pt_web_vnc/utils.py
--rw-r--r--   0 runner    (1001) docker     (122)      153 2023-04-19 13:04:22.000000 pt-web-vnc-0.4.0.post1/pt_web_vnc/version.py
--rw-r--r--   0 runner    (1001) docker     (122)     6066 2023-04-19 13:04:22.000000 pt-web-vnc-0.4.0.post1/pt_web_vnc/vnc.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 13:04:32.000000 pt-web-vnc-0.4.0.post1/pt_web_vnc.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     7030 2023-04-19 13:04:32.000000 pt-web-vnc-0.4.0.post1/pt_web_vnc.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      417 2023-04-19 13:04:32.000000 pt-web-vnc-0.4.0.post1/pt_web_vnc.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-19 13:04:32.000000 pt-web-vnc-0.4.0.post1/pt_web_vnc.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       78 2023-04-19 13:04:32.000000 pt-web-vnc-0.4.0.post1/pt_web_vnc.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       17 2023-04-19 13:04:32.000000 pt-web-vnc-0.4.0.post1/pt_web_vnc.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 13:04:32.000000 pt-web-vnc-0.4.0.post1/scripts/
--rwxr-xr-x   0 runner    (1001) docker     (122)     9270 2023-04-19 13:04:22.000000 pt-web-vnc-0.4.0.post1/scripts/pt-web-vnc
--rw-r--r--   0 runner    (1001) docker     (122)     1256 2023-04-19 13:04:32.000000 pt-web-vnc-0.4.0.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)      224 2023-04-19 13:04:22.000000 pt-web-vnc-0.4.0.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-04 13:15:29.000000 pt-web-vnc-0.5.0.post1/
+-rw-r--r--   0 runner    (1001) docker     (122)      263 2023-05-04 13:15:16.000000 pt-web-vnc-0.5.0.post1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)     7030 2023-05-04 13:15:29.000000 pt-web-vnc-0.5.0.post1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     5114 2023-05-04 13:15:16.000000 pt-web-vnc-0.5.0.post1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-04 13:15:29.000000 pt-web-vnc-0.5.0.post1/pt_web_vnc/
+-rw-r--r--   0 runner    (1001) docker     (122)      194 2023-05-04 13:15:16.000000 pt-web-vnc-0.5.0.post1/pt_web_vnc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      547 2023-05-04 13:15:16.000000 pt-web-vnc-0.5.0.post1/pt_web_vnc/connection_details.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2946 2023-05-04 13:15:16.000000 pt-web-vnc-0.5.0.post1/pt_web_vnc/display_activity_monitor.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1867 2023-05-04 13:15:16.000000 pt-web-vnc-0.5.0.post1/pt_web_vnc/screenshot_monitor.py
+-rw-r--r--   0 runner    (1001) docker     (122)      572 2023-05-04 13:15:16.000000 pt-web-vnc-0.5.0.post1/pt_web_vnc/utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)      153 2023-05-04 13:15:16.000000 pt-web-vnc-0.5.0.post1/pt_web_vnc/version.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6187 2023-05-04 13:15:16.000000 pt-web-vnc-0.5.0.post1/pt_web_vnc/vnc.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-04 13:15:29.000000 pt-web-vnc-0.5.0.post1/pt_web_vnc.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     7030 2023-05-04 13:15:29.000000 pt-web-vnc-0.5.0.post1/pt_web_vnc.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      417 2023-05-04 13:15:29.000000 pt-web-vnc-0.5.0.post1/pt_web_vnc.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-04 13:15:29.000000 pt-web-vnc-0.5.0.post1/pt_web_vnc.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       78 2023-05-04 13:15:29.000000 pt-web-vnc-0.5.0.post1/pt_web_vnc.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       17 2023-05-04 13:15:29.000000 pt-web-vnc-0.5.0.post1/pt_web_vnc.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-04 13:15:29.000000 pt-web-vnc-0.5.0.post1/scripts/
+-rwxr-xr-x   0 runner    (1001) docker     (122)     9270 2023-05-04 13:15:16.000000 pt-web-vnc-0.5.0.post1/scripts/pt-web-vnc
+-rw-r--r--   0 runner    (1001) docker     (122)     1256 2023-05-04 13:15:29.000000 pt-web-vnc-0.5.0.post1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)      224 2023-05-04 13:15:16.000000 pt-web-vnc-0.5.0.post1/setup.py
```

### Comparing `pt-web-vnc-0.4.0.post1/PKG-INFO` & `pt-web-vnc-0.5.0.post1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pt-web-vnc
-Version: 0.4.0.post1
+Version: 0.5.0.post1
 Summary: pi-top Web VNC Tool
 Home-page: https://github.com/pi-top/pt-web-vnc
 Author: pi-top (CEED Ltd)
 Author-email: deb-maintainers@pi-top.com
 License: Apache Software License
 Description: pt-web-vnc
         ==========
```

### Comparing `pt-web-vnc-0.4.0.post1/README.rst` & `pt-web-vnc-0.5.0.post1/README.rst`

 * *Files identical despite different names*

### Comparing `pt-web-vnc-0.4.0.post1/pt_web_vnc/connection_details.py` & `pt-web-vnc-0.5.0.post1/pt_web_vnc/connection_details.py`

 * *Files identical despite different names*

### Comparing `pt-web-vnc-0.4.0.post1/pt_web_vnc/display_activity_monitor.py` & `pt-web-vnc-0.5.0.post1/pt_web_vnc/display_activity_monitor.py`

 * *Files identical despite different names*

### Comparing `pt-web-vnc-0.4.0.post1/pt_web_vnc/utils.py` & `pt-web-vnc-0.5.0.post1/pt_web_vnc/utils.py`

 * *Files identical despite different names*

### Comparing `pt-web-vnc-0.4.0.post1/pt_web_vnc/vnc.py` & `pt-web-vnc-0.5.0.post1/pt_web_vnc/vnc.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,18 @@
 import asyncio
 import logging
 from typing import Callable, Optional
 
 from .connection_details import VncConnectionDetails
 from .display_activity_monitor import start_activity_monitor, stop_activity_monitor
-from .screenshot_monitor import ScreenshotMonitor
+from .screenshot_monitor import (
+    ScreenshotMonitor,
+    start_screenshot_monitor,
+    stop_screenshot_monitor,
+)
 from .utils import run_command
 
 logger = logging.getLogger(__name__)
 
 
 class PtWebVncCommands:
     @staticmethod
@@ -148,22 +152,23 @@
     if callable(on_display_activity):
         start_activity_monitor(
             display_id, on_display_activity, connection_details(display_id)
         )
 
     screenshot_monitor = None
     if screenshot_timeout > 0:
-        screenshot_monitor = ScreenshotMonitor(display_id, screenshot_timeout)
+        screenshot_monitor = start_screenshot_monitor(display_id, screenshot_timeout)
     return screenshot_monitor
 
 
 async def async_stop(display_id: int) -> None:
     cmd = PtWebVncCommands.stop(display_id)
     logging.info(f"Stopping pt-web-vnc: {cmd}")
     await stop_activity_monitor(display_id)
+    await stop_screenshot_monitor(display_id)
     proc = await asyncio.create_subprocess_shell(
         cmd,
         stdout=asyncio.subprocess.PIPE,
         stderr=asyncio.subprocess.PIPE,
     )
     await proc.wait()
```

### Comparing `pt-web-vnc-0.4.0.post1/pt_web_vnc.egg-info/PKG-INFO` & `pt-web-vnc-0.5.0.post1/pt_web_vnc.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pt-web-vnc
-Version: 0.4.0.post1
+Version: 0.5.0.post1
 Summary: pi-top Web VNC Tool
 Home-page: https://github.com/pi-top/pt-web-vnc
 Author: pi-top (CEED Ltd)
 Author-email: deb-maintainers@pi-top.com
 License: Apache Software License
 Description: pt-web-vnc
         ==========
```

### Comparing `pt-web-vnc-0.4.0.post1/scripts/pt-web-vnc` & `pt-web-vnc-0.5.0.post1/scripts/pt-web-vnc`

 * *Files identical despite different names*

### Comparing `pt-web-vnc-0.4.0.post1/setup.cfg` & `pt-web-vnc-0.5.0.post1/setup.cfg`

 * *Files identical despite different names*

