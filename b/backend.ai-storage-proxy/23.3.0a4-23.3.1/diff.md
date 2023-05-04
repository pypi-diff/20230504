# Comparing `tmp/backend.ai-storage-proxy-23.3.0a4.tar.gz` & `tmp/backend.ai-storage-proxy-23.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "backend.ai-storage-proxy-23.3.0a4.tar", last modified: Thu Mar 16 02:53:01 2023, max compression
+gzip compressed data, was "backend.ai-storage-proxy-23.3.1.tar", last modified: Thu May  4 05:10:16 2023, max compression
```

## Comparing `backend.ai-storage-proxy-23.3.0a4.tar` & `backend.ai-storage-proxy-23.3.1.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 02:53:01.772221 backend.ai-storage-proxy-23.3.0a4/
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-03-16 02:53:01.000000 backend.ai-storage-proxy-23.3.0a4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     6674 2023-03-16 02:53:01.772221 backend.ai-storage-proxy-23.3.0a4/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 02:53:01.764221 backend.ai-storage-proxy-23.3.0a4/ai/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 02:53:01.764221 backend.ai-storage-proxy-23.3.0a4/ai/backend/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 02:53:01.768221 backend.ai-storage-proxy-23.3.0a4/ai/backend/storage/
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-03-16 02:53:01.000000 backend.ai-storage-proxy-23.3.0a4/ai/backend/storage/VERSION
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-03-16 02:53:01.000000 backend.ai-storage-proxy-23.3.0a4/ai/backend/storage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6467 2023-03-16 02:53:01.000000 backend.ai-storage-proxy-23.3.0a4/ai/backend/storage/abc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 02:53:01.768221 backend.ai-storage-proxy-23.3.0a4/ai/backend/storage/api/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-16 02:53:01.000000 backend.ai-storage-proxy-23.3.0a4/ai/backend/storage/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13341 2023-03-16 02:53:01.000000 backend.ai-storage-proxy-23.3.0a4/ai/backend/storage/api/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    23438 2023-03-16 02:53:01.000000 backend.ai-storage-proxy-23.3.0a4/ai/backend/storage/api/manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 02:53:01.768221 backend.ai-storage-proxy-23.3.0a4/ai/backend/storage/cephfs/
--rw-r--r--   0 runner    (1001) docker     (123)     3348 2023-03-16 02:53:01.000000 backend.ai-storage-proxy-23.3.0a4/ai/backend/storage/cephfs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3358 2023-03-16 02:53:01.000000 backend.ai-storage-proxy-23.3.0a4/ai/backend/storage/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2025 2023-03-16 02:53:01.000000 backend.ai-storage-proxy-23.3.0a4/ai/backend/storage/context.py
--rw-r--r--   0 runner    (1001) docker     (123)     1034 2023-03-16 02:53:01.000000 backend.ai-storage-proxy-23.3.0a4/ai/backend/storage/exception.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 02:53:01.768221 backend.ai-storage-proxy-23.3.0a4/ai/backend/storage/gpfs/
--rw-r--r--   0 runner    (1001) docker     (123)     6616 2023-03-16 02:53:01.000000 backend.ai-storage-proxy-23.3.0a4/ai/backend/storage/gpfs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      721 2023-03-16 02:53:01.000000 backend.ai-storage-proxy-23.3.0a4/ai/backend/storage/gpfs/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    12362 2023-03-16 02:53:01.000000 backend.ai-storage-proxy-23.3.0a4/ai/backend/storage/gpfs/gpfs_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     5462 2023-03-16 02:53:01.000000 backend.ai-storage-proxy-23.3.0a4/ai/backend/storage/gpfs/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 02:53:01.768221 backend.ai-storage-proxy-23.3.0a4/ai/backend/storage/netapp/
--rw-r--r--   0 runner    (1001) docker     (123)    15694 2023-03-16 02:53:01.000000 backend.ai-storage-proxy-23.3.0a4/ai/backend/storage/netapp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8329 2023-03-16 02:53:01.000000 backend.ai-storage-proxy-23.3.0a4/ai/backend/storage/netapp/netappclient.py
--rw-r--r--   0 runner    (1001) docker     (123)     5332 2023-03-16 02:53:01.000000 backend.ai-storage-proxy-23.3.0a4/ai/backend/storage/netapp/quotamanager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 02:53:01.768221 backend.ai-storage-proxy-23.3.0a4/ai/backend/storage/purestorage/
--rw-r--r--   0 runner    (1001) docker     (123)     9274 2023-03-16 02:53:01.000000 backend.ai-storage-proxy-23.3.0a4/ai/backend/storage/purestorage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4946 2023-03-16 02:53:01.000000 backend.ai-storage-proxy-23.3.0a4/ai/backend/storage/purestorage/purity.py
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-03-16 02:53:01.000000 backend.ai-storage-proxy-23.3.0a4/ai/backend/storage/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     9501 2023-03-16 02:53:01.000000 backend.ai-storage-proxy-23.3.0a4/ai/backend/storage/server.py
--rw-r--r--   0 runner    (1001) docker     (123)     2252 2023-03-16 02:53:01.000000 backend.ai-storage-proxy-23.3.0a4/ai/backend/storage/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     3924 2023-03-16 02:53:01.000000 backend.ai-storage-proxy-23.3.0a4/ai/backend/storage/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 02:53:01.768221 backend.ai-storage-proxy-23.3.0a4/ai/backend/storage/vfs/
--rw-r--r--   0 runner    (1001) docker     (123)    16545 2023-03-16 02:53:01.000000 backend.ai-storage-proxy-23.3.0a4/ai/backend/storage/vfs/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 02:53:01.772221 backend.ai-storage-proxy-23.3.0a4/ai/backend/storage/weka/
--rw-r--r--   0 runner    (1001) docker     (123)     6243 2023-03-16 02:53:01.000000 backend.ai-storage-proxy-23.3.0a4/ai/backend/storage/weka/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      622 2023-03-16 02:53:01.000000 backend.ai-storage-proxy-23.3.0a4/ai/backend/storage/weka/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    12747 2023-03-16 02:53:01.000000 backend.ai-storage-proxy-23.3.0a4/ai/backend/storage/weka/weka_client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 02:53:01.772221 backend.ai-storage-proxy-23.3.0a4/ai/backend/storage/xfs/
--rw-r--r--   0 runner    (1001) docker     (123)    10645 2023-03-16 02:53:01.000000 backend.ai-storage-proxy-23.3.0a4/ai/backend/storage/xfs/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 02:53:01.772221 backend.ai-storage-proxy-23.3.0a4/backend.ai_storage_proxy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6674 2023-03-16 02:53:01.000000 backend.ai-storage-proxy-23.3.0a4/backend.ai_storage_proxy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1342 2023-03-16 02:53:01.000000 backend.ai-storage-proxy-23.3.0a4/backend.ai_storage_proxy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-16 02:53:01.000000 backend.ai-storage-proxy-23.3.0a4/backend.ai_storage_proxy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-16 02:53:01.000000 backend.ai-storage-proxy-23.3.0a4/backend.ai_storage_proxy.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-16 02:53:01.000000 backend.ai-storage-proxy-23.3.0a4/backend.ai_storage_proxy.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      310 2023-03-16 02:53:01.000000 backend.ai-storage-proxy-23.3.0a4/backend.ai_storage_proxy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        3 2023-03-16 02:53:01.000000 backend.ai-storage-proxy-23.3.0a4/backend.ai_storage_proxy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      626 2023-03-16 02:53:01.000000 backend.ai-storage-proxy-23.3.0a4/backend_shim.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-16 02:53:01.772221 backend.ai-storage-proxy-23.3.0a4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     7996 2023-03-16 02:53:01.000000 backend.ai-storage-proxy-23.3.0a4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 05:10:16.954679 backend.ai-storage-proxy-23.3.1/
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-04 05:10:16.000000 backend.ai-storage-proxy-23.3.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     6684 2023-05-04 05:10:16.954679 backend.ai-storage-proxy-23.3.1/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 05:10:16.950679 backend.ai-storage-proxy-23.3.1/ai/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 05:10:16.950679 backend.ai-storage-proxy-23.3.1/ai/backend/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 05:10:16.950679 backend.ai-storage-proxy-23.3.1/ai/backend/storage/
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-04 05:10:16.000000 backend.ai-storage-proxy-23.3.1/ai/backend/storage/VERSION
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-04 05:10:16.000000 backend.ai-storage-proxy-23.3.1/ai/backend/storage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6431 2023-05-04 05:10:16.000000 backend.ai-storage-proxy-23.3.1/ai/backend/storage/abc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 05:10:16.950679 backend.ai-storage-proxy-23.3.1/ai/backend/storage/api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 05:10:16.000000 backend.ai-storage-proxy-23.3.1/ai/backend/storage/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13343 2023-05-04 05:10:16.000000 backend.ai-storage-proxy-23.3.1/ai/backend/storage/api/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23528 2023-05-04 05:10:16.000000 backend.ai-storage-proxy-23.3.1/ai/backend/storage/api/manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 05:10:16.950679 backend.ai-storage-proxy-23.3.1/ai/backend/storage/cephfs/
+-rw-r--r--   0 runner    (1001) docker     (123)     3348 2023-05-04 05:10:16.000000 backend.ai-storage-proxy-23.3.1/ai/backend/storage/cephfs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4629 2023-05-04 05:10:16.000000 backend.ai-storage-proxy-23.3.1/ai/backend/storage/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2025 2023-05-04 05:10:16.000000 backend.ai-storage-proxy-23.3.1/ai/backend/storage/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1034 2023-05-04 05:10:16.000000 backend.ai-storage-proxy-23.3.1/ai/backend/storage/exception.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 05:10:16.950679 backend.ai-storage-proxy-23.3.1/ai/backend/storage/gpfs/
+-rw-r--r--   0 runner    (1001) docker     (123)     6490 2023-05-04 05:10:16.000000 backend.ai-storage-proxy-23.3.1/ai/backend/storage/gpfs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      721 2023-05-04 05:10:16.000000 backend.ai-storage-proxy-23.3.1/ai/backend/storage/gpfs/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12362 2023-05-04 05:10:16.000000 backend.ai-storage-proxy-23.3.1/ai/backend/storage/gpfs/gpfs_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5462 2023-05-04 05:10:16.000000 backend.ai-storage-proxy-23.3.1/ai/backend/storage/gpfs/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 05:10:16.950679 backend.ai-storage-proxy-23.3.1/ai/backend/storage/netapp/
+-rw-r--r--   0 runner    (1001) docker     (123)    14060 2023-05-04 05:10:16.000000 backend.ai-storage-proxy-23.3.1/ai/backend/storage/netapp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8329 2023-05-04 05:10:16.000000 backend.ai-storage-proxy-23.3.1/ai/backend/storage/netapp/netappclient.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5332 2023-05-04 05:10:16.000000 backend.ai-storage-proxy-23.3.1/ai/backend/storage/netapp/quotamanager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 05:10:16.950679 backend.ai-storage-proxy-23.3.1/ai/backend/storage/purestorage/
+-rw-r--r--   0 runner    (1001) docker     (123)     9318 2023-05-04 05:10:16.000000 backend.ai-storage-proxy-23.3.1/ai/backend/storage/purestorage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4946 2023-05-04 05:10:16.000000 backend.ai-storage-proxy-23.3.1/ai/backend/storage/purestorage/purity.py
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-04 05:10:16.000000 backend.ai-storage-proxy-23.3.1/ai/backend/storage/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     8726 2023-05-04 05:10:16.000000 backend.ai-storage-proxy-23.3.1/ai/backend/storage/server.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2252 2023-05-04 05:10:16.000000 backend.ai-storage-proxy-23.3.1/ai/backend/storage/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3924 2023-05-04 05:10:16.000000 backend.ai-storage-proxy-23.3.1/ai/backend/storage/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 05:10:16.950679 backend.ai-storage-proxy-23.3.1/ai/backend/storage/vfs/
+-rw-r--r--   0 runner    (1001) docker     (123)    16485 2023-05-04 05:10:16.000000 backend.ai-storage-proxy-23.3.1/ai/backend/storage/vfs/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 05:10:16.954679 backend.ai-storage-proxy-23.3.1/ai/backend/storage/weka/
+-rw-r--r--   0 runner    (1001) docker     (123)     6243 2023-05-04 05:10:16.000000 backend.ai-storage-proxy-23.3.1/ai/backend/storage/weka/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      622 2023-05-04 05:10:16.000000 backend.ai-storage-proxy-23.3.1/ai/backend/storage/weka/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12747 2023-05-04 05:10:16.000000 backend.ai-storage-proxy-23.3.1/ai/backend/storage/weka/weka_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 05:10:16.954679 backend.ai-storage-proxy-23.3.1/ai/backend/storage/xfs/
+-rw-r--r--   0 runner    (1001) docker     (123)    10645 2023-05-04 05:10:16.000000 backend.ai-storage-proxy-23.3.1/ai/backend/storage/xfs/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 05:10:16.954679 backend.ai-storage-proxy-23.3.1/backend.ai_storage_proxy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6684 2023-05-04 05:10:16.000000 backend.ai-storage-proxy-23.3.1/backend.ai_storage_proxy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1342 2023-05-04 05:10:16.000000 backend.ai-storage-proxy-23.3.1/backend.ai_storage_proxy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 05:10:16.000000 backend.ai-storage-proxy-23.3.1/backend.ai_storage_proxy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 05:10:16.000000 backend.ai-storage-proxy-23.3.1/backend.ai_storage_proxy.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 05:10:16.000000 backend.ai-storage-proxy-23.3.1/backend.ai_storage_proxy.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      308 2023-05-04 05:10:16.000000 backend.ai-storage-proxy-23.3.1/backend.ai_storage_proxy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        3 2023-05-04 05:10:16.000000 backend.ai-storage-proxy-23.3.1/backend.ai_storage_proxy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      626 2023-05-04 05:10:16.000000 backend.ai-storage-proxy-23.3.1/backend_shim.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-04 05:10:16.954679 backend.ai-storage-proxy-23.3.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     8004 2023-05-04 05:10:16.000000 backend.ai-storage-proxy-23.3.1/setup.py
```

### Comparing `backend.ai-storage-proxy-23.3.0a4/PKG-INFO` & `backend.ai-storage-proxy-23.3.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: backend.ai-storage-proxy
-Version: 23.3.0a4
+Version: 23.3.1
 Summary: Backend.AI Storage Proxy
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
 
 # Backend.AI Storage Proxy
 
 Backend.AI Storage Proxy is an RPC daemon to manage vfolders used in Backend.AI agent, with quota and
```

### Comparing `backend.ai-storage-proxy-23.3.0a4/ai/backend/storage/abc.py` & `backend.ai-storage-proxy-23.3.1/ai/backend/storage/abc.py`

 * *Files 1% similar despite different names*

```diff
@@ -86,15 +86,14 @@
     async def delete_vfolder(self, vfid: UUID) -> None:
         pass
 
     @abstractmethod
     async def clone_vfolder(
         self,
         src_vfid: UUID,
-        dst_volume: AbstractVolume,
         dst_vfid: UUID,
         options: VFolderCreationOptions = None,
     ) -> None:
         """
         Create a new vfolder on the destination volume with
         ``exist_ok=True`` option and copy all contents of the source
         vfolder into it, preserving file permissions and timestamps.
```

### Comparing `backend.ai-storage-proxy-23.3.0a4/ai/backend/storage/api/client.py` & `backend.ai-storage-proxy-23.3.1/ai/backend/storage/api/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -132,15 +132,15 @@
         file_path.name.encode("ascii", errors="ignore").decode("ascii").replace('"', r"\"")
     )
     encoded_filename = urllib.parse.quote(file_path.name, encoding="utf-8")
     headers = {
         hdrs.CONTENT_TYPE: "application/octet-stream",
         hdrs.CONTENT_DISPOSITION: " ".join(
             [
-                "attachment;" f'filename="{ascii_filename}";',  # RFC-2616 sec2.2
+                f'attachment;filename="{ascii_filename}";',  # RFC-2616 sec2.2
                 f"filename*=UTF-8''{encoded_filename}",  # RFC-5987
             ],
         ),
     }
     if params["no_cache"]:
         headers[hdrs.CACHE_CONTROL] = "no-store"
     return web.FileResponse(file_path, headers=cast(Mapping[str, str], headers))
@@ -195,15 +195,15 @@
     )
     encoded_filename = urllib.parse.quote(zip_filename, encoding="utf-8")
     response = web.StreamResponse(
         headers={
             hdrs.CONTENT_TYPE: "application/zip",
             hdrs.CONTENT_DISPOSITION: " ".join(
                 [
-                    "attachment;" f'filename="{ascii_filename}";',  # RFC-2616 sec2.2
+                    f'attachment;filename="{ascii_filename}";',  # RFC-2616 sec2.2
                     f"filename*=UTF-8''{encoded_filename}",  # RFC-5987
                 ],
             ),
         },
     )
     await response.prepare(request)
     async for chunk in _iter2aiter(zf):
@@ -294,20 +294,20 @@
 async def tus_options(request: web.Request) -> web.Response:
     """
     Let clients discover the supported features of our tus.io server-side implementation.
     """
     ctx: Context = request.app["ctx"]
     headers = {}
     headers["Access-Control-Allow-Origin"] = "*"
-    headers[
-        "Access-Control-Allow-Headers"
-    ] = "Tus-Resumable, Upload-Length, Upload-Metadata, Upload-Offset, Content-Type"
-    headers[
-        "Access-Control-Expose-Headers"
-    ] = "Tus-Resumable, Upload-Length, Upload-Metadata, Upload-Offset, Content-Type"
+    headers["Access-Control-Allow-Headers"] = (
+        "Tus-Resumable, Upload-Length, Upload-Metadata, Upload-Offset, Content-Type"
+    )
+    headers["Access-Control-Expose-Headers"] = (
+        "Tus-Resumable, Upload-Length, Upload-Metadata, Upload-Offset, Content-Type"
+    )
     headers["Access-Control-Allow-Methods"] = "*"
     headers["Tus-Resumable"] = "1.0.0"
     headers["Tus-Version"] = "1.0.0"
     headers["Tus-Max-Size"] = str(
         int(ctx.local_config["storage-proxy"]["max-upload-size"]),
     )
     headers["X-Content-Type-Options"] = "nosniff"
@@ -329,20 +329,20 @@
                     "type": "https://api.backend.ai/probs/storage/no-such-upload-session",
                 },
             ),
             content_type="application/problem+json",
         )
     headers = {}
     headers["Access-Control-Allow-Origin"] = "*"
-    headers[
-        "Access-Control-Allow-Headers"
-    ] = "Tus-Resumable, Upload-Length, Upload-Metadata, Upload-Offset, Content-Type"
-    headers[
-        "Access-Control-Expose-Headers"
-    ] = "Tus-Resumable, Upload-Length, Upload-Metadata, Upload-Offset, Content-Type"
+    headers["Access-Control-Allow-Headers"] = (
+        "Tus-Resumable, Upload-Length, Upload-Metadata, Upload-Offset, Content-Type"
+    )
+    headers["Access-Control-Expose-Headers"] = (
+        "Tus-Resumable, Upload-Length, Upload-Metadata, Upload-Offset, Content-Type"
+    )
     headers["Access-Control-Allow-Methods"] = "*"
     headers["Cache-Control"] = "no-store"
     headers["Tus-Resumable"] = "1.0.0"
     headers["Upload-Offset"] = str(Path(upload_temp_path).stat().st_size)
     headers["Upload-Length"] = str(token_data["size"])
     return headers
```

### Comparing `backend.ai-storage-proxy-23.3.0a4/ai/backend/storage/api/manager.py` & `backend.ai-storage-proxy-23.3.1/ai/backend/storage/api/manager.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 
 from ai.backend.common import validators as tx
 from ai.backend.common.logging import BraceStyleAdapter
 from ai.backend.storage.exception import ExecutionError
 
 from ..abc import AbstractVolume
 from ..context import Context
-from ..exception import InvalidSubpathError, VFolderNotFoundError
+from ..exception import InvalidSubpathError, StorageProxyError, VFolderNotFoundError
 from ..types import VFolderCreationOptions
 from ..utils import check_params, log_manager_api_entry
 
 log = BraceStyleAdapter(logging.getLogger(__spec__.name))  # type: ignore[name-defined]
 
 
 @web.middleware
@@ -158,29 +158,29 @@
 async def clone_vfolder(request: web.Request) -> web.Response:
     async with check_params(
         request,
         t.Dict(
             {
                 t.Key("src_volume"): t.String(),
                 t.Key("src_vfid"): tx.UUID(),
-                t.Key("dst_volume"): t.String(),
+                t.Key("dst_volume"): t.String() | t.Null,
                 t.Key("dst_vfid"): tx.UUID(),
                 t.Key("options", default=None): t.Null | VFolderCreationOptions.as_trafaret(),
             },
         ),
     ) as params:
         await log_manager_api_entry(log, "clone_vfolder", params)
         ctx: Context = request.app["ctx"]
+        if params["dst_volume"] is not None and params["dst_volume"] != params["src_volume"]:
+            raise StorageProxyError("Cross-volume vfolder cloning is not implemented yet")
         async with ctx.get_volume(params["src_volume"]) as src_volume:
-            async with ctx.get_volume(params["dst_volume"]) as dst_volume:
-                await src_volume.clone_vfolder(
-                    params["src_vfid"],
-                    dst_volume,
-                    params["dst_vfid"],
-                )
+            await src_volume.clone_vfolder(
+                params["src_vfid"],
+                params["dst_vfid"],
+            )
         return web.Response(status=204)
 
 
 async def get_vfolder_mount(request: web.Request) -> web.Response:
     async with check_params(
         request,
         t.Dict(
```

### Comparing `backend.ai-storage-proxy-23.3.0a4/ai/backend/storage/cephfs/__init__.py` & `backend.ai-storage-proxy-23.3.1/ai/backend/storage/cephfs/__init__.py`

 * *Files identical despite different names*

### Comparing `backend.ai-storage-proxy-23.3.0a4/ai/backend/storage/context.py` & `backend.ai-storage-proxy-23.3.1/ai/backend/storage/context.py`

 * *Files identical despite different names*

### Comparing `backend.ai-storage-proxy-23.3.0a4/ai/backend/storage/exception.py` & `backend.ai-storage-proxy-23.3.1/ai/backend/storage/exception.py`

 * *Files identical despite different names*

### Comparing `backend.ai-storage-proxy-23.3.0a4/ai/backend/storage/gpfs/__init__.py` & `backend.ai-storage-proxy-23.3.1/ai/backend/storage/gpfs/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import logging
 from pathlib import Path, PurePath
 from typing import Any, FrozenSet, Mapping, Optional
 from uuid import UUID
 
 from ai.backend.common.logging import BraceStyleAdapter
 from ai.backend.common.types import BinarySize, HardwareMetadata
-from ai.backend.storage.abc import CAP_METRIC, CAP_QUOTA, CAP_VFOLDER, AbstractVolume
+from ai.backend.storage.abc import CAP_METRIC, CAP_QUOTA, CAP_VFOLDER
 from ai.backend.storage.types import FSPerfMetric, FSUsage, VFolderCreationOptions
 from ai.backend.storage.vfs import BaseVolume
 
 from ..exception import VFolderCreationError
 from .exceptions import GPFSJobFailedError, GPFSNoMetricError
 from .gpfs_client import GPFSAPIClient
 
@@ -137,32 +137,30 @@
             except GPFSJobFailedError:
                 await self.api_client.remove_fileset(self.fs, str(vfid))
                 raise VFolderCreationError("Failed to set quota")
 
     async def clone_vfolder(
         self,
         src_vfid: UUID,
-        dst_volume: AbstractVolume,
         dst_vfid: UUID,
         options: Optional[VFolderCreationOptions] = None,
     ) -> None:
-        assert isinstance(dst_volume, GPFSVolume)
-        await dst_volume.create_vfolder(dst_vfid, options=options)
+        await self.create_vfolder(dst_vfid, options=options)
 
-        fs_usage = await dst_volume.get_fs_usage()
+        fs_usage = await self.get_fs_usage()
         vfolder_usage = await self.get_usage(src_vfid)
         if vfolder_usage.used_bytes > fs_usage.capacity_bytes - fs_usage.used_bytes:
             raise VFolderCreationError("Not enough space available for clone")
 
         # TODO: Wait until file operation is done
         await self.api_client.copy_folder(
             self.fs,
             self.mangle_vfpath(src_vfid),
-            dst_volume.fs,
-            dst_volume.mangle_vfpath(dst_vfid),
+            self.fs,
+            self.mangle_vfpath(dst_vfid),
         )
 
     async def delete_vfolder(self, vfid: UUID) -> None:
         await self.api_client.remove_fileset(self.fs, str(vfid))
 
     async def get_quota(self, vfid: UUID) -> BinarySize:
         quotas = await self.api_client.list_fileset_quotas(self.fs, str(vfid))
```

### Comparing `backend.ai-storage-proxy-23.3.0a4/ai/backend/storage/gpfs/exceptions.py` & `backend.ai-storage-proxy-23.3.1/ai/backend/storage/gpfs/exceptions.py`

 * *Files identical despite different names*

### Comparing `backend.ai-storage-proxy-23.3.0a4/ai/backend/storage/gpfs/gpfs_client.py` & `backend.ai-storage-proxy-23.3.1/ai/backend/storage/gpfs/gpfs_client.py`

 * *Files identical despite different names*

### Comparing `backend.ai-storage-proxy-23.3.0a4/ai/backend/storage/gpfs/types.py` & `backend.ai-storage-proxy-23.3.1/ai/backend/storage/gpfs/types.py`

 * *Files identical despite different names*

### Comparing `backend.ai-storage-proxy-23.3.0a4/ai/backend/storage/netapp/__init__.py` & `backend.ai-storage-proxy-23.3.1/ai/backend/storage/netapp/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 from typing import FrozenSet
 from uuid import UUID
 
 import aiofiles
 
 from ai.backend.common.types import BinarySize, HardwareMetadata
 
-from ..abc import CAP_METRIC, CAP_VFHOST_QUOTA, CAP_VFOLDER, AbstractVolume
+from ..abc import CAP_METRIC, CAP_VFHOST_QUOTA, CAP_VFOLDER
 from ..exception import ExecutionError, StorageProxyError, VFolderCreationError
 from ..types import FSPerfMetric, FSUsage, VFolderCreationOptions, VFolderUsage
 from ..vfs import BaseVolume
 from .netappclient import NetAppClient
 from .quotamanager import QuotaManager
 
 
@@ -55,75 +55,74 @@
             password=self.netapp_password,
             svm=str(self.netapp_svm),
             volume_name=self.netapp_volume_name,
         )
 
         # assign qtree info after netapp_client and quotamanager are initiated
         self.netapp_volume_uuid = await self.netapp_client.get_volume_uuid_by_name()
-        default_qtree = await self.get_default_qtree_by_volume_id(
+        default_qtree = await self.netapp_client.get_default_qtree_by_volume_id(
             self.netapp_volume_uuid,
         )
         self.netapp_qtree_name = default_qtree.get(
             "name",
             self.config["netapp_qtree_name"],
         )
-        self.netapp_qtree_id = await self.get_qtree_id_by_name(self.netapp_qtree_name)
+        self.netapp_qtree_id = await self.netapp_client.get_qtree_id_by_name(self.netapp_qtree_name)
 
         # adjust mount path (volume + qtree)
-        self.mount_path = (self.mount_path / Path(self.netapp_qtree_name)).resolve()
+        self.mount_path = (self.mount_path / self.netapp_qtree_name).resolve()
 
     async def get_capabilities(self) -> FrozenSet[str]:
         return frozenset([CAP_VFOLDER, CAP_VFHOST_QUOTA, CAP_METRIC])
 
     async def get_hwinfo(self) -> HardwareMetadata:
         raw_metadata = await self.netapp_client.get_metadata()
-        qtree_info = await self.get_default_qtree_by_volume_id(self.netapp_volume_uuid)
+        qtree_info = await self.netapp_client.get_default_qtree_by_volume_id(
+            self.netapp_volume_uuid
+        )
         self.netapp_qtree_name = qtree_info["name"]
         quota = await self.quota_manager.get_quota_by_qtree_name(self.netapp_qtree_name)
         # add quota in hwinfo
         metadata = {"quota": json.dumps(quota), **raw_metadata}
         return {"status": "healthy", "status_info": None, "metadata": {**metadata}}
 
     async def get_fs_usage(self) -> FSUsage:
         volume_usage = await self.netapp_client.get_usage()
-        qtree_info = await self.get_default_qtree_by_volume_id(self.netapp_volume_uuid)
+        qtree_info = await self.netapp_client.get_default_qtree_by_volume_id(
+            self.netapp_volume_uuid
+        )
         self.netapp_qtree_name = qtree_info["name"]
         quota = await self.quota_manager.get_quota_by_qtree_name(self.netapp_qtree_name)
         space = quota.get("space")
         if space and space.get("hard_limit"):
             capacity_bytes = space["hard_limit"]
         else:
             capacity_bytes = volume_usage["capacity_bytes"]
         return FSUsage(
             capacity_bytes=capacity_bytes,
             used_bytes=volume_usage["used_bytes"],
         )
 
     async def get_performance_metric(self) -> FSPerfMetric:
-        uuid = await self.get_volume_uuid_by_name()
-        volume_info = await self.get_volume_info(uuid)
+        uuid = await self.netapp_client.get_volume_uuid_by_name()
+        volume_info = await self.netapp_client.get_volume_info(uuid)
         metric = volume_info["metric"]
         return FSPerfMetric(
             iops_read=metric["iops"]["read"],
             iops_write=metric["iops"]["write"],
             io_bytes_read=metric["throughput"]["read"],
             io_bytes_write=metric["throughput"]["write"],
             io_usec_read=metric["latency"]["read"],
             io_usec_write=metric["latency"]["write"],
         )
 
     async def delete_vfolder(self, vfid: UUID) -> None:
         vfpath = self.mangle_vfpath(vfid)
-
-        # extract target_dir from vfpath
-        target_dir = str(vfpath).split(self.netapp_qtree_name + "/", 1)[1].split("/")[0]
-        nfs_path = (
-            f"{self.netapp_xcp_hostname}:/{self.netapp_volume_name}/"
-            + f"{self.netapp_qtree_name}/{target_dir}"
-        )
+        vfrelpath = vfpath.relative_to(self.mount_path)
+        nfs_path = f"{self.netapp_xcp_hostname}:/{self.netapp_volume_name}/{vfrelpath}"
 
         async def watch_delete_dir(root_dir):
             delete_cmd = ["xcp", "delete", "-force", nfs_path]
             if self.netapp_xcp_container_name is not None:
                 delete_cmd = [
                     "docker",
                     "exec",
@@ -152,45 +151,34 @@
             await aiofile_os.rmdir(vfpath.parent.parent)
 
         await read_progress(nfs_path)
 
     async def clone_vfolder(
         self,
         src_vfid: UUID,
-        dst_volume: AbstractVolume,
         dst_vfid: UUID,
         options: VFolderCreationOptions = None,
     ) -> None:
         # check if there is enough space in destination
-        fs_usage = await dst_volume.get_fs_usage()
+        fs_usage = await self.get_fs_usage()
         vfolder_usage = await self.get_usage(src_vfid)
         if vfolder_usage.used_bytes > fs_usage.capacity_bytes - fs_usage.used_bytes:
             raise VFolderCreationError("Not enough space available for clone")
 
         # create the target vfolder
-        await dst_volume.create_vfolder(dst_vfid, options=options, exist_ok=True)
+        await self.create_vfolder(dst_vfid, options=options, exist_ok=True)
 
         # arrange directory based on nfs
-        src_vfpath = str(self.mangle_vfpath(src_vfid)).split(
-            self.netapp_qtree_name + "/",
-            1,
-        )[1]
-        dst_vfpath = str(dst_volume.mangle_vfpath(dst_vfid)).split(
-            self.netapp_qtree_name + "/",
-            1,
-        )[1]
-
-        nfs_src_path = (
-            f"{self.netapp_xcp_hostname}:/{self.netapp_volume_name}/"
-            + f"{self.netapp_qtree_name}/{src_vfpath}"
-        )
-        nfs_dst_path = (
-            f"{self.netapp_xcp_hostname}:/{dst_volume.config['netapp_volume_name']}/"
-            + f"{dst_volume.config['netapp_qtree_name']}/{dst_vfpath}"
-        )
+        src_vfpath = self.mangle_vfpath(src_vfid)
+        dst_vfpath = self.mangle_vfpath(dst_vfid)
+        src_vfrelpath = src_vfpath.relative_to(self.mount_path)
+        dst_vfrelpath = dst_vfpath.relative_to(self.mount_path)
+
+        nfs_src_path = f"{self.netapp_xcp_hostname}:/{self.netapp_volume_name}/{src_vfrelpath}"
+        nfs_dst_path = f"{self.netapp_xcp_hostname}:/{self.netapp_volume_name}/{dst_vfrelpath}"
 
         # perform clone using xcp copy (exception handling needed)
         try:
 
             async def watch_copy_dir(src_path, dst_path):
                 copy_cmd = ["xcp", "copy", src_path, dst_path]
                 if self.netapp_xcp_container_name is not None:
@@ -218,78 +206,40 @@
                 async for line in watch_copy_dir(src_path, dst_path):
                     # TODO: line for bgtask
                     pass
 
             await read_progress(nfs_src_path, nfs_dst_path)
 
         except Exception:
-            await dst_volume.delete_vfolder(dst_vfid)
+            await self.delete_vfolder(dst_vfid)
             raise RuntimeError("Copying files from source directories failed.")
 
     async def shutdown(self) -> None:
         await self.netapp_client.aclose()
         await self.quota_manager.aclose()
 
     # ------ volume operations ------
-    async def get_list_volumes(self):
-        resp = await self.netapp_client.get_list_volumes()
-
-        if "error" in resp:
-            raise ExecutionError("api error")
-        return resp
-
-    async def get_volume_uuid_by_name(self):
-        resp = await self.netapp_client.get_volume_uuid_by_name()
-
-        if "error" in resp:
-            raise ExecutionError("api error")
-        return resp
-
-    async def get_volume_info(self, volume_uuid):
-        resp = await self.netapp_client.get_volume_info(volume_uuid)
-
-        if "error" in resp:
-            raise ExecutionError("api error")
-        return resp
 
     # ------ qtree and quotas operations ------
-    async def get_default_qtree_by_volume_id(self, volume_uuid):
-        volume_uuid = volume_uuid if volume_uuid else self.netapp_volume_uuid
-        resp = await self.netapp_client.get_default_qtree_by_volume_id(volume_uuid)
-        if "error" in resp:
-            raise ExecutionError("api error")
-        return resp
-
-    async def get_qtree_id_by_name(self, qtree_name):
-        qtree_name = qtree_name if qtree_name else await self.get_default_qtree_by_volume_id()
-        resp = await self.netapp_client.get_qtree_id_by_name(qtree_name)
-
-        if "error" in resp:
-            raise ExecutionError("api error")
-        return resp
-
     async def get_quota(self, vfid: UUID) -> BinarySize:
         raise NotImplementedError
 
     async def set_quota(self, vfid: UUID, size_bytes: BinarySize) -> None:
         raise NotImplementedError
 
     async def get_usage(
         self,
         vfid: UUID,
         relpath: PurePosixPath = PurePosixPath("."),
     ) -> VFolderUsage:
         target_path = self.sanitize_vfpath(vfid, relpath)
+        target_relpath = target_path.relative_to(self.mount_path)
+        nfs_path = f"{self.netapp_xcp_hostname}:/{self.netapp_volume_name}/{target_relpath}"
         total_size = 0
         total_count = 0
-        raw_target_path = str(target_path).split(self.netapp_qtree_name + "/", 1)[1]
-        nfs_path = (
-            f"{self.netapp_xcp_hostname}:/{self.netapp_volume_name}/"
-            + f"{self.netapp_qtree_name}/{raw_target_path}"
-        )
         start_time = time.monotonic()
         available = True
 
         prev_files_count = 0
         curr_files_count = 0
 
         # check the number of scan result files changed
```

### Comparing `backend.ai-storage-proxy-23.3.0a4/ai/backend/storage/netapp/netappclient.py` & `backend.ai-storage-proxy-23.3.1/ai/backend/storage/netapp/netappclient.py`

 * *Files identical despite different names*

### Comparing `backend.ai-storage-proxy-23.3.0a4/ai/backend/storage/netapp/quotamanager.py` & `backend.ai-storage-proxy-23.3.1/ai/backend/storage/netapp/quotamanager.py`

 * *Files identical despite different names*

### Comparing `backend.ai-storage-proxy-23.3.0a4/ai/backend/storage/purestorage/__init__.py` & `backend.ai-storage-proxy-23.3.1/ai/backend/storage/purestorage/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -34,16 +34,18 @@
                 stdout, stderr = await proc.communicate()
                 if b"RapidFile Toolkit" not in stdout or proc.returncode != 0:
                     available = False
             finally:
                 await proc.wait()
         if not available:
             raise RuntimeError(
-                "PureStorage RapidFile Toolkit is not installed. "
-                "You cannot use the PureStorage backend for the stroage proxy.",
+                (
+                    "PureStorage RapidFile Toolkit is not installed. "
+                    "You cannot use the PureStorage backend for the stroage proxy."
+                ),
             )
         self.purity_client = PurityClient(
             self.config["purity_endpoint"],
             self.config["purity_api_token"],
             api_version=self.config["purity_api_version"],
         )
```

### Comparing `backend.ai-storage-proxy-23.3.0a4/ai/backend/storage/purestorage/purity.py` & `backend.ai-storage-proxy-23.3.1/ai/backend/storage/purestorage/purity.py`

 * *Files identical despite different names*

### Comparing `backend.ai-storage-proxy-23.3.0a4/ai/backend/storage/server.py` & `backend.ai-storage-proxy-23.3.1/ai/backend/storage/server.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,33 +3,33 @@
 import logging
 import multiprocessing
 import os
 import pwd
 import ssl
 import sys
 from pathlib import Path
-from pprint import pformat, pprint
+from pprint import pprint
 from typing import Any, AsyncIterator, Sequence
 
 import aiomonitor
 import aiotools
 import click
 from aiohttp import web
 from setproctitle import setproctitle
 
-from ai.backend.common import config
+from ai.backend.common.config import ConfigurationError, override_key
 from ai.backend.common.etcd import AsyncEtcd, ConfigScopes
 from ai.backend.common.logging import BraceStyleAdapter, Logger
 from ai.backend.common.types import LogSeverity
 from ai.backend.common.utils import env_info
 
 from . import __version__ as VERSION
 from .api.client import init_client_app
 from .api.manager import init_manager_app
-from .config import local_config_iv
+from .config import load_local_config
 from .context import Context
 
 log = BraceStyleAdapter(logging.getLogger(__spec__.name))  # type: ignore[name-defined]
 
 
 @aiotools.server
 async def server_main_logwrapper(loop, pidx, _args):
@@ -154,69 +154,56 @@
 @click.group(invoke_without_command=True)
 @click.option(
     "-f",
     "--config-path",
     "--config",
     type=Path,
     default=None,
-    help="The config file path. "
-    "(default: ./storage-proxy.toml and /etc/backend.ai/storage-proxy.toml)",
+    help=(
+        "The config file path. "
+        "(default: ./storage-proxy.toml and /etc/backend.ai/storage-proxy.toml)"
+    ),
 )
 @click.option(
     "--debug",
     is_flag=True,
     help="This option will soon change to --log-level TEXT option.",
 )
 @click.option(
     "--log-level",
     type=click.Choice(LogSeverity, case_sensitive=False),
     default=LogSeverity.INFO,
     help="Choose logging level from... debug, info, warning, error, critical",
 )
 @click.pass_context
-def main(cli_ctx, config_path, log_level, debug=False):
+def main(
+    cli_ctx,
+    config_path: Path,
+    log_level: LogSeverity,
+    debug: bool = False,
+) -> int:
     if debug:
         click.echo("Please use --log-level options instead")
         click.echo("--debug options will soon change to --log-level TEXT option.")
         log_level = LogSeverity.DEBUG
 
-    # Determine where to read configuration.
-    raw_cfg, cfg_src_path = config.read_from_file(config_path, "storage-proxy")
-
-    config.override_with_env(raw_cfg, ("etcd", "namespace"), "BACKEND_NAMESPACE")
-    config.override_with_env(raw_cfg, ("etcd", "addr"), "BACKEND_ETCD_ADDR")
-    config.override_with_env(raw_cfg, ("etcd", "user"), "BACKEND_ETCD_USER")
-    config.override_with_env(raw_cfg, ("etcd", "password"), "BACKEND_ETCD_PASSWORD")
-    if log_level == LogSeverity.DEBUG:
-        config.override_key(raw_cfg, ("debug", "enabled"), True)
-
     try:
-        local_config = config.check(raw_cfg, local_config_iv)
-        local_config["_src"] = cfg_src_path
-    except config.ConfigurationError as e:
-        print(
-            "ConfigurationError: Validation of agent configuration has failed:",
-            file=sys.stderr,
-        )
-        print(pformat(e.invalid_data), file=sys.stderr)
+        local_config = load_local_config(config_path, debug=debug)
+    except ConfigurationError:
         raise click.Abort()
-
-    config.override_key(local_config, ("logging", "level"), log_level.name)
-    config.override_key(local_config, ("logging", "pkg-ns", "ai.backend"), log_level.name)
-
-    # if os.getuid() != 0:
-    #     print('Storage agent can only be run as root', file=sys.stderr)
-    #     raise click.Abort()
+    override_key(local_config, ("logging", "level"), log_level.name)
+    override_key(local_config, ("logging", "pkg-ns", "ai.backend"), log_level.name)
 
     multiprocessing.set_start_method("spawn")
 
     if cli_ctx.invoked_subcommand is None:
         local_config["storage-proxy"]["pid-file"].write_text(str(os.getpid()))
+        ipc_base_path = local_config["storage-proxy"]["ipc-base-path"]
         log_sockpath = Path(
-            f"/tmp/backend.ai/ipc/storage-proxy-logger-{os.getpid()}.sock",
+            ipc_base_path / f"storage-proxy-logger-{os.getpid()}.sock",
         )
         log_sockpath.parent.mkdir(parents=True, exist_ok=True)
         log_endpoint = f"ipc://{log_sockpath}"
         local_config["logging"]["endpoint"] = log_endpoint
         try:
             logger = Logger(
                 local_config["logging"],
```

### Comparing `backend.ai-storage-proxy-23.3.0a4/ai/backend/storage/types.py` & `backend.ai-storage-proxy-23.3.1/ai/backend/storage/types.py`

 * *Files identical despite different names*

### Comparing `backend.ai-storage-proxy-23.3.0a4/ai/backend/storage/utils.py` & `backend.ai-storage-proxy-23.3.1/ai/backend/storage/utils.py`

 * *Files identical despite different names*

### Comparing `backend.ai-storage-proxy-23.3.0a4/ai/backend/storage/vfs/__init__.py` & `backend.ai-storage-proxy-23.3.1/ai/backend/storage/vfs/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -96,34 +96,33 @@
                 pass
 
         await loop.run_in_executor(None, _delete_vfolder)
 
     async def clone_vfolder(
         self,
         src_vfid: UUID,
-        dst_volume: AbstractVolume,
         dst_vfid: UUID,
         options: VFolderCreationOptions = None,
     ) -> None:
         # check if there is enough space in the destination
-        fs_usage = await dst_volume.get_fs_usage()
+        fs_usage = await self.get_fs_usage()
         vfolder_usage = await self.get_usage(src_vfid)
         if vfolder_usage.used_bytes > fs_usage.capacity_bytes - fs_usage.used_bytes:
             raise ExecutionError("Not enough space available for clone.")
 
         # create the target vfolder
         src_vfpath = self.mangle_vfpath(src_vfid)
-        await dst_volume.create_vfolder(dst_vfid, options=options, exist_ok=True)
-        dst_vfpath = dst_volume.mangle_vfpath(dst_vfid)
+        await self.create_vfolder(dst_vfid, options=options, exist_ok=True)
+        dst_vfpath = self.mangle_vfpath(dst_vfid)
 
         # perform the file-tree copy
         try:
             await self.copy_tree(src_vfpath, dst_vfpath)
         except Exception:
-            await dst_volume.delete_vfolder(dst_vfid)
+            await self.delete_vfolder(dst_vfid)
             log.exception("clone_vfolder: error during copy_tree()")
             raise ExecutionError("Copying files from source directories failed.")
 
     async def copy_tree(
         self,
         src_vfpath: Path,
         dst_vfpath: Path,
```

### Comparing `backend.ai-storage-proxy-23.3.0a4/ai/backend/storage/weka/__init__.py` & `backend.ai-storage-proxy-23.3.1/ai/backend/storage/weka/__init__.py`

 * *Files identical despite different names*

### Comparing `backend.ai-storage-proxy-23.3.0a4/ai/backend/storage/weka/exceptions.py` & `backend.ai-storage-proxy-23.3.1/ai/backend/storage/weka/exceptions.py`

 * *Files identical despite different names*

### Comparing `backend.ai-storage-proxy-23.3.0a4/ai/backend/storage/weka/weka_client.py` & `backend.ai-storage-proxy-23.3.1/ai/backend/storage/weka/weka_client.py`

 * *Files identical despite different names*

### Comparing `backend.ai-storage-proxy-23.3.0a4/ai/backend/storage/xfs/__init__.py` & `backend.ai-storage-proxy-23.3.1/ai/backend/storage/xfs/__init__.py`

 * *Files identical despite different names*

### Comparing `backend.ai-storage-proxy-23.3.0a4/backend.ai_storage_proxy.egg-info/PKG-INFO` & `backend.ai-storage-proxy-23.3.1/backend.ai_storage_proxy.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: backend.ai-storage-proxy
-Version: 23.3.0a4
+Version: 23.3.1
 Summary: Backend.AI Storage Proxy
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
 
 # Backend.AI Storage Proxy
 
 Backend.AI Storage Proxy is an RPC daemon to manage vfolders used in Backend.AI agent, with quota and
```

### Comparing `backend.ai-storage-proxy-23.3.0a4/backend.ai_storage_proxy.egg-info/SOURCES.txt` & `backend.ai-storage-proxy-23.3.1/backend.ai_storage_proxy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `backend.ai-storage-proxy-23.3.0a4/backend_shim.py` & `backend.ai-storage-proxy-23.3.1/backend_shim.py`

 * *Files identical despite different names*

### Comparing `backend.ai-storage-proxy-23.3.0a4/setup.py` & `backend.ai-storage-proxy-23.3.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,27 +11,27 @@
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
     'description': 'Backend.AI Storage Proxy',
     'install_requires': (
         'PyJWT~=2.0',
         'aiofiles~=0.8.0',
         'aiohttp_cors~=0.7',
         'aiohttp~=3.8.1',
-        'aiomonitor-ng~=0.7.0',
-        'aiotools~=1.5.9',
+        'aiomonitor-ng~=0.7.2',
+        'aiotools~=1.6.1',
         'attrs>=20.3',
-        """backend.ai-common==23.03.0a4
+        """backend.ai-common==23.03.1
 """,
         'click>=7.1.2',
         'dataclasses-json~=0.5.7',
         'janus~=1.0.0',
         'setproctitle~=1.2.2',
         'tenacity>=8.0',
         'trafaret~=2.1',
@@ -243,11 +243,11 @@
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

