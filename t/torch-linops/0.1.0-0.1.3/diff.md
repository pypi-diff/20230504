# Comparing `tmp/torch-linops-0.1.0.tar.gz` & `tmp/torch-linops-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "torch-linops-0.1.0.tar", last modified: Sun Oct 30 18:39:32 2022, max compression
+gzip compressed data, was "torch-linops-0.1.3.tar", last modified: Thu May  4 21:52:19 2023, max compression
```

## Comparing `torch-linops-0.1.0.tar` & `torch-linops-0.1.3.tar`

### file list

```diff
@@ -1,21 +1,25 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-30 18:39:32.064284 torch-linops-0.1.0/
--rw-r--r--   0 root         (0) root         (0)     6548 2022-10-30 18:39:32.064284 torch-linops-0.1.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     5168 2022-10-30 18:39:25.000000 torch-linops-0.1.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-30 18:39:32.064284 torch-linops-0.1.0/linops/
--rw-r--r--   0 root         (0) root         (0)      372 2022-10-30 18:39:25.000000 torch-linops-0.1.0/linops/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2488 2022-10-30 18:39:25.000000 torch-linops-0.1.0/linops/blocks.py
--rw-r--r--   0 root         (0) root         (0)     5240 2022-10-30 18:39:25.000000 torch-linops-0.1.0/linops/cg.py
--rw-r--r--   0 root         (0) root         (0)     1978 2022-10-30 18:39:25.000000 torch-linops-0.1.0/linops/equilibration.py
--rw-r--r--   0 root         (0) root         (0)    11584 2022-10-30 18:39:25.000000 torch-linops-0.1.0/linops/linops.py
--rw-r--r--   0 root         (0) root         (0)     5003 2022-10-30 18:39:25.000000 torch-linops-0.1.0/linops/minres.py
--rw-r--r--   0 root         (0) root         (0)     2285 2022-10-30 18:39:25.000000 torch-linops-0.1.0/linops/nystrom_precondition.py
--rw-r--r--   0 root         (0) root         (0)     1456 2022-10-30 18:39:25.000000 torch-linops-0.1.0/linops/trace.py
--rw-r--r--   0 root         (0) root         (0)       97 2022-10-30 18:39:25.000000 torch-linops-0.1.0/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2022-10-30 18:39:32.064284 torch-linops-0.1.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      732 2022-10-30 18:39:25.000000 torch-linops-0.1.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-30 18:39:32.064284 torch-linops-0.1.0/torch_linops.egg-info/
--rw-r--r--   0 root         (0) root         (0)     6548 2022-10-30 18:39:31.000000 torch-linops-0.1.0/torch_linops.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      366 2022-10-30 18:39:32.000000 torch-linops-0.1.0/torch_linops.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-10-30 18:39:31.000000 torch-linops-0.1.0/torch_linops.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       12 2022-10-30 18:39:31.000000 torch-linops-0.1.0/torch_linops.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        7 2022-10-30 18:39:31.000000 torch-linops-0.1.0/torch_linops.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 21:52:19.147651 torch-linops-0.1.3/
+-rw-r--r--   0 root         (0) root         (0)    11357 2023-05-04 21:52:04.000000 torch-linops-0.1.3/LICENSE.md
+-rw-r--r--   0 root         (0) root         (0)     5618 2023-05-04 21:52:19.147651 torch-linops-0.1.3/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     5168 2023-05-04 21:52:04.000000 torch-linops-0.1.3/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 21:52:19.147651 torch-linops-0.1.3/linops/
+-rw-r--r--   0 root         (0) root         (0)      408 2023-05-04 21:52:04.000000 torch-linops-0.1.3/linops/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2488 2023-05-04 21:52:04.000000 torch-linops-0.1.3/linops/blocks.py
+-rw-r--r--   0 root         (0) root         (0)     5240 2023-05-04 21:52:04.000000 torch-linops-0.1.3/linops/cg.py
+-rw-r--r--   0 root         (0) root         (0)      860 2023-05-04 21:52:04.000000 torch-linops-0.1.3/linops/diag.py
+-rw-r--r--   0 root         (0) root         (0)     1978 2023-05-04 21:52:04.000000 torch-linops-0.1.3/linops/equilibration.py
+-rw-r--r--   0 root         (0) root         (0)     1808 2023-05-04 21:52:04.000000 torch-linops-0.1.3/linops/linop_impls.py
+-rw-r--r--   0 root         (0) root         (0)    11629 2023-05-04 21:52:04.000000 torch-linops-0.1.3/linops/linops.py
+-rw-r--r--   0 root         (0) root         (0)     6583 2023-05-04 21:52:04.000000 torch-linops-0.1.3/linops/lsqr.py
+-rw-r--r--   0 root         (0) root         (0)     5003 2023-05-04 21:52:04.000000 torch-linops-0.1.3/linops/minres.py
+-rw-r--r--   0 root         (0) root         (0)     2285 2023-05-04 21:52:04.000000 torch-linops-0.1.3/linops/nystrom_precondition.py
+-rw-r--r--   0 root         (0) root         (0)     4780 2023-05-04 21:52:04.000000 torch-linops-0.1.3/linops/trace.py
+-rw-r--r--   0 root         (0) root         (0)       97 2023-05-04 21:52:04.000000 torch-linops-0.1.3/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-04 21:52:19.147651 torch-linops-0.1.3/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      732 2023-05-04 21:52:04.000000 torch-linops-0.1.3/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 21:52:19.147651 torch-linops-0.1.3/torch_linops.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     5618 2023-05-04 21:52:19.000000 torch-linops-0.1.3/torch_linops.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      429 2023-05-04 21:52:19.000000 torch-linops-0.1.3/torch_linops.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-04 21:52:19.000000 torch-linops-0.1.3/torch_linops.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       12 2023-05-04 21:52:19.000000 torch-linops-0.1.3/torch_linops.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        7 2023-05-04 21:52:19.000000 torch-linops-0.1.3/torch_linops.egg-info/top_level.txt
```

### Comparing `torch-linops-0.1.0/PKG-INFO` & `torch-linops-0.1.3/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,130 +1,133 @@
 Metadata-Version: 2.1
 Name: torch-linops
-Version: 0.1.0
+Version: 0.1.3
 Summary: A library to define abstract linear operators, and associated algebra and matrix-free algorithms, that works with pyTorch Tensors.
 Home-page: https://github.com/cvxgrp/torch_linops
 Author: Parth Nobel
 Author-email: ptnobel@stanford.edu
 License: GPLv3
-Description: # An Abstract Linear Operator Library for pyTorch
-        
-        This library implements a generic structure for abstract linear operators and
-        enables a number of standard operations on them:
-         * Arithmetic: `A + B`, `A - B`, `-A`, `A @ B` all work exactly as expected to
-            combine linear operators.
-         * Indexing: `A[k:ell,m:n]` works as expected.
-         * Solves: `Ax = b` can be solved with `CG` for PSD matrices, `minres` for
-         symmetric matrices, `LSQR` (to be implemented), or `LSMR` (to be implemented).
-         * Trace estimation: The trace of square matrices, can be estimated via Hutch++
-            and Hutchinson's estimator.
-         * [Diamond-Boyd stochastic equilibration](https://web.stanford.edu/~boyd/papers/mf_equil.html)
-         * [Randomized Nyström Preconditioning](https://arxiv.org/abs/2110.02820)
-         * Automatic adjoint operator generation.
-        
-        # Using `LinearOperator`s
-        
-        The public API of the `LinearOperator` library is that every `LinearOperator` has the
-        following properties and methods:
-        ```python
-        
-        class LinearOperator:
-        
-            # Properties
-            shape: tuple[int, int]
-            T: LinearOperator
-            supports_operator_matrix: bool
-            device: torch.Device
-        
-            # Matrix multiply
-            def __matmul__(self, b: torch.Tensor) -> torch.Tensor: ...
-            def __rmatmul__(self, b: torch.Tensor) -> torch.Tensor: ...
-        
-            def __matmul__(self, b: LinearOperator) -> LinearOperator: ...
-            def __rmatmul__(self, b: LinearOperator) -> LinearOperator: ...
-            
-            # Linear Solve Methods
-            def solve_I_p_lambda_AT_A_x_eq_b(self,
-                lambda_: float,
-                b: torch.Tensor,
-                x0: torch.Tensor | None=None,
-                *, precondition: None | Literal['nsytrom'], hot=False) -> torch.Tensor: ...
-        
-            def solve_A_x_eq_b(self,
-                b: torch.Tensor,
-                x0: torch.Tensor | None=None) -> torch.Tensor: ...
-        
-            # Transformations on LinearOperator
-            def __mul__(self, c: float) -> LinearOperator: ...
-            def __rmul__(self, c: float) -> LinearOperator: ...
-        
-            def __truediv__(self, c: float) -> LinearOperator: ...
-        
-            def __pow__(self, k: int) -> LinearOperator: ...
-        
-            def __add__(self, c: LinearOperator) -> LinearOperator: ...
-        
-            def __sub__(self, c: LinearOperator) -> LinearOperator: ...
-        
-            def __neg__(self) -> LinearOperator: ...
-        
-            def __pos__(self) -> LinearOperator: ...
-        
-            def __getitem__(self, key) -> LinearOperator: ...
-        ```
-        
-        The following functions are available in the root of the library:
-        ```python
-        def operator_matrix_product(A: LinearOperator, M: torch.Tensor) -> torch.Tensor: ...
-        def aslinearoperator(A: torch.Tensor | LinearOperator) -> LinearOperator: ...
-        def vstack(ops: list[LinearOperator] | tuple[LinearOperator, ...]) -> LinearOperator: ...
-        def hstack(ops: list[LinearOperator] | tuple[LinearOperator, ...]) -> LinearOperator: ...
-        
-        # To be implemented:
-        def bmat(ops: list[list[LinearOperator]]) -> LinearOperator: ... # Optimizes out ZeroOperator
-        ```
-        
-        The following functions are available in `linops.trace` for trace estimation:
-        ```python
-        def hutchpp(A: lo.LinearOperator, m: int) -> float: ...
-        def hutchinson(A: lo.LinearOperator, m: int) -> float: ...
-        ```
-        
-        `linops.equilibration` contains `equilibrate` and `symmetric_equilibrate`.
-        Their public API is not finalized, if you wish to use them it is recommend you read the source code.
-        
-        # Creating Linear Operators
-        
-        Linear operators can be constructed in the following way:
-         * Creating a sub-class of `LinearOperator` 
-         * Calling one of the following constructors:
-            * `IdentityOperator(n: int)`
-            * `DiagonalOperator(diag: torch.Tensor)`: where `diag` is a 1D torch tensor.
-            * `MatrixOperator(M: torch.Tensor)`: where `M` is a 2D torch tensor.
-            * `SelectionOperator(shape: tuple[int, int], idxs: slice | list[int | slice])`
-            * `KKTOperator(H: LinearOperator, A: LinearOperator)`: where `H` is a square `LinearOperator` and `A` is a `LinearOperator`
-            * `VectorJacobianOperator(f: torch.Tensor, x: torch.Tensor)`: where `f` is the output of the function being differentiated
-                which has a torch autograd value and `x` is the vector on which `ensures_grad` was called.
-            * `ZeroOperator(shape: tuple[int, int])`
-         * Combining operators via:
-            * `A + B`, `A - B`, `A @ B` for `A`, `B` linear operators
-            * `hstack`, `vstack`
-            * `A`, `c A`, `A / c`, `v * A`, `A / v` for scalar `c` and vector `v`.
-        
-        # Implementing `LinearOperator`s
-        
-        To implement a `LinearOperator` the following are mandatory:
-        
-         * Set `_shape: tuple[int, int]`  to the shape of the operator.
-         * Set `device` appropriately, if the operator requires vectors to be on a particular device.
-         *  Implement a method `def _matmul_impl(self, v: torch.Tensor) -> torch.Tensor: ...` that implements your matrix vector product.
-        
-        The following are recommended to improve performance:
-        
-         * If your `_matmul_impl` method handles matrix inputs correctly, set `supports_operator_matrix: bool` to `True`.
-         * If it is possible to describe the adjoint operator, set `_adjoint: LinearOperator` to point to the adjoint of your operator. If you do not compute this, then one will be autogenerated by differentiating through your `_matmul_impl`.
-        
-        It is suggested that, if possible, you replace any other methods with specialized implementations.
-        
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
+License-File: LICENSE.md
+
+# An Abstract Linear Operator Library for pyTorch
+
+This library implements a generic structure for abstract linear operators and
+enables a number of standard operations on them:
+ * Arithmetic: `A + B`, `A - B`, `-A`, `A @ B` all work exactly as expected to
+    combine linear operators.
+ * Indexing: `A[k:ell,m:n]` works as expected.
+ * Solves: `Ax = b` can be solved with `CG` for PSD matrices, `minres` for
+ symmetric matrices, `LSQR` (to be implemented), or `LSMR` (to be implemented).
+ * Trace estimation: The trace of square matrices, can be estimated via Hutch++
+    and Hutchinson's estimator.
+ * [Diamond-Boyd stochastic equilibration](https://web.stanford.edu/~boyd/papers/mf_equil.html)
+ * [Randomized Nyström Preconditioning](https://arxiv.org/abs/2110.02820)
+ * Automatic adjoint operator generation.
+
+# Using `LinearOperator`s
+
+The public API of the `LinearOperator` library is that every `LinearOperator` has the
+following properties and methods:
+```python
+
+class LinearOperator:
+
+    # Properties
+    shape: tuple[int, int]
+    T: LinearOperator
+    supports_operator_matrix: bool
+    device: torch.Device
+
+    # Matrix multiply
+    def __matmul__(self, b: torch.Tensor) -> torch.Tensor: ...
+    def __rmatmul__(self, b: torch.Tensor) -> torch.Tensor: ...
+
+    def __matmul__(self, b: LinearOperator) -> LinearOperator: ...
+    def __rmatmul__(self, b: LinearOperator) -> LinearOperator: ...
+    
+    # Linear Solve Methods
+    def solve_I_p_lambda_AT_A_x_eq_b(self,
+        lambda_: float,
+        b: torch.Tensor,
+        x0: torch.Tensor | None=None,
+        *, precondition: None | Literal['nsytrom'], hot=False) -> torch.Tensor: ...
+
+    def solve_A_x_eq_b(self,
+        b: torch.Tensor,
+        x0: torch.Tensor | None=None) -> torch.Tensor: ...
+
+    # Transformations on LinearOperator
+    def __mul__(self, c: float) -> LinearOperator: ...
+    def __rmul__(self, c: float) -> LinearOperator: ...
+
+    def __truediv__(self, c: float) -> LinearOperator: ...
+
+    def __pow__(self, k: int) -> LinearOperator: ...
+
+    def __add__(self, c: LinearOperator) -> LinearOperator: ...
+
+    def __sub__(self, c: LinearOperator) -> LinearOperator: ...
+
+    def __neg__(self) -> LinearOperator: ...
+
+    def __pos__(self) -> LinearOperator: ...
+
+    def __getitem__(self, key) -> LinearOperator: ...
+```
+
+The following functions are available in the root of the library:
+```python
+def operator_matrix_product(A: LinearOperator, M: torch.Tensor) -> torch.Tensor: ...
+def aslinearoperator(A: torch.Tensor | LinearOperator) -> LinearOperator: ...
+def vstack(ops: list[LinearOperator] | tuple[LinearOperator, ...]) -> LinearOperator: ...
+def hstack(ops: list[LinearOperator] | tuple[LinearOperator, ...]) -> LinearOperator: ...
+
+# To be implemented:
+def bmat(ops: list[list[LinearOperator]]) -> LinearOperator: ... # Optimizes out ZeroOperator
+```
+
+The following functions are available in `linops.trace` for trace estimation:
+```python
+def hutchpp(A: lo.LinearOperator, m: int) -> float: ...
+def hutchinson(A: lo.LinearOperator, m: int) -> float: ...
+```
+
+`linops.equilibration` contains `equilibrate` and `symmetric_equilibrate`.
+Their public API is not finalized, if you wish to use them it is recommend you read the source code.
+
+# Creating Linear Operators
+
+Linear operators can be constructed in the following way:
+ * Creating a sub-class of `LinearOperator` 
+ * Calling one of the following constructors:
+    * `IdentityOperator(n: int)`
+    * `DiagonalOperator(diag: torch.Tensor)`: where `diag` is a 1D torch tensor.
+    * `MatrixOperator(M: torch.Tensor)`: where `M` is a 2D torch tensor.
+    * `SelectionOperator(shape: tuple[int, int], idxs: slice | list[int | slice])`
+    * `KKTOperator(H: LinearOperator, A: LinearOperator)`: where `H` is a square `LinearOperator` and `A` is a `LinearOperator`
+    * `VectorJacobianOperator(f: torch.Tensor, x: torch.Tensor)`: where `f` is the output of the function being differentiated
+        which has a torch autograd value and `x` is the vector on which `ensures_grad` was called.
+    * `ZeroOperator(shape: tuple[int, int])`
+ * Combining operators via:
+    * `A + B`, `A - B`, `A @ B` for `A`, `B` linear operators
+    * `hstack`, `vstack`
+    * `A`, `c A`, `A / c`, `v * A`, `A / v` for scalar `c` and vector `v`.
+
+# Implementing `LinearOperator`s
+
+To implement a `LinearOperator` the following are mandatory:
+
+ * Set `_shape: tuple[int, int]`  to the shape of the operator.
+ * Set `device` appropriately, if the operator requires vectors to be on a particular device.
+ *  Implement a method `def _matmul_impl(self, v: torch.Tensor) -> torch.Tensor: ...` that implements your matrix vector product.
+
+The following are recommended to improve performance:
+
+ * If your `_matmul_impl` method handles matrix inputs correctly, set `supports_operator_matrix: bool` to `True`.
+ * If it is possible to describe the adjoint operator, set `_adjoint: LinearOperator` to point to the adjoint of your operator. If you do not compute this, then one will be autogenerated by differentiating through your `_matmul_impl`.
+
+It is suggested that, if possible, you replace any other methods with specialized implementations.
+
+
```

### Comparing `torch-linops-0.1.0/README.md` & `torch-linops-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `torch-linops-0.1.0/linops/blocks.py` & `torch-linops-0.1.3/linops/blocks.py`

 * *Files identical despite different names*

### Comparing `torch-linops-0.1.0/linops/cg.py` & `torch-linops-0.1.3/linops/cg.py`

 * *Files identical despite different names*

### Comparing `torch-linops-0.1.0/linops/equilibration.py` & `torch-linops-0.1.3/linops/equilibration.py`

 * *Files identical despite different names*

### Comparing `torch-linops-0.1.0/linops/linops.py` & `torch-linops-0.1.3/linops/linops.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 import torch
 import operator
+import linops as lo
 from linops.cg import CG
 from linops.minres import minres
 import linops.nystrom_precondition as nystrom 
 
 
 
 def operator_matrix_product(A, M):
     assert A.shape[1] == M.shape[0]
     if A.supports_operator_matrix:
         return A @ M
-    out = torch.empty((A.shape[0], M.shape[1]))
+    out = torch.empty((A.shape[0], M.shape[1]), device=M.device, dtype=M.dtype)
     for i in range(M.shape[1]):
         out[:, i] = A @ M[:, i]
     return out
 
 
 def aslinearoperator(A):
     if isinstance(A, LinearOperator):
@@ -25,23 +26,33 @@
 class LinearOperator:
     _adjoint = None
     _shape: tuple[int, int] = None
     _nystrom_sketch = None
     _last_solve_of_x = None
     device = None
     supports_operator_matrix = False
+    efficient_inverse = False
 
     def __call__(self, x):
         return self @ x
 
     def __matmul__(self, b):
         if isinstance(b, LinearOperator):
             return _JoinOperator(self, b)
-        else:
+        elif len(b.shape) == 1:
             return self._matmul_impl(b)
+        elif len(b.shape) == 2:
+            assert self.shape[1] == b.shape[0]
+            if self.supports_operator_matrix:
+                return self._matmul_impl(b)
+            else:
+                out = torch.empty((self.shape[0], b.shape[1]), device=b.device, dtype=b.dtype)
+                for i in range(b.shape[1]):
+                    out[:, i] = self._matmul_impl(b[:, i])
+                return out
 
     def __rmatmul__(self, a):
         if isinstance(a, LinearOperator):
             return _JoinOperator(a, self)
         else:
             return (self.T @ a.T).T
 
@@ -72,24 +83,23 @@
         return _UrnaryOperator(self, operator.neg)
 
     def __pos__(self):
         return _UrnaryOperator(self, operator.pos)
 
     def __pow__(self, n):
         return _PowOperator(self, n)
-    
+
     def __getitem__(self, key):
-        out = torch.empty(self.shape[0])
-        in_ = torch.empty(self.shape[1])
         if not isinstance(key, tuple):
             # Only recieved one index, so we're only applying to the output
-            shape = (out[key].shape[0], self.shape[1])
-            return SelectionOperator(shape, key) @ self
-        shape = (out[key[0]].shape[0], in_[key[1]][0])
-        return SelectionOperator(shape, key[0]) @ self @ SelectionOperator(shape, key[1]).T
+            S = _generate_selector(self.shape[0], key[0])
+            return S @ self
+        leftS = _generate_selector(self.shape[0], key[0])
+        rightS = _generate_selector(self.shape[1], key[1], flip=True)
+        return leftS @ self @ rightS.T
 
     @property
     def shape(self) -> tuple[int, int]:
         return self._shape
 
     @property
     def T(self):
@@ -117,103 +127,52 @@
                     l_max=kwargs.get('l_max', 500),
                     power_iter_count=kwargs.get('power_iter_count', 50),
                     error_tol=kwargs.get('error_tol', 1.0),
                     )
             precondition = nystrom.NystromPreconditioner(
                     self._nystrom_sketch, lambda_)
         self._last_solve_of_x = CG(
-                IdentityOperator(self.shape[1]) + lambda_ * (self.T @ self),
+                lo.IdentityOperator(self.shape[1]) + lambda_ * (self.T @ self),
                 precondition)(b)
         return self._last_solve_of_x
 
     def solve_A_x_eq_b(self, b, x0=None):
         if self is self._adjoint:
             return minres(self, b, x0=x0)
         else:
             raise NotImplementedError()
 
-class ZeroOperator(LinearOperator):
-    supports_operator_matrix = True
-    def __init__(self, shape, adjoint=None):
-        self._shape = shape
-        self._adjoint = ZeroOperator((shape[1], shape[0]), self) \
-                if adjoint is None else adjoint
-
-    def _matmul_impl(self, v):
-        shape = (self.shape[0], *v.shape[1:])
-        return torch.zeros(shape, device=v.device)
-
-
-class VectorJacobianOperator(LinearOperator):
-    def __init__(self, g, x, adjoint=None):
-        self._shape = (x.shape[0], g.shape[0])
-        self._adjoint = adjoint
-        self._g = g
-        self._x = x
-
-    def _matmul_impl(self, v):
-        self._x.grad = None
-        self._g.backward(gradient=v, retain_graph=True)
-        out = self._x.grad
-        self._x.grad = None
-        return out
-
-class IdentityOperator(LinearOperator):
-    supports_operator_matrix = True
-    def __init__(self, n):
-        self._adjoint = self
-        self._shape = (n, n)
-
-    def _matmul_impl(self, v):
-        return v
-
-    def solve_A_x_eq_b(self, b, x0=None):
-        return b
-
-class DiagonalOperator(LinearOperator):
-    supports_operator_matrix = True
-    def __init__(self, diag):
-        self._adjoint = self
-        self._diag = diag
-        m, = diag.shape
-        self._shape = (m, m)
-
-    def _matmul_impl(self, v):
-        if len(v.shape) == 1:
-            return self._diag * v
-        else:
-            return self._diag[:, None] * v
-
-    def solve_A_x_eq_b(self, b, x0=None):
-        if len(b.shape) == 1:
-            return b / self._diag
-        else:
-            return b / self._diag[:, None]
-
-
 class _ScaleOperator(LinearOperator):
     supports_operator_matrix = True
+    efficient_inverse = True
     def __init__(self, c, shape):
         self._c = c
         self._adjoint = self
         self._shape = shape
 
     def _matmul_impl(self, v):
         return self._c * v
 
+    def solve_A_x_eq_b(self, b, x0=None):
+        return b / self._c
+
 class _ScaledownOperator(LinearOperator):
     supports_operator_matrix = True
+    efficient_inverse = True
     def __init__(self, c, shape):
         self._c = c
         self._adjoint = self
         self._shape = shape
 
     def _matmul_impl(self, v):
         return v / self._c
 
+    def solve_A_x_eq_b(self, b, x0=None):
+        return b * self._c
+
 class MatrixOperator(LinearOperator):
     supports_operator_matrix = True
     def __init__(self, matrix, adjoint=None):
         self._matrix = matrix
         assert len(matrix.shape) == 2
         self._shape = matrix.shape
         if adjoint is None:
@@ -260,22 +219,33 @@
         self.supports_operator_matrix = linop.supports_operator_matrix
         self._linop = linop
         self._k = k
         assert k >= 0
         assert linop.shape[0] == linop.shape[1]
         self._adjoint = _PowOperator(self._linop.T, self._k)
         self._shape = linop.shape
+        self.efficient_inverse = linop.efficient_inverse
 
     def _matmul_impl(self, v):
         k = self._k
         while k > 0:
             v = self._linop @ v
             k -= 1
         return v
 
+    def solve_A_x_eq_b(self, b, x0=None):
+        if self.efficient_inverse:
+            k = self._k
+            while k > 0:
+                b = self._linop.solve_A_x_eq_b(b, x0)
+                k -= 1
+            return b
+        else:
+            return super().solve_A_x_eq_b(b, x0=x0)
+
 class _BinaryOperator(LinearOperator):
     """transpose must distribute over op"""
     def __init__(self, left, right, op, adjoint=None):
         assert left.shape == right.shape
         self.supports_operator_matrix = \
                 left.supports_operator_matrix and right.supports_operator_matrix
         self._left = left
@@ -304,26 +274,50 @@
     def _matmul_impl(self, y):
         return self._op(self._linop @ y)
     
 class _JoinOperator(LinearOperator):
     def __init__(self, left, right, adjoint=None):
         self._left = left
         self._right = right
+        self.efficient_inverse = \
+                left.efficient_inverse and right.efficient_inverse
 
         self.supports_operator_matrix = \
                 left.supports_operator_matrix and right.supports_operator_matrix
         if adjoint is None:
             self._adjoint = _JoinOperator(self._right.T, self._left.T, self)
         else:
             self._adjoint = adjoint
         self._shape = (left.shape[0], right.shape[1])
 
     def _matmul_impl(self, y):
         return self._left @ (self._right @ y)
 
+    def solve_A_x_eq_b(self, b, x0=None):
+        if self.efficient_inverse:
+            y = self._left.solve_A_x_eq_b(b, self._right @ x0)
+            return self._right.solve_A_x_eq_b(y, x0)
+        else:
+            return super().solve_A_x_eq_b(b, x0=x0)
+
+class VectorJacobianOperator(LinearOperator):
+    def __init__(self, g, x, adjoint=None):
+        self._shape = (x.shape[0], g.shape[0])
+        self._adjoint = adjoint
+        self.device = x.device
+        self._g = g
+        self._x = x
+
+    def _matmul_impl(self, v):
+        self._x.grad = None
+        self._g.backward(gradient=v, retain_graph=True)
+        out = self._x.grad
+        self._x.grad = None
+        return out
+
 class SelectionOperator(LinearOperator):
     #supports_operator_matrix = True
     def __init__(self, shape, idxs):
         self._shape = shape
         self._adjoint = _AdjointSelectionOperator(idxs,
                 (self._shape[1], self._shape[0]), self)
         self._idxs = idxs
@@ -344,26 +338,17 @@
         self._shape = shape
 
     def _matmul_impl(self, y):
         z = torch.zeros(self.shape[0], dtype=y.dtype, device=y.device)
         z[self._idxs] = y
         return z.reshape(-1)
 
-class KKTOperator(LinearOperator):
-    def __init__(self, H: LinearOperator, A: LinearOperator):
-        k, ell = H.shape
-        assert k == ell
-        m, n = A.shape
-        assert n == k
-        self._shape = (m + n, m + n)
-        self._adjoint = self
-        self._A = A
-        self._H = H
-        self._m = m
-        self._n = n
-
-    def _matmul_impl(self, y):
-        n = self._n
-        return torch.hstack([
-            self._H @ y[:n] - self._A.T @ y[n:],
-            -self._A @ y[:n]
-        ])
+def _generate_selector(size_of_vec, key, flip=False):
+    shape_of_output = torch.empty(size_of_vec)[key].shape
+    if len(shape_of_output) == 0:
+        shape_of_output = 1
+    else:
+        shape_of_output = shape_of_output[0]
+    return SelectionOperator(
+            (size_of_vec, shape_of_output)
+                if not flip else (shape_of_output, size_of_vec)
+            , key)
```

### Comparing `torch-linops-0.1.0/linops/minres.py` & `torch-linops-0.1.3/linops/minres.py`

 * *Files identical despite different names*

### Comparing `torch-linops-0.1.0/linops/nystrom_precondition.py` & `torch-linops-0.1.3/linops/nystrom_precondition.py`

 * *Files identical despite different names*

### Comparing `torch-linops-0.1.0/setup.py` & `torch-linops-0.1.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 
 with open("README.md", "r") as fh:
    long_description = fh.read()
 
 setup(
     name="torch-linops",
-    version="0.1.0",
+    version="0.1.3",
     packages=["linops"],
     license="GPLv3",
     description="A library to define abstract linear operators, and associated algebra and matrix-free algorithms, that works with pyTorch Tensors.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     setup_requires=["setuptools>=18.0"],
     install_requires=[
```

### Comparing `torch-linops-0.1.0/torch_linops.egg-info/PKG-INFO` & `torch-linops-0.1.3/torch_linops.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,130 +1,133 @@
 Metadata-Version: 2.1
 Name: torch-linops
-Version: 0.1.0
+Version: 0.1.3
 Summary: A library to define abstract linear operators, and associated algebra and matrix-free algorithms, that works with pyTorch Tensors.
 Home-page: https://github.com/cvxgrp/torch_linops
 Author: Parth Nobel
 Author-email: ptnobel@stanford.edu
 License: GPLv3
-Description: # An Abstract Linear Operator Library for pyTorch
-        
-        This library implements a generic structure for abstract linear operators and
-        enables a number of standard operations on them:
-         * Arithmetic: `A + B`, `A - B`, `-A`, `A @ B` all work exactly as expected to
-            combine linear operators.
-         * Indexing: `A[k:ell,m:n]` works as expected.
-         * Solves: `Ax = b` can be solved with `CG` for PSD matrices, `minres` for
-         symmetric matrices, `LSQR` (to be implemented), or `LSMR` (to be implemented).
-         * Trace estimation: The trace of square matrices, can be estimated via Hutch++
-            and Hutchinson's estimator.
-         * [Diamond-Boyd stochastic equilibration](https://web.stanford.edu/~boyd/papers/mf_equil.html)
-         * [Randomized Nyström Preconditioning](https://arxiv.org/abs/2110.02820)
-         * Automatic adjoint operator generation.
-        
-        # Using `LinearOperator`s
-        
-        The public API of the `LinearOperator` library is that every `LinearOperator` has the
-        following properties and methods:
-        ```python
-        
-        class LinearOperator:
-        
-            # Properties
-            shape: tuple[int, int]
-            T: LinearOperator
-            supports_operator_matrix: bool
-            device: torch.Device
-        
-            # Matrix multiply
-            def __matmul__(self, b: torch.Tensor) -> torch.Tensor: ...
-            def __rmatmul__(self, b: torch.Tensor) -> torch.Tensor: ...
-        
-            def __matmul__(self, b: LinearOperator) -> LinearOperator: ...
-            def __rmatmul__(self, b: LinearOperator) -> LinearOperator: ...
-            
-            # Linear Solve Methods
-            def solve_I_p_lambda_AT_A_x_eq_b(self,
-                lambda_: float,
-                b: torch.Tensor,
-                x0: torch.Tensor | None=None,
-                *, precondition: None | Literal['nsytrom'], hot=False) -> torch.Tensor: ...
-        
-            def solve_A_x_eq_b(self,
-                b: torch.Tensor,
-                x0: torch.Tensor | None=None) -> torch.Tensor: ...
-        
-            # Transformations on LinearOperator
-            def __mul__(self, c: float) -> LinearOperator: ...
-            def __rmul__(self, c: float) -> LinearOperator: ...
-        
-            def __truediv__(self, c: float) -> LinearOperator: ...
-        
-            def __pow__(self, k: int) -> LinearOperator: ...
-        
-            def __add__(self, c: LinearOperator) -> LinearOperator: ...
-        
-            def __sub__(self, c: LinearOperator) -> LinearOperator: ...
-        
-            def __neg__(self) -> LinearOperator: ...
-        
-            def __pos__(self) -> LinearOperator: ...
-        
-            def __getitem__(self, key) -> LinearOperator: ...
-        ```
-        
-        The following functions are available in the root of the library:
-        ```python
-        def operator_matrix_product(A: LinearOperator, M: torch.Tensor) -> torch.Tensor: ...
-        def aslinearoperator(A: torch.Tensor | LinearOperator) -> LinearOperator: ...
-        def vstack(ops: list[LinearOperator] | tuple[LinearOperator, ...]) -> LinearOperator: ...
-        def hstack(ops: list[LinearOperator] | tuple[LinearOperator, ...]) -> LinearOperator: ...
-        
-        # To be implemented:
-        def bmat(ops: list[list[LinearOperator]]) -> LinearOperator: ... # Optimizes out ZeroOperator
-        ```
-        
-        The following functions are available in `linops.trace` for trace estimation:
-        ```python
-        def hutchpp(A: lo.LinearOperator, m: int) -> float: ...
-        def hutchinson(A: lo.LinearOperator, m: int) -> float: ...
-        ```
-        
-        `linops.equilibration` contains `equilibrate` and `symmetric_equilibrate`.
-        Their public API is not finalized, if you wish to use them it is recommend you read the source code.
-        
-        # Creating Linear Operators
-        
-        Linear operators can be constructed in the following way:
-         * Creating a sub-class of `LinearOperator` 
-         * Calling one of the following constructors:
-            * `IdentityOperator(n: int)`
-            * `DiagonalOperator(diag: torch.Tensor)`: where `diag` is a 1D torch tensor.
-            * `MatrixOperator(M: torch.Tensor)`: where `M` is a 2D torch tensor.
-            * `SelectionOperator(shape: tuple[int, int], idxs: slice | list[int | slice])`
-            * `KKTOperator(H: LinearOperator, A: LinearOperator)`: where `H` is a square `LinearOperator` and `A` is a `LinearOperator`
-            * `VectorJacobianOperator(f: torch.Tensor, x: torch.Tensor)`: where `f` is the output of the function being differentiated
-                which has a torch autograd value and `x` is the vector on which `ensures_grad` was called.
-            * `ZeroOperator(shape: tuple[int, int])`
-         * Combining operators via:
-            * `A + B`, `A - B`, `A @ B` for `A`, `B` linear operators
-            * `hstack`, `vstack`
-            * `A`, `c A`, `A / c`, `v * A`, `A / v` for scalar `c` and vector `v`.
-        
-        # Implementing `LinearOperator`s
-        
-        To implement a `LinearOperator` the following are mandatory:
-        
-         * Set `_shape: tuple[int, int]`  to the shape of the operator.
-         * Set `device` appropriately, if the operator requires vectors to be on a particular device.
-         *  Implement a method `def _matmul_impl(self, v: torch.Tensor) -> torch.Tensor: ...` that implements your matrix vector product.
-        
-        The following are recommended to improve performance:
-        
-         * If your `_matmul_impl` method handles matrix inputs correctly, set `supports_operator_matrix: bool` to `True`.
-         * If it is possible to describe the adjoint operator, set `_adjoint: LinearOperator` to point to the adjoint of your operator. If you do not compute this, then one will be autogenerated by differentiating through your `_matmul_impl`.
-        
-        It is suggested that, if possible, you replace any other methods with specialized implementations.
-        
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
+License-File: LICENSE.md
+
+# An Abstract Linear Operator Library for pyTorch
+
+This library implements a generic structure for abstract linear operators and
+enables a number of standard operations on them:
+ * Arithmetic: `A + B`, `A - B`, `-A`, `A @ B` all work exactly as expected to
+    combine linear operators.
+ * Indexing: `A[k:ell,m:n]` works as expected.
+ * Solves: `Ax = b` can be solved with `CG` for PSD matrices, `minres` for
+ symmetric matrices, `LSQR` (to be implemented), or `LSMR` (to be implemented).
+ * Trace estimation: The trace of square matrices, can be estimated via Hutch++
+    and Hutchinson's estimator.
+ * [Diamond-Boyd stochastic equilibration](https://web.stanford.edu/~boyd/papers/mf_equil.html)
+ * [Randomized Nyström Preconditioning](https://arxiv.org/abs/2110.02820)
+ * Automatic adjoint operator generation.
+
+# Using `LinearOperator`s
+
+The public API of the `LinearOperator` library is that every `LinearOperator` has the
+following properties and methods:
+```python
+
+class LinearOperator:
+
+    # Properties
+    shape: tuple[int, int]
+    T: LinearOperator
+    supports_operator_matrix: bool
+    device: torch.Device
+
+    # Matrix multiply
+    def __matmul__(self, b: torch.Tensor) -> torch.Tensor: ...
+    def __rmatmul__(self, b: torch.Tensor) -> torch.Tensor: ...
+
+    def __matmul__(self, b: LinearOperator) -> LinearOperator: ...
+    def __rmatmul__(self, b: LinearOperator) -> LinearOperator: ...
+    
+    # Linear Solve Methods
+    def solve_I_p_lambda_AT_A_x_eq_b(self,
+        lambda_: float,
+        b: torch.Tensor,
+        x0: torch.Tensor | None=None,
+        *, precondition: None | Literal['nsytrom'], hot=False) -> torch.Tensor: ...
+
+    def solve_A_x_eq_b(self,
+        b: torch.Tensor,
+        x0: torch.Tensor | None=None) -> torch.Tensor: ...
+
+    # Transformations on LinearOperator
+    def __mul__(self, c: float) -> LinearOperator: ...
+    def __rmul__(self, c: float) -> LinearOperator: ...
+
+    def __truediv__(self, c: float) -> LinearOperator: ...
+
+    def __pow__(self, k: int) -> LinearOperator: ...
+
+    def __add__(self, c: LinearOperator) -> LinearOperator: ...
+
+    def __sub__(self, c: LinearOperator) -> LinearOperator: ...
+
+    def __neg__(self) -> LinearOperator: ...
+
+    def __pos__(self) -> LinearOperator: ...
+
+    def __getitem__(self, key) -> LinearOperator: ...
+```
+
+The following functions are available in the root of the library:
+```python
+def operator_matrix_product(A: LinearOperator, M: torch.Tensor) -> torch.Tensor: ...
+def aslinearoperator(A: torch.Tensor | LinearOperator) -> LinearOperator: ...
+def vstack(ops: list[LinearOperator] | tuple[LinearOperator, ...]) -> LinearOperator: ...
+def hstack(ops: list[LinearOperator] | tuple[LinearOperator, ...]) -> LinearOperator: ...
+
+# To be implemented:
+def bmat(ops: list[list[LinearOperator]]) -> LinearOperator: ... # Optimizes out ZeroOperator
+```
+
+The following functions are available in `linops.trace` for trace estimation:
+```python
+def hutchpp(A: lo.LinearOperator, m: int) -> float: ...
+def hutchinson(A: lo.LinearOperator, m: int) -> float: ...
+```
+
+`linops.equilibration` contains `equilibrate` and `symmetric_equilibrate`.
+Their public API is not finalized, if you wish to use them it is recommend you read the source code.
+
+# Creating Linear Operators
+
+Linear operators can be constructed in the following way:
+ * Creating a sub-class of `LinearOperator` 
+ * Calling one of the following constructors:
+    * `IdentityOperator(n: int)`
+    * `DiagonalOperator(diag: torch.Tensor)`: where `diag` is a 1D torch tensor.
+    * `MatrixOperator(M: torch.Tensor)`: where `M` is a 2D torch tensor.
+    * `SelectionOperator(shape: tuple[int, int], idxs: slice | list[int | slice])`
+    * `KKTOperator(H: LinearOperator, A: LinearOperator)`: where `H` is a square `LinearOperator` and `A` is a `LinearOperator`
+    * `VectorJacobianOperator(f: torch.Tensor, x: torch.Tensor)`: where `f` is the output of the function being differentiated
+        which has a torch autograd value and `x` is the vector on which `ensures_grad` was called.
+    * `ZeroOperator(shape: tuple[int, int])`
+ * Combining operators via:
+    * `A + B`, `A - B`, `A @ B` for `A`, `B` linear operators
+    * `hstack`, `vstack`
+    * `A`, `c A`, `A / c`, `v * A`, `A / v` for scalar `c` and vector `v`.
+
+# Implementing `LinearOperator`s
+
+To implement a `LinearOperator` the following are mandatory:
+
+ * Set `_shape: tuple[int, int]`  to the shape of the operator.
+ * Set `device` appropriately, if the operator requires vectors to be on a particular device.
+ *  Implement a method `def _matmul_impl(self, v: torch.Tensor) -> torch.Tensor: ...` that implements your matrix vector product.
+
+The following are recommended to improve performance:
+
+ * If your `_matmul_impl` method handles matrix inputs correctly, set `supports_operator_matrix: bool` to `True`.
+ * If it is possible to describe the adjoint operator, set `_adjoint: LinearOperator` to point to the adjoint of your operator. If you do not compute this, then one will be autogenerated by differentiating through your `_matmul_impl`.
+
+It is suggested that, if possible, you replace any other methods with specialized implementations.
+
+
```

