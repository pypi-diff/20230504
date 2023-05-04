# Comparing `tmp/safe-pysha3-1.0.3.tar.gz` & `tmp/safe-pysha3-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "safe-pysha3-1.0.3.tar", last modified: Thu Nov  3 16:28:57 2022, max compression
+gzip compressed data, was "safe-pysha3-1.0.4.tar", last modified: Thu May  4 10:35:20 2023, max compression
```

## Comparing `safe-pysha3-1.0.3.tar` & `safe-pysha3-1.0.4.tar`

### file list

```diff
@@ -1,55 +1,55 @@
-drwxr-xr-x   0 uxio      (1000) uxio      (1000)        0 2022-11-03 16:28:57.363574 safe-pysha3-1.0.3/
--rw-r--r--   0 uxio      (1000) uxio      (1000)     3317 2022-11-03 15:55:46.000000 safe-pysha3-1.0.3/CHANGES.txt
--rw-r--r--   0 uxio      (1000) uxio      (1000)     2409 2022-11-03 15:46:01.000000 safe-pysha3-1.0.3/LICENSE
--rw-r--r--   0 uxio      (1000) uxio      (1000)      233 2022-11-03 15:55:46.000000 safe-pysha3-1.0.3/MANIFEST.in
--rw-r--r--   0 uxio      (1000) uxio      (1000)     1675 2022-11-03 15:55:46.000000 safe-pysha3-1.0.3/Makefile
-drwxr-xr-x   0 uxio      (1000) uxio      (1000)        0 2022-11-03 16:28:57.356904 safe-pysha3-1.0.3/Modules/
-drwxr-xr-x   0 uxio      (1000) uxio      (1000)        0 2022-11-03 16:28:57.356904 safe-pysha3-1.0.3/Modules/_sha3/
--rw-r--r--   0 uxio      (1000) uxio      (1000)     1832 2022-11-03 15:55:46.000000 safe-pysha3-1.0.3/Modules/_sha3/backport.inc
--rwxr-xr-x   0 uxio      (1000) uxio      (1000)     1498 2022-11-03 15:55:46.000000 safe-pysha3-1.0.3/Modules/_sha3/cleanup.py
-drwxr-xr-x   0 uxio      (1000) uxio      (1000)        0 2022-11-03 16:28:57.356904 safe-pysha3-1.0.3/Modules/_sha3/clinic/
--rw-r--r--   0 uxio      (1000) uxio      (1000)     4099 2022-11-03 15:55:46.000000 safe-pysha3-1.0.3/Modules/_sha3/clinic/sha3module.c.h
-drwxr-xr-x   0 uxio      (1000) uxio      (1000)        0 2022-11-03 16:28:57.363574 safe-pysha3-1.0.3/Modules/_sha3/kcp/
--rw-r--r--   0 uxio      (1000) uxio      (1000)     3269 2022-11-03 15:55:46.000000 safe-pysha3-1.0.3/Modules/_sha3/kcp/KeccakHash.c
--rw-r--r--   0 uxio      (1000) uxio      (1000)     5482 2022-11-03 15:55:46.000000 safe-pysha3-1.0.3/Modules/_sha3/kcp/KeccakHash.h
--rw-r--r--   0 uxio      (1000) uxio      (1000)    70929 2022-11-03 15:55:46.000000 safe-pysha3-1.0.3/Modules/_sha3/kcp/KeccakP-1600-64.macros
--rw-r--r--   0 uxio      (1000) uxio      (1000)     1649 2022-11-03 15:55:46.000000 safe-pysha3-1.0.3/Modules/_sha3/kcp/KeccakP-1600-SnP-opt32.h
--rw-r--r--   0 uxio      (1000) uxio      (1000)     2092 2022-11-03 15:55:46.000000 safe-pysha3-1.0.3/Modules/_sha3/kcp/KeccakP-1600-SnP-opt64.h
--rw-r--r--   0 uxio      (1000) uxio      (1000)      155 2022-11-03 15:55:46.000000 safe-pysha3-1.0.3/Modules/_sha3/kcp/KeccakP-1600-SnP.h
--rw-r--r--   0 uxio      (1000) uxio      (1000)    41475 2022-11-03 15:55:46.000000 safe-pysha3-1.0.3/Modules/_sha3/kcp/KeccakP-1600-inplace32BI.c
--rw-r--r--   0 uxio      (1000) uxio      (1000)      159 2022-11-03 15:55:46.000000 safe-pysha3-1.0.3/Modules/_sha3/kcp/KeccakP-1600-opt64-config.h
--rw-r--r--   0 uxio      (1000) uxio      (1000)    15178 2022-11-03 15:55:46.000000 safe-pysha3-1.0.3/Modules/_sha3/kcp/KeccakP-1600-opt64.c
--rw-r--r--   0 uxio      (1000) uxio      (1000)     6290 2022-11-03 15:55:46.000000 safe-pysha3-1.0.3/Modules/_sha3/kcp/KeccakP-1600-unrolling.macros
--rw-r--r--   0 uxio      (1000) uxio      (1000)     2541 2022-11-03 15:55:46.000000 safe-pysha3-1.0.3/Modules/_sha3/kcp/KeccakSponge.c
--rw-r--r--   0 uxio      (1000) uxio      (1000)     8992 2022-11-03 15:55:46.000000 safe-pysha3-1.0.3/Modules/_sha3/kcp/KeccakSponge.h
--rw-r--r--   0 uxio      (1000) uxio      (1000)    11232 2022-11-03 15:55:46.000000 safe-pysha3-1.0.3/Modules/_sha3/kcp/KeccakSponge.inc
--rw-r--r--   0 uxio      (1000) uxio      (1000)     9530 2022-11-03 15:55:46.000000 safe-pysha3-1.0.3/Modules/_sha3/kcp/PlSnP-Fallback.inc
--rw-r--r--   0 uxio      (1000) uxio      (1000)     5959 2022-11-03 15:55:46.000000 safe-pysha3-1.0.3/Modules/_sha3/kcp/SnP-Relaned.h
--rw-r--r--   0 uxio      (1000) uxio      (1000)      940 2022-11-03 15:55:46.000000 safe-pysha3-1.0.3/Modules/_sha3/kcp/align.h
--rw-r--r--   0 uxio      (1000) uxio      (1000)     5546 2022-11-03 15:55:46.000000 safe-pysha3-1.0.3/Modules/_sha3/kcp/brg_endian.h
--rw-r--r--   0 uxio      (1000) uxio      (1000)    23801 2022-11-03 16:08:08.000000 safe-pysha3-1.0.3/Modules/_sha3/sha3module.c
--rw-r--r--   0 uxio      (1000) uxio      (1000)     2251 2022-11-03 15:55:46.000000 safe-pysha3-1.0.3/Modules/hashlib.h
--rw-r--r--   0 uxio      (1000) uxio      (1000)     3020 2022-11-03 15:55:46.000000 safe-pysha3-1.0.3/Modules/pymemsets.c
--rw-r--r--   0 uxio      (1000) uxio      (1000)      492 2022-11-03 15:55:46.000000 safe-pysha3-1.0.3/Modules/pymemsets.h
--rw-r--r--   0 uxio      (1000) uxio      (1000)     6894 2022-11-03 16:28:57.363574 safe-pysha3-1.0.3/PKG-INFO
--rw-r--r--   0 uxio      (1000) uxio      (1000)     2388 2022-11-03 15:55:46.000000 safe-pysha3-1.0.3/README.txt
-drwxr-xr-x   0 uxio      (1000) uxio      (1000)        0 2022-11-03 16:28:57.363574 safe-pysha3-1.0.3/safe_pysha3.egg-info/
--rw-r--r--   0 uxio      (1000) uxio      (1000)     6894 2022-11-03 16:28:57.000000 safe-pysha3-1.0.3/safe_pysha3.egg-info/PKG-INFO
--rw-r--r--   0 uxio      (1000) uxio      (1000)     1241 2022-11-03 16:28:57.000000 safe-pysha3-1.0.3/safe_pysha3.egg-info/SOURCES.txt
--rw-r--r--   0 uxio      (1000) uxio      (1000)        1 2022-11-03 16:28:57.000000 safe-pysha3-1.0.3/safe_pysha3.egg-info/dependency_links.txt
--rw-r--r--   0 uxio      (1000) uxio      (1000)       13 2022-11-03 16:28:57.000000 safe-pysha3-1.0.3/safe_pysha3.egg-info/top_level.txt
--rw-r--r--   0 uxio      (1000) uxio      (1000)       38 2022-11-03 16:28:57.363574 safe-pysha3-1.0.3/setup.cfg
--rw-r--r--   0 uxio      (1000) uxio      (1000)     3997 2022-11-03 16:28:13.000000 safe-pysha3-1.0.3/setup.py
--rw-r--r--   0 uxio      (1000) uxio      (1000)      746 2022-11-03 15:55:46.000000 safe-pysha3-1.0.3/sha3.py
--rw-r--r--   0 uxio      (1000) uxio      (1000)    11092 2022-11-03 15:55:46.000000 safe-pysha3-1.0.3/tests.py
-drwxr-xr-x   0 uxio      (1000) uxio      (1000)        0 2022-11-03 16:28:57.363574 safe-pysha3-1.0.3/vectors/
--rw-r--r--   0 uxio      (1000) uxio      (1000)    80156 2022-11-03 15:55:46.000000 safe-pysha3-1.0.3/vectors/keccak_224.txt
--rw-r--r--   0 uxio      (1000) uxio      (1000)    82204 2022-11-03 15:55:46.000000 safe-pysha3-1.0.3/vectors/keccak_256.txt
--rw-r--r--   0 uxio      (1000) uxio      (1000)    90396 2022-11-03 15:55:46.000000 safe-pysha3-1.0.3/vectors/keccak_384.txt
--rw-r--r--   0 uxio      (1000) uxio      (1000)    98588 2022-11-03 15:55:46.000000 safe-pysha3-1.0.3/vectors/keccak_512.txt
--rw-r--r--   0 uxio      (1000) uxio      (1000)    80161 2022-11-03 15:55:46.000000 safe-pysha3-1.0.3/vectors/sha3_224.txt
--rw-r--r--   0 uxio      (1000) uxio      (1000)    82209 2022-11-03 15:55:46.000000 safe-pysha3-1.0.3/vectors/sha3_256.txt
--rw-r--r--   0 uxio      (1000) uxio      (1000)    90401 2022-11-03 15:55:46.000000 safe-pysha3-1.0.3/vectors/sha3_384.txt
--rw-r--r--   0 uxio      (1000) uxio      (1000)    98593 2022-11-03 15:55:46.000000 safe-pysha3-1.0.3/vectors/sha3_512.txt
--rw-r--r--   0 uxio      (1000) uxio      (1000)   327969 2022-11-03 15:55:46.000000 safe-pysha3-1.0.3/vectors/shake_128.txt
--rw-r--r--   0 uxio      (1000) uxio      (1000)   327969 2022-11-03 15:55:46.000000 safe-pysha3-1.0.3/vectors/shake_256.txt
+drwxr-xr-x   0 uxio      (1000) users      (985)        0 2023-05-04 10:35:20.314441 safe-pysha3-1.0.4/
+-rw-r--r--   0 uxio      (1000) users      (985)     3317 2023-05-04 09:53:54.000000 safe-pysha3-1.0.4/CHANGES.txt
+-rw-r--r--   0 uxio      (1000) users      (985)     2409 2023-05-04 09:53:54.000000 safe-pysha3-1.0.4/LICENSE
+-rw-r--r--   0 uxio      (1000) users      (985)      233 2023-05-04 09:53:54.000000 safe-pysha3-1.0.4/MANIFEST.in
+-rw-r--r--   0 uxio      (1000) users      (985)     1675 2023-05-04 09:53:54.000000 safe-pysha3-1.0.4/Makefile
+drwxr-xr-x   0 uxio      (1000) users      (985)        0 2023-05-04 10:35:20.311107 safe-pysha3-1.0.4/Modules/
+drwxr-xr-x   0 uxio      (1000) users      (985)        0 2023-05-04 10:35:20.311107 safe-pysha3-1.0.4/Modules/_sha3/
+-rw-r--r--   0 uxio      (1000) users      (985)     1832 2023-05-04 09:53:54.000000 safe-pysha3-1.0.4/Modules/_sha3/backport.inc
+-rwxr-xr-x   0 uxio      (1000) users      (985)     1498 2023-05-04 09:53:54.000000 safe-pysha3-1.0.4/Modules/_sha3/cleanup.py
+drwxr-xr-x   0 uxio      (1000) users      (985)        0 2023-05-04 10:35:20.311107 safe-pysha3-1.0.4/Modules/_sha3/clinic/
+-rw-r--r--   0 uxio      (1000) users      (985)     4099 2023-05-04 09:53:54.000000 safe-pysha3-1.0.4/Modules/_sha3/clinic/sha3module.c.h
+drwxr-xr-x   0 uxio      (1000) users      (985)        0 2023-05-04 10:35:20.311107 safe-pysha3-1.0.4/Modules/_sha3/kcp/
+-rw-r--r--   0 uxio      (1000) users      (985)     3269 2023-05-04 09:53:54.000000 safe-pysha3-1.0.4/Modules/_sha3/kcp/KeccakHash.c
+-rw-r--r--   0 uxio      (1000) users      (985)     5482 2023-05-04 09:53:54.000000 safe-pysha3-1.0.4/Modules/_sha3/kcp/KeccakHash.h
+-rw-r--r--   0 uxio      (1000) users      (985)    70929 2023-05-04 09:53:54.000000 safe-pysha3-1.0.4/Modules/_sha3/kcp/KeccakP-1600-64.macros
+-rw-r--r--   0 uxio      (1000) users      (985)     1649 2023-05-04 09:53:54.000000 safe-pysha3-1.0.4/Modules/_sha3/kcp/KeccakP-1600-SnP-opt32.h
+-rw-r--r--   0 uxio      (1000) users      (985)     2092 2023-05-04 09:53:54.000000 safe-pysha3-1.0.4/Modules/_sha3/kcp/KeccakP-1600-SnP-opt64.h
+-rw-r--r--   0 uxio      (1000) users      (985)      155 2023-05-04 09:53:54.000000 safe-pysha3-1.0.4/Modules/_sha3/kcp/KeccakP-1600-SnP.h
+-rw-r--r--   0 uxio      (1000) users      (985)    41475 2023-05-04 09:53:54.000000 safe-pysha3-1.0.4/Modules/_sha3/kcp/KeccakP-1600-inplace32BI.c
+-rw-r--r--   0 uxio      (1000) users      (985)      159 2023-05-04 09:53:54.000000 safe-pysha3-1.0.4/Modules/_sha3/kcp/KeccakP-1600-opt64-config.h
+-rw-r--r--   0 uxio      (1000) users      (985)    15178 2023-05-04 09:53:54.000000 safe-pysha3-1.0.4/Modules/_sha3/kcp/KeccakP-1600-opt64.c
+-rw-r--r--   0 uxio      (1000) users      (985)     6290 2023-05-04 09:53:54.000000 safe-pysha3-1.0.4/Modules/_sha3/kcp/KeccakP-1600-unrolling.macros
+-rw-r--r--   0 uxio      (1000) users      (985)     2541 2023-05-04 09:58:23.000000 safe-pysha3-1.0.4/Modules/_sha3/kcp/KeccakSponge.c
+-rw-r--r--   0 uxio      (1000) users      (985)     8992 2023-05-04 09:58:25.000000 safe-pysha3-1.0.4/Modules/_sha3/kcp/KeccakSponge.h
+-rw-r--r--   0 uxio      (1000) users      (985)    11249 2023-05-04 10:34:06.000000 safe-pysha3-1.0.4/Modules/_sha3/kcp/KeccakSponge.inc
+-rw-r--r--   0 uxio      (1000) users      (985)     9530 2023-05-04 09:53:54.000000 safe-pysha3-1.0.4/Modules/_sha3/kcp/PlSnP-Fallback.inc
+-rw-r--r--   0 uxio      (1000) users      (985)     5959 2023-05-04 09:53:54.000000 safe-pysha3-1.0.4/Modules/_sha3/kcp/SnP-Relaned.h
+-rw-r--r--   0 uxio      (1000) users      (985)      940 2023-05-04 09:53:54.000000 safe-pysha3-1.0.4/Modules/_sha3/kcp/align.h
+-rw-r--r--   0 uxio      (1000) users      (985)     5546 2023-05-04 09:53:54.000000 safe-pysha3-1.0.4/Modules/_sha3/kcp/brg_endian.h
+-rw-r--r--   0 uxio      (1000) users      (985)    23801 2023-05-04 09:53:54.000000 safe-pysha3-1.0.4/Modules/_sha3/sha3module.c
+-rw-r--r--   0 uxio      (1000) users      (985)     2251 2023-05-04 09:53:54.000000 safe-pysha3-1.0.4/Modules/hashlib.h
+-rw-r--r--   0 uxio      (1000) users      (985)     3020 2023-05-04 09:53:54.000000 safe-pysha3-1.0.4/Modules/pymemsets.c
+-rw-r--r--   0 uxio      (1000) users      (985)      492 2023-05-04 09:53:54.000000 safe-pysha3-1.0.4/Modules/pymemsets.h
+-rw-r--r--   0 uxio      (1000) users      (985)     6894 2023-05-04 10:35:20.314441 safe-pysha3-1.0.4/PKG-INFO
+-rw-r--r--   0 uxio      (1000) users      (985)     2388 2023-05-04 09:53:54.000000 safe-pysha3-1.0.4/README.txt
+drwxr-xr-x   0 uxio      (1000) users      (985)        0 2023-05-04 10:35:20.314441 safe-pysha3-1.0.4/safe_pysha3.egg-info/
+-rw-r--r--   0 uxio      (1000) users      (985)     6894 2023-05-04 10:35:20.000000 safe-pysha3-1.0.4/safe_pysha3.egg-info/PKG-INFO
+-rw-r--r--   0 uxio      (1000) users      (985)     1241 2023-05-04 10:35:20.000000 safe-pysha3-1.0.4/safe_pysha3.egg-info/SOURCES.txt
+-rw-r--r--   0 uxio      (1000) users      (985)        1 2023-05-04 10:35:20.000000 safe-pysha3-1.0.4/safe_pysha3.egg-info/dependency_links.txt
+-rw-r--r--   0 uxio      (1000) users      (985)       13 2023-05-04 10:35:20.000000 safe-pysha3-1.0.4/safe_pysha3.egg-info/top_level.txt
+-rw-r--r--   0 uxio      (1000) users      (985)       38 2023-05-04 10:35:20.314441 safe-pysha3-1.0.4/setup.cfg
+-rw-r--r--   0 uxio      (1000) users      (985)     3997 2023-05-04 10:34:06.000000 safe-pysha3-1.0.4/setup.py
+-rw-r--r--   0 uxio      (1000) users      (985)      746 2023-05-04 09:53:54.000000 safe-pysha3-1.0.4/sha3.py
+-rw-r--r--   0 uxio      (1000) users      (985)    11092 2023-05-04 09:53:54.000000 safe-pysha3-1.0.4/tests.py
+drwxr-xr-x   0 uxio      (1000) users      (985)        0 2023-05-04 10:35:20.314441 safe-pysha3-1.0.4/vectors/
+-rw-r--r--   0 uxio      (1000) users      (985)    80156 2023-05-04 09:53:54.000000 safe-pysha3-1.0.4/vectors/keccak_224.txt
+-rw-r--r--   0 uxio      (1000) users      (985)    82204 2023-05-04 09:53:54.000000 safe-pysha3-1.0.4/vectors/keccak_256.txt
+-rw-r--r--   0 uxio      (1000) users      (985)    90396 2023-05-04 09:53:54.000000 safe-pysha3-1.0.4/vectors/keccak_384.txt
+-rw-r--r--   0 uxio      (1000) users      (985)    98588 2023-05-04 09:53:54.000000 safe-pysha3-1.0.4/vectors/keccak_512.txt
+-rw-r--r--   0 uxio      (1000) users      (985)    80161 2023-05-04 09:53:54.000000 safe-pysha3-1.0.4/vectors/sha3_224.txt
+-rw-r--r--   0 uxio      (1000) users      (985)    82209 2023-05-04 09:53:54.000000 safe-pysha3-1.0.4/vectors/sha3_256.txt
+-rw-r--r--   0 uxio      (1000) users      (985)    90401 2023-05-04 09:53:54.000000 safe-pysha3-1.0.4/vectors/sha3_384.txt
+-rw-r--r--   0 uxio      (1000) users      (985)    98593 2023-05-04 09:53:54.000000 safe-pysha3-1.0.4/vectors/sha3_512.txt
+-rw-r--r--   0 uxio      (1000) users      (985)   327969 2023-05-04 09:53:54.000000 safe-pysha3-1.0.4/vectors/shake_128.txt
+-rw-r--r--   0 uxio      (1000) users      (985)   327969 2023-05-04 09:53:54.000000 safe-pysha3-1.0.4/vectors/shake_256.txt
```

### Comparing `safe-pysha3-1.0.3/CHANGES.txt` & `safe-pysha3-1.0.4/CHANGES.txt`

 * *Files identical despite different names*

### Comparing `safe-pysha3-1.0.3/LICENSE` & `safe-pysha3-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `safe-pysha3-1.0.3/Makefile` & `safe-pysha3-1.0.4/Makefile`

 * *Files identical despite different names*

### Comparing `safe-pysha3-1.0.3/Modules/_sha3/backport.inc` & `safe-pysha3-1.0.4/Modules/_sha3/backport.inc`

 * *Files identical despite different names*

### Comparing `safe-pysha3-1.0.3/Modules/_sha3/cleanup.py` & `safe-pysha3-1.0.4/Modules/_sha3/cleanup.py`

 * *Files identical despite different names*

### Comparing `safe-pysha3-1.0.3/Modules/_sha3/clinic/sha3module.c.h` & `safe-pysha3-1.0.4/Modules/_sha3/clinic/sha3module.c.h`

 * *Files identical despite different names*

### Comparing `safe-pysha3-1.0.3/Modules/_sha3/kcp/KeccakHash.c` & `safe-pysha3-1.0.4/Modules/_sha3/kcp/KeccakHash.c`

 * *Files identical despite different names*

### Comparing `safe-pysha3-1.0.3/Modules/_sha3/kcp/KeccakHash.h` & `safe-pysha3-1.0.4/Modules/_sha3/kcp/KeccakHash.h`

 * *Files identical despite different names*

### Comparing `safe-pysha3-1.0.3/Modules/_sha3/kcp/KeccakP-1600-64.macros` & `safe-pysha3-1.0.4/Modules/_sha3/kcp/KeccakP-1600-64.macros`

 * *Files identical despite different names*

### Comparing `safe-pysha3-1.0.3/Modules/_sha3/kcp/KeccakP-1600-SnP-opt32.h` & `safe-pysha3-1.0.4/Modules/_sha3/kcp/KeccakP-1600-SnP-opt32.h`

 * *Files identical despite different names*

### Comparing `safe-pysha3-1.0.3/Modules/_sha3/kcp/KeccakP-1600-SnP-opt64.h` & `safe-pysha3-1.0.4/Modules/_sha3/kcp/KeccakP-1600-SnP-opt64.h`

 * *Files identical despite different names*

### Comparing `safe-pysha3-1.0.3/Modules/_sha3/kcp/KeccakP-1600-inplace32BI.c` & `safe-pysha3-1.0.4/Modules/_sha3/kcp/KeccakP-1600-inplace32BI.c`

 * *Files identical despite different names*

### Comparing `safe-pysha3-1.0.3/Modules/_sha3/kcp/KeccakP-1600-opt64.c` & `safe-pysha3-1.0.4/Modules/_sha3/kcp/KeccakP-1600-opt64.c`

 * *Files identical despite different names*

### Comparing `safe-pysha3-1.0.3/Modules/_sha3/kcp/KeccakP-1600-unrolling.macros` & `safe-pysha3-1.0.4/Modules/_sha3/kcp/KeccakP-1600-unrolling.macros`

 * *Files identical despite different names*

### Comparing `safe-pysha3-1.0.3/Modules/_sha3/kcp/KeccakSponge.c` & `safe-pysha3-1.0.4/Modules/_sha3/kcp/KeccakSponge.c`

 * *Files identical despite different names*

### Comparing `safe-pysha3-1.0.3/Modules/_sha3/kcp/KeccakSponge.h` & `safe-pysha3-1.0.4/Modules/_sha3/kcp/KeccakSponge.h`

 * *Files identical despite different names*

### Comparing `safe-pysha3-1.0.3/Modules/_sha3/kcp/KeccakSponge.inc` & `safe-pysha3-1.0.4/Modules/_sha3/kcp/KeccakSponge.inc`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 /*
-Implementation by the Keccak, Keyak and Ketje Teams, namely, Guido Bertoni,
-Joan Daemen, Michaël Peeters, Gilles Van Assche and Ronny Van Keer, hereby
-denoted as "the implementer".
-
-For more information, feedback or questions, please refer to our websites:
-http://keccak.noekeon.org/
-http://keyak.noekeon.org/
-http://ketje.noekeon.org/
+The eXtended Keccak Code Package (XKCP)
+https://github.com/XKCP/XKCP
+
+Keccak, designed by Guido Bertoni, Joan Daemen, Michaël Peeters and Gilles Van Assche.
+
+Implementation by the designers, hereby denoted as "the implementer".
+
+For more information, feedback or questions, please refer to the Keccak Team website:
+https://keccak.team/
 
 To the extent possible under law, the implementer has waived all copyright
 and related or neighboring rights to the source code in this file.
 http://creativecommons.org/publicdomain/zero/1.0/
 */
 
 #define JOIN0(a, b)                     a ## b
@@ -43,24 +44,21 @@
         return 1;
     if ((rate <= 0) || (rate > SnP_width) || ((rate % 8) != 0))
         return 1;
     if (suffix == 0)
         return 1;
 
     /* Initialize the state */
-
     SnP_StaticInitialize();
     SnP_Initialize(state);
 
     /* First, absorb whole blocks */
-
 #ifdef SnP_FastLoop_Absorb
     if (((rateInBytes % (SnP_width/200)) == 0) && (inputByteLen >= rateInBytes)) {
         /* fast lane: whole lane rate */
-
         size_t j;
         j = SnP_FastLoop_Absorb(state, rateInBytes/(SnP_width/200), curInput, inputByteLen);
         curInput += j;
         inputByteLen -= j;
     }
 #endif
     while(inputByteLen >= (size_t)rateInBytes) {
@@ -70,39 +68,34 @@
         SnP_AddBytes(state, curInput, 0, rateInBytes);
         SnP_Permute(state);
         curInput += rateInBytes;
         inputByteLen -= rateInBytes;
     }
 
     /* Then, absorb what remains */
-
     partialBlock = (unsigned int)inputByteLen;
     #ifdef KeccakReference
     displayBytes(1, "Block to be absorbed (part)", curInput, partialBlock);
     #endif
     SnP_AddBytes(state, curInput, 0, partialBlock);
 
     /* Finally, absorb the suffix */
-
     #ifdef KeccakReference
     {
         unsigned char delimitedData1[1];
         delimitedData1[0] = suffix;
         displayBytes(1, "Block to be absorbed (last few bits + first bit of padding)", delimitedData1, 1);
     }
     #endif
     /* Last few bits, whose delimiter coincides with first bit of padding */
-
     SnP_AddByte(state, suffix, partialBlock);
     /* If the first bit of padding is at position rate-1, we need a whole new block for the second bit of padding */
-
     if ((suffix >= 0x80) && (partialBlock == (rateInBytes-1)))
         SnP_Permute(state);
     /* Second bit of padding */
-
     SnP_AddByte(state, 0x80, rateInBytes-1);
     #ifdef KeccakReference
     {
         unsigned char block[SnP_width/8];
         memset(block, 0, SnP_width/8);
         block[rateInBytes-1] = 0x80;
         displayBytes(1, "Second bit of padding", block, rateInBytes);
@@ -110,27 +103,25 @@
     #endif
     SnP_Permute(state);
     #ifdef KeccakReference
     displayText(1, "--- Switching to squeezing phase ---");
     #endif
 
     /* First, output whole blocks */
-
     while(outputByteLen > (size_t)rateInBytes) {
         SnP_ExtractBytes(state, curOutput, 0, rateInBytes);
         SnP_Permute(state);
         #ifdef KeccakReference
         displayBytes(1, "Squeezed block", curOutput, rateInBytes);
         #endif
         curOutput += rateInBytes;
         outputByteLen -= rateInBytes;
     }
 
     /* Finally, output what remains */
-
     partialBlock = (unsigned int)outputByteLen;
     SnP_ExtractBytes(state, curOutput, 0, partialBlock);
     #ifdef KeccakReference
     displayBytes(1, "Squeezed block (part)", curOutput, partialBlock);
     #endif
 
     return 0;
@@ -163,25 +154,22 @@
     unsigned int partialBlock;
     const unsigned char *curData;
     unsigned int rateInBytes = instance->rate/8;
 
     if (instance->squeezing)
         return 1; /* Too late for additional input */
 
-
     i = 0;
     curData = data;
     while(i < dataByteLen) {
-        if ((instance->byteIOIndex == 0) && (dataByteLen >= (i + rateInBytes))) {
+        if ((instance->byteIOIndex == 0) && (dataByteLen-i >= rateInBytes)) {
 #ifdef SnP_FastLoop_Absorb
             /* processing full blocks first */
-
             if ((rateInBytes % (SnP_width/200)) == 0) {
                 /* fast lane: whole lane rate */
-
                 j = SnP_FastLoop_Absorb(instance->state, rateInBytes/(SnP_width/200), curData, dataByteLen - i);
                 i += j;
                 curData += j;
             }
             else {
 #endif
                 for(j=dataByteLen-i; j>=rateInBytes; j-=rateInBytes) {
@@ -195,18 +183,18 @@
                 i = dataByteLen - j;
 #ifdef SnP_FastLoop_Absorb
             }
 #endif
         }
         else {
             /* normal lane: using the message queue */
-
-            partialBlock = (unsigned int)(dataByteLen - i);
-            if (partialBlock+instance->byteIOIndex > rateInBytes)
+            if (dataByteLen-i > rateInBytes-instance->byteIOIndex)
                 partialBlock = rateInBytes-instance->byteIOIndex;
+            else
+                partialBlock = (unsigned int)(dataByteLen - i);
             #ifdef KeccakReference
             displayBytes(1, "Block to be absorbed (part)", curData, partialBlock);
             #endif
             i += partialBlock;
 
             SnP_AddBytes(instance->state, curData, instance->byteIOIndex, partialBlock);
             curData += partialBlock;
@@ -227,31 +215,27 @@
     unsigned int rateInBytes = instance->rate/8;
 
     if (delimitedData == 0)
         return 1;
     if (instance->squeezing)
         return 1; /* Too late for additional input */
 
-
     #ifdef KeccakReference
     {
         unsigned char delimitedData1[1];
         delimitedData1[0] = delimitedData;
         displayBytes(1, "Block to be absorbed (last few bits + first bit of padding)", delimitedData1, 1);
     }
     #endif
     /* Last few bits, whose delimiter coincides with first bit of padding */
-
     SnP_AddByte(instance->state, delimitedData, instance->byteIOIndex);
     /* If the first bit of padding is at position rate-1, we need a whole new block for the second bit of padding */
-
     if ((delimitedData >= 0x80) && (instance->byteIOIndex == (rateInBytes-1)))
         SnP_Permute(instance->state);
     /* Second bit of padding */
-
     SnP_AddByte(instance->state, 0x80, rateInBytes-1);
     #ifdef KeccakReference
     {
         unsigned char block[SnP_width/8];
         memset(block, 0, SnP_width/8);
         block[rateInBytes-1] = 0x80;
         displayBytes(1, "Second bit of padding", block, rateInBytes);
@@ -277,35 +261,35 @@
 
     if (!instance->squeezing)
         SpongeAbsorbLastFewBits(instance, 0x01);
 
     i = 0;
     curData = data;
     while(i < dataByteLen) {
-        if ((instance->byteIOIndex == rateInBytes) && (dataByteLen >= (i + rateInBytes))) {
+        if ((instance->byteIOIndex == rateInBytes) && (dataByteLen-i >= rateInBytes)) {
             for(j=dataByteLen-i; j>=rateInBytes; j-=rateInBytes) {
                 SnP_Permute(instance->state);
                 SnP_ExtractBytes(instance->state, curData, 0, rateInBytes);
                 #ifdef KeccakReference
                 displayBytes(1, "Squeezed block", curData, rateInBytes);
                 #endif
                 curData+=rateInBytes;
             }
             i = dataByteLen - j;
         }
         else {
             /* normal lane: using the message queue */
-
             if (instance->byteIOIndex == rateInBytes) {
                 SnP_Permute(instance->state);
                 instance->byteIOIndex = 0;
             }
-            partialBlock = (unsigned int)(dataByteLen - i);
-            if (partialBlock+instance->byteIOIndex > rateInBytes)
+            if (dataByteLen-i > rateInBytes-instance->byteIOIndex)
                 partialBlock = rateInBytes-instance->byteIOIndex;
+            else
+                partialBlock = (unsigned int)(dataByteLen - i);
             i += partialBlock;
 
             SnP_ExtractBytes(instance->state, curData, instance->byteIOIndex, partialBlock);
             #ifdef KeccakReference
             displayBytes(1, "Squeezed block (part)", curData, partialBlock);
             #endif
             curData += partialBlock;
```

### Comparing `safe-pysha3-1.0.3/Modules/_sha3/kcp/PlSnP-Fallback.inc` & `safe-pysha3-1.0.4/Modules/_sha3/kcp/PlSnP-Fallback.inc`

 * *Files identical despite different names*

### Comparing `safe-pysha3-1.0.3/Modules/_sha3/kcp/SnP-Relaned.h` & `safe-pysha3-1.0.4/Modules/_sha3/kcp/SnP-Relaned.h`

 * *Files identical despite different names*

### Comparing `safe-pysha3-1.0.3/Modules/_sha3/kcp/align.h` & `safe-pysha3-1.0.4/Modules/_sha3/kcp/align.h`

 * *Files identical despite different names*

### Comparing `safe-pysha3-1.0.3/Modules/_sha3/kcp/brg_endian.h` & `safe-pysha3-1.0.4/Modules/_sha3/kcp/brg_endian.h`

 * *Files identical despite different names*

### Comparing `safe-pysha3-1.0.3/Modules/_sha3/sha3module.c` & `safe-pysha3-1.0.4/Modules/_sha3/sha3module.c`

 * *Files identical despite different names*

### Comparing `safe-pysha3-1.0.3/Modules/hashlib.h` & `safe-pysha3-1.0.4/Modules/hashlib.h`

 * *Files identical despite different names*

### Comparing `safe-pysha3-1.0.3/Modules/pymemsets.c` & `safe-pysha3-1.0.4/Modules/pymemsets.c`

 * *Files identical despite different names*

### Comparing `safe-pysha3-1.0.3/PKG-INFO` & `safe-pysha3-1.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: safe-pysha3
-Version: 1.0.3
+Version: 1.0.4
 Summary: SHA-3 (Keccak) for Python 3.9 - 3.11
 Home-page: https://github.com/5afe/pysha3
 Author: Christian Heimes
 Author-email: christian@python.org
 Maintainer: Uxío Fuentefría
 Maintainer-email: uxio@safe.global
 License: PSFL (Keccak: CC0 1.0 Universal)
```

### Comparing `safe-pysha3-1.0.3/README.txt` & `safe-pysha3-1.0.4/README.txt`

 * *Files identical despite different names*

### Comparing `safe-pysha3-1.0.3/safe_pysha3.egg-info/PKG-INFO` & `safe-pysha3-1.0.4/safe_pysha3.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: safe-pysha3
-Version: 1.0.3
+Version: 1.0.4
 Summary: SHA-3 (Keccak) for Python 3.9 - 3.11
 Home-page: https://github.com/5afe/pysha3
 Author: Christian Heimes
 Author-email: christian@python.org
 Maintainer: Uxío Fuentefría
 Maintainer-email: uxio@safe.global
 License: PSFL (Keccak: CC0 1.0 Universal)
```

### Comparing `safe-pysha3-1.0.3/safe_pysha3.egg-info/SOURCES.txt` & `safe-pysha3-1.0.4/safe_pysha3.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `safe-pysha3-1.0.3/setup.py` & `safe-pysha3-1.0.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -85,15 +85,15 @@
 
 with open("CHANGES.txt") as f:
     long_description.append(f.read())
 
 
 setup(
     name="safe-pysha3",
-    version="1.0.3",
+    version="1.0.4",
     ext_modules=exts,
     py_modules=["sha3"],
     cmdclass={"test": TestCommand},
     author="Christian Heimes",
     author_email="christian@python.org",
     maintainer="Uxío Fuentefría",
     maintainer_email="uxio@safe.global",
```

### Comparing `safe-pysha3-1.0.3/sha3.py` & `safe-pysha3-1.0.4/sha3.py`

 * *Files identical despite different names*

### Comparing `safe-pysha3-1.0.3/tests.py` & `safe-pysha3-1.0.4/tests.py`

 * *Files identical despite different names*

### Comparing `safe-pysha3-1.0.3/vectors/keccak_224.txt` & `safe-pysha3-1.0.4/vectors/keccak_224.txt`

 * *Files identical despite different names*

### Comparing `safe-pysha3-1.0.3/vectors/keccak_256.txt` & `safe-pysha3-1.0.4/vectors/keccak_256.txt`

 * *Files identical despite different names*

### Comparing `safe-pysha3-1.0.3/vectors/keccak_384.txt` & `safe-pysha3-1.0.4/vectors/keccak_384.txt`

 * *Files identical despite different names*

### Comparing `safe-pysha3-1.0.3/vectors/keccak_512.txt` & `safe-pysha3-1.0.4/vectors/keccak_512.txt`

 * *Files identical despite different names*

### Comparing `safe-pysha3-1.0.3/vectors/sha3_224.txt` & `safe-pysha3-1.0.4/vectors/sha3_224.txt`

 * *Files identical despite different names*

### Comparing `safe-pysha3-1.0.3/vectors/sha3_256.txt` & `safe-pysha3-1.0.4/vectors/sha3_256.txt`

 * *Files identical despite different names*

### Comparing `safe-pysha3-1.0.3/vectors/sha3_384.txt` & `safe-pysha3-1.0.4/vectors/sha3_384.txt`

 * *Files identical despite different names*

### Comparing `safe-pysha3-1.0.3/vectors/sha3_512.txt` & `safe-pysha3-1.0.4/vectors/sha3_512.txt`

 * *Files identical despite different names*

### Comparing `safe-pysha3-1.0.3/vectors/shake_128.txt` & `safe-pysha3-1.0.4/vectors/shake_128.txt`

 * *Files identical despite different names*

### Comparing `safe-pysha3-1.0.3/vectors/shake_256.txt` & `safe-pysha3-1.0.4/vectors/shake_256.txt`

 * *Files identical despite different names*

