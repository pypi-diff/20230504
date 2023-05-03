# Comparing `tmp/geometrout-0.1.0.6.tar.gz` & `tmp/geometrout-0.1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "geometrout-0.1.0.6.tar", last modified: Tue May  2 00:54:59 2023, max compression
+gzip compressed data, was "geometrout-0.1.0.7.tar", last modified: Wed May  3 23:35:31 2023, max compression
```

## Comparing `geometrout-0.1.0.6.tar` & `geometrout-0.1.0.7.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 00:54:59.605587 geometrout-0.1.0.6/
--rw-r--r--   0 runner    (1001) docker     (123)     2327 2023-05-02 00:54:50.000000 geometrout-0.1.0.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      578 2023-05-02 00:54:59.605587 geometrout-0.1.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-05-02 00:54:50.000000 geometrout-0.1.0.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 00:54:59.601587 geometrout-0.1.0.6/geometrout/
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-05-02 00:54:50.000000 geometrout-0.1.0.6/geometrout/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1853 2023-05-02 00:54:50.000000 geometrout-0.1.0.6/geometrout/pointcloud.py
--rw-r--r--   0 runner    (1001) docker     (123)    21122 2023-05-02 00:54:50.000000 geometrout-0.1.0.6/geometrout/primitive.py
--rw-r--r--   0 runner    (1001) docker     (123)    10397 2023-05-02 00:54:50.000000 geometrout-0.1.0.6/geometrout/transform.py
--rw-r--r--   0 runner    (1001) docker     (123)     1338 2023-05-02 00:54:50.000000 geometrout-0.1.0.6/geometrout/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 00:54:59.605587 geometrout-0.1.0.6/geometrout.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      578 2023-05-02 00:54:59.000000 geometrout-0.1.0.6/geometrout.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      327 2023-05-02 00:54:59.000000 geometrout-0.1.0.6/geometrout.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 00:54:59.000000 geometrout-0.1.0.6/geometrout.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-02 00:54:59.000000 geometrout-0.1.0.6/geometrout.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-02 00:54:59.000000 geometrout-0.1.0.6/geometrout.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-02 00:54:50.000000 geometrout-0.1.0.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      689 2023-05-02 00:54:59.605587 geometrout-0.1.0.6/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 23:35:31.698936 geometrout-0.1.0.7/
+-rw-r--r--   0 runner    (1001) docker     (123)     2327 2023-05-03 23:35:21.000000 geometrout-0.1.0.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      578 2023-05-03 23:35:31.698936 geometrout-0.1.0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-05-03 23:35:21.000000 geometrout-0.1.0.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 23:35:31.698936 geometrout-0.1.0.7/geometrout/
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-05-03 23:35:21.000000 geometrout-0.1.0.7/geometrout/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1853 2023-05-03 23:35:21.000000 geometrout-0.1.0.7/geometrout/pointcloud.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21396 2023-05-03 23:35:21.000000 geometrout-0.1.0.7/geometrout/primitive.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10592 2023-05-03 23:35:21.000000 geometrout-0.1.0.7/geometrout/transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1338 2023-05-03 23:35:21.000000 geometrout-0.1.0.7/geometrout/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 23:35:31.698936 geometrout-0.1.0.7/geometrout.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      578 2023-05-03 23:35:31.000000 geometrout-0.1.0.7/geometrout.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      327 2023-05-03 23:35:31.000000 geometrout-0.1.0.7/geometrout.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-03 23:35:31.000000 geometrout-0.1.0.7/geometrout.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-03 23:35:31.000000 geometrout-0.1.0.7/geometrout.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-03 23:35:31.000000 geometrout-0.1.0.7/geometrout.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-03 23:35:21.000000 geometrout-0.1.0.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      689 2023-05-03 23:35:31.698936 geometrout-0.1.0.7/setup.cfg
```

### Comparing `geometrout-0.1.0.6/LICENSE` & `geometrout-0.1.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `geometrout-0.1.0.6/PKG-INFO` & `geometrout-0.1.0.7/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: geometrout
-Version: 0.1.0.6
+Version: 0.1.0.7
 Summary: A collection of geometric methods and concepts tailored to machine learning for robotics
-Download-URL: https://github.com/fishbotics/geometrout/archive/refs/tags/v0.1.0.6.tar.gz
+Download-URL: https://github.com/fishbotics/geometrout/archive/refs/tags/v0.1.0.7.tar.gz
 License: MIT
 Requires-Python: >=3.6
 License-File: LICENSE
 
 This is a high-performance set of tools used for CPU-based geometric processing in Python. By-in-large, these are simple methods, written with Numpy and Numba. These tools were designed for Machine Learning and Robotics, but could feasibly be used for any 3D processing task.
```

### Comparing `geometrout-0.1.0.6/geometrout/pointcloud.py` & `geometrout-0.1.0.7/geometrout/pointcloud.py`

 * *Files identical despite different names*

### Comparing `geometrout-0.1.0.6/geometrout/primitive.py` & `geometrout-0.1.0.7/geometrout/primitive.py`

 * *Files 2% similar despite different names*

```diff
@@ -162,27 +162,27 @@
                 " /    y     /   |",
                 "+----------+    |",
                 "|          |    /",
                 "|          |   / ",
                 "|         z|  /  ",
                 "|          | /   ",
                 "+----------+     ",
-                f"Center: {self.center}",
-                f"Dimensions: {self.dims}",
-                f"Orientation (wxyz): {self.pose.so3.wxyz}",
+                f"Center: {repr(self.center)}",
+                f"Dimensions: {repr(self.dims)}",
+                f"Orientation (wxyz): {repr(self.pose.so3.q)}",
             ]
         )
 
     def __repr__(self):
         return "\n".join(
             [
                 "Cuboid(",
-                f"    center={self.center},",
-                f"    dims={self.dims},",
-                f"    quaternion={self.pose.so3.wxyz},",
+                f"    center={repr(self.center)},",
+                f"    dims={repr(self.dims)},",
+                f"    quaternion={repr(self.pose.so3.q)},",
                 ")",
             ]
         )
 
     @staticmethod
     def unit():
         return Cuboid(
@@ -335,14 +335,24 @@
         :param center: The center of the sphere as a list of numpy array
         :param radius: The radius of the sphere as a number
         """
         self.center = center.astype(np.double)
         assert radius >= 0
         self.radius = radius
 
+    def __repr__(self):
+        return "\n".join(
+            [
+                "Sphere(",
+                f"    center={repr(self.center)},",
+                f"    radius={self.radius},",
+                ")",
+            ]
+        )
+
     def copy(self):
         return Sphere(np.copy(self.center), self.radius)
 
     @staticmethod
     def unit():
         return Sphere(np.zeros(3), 1.0)
 
@@ -529,18 +539,18 @@
             np.copy(self.pose.pos), self.radius, self.height, np.copy(self.pose.so3.q)
         )
 
     def __repr__(self):
         return "\n".join(
             [
                 "Cylinder(",
-                f"    center={self.center},",
+                f"    center={repr(self.center)},",
                 f"    radius={self.radius},",
                 f"    height={self.height},",
-                f"    quaternion={self.pose.so3.wxyz},",
+                f"    quaternion={repr(self.pose.so3.q)},",
                 ")",
             ]
         )
 
     @property
     def center(self):
         """
```

### Comparing `geometrout-0.1.0.6/geometrout/transform.py` & `geometrout-0.1.0.7/geometrout/transform.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,9 @@
-import numpy as np
 import numba as nb
-from numba.experimental import jitclass
+import numpy as np
 
 
 @nb.jit(nopython=True, cache=True)
 def _quaternion_trace_method(matrix, rtol=1e-7, atol=1e-7):
     """
     This code uses a modification of the algorithm described in:
     https://d3cw3dd2w32x2b.cloudfront.net/wp-content/uploads/2015/01/matrix-to-quat.pdf
@@ -339,14 +338,24 @@
         return [x, y, z]
 
     @staticmethod
     def from_matrix(matrix, rtol=1e-7, atol=1e-7):
         q = _quaternion_trace_method(np.copy(matrix[:3, :3]), rtol, atol)
         return SE3(np.copy(matrix[:3, 3]), q)
 
+    def __repr__(self):
+        return "\n".join(
+            [
+                "SE3(",
+                f"    pos={repr(self.pos)},",
+                f"    quaternion={repr(self.so3.q)},",
+                ")",
+            ]
+        )
+
     @staticmethod
     def from_unit_axes(origin, x, y, z, rtol=1e-7, atol=1e-7):
         """
         Constructs SE3 object from unit axes indicating direction and an origin
 
         :param origin: np.array indicating the placement of the origin
         :param x: A unit axis indicating the direction of the x axis
```

### Comparing `geometrout-0.1.0.6/geometrout/utils.py` & `geometrout-0.1.0.7/geometrout/utils.py`

 * *Files identical despite different names*

### Comparing `geometrout-0.1.0.6/geometrout.egg-info/PKG-INFO` & `geometrout-0.1.0.7/geometrout.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: geometrout
-Version: 0.1.0.6
+Version: 0.1.0.7
 Summary: A collection of geometric methods and concepts tailored to machine learning for robotics
-Download-URL: https://github.com/fishbotics/geometrout/archive/refs/tags/v0.1.0.6.tar.gz
+Download-URL: https://github.com/fishbotics/geometrout/archive/refs/tags/v0.1.0.7.tar.gz
 License: MIT
 Requires-Python: >=3.6
 License-File: LICENSE
 
 This is a high-performance set of tools used for CPU-based geometric processing in Python. By-in-large, these are simple methods, written with Numpy and Numba. These tools were designed for Machine Learning and Robotics, but could feasibly be used for any 3D processing task.
```

### Comparing `geometrout-0.1.0.6/setup.cfg` & `geometrout-0.1.0.7/setup.cfg`

 * *Files 26% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [metadata]
 name = geometrout
-version = 0.1.0.6
+version = 0.1.0.7
 description = A collection of geometric methods and concepts tailored to machine learning for robotics
 long_description = This is a high-performance set of tools used for CPU-based geometric processing in Python. By-in-large, these are simple methods, written with Numpy and Numba. These tools were designed for Machine Learning and Robotics, but could feasibly be used for any 3D processing task.
 license = MIT
-download_url = https://github.com/fishbotics/geometrout/archive/refs/tags/v0.1.0.6.tar.gz
+download_url = https://github.com/fishbotics/geometrout/archive/refs/tags/v0.1.0.7.tar.gz
 
 [options]
 packages = geometrout
 python_requires = >=3.6
 install_requires = 
 	numpy
 	numba >= 0.56.4
```

