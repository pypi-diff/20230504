# Comparing `tmp/mpipartition-1.0.3.tar.gz` & `tmp/mpipartition-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mpipartition-1.0.3.tar", max compression
+gzip compressed data, was "mpipartition-1.0.4.tar", max compression
```

## Comparing `mpipartition-1.0.3.tar` & `mpipartition-1.0.4.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1076 2023-05-04 18:02:15.055333 mpipartition-1.0.3/LICENSE
--rw-r--r--   0        0        0     3723 2023-05-04 18:02:15.055333 mpipartition-1.0.3/README.rst
--rw-r--r--   0        0        0      274 2023-05-04 18:02:15.059332 mpipartition-1.0.3/mpipartition/__init__.py
--rw-r--r--   0        0        0     4942 2023-05-04 18:02:15.059332 mpipartition-1.0.3/mpipartition/distribute.py
--rw-r--r--   0        0        0    11698 2023-05-04 18:02:15.059332 mpipartition-1.0.3/mpipartition/exchange.py
--rw-r--r--   0        0        0     5047 2023-05-04 18:02:15.059332 mpipartition-1.0.3/mpipartition/overload.py
--rw-r--r--   0        0        0     7430 2023-05-04 18:02:15.059332 mpipartition-1.0.3/mpipartition/partition.py
--rw-r--r--   0        0        0     1291 2023-05-04 18:02:15.059332 mpipartition-1.0.3/pyproject.toml
--rw-r--r--   0        0        0     4936 1970-01-01 00:00:00.000000 mpipartition-1.0.3/PKG-INFO
+-rw-r--r--   0        0        0     1076 2023-05-04 18:29:01.965921 mpipartition-1.0.4/LICENSE
+-rw-r--r--   0        0        0     3723 2023-05-04 18:29:01.965921 mpipartition-1.0.4/README.rst
+-rw-r--r--   0        0        0      274 2023-05-04 18:29:01.965921 mpipartition-1.0.4/mpipartition/__init__.py
+-rw-r--r--   0        0        0     4942 2023-05-04 18:29:01.965921 mpipartition-1.0.4/mpipartition/distribute.py
+-rw-r--r--   0        0        0    11687 2023-05-04 18:29:01.965921 mpipartition-1.0.4/mpipartition/exchange.py
+-rw-r--r--   0        0        0     5047 2023-05-04 18:29:01.965921 mpipartition-1.0.4/mpipartition/overload.py
+-rw-r--r--   0        0        0     7395 2023-05-04 18:29:01.965921 mpipartition-1.0.4/mpipartition/partition.py
+-rw-r--r--   0        0        0     1291 2023-05-04 18:29:01.965921 mpipartition-1.0.4/pyproject.toml
+-rw-r--r--   0        0        0     4936 1970-01-01 00:00:00.000000 mpipartition-1.0.4/PKG-INFO
```

### Comparing `mpipartition-1.0.3/LICENSE` & `mpipartition-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `mpipartition-1.0.3/README.rst` & `mpipartition-1.0.4/README.rst`

 * *Files identical despite different names*

### Comparing `mpipartition-1.0.3/mpipartition/distribute.py` & `mpipartition-1.0.4/mpipartition/distribute.py`

 * *Files identical despite different names*

### Comparing `mpipartition-1.0.3/mpipartition/exchange.py` & `mpipartition-1.0.4/mpipartition/exchange.py`

 * *Files 1% similar despite different names*

```diff
@@ -49,15 +49,15 @@
         exchange_Alltoallv = exchange_comm.Alltoallv
         exchange_Allgather = exchange_comm.Allgather
         exchange_Allgatherv = exchange_comm.Allgatherv
 
     else:
         # exchange particles with the neighboring ranks
         exchange_comm = partition.comm_neighbor
-        exchange_nranks = exchange_comm.Get_dist_neighbors_count()
+        exchange_nranks = len(partition.neighbor_ranks)
         exchange_Alltoall = exchange_comm.Neighbor_alltoall
         exchange_Alltoallv = exchange_comm.Neighbor_alltoallv
         exchange_Allgather = exchange_comm.Neighbor_allgather
         exchange_Allgatherv = exchange_comm.Neighbor_allgatherv
 
     localcount = len(data[key])
     data_keys = np.unique(data[key])
```

### Comparing `mpipartition-1.0.3/mpipartition/overload.py` & `mpipartition-1.0.4/mpipartition/overload.py`

 * *Files identical despite different names*

### Comparing `mpipartition-1.0.3/mpipartition/partition.py` & `mpipartition-1.0.4/mpipartition/partition.py`

 * *Files 1% similar despite different names*

```diff
@@ -86,15 +86,14 @@
         self,
         dimensions=3,
         *,
         create_neighbor_topo: bool = False,
         commensurate_topo: List[int] = None,
     ):
         self._topo = None
-        self._neighbor_topo = None
         assert dimensions > 0
         assert type(dimensions) == int
         self._dimensions = dimensions
         self._rank = _rank
         self._nranks = _nranks
         if commensurate_topo is None:
             self._decomposition = MPI.Compute_dims(_nranks, [0] * self._dimensions)
```

### Comparing `mpipartition-1.0.3/pyproject.toml` & `mpipartition-1.0.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "mpipartition"
-version = "1.0.3"
+version = "1.0.4"
 description = "MPI volume decomposition and particle distribution tools"
 authors = ["Michael Buehlmann <buehlmann.michi@gmail.com>"]
 license = "MIT"
 readme = "README.rst"
 homepage = "https://github.com/ArgonneCPAC/MPIPartition"
 repository = "https://github.com/ArgonneCPAC/MPIPartition"
 documentation = "https://argonnecpac.github.io/MPIPartition"
```

### Comparing `mpipartition-1.0.3/PKG-INFO` & `mpipartition-1.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mpipartition
-Version: 1.0.3
+Version: 1.0.4
 Summary: MPI volume decomposition and particle distribution tools
 Home-page: https://github.com/ArgonneCPAC/MPIPartition
 License: MIT
 Keywords: MPI,mpi4py,scientific computing,parallel computing
 Author: Michael Buehlmann
 Author-email: buehlmann.michi@gmail.com
 Requires-Python: >=3.7,<4.0
```

