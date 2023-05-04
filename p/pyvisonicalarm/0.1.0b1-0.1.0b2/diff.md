# Comparing `tmp/pyvisonicalarm-0.1.0b1.tar.gz` & `tmp/pyvisonicalarm-0.1.0b2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyvisonicalarm-0.1.0b1.tar", last modified: Tue May  2 12:55:54 2023, max compression
+gzip compressed data, was "pyvisonicalarm-0.1.0b2.tar", last modified: Thu May  4 15:20:14 2023, max compression
```

## Comparing `pyvisonicalarm-0.1.0b1.tar` & `pyvisonicalarm-0.1.0b2.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 12:55:54.682879 pyvisonicalarm-0.1.0b1/
--rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-05-02 12:55:40.000000 pyvisonicalarm-0.1.0b1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    22639 2023-05-02 12:55:54.682879 pyvisonicalarm-0.1.0b1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    22653 2023-05-02 12:55:40.000000 pyvisonicalarm-0.1.0b1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 12:55:54.682879 pyvisonicalarm-0.1.0b1/pyvisonicalarm/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 12:55:40.000000 pyvisonicalarm-0.1.0b1/pyvisonicalarm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7566 2023-05-02 12:55:40.000000 pyvisonicalarm-0.1.0b1/pyvisonicalarm/alarm.py
--rw-r--r--   0 runner    (1001) docker     (123)    13678 2023-05-02 12:55:40.000000 pyvisonicalarm-0.1.0b1/pyvisonicalarm/classes.py
--rw-r--r--   0 runner    (1001) docker     (123)     1510 2023-05-02 12:55:40.000000 pyvisonicalarm-0.1.0b1/pyvisonicalarm/const.py
--rw-r--r--   0 runner    (1001) docker     (123)    20093 2023-05-02 12:55:40.000000 pyvisonicalarm-0.1.0b1/pyvisonicalarm/core.py
--rw-r--r--   0 runner    (1001) docker     (123)      515 2023-05-02 12:55:40.000000 pyvisonicalarm-0.1.0b1/pyvisonicalarm/device_definitions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3508 2023-05-02 12:55:40.000000 pyvisonicalarm-0.1.0b1/pyvisonicalarm/devices.py
--rw-r--r--   0 runner    (1001) docker     (123)     8825 2023-05-02 12:55:40.000000 pyvisonicalarm-0.1.0b1/pyvisonicalarm/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 12:55:54.682879 pyvisonicalarm-0.1.0b1/pyvisonicalarm.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    22639 2023-05-02 12:55:54.000000 pyvisonicalarm-0.1.0b1/pyvisonicalarm.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      431 2023-05-02 12:55:54.000000 pyvisonicalarm-0.1.0b1/pyvisonicalarm.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 12:55:54.000000 pyvisonicalarm-0.1.0b1/pyvisonicalarm.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-02 12:55:54.000000 pyvisonicalarm-0.1.0b1/pyvisonicalarm.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-02 12:55:54.000000 pyvisonicalarm-0.1.0b1/pyvisonicalarm.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-02 12:55:54.682879 pyvisonicalarm-0.1.0b1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      738 2023-05-02 12:55:40.000000 pyvisonicalarm-0.1.0b1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:20:14.760583 pyvisonicalarm-0.1.0b2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-05-04 15:20:01.000000 pyvisonicalarm-0.1.0b2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    22639 2023-05-04 15:20:14.756583 pyvisonicalarm-0.1.0b2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    22653 2023-05-04 15:20:01.000000 pyvisonicalarm-0.1.0b2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:20:14.756583 pyvisonicalarm-0.1.0b2/pyvisonicalarm/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 15:20:01.000000 pyvisonicalarm-0.1.0b2/pyvisonicalarm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7566 2023-05-04 15:20:01.000000 pyvisonicalarm-0.1.0b2/pyvisonicalarm/alarm.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13678 2023-05-04 15:20:01.000000 pyvisonicalarm-0.1.0b2/pyvisonicalarm/classes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1533 2023-05-04 15:20:01.000000 pyvisonicalarm-0.1.0b2/pyvisonicalarm/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20093 2023-05-04 15:20:01.000000 pyvisonicalarm-0.1.0b2/pyvisonicalarm/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)      515 2023-05-04 15:20:01.000000 pyvisonicalarm-0.1.0b2/pyvisonicalarm/device_definitions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3526 2023-05-04 15:20:01.000000 pyvisonicalarm-0.1.0b2/pyvisonicalarm/devices.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8825 2023-05-04 15:20:01.000000 pyvisonicalarm-0.1.0b2/pyvisonicalarm/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:20:14.756583 pyvisonicalarm-0.1.0b2/pyvisonicalarm.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    22639 2023-05-04 15:20:14.000000 pyvisonicalarm-0.1.0b2/pyvisonicalarm.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      431 2023-05-04 15:20:14.000000 pyvisonicalarm-0.1.0b2/pyvisonicalarm.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 15:20:14.000000 pyvisonicalarm-0.1.0b2/pyvisonicalarm.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-04 15:20:14.000000 pyvisonicalarm-0.1.0b2/pyvisonicalarm.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-04 15:20:14.000000 pyvisonicalarm-0.1.0b2/pyvisonicalarm.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-04 15:20:14.760583 pyvisonicalarm-0.1.0b2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      738 2023-05-04 15:20:01.000000 pyvisonicalarm-0.1.0b2/setup.py
```

### Comparing `pyvisonicalarm-0.1.0b1/LICENSE` & `pyvisonicalarm-0.1.0b2/LICENSE`

 * *Files identical despite different names*

### Comparing `pyvisonicalarm-0.1.0b1/PKG-INFO` & `pyvisonicalarm-0.1.0b2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyvisonicalarm
-Version: 0.1.0b1
+Version: 0.1.0b2
 Summary: A simple library for the Visonic Alarm API written in Python 3
 Home-page: https://github.com/msp1974/pyvisonicalarm
 Author: Mark Parker
 Author-email: msparker@sky.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `pyvisonicalarm-0.1.0b1/README.md` & `pyvisonicalarm-0.1.0b2/README.md`

 * *Files identical despite different names*

### Comparing `pyvisonicalarm-0.1.0b1/pyvisonicalarm/alarm.py` & `pyvisonicalarm-0.1.0b2/pyvisonicalarm/alarm.py`

 * *Files identical despite different names*

### Comparing `pyvisonicalarm-0.1.0b1/pyvisonicalarm/classes.py` & `pyvisonicalarm-0.1.0b2/pyvisonicalarm/classes.py`

 * *Files identical despite different names*

### Comparing `pyvisonicalarm-0.1.0b1/pyvisonicalarm/const.py` & `pyvisonicalarm-0.1.0b2/pyvisonicalarm/const.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
-__VERSION__ = "0.1.0b1"
+__VERSION__ = "0.1.0b2"
 
 import enum
 
 
 TEXT_UNKNOWN = "Unknown"
 TEXT_OPEN = "Open"
+TEXT_OPENED = "OPENED"
 TEXT_CLOSED = "Closed"
 TEXT_STATUS_HOME = "HOME"
 TEXT_STATUS_AWAY = "AWAY"
 TEXT_STATUS_DISARM = "DISARM"
 
 
 class RequestType:
```

### Comparing `pyvisonicalarm-0.1.0b1/pyvisonicalarm/core.py` & `pyvisonicalarm-0.1.0b2/pyvisonicalarm/core.py`

 * *Files identical despite different names*

### Comparing `pyvisonicalarm-0.1.0b1/pyvisonicalarm/device_definitions.py` & `pyvisonicalarm-0.1.0b2/pyvisonicalarm/device_definitions.py`

 * *Files identical despite different names*

### Comparing `pyvisonicalarm-0.1.0b1/pyvisonicalarm/devices.py` & `pyvisonicalarm-0.1.0b2/pyvisonicalarm/devices.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from dataclasses import dataclass
 from .classes import BaseClass, title_case
-from .const import TEXT_CLOSED, TEXT_OPEN, TEXT_UNKNOWN
+from .const import TEXT_CLOSED, TEXT_OPEN, TEXT_OPENED, TEXT_UNKNOWN
 
 
 @dataclass
 class Device(BaseClass):
     """Base class definition of a device in the alarm system."""
 
     # Device properties
@@ -78,20 +78,19 @@
 @dataclass
 class ContactDevice(Device):
     """Contact device class definition."""
 
     @property
     def state(self) -> str:
         """Returns the current state of the contact."""
-        if not self.warnings:
-            return TEXT_CLOSED
-        for warning in self.warnings:
-            if warning["type"] == TEXT_OPEN:
-                return TEXT_OPEN
-
+        if self.warnings:
+            for warning in self.warnings:
+                if warning["type"] == TEXT_OPENED:
+                    return TEXT_OPEN
+        return TEXT_CLOSED
 
 @dataclass
 class MotionDevice(Device):
     """Motion sensor device class definition."""
 
     @property
     def brightness(self) -> int:
```

### Comparing `pyvisonicalarm-0.1.0b1/pyvisonicalarm/exceptions.py` & `pyvisonicalarm-0.1.0b2/pyvisonicalarm/exceptions.py`

 * *Files identical despite different names*

### Comparing `pyvisonicalarm-0.1.0b1/pyvisonicalarm.egg-info/PKG-INFO` & `pyvisonicalarm-0.1.0b2/pyvisonicalarm.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyvisonicalarm
-Version: 0.1.0b1
+Version: 0.1.0b2
 Summary: A simple library for the Visonic Alarm API written in Python 3
 Home-page: https://github.com/msp1974/pyvisonicalarm
 Author: Mark Parker
 Author-email: msparker@sky.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `pyvisonicalarm-0.1.0b1/setup.py` & `pyvisonicalarm-0.1.0b2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="pyvisonicalarm",
-    version="0.1.0b1",
+    version="0.1.0b2",
     author="Mark Parker",
     author_email="msparker@sky.com",
     description="A simple library for the Visonic Alarm API written in Python 3",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/msp1974/pyvisonicalarm",
     packages=setuptools.find_packages(),
```

