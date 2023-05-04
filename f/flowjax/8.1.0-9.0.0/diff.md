# Comparing `tmp/flowjax-8.1.0.tar.gz` & `tmp/flowjax-9.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flowjax-8.1.0.tar", last modified: Sun Feb  5 17:22:43 2023, max compression
+gzip compressed data, was "flowjax-9.0.0.tar", last modified: Thu May  4 19:01:03 2023, max compression
```

## Comparing `flowjax-8.1.0.tar` & `flowjax-9.0.0.tar`

### file list

```diff
@@ -1,41 +1,47 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-05 17:22:43.692125 flowjax-8.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-02-05 17:22:34.000000 flowjax-8.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2515 2023-02-05 17:22:43.692125 flowjax-8.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1940 2023-02-05 17:22:34.000000 flowjax-8.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-05 17:22:43.688125 flowjax-8.1.0/flowjax/
--rw-r--r--   0 runner    (1001) docker     (123)      143 2023-02-05 17:22:34.000000 flowjax-8.1.0/flowjax/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-05 17:22:43.692125 flowjax-8.1.0/flowjax/bijections/
--rw-r--r--   0 runner    (1001) docker     (123)      930 2023-02-05 17:22:34.000000 flowjax-8.1.0/flowjax/bijections/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5280 2023-02-05 17:22:34.000000 flowjax-8.1.0/flowjax/bijections/affine.py
--rw-r--r--   0 runner    (1001) docker     (123)     3401 2023-02-05 17:22:34.000000 flowjax-8.1.0/flowjax/bijections/bijection.py
--rw-r--r--   0 runner    (1001) docker     (123)     3791 2023-02-05 17:22:34.000000 flowjax-8.1.0/flowjax/bijections/block_autoregressive_network.py
--rw-r--r--   0 runner    (1001) docker     (123)     2096 2023-02-05 17:22:34.000000 flowjax-8.1.0/flowjax/bijections/chain.py
--rw-r--r--   0 runner    (1001) docker     (123)     4687 2023-02-05 17:22:34.000000 flowjax-8.1.0/flowjax/bijections/coupling.py
--rw-r--r--   0 runner    (1001) docker     (123)      628 2023-02-05 17:22:34.000000 flowjax-8.1.0/flowjax/bijections/exp.py
--rw-r--r--   0 runner    (1001) docker     (123)     6335 2023-02-05 17:22:34.000000 flowjax-8.1.0/flowjax/bijections/jax_transforms.py
--rw-r--r--   0 runner    (1001) docker     (123)     4866 2023-02-05 17:22:34.000000 flowjax-8.1.0/flowjax/bijections/masked_autoregressive.py
--rw-r--r--   0 runner    (1001) docker     (123)     6043 2023-02-05 17:22:34.000000 flowjax-8.1.0/flowjax/bijections/rational_quadratic_spline.py
--rw-r--r--   0 runner    (1001) docker     (123)     2806 2023-02-05 17:22:34.000000 flowjax-8.1.0/flowjax/bijections/tanh.py
--rw-r--r--   0 runner    (1001) docker     (123)     6581 2023-02-05 17:22:34.000000 flowjax-8.1.0/flowjax/bijections/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    19048 2023-02-05 17:22:34.000000 flowjax-8.1.0/flowjax/distributions.py
--rw-r--r--   0 runner    (1001) docker     (123)    11721 2023-02-05 17:22:34.000000 flowjax-8.1.0/flowjax/flows.py
--rw-r--r--   0 runner    (1001) docker     (123)     1422 2023-02-05 17:22:34.000000 flowjax-8.1.0/flowjax/masks.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-05 17:22:43.692125 flowjax-8.1.0/flowjax/nn/
--rw-r--r--   0 runner    (1001) docker     (123)      248 2023-02-05 17:22:34.000000 flowjax-8.1.0/flowjax/nn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4404 2023-02-05 17:22:34.000000 flowjax-8.1.0/flowjax/nn/block_autoregressive.py
--rw-r--r--   0 runner    (1001) docker     (123)     3339 2023-02-05 17:22:34.000000 flowjax-8.1.0/flowjax/nn/masked_autoregressive.py
--rw-r--r--   0 runner    (1001) docker     (123)      452 2023-02-05 17:22:34.000000 flowjax-8.1.0/flowjax/tasks.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-05 17:22:43.692125 flowjax-8.1.0/flowjax/train/
--rw-r--r--   0 runner    (1001) docker     (123)      181 2023-02-05 17:22:34.000000 flowjax-8.1.0/flowjax/train/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5120 2023-02-05 17:22:34.000000 flowjax-8.1.0/flowjax/train/data_fit.py
--rw-r--r--   0 runner    (1001) docker     (123)     1198 2023-02-05 17:22:34.000000 flowjax-8.1.0/flowjax/train/train_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3645 2023-02-05 17:22:34.000000 flowjax-8.1.0/flowjax/train/variational_fit.py
--rw-r--r--   0 runner    (1001) docker     (123)     3680 2023-02-05 17:22:34.000000 flowjax-8.1.0/flowjax/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-05 17:22:43.688125 flowjax-8.1.0/flowjax.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2515 2023-02-05 17:22:43.000000 flowjax-8.1.0/flowjax.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      913 2023-02-05 17:22:43.000000 flowjax-8.1.0/flowjax.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-05 17:22:43.000000 flowjax-8.1.0/flowjax.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-02-05 17:22:43.000000 flowjax-8.1.0/flowjax.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-02-05 17:22:43.000000 flowjax-8.1.0/flowjax.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-05 17:22:43.692125 flowjax-8.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1204 2023-02-05 17:22:34.000000 flowjax-8.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 19:01:03.688014 flowjax-9.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-05-04 19:00:52.000000 flowjax-9.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2515 2023-05-04 19:01:03.688014 flowjax-9.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1940 2023-05-04 19:00:52.000000 flowjax-9.0.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 19:01:03.684014 flowjax-9.0.0/flowjax/
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-05-04 19:00:52.000000 flowjax-9.0.0/flowjax/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 19:01:03.684014 flowjax-9.0.0/flowjax/bijections/
+-rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-05-04 19:00:52.000000 flowjax-9.0.0/flowjax/bijections/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5298 2023-05-04 19:00:52.000000 flowjax-9.0.0/flowjax/bijections/affine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3371 2023-05-04 19:00:52.000000 flowjax-9.0.0/flowjax/bijections/bijection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3843 2023-05-04 19:00:52.000000 flowjax-9.0.0/flowjax/bijections/block_autoregressive_network.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2139 2023-05-04 19:00:52.000000 flowjax-9.0.0/flowjax/bijections/chain.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5460 2023-05-04 19:00:52.000000 flowjax-9.0.0/flowjax/bijections/concatenate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5208 2023-05-04 19:00:52.000000 flowjax-9.0.0/flowjax/bijections/coupling.py
+-rw-r--r--   0 runner    (1001) docker     (123)      904 2023-05-04 19:00:52.000000 flowjax-9.0.0/flowjax/bijections/exp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7381 2023-05-04 19:00:52.000000 flowjax-9.0.0/flowjax/bijections/jax_transforms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4787 2023-05-04 19:00:52.000000 flowjax-9.0.0/flowjax/bijections/masked_autoregressive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6395 2023-05-04 19:00:52.000000 flowjax-9.0.0/flowjax/bijections/rational_quadratic_spline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3313 2023-05-04 19:00:52.000000 flowjax-9.0.0/flowjax/bijections/tanh.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7354 2023-05-04 19:00:52.000000 flowjax-9.0.0/flowjax/bijections/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20455 2023-05-04 19:00:52.000000 flowjax-9.0.0/flowjax/distributions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12644 2023-05-04 19:00:52.000000 flowjax-9.0.0/flowjax/flows.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1418 2023-05-04 19:00:52.000000 flowjax-9.0.0/flowjax/masks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 19:01:03.684014 flowjax-9.0.0/flowjax/nn/
+-rw-r--r--   0 runner    (1001) docker     (123)      378 2023-05-04 19:00:52.000000 flowjax-9.0.0/flowjax/nn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4651 2023-05-04 19:00:52.000000 flowjax-9.0.0/flowjax/nn/block_autoregressive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3496 2023-05-04 19:00:52.000000 flowjax-9.0.0/flowjax/nn/masked_autoregressive.py
+-rw-r--r--   0 runner    (1001) docker     (123)      460 2023-05-04 19:00:52.000000 flowjax-9.0.0/flowjax/tasks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 19:01:03.684014 flowjax-9.0.0/flowjax/train/
+-rw-r--r--   0 runner    (1001) docker     (123)      305 2023-05-04 19:00:52.000000 flowjax-9.0.0/flowjax/train/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5318 2023-05-04 19:00:52.000000 flowjax-9.0.0/flowjax/train/data_fit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1257 2023-05-04 19:00:52.000000 flowjax-9.0.0/flowjax/train/train_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4097 2023-05-04 19:00:52.000000 flowjax-9.0.0/flowjax/train/variational_fit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3372 2023-05-04 19:00:52.000000 flowjax-9.0.0/flowjax/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 19:01:03.684014 flowjax-9.0.0/flowjax.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2515 2023-05-04 19:01:03.000000 flowjax-9.0.0/flowjax.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1035 2023-05-04 19:01:03.000000 flowjax-9.0.0/flowjax.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 19:01:03.000000 flowjax-9.0.0/flowjax.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-04 19:01:03.000000 flowjax-9.0.0/flowjax.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-04 19:01:03.000000 flowjax-9.0.0/flowjax.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-04 19:01:03.688014 flowjax-9.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1189 2023-05-04 19:00:52.000000 flowjax-9.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 19:01:03.688014 flowjax-9.0.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     5387 2023-05-04 19:00:52.000000 flowjax-9.0.0/tests/test_distributions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2312 2023-05-04 19:00:52.000000 flowjax-9.0.0/tests/test_flows.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-05-04 19:00:52.000000 flowjax-9.0.0/tests/test_masks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1514 2023-05-04 19:00:52.000000 flowjax-9.0.0/tests/test_utils.py
```

### Comparing `flowjax-8.1.0/LICENSE` & `flowjax-9.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `flowjax-8.1.0/PKG-INFO` & `flowjax-9.0.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flowjax
-Version: 8.1.0
+Version: 9.0.0
 Summary: Normalizing flow implementations in jax.
 Home-page: https://github.com/danielward27/flowjax.git
 Author: Daniel Ward
 Author-email: danielward27@outlook.com
 License: MIT
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `flowjax-8.1.0/README.md` & `flowjax-9.0.0/README.md`

 * *Files identical despite different names*

### Comparing `flowjax-8.1.0/flowjax/bijections/__init__.py` & `flowjax-9.0.0/flowjax/bijections/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,35 +1,39 @@
 """Bijections from ``flowjax.bijections``"""
 
-from .bijection import Bijection
 from .affine import AdditiveLinearCondition, Affine, TriangularAffine
+from .bijection import Bijection
 from .block_autoregressive_network import BlockAutoregressiveNetwork
 from .chain import Chain
+from .concatenate import Concatenate, Stack
 from .coupling import Coupling
+from .exp import Exp
+from .jax_transforms import Scan, Batch
 from .masked_autoregressive import MaskedAutoregressive
+from .rational_quadratic_spline import RationalQuadraticSpline
 from .tanh import Tanh, TanhLinearTails
-from .exp import Exp
+
 from .utils import EmbedCondition, Flip, Invert, Partial, Permute
-from .rational_quadratic_spline import RationalQuadraticSpline
-from .jax_transforms import Scan, Vmap
 
 __all__ = [
     "Bijection",
     "Affine",
     "TriangularAffine",
     "BlockAutoregressiveNetwork",
     "Coupling",
     "MaskedAutoregressive",
     "Tanh",
     "Exp",
     "TanhLinearTails",
     "Chain",
     "Scan",
-    "Vmap",
+    "Batch",
     "Invert",
     "Flip",
     "Permute",
     "AdditiveLinearCondition",
     "Partial",
     "EmbedCondition",
     "RationalQuadraticSpline",
+    "Concatenate",
+    "Stack",
 ]
```

### Comparing `flowjax-8.1.0/flowjax/bijections/affine.py` & `flowjax-9.0.0/flowjax/bijections/affine.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,86 +1,90 @@
-from typing import Optional
+"""Affine bijections."""
 
 import jax.numpy as jnp
+from jax import Array
 from jax.experimental import checkify
 from jax.scipy.linalg import solve_triangular
+from jax.typing import ArrayLike
 
-from flowjax.bijections import Bijection
-from flowjax.utils import Array
-from jax.experimental import checkify
+from flowjax.bijections.bijection import Bijection
 
 
 class Affine(Bijection):
+    """Elementwise affine transformation ``y = a*x + b``. loc and scale should broadcast
+    to the desired shape of the bijection.
+    """
+
     loc: Array
     log_scale: Array
-    
-    def __init__(self, loc: Array=0, scale: Array=1):
-        """Elementwise affine transformation y = ax + b. loc and scale should broadcast
-        to the desired shape of the bijection.
 
+    def __init__(self, loc: ArrayLike = 0, scale: ArrayLike = 1):
+        """
         Args:
-            loc (int, optional): Location parameter. Defaults to 0.
-            scale (int, optional): Scale parameter. Defaults to 1.
+            loc (int): Location parameter. Defaults to 0.
+            scale (int): Scale parameter. Defaults to 1.
         """
         loc, scale = [jnp.asarray(a, dtype=jnp.float32) for a in (loc, scale)]
         self.shape = jnp.broadcast_shapes(jnp.shape(loc), jnp.shape(scale))
         self.cond_shape = None
 
         self.loc = jnp.broadcast_to(loc, self.shape)
         self.log_scale = jnp.broadcast_to(jnp.log(scale), self.shape)
 
     def transform(self, x, condition=None):
         self._argcheck(x)
         return x * self.scale + self.loc
 
-    def transform_and_log_abs_det_jacobian(self, x, condition=None):
+    def transform_and_log_det(self, x, condition=None):
         self._argcheck(x)
         return x * self.scale + self.loc, self.log_scale.sum()
 
     def inverse(self, y, condition=None):
         self._argcheck(y)
         return (y - self.loc) / self.scale
 
-    def inverse_and_log_abs_det_jacobian(self, y, condition=None):
+    def inverse_and_log_det(self, y, condition=None):
         self._argcheck(y)
         return (y - self.loc) / self.scale, -self.log_scale.sum()
 
     @property
     def scale(self):
+        """The scale parameter of the affine transformation."""
         return jnp.exp(self.log_scale)
 
 
 class TriangularAffine(Bijection):
     """Transformation of the form ``Ax + b``, where ``A`` is a lower or upper triangular matrix."""
 
     loc: Array
     diag_idxs: Array
     tri_mask: Array
     lower: bool
-    weight_log_scale: Optional[Array]
+    weight_log_scale: Array | None
     _arr: Array
     _log_diag: Array
 
     def __init__(
         self,
         loc: Array,
         arr: Array,
         lower: bool = True,
         weight_normalisation: bool = False,
     ):
         """
         Args:
             loc (Array): Location parameter.
             arr (Array): Triangular matrix.
-            lower (bool, optional): Whether the mask should select the lower or upper triangular matrix (other elements ignored). Defaults to True.
-            weight_log_scale (Optional[Array], optional): If provided, carry out weight normalisation.
+            lower (bool): Whether the mask should select the lower or upper
+                triangular matrix (other elements ignored). Defaults to True.
+            weight_log_scale (Array | None): If provided, carry out weight
+                normalisation.
         """
-
         if (arr.ndim != 2) or (arr.shape[0] != arr.shape[1]):
-            ValueError("arr must be a square, 2-dimensional matrix.")
+            raise ValueError("arr must be a square, 2-dimensional matrix.")
         checkify.check(
             jnp.all(jnp.diag(arr) > 0),
             "arr diagonal entries must be greater than 0",
         )
         dim = arr.shape[0]
         self.diag_idxs = jnp.diag_indices(dim)
         tri_mask = jnp.tril(jnp.ones((dim, dim), dtype=jnp.int32), k=-1)
@@ -94,67 +98,69 @@
         self.weight_log_scale = jnp.zeros((dim, 1)) if weight_normalisation else None
 
         self.shape = (dim,)
         self.cond_shape = None
 
     @property
     def arr(self):
-        "Get triangular array, (applies masking and min_diag constraint)."
+        """Get triangular array, (applies masking and min_diag constraint)."""
         diag = jnp.exp(self._log_diag)
         off_diag = self.tri_mask * self._arr
         arr = off_diag.at[self.diag_idxs].set(diag)
 
         if self.weight_log_scale is not None:
             norms = jnp.linalg.norm(arr, axis=1, keepdims=True)
             arr = jnp.exp(self.weight_log_scale) * arr / norms
 
         return arr
 
     def transform(self, x, condition=None):
         self._argcheck(x)
         return self.arr @ x + self.loc
 
-    def transform_and_log_abs_det_jacobian(self, x, condition=None):
+    def transform_and_log_det(self, x, condition=None):
         self._argcheck(x)
-        a = self.arr
-        return a @ x + self.loc, jnp.log(jnp.diag(a)).sum()
+        arr = self.arr
+        return arr @ x + self.loc, jnp.log(jnp.diag(arr)).sum()
 
     def inverse(self, y, condition=None):
         self._argcheck(y)
         return solve_triangular(self.arr, y - self.loc, lower=self.lower)
 
-    def inverse_and_log_abs_det_jacobian(self, y, condition=None):
+    def inverse_and_log_det(self, y, condition=None):
         self._argcheck(y)
-        a = self.arr
-        x = solve_triangular(a, y - self.loc, lower=self.lower)
-        return x, -jnp.log(jnp.diag(a)).sum()
+        arr = self.arr
+        x = solve_triangular(arr, y - self.loc, lower=self.lower)
+        return x, -jnp.log(jnp.diag(arr)).sum()
 
 
 class AdditiveLinearCondition(Bijection):
     """Carries out ``y = x + W @ condition``, as the forward transformation and
-    ``x = y - W @ condition`` as the inverse."""
+    ``x = y - W @ condition`` as the inverse.
+    """
 
     W: Array
 
     def __init__(self, arr: Array):
         """
         Args:
             arr (Array): Array (``W`` in the description.)
         """
         self.W = arr
-        super().__init__(shape=(arr.shape[-2],), cond_shape=(arr.shape[-1],))
+        self.shape = (arr.shape[-2],)
+        self.cond_shape = (arr.shape[-1],)
 
     def transform(self, x, condition=None):
         self._argcheck(x, condition)
         return x + self.W @ condition
 
-    def transform_and_log_abs_det_jacobian(self, x, condition=None):
+    def transform_and_log_det(self, x, condition=None):
         self._argcheck(x, condition)
         return self.transform(x, condition), jnp.array(0)
 
     def inverse(self, y, condition=None):
         self._argcheck(y, condition)
         return y - self.W @ condition
 
-    def inverse_and_log_abs_det_jacobian(self, y, condition=None):
+    def inverse_and_log_det(self, y, condition=None):
         self._argcheck(y, condition)
         return self.inverse(y, condition), jnp.array(0)
```

### Comparing `flowjax-8.1.0/flowjax/bijections/bijection.py` & `flowjax-9.0.0/flowjax/bijections/bijection.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,79 +1,78 @@
-"""
-Abstact base classes for the `Bijection` and `Bijection` types. Note when implementing bijections,
-by convention we try to i) implement the "transform" methods as the faster/more intuitive approach 
-(compared to the inverse methods); and ii) implement only the forward methods if an inverse
-is not available. The `Invert` bijection can be used to invert the orientation if a fast inverse is
-desired (e.g. maximum likelihood fitting of flows).
+"""Abstact base classes for the `Bijection` and `Bijection` types. Note when implementing
+bijections, by convention we try to i) implement the "transform" methods as the
+faster/more intuitive approach (compared to the inverse methods); and ii) implement only
+the forward methods if an inverse is not available. The `Invert` bijection can be used
+to invert the orientation if a fast inverse is desired (e.g. maximum likelihood fitting
+of flows).
 """
 
-from abc import ABC, abstractmethod
-from typing import Optional, Tuple, Union
+from abc import abstractmethod
 
 from equinox import Module
+from jax import Array
 
-from flowjax.utils import Array
-
-
-class Bijection(ABC, Module):
 
+class Bijection(Module):
     """Bijection base class. Similar to :py:class:`~flowjax.distributions.Distribution`,
     bijections have a ``shape`` and a ``cond_shape`` attribute. To allow easy composing
     of bijections, all bijections support passing of conditioning variables (even if
     ignored). Unlike distributions, the ``shape`` attribute can be None, for cases where
     the shape may be unknown, or unimportant (e.g. the
     :py:class:`~flowjax.bijections.tanh.Tanh` bijection is compatible with any shape of
     input).
 
     The methods of bijections do not generally support passing of additional batch
     dimensions, however, ``jax.vmap`` or ``eqx.filter_vmap`` can be used to vmap
     specific methods if desired, and a bijection can be explicitly vectorised using the
-    :py:class:`~flowjax.bijections.jax_transforms.Vmap` bijection.
+    :py:class:`~flowjax.bijections.jax_transforms.Batch` bijection.
 
     Bijections are registered as Jax PyTrees (as they are equinox modules), so are
     compatible with normal jax operations.
 
     Implementing a bijection
 
         (1) Inherit from ``Bijection``.
         (2) Define the attributes ``shape`` and ``cond_shape``
-        (3) Implement the abstract methods ``transform``, ``transform_and_log_abs_det_jacobian``,
-            ``inverse`` and ``inverse_and_log_abs_det_jacobian``. These should act on inputs compatible
-            with the shapes ``shape`` for ``x``, and ``cond_shape`` for ``condition``.
+        (3) Implement the abstract methods ``transform``, ``transform_and_log_det``,
+            ``inverse`` and ``inverse_and_log_det``. These should act on
+            inputs compatible with the shapes ``shape`` for ``x``, and ``cond_shape``
+            for ``condition``.
 
     """
 
-    shape: Union[None, Tuple[int]]
-    cond_shape: Union[None, Tuple[int]]
+    shape: tuple[int, ...]
+    cond_shape: tuple[int, ...] | None
 
     @abstractmethod
-    def transform(self, x: Array, condition: Optional[Array] = None) -> Array:
+    def transform(self, x: Array, condition: Array | None = None) -> Array:
         """Apply transformation."""
 
     @abstractmethod
-    def transform_and_log_abs_det_jacobian(
-        self, x: Array, condition: Optional[Array] = None
-    ) -> Tuple:
+    def transform_and_log_det(
+        self, x: Array, condition: Array | None = None
+    ) -> tuple[Array, Array]:
         """Apply transformation and compute log absolute value of the Jacobian determinant."""
 
     @abstractmethod
-    def inverse(self, y: Array, condition: Optional[Array] = None) -> Array:
+    def inverse(self, y: Array, condition: Array | None = None) -> Array:
         """Invert the transformation."""
 
     @abstractmethod
-    def inverse_and_log_abs_det_jacobian(
-        self, y: Array, condition: Optional[Array] = None
-    ) -> Array:
+    def inverse_and_log_det(
+        self, y: Array, condition: Array | None = None
+    ) -> tuple[Array, Array]:
         """Invert the transformation and compute log absolute value of the Jacobian determinant."""
 
-    def _argcheck(self, x, condition=None):
-        "Utility argcheck that can be added to bijection methods as required."
-        if x.shape != self.shape:
-            raise ValueError(f"Expected x.shape {self.shape}, got {x.shape}")
+    def _argcheck(self, x: Array, condition: Array | None = None):
+        """Utility argcheck that can be added to bijection methods as required."""
+        if self.shape is not None:
+            if x.shape != self.shape:
+                raise ValueError(f"Expected x.shape {self.shape}, got {x.shape}")
 
         if self.cond_shape is not None:
             if condition is None:
                 raise ValueError("Condition should be provided")
-            elif condition.shape != self.cond_shape:
+            if condition.shape != self.cond_shape:
                 raise ValueError(
                     f"Expected condition.shape {self.cond_shape}, got {condition.shape}"
                 )
```

### Comparing `flowjax-8.1.0/flowjax/bijections/block_autoregressive_network.py` & `flowjax-9.0.0/flowjax/bijections/block_autoregressive_network.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,68 +1,66 @@
-"""
-Block Neural Autoregressive bijection implementation.
-"""
-
-import math
-from typing import Callable, Optional, Union, Tuple
+"""Block Neural Autoregressive bijection implementation."""
+from typing import Callable, Any
 
 import jax
 import jax.numpy as jnp
 from jax import random
 from jax.random import KeyArray
 
-from flowjax.bijections import Bijection
-from flowjax.nn.block_autoregressive import BlockAutoregressiveLinear, BlockTanh
+from flowjax.bijections.bijection import Bijection
+from flowjax.nn.block_autoregressive import (
+    BlockAutoregressiveLinear,
+    _block_tanh_activation,
+)
 
 
 class BlockAutoregressiveNetwork(Bijection):
     """Block Autoregressive Network (https://arxiv.org/abs/1904.04676)."""
 
     depth: int
     layers: list
     block_dim: int
     activation: Callable
 
     def __init__(
         self,
         key: KeyArray,
         dim: int,
-        cond_dim: Union[None, int],
+        cond_dim: int | None,
         depth: int,
         block_dim: int,
-        activation: Optional[Callable] = None,
+        activation: Callable | None = None,
     ):
         """
         Args:
             key (KeyArray): Jax PRNGKey
             dim (int): Dimension of the distribution.
-            cond_dim (Union[None, Tuple[int]]): Dimension of extra conditioning variables.
+            cond_dim (tuple[int, ...] | None): Dimension of extra conditioning variables.
             depth (int): Number of hidden layers in the network.
             block_dim (int): Block dimension (hidden layer size is `dim*block_dim`).
-            activation (Callable, optional): Activation function. Defaults to BlockTanh.
+            activation (Callable): Activation function. Defaults to block_tanh.
         """
-        activation = BlockTanh(dim) if activation is None else activation
-        layers = []
+        activation = _block_tanh_activation(dim) if activation is None else activation
+        layers = []  # type: list[Any]
         if depth == 0:
             layers.append(BlockAutoregressiveLinear(key, dim, (1, 1), cond_dim))
         else:
             keys = random.split(key, depth + 1)
 
             block_shapes = [
                 (block_dim, 1),
                 *[(block_dim, block_dim)] * (depth - 1),
                 (1, block_dim),
             ]
             cond_dims = [cond_dim] + [None] * depth
 
-            for key, block_shape, cd in zip(keys, block_shapes, cond_dims):
-
+            for layer_key, block_shape, cond_d in zip(keys, block_shapes, cond_dims):
                 layers.extend(
                     [
-                        BlockAutoregressiveLinear(key, dim, block_shape, cd),
+                        BlockAutoregressiveLinear(layer_key, dim, block_shape, cond_d),
                         activation,
                     ]
                 )
             layers = layers[:-1]  # remove last activation
 
         self.depth = depth
         self.layers = layers
@@ -74,39 +72,41 @@
     def transform(self, x, condition=None):
         self._argcheck(x, condition)
         x = self.layers[0](x, condition)[0]
         for layer in self.layers[1:]:
             x = layer(x)[0]
         return x
 
-    def transform_and_log_abs_det_jacobian(self, x, condition=None):
+    def transform_and_log_det(self, x, condition=None):
         self._argcheck(x, condition)
-        x, log_det_3d_0 = self.layers[0](x, condition)
-        log_det_3ds = [log_det_3d_0]
+        x, log_jacobian_3d_0 = self.layers[0](x, condition)
+        log_jacobian_3ds = [log_jacobian_3d_0]
         for layer in self.layers[1:]:
             x, log_det_3d = layer(x)
-            log_det_3ds.append(log_det_3d)
+            log_jacobian_3ds.append(log_det_3d)
 
-        logdet = log_det_3ds[-1]
-        for ld in reversed(log_det_3ds[:-1]):  # TODO avoid loop
-            logdet = logmatmulexp(logdet, ld)
-        return x, logdet.sum()
+        log_det = log_jacobian_3ds[-1]
+        for log_jacobian in reversed(log_jacobian_3ds[:-1]):
+            log_det = logmatmulexp(log_det, log_jacobian)
+        return x, log_det.sum()
 
     def inverse(self, *args, **kwargs):
         raise NotImplementedError(
             "This transform would require numerical methods for inversion."
         )
 
-    def inverse_and_log_abs_det_jacobian(self, *args, **kwargs):
+    def inverse_and_log_det(self, *args, **kwargs):
         raise NotImplementedError(
             "This transform would require numerical methods for inversion."
         )
 
 
 def logmatmulexp(x, y):
     """
-    Numerically stable version of ``(x.log() @ y.log()).exp()``. From numpyro https://github.com/pyro-ppl/numpyro/blob/f2ff89a3a7147617e185eb51148eb15d56d44661/numpyro/distributions/util.py#L387
+    Numerically stable version of ``(x.log() @ y.log()).exp()``.
+    From numpyro https://github.com/pyro-ppl/numpyro/blob/
+    f2ff89a3a7147617e185eb51148eb15d56d44661/numpyro/distributions/util.py#L387
     """
     x_shift = jax.lax.stop_gradient(jnp.amax(x, -1, keepdims=True))
     y_shift = jax.lax.stop_gradient(jnp.amax(y, -2, keepdims=True))
     xy = jnp.log(jnp.matmul(jnp.exp(x - x_shift), jnp.exp(y - y_shift)))
     return xy + x_shift + y_shift
```

### Comparing `flowjax-8.1.0/flowjax/bijections/chain.py` & `flowjax-9.0.0/flowjax/bijections/chain.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,62 +1,62 @@
-from typing import Sequence, Tuple, Union
+"""Module contains the Chain bijection, that allows sequentially application of arbitrary
+bijections, with compatible shapes.
+"""
+from typing import Sequence
 
-from flowjax.utils import merge_shapes
-from flowjax.bijections import Bijection
-from flowjax.utils import Array
+from jax import Array
+
+from flowjax.bijections.bijection import Bijection
+from flowjax.utils import merge_cond_shapes, check_shapes_match
 
 
 class Chain(Bijection):
     """Chain together arbitrary bijections to form another bijection."""
 
-    bijections: Tuple[Bijection]
+    bijections: tuple[Bijection]
 
     def __init__(self, bijections: Sequence[Bijection]):
         """
         Args:
             bijections (Sequence[Bijection]): Sequence of bijections.
         """
-        self.shape = merge_shapes([s.shape for s in bijections])
-        self.cond_shape = merge_shapes([b.cond_shape for b in bijections])
+        check_shapes_match([b.shape for b in bijections])
+        self.shape = bijections[0].shape
+        self.cond_shape = merge_cond_shapes([b.cond_shape for b in bijections])
         self.bijections = tuple(bijections)
 
     def transform(self, x, condition=None):
         for bijection in self.bijections:
             x = bijection.transform(x, condition)
         return x
 
-    def transform_and_log_abs_det_jacobian(self, x, condition=None):
+    def transform_and_log_det(self, x, condition=None):
         log_abs_det_jac = 0
         for bijection in self.bijections:
-            x, log_abs_det_jac_i = bijection.transform_and_log_abs_det_jacobian(
-                x, condition
-            )
+            x, log_abs_det_jac_i = bijection.transform_and_log_det(x, condition)
             log_abs_det_jac += log_abs_det_jac_i.sum()
         return x, log_abs_det_jac
 
     def inverse(self, y: Array, condition=None):
         for bijection in reversed(self.bijections):
             y = bijection.inverse(y, condition)
         return y
 
-    def inverse_and_log_abs_det_jacobian(self, y, condition=None):
+    def inverse_and_log_det(self, y, condition=None):
         log_abs_det_jac = 0
         for bijection in reversed(self.bijections):
-            y, log_abs_det_jac_i = bijection.inverse_and_log_abs_det_jacobian(
-                y, condition
-            )
+            y, log_abs_det_jac_i = bijection.inverse_and_log_det(y, condition)
             log_abs_det_jac += log_abs_det_jac_i.sum()
         return y, log_abs_det_jac
 
-    def __getitem__(self, i: Union[int, slice]) -> Bijection:
+    def __getitem__(self, i: int | slice) -> Bijection:
         if isinstance(i, int):
             return self.bijections[i]
-        elif isinstance(i, slice):
+        if isinstance(i, slice):
             return Chain(self.bijections[i])
-        else:
-            raise TypeError(f"Indexing with type {type(i)} is not supported.")
+        raise TypeError(f"Indexing with type {type(i)} is not supported.")
 
     def __iter__(self):
         yield from self.bijections
 
     def __len__(self):
         return len(self.bijections)
```

### Comparing `flowjax-8.1.0/flowjax/bijections/coupling.py` & `flowjax-9.0.0/flowjax/bijections/masked_autoregressive.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,116 +1,127 @@
-from typing import Callable, Union
-import math
+"""Masked autoregressive network and bijection."""
+
+from functools import partial
+from typing import Callable
+
 import equinox as eqx
+import jax
 import jax.nn as jnn
 import jax.numpy as jnp
+from jax import Array
 from jax.random import KeyArray
-from flowjax.bijections import Bijection
-from flowjax.utils import get_ravelled_bijection_constructor, Array
-from flowjax.bijections.jax_transforms import Vmap
+
+from flowjax.bijections.bijection import Bijection
+from flowjax.bijections.jax_transforms import Batch
+from flowjax.nn import AutoregressiveMLP
+from flowjax.utils import get_ravelled_bijection_constructor
 
 
-class Coupling(Bijection):
-    d: int
-    D: int
+class MaskedAutoregressive(Bijection):
+    """Masked autoregressive bijection implementation (https://arxiv.org/abs/1705.07057v4).
+    The transformer is parameterised by a neural network, with weights masked to ensure
+    an autoregressive structure.
+    """
+
     transformer_constructor: Callable
-    conditioner: eqx.nn.MLP
+    autoregressive_mlp: AutoregressiveMLP
 
     def __init__(
         self,
         key: KeyArray,
         transformer: Bijection,
-        d: int,
-        D: int,
-        cond_dim: Union[None, int],
+        dim: int,
+        cond_dim: int | None,
         nn_width: int,
         nn_depth: int,
         nn_activation: Callable = jnn.relu,
-    ):
-        """Coupling layer implementation (https://arxiv.org/abs/1605.08803).
+    ) -> None:
+        """
         Args:
             key (KeyArray): Jax PRNGKey
-            transformer (Bijection): Bijection with shape () to be parameterised by the conditioner neural netork.
-            d (int): Number of untransformed conditioning variables.
-            D (int): Total dimension.
-            cond_dim (Union[None, int]): Dimension of additional conditioning variables.
-            nn_width (int): Neural network hidden layer width.
-            nn_depth (int): Neural network hidden layer size.
-            nn_activation (Callable, optional): Neural network activation function. Defaults to jnn.relu.
+            transformer (Bijection): Bijection with shape () to be parameterised by the
+                autoregressive network.
+            dim (int): Dimension.
+            cond_dim (int | None): Dimension of any conditioning variables.
+            nn_width (int): Neural network width.
+            nn_depth (int): Neural network depth.
+            nn_activation (Callable): Neural network activation. Defaults to jnn.relu.
         """
         if transformer.shape != () or transformer.cond_shape is not None:
             raise ValueError(
                 "Currently, only unconditional transformers with shape () are supported."
             )
 
         constructor, transformer_init_params = get_ravelled_bijection_constructor(
             transformer
         )
 
-        self.transformer_constructor = constructor
-        self.d = d
-        self.D = D
-        self.shape = (D,)
-        self.cond_shape = (cond_dim,) if cond_dim is not None else None
-
-        conditioner_output_size = transformer_init_params.size * (D - d)
-
-        conditioner = eqx.nn.MLP(
-            in_size=d if cond_dim is None else d + cond_dim,
-            out_size=conditioner_output_size,
-            width_size=nn_width,
-            depth=nn_depth,
-            activation=nn_activation,
+        if cond_dim is None:
+            self.cond_shape = None
+            in_ranks = jnp.arange(dim)
+        else:
+            self.cond_shape = (cond_dim,)
+            # we give conditioning variables rank -1 (no masking of edges to output)
+            in_ranks = jnp.hstack((jnp.arange(dim), -jnp.ones(cond_dim)))
+
+        hidden_ranks = jnp.arange(nn_width) % dim
+        out_ranks = jnp.repeat(jnp.arange(dim), transformer_init_params.size)
+
+        autoregressive_mlp = AutoregressiveMLP(
+            in_ranks,
+            hidden_ranks,
+            out_ranks,
+            nn_depth,
+            nn_activation,
             key=key,
         )
 
         # Initialise bias terms to match the provided transformer parameters
-        self.conditioner = eqx.tree_at(
-            where=lambda mlp: mlp.layers[-1].bias,
-            pytree=conditioner,
-            replace=jnp.tile(transformer_init_params, D - d),
+        self.autoregressive_mlp = eqx.tree_at(
+            where=lambda t: t.layers[-1].linear.bias,  # type: ignore
+            pytree=autoregressive_mlp,
+            replace=jnp.tile(transformer_init_params, dim),
         )
 
+        self.transformer_constructor = constructor
+        self.shape = (dim,)
+        self.cond_shape = None if cond_dim is None else (cond_dim,)
+
     def transform(self, x, condition=None):
-        x_cond, x_trans = x[: self.d], x[self.d :]
-        nn_input = x_cond if condition is None else jnp.hstack((x_cond, condition))
-        transformer_params = self.conditioner(nn_input)
+        nn_input = x if condition is None else jnp.hstack((x, condition))
+        transformer_params = self.autoregressive_mlp(nn_input)
         transformer = self._flat_params_to_transformer(transformer_params)
-        y_trans = transformer.transform(x_trans)
-        y = jnp.hstack((x_cond, y_trans))
-        return y
-
-    def transform_and_log_abs_det_jacobian(self, x, condition=None):
-        x_cond, x_trans = x[: self.d], x[self.d :]
-        nn_input = x_cond if condition is None else jnp.hstack((x_cond, condition))
-        transformer_params = self.conditioner(nn_input)
+        return transformer.transform(x)
+
+    def transform_and_log_det(self, x, condition=None):
+        nn_input = x if condition is None else jnp.hstack((x, condition))
+        transformer_params = self.autoregressive_mlp(nn_input)
         transformer = self._flat_params_to_transformer(transformer_params)
-        y_trans, log_det = transformer.transform_and_log_abs_det_jacobian(x_trans)
-        y = jnp.hstack((x_cond, y_trans))
-        return y, log_det
+        return transformer.transform_and_log_det(x)
 
     def inverse(self, y, condition=None):
-        x_cond, y_trans = y[: self.d], y[self.d :]
-        nn_input = x_cond if condition is None else jnp.concatenate((x_cond, condition))
-        transformer_params = self.conditioner(nn_input)
-        transformer = self._flat_params_to_transformer(transformer_params)
-        x_trans = transformer.inverse(y_trans)
-        x = jnp.hstack((x_cond, x_trans))
+        init = (y, 0)
+        fn = partial(self.inv_scan_fn, condition=condition)
+        (x, _), _ = jax.lax.scan(fn, init, None, length=len(y))
         return x
 
-    def inverse_and_log_abs_det_jacobian(self, y, condition=None):
-        x_cond, y_trans = y[: self.d], y[self.d :]
-        nn_input = x_cond if condition is None else jnp.concatenate((x_cond, condition))
-        transformer_params = self.conditioner(nn_input)
+    def inv_scan_fn(self, init, _, condition):
+        """One 'step' in computing the inverse."""
+        y, rank = init
+        nn_input = y if condition is None else jnp.hstack((y, condition))
+        transformer_params = self.autoregressive_mlp(nn_input)
         transformer = self._flat_params_to_transformer(transformer_params)
-        x_trans, log_det = transformer.inverse_and_log_abs_det_jacobian(y_trans)
-        x = jnp.hstack((x_cond, x_trans))
-        return x, log_det
-
-    def _flat_params_to_transformer(
-        self, params: Array
-    ):  # TODO code repetition with MAF
-        "Reshape to dim X params_per_dim, then vmap."
-        dim = self.D - self.d
+        x = transformer.inverse(y)
+        x = y.at[rank].set(x[rank])
+        return (x, rank + 1), None
+
+    def inverse_and_log_det(self, y, condition=None):
+        x = self.inverse(y, condition)
+        log_det = self.transform_and_log_det(x, condition)[1]
+        return x, -log_det
+
+    def _flat_params_to_transformer(self, params: Array):
+        """Reshape to dim X params_per_dim, then vmap."""
+        dim = self.shape[-1]  # type: ignore
         transformer_params = jnp.reshape(params, (dim, -1))
         transformer = eqx.filter_vmap(self.transformer_constructor)(transformer_params)
-        return Vmap(transformer, (dim,))
+        return Batch(transformer, (dim,), vectorize_bijection=True)
```

### Comparing `flowjax-8.1.0/flowjax/bijections/jax_transforms.py` & `flowjax-9.0.0/flowjax/bijections/jax_transforms.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,108 +1,142 @@
+"""Bijections that wrap jax function transforms (scan and vmap)."""
 from functools import partial
+from typing import Any, Callable
+
 import equinox as eqx
-from flowjax.bijections import Bijection
 from jax.lax import scan
-from typing import Any, Tuple
+import jax.numpy as jnp
+from flowjax.bijections.bijection import Bijection
 
 
-class Vmap(Bijection):
-    """Expand the dimension of a bijection by vmapping. By default, we vmap over both the
-    bijection parameters and x, although this behaviour can be modified by providing key
-    word arguments that are passed to ``equinox.filter_vmap``. The arguments names for
-    the vmapped functions are (bijection, x).
-    
-    Vmapping over the conditioning variable is not currently supported.
+class Batch(Bijection):
+    """Add batch dimensions to a bijection, such that the new shape is
+    batch_shape + bijection.shape. The batch dimensions are added using multiple
+    applications of eqx.filter_vmap.
 
     Example:
-        Affine parameters usually act elementwise, but we could vmap excluding the
-        the bijection to create a global affine (sharing the location and scale).
-        
-        .. doctest::
-
-            >>> from flowjax.bijections import Vmap, Affine
-            >>> import jax.numpy as jnp
-            >>> affine = Vmap(Affine(1), (3,), kwargs=dict(bijection=None))
-            >>> affine.transform(jnp.ones(3))
-            Array([2., 2., 2.], dtype=float32)
 
+    .. doctest::
+
+        >>> import jax.numpy as jnp
+        >>> from flowjax.bijections import Batch, Affine
+        >>> x = jnp.ones(2)
+        >>> batched = Batch(Affine(1), (2,), vectorize_bijection=False)
+        >>> batched.transform(x)
+        Array([2., 2.], dtype=float32)
     """
 
-    ndim_to_add: int
     bijection: Bijection
-    kwargs: dict
+    in_axes: tuple
+    batch_shape: tuple[int, ...]
 
-    def __init__(self, bijection: Bijection, shape: Tuple[int], **kwargs):
+    def __init__(
+        self,
+        bijection: Bijection,
+        batch_shape: tuple[int, ...],
+        vectorize_bijection: bool,
+        vectorize_condition: bool | None = None,
+    ):
         """
-        
-
         Args:
-            bijection (Bijection): Bijection. If vmapping over the bijection, the array leaves
-                in bijection should have additional leading axes with shape equalling `shape`.
-                Often it is convenient to construct these using `equinox.filter_vmap`.
-            shape (Tuple[int]): Shape prepended to the bijection shape. If len(shape)>1, multiple applications of vmap will be used.
-            **kwargs: kwargs, passed to equinox.filter_vmap, allowing e.g. control over which variables to map over.
+            bijection (Bijection): Bijection to add batch dimensions to.
+            batch_shape (tuple[int, ...]): The shape of the batch dimension.
+            vectorize_bijection (bool): Whether to vectorise bijection parameters.
+                * If True: we vectorize across the leading dimensions in the array
+                leaves of the bijection. In this case, the array leaves must
+                have leading dimensions equal to batch_shape. For construction of
+                compatible bijections, see eqx.filter_vmap.
+                * If False: we broadcast the parameters, meaning
+                the same bijection parameters are used for each x.
+            vectorize_condition (bool | None): Whether to vectorize or broadcast the
+                conditioning variables. If broadcasting, the condition shape is
+                unchanged. If vectorising, the condition shape will be
+                ``batch_shape + bijection.cond_shape``. Defaults to None.
         """
-
-        self.bijection = bijection
-        self.ndim_to_add = len(shape)
-        self.kwargs = kwargs  # For filter vmap
-        self.shape = (
-            shape + self.bijection.shape if self.bijection.shape is not None else None
+        if vectorize_condition is None and bijection.cond_shape is not None:
+            raise ValueError(
+                "vectorize_condition must be specified for conditional bijections."
+            )
+
+        self.in_axes = (
+            eqx.if_array(axis=0) if vectorize_bijection else None,
+            eqx.if_array(axis=0),
+            0 if vectorize_condition else None,
         )
-        self.cond_shape = bijection.cond_shape
+        self.shape = batch_shape + bijection.shape
+        self.batch_shape = batch_shape
+        self.bijection = bijection
+
+        if self.bijection.cond_shape is None:
+            self.cond_shape = None
+        elif vectorize_condition:
+            self.cond_shape = batch_shape + self.bijection.cond_shape
+        else:
+            self.cond_shape = self.bijection.cond_shape
 
     def transform(self, x, condition=None):
         self._argcheck(x, condition)
-        f = lambda bijection, x: bijection.transform(x, condition)
-        f = self._multivmap(f)
-        return f(self.bijection, x)
+
+        def _transform(bijection, x, condition):
+            return bijection.transform(x, condition)
+
+        return self.multi_vmap(_transform)(self.bijection, x, condition)
+
+    def transform_and_log_det(self, x, condition=None):
+        self._argcheck(x, condition)
+
+        def _transform_and_log_det(bijection, x, condition):
+            return bijection.transform_and_log_det(x, condition)
+
+        y, log_det = self.multi_vmap(_transform_and_log_det)(
+            self.bijection, x, condition
+        )
+        return y, jnp.sum(log_det)
 
     def inverse(self, y, condition=None):
         self._argcheck(y, condition)
-        f = lambda bijection, x: bijection.inverse(x, condition)
-        f = self._multivmap(f)
-        return f(self.bijection, y)
 
-    def transform_and_log_abs_det_jacobian(self, x, condition=None):
-        self._argcheck(x, condition)
-        f = lambda bijection, x: bijection.transform_and_log_abs_det_jacobian(x, condition)
-        f = self._multivmap(f)
-        y, log_det = f(self.bijection, x)
-        return y, log_det.sum()
+        def _inverse(bijection, x, condition):
+            return bijection.inverse(x, condition)
 
-    def inverse_and_log_abs_det_jacobian(self, y, condition=None):
+        return self.multi_vmap(_inverse)(self.bijection, y, condition)
+
+    def inverse_and_log_det(self, y, condition=None):
         self._argcheck(y, condition)
-        f = lambda bijection, x: bijection.inverse_and_log_abs_det_jacobian(x, condition)
-        f = self._multivmap(f)
-        x, log_det = f(self.bijection, y)
-        return x, log_det.sum()
-
-    def _multivmap(self, f):
-        "Compose Vmap to add ndim batch dimensions."
-        for _ in range(self.ndim_to_add):
-            f = eqx.filter_vmap(f, **self.kwargs)
-        return f
+
+        def _inverse_and_log_det(bijection, x, condition):
+            return bijection.inverse_and_log_det(x, condition)
+
+        x, log_det = self.multi_vmap(_inverse_and_log_det)(self.bijection, y, condition)
+        return x, jnp.sum(log_det)
+
+    def multi_vmap(self, func: Callable) -> Callable:
+        """Compose vmap to add ndim batch dimensions."""
+        for _ in range(len(self.batch_shape)):
+            func = eqx.filter_vmap(func, in_axes=self.in_axes)
+        return func
 
 
 class Scan(Bijection):
     """Repeatedly apply the same bijection with different parameter values. Internally,
-    uses `jax.lax.scan` to reduce compilation time."""
+    uses `jax.lax.scan` to reduce compilation time.
+    """
 
     static: Any
     params: Any
 
     def __init__(self, bijection: Bijection):
         """
         The array leaves in `bijection` should have an additional leading axis to scan over.
         Often it is convenient to construct these using `equinox.filter_vmap`.
 
         Args:
-            bijection (Bijection): A bijection, in which the arrays leaves have an additional leading axis to scan over.
-                For complex bijections, it can be convenient to create compatible bijections with ``equinox.filter_vmap``.
+            bijection (Bijection): A bijection, in which the arrays leaves have an
+                additional leading axis to scan over. For complex bijections, it can be
+                convenient to create compatible bijections with ``equinox.filter_vmap``.
 
         Example:
             Below is equivilent to ``Chain([Affine(p) for p in params])``.
 
             .. doctest::
 
                 >>> from flowjax.bijections import Scan, Affine
@@ -115,53 +149,53 @@
         self.params, self.static = eqx.partition(bijection, eqx.is_array)  # type: ignore
         self.shape = bijection.shape
         self.cond_shape = bijection.cond_shape
 
     def transform(self, x, condition=None):
         self._argcheck(x, condition)
 
-        def fn(x, p, condition=None):
-            bijection = eqx.combine(self.static, p)
+        def step(x, params, condition=None):
+            bijection = eqx.combine(self.static, params)
             result = bijection.transform(x, condition)  # type: ignore
             return (result, None)
 
-        fn = partial(fn, condition=condition)
-        y, _ = scan(fn, x, self.params)
+        step = partial(step, condition=condition)
+        y, _ = scan(step, x, self.params)
         return y
 
-    def transform_and_log_abs_det_jacobian(self, x, condition=None):
+    def transform_and_log_det(self, x, condition=None):
         self._argcheck(x, condition)
 
-        def fn(carry, p, condition):
+        def step(carry, params, condition):
             x, log_det = carry
-            bijection = eqx.combine(self.static, p)
-            y, log_det_i = bijection.transform_and_log_abs_det_jacobian(x, condition)  # type: ignore
+            bijection = eqx.combine(self.static, params)
+            y, log_det_i = bijection.transform_and_log_det(x, condition)  # type: ignore
             return ((y, log_det + log_det_i.sum()), None)
 
-        fn = partial(fn, condition=condition)
-        (y, log_det), _ = scan(fn, (x, 0), self.params)
+        step = partial(step, condition=condition)
+        (y, log_det), _ = scan(step, (x, 0), self.params)
         return y, log_det
 
     def inverse(self, y, condition=None):
         self._argcheck(y, condition)
 
-        def fn(y, p, condition=None):
-            bijection = eqx.combine(self.static, p)
+        def step(y, params, condition):
+            bijection = eqx.combine(self.static, params)
             x = bijection.inverse(y, condition)  # type: ignore
             return (x, None)
 
-        fn = partial(fn, condition=condition)
-        x, _ = scan(fn, y, self.params, reverse=True)
+        step = partial(step, condition=condition)
+        x, _ = scan(step, y, self.params, reverse=True)
         return x
 
-    def inverse_and_log_abs_det_jacobian(self, y, condition=None):
+    def inverse_and_log_det(self, y, condition=None):
         self._argcheck(y, condition)
 
-        def fn(carry, p, condition=None):
+        def step(carry, params, condition):
             y, log_det = carry
-            bijection = eqx.combine(self.static, p)
-            x, log_det_i = bijection.inverse_and_log_abs_det_jacobian(y, condition)  # type: ignore
+            bijection = eqx.combine(self.static, params)
+            x, log_det_i = bijection.inverse_and_log_det(y, condition)  # type: ignore
             return ((x, log_det + log_det_i.sum()), None)
 
-        fn = partial(fn, condition=condition)
-        (y, log_det), _ = scan(fn, (y, 0), self.params, reverse=True)
+        step = partial(step, condition=condition)
+        (y, log_det), _ = scan(step, (y, 0), self.params, reverse=True)
         return y, log_det
```

### Comparing `flowjax-8.1.0/flowjax/bijections/masked_autoregressive.py` & `flowjax-9.0.0/flowjax/bijections/coupling.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,129 +1,127 @@
-"""Masked autoregressive network and bijection."""
+"""Implemenetation of Coupling flow layer with arbitrary transformer.
+See https://arxiv.org/abs/1605.08803 for more information.
+"""
+from typing import Callable
 
-from functools import partial
-from typing import Callable, Union
-
-import jax
+import equinox as eqx
 import jax.nn as jnn
 import jax.numpy as jnp
 from jax.random import KeyArray
-import equinox as eqx
 
-from flowjax.bijections import Bijection
-from flowjax.nn import AutoregressiveMLP
-from flowjax.utils import Array, tile_until_length, get_ravelled_bijection_constructor
+from flowjax.bijections.bijection import Bijection
+from flowjax.bijections.jax_transforms import Batch
+from flowjax.utils import Array, get_ravelled_bijection_constructor
 
-from flowjax.bijections.jax_transforms import Vmap
 
+class Coupling(Bijection):
+    """Coupling layer implementation (https://arxiv.org/abs/1605.08803)."""
 
-class MaskedAutoregressive(Bijection):
+    untransformed_dim: int
+    dim: int
     transformer_constructor: Callable
-    autoregressive_mlp: AutoregressiveMLP
+    conditioner: eqx.nn.MLP
 
     def __init__(
         self,
         key: KeyArray,
         transformer: Bijection,
+        untransformed_dim: int,
         dim: int,
-        cond_dim: Union[None, int],
+        cond_dim: int | None,
         nn_width: int,
         nn_depth: int,
         nn_activation: Callable = jnn.relu,
-    ) -> None:
-        """Masked autoregressive bijection implementation (https://arxiv.org/abs/1705.07057v4).
-        The transformer is parameterised by a neural network, with weights masked to ensure
-        an autoregressive structure.
-
+    ):
+        """
         Args:
             key (KeyArray): Jax PRNGKey
-            transformer (Bijection): Bijection with shape () to be parameterised by the autoregressive network.
-            dim (int): Dimension.
-            cond_dim (Union[None, int]): Dimension of any conditioning variables.
-            nn_width (int): Neural network width.
-            nn_depth (int): Neural network depth.
-            nn_activation (Callable, optional): Neural network activation. Defaults to jnn.relu.
+            transformer (Bijection): Unconditional bijection with shape () to be
+                parameterised by the conditioner neural netork.
+            untransformed_dim (int): Number of untransformed conditioning variables (
+                e.g. dim // 2).
+            dim (int): Total dimension.
+            cond_dim (int | None): Dimension of additional conditioning variables.
+            nn_width (int): Neural network hidden layer width.
+            nn_depth (int): Neural network hidden layer size.
+            nn_activation (Callable): Neural network activation function.
+                Defaults to jnn.relu.
         """
         if transformer.shape != () or transformer.cond_shape is not None:
             raise ValueError(
                 "Currently, only unconditional transformers with shape () are supported."
             )
 
         constructor, transformer_init_params = get_ravelled_bijection_constructor(
             transformer
         )
 
-        if cond_dim is None:
-            self.cond_shape = None
-            in_ranks = jnp.arange(dim)
-        else:
-            self.cond_shape = (cond_dim,)
-            # we give conditioning variables rank -1 (no masking of edges to output)
-            in_ranks = jnp.hstack((jnp.arange(dim), -jnp.ones(cond_dim)))
-
-        hidden_ranks = tile_until_length(jnp.arange(dim), nn_width)
-
-        out_ranks = jnp.repeat(jnp.arange(dim), transformer_init_params.size)
-
-        autoregressive_mlp = AutoregressiveMLP(
-            in_ranks,
-            hidden_ranks,
-            out_ranks,
-            nn_depth,
-            nn_activation,
-            key=key,
-        )
+        self.transformer_constructor = constructor
+        self.untransformed_dim = untransformed_dim
+        self.dim = dim
+        self.shape = (dim,)
+        self.cond_shape = (cond_dim,) if cond_dim is not None else None
 
-        # Initialise bias terms to match the provided transformer parameters
-        self.autoregressive_mlp = eqx.tree_at(
-            where=lambda t: t.layers[-1].linear.bias,
-            pytree=autoregressive_mlp,
-            replace=jnp.tile(
-                transformer_init_params, dim
-            ),
+        conditioner_output_size = transformer_init_params.size * (
+            dim - untransformed_dim
         )
 
-        self.transformer_constructor = constructor
-        self.shape = (dim,)
-        self.cond_shape = None if cond_dim is None else (cond_dim,)
+        conditioner = eqx.nn.MLP(
+            in_size=untransformed_dim
+            if cond_dim is None
+            else untransformed_dim + cond_dim,
+            out_size=conditioner_output_size,
+            width_size=nn_width,
+            depth=nn_depth,
+            activation=nn_activation,
+            key=key,
+        )  # type: eqx.nn.MLP
+
+        # Initialise last bias terms to match the provided transformer parameters
+        self.conditioner = eqx.tree_at(
+            where=lambda mlp: mlp.layers[-1].bias,  # type: ignore
+            pytree=conditioner,
+            replace=jnp.tile(transformer_init_params, dim - untransformed_dim),
+        )
 
     def transform(self, x, condition=None):
-        nn_input = x if condition is None else jnp.hstack((x, condition))
-        transformer_params = self.autoregressive_mlp(nn_input)
+        x_cond, x_trans = x[: self.untransformed_dim], x[self.untransformed_dim :]
+        nn_input = x_cond if condition is None else jnp.hstack((x_cond, condition))
+        transformer_params = self.conditioner(nn_input)
         transformer = self._flat_params_to_transformer(transformer_params)
-        return transformer.transform(x)
-
-    def transform_and_log_abs_det_jacobian(self, x, condition=None):
-        nn_input = x if condition is None else jnp.hstack((x, condition))
-        transformer_params = self.autoregressive_mlp(nn_input)
+        y_trans = transformer.transform(x_trans)
+        y = jnp.hstack((x_cond, y_trans))
+        return y
+
+    def transform_and_log_det(self, x, condition=None):
+        x_cond, x_trans = x[: self.untransformed_dim], x[self.untransformed_dim :]
+        nn_input = x_cond if condition is None else jnp.hstack((x_cond, condition))
+        transformer_params = self.conditioner(nn_input)
         transformer = self._flat_params_to_transformer(transformer_params)
-        return transformer.transform_and_log_abs_det_jacobian(x)
+        y_trans, log_det = transformer.transform_and_log_det(x_trans)
+        y = jnp.hstack((x_cond, y_trans))
+        return y, log_det
 
     def inverse(self, y, condition=None):
-        init = (y, 0)
-        fn = partial(self.inv_scan_fn, condition=condition)
-        (x, _), _ = jax.lax.scan(fn, init, None, length=len(y))
+        x_cond, y_trans = y[: self.untransformed_dim], y[self.untransformed_dim :]
+        nn_input = x_cond if condition is None else jnp.concatenate((x_cond, condition))
+        transformer_params = self.conditioner(nn_input)
+        transformer = self._flat_params_to_transformer(transformer_params)
+        x_trans = transformer.inverse(y_trans)
+        x = jnp.hstack((x_cond, x_trans))
         return x
 
-    def inv_scan_fn(self, init, _, condition):
-        "One 'step' in computing the inverse"
-        y, rank = init
-        nn_input = y if condition is None else jnp.hstack((y, condition))
-        transformer_params = self.autoregressive_mlp(nn_input)
+    def inverse_and_log_det(self, y, condition=None):
+        x_cond, y_trans = y[: self.untransformed_dim], y[self.untransformed_dim :]
+        nn_input = x_cond if condition is None else jnp.concatenate((x_cond, condition))
+        transformer_params = self.conditioner(nn_input)
         transformer = self._flat_params_to_transformer(transformer_params)
-        x = transformer.inverse(y)
-        x = y.at[rank].set(x[rank])
-        return (x, rank + 1), None
-
-    def inverse_and_log_abs_det_jacobian(self, y, condition=None):
-        x = self.inverse(y, condition)
-        log_det = self.transform_and_log_abs_det_jacobian(x, condition)[1]
-        return x, -log_det
-
-    def _flat_params_to_transformer(
-        self, params: Array
-    ):  # TODO code repetition with MAF
-        "Reshape to dim X params_per_dim, then vmap."
-        dim = self.shape[-1]
+        x_trans, log_det = transformer.inverse_and_log_det(y_trans)
+        x = jnp.hstack((x_cond, x_trans))
+        return x, log_det
+
+    def _flat_params_to_transformer(self, params: Array):
+        """Reshape to dim X params_per_dim, then vmap."""
+        dim = self.dim - self.untransformed_dim
         transformer_params = jnp.reshape(params, (dim, -1))
         transformer = eqx.filter_vmap(self.transformer_constructor)(transformer_params)
-        return Vmap(transformer, (dim,))
+        return Batch(transformer, (dim,), vectorize_bijection=True)
```

### Comparing `flowjax-8.1.0/flowjax/bijections/rational_quadratic_spline.py` & `flowjax-9.0.0/flowjax/bijections/rational_quadratic_spline.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,18 @@
-from functools import partial
-from typing import Tuple
+"""Rational quadratic spline bijections (https://arxiv.org/abs/1906.04032)."""
+
+
+import equinox as eqx
 import jax
 import jax.numpy as jnp
-from flowjax.utils import Array, real_to_increasing_on_interval
-from flowjax.bijections import Bijection
-from flowjax.bijections.jax_transforms import Vmap
-import equinox as eqx
+from jax import Array
+
+from flowjax.bijections.bijection import Bijection
+from flowjax.bijections.jax_transforms import Batch
+from flowjax.utils import real_to_increasing_on_interval
 
 
 class _ScalarRationalQuadraticSpline(Bijection):
     """Scaler RationalQuadraticSpline transformation (https://arxiv.org/abs/1906.04032)."""
 
     knots: int
     interval: float
@@ -38,52 +41,56 @@
         self.unbounded_y_pos = jnp.zeros(knots)
         self.unbounded_derivatives = jnp.full(
             knots + 2, jnp.log(jnp.exp(1 - min_derivative) - 1)
         )
 
     @property
     def x_pos(self):
-        "Get the knot x positions."
+        """Get the knot x positions."""
         x_pos = real_to_increasing_on_interval(
             self.unbounded_x_pos, self.interval, self.softmax_adjust
         )
         return jnp.pad(x_pos, 1, constant_values=(-self.interval, self.interval))
 
     @property
     def y_pos(self):
-        "Get the knot y positions."
+        """Get the knot y positions."""
         y_pos = real_to_increasing_on_interval(
             self.unbounded_y_pos, self.interval, self.softmax_adjust
         )
         return jnp.pad(y_pos, 1, constant_values=(-self.interval, self.interval))
 
     @property
     def derivatives(self):
-        "Get the knot derivitives"
+        """Get the knot derivitives."""
         return jax.nn.softplus(self.unbounded_derivatives) + self.min_derivative
 
     def transform(self, x, condition=None):
+        # Following notation from the paper
+        # pylint: disable=C0103
         x_pos, y_pos, derivatives = self.x_pos, self.y_pos, self.derivatives
         in_bounds = jnp.logical_and(x > -self.interval, x < self.interval)
         x_robust = jnp.where(in_bounds, x, 0)  # To avoid nans
         k = jnp.searchsorted(x_pos, x_robust) - 1  # k is bin number
         xi = (x_robust - x_pos[k]) / (x_pos[k + 1] - x_pos[k])
         sk = (y_pos[k + 1] - y_pos[k]) / (x_pos[k + 1] - x_pos[k])
         dk, dk1, yk, yk1 = derivatives[k], derivatives[k + 1], y_pos[k], y_pos[k + 1]
         num = (yk1 - yk) * (sk * xi**2 + dk * xi * (1 - xi))
         den = sk + (dk1 + dk - 2 * sk) * xi * (1 - xi)
         y = yk + num / den  # eq. 4
         return jnp.where(in_bounds, y, x)
 
-    def transform_and_log_abs_det_jacobian(self, x, condition=None):
+    def transform_and_log_det(self, x, condition=None):
         y = self.transform(x)
         derivative = self.derivative(x)
         return y, jnp.log(derivative).sum()
 
     def inverse(self, y, condition=None):
+        # Following notation from the paper
+        # pylint: disable=C0103
         x_pos, y_pos, derivatives = self.x_pos, self.y_pos, self.derivatives
         in_bounds = jnp.logical_and(y > -self.interval, y < self.interval)
 
         y_robust = jnp.where(in_bounds, y, 0)  # To avoid nans
         k = jnp.searchsorted(y_pos, y_robust) - 1
         xk, xk1, yk, yk1 = x_pos[k], x_pos[k + 1], y_pos[k], y_pos[k + 1]
         sk = (yk1 - yk) / (xk1 - xk)
@@ -94,60 +101,65 @@
         b = (yk1 - yk) * derivatives[k] - y_delta_s_term
         c = -sk * (y_robust - yk)
         sqrt_term = jnp.sqrt(b**2 - 4 * a * c)
         xi = (2 * c) / (-b - sqrt_term)
         x = xi * (xk1 - xk) + xk
         return jnp.where(in_bounds, x, y)
 
-    def inverse_and_log_abs_det_jacobian(self, y, condition=None):
+    def inverse_and_log_det(self, y, condition=None):
         x = self.inverse(y)
         derivative = self.derivative(x)
         return x, -jnp.log(derivative).sum()
 
-    def derivative(self, x):  # eq. 5
+    def derivative(self, x) -> Array:
+        """The derivative dy/dx of the forward transformation."""
+        # Following notation from the paper (eq. 5)
+        # pylint: disable=C0103
         x_pos, y_pos, derivatives = self.x_pos, self.y_pos, self.derivatives
         in_bounds = jnp.logical_and(x > -self.interval, x < self.interval)
         x_robust = jnp.where(in_bounds, x, 0)  # To avoid nans
         k = jnp.searchsorted(x_pos, x_robust) - 1
         xi = (x_robust - x_pos[k]) / (x_pos[k + 1] - x_pos[k])
         sk = (y_pos[k + 1] - y_pos[k]) / (x_pos[k + 1] - x_pos[k])
         dk, dk1 = derivatives[k], derivatives[k + 1]
         num = sk**2 * (dk1 * xi**2 + 2 * sk * xi * (1 - xi) + dk * (1 - xi) ** 2)
         den = (sk + (dk1 + dk - 2 * sk) * xi * (1 - xi)) ** 2
         derivative = num / den
-        return jnp.where(in_bounds, derivative, 1.0)
+        return jnp.where(in_bounds, derivative, 1.0)  # type: ignore
+
 
+class RationalQuadraticSpline(Batch):
+    """Elementwise rational quadratic spline transform (https://arxiv.org/abs/1906.04032),
+    initialised at the identity function.
+    """
 
-class RationalQuadraticSpline(Vmap):
     def __init__(
         self,
         knots: int,
         interval: float,
-        shape: Tuple[int] = (),
+        shape: tuple[int, ...] = (),
         min_derivative: float = 1e-3,
         softmax_adjust: float = 1e-2,
     ) -> None:
-        """Elementwise rational quadratic spline transform (https://arxiv.org/abs/1906.04032),
-        initialised at the identity function.
-
+        """
         Args:
             knots (int): Number of knots.
             interval (float): interval to transform, [-interval, interval].
-            shape (Tuple[int], optional): Shape of transformation. Defaults to ().
-            min_derivative (float, optional): Minimum dervivative. Defaults to 1e-3.
-            softmax_adjust (float, optional): Controls minimum bin width and height by
+            shape (tuple[int, ...]): Shape of transformation. Defaults to ().
+            min_derivative (float): Minimum dervivative. Defaults to 1e-3.
+            softmax_adjust (float): Controls minimum bin width and height by
                 rescaling softmax output, e.g. 0=no adjustment, 1=average softmax output
                 with evenly spaced widths, >1 promotes more evenly spaced widths.
                 See ``real_to_increasing_on_interval``.. Defaults to 1e-2.
         """
 
-        def constructor(dummy):  # Dummy variable to vmap over
+        def constructor():
             return _ScalarRationalQuadraticSpline(
                 knots, interval, min_derivative, softmax_adjust
             )
 
         # Create constructor with appropriate number of batch dimensions
-        for _ in shape:
-            constructor = eqx.filter_vmap(constructor)
+        for dim in reversed(shape):
+            constructor = eqx.filter_vmap(constructor, axis_size=dim)
 
-        spline = constructor(jnp.zeros(shape))
-        super().__init__(spline, shape)
+        spline = constructor()
+        super().__init__(spline, shape, vectorize_bijection=True)
```

### Comparing `flowjax-8.1.0/flowjax/bijections/tanh.py` & `flowjax-9.0.0/flowjax/bijections/tanh.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,37 +1,46 @@
+"""Tanh bijection."""
+import math
+
 import jax
 import jax.numpy as jnp
-import math
-from flowjax.bijections import Bijection
+
+from flowjax.bijections.bijection import Bijection
 
 
 def _tanh_log_grad(x):
-    "log gradient vector of tanh transformation"
+    """log gradient vector of tanh transformation."""
     return -2 * (x + jax.nn.softplus(-2 * x) - jnp.log(2.0))
 
 
 class Tanh(Bijection):
-    """
-    Tanh bijection.
-    """
+    """Tanh bijection."""
 
-    def __init__(self) -> None:
-        self.shape = None
+    def __init__(self, shape: tuple[int, ...] = ()) -> None:
+        """
+        Args:
+            shape (tuple[int, ...] | None): Shape of the bijection. Defaults to None.
+        """
+        self.shape = shape
         self.cond_shape = None
 
     def transform(self, x, condition=None):
+        self._argcheck(x)
         return jnp.tanh(x)
 
-    def transform_and_log_abs_det_jacobian(self, x, condition=None):
+    def transform_and_log_det(self, x, condition=None):
+        self._argcheck(x)
         return jnp.tanh(x), jnp.sum(_tanh_log_grad(x))
 
     def inverse(self, y, condition=None):
+        self._argcheck(y)
         return jnp.arctanh(y)
 
-    def inverse_and_log_abs_det_jacobian(self, y, condition=None):
+    def inverse_and_log_det(self, y, condition=None):
+        self._argcheck(y)
         x = jnp.arctanh(y)
         return x, -jnp.sum(_tanh_log_grad(x))
 
 
 class TanhLinearTails(Bijection):
     """
     Tanh bijection, with linear "tails" beyond +/- max_val. Note due to the linear
@@ -41,46 +50,52 @@
     avoiding issues with numerical instability.
     """
 
     max_val: float
     intercept: float
     linear_grad: float
 
-    def __init__(self, max_val: float):
+    def __init__(self, max_val: float, shape: tuple[int, ...] = ()):
         """Create a tanh bijection with linear "tails" beyond +/- max_val.
 
         Args:
             max_val (int): Value above or below which the function becomes linear.
+            shape (tuple[int, ...] | None): The shape of the bijection. Defaults to
+                None.
         """
         self.max_val = max_val
         self.linear_grad = math.exp(_tanh_log_grad(max_val))
         self.intercept = math.tanh(max_val) - self.linear_grad * max_val
-        self.shape = None
+        self.shape = shape
         self.cond_shape = None
 
     def transform(self, x, condition=None):
+        self._argcheck(x)
         is_linear = jnp.abs(x) >= self.max_val
         linear_y = self.linear_grad * x + jnp.sign(x) * self.intercept
         tanh_y = jnp.tanh(x)
         return jnp.where(is_linear, linear_y, tanh_y)
 
-    def transform_and_log_abs_det_jacobian(self, x, condition=None):
+    def transform_and_log_det(self, x, condition=None):
+        self._argcheck(x)
         y = self.transform(x)
         log_grads = jnp.where(
             jnp.abs(x) >= self.max_val, jnp.log(self.linear_grad), _tanh_log_grad(x)
         )
-        return y, jnp.sum(log_grads)
+        return y, jnp.sum(log_grads)  # type: ignore
 
     def inverse(self, y, condition=None):
+        self._argcheck(y)
         is_linear = jnp.abs(y) >= jnp.tanh(self.max_val)
         x_linear = (y - jnp.sign(y) * self.intercept) / self.linear_grad
         x_arctan = jnp.arctanh(y)
         return jnp.where(is_linear, x_linear, x_arctan)
 
-    def inverse_and_log_abs_det_jacobian(self, y, condition=None):
+    def inverse_and_log_det(self, y, condition=None):
+        self._argcheck(y)
         x = self.inverse(y)
         log_grads = jnp.where(
             jnp.abs(y) >= jnp.tanh(self.max_val),
             jnp.log(self.linear_grad),
             _tanh_log_grad(x),
         )
-        return x, -jnp.sum(log_grads)
+        return x, -jnp.sum(log_grads)  # type: ignore
```

### Comparing `flowjax-8.1.0/flowjax/bijections/utils.py` & `flowjax-9.0.0/flowjax/bijections/utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,180 +1,211 @@
-from typing import Tuple, Union
+"""Utility bijections (embedding network, permutations, inversion etc.)"""
+from typing import Callable
 
-import equinox as eqx
 import jax.numpy as jnp
+from jax import Array
 from jax.experimental import checkify
 
-from flowjax.bijections import Bijection
-from flowjax.utils import Array
+from flowjax.bijections.bijection import Bijection
 
 
 class Invert(Bijection):
+    """Invert a bijection, such that the transform methods become the inverse
+    methods and vice versa. Note that in general, we define bijections such that
+    the forward methods are preffered, i.e. faster/actually implemented. For
+    training flows, we generally want the inverse method (used in density
+    evaluation), to be faster. Hence it is often useful to use this class to
+    achieve this aim.
+    """
+
     bijection: Bijection
 
     def __init__(self, bijection: Bijection):
-        """Invert a bijection, such that the transform methods become the inverse methods and vice versa.
-        Note that in general, we define bijections such that the forward methods are preffered, i.e.
-        faster/actually implemented. For training flows, we generally want the inverse method (used in
-        density evaluation), to be faster. Hence it is often useful to use this class to achieve this aim.
-
+        """
         Args:
-            bijection (Bijection): Bijection to "invert".
+            bijection (Bijection): Bijection to invert.
         """
         self.bijection = bijection
         self.shape = bijection.shape
         self.cond_shape = bijection.cond_shape
 
     def transform(self, x, condition=None):
         return self.bijection.inverse(x, condition)
 
-    def transform_and_log_abs_det_jacobian(self, x, condition=None):
-        return self.bijection.inverse_and_log_abs_det_jacobian(x, condition)
+    def transform_and_log_det(self, x, condition=None):
+        return self.bijection.inverse_and_log_det(x, condition)
 
     def inverse(self, y, condition=None):
         return self.bijection.transform(y, condition)
 
-    def inverse_and_log_abs_det_jacobian(self, y, condition=None):
-        return self.bijection.transform_and_log_abs_det_jacobian(y, condition)
+    def inverse_and_log_det(self, y, condition=None):
+        return self.bijection.transform_and_log_det(y, condition)
 
 
 class Permute(Bijection):
-    permutation: Array
-    inverse_permutation: Array
+    """Permutation transformation."""
 
-    def __init__(self, permutation: Array):
-        """Permutation transformation.
+    permutation: tuple[Array, ...]
+    inverse_permutation: tuple[Array, ...]
 
+    def __init__(self, permutation: Array):
+        """
         Args:
             permutation (Array): An array with shape matching the array to transform,
                 with elements 0-(array.size-1) representing the new order based on the
                 flattened array (uses, C-like ordering).
         """
         checkify.check(
             (permutation.ravel().sort() == jnp.arange(permutation.size)).all(),
             "Invalid permutation array provided.",
         )
         self.shape = permutation.shape
         self.cond_shape = None
 
         indices = jnp.unravel_index(permutation.ravel(), permutation.shape)
         self.permutation = tuple(jnp.reshape(i, permutation.shape) for i in indices)
-        
-        inv_indices = jnp.unravel_index(jnp.argsort(permutation.ravel()), permutation.shape)
-        self.inverse_permutation = tuple(jnp.reshape(i, permutation.shape) for i in inv_indices)
+
+        inv_indices = jnp.unravel_index(
+            jnp.argsort(permutation.ravel()), permutation.shape
+        )
+        self.inverse_permutation = tuple(
+            jnp.reshape(i, permutation.shape) for i in inv_indices
+        )
 
     def transform(self, x, condition=None):
         self._argcheck(x)
         return x[self.permutation]
 
-    def transform_and_log_abs_det_jacobian(self, x, condition=None):
+    def transform_and_log_det(self, x, condition=None):
         return x[self.permutation], jnp.array(0)
 
     def inverse(self, y, condition=None):
         self._argcheck(y)
         return y[self.inverse_permutation]
 
-    def inverse_and_log_abs_det_jacobian(self, y, condition=None):
+    def inverse_and_log_det(self, y, condition=None):
         return y[self.inverse_permutation], jnp.array(0)
 
 
 class Flip(Bijection):
     """Flip the input array. Condition argument is ignored."""
 
-    def __init__(self) -> None:
-        self.shape = None
-        self.cond_shape = None    
+    def __init__(self, shape: tuple[int, ...]) -> None:
+        """
+        Args:
+            shape (tuple[int, ...] | None): The shape of the bijection. Defaults to None.
+        """
+        self.shape = shape
+        self.cond_shape = None
 
     def transform(self, x, condition=None):
+        self._argcheck(x)
         return jnp.flip(x)
 
-    def transform_and_log_abs_det_jacobian(self, x, condition=None):
+    def transform_and_log_det(self, x, condition=None):
+        self._argcheck(x)
         return jnp.flip(x), jnp.array(0)
 
     def inverse(self, y, condition=None):
+        self._argcheck(y)
         return jnp.flip(y)
 
-    def inverse_and_log_abs_det_jacobian(self, y, condition=None):
+    def inverse_and_log_det(self, y, condition=None):
+        self._argcheck(y)
         return jnp.flip(y), jnp.array(0)
 
 
 class Partial(Bijection):
     """Applies bijection to specific indices of an input."""
 
-    bijection: Array
-    idxs: Union[int, slice, Array, tuple]
+    bijection: Bijection
+    idxs: int | slice | Array | tuple
 
-    def __init__(self, bijection: Bijection, idxs):
+    def __init__(self, bijection: Bijection, idxs, shape: tuple[int, ...]):
         """
         Args:
-            bijection (Bijection): Bijection that is compatible with the subset of x indexed by idxs.
-            idxs: Indices (Integer, a slice, or an ndarray with integer/bool dtype) of the transformed portion.
+            bijection (Bijection): Bijection that is compatible with the subset of x
+                indexed by idxs. idxs: Indices (Integer, a slice, or an ndarray with
+                integer/bool dtype) of the transformed portion.
+            shape (tuple[int, ...] | None): Shape of the bijection. Defaults to None.
         """
         self.bijection = bijection
         self.idxs = idxs
-        self.shape = None
+        self.shape = shape
         self.cond_shape = bijection.cond_shape
 
+        if jnp.zeros(shape)[idxs].shape != bijection.shape:
+            raise ValueError(
+                f"The bijection shape is incompatible with the subset of the input "
+                f"indexed by 'idxs'. The bijection has a shape of {bijection.shape}, "
+                f"while the subset has a shape of {jnp.zeros(shape)[idxs].shape}."
+            )
+
     def transform(self, x: Array, condition=None):
+        self._argcheck(x)
         y = self.bijection.transform(x[self.idxs], condition)
         return x.at[self.idxs].set(y)
 
-    def transform_and_log_abs_det_jacobian(self, x: Array, condition=None):
-        y, log_det = self.bijection.transform_and_log_abs_det_jacobian(
-            x[self.idxs], condition
-        )
+    def transform_and_log_det(self, x: Array, condition=None):
+        self._argcheck(x)
+        y, log_det = self.bijection.transform_and_log_det(x[self.idxs], condition)
         return x.at[self.idxs].set(y), log_det
 
-    def inverse(self, y: Array, condition=None) -> Array:
+    def inverse(self, y: Array, condition=None):
+        self._argcheck(y)
         x = self.bijection.inverse(y[self.idxs], condition)
         return y.at[self.idxs].set(x)
 
-    def inverse_and_log_abs_det_jacobian(self, y: Array, condition=None) -> Array:
-        x, log_det = self.bijection.inverse_and_log_abs_det_jacobian(
-            y[self.idxs], condition
-        )
+    def inverse_and_log_det(self, y: Array, condition=None):
+        self._argcheck(y)
+        x, log_det = self.bijection.inverse_and_log_det(y[self.idxs], condition)
         return y.at[self.idxs].set(x), log_det
 
 
 class EmbedCondition(Bijection):
+    """Use an embedding network to reduce the dimensionality of the conditioning variable.
+    The returned bijection has cond_dim equal to the raw condition size.
+    """
+
     bijection: Bijection
-    embedding_net: eqx.Module
+    embedding_net: Callable
 
     def __init__(
         self,
         bijection: Bijection,
-        embedding_net: eqx.Module,
-        raw_cond_shape: Tuple[int],
+        embedding_net: Callable,
+        raw_cond_shape: tuple[int, ...],
     ) -> None:
-        """Use an embedding network to reduce the dimensionality of the conditioning variable.
-        The returned bijection has cond_dim equal to the raw condition size.
-
+        """
         Args:
-            bijection (Bijection): Bijection with ``bijection.cond_dim`` equal to the embedded size.
-            embedding_net (eqx.Module): A callable equinox module that embeds a conditioning variable to size ``bijection.cond_dim``.
-            raw_cond_shape (Union[None, Tuple[int]]): The dimension of the raw conditioning variable.
+            bijection (Bijection): Bijection with ``bijection.cond_dim`` equal to the
+                embedded size.
+            embedding_net (Callable): A callable (e.g. equinox module) that embeds a
+                conditioning variable to size ``bijection.cond_dim``.
+            raw_cond_shape (tuple[int, ...] | None): The dimension of the raw
+                conditioning variable.
         """
         self.bijection = bijection
         self.embedding_net = embedding_net
 
         self.shape = bijection.shape
         self.cond_shape = raw_cond_shape
 
     def transform(self, x, condition=None):
         self._argcheck(x, condition)
         condition = self.embedding_net(condition)
         return self.bijection.transform(x, condition)
 
-    def transform_and_log_abs_det_jacobian(self, x, condition=None):
+    def transform_and_log_det(self, x, condition=None):
         self._argcheck(x, condition)
         condition = self.embedding_net(condition)
-        return self.bijection.transform_and_log_abs_det_jacobian(x, condition)
+        return self.bijection.transform_and_log_det(x, condition)
 
     def inverse(self, y, condition=None):
         self._argcheck(y, condition)
         condition = self.embedding_net(condition)
         return self.bijection.inverse(y, condition)
 
-    def inverse_and_log_abs_det_jacobian(self, y, condition=None):
+    def inverse_and_log_det(self, y, condition=None):
         self._argcheck(y, condition)
         condition = self.embedding_net(condition)
-        return self.bijection.inverse_and_log_abs_det_jacobian(y, condition)
+        return self.bijection.inverse_and_log_det(y, condition)
```

### Comparing `flowjax-8.1.0/flowjax/distributions.py` & `flowjax-9.0.0/flowjax/distributions.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,26 +1,27 @@
-from abc import ABC, abstractmethod
-from typing import Optional, Tuple, Union
-
+"""Distributions - including the base class Distribution, common distributions
+and a Transformed distribution class.
+"""
+from abc import abstractmethod
+from math import prod
 import equinox as eqx
 import jax.numpy as jnp
-
 import jax.random as jr
+from jax import Array
+from jax.experimental import checkify
 from jax.scipy import stats as jstats
+from jax.typing import ArrayLike
 
 from flowjax.bijections import Affine, Bijection
-from flowjax.utils import Array, _get_ufunc_signature
-from math import prod
-from flowjax.utils import merge_shapes
+from flowjax.utils import _get_ufunc_signature, merge_cond_shapes
 
-from jax.experimental import checkify
 
-class Distribution(eqx.Module, ABC):
+class Distribution(eqx.Module):
     """Distribution base class. Distributions all have an attribute ``shape``,
-    denoting the shape of a single sample from the distribution. This corresponds to the 
+    denoting the shape of a single sample from the distribution. This corresponds to the
     ``batch_shape + event_shape`` in torch/numpyro distributions. Similarly, the
     ``cond_shape`` attribute denotes the shape of the conditioning variable.
     This attribute is None for unconditional distributions. For example
 
     .. doctest::
 
         >>> import jax.numpy as jnp
@@ -33,94 +34,99 @@
 
     Distributions are registered as jax PyTrees (as they are equinox modules), and as such
     they are compatible with normal jax operations.
 
     Implementing a distribution
 
         (1) Inherit from ``Distribution``.
-        (2) Define attributes ``shape`` and ``cond_shape`` (cond shape should be None for unconditional distributions).
-        (3) Define the ``_sample`` method, which samples a point with a shape of ``shape``, (given a conditioning variable with shape ``cond_shape`` for conditional distributions).
-        (4) Define the ``_log_prob`` method, which evaluates the log probability, given an input of shape ``shape`` (and a conditioning variable with shape ``cond_shape`` for conditional distributions).
+        (2) Define attributes ``shape`` and ``cond_shape`` (cond shape should be None
+            for unconditional distributions).
+        (3) Define the ``_sample`` method, which samples a point with a shape of
+            ``shape``, (given a conditioning variable with shape ``cond_shape`` for
+            conditional distributions).
+        (4) Define the ``_log_prob`` method, which evaluates the log probability,
+            given an input of shape ``shape`` (and a conditioning variable with shape
+            ``cond_shape`` for conditional distributions).
 
-        The base class will handle defining more convenient log_prob and sample methods that support broadcasting and perform argument checks.
+        The base class will handle defining more convenient log_prob and sample methods
+        that support broadcasting and perform argument checks.
 
     """
 
-    shape: Tuple[int]
-    cond_shape: Union[None, Tuple[int]]
+    shape: tuple[int, ...]
+    cond_shape: tuple[int, ...] | None
 
     @abstractmethod
-    def _log_prob(self, x: Array, condition: Optional[Array] = None):
-        "Evaluate the log probability of point x."
-        pass
+    def _log_prob(self, x: Array, condition: Array | None = None) -> Array:
+        """Evaluate the log probability of point x."""
 
     @abstractmethod
-    def _sample(self, key: jr.KeyArray, condition: Optional[Array] = None):
-        "Sample a point from the distribution."
-        pass
+    def _sample(self, key: jr.KeyArray, condition: Array | None = None) -> Array:
+        """Sample a point from the distribution."""
 
     def _sample_and_log_prob(
-        self,
-        key: jr.PRNGKey,
-        condition: Optional[Array] = None
-        ):
-        """
-        Sample a point from the distribution, and return its log probability.
-        Subclasses can reimplement this method in cases where more efficient methods exists (e.g. see Transformed).
+        self, key: jr.KeyArray, condition: Array | None = None
+    ) -> tuple[Array, Array]:
+        """Sample a point from the distribution, and return its log probability.
+        Subclasses can reimplement this method in cases where more efficient methods
+        exists (e.g. see Transformed).
         """
         x = self._sample(key, condition)
         log_prob = self._log_prob(x, condition)
         return x, log_prob
 
-    def log_prob(self, x: Array, condition: Optional[Array] = None):
+    def log_prob(self, x: Array, condition: Array | None = None) -> Array:
         """Evaluate the log probability. Uses numpy like broadcasting if additional
         leading dimensions are passed.
 
         Args:
             x (Array): Points at which to evaluate density.
-            condition (Optional[Array], optional): Conditioning variables. Defaults to None.
+            condition (Array | None): Conditioning variables. Defaults to None.
 
         Returns:
             Array: Jax array of log probabilities.
         """
         self._argcheck(x, condition)
-        if condition is not None:
-            sig = _get_ufunc_signature([self.shape, self.cond_shape], [()])
-            exclude = {}
-        else:
+        if condition is None:
             sig = _get_ufunc_signature([self.shape], [()])
-            exclude = {1}
+            exclude = frozenset([1])
+        else:
+            sig = _get_ufunc_signature([self.shape, self.cond_shape], [()])
+            exclude = frozenset()
+
         lps = jnp.vectorize(self._log_prob, signature=sig, excluded=exclude)(
             x, condition
         )
-        return jnp.where(jnp.isnan(lps), -jnp.inf, lps)
+        return jnp.where(jnp.isnan(lps), -jnp.inf, lps)  # type: ignore
 
     def sample(
         self,
-        key: jr.PRNGKey,
-        sample_shape: Tuple[int] = (),
-        condition: Optional[Array] = None,
-    ):
+        key: jr.KeyArray,
+        sample_shape: tuple[int, ...] = (),
+        condition: Array | None = None,
+    ) -> Array:
         """Sample from the distribution. For unconditional distributions, the output will
         be of shape ``sample_shape + dist.shape``.
-        
+
         Example:
 
             .. testsetup::
 
                 from flowjax.distributions import StandardNormal
                 import jax.random as jr
                 import jax.numpy as jnp
                 from flowjax.flows import CouplingFlow
                 from flowjax.bijections import Affine
                 # For a unconditional distribution:
                 key = jr.PRNGKey(0)
                 dist = StandardNormal((2,))
                 # For a conditional distribution
-                cond_dist = CouplingFlow(key, StandardNormal((2,)), cond_dim=3, transformer=Affine())
+                cond_dist = CouplingFlow(
+                    key, StandardNormal((2,)), cond_dim=3, transformer=Affine()
+                    )
 
             For an unconditional distribution:
 
             .. doctest::
 
                 >>> dist.shape
                 (2,)
@@ -146,402 +152,425 @@
                 (5, 2)
                 >>> # Sample 10 times for each of 5 conditioning variables
                 >>> samples = cond_dist.sample(key, (10,), condition=jnp.ones((5, 3)))
                 >>> samples.shape
                 (10, 5, 2)
 
         Args:
-            key (jr.PRNGKey): Jax random key.
-            condition (Optional[Array], optional): Conditioning variables. Defaults to None.
-            sample_shape (Tuple[int], optional): Sample shape. Defaults to ().
+            key (jr.KeyArray): Jax random key.
+            condition (Array | None): Conditioning variables. Defaults to None.
+            sample_shape (tuple[int, ...]): Sample shape. Defaults to ().
 
         """
         self._argcheck(condition=condition)
-
-        if condition is None:
-            key_shape = sample_shape
-            excluded = {1}
-            sig = _get_ufunc_signature([(2,)], [self.shape])
-        else:
-            leading_cond_shape = condition.shape[: -len(self.cond_shape)] if self.cond_ndim > 0 else condition.shape
-            key_shape = sample_shape + leading_cond_shape
-            excluded = {}
-            sig = _get_ufunc_signature([(2,), self.cond_shape], [self.shape])
-
-        key_size = max(1, prod(key_shape))  # Still need 1 key for scalar input
-        keys = jnp.reshape(jr.split(key, key_size), key_shape + (2,))
-
-        return jnp.vectorize(self._sample, excluded=excluded, signature=sig)(
+        excluded, signature = self._vectorize_sample_args()
+        keys = self._get_sample_keys(key, sample_shape, condition)
+        return jnp.vectorize(self._sample, excluded=excluded, signature=signature)(
             keys, condition
-        )
-
+        )  # type: ignore
 
     def sample_and_log_prob(
         self,
-        key: jr.PRNGKey,
-        sample_shape: Tuple[int] = (),
-        condition: Optional[Array] = None,
-        ):
+        key: jr.KeyArray,
+        sample_shape: tuple[int, ...] = (),
+        condition: Array | None = None,
+    ):
         """Sample the distribution and return the samples and corresponding log probabilities.
         For transformed distributions (especially flows), this will generally be more efficient
         than calling the methods seperately.
-        
+
         Refer to the :py:meth:`~flowjax.distributions.Distribution.sample` and
         Refer to the :py:meth:`~flowjax.distributions.Distribution.log_prob` documentation
         for more information.
 
         Args:
-            key (jr.PRNGKey): Jax random key.
-            condition (Optional[Array], optional): Conditioning variables. Defaults to None.
-            sample_shape (Tuple[int], optional): Sample shape. Defaults to ().
+            key (jr.KeyArray): Jax random key.
+            condition (Array | None): Conditioning variables. Defaults to None.
+            sample_shape (tuple[int, ...]): Sample shape. Defaults to ().
         """
         self._argcheck(condition=condition)
 
-        if condition is None:
+        excluded, signature = self._vectorize_sample_args(sample_and_log_prob=True)
+        keys = self._get_sample_keys(key, sample_shape, condition)
+
+        return jnp.vectorize(
+            self._sample_and_log_prob, excluded=excluded, signature=signature
+        )(keys, condition)
+
+    def _vectorize_sample_args(self, sample_and_log_prob=False):
+        """Get the excluded arguments and ufunc signature for sample or sample_and_log_prob"""
+        out_shapes = [self.shape, ()] if sample_and_log_prob else [self.shape]
+        if self.cond_shape is None:
+            excluded = frozenset([1])
+            in_shapes = [(2,)]
+        else:
+            excluded = frozenset()
+            in_shapes = [(2,), self.cond_shape]
+        signature = _get_ufunc_signature(in_shapes, out_shapes)
+        return excluded, signature
+
+    def _get_sample_keys(self, key, sample_shape, condition):
+        """Splits a key into an arrray of keys with shape
+        sample_shape + leading_cond_shape + (2,)."""
+        if self.cond_shape is None:
             key_shape = sample_shape
-            excluded = {1}
-            sig = _get_ufunc_signature([(2,)], [self.shape, ()])
         else:
-            leading_cond_shape = condition.shape[: -len(self.cond_shape)] if self.cond_ndim > 0 else condition.shape
+            leading_cond_shape = (
+                condition.shape[: -len(self.cond_shape)]
+                if len(self.cond_shape) > 0
+                else condition.shape
+            )
             key_shape = sample_shape + leading_cond_shape
-            excluded = {}
-            sig = _get_ufunc_signature([(2,), self.cond_shape], [self.shape, ()])
 
-        key_size = max(1, prod(key_shape))  # Still need 1 key for scalar input
-        keys = jnp.reshape(jr.split(key, key_size), key_shape + (2,))
-
-        return jnp.vectorize(self._sample_and_log_prob, excluded=excluded, signature=sig)(
-            keys, condition
-        )
+        key_size = max(1, prod(key_shape))  # Still need 1 key for scalar sample
+        keys = jnp.reshape(jr.split(key, key_size), key_shape + (2,))  # type: ignore
+        return keys
 
     def _argcheck(self, x=None, condition=None):
         # jnp.vectorize would catch ndim mismatches, but it doesn't check axis lengths.
         if x is not None:
             x_trailing = x.shape[-self.ndim :] if self.ndim > 0 else ()
             if x_trailing != self.shape:
                 raise ValueError(
-                    f"Expected trailing dimensions in input x to match the distribution shape, but got "
-                    f"x shape {x.shape}, and distribution shape {self.shape}."
+                    "Expected trailing dimensions in input x to match the distribution "
+                    f"shape, but got x shape {x.shape}, and distribution shape "
+                    f"{self.shape}."
                 )
 
         if condition is None and self.cond_shape is not None:
             raise ValueError(
                 f"Conditioning variable was not provided. "
-                f"Expected conditioning variable with trailing shape {self.shape}."
+                f"Expected conditioning variable with trailing shape {self.cond_shape}."
             )
 
         if condition is not None:
             if self.cond_shape is None:
-                raise ValueError("condition should not be provided for unconditional distribution.")
-            else:
-                condition_trailing = (
-                    condition.shape[-self.cond_ndim :] if self.cond_ndim > 0 else ()
+                raise ValueError(
+                    "condition should not be provided for unconditional distribution."
+                )
+            condition_trailing = (
+                condition.shape[-len(self.cond_shape) :] if self.cond_ndim > 0 else ()  # type: ignore
+            )
+            if condition_trailing != self.cond_shape:
+                raise ValueError(
+                    "Expected trailing dimensions in the condition to match "
+                    "distribution.cond_shape, but got condition shape "
+                    f"{condition.shape}, and distribution.cond_shape {self.cond_shape}."
                 )
-                if condition_trailing != self.cond_shape:
-                    raise ValueError(
-                        f"Expected trailing dimensions in the condition to match distribution.cond_shape, but got "
-                        f"condition shape {condition.shape}, and distribution.cond_shape {self.cond_shape}."
-                    )
 
     @property
     def ndim(self):
+        """The number of dimensions in the distribution (the length of the shape)."""
         return len(self.shape)
 
     @property
     def cond_ndim(self):
-        return len(self.cond_shape)
+        """The number of dimensions of the conditioning variable (length of cond_shape)."""
+        if self.cond_shape is not None:
+            return len(self.cond_shape)
+        return None
 
 
 class Transformed(Distribution):
+    """Form a distribution like object using a base distribution and a
+    bijection. We take the forward bijection for use in sampling, and the inverse
+    bijection for use in density evaluation.
+    """
+
     base_dist: Distribution
     bijection: Bijection
-    cond_shape: Union[None, Tuple[int]]
+    cond_shape: tuple[int, ...] | None
 
     def __init__(
         self,
         base_dist: Distribution,
         bijection: Bijection,
     ):
         """
-        Form a distribution like object using a base distribution and a
-        bijection. We take the forward bijection for use in sampling, and the inverse
-        bijection for use in density evaluation.
-
         Args:
             base_dist (Distribution): Base distribution.
             bijection (Bijection): Bijection to transform distribution.
 
         Example:
 
         .. doctest::
 
             >>> from flowjax.distributions import StandardNormal, Transformed
             >>> from flowjax.bijections import Affine
             >>> normal = StandardNormal()
             >>> bijection = Affine(1)
             >>> transformed = Transformed(normal, bijection)
 
-        
+
         .. warning::
             It is the currently the users responsibility to ensure the bijection is valid
             across the entire support of the distribution. Failure to do so may lead to
             to unexpected results. In future versions explicit constraints may be introduced.
         """
         self.base_dist = base_dist
         self.bijection = bijection
         self.shape = self.base_dist.shape
-        self.cond_shape = merge_shapes(
+        self.cond_shape = merge_cond_shapes(
             (self.bijection.cond_shape, self.base_dist.cond_shape)
         )
 
-    def _log_prob(self, x: Array, condition: Optional[Array] = None):
-        z, log_abs_det = self.bijection.inverse_and_log_abs_det_jacobian(x, condition)
-        p_z = self.base_dist._log_prob(z, condition)
+    def _log_prob(self, x: Array, condition: Array | None = None):
+        z, log_abs_det = self.bijection.inverse_and_log_det(x, condition)
+        p_z = self.base_dist._log_prob(z, condition)  # pylint: disable W0212
         return p_z + log_abs_det
 
-    def _sample(self, key: jr.KeyArray, condition: Optional[Array] = None):
-        z = self.base_dist._sample(key, condition)
-        x = self.bijection.transform(z, condition)
-        return x
+    def _sample(self, key: jr.KeyArray, condition: Array | None = None):
+        base_sample = self.base_dist._sample(key, condition)
+        return self.bijection.transform(base_sample, condition)
 
-    def _sample_and_log_prob(self, key: jr.PRNGKey, condition: Optional[Array] = None):
+    def _sample_and_log_prob(self, key: jr.KeyArray, condition: Array | None = None):
         # We overwrite the naive implementation of calling both methods seperately to
         # avoid computing the inverse transformation.
-        x, log_prob_base = self.base_dist._sample_and_log_prob(key, condition)
-        y, forward_log_dets = self.bijection.transform_and_log_abs_det_jacobian(x, condition)
-        return y, log_prob_base - forward_log_dets
+        base_sample, log_prob_base = self.base_dist._sample_and_log_prob(key, condition)
+        sample, forward_log_dets = self.bijection.transform_and_log_det(
+            base_sample, condition
+        )
+        return sample, log_prob_base - forward_log_dets
 
 
 class StandardNormal(Distribution):
-    def __init__(self, shape: Tuple[int] = ()):
-        """
-        Implements a standard normal distribution, condition is ignored.
+    """Implements a standard normal distribution, condition is ignored."""
 
+    def __init__(self, shape: tuple[int, ...] = ()):
+        """
         Args:
-            shape (Tuple[int]): The shape of the normal distribution. Defaults to ().
+            shape (tuple[int, ...]): The shape of the normal distribution. Defaults to ().
         """
         self.shape = shape
         self.cond_shape = None
 
-    def _log_prob(self, x: Array, condition: Optional[Array] = None):
+    def _log_prob(self, x: Array, condition: Array | None = None):
         return jstats.norm.logpdf(x).sum()
 
-    def _sample(self, key: jr.KeyArray, condition: Optional[Array] = None):
+    def _sample(self, key: jr.KeyArray, condition: Array | None = None):
         return jr.normal(key, self.shape)
 
 
 class Normal(Transformed):
-    """
-    Implements an independent Normal distribution with mean and std for
+    """Implements an independent Normal distribution with mean and std for
     each dimension. `loc` and `scale` should be broadcastable.
     """
 
-    def __init__(self, loc: Array=0, scale: Array=1):
+    bijection: Affine
+
+    def __init__(self, loc: ArrayLike = 0, scale: ArrayLike = 1):
         """
         Args:
             loc (Array): Means. Defaults to 0.
             scale (Array): Standard deviations. Defaults to 1.
         """
-        self.shape = jnp.broadcast_shapes(jnp.shape(loc), jnp.shape(scale))
-        self.cond_shape = None
-        base_dist = StandardNormal(self.shape)
+        shape = jnp.broadcast_shapes(jnp.shape(loc), jnp.shape(scale))
+        base_dist = StandardNormal(shape)
         bijection = Affine(loc=loc, scale=scale)
         super().__init__(base_dist, bijection)
 
     @property
     def loc(self):
+        """Location of the distribution"""
         return self.bijection.loc
 
     @property
     def scale(self):
+        """scale of the distribution"""
         return self.bijection.scale
 
 
 class _StandardUniform(Distribution):
-    """
-    Implements a standard independent Uniform distribution, ie X ~ Uniform([0, 1]^dim).
-    """
+    """Implements a standard independent Uniform distribution, ie X ~ Uniform([0, 1]^dim)."""
 
-    def __init__(self, shape: Tuple[int] = ()):
+    def __init__(self, shape: tuple[int, ...] = ()):
         self.shape = shape
         self.cond_shape = None
 
-    def _log_prob(self, x: Array, condition: Optional[Array] = None):
+    def _log_prob(self, x: Array, condition: Array | None = None):
         return jstats.uniform.logpdf(x).sum()
 
-    def _sample(self, key: jr.KeyArray, condition: Optional[Array] = None):
+    def _sample(self, key: jr.KeyArray, condition: Array | None = None):
         return jr.uniform(key, shape=self.shape)
 
 
-
-
 class Uniform(Transformed):
-    """
-    Implements an independent uniform distribution
-    between min and max for each dimension. `minval` and `maxval` should be broadcastable.
+    """Implements an independent uniform distribution between min and max for each
+    dimension. `minval` and `maxval` should be broadcastable.
     """
 
-    def __init__(self, minval: Array, maxval: Array):
+    bijection: Affine
+
+    def __init__(self, minval: ArrayLike, maxval: ArrayLike):
         """
         Args:
             minval (Array): Minimum values.
             maxval (Array): Maximum values.
         """
-        self.shape = jnp.broadcast_shapes(jnp.shape(minval), jnp.shape(maxval))
-        self.cond_shape = None
-
+        shape = jnp.broadcast_shapes(jnp.shape(minval), jnp.shape(maxval))
+        minval, maxval = jnp.array(minval), jnp.array(maxval)
         checkify.check(
-            jnp.all(maxval >= minval), "Minimums must be less than the maximums."
+            jnp.all(maxval >= minval),
+            "Minimums must be less than the maximums.",
         )
 
-        base_dist = _StandardUniform(self.shape)
+        base_dist = _StandardUniform(shape)
         bijection = Affine(loc=minval, scale=maxval - minval)
         super().__init__(base_dist, bijection)
 
     @property
     def minval(self):
+        """Minimum value of the uniform distribution."""
         return self.bijection.loc
 
     @property
     def maxval(self):
+        """Maximum value of the uniform distribution."""
         return self.bijection.loc + self.bijection.scale
 
 
 class _StandardGumbel(Distribution):
     """Standard gumbel distribution (https://en.wikipedia.org/wiki/Gumbel_distribution)."""
 
-    def __init__(self, shape: Tuple[int] = ()):
+    def __init__(self, shape: tuple[int, ...] = ()):
         self.shape = shape
         self.cond_shape = None
 
-    def _log_prob(self, x: Array, condition: Optional[Array] = None):
+    def _log_prob(self, x: Array, condition: Array | None = None):
         return -(x + jnp.exp(-x)).sum()
 
-    def _sample(self, key: jr.KeyArray, condition: Optional[Array] = None):
+    def _sample(self, key: jr.KeyArray, condition: Array | None = None):
         return jr.gumbel(key, shape=self.shape)
 
 
 class Gumbel(Transformed):
     """Gumbel distribution (https://en.wikipedia.org/wiki/Gumbel_distribution)"""
 
-    def __init__(self, loc: Array=0, scale: Array=1):
+    bijection: Affine
+
+    def __init__(self, loc: ArrayLike = 0, scale: ArrayLike = 1):
         """
         `loc` and `scale` should broadcast to the dimension of the distribution.
 
         Args:
             loc (Array): Location paramter.
-            scale (Array, optional): Scale parameter. Defaults to 1.0.
+            scale (Array): Scale parameter. Defaults to 1.0.
         """
-        self.shape = jnp.broadcast_shapes(jnp.shape(loc), jnp.shape(scale))
-        self.cond_shape = None
-        base_dist = _StandardGumbel(self.shape)
+        shape = jnp.broadcast_shapes(jnp.shape(loc), jnp.shape(scale))
+        base_dist = _StandardGumbel(shape)
         bijection = Affine(loc, scale)
 
         super().__init__(base_dist, bijection)
 
     @property
     def loc(self):
+        """Location of the distribution"""
         return self.bijection.loc
 
     @property
     def scale(self):
+        """Scale of the distribution."""
         return self.bijection.scale
 
 
 class _StandardCauchy(Distribution):
     """
     Implements standard cauchy distribution (loc=0, scale=1)
     Ref: https://en.wikipedia.org/wiki/Cauchy_distribution
     """
 
-    def __init__(self, shape: Tuple[int] = ()):
+    def __init__(self, shape: tuple[int, ...] = ()):
         self.shape = shape
         self.cond_shape = None
 
-    def _log_prob(self, x: Array, condition: Optional[Array] = None):
+    def _log_prob(self, x: Array, condition: Array | None = None):
         return jstats.cauchy.logpdf(x).sum()
 
-    def _sample(self, key: jr.KeyArray, condition: Optional[Array] = None):
+    def _sample(self, key: jr.KeyArray, condition: Array | None = None):
         return jr.cauchy(key, shape=self.shape)
 
 
 class Cauchy(Transformed):
-    """
-    Cauchy distribution (https://en.wikipedia.org/wiki/Cauchy_distribution).
-    """
+    """Cauchy distribution (https://en.wikipedia.org/wiki/Cauchy_distribution)."""
+
+    bijection: Affine
 
-    def __init__(self, loc: Array=0, scale: Array=1):
+    def __init__(self, loc: ArrayLike = 0, scale: ArrayLike = 1):
         """
         `loc` and `scale` should broadcast to the dimension of the distribution.
 
         Args:
             loc (Array): Location paramter.
-            scale (Array, optional): Scale parameter. Defaults to 1.0.
+            scale (Array): Scale parameter. Defaults to 1.0.
         """
-        self.shape = jnp.broadcast_shapes(jnp.shape(loc), jnp.shape(scale))
-        self.cond_shape = None
-        base_dist = _StandardCauchy(self.shape)
+        shape = jnp.broadcast_shapes(jnp.shape(loc), jnp.shape(scale))
+        base_dist = _StandardCauchy(shape)
         bijection = Affine(loc, scale)
         super().__init__(base_dist, bijection)
 
     @property
     def loc(self):
+        """Location of the distribution"""
         return self.bijection.loc
 
     @property
     def scale(self):
+        """scale of the distribution"""
         return self.bijection.scale
 
 
 class _StandardStudentT(Distribution):
-    """
-    Implements student T distribution with specified degrees of freedom.
-    """
+    """Implements student T distribution with specified degrees of freedom."""
 
     log_df: Array
 
     def __init__(self, df: Array):
         self.shape = df.shape
         self.cond_shape = None
         self.log_df = jnp.log(df)
 
-    def _log_prob(self, x: Array, condition: Optional[Array] = None):
+    def _log_prob(self, x: Array, condition: Array | None = None):
         return jstats.t.logpdf(x, df=self.df).sum()
 
-    def _sample(self, key: jr.KeyArray, condition: Optional[Array] = None):
+    def _sample(self, key: jr.KeyArray, condition: Array | None = None):
         return jr.t(key, df=self.df, shape=self.shape)
 
     @property
     def df(self):
+        """The degrees of freedom of the distibution."""
         return jnp.exp(self.log_df)
 
 
 class StudentT(Transformed):
     """Student T distribution (https://en.wikipedia.org/wiki/Student%27s_t-distribution)."""
 
-    def __init__(self, df: Array, loc: Array=0, scale: Array=1):
+    bijection: Affine
+    base_dist: _StandardStudentT
+
+    def __init__(self, df: Array, loc: ArrayLike = 0, scale: ArrayLike = 1):
         """
         `df`, `loc` and `scale` broadcast to the dimension of the distribution.
 
         Args:
             df (Array): The degrees of freedom.
             loc (Array): Location parameter. Defaults to 0.0.
-            scale (Array, optional): Scale parameter. Defaults to 1.0.
+            scale (Array): Scale parameter. Defaults to 1.0.
         """
         df, loc, scale = jnp.broadcast_arrays(df, loc, scale)
-        self.shape = df.shape
-        self.cond_shape = None
         base_dist = _StandardStudentT(df)
         bijection = Affine(loc, scale)
         super().__init__(base_dist, bijection)
 
     @property
     def loc(self):
+        """Location of the distribution"""
         return self.bijection.loc
 
     @property
     def scale(self):
+        """scale of the distribution"""
         return self.bijection.scale
 
     @property
     def df(self):
+        """The degrees of freedom of the distribution."""
         return self.base_dist.df
```

### Comparing `flowjax-8.1.0/flowjax/flows.py` & `flowjax-9.0.0/flowjax/flows.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,147 +1,147 @@
-"""
-Premade versions of common flow architetctures from ``flowjax.flows``.
-"""
+"""Premade versions of common flow architetctures from ``flowjax.flows``."""
 # Note that here although we could chain arbitrary bijections using `Chain`, here,
 # we generally opt to use `Scan`, which avoids excessive compilation
 # when the flow layers share the same structure.
 
-from typing import Callable, Optional
+from typing import Callable
 
 import equinox as eqx
 import jax.nn as jnn
 import jax.numpy as jnp
 from jax import random
 from jax.nn.initializers import glorot_uniform
 from jax.random import KeyArray
 
 from flowjax.bijections import (
     AdditiveLinearCondition,
+    Bijection,
     BlockAutoregressiveNetwork,
     Chain,
     Coupling,
     Flip,
     Invert,
     MaskedAutoregressive,
     Permute,
+    RationalQuadraticSpline,
     Scan,
     TanhLinearTails,
     TriangularAffine,
-    RationalQuadraticSpline,
-    Bijection,
 )
 from flowjax.distributions import Distribution, Transformed
 
 
-class CouplingFlow(
-    Transformed
-):  # TODO allow flows to work on higher dimensional inputs?
+class CouplingFlow(Transformed):
+    """Coupling flow (https://arxiv.org/abs/1605.08803)."""
+
     flow_layers: int
     nn_width: int
     nn_depth: int
     permute_strategy: str
 
     def __init__(
         self,
         key: KeyArray,
         base_dist: Distribution,
         transformer: Bijection,
-        cond_dim: int = None,
+        cond_dim: int | None = None,
         flow_layers: int = 8,
         nn_width: int = 40,
         nn_depth: int = 2,
         nn_activation: Callable = jnn.relu,
         invert: bool = True,
     ):
-        """Coupling flow (https://arxiv.org/abs/1605.08803).
-
+        """
         Args:
             key (KeyArray): Jax PRNGKey.
             base_dist (Distribution): Base distribution.
             transformer (Bijection): Bijection to be parameterised by conditioner.
-            cond_dim (int, optional): Dimension of conditioning variables. Defaults to None.
-            flow_layers (int, optional): Number of coupling layers. Defaults to 5.
-            nn_width (int, optional): Conditioner hidden layer size. Defaults to 40.
-            nn_depth (int, optional): Conditioner depth. Defaults to 2.
-            nn_activation (int, optional): Conditioner activation function. Defaults to jnn.relu.
-            invert: (bool, optional): Whether to invert the bijection. Broadly, True will prioritise a faster `inverse` methods, leading to faster `log_prob`, False will prioritise faster `transform` methods, leading to faster `sample`. Defaults to True
+            cond_dim (int): Dimension of conditioning variables. Defaults to None.
+            flow_layers (int): Number of coupling layers. Defaults to 5.
+            nn_width (int): Conditioner hidden layer size. Defaults to 40.
+            nn_depth (int): Conditioner depth. Defaults to 2.
+            nn_activation (int): Conditioner activation function. Defaults to jnn.relu.
+            invert: (bool): Whether to invert the bijection. Broadly, True will
+                prioritise a faster `inverse` methods, leading to faster `log_prob`,
+                False will prioritise faster `transform` methods, leading to faster
+                `sample`. Defaults to True
         """
         if base_dist.ndim != 1:
             raise ValueError(f"Expected base_dist.ndim==1, got {base_dist.ndim}")
 
         dim = base_dist.shape[0]
         permute_strategy = _default_permute_strategy(dim)
 
         def make_layer(key):  # coupling layer + permutation
             c_key, p_key = random.split(key)
             coupling = Coupling(
                 key=c_key,
                 transformer=transformer,
-                d=dim // 2,
-                D=dim,
+                untransformed_dim=dim // 2,
+                dim=dim,
                 cond_dim=cond_dim,
                 nn_width=nn_width,
                 nn_depth=nn_depth,
                 nn_activation=nn_activation,
             )
 
             if permute_strategy == "flip":
-                return Chain([coupling, Flip()])
-            elif permute_strategy == "random":
+                return Chain([coupling, Flip((dim,))])
+            if permute_strategy == "random":
                 perm = Permute(random.permutation(p_key, jnp.arange(dim)))
                 return Chain([coupling, perm])
-            else:
-                return coupling
+            return coupling
 
         keys = random.split(key, flow_layers)
         layers = eqx.filter_vmap(make_layer)(keys)
-        bijection = Scan(layers)
-        bijection = Invert(bijection) if invert else bijection
+        bijection = Invert(Scan(layers)) if invert else Scan(layers)
 
         self.nn_width = nn_width
         self.nn_depth = nn_depth
         self.flow_layers = flow_layers
         self.permute_strategy = permute_strategy
         self.shape = (dim,)
         self.cond_shape = None if cond_dim is None else (cond_dim,)
         super().__init__(base_dist, bijection)
 
 
 class MaskedAutoregressiveFlow(Transformed):
+    """Masked autoregressive flow (https://arxiv.org/abs/1606.04934,
+    https://arxiv.org/abs/1705.07057v4). Parameterises a transformer with an
+    autoregressive neural network.
+    """
+
     flow_layers: int
     nn_width: int
     nn_depth: int
     permute_strategy: str
 
     def __init__(
         self,
         key: KeyArray,
         base_dist: Distribution,
         transformer: Bijection,
-        cond_dim: int = None,
+        cond_dim: int | None = None,
         flow_layers: int = 8,
         nn_width: int = 40,
         nn_depth: int = 2,
         nn_activation: Callable = jnn.relu,
         invert: bool = True,
     ):
-        """Masked autoregressive flow (https://arxiv.org/abs/1606.04934,
-        https://arxiv.org/abs/1705.07057v4). Parameterises a transformer with an
-        autoregressive neural network.
-
+        """
         Args:
             key (KeyArray): Random seed.
             base_dist (Distribution): Base distribution.
             transformer (Bijection): Bijection parameterised by autoregressive network.
-            cond_dim (int, optional): _description_. Defaults to 0.
-            flow_layers (int, optional): Number of flow layers. Defaults to 5.
-            nn_width (int, optional): Number of hidden layers in neural network. Defaults to 40.
-            nn_depth (int, optional): Depth of neural network. Defaults to 2.
-            nn_activation (Callable, optional): _description_. Defaults to jnn.relu.
-            invert (bool, optional): Whether to invert the bijection. Broadly, True will
+            cond_dim (int): _description_. Defaults to 0.
+            flow_layers (int): Number of flow layers. Defaults to 5.
+            nn_width (int): Number of hidden layers in neural network. Defaults to 40.
+            nn_depth (int): Depth of neural network. Defaults to 2.
+            nn_activation (Callable): _description_. Defaults to jnn.relu.
+            invert (bool): Whether to invert the bijection. Broadly, True will
                 prioritise a faster inverse, leading to faster `log_prob`, False will prioritise
                 faster forward, leading to faster `sample`. Defaults to True. Defaults to True.
         """
         if len(base_dist.shape) != 1:
             raise ValueError(f"Expected base_dist.ndim==1, got {base_dist.ndim}")
 
         dim = base_dist.shape[0]
@@ -155,61 +155,64 @@
                 dim=dim,
                 cond_dim=cond_dim,
                 nn_width=nn_width,
                 nn_depth=nn_depth,
                 nn_activation=nn_activation,
             )
             if permute_strategy == "flip":
-                return Chain([masked_autoregressive, Flip()])
-            elif permute_strategy == "random":
+                return Chain([masked_autoregressive, Flip((dim,))])
+            if permute_strategy == "random":
                 perm = Permute(random.permutation(p_key, jnp.arange(dim)))
                 return Chain([masked_autoregressive, perm])
-            else:
-                return masked_autoregressive
+            return masked_autoregressive
 
         keys = random.split(key, flow_layers)
         layers = eqx.filter_vmap(make_layer)(keys)
-        bijection = Scan(layers)
-        bijection = Invert(bijection) if invert else bijection
+        bijection = Invert(Scan(layers)) if invert else Scan(layers)
 
         self.nn_width = nn_width
         self.nn_depth = nn_depth
         self.flow_layers = flow_layers
         self.permute_strategy = permute_strategy
         self.shape = (dim,)
         self.cond_shape = None if cond_dim is None else (cond_dim,)
         super().__init__(base_dist, bijection)
 
 
 class BlockNeuralAutoregressiveFlow(Transformed):
+    """Block neural autoregressive flow (BNAF) (https://arxiv.org/abs/1904.04676)."""
+
     flow_layers: int
     nn_block_dim: int
     nn_depth: int
     permute_strategy: str
 
     def __init__(
         self,
         key: KeyArray,
         base_dist: Distribution,
-        cond_dim: Optional[int] = None,
+        cond_dim: int | None = None,
         nn_depth: int = 1,
         nn_block_dim: int = 8,
         flow_layers: int = 1,
         invert: bool = True,
     ):
-        """Block neural autoregressive flow (BNAF) (https://arxiv.org/abs/1904.04676).
-
+        """
         Args:
             key (KeyArray): Jax PRNGKey.
             base_dist (Distribution): Base distribution.
-            cond_dim (Union[None, Tuple[int]]): Dimension of conditional variables.
-            nn_depth (int, optional): Number of hidden layers within the networks. Defaults to 1.
-            nn_block_dim (int, optional): Block size. Hidden layer width is dim*nn_block_dim. Defaults to 8.
-            flow_layers (int, optional): Number of BNAF layers. Defaults to 1.
-            invert: (bool, optional): Use `True` for access of `log_prob` only (e.g. fitting by maximum likelihood), `False` for the forward direction (sampling) only (e.g. for fitting variationally).
+            cond_dim (int | None): Dimension of conditional variables.
+            nn_depth (int): Number of hidden layers within the networks.
+                Defaults to 1.
+            nn_block_dim (int): Block size. Hidden layer width is
+                dim*nn_block_dim. Defaults to 8.
+            flow_layers (int): Number of BNAF layers. Defaults to 1.
+            invert: (bool): Use `True` for access of `log_prob` only (e.g.
+                fitting by maximum likelihood), `False` for the forward direction
+                (sampling) only (e.g. for fitting variationally).
         """
         if len(base_dist.shape) != 1:
             raise ValueError(f"Expected base_dist.ndim==1, got {base_dist.ndim}")
 
         dim = base_dist.shape[-1]
         permute_strategy = _default_permute_strategy(base_dist.shape[0])
 
@@ -219,103 +222,119 @@
                 key=ban_key,
                 dim=dim,
                 cond_dim=cond_dim,
                 depth=nn_depth,
                 block_dim=nn_block_dim,
             )
             if permute_strategy == "flip":
-                return Chain([ban, Flip()])
-            elif permute_strategy == "random":
+                return Chain([ban, Flip((dim,))])
+            if permute_strategy == "random":
                 perm = Permute(random.permutation(p_key, jnp.arange(dim)))
                 return Chain([ban, perm])
-            else:
-                return ban
+            return ban
 
         keys = random.split(key, flow_layers)
         layers = eqx.filter_vmap(make_layer)(keys)
-        bijection = Scan(layers)
-        bijection = Invert(bijection) if invert else bijection
+        bijection = Invert(Scan(layers)) if invert else Scan(layers)
 
         self.nn_block_dim = nn_block_dim
         self.nn_depth = nn_depth
         self.flow_layers = flow_layers
         self.permute_strategy = permute_strategy
 
         self.shape = (dim,)
         self.cond_shape = None if cond_dim is None else (cond_dim,)
         super().__init__(base_dist, bijection)
 
 
 class TriangularSplineFlow(Transformed):
+    """A stack of layers, where each layer consists of a triangular affine
+    transformation with weight normalisation, and an elementwise rational quadratic
+    spline. Tanh is used to constrain to the input to [-1, 1] before spline
+    transformations.
+    """
+
     flow_layers: int
     permute_strategy: str
     knots: int
     tanh_max_val: float
 
     def __init__(
         self,
         key: KeyArray,
         base_dist: Distribution,
-        cond_dim: Optional[int] = None,
+        cond_dim: int | None = None,
         flow_layers: int = 8,
         knots: int = 8,
         tanh_max_val: float = 3.0,
         invert: bool = True,
-        permute_strategy: Optional[str] = None,
         init: Callable = glorot_uniform(),
     ):
-
+        """
+        Args:
+            key (KeyArray): Jax random seed.
+            base_dist (Distribution): Base distribution of the flow.
+            cond_dim (int | None): The number of conditioning features.
+                Defaults to None.
+            flow_layers (int): Number of flow layers. Defaults to 8.
+            knots (int): Number of knots in the splines. Defaults to 8.
+            tanh_max_val (float): Maximum absolute value beyond which we use linear
+                "tails" in the tanh function. Defaults to 3.0.
+            invert: (bool): Use `True` for access of `log_prob` only (e.g.
+                fitting by maximum likelihood), `False` for the forward direction
+                (sampling) only (e.g. for fitting variationally).
+            init (Callable): Initialisation method for the lower triangular weights.
+                Defaults to glorot_uniform().
+        """
         if len(base_dist.shape) != 1:
             raise ValueError(f"Expected base_dist.ndim==1, got {base_dist.ndim}")
 
         dim = base_dist.shape[-1]
-
         permute_strategy = _default_permute_strategy(dim)
 
         def make_layer(key):
-
             lt_key, perm_key = random.split(key)
             c_dim = 0 if cond_dim is None else cond_dim
             weights = init(lt_key, (dim, dim + c_dim))
             lt_weights = weights[:, :dim].at[jnp.diag_indices(dim)].set(1)
             cond_weights = weights[:, dim:]
-            lt = TriangularAffine(jnp.zeros(dim), lt_weights, weight_normalisation=True)
+            lower_tri = TriangularAffine(
+                jnp.zeros(dim), lt_weights, weight_normalisation=True
+            )
 
             bijections = [
-                TanhLinearTails(tanh_max_val),
+                TanhLinearTails(tanh_max_val, (dim,)),
                 RationalQuadraticSpline(knots, interval=1, shape=(dim,)),
-                Invert(TanhLinearTails(tanh_max_val)),
-                lt,
+                Invert(TanhLinearTails(tanh_max_val, (dim,))),
+                lower_tri,
             ]
 
             if cond_dim is not None:
                 linear_condition = AdditiveLinearCondition(cond_weights)
                 bijections.append(linear_condition)
 
             if permute_strategy == "flip":
-                bijections.append(Flip())
+                bijections.append(Flip((dim,)))
             elif permute_strategy == "random":
                 bijections.append(
                     Permute(random.permutation(perm_key, jnp.arange(dim)))
                 )
             return Chain(bijections)
 
         keys = random.split(key, flow_layers)
         layers = eqx.filter_vmap(make_layer)(keys)
-        bijection = Scan(layers)
-        bijection = Invert(bijection) if invert else bijection
+        bijection = Invert(Scan(layers)) if invert else Scan(layers)
 
         self.flow_layers = flow_layers
         self.permute_strategy = permute_strategy
         self.knots = knots
         self.tanh_max_val = tanh_max_val
         self.shape = (dim,)
         self.cond_shape = None if cond_dim is None else (cond_dim,)
 
         super().__init__(base_dist, bijection)
 
 
 def _default_permute_strategy(dim):
     if dim <= 2:
         return {1: "none", 2: "flip"}[dim]
-    else:
-        return "random"
+    return "random"
```

### Comparing `flowjax-8.1.0/flowjax/masks.py` & `flowjax-9.0.0/flowjax/masks.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,44 +1,42 @@
 """
 Various masks, generally used in flows to enforce e.g. a dependency structure
 that leads to invertibility and efficient Jacobian determinant calculations.
 """
 
 import jax.numpy as jnp
+from jax import Array
 from jax.scipy.linalg import block_diag
 
-from flowjax.utils import Array
-
 
 def rank_based_mask(in_ranks: Array, out_ranks: Array, eq: bool = False):
     """Forms mask matrix, with 1s where the out_ranks > or >= in_ranks.
 
     Args:
         in_ranks (Array): Ranks of the inputs.
         out_ranks (Array): Ranks of the outputs.
         eq (bool): If true, compares with >= instead of >. Defaults to False.
 
     Returns:
         Array: Mask with shape `(len(out_ranks), len(in_ranks))`
     """
-
     assert (in_ranks.ndim) == 1 and (out_ranks.ndim == 1)
     if eq:
         mask = out_ranks[:, None] >= in_ranks
     else:
         mask = out_ranks[:, None] > in_ranks
     return mask.astype(jnp.int32)
 
 
 def block_diag_mask(block_shape: tuple, n_blocks: int):
-    "Block diagonal mask."
+    """Block diagonal mask."""
     return block_diag(*jnp.ones((n_blocks, *block_shape), jnp.int32))
 
 
 def block_tril_mask(block_shape: tuple, n_blocks: int):
-    "Upper triangular block mask, excluding diagonal blocks."
+    """Upper triangular block mask, excluding diagonal blocks."""
     mask = jnp.zeros((block_shape[0] * n_blocks, block_shape[1] * n_blocks), jnp.int32)
     for i in range(n_blocks):
         mask = mask.at[
             (i + 1) * block_shape[0] :, i * block_shape[1] : (i + 1) * block_shape[1]
         ].set(1)
     return mask
```

### Comparing `flowjax-8.1.0/flowjax/nn/block_autoregressive.py` & `flowjax-9.0.0/flowjax/nn/block_autoregressive.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,56 +1,60 @@
-from typing import Callable, Optional
+"""Block autoregressive neural network components."""
+from typing import Callable
 
 import equinox as eqx
+import jax
 import jax.numpy as jnp
-from jax import random
+from jax import Array, random
 from jax.nn.initializers import glorot_uniform
 from jax.random import KeyArray
-
+from flowjax.bijections.tanh import Tanh
 from flowjax.masks import block_diag_mask, block_tril_mask
-from flowjax.utils import Array
-import jax
 
 
 def _tanh_log_grad(x):
-    "log gradient vector of tanh transformation"
+    """log gradient vector of tanh transformation."""
     return -2 * (x + jax.nn.softplus(-2 * x) - jnp.log(2.0))
 
 
 class BlockAutoregressiveLinear(eqx.Module):
+    """Block autoregressive neural network layer (https://arxiv.org/abs/1904.04676).
+    Conditioning variables are incorporated by appending columns (one for each
+    conditioning variable) to the left of the block diagonal weight matrix.
+    """
+
     n_blocks: int
     block_shape: tuple
-    cond_dim: Optional[int]
-    W: Array
+    cond_dim: int | None
+    weights: Array
     bias: Array
-    W_log_scale: Array
+    weight_log_scale: Array
     in_features: int
     out_features: int
     b_diag_mask: Array
     b_diag_mask_idxs: Array
     b_tril_mask: Array
 
     def __init__(
         self,
         key: KeyArray,
         n_blocks: int,
         block_shape: tuple,
-        cond_dim: Optional[int] = None,
+        cond_dim: int | None = None,
         init: Callable = glorot_uniform(),
     ):
-        """Block autoregressive neural network layer (https://arxiv.org/abs/1904.04676).
-        Conditioning variables are incorporated by appending columns (one for each
-        conditioning variable) to the left of the block diagonal weight matrix.
-
+        """
         Args:
             key KeyArray: Random key
             n_blocks (int): Number of diagonal blocks (dimension of original input).
-            block_shape (Tuple): The shape of the (unconstrained) blocks.
-            cond_dim (Union[None, int]): Number of additional conditioning variables. Defaults to None.
-            init (Callable, optional): Default initialisation method for the weight matrix. Defaults to ``glorot_uniform()``.
+            block_shape (tuple): The shape of the (unconstrained) blocks.
+            cond_dim (int | None): Number of additional conditioning variables.
+                Defaults to None.
+            init (Callable): Default initialisation method for the weight
+                matrix. Defaults to ``glorot_uniform()``.
         """
         self.cond_dim = cond_dim
 
         if cond_dim is None:
             cond_dim = 0
 
         cond_size = (block_shape[0] * n_blocks, cond_dim)
@@ -61,70 +65,73 @@
 
         self.b_tril_mask = jnp.column_stack(
             (block_tril_mask(block_shape, n_blocks), jnp.ones(cond_size, jnp.int32))
         )
 
         self.b_diag_mask_idxs = jnp.where(
             self.b_diag_mask, size=block_shape[0] * block_shape[1] * n_blocks
-        )
+        )  # type: ignore
 
         in_features, out_features = (
             block_shape[1] * n_blocks + cond_dim,
             block_shape[0] * n_blocks,
         )
 
         *w_key, bias_key, scale_key = random.split(key, n_blocks + 2)
 
-        self.W = init(w_key[0], (out_features, in_features)) * (
+        self.weights = init(w_key[0], (out_features, in_features)) * (
             self.b_tril_mask + self.b_diag_mask
         )
         self.bias = (random.uniform(bias_key, (out_features,)) - 0.5) * (
             2 / jnp.sqrt(out_features)
         )
 
         self.n_blocks = n_blocks
         self.block_shape = block_shape
         self.cond_dim = cond_dim
-        self.W_log_scale = jnp.log(random.uniform(scale_key, (out_features, 1)))
+        self.weight_log_scale = jnp.log(random.uniform(scale_key, (out_features, 1)))
         self.in_features = in_features
         self.out_features = out_features
 
     def get_normalised_weights(self):
-        "Carries out weight normalisation."
-        W = jnp.exp(self.W) * self.b_diag_mask + self.W * self.b_tril_mask
-        W_norms = jnp.linalg.norm(W, axis=-1, keepdims=True)
-        return jnp.exp(self.W_log_scale) * W / W_norms
+        """Carries out weight normalisation."""
+        weights = (
+            jnp.exp(self.weights) * self.b_diag_mask + self.weights * self.b_tril_mask
+        )
+        weight_norms = jnp.linalg.norm(weights, axis=-1, keepdims=True)
+        return jnp.exp(self.weight_log_scale) * weights / weight_norms
 
     def __call__(self, x, condition=None):
-        "returns output y, and components of weight matrix needed log_det component (n_blocks, block_shape[0], block_shape[1])"
-        W = self.get_normalised_weights()
+        """returns output y, and components of weight matrix needed log_det component
+        (n_blocks, block_shape[0], block_shape[1]).
+        """
+        weights = self.get_normalised_weights()
         if condition is not None:
             x = jnp.concatenate((x, condition))
-        y = W @ x + self.bias
-        jac_3d = W[self.b_diag_mask_idxs].reshape(self.n_blocks, *self.block_shape)
+        y = weights @ x + self.bias
+        jac_3d = weights[self.b_diag_mask_idxs].reshape(
+            self.n_blocks, *self.block_shape
+        )
         return y, jnp.log(jac_3d)
 
 
-class BlockTanh:
+def _block_tanh_activation(n_blocks: int):
+    """Returms a Tanh activation compatible with a block neural autoregressive network,
+    i.e. returning the transformed variable and the absolute log gradients as a 3D
+    array with shape (n_blocks,) + block_shape
     """
-    Tanh transformation compatible with block neural autoregressive flow (log_abs_det provided as 3D array).
-    """
-
-    def __init__(self, n_blocks: int):
-        self.n_blocks = n_blocks
-
-    def __call__(self, x, condition=None):
-        """Applies the activation and computes the Jacobian. Jacobian shape is
-        (n_blocks, *block_size). Condition is ignored.
 
-        Returns:
-            Tuple: output, jacobian
-        """
-        log_det = _tanh_log_grad(x)
-        return jnp.tanh(x), _3d_log_det(log_det, self.n_blocks)
+    def activation(x: Array):
+        tanh = Tanh()
+        y, log_jacobian = jax.vmap(tanh.transform_and_log_det)(x)
+        return y, _reshape_jacobian_to_3d(log_jacobian, n_blocks)
+
+    return activation
 
 
-def _3d_log_det(vals, n_blocks):
-    d = vals.shape[0] // n_blocks
-    log_det = jnp.full((n_blocks, d, d), -jnp.inf)
-    log_det = log_det.at[:, jnp.arange(d), jnp.arange(d)].set(vals.reshape(n_blocks, d))
+def _reshape_jacobian_to_3d(vals, n_blocks):
+    block_dim = vals.shape[0] // n_blocks
+    log_det = jnp.full((n_blocks, block_dim, block_dim), -jnp.inf)
+    log_det = log_det.at[:, jnp.arange(block_dim), jnp.arange(block_dim)].set(
+        vals.reshape(n_blocks, block_dim)
+    )
     return log_det
```

### Comparing `flowjax-8.1.0/flowjax/nn/masked_autoregressive.py` & `flowjax-9.0.0/flowjax/nn/masked_autoregressive.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,79 +1,89 @@
-from typing import Callable, List
+"""Autoregressive linear layers and multilayer perceptron."""
+from typing import Callable
 
 import jax.nn as jnn
-import jax.numpy as jnp
 from equinox import Module
 from equinox.nn import Linear
-from jax import random
+from jax import Array, random
 from jax.random import KeyArray
 
 from flowjax.masks import rank_based_mask
-from flowjax.utils import Array, _identity
+
+
+def _identity(x):
+    return x
 
 
 class MaskedLinear(Module):
+    """Masked linear neural network layer."""
+
     linear: Linear
     mask: Array
 
     def __init__(self, mask: Array, use_bias: bool = True, *, key: KeyArray):
         """
-        Masked linear layer.
 
         Args:
             mask (Array): Mask with shape (out_features, in_features).
             key (KeyArray): Jax PRNGKey
-            use_bias (bool, optional): Whether to include bias terms. Defaults to True.
+            use_bias (bool): Whether to include bias terms. Defaults to True.
         """
         self.linear = Linear(mask.shape[1], mask.shape[0], use_bias, key=key)
         self.mask = mask
 
     def __call__(self, x: Array):
+        """Run the masked linear layer
+
+        Args:
+            x (Array): Array with shape ``(mask.shape[1], )``
+        """
         x = self.linear.weight * self.mask @ x
         if self.linear.bias is not None:
             x = x + self.linear.bias
         return x
 
 
 class AutoregressiveMLP(Module):
+    """An autoregressive multilayer perceptron, similar to ``equinox.nn.composed.MLP``.
+    Connections will only exist where in_ranks < out_ranks.
+    """
+
     in_size: int
     out_size: int
     width_size: int
     depth: int
     in_ranks: Array
     out_ranks: Array
     hidden_ranks: Array
-    layers: List[MaskedLinear]
+    layers: list[MaskedLinear]
     activation: Callable
     final_activation: Callable
 
     def __init__(
         self,
         in_ranks: Array,
         hidden_ranks: Array,
         out_ranks: Array,
         depth: int,
         activation: Callable = jnn.relu,
         final_activation: Callable = _identity,
         *,
         key
     ) -> None:
-        """An autoregressive multilayer perceptron, similar to ``equinox.nn.composed.MLP``.
-        Connections will only exist where in_ranks < out_ranks.
-
+        """
         Args:
             in_ranks (Array): Ranks of the inputs.
             hidden_ranks (Array): Ranks of the hidden layer(s).
             out_ranks (Array): Ranks of the outputs.
             depth (int): Number of hidden layers.
-            activation (Callable, optional): Activation function. Defaults to jnn.relu.
-            final_activation (Callable, optional): Final activation function. Defaults to _identity.
-            key (KeyArray): Jax PRNGKey
+            activation (Callable): Activation function. Defaults to jnn.relu.
+            final_activation (Callable): Final activation function. Defaults to _identity.
+            key (KeyArray): Jax PRNGKey.
         """
-
         masks = []
         if depth == 0:
             masks.append(rank_based_mask(in_ranks, out_ranks, eq=False))
         else:
             masks.append(rank_based_mask(in_ranks, hidden_ranks, eq=True))
             for _ in range(depth - 1):
                 masks.append(rank_based_mask(hidden_ranks, hidden_ranks, eq=True))
```

### Comparing `flowjax-8.1.0/flowjax/train/data_fit.py` & `flowjax-9.0.0/flowjax/train/data_fit.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,120 +1,135 @@
-from typing import Dict, List, Optional
-
+"""Function to fit flows to samples from a distribution."""
+from typing import Any, Callable, Dict
 import equinox as eqx
 import jax.numpy as jnp
+import jax.random as jr
 import optax
-from equinox.custom_types import BoolAxisSpec
-from jax import random
-from jax.random import KeyArray
-from jaxtyping import PyTree
+from jax.typing import ArrayLike
 from tqdm import tqdm
-import optax
 
 from flowjax.distributions import Distribution
-from flowjax.utils import Array
+from flowjax.train.train_utils import count_fruitless, train_val_split
+
+PyTree = Any
 
-from flowjax.train.train_utils import train_val_split, count_fruitless
 
 def fit_to_data(
-    key: KeyArray,
+    key: jr.KeyArray,
     dist: Distribution,
-    x: Array,
-    condition: Optional[Array] = None,
+    x: ArrayLike,
+    condition: ArrayLike | None = None,
     max_epochs: int = 50,
     max_patience: int = 5,
     batch_size: int = 256,
     val_prop: float = 0.1,
     learning_rate: float = 5e-4,
     clip_norm: float = 0.5,
-    optimizer: Optional[optax.GradientTransformation] = None,
-    filter_spec: PyTree[BoolAxisSpec] = eqx.is_inexact_array,
+    optimizer: optax.GradientTransformation | None = None,
+    filter_spec: Callable | PyTree = eqx.is_inexact_array,
     show_progress: bool = True,
 ):
-    """Train a distribution (e.g. a flow) to samples by maximum likelihood. Note that the last batch in each epoch is dropped if truncated.
+    """Train a distribution (e.g. a flow) to samples by maximum likelihood. Note that
+        the last batch in each epoch is dropped if truncated.
 
     Args:
         key (KeyArray): Jax PRNGKey.
         dist (Distribution): Distribution object.
         x (Array): Samples from target distribution.
-        condition (Optional[Array], optional): Conditioning variables. Defaults to None.
-        max_epochs (int, optional): Maximum number of epochs. Defaults to 50.
-        max_patience (int, optional): Number of consecutive epochs with no validation loss improvement after which training is terminated. Defaults to 5.
-        batch_size (int, optional): Batch size. Defaults to 256.
-        val_prop (float, optional): Proportion of data to use in validation set. Defaults to 0.1.
-        learning_rate (float, optional): Adam learning rate. Defaults to 5e-4.
-        clip_norm (float, optional): Maximum gradient norm before clipping occurs. Defaults to 0.5.
-        optimizer (optax.GradientTransformation): Optax optimizer. If provided, this overrides the default Adam optimizer, and the learning_rate and clip_norm arguments are ignored. Defaults to None.
-        filter_spec (PyTree[BoolAxisSpec], optional): Equinox `filter_spec` for specifying trainable parameters. Either a callable `leaf -> bool`, or a PyTree with prefix structure matching `dist` with True/False values. Defaults to `eqx.is_inexact_array`.
-        show_progress (bool, optional): Whether to show progress bar. Defaults to True.
+        condition (Array | None): Conditioning variables. Defaults to None.
+        max_epochs (int): Maximum number of epochs. Defaults to 50.
+        max_patience (int): Number of consecutive epochs with no validation
+            loss improvement after which training is terminated. Defaults to 5.
+        batch_size (int): Batch size. Defaults to 256.
+        val_prop (float): Proportion of data to use in validation set. Defaults to 0.1.
+        learning_rate (float): Adam learning rate. Defaults to 5e-4.
+        clip_norm (float): Maximum gradient norm before clipping occurs. Defaults to 0.5.
+        optimizer (optax.GradientTransformation): Optax optimizer. If provided, this
+            overrides the default Adam optimizer, and the learning_rate and clip_norm
+            arguments are ignored. Defaults to None.
+        filter_spec (Callable | PyTree): Equinox `filter_spec` for
+            specifying trainable parameters. Either a callable `leaf -> bool`, or a
+            PyTree with prefix structure matching `dist` with True/False values.
+            Defaults to `eqx.is_inexact_array`.
+        show_progress (bool): Whether to show progress bar. Defaults to True.
     """
+    x = jnp.asarray(x)
+
+    if condition is not None:
+        condition = jnp.asarray(condition)
 
     @eqx.filter_jit
-    def loss_fn(dist, x, condition=None):
+    def loss_fn(dist_trainable, dist_static, x, condition=None):
+        dist = eqx.combine(dist_trainable, dist_static)
         return -dist.log_prob(x, condition).mean()
 
     @eqx.filter_jit
     def step(dist, optimizer, opt_state, x, condition=None):
-        loss_val, grads = eqx.filter_value_and_grad(loss_fn, arg=filter_spec)(
-            dist, x, condition
+        dist_trainable, dist_static = eqx.partition(dist, filter_spec)
+        loss_val, grads = eqx.filter_value_and_grad(loss_fn)(
+            dist_trainable, dist_static, x, condition
         )
         updates, opt_state = optimizer.update(grads, opt_state)
         dist = eqx.apply_updates(dist, updates)
         return dist, opt_state, loss_val
 
     if optimizer is None:
-        optimizer = optimizer = optax.chain(
-            optax.clip_by_global_norm(clip_norm), optax.adam(learning_rate=learning_rate)
+        optimizer = optax.chain(
+            optax.clip_by_global_norm(clip_norm),
+            optax.adam(learning_rate=learning_rate),
         )
-    
-    best_params, static = eqx.partition(dist, filter_spec)
+
+    best_params, static = eqx.partition(dist, filter_spec)  # type: ignore
     opt_state = optimizer.init(best_params)
 
-    key, train_val_split_key = random.split(key)
+    key, train_val_split_key = jr.split(key)
 
     inputs = (x,) if condition is None else (x, condition)
-    train_args, val_args = train_val_split(train_val_split_key, inputs, val_prop=val_prop)
+    train_args, val_args = train_val_split(
+        train_val_split_key, inputs, val_prop=val_prop
+    )
     train_len, val_len = train_args[0].shape[0], val_args[0].shape[0]
     if batch_size > train_len:
         raise ValueError(
-            f"The batch size ({batch_size}) cannot be greater than the train set size ({train_len})."
-            )
+            f"The batch size ({batch_size}) cannot be greater than the train set size "
+            f"({train_len})."
+        )
 
-    losses = {"train": [], "val": []}  # type: Dict[str, List[float]]
+    losses = {"train": [], "val": []}  # type: Dict[str, list[float]]
 
-    loop = tqdm(range(max_epochs)) if show_progress is True else range(max_epochs)
+    loop = tqdm(range(max_epochs), disable=not show_progress)
 
-    for epoch in loop:
-        key, subkey = random.split(key)
-        permutation = random.permutation(subkey, jnp.arange(train_len))
+    for _ in loop:
+        key, subkey = jr.split(key)
+        permutation = jr.permutation(subkey, jnp.arange(train_len))
         train_args = tuple(a[permutation] for a in train_args)
 
         epoch_train_loss = 0
         batch_start_idxs = range(0, train_len - batch_size + 1, batch_size)
         for i in batch_start_idxs:
             batch = tuple(a[i : i + batch_size] for a in train_args)
             dist, opt_state, loss_i = step(dist, optimizer, opt_state, *batch)
             epoch_train_loss += loss_i.item() / len(batch_start_idxs)
 
         epoch_val_loss = 0
         batch_start_idxs = range(0, val_len - batch_size + 1, batch_size)
         for i in batch_start_idxs:
             batch = tuple(a[i : i + batch_size] for a in val_args)
-            epoch_val_loss += loss_fn(dist, *batch).item() / len(batch_start_idxs)
+
+            epoch_val_loss += loss_fn(
+                *eqx.partition(dist, filter_spec), *batch
+            ).item() / len(batch_start_idxs)
 
         losses["train"].append(epoch_train_loss)
         losses["val"].append(epoch_val_loss)
 
         if epoch_val_loss == min(losses["val"]):
             best_params = eqx.filter(dist, filter_spec)
 
         elif count_fruitless(losses["val"]) > max_patience:
-            if show_progress == True:
-                loop.set_postfix_str(f"{loop.postfix} (Max patience reached)")
+            loop.set_postfix_str(f"{loop.postfix} (Max patience reached)")
             break
 
-        if show_progress:
-            loop.set_postfix({k: v[-1] for k, v in losses.items()})
+        loop.set_postfix({k: v[-1] for k, v in losses.items()})
 
-    dist = eqx.combine(best_params, static)
+    dist = eqx.combine(best_params, static)  # type: ignore
     return dist, losses
-
```

### Comparing `flowjax-8.1.0/flowjax/train/train_utils.py` & `flowjax-9.0.0/flowjax/train/train_utils.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,38 +1,40 @@
-from typing import Sequence, List
-from flowjax.utils import Array
-import jax.random as jr
+"""Utility functions for training."""
+from typing import Sequence
+
 import jax.numpy as jnp
+import jax.random as jr
+from jax import Array
 
 
 def train_val_split(key: jr.KeyArray, arrays: Sequence[Array], val_prop: float = 0.1):
     """Train validation split along axis 0.
 
     Args:
         key (KeyArray): Jax PRNGKey
-        arrays List[Array]: List of arrays.
-        val_prop (float, optional): Proportion of data to use for validation. Defaults to 0.1.
+        arrays Sequence[Array]: Sequence of arrays.
+        val_prop (float): Proportion of data to use for validation. Defaults to 0.1.
 
     Returns:
-        Tuple[Tuple]: (train_arrays, validation_arrays)
+        tuple[tuple]: (train_arrays, validation_arrays)
     """
-    if not (0 <= val_prop <= 1):
+    if not 0 <= val_prop <= 1:
         raise ValueError("val_prop should be between 0 and 1.")
-    n = arrays[0].shape[0]
-    permutation = jr.permutation(key, jnp.arange(n))
+    size_axis_0 = arrays[0].shape[0]
+    permutation = jr.permutation(key, jnp.arange(size_axis_0))
     arrays = tuple(a[permutation] for a in arrays)
-    n_train = n - round(val_prop * n)
+    n_train = size_axis_0 - round(val_prop * size_axis_0)
     train = tuple(a[:n_train] for a in arrays)
     val = tuple(a[n_train:] for a in arrays)
     return train, val
 
 
-def count_fruitless(losses: List[float]) -> int:
+def count_fruitless(losses: list[float]) -> int:
     """Given a list of losses from each epoch, count the number of epochs since
     the minimum loss.
 
     Args:
-        losses (List[float]): List of losses.
+        losses (list[float]): List of losses.
 
     """
     min_idx = jnp.argmin(jnp.array(losses)).item()
     return len(losses) - min_idx - 1
```

### Comparing `flowjax-8.1.0/flowjax/train/variational_fit.py` & `flowjax-9.0.0/flowjax/train/variational_fit.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,81 +1,107 @@
-from typing import Callable
+"""Basic training script for fitting a flow using variational inference."""
+from typing import Any, Callable
 
+import equinox as eqx
 import jax.random as jr
 import optax
-import equinox as eqx
+from jax import Array
 from tqdm import tqdm
 
-from flowjax.utils import Array
 from flowjax.distributions import Distribution
-from jaxtyping import PyTree
-from equinox.custom_types import BoolAxisSpec
+
+PyTree = Any
+
 
 @eqx.filter_jit
-def elbo_loss(key: jr.KeyArray, dist: Distribution, target: Callable[[Array], Array], num_samples: int):
+def elbo_loss(
+    dist: Distribution,
+    target: Callable[[Array], Array],
+    key: jr.KeyArray,
+    num_samples: int,
+) -> Array:
+    """The evidence lower bound loss function."""
     samples, approx_density = dist.sample_and_log_prob(key, (num_samples,))
     target_density = target(samples)
     losses = approx_density - target_density
     return losses.mean()
 
+
 def fit_to_variational_target(
     key: jr.KeyArray,
     dist: Distribution,
     target: Callable[[Array], Array],
-    loss_fn: Callable[[Distribution, Callable, jr.KeyArray, int], float] = elbo_loss,
+    loss_fn: Callable[[Distribution, Callable, jr.KeyArray, int], Array] = elbo_loss,
     steps: int = 100,
     samples_per_step: int = 500,
     learning_rate: float = 5e-4,
     clip_norm: float = 0.5,
-    optimizer: optax.GradientTransformation = None,
-    filter_spec: PyTree[BoolAxisSpec] = eqx.is_inexact_array,
+    optimizer: optax.GradientTransformation | None = None,
+    filter_spec: Callable | PyTree = eqx.is_inexact_array,
     show_progress: bool = True,
 ):
     """
     Train a distribution (e.g. a flow) by variational inference to a target
     (e.g. an unnormalized density).
-    
+
     Args:
         key (KeyArray): Jax PRNGKey.
-        dist (Distribution): Distribution object, trainable parameters are found using equinox.is_inexact_array.
-        target (Callable): The variational target (this is usually the unormalized log posterior)
-        loss_fn (Callable, optional): The loss function to optimize. The loss function should take
-            a random key, the distribution, a callable that maps samples from the distribution to a scalar loss,
-            and a number of samples to use. Defaults to elbo_loss.
-        steps (int, optional): The number of training steps to run. Defaults to 100.
-        samples_per_step (int, optional): number of samples to use at each step. Defaults to 500.
-        learning_rate (float, optional): Adam learning rate. Defaults to 5e-4.
-        clip_norm (float, optional): Maximum gradient norm before clipping occurs. Defaults to 0.5.
-        optimizer (optax.GradientTransformation): Optax optimizer. If provided, this overrides the default Adam optimizer, and the learning_rate and clip_norm arguments are ignored. Defaults to None.
-        filter_spec (PyTree[BoolAxisSpec], optional): Equinox `filter_spec` for specifying trainable parameters. Either a callable `leaf -> bool`, or a PyTree with prefix structure matching `dist` with True/False values. Defaults to `eqx.is_inexact_array`.
-        show_progress (bool, optional): Whether to show progress bar. Defaults to True.
+        dist (Distribution): Distribution object, trainable parameters are found
+            using equinox.is_inexact_array.
+        target (Callable): The variational target (this is usually the unormalized log
+            posterior)
+        loss_fn (Callable): The loss function to optimize. The loss function
+            should take a random key, the distribution, a callable that maps samples
+            from the distribution to a scalar loss, and a number of samples to use.
+            Defaults to elbo_loss.
+        steps (int): The number of training steps to run. Defaults to 100.
+        samples_per_step (int): number of samples to use at each step.
+            Defaults to 500.
+        learning_rate (float): Adam learning rate. Defaults to 5e-4.
+        clip_norm (float): Maximum gradient norm before clipping occurs.
+            Defaults to 0.5.
+        optimizer (optax.GradientTransformation | None): Optax optimizer. If provided,
+            this overrides the default Adam optimizer, and the learning_rate and
+            clip_norm arguments are ignored. Defaults to None.
+        filter_spec (Callable | PyTree): Equinox `filter_spec` for
+            specifying trainable parameters. Either a callable `leaf -> bool`, or a
+            PyTree with prefix structure matching `dist` with True/False values.
+            Defaults to `eqx.is_inexact_array`.
+        show_progress (bool): Whether to show progress bar. Defaults to True.
     """
     if optimizer is None:
         optimizer = optimizer = optax.chain(
-            optax.clip_by_global_norm(clip_norm), optax.adam(learning_rate=learning_rate)
+            optax.clip_by_global_norm(clip_norm),
+            optax.adam(learning_rate=learning_rate),
         )
 
     @eqx.filter_jit
     def step(dist, target, key, optimizer, opt_state):
-        loss_val, grads = eqx.filter_value_and_grad(loss_fn, arg=filter_spec)(
-            key, dist, target, samples_per_step
-            )
+        @eqx.filter_value_and_grad
+        def loss_val_and_grad(
+            dist_trainable, dist_static, target, key, samples_per_step
+        ):
+            dist = eqx.combine(dist_trainable, dist_static)
+            return loss_fn(dist, target, key, samples_per_step)
+
+        dist_trainable, dist_static = eqx.partition(dist, filter_spec)
+        loss_val, grads = loss_val_and_grad(
+            dist_trainable, dist_static, target, key, samples_per_step
+        )
         updates, opt_state = optimizer.update(grads, opt_state)
         dist = eqx.apply_updates(dist, updates)
         return dist, opt_state, loss_val
 
-    trainable_params, _ = eqx.partition(dist, filter_spec)
-    opt_state = optimizer.init(trainable_params)
+    dist_trainable, _ = eqx.partition(dist, filter_spec)  # type: ignore
+    opt_state = optimizer.init(dist_trainable)
 
     losses = []
 
-    loop = tqdm(range(steps)) if show_progress is True else range(steps)
-    for iteration in loop:
+    loop = tqdm(range(steps), disable=not show_progress)
+    for _ in loop:
         key, subkey = jr.split(key)
-        dist, opt_state, loss = step(dist, target, subkey, optimizer, opt_state)
-        
-        losses.append(loss.item())
+        dist, opt_state, loss = step(dist, target, subkey, optimizer, opt_state)  # type: ignore
 
-        if show_progress:
-            loop.set_postfix({'loss': losses[-1]})
+        losses.append(loss.item())
+        loop.set_postfix({"loss": losses[-1]})
 
-    return dist, losses
+    return dist, losses
```

### Comparing `flowjax-8.1.0/flowjax/utils.py` & `flowjax-9.0.0/flowjax/utils.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,111 +1,100 @@
-from typing import Any, Sequence
+"""Utility functions."""
+from typing import Sequence
+
+import equinox as eqx
 import jax
 import jax.numpy as jnp
-import equinox as eqx
-import jax.flatten_util as jfu
-
-Array = Any  # TODO Can use TypeAlias from typing in future.
-
+from jax import Array
+from jax.flatten_util import ravel_pytree
 
-def _identity(x):
-    return x
-
-
-def tile_until_length(x: Array, max_len: int):
-    """Tile array along until a maximum length is reached. If x.ndim > 1,
-    then the array is flattened, and a flattened array is returned.
-
-    Args:
-        x (Array): Input array.
-        max_len (int): Maximum length of output array.
-    """
-    x = jnp.ravel(x)
-    num_reps = max_len // len(x) + 1
-    y = jnp.tile(x, num_reps)
-    return y[:max_len]
+from flowjax.bijections.bijection import Bijection
 
 
 def real_to_increasing_on_interval(
     arr: Array, B: float = 1, softmax_adjust: float = 1e-2
 ):
     """Transform unconstrained parameter vector to monotonically increasing positions on [-B, B].
 
     Args:
         arr (Array): Parameter vector.
-        B (float, optional): Interval to transform output. Defaults to 1.
-        softmax_adjust (float, optional): Rescales softmax output using (widths + softmax_adjust/widths.size) / (1 + softmax_adjust). e.g. 0=no adjustment, 1=average softmax output with evenly spaced widths, >1 promotes more evenly spaced widths.
+        B (float): Interval to transform output. Defaults to 1.
+        softmax_adjust (float): Rescales softmax output using (widths +
+            softmax_adjust/widths.size) / (1 + softmax_adjust). e.g. 0=no adjustment,
+            1=average softmax output with evenly spaced widths, >1 promotes more evenly
+            spaced widths.
     """
     if softmax_adjust < 0:
         raise ValueError("softmax_adjust should be >= 0.")
-    widths = jax.nn.softmax(arr)
+    widths = jax.nn.softmax(arr)  # type: ignore
     widths = (widths + softmax_adjust / widths.size) / (1 + softmax_adjust)
     widths = widths.at[0].set(widths[0] / 2)
     return 2 * B * jnp.cumsum(widths) - B
 
 
 def inv_cum_sum(x):
+    """Inverse of cumulative sum operation."""
     return x - jnp.pad(x[:-1], (1, 0))
 
 
-def merge_shapes(shapes: Sequence):
-    """ "Broadcast shapes used in bijections and distributions.
-
-    Namely:
-        - A shape None is used to mean any shape (either unknown, unimportant, or compatible with any shape).
-        - We require all shapes that are not None to have the same length, and matching values.
-    """  # TODO update these docs.
+def merge_cond_shapes(shapes: Sequence):
+    """Merges shapes (tuples of ints or None) used in bijections and distributions.
+    Returns None if all shapes are None, otherwise checks the shapes match, and returns
+    the shape.
+    """
     if len(shapes) == 0:
         raise ValueError("No shapes have been provided.")
-    elif all(s is None for s in shapes):
+    if all(s is None for s in shapes):
         return None
-    else:
-        shapes = [s for s in shapes if s is not None]
-        if all(s == shapes[0] for s in shapes):
-            return shapes[0]
-        else:
-            raise ValueError("The shapes do not match.")
+    shapes = [s for s in shapes if s is not None]
+    if all(s == shapes[0] for s in shapes):
+        return shapes[0]
+    raise ValueError("The shapes do not match.")
 
 
-def check_shapes(shapes):  # TODO test this?
-    shapes = [s for s in shapes if s is not None]
-    if not all(s == shapes[0] for s in shapes):
-        raise ValueError("The shapes do not match.")
+def check_shapes_match(shapes: list[tuple[int, ...]]):
+    """Check shapes match and produce a useful error message."""
+
+    for i, shape in enumerate(shapes):
+        if shape != shapes[0]:
+            raise ValueError(
+                f"Expected shapes to match, but index 0 had shape {shapes[0]}, and "
+                f"index {i} had shape {shape}."
+            )
 
 
 def _get_ufunc_signature(in_shapes, out_shapes):
     """Convert a sequence of in_shapes, and out_shapes to a universal function signature.
-    
+
     Example:
         >>> _get_ufunc_signature([(3,),(2,3)], [()])
         "(3),(2,3)->()"
     """
+
     def _shapes_to_str(shapes):
-        result = [str(s) if len(s)!=1 else str(s).replace(",", "") for s in shapes]
+        result = [str(s) if len(s) != 1 else str(s).replace(",", "") for s in shapes]
         return ",".join(result).replace(" ", "")
 
     in_shapes_str = _shapes_to_str(in_shapes)
     out_shapes_str = _shapes_to_str(out_shapes)
     return f"{in_shapes_str}->{out_shapes_str}"
 
 
-
-
-def get_ravelled_bijection_constructor(bijection, filter_spec=eqx.is_inexact_array):
+def get_ravelled_bijection_constructor(
+    bijection: Bijection, filter_spec=eqx.is_inexact_array
+):
     """Given a bijection, returns a tuple containing
     1) a constructor for the bijection from a flattened array; 2) the current flattened
     parameters.
 
     Args:
         bijection (Bijection): Bijection.
         filter_spec: Filter function. Defaults to eqx.is_inexact_array.
     """
+    params, static = eqx.partition(bijection, filter_spec)  # type: ignore
+    current, unravel = ravel_pytree(params)
 
-    params, static = eqx.partition(bijection, filter_spec)
-    bias, unravel = jfu.ravel_pytree(params)
-
-    def f(ravelled_params: Array):
-        ravelled_params = ravelled_params + bias
+    def constructor(ravelled_params: Array):
         params = unravel(ravelled_params)
         return eqx.combine(params, static)
 
-    return f, bias
+    return constructor, current
```

### Comparing `flowjax-8.1.0/flowjax.egg-info/PKG-INFO` & `flowjax-9.0.0/flowjax.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flowjax
-Version: 8.1.0
+Version: 9.0.0
 Summary: Normalizing flow implementations in jax.
 Home-page: https://github.com/danielward27/flowjax.git
 Author: Daniel Ward
 Author-email: danielward27@outlook.com
 License: MIT
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `flowjax-8.1.0/flowjax.egg-info/SOURCES.txt` & `flowjax-9.0.0/flowjax.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -13,21 +13,26 @@
 flowjax.egg-info/requires.txt
 flowjax.egg-info/top_level.txt
 flowjax/bijections/__init__.py
 flowjax/bijections/affine.py
 flowjax/bijections/bijection.py
 flowjax/bijections/block_autoregressive_network.py
 flowjax/bijections/chain.py
+flowjax/bijections/concatenate.py
 flowjax/bijections/coupling.py
 flowjax/bijections/exp.py
 flowjax/bijections/jax_transforms.py
 flowjax/bijections/masked_autoregressive.py
 flowjax/bijections/rational_quadratic_spline.py
 flowjax/bijections/tanh.py
 flowjax/bijections/utils.py
 flowjax/nn/__init__.py
 flowjax/nn/block_autoregressive.py
 flowjax/nn/masked_autoregressive.py
 flowjax/train/__init__.py
 flowjax/train/data_fit.py
 flowjax/train/train_utils.py
-flowjax/train/variational_fit.py
+flowjax/train/variational_fit.py
+tests/test_distributions.py
+tests/test_flows.py
+tests/test_masks.py
+tests/test_utils.py
```

### Comparing `flowjax-8.1.0/setup.py` & `flowjax-9.0.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,30 +10,29 @@
     text_type = type("")
     with io.open(filename, mode="r", encoding="utf-8") as fd:
         return re.sub(text_type(r":[a-z]+:`~?(.*?)`"), text_type(r"``\1``"), fd.read())
 
 
 setup(
     name="flowjax",
-    version="8.1.0",
+    version="9.0.0",
     url="https://github.com/danielward27/flowjax.git",
     license="MIT",
     author="Daniel Ward",
     author_email="danielward27@outlook.com",
     description="Normalizing flow implementations in jax.",
     long_description=read("README.md"),
     long_description_content_type="text/markdown",
     packages=find_packages(exclude=("tests",)),
     install_requires=[
         "jax",
         "jaxlib>=0.3",
-        "equinox",
+        "equinox>=0.10",
         "tqdm",
         "optax",
-        "jaxtyping",
     ],
     python_requires=">=3.7",
     extras_require={"dev": ["pytest"]},
     classifiers=[
         "Development Status :: 2 - Pre-Alpha",
         "License :: OSI Approved :: MIT License",
         "Programming Language :: Python",
```

