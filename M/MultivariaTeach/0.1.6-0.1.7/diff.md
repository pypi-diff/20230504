# Comparing `tmp/MultivariaTeach-0.1.6.tar.gz` & `tmp/MultivariaTeach-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "MultivariaTeach-0.1.6.tar", last modified: Tue May  2 21:32:47 2023, max compression
+gzip compressed data, was "MultivariaTeach-0.1.7.tar", last modified: Thu May  4 16:52:27 2023, max compression
```

## Comparing `MultivariaTeach-0.1.6.tar` & `MultivariaTeach-0.1.7.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwx------   0 ben        (501) staff       (20)        0 2023-05-02 21:32:47.749146 MultivariaTeach-0.1.6/
--rw-------   0 ben        (501) staff       (20)      743 2023-04-25 22:03:04.000000 MultivariaTeach-0.1.6/LICENSE
-drwx------   0 ben        (501) staff       (20)        0 2023-05-02 21:32:47.747702 MultivariaTeach-0.1.6/MultivariaTeach.egg-info/
--rw-------   0 ben        (501) staff       (20)    15366 2023-05-02 21:32:47.000000 MultivariaTeach-0.1.6/MultivariaTeach.egg-info/PKG-INFO
--rw-------   0 ben        (501) staff       (20)      330 2023-05-02 21:32:47.000000 MultivariaTeach-0.1.6/MultivariaTeach.egg-info/SOURCES.txt
--rw-------   0 ben        (501) staff       (20)        1 2023-05-02 21:32:47.000000 MultivariaTeach-0.1.6/MultivariaTeach.egg-info/dependency_links.txt
--rw-------   0 ben        (501) staff       (20)       41 2023-05-02 21:32:47.000000 MultivariaTeach-0.1.6/MultivariaTeach.egg-info/requires.txt
--rw-------   0 ben        (501) staff       (20)       22 2023-05-02 21:32:47.000000 MultivariaTeach-0.1.6/MultivariaTeach.egg-info/top_level.txt
--rw-------   0 ben        (501) staff       (20)    15366 2023-05-02 21:32:47.748999 MultivariaTeach-0.1.6/PKG-INFO
--rw-------   0 ben        (501) staff       (20)    14698 2023-05-02 21:32:06.000000 MultivariaTeach-0.1.6/README.md
-drwx------   0 ben        (501) staff       (20)        0 2023-05-02 21:32:47.748102 MultivariaTeach-0.1.6/multivariateach/
--rw-------   0 ben        (501) staff       (20)       31 2023-05-02 20:33:56.000000 MultivariaTeach-0.1.6/multivariateach/__init__.py
--rw-------   0 ben        (501) staff       (20)    11161 2023-05-01 19:52:12.000000 MultivariaTeach-0.1.6/multivariateach/multivariateach.py
--rw-------   0 ben        (501) staff       (20)       38 2023-05-02 21:32:47.749182 MultivariaTeach-0.1.6/setup.cfg
--rw-------   0 ben        (501) staff       (20)      932 2023-05-02 21:32:38.000000 MultivariaTeach-0.1.6/setup.py
-drwx------   0 ben        (501) staff       (20)        0 2023-05-02 21:32:47.748569 MultivariaTeach-0.1.6/tests/
--rw-------   0 ben        (501) staff       (20)        0 2023-04-25 22:05:08.000000 MultivariaTeach-0.1.6/tests/__init__.py
--rw-------   0 ben        (501) staff       (20)     7016 2023-05-01 22:22:43.000000 MultivariaTeach-0.1.6/tests/test_multivariteach.py
+drwx------   0 ben        (501) staff       (20)        0 2023-05-04 16:52:27.096936 MultivariaTeach-0.1.7/
+-rw-------   0 ben        (501) staff       (20)      743 2023-04-25 22:03:04.000000 MultivariaTeach-0.1.7/LICENSE
+drwx------   0 ben        (501) staff       (20)        0 2023-05-04 16:52:27.095703 MultivariaTeach-0.1.7/MultivariaTeach.egg-info/
+-rw-------   0 ben        (501) staff       (20)    25739 2023-05-04 16:52:27.000000 MultivariaTeach-0.1.7/MultivariaTeach.egg-info/PKG-INFO
+-rw-------   0 ben        (501) staff       (20)      330 2023-05-04 16:52:27.000000 MultivariaTeach-0.1.7/MultivariaTeach.egg-info/SOURCES.txt
+-rw-------   0 ben        (501) staff       (20)        1 2023-05-04 16:52:27.000000 MultivariaTeach-0.1.7/MultivariaTeach.egg-info/dependency_links.txt
+-rw-------   0 ben        (501) staff       (20)       41 2023-05-04 16:52:27.000000 MultivariaTeach-0.1.7/MultivariaTeach.egg-info/requires.txt
+-rw-------   0 ben        (501) staff       (20)       22 2023-05-04 16:52:27.000000 MultivariaTeach-0.1.7/MultivariaTeach.egg-info/top_level.txt
+-rw-------   0 ben        (501) staff       (20)    25739 2023-05-04 16:52:27.096812 MultivariaTeach-0.1.7/PKG-INFO
+-rw-------   0 ben        (501) staff       (20)    25071 2023-05-04 16:51:38.000000 MultivariaTeach-0.1.7/README.md
+drwx------   0 ben        (501) staff       (20)        0 2023-05-04 16:52:27.096042 MultivariaTeach-0.1.7/multivariateach/
+-rw-------   0 ben        (501) staff       (20)       31 2023-05-02 20:33:56.000000 MultivariaTeach-0.1.7/multivariateach/__init__.py
+-rw-------   0 ben        (501) staff       (20)    11161 2023-05-04 15:08:09.000000 MultivariaTeach-0.1.7/multivariateach/multivariateach.py
+-rw-------   0 ben        (501) staff       (20)       38 2023-05-04 16:52:27.096975 MultivariaTeach-0.1.7/setup.cfg
+-rw-------   0 ben        (501) staff       (20)      932 2023-05-04 15:11:19.000000 MultivariaTeach-0.1.7/setup.py
+drwx------   0 ben        (501) staff       (20)        0 2023-05-04 16:52:27.096345 MultivariaTeach-0.1.7/tests/
+-rw-------   0 ben        (501) staff       (20)        0 2023-04-25 22:05:08.000000 MultivariaTeach-0.1.7/tests/__init__.py
+-rw-------   0 ben        (501) staff       (20)     7016 2023-05-01 22:22:43.000000 MultivariaTeach-0.1.7/tests/test_multivariteach.py
```

### Comparing `MultivariaTeach-0.1.6/LICENSE` & `MultivariaTeach-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `MultivariaTeach-0.1.6/multivariateach/multivariateach.py` & `MultivariaTeach-0.1.7/multivariateach/multivariateach.py`

 * *Files 0% similar despite different names*

```diff
@@ -204,15 +204,15 @@
 
 def mauchly(X, Y):
     """
     X: model (column of ones followed by ``dummies'' for groups)
     Y: data (rows must match X)
     """
 
-    n = X.shape[1]
+    n = Y.shape[1]
     degree = n - 1
     M = orthopolynomial_contrasts(n, degree)
     S_p = calculate_pooled_covariance_matrix(X, Y)
 
     k = M.shape[1]
     lsl_matrix = M.T @ S_p @ M
     determinant = np.linalg.det(lsl_matrix)
```

### Comparing `MultivariaTeach-0.1.6/setup.py` & `MultivariaTeach-0.1.7/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="MultivariaTeach",
-    version="0.1.6",
+    version="0.1.7",
     description="A collection of tools intended for students of multivariate analysis",
     long_description=open("README.md", "r").read(),
     long_description_content_type="text/markdown",
     author="Ben Goren",
     author_email="bgoren@asu.edu",
     url="https://github.com/Ben-Goren/MultivariaTeach",
     packages=find_packages(),
```

### Comparing `MultivariaTeach-0.1.6/tests/test_multivariteach.py` & `MultivariaTeach-0.1.7/tests/test_multivariteach.py`

 * *Files identical despite different names*

