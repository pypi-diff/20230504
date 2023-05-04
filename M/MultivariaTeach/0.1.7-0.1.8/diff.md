# Comparing `tmp/MultivariaTeach-0.1.7.tar.gz` & `tmp/MultivariaTeach-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "MultivariaTeach-0.1.7.tar", last modified: Thu May  4 16:52:27 2023, max compression
+gzip compressed data, was "MultivariaTeach-0.1.8.tar", last modified: Thu May  4 17:00:36 2023, max compression
```

## Comparing `MultivariaTeach-0.1.7.tar` & `MultivariaTeach-0.1.8.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwx------   0 ben        (501) staff       (20)        0 2023-05-04 16:52:27.096936 MultivariaTeach-0.1.7/
--rw-------   0 ben        (501) staff       (20)      743 2023-04-25 22:03:04.000000 MultivariaTeach-0.1.7/LICENSE
-drwx------   0 ben        (501) staff       (20)        0 2023-05-04 16:52:27.095703 MultivariaTeach-0.1.7/MultivariaTeach.egg-info/
--rw-------   0 ben        (501) staff       (20)    25739 2023-05-04 16:52:27.000000 MultivariaTeach-0.1.7/MultivariaTeach.egg-info/PKG-INFO
--rw-------   0 ben        (501) staff       (20)      330 2023-05-04 16:52:27.000000 MultivariaTeach-0.1.7/MultivariaTeach.egg-info/SOURCES.txt
--rw-------   0 ben        (501) staff       (20)        1 2023-05-04 16:52:27.000000 MultivariaTeach-0.1.7/MultivariaTeach.egg-info/dependency_links.txt
--rw-------   0 ben        (501) staff       (20)       41 2023-05-04 16:52:27.000000 MultivariaTeach-0.1.7/MultivariaTeach.egg-info/requires.txt
--rw-------   0 ben        (501) staff       (20)       22 2023-05-04 16:52:27.000000 MultivariaTeach-0.1.7/MultivariaTeach.egg-info/top_level.txt
--rw-------   0 ben        (501) staff       (20)    25739 2023-05-04 16:52:27.096812 MultivariaTeach-0.1.7/PKG-INFO
--rw-------   0 ben        (501) staff       (20)    25071 2023-05-04 16:51:38.000000 MultivariaTeach-0.1.7/README.md
-drwx------   0 ben        (501) staff       (20)        0 2023-05-04 16:52:27.096042 MultivariaTeach-0.1.7/multivariateach/
--rw-------   0 ben        (501) staff       (20)       31 2023-05-02 20:33:56.000000 MultivariaTeach-0.1.7/multivariateach/__init__.py
--rw-------   0 ben        (501) staff       (20)    11161 2023-05-04 15:08:09.000000 MultivariaTeach-0.1.7/multivariateach/multivariateach.py
--rw-------   0 ben        (501) staff       (20)       38 2023-05-04 16:52:27.096975 MultivariaTeach-0.1.7/setup.cfg
--rw-------   0 ben        (501) staff       (20)      932 2023-05-04 15:11:19.000000 MultivariaTeach-0.1.7/setup.py
-drwx------   0 ben        (501) staff       (20)        0 2023-05-04 16:52:27.096345 MultivariaTeach-0.1.7/tests/
--rw-------   0 ben        (501) staff       (20)        0 2023-04-25 22:05:08.000000 MultivariaTeach-0.1.7/tests/__init__.py
--rw-------   0 ben        (501) staff       (20)     7016 2023-05-01 22:22:43.000000 MultivariaTeach-0.1.7/tests/test_multivariteach.py
+drwx------   0 ben        (501) staff       (20)        0 2023-05-04 17:00:36.226903 MultivariaTeach-0.1.8/
+-rw-------   0 ben        (501) staff       (20)      743 2023-04-25 22:03:04.000000 MultivariaTeach-0.1.8/LICENSE
+drwx------   0 ben        (501) staff       (20)        0 2023-05-04 17:00:36.225736 MultivariaTeach-0.1.8/MultivariaTeach.egg-info/
+-rw-------   0 ben        (501) staff       (20)    25742 2023-05-04 17:00:36.000000 MultivariaTeach-0.1.8/MultivariaTeach.egg-info/PKG-INFO
+-rw-------   0 ben        (501) staff       (20)      330 2023-05-04 17:00:36.000000 MultivariaTeach-0.1.8/MultivariaTeach.egg-info/SOURCES.txt
+-rw-------   0 ben        (501) staff       (20)        1 2023-05-04 17:00:36.000000 MultivariaTeach-0.1.8/MultivariaTeach.egg-info/dependency_links.txt
+-rw-------   0 ben        (501) staff       (20)       41 2023-05-04 17:00:36.000000 MultivariaTeach-0.1.8/MultivariaTeach.egg-info/requires.txt
+-rw-------   0 ben        (501) staff       (20)       22 2023-05-04 17:00:36.000000 MultivariaTeach-0.1.8/MultivariaTeach.egg-info/top_level.txt
+-rw-------   0 ben        (501) staff       (20)    25742 2023-05-04 17:00:36.226778 MultivariaTeach-0.1.8/PKG-INFO
+-rw-------   0 ben        (501) staff       (20)    25074 2023-05-04 16:57:58.000000 MultivariaTeach-0.1.8/README.md
+drwx------   0 ben        (501) staff       (20)        0 2023-05-04 17:00:36.226069 MultivariaTeach-0.1.8/multivariateach/
+-rw-------   0 ben        (501) staff       (20)       31 2023-05-02 20:33:56.000000 MultivariaTeach-0.1.8/multivariateach/__init__.py
+-rw-------   0 ben        (501) staff       (20)    11161 2023-05-04 15:08:09.000000 MultivariaTeach-0.1.8/multivariateach/multivariateach.py
+-rw-------   0 ben        (501) staff       (20)       38 2023-05-04 17:00:36.226938 MultivariaTeach-0.1.8/setup.cfg
+-rw-------   0 ben        (501) staff       (20)      932 2023-05-04 16:59:57.000000 MultivariaTeach-0.1.8/setup.py
+drwx------   0 ben        (501) staff       (20)        0 2023-05-04 17:00:36.226376 MultivariaTeach-0.1.8/tests/
+-rw-------   0 ben        (501) staff       (20)        0 2023-04-25 22:05:08.000000 MultivariaTeach-0.1.8/tests/__init__.py
+-rw-------   0 ben        (501) staff       (20)     7016 2023-05-01 22:22:43.000000 MultivariaTeach-0.1.8/tests/test_multivariteach.py
```

### Comparing `MultivariaTeach-0.1.7/LICENSE` & `MultivariaTeach-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `MultivariaTeach-0.1.7/MultivariaTeach.egg-info/PKG-INFO` & `MultivariaTeach-0.1.8/MultivariaTeach.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MultivariaTeach
-Version: 0.1.7
+Version: 0.1.8
 Summary: A collection of tools intended for students of multivariate analysis
 Home-page: https://github.com/Ben-Goren/MultivariaTeach
 Author: Ben Goren
 Author-email: bgoren@asu.edu
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Education
 Classifier: License :: OSI Approved :: ISC License (ISCL)
@@ -135,40 +135,44 @@
 X = mt.create_design_matrix(data, 'group')
 Y = mt.create_response_matrix(data, ['x1', 'x2', 'x3', 'x4'])
 C = mt.create_contrast_type_iii(X)
 M = np.eye(Y.shape[1])
 
 results = mt.run_manova(X, Y, C, M)
 
-print("beta_hat: ", results.beta_hat)
-print("E: ", results.E)
-print("B: ", results.B)
-print("H: ", results.H)
+print("beta_hat:\n", results.beta_hat)
+print("E:\n", results.E)
+print("B:\n", results.B)
+print("H:\n", results.H)
 print("wilks_lambda: ", results.wilks_lambda.statistic, results.wilks_lambda.F, results.wilks_lambda.df_n, results.wilks_lambda.df_d, results.wilks_lambda.p_value)
 print("pillais_trace: ", results.pillais_trace.statistic, results.pillais_trace.F, results.pillais_trace.df_n, results.pillais_trace.df_d, results.pillais_trace.p_value)
 print("hotelling_lawley_trace: ", results.hotelling_lawley_trace.statistic, results.hotelling_lawley_trace.F, results.hotelling_lawley_trace.df_n, results.hotelling_lawley_trace.df_d, results.hotelling_lawley_trace.p_value)
 print("roys_largest_root: ", results.roys_largest_root.statistic, results.roys_largest_root.F, results.roys_largest_root.df_n, results.roys_largest_root.df_d, results.roys_largest_root.p_value)
 ```
 
 This will create the following output:
 
 ```[text]
-beta_hat:  [[ 4.3825  2.293   2.8185  0.8995]
+beta_hat:
+ [[ 4.3825  2.293   2.8185  0.8995]
  [ 0.6235  1.135  -1.3565 -0.6535]
  [ 1.5535  0.477   1.4415  0.4265]
  [ 2.2055  0.681   2.7335  1.1265]]
-E:  [[38.9562 13.63   24.6246  5.645 ]
+E:
+ [[38.9562 13.63   24.6246  5.645 ]
  [13.63   16.962   8.1208  4.8084]
  [24.6246  8.1208 27.2226  6.2718]
  [ 5.645   4.8084  6.2718  6.1566]]
-B:  [[ 63.21213333 -19.95266667 165.2484      71.27933333]
+B:
+ [[ 63.21213333 -19.95266667 165.2484      71.27933333]
  [-19.95266667  11.34493333 -57.2396     -22.93266667]
  [165.2484     -57.2396     437.1028     186.774     ]
  [ 71.27933333 -22.93266667 186.774       80.41333333]]
-H:  [[ 63.21213333 -19.95266667 165.2484      71.27933333]
+H:
+ [[ 63.21213333 -19.95266667 165.2484      71.27933333]
  [-19.95266667  11.34493333 -57.2396     -22.93266667]
  [165.2484     -57.2396     437.1028     186.774     ]
  [ 71.27933333 -22.93266667 186.774       80.41333333]]
 wilks_lambda:  0.023438630650877965 199.14534354008606 8 288 1.3650058325882981e-112
 pillais_trace:  1.191898825041458 53.466488784612224 8.0 290.0 9.74216271945252e-53
 hotelling_lawley_trace:  32.4773202409019 580.5320993061215 8.0 286.0 6.436176201217028e-172
 roys_largest_root:  32.19192919827884 1166.957433437608 4 145 3.42202725324015e-19
@@ -373,15 +377,15 @@
 
 First, as we will be directly computing the $p$-value towards the end, be sure to load the scientific computing library at the top of your script:
 
 ```python
 import scipy
 ```
 
-Assuming you have immediately previously performed the above calculation of $\epsilon$, he univariate test may be performed with:
+Assuming you have immediately previously performed the above calculation of $\epsilon$, the univariate test may be performed with:
 
 ```python
 Y_1 = Y[:, 0].reshape(-1, 1) # Note that the first column is index zero.
 univariate_1 = mt.run_manova(X, Y, C, M)
 corrected_wilks_1 = univariate_1.wilks_lambda.statistic * epsilon
 corrected_df_n_1 = univariate_1.wilks_lambda.df_n * epsilon
 corrected_df_d_1 = univariate_1.wilks_lambda.df_d * epsilon
@@ -432,16 +436,14 @@
 S_pooled:
  [[ 1.39956621 -0.08661187  2.601       1.05375799]
  [-0.08661187  0.38776621 -0.67286027 -0.24827763]
  [ 2.601      -0.67286027  6.36062192  2.64446301]
  [ 1.05375799 -0.24827763  2.64446301  1.1858895 ]]
 ```
 
-
-
 #### Individual test statistic calculations
 
 For each of the four main MANOVA test statistics, you can directly provide the $\mathbf{E}$ and $\mathbf{H}$ matrices in addition to three or four of the following (depending on the statistic):
 
 * n, the number of observations (rows of data);
 * p, the number of variables (columns in $\mathbf{Y}$)
 * g, the number of groups (equal to one less than the number of columns of $\mathbf{X}$)
```

### Comparing `MultivariaTeach-0.1.7/PKG-INFO` & `MultivariaTeach-0.1.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MultivariaTeach
-Version: 0.1.7
+Version: 0.1.8
 Summary: A collection of tools intended for students of multivariate analysis
 Home-page: https://github.com/Ben-Goren/MultivariaTeach
 Author: Ben Goren
 Author-email: bgoren@asu.edu
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Education
 Classifier: License :: OSI Approved :: ISC License (ISCL)
@@ -135,40 +135,44 @@
 X = mt.create_design_matrix(data, 'group')
 Y = mt.create_response_matrix(data, ['x1', 'x2', 'x3', 'x4'])
 C = mt.create_contrast_type_iii(X)
 M = np.eye(Y.shape[1])
 
 results = mt.run_manova(X, Y, C, M)
 
-print("beta_hat: ", results.beta_hat)
-print("E: ", results.E)
-print("B: ", results.B)
-print("H: ", results.H)
+print("beta_hat:\n", results.beta_hat)
+print("E:\n", results.E)
+print("B:\n", results.B)
+print("H:\n", results.H)
 print("wilks_lambda: ", results.wilks_lambda.statistic, results.wilks_lambda.F, results.wilks_lambda.df_n, results.wilks_lambda.df_d, results.wilks_lambda.p_value)
 print("pillais_trace: ", results.pillais_trace.statistic, results.pillais_trace.F, results.pillais_trace.df_n, results.pillais_trace.df_d, results.pillais_trace.p_value)
 print("hotelling_lawley_trace: ", results.hotelling_lawley_trace.statistic, results.hotelling_lawley_trace.F, results.hotelling_lawley_trace.df_n, results.hotelling_lawley_trace.df_d, results.hotelling_lawley_trace.p_value)
 print("roys_largest_root: ", results.roys_largest_root.statistic, results.roys_largest_root.F, results.roys_largest_root.df_n, results.roys_largest_root.df_d, results.roys_largest_root.p_value)
 ```
 
 This will create the following output:
 
 ```[text]
-beta_hat:  [[ 4.3825  2.293   2.8185  0.8995]
+beta_hat:
+ [[ 4.3825  2.293   2.8185  0.8995]
  [ 0.6235  1.135  -1.3565 -0.6535]
  [ 1.5535  0.477   1.4415  0.4265]
  [ 2.2055  0.681   2.7335  1.1265]]
-E:  [[38.9562 13.63   24.6246  5.645 ]
+E:
+ [[38.9562 13.63   24.6246  5.645 ]
  [13.63   16.962   8.1208  4.8084]
  [24.6246  8.1208 27.2226  6.2718]
  [ 5.645   4.8084  6.2718  6.1566]]
-B:  [[ 63.21213333 -19.95266667 165.2484      71.27933333]
+B:
+ [[ 63.21213333 -19.95266667 165.2484      71.27933333]
  [-19.95266667  11.34493333 -57.2396     -22.93266667]
  [165.2484     -57.2396     437.1028     186.774     ]
  [ 71.27933333 -22.93266667 186.774       80.41333333]]
-H:  [[ 63.21213333 -19.95266667 165.2484      71.27933333]
+H:
+ [[ 63.21213333 -19.95266667 165.2484      71.27933333]
  [-19.95266667  11.34493333 -57.2396     -22.93266667]
  [165.2484     -57.2396     437.1028     186.774     ]
  [ 71.27933333 -22.93266667 186.774       80.41333333]]
 wilks_lambda:  0.023438630650877965 199.14534354008606 8 288 1.3650058325882981e-112
 pillais_trace:  1.191898825041458 53.466488784612224 8.0 290.0 9.74216271945252e-53
 hotelling_lawley_trace:  32.4773202409019 580.5320993061215 8.0 286.0 6.436176201217028e-172
 roys_largest_root:  32.19192919827884 1166.957433437608 4 145 3.42202725324015e-19
@@ -373,15 +377,15 @@
 
 First, as we will be directly computing the $p$-value towards the end, be sure to load the scientific computing library at the top of your script:
 
 ```python
 import scipy
 ```
 
-Assuming you have immediately previously performed the above calculation of $\epsilon$, he univariate test may be performed with:
+Assuming you have immediately previously performed the above calculation of $\epsilon$, the univariate test may be performed with:
 
 ```python
 Y_1 = Y[:, 0].reshape(-1, 1) # Note that the first column is index zero.
 univariate_1 = mt.run_manova(X, Y, C, M)
 corrected_wilks_1 = univariate_1.wilks_lambda.statistic * epsilon
 corrected_df_n_1 = univariate_1.wilks_lambda.df_n * epsilon
 corrected_df_d_1 = univariate_1.wilks_lambda.df_d * epsilon
@@ -432,16 +436,14 @@
 S_pooled:
  [[ 1.39956621 -0.08661187  2.601       1.05375799]
  [-0.08661187  0.38776621 -0.67286027 -0.24827763]
  [ 2.601      -0.67286027  6.36062192  2.64446301]
  [ 1.05375799 -0.24827763  2.64446301  1.1858895 ]]
 ```
 
-
-
 #### Individual test statistic calculations
 
 For each of the four main MANOVA test statistics, you can directly provide the $\mathbf{E}$ and $\mathbf{H}$ matrices in addition to three or four of the following (depending on the statistic):
 
 * n, the number of observations (rows of data);
 * p, the number of variables (columns in $\mathbf{Y}$)
 * g, the number of groups (equal to one less than the number of columns of $\mathbf{X}$)
```

### Comparing `MultivariaTeach-0.1.7/README.md` & `MultivariaTeach-0.1.8/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -117,40 +117,44 @@
 X = mt.create_design_matrix(data, 'group')
 Y = mt.create_response_matrix(data, ['x1', 'x2', 'x3', 'x4'])
 C = mt.create_contrast_type_iii(X)
 M = np.eye(Y.shape[1])
 
 results = mt.run_manova(X, Y, C, M)
 
-print("beta_hat: ", results.beta_hat)
-print("E: ", results.E)
-print("B: ", results.B)
-print("H: ", results.H)
+print("beta_hat:\n", results.beta_hat)
+print("E:\n", results.E)
+print("B:\n", results.B)
+print("H:\n", results.H)
 print("wilks_lambda: ", results.wilks_lambda.statistic, results.wilks_lambda.F, results.wilks_lambda.df_n, results.wilks_lambda.df_d, results.wilks_lambda.p_value)
 print("pillais_trace: ", results.pillais_trace.statistic, results.pillais_trace.F, results.pillais_trace.df_n, results.pillais_trace.df_d, results.pillais_trace.p_value)
 print("hotelling_lawley_trace: ", results.hotelling_lawley_trace.statistic, results.hotelling_lawley_trace.F, results.hotelling_lawley_trace.df_n, results.hotelling_lawley_trace.df_d, results.hotelling_lawley_trace.p_value)
 print("roys_largest_root: ", results.roys_largest_root.statistic, results.roys_largest_root.F, results.roys_largest_root.df_n, results.roys_largest_root.df_d, results.roys_largest_root.p_value)
 ```
 
 This will create the following output:
 
 ```[text]
-beta_hat:  [[ 4.3825  2.293   2.8185  0.8995]
+beta_hat:
+ [[ 4.3825  2.293   2.8185  0.8995]
  [ 0.6235  1.135  -1.3565 -0.6535]
  [ 1.5535  0.477   1.4415  0.4265]
  [ 2.2055  0.681   2.7335  1.1265]]
-E:  [[38.9562 13.63   24.6246  5.645 ]
+E:
+ [[38.9562 13.63   24.6246  5.645 ]
  [13.63   16.962   8.1208  4.8084]
  [24.6246  8.1208 27.2226  6.2718]
  [ 5.645   4.8084  6.2718  6.1566]]
-B:  [[ 63.21213333 -19.95266667 165.2484      71.27933333]
+B:
+ [[ 63.21213333 -19.95266667 165.2484      71.27933333]
  [-19.95266667  11.34493333 -57.2396     -22.93266667]
  [165.2484     -57.2396     437.1028     186.774     ]
  [ 71.27933333 -22.93266667 186.774       80.41333333]]
-H:  [[ 63.21213333 -19.95266667 165.2484      71.27933333]
+H:
+ [[ 63.21213333 -19.95266667 165.2484      71.27933333]
  [-19.95266667  11.34493333 -57.2396     -22.93266667]
  [165.2484     -57.2396     437.1028     186.774     ]
  [ 71.27933333 -22.93266667 186.774       80.41333333]]
 wilks_lambda:  0.023438630650877965 199.14534354008606 8 288 1.3650058325882981e-112
 pillais_trace:  1.191898825041458 53.466488784612224 8.0 290.0 9.74216271945252e-53
 hotelling_lawley_trace:  32.4773202409019 580.5320993061215 8.0 286.0 6.436176201217028e-172
 roys_largest_root:  32.19192919827884 1166.957433437608 4 145 3.42202725324015e-19
@@ -355,15 +359,15 @@
 
 First, as we will be directly computing the $p$-value towards the end, be sure to load the scientific computing library at the top of your script:
 
 ```python
 import scipy
 ```
 
-Assuming you have immediately previously performed the above calculation of $\epsilon$, he univariate test may be performed with:
+Assuming you have immediately previously performed the above calculation of $\epsilon$, the univariate test may be performed with:
 
 ```python
 Y_1 = Y[:, 0].reshape(-1, 1) # Note that the first column is index zero.
 univariate_1 = mt.run_manova(X, Y, C, M)
 corrected_wilks_1 = univariate_1.wilks_lambda.statistic * epsilon
 corrected_df_n_1 = univariate_1.wilks_lambda.df_n * epsilon
 corrected_df_d_1 = univariate_1.wilks_lambda.df_d * epsilon
@@ -414,16 +418,14 @@
 S_pooled:
  [[ 1.39956621 -0.08661187  2.601       1.05375799]
  [-0.08661187  0.38776621 -0.67286027 -0.24827763]
  [ 2.601      -0.67286027  6.36062192  2.64446301]
  [ 1.05375799 -0.24827763  2.64446301  1.1858895 ]]
 ```
 
-
-
 #### Individual test statistic calculations
 
 For each of the four main MANOVA test statistics, you can directly provide the $\mathbf{E}$ and $\mathbf{H}$ matrices in addition to three or four of the following (depending on the statistic):
 
 * n, the number of observations (rows of data);
 * p, the number of variables (columns in $\mathbf{Y}$)
 * g, the number of groups (equal to one less than the number of columns of $\mathbf{X}$)
```

### Comparing `MultivariaTeach-0.1.7/multivariateach/multivariateach.py` & `MultivariaTeach-0.1.8/multivariateach/multivariateach.py`

 * *Files identical despite different names*

### Comparing `MultivariaTeach-0.1.7/setup.py` & `MultivariaTeach-0.1.8/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="MultivariaTeach",
-    version="0.1.7",
+    version="0.1.8",
     description="A collection of tools intended for students of multivariate analysis",
     long_description=open("README.md", "r").read(),
     long_description_content_type="text/markdown",
     author="Ben Goren",
     author_email="bgoren@asu.edu",
     url="https://github.com/Ben-Goren/MultivariaTeach",
     packages=find_packages(),
```

### Comparing `MultivariaTeach-0.1.7/tests/test_multivariteach.py` & `MultivariaTeach-0.1.8/tests/test_multivariteach.py`

 * *Files identical despite different names*

