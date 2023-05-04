# Comparing `tmp/mpipartition-1.0.1.tar.gz` & `tmp/mpipartition-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mpipartition-1.0.1.tar", max compression
+gzip compressed data, was "mpipartition-1.0.2.tar", max compression
```

## Comparing `mpipartition-1.0.1.tar` & `mpipartition-1.0.2.tar`

### file list

```diff
@@ -1,10 +1,9 @@
--rw-r--r--   0        0        0     1076 2022-04-21 01:36:40.763152 mpipartition-1.0.1/LICENSE
--rw-r--r--   0        0        0     3705 2022-04-21 01:36:40.763152 mpipartition-1.0.1/README.rst
--rw-r--r--   0        0        0      274 2022-04-21 01:36:40.767152 mpipartition-1.0.1/mpipartition/__init__.py
--rw-r--r--   0        0        0     4940 2022-04-21 01:36:40.767152 mpipartition-1.0.1/mpipartition/distribute.py
--rw-r--r--   0        0        0    11483 2022-04-21 01:36:40.767152 mpipartition-1.0.1/mpipartition/exchange.py
--rw-r--r--   0        0        0     5050 2022-04-21 01:36:40.767152 mpipartition-1.0.1/mpipartition/overload.py
--rw-r--r--   0        0        0     7435 2022-04-21 01:36:40.767152 mpipartition-1.0.1/mpipartition/partition.py
--rw-r--r--   0        0        0     1291 2022-04-21 01:36:40.767152 mpipartition-1.0.1/pyproject.toml
--rw-r--r--   0        0        0     4561 2022-04-21 01:41:28.697132 mpipartition-1.0.1/setup.py
--rw-r--r--   0        0        0     4867 2022-04-21 01:41:28.697706 mpipartition-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1076 2023-05-04 17:41:44.911113 mpipartition-1.0.2/LICENSE
+-rw-r--r--   0        0        0     3723 2023-05-04 17:41:44.911113 mpipartition-1.0.2/README.rst
+-rw-r--r--   0        0        0      274 2023-05-04 17:41:44.911113 mpipartition-1.0.2/mpipartition/__init__.py
+-rw-r--r--   0        0        0     4942 2023-05-04 17:41:44.911113 mpipartition-1.0.2/mpipartition/distribute.py
+-rw-r--r--   0        0        0    11692 2023-05-04 17:41:44.911113 mpipartition-1.0.2/mpipartition/exchange.py
+-rw-r--r--   0        0        0     5047 2023-05-04 17:41:44.911113 mpipartition-1.0.2/mpipartition/overload.py
+-rw-r--r--   0        0        0     7430 2023-05-04 17:41:44.911113 mpipartition-1.0.2/mpipartition/partition.py
+-rw-r--r--   0        0        0     1291 2023-05-04 17:41:44.911113 mpipartition-1.0.2/pyproject.toml
+-rw-r--r--   0        0        0     4936 1970-01-01 00:00:00.000000 mpipartition-1.0.2/PKG-INFO
```

### Comparing `mpipartition-1.0.1/LICENSE` & `mpipartition-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `mpipartition-1.0.1/README.rst` & `mpipartition-1.0.2/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -45,14 +45,15 @@
    cd mpipartition
    python setup.py develop
 
 
 Requirements
 ------------
 
+* Python >= 3.7
 * `mpi4py <https://mpi4py.readthedocs.io/en/stable/>`_: MPI for Python
 * `numpy <https://numpy.org/>`_: Python array library
 
 
 Basic Usage
 -----------
 Check the `documentation <https://argonnecpac.github.io/MPIPartition>`_ for
@@ -109,17 +110,17 @@
    box_size = 64.  # box size in Mpc/h
    partition = Partition(3)  # by default, the dimension is 3
 
    # read GenericIO data in parallel
    data = pygio.read_genericio("m000p-499.haloproperties")
 
    # distribute
-   data = distribute(partition, box_size, data, [f"fof_halo_center{x}" for x in "xyz"])
+   data = distribute(partition, box_size, data, [f"fof_halo_center_{x}" for x in "xyz"])
 
    # mark "owned" data with rank (allows differentiating owned and overloaded data)
    data["status"] = partition.rank * np.ones(len(data["fof_halo_center_x"]), dtype=np.uint16)
 
    # overload by 4Mpc/h
-   data = overload(partition, box_size, data, 4., [f"fof_halo_center{x}" for x in "xyz"])
+   data = overload(partition, box_size, data, 4., [f"fof_halo_center_{x}" for x in "xyz"])
 
    # now we can do analysis such as 2pt correlation functions (up to 4Mpc/h)
    # or neighbor finding, etc.
```

### Comparing `mpipartition-1.0.1/mpipartition/distribute.py` & `mpipartition-1.0.2/mpipartition/distribute.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,14 @@
-from .partition import Partition, MPI
-from typing import Mapping, List, Union
 import sys
+from typing import List, Mapping, Union
+
 import numpy as np
 
+from .partition import MPI, Partition
+
 ParticleDataT = Mapping[str, np.ndarray]
 
 
 def distribute(
     partition: Partition,
     box_size: float,
     data: ParticleDataT,
```

### Comparing `mpipartition-1.0.1/mpipartition/exchange.py` & `mpipartition-1.0.2/mpipartition/exchange.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,13 @@
-from .partition import Partition
-from typing import Mapping, Union, Callable
-import numpy as np
 import sys
+from typing import Callable, Mapping, Union
+
+import numpy as np
+
+from .partition import Partition
 
 ParticleDataT = Mapping[str, np.ndarray]
 
 
 def exchange(
     partition: Partition,
     data: dict,
@@ -15,18 +17,20 @@
     verbose: bool = False,
     filter_key: Union[int, Callable[[np.ndarray], np.ndarray]] = None,
     do_all2all: bool = False,
     replace_notfound_key: int = None,
 ):
     """Distribute data among neighboring ranks and all2all by a key
 
-    This function will assign data to the rank that owns the key. The keys that the local rank owns are given by
-    ``local_keys``, which should be unique. The keys of the data that the local rank currently has is in ``data[key]``.
-    Certain values can be ignored by setting filter_key to that value or by setting filter_key to a (vectorized) function
-    that returns ``True`` for keys that should be redistributed and ``False`` for keys that should be ignored.
+    This function will assign data to the rank that owns the key. The keys that the
+    local rank owns are given by ``local_keys``, which should be unique. The keys of the
+    data that the local rank currently has is in ``data[key]``. Certain values can be
+    ignored by setting filter_key to that value or by setting filter_key to a
+    (vectorized) function that returns ``True`` for keys that should be redistributed
+    and ``False`` for keys that should be ignored.
 
     Parameters
     ----------
 
 
     Returns
     -------
@@ -43,17 +47,17 @@
         exchange_nranks = nranks
         exchange_Alltoall = exchange_comm.Alltoall
         exchange_Alltoallv = exchange_comm.Alltoallv
         exchange_Allgather = exchange_comm.Allgather
         exchange_Allgatherv = exchange_comm.Allgatherv
 
     else:
-        # exchange particles with the 26 neighboring ranks
-        exchange_comm = partition.comm26
-        exchange_nranks = partition.neighbors26_count
+        # exchange particles with the neighboring ranks
+        exchange_comm = partition.comm_neighbor
+        exchange_nranks = partition.comm_neighbor.Get_size()
         exchange_Alltoall = exchange_comm.Neighbor_alltoall
         exchange_Alltoallv = exchange_comm.Neighbor_alltoallv
         exchange_Allgather = exchange_comm.Neighbor_allgather
         exchange_Allgatherv = exchange_comm.Neighbor_allgatherv
 
     localcount = len(data[key])
     data_keys = np.unique(data[key])
@@ -139,15 +143,16 @@
             comm.Barrier()
 
     # verify that we don't aks ourselves for particles
     if do_all2all and (
         orphan_requests_send_counts[rank] != 0 or orphan_requests_recv_counts[rank] != 0
     ):
         print(
-            f"Error in exchange: rank {rank} is asking itself for an orphan halo: {orphan_requests_send_counts[rank]}/{orphan_requests_recv_counts[rank]}",
+            f"Error in exchange: rank {rank} is asking itself for an orphan halo: "
+            f"{orphan_requests_send_counts[rank]}/{orphan_requests_recv_counts[rank]}",
             file=sys.stderr,
             flush=True,
         )
         comm.Abort()
 
     # prepare data to send
     orphan_requests_indices = []
@@ -231,72 +236,83 @@
         totalcount_before,
         totalcount_after,
         totalcount_missmatch,
         totalcount_missmatch_after,
     ) = totalcounts
 
     if verbose and rank == 0:
-        print(f"exchange summary ({'all2all' if do_all2all else '26-neighbors'}):")
+        print(f"exchange summary ({'all2all' if do_all2all else 'neighbors'}):")
         print(
-            f"   Ntot -> Ntot: {totalcount_before:10d} -> {totalcount_after:10d} (should remain the same)"
+            f"   Ntot -> Ntot: {totalcount_before:10d} -> {totalcount_after:10d} "
+            "(should remain the same)"
         )
         print(
-            f"   Orph -> Orph: {totalcount_missmatch:10d} -> {totalcount_missmatch_after:10d} (should be 0 after)"
+            f"   Orph -> Orph: {totalcount_missmatch:10d} -> "
+            f"{totalcount_missmatch_after:10d} (should be 0 after)"
         )
         print("", flush=True)
 
     # did we conserve number of particles?
     if rank == 0 and totalcount_before != totalcount_after:
         print(
-            f"Error in exchange: Lost halos during progenitor exchange: {totalcount_before} -> {totalcount_after}",
+            "Error in exchange: Lost halos during progenitor exchange: "
+            f"{totalcount_before} -> {totalcount_after}",
             file=sys.stderr,
             flush=True,
         )
         comm.Abort()
 
-    # if we were not able to assign all orphans to the 26 neighbors, try all2all
+    # if we were not able to assign all orphans to the neighbors, try all2all
     if not do_all2all and totalcount_missmatch_after > 0:
         if verbose and rank == 0:
             print(
-                f"exchange all2all since neighbor exchange was not able to assign all: {totalcount_missmatch} -> {totalcount_missmatch_after}",
+                "exchange all2all since neighbor exchange was not able to assign all: "
+                f"{totalcount_missmatch} -> {totalcount_missmatch_after}",
                 flush=True,
             )
         return exchange(
             partition,
             data_new,
             key,
             local_keys,
             verbose=verbose,
             filter_key=filter_key,
             do_all2all=True,
             replace_notfound_key=replace_notfound_key,
         )
 
-    # if we are still not able to assign all orphans, replace key or abort after printing some debug messages
+    # if we are still not able to assign all orphans, replace key or abort after
+    # printing some debug messages
     if replace_notfound_key is not None and localcount_missmatch_after > 0:
         d = data_new[key]
         d[np.isin(d, missing_keys)] = replace_notfound_key
     for i in range(nranks):
-        if rank == i:
-            if localcount_missmatch_after != 0:
-                print(
-                    f"Warning from rank {rank} in exchange: Unable to assign all progenitors to correct ranks (failed for {localcount_missmatch_after} out of {localcount_missmatch})"
-                )
-                print(f"Could not assign keys: ", missing_keys)
-                print("", flush=True)
+        if rank == i and localcount_missmatch_after != 0:
+            print(
+                f"Warning from rank {rank} in exchange: Unable to assign all "
+                f"progenitors to correct ranks (failed for "
+                f"{localcount_missmatch_after} out of {localcount_missmatch})"
+            )
+            print("Could not assign keys: ", missing_keys)
+            print("", flush=True)
         comm.Barrier()
 
     if rank == 0 and totalcount_missmatch_after != 0:
         if replace_notfound_key is None:
             print(
-                f"Error in exchange: Unable to assign all progenitors to correct ranks (tried to reassign {totalcount_missmatch}, failed for {totalcount_missmatch_after})",
+                f"Error in exchange: Unable to assign all progenitors to correct ranks "
+                f"(tried to reassign {totalcount_missmatch}, failed for "
+                f"{totalcount_missmatch_after})",
                 file=sys.stderr,
                 flush=True,
             )
             comm.Abort()
         else:
             print(
-                f"Warning in exchange: Unable to assign all progenitors to correct ranks (tried to reassign {totalcount_missmatch}, failed for {totalcount_missmatch_after}), replacing missing values with {replace_notfound_key}",
+                f"Warning in exchange: Unable to assign all progenitors to correct "
+                f"ranks (tried to reassign {totalcount_missmatch}, failed for "
+                f"{totalcount_missmatch_after}), replacing missing values with "
+                f"{replace_notfound_key}",
                 flush=True,
             )
 
     return data_new
```

### Comparing `mpipartition-1.0.1/mpipartition/overload.py` & `mpipartition-1.0.2/mpipartition/overload.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,25 +1,27 @@
-from .partition import Partition
-from typing import Mapping, Union, List
-import numpy as np
 import itertools
+from typing import List, Mapping, Union
+
+import numpy as np
+
+from .partition import Partition
 
 ParticleDataT = Mapping[str, np.ndarray]
 
 
 def overload(
     partition: Partition,
     box_size: float,
     data: ParticleDataT,
     overload_length: float,
     coord_keys: List[str],
     *,
     verbose: Union[bool, int] = False,
 ):
-    """Copy data within an overload length to the 26 neighboring ranks
+    """Copy data within an overload length to the neighboring ranks
 
     This method assumes that the volume cube is periodic and will wrap the data
     around the boundary interfaces.
 
     Parameters
     ----------
     partition:
@@ -71,15 +73,15 @@
     origin = box_size * np.array(partition.origin)
     extent = box_size * np.array(partition.extent)
 
     neighbors = partition.neighbors
 
     # Find all overload regions each particle should be in
     overload = {}
-    for (i, x) in enumerate(coord_keys):
+    for i, x in enumerate(coord_keys):
         _i = np.zeros_like(data[x], dtype=np.int8)
         _i[data[x] < origin[i] + overload_length] = -1
         _i[data[x] > origin[i] + extent[i] - overload_length] = 1
         overload[i] = _i
 
     # Get particle indices of each of the 27 neighbors overload
     exchange_indices = [np.empty(0, dtype=np.int64) for i in range(nranks)]
```

### Comparing `mpipartition-1.0.1/mpipartition/partition.py` & `mpipartition-1.0.2/mpipartition/partition.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 """MPI Partitioning of a cube
 
 """
 
-from mpi4py import MPI
-import numpy as np
-import sys, time
-from typing import List
 import itertools
+import sys
+from typing import List
+
+import numpy as np
+from mpi4py import MPI
 
 _comm = MPI.COMM_WORLD
 _rank = _comm.Get_rank()
 _nranks = _comm.Get_size()
 
 
 def _factorize(n):
```

### Comparing `mpipartition-1.0.1/pyproject.toml` & `mpipartition-1.0.2/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "mpipartition"
-version = "1.0.1"
+version = "1.0.2"
 description = "MPI volume decomposition and particle distribution tools"
 authors = ["Michael Buehlmann <buehlmann.michi@gmail.com>"]
 license = "MIT"
 readme = "README.rst"
 homepage = "https://github.com/ArgonneCPAC/MPIPartition"
 repository = "https://github.com/ArgonneCPAC/MPIPartition"
 documentation = "https://argonnecpac.github.io/MPIPartition"
```

### Comparing `mpipartition-1.0.1/PKG-INFO` & `mpipartition-1.0.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 Metadata-Version: 2.1
 Name: mpipartition
-Version: 1.0.1
+Version: 1.0.2
 Summary: MPI volume decomposition and particle distribution tools
 Home-page: https://github.com/ArgonneCPAC/MPIPartition
 License: MIT
 Keywords: MPI,mpi4py,scientific computing,parallel computing
 Author: Michael Buehlmann
 Author-email: buehlmann.michi@gmail.com
 Requires-Python: >=3.7,<4.0
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: System :: Distributed Computing
 Requires-Dist: mpi4py (>=3.1.0,<4.0.0)
 Requires-Dist: numpy (>=1.20,<2.0)
 Project-URL: Documentation, https://argonnecpac.github.io/MPIPartition
 Project-URL: Repository, https://github.com/ArgonneCPAC/MPIPartition
@@ -72,14 +73,15 @@
    cd mpipartition
    python setup.py develop
 
 
 Requirements
 ------------
 
+* Python >= 3.7
 * `mpi4py <https://mpi4py.readthedocs.io/en/stable/>`_: MPI for Python
 * `numpy <https://numpy.org/>`_: Python array library
 
 
 Basic Usage
 -----------
 Check the `documentation <https://argonnecpac.github.io/MPIPartition>`_ for
@@ -136,18 +138,18 @@
    box_size = 64.  # box size in Mpc/h
    partition = Partition(3)  # by default, the dimension is 3
 
    # read GenericIO data in parallel
    data = pygio.read_genericio("m000p-499.haloproperties")
 
    # distribute
-   data = distribute(partition, box_size, data, [f"fof_halo_center{x}" for x in "xyz"])
+   data = distribute(partition, box_size, data, [f"fof_halo_center_{x}" for x in "xyz"])
 
    # mark "owned" data with rank (allows differentiating owned and overloaded data)
    data["status"] = partition.rank * np.ones(len(data["fof_halo_center_x"]), dtype=np.uint16)
 
    # overload by 4Mpc/h
-   data = overload(partition, box_size, data, 4., [f"fof_halo_center{x}" for x in "xyz"])
+   data = overload(partition, box_size, data, 4., [f"fof_halo_center_{x}" for x in "xyz"])
 
    # now we can do analysis such as 2pt correlation functions (up to 4Mpc/h)
    # or neighbor finding, etc.
```

