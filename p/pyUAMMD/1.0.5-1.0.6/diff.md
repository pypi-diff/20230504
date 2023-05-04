# Comparing `tmp/pyUAMMD-1.0.5.tar.gz` & `tmp/pyUAMMD-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyUAMMD-1.0.5.tar", last modified: Thu May  4 18:21:09 2023, max compression
+gzip compressed data, was "pyUAMMD-1.0.6.tar", last modified: Thu May  4 18:27:41 2023, max compression
```

## Comparing `pyUAMMD-1.0.5.tar` & `pyUAMMD-1.0.6.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxrwxr-x   0 pablo     (1000) pablo     (1000)        0 2023-05-04 18:21:09.831189 pyUAMMD-1.0.5/
--rw-rw-r--   0 pablo     (1000) pablo     (1000)     1069 2023-05-03 12:32:56.000000 pyUAMMD-1.0.5/LICENSE
--rw-rw-r--   0 pablo     (1000) pablo     (1000)      158 2023-05-04 16:45:12.000000 pyUAMMD-1.0.5/MANIFEST.in
--rw-rw-r--   0 pablo     (1000) pablo     (1000)      645 2023-05-04 18:21:09.831189 pyUAMMD-1.0.5/PKG-INFO
--rw-rw-r--   0 pablo     (1000) pablo     (1000)        9 2023-05-03 12:32:56.000000 pyUAMMD-1.0.5/README.md
-drwxrwxr-x   0 pablo     (1000) pablo     (1000)        0 2023-05-04 18:21:09.827189 pyUAMMD-1.0.5/pyUAMMD/
-drwxrwxr-x   0 pablo     (1000) pablo     (1000)        0 2023-05-04 18:21:09.831189 pyUAMMD-1.0.5/pyUAMMD/ThirdParty/
--rw-rw-r--   0 pablo     (1000) pablo     (1000)   871200 2023-05-03 13:08:59.000000 pyUAMMD-1.0.5/pyUAMMD/ThirdParty/json.hpp
--rw-rw-r--   0 pablo     (1000) pablo     (1000)     7210 2023-05-03 13:08:59.000000 pyUAMMD-1.0.5/pyUAMMD/ThirdParty/pybind11_json.hpp
--rw-rw-r--   0 pablo     (1000) pablo     (1000)     1081 2023-05-03 16:55:23.000000 pyUAMMD-1.0.5/pyUAMMD/__init__.py
--rw-rw-r--   0 pablo     (1000) pablo     (1000)     4058 2023-05-04 18:20:48.000000 pyUAMMD-1.0.5/pyUAMMD/__main__.py
-drwxrwxr-x   0 pablo     (1000) pablo     (1000)        0 2023-05-04 18:21:09.831189 pyUAMMD-1.0.5/pyUAMMD/appending/
--rw-rw-r--   0 pablo     (1000) pablo     (1000)      316 2023-05-03 12:32:56.000000 pyUAMMD-1.0.5/pyUAMMD/appending/__init__.py
--rw-rw-r--   0 pablo     (1000) pablo     (1000)    12650 2023-05-03 12:32:56.000000 pyUAMMD-1.0.5/pyUAMMD/appending/forceField.py
--rw-rw-r--   0 pablo     (1000) pablo     (1000)     4507 2023-05-03 12:32:56.000000 pyUAMMD-1.0.5/pyUAMMD/appending/glb.py
--rw-rw-r--   0 pablo     (1000) pablo     (1000)     5841 2023-05-03 12:32:56.000000 pyUAMMD-1.0.5/pyUAMMD/appending/integrator.py
--rw-rw-r--   0 pablo     (1000) pablo     (1000)    11469 2023-05-03 12:32:56.000000 pyUAMMD-1.0.5/pyUAMMD/appending/patchyParticles.py
--rw-rw-r--   0 pablo     (1000) pablo     (1000)     6664 2023-05-03 12:32:56.000000 pyUAMMD-1.0.5/pyUAMMD/appending/simulationStep.py
--rw-rw-r--   0 pablo     (1000) pablo     (1000)     3477 2023-05-03 12:32:56.000000 pyUAMMD-1.0.5/pyUAMMD/appending/state.py
--rw-rw-r--   0 pablo     (1000) pablo     (1000)     5514 2023-05-03 12:32:56.000000 pyUAMMD-1.0.5/pyUAMMD/appending/structure.py
--rw-rw-r--   0 pablo     (1000) pablo     (1000)     4291 2023-05-03 12:32:56.000000 pyUAMMD-1.0.5/pyUAMMD/appending/system.py
--rw-rw-r--   0 pablo     (1000) pablo     (1000)     8797 2023-05-03 13:49:08.000000 pyUAMMD-1.0.5/pyUAMMD/simulation.py
-drwxrwxr-x   0 pablo     (1000) pablo     (1000)        0 2023-05-04 18:21:09.831189 pyUAMMD-1.0.5/pyUAMMD/utils/
--rw-rw-r--   0 pablo     (1000) pablo     (1000)        0 2023-05-03 12:32:56.000000 pyUAMMD-1.0.5/pyUAMMD/utils/__init__.py
--rw-rw-r--   0 pablo     (1000) pablo     (1000)      637 2023-05-03 12:32:56.000000 pyUAMMD-1.0.5/pyUAMMD/utils/common.py
-drwxrwxr-x   0 pablo     (1000) pablo     (1000)        0 2023-05-04 18:21:09.831189 pyUAMMD-1.0.5/pyUAMMD/utils/launcher/
--rw-rw-r--   0 pablo     (1000) pablo     (1000)      510 2023-05-03 13:10:11.000000 pyUAMMD-1.0.5/pyUAMMD/utils/launcher/UAMMDlauncher.cu
--rw-rw-r--   0 pablo     (1000) pablo     (1000)        0 2023-05-03 12:32:56.000000 pyUAMMD-1.0.5/pyUAMMD/utils/launcher/__init__.py
-drwxrwxr-x   0 pablo     (1000) pablo     (1000)        0 2023-05-04 18:21:09.831189 pyUAMMD-1.0.5/pyUAMMD/utils/update/
--rw-rw-r--   0 pablo     (1000) pablo     (1000)        0 2023-05-03 12:32:56.000000 pyUAMMD-1.0.5/pyUAMMD/utils/update/__init__.py
--rw-rw-r--   0 pablo     (1000) pablo     (1000)     7266 2023-05-03 12:32:56.000000 pyUAMMD-1.0.5/pyUAMMD/utils/update/groups.py
--rw-rw-r--   0 pablo     (1000) pablo     (1000)     1711 2023-05-03 12:32:56.000000 pyUAMMD-1.0.5/pyUAMMD/utils/update/ids.py
-drwxrwxr-x   0 pablo     (1000) pablo     (1000)        0 2023-05-04 18:21:09.827189 pyUAMMD-1.0.5/pyUAMMD.egg-info/
--rw-rw-r--   0 pablo     (1000) pablo     (1000)      645 2023-05-04 18:21:09.000000 pyUAMMD-1.0.5/pyUAMMD.egg-info/PKG-INFO
--rw-rw-r--   0 pablo     (1000) pablo     (1000)      829 2023-05-04 18:21:09.000000 pyUAMMD-1.0.5/pyUAMMD.egg-info/SOURCES.txt
--rw-rw-r--   0 pablo     (1000) pablo     (1000)        1 2023-05-04 18:21:09.000000 pyUAMMD-1.0.5/pyUAMMD.egg-info/dependency_links.txt
--rw-rw-r--   0 pablo     (1000) pablo     (1000)       27 2023-05-04 18:21:09.000000 pyUAMMD-1.0.5/pyUAMMD.egg-info/requires.txt
--rw-rw-r--   0 pablo     (1000) pablo     (1000)        8 2023-05-04 18:21:09.000000 pyUAMMD-1.0.5/pyUAMMD.egg-info/top_level.txt
--rw-rw-r--   0 pablo     (1000) pablo     (1000)      802 2023-05-04 18:20:56.000000 pyUAMMD-1.0.5/pyproject.toml
--rw-rw-r--   0 pablo     (1000) pablo     (1000)       38 2023-05-04 18:21:09.831189 pyUAMMD-1.0.5/setup.cfg
--rw-rw-r--   0 pablo     (1000) pablo     (1000)     2367 2023-05-03 13:56:01.000000 pyUAMMD-1.0.5/setup.py
+drwxrwxr-x   0 pablo     (1000) pablo     (1000)        0 2023-05-04 18:27:41.243658 pyUAMMD-1.0.6/
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)     1069 2023-05-03 12:32:56.000000 pyUAMMD-1.0.6/LICENSE
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)      158 2023-05-04 16:45:12.000000 pyUAMMD-1.0.6/MANIFEST.in
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)      645 2023-05-04 18:27:41.243658 pyUAMMD-1.0.6/PKG-INFO
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)        9 2023-05-03 12:32:56.000000 pyUAMMD-1.0.6/README.md
+drwxrwxr-x   0 pablo     (1000) pablo     (1000)        0 2023-05-04 18:27:41.243658 pyUAMMD-1.0.6/pyUAMMD/
+drwxrwxr-x   0 pablo     (1000) pablo     (1000)        0 2023-05-04 18:27:41.243658 pyUAMMD-1.0.6/pyUAMMD/ThirdParty/
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)   871200 2023-05-03 13:08:59.000000 pyUAMMD-1.0.6/pyUAMMD/ThirdParty/json.hpp
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)     7210 2023-05-03 13:08:59.000000 pyUAMMD-1.0.6/pyUAMMD/ThirdParty/pybind11_json.hpp
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)     1081 2023-05-03 16:55:23.000000 pyUAMMD-1.0.6/pyUAMMD/__init__.py
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)     3604 2023-05-04 18:26:41.000000 pyUAMMD-1.0.6/pyUAMMD/__main__.py
+drwxrwxr-x   0 pablo     (1000) pablo     (1000)        0 2023-05-04 18:27:41.243658 pyUAMMD-1.0.6/pyUAMMD/appending/
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)      316 2023-05-03 12:32:56.000000 pyUAMMD-1.0.6/pyUAMMD/appending/__init__.py
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)    12650 2023-05-03 12:32:56.000000 pyUAMMD-1.0.6/pyUAMMD/appending/forceField.py
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)     4507 2023-05-03 12:32:56.000000 pyUAMMD-1.0.6/pyUAMMD/appending/glb.py
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)     5841 2023-05-03 12:32:56.000000 pyUAMMD-1.0.6/pyUAMMD/appending/integrator.py
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)    11469 2023-05-03 12:32:56.000000 pyUAMMD-1.0.6/pyUAMMD/appending/patchyParticles.py
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)     6664 2023-05-03 12:32:56.000000 pyUAMMD-1.0.6/pyUAMMD/appending/simulationStep.py
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)     3477 2023-05-03 12:32:56.000000 pyUAMMD-1.0.6/pyUAMMD/appending/state.py
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)     5514 2023-05-03 12:32:56.000000 pyUAMMD-1.0.6/pyUAMMD/appending/structure.py
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)     4291 2023-05-03 12:32:56.000000 pyUAMMD-1.0.6/pyUAMMD/appending/system.py
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)     8797 2023-05-03 13:49:08.000000 pyUAMMD-1.0.6/pyUAMMD/simulation.py
+drwxrwxr-x   0 pablo     (1000) pablo     (1000)        0 2023-05-04 18:27:41.243658 pyUAMMD-1.0.6/pyUAMMD/utils/
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)        0 2023-05-03 12:32:56.000000 pyUAMMD-1.0.6/pyUAMMD/utils/__init__.py
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)      637 2023-05-03 12:32:56.000000 pyUAMMD-1.0.6/pyUAMMD/utils/common.py
+drwxrwxr-x   0 pablo     (1000) pablo     (1000)        0 2023-05-04 18:27:41.243658 pyUAMMD-1.0.6/pyUAMMD/utils/launcher/
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)      510 2023-05-03 13:10:11.000000 pyUAMMD-1.0.6/pyUAMMD/utils/launcher/UAMMDlauncher.cu
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)        0 2023-05-03 12:32:56.000000 pyUAMMD-1.0.6/pyUAMMD/utils/launcher/__init__.py
+drwxrwxr-x   0 pablo     (1000) pablo     (1000)        0 2023-05-04 18:27:41.243658 pyUAMMD-1.0.6/pyUAMMD/utils/update/
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)        0 2023-05-03 12:32:56.000000 pyUAMMD-1.0.6/pyUAMMD/utils/update/__init__.py
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)     7266 2023-05-03 12:32:56.000000 pyUAMMD-1.0.6/pyUAMMD/utils/update/groups.py
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)     1711 2023-05-03 12:32:56.000000 pyUAMMD-1.0.6/pyUAMMD/utils/update/ids.py
+drwxrwxr-x   0 pablo     (1000) pablo     (1000)        0 2023-05-04 18:27:41.243658 pyUAMMD-1.0.6/pyUAMMD.egg-info/
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)      645 2023-05-04 18:27:41.000000 pyUAMMD-1.0.6/pyUAMMD.egg-info/PKG-INFO
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)      829 2023-05-04 18:27:41.000000 pyUAMMD-1.0.6/pyUAMMD.egg-info/SOURCES.txt
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)        1 2023-05-04 18:27:41.000000 pyUAMMD-1.0.6/pyUAMMD.egg-info/dependency_links.txt
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)       27 2023-05-04 18:27:41.000000 pyUAMMD-1.0.6/pyUAMMD.egg-info/requires.txt
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)        8 2023-05-04 18:27:41.000000 pyUAMMD-1.0.6/pyUAMMD.egg-info/top_level.txt
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)      802 2023-05-04 18:26:49.000000 pyUAMMD-1.0.6/pyproject.toml
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)       38 2023-05-04 18:27:41.243658 pyUAMMD-1.0.6/setup.cfg
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)     2367 2023-05-03 13:56:01.000000 pyUAMMD-1.0.6/setup.py
```

### Comparing `pyUAMMD-1.0.5/LICENSE` & `pyUAMMD-1.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `pyUAMMD-1.0.5/PKG-INFO` & `pyUAMMD-1.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyUAMMD
-Version: 1.0.5
+Version: 1.0.6
 Summary: UAMMD python
 Home-page: https://github.com/PabloIbannez/pyUAMMD
 Author-email: Pablo Ibáñez-Freire <p.ibanez.fre@gmail.com>
 License: MIT License
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `pyUAMMD-1.0.5/pyUAMMD/ThirdParty/json.hpp` & `pyUAMMD-1.0.6/pyUAMMD/ThirdParty/json.hpp`

 * *Files identical despite different names*

### Comparing `pyUAMMD-1.0.5/pyUAMMD/ThirdParty/pybind11_json.hpp` & `pyUAMMD-1.0.6/pyUAMMD/ThirdParty/pybind11_json.hpp`

 * *Files identical despite different names*

### Comparing `pyUAMMD-1.0.5/pyUAMMD/__init__.py` & `pyUAMMD-1.0.6/pyUAMMD/__init__.py`

 * *Files identical despite different names*

### Comparing `pyUAMMD-1.0.5/pyUAMMD/__main__.py` & `pyUAMMD-1.0.6/pyUAMMD/__main__.py`

 * *Files 14% similar despite different names*

```diff
@@ -22,23 +22,16 @@
                                                             the UAMMD and UAMMD-structured library")
 
     group.add_argument("--libraries", action="store_true",help="Print the libraries used to link \
                                                                 the UAMMD and UAMMD-structured library")
 
     group.add_argument("--cuda", action="store_true",help="Print the CUDA path")
 
-    #Add arch optional argument
-    parser.add_argument("--arch", type=str, help="CUDA architecture to compile for")
-
     args = parser.parse_args()
 
-    if args.arch and not args.flags:
-        logger.error("The architecture can only be set when printing the flags")
-        raise RuntimeError("Incompatible arguments")
-
     if args.includers:
 
         # Try to import read environment variables UAMMD_PATH and UAMMD_STRUCTURED_PATH
         try:
 
             UAMMD_PATH = os.environ['UAMMD_PATH']
 
@@ -76,26 +69,25 @@
     elif args.flags:
 
         try:
 
             NVCC_PATH = os.path.join(find_cuda_home_path(), 'bin', 'nvcc')
 
             gencode = []
-            if args.arch:
-                gencode.append(['-gencode',f'=arch=compute_{args.arch},code=sm_{args.arch}'])
-            else:
-                # Get the current list gpu capturing nvcc output
-                p = subprocess.Popen([NVCC_PATH, '--list-gpu-code'], stdout=subprocess.PIPE, stderr=subprocess.PIPE)
-                out, err = p.communicate()
 
-                archs = out.decode('utf-8').split('\n')[0:-1]
-                archs = [arch.split("_")[-1] for arch in archs]
+            # Get the current list gpu capturing nvcc output
+            p = subprocess.Popen([NVCC_PATH, '--list-gpu-code'], stdout=subprocess.PIPE, stderr=subprocess.PIPE)
+            out, err = p.communicate()
+
+            archs = out.decode('utf-8').split('\n')[0:-1]
+            archs = [arch.split("_")[-1] for arch in archs]
+
+            for arch in archs:
+                gencode += ['-gencode',f'arch=compute_{arch},code=sm_{arch}']
 
-                for arch in archs:
-                    gencode += ['-gencode',f'arch=compute_{arch},code=sm_{arch}']
         except:
             raise RuntimeError('Could not run nvcc')
 
         FLAGS = ['--expt-relaxed-constexpr',
                  '--expt-extended-lambda',
                  '-std=c++14',
                  '-O3',
```

### Comparing `pyUAMMD-1.0.5/pyUAMMD/appending/forceField.py` & `pyUAMMD-1.0.6/pyUAMMD/appending/forceField.py`

 * *Files identical despite different names*

### Comparing `pyUAMMD-1.0.5/pyUAMMD/appending/glb.py` & `pyUAMMD-1.0.6/pyUAMMD/appending/glb.py`

 * *Files identical despite different names*

### Comparing `pyUAMMD-1.0.5/pyUAMMD/appending/integrator.py` & `pyUAMMD-1.0.6/pyUAMMD/appending/integrator.py`

 * *Files identical despite different names*

### Comparing `pyUAMMD-1.0.5/pyUAMMD/appending/patchyParticles.py` & `pyUAMMD-1.0.6/pyUAMMD/appending/patchyParticles.py`

 * *Files identical despite different names*

### Comparing `pyUAMMD-1.0.5/pyUAMMD/appending/simulationStep.py` & `pyUAMMD-1.0.6/pyUAMMD/appending/simulationStep.py`

 * *Files identical despite different names*

### Comparing `pyUAMMD-1.0.5/pyUAMMD/appending/state.py` & `pyUAMMD-1.0.6/pyUAMMD/appending/state.py`

 * *Files identical despite different names*

### Comparing `pyUAMMD-1.0.5/pyUAMMD/appending/structure.py` & `pyUAMMD-1.0.6/pyUAMMD/appending/structure.py`

 * *Files identical despite different names*

### Comparing `pyUAMMD-1.0.5/pyUAMMD/appending/system.py` & `pyUAMMD-1.0.6/pyUAMMD/appending/system.py`

 * *Files identical despite different names*

### Comparing `pyUAMMD-1.0.5/pyUAMMD/simulation.py` & `pyUAMMD-1.0.6/pyUAMMD/simulation.py`

 * *Files identical despite different names*

### Comparing `pyUAMMD-1.0.5/pyUAMMD/utils/common.py` & `pyUAMMD-1.0.6/pyUAMMD/utils/common.py`

 * *Files identical despite different names*

### Comparing `pyUAMMD-1.0.5/pyUAMMD/utils/update/groups.py` & `pyUAMMD-1.0.6/pyUAMMD/utils/update/groups.py`

 * *Files identical despite different names*

### Comparing `pyUAMMD-1.0.5/pyUAMMD/utils/update/ids.py` & `pyUAMMD-1.0.6/pyUAMMD/utils/update/ids.py`

 * *Files identical despite different names*

### Comparing `pyUAMMD-1.0.5/pyUAMMD.egg-info/PKG-INFO` & `pyUAMMD-1.0.6/pyUAMMD.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyUAMMD
-Version: 1.0.5
+Version: 1.0.6
 Summary: UAMMD python
 Home-page: https://github.com/PabloIbannez/pyUAMMD
 Author-email: Pablo Ibáñez-Freire <p.ibanez.fre@gmail.com>
 License: MIT License
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `pyUAMMD-1.0.5/pyUAMMD.egg-info/SOURCES.txt` & `pyUAMMD-1.0.6/pyUAMMD.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyUAMMD-1.0.5/pyproject.toml` & `pyUAMMD-1.0.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools-cuda-cpp", "setuptools", "pybind11"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name="pyUAMMD"
-version="1.0.5"
+version="1.0.6"
 authors = [
     {name = "Pablo Ibáñez-Freire", email = "p.ibanez.fre@gmail.com"},
 ]
 description = "UAMMD python"
 readme = "README.md"
 requires-python = ">=3.7"
 license = {text = "MIT License"}
```

### Comparing `pyUAMMD-1.0.5/setup.py` & `pyUAMMD-1.0.6/setup.py`

 * *Files identical despite different names*

