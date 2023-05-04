# Comparing `tmp/TorchRegister-0.2.1.tar.gz` & `tmp/TorchRegister-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "TorchRegister-0.2.1.tar", last modified: Thu Apr 27 23:14:19 2023, max compression
+gzip compressed data, was "TorchRegister-0.2.2.tar", last modified: Thu May  4 09:05:25 2023, max compression
```

## Comparing `TorchRegister-0.2.1.tar` & `TorchRegister-0.2.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 23:14:19.152772 TorchRegister-0.2.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-04-27 23:14:08.000000 TorchRegister-0.2.1/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-04-27 23:14:08.000000 TorchRegister-0.2.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      336 2023-04-27 23:14:19.152772 TorchRegister-0.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3326 2023-04-27 23:14:08.000000 TorchRegister-0.2.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-27 23:14:19.152772 TorchRegister-0.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      588 2023-04-27 23:14:08.000000 TorchRegister-0.2.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 23:14:19.148772 TorchRegister-0.2.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 23:14:19.152772 TorchRegister-0.2.1/src/TorchRegister/
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-04-27 23:14:08.000000 TorchRegister-0.2.1/src/TorchRegister/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3029 2023-04-27 23:14:08.000000 TorchRegister-0.2.1/src/TorchRegister/torchregister.py
--rw-r--r--   0 runner    (1001) docker     (123)    15688 2023-04-27 23:14:08.000000 TorchRegister-0.2.1/src/TorchRegister/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     9237 2023-04-27 23:14:08.000000 TorchRegister-0.2.1/src/TorchRegister/warpings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 23:14:19.152772 TorchRegister-0.2.1/src/TorchRegister.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      336 2023-04-27 23:14:19.000000 TorchRegister-0.2.1/src/TorchRegister.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      367 2023-04-27 23:14:19.000000 TorchRegister-0.2.1/src/TorchRegister.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 23:14:19.000000 TorchRegister-0.2.1/src/TorchRegister.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-04-27 23:14:19.000000 TorchRegister-0.2.1/src/TorchRegister.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-27 23:14:19.000000 TorchRegister-0.2.1/src/TorchRegister.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:05:25.778228 TorchRegister-0.2.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-05-04 09:05:11.000000 TorchRegister-0.2.2/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-05-04 09:05:11.000000 TorchRegister-0.2.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      336 2023-05-04 09:05:25.778228 TorchRegister-0.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4449 2023-05-04 09:05:11.000000 TorchRegister-0.2.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-04 09:05:25.778228 TorchRegister-0.2.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      588 2023-05-04 09:05:11.000000 TorchRegister-0.2.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:05:25.770228 TorchRegister-0.2.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:05:25.774228 TorchRegister-0.2.2/src/TorchRegister/
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-04 09:05:11.000000 TorchRegister-0.2.2/src/TorchRegister/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3029 2023-05-04 09:05:11.000000 TorchRegister-0.2.2/src/TorchRegister/torchregister.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15993 2023-05-04 09:05:11.000000 TorchRegister-0.2.2/src/TorchRegister/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9237 2023-05-04 09:05:11.000000 TorchRegister-0.2.2/src/TorchRegister/warpings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:05:25.778228 TorchRegister-0.2.2/src/TorchRegister.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      336 2023-05-04 09:05:25.000000 TorchRegister-0.2.2/src/TorchRegister.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      367 2023-05-04 09:05:25.000000 TorchRegister-0.2.2/src/TorchRegister.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 09:05:25.000000 TorchRegister-0.2.2/src/TorchRegister.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-05-04 09:05:25.000000 TorchRegister-0.2.2/src/TorchRegister.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-04 09:05:25.000000 TorchRegister-0.2.2/src/TorchRegister.egg-info/top_level.txt
```

### Comparing `TorchRegister-0.2.1/LICENSE.md` & `TorchRegister-0.2.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `TorchRegister-0.2.1/README.md` & `TorchRegister-0.2.2/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 <h1>TorchRegister</h1>
-<p>Common medical 3D image registration methods such as rigid, affine, and flow field for PyTorch.</p>
+<p>Common 2D and 3D image registration methods such as rigid, affine, and flow field for PyTorch.</p>
 
 <p align="center">
+    <img width="600" height="200" src="https://github.com/AgamChopra/TorchGradRegister/blob/main/assets/ringo_registration_2d.jpg">
+    <br><i>Fig. Example visualizations 2D image registration.</i><br><br>
     <img width="900" height="200" src="https://github.com/AgamChopra/TorchGradRegister/blob/main/assets/flow_test.jpg">
     <br><i>Fig. Example visualizations of deep learning based flow-field brain MRI registration.</i><br><br>
     <img width="900" height="240" src="https://github.com/AgamChopra/TorchGradRegister/blob/main/assets/affine_test.jpg">
     <br><i>Fig. Example visualizations of PyTorch based Affine brain MRI registration.</i><br><br>
     <img width="900" height="240" src="https://github.com/AgamChopra/TorchGradRegister/blob/main/assets/rigid_test.jpg">
     <br><i>Fig. Example visualizations of PyTorch based Rigid brain MRI registration.</i><br><br>
     <img width="200" height="150" src="https://github.com/AgamChopra/TorchGradRegister/blob/main/assets/flow_test_loss.png"> 
@@ -17,58 +19,78 @@
 <p>Example:</p>
  <pre><code>
  
         import torch
         from torchio.transforms import RandomAffine
         from numpy import load
         from matplotlib import pyplot as plt
-        from TorchRegister import Register
+        import TorchRegister as tr
 
 
-        # augmentation function
         def rand_augment(x):
             affine = RandomAffine(image_interpolation='bspline',
-                                  degrees=45, translation=8, scales=(0.7, 1.5))
+                                  degrees=25, translation=4, scales=(0.8, 1.2))
             y = affine(x[0])
             return y.view(x.shape)
 
 
         device = 'cuda'
 
         # loading data
-        path = 'example_mri.pkl'
+        path = 'R:/img (%d).pkl' % (1)
         data = load(path, allow_pickle=True)
-        
-        moving = torch.from_numpy(data)
+        moving = torch.from_numpy(data[0])
         moving = moving.view(1, 1, moving.shape[0], moving.shape[1], moving.shape[2]).to(
             dtype=torch.float, device=device)
-        
-        target = torch.from_numpy(data)
+        target = torch.from_numpy(data[0])
         target = rand_augment(target.view(1, 1, target.shape[0], target.shape[1], target.shape[2])).to(
             dtype=torch.float, device=device)
 
-        # Flow field based registration
-        warping = Register(mode='flow', device=device, debug=True)
-        warping.optim(moving, target, lr=1E-3)
-        warped = warping(moving)
-
-        print(target.shape)
-        print(moving.shape)
-        print(warped[0].shape)
-
         plt.imshow(torch.squeeze(moving[:, :, :, :, 60]
                                  ).detach().cpu().numpy(), cmap='gray')
         plt.title('Moving')
         plt.show()
 
+        plt.imshow(torch.squeeze(target[:, :, :, :, 60]
+                                 ).detach().cpu().numpy(), cmap='gray')
+        plt.title('Target')
+        plt.show()
+
+        # Rigid registration
+        warping = tr.Register(mode='rigid', device=device, debug=False)
+        warping.optim(moving, target, max_epochs=500, lr=1E-5)
+        warped = warping(moving)
+
         plt.imshow(torch.squeeze(warped[:, :, :, :, 60]
                                  ).detach().cpu().numpy(), cmap='gray')
-        plt.title('Warped Moving')
+        plt.title('Warped Moving 1')
         plt.show()
 
-        plt.imshow(torch.squeeze(target[:, :, :, :, 60]
+        # Affine registration
+        moving = warped.detach()
+        warping = tr.Register(mode='affine', device=device, debug=False)
+        warping.optim(moving, target, max_epochs=200, lr=1E-5)
+        warped = warping(moving)
+
+        plt.imshow(torch.squeeze(warped[:, :, :, :, 60]
                                  ).detach().cpu().numpy(), cmap='gray')
-        plt.title('Target')
+        plt.title('Warped Moving 2')
+        plt.show()
+
+        # Flow field based registration
+        moving = warped.detach()
+        warping = tr.Register(mode='flow', device=device, debug=False)
+        warping.optim(moving, target, lr=1E-3, max_epochs=100)
+        warped = warping(moving)
+
+        plt.imshow(torch.squeeze(warped[:, :, :, :, 60]
+                                 ).detach().cpu().numpy(), cmap='gray')
+        plt.title('Warped Moving 3')
+        plt.show()
+
+        plt.imshow(torch.moveaxis(torch.squeeze(tr.norm(
+            torch.abs(warping.theta[:, :, :, :, 60]))), 0, -1).detach().cpu().numpy())
+        plt.title('Flow Field')
         plt.show()
 </code></pre>
 
 <p><a href="https://raw.githubusercontent.com/AgamChopra/TorchGradRegister/main/LICENSE.md" target="blank">[The MIT License]</a></p>
```

### Comparing `TorchRegister-0.2.1/setup.py` & `TorchRegister-0.2.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='TorchRegister',
-    version='0.2.1',
+    version='0.2.2',
     url='https://github.com/AgamChopra/TorchRegister',
     author='Agam Chopra',
     author_email='achopra4@uw.edu',
     description='3D image registration methods for PyTorch.',
     long_description='Common medical 3D image registration methods such as rigid, affine, and flow field for PyTorch.',
     install_requires=['torch >= 2.0.0', 'numpy >= 1.24.1',
                       'tqdm >= 4.65.0', 'matplotlib  >= 3.7.1'],
```

### Comparing `TorchRegister-0.2.1/src/TorchRegister/torchregister.py` & `TorchRegister-0.2.2/src/TorchRegister/torchregister.py`

 * *Files identical despite different names*

### Comparing `TorchRegister-0.2.1/src/TorchRegister/utils.py` & `TorchRegister-0.2.2/src/TorchRegister/utils.py`

 * *Files 9% similar despite different names*

```diff
@@ -30,35 +30,42 @@
 
     return nn.functional.pad(input=input_, pad=pads, mode=mode, value=value).to(dtype=torch.float, device=device)
 
 
 class Theta(nn.Module):
     def __init__(self):
         super(Theta, self).__init__()
-        self.activation = nn.Tanh()
+        self.sin = torch.sin
+        self.cos = torch.cos
 
     def forward(self, x):
         output = x.clone()
         if output.shape[1] > 6:
-            output[:, 0] = self.activation(output[:, 0])
-            output[:, 1] = 2 * self.activation(output[:, 1])
-            output[:, 2] = 2 * self.activation(output[:, 2])
-
-            output[:, 4] = self.activation(output[:, 4])
-            output[:, 5] = 2 * self.activation(output[:, 5])
-            output[:, 6] = 2 * self.activation(output[:, 6])
-
-            output[:, 8] = self.activation(output[:, 8])
-            output[:, 9] = self.activation(output[:, 9])
-            output[:, 10] = self.activation(output[:, 10])
+            psi, theta, phi = x[:, 0], x[:, 1], x[:, 2]
+            output[:, 0] = self.cos(psi) * self.cos(theta)
+            output[:, 1] = self.sin(phi) * self.sin(psi) * \
+                self.cos(theta) - self.cos(phi) * self.sin(theta)
+            output[:, 2] = self.cos(phi) * self.sin(psi) * \
+                self.cos(theta) + self.sin(phi) * self.sin(theta)
+
+            output[:, 4] = self.cos(psi) * self.sin(theta)
+            output[:, 5] = self.sin(phi) * self.sin(psi) * \
+                self.sin(theta) + self.cos(phi) * self.cos(theta)
+            output[:, 6] = self.cos(phi) * self.sin(psi) * \
+                self.sin(theta) - self.sin(phi) * self.cos(theta)
+
+            output[:, 8] = - self.sin(psi)
+            output[:, 9] = self.sin(phi) * self.cos(psi)
+            output[:, 10] = self.cos(phi) * self.cos(psi)
         else:
-            output[:, 0] = self.activation(output[:, 0])
-            output[:, 1] = self.activation(output[:, 1])
-            output[:, 3] = self.activation(output[:, 3])
-            output[:, 4] = self.activation(output[:, 4])
+            theta = x[:, 0]
+            output[:, 0] = self.cos(theta)
+            output[:, 1] = - self.sin(theta)
+            output[:, 3] = self.sin(theta)
+            output[:, 4] = self.cos(theta)
         return output
 
 
 class Regressor(nn.Module):
     def __init__(self, moving, per, device):
         super(Regressor, self).__init__()
         if len(moving.shape) == 5:
```

### Comparing `TorchRegister-0.2.1/src/TorchRegister/warpings.py` & `TorchRegister-0.2.2/src/TorchRegister/warpings.py`

 * *Files identical despite different names*

