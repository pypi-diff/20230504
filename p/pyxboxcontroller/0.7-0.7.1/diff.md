# Comparing `tmp/pyxboxcontroller-0.7.tar.gz` & `tmp/pyxboxcontroller-0.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyxboxcontroller-0.7.tar", last modified: Thu May  4 18:05:12 2023, max compression
+gzip compressed data, was "pyxboxcontroller-0.7.1.tar", last modified: Thu May  4 19:59:28 2023, max compression
```

## Comparing `pyxboxcontroller-0.7.tar` & `pyxboxcontroller-0.7.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-05-04 18:05:12.148387 pyxboxcontroller-0.7/
--rw-rw-rw-   0        0        0     1086 2022-10-20 14:56:56.000000 pyxboxcontroller-0.7/LICENCE
--rw-rw-rw-   0        0        0      795 2023-05-04 18:05:12.147385 pyxboxcontroller-0.7/PKG-INFO
--rw-rw-rw-   0        0        0     1234 2023-04-13 22:41:35.000000 pyxboxcontroller-0.7/README.md
-drwxrwxrwx   0        0        0        0 2023-05-04 18:05:12.135220 pyxboxcontroller-0.7/pyxboxcontroller/
--rw-rw-rw-   0        0        0     1559 2023-05-04 17:45:21.000000 pyxboxcontroller-0.7/pyxboxcontroller/XInput.py
--rw-rw-rw-   0        0        0      168 2023-05-04 17:28:58.000000 pyxboxcontroller-0.7/pyxboxcontroller/__init__.py
--rw-rw-rw-   0        0        0    11368 2023-05-04 18:04:52.000000 pyxboxcontroller-0.7/pyxboxcontroller/controller.py
-drwxrwxrwx   0        0        0        0 2023-05-04 18:05:12.145384 pyxboxcontroller-0.7/pyxboxcontroller/examples/
--rw-rw-rw-   0        0        0      104 2023-04-13 22:37:04.000000 pyxboxcontroller-0.7/pyxboxcontroller/examples/__init__.py
--rw-rw-rw-   0        0        0     1082 2023-04-13 22:20:17.000000 pyxboxcontroller-0.7/pyxboxcontroller/examples/example_print_state.py
--rw-rw-rw-   0        0        0     4607 2023-04-13 22:20:32.000000 pyxboxcontroller-0.7/pyxboxcontroller/examples/example_state_gui.py
-drwxrwxrwx   0        0        0        0 2023-05-04 18:05:12.143283 pyxboxcontroller-0.7/pyxboxcontroller.egg-info/
--rw-rw-rw-   0        0        0      795 2023-05-04 18:05:12.000000 pyxboxcontroller-0.7/pyxboxcontroller.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      432 2023-05-04 18:05:12.000000 pyxboxcontroller-0.7/pyxboxcontroller.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-04 18:05:12.000000 pyxboxcontroller-0.7/pyxboxcontroller.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2023-05-04 18:05:12.000000 pyxboxcontroller-0.7/pyxboxcontroller.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-04 18:05:12.148387 pyxboxcontroller-0.7/setup.cfg
--rw-rw-rw-   0        0        0     1105 2023-05-04 15:20:47.000000 pyxboxcontroller-0.7/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-04 18:05:12.146386 pyxboxcontroller-0.7/tests/
--rw-rw-rw-   0        0        0     1532 2023-05-04 17:51:34.000000 pyxboxcontroller-0.7/tests/test_controller.py
+drwxrwxrwx   0        0        0        0 2023-05-04 19:59:28.406313 pyxboxcontroller-0.7.1/
+-rw-rw-rw-   0        0        0     1086 2022-10-20 14:56:56.000000 pyxboxcontroller-0.7.1/LICENCE
+-rw-rw-rw-   0        0        0      797 2023-05-04 19:59:28.406313 pyxboxcontroller-0.7.1/PKG-INFO
+-rw-rw-rw-   0        0        0     1234 2023-04-13 22:41:35.000000 pyxboxcontroller-0.7.1/README.md
+drwxrwxrwx   0        0        0        0 2023-05-04 19:59:28.393301 pyxboxcontroller-0.7.1/pyxboxcontroller/
+-rw-rw-rw-   0        0        0     1559 2023-05-04 17:45:21.000000 pyxboxcontroller-0.7.1/pyxboxcontroller/XInput.py
+-rw-rw-rw-   0        0        0      168 2023-05-04 17:28:58.000000 pyxboxcontroller-0.7.1/pyxboxcontroller/__init__.py
+-rw-rw-rw-   0        0        0    11425 2023-05-04 19:59:09.000000 pyxboxcontroller-0.7.1/pyxboxcontroller/controller.py
+drwxrwxrwx   0        0        0        0 2023-05-04 19:59:28.404310 pyxboxcontroller-0.7.1/pyxboxcontroller/examples/
+-rw-rw-rw-   0        0        0      104 2023-04-13 22:37:04.000000 pyxboxcontroller-0.7.1/pyxboxcontroller/examples/__init__.py
+-rw-rw-rw-   0        0        0     1082 2023-04-13 22:20:17.000000 pyxboxcontroller-0.7.1/pyxboxcontroller/examples/example_print_state.py
+-rw-rw-rw-   0        0        0     4607 2023-04-13 22:20:32.000000 pyxboxcontroller-0.7.1/pyxboxcontroller/examples/example_state_gui.py
+drwxrwxrwx   0        0        0        0 2023-05-04 19:59:28.401307 pyxboxcontroller-0.7.1/pyxboxcontroller.egg-info/
+-rw-rw-rw-   0        0        0      797 2023-05-04 19:59:28.000000 pyxboxcontroller-0.7.1/pyxboxcontroller.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      432 2023-05-04 19:59:28.000000 pyxboxcontroller-0.7.1/pyxboxcontroller.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-04 19:59:28.000000 pyxboxcontroller-0.7.1/pyxboxcontroller.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2023-05-04 19:59:28.000000 pyxboxcontroller-0.7.1/pyxboxcontroller.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-04 19:59:28.407313 pyxboxcontroller-0.7.1/setup.cfg
+-rw-rw-rw-   0        0        0     1107 2023-05-04 19:59:17.000000 pyxboxcontroller-0.7.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-04 19:59:28.405311 pyxboxcontroller-0.7.1/tests/
+-rw-rw-rw-   0        0        0     1517 2023-05-04 19:58:32.000000 pyxboxcontroller-0.7.1/tests/test_controller.py
```

### Comparing `pyxboxcontroller-0.7/LICENCE` & `pyxboxcontroller-0.7.1/LICENCE`

 * *Files identical despite different names*

### Comparing `pyxboxcontroller-0.7/PKG-INFO` & `pyxboxcontroller-0.7.1/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyxboxcontroller
-Version: 0.7
+Version: 0.7.1
 Summary: Allows simple access to the current state of connected Xbox controllers on Windows.
 Home-page: https://github.com/SimpleHydrogen/pyxboxcontroller
 Author: Dan Forbes
 Author-email: danielforbes.123412@gmail.com
 License: MIT
 Keywords: xbox controller,XInput,xbox,controller,python,xbox-controller,xboxcontroller
 Classifier: Programming Language :: Python :: 3.11
```

### Comparing `pyxboxcontroller-0.7/README.md` & `pyxboxcontroller-0.7.1/README.md`

 * *Files identical despite different names*

### Comparing `pyxboxcontroller-0.7/pyxboxcontroller/XInput.py` & `pyxboxcontroller-0.7.1/pyxboxcontroller/XInput.py`

 * *Files identical despite different names*

### Comparing `pyxboxcontroller-0.7/pyxboxcontroller/controller.py` & `pyxboxcontroller-0.7.1/pyxboxcontroller/controller.py`

 * *Files 0% similar despite different names*

```diff
@@ -182,14 +182,16 @@
     """Different battery levels.\n
     EMPTY = 0, LOW = 1, MEDIUM = 2, FULL = 3"""
     EMPTY = 0
     LOW = 1
     MEDIUM = 2
     FULL = 3
 
+    def __str__(self) -> str:
+        return self.name
 
 class BatteryType(IntEnum):
     """Different battery types"""
     DISCONNECTED = 0
     WIRED = 1
     ALKALINE = 2
     NIMH = 3  # nickel metal hydride
```

### Comparing `pyxboxcontroller-0.7/pyxboxcontroller/examples/example_print_state.py` & `pyxboxcontroller-0.7.1/pyxboxcontroller/examples/example_print_state.py`

 * *Files identical despite different names*

### Comparing `pyxboxcontroller-0.7/pyxboxcontroller/examples/example_state_gui.py` & `pyxboxcontroller-0.7.1/pyxboxcontroller/examples/example_state_gui.py`

 * *Files identical despite different names*

### Comparing `pyxboxcontroller-0.7/pyxboxcontroller.egg-info/PKG-INFO` & `pyxboxcontroller-0.7.1/pyxboxcontroller.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyxboxcontroller
-Version: 0.7
+Version: 0.7.1
 Summary: Allows simple access to the current state of connected Xbox controllers on Windows.
 Home-page: https://github.com/SimpleHydrogen/pyxboxcontroller
 Author: Dan Forbes
 Author-email: danielforbes.123412@gmail.com
 License: MIT
 Keywords: xbox controller,XInput,xbox,controller,python,xbox-controller,xboxcontroller
 Classifier: Programming Language :: Python :: 3.11
```

### Comparing `pyxboxcontroller-0.7/setup.py` & `pyxboxcontroller-0.7.1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = "0.7"
+VERSION = "0.7.1"
 DESCRIPTION = 'Allows simple access to the current state of connected Xbox controllers on Windows.'
 
 setup(name='pyxboxcontroller',
     version = VERSION,
     description = DESCRIPTION,
     license = "MIT",
     author = 'Dan Forbes',
```

### Comparing `pyxboxcontroller-0.7/tests/test_controller.py` & `pyxboxcontroller-0.7.1/tests/test_controller.py`

 * *Files 6% similar despite different names*

```diff
@@ -57,17 +57,14 @@
     assert isinstance(battery_info, XboxBatteryInfo)
 
     battery_info.level
     battery_info.battery_type
 
     print(battery_info)
 
-
-def test_battery():
-    ...
+    print(controller.battery_level)
 
 
 if __name__ == "__main__":
     test_default_state()
     test_XboxController()
     test_XboxBatteryInfo()
-    test_battery()
```

