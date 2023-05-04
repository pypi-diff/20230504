# Comparing `tmp/spyrit-2.0.0.tar.gz` & `tmp/spyrit-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/spyrit-2.0.0.tar", last modified: Fri Mar 24 14:43:18 2023, max compression
+gzip compressed data, was "spyrit-2.1.0.tar", last modified: Thu May  4 13:19:54 2023, max compression
```

## Comparing `spyrit-2.0.0.tar` & `spyrit-2.1.0.tar`

### file list

```diff
@@ -1,34 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 14:43:18.000000 spyrit-2.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)     6054 2023-03-24 14:43:18.000000 spyrit-2.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4321 2023-03-24 14:43:14.000000 spyrit-2.0.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-24 14:43:18.000000 spyrit-2.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1279 2023-03-24 14:43:14.000000 spyrit-2.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 14:43:18.000000 spyrit-2.0.0/spyrit/
--rw-r--r--   0 runner    (1001) docker     (123)      500 2023-03-24 14:43:14.000000 spyrit-2.0.0/spyrit/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 14:43:18.000000 spyrit-2.0.0/spyrit/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-24 14:43:14.000000 spyrit-2.0.0/spyrit/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23849 2023-03-24 14:43:14.000000 spyrit-2.0.0/spyrit/core/meas.py
--rw-r--r--   0 runner    (1001) docker     (123)     8176 2023-03-24 14:43:14.000000 spyrit-2.0.0/spyrit/core/nnet.py
--rw-r--r--   0 runner    (1001) docker     (123)    16294 2023-03-24 14:43:14.000000 spyrit-2.0.0/spyrit/core/noise.py
--rw-r--r--   0 runner    (1001) docker     (123)    19473 2023-03-24 14:43:14.000000 spyrit-2.0.0/spyrit/core/prep.py
--rw-r--r--   0 runner    (1001) docker     (123)    29107 2023-03-24 14:43:14.000000 spyrit-2.0.0/spyrit/core/recon.py
--rw-r--r--   0 runner    (1001) docker     (123)    24926 2023-03-24 14:43:14.000000 spyrit-2.0.0/spyrit/core/train.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 14:43:18.000000 spyrit-2.0.0/spyrit/misc/
--rw-r--r--   0 runner    (1001) docker     (123)      472 2023-03-24 14:43:14.000000 spyrit-2.0.0/spyrit/misc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1936 2023-03-24 14:43:14.000000 spyrit-2.0.0/spyrit/misc/data_visualisation.py
--rw-r--r--   0 runner    (1001) docker     (123)     8851 2023-03-24 14:43:14.000000 spyrit-2.0.0/spyrit/misc/disp.py
--rw-r--r--   0 runner    (1001) docker     (123)     1185 2023-03-24 14:43:14.000000 spyrit-2.0.0/spyrit/misc/examples.py
--rw-r--r--   0 runner    (1001) docker     (123)     2140 2023-03-24 14:43:14.000000 spyrit-2.0.0/spyrit/misc/load_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     2968 2023-03-24 14:43:14.000000 spyrit-2.0.0/spyrit/misc/matrix_tools.py
--rw-r--r--   0 runner    (1001) docker     (123)     7981 2023-03-24 14:43:14.000000 spyrit-2.0.0/spyrit/misc/metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)    14960 2023-03-24 14:43:14.000000 spyrit-2.0.0/spyrit/misc/pattern_choice.py
--rw-r--r--   0 runner    (1001) docker     (123)     6519 2023-03-24 14:43:14.000000 spyrit-2.0.0/spyrit/misc/sampling.py
--rw-r--r--   0 runner    (1001) docker     (123)    23048 2023-03-24 14:43:14.000000 spyrit-2.0.0/spyrit/misc/statistics.py
--rw-r--r--   0 runner    (1001) docker     (123)    36895 2023-03-24 14:43:14.000000 spyrit-2.0.0/spyrit/misc/walsh_hadamard.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 14:43:18.000000 spyrit-2.0.0/spyrit.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6054 2023-03-24 14:43:18.000000 spyrit-2.0.0/spyrit.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      650 2023-03-24 14:43:18.000000 spyrit-2.0.0/spyrit.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-24 14:43:18.000000 spyrit-2.0.0/spyrit.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-24 14:43:18.000000 spyrit-2.0.0/spyrit.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-03-24 14:43:18.000000 spyrit-2.0.0/spyrit.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-03-24 14:43:18.000000 spyrit-2.0.0/spyrit.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:19:54.856442 spyrit-2.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     7651 2023-05-04 13:19:49.000000 spyrit-2.1.0/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3776 2023-05-04 13:19:54.856442 spyrit-2.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3157 2023-05-04 13:19:49.000000 spyrit-2.1.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-04 13:19:54.856442 spyrit-2.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1279 2023-05-04 13:19:49.000000 spyrit-2.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:19:54.852442 spyrit-2.1.0/spyrit/
+-rw-r--r--   0 runner    (1001) docker     (123)      500 2023-05-04 13:19:49.000000 spyrit-2.1.0/spyrit/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:19:54.852442 spyrit-2.1.0/spyrit/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 13:19:49.000000 spyrit-2.1.0/spyrit/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19100 2023-05-04 13:19:49.000000 spyrit-2.1.0/spyrit/core/meas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8176 2023-05-04 13:19:49.000000 spyrit-2.1.0/spyrit/core/nnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16294 2023-05-04 13:19:49.000000 spyrit-2.1.0/spyrit/core/noise.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17890 2023-05-04 13:19:49.000000 spyrit-2.1.0/spyrit/core/prep.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26360 2023-05-04 13:19:49.000000 spyrit-2.1.0/spyrit/core/recon.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24926 2023-05-04 13:19:49.000000 spyrit-2.1.0/spyrit/core/train.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:19:54.852442 spyrit-2.1.0/spyrit/misc/
+-rw-r--r--   0 runner    (1001) docker     (123)      472 2023-05-04 13:19:49.000000 spyrit-2.1.0/spyrit/misc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1936 2023-05-04 13:19:49.000000 spyrit-2.1.0/spyrit/misc/data_visualisation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8851 2023-05-04 13:19:49.000000 spyrit-2.1.0/spyrit/misc/disp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1185 2023-05-04 13:19:49.000000 spyrit-2.1.0/spyrit/misc/examples.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2140 2023-05-04 13:19:49.000000 spyrit-2.1.0/spyrit/misc/load_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2968 2023-05-04 13:19:49.000000 spyrit-2.1.0/spyrit/misc/matrix_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7981 2023-05-04 13:19:49.000000 spyrit-2.1.0/spyrit/misc/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14960 2023-05-04 13:19:49.000000 spyrit-2.1.0/spyrit/misc/pattern_choice.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6443 2023-05-04 13:19:49.000000 spyrit-2.1.0/spyrit/misc/sampling.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23048 2023-05-04 13:19:49.000000 spyrit-2.1.0/spyrit/misc/statistics.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36895 2023-05-04 13:19:49.000000 spyrit-2.1.0/spyrit/misc/walsh_hadamard.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:19:54.852442 spyrit-2.1.0/spyrit.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3776 2023-05-04 13:19:54.000000 spyrit-2.1.0/spyrit.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      661 2023-05-04 13:19:54.000000 spyrit-2.1.0/spyrit.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 13:19:54.000000 spyrit-2.1.0/spyrit.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 13:19:54.000000 spyrit-2.1.0/spyrit.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-04 13:19:54.000000 spyrit-2.1.0/spyrit.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-04 13:19:54.000000 spyrit-2.1.0/spyrit.egg-info/top_level.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `spyrit-2.0.0/setup.py` & `spyrit-2.1.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from sys import platform as _platform
 
 def readme():
     with open("README.md") as f:
         return f.read()
 
 setup(name='spyrit',
-      version='2.0.0',
+      version='2.1.0',
       description='Demo package',
       url='https://github.com/openspyrit/spyrit',
       long_description = readme(),
       long_description_content_type = "text/markdown",
       classifiers = [
         "Development Status :: 5 - Production/Stable",
         "License :: OSI Approved :: MIT License",
```

### Comparing `spyrit-2.0.0/spyrit/core/meas.py` & `spyrit-2.1.0/spyrit/core/meas.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,13 +1,15 @@
+import warnings
 import torch
 import torch.nn as nn
 import numpy as np
 from typing import Union
 from spyrit.misc.walsh_hadamard import walsh2_torch, walsh2_matrix
 from spyrit.misc.sampling import Permutation_Matrix
+
 # ==================================================================================
 class Linear(nn.Module):
 # ==================================================================================
     r""" 
         Computes linear measurements from incoming images: :math:`y = Hx`, 
         where :math:`H` is a linear operator (matrix) and :math:`x` is a 
         vectorized image.
@@ -15,42 +17,83 @@
         The class is constructed from a :math:`M` by :math:`N` matrix :math:`H`, 
         where :math:`N` represents the number of pixels in the image and 
         :math:`M` the number of measurements.
         
         Args:
             :attr:`H`: measurement matrix (linear operator) with shape :math:`(M, N)`.
             
+            :attr:`pinv`: Option to have access to pseudo inverse solutions. 
+            Defaults to `None` (the pseudo inverse is not initiliazed). 
+            
+            :attr:`reg` (optional): Regularization parameter (cutoff for small 
+            singular values, see :mod:`numpy.linal.pinv`). Only relevant when 
+            :attr:`pinv` is not `None`.
+
+
         Attributes:
-             :attr:`H`: The learnable measurement matrix of shape 
-             :math:`(M,N)` initialized as :math:`H`
-             
-             :attr:`H_adjoint`: The learnable adjoint measurement matrix 
-             of shape :math:`(N,M)` initialized as :math:`H^\top`
-             
+              :attr:`H`: The learnable measurement matrix of shape 
+              :math:`(M,N)` initialized as :math:`H`
              
+              :attr:`H_adjoint`: The learnable adjoint measurement matrix 
+              of shape :math:`(N,M)` initialized as :math:`H^\top`
+              
+              :attr:`H_pinv` (optional): The learnable adjoint measurement 
+              matrix of shape :math:`(N,M)` initialized as :math:`H^\dagger`.
+              Only relevant when :attr:`pinv` is not `None`.
         
         Example:
-            >>> H = np.array(np.random.random([400, 1000]))
+            >>> H = np.random.random([400, 1000])
             >>> meas_op = Linear(H)
+            >>> print(meas_op)
+            Linear(
+              (H): Linear(in_features=1000, out_features=400, bias=False)
+              (H_adjoint): Linear(in_features=400, out_features=1000, bias=False)
+            )
+            
+        Example 2:
+            >>> H = np.random.random([400, 1000])
+            >>> meas_op = Linear(H, True)
+            >>> print(meas_op)
+            Linear(
+              (H): Linear(in_features=1000, out_features=400, bias=False)
+              (H_adjoint): Linear(in_features=400, out_features=1000, bias=False)
+              (H_pinv): Linear(in_features=400, out_features=1000, bias=False)
+            )
     """
 
-    def __init__(self, H: np.ndarray):  
+    def __init__(self, H: np.ndarray, pinv = None, reg: float = 1e-15):  
         super().__init__()
         # instancier nn.linear
         self.M = H.shape[0]
         self.N = H.shape[1]
+        
+        self.h = int(self.N**0.5) 
+        self.w = int(self.N**0.5)
+        if self.h*self.w != self.N:
+            warnings.warn("N is not a square. Please assign self.h and self.w manually.")
+        
         self.H = nn.Linear(self.N, self.M, False) 
         self.H.weight.data = torch.from_numpy(H).float()
         # Data must be of type float (or double) rather than the default float64 when creating torch tensor
         self.H.weight.requires_grad = False
 
         # adjoint (Remove?)
         self.H_adjoint = nn.Linear(self.M, self.N, False)
         self.H_adjoint.weight.data = torch.from_numpy(H.transpose()).float()
         self.H_adjoint.weight.requires_grad = False
+        
+        if pinv is None:
+            H_pinv = pinv
+            print('Pseudo inverse will not instanciated')
+            
+        else: 
+            H_pinv = np.linalg.pinv(H, rcond = reg)
+            self.H_pinv = nn.Linear(self.M, self.N, False)
+            self.H_pinv.weight.data = torch.from_numpy(H_pinv).float()
+            self.H_pinv.weight.requires_grad = False
                
     def forward(self, x: torch.tensor) -> torch.tensor: 
         r""" Applies linear transform to incoming images: :math:`y = Hx`.
 
         Args:
             :math:`x`: Batch of vectorized (flatten) images.
             
@@ -101,15 +144,36 @@
         
         Example:     
             >>> H = meas_op.get_H()
             >>> print('get_mat:', H.shape)
             get_mat: torch.Size([400, 1000])
             
         """
-        return self.H.weight.data;
+        return self.H.weight.data
+    
+    def pinv(self, x: torch.tensor) -> torch.tensor:
+        r""" Computer pseudo inverse solution :math:`y = H^\dagger x`
+
+        Args:
+            :math:`x`:  batch of measurement vectors.
+            
+        Shape:
+            :math:`x`: :math:`(*, M)`
+            
+            Output: :math:`(*, N)`
+            
+        Example:
+            >>> x = torch.rand([10,400], dtype=torch.float)        
+            >>> y = meas_op.pinv(x)
+            >>> print('pinv:', y.shape)
+            adjoint: torch.Size([10, 1000])
+        """
+        #Pmat.transpose()*f
+        x = self.H_pinv(x)        
+        return x
     
 # ==================================================================================
 class LinearSplit(Linear):
 # ==================================================================================
     r""" 
     Computes linear measurements from incoming images: :math:`y = Px`, 
     where :math:`P` is a linear operator (matrix) and :math:`x` is a 
@@ -305,184 +369,14 @@
             >>> x = meas_op.pinv(y)
             >>> print(x.shape)
             torch.Size([85, 1024])
         """
         x = self.adjoint(x)/self.N
         return x
 
-
-# ==================================================================================
-class Linear_shift(Linear):
-# ==================================================================================
-    r""" Linear with shifted pattern matrix of size :math:`(M+1,N)` and :math:`Perm` matrix of size :math:`(N,N)`.
-    
-        Args:
-            - Hsub: subsampled Hadamard matrix
-            - Perm: Permuation matrix
-            
-        Shape:
-            - Input1: :math:`(M, N)`
-            - Input2: :math:`(N, N)`
-            
-        Example:
-            >>> Hsub = np.array(np.random.random([400,32*32]))
-            >>> Perm = np.array(np.random.random([32*32,32*32]))
-            >>> FO_Shift = Linear_shift(Hsub, Perm)
-    
-    """
-    def __init__(self, Hsub, Perm):           
-        super().__init__(Hsub)
-        
-        # Todo: Use index rather than permutation (see misc.walsh_hadamard)
-        self.Perm = nn.Linear(self.N, self.N, False)
-        self.Perm.weight.data = torch.from_numpy(Perm.T)
-        self.Perm.weight.data = self.Perm.weight.data.float()
-        self.Perm.weight.requires_grad = False
-        
-        H_shift = torch.cat(
-            (torch.ones((1,self.N)),(self.Hsub.weight.data+1)/2))
-        
-        self.H_shift = nn.Linear(self.N, self.M+1, False) 
-        self.H_shift.weight.data = H_shift      # include the all-one pattern
-        self.H_shift.weight.data = self.H_shift.weight.data.float() # keep ?
-        self.H_shift.weight.requires_grad = False
-         
-    def forward(self, x: torch.tensor) -> torch.tensor:
-        r""" Applies Linear transform such that :math:`y = \begin{bmatrix}{1}\\{H_{sub}}\end{bmatrix}x`.
-        
-            Args:
-                :math:`x`: batch of images.
-                
-            Shape:
-                - Input: :math:`(b*c, N)` with :math:`b` the batch size, :math:`c` the number of channels, and :math:`N` the number of pixels in the image.
-                - Output: :math:`(b*c, M+1)` with :math:`b` the batch size, :math:`c` the number of channels, and :math:`M+1` the number of measurements + 1.
-                
-            Example:
-                >>> x = torch.tensor(np.random.random([10,32*32]), dtype=torch.float)
-                >>> y = FO_Shift(x)
-                >>> print(y.shape)
-                torch.Size([10, 401])
-        """
-        # input x is a set of images with shape (b*c, N)
-        # output input is a set of measurement vector with shape (b*c, M+1)
-        x = self.H_shift(x) 
-        return x
-              
-        #x_shift = super().forward(x) - x_dark.expand(x.shape[0],self.M) # (H-1/2)x
-        
-# ==================================================================================
-class Linear_pos(Linear):
-# ==================================================================================
-    r""" Linear with Permutation Matrix :math:`Perm` of size :math:`(N,N)`.
-    
-        Args:
-            - Hsub: subsampled Hadamard matrix
-            - Perm: Permuation matrix
-
-        Shape:
-            - Input1: :math:`(M, N)`
-            - Input2: :math:`(N, N)`
-
-        Example:
-            >>> Hsub = np.array(np.random.random([400,32*32]))
-            >>> Perm = np.array(np.random.random([32*32,32*32]))
-            >>> meas_op_pos = Linear_pos(Hsub, Perm)
-    """
-    def __init__(self, Hsub, Perm):           
-        super().__init__(Hsub)
-        
-        # Todo: Use index rather than permutation (see misc.walsh_hadamard)
-        self.Perm = nn.Linear(self.N, self.N, False)
-        self.Perm.weight.data = torch.from_numpy(Perm.T)
-        self.Perm.weight.data = self.Perm.weight.data.float()
-        self.Perm.weight.requires_grad = False
-        
-    def forward(self, x: torch.tensor) -> torch.tensor:
-        r"""Computes :math:`y` according to :math:`y=0.5(H_{sub}x+\sum_{j=1}^{N}x_{j})` where :math:`j` is the pixel (column) index of :math:`x`.
-        
-        Args:
-            :math:`x`: Batch of images.
-            
-        Shape:
-            - Input: :math:`(b*c, N)` with :math:`b` the batch size, :math:`c` the number of channels, and :math:`N` the number of pixels in the image.
-            - Output: :math:`(b*c, M)` with :math:`b` the batch size, :math:`c` the number of channels, and :math:`M` the number of measurements.
-            
-        Example:
-            >>> x = torch.tensor(np.random.random([10,32*32]), dtype=torch.float)
-            >>> y = meas_op_pos(x)
-            >>> print(y.shape)
-            torch.Size([100, 400]) 
-        """
-        # input x is a set of images with shape (b*c, N)
-        # output is a set of measurement vectors with shape (b*c, M)
-        
-        # compute 1/2(H+1)x = 1/2 HX + 1/2 1x
-        x = super().forward(x) + x.sum(dim=1,keepdim=True).expand(-1, self.M)
-        x *= 0.5
-        
-        return x
-    
-# ==================================================================================
-class Linear_shift_had(Linear_shift):
-# ==================================================================================
-    r""" Linear_shift operator with inverse method.
-    
-        Args:
-            - Hsub: subsampled Hadamard matrix
-            - Perm: Permuation matrix
-
-        Shape:
-            - Input1: :math:`(M, N)`
-            - Input2: :math:`(N, N)`.   
-    
-        Example:
-            >>> Hsub = np.array(np.random.random([400,32*32]))
-            >>> Perm = np.array(np.random.random([32*32,32*32]))
-            >>> FO_Shift_Had = Linear_shift_had(Hsub, Perm)
-    """
-    def __init__(self, Hsub, Perm):           
-        super().__init__(Hsub, Perm)
-    
-    def inverse(self, x: torch.tensor, n: Union[None, int] = None) -> torch.tensor:
-        r""" Inverse transform such that :math:`x = \frac{1}{N}H_{sub}y`.
-        
-        Args:
-            :math:`x`: Batch of completed measurements.
-            
-        Shape:
-            - Input: :math:`(b*c, N)` with :math:`b` the batch size, :math:`c` the number of channels, and :math:`N` the number of measurements.
-            - Output: :math:`(b*c, N)` with :math:`b` the batch size, :math:`c` the number of channels, and :math:`N` the number of reconstructed. pixels.
-            
-        Example:
-            >>> x = torch.tensor(np.random.random([10,32*32]), dtype=torch.float)
-            >>> x_reconstruct = FO_Shift_Had.inverse(y_pad) 
-            >>> print(x_reconstruct.shape)
-            torch.Size([10, 1024])          
-        """
-        # rearrange the terms + inverse transform
-        # maybe needs to be initialised with a permutation matrix as well!
-        # Permutation matrix may be sparsified when sparse tensors are no longer in
-        # beta (as of pytorch 1.11, it is still in beta).
-        
-        # --> Use index rather than permutation (see misc.walsh_hadamard)
-        
-        # input x is a set of **measurements** with shape (b*c, N)
-        # output is a set of **images** with shape (b*c, N)
-        bc, N = x.shape
-        x = self.Perm(x);
-        
-        if n is None:
-            n = int(np.sqrt(N))
-        
-        # Inverse transform    
-        x = x.view(bc, 1, n, n)
-        x = 1/self.N*walsh2_torch(x) # todo: initialize with 1D transform to speed up
-        x = x.view(bc, N)
-        return x
-
 # ==================================================================================
 class LinearRowSplit(nn.Module):
 # ================================================================================== 
     r""" Compute linear measurement of incoming images :math:`y = Px`, where 
         :math:`P` is a linear operator and :math:`x` is an image. Note that
         the same transform applies to each of the rows of the image :math:`x`.
```

### Comparing `spyrit-2.0.0/spyrit/core/nnet.py` & `spyrit-2.1.0/spyrit/core/nnet.py`

 * *Files identical despite different names*

### Comparing `spyrit-2.0.0/spyrit/core/noise.py` & `spyrit-2.1.0/spyrit/core/noise.py`

 * *Files identical despite different names*

### Comparing `spyrit-2.0.0/spyrit/core/prep.py` & `spyrit-2.1.0/spyrit/core/prep.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,90 +1,230 @@
 import torch
 import torch.nn as nn
 from spyrit.core.meas import Linear, LinearSplit, LinearRowSplit, HadamSplit
 from typing import Union, Tuple
+  
+#==============================================================================
+class DirectPoisson(nn.Module):
+#==============================================================================
+    r"""
+    Preprocess the raw data acquired with a direct measurement operator assuming 
+    Poisson noise.  It also compensates for the affine transformation applied 
+    to the images to get positive intensities.
+    
+    It computes :math:`m = \frac{2}{\alpha}y - H1` and the variance
+    :math:`\sigma^2 = 4\frac{y}{\alpha^{2}}`, where :math:`y = Hx` are obtained 
+    using a direct linear measurement operator (see :mod:`spyrit.core.Linear`),   
+    :math:`\alpha` is the image intensity, and 1 is the all-ones vector.
+    
+    Args:
+        :attr:`alpha`: maximun image intensity :math:`\alpha` (in counts)
+        
+        :attr:`meas_op`: measurement operator (see :mod:`~spyrit.core.meas`)
+        
+        
+    Example:
+        >>> H = np.random.random([400,32*32])
+        >>> meas_op =  Linear(H)
+        >>> prep_op = DirectPoisson(1.0, meas_op)
 
+    """
+    def __init__(self, alpha: float, meas_op):
+        super().__init__()
+        self.alpha = alpha
+        self.N = meas_op.N
+        self.M = meas_op.M
+        
+        self.max = nn.MaxPool1d(self.N)
+        self.register_buffer('H_ones', meas_op(torch.ones((1,self.N))))
+            
+    def forward(self, x: torch.tensor) -> torch.tensor:
+        r""" 
+        Preprocess measurements to compensate for the affine image normalization
+        
+        It computes :math:`\frac{1}{\alpha}x - H1`, where 1 represents the 
+        all-ones vector.
+        
+        Args:
+            :attr:`x`: batch of measurement vectors 
+            
+        Shape:
+            x: :math:`(B, M)` where :math:`B` is the batch dimension
+            
+            meas_op: the number of measurements :attr:`meas_op.M` should match
+            :math:`M`.
+            
+            Output: :math:`(B, M)`
+            
+        Example:
+            >>> x = torch.rand([10,400], dtype=torch.float)
+            >>> H = np.random.random([400,32*32])
+            >>> meas_op =  Linear(H)
+            >>> prep_op = DirectPoisson(1.0, meas_op)
+            >>> m = prep_op(x)
+            >>> print(m.shape)
+            torch.Size([10, 400])
+        """
+        # normalize
+        H_ones = self.H_ones.expand(x.shape[0],self.M)
+        x = 2*x/self.alpha - H_ones
+        return x
+    
+    def sigma(self, x: torch.tensor) -> torch.tensor:
+        r""" Estimates the variance of the preprocessed measurements 
+        
+        The variance is estimated as :math:`\frac{4}{\alpha^2} x`
+        
+        Args:
+            :attr:`x`: batch of measurement vectors 
+            
+        Shape:
+            :attr:`x`: :math:`(B,M)` where :math:`B` is the batch dimension
+            
+            Output: :math:`(B, M)`
+            
+        Example:
+            >>> x = torch.rand([10,400], dtype=torch.float)
+            >>> v = prep_op.sigma(x)
+            >>> print(v.shape)
+            torch.Size([10, 400])
+            
+        """
+        x = 4*x/(self.alpha**2) # Cov is in [-1,1] so *4
+        return x  
+    
+    def denormalize_expe(self, x, beta, h, w):
+        r""" 
+        Denormalize images from the range [-1;1] to the range [0; :math:`\beta`]
+        
+        It computes :math:`m = \frac{\beta}{2}(x+1)`, where 
+        :math:`\beta` is the normalization factor. 
+        
+        Args:
+            :attr:`x`: Batch of images
+            
+            :attr:`beta`: Normalizarion factor
+            
+            :attr:`h`: Image height
+            
+            :attr:`w`: Image width
+        
+        Shape:
+            :attr:`x`: :math:`(*, 1, h, w)`
+            
+            :attr:`beta`: :math:`(*)` or :math:`(*, 1)` 
+            
+            :attr:`h`: int
+            
+            :attr:`w`: int
+            
+            :attr:`Output`: :math:`(*, 1, h, w)`
+        
+        Example:
+            >>> x = torch.rand([10, 1, 32,32], dtype=torch.float)
+            >>> beta = 9*torch.rand([10])
+            >>> y = prep_op.denormalize_expe(x, beta, 32, 32)
+            >>> print(y.shape)
+            torch.Size([10, 1, 32, 32])
+                        
+        """
+        bc = x.shape[0]
+        
+        # Denormalization
+        beta = beta.view(bc,1,1,1)
+        beta = beta.expand(bc,1,h,w)
+        x = (x+1)/2*beta
+        
+        return x
+    
 #==============================================================================
 class SplitPoisson(nn.Module):
 #==============================================================================
     r"""
-    Preprocess raw data acquired with a split measurement operator
+    Preprocess the raw data acquired with a plit measurement operator assuming 
+    Poisson noise.  It also compensates for the affine transformation applied 
+    to the images to get positive intensities.
     
-    It computes :math:`m = \frac{y_{+}-y_{-}}{\alpha}` and the variance
+    It computes :math:`m = \frac{y_{+}-y_{-}}{\alpha} - H1` and the variance
     :math:`var = \frac{2(y_{+} + y_{-})}{\alpha^{2}}`, where 
     :math:`y_{+} = H_{+}x` and :math:`y_{-} = H_{-}x` are obtained using a 
-    split measurement operator (see :mod:`spyrit.core.LinearSplit`) and 
-    :math:`\alpha` is the image intensity.
-    
-    It also compensates for the affine transformation applied to x to get 
-    positive intensities.
-
+    split measurement operator (see :mod:`spyrit.core.LinearSplit`), 
+    :math:`\alpha` is the image intensity, and 1 is the all-ones vector.
     
     Args:
         alpha (float): maximun image intensity :math:`\alpha` (in counts)
         
-        M (int): number of measurements :math:`M`
+        :attr:`meas_op`: measurement operator (see :mod:`~spyrit.core.meas`)
         
-        N (int): number of pixels in the image :math:`N`
         
     Example:
-        >>> split_op = SplitPoisson(1.0, 400, 32*32)
+        >>> H = np.random.random([400,32*32])
+        >>> meas_op =  LinearSplit(H)
+        >>> split_op = SplitPoisson(10, meas_op)
+
+    Example 2:
+        >>> Perm = np.random.random([32,32])
+        >>> meas_op = HadamSplit(400, 32,  Perm)
+        >>> split_op = SplitPoisson(10, meas_op)
 
     """
-    def __init__(self, alpha: float, M: int, N: int):
+    def __init__(self, alpha: float, meas_op):
         super().__init__()
         self.alpha = alpha
-        self.N = N
-        self.M = M
+        self.N = meas_op.N
+        self.M = meas_op.M
         
-        self.even_index = range(0,2*M,2)
-        self.odd_index  = range(1,2*M,2)
-        self.max = nn.MaxPool1d(N)
+        self.even_index = range(0,2*self.M,2)
+        self.odd_index  = range(1,2*self.M,2)
+        self.max = nn.MaxPool1d(self.N)
+        
+        self.register_buffer('H_ones', meas_op.H(torch.ones((1,self.N))))
 
-    def forward(self, 
-                x: torch.tensor, 
-                meas_op: Union[LinearSplit, HadamSplit],
-                ) -> torch.tensor:
+    def forward(self, x: torch.tensor) -> torch.tensor:
         r""" 
         Preprocess to compensates for image normalization and splitting of the 
         measurement operator.
         
-        It computes :math:`\frac{x[0::2]-x[1::2]}{\alpha}`
+        It computes :math:`\frac{x[0::2]-x[1::2]}{\alpha} - H1`
         
         Args:
-            :attr:`x`: batch of images in the Hadamard domain 
-            
-            :attr:`meas_op`: measurement operator
+            :attr:`x`: batch of measurement vectors 
             
         Shape:
             x: :math:`(B, 2M)` where :math:`B` is the batch dimension
             
             meas_op: the number of measurements :attr:`meas_op.M` should match
             :math:`M`.
             
             Output: :math:`(B, M)`
             
         Example:
             >>> x = torch.rand([10,2*400], dtype=torch.float)
             >>> H = np.random.random([400,32*32])
             >>> meas_op =  LinearSplit(H)
-            >>> m = split_op(x, meas_op)
+            >>> split_op = SplitPoisson(10, meas_op)
+            >>> m = split_op(x)
+            >>> print(m.shape)
             torch.Size([10, 400])
             
         Example 2:
-            >>> Perm = np.random.random([32*32,32*32])
-            >>> meas_op = HadamSplit(H, Perm, 32, 32)
-            >>> m = split_op(x, meas_op)
+            >>> x = torch.rand([10,2*400], dtype=torch.float)
+            >>> Perm = np.random.random([32,32])
+            >>> meas_op = HadamSplit(400, 32,  Perm)
+            >>> split_op = SplitPoisson(10, meas_op)
+            >>> m = split_op(x)
             >>> print(m.shape)
             torch.Size([10, 400])
         """
+        H_ones = self.H_ones.expand(x.shape[0],self.M)
+        
         # unsplit
         x = x[:,self.even_index] - x[:,self.odd_index]
         # normalize
-        x = 2*x/self.alpha - meas_op.H(torch.ones(x.shape[0], self.N).to(x.device))
+        x = 2*x/self.alpha - H_ones
         return x
     
     def forward_expe(self, 
                      x: torch.tensor, 
                      meas_op: Union[LinearSplit, HadamSplit]
                      ) -> Tuple[torch.tensor, torch.tensor]:
         r""" 
@@ -117,16 +257,18 @@
             :math:`M`.
             
             :math:`m`: :math:`(B, M)`
             
             :math:`\alpha`: :math:`(B)` 
         
         Example:
-            >>> Perm = np.random.random([32*32,32*32])
-            >>> meas_op = HadamSplit(H, Perm, 32, 32)
+            >>> x = torch.rand([10,2*400], dtype=torch.float)
+            >>> Perm = np.random.random([32,32])
+            >>> meas_op = HadamSplit(400, 32,  Perm)
+            >>> split_op = SplitPoisson(10, meas_op)
             >>> m, alpha = split_op.forward_expe(x, meas_op)
             >>> print(m.shape)
             >>> print(alpha.shape)
             torch.Size([10, 400])
             torch.Size([10])
         """
         bc = x.shape[0]
@@ -136,16 +278,18 @@
         
         # estimate alpha
         x_pinv = meas_op.pinv(x)
         alpha = self.max(x_pinv)
         alpha = alpha.expand(bc,self.M) # shape is (b*c, M)
         
         # normalize
+        H_ones = self.H_ones.expand(bc,self.M)
+        
         x = torch.div(x, alpha)
-        x = 2*x - meas_op.H(torch.ones(bc, self.N).to(x.device))
+        x = 2*x - H_ones
         
         alpha = alpha[:,0]    # shape is (b*c,)
 
         return x, alpha
     
     def sigma(self, x: torch.tensor) -> torch.tensor:
         r""" Estimates the variance of the preprocessed measurements 
@@ -241,17 +385,18 @@
             
             :attr:`meas_op`: An operator such that :attr:`meas_op.N` :math:`=N` 
             and :attr:`meas_op.M` :math:`=M`
             
             Output: :math:`(*, M)`
             
         Example:
-            >>> x = torch.rand([10,32*32], dtype=torch.float)
-            >>> Perm = np.random.random([32*32,32*32])
-            >>> meas_op = HadamSplit(H, Perm, 32, 32)
+            >>> x = torch.rand([10,2*400], dtype=torch.float)
+            >>> Perm = np.random.random([32,32])
+            >>> meas_op = HadamSplit(400, 32,  Perm)
+            >>> split_op = SplitPoisson(10, meas_op)
             >>> v = split_op.sigma_from_image(x, meas_op)
             >>> print(v.shape)
             torch.Size([10, 400])
         
         """        
         x = meas_op(x);
         x = x[:,self.even_index] + x[:,self.odd_index]
@@ -357,206 +502,8 @@
 
         """
         # unsplit
         x = x[:,self.even_index] - x[:,self.odd_index]
         # normalize
         e = torch.ones([x.shape[0], meas_op.N, self.h], device=x.device)
         x = 2*x/self.alpha - meas_op.forward_H(e)
-        return x
-    
-
-# ==================================================================================
-class Preprocess_shift_poisson(nn.Module):      # header needs to be updated!
-# ==================================================================================
-    r"""Preprocess the measurements acquired using shifted patterns corrupted 
-    by Poisson noise
-
-        Computes:
-        m = (2 m_shift - m_offset)/N_0
-        var = 4*Diag(m_shift + m_offset)/alpha**2
-        Warning: dark measurement is assumed to be the 0-th entry of raw measurements
-
-        Args:
-            - :math:`alpha`: noise level
-            - :math:`M`: number of measurements
-            - :math:`N`: number of image pixels
-
-        Shape:
-            - Input1: scalar
-            - Input2: scalar
-            - Input3: scalar
-
-        Example:
-            >>> PSP = Preprocess_shift_poisson(9, 400, 32*32)
-    """
-    def __init__(self, alpha, M, N):
-        super().__init__()
-        self.alpha = alpha
-        self.N = N
-        self.M = M
-
-    def forward(self, x: torch.tensor, meas_op: Linear) -> torch.tensor:
-        r"""  
-        
-            Warning:
-                - The offset measurement is the 0-th entry of the raw measurements.
-
-            Args:
-                - :math:`x`: Batch of images in Hadamard domain shifted by 1
-                - :math:`meas_op`: Forward_operator
-
-            Shape:
-                - Input: :math:`(b*c, M+1)`
-                - Output: :math:`(b*c, M)`
-
-            Example:
-                >>> Hsub = np.array(np.random.random([400,32*32]))
-                >>> FO = Forward_operator(Hsub)
-                >>> x = torch.tensor(np.random.random([10, 400+1]), dtype=torch.float)
-                >>> y_PSP = PSP(x, FO)
-                >>> print(y_PSP.shape)
-                torch.Size([10, 400])
-                         
-        """
-        y = self.offset(x)
-        x = 2*x[:,1:] - y.expand(x.shape[0],self.M) # Warning: dark measurement is the 0-th entry
-        x = x/self.alpha
-        x = 2*x - meas_op.H(torch.ones(x.shape[0], self.N).to(x.device)) # to shift images in [-1,1]^N
-        return x
-    
-    def sigma(self, x):
-        r"""
-            Args:
-                - :math:`x`: Batch of images in Hadamard domain shifted by 1
-
-            Shape:
-                - Input: :math:`(b*c, M+1)`
-
-            Example:
-                >>> x = torch.tensor(np.random.random([10, 400+1]), dtype=torch.float)
-                >>> sigma_PSP = PSP.sigma(x)
-                >>> print(sigma_PSP.shape)
-                torch.Size([10, 400])
-        """ 
-        # input x is a set of measurement vectors with shape (b*c, M+1)
-        # output is a set of measurement vectors with shape (b*c,M)
-        y = self.offset(x)
-        x = 4*x[:,1:] + y.expand(x.shape[0],self.M)
-        x = x/(self.alpha**2)
-        x = 4*x         # to shift images in [-1,1]^N
-        return x
-    
-    def cov(self, x): #return a full matrix ? It is such that Diag(a) + b
-        return x
-
-    def sigma_from_image(self, x, meas_op): # should check this!
-        # input x is a set of images with shape (b*c, N)
-        # input meas_op is a Forward_operator
-        x = meas_op.H(x)
-        y = self.offset(x)
-        x = x[:,1:] + y.expand(x.shape[0],self.M)
-        x = x/(self.alpha)     # here the alpha contribution is not squared.
-        return x
-    
-    def offset(self, x):
-        r""" Get offset component from bach of shifted images.
-        
-            Args:
-                - :math:`x`: Batch of shifted images
-
-            Shape:
-                - Input: :math:`(bc, M+1)`
-                - Output: :math:`(bc, 1)`
-
-            Example:
-                >>> x = torch.tensor(np.random.random([10, 400+1]), dtype=torch.float)
-                >>> y = PSP.offset(x)
-                >>> print(y.shape)
-                torch.Size([10, 1])
-        
-        """
-        y = x[:,0,None]
-        return y
-    
-# ==================================================================================
-class Preprocess_pos_poisson(nn.Module):  # header needs to be updated!
-# ==================================================================================
-    r"""Preprocess the measurements acquired using positive (shifted) patterns 
-    corrupted by Poisson noise
-    
-    The output value of the layer with input size :math:`(B*C, M)` can be 
-    described as:
-
-    .. math::
-        \text{out}((B*C)_i, M_j}) = 2*\text{input}((B*C)_i, M_j}) -
-        \sum_{k = 1}^{M-1} \text{input}((B*C)_i, M_k})
- 
-    The output size of the layer is :math:`(B*C, M)`, which is the imput size 
-
-
-        Warning:
-            dark measurement is assumed to be the 0-th entry of raw measurements
-
-        Args:
-            - :math:`alpha`: noise level
-            - :math:`M`: number of measurements
-            - :math:`N`: number of image pixels
-
-        Shape:
-            - Input1: scalar
-            - Input2: scalar
-            - Input3: scalar
-
-        Example:
-            >>> PPP = Preprocess_pos_poisson(9, 400, 32*32)
-               
-    """
-    def __init__(self, alpha, M, N):
-        super().__init__()
-        self.alpha = alpha
-        self.N = N
-        self.M = M
-
-    def forward(self, x: torch.tensor, meas_op: Linear) -> torch.tensor:
-        r"""
-        Args:
-            - :math:`x`: noise level
-            - :math:`meas_op`: Forward_operator
-
-        Shape:
-            - Input1: :math:`(bc, M)`
-            - Input2: None
-            - Output: :math:`(bc, M)`
-
-        Example:
-            >>> Hsub = np.array(np.random.random([400,32*32]))
-            >>> meas_op = Forward_operator(Hsub)
-            >>> x = torch.tensor(np.random.random([10, 400]), dtype=torch.float)
-            >>> y = PPP(x, meas_op)
-            torch.Size([10, 400])
-            
-        """
-        y = self.offset(x)
-        x = 2*x - y.expand(-1,self.M)
-        x = x/self.alpha
-        x = 2*x - meas_op.H(torch.ones(x.shape[0], self.N).to(x.device)) # to shift images in [-1,1]^N
-        return x
-    
-    def offset(self, x):
-        r""" Get offset component from bach of shifted images.
-        
-        Args:
-            - :math:`x`: Batch of shifted images
-        
-        Shape:
-            - Input: :math:`(bc, M)`
-            - Output: :math:`(bc, 1)`
-            
-        Example:
-            >>> x = torch.tensor(np.random.random([10, 400]), dtype=torch.float)
-            >>> y = PPP.offset(x)
-            >>> print(y.shape)
-            torch.Size([10, 1])
-        
-        """
-        y = 2/(self.M-2)*x[:,1:].sum(dim=1,keepdim=True)
-        return y
+        return x
```

### Comparing `spyrit-2.0.0/spyrit/core/recon.py` & `spyrit-2.1.0/spyrit/core/recon.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 Created on Fri Jan 20 11:03:12 2023
 
 @author: ducros
 """
 import torch
 import torch.nn as nn 
 import numpy as np
-from spyrit.core.meas import HadamSplit, LinearRowSplit
+from spyrit.core.meas import HadamSplit, LinearRowSplit, Linear
 import math
 
 # ==================================================================================
 class PseudoInverse(nn.Module):
 # ==================================================================================
     r""" Moore-Penrose Pseudoinverse
     
@@ -31,23 +31,24 @@
         >>> x = pinv_op(y, meas_op)
         >>> print(x.shape)
         torch.Size([85, 1024])
     """
     def __init__(self):
         super().__init__()
         
-    def forward(self, x: torch.tensor, meas_op: HadamSplit) -> torch.tensor:
+    def forward(self, x: torch.tensor, meas_op) -> torch.tensor:
         r""" Compute pseudo-inverse of measurements.
         
         Args:
             :attr:`x`: Batch of measurement vectors.
             
             :attr:`meas_op`: Measurement operator. Any class that 
             implements a :meth:`pinv` method can be used, e.g.,
             :class:`~spyrit.core.forwop.HadamSplit`. 
+            
         Shape:
             
             :attr:`x`: :math:`(*, M)`
             
             :attr:`meas_op`: not applicable
             
             :attr:`output`: :math:`(*, N)`
@@ -60,121 +61,14 @@
             >>> pinv_op = PseudoInverse()
             >>> x = pinv_op(y, meas_op)
             >>> print(x.shape)
             torch.Size([85, 1024])
         """
         x = meas_op.pinv(x)
         return x
-
-# ==================================================================================
-class PseudoInverseStore(nn.Module):
-# ==================================================================================
-    r""" Moore-Penrose Pseudoinverse
-    
-    Considering linear measurements :math:`y = Hx`, where :math:`H` is the
-    measurement matrix and :math:`x` is a vectorized image, it estimates 
-    :math:`x` from :math:`y` by computing :math:`\hat{x} = H^\dagger y`, where 
-    :math:`H^\dagger` is the Moore-Penrose pseudo inverse of :math:`H`.
-
-    Args:           
-        :attr:`meas_op`: Measurement operator that defines :math:`H`. Any class
-        that implements a :meth:`get_H` method can be used, e.g.,
-        :class:`~spyrit.core.forwop.LinearRowSplit`. 
-        
-        :attr:`reg` (optional): Regularization parameter (cutoff for small 
-        singular values, see :mod:`numpy.linal.pinv`). 
-        
-        :attr:`learn` (optional): Option to learn the pseudo inverse matrix. By 
-        default the pseudo inverse is frozen during training. 
-
-    Attributes:
-        :attr:`H_pinv`: The learnable pseudo inverse matrix of shape 
-        :math:`(N,M)` initialized as :math:`H^\dagger`.
-        
-    .. note::
-        Contrary to :class:`~spyrit.core.recon.PseudoInverse`, the pseudoinverse
-        matrix is stored and therefore learnable
-    
-    Example 1:
-        >>> H_pos = np.random.rand(24,64)
-        >>> H_neg = np.random.rand(24,64)
-        >>> meas_op = LinearRowSplit(H_pos,H_neg)
-        >>> recon_op = PseudoInverseStore(meas_op)
-        
-    Example 2:
-        >>> M = 63
-        >>> N = 64
-        >>> B = 1
-        >>> H = walsh_matrix(N)
-        >>> H_pos = np.where(H>0,H,0)[:M,:]
-        >>> H_neg = np.where(H<0,-H,0)[:M,:]
-        >>> meas_op = LinearRowSplit(H_pos,H_neg)
-        >>> recon_op = PseudoInverseStore(meas_op)
-        
-    """
-    def __init__(self, 
-                 meas_op: LinearRowSplit, 
-                 reg: float = 1e-15,
-                 learn: bool = False):
-        
-        H = meas_op.get_H() 
-        M, N = H.shape
-        H_pinv = np.linalg.pinv(H, rcond = reg)
-        
-        super().__init__()
-        
-        self.H_pinv = nn.Linear(M, N, False)
-        self.H_pinv.weight.data = torch.from_numpy(H_pinv).float()
-        self.H_pinv.weight.requires_grad = learn
-        
-        
-    def forward(self, x: torch.tensor) -> torch.tensor:
-        r""" Compute pseudo-inverse of measurements.
-        
-        Args:
-            - :attr:`x`: Batch of measurement vectors.
-            
-        Shape:
-            - :attr:`x`: :math:`(*, M)`
-            - :attr:`output`: :math:`(*, N)`
-
-        Example 1:
-            >>> H_pos = np.random.rand(24,64)
-            >>> H_neg = np.random.rand(24,64)
-            >>> meas_op = LinearRowSplit(H_pos,H_neg)
-            >>> recon_op = PseudoInverseStore(meas_op)
-            >>> x = torch.rand([10,24,92], dtype=torch.float)
-            >>> y = recon_op(x)
-            >>> print(y.shape)
-            torch.Size([10, 64, 92])
-            
-        Example 2:
-            >>> M = 63
-            >>> N = 64
-            >>> B = 1
-            >>> H = walsh_matrix(N)
-            >>> H_pos = np.where(H>0,H,0)[:M,:]
-            >>> H_neg = np.where(H<0,-H,0)[:M,:]
-            >>> meas_op = LinearRowSplit(H_pos,H_neg)
-            >>> noise_op = NoNoise(meas_op)
-            >>> split_op = SplitRowPoisson(1.0, M, 92)
-            >>> recon_op = PseudoInverseStore(meas_op)
-            >>> x = torch.FloatTensor(B,N,92).uniform_(-1, 1)
-            >>> y = noise_op(x)
-            >>> m = split_op(y, meas_op)
-            >>> z = recon_op(m)
-            >>> print(z.shape)
-            >>> print(torch.linalg.norm(x - z)/torch.linalg.norm(x))
-            torch.Size([1, 64, 92])
-            tensor(0.1338)
-        """
-        x = torch.transpose(x,1,2) #swap last two dimensions
-        x = self.H_pinv(x)
-        x = torch.transpose(x,1,2) #swap last two dimensions
-        return x
     
 # ===========================================================================================
 class TikhonovMeasurementPriorDiag(nn.Module): 
 # ===========================================================================================   
     r"""
     Tikhonov regularization with prior in the measurement domain
     
@@ -506,15 +400,15 @@
             >>> prep = SplitPoisson(1.0, M, H**2)
             >>> recnet = PinvNet(noise, prep) 
             >>> x = torch.rand((B*C,2*M), dtype=torch.float)
             >>> z = recnet.reconstruct(x)
             >>> print(z.shape)
             torch.Size([10, 1, 64, 64])
         """
-        m = self.prep(y, self.acqu.meas_op)
+        m = self.prep(y)
         m = torch.nn.functional.pad(m, (0, self.acqu.meas_op.N-self.acqu.meas_op.M))
         z = m @ self.acqu.meas_op.Perm.weight.data.T
         z = z.view(-1,1,self.acqu.meas_op.h, self.acqu.meas_op.w)
         
         return z
 
     def reconstruct(self, x):
@@ -540,24 +434,61 @@
             >>> print(z.shape)
             torch.Size([10, 1, 64, 64])
         """
         # Measurement to image domain mapping
         bc, _ = x.shape
     
         # Preprocessing in the measurement domain
-        x = self.prep(x, self.acqu.meas_op) # shape x = [b*c, M]
+        x = self.prep(x) # shape x = [b*c, M]
     
         # measurements to image-domain processing
         x = self.pinv(x, self.acqu.meas_op)               # shape x = [b*c,N]
                 
         # Image-domain denoising
         x = x.view(bc,1,self.acqu.meas_op.h, self.acqu.meas_op.w)   # shape x = [b*c,1,h,w]
         x = self.denoi(x)                       
         
         return x
+    
+    def reconstruct_pinv(self, x):
+        r""" Reconstruction step of a reconstruction network
+            
+        Args:
+            :attr:`x`: raw measurement vectors
+        
+        Shape:
+            :attr:`x`: :math:`(BC,2M)`
+            
+            :attr:`output`: :math:`(BC,1,H,W)`
+        
+        Example:
+            >>> B, C, H, M = 10, 1, 64, 64**2
+            >>> Ord = np.ones((H,H))
+            >>> meas = HadamSplit(M, H, Ord)
+            >>> noise = NoNoise(meas)
+            >>> prep = SplitPoisson(1.0, M, H**2)
+            >>> recnet = PinvNet(noise, prep) 
+            >>> x = torch.rand((B*C,2*M), dtype=torch.float)
+            >>> z = recnet.reconstruct_pinv(x)
+            >>> print(z.shape)
+            torch.Size([10, 1, 64, 64])
+        """
+        # Measurement to image domain mapping
+        bc, _ = x.shape
+    
+        # Preprocessing in the measurement domain
+        x = self.prep(x)#, self.acqu.meas_op) # shape x = [b*c, M]
+    
+        # measurements to image-domain processing
+        x = self.pinv(x, self.acqu.meas_op)               # shape x = [b*c,N]
+                
+        # Image-domain denoising
+        x = x.view(bc,1,self.acqu.meas_op.h, self.acqu.meas_op.w)   # shape x = [b*c,1,h,w]                       
+        
+        return x
 
 
     def reconstruct_expe(self, x):
         r""" Reconstruction step of a reconstruction network
         
         Same as :meth:`reconstruct` reconstruct except that:
             
@@ -590,15 +521,15 @@
         print(x.max())
         
         # Denormalization 
         x = self.prep.denormalize_expe(x, N0_est, self.acqu.meas_op.h, 
                                                   self.acqu.meas_op.w)
         return x
     
-# ===========================================================================================
+#%%===========================================================================================
 class DCNet(nn.Module):
 # ===========================================================================================
     r""" Denoised completion reconstruction network
     
     .. math:
         
     
@@ -751,15 +682,15 @@
             torch.Size([10, 1, 64, 64])
         """
         # x of shape [b*c, 2M]
         bc, _ = x.shape
     
         # Preprocessing
         var_noi = self.prep.sigma(x)
-        x = self.prep(x, self.Acq.meas_op) # shape x = [b*c, M]
+        x = self.prep(x) # shape x = [b*c, M]
     
         # measurements to image domain processing
         x_0 = torch.zeros((bc, self.Acq.meas_op.N), device=x.device)
         x = self.tikho(x, x_0, var_noi, self.Acq.meas_op)
         x = x.view(bc,1,self.Acq.meas_op.h, self.Acq.meas_op.w)   # shape x = [b*c,1,h,w]
         
         # Image domain denoising
```

### Comparing `spyrit-2.0.0/spyrit/core/train.py` & `spyrit-2.1.0/spyrit/core/train.py`

 * *Files identical despite different names*

### Comparing `spyrit-2.0.0/spyrit/misc/data_visualisation.py` & `spyrit-2.1.0/spyrit/misc/data_visualisation.py`

 * *Files identical despite different names*

### Comparing `spyrit-2.0.0/spyrit/misc/disp.py` & `spyrit-2.1.0/spyrit/misc/disp.py`

 * *Files identical despite different names*

### Comparing `spyrit-2.0.0/spyrit/misc/examples.py` & `spyrit-2.1.0/spyrit/misc/examples.py`

 * *Files identical despite different names*

### Comparing `spyrit-2.0.0/spyrit/misc/load_data.py` & `spyrit-2.1.0/spyrit/misc/load_data.py`

 * *Files identical despite different names*

### Comparing `spyrit-2.0.0/spyrit/misc/matrix_tools.py` & `spyrit-2.1.0/spyrit/misc/matrix_tools.py`

 * *Files identical despite different names*

### Comparing `spyrit-2.0.0/spyrit/misc/metrics.py` & `spyrit-2.1.0/spyrit/misc/metrics.py`

 * *Files identical despite different names*

### Comparing `spyrit-2.0.0/spyrit/misc/pattern_choice.py` & `spyrit-2.1.0/spyrit/misc/pattern_choice.py`

 * *Files identical despite different names*

### Comparing `spyrit-2.0.0/spyrit/misc/sampling.py` & `spyrit-2.1.0/spyrit/misc/sampling.py`

 * *Files 3% similar despite different names*

```diff
@@ -95,29 +95,31 @@
     Reorder = rankdata(-Mat, method = 'ordinal');
     Columns = np.array(range(nx*ny));
     P = np.zeros((nx*ny, nx*ny));
     P[Reorder-1, Columns] = 1;
     return P
 
 def reorder(meas: np.ndarray, 
-            ord_acq: np.ndarray, 
-            ord_rec:  np.ndarray) -> np.ndarray:
+            Perm_acq: np.ndarray, 
+            Perm_rec:  np.ndarray) -> np.ndarray:
     r"""Reorder measurement vectors
 
     Args:
         meas (np.ndarray):
             Measurements with dimensions (:math:`M_{acq} \times K_{rep}`), where 
             :math:`M_{acq}` is the number of acquired patterns and 
             :math:`K_{rep}` is the number of acquisition repetitions 
             (e.g., wavelength or image batch).
-        ord_acq (np.ndarray): 
-            Sampling order used for acquisition 
-            (:math:`N_{acq} \times N_{acq}` square matrix).
-        ord_rec (np.ndarray): 
-            Sampling order used for reconstruction 
+
+        Perm_acq (np.ndarray): 
+            Permutation matrix used for acquisition 
+            (:math:`N_{acq}^2 \times N_{acq}^2` square matrix).
+            
+        Perm_rec (np.ndarray): 
+            Permutation matrix used for reconstruction 
             (:math:`N_{rec} \times N_{rec}` square matrix).
 
     Returns:
         (np.ndarray): 
             Measurements with dimensions (:math:`M_{rec} \times K_{rep}`), 
             where :math:`M_{rec} = N_{rec}^2`.
             
@@ -125,22 +127,18 @@
             If :math:`M_{rec} < M_{acq}`, the input measurement vectors are 
             subsampled.
             
             If :math:`M_{rec} > M_{acq}`, the input measurement vectors are 
             filled with zeros.
     """    
     # Dimensions (N.B: images are assumed to be square)
-    N_acq = ord_acq.shape[0]
-    N_rec = ord_rec.shape[0]
+    N_acq = int(Perm_acq.shape[0]**.5)
+    N_rec = int(Perm_rec.shape[0]**.5)
     K_rep = meas.shape[1]
     
-    # Order used for acquisistion
-    Perm_acq = Permutation_Matrix(ord_acq) 
-    Perm_rec = Permutation_Matrix(ord_rec)
-    
     # Acquisition order -> natural order (fill with zeros if necessary)
     if N_rec > N_acq:
         
         # Square subsampling in the "natural" order
         Ord_sub = np.zeros((N_rec,N_rec))
         Ord_sub[:N_acq,:N_acq]= -np.arange(-N_acq**2,0).reshape(N_acq,N_acq)
         Perm_sub = Permutation_Matrix(Ord_sub)
```

### Comparing `spyrit-2.0.0/spyrit/misc/statistics.py` & `spyrit-2.1.0/spyrit/misc/statistics.py`

 * *Files identical despite different names*

### Comparing `spyrit-2.0.0/spyrit/misc/walsh_hadamard.py` & `spyrit-2.1.0/spyrit/misc/walsh_hadamard.py`

 * *Files identical despite different names*

### Comparing `spyrit-2.0.0/spyrit.egg-info/SOURCES.txt` & `spyrit-2.1.0/spyrit.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+LICENSE.md
 README.md
 setup.py
 spyrit/__init__.py
 spyrit.egg-info/PKG-INFO
 spyrit.egg-info/SOURCES.txt
 spyrit.egg-info/dependency_links.txt
 spyrit.egg-info/not-zip-safe
```

