# Comparing `tmp/voir-0.2.6.tar.gz` & `tmp/voir-0.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "voir-0.2.6.tar", max compression
+gzip compressed data, was "voir-0.2.7.tar", max compression
```

## Comparing `voir-0.2.6.tar` & `voir-0.2.7.tar`

### file list

```diff
@@ -1,26 +1,27 @@
--rw-r--r--   0        0        0      803 2023-05-02 17:56:23.440533 voir-0.2.6/pyproject.toml
--rw-r--r--   0        0        0      139 2023-03-23 16:47:14.434366 voir-0.2.6/voir/__init__.py
--rw-r--r--   0        0        0       61 2023-03-20 20:01:11.843872 voir-0.2.6/voir/__main__.py
--rw-r--r--   0        0        0     7819 2023-03-23 16:47:14.434629 voir-0.2.6/voir/argparse_ext.py
--rw-r--r--   0        0        0      759 2023-03-23 16:47:14.434905 voir-0.2.6/voir/cli.py
--rw-r--r--   0        0        0      107 2023-05-02 17:55:30.856401 voir-0.2.6/voir/errors.py
--rw-r--r--   0        0        0     1809 2023-03-25 15:52:21.103341 voir-0.2.6/voir/helpers.py
--rw-r--r--   0        0        0      399 2023-03-23 16:47:14.435425 voir-0.2.6/voir/instruments/__init__.py
--rw-r--r--   0        0        0     3292 2023-03-23 16:47:14.435688 voir-0.2.6/voir/instruments/dash.py
--rw-r--r--   0        0        0     3609 2023-05-02 17:55:30.856567 voir-0.2.6/voir/instruments/gpu/__init__.py
--rw-r--r--   0        0        0     2244 2023-05-02 17:55:30.856670 voir-0.2.6/voir/instruments/gpu/cuda.py
--rw-r--r--   0        0        0     5854 2023-05-02 17:55:30.856783 voir-0.2.6/voir/instruments/gpu/rocm.py
--rw-r--r--   0        0        0      884 2023-03-23 16:47:14.436583 voir-0.2.6/voir/instruments/log.py
--rw-r--r--   0        0        0      818 2023-04-01 02:22:45.030632 voir-0.2.6/voir/instruments/manage.py
--rw-r--r--   0        0        0     5981 2023-03-25 16:19:36.879569 voir-0.2.6/voir/instruments/metric.py
--rw-r--r--   0        0        0      382 2023-03-28 03:32:37.110995 voir-0.2.6/voir/instruments/utils.py
--rw-r--r--   0        0        0     6334 2023-03-23 16:47:14.437785 voir-0.2.6/voir/overseer.py
--rw-r--r--   0        0        0     9968 2023-05-02 17:55:30.857303 voir-0.2.6/voir/phase.py
--rw-r--r--   0        0        0     6183 2023-05-02 17:53:58.153830 voir-0.2.6/voir/proc.py
--rw-r--r--   0        0        0     1667 2023-03-23 16:47:14.438784 voir-0.2.6/voir/run.py
--rw-r--r--   0        0        0     1306 2023-03-23 16:47:14.439124 voir-0.2.6/voir/scriptutils.py
--rw-r--r--   0        0        0     3060 2023-03-23 16:47:14.439374 voir-0.2.6/voir/smuggle.py
--rw-r--r--   0        0        0     1720 2023-03-23 16:47:14.439677 voir-0.2.6/voir/tools.py
--rw-r--r--   0        0        0       18 2023-05-02 17:56:23.466397 voir-0.2.6/voir/version.py
--rw-r--r--   0        0        0      903 1970-01-01 00:00:00.000000 voir-0.2.6/setup.py
--rw-r--r--   0        0        0      790 1970-01-01 00:00:00.000000 voir-0.2.6/PKG-INFO
+-rw-r--r--   0        0        0      803 2023-05-04 17:50:16.855659 voir-0.2.7/pyproject.toml
+-rw-r--r--   0        0        0      139 2023-03-23 16:47:14.434366 voir-0.2.7/voir/__init__.py
+-rw-r--r--   0        0        0       61 2023-03-20 20:01:11.843872 voir-0.2.7/voir/__main__.py
+-rw-r--r--   0        0        0     7819 2023-03-23 16:47:14.434629 voir-0.2.7/voir/argparse_ext.py
+-rw-r--r--   0        0        0      759 2023-03-23 16:47:14.434905 voir-0.2.7/voir/cli.py
+-rw-r--r--   0        0        0      107 2023-05-02 17:55:30.856401 voir-0.2.7/voir/errors.py
+-rw-r--r--   0        0        0     1809 2023-03-25 15:52:21.103341 voir-0.2.7/voir/helpers.py
+-rw-r--r--   0        0        0      399 2023-03-23 16:47:14.435425 voir-0.2.7/voir/instruments/__init__.py
+-rw-r--r--   0        0        0     3292 2023-03-23 16:47:14.435688 voir-0.2.7/voir/instruments/dash.py
+-rw-r--r--   0        0        0     3408 2023-05-04 17:50:09.395001 voir-0.2.7/voir/instruments/gpu/__init__.py
+-rw-r--r--   0        0        0      253 2023-05-04 17:50:09.395110 voir-0.2.7/voir/instruments/gpu/cpu.py
+-rw-r--r--   0        0        0     2282 2023-05-04 17:50:09.395265 voir-0.2.7/voir/instruments/gpu/cuda.py
+-rw-r--r--   0        0        0     5896 2023-05-04 17:50:09.395420 voir-0.2.7/voir/instruments/gpu/rocm.py
+-rw-r--r--   0        0        0      884 2023-03-23 16:47:14.436583 voir-0.2.7/voir/instruments/log.py
+-rw-r--r--   0        0        0      818 2023-04-01 02:22:45.030632 voir-0.2.7/voir/instruments/manage.py
+-rw-r--r--   0        0        0     5981 2023-03-25 16:19:36.879569 voir-0.2.7/voir/instruments/metric.py
+-rw-r--r--   0        0        0      382 2023-03-28 03:32:37.110995 voir-0.2.7/voir/instruments/utils.py
+-rw-r--r--   0        0        0     6334 2023-03-23 16:47:14.437785 voir-0.2.7/voir/overseer.py
+-rw-r--r--   0        0        0     9968 2023-05-02 17:55:30.857303 voir-0.2.7/voir/phase.py
+-rw-r--r--   0        0        0     6183 2023-05-02 17:53:58.153830 voir-0.2.7/voir/proc.py
+-rw-r--r--   0        0        0     1667 2023-03-23 16:47:14.438784 voir-0.2.7/voir/run.py
+-rw-r--r--   0        0        0     1306 2023-03-23 16:47:14.439124 voir-0.2.7/voir/scriptutils.py
+-rw-r--r--   0        0        0     3060 2023-03-23 16:47:14.439374 voir-0.2.7/voir/smuggle.py
+-rw-r--r--   0        0        0     1720 2023-03-23 16:47:14.439677 voir-0.2.7/voir/tools.py
+-rw-r--r--   0        0        0       18 2023-05-04 17:50:16.880190 voir-0.2.7/voir/version.py
+-rw-r--r--   0        0        0      903 1970-01-01 00:00:00.000000 voir-0.2.7/setup.py
+-rw-r--r--   0        0        0      790 1970-01-01 00:00:00.000000 voir-0.2.7/PKG-INFO
```

### Comparing `voir-0.2.6/pyproject.toml` & `voir-0.2.7/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "voir"
-version = "0.2.6"
+version = "0.2.7"
 description = "Instrument, extend and visualize your programs"
 authors = ["Olivier Breuleux <breuleux@gmail.com>"]
 license = "MIT"
 
 [tool.poetry.dependencies]
 python = "^3.7"
 ptera = "^1.4.1"
```

### Comparing `voir-0.2.6/voir/argparse_ext.py` & `voir-0.2.7/voir/argparse_ext.py`

 * *Files identical despite different names*

### Comparing `voir-0.2.6/voir/cli.py` & `voir-0.2.7/voir/cli.py`

 * *Files identical despite different names*

### Comparing `voir-0.2.6/voir/helpers.py` & `voir-0.2.7/voir/helpers.py`

 * *Files identical despite different names*

### Comparing `voir-0.2.6/voir/instruments/dash.py` & `voir-0.2.7/voir/instruments/dash.py`

 * *Files identical despite different names*

### Comparing `voir-0.2.6/voir/instruments/gpu/__init__.py` & `voir-0.2.7/voir/instruments/gpu/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,12 +1,10 @@
 import glob
 import os
-import time
 import traceback
-from threading import Thread
 
 from ...errors import NotAvailable
 from ...tools import instrument_definition
 from ..utils import Monitor as Monitor2
 
 
 def find_monitors():
@@ -33,17 +31,15 @@
 
         backends[module_name] = module
 
     return backends
 
 
 BACKENDS = find_monitors()
-BACKEND = None
 DEVICESMI = None
-ARCH = None
 
 
 def get_backends():
     global BACKENDS
     return BACKENDS.keys()
 
 
@@ -74,80 +70,75 @@
     elif len(suitable) == 0:
         return "cpu"
 
     return suitable[0]
 
 
 def select_backend(arch=None):
-    global BACKEND, DEVICESMI, ARCH
+    global DEVICESMI
 
-    if ARCH is not None and ARCH == arch:
-        return DEVICESMI, ARCH
-    else:
-        _reset()
+    if DEVICESMI is not None:
+        if DEVICESMI.arch == arch:
+            return DEVICESMI
+        DEVICESMI.close()
+        DEVICESMI = None
 
     if arch is None:
         arch = deduce_backend()
 
-    ARCH = arch
-    BACKEND = BACKENDS.get(arch)
+    backend = BACKENDS.get(arch)
 
-    if BACKEND is not None:
-        if BACKEND.is_installed():
-            DEVICESMI = BACKEND.DeviceSMI()
-        else:
-            raise NotAvailable(f"{arch} is not installed")
+    if backend is not None and backend.is_installed():
+        DEVICESMI = backend.DeviceSMI()
+    else:
+        raise NotAvailable(f"{arch} is not installed")
 
-    return DEVICESMI, ARCH
+    return DEVICESMI
 
 
-def _reset():
-    global BACKEND, DEVICESMI, ARCH
-    BACKEND = None
-    DEVICESMI = None
-    ARCH = None
+def gpu_info(smi):
+    return {
+        "arch": smi.arch,
+        "gpus": smi.get_gpus_info(),
+    }
 
 
-def get_visible_devices():
-    global BACKEND
-    return BACKEND.get_visible_devices()
+def get_gpu_info(arch=None):
+    return gpu_info(select_backend(arch))
 
 
-def get_gpu_info(arch=None):
-    monitor, arch = select_backend(arch)
+def _visible_devices(smi):
+    visible = smi.visible_devices
 
-    result = {}
-    if monitor is not None:
-        result = monitor.get_gpus_info()
+    if visible:
+        ours = visible.split(",")
+    else:
+        ours = [str(x) for x in range(100)]
 
-    return {"arch": arch, "gpus": result}
+    return ours
 
 
 @instrument_definition
 def gpu_monitor(ov, poll_interval=10, arch=None):
     yield ov.phases.load_script
 
-    visible = get_visible_devices()
-
-    if visible:
-        ours = visible.split(",")
-    else:
-        ours = [str(x) for x in range(100)]
+    smi = select_backend(arch)
+    ours = _visible_devices(smi)
 
     def monitor():
         data = {
             gpu["device"]: {
                 "memory": [
                     gpu["memory"]["used"],
                     gpu["memory"]["total"],
                 ],
                 "load": gpu["utilization"]["compute"],
                 "temperature": gpu["temperature"],
             }
-            for gpu in get_gpu_info(arch)["gpus"].values()
+            for gpu in smi.get_gpus_info().values()
             if str(gpu["device"]) in ours
         }
         ov.give(task="main", gpudata=data)
 
     monitor_thread = Monitor2(poll_interval, monitor)
     monitor_thread.start()
     try:
```

### Comparing `voir-0.2.6/voir/instruments/gpu/cuda.py` & `voir-0.2.7/voir/instruments/gpu/cuda.py`

 * *Files 4% similar despite different names*

```diff
@@ -44,22 +44,14 @@
     }
 
 
 def is_installed():
     return IMPORT_ERROR is None
 
 
-def get_arch():
-    return "cuda"
-
-
-def get_visible_devices():
-    return os.environ.get("CUDA_VISIBLE_DEVICES", None)
-
-
 class DeviceSMI:
     def __init__(self) -> None:
         if IMPORT_ERROR is not None:
             raise IMPORT_ERROR
 
         try:
             nvmlInit()
@@ -67,14 +59,22 @@
 
         except NVMLError_LibraryNotFound as err:
             raise NotAvailable() from err
 
         except NVMLError_DriverNotLoaded as err:
             raise NotAvailable() from err
 
+    @property
+    def arch(self):
+        return "cuda"
+
+    @property
+    def visible_devices():
+        return os.environ.get("CUDA_VISIBLE_DEVICES", None)
+
     def get_gpus_info(self):
         to_query = [
             "gpu_name",
             "memory.free",
             "memory.used",
             "memory.total",
             "temperature.gpu",
```

### Comparing `voir-0.2.6/voir/instruments/gpu/rocm.py` & `voir-0.2.7/voir/instruments/gpu/rocm.py`

 * *Files 1% similar despite different names*

```diff
@@ -164,22 +164,14 @@
     return series
 
 
 def is_installed():
     return IMPORT_ERROR is None
 
 
-def get_arch():
-    return "rocm"
-
-
-def get_visible_devices():
-    return os.environ.get("ROCR_VISIBLE_DEVICES", None)
-
-
 class DeviceSMI:
     def __init__(self) -> None:
         if IMPORT_ERROR is not None:
             raise IMPORT_ERROR
 
         initialize_rsmi()
         self.devices = list_devices()
@@ -202,14 +194,22 @@
                 "memory": used / total,
             },
             "temperature": temp,
             "power": power,
             "selection_variable": "ROCR_VISIBLE_DEVICES",
         }
 
+    @property
+    def arch(self):
+        return "rocm"
+
+    @property
+    def visible_devices(self):
+        return os.environ.get("ROCR_VISIBLE_DEVICES", None)
+
     def get_gpus_info(self):
         gpus = dict()
         for device in self.devices:
             gpus[device] = self.get_gpu_info(device)
         return gpus
 
     def close(self):
```

### Comparing `voir-0.2.6/voir/instruments/log.py` & `voir-0.2.7/voir/instruments/log.py`

 * *Files identical despite different names*

### Comparing `voir-0.2.6/voir/instruments/manage.py` & `voir-0.2.7/voir/instruments/manage.py`

 * *Files identical despite different names*

### Comparing `voir-0.2.6/voir/instruments/metric.py` & `voir-0.2.7/voir/instruments/metric.py`

 * *Files identical despite different names*

### Comparing `voir-0.2.6/voir/overseer.py` & `voir-0.2.7/voir/overseer.py`

 * *Files identical despite different names*

### Comparing `voir-0.2.6/voir/phase.py` & `voir-0.2.7/voir/phase.py`

 * *Files identical despite different names*

### Comparing `voir-0.2.6/voir/proc.py` & `voir-0.2.7/voir/proc.py`

 * *Files identical despite different names*

### Comparing `voir-0.2.6/voir/run.py` & `voir-0.2.7/voir/run.py`

 * *Files identical despite different names*

### Comparing `voir-0.2.6/voir/scriptutils.py` & `voir-0.2.7/voir/scriptutils.py`

 * *Files identical despite different names*

### Comparing `voir-0.2.6/voir/smuggle.py` & `voir-0.2.7/voir/smuggle.py`

 * *Files identical despite different names*

### Comparing `voir-0.2.6/voir/tools.py` & `voir-0.2.7/voir/tools.py`

 * *Files identical despite different names*

### Comparing `voir-0.2.6/setup.py` & `voir-0.2.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
  'rich>=13.3.2,<14.0.0']
 
 entry_points = \
 {'console_scripts': ['voir = voir.cli:main']}
 
 setup_kwargs = {
     'name': 'voir',
-    'version': '0.2.6',
+    'version': '0.2.7',
     'description': 'Instrument, extend and visualize your programs',
     'long_description': 'None',
     'author': 'Olivier Breuleux',
     'author_email': 'breuleux@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `voir-0.2.6/PKG-INFO` & `voir-0.2.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: voir
-Version: 0.2.6
+Version: 0.2.7
 Summary: Instrument, extend and visualize your programs
 License: MIT
 Author: Olivier Breuleux
 Author-email: breuleux@gmail.com
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

