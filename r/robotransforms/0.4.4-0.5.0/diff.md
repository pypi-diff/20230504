# Comparing `tmp/robotransforms-0.4.4.tar.gz` & `tmp/robotransforms-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "robotransforms-0.4.4.tar", last modified: Tue Mar  7 02:56:27 2023, max compression
+gzip compressed data, was "robotransforms-0.5.0.tar", last modified: Wed May  3 23:32:00 2023, max compression
```

## Comparing `robotransforms-0.4.4.tar` & `robotransforms-0.5.0.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxrwxr-x   0 jonathan  (1001) jonathan  (1001)        0 2023-03-07 02:56:27.476563 robotransforms-0.4.4/
--rw-rw-r--   0 jonathan  (1001) jonathan  (1001)     1076 2022-12-01 23:55:43.000000 robotransforms-0.4.4/LICENSE
--rw-rw-r--   0 jonathan  (1001) jonathan  (1001)       37 2022-12-02 15:43:21.000000 robotransforms-0.4.4/MANIFEST.in
--rw-rw-r--   0 jonathan  (1001) jonathan  (1001)      670 2023-03-07 02:56:27.472563 robotransforms-0.4.4/PKG-INFO
--rw-rw-r--   0 jonathan  (1001) jonathan  (1001)      347 2023-01-07 23:35:03.000000 robotransforms-0.4.4/README.md
--rw-rw-r--   0 jonathan  (1001) jonathan  (1001)       60 2022-12-02 17:09:02.000000 robotransforms-0.4.4/pyproject.toml
-drwxrwxr-x   0 jonathan  (1001) jonathan  (1001)        0 2023-03-07 02:56:27.468563 robotransforms-0.4.4/robotransforms/
--rw-rw-r--   0 jonathan  (1001) jonathan  (1001)      148 2022-12-02 15:43:21.000000 robotransforms-0.4.4/robotransforms/__init__.py
--rw-rw-r--   0 jonathan  (1001) jonathan  (1001)       22 2023-03-07 00:45:08.000000 robotransforms-0.4.4/robotransforms/_version.py
-drwxrwxr-x   0 jonathan  (1001) jonathan  (1001)        0 2023-03-07 02:56:27.472563 robotransforms-0.4.4/robotransforms/dead_reckon/
--rw-rw-r--   0 jonathan  (1001) jonathan  (1001)       67 2022-12-02 15:43:21.000000 robotransforms-0.4.4/robotransforms/dead_reckon/__init__.py
--rw-rw-r--   0 jonathan  (1001) jonathan  (1001)     7533 2022-12-06 17:31:27.000000 robotransforms-0.4.4/robotransforms/dead_reckon/base.cpp
--rw-rw-r--   0 jonathan  (1001) jonathan  (1001)      732 2022-12-02 15:43:21.000000 robotransforms-0.4.4/robotransforms/dead_reckon/base.h
--rw-rw-r--   0 jonathan  (1001) jonathan  (1001)     2811 2023-03-07 00:07:47.000000 robotransforms-0.4.4/robotransforms/dead_reckon/dead_reckon.py
--rw-rw-r--   0 jonathan  (1001) jonathan  (1001)     6743 2022-12-06 17:31:00.000000 robotransforms-0.4.4/robotransforms/dead_reckon/dead_reckon_pure.py
--rw-rw-r--   0 jonathan  (1001) jonathan  (1001)    15825 2023-03-07 00:44:08.000000 robotransforms-0.4.4/robotransforms/dead_reckon/wrapper.cpp
-drwxrwxr-x   0 jonathan  (1001) jonathan  (1001)        0 2023-03-07 02:56:27.472563 robotransforms-0.4.4/robotransforms/euclidean/
--rw-rw-r--   0 jonathan  (1001) jonathan  (1001)      120 2022-12-02 15:43:21.000000 robotransforms-0.4.4/robotransforms/euclidean/__init__.py
--rw-rw-r--   0 jonathan  (1001) jonathan  (1001)     4727 2022-12-02 16:35:14.000000 robotransforms-0.4.4/robotransforms/euclidean/base.cpp
--rw-rw-r--   0 jonathan  (1001) jonathan  (1001)      992 2022-12-02 15:43:21.000000 robotransforms-0.4.4/robotransforms/euclidean/base.h
--rw-rw-r--   0 jonathan  (1001) jonathan  (1001)    10382 2022-12-02 15:43:21.000000 robotransforms-0.4.4/robotransforms/euclidean/euclidean.py
--rw-rw-r--   0 jonathan  (1001) jonathan  (1001)    10691 2022-12-02 15:43:21.000000 robotransforms-0.4.4/robotransforms/euclidean/euclidean_pure.py
--rw-rw-r--   0 jonathan  (1001) jonathan  (1001)     5906 2023-03-07 00:29:02.000000 robotransforms-0.4.4/robotransforms/euclidean/wrapper.cpp
-drwxrwxr-x   0 jonathan  (1001) jonathan  (1001)        0 2023-03-07 02:56:27.472563 robotransforms-0.4.4/robotransforms/utils/
--rw-rw-r--   0 jonathan  (1001) jonathan  (1001)       55 2022-12-02 15:43:21.000000 robotransforms-0.4.4/robotransforms/utils/__init__.py
--rw-rw-r--   0 jonathan  (1001) jonathan  (1001)     3680 2022-12-02 19:58:46.000000 robotransforms-0.4.4/robotransforms/utils/base.cpp
--rw-rw-r--   0 jonathan  (1001) jonathan  (1001)      351 2022-12-02 15:43:21.000000 robotransforms-0.4.4/robotransforms/utils/base.h
--rw-rw-r--   0 jonathan  (1001) jonathan  (1001)      545 2022-12-02 15:43:21.000000 robotransforms-0.4.4/robotransforms/utils/utils.py
--rw-rw-r--   0 jonathan  (1001) jonathan  (1001)     1055 2022-12-02 15:43:21.000000 robotransforms-0.4.4/robotransforms/utils/utils_pure.py
--rw-rw-r--   0 jonathan  (1001) jonathan  (1001)     6290 2022-12-02 15:43:21.000000 robotransforms-0.4.4/robotransforms/utils/wrapper.cpp
-drwxrwxr-x   0 jonathan  (1001) jonathan  (1001)        0 2023-03-07 02:56:27.472563 robotransforms-0.4.4/robotransforms.egg-info/
--rw-rw-r--   0 jonathan  (1001) jonathan  (1001)      670 2023-03-07 02:56:27.000000 robotransforms-0.4.4/robotransforms.egg-info/PKG-INFO
--rw-rw-r--   0 jonathan  (1001) jonathan  (1001)      943 2023-03-07 02:56:27.000000 robotransforms-0.4.4/robotransforms.egg-info/SOURCES.txt
--rw-rw-r--   0 jonathan  (1001) jonathan  (1001)        1 2023-03-07 02:56:27.000000 robotransforms-0.4.4/robotransforms.egg-info/dependency_links.txt
--rw-rw-r--   0 jonathan  (1001) jonathan  (1001)       12 2023-03-07 02:56:27.000000 robotransforms-0.4.4/robotransforms.egg-info/requires.txt
--rw-rw-r--   0 jonathan  (1001) jonathan  (1001)       67 2023-03-07 02:56:27.000000 robotransforms-0.4.4/robotransforms.egg-info/top_level.txt
--rw-rw-r--   0 jonathan  (1001) jonathan  (1001)       38 2023-03-07 02:56:27.476563 robotransforms-0.4.4/setup.cfg
--rw-rw-r--   0 jonathan  (1001) jonathan  (1001)     1907 2022-12-02 17:09:02.000000 robotransforms-0.4.4/setup.py
+drwxrwxr-x   0 jonathan  (1001) jonathan  (1001)        0 2023-05-03 23:31:59.998098 robotransforms-0.5.0/
+-rw-rw-r--   0 jonathan  (1001) jonathan  (1001)     1076 2022-12-01 23:55:43.000000 robotransforms-0.5.0/LICENSE
+-rw-rw-r--   0 jonathan  (1001) jonathan  (1001)       37 2022-12-02 15:43:21.000000 robotransforms-0.5.0/MANIFEST.in
+-rw-rw-r--   0 jonathan  (1001) jonathan  (1001)      670 2023-05-03 23:31:59.998098 robotransforms-0.5.0/PKG-INFO
+-rw-rw-r--   0 jonathan  (1001) jonathan  (1001)      347 2023-05-03 23:31:19.000000 robotransforms-0.5.0/README.md
+-rw-rw-r--   0 jonathan  (1001) jonathan  (1001)       60 2022-12-02 17:09:02.000000 robotransforms-0.5.0/pyproject.toml
+drwxrwxr-x   0 jonathan  (1001) jonathan  (1001)        0 2023-05-03 23:31:59.990098 robotransforms-0.5.0/robotransforms/
+-rw-rw-r--   0 jonathan  (1001) jonathan  (1001)      148 2022-12-02 15:43:21.000000 robotransforms-0.5.0/robotransforms/__init__.py
+-rw-rw-r--   0 jonathan  (1001) jonathan  (1001)       22 2023-05-03 23:29:40.000000 robotransforms-0.5.0/robotransforms/_version.py
+drwxrwxr-x   0 jonathan  (1001) jonathan  (1001)        0 2023-05-03 23:31:59.994098 robotransforms-0.5.0/robotransforms/dead_reckon/
+-rw-rw-r--   0 jonathan  (1001) jonathan  (1001)       67 2022-12-02 15:43:21.000000 robotransforms-0.5.0/robotransforms/dead_reckon/__init__.py
+-rw-rw-r--   0 jonathan  (1001) jonathan  (1001)     8894 2023-05-03 23:28:26.000000 robotransforms-0.5.0/robotransforms/dead_reckon/base.cpp
+-rw-rw-r--   0 jonathan  (1001) jonathan  (1001)      732 2022-12-02 15:43:21.000000 robotransforms-0.5.0/robotransforms/dead_reckon/base.h
+-rw-rw-r--   0 jonathan  (1001) jonathan  (1001)     2811 2023-03-07 00:07:47.000000 robotransforms-0.5.0/robotransforms/dead_reckon/dead_reckon.py
+-rw-rw-r--   0 jonathan  (1001) jonathan  (1001)     6684 2023-05-03 23:28:26.000000 robotransforms-0.5.0/robotransforms/dead_reckon/dead_reckon_pure.py
+-rw-rw-r--   0 jonathan  (1001) jonathan  (1001)    15825 2023-03-07 00:44:08.000000 robotransforms-0.5.0/robotransforms/dead_reckon/wrapper.cpp
+drwxrwxr-x   0 jonathan  (1001) jonathan  (1001)        0 2023-05-03 23:31:59.994098 robotransforms-0.5.0/robotransforms/euclidean/
+-rw-rw-r--   0 jonathan  (1001) jonathan  (1001)      120 2022-12-02 15:43:21.000000 robotransforms-0.5.0/robotransforms/euclidean/__init__.py
+-rw-rw-r--   0 jonathan  (1001) jonathan  (1001)     8310 2023-05-03 23:28:26.000000 robotransforms-0.5.0/robotransforms/euclidean/base.cpp
+-rw-rw-r--   0 jonathan  (1001) jonathan  (1001)     1566 2023-05-03 23:28:26.000000 robotransforms-0.5.0/robotransforms/euclidean/base.h
+-rw-rw-r--   0 jonathan  (1001) jonathan  (1001)    11585 2023-05-03 23:28:26.000000 robotransforms-0.5.0/robotransforms/euclidean/euclidean.py
+-rw-rw-r--   0 jonathan  (1001) jonathan  (1001)    14304 2023-05-03 23:28:26.000000 robotransforms-0.5.0/robotransforms/euclidean/euclidean_pure.py
+-rw-rw-r--   0 jonathan  (1001) jonathan  (1001)     6960 2023-05-03 23:28:26.000000 robotransforms-0.5.0/robotransforms/euclidean/wrapper.cpp
+drwxrwxr-x   0 jonathan  (1001) jonathan  (1001)        0 2023-05-03 23:31:59.998098 robotransforms-0.5.0/robotransforms/utils/
+-rw-rw-r--   0 jonathan  (1001) jonathan  (1001)       55 2022-12-02 15:43:21.000000 robotransforms-0.5.0/robotransforms/utils/__init__.py
+-rw-rw-r--   0 jonathan  (1001) jonathan  (1001)     3680 2022-12-02 19:58:46.000000 robotransforms-0.5.0/robotransforms/utils/base.cpp
+-rw-rw-r--   0 jonathan  (1001) jonathan  (1001)      351 2022-12-02 15:43:21.000000 robotransforms-0.5.0/robotransforms/utils/base.h
+-rw-rw-r--   0 jonathan  (1001) jonathan  (1001)      545 2022-12-02 15:43:21.000000 robotransforms-0.5.0/robotransforms/utils/utils.py
+-rw-rw-r--   0 jonathan  (1001) jonathan  (1001)     1055 2022-12-02 15:43:21.000000 robotransforms-0.5.0/robotransforms/utils/utils_pure.py
+-rw-rw-r--   0 jonathan  (1001) jonathan  (1001)     6290 2022-12-02 15:43:21.000000 robotransforms-0.5.0/robotransforms/utils/wrapper.cpp
+drwxrwxr-x   0 jonathan  (1001) jonathan  (1001)        0 2023-05-03 23:31:59.990098 robotransforms-0.5.0/robotransforms.egg-info/
+-rw-rw-r--   0 jonathan  (1001) jonathan  (1001)      670 2023-05-03 23:31:59.000000 robotransforms-0.5.0/robotransforms.egg-info/PKG-INFO
+-rw-rw-r--   0 jonathan  (1001) jonathan  (1001)      943 2023-05-03 23:31:59.000000 robotransforms-0.5.0/robotransforms.egg-info/SOURCES.txt
+-rw-rw-r--   0 jonathan  (1001) jonathan  (1001)        1 2023-05-03 23:31:59.000000 robotransforms-0.5.0/robotransforms.egg-info/dependency_links.txt
+-rw-rw-r--   0 jonathan  (1001) jonathan  (1001)       12 2023-05-03 23:31:59.000000 robotransforms-0.5.0/robotransforms.egg-info/requires.txt
+-rw-rw-r--   0 jonathan  (1001) jonathan  (1001)       67 2023-05-03 23:31:59.000000 robotransforms-0.5.0/robotransforms.egg-info/top_level.txt
+-rw-rw-r--   0 jonathan  (1001) jonathan  (1001)       38 2023-05-03 23:31:59.998098 robotransforms-0.5.0/setup.cfg
+-rw-rw-r--   0 jonathan  (1001) jonathan  (1001)     1907 2022-12-02 17:09:02.000000 robotransforms-0.5.0/setup.py
```

### Comparing `robotransforms-0.4.4/LICENSE` & `robotransforms-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `robotransforms-0.4.4/PKG-INFO` & `robotransforms-0.5.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: robotransforms
-Version: 0.4.4
+Version: 0.5.0
 Summary: A transformation library for robot motion
 Home-page: https://github.com/Nova-Dynamics/transforms-python
 Author: Jonathan D. B. Van Schenck
 Author-email: jvschenck@novadynamics.com
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `robotransforms-0.4.4/robotransforms/dead_reckon/base.cpp` & `robotransforms-0.5.0/robotransforms/dead_reckon/base.cpp`

 * *Files 7% similar despite different names*

```diff
@@ -71,21 +71,21 @@
         out[2] = ddr*ddr + 1e-8;
     }
 
     int dead_reckon_apply(double* step, double *x, double *cov) {
         if ( step[1] == 0 && step[2] == 0 ) return 1;
         // Create extended state vector as state + dl + dr
         double z[ESS] = {
-            x[0],
-            x[1],
-            x[2],
-            x[3],
-            x[4],
-            x[5],
-            x[6],
+            x[0],    // x
+            x[1],    // y
+            x[2],    // z
+            x[3],    // a
+            x[4],    // b
+            x[5],    // c
+            x[6],    // d
             step[1], // dl
             step[2], // dr
         };
 
         double dr_cov[3];
         dead_reckon_step_errors(
                 step[1], step[2], // dl, dr
@@ -113,78 +113,117 @@
         double Z[(2*L+1)*n];
         for ( int i = 0; i < n; i ++ ) {
             Z[0*n + i] = z[i]; // copy in mean
         }
         // Attempt to square-root the scaled covariance
         double R[L*L];
         if ( !utils::cholesky( L, L_PLUS_LAMBDA, P_z, R ) ) return 0;
-        
+
         for ( int i = 0; i < L; i ++ ) {
             // Extract and lrQ from the ith row of the root covariance (which is a manifold deviation)
-            double dlrQ[7], idlrQ[7];
-            euclidean::convert_lrq_to_lrQ(&R[i*L], dlrQ);
-            euclidean::invert_lrQ(dlrQ, idlrQ);
+            double dlrQ1[SS], dlrQ2[SS], R_neg_row[SM];
+            for ( int j = 0; j < SM; j++ ) {
+                R_neg_row[j] = -R[i*L + j];
+            }
+            euclidean::convert_lrrv_to_lrQ(&R[i*L], dlrQ1);
+            euclidean::convert_lrrv_to_lrQ(R_neg_row, dlrQ2);
 
             // Write into the the sigma point the difference
-            euclidean::compose_lrQ(z, dlrQ,  &Z[(i+1)*n]);
-            euclidean::compose_lrQ(z, idlrQ, &Z[(i+L+1)*n]);
-
+            euclidean::compose_lrQ(z, dlrQ1,  &Z[(i+1)*n]);
+            euclidean::compose_lrQ(z, dlrQ2, &Z[(i+L+1)*n]);
 
             // Also add in the last two elements
             Z[(i+1)*n + SS + 0] = z[SS + 0] + R[i*L + SM + 0];
             Z[(i+1)*n + SS + 1] = z[SS + 1] + R[i*L + SM + 1];
             Z[(i+L+1)*n + SS + 0] = z[SS + 0] - R[i*L + SM + 0];
             Z[(i+L+1)*n + SS + 1] = z[SS + 1] - R[i*L + SM + 1];
         }
 
         // Transform the sigma points
-        double Y[(2*L+1)*3];
+        double Y[(2*L+1)*SS];
         for ( int i = 0; i < 2*L+1; i ++ ) {
             dead_reckon_step(
                 &Z[i*n + 3], //quat
                 z[SS + 0],   // dl
                 z[SS + 1],   // dr
                 step[7],     // vave
                 step[8],     // vave
-                &Y[i*3]
+                &Y[i*SS]     // delta change
             );
             for ( int j = 0; j < 3; j ++ ) {
-                Y[i*3 + j] += Z[i*n + j];
+                Y[i*SS + j] += Z[i*n + j]; // add initial value
             }
+            // Write over the quaternion part with the new quaterion estimate
+            euclidean::compose_quat(&Z[i*n + 3], &step[3], &Y[i*SS + 3]);
         }
 
-        // Note, this probably only works becuase we have neglected the quat -- not sure how to average on the manifold....
-        double y[3], y_cov[3*3];
-        utils::GRV_statistics(3, L, Y, y, y_cov);
+        // Iteratively calculate the lrQ mean
+        // Copy Y[0] as my initial guess for y_bar
+        double y_bar[SS];
+        for ( int i = 0; i < SS; i++ ) {
+            y_bar[i] = Y[i];
+        }
+        double EPS = 1e-20;
+        int MAX = 100;
+        int i = 0;
+        double LAMBDA = 3. - L;
+        double W0 = LAMBDA / 3.;
+        double W = 1. / ( 2. * 3. );
+        double sq_error = 1.;
+        double y_bar_inv[SS];
+        double dY[(2*L+1)*SM];
+        double dlrQ[SS];
+        while ( i < MAX && sq_error > EPS ) {
+            i += 1;
+            euclidean::invert_lrQ(y_bar, y_bar_inv);
+            for ( int i = 0; i < 2*L+1; i ++ ) {
+                euclidean::compose_lrQ(y_bar_inv, &Y[i*SS], dlrQ);
+                euclidean::convert_lrQ_to_lrrv(dlrQ, &dY[i*SM]);
+            }
+
+            double e[SM];
+            for ( int i = 0; i < SM; i ++ ) {
+                e[i] = dY[i]*W0;
+            }
+            for ( int j = 1; j < 2*L+1; j ++ ) {
+                for ( int i = 0; i < SM; i ++ ) {
+                    e[i] += dY[j*SM + i]*W;
+                }
+            }
 
+            sq_error = 0;
+            for ( int i = 0; i < SM; i ++ ) {
+                sq_error += e[i]*e[i];
+            }
 
-        // Update state and covarience
-        x[0] = Y[0]; // use mean transform
-        x[1] = Y[1]; // use mean transform
-        x[2] = Y[2]; // use mean transform
-        double quat[4];
-        euclidean::compose_quat(&x[3], &step[3], quat); // accumulate difference along manifold
-        x[3] = quat[0];
-        x[4] = quat[1];
-        x[5] = quat[2];
-        x[6] = quat[3];
+            euclidean::convert_lrrv_to_lrQ(e, dlrQ);
+            euclidean::compose_lrQ(y_bar, dlrQ, y_bar_inv);
+            for ( int i = 0; i < SS; i ++ ) {
+                y_bar[i] = y_bar_inv[i];
+            }
+        }
 
-        for ( int i = 0; i < 3; i ++ ) {
-            for ( int j = 0; j < 3; j ++ ) {
-                cov[i*SM + j] = y_cov[i*3 + j];
+        // Update the covariance
+        int k = 0;
+        for ( int i = 0; i < SM; i ++ ) {
+            for ( int j = 0; j < SM; j ++ ) {
+                cov[i*SM + j] = W0 * dY[k*SM + i] * dY[k*SM + j];
             }
         }
-        for ( int i = 0; i < 3; i ++ ) {
-            for ( int j = 3; j < SM; j ++ ) {
-                cov[i*SM + j] = 0;
-                cov[j*SM + i] = 0;
+        for ( k = 1; k < 2*L+1; k ++ ) {
+            for ( int i = 0; i < SM; i ++ ) {
+                for ( int j = 0; j < SM; j ++ ) {
+                    cov[i*SM + j] += W * dY[k*SM + i] * dY[k*SM + j];
+                }
             }
         }
-        for ( int i = 3; i < SM; i ++ ) {
-            cov[i*SM + i] = 1e-5; // TODO : this is a rough estimate of IMU's accuracy
+
+        // Update mean as transform of mean
+        for ( int i = 0; i < SS; i++ ) {
+            x[i] = Y[i];
         }
 
         return 1;
     }
     int dead_reckon_apply(double* step, double *x, double *cov, double *x_new, double *cov_new ) {
         // Copy data in
         for ( int i = 0; i < SS; i ++ ) {
```

### Comparing `robotransforms-0.4.4/robotransforms/dead_reckon/base.h` & `robotransforms-0.5.0/robotransforms/dead_reckon/base.h`

 * *Files identical despite different names*

### Comparing `robotransforms-0.4.4/robotransforms/dead_reckon/dead_reckon.py` & `robotransforms-0.5.0/robotransforms/dead_reckon/dead_reckon.py`

 * *Files identical despite different names*

### Comparing `robotransforms-0.4.4/robotransforms/dead_reckon/dead_reckon_pure.py` & `robotransforms-0.5.0/robotransforms/dead_reckon/dead_reckon_pure.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import numpy as np
+import matplotlib.pyplot as plt
 
 from .. import euclidean as t
 # from ..euclidean import pure as t
 
 def DeadReckonStep(timestamp, dl, dr, Dq, vave, vdiff):
     return np.array([ timestamp, dl, dr, Dq[0], Dq[1], Dq[2], Dq[3], vave, vdiff ])
 
@@ -77,14 +78,15 @@
     P_z[1+SM][0+SM] = e[1] # cov_dldr
     P_z[1+SM][1+SM] = e[2] # var_dr
 
     # Generate sigma points along manifold from enclosing deviation vectors with the state
     L = SM+2
     Z = np.zeros((2*L+1,SS+2))
     Z[0] = z.copy()
+
     scaled_cov = P_z * L_PLUS_LAMBDA
     # Rows of the R matrix in A=R^TR function like a square root
     try:
         # Generate the deviation vectors along manifold
         dz = np.linalg.cholesky( scaled_cov ).T # NOTE, np returns L, not R, so we transpose it
     except Exception as e:
         v,w = np.linalg.eigh(scaled_cov)
@@ -96,49 +98,62 @@
         print("Evecs")
         for s in w:
             print(*[ "{: >9.5f}".format(_s) for _s in s])
         # print(scaled_cov)
         # print(v)
         # print(w.T)
         raise e
+
+
+    # extract the mean lrQ part
+    lrQ = z[:SS]
     for i in range(L):
-        # The first SS are gotten via composition
-        dlrQ = t.lrq2lrQ(dz[i][:SM])
-        Z[1 + i][:SS] = t.compose_lrQ(z[:SS], dlrQ)
-        Z[1 + i + L][:SS] = t.compose_lrQ(z[:SS], t.invert_lrQ(dlrQ))
-
-        # The last 2 are gotten via addition
-        Z[1 + i][SS:] = z[SS:] + dz[i][SM:]
-        Z[1 + i + L][SS:] = z[SS:] - dz[i][SM:]
+        Z[1 + i][:SS] = t.compose_lrQ(lrQ, t.lrrv2lrQ(dz[i,:SM]))
+        Z[1 + i][-2:] = Z[0,-2:] + dz[i,-2:]
+
+        Z[1 + i + L][:SS] = t.compose_lrQ(lrQ, t.lrrv2lrQ(-dz[i,:SM]))
+        Z[1 + i + L][-2:] = Z[0,-2:] - dz[i,-2:]
 
     # Transform to new vectors
     def T(_z):
         quat = _z[3:SS]
-        dx = dead_reckon_step( quat=_z[3:SS], dl=z[SS+0], dr=z[SS+1], vave=step[7], vdiff=step[8] )
-        # Only return offset, this is marginalizing out all the quat dependances
-        return _z[:3] + dx
+        dx = dead_reckon_step( quat=quat, dl=z[SS+0], dr=z[SS+1], vave=step[7], vdiff=step[8] )
+        nquat = t.compose_quat(quat,step[3:7])
+        return np.hstack([_z[:3] + dx, nquat]);
 
     Y = np.array([ T(_z) for _z in Z ])
 
-    M = len(Y[0])
     LAMBDA = L_PLUS_LAMBDA - L
     W0 = LAMBDA / L_PLUS_LAMBDA
     W = 1 / ( 2 * L_PLUS_LAMBDA )
 
-    y_bar = Y[0]*W0 + np.sum(Y[1:]*W,axis=0) # Note, this probably only works becuase we have neglected the quat -- not sure how to average on the manifold....
-    dY = Y - y_bar
+    ## Iteratively calculate the quaternion mean
+    y_bar = Y[0]
+    EPS = 1e-10
+    MAX = 100
+    i = 0
+    error = 1
+    while ( i < MAX and error > EPS ):
+        i += 1
+        y_bar_inv = t.invert_lrQ(y_bar)
+        dY = np.array([t.lrQ2lrrv(t.compose_lrQ(y_bar_inv, y)) for y in Y])
+        e = (dY[0]*W0 + np.sum(dY[1:]*W,axis=0))
+        error = np.linalg.norm(e) # TODO : should this be normalized?
+        y_bar = t.compose_lrQ(y_bar, t.lrrv2lrQ(e))
+
+
     cov = W0 * np.array([dY[0]]).T @ np.array([dY[0]]) # exterior product
     for k in range(1,len(dY)):
         cov = cov + W * np.array([dY[k]]).T @ np.array([dY[k]]) # exterior product
 
-    x_tilde = np.zeros(7)
-    x_tilde[:3] = T(z)                                                   # transform the mean
-    x_tilde[3:] = t.compose_quat(x_hat[3:],step[3:7])                    # accumulate the new difference along the manifold
-    P_tilde = np.eye(6)*1e-5                                             # Set imu variance value
-    P_tilde[:3,:3] = cov                                                 # write in deviation for translation
+
+
+    x_tilde = T(z)                                       # transform the mean
+    # x_tilde = np.hstack([y_pos_bar, q_bar])              # mean of transform
+    P_tilde = cov
 
     return x_tilde, P_tilde
 
 def dead_reckon(x_hat, P_hat, steps):
     for step in steps:
         x_hat, P_hat = dead_reckon_apply(x_hat, P_hat, step)
     return x_hat, P_hat
@@ -176,25 +191,25 @@
             return False, None, None
 
         steps_between_ts = []
 
         for step in self.reckon_steps:
             if (step[0] <= end_timestamp and step[0] >= start_timestamp):
                 steps_between_ts.append(step)
- 
+
         x_hat = start_x_hat.copy()
         P = start_P.copy()
 
         x_hat, P = dead_reckon(x_hat, P, steps_between_ts)
 
         return True, x_hat, P
 
 
     def reset_reference(self):
         # Full state: x,y,z, a,b,c,d
-        self.x_hat = np.array([0,0,0, 1,0,0,0]) 
+        self.x_hat = np.array([0,0,0, 1,0,0,0])
         # Manifold deviation: x,y,z (in terminal coordinates) b,c,d (relative to terminal coordinates)
         self.P = np.eye(6)*1e-8
 
     def push_step(self, timestamp=0, dl=0, dr=0, Dq=[1,0,0,0], vave=0, vdiff=0):
         self.reckon_steps.append(DeadReckonStep(timestamp, dl, dr, Dq, vave, vdiff))
         self.reckon_steps = self.reckon_steps[-self.max_size:]
```

### Comparing `robotransforms-0.4.4/robotransforms/dead_reckon/wrapper.cpp` & `robotransforms-0.5.0/robotransforms/dead_reckon/wrapper.cpp`

 * *Files identical despite different names*

### Comparing `robotransforms-0.4.4/robotransforms/euclidean/base.h` & `robotransforms-0.5.0/robotransforms/euclidean/base.h`

 * *Files 24% similar despite different names*

```diff
@@ -1,23 +1,33 @@
 
 namespace euclidean {
     // Conversion
     void convert_quat_to_redquat(double *q, double *rq);
     void convert_redquat_to_quat(double *rq, double *q);
+    void convert_quat_to_rotvec(double *q, double *rq);
+    void convert_rotvec_to_quat(double *rq, double *q);
     void convert_lrq_to_lrQ(double *lrq, double *lrQ);
     void convert_lrQ_to_lrq(double *lrQ, double *lrq);
+    void convert_lrrv_to_lrQ(double *lrrv, double *lrQ);
+    void convert_lrQ_to_lrrv(double *lrQ, double *lrrv);
     // Application
     void apply_quat(double *q, double *v, double *w);
     void apply_redquat(double *rq, double *v, double *w);
+    void apply_rotvec(double *rq, double *v, double *w);
     void apply_lrQ(double *lrQ, double *v, double *w);
     void apply_lrq(double *lrq, double *v, double *w);
+    void apply_lrrv(double *lrrv, double *v, double *w);
     // Inversion
     void invert_quat(double *q1, double *q2);
     void invert_redquat(double *rq1, double *rq2);
+    void invert_rotvec(double *rq1, double *rq2);
     void invert_lrQ(double *lrQ1, double *lrQ2);
     void invert_lrq(double *lrq1, double *lrq2);
+    void invert_lrrv(double *lrrv1, double *lrrv2);
     // Compositions
     void compose_quat(double *q1, double *q2, double *q3);
     void compose_redquat(double *rq1, double *rq2, double *rq3);
+    void compose_rotvec(double *rq1, double *rq2, double *rq3);
     void compose_lrQ(double *lrQ1, double *lrQ2, double *lrq3);
     void compose_lrq(double *lrq1, double *lrq2, double *lrq3);
+    void compose_lrrv(double *lrrv1, double *lrrv2, double *lrrv3);
 }
```

### Comparing `robotransforms-0.4.4/robotransforms/euclidean/euclidean.py` & `robotransforms-0.5.0/robotransforms/euclidean/euclidean.py`

 * *Files 19% similar despite different names*

```diff
@@ -5,21 +5,23 @@
 'sr' means shift then rotate, so that the "shift" (what I add to a vector to put it into the new coordinate reference frame) is in the initial coordinate reference frame
 'lr' means location then rotate, so that the "location" (where the terminal coordinate's origin is relative to the initial) is in the initial coordinate reference frame
 
 Types:
     euler   - [ yaw, pitch, roll ]
     quat    - [ re, i, j, k ]
     redquat - [ i, j, k ] (where re is assumed positive)
+    rotvec -  [ e1, e2, e3 ] = 2*arcsin(|[i,j,k]|)* hat([i,j,k])
     rotmat  - 3x3
     homo    - 4x4
     srq     - [ x, y, z, i, j, k]
     sre     - [ x, y, z, yaw, pitch, roll ]
     lrq     - [ x, y, z, i, j, k ]
     lre     - [ x, y, z, yaw, pitch, roll ]
     lrQ     - [ x, y, z, re, i, j, k ]
+    lrrv    - [ x, y, z, e1, e2, e3 ]
 """
 import numpy as np
 
 # Pull c-wrappers for faster usage
 import euclidean_wrapper as wrap
 
 def convert_quat_to_redquat(a):
@@ -30,86 +32,140 @@
 
 def convert_redquat_to_quat(a):
     out = np.zeros(4)
     wrap.convert_redquat_to_quat(a,out)
     return out
 redquat2quat = convert_redquat_to_quat
 
+def convert_quat_to_rotvec(a):
+    out = np.zeros(3)
+    wrap.convert_quat_to_rotvec(a,out)
+    return out
+quat2rotvec = convert_quat_to_rotvec
+
+def convert_rotvec_to_quat(a):
+    out = np.zeros(4)
+    wrap.convert_rotvec_to_quat(a,out)
+    return out
+rotvec2quat = convert_rotvec_to_quat
+
 def convert_lrq_to_lrQ(a):
     out = np.zeros(7)
     wrap.convert_lrq_to_lrQ(a,out)
     return out
 lrq2lrQ = convert_lrq_to_lrQ
 
+def convert_lrrv_to_lrQ(a):
+    out = np.zeros(7)
+    wrap.convert_lrrv_to_lrQ(a,out)
+    return out
+lrrv2lrQ = convert_lrrv_to_lrQ
+
 def convert_lrQ_to_lrq(a):
     out = np.zeros(6)
     wrap.convert_lrQ_to_lrq(a,out)
     return out
 lrQ2lrq = convert_lrQ_to_lrq
 
+def convert_lrQ_to_lrrv(a):
+    out = np.zeros(6)
+    wrap.convert_lrQ_to_lrrv(a,out)
+    return out
+lrQ2lrrv = convert_lrQ_to_lrrv
+
 def apply_quat(a,b):
     out = np.zeros(3)
     wrap.apply_quat(a,b,out)
     return out
 
 def apply_redquat(a,b):
     out = np.zeros(3)
     wrap.apply_redquat(a,b,out)
     return out
 
+def apply_rotvec(a,b):
+    out = np.zeros(3)
+    wrap.apply_rotvec(a,b,out)
+    return out
+
 def apply_lrQ(a,b):
     out = np.zeros(3)
     wrap.apply_lrQ(a,b,out)
     return out
 
 def apply_lrq(a,b):
     out = np.zeros(3)
     wrap.apply_lrq(a,b,out)
     return out
 
+def apply_lrrv(a,b):
+    out = np.zeros(3)
+    wrap.apply_lrrv(a,b,out)
+    return out
+
 def invert_quat(a):
     out = np.zeros(4)
     wrap.invert_quat(a,out)
     return out
 
 def invert_redquat(a):
     out = np.zeros(3)
     wrap.invert_redquat(a,out)
     return out
 
+def invert_rotvec(a):
+    out = np.zeros(3)
+    wrap.invert_rotvec(a,out)
+    return out
+
 def invert_lrQ(a):
     out = np.zeros(7)
     wrap.invert_lrQ(a,out)
     return out
 
 def invert_lrq(a):
     out = np.zeros(6)
     wrap.invert_lrq(a,out)
     return out
 
+def invert_lrrv(a):
+    out = np.zeros(6)
+    wrap.invert_lrrv(a,out)
+    return out
+
 def compose_quat(a,b):
     out = np.zeros(4)
     wrap.compose_quat(a,b,out)
     return out
 
 def compose_redquat(a,b):
     out = np.zeros(3)
     wrap.compose_redquat(a,b,out)
     return out
 
+def compose_rotvec(a,b):
+    out = np.zeros(3)
+    wrap.compose_rotvec(a,b,out)
+    return out
+
 def compose_lrQ(a,b):
     out = np.zeros(7)
     wrap.compose_lrQ(a,b,out)
     return out
 
 def compose_lrq(a,b):
     out = np.zeros(6)
     wrap.compose_lrq(a,b,out)
     return out
 
+def compose_lrrv(a,b):
+    out = np.zeros(6)
+    wrap.compose_lrrv(a,b,out)
+    return out
+
 # Keep all the "slow" functions, until we get around to wrapping them too
 
 # ---------------------
 #  Rotation conversion
 # ---------------------
 
 def euler2rotmat(euler):
```

### Comparing `robotransforms-0.4.4/robotransforms/euclidean/wrapper.cpp` & `robotransforms-0.5.0/robotransforms/euclidean/wrapper.cpp`

 * *Files 13% similar despite different names*

```diff
@@ -117,53 +117,73 @@
     RETURN_3_VECTORS(obj1, obj2, obj3) \
 }
 
 
 // Conversion
 APPLY_2_VECTORS(convert_quat_to_redquat, 4, 3)
 APPLY_2_VECTORS(convert_redquat_to_quat, 3, 4)
+APPLY_2_VECTORS(convert_quat_to_rotvec, 4, 3)
+APPLY_2_VECTORS(convert_rotvec_to_quat, 3, 4)
 APPLY_2_VECTORS(convert_lrq_to_lrQ, 6, 7)
 APPLY_2_VECTORS(convert_lrQ_to_lrq, 7, 6)
+APPLY_2_VECTORS(convert_lrrv_to_lrQ, 6, 7)
+APPLY_2_VECTORS(convert_lrQ_to_lrrv, 7, 6)
 // Application
 APPLY_3_VECTORS(apply_quat, 4, 3, 3)
 APPLY_3_VECTORS(apply_redquat, 3, 3, 3)
+APPLY_3_VECTORS(apply_rotvec, 3, 3, 3)
 APPLY_3_VECTORS(apply_lrQ, 7, 3, 3)
 APPLY_3_VECTORS(apply_lrq, 6, 3, 3)
+APPLY_3_VECTORS(apply_lrrv, 6, 3, 3)
 // Inversion
 APPLY_2_VECTORS(invert_quat, 4, 4)
 APPLY_2_VECTORS(invert_redquat, 3, 3)
+APPLY_2_VECTORS(invert_rotvec, 3, 3)
 APPLY_2_VECTORS(invert_lrQ, 7, 7)
 APPLY_2_VECTORS(invert_lrq, 6, 6)
+APPLY_2_VECTORS(invert_lrrv, 6, 6)
 // Composition
 APPLY_3_VECTORS(compose_quat, 4, 4, 4)
 APPLY_3_VECTORS(compose_redquat, 3, 3, 3)
+APPLY_3_VECTORS(compose_rotvec, 3, 3, 3)
 APPLY_3_VECTORS(compose_lrQ, 7, 7, 7)
 APPLY_3_VECTORS(compose_lrq, 6, 6, 6)
+APPLY_3_VECTORS(compose_lrrv, 6, 6, 6)
 
 /*
  * Globals
  */
 
 static PyMethodDef EuclideanMethods[] = {
     {"convert_quat_to_redquat", convert_quat_to_redquat, METH_VARARGS, "TODO"},
     {"convert_redquat_to_quat", convert_redquat_to_quat, METH_VARARGS, "TODO"},
+    {"convert_quat_to_rotvec", convert_quat_to_rotvec, METH_VARARGS, "TODO"},
+    {"convert_rotvec_to_quat", convert_rotvec_to_quat, METH_VARARGS, "TODO"},
     {"convert_lrq_to_lrQ", convert_lrq_to_lrQ, METH_VARARGS, "TODO"},
     {"convert_lrQ_to_lrq", convert_lrQ_to_lrq, METH_VARARGS, "TODO"},
+    {"convert_lrrv_to_lrQ", convert_lrrv_to_lrQ, METH_VARARGS, "TODO"},
+    {"convert_lrQ_to_lrrv", convert_lrQ_to_lrrv, METH_VARARGS, "TODO"},
     {"apply_quat", apply_quat, METH_VARARGS, "TODO"},
     {"apply_redquat", apply_redquat, METH_VARARGS, "TODO"},
+    {"apply_rotvec", apply_rotvec, METH_VARARGS, "TODO"},
     {"apply_lrQ", apply_lrQ, METH_VARARGS, "TODO"},
     {"apply_lrq", apply_lrq, METH_VARARGS, "TODO"},
+    {"apply_lrrv", apply_lrrv, METH_VARARGS, "TODO"},
     {"invert_quat", invert_quat, METH_VARARGS, "TODO"},
     {"invert_redquat", invert_redquat, METH_VARARGS, "TODO"},
+    {"invert_rotvec", invert_rotvec, METH_VARARGS, "TODO"},
     {"invert_lrQ", invert_lrQ, METH_VARARGS, "TODO"},
     {"invert_lrq", invert_lrq, METH_VARARGS, "TODO"},
+    {"invert_lrrv", invert_lrrv, METH_VARARGS, "TODO"},
     {"compose_quat", compose_quat, METH_VARARGS, "TODO"},
     {"compose_redquat", compose_redquat, METH_VARARGS, "TODO"},
+    {"compose_rotvec", compose_rotvec, METH_VARARGS, "TODO"},
     {"compose_lrQ", compose_lrQ, METH_VARARGS, "TODO"},
     {"compose_lrq", compose_lrq, METH_VARARGS, "TODO"},
+    {"compose_lrrv", compose_lrrv, METH_VARARGS, "TODO"},
     {NULL, NULL, 0, NULL}
 };
 
 static struct PyModuleDef EuclideanModule = {
     PyModuleDef_HEAD_INIT,
     "euclidean_wrapper",
     NULL, // TODO : should be documentation?
```

### Comparing `robotransforms-0.4.4/robotransforms/utils/base.cpp` & `robotransforms-0.5.0/robotransforms/utils/base.cpp`

 * *Files identical despite different names*

### Comparing `robotransforms-0.4.4/robotransforms/utils/utils.py` & `robotransforms-0.5.0/robotransforms/utils/utils.py`

 * *Files identical despite different names*

### Comparing `robotransforms-0.4.4/robotransforms/utils/utils_pure.py` & `robotransforms-0.5.0/robotransforms/utils/utils_pure.py`

 * *Files identical despite different names*

### Comparing `robotransforms-0.4.4/robotransforms/utils/wrapper.cpp` & `robotransforms-0.5.0/robotransforms/utils/wrapper.cpp`

 * *Files identical despite different names*

### Comparing `robotransforms-0.4.4/robotransforms.egg-info/PKG-INFO` & `robotransforms-0.5.0/robotransforms.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: robotransforms
-Version: 0.4.4
+Version: 0.5.0
 Summary: A transformation library for robot motion
 Home-page: https://github.com/Nova-Dynamics/transforms-python
 Author: Jonathan D. B. Van Schenck
 Author-email: jvschenck@novadynamics.com
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `robotransforms-0.4.4/robotransforms.egg-info/SOURCES.txt` & `robotransforms-0.5.0/robotransforms.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `robotransforms-0.4.4/setup.py` & `robotransforms-0.5.0/setup.py`

 * *Files identical despite different names*

