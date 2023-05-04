# Comparing `tmp/hgdl-2.0.6.tar.gz` & `tmp/hgdl-2.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hgdl-2.0.6.tar", last modified: Thu Feb  2 23:17:37 2023, max compression
+gzip compressed data, was "hgdl-2.0.7.tar", last modified: Thu May  4 18:26:58 2023, max compression
```

## Comparing `hgdl-2.0.6.tar` & `hgdl-2.0.7.tar`

### file list

```diff
@@ -1,32 +1,38 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-02 23:17:37.955564 hgdl-2.0.6/
--rw-r--r--   0 runner    (1001) docker     (123)      184 2023-02-02 23:17:29.000000 hgdl-2.0.6/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2421 2023-02-02 23:17:29.000000 hgdl-2.0.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-02-02 23:17:29.000000 hgdl-2.0.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2875 2023-02-02 23:17:37.955564 hgdl-2.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2388 2023-02-02 23:17:29.000000 hgdl-2.0.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-02 23:17:37.955564 hgdl-2.0.6/hgdl/
--rwxr-xr-x   0 runner    (1001) docker     (123)      133 2023-02-02 23:17:29.000000 hgdl-2.0.6/hgdl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-02-02 23:17:37.955564 hgdl-2.0.6/hgdl/_version.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1432 2023-02-02 23:17:29.000000 hgdl-2.0.6/hgdl/constraints.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-02 23:17:37.951564 hgdl-2.0.6/hgdl/global_methods/
--rwxr-xr-x   0 runner    (1001) docker     (123)      119 2023-02-02 23:17:29.000000 hgdl-2.0.6/hgdl/global_methods/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3668 2023-02-02 23:17:29.000000 hgdl-2.0.6/hgdl/global_methods/global_optimizer.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    21372 2023-02-02 23:17:29.000000 hgdl-2.0.6/hgdl/hgdl.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-02 23:17:37.955564 hgdl-2.0.6/hgdl/local_methods/
--rwxr-xr-x   0 runner    (1001) docker     (123)      119 2023-02-02 23:17:29.000000 hgdl-2.0.6/hgdl/local_methods/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2446 2023-02-02 23:17:29.000000 hgdl-2.0.6/hgdl/local_methods/bump_function.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1862 2023-02-02 23:17:29.000000 hgdl-2.0.6/hgdl/local_methods/dNewton.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4328 2023-02-02 23:17:29.000000 hgdl-2.0.6/hgdl/local_methods/local_optimizer.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      945 2023-02-02 23:17:29.000000 hgdl-2.0.6/hgdl/meta_data.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1016 2023-02-02 23:17:29.000000 hgdl-2.0.6/hgdl/misc.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    11124 2023-02-02 23:17:29.000000 hgdl-2.0.6/hgdl/optima.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1439 2023-02-02 23:17:29.000000 hgdl-2.0.6/hgdl/support_functions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-02 23:17:37.951564 hgdl-2.0.6/hgdl.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2875 2023-02-02 23:17:37.000000 hgdl-2.0.6/hgdl.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      559 2023-02-02 23:17:37.000000 hgdl-2.0.6/hgdl.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-02 23:17:37.000000 hgdl-2.0.6/hgdl.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-02-02 23:17:37.000000 hgdl-2.0.6/hgdl.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-02-02 23:17:37.000000 hgdl-2.0.6/hgdl.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      191 2023-02-02 23:17:37.955564 hgdl-2.0.6/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     2363 2023-02-02 23:17:29.000000 hgdl-2.0.6/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)    80044 2023-02-02 23:17:29.000000 hgdl-2.0.6/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 18:26:58.813543 hgdl-2.0.7/
+-rw-r--r--   0 runner    (1001) docker     (123)      184 2023-05-04 18:26:45.000000 hgdl-2.0.7/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2421 2023-05-04 18:26:45.000000 hgdl-2.0.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-04 18:26:45.000000 hgdl-2.0.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2875 2023-05-04 18:26:58.813543 hgdl-2.0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2388 2023-05-04 18:26:45.000000 hgdl-2.0.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 18:26:58.813543 hgdl-2.0.7/hgdl/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      133 2023-05-04 18:26:45.000000 hgdl-2.0.7/hgdl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-05-04 18:26:58.813543 hgdl-2.0.7/hgdl/_version.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1432 2023-05-04 18:26:45.000000 hgdl-2.0.7/hgdl/constraints.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 18:26:58.809543 hgdl-2.0.7/hgdl/global_methods/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      119 2023-05-04 18:26:45.000000 hgdl-2.0.7/hgdl/global_methods/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3668 2023-05-04 18:26:45.000000 hgdl-2.0.7/hgdl/global_methods/global_optimizer.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    21372 2023-05-04 18:26:45.000000 hgdl-2.0.7/hgdl/hgdl.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 18:26:58.813543 hgdl-2.0.7/hgdl/local_methods/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      119 2023-05-04 18:26:45.000000 hgdl-2.0.7/hgdl/local_methods/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2446 2023-05-04 18:26:45.000000 hgdl-2.0.7/hgdl/local_methods/bump_function.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1865 2023-05-04 18:26:45.000000 hgdl-2.0.7/hgdl/local_methods/dNewton.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4328 2023-05-04 18:26:45.000000 hgdl-2.0.7/hgdl/local_methods/local_optimizer.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      945 2023-05-04 18:26:45.000000 hgdl-2.0.7/hgdl/meta_data.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1016 2023-05-04 18:26:45.000000 hgdl-2.0.7/hgdl/misc.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    11124 2023-05-04 18:26:45.000000 hgdl-2.0.7/hgdl/optima.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1439 2023-05-04 18:26:45.000000 hgdl-2.0.7/hgdl/support_functions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 18:26:58.809543 hgdl-2.0.7/hgdl.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2875 2023-05-04 18:26:58.000000 hgdl-2.0.7/hgdl.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      684 2023-05-04 18:26:58.000000 hgdl-2.0.7/hgdl.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 18:26:58.000000 hgdl-2.0.7/hgdl.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-05-04 18:26:58.000000 hgdl-2.0.7/hgdl.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-04 18:26:58.000000 hgdl-2.0.7/hgdl.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      191 2023-05-04 18:26:58.813543 hgdl-2.0.7/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2363 2023-05-04 18:26:45.000000 hgdl-2.0.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 18:26:58.813543 hgdl-2.0.7/tests/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      937 2023-05-04 18:26:45.000000 hgdl-2.0.7/tests/test_non_diff.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1339 2023-05-04 18:26:45.000000 hgdl-2.0.7/tests/test_rosenbrock.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1219 2023-05-04 18:26:45.000000 hgdl-2.0.7/tests/test_schwefel.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1215 2023-05-04 18:26:45.000000 hgdl-2.0.7/tests/test_schwefel_BFGS.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1213 2023-05-04 18:26:45.000000 hgdl-2.0.7/tests/test_schwefel_CG.py
+-rw-r--r--   0 runner    (1001) docker     (123)    80044 2023-05-04 18:26:45.000000 hgdl-2.0.7/versioneer.py
```

### Comparing `hgdl-2.0.6/LICENSE` & `hgdl-2.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `hgdl-2.0.6/PKG-INFO` & `hgdl-2.0.7/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hgdl
-Version: 2.0.6
+Version: 2.0.7
 Summary: HGDL Optimization
 Home-page: https://github.com//hgdl
 Author: David Perryman, Marcus Noack
 Author-email: MarcusNoack@lbl.gov
 License: BSD3
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Natural Language :: English
```

### Comparing `hgdl-2.0.6/README.md` & `hgdl-2.0.7/README.md`

 * *Files identical despite different names*

### Comparing `hgdl-2.0.6/hgdl/constraints.py` & `hgdl-2.0.7/hgdl/constraints.py`

 * *Files identical despite different names*

### Comparing `hgdl-2.0.6/hgdl/global_methods/global_optimizer.py` & `hgdl-2.0.7/hgdl/global_methods/global_optimizer.py`

 * *Files identical despite different names*

### Comparing `hgdl-2.0.6/hgdl/hgdl.py` & `hgdl-2.0.7/hgdl/hgdl.py`

 * *Files identical despite different names*

### Comparing `hgdl-2.0.6/hgdl/local_methods/bump_function.py` & `hgdl-2.0.7/hgdl/local_methods/bump_function.py`

 * *Files identical despite different names*

### Comparing `hgdl-2.0.6/hgdl/local_methods/dNewton.py` & `hgdl-2.0.7/hgdl/local_methods/dNewton.py`

 * *Files 8% similar despite different names*

```diff
@@ -23,17 +23,17 @@
         try: gamma = np.linalg.solve(hessian,-gradient)
         except Exception as error: gamma,a,b,c = np.linalg.lstsq(hessian,-gradient,rcond=None)
         if any(gamma == np.nan) or any(gamma == np.inf): return x,func(x, *args),gradient,np.linalg.eig(hess(x, *args))[0], False
         x += gamma
         e = np.max(abs(gamma))
         logger.debug("dNewton step size: ", e, " max gradient: ",np.max(abs(gradient)))
         #print("dNewton step size: ", e, " max gradient: ",np.max(abs(gradient)))
-        if counter > max_iter: return x,func(x, *args),gradient,np.linalg.eig(hess(x, *args))[0], False, "max_iter reached"
+        if counter > max_iter: return x,func(x, *args),gradient,np.linalg.eig(hess(x, *args))[0], False#, "max_iter reached"
         counter += 1
-    return x,func(x, *args),gradient,np.linalg.eig(hess(x, *args))[0], True, "converged"
+    return x,func(x, *args),gradient,np.linalg.eig(hess(x, *args))[0], True #, "converged"
 
 
 
 def approximate_hessian(x, grad, *args):
     ##implements a first-order approximation
     len_x = len(x)
     hess = np.zeros((len_x,len_x))
```

### Comparing `hgdl-2.0.6/hgdl/local_methods/local_optimizer.py` & `hgdl-2.0.7/hgdl/local_methods/local_optimizer.py`

 * *Files identical despite different names*

### Comparing `hgdl-2.0.6/hgdl/meta_data.py` & `hgdl-2.0.7/hgdl/meta_data.py`

 * *Files identical despite different names*

### Comparing `hgdl-2.0.6/hgdl/misc.py` & `hgdl-2.0.7/hgdl/misc.py`

 * *Files identical despite different names*

### Comparing `hgdl-2.0.6/hgdl/optima.py` & `hgdl-2.0.7/hgdl/optima.py`

 * *Files identical despite different names*

### Comparing `hgdl-2.0.6/hgdl/support_functions.py` & `hgdl-2.0.7/hgdl/support_functions.py`

 * *Files identical despite different names*

### Comparing `hgdl-2.0.6/hgdl.egg-info/PKG-INFO` & `hgdl-2.0.7/hgdl.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hgdl
-Version: 2.0.6
+Version: 2.0.7
 Summary: HGDL Optimization
 Home-page: https://github.com//hgdl
 Author: David Perryman, Marcus Noack
 Author-email: MarcusNoack@lbl.gov
 License: BSD3
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Natural Language :: English
```

### Comparing `hgdl-2.0.6/hgdl.egg-info/SOURCES.txt` & `hgdl-2.0.7/hgdl.egg-info/SOURCES.txt`

 * *Files 17% similar despite different names*

```diff
@@ -19,8 +19,13 @@
 hgdl.egg-info/requires.txt
 hgdl.egg-info/top_level.txt
 hgdl/global_methods/__init__.py
 hgdl/global_methods/global_optimizer.py
 hgdl/local_methods/__init__.py
 hgdl/local_methods/bump_function.py
 hgdl/local_methods/dNewton.py
-hgdl/local_methods/local_optimizer.py
+hgdl/local_methods/local_optimizer.py
+tests/test_non_diff.py
+tests/test_rosenbrock.py
+tests/test_schwefel.py
+tests/test_schwefel_BFGS.py
+tests/test_schwefel_CG.py
```

### Comparing `hgdl-2.0.6/setup.py` & `hgdl-2.0.7/setup.py`

 * *Files identical despite different names*

### Comparing `hgdl-2.0.6/versioneer.py` & `hgdl-2.0.7/versioneer.py`

 * *Files identical despite different names*

