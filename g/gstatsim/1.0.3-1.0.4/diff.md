# Comparing `tmp/gstatsim-1.0.3.tar.gz` & `tmp/gstatsim-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gstatsim-1.0.3.tar", last modified: Thu May  4 18:16:24 2023, max compression
+gzip compressed data, was "gstatsim-1.0.4.tar", last modified: Thu May  4 20:12:07 2023, max compression
```

## Comparing `gstatsim-1.0.3.tar` & `gstatsim-1.0.4.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 michaelfield   (502) staff       (20)        0 2023-05-04 18:16:24.713975 gstatsim-1.0.3/
--rw-r--r--   0 michaelfield   (502) staff       (20)     1068 2023-04-27 17:08:18.000000 gstatsim-1.0.3/LICENSE
--rw-r--r--   0 michaelfield   (502) staff       (20)     5160 2023-05-04 18:16:24.713855 gstatsim-1.0.3/PKG-INFO
--rw-r--r--   0 michaelfield   (502) staff       (20)     4620 2023-05-04 18:15:23.000000 gstatsim-1.0.3/README.md
-drwxr-xr-x   0 michaelfield   (502) staff       (20)        0 2023-05-04 18:16:24.713672 gstatsim-1.0.3/gstatsim.egg-info/
--rw-r--r--   0 michaelfield   (502) staff       (20)     5160 2023-05-04 18:16:24.000000 gstatsim-1.0.3/gstatsim.egg-info/PKG-INFO
--rw-r--r--   0 michaelfield   (502) staff       (20)      197 2023-05-04 18:16:24.000000 gstatsim-1.0.3/gstatsim.egg-info/SOURCES.txt
--rw-r--r--   0 michaelfield   (502) staff       (20)        1 2023-05-04 18:16:24.000000 gstatsim-1.0.3/gstatsim.egg-info/dependency_links.txt
--rw-r--r--   0 michaelfield   (502) staff       (20)       69 2023-05-04 18:16:24.000000 gstatsim-1.0.3/gstatsim.egg-info/requires.txt
--rw-r--r--   0 michaelfield   (502) staff       (20)        9 2023-05-04 18:16:24.000000 gstatsim-1.0.3/gstatsim.egg-info/top_level.txt
--rw-r--r--   0 michaelfield   (502) staff       (20)    56584 2023-04-27 16:20:42.000000 gstatsim-1.0.3/gstatsim.py
--rw-r--r--   0 michaelfield   (502) staff       (20)       38 2023-05-04 18:16:24.714012 gstatsim-1.0.3/setup.cfg
--rw-r--r--   0 michaelfield   (502) staff       (20)      938 2023-05-04 18:15:36.000000 gstatsim-1.0.3/setup.py
+drwxr-xr-x   0 michaelfield   (502) staff       (20)        0 2023-05-04 20:12:07.027526 gstatsim-1.0.4/
+-rw-r--r--   0 michaelfield   (502) staff       (20)     1068 2023-05-04 18:46:36.000000 gstatsim-1.0.4/LICENSE
+-rw-r--r--   0 michaelfield   (502) staff       (20)     5530 2023-05-04 20:12:07.027387 gstatsim-1.0.4/PKG-INFO
+-rw-r--r--   0 michaelfield   (502) staff       (20)     4990 2023-05-04 20:11:32.000000 gstatsim-1.0.4/README.md
+drwxr-xr-x   0 michaelfield   (502) staff       (20)        0 2023-05-04 20:12:07.027192 gstatsim-1.0.4/gstatsim.egg-info/
+-rw-r--r--   0 michaelfield   (502) staff       (20)     5530 2023-05-04 20:12:07.000000 gstatsim-1.0.4/gstatsim.egg-info/PKG-INFO
+-rw-r--r--   0 michaelfield   (502) staff       (20)      197 2023-05-04 20:12:07.000000 gstatsim-1.0.4/gstatsim.egg-info/SOURCES.txt
+-rw-r--r--   0 michaelfield   (502) staff       (20)        1 2023-05-04 20:12:07.000000 gstatsim-1.0.4/gstatsim.egg-info/dependency_links.txt
+-rw-r--r--   0 michaelfield   (502) staff       (20)       69 2023-05-04 20:12:07.000000 gstatsim-1.0.4/gstatsim.egg-info/requires.txt
+-rw-r--r--   0 michaelfield   (502) staff       (20)        9 2023-05-04 20:12:07.000000 gstatsim-1.0.4/gstatsim.egg-info/top_level.txt
+-rw-r--r--   0 michaelfield   (502) staff       (20)    56696 2023-05-04 18:46:36.000000 gstatsim-1.0.4/gstatsim.py
+-rw-r--r--   0 michaelfield   (502) staff       (20)       38 2023-05-04 20:12:07.027566 gstatsim-1.0.4/setup.cfg
+-rw-r--r--   0 michaelfield   (502) staff       (20)      938 2023-05-04 20:11:51.000000 gstatsim-1.0.4/setup.py
```

### Comparing `gstatsim-1.0.3/LICENSE` & `gstatsim-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `gstatsim-1.0.3/PKG-INFO` & `gstatsim-1.0.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,28 @@
 Metadata-Version: 2.1
 Name: gstatsim
-Version: 1.0.3
+Version: 1.0.4
 Summary: Geostatistics tools for interpolation and simulation.
 Home-page: https://github.com/GatorGlaciology/GStatSim
 Author: (Emma) Mickey MacKie
 Author-email: emackie@ufl.edu
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Requires-Python: >=3
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 
+[![Jupyter Book Badge](https://jupyterbook.org/badge.svg)](<https://gatorglaciology.github.io/gstatsimbook/intro.html>) [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/GatorGlaciology/gstatsimbook/HEAD?urlpath=lab)
+
+</p>
+
 # GStatSim
 GStatSim is a Python package specifically designed for geostatistical interpolation and simulation. It is inspired by open source geostatistical resources such as GeostatsPy and SciKit-GStat. The functions are intended to address the challenges of working with datasets with large crossover errors, non-linear trends, variability in measurement density, and non-stationarity. These tools are part of our ongoing effort to develop and adapt open-access geostatistical functions.
 
 We have created Jupyter Book tutorials here: https://gatorglaciology.github.io/gstatsimbook/intro.html
 
 In its current state, the demos focus on the geostatistical simulation of subglacial topography. However, these protocols could be applied to a number topics in glaciology, or geoscientific problems in general.
 
@@ -41,19 +45,20 @@
 ## Demos
 We have created tutorials that are designed to provide an intuitive understanding of geostatistical methods and to demonstrate how these methods are used. The current demos are:
 
 * **1_Experimental_Variogram.ipynb** - Demonstration of experimental variogram calculation to quantify spatial relationships.
 * **2_Variogram_model.ipynb** - A tutorial on fitting a variogram model to an experimental variogram.
 * **3_Simple_kriging_and_ordinary_kriging.ipynb** - Demonstration of simple kriging and ordinary kriging interpolation.
 * **4_Sequential_Gaussian_Simulation.ipynb** - An introduction to stochastic simulation.
-* **5_interpolation_with_anisotropy.ipynb** - A demonstration of kriging and SGS with anisotropy.
-* **6_non-stationary_SGS_example1.ipynb** - A tutorial on SGS with multiple variograms. This demo uses k-means clustering to divide the conditioning data into groups that are each assigned their own variogram.
-* **7_non-stationary_SGS_example2.ipynb** - SGS using multiple variograms where the clusters are determined automatically.
-* **8_interpolation_with_a_trend.ipynb** - Kriging and SGS in the presence of a large-scale trend.
-* **9_cokriging_and_cosimulation_MM1.ipynb** - Kriging and SGS using secondary constraints.
+* **5_Variogram_interpolation_comparison.ipynb** - A demonstration of kriging and SGS with different variogram models.
+* **6_interpolation_with_anisotropy.ipynb** - A demonstration of kriging and SGS with anisotropy.
+* **7_non-stationary_SGS_example1.ipynb** - A tutorial on SGS with multiple variograms. This demo uses k-means clustering to divide the conditioning data into groups that are each assigned their own variogram.
+* **8_non-stationary_SGS_example2.ipynb** - SGS using multiple variograms where the clusters are determined automatically.
+* **9_interpolation_with_a_trend.ipynb** - Kriging and SGS in the presence of a large-scale trend.
+* **10_cokriging_and_cosimulation_MM1.ipynb** - Kriging and SGS using secondary constraints.
 
 
 
 # Contributors
 (Emma) Mickey MacKie, University of Florida
 
 Michael Field, University of Florida
```

### Comparing `gstatsim-1.0.3/README.md` & `gstatsim-1.0.4/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,12 @@
 
+[![Jupyter Book Badge](https://jupyterbook.org/badge.svg)](<https://gatorglaciology.github.io/gstatsimbook/intro.html>) [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/GatorGlaciology/gstatsimbook/HEAD?urlpath=lab)
+
+</p>
+
 # GStatSim
 GStatSim is a Python package specifically designed for geostatistical interpolation and simulation. It is inspired by open source geostatistical resources such as GeostatsPy and SciKit-GStat. The functions are intended to address the challenges of working with datasets with large crossover errors, non-linear trends, variability in measurement density, and non-stationarity. These tools are part of our ongoing effort to develop and adapt open-access geostatistical functions.
 
 We have created Jupyter Book tutorials here: https://gatorglaciology.github.io/gstatsimbook/intro.html
 
 In its current state, the demos focus on the geostatistical simulation of subglacial topography. However, these protocols could be applied to a number topics in glaciology, or geoscientific problems in general.
 
@@ -25,19 +29,20 @@
 ## Demos
 We have created tutorials that are designed to provide an intuitive understanding of geostatistical methods and to demonstrate how these methods are used. The current demos are:
 
 * **1_Experimental_Variogram.ipynb** - Demonstration of experimental variogram calculation to quantify spatial relationships.
 * **2_Variogram_model.ipynb** - A tutorial on fitting a variogram model to an experimental variogram.
 * **3_Simple_kriging_and_ordinary_kriging.ipynb** - Demonstration of simple kriging and ordinary kriging interpolation.
 * **4_Sequential_Gaussian_Simulation.ipynb** - An introduction to stochastic simulation.
-* **5_interpolation_with_anisotropy.ipynb** - A demonstration of kriging and SGS with anisotropy.
-* **6_non-stationary_SGS_example1.ipynb** - A tutorial on SGS with multiple variograms. This demo uses k-means clustering to divide the conditioning data into groups that are each assigned their own variogram.
-* **7_non-stationary_SGS_example2.ipynb** - SGS using multiple variograms where the clusters are determined automatically.
-* **8_interpolation_with_a_trend.ipynb** - Kriging and SGS in the presence of a large-scale trend.
-* **9_cokriging_and_cosimulation_MM1.ipynb** - Kriging and SGS using secondary constraints.
+* **5_Variogram_interpolation_comparison.ipynb** - A demonstration of kriging and SGS with different variogram models.
+* **6_interpolation_with_anisotropy.ipynb** - A demonstration of kriging and SGS with anisotropy.
+* **7_non-stationary_SGS_example1.ipynb** - A tutorial on SGS with multiple variograms. This demo uses k-means clustering to divide the conditioning data into groups that are each assigned their own variogram.
+* **8_non-stationary_SGS_example2.ipynb** - SGS using multiple variograms where the clusters are determined automatically.
+* **9_interpolation_with_a_trend.ipynb** - Kriging and SGS in the presence of a large-scale trend.
+* **10_cokriging_and_cosimulation_MM1.ipynb** - Kriging and SGS using secondary constraints.
 
 
 
 # Contributors
 (Emma) Mickey MacKie, University of Florida
 
 Michael Field, University of Florida
```

### Comparing `gstatsim-1.0.3/gstatsim.egg-info/PKG-INFO` & `gstatsim-1.0.4/gstatsim.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,28 @@
 Metadata-Version: 2.1
 Name: gstatsim
-Version: 1.0.3
+Version: 1.0.4
 Summary: Geostatistics tools for interpolation and simulation.
 Home-page: https://github.com/GatorGlaciology/GStatSim
 Author: (Emma) Mickey MacKie
 Author-email: emackie@ufl.edu
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Requires-Python: >=3
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 
+[![Jupyter Book Badge](https://jupyterbook.org/badge.svg)](<https://gatorglaciology.github.io/gstatsimbook/intro.html>) [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/GatorGlaciology/gstatsimbook/HEAD?urlpath=lab)
+
+</p>
+
 # GStatSim
 GStatSim is a Python package specifically designed for geostatistical interpolation and simulation. It is inspired by open source geostatistical resources such as GeostatsPy and SciKit-GStat. The functions are intended to address the challenges of working with datasets with large crossover errors, non-linear trends, variability in measurement density, and non-stationarity. These tools are part of our ongoing effort to develop and adapt open-access geostatistical functions.
 
 We have created Jupyter Book tutorials here: https://gatorglaciology.github.io/gstatsimbook/intro.html
 
 In its current state, the demos focus on the geostatistical simulation of subglacial topography. However, these protocols could be applied to a number topics in glaciology, or geoscientific problems in general.
 
@@ -41,19 +45,20 @@
 ## Demos
 We have created tutorials that are designed to provide an intuitive understanding of geostatistical methods and to demonstrate how these methods are used. The current demos are:
 
 * **1_Experimental_Variogram.ipynb** - Demonstration of experimental variogram calculation to quantify spatial relationships.
 * **2_Variogram_model.ipynb** - A tutorial on fitting a variogram model to an experimental variogram.
 * **3_Simple_kriging_and_ordinary_kriging.ipynb** - Demonstration of simple kriging and ordinary kriging interpolation.
 * **4_Sequential_Gaussian_Simulation.ipynb** - An introduction to stochastic simulation.
-* **5_interpolation_with_anisotropy.ipynb** - A demonstration of kriging and SGS with anisotropy.
-* **6_non-stationary_SGS_example1.ipynb** - A tutorial on SGS with multiple variograms. This demo uses k-means clustering to divide the conditioning data into groups that are each assigned their own variogram.
-* **7_non-stationary_SGS_example2.ipynb** - SGS using multiple variograms where the clusters are determined automatically.
-* **8_interpolation_with_a_trend.ipynb** - Kriging and SGS in the presence of a large-scale trend.
-* **9_cokriging_and_cosimulation_MM1.ipynb** - Kriging and SGS using secondary constraints.
+* **5_Variogram_interpolation_comparison.ipynb** - A demonstration of kriging and SGS with different variogram models.
+* **6_interpolation_with_anisotropy.ipynb** - A demonstration of kriging and SGS with anisotropy.
+* **7_non-stationary_SGS_example1.ipynb** - A tutorial on SGS with multiple variograms. This demo uses k-means clustering to divide the conditioning data into groups that are each assigned their own variogram.
+* **8_non-stationary_SGS_example2.ipynb** - SGS using multiple variograms where the clusters are determined automatically.
+* **9_interpolation_with_a_trend.ipynb** - Kriging and SGS in the presence of a large-scale trend.
+* **10_cokriging_and_cosimulation_MM1.ipynb** - Kriging and SGS using secondary constraints.
 
 
 
 # Contributors
 (Emma) Mickey MacKie, University of Florida
 
 Michael Field, University of Florida
```

### Comparing `gstatsim-1.0.3/gstatsim.py` & `gstatsim-1.0.4/gstatsim.py`

 * *Files 2% similar despite different names*

```diff
@@ -1152,15 +1152,16 @@
         minor_range = vario[3]
         rotation_matrix = make_rotation_matrix(azimuth, major_range, minor_range) 
 
         df1 = df1.rename(columns = {xx1: "X", yy1: "Y", zz1: "Z"})
         df2 = df2.rename(columns = {xx2: "X", yy2: "Y", zz2: "Z"})
 
         mean_1 = np.average(df1['Z']) 
-        var_1 = vario[4]
+        var_1 = np.var(df1['Z']) # replaced var_1 = vario[4]
+        vario[4] = np.var(df1['Z']) 
         mean_2 = np.average(df2['Z']) 
         var_2 = np.var(df2['Z'])
 
         est_cokrige = np.zeros(shape=len(prediction_grid)) 
         var_cokrige = np.zeros(shape=len(prediction_grid))
 
         for z, predxy in enumerate(tqdm(prediction_grid, position=0, leave=True)):
@@ -1204,15 +1205,15 @@
 
                 # solve kriging system
                 k_weights, res, rank, s = np.linalg.lstsq(covariance_matrix, covariance_array, rcond = None) 
                 part1 = mean_1 + np.sum(k_weights[0:new_num_pts]*(norm_data_val[0:new_num_pts] - mean_1)/np.sqrt(var_1))
                 part2 = k_weights[new_num_pts] * (nearest_second[-1] - mean_2)/np.sqrt(var_2)
                                
                 est_cokrige[z] = part1 + part2 
-                var_cokrige[z] = var_1 - np.sum(k_weights[0:new_num_pts+1]*covariance_array[0:new_num_pts+1]) 
+                var_cokrige[z] = var_1 - np.sum(k_weights*covariance_array) 
             else:
                 est_cokrige[z] = df1['Z'].values[np.where(test_idx==2)[0][0]]
                 var_cokrige[z] = 0
 
         return est_cokrige, var_cokrige
 
     def cosim_mm1(prediction_grid, df1, xx1, yy1, zz1, df2, xx2, yy2, zz2, num_points, vario, radius, corrcoef):
@@ -1263,15 +1264,16 @@
         rotation_matrix = make_rotation_matrix(azimuth, major_range, minor_range)
         df1 = df1.rename(columns = {xx1: "X", yy1: "Y", zz1: "Z"}) 
         df2 = df2.rename(columns = {xx2: "X", yy2: "Y", zz2: "Z"})
         xyindex = np.arange(len(prediction_grid)) 
         random.shuffle(xyindex)
 
         mean_1 = np.average(df1['Z']) 
-        var_1 = vario[4]
+        var_1 = np.var(df1['Z']) # replaced var_1 = vario[4]
+        vario[4] = np.var(df1['Z']) 
         mean_2 = np.average(df2['Z']) 
         var_2 = np.var(df2['Z'])
    
         cosim = np.zeros(shape=len(prediction_grid))
 
         # for each coordinate in the prediction grid
         for idx, predxy in enumerate(tqdm(prediction_grid, position=0, leave=True)):
```

### Comparing `gstatsim-1.0.3/setup.py` & `gstatsim-1.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup
 
-version = '1.0.3'
+version = '1.0.4'
 
 classifiers = [
     'Programming Language :: Python :: 3',
     'License :: OSI Approved :: MIT License',
     'Operating System :: OS Independent',
     'Topic :: Scientific/Engineering :: Information Analysis',
 ]
```

