# Comparing `tmp/lumos-sat-1.0.4.tar.gz` & `tmp/lumos-sat-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lumos-sat-1.0.4.tar", last modified: Mon May  1 19:58:46 2023, max compression
+gzip compressed data, was "lumos-sat-1.0.5.tar", last modified: Thu May  4 20:23:55 2023, max compression
```

## Comparing `lumos-sat-1.0.4.tar` & `lumos-sat-1.0.5.tar`

### file list

```diff
@@ -1,32 +1,28 @@
-drwxrwxrwx   0        0        0        0 2023-05-01 19:58:46.162750 lumos-sat-1.0.4/
--rw-rw-rw-   0        0        0     1096 2023-04-06 18:33:06.000000 lumos-sat-1.0.4/LICENSE
--rw-rw-rw-   0        0        0      834 2023-05-01 19:58:46.161753 lumos-sat-1.0.4/PKG-INFO
--rw-rw-rw-   0        0        0      577 2023-04-06 19:37:58.000000 lumos-sat-1.0.4/README.md
-drwxrwxrwx   0        0        0        0 2023-05-01 19:58:46.096815 lumos-sat-1.0.4/lumos/
--rw-rw-rw-   0        0        0        0 2023-04-06 18:42:57.000000 lumos-sat-1.0.4/lumos/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-01 19:58:46.107786 lumos-sat-1.0.4/lumos/brdf/
--rw-rw-rw-   0        0        0        0 2023-04-06 18:51:47.000000 lumos-sat-1.0.4/lumos/brdf/__init__.py
--rw-rw-rw-   0        0        0     2140 2023-05-01 18:30:13.000000 lumos-sat-1.0.4/lumos/brdf/fit_tools.py
--rw-rw-rw-   0        0        0     6648 2023-05-01 19:26:37.000000 lumos-sat-1.0.4/lumos/brdf/library.py
-drwxrwxrwx   0        0        0        0 2023-05-01 19:58:46.115767 lumos-sat-1.0.4/lumos/calculators/
--rw-rw-rw-   0        0        0        0 2023-04-06 18:51:54.000000 lumos-sat-1.0.4/lumos/calculators/__init__.py
--rw-rw-rw-   0        0        0     8086 2023-05-01 19:37:37.000000 lumos-sat-1.0.4/lumos/calculators/brightness_frame.py
--rw-rw-rw-   0        0        0     5444 2023-05-01 19:40:31.000000 lumos-sat-1.0.4/lumos/calculators/ground_frame.py
--rw-rw-rw-   0        0        0      340 2023-04-09 01:56:39.000000 lumos-sat-1.0.4/lumos/constants.py
--rw-rw-rw-   0        0        0     2369 2023-05-01 16:44:37.000000 lumos-sat-1.0.4/lumos/conversions.py
--rw-rw-rw-   0        0        0     3479 2023-04-09 02:37:52.000000 lumos-sat-1.0.4/lumos/functions.py
--rw-rw-rw-   0        0        0     3971 2023-05-01 19:53:20.000000 lumos-sat-1.0.4/lumos/geometry.py
-drwxrwxrwx   0        0        0        0 2023-05-01 19:58:46.129727 lumos-sat-1.0.4/lumos/plot/
--rw-rw-rw-   0        0        0        0 2023-03-10 18:54:08.000000 lumos-sat-1.0.4/lumos/plot/__init__.py
--rw-rw-rw-   0        0        0     2153 2023-05-01 17:13:16.000000 lumos-sat-1.0.4/lumos/plot/brdf.py
--rw-rw-rw-   0        0        0     3029 2023-05-01 17:48:10.000000 lumos-sat-1.0.4/lumos/plot/brightness_frame.py
--rw-rw-rw-   0        0        0     4027 2023-05-01 17:58:04.000000 lumos-sat-1.0.4/lumos/plot/ground_frame.py
--rw-rw-rw-   0        0        0      955 2023-05-01 17:10:23.000000 lumos-sat-1.0.4/lumos/video_tools.py
-drwxrwxrwx   0        0        0        0 2023-05-01 19:58:46.159759 lumos-sat-1.0.4/lumos_sat.egg-info/
--rw-rw-rw-   0        0        0      834 2023-05-01 19:58:45.000000 lumos-sat-1.0.4/lumos_sat.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      583 2023-05-01 19:58:46.000000 lumos-sat-1.0.4/lumos_sat.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-01 19:58:45.000000 lumos-sat-1.0.4/lumos_sat.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      220 2023-05-01 19:58:46.000000 lumos-sat-1.0.4/lumos_sat.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-05-01 19:58:46.000000 lumos-sat-1.0.4/lumos_sat.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      588 2023-05-01 19:57:44.000000 lumos-sat-1.0.4/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-01 19:58:46.163760 lumos-sat-1.0.4/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-04 20:23:55.536374 lumos-sat-1.0.5/
+-rw-rw-rw-   0        0        0     1096 2023-04-06 18:33:06.000000 lumos-sat-1.0.5/LICENSE
+-rw-rw-rw-   0        0        0      834 2023-05-04 20:23:55.533381 lumos-sat-1.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0      577 2023-04-06 19:37:58.000000 lumos-sat-1.0.5/README.md
+drwxrwxrwx   0        0        0        0 2023-05-04 20:23:55.469553 lumos-sat-1.0.5/lumos/
+-rw-rw-rw-   0        0        0        0 2023-04-06 18:42:57.000000 lumos-sat-1.0.5/lumos/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-04 20:23:55.477535 lumos-sat-1.0.5/lumos/brdf/
+-rw-rw-rw-   0        0        0        0 2023-04-06 18:51:47.000000 lumos-sat-1.0.5/lumos/brdf/__init__.py
+-rw-rw-rw-   0        0        0     6648 2023-05-02 20:42:09.000000 lumos-sat-1.0.5/lumos/brdf/library.py
+-rw-rw-rw-   0        0        0     3255 2023-05-03 21:42:13.000000 lumos-sat-1.0.5/lumos/brdf/tools.py
+-rw-rw-rw-   0        0        0    14276 2023-05-03 22:10:42.000000 lumos-sat-1.0.5/lumos/calculator.py
+-rw-rw-rw-   0        0        0      340 2023-04-09 01:56:39.000000 lumos-sat-1.0.5/lumos/constants.py
+drwxrwxrwx   0        0        0        0 2023-05-04 20:23:55.484512 lumos-sat-1.0.5/lumos/constellation/
+-rw-rw-rw-   0        0        0        0 2023-05-02 20:49:52.000000 lumos-sat-1.0.5/lumos/constellation/__init__.py
+-rw-rw-rw-   0        0        0     5105 2023-05-03 19:16:32.000000 lumos-sat-1.0.5/lumos/constellation/library.py
+-rw-rw-rw-   0        0        0     1088 2023-05-03 19:16:14.000000 lumos-sat-1.0.5/lumos/constellation/tools.py
+-rw-rw-rw-   0        0        0     2369 2023-05-01 16:44:37.000000 lumos-sat-1.0.5/lumos/conversions.py
+-rw-rw-rw-   0        0        0     3479 2023-04-09 02:37:52.000000 lumos-sat-1.0.5/lumos/functions.py
+-rw-rw-rw-   0        0        0     3971 2023-05-01 19:53:20.000000 lumos-sat-1.0.5/lumos/geometry.py
+-rw-rw-rw-   0        0        0     9728 2023-05-03 22:36:00.000000 lumos-sat-1.0.5/lumos/plot.py
+drwxrwxrwx   0        0        0        0 2023-05-04 20:23:55.531387 lumos-sat-1.0.5/lumos_sat.egg-info/
+-rw-rw-rw-   0        0        0      834 2023-05-04 20:23:55.000000 lumos-sat-1.0.5/lumos_sat.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      482 2023-05-04 20:23:55.000000 lumos-sat-1.0.5/lumos_sat.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-04 20:23:55.000000 lumos-sat-1.0.5/lumos_sat.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      220 2023-05-04 20:23:55.000000 lumos-sat-1.0.5/lumos_sat.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-05-04 20:23:55.000000 lumos-sat-1.0.5/lumos_sat.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      588 2023-05-04 20:22:30.000000 lumos-sat-1.0.5/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-04 20:23:55.536374 lumos-sat-1.0.5/setup.cfg
```

### Comparing `lumos-sat-1.0.4/LICENSE` & `lumos-sat-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `lumos-sat-1.0.4/PKG-INFO` & `lumos-sat-1.0.5/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lumos-sat
-Version: 1.0.4
+Version: 1.0.5
 Summary: Satellite Brightness Calculation Tools
 Author-email: Forrest Fankhauser <fafankhauser@ucdavis.edu>
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # lumos-sat
```

### Comparing `lumos-sat-1.0.4/README.md` & `lumos-sat-1.0.5/README.md`

 * *Files identical despite different names*

### Comparing `lumos-sat-1.0.4/lumos/brdf/fit_tools.py` & `lumos-sat-1.0.5/lumos/brdf/tools.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,20 +1,40 @@
 """
-Tools for fitting experimental BRDF data to models
+Tools for working with BRDF models and data
 """
 
 import numpy as np
 import scipy.optimize
 import lumos.conversions
 
-def fit_model(
+def read_brdf(brdf_file_path):
+    """
+    Reads data from a BRDF file
+
+    :param brdf_file_path: Path to the BRDF file
+    :type brdf_file_path: str
+    :return: :math:`\\phi_i, \\theta_i, \\phi_o, \\theta_o, BRDF`
+    :rtype: tuple[:class:`np.ndarray`]
+    """
+
+    data = np.loadtxt(brdf_file_path, skiprows = 1)
+
+    phi_in = data[:, 0]
+    theta_in = data[:, 1]
+    phi_out = data[:, 2]
+    theta_out = data[:, 3]
+    brdf = data[:, 4]
+
+    return phi_in, theta_in, phi_out, theta_out, brdf
+
+def fit(
         data_file,
         model_func,
-        bounds,
-        p0,
+        bounds = None,
+        p0 = None,
         log_space = True,
         clip = 0
         ):
     
     """
     Fits a model to experimental data.
 
@@ -28,21 +48,17 @@
     :type p0: tuple
     :param log_space: Whether or not to fit BRDF in log_space
     :type log_space: bool
     :param clip: Removes BRDF data below this cutoff from fitting
     :type clip: float
     """
 
-    data = np.loadtxt(data_file, skiprows = 1)
-
-    phi_in = np.deg2rad(data[:, 0])
-    theta_in = np.deg2rad(data[:, 1])
-    phi_out = np.deg2rad(data[:, 2])
-    theta_out = np.deg2rad(data[:, 3])
-    brdf = data[:, 4]
+    phi_in, theta_in, phi_out, theta_out, brdf = read_brdf(data_file)
+    phi_in, theta_in = np.deg2rad(phi_in), np.deg2rad(theta_in)
+    phi_out, theta_out = np.deg2rad(phi_out), np.deg2rad(theta_out)
 
     mask = brdf > clip
 
     phi_in = phi_in[mask]
     theta_in = theta_in[mask]
     phi_out = phi_out[mask]
     theta_out = theta_out[mask]
@@ -68,8 +84,30 @@
 
     popt, _ = scipy.optimize.curve_fit(fit_function, 
                                        indexes, 
                                        np.log10(brdf) if log_space else brdf, 
                                        bounds = bounds,
                                        p0 = p0)
 
-    return popt
+    return popt
+
+def pack_binomial_parameters(n, m, l1, l2, *params):
+    """
+    Convert list into B & C matrices, which can then be passed to the Binomial Model
+
+    :param n: n
+    :type n: int
+    :param m: m
+    :type m: int
+    :param l1: l1
+    :type l1: int
+    :param l2: l2, ensure l2 > l1
+    :type l2: int
+    :param params: list of values
+    :type params: list[float]
+    :return: B, C, d
+    :rtype: :class:`np.ndarray`, :class:`np.ndarray`, float
+    """
+    params = np.array(params)
+    B = np.reshape( params[:n * m], (n, m) )
+    C = np.reshape( params[n * m:], (n, l2 - l1))
+    return B, C
```

### Comparing `lumos-sat-1.0.4/lumos/brdf/library.py` & `lumos-sat-1.0.5/lumos/brdf/library.py`

 * *Files identical despite different names*

### Comparing `lumos-sat-1.0.4/lumos/conversions.py` & `lumos-sat-1.0.5/lumos/conversions.py`

 * *Files identical despite different names*

### Comparing `lumos-sat-1.0.4/lumos/functions.py` & `lumos-sat-1.0.5/lumos/functions.py`

 * *Files identical despite different names*

### Comparing `lumos-sat-1.0.4/lumos/geometry.py` & `lumos-sat-1.0.5/lumos/geometry.py`

 * *Files identical despite different names*

### Comparing `lumos-sat-1.0.4/lumos_sat.egg-info/PKG-INFO` & `lumos-sat-1.0.5/lumos_sat.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lumos-sat
-Version: 1.0.4
+Version: 1.0.5
 Summary: Satellite Brightness Calculation Tools
 Author-email: Forrest Fankhauser <fafankhauser@ucdavis.edu>
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # lumos-sat
```

### Comparing `lumos-sat-1.0.4/pyproject.toml` & `lumos-sat-1.0.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "lumos-sat"
-version = "1.0.4"
+version = "1.0.5"
 description = "Satellite Brightness Calculation Tools"
 authors = [
     {name = "Forrest Fankhauser", email = "fafankhauser@ucdavis.edu"},
 ]
 requires-python = ">=3.10"
 readme = "README.md"
```

