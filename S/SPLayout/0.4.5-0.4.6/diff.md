# Comparing `tmp/SPLayout-0.4.5.tar.gz` & `tmp/SPLayout-0.4.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\SPLayout-0.4.5.tar", last modified: Sat Apr 15 14:29:30 2023, max compression
+gzip compressed data, was "dist\SPLayout-0.4.6.tar", last modified: Thu May  4 12:35:07 2023, max compression
```

## Comparing `SPLayout-0.4.5.tar` & `SPLayout-0.4.6.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxrwxrwx   0        0        0        0 2023-04-15 14:29:30.000000 SPLayout-0.4.5/
--rw-rw-rw-   0        0        0     2146 2023-04-15 14:29:30.000000 SPLayout-0.4.5/PKG-INFO
--rw-rw-rw-   0        0        0     2433 2023-02-23 14:51:36.000000 SPLayout-0.4.5/README.md
--rw-rw-rw-   0        0        0     1473 2023-02-23 14:51:44.000000 SPLayout-0.4.5/README.rst
-drwxrwxrwx   0        0        0        0 2023-04-15 14:29:30.000000 SPLayout-0.4.5/SPLayout.egg-info/
--rw-rw-rw-   0        0        0     2146 2023-04-15 14:29:30.000000 SPLayout-0.4.5/SPLayout.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1491 2023-04-15 14:29:30.000000 SPLayout-0.4.5/SPLayout.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-15 14:29:30.000000 SPLayout-0.4.5/SPLayout.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       18 2023-04-15 14:29:30.000000 SPLayout-0.4.5/SPLayout.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-04-15 14:29:30.000000 SPLayout-0.4.5/SPLayout.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-15 14:29:30.000000 SPLayout-0.4.5/setup.cfg
--rw-rw-rw-   0        0        0      687 2023-02-23 14:06:17.000000 SPLayout-0.4.5/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-15 14:29:30.000000 SPLayout-0.4.5/splayout/
--rw-rw-rw-   0        0        0     1987 2023-04-15 14:27:55.000000 SPLayout-0.4.5/splayout/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-15 14:29:30.000000 SPLayout-0.4.5/splayout/adjointmethod/
--rw-rw-rw-   0        0        0      293 2023-02-24 04:21:26.000000 SPLayout-0.4.5/splayout/adjointmethod/__init__.py
--rw-rw-rw-   0        0        0    10984 2023-02-23 12:33:21.000000 SPLayout-0.4.5/splayout/adjointmethod/adjointshapeopt.py
--rw-rw-rw-   0        0        0    10647 2023-02-24 04:32:00.000000 SPLayout-0.4.5/splayout/adjointmethod/adjointtopologyopt.py
--rw-rw-rw-   0        0        0    10586 2023-02-23 12:35:47.000000 SPLayout-0.4.5/splayout/adjointmethod/shaperegion2d.py
--rw-rw-rw-   0        0        0    10652 2023-02-23 12:35:57.000000 SPLayout-0.4.5/splayout/adjointmethod/shaperegion3d.py
--rw-rw-rw-   0        0        0    11374 2023-02-23 12:36:38.000000 SPLayout-0.4.5/splayout/adjointmethod/topologyregion2d.py
--rw-rw-rw-   0        0        0    11149 2023-02-24 02:38:35.000000 SPLayout-0.4.5/splayout/adjointmethod/topologyregion3d.py
-drwxrwxrwx   0        0        0        0 2023-04-15 14:29:30.000000 SPLayout-0.4.5/splayout/algorithms/
--rw-rw-rw-   0        0        0      312 2023-02-23 13:06:11.000000 SPLayout-0.4.5/splayout/algorithms/__init__.py
--rw-rw-rw-   0        0        0     5781 2022-01-04 05:22:28.000000 SPLayout-0.4.5/splayout/algorithms/binarybatalgorithm.py
--rw-rw-rw-   0        0        0     6360 2022-01-04 06:04:34.000000 SPLayout-0.4.5/splayout/algorithms/binarygeneticalgorithm.py
--rw-rw-rw-   0        0        0     5831 2022-01-04 06:03:59.000000 SPLayout-0.4.5/splayout/algorithms/binaryparticleswarmalgorithm.py
--rw-rw-rw-   0        0        0     4305 2023-02-23 12:22:49.000000 SPLayout-0.4.5/splayout/algorithms/directbinarysearchalgorithm.py
--rw-rw-rw-   0        0        0     7333 2023-02-23 11:24:29.000000 SPLayout-0.4.5/splayout/algorithms/particleswarmalgorithm.py
-drwxrwxrwx   0        0        0        0 2023-04-15 14:29:30.000000 SPLayout-0.4.5/splayout/components/
--rw-rw-rw-   0        0        0     3728 2023-02-23 12:38:12.000000 SPLayout-0.4.5/splayout/components/AEMDgrating.py
--rw-rw-rw-   0        0        0      714 2023-02-23 13:44:58.000000 SPLayout-0.4.5/splayout/components/__init__.py
--rw-rw-rw-   0        0        0     4403 2023-02-23 12:38:42.000000 SPLayout-0.4.5/splayout/components/bend.py
--rw-rw-rw-   0        0        0     9026 2023-02-23 12:39:10.000000 SPLayout-0.4.5/splayout/components/doubleconnector.py
--rw-rw-rw-   0        0        0     6092 2023-02-23 12:42:22.000000 SPLayout-0.4.5/splayout/components/filledpattern.py
--rw-rw-rw-   0        0        0    49359 2023-02-23 12:42:22.000000 SPLayout-0.4.5/splayout/components/microring.py
--rw-rw-rw-   0        0        0    21403 2023-02-23 12:42:22.000000 SPLayout-0.4.5/splayout/components/pixelsregion.py
--rw-rw-rw-   0        0        0     7433 2023-02-23 12:41:22.000000 SPLayout-0.4.5/splayout/components/polygon.py
--rw-rw-rw-   0        0        0    14219 2023-02-23 12:42:22.000000 SPLayout-0.4.5/splayout/components/quarbend.py
--rw-rw-rw-   0        0        0    18098 2023-02-23 12:42:22.000000 SPLayout-0.4.5/splayout/components/sbend.py
--rw-rw-rw-   0        0        0    13136 2023-02-23 12:41:22.000000 SPLayout-0.4.5/splayout/components/selfdefinecomponent.py
--rw-rw-rw-   0        0        0    28052 2023-02-23 12:43:30.000000 SPLayout-0.4.5/splayout/components/simpleasymmetricdirectionalcoupler.py
--rw-rw-rw-   0        0        0     7270 2023-02-23 12:41:22.000000 SPLayout-0.4.5/splayout/components/slowlyvaryingtaper.py
--rw-rw-rw-   0        0        0     6668 2023-02-23 14:27:24.000000 SPLayout-0.4.5/splayout/components/taper.py
--rw-rw-rw-   0        0        0     1269 2023-02-23 12:41:22.000000 SPLayout-0.4.5/splayout/components/text.py
--rw-rw-rw-   0        0        0     8908 2023-02-23 12:42:22.000000 SPLayout-0.4.5/splayout/components/waveguide.py
-drwxrwxrwx   0        0        0        0 2023-04-15 14:29:30.000000 SPLayout-0.4.5/splayout/lumericalcommun/
--rw-rw-rw-   0        0        0       72 2023-02-23 12:26:37.000000 SPLayout-0.4.5/splayout/lumericalcommun/__init__.py
--rw-rw-rw-   0        0        0    77831 2023-04-15 14:25:50.000000 SPLayout-0.4.5/splayout/lumericalcommun/fdtdapi.py
--rw-rw-rw-   0        0        0    44213 2023-02-23 12:42:48.000000 SPLayout-0.4.5/splayout/lumericalcommun/modeapi.py
-drwxrwxrwx   0        0        0        0 2023-04-15 14:29:30.000000 SPLayout-0.4.5/splayout/utils/
--rw-rw-rw-   0        0        0       20 2023-02-23 12:27:14.000000 SPLayout-0.4.5/splayout/utils/__init__.py
--rw-rw-rw-   0        0        0     7931 2023-02-23 12:43:16.000000 SPLayout-0.4.5/splayout/utils/utils.py
+drwxrwxrwx   0        0        0        0 2023-05-04 12:35:07.000000 SPLayout-0.4.6/
+-rw-rw-rw-   0        0        0     2146 2023-05-04 12:35:07.000000 SPLayout-0.4.6/PKG-INFO
+-rw-rw-rw-   0        0        0     2433 2023-02-23 14:51:36.000000 SPLayout-0.4.6/README.md
+-rw-rw-rw-   0        0        0     1473 2023-02-23 14:51:44.000000 SPLayout-0.4.6/README.rst
+drwxrwxrwx   0        0        0        0 2023-05-04 12:35:07.000000 SPLayout-0.4.6/SPLayout.egg-info/
+-rw-rw-rw-   0        0        0     2146 2023-05-04 12:35:06.000000 SPLayout-0.4.6/SPLayout.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1491 2023-05-04 12:35:07.000000 SPLayout-0.4.6/SPLayout.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-04 12:35:06.000000 SPLayout-0.4.6/SPLayout.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       18 2023-05-04 12:35:06.000000 SPLayout-0.4.6/SPLayout.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-05-04 12:35:06.000000 SPLayout-0.4.6/SPLayout.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-04 12:35:07.000000 SPLayout-0.4.6/setup.cfg
+-rw-rw-rw-   0        0        0      687 2023-02-23 14:06:17.000000 SPLayout-0.4.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-04 12:35:07.000000 SPLayout-0.4.6/splayout/
+-rw-rw-rw-   0        0        0     1987 2023-05-04 12:32:29.000000 SPLayout-0.4.6/splayout/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-04 12:35:07.000000 SPLayout-0.4.6/splayout/adjointmethod/
+-rw-rw-rw-   0        0        0      293 2023-02-24 04:21:26.000000 SPLayout-0.4.6/splayout/adjointmethod/__init__.py
+-rw-rw-rw-   0        0        0    10984 2023-02-23 12:33:21.000000 SPLayout-0.4.6/splayout/adjointmethod/adjointshapeopt.py
+-rw-rw-rw-   0        0        0    10645 2023-05-04 11:28:32.000000 SPLayout-0.4.6/splayout/adjointmethod/adjointtopologyopt.py
+-rw-rw-rw-   0        0        0    10586 2023-02-23 12:35:47.000000 SPLayout-0.4.6/splayout/adjointmethod/shaperegion2d.py
+-rw-rw-rw-   0        0        0    10652 2023-02-23 12:35:57.000000 SPLayout-0.4.6/splayout/adjointmethod/shaperegion3d.py
+-rw-rw-rw-   0        0        0    11374 2023-02-23 12:36:38.000000 SPLayout-0.4.6/splayout/adjointmethod/topologyregion2d.py
+-rw-rw-rw-   0        0        0    11304 2023-05-04 05:46:43.000000 SPLayout-0.4.6/splayout/adjointmethod/topologyregion3d.py
+drwxrwxrwx   0        0        0        0 2023-05-04 12:35:07.000000 SPLayout-0.4.6/splayout/algorithms/
+-rw-rw-rw-   0        0        0      312 2023-05-04 05:08:40.000000 SPLayout-0.4.6/splayout/algorithms/__init__.py
+-rw-rw-rw-   0        0        0     5781 2022-01-04 05:22:28.000000 SPLayout-0.4.6/splayout/algorithms/binarybatalgorithm.py
+-rw-rw-rw-   0        0        0     6360 2022-01-04 06:04:34.000000 SPLayout-0.4.6/splayout/algorithms/binarygeneticalgorithm.py
+-rw-rw-rw-   0        0        0     5831 2023-05-04 05:07:54.000000 SPLayout-0.4.6/splayout/algorithms/binaryparticleswarmalgorithm.py
+-rw-rw-rw-   0        0        0     4305 2023-02-23 12:22:49.000000 SPLayout-0.4.6/splayout/algorithms/directbinarysearchalgorithm.py
+-rw-rw-rw-   0        0        0     7326 2023-05-04 05:08:40.000000 SPLayout-0.4.6/splayout/algorithms/particleswarmalgorithm.py
+drwxrwxrwx   0        0        0        0 2023-05-04 12:35:07.000000 SPLayout-0.4.6/splayout/components/
+-rw-rw-rw-   0        0        0     3728 2023-02-23 12:38:12.000000 SPLayout-0.4.6/splayout/components/AEMDgrating.py
+-rw-rw-rw-   0        0        0      714 2023-02-23 13:44:58.000000 SPLayout-0.4.6/splayout/components/__init__.py
+-rw-rw-rw-   0        0        0     4403 2023-02-23 12:38:42.000000 SPLayout-0.4.6/splayout/components/bend.py
+-rw-rw-rw-   0        0        0     9026 2023-02-23 12:39:10.000000 SPLayout-0.4.6/splayout/components/doubleconnector.py
+-rw-rw-rw-   0        0        0     6092 2023-02-23 12:42:22.000000 SPLayout-0.4.6/splayout/components/filledpattern.py
+-rw-rw-rw-   0        0        0    49359 2023-02-23 12:42:22.000000 SPLayout-0.4.6/splayout/components/microring.py
+-rw-rw-rw-   0        0        0    21403 2023-02-23 12:42:22.000000 SPLayout-0.4.6/splayout/components/pixelsregion.py
+-rw-rw-rw-   0        0        0     7433 2023-02-23 12:41:22.000000 SPLayout-0.4.6/splayout/components/polygon.py
+-rw-rw-rw-   0        0        0    14219 2023-02-23 12:42:22.000000 SPLayout-0.4.6/splayout/components/quarbend.py
+-rw-rw-rw-   0        0        0    18098 2023-02-23 12:42:22.000000 SPLayout-0.4.6/splayout/components/sbend.py
+-rw-rw-rw-   0        0        0    13136 2023-02-23 12:41:22.000000 SPLayout-0.4.6/splayout/components/selfdefinecomponent.py
+-rw-rw-rw-   0        0        0    28052 2023-02-23 12:43:30.000000 SPLayout-0.4.6/splayout/components/simpleasymmetricdirectionalcoupler.py
+-rw-rw-rw-   0        0        0     7270 2023-02-23 12:41:22.000000 SPLayout-0.4.6/splayout/components/slowlyvaryingtaper.py
+-rw-rw-rw-   0        0        0     6668 2023-02-23 14:27:24.000000 SPLayout-0.4.6/splayout/components/taper.py
+-rw-rw-rw-   0        0        0     1269 2023-02-23 12:41:22.000000 SPLayout-0.4.6/splayout/components/text.py
+-rw-rw-rw-   0        0        0     8908 2023-02-23 12:42:22.000000 SPLayout-0.4.6/splayout/components/waveguide.py
+drwxrwxrwx   0        0        0        0 2023-05-04 12:35:07.000000 SPLayout-0.4.6/splayout/lumericalcommun/
+-rw-rw-rw-   0        0        0       72 2023-02-23 12:26:37.000000 SPLayout-0.4.6/splayout/lumericalcommun/__init__.py
+-rw-rw-rw-   0        0        0    77831 2023-04-15 14:25:50.000000 SPLayout-0.4.6/splayout/lumericalcommun/fdtdapi.py
+-rw-rw-rw-   0        0        0    44213 2023-02-23 12:42:48.000000 SPLayout-0.4.6/splayout/lumericalcommun/modeapi.py
+drwxrwxrwx   0        0        0        0 2023-05-04 12:35:07.000000 SPLayout-0.4.6/splayout/utils/
+-rw-rw-rw-   0        0        0       20 2023-02-23 12:27:14.000000 SPLayout-0.4.6/splayout/utils/__init__.py
+-rw-rw-rw-   0        0        0    14788 2023-05-04 04:58:18.000000 SPLayout-0.4.6/splayout/utils/utils.py
```

### Comparing `SPLayout-0.4.5/PKG-INFO` & `SPLayout-0.4.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.0
 Name: SPLayout
-Version: 0.4.5
+Version: 0.4.6
 Summary: Silicon Photonics Design Tools for GDSII Files.
 Home-page: https://github.com/Hideousmon/SPLayout
 Author: Zhenyu ZHAO
 Author-email: mailtozyzhao@163.com
 License: UNKNOWN
 Description: SPLayout
         ========
```

### Comparing `SPLayout-0.4.5/README.md` & `SPLayout-0.4.6/README.md`

 * *Files identical despite different names*

### Comparing `SPLayout-0.4.5/README.rst` & `SPLayout-0.4.6/README.rst`

 * *Files identical despite different names*

### Comparing `SPLayout-0.4.5/SPLayout.egg-info/PKG-INFO` & `SPLayout-0.4.6/SPLayout.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.0
 Name: SPLayout
-Version: 0.4.5
+Version: 0.4.6
 Summary: Silicon Photonics Design Tools for GDSII Files.
 Home-page: https://github.com/Hideousmon/SPLayout
 Author: Zhenyu ZHAO
 Author-email: mailtozyzhao@163.com
 License: UNKNOWN
 Description: SPLayout
         ========
```

### Comparing `SPLayout-0.4.5/SPLayout.egg-info/SOURCES.txt` & `SPLayout-0.4.6/SPLayout.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `SPLayout-0.4.5/setup.py` & `SPLayout-0.4.6/setup.py`

 * *Files identical despite different names*

### Comparing `SPLayout-0.4.5/splayout/__init__.py` & `SPLayout-0.4.6/splayout/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "0.4.5"
+__version__ = "0.4.6"
 
 ## Submodules
 from . import utils
 from . import components
 from . import algorithms
 from . import lumericalcommun
 from . import adjointmethod
@@ -35,13 +35,13 @@
 from .adjointmethod.topologyregion3d import TopologyOptRegion3D
 from .adjointmethod.adjointshapeopt import AdjointForShapeOpt
 from .adjointmethod.adjointtopologyopt import AdjointForTO
 
 ## Algorithms
 from .algorithms.binarybatalgorithm import BinaryBatAlgorithm
 from .algorithms.directbinarysearchalgorithm import  DirectBinarySearchAlgorithm
-from .algorithms.particleswarmalgorithm import ParitcleSwarmAlgorithm
-from .algorithms.binaryparticleswarmalgorithm import BinaryParitcleSwarmAlgorithm
+from .algorithms.particleswarmalgorithm import ParticleSwarmAlgorithm
+from .algorithms.binaryparticleswarmalgorithm import BinaryParticleSwarmAlgorithm
 from .algorithms.binarygeneticalgorithm import BinaryGeneticAlgorithm
 
 ## Utils
 from .utils import *
```

### Comparing `SPLayout-0.4.5/splayout/adjointmethod/adjointshapeopt.py` & `SPLayout-0.4.6/splayout/adjointmethod/adjointshapeopt.py`

 * *Files identical despite different names*

### Comparing `SPLayout-0.4.5/splayout/adjointmethod/adjointtopologyopt.py` & `SPLayout-0.4.6/splayout/adjointmethod/adjointtopologyopt.py`

 * *Files 1% similar despite different names*

```diff
@@ -108,15 +108,15 @@
                 self.fom = const_term - error_term
             else:
                 self.fom = np.abs(self.target_T) - np.abs(self.T_fwd_vs_wavelengths.flatten() - self.target_T)
         else:
             wavelength = self.fdtd_engine.get_wavelength()
             wavelength_range = wavelength.max() - wavelength.min()
             if (wavelength.size > 1):
-                self.fom = np.trapz(y=np.squeeze(self.T_fwd_vs_wavelengths), x=wavelength, axis=1) / wavelength_range
+                self.fom = np.trapz(y=np.squeeze(self.T_fwd_vs_wavelengths), x=wavelength, axis=0) / wavelength_range
             else:
                 self.fom = self.T_fwd_vs_wavelengths.flatten()
         return self.fom
 
     def call_grad(self, params):
         """
         Calculate Gradient(Figure of Merit) and return.
@@ -177,25 +177,26 @@
                     T_fwd_error = self.T_fwd_vs_wavelengths[i] - self.target_T[i]
                     T_fwd_error_integrand = np.abs(T_fwd_error) / wavelength_range
                     const_factor = -1.0 * np.trapz(y = T_fwd_error_integrand, x = wavelength)
                     integral_kernel = np.sign(T_fwd_error) / wavelength_range
                     quad_weight = np.append(np.append(d[0], d[0:-1] + d[1:]),
                                             d[-1]) / 2
                     v = const_factor * integral_kernel.flatten() * quad_weight
-                    T_fwd_partial_derivs.append(np.real(partial_fom).transpose().dot(v).flatten().real)
+
+                    T_fwd_partial_derivs.append(np.real(partial_fom).dot(v).flatten().real)
                 else:
-                    T_fwd_partial_derivs.append((-1.0*np.sign(self.T_fwd_vs_wavelengths[i] - self.target_T[i]) * np.real(partial_fom)).real)
+                    T_fwd_partial_derivs.append((-1.0*np.sign(self.T_fwd_vs_wavelengths[i] - self.target_T[i]) * np.real(partial_fom))[:, 0].real)
 
             else:
                 T_fwd_partial_derivs.append(np.real(partial_fom))
 
 
 
         if (self.if_default_fom == 1):
-            T_fwd_partial_derivs = np.sum(np.array(T_fwd_partial_derivs), axis=0)
+            T_fwd_partial_derivs = - np.sum(np.array(T_fwd_partial_derivs), axis=0)
         else:
             T_fwd_partial_derivs = np.array(T_fwd_partial_derivs)
 
         return T_fwd_partial_derivs
 
     def reset_fom_monitor_name(self, fom_monitor_name):
         """
```

### Comparing `SPLayout-0.4.5/splayout/adjointmethod/shaperegion2d.py` & `SPLayout-0.4.6/splayout/adjointmethod/shaperegion2d.py`

 * *Files identical despite different names*

### Comparing `SPLayout-0.4.5/splayout/adjointmethod/shaperegion3d.py` & `SPLayout-0.4.6/splayout/adjointmethod/shaperegion3d.py`

 * *Files identical despite different names*

### Comparing `SPLayout-0.4.5/splayout/adjointmethod/topologyregion2d.py` & `SPLayout-0.4.6/splayout/adjointmethod/topologyregion2d.py`

 * *Files identical despite different names*

### Comparing `SPLayout-0.4.5/splayout/adjointmethod/topologyregion3d.py` & `SPLayout-0.4.6/splayout/adjointmethod/topologyregion3d.py`

 * *Files 2% similar despite different names*

```diff
@@ -125,14 +125,19 @@
 
         self.fdtd_engine.fdtd.eval('select("{}");'.format(self.rename) +
                   'delete;' +
                   'addimport;' +
                   'set("name","{}");'.format(self.rename) +
                   'importnk2(sqrt(eps_geo),x_geo,y_geo,z_geo);')
 
+    def reset_index(self, lower_index, higher_index):
+
+        self.lower_epsilon = lower_index ** 2
+        self.higher_epsilon = higher_index ** 2
+
     def get_E_distribution(self, if_get_spatial = 0):
         """
         Get electric field distribution from the region.
 
         Parameters
         ----------
         if_get_spatial : Bool
```

### Comparing `SPLayout-0.4.5/splayout/algorithms/binarybatalgorithm.py` & `SPLayout-0.4.6/splayout/algorithms/binarybatalgorithm.py`

 * *Files identical despite different names*

### Comparing `SPLayout-0.4.5/splayout/algorithms/binarygeneticalgorithm.py` & `SPLayout-0.4.6/splayout/algorithms/binarygeneticalgorithm.py`

 * *Files identical despite different names*

### Comparing `SPLayout-0.4.5/splayout/algorithms/binaryparticleswarmalgorithm.py` & `SPLayout-0.4.6/splayout/algorithms/binaryparticleswarmalgorithm.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 ## Malihe.(2008).Binary Particle Swarm Optimization: challenges and New Solutions.
 ## The Journal of Computer Society of Iran (CSI) On Computer Scienceand Engineering (JCSE),.
 ## 6. 21-32.
 ################################################################################################
 import numpy as np
 import math
 
-class BinaryParitcleSwarmAlgorithm:
+class BinaryParticleSwarmAlgorithm:
     """
     Binary Particle Swarm Optimization Algorithm.
     Parameters
     ----------
     noS : Int
         Initial Number of solutions.
     loS : Int
```

### Comparing `SPLayout-0.4.5/splayout/algorithms/directbinarysearchalgorithm.py` & `SPLayout-0.4.6/splayout/algorithms/directbinarysearchalgorithm.py`

 * *Files identical despite different names*

### Comparing `SPLayout-0.4.5/splayout/algorithms/particleswarmalgorithm.py` & `SPLayout-0.4.6/splayout/algorithms/particleswarmalgorithm.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,17 +3,17 @@
 ## Malihe.(2008).Binary Particle Swarm Optimization: challenges and New Solutions.
 ## The Journal of Computer Society of Iran (CSI) On Computer Scienceand Engineering (JCSE),.
 ## 6. 21-32.
 ################################################################################################
 import numpy as np
 import math
 
-class ParitcleSwarmAlgorithm:
+class ParticleSwarmAlgorithm:
     """
-    Binary Particle Swarm Optimization Algorithm.
+    Particle Swarm Optimization Algorithm.
     Parameters
     ----------
     noS : Int
         Initial Number of solutions.
     loS : Int
         Length of a single solution.
     cost_function : func
```

### Comparing `SPLayout-0.4.5/splayout/components/AEMDgrating.py` & `SPLayout-0.4.6/splayout/components/AEMDgrating.py`

 * *Files identical despite different names*

### Comparing `SPLayout-0.4.5/splayout/components/__init__.py` & `SPLayout-0.4.6/splayout/components/__init__.py`

 * *Files identical despite different names*

### Comparing `SPLayout-0.4.5/splayout/components/bend.py` & `SPLayout-0.4.6/splayout/components/bend.py`

 * *Files identical despite different names*

### Comparing `SPLayout-0.4.5/splayout/components/doubleconnector.py` & `SPLayout-0.4.6/splayout/components/doubleconnector.py`

 * *Files identical despite different names*

### Comparing `SPLayout-0.4.5/splayout/components/filledpattern.py` & `SPLayout-0.4.6/splayout/components/filledpattern.py`

 * *Files identical despite different names*

### Comparing `SPLayout-0.4.5/splayout/components/microring.py` & `SPLayout-0.4.6/splayout/components/microring.py`

 * *Files identical despite different names*

### Comparing `SPLayout-0.4.5/splayout/components/pixelsregion.py` & `SPLayout-0.4.6/splayout/components/pixelsregion.py`

 * *Files identical despite different names*

### Comparing `SPLayout-0.4.5/splayout/components/polygon.py` & `SPLayout-0.4.6/splayout/components/polygon.py`

 * *Files identical despite different names*

### Comparing `SPLayout-0.4.5/splayout/components/quarbend.py` & `SPLayout-0.4.6/splayout/components/quarbend.py`

 * *Files identical despite different names*

### Comparing `SPLayout-0.4.5/splayout/components/sbend.py` & `SPLayout-0.4.6/splayout/components/sbend.py`

 * *Files identical despite different names*

### Comparing `SPLayout-0.4.5/splayout/components/selfdefinecomponent.py` & `SPLayout-0.4.6/splayout/components/selfdefinecomponent.py`

 * *Files identical despite different names*

### Comparing `SPLayout-0.4.5/splayout/components/simpleasymmetricdirectionalcoupler.py` & `SPLayout-0.4.6/splayout/components/simpleasymmetricdirectionalcoupler.py`

 * *Files identical despite different names*

### Comparing `SPLayout-0.4.5/splayout/components/slowlyvaryingtaper.py` & `SPLayout-0.4.6/splayout/components/slowlyvaryingtaper.py`

 * *Files identical despite different names*

### Comparing `SPLayout-0.4.5/splayout/components/taper.py` & `SPLayout-0.4.6/splayout/components/taper.py`

 * *Files identical despite different names*

### Comparing `SPLayout-0.4.5/splayout/components/text.py` & `SPLayout-0.4.6/splayout/components/text.py`

 * *Files identical despite different names*

### Comparing `SPLayout-0.4.5/splayout/components/waveguide.py` & `SPLayout-0.4.6/splayout/components/waveguide.py`

 * *Files identical despite different names*

### Comparing `SPLayout-0.4.5/splayout/lumericalcommun/fdtdapi.py` & `SPLayout-0.4.6/splayout/lumericalcommun/fdtdapi.py`

 * *Files identical despite different names*

### Comparing `SPLayout-0.4.5/splayout/lumericalcommun/modeapi.py` & `SPLayout-0.4.6/splayout/lumericalcommun/modeapi.py`

 * *Files identical despite different names*

