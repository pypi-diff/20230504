# Comparing `tmp/backend.ai-accelerator-cuda-open-23.3.0a4.tar.gz` & `tmp/backend.ai-accelerator-cuda-open-23.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "backend.ai-accelerator-cuda-open-23.3.0a4.tar", last modified: Thu Mar 16 02:53:03 2023, max compression
+gzip compressed data, was "backend.ai-accelerator-cuda-open-23.3.1.tar", last modified: Thu May  4 05:10:17 2023, max compression
```

## Comparing `backend.ai-accelerator-cuda-open-23.3.0a4.tar` & `backend.ai-accelerator-cuda-open-23.3.1.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 02:53:03.908310 backend.ai-accelerator-cuda-open-23.3.0a4/
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-03-16 02:53:03.000000 backend.ai-accelerator-cuda-open-23.3.0a4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1986 2023-03-16 02:53:03.908310 backend.ai-accelerator-cuda-open-23.3.0a4/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 02:53:03.908310 backend.ai-accelerator-cuda-open-23.3.0a4/ai/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 02:53:03.908310 backend.ai-accelerator-cuda-open-23.3.0a4/ai/backend/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 02:53:03.908310 backend.ai-accelerator-cuda-open-23.3.0a4/ai/backend/accelerator/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 02:53:03.908310 backend.ai-accelerator-cuda-open-23.3.0a4/ai/backend/accelerator/cuda_open/
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-03-16 02:53:03.000000 backend.ai-accelerator-cuda-open-23.3.0a4/ai/backend/accelerator/cuda_open/VERSION
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-03-16 02:53:03.000000 backend.ai-accelerator-cuda-open-23.3.0a4/ai/backend/accelerator/cuda_open/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18913 2023-03-16 02:53:03.000000 backend.ai-accelerator-cuda-open-23.3.0a4/ai/backend/accelerator/cuda_open/nvidia.py
--rw-r--r--   0 runner    (1001) docker     (123)    17558 2023-03-16 02:53:03.000000 backend.ai-accelerator-cuda-open-23.3.0a4/ai/backend/accelerator/cuda_open/plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-03-16 02:53:03.000000 backend.ai-accelerator-cuda-open-23.3.0a4/ai/backend/accelerator/cuda_open/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 02:53:03.908310 backend.ai-accelerator-cuda-open-23.3.0a4/backend.ai_accelerator_cuda_open.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1986 2023-03-16 02:53:03.000000 backend.ai-accelerator-cuda-open-23.3.0a4/backend.ai_accelerator_cuda_open.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      708 2023-03-16 02:53:03.000000 backend.ai-accelerator-cuda-open-23.3.0a4/backend.ai_accelerator_cuda_open.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-16 02:53:03.000000 backend.ai-accelerator-cuda-open-23.3.0a4/backend.ai_accelerator_cuda_open.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-03-16 02:53:03.000000 backend.ai-accelerator-cuda-open-23.3.0a4/backend.ai_accelerator_cuda_open.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-16 02:53:03.000000 backend.ai-accelerator-cuda-open-23.3.0a4/backend.ai_accelerator_cuda_open.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-16 02:53:03.000000 backend.ai-accelerator-cuda-open-23.3.0a4/backend.ai_accelerator_cuda_open.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      246 2023-03-16 02:53:03.000000 backend.ai-accelerator-cuda-open-23.3.0a4/backend.ai_accelerator_cuda_open.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        3 2023-03-16 02:53:03.000000 backend.ai-accelerator-cuda-open-23.3.0a4/backend.ai_accelerator_cuda_open.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      626 2023-03-16 02:53:03.000000 backend.ai-accelerator-cuda-open-23.3.0a4/backend_shim.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-16 02:53:03.908310 backend.ai-accelerator-cuda-open-23.3.0a4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3095 2023-03-16 02:53:03.000000 backend.ai-accelerator-cuda-open-23.3.0a4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 05:10:17.310674 backend.ai-accelerator-cuda-open-23.3.1/
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-04 05:10:17.000000 backend.ai-accelerator-cuda-open-23.3.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1996 2023-05-04 05:10:17.310674 backend.ai-accelerator-cuda-open-23.3.1/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 05:10:17.306674 backend.ai-accelerator-cuda-open-23.3.1/ai/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 05:10:17.306674 backend.ai-accelerator-cuda-open-23.3.1/ai/backend/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 05:10:17.306674 backend.ai-accelerator-cuda-open-23.3.1/ai/backend/accelerator/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 05:10:17.306674 backend.ai-accelerator-cuda-open-23.3.1/ai/backend/accelerator/cuda_open/
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-04 05:10:17.000000 backend.ai-accelerator-cuda-open-23.3.1/ai/backend/accelerator/cuda_open/VERSION
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-04 05:10:17.000000 backend.ai-accelerator-cuda-open-23.3.1/ai/backend/accelerator/cuda_open/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18913 2023-05-04 05:10:17.000000 backend.ai-accelerator-cuda-open-23.3.1/ai/backend/accelerator/cuda_open/nvidia.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17483 2023-05-04 05:10:17.000000 backend.ai-accelerator-cuda-open-23.3.1/ai/backend/accelerator/cuda_open/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-04 05:10:17.000000 backend.ai-accelerator-cuda-open-23.3.1/ai/backend/accelerator/cuda_open/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 05:10:17.310674 backend.ai-accelerator-cuda-open-23.3.1/backend.ai_accelerator_cuda_open.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1996 2023-05-04 05:10:17.000000 backend.ai-accelerator-cuda-open-23.3.1/backend.ai_accelerator_cuda_open.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      708 2023-05-04 05:10:17.000000 backend.ai-accelerator-cuda-open-23.3.1/backend.ai_accelerator_cuda_open.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 05:10:17.000000 backend.ai-accelerator-cuda-open-23.3.1/backend.ai_accelerator_cuda_open.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-05-04 05:10:17.000000 backend.ai-accelerator-cuda-open-23.3.1/backend.ai_accelerator_cuda_open.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 05:10:17.000000 backend.ai-accelerator-cuda-open-23.3.1/backend.ai_accelerator_cuda_open.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 05:10:17.000000 backend.ai-accelerator-cuda-open-23.3.1/backend.ai_accelerator_cuda_open.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      232 2023-05-04 05:10:17.000000 backend.ai-accelerator-cuda-open-23.3.1/backend.ai_accelerator_cuda_open.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        3 2023-05-04 05:10:17.000000 backend.ai-accelerator-cuda-open-23.3.1/backend.ai_accelerator_cuda_open.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      626 2023-05-04 05:10:17.000000 backend.ai-accelerator-cuda-open-23.3.1/backend_shim.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-04 05:10:17.310674 backend.ai-accelerator-cuda-open-23.3.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3091 2023-05-04 05:10:17.000000 backend.ai-accelerator-cuda-open-23.3.1/setup.py
```

### Comparing `backend.ai-accelerator-cuda-open-23.3.0a4/PKG-INFO` & `backend.ai-accelerator-cuda-open-23.3.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: backend.ai-accelerator-cuda-open
-Version: 23.3.0a4
+Version: 23.3.1
 Summary: Backend.AI Accelerator Plugin for CUDA
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
 
 Backend.AI Accelerator Plugin for CUDA
 ======================================
```

### Comparing `backend.ai-accelerator-cuda-open-23.3.0a4/ai/backend/accelerator/cuda_open/nvidia.py` & `backend.ai-accelerator-cuda-open-23.3.1/ai/backend/accelerator/cuda_open/nvidia.py`

 * *Files identical despite different names*

### Comparing `backend.ai-accelerator-cuda-open-23.3.0a4/ai/backend/accelerator/cuda_open/plugin.py` & `backend.ai-accelerator-cuda-open-23.3.1/ai/backend/accelerator/cuda_open/plugin.py`

 * *Files 1% similar despite different names*

```diff
@@ -163,17 +163,15 @@
             return []
         all_devices = []
         num_devices = libcudart.get_device_count()
         for dev_id in map(lambda idx: DeviceId(str(idx)), range(num_devices)):
             if dev_id in self.device_mask:
                 continue
             raw_info = libcudart.get_device_props(int(dev_id))
-            sysfs_node_path = (
-                "/sys/bus/pci/devices/" f"{raw_info['pciBusID_str'].lower()}/numa_node"
-            )
+            sysfs_node_path = f"/sys/bus/pci/devices/{raw_info['pciBusID_str'].lower()}/numa_node"
             node: Optional[int]
             try:
                 node = int(Path(sysfs_node_path).read_text().strip())
             except OSError:
                 node = None
             dev_uuid, raw_dev_uuid = None, raw_info.get("uuid", None)
             if raw_dev_uuid is not None:
@@ -276,17 +274,15 @@
     ) -> Sequence[ProcessMeasurement]:
         return []
 
     async def create_alloc_map(self) -> AbstractAllocMap:
         devices = await self.list_devices()
         return DiscretePropertyAllocMap(
             device_slots={
-                dev.device_id: (
-                    DeviceSlotInfo(SlotTypes.COUNT, SlotName("cuda.device"), Decimal(1))
-                )
+                dev.device_id: DeviceSlotInfo(SlotTypes.COUNT, SlotName("cuda.device"), Decimal(1))
                 for dev in devices
             },
         )
 
     async def get_hooks(self, distro: str, arch: str) -> Sequence[Path]:
         return []
```

### Comparing `backend.ai-accelerator-cuda-open-23.3.0a4/backend.ai_accelerator_cuda_open.egg-info/PKG-INFO` & `backend.ai-accelerator-cuda-open-23.3.1/backend.ai_accelerator_cuda_open.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: backend.ai-accelerator-cuda-open
-Version: 23.3.0a4
+Version: 23.3.1
 Summary: Backend.AI Accelerator Plugin for CUDA
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
 
 Backend.AI Accelerator Plugin for CUDA
 ======================================
```

### Comparing `backend.ai-accelerator-cuda-open-23.3.0a4/backend.ai_accelerator_cuda_open.egg-info/SOURCES.txt` & `backend.ai-accelerator-cuda-open-23.3.1/backend.ai_accelerator_cuda_open.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `backend.ai-accelerator-cuda-open-23.3.0a4/backend_shim.py` & `backend.ai-accelerator-cuda-open-23.3.1/backend_shim.py`

 * *Files identical despite different names*

### Comparing `backend.ai-accelerator-cuda-open-23.3.0a4/setup.py` & `backend.ai-accelerator-cuda-open-23.3.1/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -11,39 +11,39 @@
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
     'description': 'Backend.AI Accelerator Plugin for CUDA',
     'entry_points': {
         'backendai_accelerator_v21': [
             'cuda = ai.backend.accelerator.cuda_open.plugin:CUDAPlugin',
         ],
     },
     'install_requires': (
         'aiodocker~=0.21.0',
         'aiohttp~=3.8.1',
-        """backend.ai-agent==23.03.0a4
+        """backend.ai-agent==23.03.1
 """,
-        """backend.ai-cli==23.03.0a4
+        """backend.ai-cli==23.03.1
 """,
-        """backend.ai-common==23.03.0a4
+        """backend.ai-common==23.03.1
 """,
-        """backend.ai-kernel-binary==23.03.0a4
+        """backend.ai-kernel-binary==23.03.1
 """,
-        """backend.ai-kernel-helper==23.03.0a4
+        """backend.ai-kernel-helper==23.03.1
 """,
-        """backend.ai-kernel==23.03.0a4
+        """backend.ai-kernel==23.03.1
 """,
-        """backend.ai-plugin==23.03.0a4
+        """backend.ai-plugin==23.03.1
 """,
     ),
     'license': 'LGPLv3',
     'long_description': """Backend.AI Accelerator Plugin for CUDA
 ======================================
 
 Just install this along with Backend.AI agents, using the same virtual environment.
@@ -87,11 +87,11 @@
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

