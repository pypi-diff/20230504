# Comparing `tmp/MDbrew-2.2.4.tar.gz` & `tmp/MDbrew-2.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "MDbrew-2.2.4.tar", last modified: Wed May  3 12:42:58 2023, max compression
+gzip compressed data, was "dist/MDbrew-2.2.5.tar", last modified: Thu May  4 05:34:49 2023, max compression
```

## Comparing `MDbrew-2.2.4.tar` & `MDbrew-2.2.5.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxrwx---   0 minu928   (1216) minu928   (1216)        0 2023-05-03 12:39:41.112716 MDbrew-2.2.4/
--rw-rw----   0 minu928   (1216) minu928   (1216)       24 2023-05-02 21:58:36.000000 MDbrew-2.2.4/MANIFEST.in
-drwxrwx---   0 minu928   (1216) minu928   (1216)        0 2023-05-03 12:39:41.066048 MDbrew-2.2.4/MDbrew/
--rw-rw----   0 minu928   (1216) minu928   (1216)      229 2023-05-03 12:38:21.000000 MDbrew-2.2.4/MDbrew/__init__.py
-drwxrwx---   0 minu928   (1216) minu928   (1216)        0 2023-05-03 12:39:41.082715 MDbrew-2.2.4/MDbrew/analysis/
--rw-rw----   0 minu928   (1216) minu928   (1216)        0 2023-05-03 12:38:21.000000 MDbrew-2.2.4/MDbrew/analysis/__init__.py
--rw-rw----   0 minu928   (1216) minu928   (1216)     4546 2023-05-03 12:38:21.000000 MDbrew-2.2.4/MDbrew/analysis/msd.py
--rw-rw----   0 minu928   (1216) minu928   (1216)     5630 2023-05-03 12:38:21.000000 MDbrew-2.2.4/MDbrew/analysis/rdf.py
-drwxrwx---   0 minu928   (1216) minu928   (1216)        0 2023-05-03 12:39:41.086049 MDbrew-2.2.4/MDbrew/application/
--rw-rw----   0 minu928   (1216) minu928   (1216)        0 2023-05-03 12:38:21.000000 MDbrew-2.2.4/MDbrew/application/__init__.py
--rw-rw----   0 minu928   (1216) minu928   (1216)     9214 2023-05-03 12:38:21.000000 MDbrew-2.2.4/MDbrew/application/brewcp2k.py
-drwxrwx---   0 minu928   (1216) minu928   (1216)        0 2023-05-03 12:39:41.092716 MDbrew-2.2.4/MDbrew/main/
--rw-rw----   0 minu928   (1216) minu928   (1216)        0 2023-05-03 12:38:21.000000 MDbrew-2.2.4/MDbrew/main/__init__.py
--rw-rw----   0 minu928   (1216) minu928   (1216)     2605 2023-05-03 12:38:22.000000 MDbrew-2.2.4/MDbrew/main/brewer.py
--rw-rw----   0 minu928   (1216) minu928   (1216)     4183 2023-05-03 12:38:22.000000 MDbrew-2.2.4/MDbrew/main/brewery.py
-drwxrwx---   0 minu928   (1216) minu928   (1216)        0 2023-05-03 12:39:41.102716 MDbrew-2.2.4/MDbrew/main/filetype/
--rw-rw----   0 minu928   (1216) minu928   (1216)        0 2023-05-03 12:38:22.000000 MDbrew-2.2.4/MDbrew/main/filetype/__init__.py
--rw-rw----   0 minu928   (1216) minu928   (1216)      838 2023-05-03 12:38:23.000000 MDbrew-2.2.4/MDbrew/main/filetype/lmps.py
--rw-rw----   0 minu928   (1216) minu928   (1216)      712 2023-05-03 12:38:23.000000 MDbrew-2.2.4/MDbrew/main/filetype/pdb.py
--rw-rw----   0 minu928   (1216) minu928   (1216)     1291 2023-05-03 12:38:23.000000 MDbrew-2.2.4/MDbrew/main/filetype/vasp.py
--rw-rw----   0 minu928   (1216) minu928   (1216)      431 2023-05-03 12:38:23.000000 MDbrew-2.2.4/MDbrew/main/filetype/xyz.py
--rw-rw----   0 minu928   (1216) minu928   (1216)     1960 2023-05-03 12:38:23.000000 MDbrew-2.2.4/MDbrew/main/opener.py
-drwxrwx---   0 minu928   (1216) minu928   (1216)        0 2023-05-03 12:39:41.112716 MDbrew-2.2.4/MDbrew/tool/
--rw-rw----   0 minu928   (1216) minu928   (1216)        0 2023-05-03 12:38:23.000000 MDbrew-2.2.4/MDbrew/tool/__init__.py
--rw-rw----   0 minu928   (1216) minu928   (1216)     3545 2023-05-03 12:38:23.000000 MDbrew-2.2.4/MDbrew/tool/colorfont.py
--rw-rw----   0 minu928   (1216) minu928   (1216)      947 2023-05-03 12:38:23.000000 MDbrew-2.2.4/MDbrew/tool/decorator.py
--rw-rw----   0 minu928   (1216) minu928   (1216)      761 2023-05-03 12:38:23.000000 MDbrew-2.2.4/MDbrew/tool/doctor.py
--rw-rw----   0 minu928   (1216) minu928   (1216)     1563 2023-05-03 12:38:24.000000 MDbrew-2.2.4/MDbrew/tool/spacer.py
-drwxrwx---   0 minu928   (1216) minu928   (1216)        0 2023-05-03 12:39:41.079382 MDbrew-2.2.4/MDbrew.egg-info/
--rw-rw----   0 minu928   (1216) minu928   (1216)      332 2023-05-03 12:39:38.000000 MDbrew-2.2.4/MDbrew.egg-info/PKG-INFO
--rw-rw----   0 minu928   (1216) minu928   (1216)      706 2023-05-03 12:39:39.000000 MDbrew-2.2.4/MDbrew.egg-info/SOURCES.txt
--rw-rw----   0 minu928   (1216) minu928   (1216)        1 2023-05-03 12:39:38.000000 MDbrew-2.2.4/MDbrew.egg-info/dependency_links.txt
--rw-rw----   0 minu928   (1216) minu928   (1216)        1 2023-05-03 12:39:38.000000 MDbrew-2.2.4/MDbrew.egg-info/not-zip-safe
--rw-rw----   0 minu928   (1216) minu928   (1216)        7 2023-05-03 12:39:38.000000 MDbrew-2.2.4/MDbrew.egg-info/top_level.txt
--rw-rw----   0 minu928   (1216) minu928   (1216)      332 2023-05-03 12:39:41.112716 MDbrew-2.2.4/PKG-INFO
--rw-rw----   0 minu928   (1216) minu928   (1216)       58 2023-05-02 21:58:36.000000 MDbrew-2.2.4/requirement.txt
--rw-rw----   0 minu928   (1216) minu928   (1216)       79 2023-05-03 12:39:41.116049 MDbrew-2.2.4/setup.cfg
--rw-rw----   0 minu928   (1216) minu928   (1216)      631 2023-05-03 12:38:57.000000 MDbrew-2.2.4/setup.py
+drwxrwx---   0 minu928   (1216) minu928   (1216)        0 2023-05-04 05:31:31.000000 MDbrew-2.2.5/
+-rw-rw----   0 minu928   (1216) minu928   (1216)       24 2023-05-03 12:53:55.000000 MDbrew-2.2.5/MANIFEST.in
+drwxrwx---   0 minu928   (1216) minu928   (1216)        0 2023-05-04 05:31:31.000000 MDbrew-2.2.5/MDbrew.egg-info/
+-rw-rw----   0 minu928   (1216) minu928   (1216)      388 2023-05-04 05:31:31.000000 MDbrew-2.2.5/MDbrew.egg-info/PKG-INFO
+-rw-rw----   0 minu928   (1216) minu928   (1216)        1 2023-05-04 05:31:31.000000 MDbrew-2.2.5/MDbrew.egg-info/not-zip-safe
+-rw-rw----   0 minu928   (1216) minu928   (1216)      706 2023-05-04 05:31:31.000000 MDbrew-2.2.5/MDbrew.egg-info/SOURCES.txt
+-rw-rw----   0 minu928   (1216) minu928   (1216)        1 2023-05-04 05:31:31.000000 MDbrew-2.2.5/MDbrew.egg-info/dependency_links.txt
+-rw-rw----   0 minu928   (1216) minu928   (1216)        7 2023-05-04 05:31:31.000000 MDbrew-2.2.5/MDbrew.egg-info/top_level.txt
+drwxrwx---   0 minu928   (1216) minu928   (1216)        0 2023-05-04 05:31:31.000000 MDbrew-2.2.5/MDbrew/
+drwxrwx---   0 minu928   (1216) minu928   (1216)        0 2023-05-04 05:31:31.000000 MDbrew-2.2.5/MDbrew/tool/
+-rw-rw----   0 minu928   (1216) minu928   (1216)        0 2023-05-04 05:30:46.000000 MDbrew-2.2.5/MDbrew/tool/__init__.py
+-rw-rw----   0 minu928   (1216) minu928   (1216)     3545 2023-05-04 05:30:46.000000 MDbrew-2.2.5/MDbrew/tool/colorfont.py
+-rw-rw----   0 minu928   (1216) minu928   (1216)      761 2023-05-04 05:30:46.000000 MDbrew-2.2.5/MDbrew/tool/doctor.py
+-rw-rw----   0 minu928   (1216) minu928   (1216)      947 2023-05-04 05:30:46.000000 MDbrew-2.2.5/MDbrew/tool/decorator.py
+-rw-rw----   0 minu928   (1216) minu928   (1216)      599 2023-05-04 05:30:46.000000 MDbrew-2.2.5/MDbrew/tool/spacer.py
+drwxrwx---   0 minu928   (1216) minu928   (1216)        0 2023-05-04 05:31:31.000000 MDbrew-2.2.5/MDbrew/application/
+-rw-rw----   0 minu928   (1216) minu928   (1216)        0 2023-05-04 05:30:46.000000 MDbrew-2.2.5/MDbrew/application/__init__.py
+-rw-rw----   0 minu928   (1216) minu928   (1216)     9449 2023-05-04 05:30:46.000000 MDbrew-2.2.5/MDbrew/application/brewcp2k.py
+drwxrwx---   0 minu928   (1216) minu928   (1216)        0 2023-05-04 05:31:31.000000 MDbrew-2.2.5/MDbrew/analysis/
+-rw-rw----   0 minu928   (1216) minu928   (1216)     4342 2023-05-04 05:30:46.000000 MDbrew-2.2.5/MDbrew/analysis/msd.py
+-rw-rw----   0 minu928   (1216) minu928   (1216)     5475 2023-05-04 05:30:46.000000 MDbrew-2.2.5/MDbrew/analysis/rdf.py
+-rw-rw----   0 minu928   (1216) minu928   (1216)        0 2023-05-04 05:30:46.000000 MDbrew-2.2.5/MDbrew/analysis/__init__.py
+drwxrwx---   0 minu928   (1216) minu928   (1216)        0 2023-05-04 05:31:31.000000 MDbrew-2.2.5/MDbrew/main/
+-rw-rw----   0 minu928   (1216) minu928   (1216)        0 2023-05-04 05:30:46.000000 MDbrew-2.2.5/MDbrew/main/__init__.py
+-rw-rw----   0 minu928   (1216) minu928   (1216)     2605 2023-05-04 05:30:46.000000 MDbrew-2.2.5/MDbrew/main/brewer.py
+drwxrwx---   0 minu928   (1216) minu928   (1216)        0 2023-05-04 05:31:31.000000 MDbrew-2.2.5/MDbrew/main/filetype/
+-rw-rw----   0 minu928   (1216) minu928   (1216)      712 2023-05-04 05:30:46.000000 MDbrew-2.2.5/MDbrew/main/filetype/pdb.py
+-rw-rw----   0 minu928   (1216) minu928   (1216)     1291 2023-05-04 05:30:46.000000 MDbrew-2.2.5/MDbrew/main/filetype/vasp.py
+-rw-rw----   0 minu928   (1216) minu928   (1216)        0 2023-05-04 05:30:46.000000 MDbrew-2.2.5/MDbrew/main/filetype/__init__.py
+-rw-rw----   0 minu928   (1216) minu928   (1216)      838 2023-05-04 05:30:46.000000 MDbrew-2.2.5/MDbrew/main/filetype/lmps.py
+-rw-rw----   0 minu928   (1216) minu928   (1216)      431 2023-05-04 05:30:46.000000 MDbrew-2.2.5/MDbrew/main/filetype/xyz.py
+-rw-rw----   0 minu928   (1216) minu928   (1216)     4183 2023-05-04 05:30:46.000000 MDbrew-2.2.5/MDbrew/main/brewery.py
+-rw-rw----   0 minu928   (1216) minu928   (1216)     1960 2023-05-04 05:30:46.000000 MDbrew-2.2.5/MDbrew/main/opener.py
+-rw-rw----   0 minu928   (1216) minu928   (1216)      229 2023-05-04 05:30:46.000000 MDbrew-2.2.5/MDbrew/__init__.py
+-rw-rw----   0 minu928   (1216) minu928   (1216)      388 2023-05-04 05:31:31.000000 MDbrew-2.2.5/PKG-INFO
+-rw-rw----   0 minu928   (1216) minu928   (1216)      631 2023-05-04 05:31:13.000000 MDbrew-2.2.5/setup.py
+-rw-rw----   0 minu928   (1216) minu928   (1216)       79 2023-05-04 05:31:31.000000 MDbrew-2.2.5/setup.cfg
+-rw-rw----   0 minu928   (1216) minu928   (1216)       58 2023-05-03 12:53:56.000000 MDbrew-2.2.5/requirement.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `MDbrew-2.2.4/MDbrew/analysis/msd.py` & `MDbrew-2.2.5/MDbrew/analysis/msd.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 import numpy as np
 from tqdm import trange, tqdm
-from numpy.typing import NDArray
 from ..tool import spacer
 from ..main.brewery import Brewery
 from ..tool.colorfont import color
 
 
 # Class of Mean Square Displacement
 class MSD(object):
@@ -23,15 +22,15 @@
     def __init__(self, position, fft: bool = True, dtype: str = "float32"):
         """MSD
 
         Calculate the msd data and return it with method and fft
 
         Parameters
         ------------
-        position : NDArray
+        position
             Data of Particle's position in each frame
         fft : bool, optional
             default = True, if True the calculation in FFT, else  matrix
 
         ## Result of 'Mean Square Displacement'
         >>> my_msd      = MSD(position = position, fft = True)
         >>> msd_result  = my_msd.result
@@ -42,15 +41,15 @@
             pos_range = tqdm(self.position, **self.kwrgs_pos)
             self.position = np.array([data for data in pos_range], dtype=dtype)
         else:
             self.position = spacer.check_dimension(position, dim=3)
         self.frame_number = self.position.shape[0]
         self.fft = fft
 
-    def run(self) -> NDArray[np.float64]:
+    def run(self):
         """run
 
         Return
         ----------
         NDArray[np.float64]: result of MSD
         """
         if self.fft:
@@ -60,15 +59,15 @@
         return self
 
     @property
     def result(self):
         return self._result
 
     # window method with non-FFT
-    def __get_msd_window(self) -> NDArray[np.float64]:
+    def __get_msd_window(self):
         """MSD - Window Method with non-FFT
 
         Calculate the MSD list with linear loop with numpy function
 
         Time complexity : O(N**2)
 
         Returns
@@ -80,15 +79,15 @@
         for frame in trange(1, self.frame_number, **self.kwrgs_trange):
             diff_position = spacer.get_diff_position(self.position[frame:], self.position[:-frame])
             distance = self.__square_sum_position(diff_position)
             msd_list[frame, :] = np.mean(distance, axis=self.axis_dict["frame"])
         return self.__mean_msd_list(msd_list=msd_list)
 
     # window method with FFT
-    def __get_msd_fft(self) -> NDArray[np.float64]:
+    def __get_msd_fft(self):
         """MSD - Window method wit FFT
 
         Calculate the MSD list with linear loop with numpy function
 
         Time complexity : O(N logN)
 
         Returns
@@ -97,35 +96,35 @@
             MSD data of each frame
         """
         S_1 = self.__get_S_1()
         S_2 = self.__get_S_2()
         msd_list = np.subtract(S_1, 2.0 * S_2)
         return self.__mean_msd_list(msd_list=msd_list)
 
-    def __get_S_1(self) -> NDArray[np.float64]:
+    def __get_S_1(self):
         empty_matrix = np.zeros(self.position.shape[:2])
         D = self.__square_sum_position(self.position)
         D = np.append(D, empty_matrix, axis=self.axis_dict["frame"])
         Q = 2.0 * np.sum(D, axis=self.axis_dict["frame"])
         S_1 = empty_matrix
         for m in trange(self.frame_number, **self.kwrgs_trange):
             Q -= D[m - 1, :] + D[self.frame_number - m, :]
             S_1[m, :] = Q / (self.frame_number - m)
         return S_1
 
     # get S2 for FFT
-    def __get_S_2(self) -> NDArray[np.float64]:
+    def __get_S_2(self):
         X = np.fft.fft(self.position, n=2 * self.frame_number, axis=self.axis_dict["frame"])
         dot_X = X * X.conjugate()
         x = np.fft.ifft(dot_X, axis=self.axis_dict["frame"])
         x = x[: self.frame_number].real
         x = x.sum(axis=self.axis_dict["pos"])
         n = np.arange(self.frame_number, 0, -1)
         return x / n[:, np.newaxis]
 
     # do square and sum about position
-    def __square_sum_position(self, position_data) -> NDArray[np.float64]:
+    def __square_sum_position(self, position_data):
         return np.square(position_data).sum(axis=self.axis_dict["pos"])
 
     # do mean about msd list
-    def __mean_msd_list(self, msd_list) -> NDArray[np.float64]:
+    def __mean_msd_list(self, msd_list):
         return msd_list.mean(axis=self.axis_dict["N_particle"])
```

### Comparing `MDbrew-2.2.4/MDbrew/analysis/rdf.py` & `MDbrew-2.2.5/MDbrew/analysis/rdf.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 import numpy as np
 from tqdm import trange, tqdm
-from numpy.typing import NDArray
 from ..main.brewery import Brewery
 from ..tool.spacer import *
 from ..tool.colorfont import color
 
 
 # Calculate and Plot the RDF
 class RDF(object):
@@ -96,43 +95,43 @@
         self.frame_num = frame_num
 
     # select the mode with Boundary Layer
     def __set_boundary_condition(self):
         return self.__add_layer if self.layer_depth else self.__check_pbc
 
     # set the pbc only consider single system
-    def __check_pbc(self, diff_position) -> NDArray[np.float64]:
+    def __check_pbc(self, diff_position):
         diff_position = np.abs(diff_position)
         return np.where(
             diff_position > self.half_box_size,
             self.box_size - diff_position,
             diff_position,
         )
 
     # set the pbc with 27 system
-    def __add_layer(self, diff_position) -> NDArray[np.float64]:
+    def __add_layer(self, diff_position):
         return diff_position[..., np.newaxis, :] + self.layer
 
     # Make a 3D layer_idx
-    def __make_layer(self) -> NDArray[np.float64]:
+    def __make_layer(self):
         list_direction = []
         idx_direction_ = range(-self.layer_depth, self.layer_depth + 1)
         for i in idx_direction_:
             for j in idx_direction_:
                 for k in idx_direction_:
                     list_direction.append([i, j, k])
         return np.array(list_direction) * self.box_size
 
     # get idx for histogram
-    def __cal_idx_histogram(self, distance: NDArray) -> NDArray[np.int64]:
+    def __cal_idx_histogram(self, distance):
         idx_hist = (distance / self.dr).astype(np.int64)
         return idx_hist[np.where((0 < idx_hist) & (idx_hist < self.resolution))]
 
     # Calculate the Density Function
-    def __cal_rdf_from_hist_data(self) -> NDArray[np.float64]:
+    def __cal_rdf_from_hist_data(self):
         r_i = self.radii[1:]
         g_r = np.append(0.0, self.hist_data[1:] / np.square(r_i))
         factor = np.array(
             4.0 * np.pi * self.dr * self.frame_num * self.a_number * self.b_number,
             dtype=np.float64,
         )
         box_volume = np.prod(self.box_size, dtype=np.float64)
```

### Comparing `MDbrew-2.2.4/MDbrew/application/brewcp2k.py` & `MDbrew-2.2.5/MDbrew/application/brewcp2k.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 #!/usr/bin/env python3
+import os
 import numpy as np
 from tqdm import tqdm
 from scipy import constants
 from ..main.brewery import Brewery
 from ..tool.colorfont import color
 from ..tool.decorator import color_print
 
@@ -78,35 +79,37 @@
         ), f"Frame of Energy {F_energy}, Frame of Stress {F_stress} , Frame of Coords {F_coords}"
         self._num_frame = F_energy
         self._num_atom = len(self._force_list) / F_energy
 
     @color_print(name=printing_option["save"])
     def save_data(self, folder: str = "./", mode: str = "dpdata"):
         folder = folder if folder[-1] == "/" else folder + "/"
-        mode_list = ["dpdata", "raw"]
+        data_path = os.path.join(folder, "set.000")
+        if not os.path.exists(data_path):
+            os.makedirs(data_path)
+        mode_list = ("dpdata", "raw")
         mode = mode.lower()
+        energy_path = os.path.join(data_path, "energy.npy")
+        box_path = os.path.join(data_path, "box.npy")
+        virial_path = os.path.join(data_path, "virial.npy")
+        force_path = os.path.join(data_path, "force.npy")
+        coord_path = os.path.join(data_path, "coord.npy")
         assert mode in mode_list, f"[ ERROR ] mode should be dpata, raw || Not {mode}"
         if mode == "dpdata":
-            np.save(folder + "energy.npy", self.energies)
-            np.save(folder + "box.npy", self.cells.reshape(self._num_frame, 9))
-            np.save(folder + "virial.npy", self.virials.reshape(self._num_frame, 9))
-            np.save(
-                folder + "force.npy",
-                self.forces.reshape(self._num_frame, int(self._num_atom * 3)),
-            )
-            np.save(
-                folder + "coord.npy",
-                self.coords.reshape(self._num_frame, int(self._num_atom * 3)),
-            )
+            np.save(energy_path, self.energies)
+            np.save(box_path, self.cells.reshape(self._num_frame, 9))
+            np.save(virial_path, self.virials.reshape(self._num_frame, 9))
+            np.save(force_path, self.forces.reshape(self._num_frame, int(self._num_atom * 3)))
+            np.save(coord_path, self.coords.reshape(self._num_frame, int(self._num_atom * 3)))
         elif mode == "raw":
-            np.save(folder + "energy.npy", self.energies)
-            np.save(folder + "virial.npy", self.virials)
-            np.save(folder + "force.npy", self.forces)
-            np.save(folder + "coord.npy", self.coords)
-            np.save(folder + "box.npy", self.cells)
+            np.save(energy_path, self.energies)
+            np.save(box_path, self.cells)
+            np.save(virial_path, self.virials)
+            np.save(force_path, self.forces)
+            np.save(coord_path, self.coords)
         np.savetxt(folder + "type.raw", self.types, fmt="%d")
         np.savetxt(folder + "type_map.raw", self._type_map, fmt="%s")
 
     def _brew_xyzfile(self, xyz_file):
         database = Brewery(path=xyz_file, fmt="xyz", is_generator=True).coords
         line_range = tqdm(
             database,
```

### Comparing `MDbrew-2.2.4/MDbrew/main/brewer.py` & `MDbrew-2.2.5/MDbrew/main/brewer.py`

 * *Files identical despite different names*

### Comparing `MDbrew-2.2.4/MDbrew/main/brewery.py` & `MDbrew-2.2.5/MDbrew/main/brewery.py`

 * *Files identical despite different names*

### Comparing `MDbrew-2.2.4/MDbrew/main/filetype/lmps.py` & `MDbrew-2.2.5/MDbrew/main/filetype/lmps.py`

 * *Files identical despite different names*

### Comparing `MDbrew-2.2.4/MDbrew/main/filetype/pdb.py` & `MDbrew-2.2.5/MDbrew/main/filetype/pdb.py`

 * *Files identical despite different names*

### Comparing `MDbrew-2.2.4/MDbrew/main/filetype/vasp.py` & `MDbrew-2.2.5/MDbrew/main/filetype/vasp.py`

 * *Files identical despite different names*

### Comparing `MDbrew-2.2.4/MDbrew/main/opener.py` & `MDbrew-2.2.5/MDbrew/main/opener.py`

 * *Files identical despite different names*

### Comparing `MDbrew-2.2.4/MDbrew/tool/colorfont.py` & `MDbrew-2.2.5/MDbrew/tool/colorfont.py`

 * *Files identical despite different names*

### Comparing `MDbrew-2.2.4/MDbrew/tool/decorator.py` & `MDbrew-2.2.5/MDbrew/tool/decorator.py`

 * *Files identical despite different names*

### Comparing `MDbrew-2.2.4/MDbrew/tool/doctor.py` & `MDbrew-2.2.5/MDbrew/tool/doctor.py`

 * *Files identical despite different names*

### Comparing `MDbrew-2.2.4/MDbrew.egg-info/SOURCES.txt` & `MDbrew-2.2.5/MDbrew.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `MDbrew-2.2.4/setup.py` & `MDbrew-2.2.5/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="MDbrew",
-    version="2.2.4",
+    version="2.2.5",
     author="Knu",
     author_email="minu928@snu.ac.kr",
     url="https://github.com/MyKnu/MDbrew",
     download_url="https://github.com/MyKnu/MDbrew/install_file/MDbrew-2.2.3.tar.gz",
     install_requies=[
         "numpy>=1.0.0",
         "pandas>=1.0.0",
```

