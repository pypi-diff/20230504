# Comparing `tmp/monotonic derivative-0.13.tar.gz` & `tmp/monotonic derivative-0.14.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "monotonic derivative-0.13.tar", last modified: Thu May  4 08:29:02 2023, max compression
+gzip compressed data, was "monotonic derivative-0.14.tar", last modified: Thu May  4 09:30:17 2023, max compression
```

## Comparing `monotonic derivative-0.13.tar` & `monotonic derivative-0.14.tar`

### file list

```diff
@@ -1,16 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 08:29:02.298344 monotonic derivative-0.13/
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-05-04 08:28:48.000000 monotonic derivative-0.13/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      509 2023-05-04 08:29:02.298344 monotonic derivative-0.13/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3069 2023-05-04 08:28:48.000000 monotonic derivative-0.13/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 08:29:02.298344 monotonic derivative-0.13/monotonic_derivative/
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-05-04 08:28:48.000000 monotonic derivative-0.13/monotonic_derivative/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-04 08:28:48.000000 monotonic derivative-0.13/monotonic_derivative/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     4789 2023-05-04 08:28:48.000000 monotonic derivative-0.13/monotonic_derivative/monotonic_derivative.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 08:29:02.298344 monotonic derivative-0.13/monotonic_derivative.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      509 2023-05-04 08:29:02.000000 monotonic derivative-0.13/monotonic_derivative.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      356 2023-05-04 08:29:02.000000 monotonic derivative-0.13/monotonic_derivative.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 08:29:02.000000 monotonic derivative-0.13/monotonic_derivative.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-05-04 08:29:02.000000 monotonic derivative-0.13/monotonic_derivative.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-04 08:29:02.000000 monotonic derivative-0.13/monotonic_derivative.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-04 08:29:02.298344 monotonic derivative-0.13/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      637 2023-05-04 08:28:48.000000 monotonic derivative-0.13/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:17.655881 monotonic derivative-0.14/
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-05-04 09:30:07.000000 monotonic derivative-0.14/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      509 2023-05-04 09:30:17.655881 monotonic derivative-0.14/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3424 2023-05-04 09:30:07.000000 monotonic derivative-0.14/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:17.655881 monotonic derivative-0.14/monotonic_derivative/
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-05-04 09:30:07.000000 monotonic derivative-0.14/monotonic_derivative/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-04 09:30:07.000000 monotonic derivative-0.14/monotonic_derivative/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4961 2023-05-04 09:30:07.000000 monotonic derivative-0.14/monotonic_derivative/monotonic_derivative.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:17.655881 monotonic derivative-0.14/monotonic_derivative.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      509 2023-05-04 09:30:17.000000 monotonic derivative-0.14/monotonic_derivative.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      370 2023-05-04 09:30:17.000000 monotonic derivative-0.14/monotonic_derivative.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 09:30:17.000000 monotonic derivative-0.14/monotonic_derivative.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-05-04 09:30:17.000000 monotonic derivative-0.14/monotonic_derivative.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-04 09:30:17.000000 monotonic derivative-0.14/monotonic_derivative.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-04 09:30:17.655881 monotonic derivative-0.14/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      637 2023-05-04 09:30:07.000000 monotonic derivative-0.14/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:17.655881 monotonic derivative-0.14/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1564 2023-05-04 09:30:07.000000 monotonic derivative-0.14/tests/test.py
```

### Comparing `monotonic derivative-0.13/LICENSE` & `monotonic derivative-0.14/LICENSE`

 * *Files identical despite different names*

### Comparing `monotonic derivative-0.13/README.md` & `monotonic derivative-0.14/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -9,19 +9,18 @@
 - [Example](#example)
 - [Real-life Applications](#real-life-applications)
 - [Contributing](#contributing)
 - [License](#license)
 
 ### Installation
 
-To install the Monotonic Derivative library, cloent he repo (soon use pip:)
+To install the Monotonic Derivative library:
 
 ```
-       git clone https://github.com/A-Wpro/monotonic_derivative.git
-(soon) pip install monotonic-derivative
+pip install monotonic-derivative
 ```
 
 ### Usage
 
 First, import the `ensure_monotonic_derivative` function from the `monotonic_derivative` module:
 
 ```python
@@ -44,17 +43,33 @@
 ```python
 import numpy as np
 from monotonic_derivative import ensure_monotonic_derivative
 
 x = np.array([0, 1, 2, 3, 4, 5])
 y = np.array([100, 55, 53, 40, 35, 5])
 
-modified_y_positive = ensure_monotonic_derivative(x, y, degree=2, force_negative_derivative=False, verbose=True, save_plot=True)
+modified_y = ensure_monotonic_derivative(
+    x, y, degree=2, force_negative_derivative=True, verbose=True, save_plot=True)
 ```
 
+#### Result :
+
+We got a new curve that follow one rule : The Xth degree (depending of paramter degree) derivate must be increasing/decreasing (depending of force_negative_derivative parameter) curve.
+
+```
+#from
+y = [100, 55, 53, 40, 35, 5]
+#to
+modified_y = [99.78638543 56.7089208  48.94131484 44.05868538 33.29107987  5.21361543]
+```
+
+As you can see, slight change on y can totaly change how react the 2rd derivate.
+
+![Derivative Example](./images/derivative.png)
+
 ### Real-life Applications
 
 In many real-life scenarios, the collected data may produce curves that are not logical or do not follow the expected constraints. For example, the data representing the velocity of a car over time should show an increasing or decreasing acceleration, but due to measurement errors or other factors, the collected data points may not reflect this.
 
 The Monotonic Derivative library offers an easy solution to slightly modify the data to respect these constraints. By using this library, you can ensure that the specified degree derivative of the cubic spline is always monotonically increasing or decreasing, making your data analysis more accurate and reliable.
 
 ### Contributing
```

### Comparing `monotonic derivative-0.13/monotonic_derivative/monotonic_derivative.py` & `monotonic derivative-0.14/monotonic_derivative/monotonic_derivative.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,34 +1,36 @@
 import numpy as np
 from scipy.interpolate import CubicSpline
 from scipy.optimize import minimize
 import matplotlib.pyplot as plt
 from io import BytesIO
 import imageio
 
-def ensure_monotonic_derivative(x, y, degree=2, force_negative_derivative=False, verbose=False, save_plot=False):
+
+def ensure_monotonic_derivative(
+    x, y, degree=2, force_negative_derivative=False, verbose=False, save_plot=False
+):
     """
     Modify the given data points to ensure that the specified degree derivative of the cubic spline is always monotonically increasing or decreasing.
 
     Parameters:
     x: numpy array, the independent variable data points
     y: numpy array, the dependent variable data points
     degree: int, the degree of the derivative to check for monotonicity
     force_negative_derivative: bool, force the specified degree derivative to be monotonically decreasing if True
     verbose: bool, print additional information if True
     save_plot: bool, save the plots as GIF images if True
 
     Returns:
     modified_y: numpy array, the modified dependent variable data points
     """
-    
+
     def objective_function(y, x, y_original):
         return np.sum((y - y_original) ** 2)
 
-
     def constraint_second_derivative_increasing(y, x):
         """
         Function to create a constraint function to be used in the optimization problem.
         The constraint function calculates the minimum difference between consecutive second derivatives.
 
         Parameters:
         y: numpy array, the dependent variable data points
@@ -41,15 +43,14 @@
         def constraint(y):
             cs = CubicSpline(x, y)
             y_2nd_derivative = cs(x, 2)
             return np.min(np.diff(y_2nd_derivative))
 
         return constraint
 
-
     def constraint_second_derivative_decreasing(y, x):
         """
         Function to create a constraint function to be used in the optimization problem.
         The constraint function calculates the maximum difference between consecutive second derivatives.
 
         Parameters:
         y: numpy array, the dependent variable data points
@@ -61,28 +62,30 @@
 
         def constraint(y):
             cs = CubicSpline(x, y)
             y_2nd_derivative = cs(x, 2)
             return np.min(-np.diff(y_2nd_derivative))
 
         return constraint
-    
+
     # Check if x and y have the same length
     if len(x) != len(y):
         raise ValueError("x and y must have the same length")
     # Check if the specified degree is valid
     if degree >= len(y) - 1:
-        raise ValueError("Degree must be less than the length of the data minus 1, since we lose one data point for each derivative and need at least two data points")
+        raise ValueError(
+            "Degree must be less than the length of the data minus 1, since we lose one data point for each derivative and need at least two data points"
+        )
 
     # Define the constraint for the optimization problem
     if force_negative_derivative:
-        cons = {'type': 'ineq', 'fun': constraint_second_derivative_decreasing(y, x)}
+        cons = {"type": "ineq", "fun": constraint_second_derivative_decreasing(y, x)}
     else:
-        cons = {'type': 'ineq', 'fun': constraint_second_derivative_increasing(y, x)}
-    
+        cons = {"type": "ineq", "fun": constraint_second_derivative_increasing(y, x)}
+
     # Solve the optimization problem
     res = minimize(objective_function, y, args=(x, y), constraints=cons)
     modified_y = res.x
 
     if verbose:
         print("Original y    :", y)
         print("Modified y    :", modified_y)
@@ -101,16 +104,26 @@
         ax[0].legend()
 
         cs_original = CubicSpline(x, y)
         cs_modified = CubicSpline(x, modified_y)
 
         # Plot derivatives from 1st to the specified degree
         for d, ax_i in enumerate(ax[1:], start=1):
-            ax_i.plot(x[:-d], np.diff(y, n=d) / np.prod([np.diff(x) for _ in range(d)]), "o--", label=f"{d}th derivative (original)")
-            ax_i.plot(x[:-d], np.diff(modified_y, n=d) / np.prod([np.diff(x) for _ in range(d)]), "o--", label=f"{d}th derivative (modified)")
+            ax_i.plot(
+                x[:-d],
+                np.diff(y, n=d) / np.prod([np.diff(x) for _ in range(d)]),
+                "o--",
+                label=f"{d}th derivative (original)",
+            )
+            ax_i.plot(
+                x[:-d],
+                np.diff(modified_y, n=d) / np.prod([np.diff(x) for _ in range(d)]),
+                "o--",
+                label=f"{d}th derivative (modified)",
+            )
             ax_i.set_xlabel("x")
             ax_i.set_ylabel(f"{d}th derivative")
             ax_i.legend()
 
         plt.tight_layout()
 
         buf = BytesIO()
@@ -118,9 +131,8 @@
         buf.seek(0)
         image = imageio.imread(buf)
         plt.close(fig)
 
         # Save the image as a png
         imageio.imwrite("derivative.png", image)
 
-
     return modified_y
```

### Comparing `monotonic derivative-0.13/setup.py` & `monotonic derivative-0.14/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup
 
 setup(
     name="monotonic derivative",
-    version="0.13",
+    version="0.14",
     description="Monotonic Derivative is a Python library designed to modify real-life data to ensure that the specified degree derivative of the cubic spline is always monotonically increasing or decreasing. This library can be particularly useful in applications where the derivatives of the given data must follow specific monotonicity constraints, such as in scientific modeling or engineering applications.",
     author="Adam Wecker",
     packages=["monotonic_derivative"],
     install_requires=["numpy", "scipy", "matplotlib", "imageio"],
 )
```

